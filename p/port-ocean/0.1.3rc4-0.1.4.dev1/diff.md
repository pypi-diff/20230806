# Comparing `tmp/port_ocean-0.1.3rc4.tar.gz` & `tmp/port_ocean-0.1.4.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "port_ocean-0.1.3rc4.tar", max compression
+gzip compressed data, was "port_ocean-0.1.4.dev1.tar", max compression
```

## Comparing `port_ocean-0.1.3rc4.tar` & `port_ocean-0.1.4.dev1.tar`

### file list

```diff
@@ -1,99 +1,101 @@
--rw-r--r--   0        0        0    11357 2023-07-30 14:48:42.414159 port_ocean-0.1.3rc4/LICENSE
--rw-r--r--   0        0        0     4639 2023-07-30 14:48:42.414159 port_ocean-0.1.3rc4/README.md
--rw-r--r--   0        0        0      270 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/__init__.py
--rw-r--r--   0        0        0      328 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/cli/__init__.py
--rw-r--r--   0        0        0       57 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/cli/cli.py
--rw-r--r--   0        0        0      278 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/cli/commands/__init__.py
--rw-r--r--   0        0        0     1134 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/cli/commands/list_integrations.py
--rw-r--r--   0        0        0     1057 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/cli/commands/main.py
--rw-r--r--   0        0        0     1710 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/cli/commands/new.py
--rw-r--r--   0        0        0     2306 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/cli/commands/pull.py
--rw-r--r--   0        0        0     1534 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/cli/commands/sail.py
--rw-r--r--   0        0        0      536 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/cli/commands/version.py
--rw-r--r--   0        0        0      429 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/cli/cookiecutter/cookiecutter.json
--rw-r--r--   0        0        0       42 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.dockerignore
--rw-r--r--   0        0        0     2698 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.gitignore
--rw-r--r--   0        0        0       12 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.port/resources/.gitignore
--rw-r--r--   0        0        0      388 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.port/spec.yaml
--rw-r--r--   0        0        0      292 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/CHANGELOG.md
--rw-r--r--   0        0        0      449 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Dockerfile
--rw-r--r--   0        0        0     1680 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Makefile
--rw-r--r--   0        0        0      655 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/README.md
--rw-r--r--   0        0        0       12 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/changelog/.gitignore
--rw-r--r--   0        0        0      898 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/config.yaml
--rw-r--r--   0        0        0       65 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/debug.py
--rw-r--r--   0        0        0     1669 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/main.py
--rw-r--r--   0        0        0       46 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/poetry.toml
--rw-r--r--   0        0        0     1920 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/tests/__init__.py
--rw-r--r--   0        0        0       54 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/cli/utils.py
--rw-r--r--   0        0        0        0 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/clients/__init__.py
--rw-r--r--   0        0        0        0 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/clients/port/__init__.py
--rw-r--r--   0        0        0     2563 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/clients/port/authentication.py
--rw-r--r--   0        0        0     2309 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/clients/port/client.py
--rw-r--r--   0        0        0        0 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/clients/port/mixins/__init__.py
--rw-r--r--   0        0        0     2928 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/clients/port/mixins/blueprints.py
--rw-r--r--   0        0        0     5623 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/clients/port/mixins/entities.py
--rw-r--r--   0        0        0     3909 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/clients/port/mixins/integrations.py
--rw-r--r--   0        0        0      593 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/clients/port/types.py
--rw-r--r--   0        0        0      781 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/clients/port/utils.py
--rw-r--r--   0        0        0        0 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/config/__init__.py
--rw-r--r--   0        0        0     4019 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/config/base.py
--rw-r--r--   0        0        0     1816 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/config/dynamic.py
--rw-r--r--   0        0        0     1231 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/config/settings.py
--rw-r--r--   0        0        0        0 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/consumers/__init__.py
--rw-r--r--   0        0        0      125 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/consumers/base_consumer.py
--rw-r--r--   0        0        0     4147 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/consumers/kafka_consumer.py
--rw-r--r--   0        0        0        0 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/context/__init__.py
--rw-r--r--   0        0        0     3201 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/context/event.py
--rw-r--r--   0        0        0     4283 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/context/ocean.py
--rw-r--r--   0        0        0        0 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/core/__init__.py
--rw-r--r--   0        0        0      219 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/core/base.py
--rw-r--r--   0        0        0      607 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/core/event_listener/__init__.py
--rw-r--r--   0        0        0      580 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/core/event_listener/base.py
--rw-r--r--   0        0        0     2555 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/core/event_listener/factory.py
--rw-r--r--   0        0        0     1165 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/core/event_listener/http/event_listener.py
--rw-r--r--   0        0        0     3349 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/core/event_listener/kafka/event_listener.py
--rw-r--r--   0        0        0     1867 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/core/event_listener/polling/event_listener.py
--rw-r--r--   0        0        0     2799 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/core/event_listener/polling/utils.py
--rw-r--r--   0        0        0      716 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/core/handlers/__init__.py
--rw-r--r--   0        0        0        0 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/core/handlers/entities_state_applier/__init__.py
--rw-r--r--   0        0        0      869 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/core/handlers/entities_state_applier/base.py
--rw-r--r--   0        0        0        0 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/core/handlers/entities_state_applier/port/__init__.py
--rw-r--r--   0        0        0     7977 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/core/handlers/entities_state_applier/port/applier.py
--rw-r--r--   0        0        0     1339 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/core/handlers/entities_state_applier/port/get_related_entities.py
--rw-r--r--   0        0        0      988 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/core/handlers/entities_state_applier/port/order_by_entities_dependencies.py
--rw-r--r--   0        0        0     1392 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/core/handlers/entities_state_applier/port/validate_entity_relations.py
--rw-r--r--   0        0        0        0 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/core/handlers/entity_processor/__init__.py
--rw-r--r--   0        0        0      955 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/core/handlers/entity_processor/base.py
--rw-r--r--   0        0        0     2685 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/core/handlers/entity_processor/jq_entity_processor.py
--rw-r--r--   0        0        0        0 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/core/handlers/port_app_config/__init__.py
--rw-r--r--   0        0        0      396 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/core/handlers/port_app_config/api.py
--rw-r--r--   0        0        0      651 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/core/handlers/port_app_config/base.py
--rw-r--r--   0        0        0     1810 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/core/handlers/port_app_config/models.py
--rw-r--r--   0        0        0        0 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/core/integrations/__init__.py
--rw-r--r--   0        0        0     1912 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/core/integrations/base.py
--rw-r--r--   0        0        0        0 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/core/integrations/mixins/__init__.py
--rw-r--r--   0        0        0      698 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/core/integrations/mixins/events.py
--rw-r--r--   0        0        0     2569 2023-07-30 14:48:42.426159 port_ocean-0.1.3rc4/port_ocean/core/integrations/mixins/handler.py
--rw-r--r--   0        0        0    11843 2023-07-30 14:48:42.430159 port_ocean-0.1.3rc4/port_ocean/core/integrations/mixins/sync.py
--rw-r--r--   0        0        0     1683 2023-07-30 14:48:42.430159 port_ocean-0.1.3rc4/port_ocean/core/integrations/mixins/utils.py
--rw-r--r--   0        0        0     1368 2023-07-30 14:48:42.430159 port_ocean-0.1.3rc4/port_ocean/core/models.py
--rw-r--r--   0        0        0      781 2023-07-30 14:48:42.430159 port_ocean-0.1.3rc4/port_ocean/core/ocean_types.py
--rw-r--r--   0        0        0     1957 2023-07-30 14:48:42.430159 port_ocean-0.1.3rc4/port_ocean/core/utils.py
--rw-r--r--   0        0        0        0 2023-07-30 14:48:42.430159 port_ocean-0.1.3rc4/port_ocean/exceptions/__init__.py
--rw-r--r--   0        0        0      426 2023-07-30 14:48:42.430159 port_ocean-0.1.3rc4/port_ocean/exceptions/api.py
--rw-r--r--   0        0        0       46 2023-07-30 14:48:42.430159 port_ocean-0.1.3rc4/port_ocean/exceptions/base.py
--rw-r--r--   0        0        0      180 2023-07-30 14:48:42.430159 port_ocean-0.1.3rc4/port_ocean/exceptions/clients.py
--rw-r--r--   0        0        0      235 2023-07-30 14:48:42.430159 port_ocean-0.1.3rc4/port_ocean/exceptions/context.py
--rw-r--r--   0        0        0      532 2023-07-30 14:48:42.430159 port_ocean-0.1.3rc4/port_ocean/exceptions/core.py
--rw-r--r--   0        0        0      407 2023-07-30 14:48:42.430159 port_ocean-0.1.3rc4/port_ocean/exceptions/port_defaults.py
--rw-r--r--   0        0        0      551 2023-07-30 14:48:42.430159 port_ocean-0.1.3rc4/port_ocean/logger_setup.py
--rw-r--r--   0        0        0     2475 2023-07-30 14:48:42.430159 port_ocean-0.1.3rc4/port_ocean/middlewares.py
--rw-r--r--   0        0        0     2263 2023-07-30 14:48:42.430159 port_ocean-0.1.3rc4/port_ocean/ocean.py
--rw-r--r--   0        0        0     7161 2023-07-30 14:48:42.430159 port_ocean-0.1.3rc4/port_ocean/port_defaults.py
--rw-r--r--   0        0        0        0 2023-07-30 14:48:42.430159 port_ocean-0.1.3rc4/port_ocean/py.typed
--rw-r--r--   0        0        0     2834 2023-07-30 14:48:42.430159 port_ocean-0.1.3rc4/port_ocean/run.py
--rw-r--r--   0        0        0     1007 2023-07-30 14:48:42.430159 port_ocean-0.1.3rc4/port_ocean/utils.py
--rw-r--r--   0        0        0     3461 2023-07-30 14:48:42.430159 port_ocean-0.1.3rc4/pyproject.toml
--rw-r--r--   0        0        0     6359 1970-01-01 00:00:00.000000 port_ocean-0.1.3rc4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-08-06 15:48:03.368126 port_ocean-0.1.4.dev1/LICENSE
+-rw-r--r--   0        0        0     4639 2023-08-06 15:48:03.368126 port_ocean-0.1.4.dev1/README.md
+-rw-r--r--   0        0        0      270 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/__init__.py
+-rw-r--r--   0        0        0      328 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/cli/__init__.py
+-rw-r--r--   0        0        0       57 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/cli/cli.py
+-rw-r--r--   0        0        0      278 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/cli/commands/__init__.py
+-rw-r--r--   0        0        0     1134 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/cli/commands/list_integrations.py
+-rw-r--r--   0        0        0     1057 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/cli/commands/main.py
+-rw-r--r--   0        0        0     1816 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/cli/commands/new.py
+-rw-r--r--   0        0        0     2306 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/cli/commands/pull.py
+-rw-r--r--   0        0        0     1534 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/cli/commands/sail.py
+-rw-r--r--   0        0        0      536 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/cli/commands/version.py
+-rw-r--r--   0        0        0      429 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/cli/cookiecutter/cookiecutter.json
+-rw-r--r--   0        0        0       42 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.dockerignore
+-rw-r--r--   0        0        0     2698 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.gitignore
+-rw-r--r--   0        0        0       12 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.port/resources/.gitignore
+-rw-r--r--   0        0        0      388 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.port/spec.yaml
+-rw-r--r--   0        0        0      292 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/CHANGELOG.md
+-rw-r--r--   0        0        0      449 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Dockerfile
+-rw-r--r--   0        0        0     1680 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Makefile
+-rw-r--r--   0        0        0      655 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/README.md
+-rw-r--r--   0        0        0       12 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/changelog/.gitignore
+-rw-r--r--   0        0        0      898 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/config.yaml
+-rw-r--r--   0        0        0       65 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/debug.py
+-rw-r--r--   0        0        0     1669 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/main.py
+-rw-r--r--   0        0        0       46 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/poetry.toml
+-rw-r--r--   0        0        0     1941 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/tests/__init__.py
+-rw-r--r--   0        0        0       54 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/cli/utils.py
+-rw-r--r--   0        0        0        0 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/clients/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/clients/port/__init__.py
+-rw-r--r--   0        0        0     2563 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/clients/port/authentication.py
+-rw-r--r--   0        0        0     2309 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/clients/port/client.py
+-rw-r--r--   0        0        0        0 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/clients/port/mixins/__init__.py
+-rw-r--r--   0        0        0     2928 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/clients/port/mixins/blueprints.py
+-rw-r--r--   0        0        0     5623 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/clients/port/mixins/entities.py
+-rw-r--r--   0        0        0     3909 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/clients/port/mixins/integrations.py
+-rw-r--r--   0        0        0      593 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/clients/port/types.py
+-rw-r--r--   0        0        0      781 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/clients/port/utils.py
+-rw-r--r--   0        0        0        0 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/config/__init__.py
+-rw-r--r--   0        0        0     4011 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/config/base.py
+-rw-r--r--   0        0        0     1816 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/config/dynamic.py
+-rw-r--r--   0        0        0     1231 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/config/settings.py
+-rw-r--r--   0        0        0        0 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/consumers/__init__.py
+-rw-r--r--   0        0        0      125 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/consumers/base_consumer.py
+-rw-r--r--   0        0        0     4147 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/consumers/kafka_consumer.py
+-rw-r--r--   0        0        0        0 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/context/__init__.py
+-rw-r--r--   0        0        0     3201 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/context/event.py
+-rw-r--r--   0        0        0     4283 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/context/ocean.py
+-rw-r--r--   0        0        0        0 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/core/__init__.py
+-rw-r--r--   0        0        0      219 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/core/base.py
+-rw-r--r--   0        0        0      607 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/core/event_listener/__init__.py
+-rw-r--r--   0        0        0      891 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/core/event_listener/base.py
+-rw-r--r--   0        0        0     3474 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/core/event_listener/factory.py
+-rw-r--r--   0        0        0        0 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/core/event_listener/http/__init__.py
+-rw-r--r--   0        0        0     2511 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/core/event_listener/http/event_listener.py
+-rw-r--r--   0        0        0        0 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/core/event_listener/kafka/__init__.py
+-rw-r--r--   0        0        0     6351 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/core/event_listener/kafka/event_listener.py
+-rw-r--r--   0        0        0     3264 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/core/event_listener/polling/event_listener.py
+-rw-r--r--   0        0        0     2799 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/core/event_listener/polling/utils.py
+-rw-r--r--   0        0        0      716 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/core/handlers/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/core/handlers/entities_state_applier/__init__.py
+-rw-r--r--   0        0        0      869 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/core/handlers/entities_state_applier/base.py
+-rw-r--r--   0        0        0        0 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/core/handlers/entities_state_applier/port/__init__.py
+-rw-r--r--   0        0        0     7977 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/core/handlers/entities_state_applier/port/applier.py
+-rw-r--r--   0        0        0     1751 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/core/handlers/entities_state_applier/port/get_related_entities.py
+-rw-r--r--   0        0        0      988 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/core/handlers/entities_state_applier/port/order_by_entities_dependencies.py
+-rw-r--r--   0        0        0     1392 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/core/handlers/entities_state_applier/port/validate_entity_relations.py
+-rw-r--r--   0        0        0        0 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/core/handlers/entity_processor/__init__.py
+-rw-r--r--   0        0        0      955 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/core/handlers/entity_processor/base.py
+-rw-r--r--   0        0        0     2685 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/core/handlers/entity_processor/jq_entity_processor.py
+-rw-r--r--   0        0        0        0 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/core/handlers/port_app_config/__init__.py
+-rw-r--r--   0        0        0      396 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/core/handlers/port_app_config/api.py
+-rw-r--r--   0        0        0      651 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/core/handlers/port_app_config/base.py
+-rw-r--r--   0        0        0     1810 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/core/handlers/port_app_config/models.py
+-rw-r--r--   0        0        0        0 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/core/integrations/__init__.py
+-rw-r--r--   0        0        0     3162 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/core/integrations/base.py
+-rw-r--r--   0        0        0        0 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/core/integrations/mixins/__init__.py
+-rw-r--r--   0        0        0      698 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/core/integrations/mixins/events.py
+-rw-r--r--   0        0        0     2569 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/core/integrations/mixins/handler.py
+-rw-r--r--   0        0        0    11843 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/core/integrations/mixins/sync.py
+-rw-r--r--   0        0        0     1747 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/core/integrations/mixins/utils.py
+-rw-r--r--   0        0        0      909 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/core/models.py
+-rw-r--r--   0        0        0      781 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/core/ocean_types.py
+-rw-r--r--   0        0        0     1957 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/core/utils.py
+-rw-r--r--   0        0        0        0 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/exceptions/__init__.py
+-rw-r--r--   0        0        0      426 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/exceptions/api.py
+-rw-r--r--   0        0        0       46 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/exceptions/base.py
+-rw-r--r--   0        0        0      180 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/exceptions/clients.py
+-rw-r--r--   0        0        0      235 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/exceptions/context.py
+-rw-r--r--   0        0        0      532 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/exceptions/core.py
+-rw-r--r--   0        0        0      407 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/exceptions/port_defaults.py
+-rw-r--r--   0        0        0     1107 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/logger_setup.py
+-rw-r--r--   0        0        0     2475 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/middlewares.py
+-rw-r--r--   0        0        0     2263 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/ocean.py
+-rw-r--r--   0        0        0     7161 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/port_defaults.py
+-rw-r--r--   0        0        0        0 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/py.typed
+-rw-r--r--   0        0        0     2834 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/run.py
+-rw-r--r--   0        0        0     1007 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/utils.py
+-rw-r--r--   0        0        0     3462 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/pyproject.toml
+-rw-r--r--   0        0        0     6361 1970-01-01 00:00:00.000000 port_ocean-0.1.4.dev1/PKG-INFO
```

### Comparing `port_ocean-0.1.3rc4/LICENSE` & `port_ocean-0.1.4.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.3rc4/README.md` & `port_ocean-0.1.4.dev1/README.md`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.3rc4/port_ocean/cli/commands/list_integrations.py` & `port_ocean-0.1.4.dev1/port_ocean/cli/commands/list_integrations.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.3rc4/port_ocean/cli/commands/main.py` & `port_ocean-0.1.4.dev1/port_ocean/cli/commands/main.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.3rc4/port_ocean/cli/commands/new.py` & `port_ocean-0.1.4.dev1/port_ocean/cli/commands/new.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 
 import click
 from cookiecutter.main import cookiecutter  # type: ignore
 
+from port_ocean import __version__
 from port_ocean.cli.commands.main import cli_start, print_logo, console
 from port_ocean.cli.utils import cli_root_path
 
 
 @cli_start.command()
 @click.argument("path", default=".", type=click.Path(exists=True))
 def new(path: str) -> None:
@@ -17,15 +18,19 @@
     """
     print_logo()
 
     console.print(
         "🚢 Unloading cargo... Setting up your integration at the dock.", style="bold"
     )
 
-    result = cookiecutter(f"{cli_root_path}/cookiecutter", output_dir=path)
+    result = cookiecutter(
+        f"{cli_root_path}/cookiecutter",
+        output_dir=path,
+        extra_context={"version": __version__},
+    )
     name = result.split("/")[-1]
 
     console.print(
         "\n🌊 Ahoy, Captain! Your project is ready to set sail into the vast ocean of possibilities!",
         style="bold",
     )
     console.print("Here are your next steps:\n", style="bold")
```

