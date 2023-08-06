# Comparing `tmp/port_ocean-0.1.4.dev1.tar.gz` & `tmp/port_ocean-0.1.4.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "port_ocean-0.1.4.dev1.tar", max compression
+gzip compressed data, was "port_ocean-0.1.4.dev2.tar", max compression
```

## Comparing `port_ocean-0.1.4.dev1.tar` & `port_ocean-0.1.4.dev2.tar`

### file list

```diff
@@ -1,101 +1,101 @@
--rw-r--r--   0        0        0    11357 2023-08-06 15:48:03.368126 port_ocean-0.1.4.dev1/LICENSE
--rw-r--r--   0        0        0     4639 2023-08-06 15:48:03.368126 port_ocean-0.1.4.dev1/README.md
--rw-r--r--   0        0        0      270 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/__init__.py
--rw-r--r--   0        0        0      328 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/cli/__init__.py
--rw-r--r--   0        0        0       57 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/cli/cli.py
--rw-r--r--   0        0        0      278 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/cli/commands/__init__.py
--rw-r--r--   0        0        0     1134 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/cli/commands/list_integrations.py
--rw-r--r--   0        0        0     1057 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/cli/commands/main.py
--rw-r--r--   0        0        0     1816 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/cli/commands/new.py
--rw-r--r--   0        0        0     2306 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/cli/commands/pull.py
--rw-r--r--   0        0        0     1534 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/cli/commands/sail.py
--rw-r--r--   0        0        0      536 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/cli/commands/version.py
--rw-r--r--   0        0        0      429 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/cli/cookiecutter/cookiecutter.json
--rw-r--r--   0        0        0       42 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.dockerignore
--rw-r--r--   0        0        0     2698 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.gitignore
--rw-r--r--   0        0        0       12 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.port/resources/.gitignore
--rw-r--r--   0        0        0      388 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.port/spec.yaml
--rw-r--r--   0        0        0      292 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/CHANGELOG.md
--rw-r--r--   0        0        0      449 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Dockerfile
--rw-r--r--   0        0        0     1680 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Makefile
--rw-r--r--   0        0        0      655 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/README.md
--rw-r--r--   0        0        0       12 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/changelog/.gitignore
--rw-r--r--   0        0        0      898 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/config.yaml
--rw-r--r--   0        0        0       65 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/debug.py
--rw-r--r--   0        0        0     1669 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/main.py
--rw-r--r--   0        0        0       46 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/poetry.toml
--rw-r--r--   0        0        0     1941 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/pyproject.toml
--rw-r--r--   0        0        0        0 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/tests/__init__.py
--rw-r--r--   0        0        0       54 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/cli/utils.py
--rw-r--r--   0        0        0        0 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/clients/__init__.py
--rw-r--r--   0        0        0        0 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/clients/port/__init__.py
--rw-r--r--   0        0        0     2563 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/clients/port/authentication.py
--rw-r--r--   0        0        0     2309 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/clients/port/client.py
--rw-r--r--   0        0        0        0 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/clients/port/mixins/__init__.py
--rw-r--r--   0        0        0     2928 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/clients/port/mixins/blueprints.py
--rw-r--r--   0        0        0     5623 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/clients/port/mixins/entities.py
--rw-r--r--   0        0        0     3909 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/clients/port/mixins/integrations.py
--rw-r--r--   0        0        0      593 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/clients/port/types.py
--rw-r--r--   0        0        0      781 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/clients/port/utils.py
--rw-r--r--   0        0        0        0 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/config/__init__.py
--rw-r--r--   0        0        0     4011 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/config/base.py
--rw-r--r--   0        0        0     1816 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/config/dynamic.py
--rw-r--r--   0        0        0     1231 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/config/settings.py
--rw-r--r--   0        0        0        0 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/consumers/__init__.py
--rw-r--r--   0        0        0      125 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/consumers/base_consumer.py
--rw-r--r--   0        0        0     4147 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/consumers/kafka_consumer.py
--rw-r--r--   0        0        0        0 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/context/__init__.py
--rw-r--r--   0        0        0     3201 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/context/event.py
--rw-r--r--   0        0        0     4283 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/context/ocean.py
--rw-r--r--   0        0        0        0 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/core/__init__.py
--rw-r--r--   0        0        0      219 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/core/base.py
--rw-r--r--   0        0        0      607 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/core/event_listener/__init__.py
--rw-r--r--   0        0        0      891 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/core/event_listener/base.py
--rw-r--r--   0        0        0     3474 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/core/event_listener/factory.py
--rw-r--r--   0        0        0        0 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/core/event_listener/http/__init__.py
--rw-r--r--   0        0        0     2511 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/core/event_listener/http/event_listener.py
--rw-r--r--   0        0        0        0 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/core/event_listener/kafka/__init__.py
--rw-r--r--   0        0        0     6351 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/core/event_listener/kafka/event_listener.py
--rw-r--r--   0        0        0     3264 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/core/event_listener/polling/event_listener.py
--rw-r--r--   0        0        0     2799 2023-08-06 15:48:03.384127 port_ocean-0.1.4.dev1/port_ocean/core/event_listener/polling/utils.py
--rw-r--r--   0        0        0      716 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/core/handlers/__init__.py
--rw-r--r--   0        0        0        0 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/core/handlers/entities_state_applier/__init__.py
--rw-r--r--   0        0        0      869 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/core/handlers/entities_state_applier/base.py
--rw-r--r--   0        0        0        0 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/core/handlers/entities_state_applier/port/__init__.py
--rw-r--r--   0        0        0     7977 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/core/handlers/entities_state_applier/port/applier.py
--rw-r--r--   0        0        0     1751 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/core/handlers/entities_state_applier/port/get_related_entities.py
--rw-r--r--   0        0        0      988 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/core/handlers/entities_state_applier/port/order_by_entities_dependencies.py
--rw-r--r--   0        0        0     1392 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/core/handlers/entities_state_applier/port/validate_entity_relations.py
--rw-r--r--   0        0        0        0 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/core/handlers/entity_processor/__init__.py
--rw-r--r--   0        0        0      955 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/core/handlers/entity_processor/base.py
--rw-r--r--   0        0        0     2685 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/core/handlers/entity_processor/jq_entity_processor.py
--rw-r--r--   0        0        0        0 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/core/handlers/port_app_config/__init__.py
--rw-r--r--   0        0        0      396 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/core/handlers/port_app_config/api.py
--rw-r--r--   0        0        0      651 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/core/handlers/port_app_config/base.py
--rw-r--r--   0        0        0     1810 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/core/handlers/port_app_config/models.py
--rw-r--r--   0        0        0        0 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/core/integrations/__init__.py
--rw-r--r--   0        0        0     3162 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/core/integrations/base.py
--rw-r--r--   0        0        0        0 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/core/integrations/mixins/__init__.py
--rw-r--r--   0        0        0      698 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/core/integrations/mixins/events.py
--rw-r--r--   0        0        0     2569 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/core/integrations/mixins/handler.py
--rw-r--r--   0        0        0    11843 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/core/integrations/mixins/sync.py
--rw-r--r--   0        0        0     1747 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/core/integrations/mixins/utils.py
--rw-r--r--   0        0        0      909 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/core/models.py
--rw-r--r--   0        0        0      781 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/core/ocean_types.py
--rw-r--r--   0        0        0     1957 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/core/utils.py
--rw-r--r--   0        0        0        0 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/exceptions/__init__.py
--rw-r--r--   0        0        0      426 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/exceptions/api.py
--rw-r--r--   0        0        0       46 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/exceptions/base.py
--rw-r--r--   0        0        0      180 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/exceptions/clients.py
--rw-r--r--   0        0        0      235 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/exceptions/context.py
--rw-r--r--   0        0        0      532 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/exceptions/core.py
--rw-r--r--   0        0        0      407 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/exceptions/port_defaults.py
--rw-r--r--   0        0        0     1107 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/logger_setup.py
--rw-r--r--   0        0        0     2475 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/middlewares.py
--rw-r--r--   0        0        0     2263 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/ocean.py
--rw-r--r--   0        0        0     7161 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/port_defaults.py
--rw-r--r--   0        0        0        0 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/py.typed
--rw-r--r--   0        0        0     2834 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/run.py
--rw-r--r--   0        0        0     1007 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/port_ocean/utils.py
--rw-r--r--   0        0        0     3462 2023-08-06 15:48:03.388127 port_ocean-0.1.4.dev1/pyproject.toml
--rw-r--r--   0        0        0     6361 1970-01-01 00:00:00.000000 port_ocean-0.1.4.dev1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-08-06 15:56:06.954321 port_ocean-0.1.4.dev2/LICENSE
+-rw-r--r--   0        0        0     4639 2023-08-06 15:56:06.954321 port_ocean-0.1.4.dev2/README.md
+-rw-r--r--   0        0        0      270 2023-08-06 15:56:06.970321 port_ocean-0.1.4.dev2/port_ocean/__init__.py
+-rw-r--r--   0        0        0      328 2023-08-06 15:56:06.970321 port_ocean-0.1.4.dev2/port_ocean/cli/__init__.py
+-rw-r--r--   0        0        0       57 2023-08-06 15:56:06.970321 port_ocean-0.1.4.dev2/port_ocean/cli/cli.py
+-rw-r--r--   0        0        0      278 2023-08-06 15:56:06.970321 port_ocean-0.1.4.dev2/port_ocean/cli/commands/__init__.py
+-rw-r--r--   0        0        0     1134 2023-08-06 15:56:06.970321 port_ocean-0.1.4.dev2/port_ocean/cli/commands/list_integrations.py
+-rw-r--r--   0        0        0     1057 2023-08-06 15:56:06.970321 port_ocean-0.1.4.dev2/port_ocean/cli/commands/main.py
+-rw-r--r--   0        0        0     1816 2023-08-06 15:56:06.970321 port_ocean-0.1.4.dev2/port_ocean/cli/commands/new.py
+-rw-r--r--   0        0        0     2306 2023-08-06 15:56:06.970321 port_ocean-0.1.4.dev2/port_ocean/cli/commands/pull.py
+-rw-r--r--   0        0        0     1534 2023-08-06 15:56:06.970321 port_ocean-0.1.4.dev2/port_ocean/cli/commands/sail.py
+-rw-r--r--   0        0        0      536 2023-08-06 15:56:06.970321 port_ocean-0.1.4.dev2/port_ocean/cli/commands/version.py
+-rw-r--r--   0        0        0      429 2023-08-06 15:56:06.970321 port_ocean-0.1.4.dev2/port_ocean/cli/cookiecutter/cookiecutter.json
+-rw-r--r--   0        0        0       42 2023-08-06 15:56:06.970321 port_ocean-0.1.4.dev2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.dockerignore
+-rw-r--r--   0        0        0     2698 2023-08-06 15:56:06.970321 port_ocean-0.1.4.dev2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.gitignore
+-rw-r--r--   0        0        0       12 2023-08-06 15:56:06.970321 port_ocean-0.1.4.dev2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.port/resources/.gitignore
+-rw-r--r--   0        0        0      388 2023-08-06 15:56:06.970321 port_ocean-0.1.4.dev2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.port/spec.yaml
+-rw-r--r--   0        0        0      292 2023-08-06 15:56:06.970321 port_ocean-0.1.4.dev2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/CHANGELOG.md
+-rw-r--r--   0        0        0      449 2023-08-06 15:56:06.970321 port_ocean-0.1.4.dev2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Dockerfile
+-rw-r--r--   0        0        0     1680 2023-08-06 15:56:06.970321 port_ocean-0.1.4.dev2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Makefile
+-rw-r--r--   0        0        0      655 2023-08-06 15:56:06.970321 port_ocean-0.1.4.dev2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/README.md
+-rw-r--r--   0        0        0       12 2023-08-06 15:56:06.970321 port_ocean-0.1.4.dev2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/changelog/.gitignore
+-rw-r--r--   0        0        0      898 2023-08-06 15:56:06.970321 port_ocean-0.1.4.dev2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/config.yaml
+-rw-r--r--   0        0        0       65 2023-08-06 15:56:06.970321 port_ocean-0.1.4.dev2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/debug.py
+-rw-r--r--   0        0        0     1669 2023-08-06 15:56:06.970321 port_ocean-0.1.4.dev2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/main.py
+-rw-r--r--   0        0        0       46 2023-08-06 15:56:06.970321 port_ocean-0.1.4.dev2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/poetry.toml
+-rw-r--r--   0        0        0     1941 2023-08-06 15:56:06.970321 port_ocean-0.1.4.dev2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-06 15:56:06.970321 port_ocean-0.1.4.dev2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/tests/__init__.py
+-rw-r--r--   0        0        0       54 2023-08-06 15:56:06.970321 port_ocean-0.1.4.dev2/port_ocean/cli/utils.py
+-rw-r--r--   0        0        0        0 2023-08-06 15:56:06.970321 port_ocean-0.1.4.dev2/port_ocean/clients/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-06 15:56:06.970321 port_ocean-0.1.4.dev2/port_ocean/clients/port/__init__.py
+-rw-r--r--   0        0        0     2563 2023-08-06 15:56:06.970321 port_ocean-0.1.4.dev2/port_ocean/clients/port/authentication.py
+-rw-r--r--   0        0        0     2309 2023-08-06 15:56:06.970321 port_ocean-0.1.4.dev2/port_ocean/clients/port/client.py
+-rw-r--r--   0        0        0        0 2023-08-06 15:56:06.970321 port_ocean-0.1.4.dev2/port_ocean/clients/port/mixins/__init__.py
+-rw-r--r--   0        0        0     2928 2023-08-06 15:56:06.970321 port_ocean-0.1.4.dev2/port_ocean/clients/port/mixins/blueprints.py
+-rw-r--r--   0        0        0     5623 2023-08-06 15:56:06.970321 port_ocean-0.1.4.dev2/port_ocean/clients/port/mixins/entities.py
+-rw-r--r--   0        0        0     3909 2023-08-06 15:56:06.970321 port_ocean-0.1.4.dev2/port_ocean/clients/port/mixins/integrations.py
+-rw-r--r--   0        0        0      593 2023-08-06 15:56:06.970321 port_ocean-0.1.4.dev2/port_ocean/clients/port/types.py
+-rw-r--r--   0        0        0      781 2023-08-06 15:56:06.970321 port_ocean-0.1.4.dev2/port_ocean/clients/port/utils.py
+-rw-r--r--   0        0        0        0 2023-08-06 15:56:06.970321 port_ocean-0.1.4.dev2/port_ocean/config/__init__.py
+-rw-r--r--   0        0        0     4011 2023-08-06 15:56:06.970321 port_ocean-0.1.4.dev2/port_ocean/config/base.py
+-rw-r--r--   0        0        0     1816 2023-08-06 15:56:06.970321 port_ocean-0.1.4.dev2/port_ocean/config/dynamic.py
+-rw-r--r--   0        0        0     1231 2023-08-06 15:56:06.970321 port_ocean-0.1.4.dev2/port_ocean/config/settings.py
+-rw-r--r--   0        0        0        0 2023-08-06 15:56:06.970321 port_ocean-0.1.4.dev2/port_ocean/consumers/__init__.py
+-rw-r--r--   0        0        0      125 2023-08-06 15:56:06.970321 port_ocean-0.1.4.dev2/port_ocean/consumers/base_consumer.py
+-rw-r--r--   0        0        0     4147 2023-08-06 15:56:06.970321 port_ocean-0.1.4.dev2/port_ocean/consumers/kafka_consumer.py
+-rw-r--r--   0        0        0        0 2023-08-06 15:56:06.970321 port_ocean-0.1.4.dev2/port_ocean/context/__init__.py
+-rw-r--r--   0        0        0     3201 2023-08-06 15:56:06.970321 port_ocean-0.1.4.dev2/port_ocean/context/event.py
+-rw-r--r--   0        0        0     4283 2023-08-06 15:56:06.970321 port_ocean-0.1.4.dev2/port_ocean/context/ocean.py
+-rw-r--r--   0        0        0        0 2023-08-06 15:56:06.970321 port_ocean-0.1.4.dev2/port_ocean/core/__init__.py
+-rw-r--r--   0        0        0      219 2023-08-06 15:56:06.970321 port_ocean-0.1.4.dev2/port_ocean/core/base.py
+-rw-r--r--   0        0        0      607 2023-08-06 15:56:06.970321 port_ocean-0.1.4.dev2/port_ocean/core/event_listener/__init__.py
+-rw-r--r--   0        0        0      891 2023-08-06 15:56:06.970321 port_ocean-0.1.4.dev2/port_ocean/core/event_listener/base.py
+-rw-r--r--   0        0        0     3474 2023-08-06 15:56:06.970321 port_ocean-0.1.4.dev2/port_ocean/core/event_listener/factory.py
+-rw-r--r--   0        0        0        0 2023-08-06 15:56:06.974321 port_ocean-0.1.4.dev2/port_ocean/core/event_listener/http/__init__.py
+-rw-r--r--   0        0        0     2511 2023-08-06 15:56:06.974321 port_ocean-0.1.4.dev2/port_ocean/core/event_listener/http/event_listener.py
+-rw-r--r--   0        0        0        0 2023-08-06 15:56:06.974321 port_ocean-0.1.4.dev2/port_ocean/core/event_listener/kafka/__init__.py
+-rw-r--r--   0        0        0     6351 2023-08-06 15:56:06.974321 port_ocean-0.1.4.dev2/port_ocean/core/event_listener/kafka/event_listener.py
+-rw-r--r--   0        0        0     3264 2023-08-06 15:56:06.974321 port_ocean-0.1.4.dev2/port_ocean/core/event_listener/polling/event_listener.py
+-rw-r--r--   0        0        0     2799 2023-08-06 15:56:06.974321 port_ocean-0.1.4.dev2/port_ocean/core/event_listener/polling/utils.py
+-rw-r--r--   0        0        0      716 2023-08-06 15:56:06.974321 port_ocean-0.1.4.dev2/port_ocean/core/handlers/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-06 15:56:06.974321 port_ocean-0.1.4.dev2/port_ocean/core/handlers/entities_state_applier/__init__.py
+-rw-r--r--   0        0        0      869 2023-08-06 15:56:06.974321 port_ocean-0.1.4.dev2/port_ocean/core/handlers/entities_state_applier/base.py
+-rw-r--r--   0        0        0        0 2023-08-06 15:56:06.974321 port_ocean-0.1.4.dev2/port_ocean/core/handlers/entities_state_applier/port/__init__.py
+-rw-r--r--   0        0        0     7977 2023-08-06 15:56:06.974321 port_ocean-0.1.4.dev2/port_ocean/core/handlers/entities_state_applier/port/applier.py
+-rw-r--r--   0        0        0     1751 2023-08-06 15:56:06.974321 port_ocean-0.1.4.dev2/port_ocean/core/handlers/entities_state_applier/port/get_related_entities.py
+-rw-r--r--   0        0        0     1151 2023-08-06 15:56:06.974321 port_ocean-0.1.4.dev2/port_ocean/core/handlers/entities_state_applier/port/order_by_entities_dependencies.py
+-rw-r--r--   0        0        0     1392 2023-08-06 15:56:06.974321 port_ocean-0.1.4.dev2/port_ocean/core/handlers/entities_state_applier/port/validate_entity_relations.py
+-rw-r--r--   0        0        0        0 2023-08-06 15:56:06.974321 port_ocean-0.1.4.dev2/port_ocean/core/handlers/entity_processor/__init__.py
+-rw-r--r--   0        0        0      955 2023-08-06 15:56:06.974321 port_ocean-0.1.4.dev2/port_ocean/core/handlers/entity_processor/base.py
+-rw-r--r--   0        0        0     2685 2023-08-06 15:56:06.974321 port_ocean-0.1.4.dev2/port_ocean/core/handlers/entity_processor/jq_entity_processor.py
+-rw-r--r--   0        0        0        0 2023-08-06 15:56:06.974321 port_ocean-0.1.4.dev2/port_ocean/core/handlers/port_app_config/__init__.py
+-rw-r--r--   0        0        0      396 2023-08-06 15:56:06.974321 port_ocean-0.1.4.dev2/port_ocean/core/handlers/port_app_config/api.py
+-rw-r--r--   0        0        0      651 2023-08-06 15:56:06.974321 port_ocean-0.1.4.dev2/port_ocean/core/handlers/port_app_config/base.py
+-rw-r--r--   0        0        0     1810 2023-08-06 15:56:06.974321 port_ocean-0.1.4.dev2/port_ocean/core/handlers/port_app_config/models.py
+-rw-r--r--   0        0        0        0 2023-08-06 15:56:06.974321 port_ocean-0.1.4.dev2/port_ocean/core/integrations/__init__.py
+-rw-r--r--   0        0        0     3162 2023-08-06 15:56:06.974321 port_ocean-0.1.4.dev2/port_ocean/core/integrations/base.py
+-rw-r--r--   0        0        0        0 2023-08-06 15:56:06.974321 port_ocean-0.1.4.dev2/port_ocean/core/integrations/mixins/__init__.py
+-rw-r--r--   0        0        0      698 2023-08-06 15:56:06.974321 port_ocean-0.1.4.dev2/port_ocean/core/integrations/mixins/events.py
+-rw-r--r--   0        0        0     2569 2023-08-06 15:56:06.974321 port_ocean-0.1.4.dev2/port_ocean/core/integrations/mixins/handler.py
+-rw-r--r--   0        0        0    11843 2023-08-06 15:56:06.974321 port_ocean-0.1.4.dev2/port_ocean/core/integrations/mixins/sync.py
+-rw-r--r--   0        0        0     1747 2023-08-06 15:56:06.974321 port_ocean-0.1.4.dev2/port_ocean/core/integrations/mixins/utils.py
+-rw-r--r--   0        0        0      909 2023-08-06 15:56:06.974321 port_ocean-0.1.4.dev2/port_ocean/core/models.py
+-rw-r--r--   0        0        0      781 2023-08-06 15:56:06.974321 port_ocean-0.1.4.dev2/port_ocean/core/ocean_types.py
+-rw-r--r--   0        0        0     1957 2023-08-06 15:56:06.974321 port_ocean-0.1.4.dev2/port_ocean/core/utils.py
+-rw-r--r--   0        0        0        0 2023-08-06 15:56:06.974321 port_ocean-0.1.4.dev2/port_ocean/exceptions/__init__.py
+-rw-r--r--   0        0        0      426 2023-08-06 15:56:06.974321 port_ocean-0.1.4.dev2/port_ocean/exceptions/api.py
+-rw-r--r--   0        0        0       46 2023-08-06 15:56:06.974321 port_ocean-0.1.4.dev2/port_ocean/exceptions/base.py
+-rw-r--r--   0        0        0      180 2023-08-06 15:56:06.974321 port_ocean-0.1.4.dev2/port_ocean/exceptions/clients.py
+-rw-r--r--   0        0        0      235 2023-08-06 15:56:06.974321 port_ocean-0.1.4.dev2/port_ocean/exceptions/context.py
+-rw-r--r--   0        0        0      532 2023-08-06 15:56:06.974321 port_ocean-0.1.4.dev2/port_ocean/exceptions/core.py
+-rw-r--r--   0        0        0      407 2023-08-06 15:56:06.974321 port_ocean-0.1.4.dev2/port_ocean/exceptions/port_defaults.py
+-rw-r--r--   0        0        0     1107 2023-08-06 15:56:06.974321 port_ocean-0.1.4.dev2/port_ocean/logger_setup.py
+-rw-r--r--   0        0        0     2475 2023-08-06 15:56:06.974321 port_ocean-0.1.4.dev2/port_ocean/middlewares.py
+-rw-r--r--   0        0        0     2263 2023-08-06 15:56:06.974321 port_ocean-0.1.4.dev2/port_ocean/ocean.py
+-rw-r--r--   0        0        0     7161 2023-08-06 15:56:06.974321 port_ocean-0.1.4.dev2/port_ocean/port_defaults.py
+-rw-r--r--   0        0        0        0 2023-08-06 15:56:06.974321 port_ocean-0.1.4.dev2/port_ocean/py.typed
+-rw-r--r--   0        0        0     2834 2023-08-06 15:56:06.974321 port_ocean-0.1.4.dev2/port_ocean/run.py
+-rw-r--r--   0        0        0     1007 2023-08-06 15:56:06.974321 port_ocean-0.1.4.dev2/port_ocean/utils.py
+-rw-r--r--   0        0        0     3462 2023-08-06 15:56:06.974321 port_ocean-0.1.4.dev2/pyproject.toml
+-rw-r--r--   0        0        0     6361 1970-01-01 00:00:00.000000 port_ocean-0.1.4.dev2/PKG-INFO
```

### Comparing `port_ocean-0.1.4.dev1/LICENSE` & `port_ocean-0.1.4.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev1/README.md` & `port_ocean-0.1.4.dev2/README.md`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev1/port_ocean/cli/commands/list_integrations.py` & `port_ocean-0.1.4.dev2/port_ocean/cli/commands/list_integrations.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev1/port_ocean/cli/commands/main.py` & `port_ocean-0.1.4.dev2/port_ocean/cli/commands/main.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev1/port_ocean/cli/commands/new.py` & `port_ocean-0.1.4.dev2/port_ocean/cli/commands/new.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev1/port_ocean/cli/commands/pull.py` & `port_ocean-0.1.4.dev2/port_ocean/cli/commands/pull.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev1/port_ocean/cli/commands/sail.py` & `port_ocean-0.1.4.dev2/port_ocean/cli/commands/sail.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev1/port_ocean/cli/commands/version.py` & `port_ocean-0.1.4.dev2/port_ocean/cli/commands/version.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.gitignore` & `port_ocean-0.1.4.dev2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.gitignore`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Makefile` & `port_ocean-0.1.4.dev2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Makefile`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/README.md` & `port_ocean-0.1.4.dev2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/README.md`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/config.yaml` & `port_ocean-0.1.4.dev2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/config.yaml`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/main.py` & `port_ocean-0.1.4.dev2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/main.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/pyproject.toml` & `port_ocean-0.1.4.dev2/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/pyproject.toml`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev1/port_ocean/clients/port/authentication.py` & `port_ocean-0.1.4.dev2/port_ocean/clients/port/authentication.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev1/port_ocean/clients/port/client.py` & `port_ocean-0.1.4.dev2/port_ocean/clients/port/client.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev1/port_ocean/clients/port/mixins/blueprints.py` & `port_ocean-0.1.4.dev2/port_ocean/clients/port/mixins/blueprints.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev1/port_ocean/clients/port/mixins/entities.py` & `port_ocean-0.1.4.dev2/port_ocean/clients/port/mixins/entities.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev1/port_ocean/clients/port/mixins/integrations.py` & `port_ocean-0.1.4.dev2/port_ocean/clients/port/mixins/integrations.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev1/port_ocean/clients/port/types.py` & `port_ocean-0.1.4.dev2/port_ocean/clients/port/types.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev1/port_ocean/clients/port/utils.py` & `port_ocean-0.1.4.dev2/port_ocean/clients/port/utils.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev1/port_ocean/config/base.py` & `port_ocean-0.1.4.dev2/port_ocean/config/base.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev1/port_ocean/config/dynamic.py` & `port_ocean-0.1.4.dev2/port_ocean/config/dynamic.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev1/port_ocean/config/settings.py` & `port_ocean-0.1.4.dev2/port_ocean/config/settings.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev1/port_ocean/consumers/kafka_consumer.py` & `port_ocean-0.1.4.dev2/port_ocean/consumers/kafka_consumer.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev1/port_ocean/context/event.py` & `port_ocean-0.1.4.dev2/port_ocean/context/event.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev1/port_ocean/context/ocean.py` & `port_ocean-0.1.4.dev2/port_ocean/context/ocean.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev1/port_ocean/core/event_listener/__init__.py` & `port_ocean-0.1.4.dev2/port_ocean/core/event_listener/__init__.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev1/port_ocean/core/event_listener/base.py` & `port_ocean-0.1.4.dev2/port_ocean/core/event_listener/base.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev1/port_ocean/core/event_listener/factory.py` & `port_ocean-0.1.4.dev2/port_ocean/core/event_listener/factory.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev1/port_ocean/core/event_listener/http/event_listener.py` & `port_ocean-0.1.4.dev2/port_ocean/core/event_listener/http/event_listener.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev1/port_ocean/core/event_listener/kafka/event_listener.py` & `port_ocean-0.1.4.dev2/port_ocean/core/event_listener/kafka/event_listener.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev1/port_ocean/core/event_listener/polling/event_listener.py` & `port_ocean-0.1.4.dev2/port_ocean/core/event_listener/polling/event_listener.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev1/port_ocean/core/event_listener/polling/utils.py` & `port_ocean-0.1.4.dev2/port_ocean/core/event_listener/polling/utils.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev1/port_ocean/core/handlers/__init__.py` & `port_ocean-0.1.4.dev2/port_ocean/core/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev1/port_ocean/core/handlers/entities_state_applier/base.py` & `port_ocean-0.1.4.dev2/port_ocean/core/handlers/entities_state_applier/base.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev1/port_ocean/core/handlers/entities_state_applier/port/applier.py` & `port_ocean-0.1.4.dev2/port_ocean/core/handlers/entities_state_applier/port/applier.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev1/port_ocean/core/handlers/entities_state_applier/port/get_related_entities.py` & `port_ocean-0.1.4.dev2/port_ocean/core/handlers/entities_state_applier/port/get_related_entities.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev1/port_ocean/core/handlers/entities_state_applier/port/order_by_entities_dependencies.py` & `port_ocean-0.1.4.dev2/port_ocean/core/handlers/entities_state_applier/port/order_by_entities_dependencies.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,19 +15,23 @@
     entities_map = {}
 
     for entity in entities:
         nodes[node(entity)] = set()
         entities_map[node(entity)] = entity
 
     for entity in entities:
-        relation_target_ids = [
-            identifier
-            for relation in entity.relations.values()
-            for identifier in relation
-        ]
+        relation_target_ids: list[str] = sum(
+            [
+                identifier if isinstance(identifier, list) else [identifier]
+                for relation in entity.relations.values()
+                for identifier in relation
+                if identifier is not None
+            ],
+            [],
+        )
         related_entities = [
             related for related in entities if related.identifier in relation_target_ids
         ]
 
         for related_entity in related_entities:
             nodes[node(entity)].add(node(related_entity))
```

### Comparing `port_ocean-0.1.4.dev1/port_ocean/core/handlers/entities_state_applier/port/validate_entity_relations.py` & `port_ocean-0.1.4.dev2/port_ocean/core/handlers/entities_state_applier/port/validate_entity_relations.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev1/port_ocean/core/handlers/entity_processor/base.py` & `port_ocean-0.1.4.dev2/port_ocean/core/handlers/entity_processor/base.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev1/port_ocean/core/handlers/entity_processor/jq_entity_processor.py` & `port_ocean-0.1.4.dev2/port_ocean/core/handlers/entity_processor/jq_entity_processor.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev1/port_ocean/core/handlers/port_app_config/base.py` & `port_ocean-0.1.4.dev2/port_ocean/core/handlers/port_app_config/base.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev1/port_ocean/core/handlers/port_app_config/models.py` & `port_ocean-0.1.4.dev2/port_ocean/core/handlers/port_app_config/models.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev1/port_ocean/core/integrations/base.py` & `port_ocean-0.1.4.dev2/port_ocean/core/integrations/base.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev1/port_ocean/core/integrations/mixins/events.py` & `port_ocean-0.1.4.dev2/port_ocean/core/integrations/mixins/events.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev1/port_ocean/core/integrations/mixins/handler.py` & `port_ocean-0.1.4.dev2/port_ocean/core/integrations/mixins/handler.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev1/port_ocean/core/integrations/mixins/sync.py` & `port_ocean-0.1.4.dev2/port_ocean/core/integrations/mixins/sync.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev1/port_ocean/core/integrations/mixins/utils.py` & `port_ocean-0.1.4.dev2/port_ocean/core/integrations/mixins/utils.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev1/port_ocean/core/models.py` & `port_ocean-0.1.4.dev2/port_ocean/core/models.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev1/port_ocean/core/ocean_types.py` & `port_ocean-0.1.4.dev2/port_ocean/core/ocean_types.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev1/port_ocean/core/utils.py` & `port_ocean-0.1.4.dev2/port_ocean/core/utils.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev1/port_ocean/exceptions/core.py` & `port_ocean-0.1.4.dev2/port_ocean/exceptions/core.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev1/port_ocean/logger_setup.py` & `port_ocean-0.1.4.dev2/port_ocean/logger_setup.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev1/port_ocean/middlewares.py` & `port_ocean-0.1.4.dev2/port_ocean/middlewares.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev1/port_ocean/ocean.py` & `port_ocean-0.1.4.dev2/port_ocean/ocean.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev1/port_ocean/port_defaults.py` & `port_ocean-0.1.4.dev2/port_ocean/port_defaults.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev1/port_ocean/run.py` & `port_ocean-0.1.4.dev2/port_ocean/run.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev1/port_ocean/utils.py` & `port_ocean-0.1.4.dev2/port_ocean/utils.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev1/pyproject.toml` & `port_ocean-0.1.4.dev2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "port-ocean"
-version = "0.1.4dev1"
+version = "0.1.4dev2"
 description = "Port Ocean is a CLI tool for managing your Port projects."
 readme = "README.md"
 homepage = "https://app.getport.io"
 repository = "https://github.com/port-labs/Port-Ocean"
 
 authors = ["Daniel Sinai <daniel@getport.io>", "Yair Siman-Tov <yair@getport.io>"]
 packages = [
```

### Comparing `port_ocean-0.1.4.dev1/PKG-INFO` & `port_ocean-0.1.4.dev2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: port-ocean
-Version: 0.1.4.dev1
+Version: 0.1.4.dev2
 Summary: Port Ocean is a CLI tool for managing your Port projects.
 Home-page: https://app.getport.io
 Keywords: ocean,port-ocean,port
 Author: Daniel Sinai
 Author-email: daniel@getport.io
 Requires-Python: >=3.11,<4.0
 Classifier: Framework :: FastAPI
```