### Comparing `port_ocean-0.1.3rc4/port_ocean/cli/commands/pull.py` & `port_ocean-0.1.4.dev1/port_ocean/cli/commands/pull.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.3rc4/port_ocean/cli/commands/sail.py` & `port_ocean-0.1.4.dev1/port_ocean/cli/commands/sail.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.3rc4/port_ocean/cli/commands/version.py` & `port_ocean-0.1.4.dev1/port_ocean/cli/commands/version.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.3rc4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.gitignore` & `port_ocean-0.1.4.dev1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.gitignore`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.3rc4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Makefile` & `port_ocean-0.1.4.dev1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Makefile`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.3rc4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/README.md` & `port_ocean-0.1.4.dev1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/README.md`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.3rc4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/config.yaml` & `port_ocean-0.1.4.dev1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/config.yaml`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.3rc4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/main.py` & `port_ocean-0.1.4.dev1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/main.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.3rc4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/pyproject.toml` & `port_ocean-0.1.4.dev1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 name = "{{cookiecutter.integration_name}}"
 version = "0.1.0"
 description = "{{cookiecutter.integration_short_description}}"
 authors = ["{{cookiecutter.full_name}} <{{cookiecutter.email}}>"]
 
 [tool.poetry.dependencies]
 python = "^3.11"
-port_ocean = { version = "^0.1.0", extras = ["cli"] }
+port_ocean = { version = "^{{ cookiecutter.version }}", extras = ["cli"] }
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2"
 black = "^23.3.0"
 mypy = "^1.3.0"
 ruff = "^0.0.278"
 pylint = "^2.17.4"
```

### Comparing `port_ocean-0.1.3rc4/port_ocean/clients/port/authentication.py` & `port_ocean-0.1.4.dev1/port_ocean/clients/port/authentication.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.3rc4/port_ocean/clients/port/client.py` & `port_ocean-0.1.4.dev1/port_ocean/clients/port/client.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.3rc4/port_ocean/clients/port/mixins/blueprints.py` & `port_ocean-0.1.4.dev1/port_ocean/clients/port/mixins/blueprints.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.3rc4/port_ocean/clients/port/mixins/entities.py` & `port_ocean-0.1.4.dev1/port_ocean/clients/port/mixins/entities.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.3rc4/port_ocean/clients/port/mixins/integrations.py` & `port_ocean-0.1.4.dev1/port_ocean/clients/port/mixins/integrations.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.3rc4/port_ocean/clients/port/types.py` & `port_ocean-0.1.4.dev1/port_ocean/clients/port/types.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.3rc4/port_ocean/clients/port/utils.py` & `port_ocean-0.1.4.dev1/port_ocean/clients/port/utils.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.3rc4/port_ocean/config/base.py` & `port_ocean-0.1.4.dev1/port_ocean/config/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Any
 
 import yaml
 from humps import decamelize
 from pydantic import BaseSettings
 from pydantic.env_settings import EnvSettingsSource, InitSettingsSource
 
-PROVIDER_WRAPPER_PATTERN = r"\\{\\{ from (.*) \\}\\}"
+PROVIDER_WRAPPER_PATTERN = r"{{ from (.*) }}"
 PROVIDER_CONFIG_PATTERN = r"^[a-zA-Z0-9]+ .*$"
 
 
 def read_yaml_config_settings_source(
     settings: "BaseOceanSettings", base_path: str
 ) -> str:
     yaml_file = getattr(settings.__config__, "yaml_file", "")
```

### Comparing `port_ocean-0.1.3rc4/port_ocean/config/dynamic.py` & `port_ocean-0.1.4.dev1/port_ocean/config/dynamic.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.3rc4/port_ocean/config/settings.py` & `port_ocean-0.1.4.dev1/port_ocean/config/settings.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.3rc4/port_ocean/consumers/kafka_consumer.py` & `port_ocean-0.1.4.dev1/port_ocean/consumers/kafka_consumer.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.3rc4/port_ocean/context/event.py` & `port_ocean-0.1.4.dev1/port_ocean/context/event.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.3rc4/port_ocean/context/ocean.py` & `port_ocean-0.1.4.dev1/port_ocean/context/ocean.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.3rc4/port_ocean/core/event_listener/__init__.py` & `port_ocean-0.1.4.dev1/port_ocean/core/event_listener/__init__.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.3rc4/port_ocean/core/event_listener/base.py` & `port_ocean-0.1.4.dev1/port_ocean/core/event_listener/base.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from abc import abstractmethod
 from typing import TypedDict, Callable, Any, Awaitable
 
 from pydantic import BaseModel, Extra
 
 
 class EventListenerEvents(TypedDict):
+    """
+    A dictionary containing event types and their corresponding event handlers.
+    """
     on_resync: Callable[[dict[Any, Any]], Awaitable[None]]
 
 
 class BaseEventListener:
     def __init__(
         self,
         events: EventListenerEvents,
@@ -20,8 +23,12 @@
         pass
 
 
 class EventListenerSettings(BaseModel, extra=Extra.allow):
     type: str
 
     def to_request(self) -> dict[str, Any]:
+        """
+        Converts the Settings object to a dictionary representation (request format).
+        This method is used when configuring the event listener settings for the Polling event listener.
+        """
         return {"type": self.type}
```

### Comparing `port_ocean-0.1.3rc4/port_ocean/core/event_listener/factory.py` & `port_ocean-0.1.4.dev1/port_ocean/core/event_listener/factory.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,25 +16,42 @@
     BaseEventListener,
     EventListenerEvents,
 )
 from port_ocean.exceptions.core import UnsupportedEventListenerTypeException
 
 
 class EventListenerFactory(BaseWithContext):
+    """
+    This class is responsible for creating different types of event listeners based on the provided configuration.
+    The factory takes a PortOceanContext, installation_id, and events dictionary as parameters.
+
+    Parameters:
+        context (PortOceanContext): The PortOceanContext object containing information about the current application context.
+        installation_id (str): The identifier of the installation associated with the event listener.
+        events (EventListenerEvents): A dictionary containing event types and their corresponding event handlers.
+
+    """
     def __init__(
         self,
         context: PortOceanContext,
         installation_id: str,
         events: EventListenerEvents,
     ):
         super().__init__(context)
         self.installation_id = installation_id
         self.events = events
 
     async def create_event_listener(self) -> BaseEventListener:
+        """
+        Creates and returns a specific event listener based on the provided configuration.
+        The event listener is wrapped with the events provided in the factory's initialization.
+        
+        Raises:
+            UnsupportedEventListenerTypeException: If the event listener type is not supported.
+        """
         wrapped_events: EventListenerEvents = {"on_resync": self.events["on_resync"]}
         event_listener: BaseEventListener
         config = self.context.config.event_listener
         _type = config.type.lower()
         assert_message = "Invalid event listener config, expected KafkaEventListenerSettings and got {0}"
         logger.info(f"Found event listener type: {_type}")
```

### Comparing `port_ocean-0.1.3rc4/port_ocean/core/event_listener/polling/event_listener.py` & `port_ocean-0.1.4.dev1/port_ocean/core/event_listener/polling/event_listener.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,33 +8,55 @@
     EventListenerEvents,
     EventListenerSettings,
 )
 from port_ocean.core.event_listener.polling.utils import repeat_every
 
 
 class PollingEventListenerSettings(EventListenerSettings):
+    """
+    Attributes:
+        type (Literal["POLLING"]): A literal indicating the type of the event listener, which is set to "POLLING" for this class.
+        resync_on_start (bool): A flag indicating whether to trigger a resync event on the start of the polling event listener.
+                                If True, the "on_resync" event will be triggered immediately when the polling listener starts.
+        interval (int): The interval in seconds at which the polling event listener checks for changes in the integration.
+                        The default interval is set to 60 seconds.
+    """
     type: Literal["POLLING"]
     resync_on_start: bool = True
     interval: int = 60
 
     def to_request(self) -> dict[str, Any]:
         return {}
 
 
 class PollingEventListener(BaseEventListener):
+    """
+    Polling event listener that checks for changes in the integration every `interval` seconds.
+
+    The `PollingEventListener` periodically checks for changes in the integration and triggers the "on_resync" event if changes are detected.
+
+    Parameters:
+        events (EventListenerEvents): A dictionary containing event types and their corresponding event handlers.
+        event_listener_config (PollingEventListenerSettings): Configuration settings for the Polling event listener.
+    """
     def __init__(
         self,
         events: EventListenerEvents,
         event_listener_config: PollingEventListenerSettings,
     ):
         super().__init__(events)
         self.event_listener_config = event_listener_config
         self._last_updated_at = None
 
     async def start(self) -> None:
+        """
+        Starts the polling event listener.
+        It registers the "on_resync" event to be called every `interval` seconds specified in the `event_listener_config`.
+        The `on_resync` event is triggered if the integration has changed since the last update.
+        """
         logger.info(
             f"Setting up Polling event listener with interval: {self.event_listener_config.interval}"
         )
 
         @repeat_every(seconds=self.event_listener_config.interval)
         async def resync() -> None:
             logger.info(
```

### Comparing `port_ocean-0.1.3rc4/port_ocean/core/event_listener/polling/utils.py` & `port_ocean-0.1.4.dev1/port_ocean/core/event_listener/polling/utils.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.3rc4/port_ocean/core/handlers/__init__.py` & `port_ocean-0.1.4.dev1/port_ocean/core/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.3rc4/port_ocean/core/handlers/entities_state_applier/base.py` & `port_ocean-0.1.4.dev1/port_ocean/core/handlers/entities_state_applier/base.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.3rc4/port_ocean/core/handlers/entities_state_applier/port/applier.py` & `port_ocean-0.1.4.dev1/port_ocean/core/handlers/entities_state_applier/port/applier.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.3rc4/port_ocean/core/handlers/entities_state_applier/port/get_related_entities.py` & `port_ocean-0.1.4.dev1/port_ocean/core/handlers/entities_state_applier/port/get_related_entities.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import asyncio
+from collections import defaultdict
 from itertools import groupby
 
 from port_ocean.clients.port.client import PortClient
 from port_ocean.core.models import Entity
 
 
 async def get_related_entities(
@@ -29,16 +30,22 @@
                 for blueprint in blueprints
                 if blueprint.identifier == entity.blueprint
             ),
         )
         for entity in entities_with_relations
     ]
 
-    related_entities = []
+    blueprints_to_relations = defaultdict(list)
     for entity, blueprint in entity_to_blueprint:
         for relation_name, relation in entity.relations.items():
             relation_blueprint = blueprint.relations[relation_name].target
-            related_entities.append(
-                Entity(identifier=relation, blueprint=relation_blueprint)
+            blueprints_to_relations[relation_blueprint].extend(
+                relation if isinstance(relation, list) else [relation]
             )
 
-    return related_entities
+    return [
+        Entity(identifier=relation, blueprint=blueprint)
+        for blueprint, relations in blueprints_to_relations.items()
+        # multiple entities can point to the same relation in the same blueprint, for performance reasons
+        # we want to avoid fetching the same relation multiple times
+        for relation in set(relations)
+    ]
```

### Comparing `port_ocean-0.1.3rc4/port_ocean/core/handlers/entities_state_applier/port/order_by_entities_dependencies.py` & `port_ocean-0.1.4.dev1/port_ocean/core/handlers/entities_state_applier/port/order_by_entities_dependencies.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.3rc4/port_ocean/core/handlers/entities_state_applier/port/validate_entity_relations.py` & `port_ocean-0.1.4.dev1/port_ocean/core/handlers/entities_state_applier/port/validate_entity_relations.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.3rc4/port_ocean/core/handlers/entity_processor/base.py` & `port_ocean-0.1.4.dev1/port_ocean/core/handlers/entity_processor/base.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.3rc4/port_ocean/core/handlers/entity_processor/jq_entity_processor.py` & `port_ocean-0.1.4.dev1/port_ocean/core/handlers/entity_processor/jq_entity_processor.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.3rc4/port_ocean/core/handlers/port_app_config/base.py` & `port_ocean-0.1.4.dev1/port_ocean/core/handlers/port_app_config/base.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.3rc4/port_ocean/core/handlers/port_app_config/models.py` & `port_ocean-0.1.4.dev1/port_ocean/core/handlers/port_app_config/models.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.3rc4/port_ocean/core/integrations/base.py` & `port_ocean-0.1.4.dev1/port_ocean/ocean.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,57 +1,63 @@
-import asyncio
+import sys
+from typing import Callable
 
+from fastapi import FastAPI, APIRouter
 from loguru import logger
+from pydantic import BaseModel
+from starlette.types import Scope, Receive, Send
 
-from port_ocean.context.event import (
-    event_context,
-    EventType,
+from port_ocean.clients.port.client import PortClient
+from port_ocean.config.settings import (
+    IntegrationConfiguration,
 )
-from port_ocean.context.ocean import PortOceanContext
-from port_ocean.core.event_listener.factory import (
-    EventListenerFactory,
+from port_ocean.context.ocean import (
+    PortOceanContext,
+    ocean,
+    initialize_port_ocean_context,
 )
-from port_ocean.core.integrations.mixins.sync import SyncRawMixin, SyncMixin
-from port_ocean.exceptions.core import IntegrationAlreadyStartedException
+from port_ocean.core.integrations.base import BaseIntegration
+from port_ocean.middlewares import request_handler
 
 
-class BaseIntegration(SyncRawMixin, SyncMixin):
-    def __init__(self, context: PortOceanContext):
-        SyncRawMixin.__init__(self)
-        SyncMixin.__init__(self)
-        self.started = False
-        self.context = context
-        self.event_listener_factory = EventListenerFactory(
-            context,
-            self.context.config.integration.identifier,
-            {"on_resync": self.sync_raw_all},
+class Ocean:
+    def __init__(
+        self,
+        app: FastAPI | None = None,
+        integration_class: Callable[[PortOceanContext], BaseIntegration] | None = None,
+        integration_router: APIRouter | None = None,
+        config_factory: Callable[..., BaseModel] | None = None,
+    ):
+        initialize_port_ocean_context(self)
+        self.fast_api_app = app or FastAPI()
+        self.fast_api_app.middleware("http")(request_handler)
+
+        self.config = IntegrationConfiguration(base_path="./")
+        if config_factory:
+            self.config.integration.config = config_factory(
+                **self.config.integration.config
+            ).dict()
+        self.integration_router = integration_router or APIRouter()
+
+        self.port_client = PortClient(
+            base_url=self.config.port.base_url,
+            client_id=self.config.port.client_id,
+            client_secret=self.config.port.client_secret,
+            integration_identifier=self.config.integration.identifier,
+            integration_type=self.config.integration.type,
         )
-
-    async def start(self) -> None:
-        logger.info("Starting integration")
-        if self.started:
-            raise IntegrationAlreadyStartedException("Integration already started")
-
-        if (
-            not self.event_strategy["resync"]
-            and self.__class__._on_resync == BaseIntegration._on_resync
-        ):
-            raise NotImplementedError("on_resync is not implemented")
-
-        await self.initialize_handlers()
-
-        logger.info("Initializing integration at port")
-        await self.context.port_client.initialize_integration(
-            self.context.config.integration.type,
-            self.context.config.event_listener.to_request(),
+        self.integration = (
+            integration_class(ocean) if integration_class else BaseIntegration(ocean)
         )
 
-        self.started = True
+    async def __call__(self, scope: Scope, receive: Receive, send: Send) -> None:
+        self.fast_api_app.include_router(self.integration_router, prefix="/integration")
+
+        @self.fast_api_app.on_event("startup")
+        async def startup() -> None:
+            try:
+                await self.integration.start()
+            except Exception as e:
+                logger.error(f"Failed to start integration with error: {e}")
+                sys.exit("Server stopped")
 
-        async with event_context(EventType.START, trigger_type="machine"):
-            await asyncio.gather(
-                *(listener() for listener in self.event_strategy["start"])
-            )
-
-        logger.info("Initializing event listener")
-        event_listener = await self.event_listener_factory.create_event_listener()
-        await event_listener.start()
+        await self.fast_api_app(scope, receive, send)
```

### Comparing `port_ocean-0.1.3rc4/port_ocean/core/integrations/mixins/events.py` & `port_ocean-0.1.4.dev1/port_ocean/core/integrations/mixins/events.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.3rc4/port_ocean/core/integrations/mixins/handler.py` & `port_ocean-0.1.4.dev1/port_ocean/core/integrations/mixins/handler.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.3rc4/port_ocean/core/integrations/mixins/sync.py` & `port_ocean-0.1.4.dev1/port_ocean/core/integrations/mixins/sync.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.3rc4/port_ocean/core/integrations/mixins/utils.py` & `port_ocean-0.1.4.dev1/port_ocean/core/integrations/mixins/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from contextlib import contextmanager
 from typing import Awaitable, Generator, Callable
 
+from loguru import logger
 from port_ocean.core.ocean_types import (
     ASYNC_GENERATOR_RESYNC_TYPE,
     RAW_RESULT,
 )
 from port_ocean.core.utils import validate_result
 from port_ocean.exceptions.core import RawObjectValidationException, OceanAbortException
 
@@ -16,17 +17,17 @@
     except RawObjectValidationException as error:
         raise OceanAbortException(
             f"Failed to validate raw data for returned data from resync function, error: {error}"
         ) from error
     except StopAsyncIteration:
         raise
     except Exception as error:
-        raise OceanAbortException(
-            f"Failed to execute resync function, error: {error}"
-        ) from error
+        err_msg = f"Failed to execute resync function, error: {error}"
+        logger.exception(err_msg)
+        raise OceanAbortException(err_msg) from error
 
 
 async def resync_function_wrapper(
     fn: Callable[[str], Awaitable[RAW_RESULT]], kind: str
 ) -> RAW_RESULT:
     with resync_error_handling():
         results = await fn(kind)
```

### Comparing `port_ocean-0.1.3rc4/port_ocean/core/models.py` & `port_ocean-0.1.4.dev1/port_ocean/core/models.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,35 +6,23 @@
 Model = TypeVar("Model", bound="BaseModel")
 
 
 class Entity(BaseModel):
     identifier: str
     blueprint: str
     title: str | None
-    team: str | list[str] = []
+    team: str | None | list[str | None] = []
     properties: dict[str, Any] = {}
     relations: dict[str, Any] = {}
 
     @classmethod
     def parse_obj(cls: Type["Model"], obj: dict[Any, Any]) -> "Model":
         obj["identifier"] = str(obj.get("identifier"))
         obj["blueprint"] = str(obj.get("blueprint"))
-        if obj.get("team"):
-            team = obj.get("team")
-            obj["team"] = (
-                [str(item) for item in team]
-                if isinstance(team, list)
-                else str(obj.get("team"))
-            )
-
-        for key, value in obj.get("relations", {}).items():
-            if isinstance(value, list):
-                obj["relations"][key] = [str(item) for item in value]
-            else:
-                obj["relations"][key] = str(value)
+
         return super(Entity, cls).parse_obj(obj)
 
 
 class BlueprintRelation(BaseModel):
     many: bool
     required: bool
     target: str
```

### Comparing `port_ocean-0.1.3rc4/port_ocean/core/ocean_types.py` & `port_ocean-0.1.4.dev1/port_ocean/core/ocean_types.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.3rc4/port_ocean/core/utils.py` & `port_ocean-0.1.4.dev1/port_ocean/core/utils.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.3rc4/port_ocean/exceptions/core.py` & `port_ocean-0.1.4.dev1/port_ocean/exceptions/core.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.3rc4/port_ocean/middlewares.py` & `port_ocean-0.1.4.dev1/port_ocean/middlewares.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.3rc4/port_ocean/port_defaults.py` & `port_ocean-0.1.4.dev1/port_ocean/port_defaults.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.3rc4/port_ocean/run.py` & `port_ocean-0.1.4.dev1/port_ocean/run.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.3rc4/port_ocean/utils.py` & `port_ocean-0.1.4.dev1/port_ocean/utils.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.3rc4/pyproject.toml` & `port_ocean-0.1.4.dev1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "port-ocean"
-version = "0.1.3rc4"
+version = "0.1.4dev1"
 description = "Port Ocean is a CLI tool for managing your Port projects."
 readme = "README.md"
 homepage = "https://app.getport.io"
 repository = "https://github.com/port-labs/Port-Ocean"
 
 authors = ["Daniel Sinai <daniel@getport.io>", "Yair Siman-Tov <yair@getport.io>"]
 packages = [
```

### Comparing `port_ocean-0.1.3rc4/PKG-INFO` & `port_ocean-0.1.4.dev1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: port-ocean
-Version: 0.1.3rc4
+Version: 0.1.4.dev1
 Summary: Port Ocean is a CLI tool for managing your Port projects.
 Home-page: https://app.getport.io
 Keywords: ocean,port-ocean,port
 Author: Daniel Sinai
 Author-email: daniel@getport.io
 Requires-Python: >=3.11,<4.0
 Classifier: Framework :: FastAPI
```

