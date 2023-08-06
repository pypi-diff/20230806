# Comparing `tmp/dagworks-sdk-0.0.11.tar.gz` & `tmp/dagworks-sdk-0.0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagworks-sdk-0.0.11.tar", last modified: Tue Jul  4 03:34:45 2023, max compression
+gzip compressed data, was "dagworks-sdk-0.0.12.tar", last modified: Sun Aug  6 06:00:15 2023, max compression
```

## Comparing `dagworks-sdk-0.0.11.tar` & `dagworks-sdk-0.0.12.tar`

### file list

```diff
@@ -1,189 +1,189 @@
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-07-04 03:34:45.341473 dagworks-sdk-0.0.11/
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2212 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/LICENSE
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     4696 2023-07-04 03:34:45.341335 dagworks-sdk-0.0.11/PKG-INFO
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     3655 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/README.md
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1898 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/pyproject.toml
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)       14 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/requirements-test.txt
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      221 2023-07-04 03:29:29.000000 dagworks-sdk-0.0.11/requirements.txt
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)       38 2023-07-04 03:34:45.341518 dagworks-sdk-0.0.11/setup.cfg
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      115 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/setup.py
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-07-04 03:34:45.319970 dagworks-sdk-0.0.11/src/
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-07-04 03:34:45.320989 dagworks-sdk-0.0.11/src/dagworks/
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1093 2023-07-04 03:29:29.000000 dagworks-sdk-0.0.11/src/dagworks/__init__.py
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-07-04 03:34:45.321445 dagworks-sdk-0.0.11/src/dagworks/api/
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1067 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/__init__.py
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-07-04 03:34:45.321905 dagworks-sdk-0.0.11/src/dagworks/api/api_client/
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      152 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/__init__.py
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-07-04 03:34:45.322026 dagworks-sdk-0.0.11/src/dagworks/api/api_client/api/
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)       47 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/api/__init__.py
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-07-04 03:34:45.322714 dagworks-sdk-0.0.11/src/dagworks/api/api_client/api/auth/
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)        0 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/api/auth/__init__.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     3379 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/api/auth/trackingserver_api_api_create_api_key.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2926 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/api/auth/trackingserver_api_api_delete_api_key.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     5383 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/api/auth/trackingserver_api_api_get_api_keys.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     4111 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/api/auth/trackingserver_api_api_phone_home.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     4813 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/api/auth/trackingserver_api_api_whoami.py
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-07-04 03:34:45.324143 dagworks-sdk-0.0.11/src/dagworks/api/api_client/api/projects/
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)        0 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/api/projects/__init__.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     3035 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/api/projects/trackingserver_api_api_archive_project_version.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     5855 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/api/projects/trackingserver_api_api_create_project.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     4711 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/api/projects/trackingserver_api_api_create_project_version.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     5053 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_latest_project_version.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     4516 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_by_id.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     4994 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_version.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     8029 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_versions.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     5693 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_versions_bulk_by_id.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     5511 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_projects.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     5779 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_projects_by_name.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     6327 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/api/projects/trackingserver_api_api_update_project.py
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-07-04 03:34:45.324802 dagworks-sdk-0.0.11/src/dagworks/api/api_client/api/runs/
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)        0 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/api/runs/__init__.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     4421 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_run.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     5087 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_runs.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     6058 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_runs_from_project.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     6286 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_runs_from_project_version.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     5367 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/api/runs/trackingserver_api_api_log_run.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2817 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/client.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      470 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/errors.py
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-07-04 03:34:45.331999 dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     4237 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/__init__.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2443 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/api_key_out.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1982 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/dependency.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2706 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/documentation_asset_in.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1285 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/documentation_asset_in_documentation.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     3019 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/documentation_asset_out.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1268 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/documentation_asset_out_documentation.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2766 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/hamilton_dag.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2480 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/hamilton_function.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     3778 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/hamilton_node.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1692 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/hamilton_node_dependencies.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1175 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/hamilton_node_tags.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1898 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/organization_out.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2231 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/paged_api_key_out.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2238 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/paged_project_out.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2231 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/paged_run_log_out.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1649 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/phone_home_result.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1977 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/project_in.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1179 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/project_in_tags.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     4499 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/project_out.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1165 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/project_out_tags.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     3909 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/project_version_in_git.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1241 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/project_version_in_git_dag.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1243 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/project_version_in_git_tags.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     5339 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/project_version_out.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1203 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/project_version_out_tags.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1241 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/project_version_out_version_info.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     5848 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/project_version_out_with_dag.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1244 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/project_version_out_with_dag_tags.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1282 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/project_version_out_with_dag_version_info.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1422 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/python_type.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1791 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/run_log_data.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     5416 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/run_log_in.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1204 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/run_log_in_config.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1185 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/run_log_in_inputs.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1171 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/run_log_in_run_log.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1173 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/run_log_in_tags.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     6517 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/run_log_out.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1173 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/run_log_out_config.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1173 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/run_log_out_inputs.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1163 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/run_log_out_tags.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     7054 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/run_log_out_with_run.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1214 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/run_log_out_with_run_config.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1214 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/run_log_out_with_run_inputs.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1204 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/run_log_out_with_run_tags.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     3710 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/task_run.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1198 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/task_run_result_summary.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      226 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/task_run_status.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     3189 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/trackingserver_api_api_create_project_body_params.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2916 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/trackingserver_api_api_update_project_body_params.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1586 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/user_out.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     4362 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/visibility_full.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     3802 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/visibility_in.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2306 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/who_am_i_result.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      993 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/api_client/types.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     9831 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/clients.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1161 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/constants.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1311 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/api/projecttypes.py
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-07-04 03:34:45.332417 dagworks-sdk-0.0.11/src/dagworks/cli/
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1067 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/cli/__init__.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2025 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/cli/cli.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     6513 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/cli/initialize.py
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-07-04 03:34:45.332561 dagworks-sdk-0.0.11/src/dagworks/cli/templates/
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)        0 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/cli/templates/__init__.py
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-07-04 03:34:45.333222 dagworks-sdk-0.0.11/src/dagworks/cli/templates/common/
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      123 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/cli/templates/common/.env.jinja2
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      307 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/cli/templates/common/README.md.jinja2
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)       51 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/cli/templates/common/requirements.txt.jinja2
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2698 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/cli/templates/common/run.py.jinja2
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      697 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/cli/templates/common/run.sh.jinja2
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-07-04 03:34:45.333359 dagworks-sdk-0.0.11/src/dagworks/cli/templates/data_processing/
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-07-04 03:34:45.333911 dagworks-sdk-0.0.11/src/dagworks/cli/templates/data_processing/components/
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)        0 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/cli/templates/data_processing/components/__init__.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      351 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/cli/templates/data_processing/components/_run.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      520 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/cli/templates/data_processing/components/common.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2528 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/cli/templates/data_processing/components/data_loader.py
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-07-04 03:34:45.334046 dagworks-sdk-0.0.11/src/dagworks/cli/templates/data_processing/config/
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)       26 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/cli/templates/data_processing/config/config.json
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-07-04 03:34:45.334494 dagworks-sdk-0.0.11/src/dagworks/cli/templates/data_processing/data/
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      232 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/cli/templates/data_processing/data/order_details.csv
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      480 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/cli/templates/data_processing/data/orders_new.csv
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      309 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/cli/templates/data_processing/data/orders_old.csv
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      678 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/cli/templates/data_processing/template_data.json
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-07-04 03:34:45.334644 dagworks-sdk-0.0.11/src/dagworks/cli/templates/hello_world/
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-07-04 03:34:45.334936 dagworks-sdk-0.0.11/src/dagworks/cli/templates/hello_world/components/
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)        0 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/cli/templates/hello_world/components/__init__.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1577 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/cli/templates/hello_world/components/transforms.py
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-07-04 03:34:45.335369 dagworks-sdk-0.0.11/src/dagworks/cli/templates/hello_world/data/
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      157 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/cli/templates/hello_world/data/signups.csv
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      149 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/cli/templates/hello_world/data/spend.csv
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      674 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/cli/templates/hello_world/template_data.json
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-07-04 03:34:45.335583 dagworks-sdk-0.0.11/src/dagworks/cli/templates/machine_learning/
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-07-04 03:34:45.336675 dagworks-sdk-0.0.11/src/dagworks/cli/templates/machine_learning/components/
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)        0 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/cli/templates/machine_learning/components/__init__.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      488 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/cli/templates/machine_learning/components/_run.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     3736 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/cli/templates/machine_learning/components/feature_transforms.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      598 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/cli/templates/machine_learning/components/iris_loader.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2531 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/cli/templates/machine_learning/components/model_fitting.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1402 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/cli/templates/machine_learning/components/models.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      477 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/cli/templates/machine_learning/template_data.json
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-07-04 03:34:45.336821 dagworks-sdk-0.0.11/src/dagworks/cli/templates/time_series_feature_engineering/
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-07-04 03:34:45.337572 dagworks-sdk-0.0.11/src/dagworks/cli/templates/time_series_feature_engineering/components/
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)        0 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/cli/templates/time_series_feature_engineering/components/__init__.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1447 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/cli/templates/time_series_feature_engineering/components/_run.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      369 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/cli/templates/time_series_feature_engineering/components/data_loader.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      710 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_autoregression.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      931 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_calendar.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      744 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_common_prep.py
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-07-04 03:34:45.337693 dagworks-sdk-0.0.11/src/dagworks/cli/templates/time_series_feature_engineering/data/
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)   991302 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/cli/templates/time_series_feature_engineering/data/train_sample.csv
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      679 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/cli/templates/time_series_feature_engineering/template_data.json
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)    14619 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/driver.py
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-07-04 03:34:45.338595 dagworks-sdk-0.0.11/src/dagworks/parsing/
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1067 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/parsing/__init__.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2394 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/parsing/dagtypes.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     6979 2023-07-04 03:29:29.000000 dagworks-sdk-0.0.11/src/dagworks/parsing/parse.py
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-07-04 03:34:45.338803 dagworks-sdk-0.0.11/src/dagworks/telemetry/
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1067 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/telemetry/__init__.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     7465 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/telemetry/telemetry.py
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-07-04 03:34:45.339858 dagworks-sdk-0.0.11/src/dagworks/tracking/
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1067 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/tracking/__init__.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     3486 2023-06-22 18:14:39.000000 dagworks-sdk-0.0.11/src/dagworks/tracking/dataframe_stats.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     5969 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/tracking/example_tracking.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     6307 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/tracking/pandas_col_stats.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     5691 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/tracking/pandas_stats.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     7107 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/tracking/polars_col_stats.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     5549 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/tracking/polars_stats.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     9073 2023-06-22 18:38:45.000000 dagworks-sdk-0.0.11/src/dagworks/tracking/runs.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2827 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/tracking/stats.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2411 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/src/dagworks/tracking/trackingtypes.py
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-07-04 03:34:45.340826 dagworks-sdk-0.0.11/src/dagworks_sdk.egg-info/
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     4696 2023-07-04 03:34:45.000000 dagworks-sdk-0.0.11/src/dagworks_sdk.egg-info/PKG-INFO
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     8764 2023-07-04 03:34:45.000000 dagworks-sdk-0.0.11/src/dagworks_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)        1 2023-07-04 03:34:45.000000 dagworks-sdk-0.0.11/src/dagworks_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)       50 2023-07-04 03:34:45.000000 dagworks-sdk-0.0.11/src/dagworks_sdk.egg-info/entry_points.txt
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)      200 2023-07-04 03:34:45.000000 dagworks-sdk-0.0.11/src/dagworks_sdk.egg-info/requires.txt
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)        9 2023-07-04 03:34:45.000000 dagworks-sdk-0.0.11/src/dagworks_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-07-04 03:34:45.341154 dagworks-sdk-0.0.11/tests/
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2970 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/tests/test_driver.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     3343 2023-06-22 18:14:32.000000 dagworks-sdk-0.0.11/tests/test_telemetry.py
--rw-r--r--   0 elijahbenizzy   (501) staff       (20)     6185 2023-06-22 18:38:45.000000 dagworks-sdk-0.0.11/tests/test_tracking.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-08-06 06:00:15.292690 dagworks-sdk-0.0.12/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2212 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/LICENSE
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4696 2023-08-06 06:00:15.292456 dagworks-sdk-0.0.12/PKG-INFO
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3655 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/README.md
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1898 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/pyproject.toml
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)       14 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/requirements-test.txt
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      221 2023-08-06 05:59:18.000000 dagworks-sdk-0.0.12/requirements.txt
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)       38 2023-08-06 06:00:15.292798 dagworks-sdk-0.0.12/setup.cfg
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      115 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/setup.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-08-06 06:00:15.238450 dagworks-sdk-0.0.12/src/
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-08-06 06:00:15.240550 dagworks-sdk-0.0.12/src/dagworks/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1093 2023-08-06 05:59:25.000000 dagworks-sdk-0.0.12/src/dagworks/__init__.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-08-06 06:00:15.241536 dagworks-sdk-0.0.12/src/dagworks/api/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1067 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/__init__.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-08-06 06:00:15.242601 dagworks-sdk-0.0.12/src/dagworks/api/api_client/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      152 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/__init__.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-08-06 06:00:15.242841 dagworks-sdk-0.0.12/src/dagworks/api/api_client/api/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)       47 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/api/__init__.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-08-06 06:00:15.244329 dagworks-sdk-0.0.12/src/dagworks/api/api_client/api/auth/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/api/auth/__init__.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3379 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/api/auth/trackingserver_api_api_create_api_key.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2926 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/api/auth/trackingserver_api_api_delete_api_key.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5383 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/api/auth/trackingserver_api_api_get_api_keys.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4111 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/api/auth/trackingserver_api_api_phone_home.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4813 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/api/auth/trackingserver_api_api_whoami.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-08-06 06:00:15.248480 dagworks-sdk-0.0.12/src/dagworks/api/api_client/api/projects/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/api/projects/__init__.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3035 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/api/projects/trackingserver_api_api_archive_project_version.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5855 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/api/projects/trackingserver_api_api_create_project.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4711 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/api/projects/trackingserver_api_api_create_project_version.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5053 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_latest_project_version.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4516 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_by_id.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4994 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_version.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     8029 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_versions.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5693 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_versions_bulk_by_id.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5511 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_projects.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5779 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_projects_by_name.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     6327 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/api/projects/trackingserver_api_api_update_project.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-08-06 06:00:15.250198 dagworks-sdk-0.0.12/src/dagworks/api/api_client/api/runs/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/api/runs/__init__.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4421 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_run.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5087 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_runs.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     6058 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_runs_from_project.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     6286 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_runs_from_project_version.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5367 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/api/runs/trackingserver_api_api_log_run.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2817 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/client.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      470 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/errors.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-08-06 06:00:15.267227 dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4237 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/__init__.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2443 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/api_key_out.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1982 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/dependency.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2706 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/documentation_asset_in.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1285 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/documentation_asset_in_documentation.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3019 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/documentation_asset_out.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1268 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/documentation_asset_out_documentation.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2766 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/hamilton_dag.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2480 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/hamilton_function.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3778 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/hamilton_node.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1692 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/hamilton_node_dependencies.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1175 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/hamilton_node_tags.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1898 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/organization_out.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2231 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/paged_api_key_out.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2238 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/paged_project_out.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2231 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/paged_run_log_out.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1649 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/phone_home_result.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1977 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/project_in.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1179 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/project_in_tags.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4499 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/project_out.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1165 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/project_out_tags.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3909 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/project_version_in_git.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1241 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/project_version_in_git_dag.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1243 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/project_version_in_git_tags.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5339 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/project_version_out.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1203 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/project_version_out_tags.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1241 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/project_version_out_version_info.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5848 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/project_version_out_with_dag.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1244 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/project_version_out_with_dag_tags.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1282 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/project_version_out_with_dag_version_info.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1422 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/python_type.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1791 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/run_log_data.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5416 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/run_log_in.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1204 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/run_log_in_config.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1185 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/run_log_in_inputs.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1171 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/run_log_in_run_log.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1173 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/run_log_in_tags.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     6517 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/run_log_out.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1173 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/run_log_out_config.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1173 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/run_log_out_inputs.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1163 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/run_log_out_tags.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     7054 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/run_log_out_with_run.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1214 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/run_log_out_with_run_config.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1214 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/run_log_out_with_run_inputs.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1204 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/run_log_out_with_run_tags.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3710 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/task_run.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1198 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/task_run_result_summary.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      226 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/task_run_status.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3189 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/trackingserver_api_api_create_project_body_params.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2916 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/trackingserver_api_api_update_project_body_params.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1586 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/user_out.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4362 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/visibility_full.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3802 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/visibility_in.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2306 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/who_am_i_result.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      993 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/api_client/types.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     9831 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/clients.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1161 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/constants.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1311 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/api/projecttypes.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-08-06 06:00:15.268209 dagworks-sdk-0.0.12/src/dagworks/cli/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1067 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/cli/__init__.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2025 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/cli/cli.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     6513 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/cli/initialize.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-08-06 06:00:15.268614 dagworks-sdk-0.0.12/src/dagworks/cli/templates/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/cli/templates/__init__.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-08-06 06:00:15.270679 dagworks-sdk-0.0.12/src/dagworks/cli/templates/common/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      123 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/cli/templates/common/.env.jinja2
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      307 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/cli/templates/common/README.md.jinja2
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)       51 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/cli/templates/common/requirements.txt.jinja2
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2698 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/cli/templates/common/run.py.jinja2
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      697 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/cli/templates/common/run.sh.jinja2
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-08-06 06:00:15.271214 dagworks-sdk-0.0.12/src/dagworks/cli/templates/data_processing/
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-08-06 06:00:15.273070 dagworks-sdk-0.0.12/src/dagworks/cli/templates/data_processing/components/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/cli/templates/data_processing/components/__init__.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      351 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/cli/templates/data_processing/components/_run.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      520 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/cli/templates/data_processing/components/common.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2528 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/cli/templates/data_processing/components/data_loader.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-08-06 06:00:15.273584 dagworks-sdk-0.0.12/src/dagworks/cli/templates/data_processing/config/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)       26 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/cli/templates/data_processing/config/config.json
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-08-06 06:00:15.274917 dagworks-sdk-0.0.12/src/dagworks/cli/templates/data_processing/data/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      232 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/cli/templates/data_processing/data/order_details.csv
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      480 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/cli/templates/data_processing/data/orders_new.csv
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      309 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/cli/templates/data_processing/data/orders_old.csv
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      678 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/cli/templates/data_processing/template_data.json
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-08-06 06:00:15.275335 dagworks-sdk-0.0.12/src/dagworks/cli/templates/hello_world/
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-08-06 06:00:15.276143 dagworks-sdk-0.0.12/src/dagworks/cli/templates/hello_world/components/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/cli/templates/hello_world/components/__init__.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1577 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/cli/templates/hello_world/components/transforms.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-08-06 06:00:15.277003 dagworks-sdk-0.0.12/src/dagworks/cli/templates/hello_world/data/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      157 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/cli/templates/hello_world/data/signups.csv
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      149 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/cli/templates/hello_world/data/spend.csv
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      674 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/cli/templates/hello_world/template_data.json
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-08-06 06:00:15.277444 dagworks-sdk-0.0.12/src/dagworks/cli/templates/machine_learning/
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-08-06 06:00:15.280256 dagworks-sdk-0.0.12/src/dagworks/cli/templates/machine_learning/components/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/cli/templates/machine_learning/components/__init__.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      488 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/cli/templates/machine_learning/components/_run.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3736 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/cli/templates/machine_learning/components/feature_transforms.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      598 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/cli/templates/machine_learning/components/iris_loader.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2531 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/cli/templates/machine_learning/components/model_fitting.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1402 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/cli/templates/machine_learning/components/models.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      477 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/cli/templates/machine_learning/template_data.json
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-08-06 06:00:15.280758 dagworks-sdk-0.0.12/src/dagworks/cli/templates/time_series_feature_engineering/
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-08-06 06:00:15.283559 dagworks-sdk-0.0.12/src/dagworks/cli/templates/time_series_feature_engineering/components/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/cli/templates/time_series_feature_engineering/components/__init__.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1447 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/cli/templates/time_series_feature_engineering/components/_run.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      369 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/cli/templates/time_series_feature_engineering/components/data_loader.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      710 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_autoregression.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      931 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_calendar.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      744 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_common_prep.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-08-06 06:00:15.283989 dagworks-sdk-0.0.12/src/dagworks/cli/templates/time_series_feature_engineering/data/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)   991302 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/cli/templates/time_series_feature_engineering/data/train_sample.csv
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      679 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/cli/templates/time_series_feature_engineering/template_data.json
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)    14783 2023-08-06 05:59:18.000000 dagworks-sdk-0.0.12/src/dagworks/driver.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-08-06 06:00:15.285764 dagworks-sdk-0.0.12/src/dagworks/parsing/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1067 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/parsing/__init__.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2394 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/parsing/dagtypes.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     6979 2023-08-06 05:59:18.000000 dagworks-sdk-0.0.12/src/dagworks/parsing/parse.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-08-06 06:00:15.286398 dagworks-sdk-0.0.12/src/dagworks/telemetry/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1067 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/telemetry/__init__.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     7465 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/telemetry/telemetry.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-08-06 06:00:15.289357 dagworks-sdk-0.0.12/src/dagworks/tracking/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1067 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/tracking/__init__.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3486 2023-06-21 04:37:19.000000 dagworks-sdk-0.0.12/src/dagworks/tracking/dataframe_stats.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5969 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/tracking/example_tracking.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     6307 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/tracking/pandas_col_stats.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5691 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/tracking/pandas_stats.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     7107 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/tracking/polars_col_stats.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5549 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/tracking/polars_stats.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     9073 2023-08-06 05:59:18.000000 dagworks-sdk-0.0.12/src/dagworks/tracking/runs.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2827 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/tracking/stats.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2411 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/src/dagworks/tracking/trackingtypes.py
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-08-06 06:00:15.291042 dagworks-sdk-0.0.12/src/dagworks_sdk.egg-info/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4696 2023-08-06 06:00:15.000000 dagworks-sdk-0.0.12/src/dagworks_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     8764 2023-08-06 06:00:15.000000 dagworks-sdk-0.0.12/src/dagworks_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)        1 2023-08-06 06:00:15.000000 dagworks-sdk-0.0.12/src/dagworks_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)       50 2023-08-06 06:00:15.000000 dagworks-sdk-0.0.12/src/dagworks_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)      200 2023-08-06 06:00:15.000000 dagworks-sdk-0.0.12/src/dagworks_sdk.egg-info/requires.txt
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)        9 2023-08-06 06:00:15.000000 dagworks-sdk-0.0.12/src/dagworks_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-08-06 06:00:15.292091 dagworks-sdk-0.0.12/tests/
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3531 2023-08-06 05:59:18.000000 dagworks-sdk-0.0.12/tests/test_driver.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3343 2023-06-21 04:35:00.000000 dagworks-sdk-0.0.12/tests/test_telemetry.py
+-rw-r--r--   0 stefankrawczyk   (501) staff       (20)     6185 2023-08-06 05:59:18.000000 dagworks-sdk-0.0.12/tests/test_tracking.py
```

### Comparing `dagworks-sdk-0.0.11/LICENSE` & `dagworks-sdk-0.0.12/LICENSE`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/PKG-INFO` & `dagworks-sdk-0.0.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagworks-sdk
-Version: 0.0.11
+Version: 0.0.12
 Summary: DAGWorks SDK.
 Author-email: Stefan Krawczyk <stefan@dagworks.io>, Elijah ben Izzy <elijah@dagworks.io>
 Project-URL: Homepage, https://www.dagworks.io
 Project-URL: Bug Reports, https://docs.google.com/forms/d/e/1FAIpQLScS9YvcuNOTretZWXUdur8XNcJPpkJwZwzxuGfbPJKc8IRS6A/viewform
 Project-URL: Source, https://github.com/dagworks-inc/dagworks-sdk/
 Project-URL: Documenation, https://docs.dagworks.io/
 Keywords: hamilton,dagworks,observability
```

### Comparing `dagworks-sdk-0.0.11/README.md` & `dagworks-sdk-0.0.12/README.md`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/pyproject.toml` & `dagworks-sdk-0.0.12/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/__init__.py` & `dagworks-sdk-0.0.12/src/dagworks/api/constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,8 +14,9 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-__version__ = (0, 0, 11)
+DAGWORKS_API_URL = "https://api.app.dagworks.io"
+DAGWORKS_UI_URL = "https://app.dagworks.io"
```

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/__init__.py` & `dagworks-sdk-0.0.12/src/dagworks/api/__init__.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/api/auth/trackingserver_api_api_create_api_key.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/api/auth/trackingserver_api_api_create_api_key.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/api/auth/trackingserver_api_api_delete_api_key.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/api/auth/trackingserver_api_api_delete_api_key.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/api/auth/trackingserver_api_api_get_api_keys.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/api/auth/trackingserver_api_api_get_api_keys.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/api/auth/trackingserver_api_api_phone_home.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/api/auth/trackingserver_api_api_phone_home.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/api/auth/trackingserver_api_api_whoami.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/api/auth/trackingserver_api_api_whoami.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/api/projects/trackingserver_api_api_archive_project_version.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/api/projects/trackingserver_api_api_archive_project_version.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/api/projects/trackingserver_api_api_create_project.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/api/projects/trackingserver_api_api_create_project.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/api/projects/trackingserver_api_api_create_project_version.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/api/projects/trackingserver_api_api_create_project_version.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_latest_project_version.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_latest_project_version.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_by_id.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_by_id.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_version.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_version.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_versions.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_versions.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_versions_bulk_by_id.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_versions_bulk_by_id.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_projects.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_projects.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_projects_by_name.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_projects_by_name.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/api/projects/trackingserver_api_api_update_project.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/api/projects/trackingserver_api_api_update_project.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_run.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_run.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_runs.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_runs.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_runs_from_project.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_runs_from_project.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_runs_from_project_version.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_runs_from_project_version.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/api/runs/trackingserver_api_api_log_run.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/api/runs/trackingserver_api_api_log_run.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/client.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/client.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/__init__.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/api_key_out.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/api_key_out.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/dependency.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/dependency.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/documentation_asset_in.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/documentation_asset_in.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/documentation_asset_in_documentation.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/documentation_asset_in_documentation.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/documentation_asset_out.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/documentation_asset_out.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/documentation_asset_out_documentation.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/documentation_asset_out_documentation.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/hamilton_dag.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/hamilton_dag.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/hamilton_function.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/hamilton_function.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/hamilton_node.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/hamilton_node.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/hamilton_node_dependencies.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/hamilton_node_dependencies.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/hamilton_node_tags.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/hamilton_node_tags.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/organization_out.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/organization_out.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/paged_api_key_out.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/paged_api_key_out.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/paged_project_out.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/paged_project_out.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/paged_run_log_out.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/paged_run_log_out.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/phone_home_result.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/phone_home_result.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/project_in.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/project_in.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/project_in_tags.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/project_in_tags.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/project_out.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/project_out.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/project_out_tags.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/project_out_tags.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/project_version_in_git.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/project_version_in_git.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/project_version_in_git_dag.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/project_version_in_git_dag.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/project_version_in_git_tags.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/project_version_in_git_tags.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/project_version_out.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/project_version_out.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/project_version_out_tags.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/project_version_out_tags.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/project_version_out_version_info.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/project_version_out_version_info.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/project_version_out_with_dag.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/project_version_out_with_dag.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/project_version_out_with_dag_tags.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/project_version_out_with_dag_tags.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/project_version_out_with_dag_version_info.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/project_version_out_with_dag_version_info.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/python_type.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/python_type.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/run_log_data.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/run_log_data.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/run_log_in.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/run_log_in.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/run_log_in_config.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/run_log_in_config.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/run_log_in_inputs.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/run_log_in_inputs.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/run_log_in_run_log.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/run_log_in_run_log.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/run_log_in_tags.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/run_log_in_tags.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/run_log_out.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/run_log_out.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/run_log_out_config.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/run_log_out_config.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/run_log_out_inputs.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/run_log_out_inputs.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/run_log_out_tags.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/run_log_out_tags.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/run_log_out_with_run.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/run_log_out_with_run.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/run_log_out_with_run_config.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/run_log_out_with_run_config.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/run_log_out_with_run_inputs.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/run_log_out_with_run_inputs.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/run_log_out_with_run_tags.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/run_log_out_with_run_tags.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/task_run.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/task_run.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/task_run_result_summary.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/task_run_result_summary.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/trackingserver_api_api_create_project_body_params.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/trackingserver_api_api_create_project_body_params.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/trackingserver_api_api_update_project_body_params.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/trackingserver_api_api_update_project_body_params.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/user_out.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/user_out.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/visibility_full.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/visibility_full.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/visibility_in.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/visibility_in.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/models/who_am_i_result.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/models/who_am_i_result.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/api_client/types.py` & `dagworks-sdk-0.0.12/src/dagworks/api/api_client/types.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/clients.py` & `dagworks-sdk-0.0.12/src/dagworks/api/clients.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/constants.py` & `dagworks-sdk-0.0.12/src/dagworks/cli/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,10 +13,7 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
-
-DAGWORKS_API_URL = "https://api.app.dagworks.io"
-DAGWORKS_UI_URL = "https://app.dagworks.io"
```

### Comparing `dagworks-sdk-0.0.11/src/dagworks/api/projecttypes.py` & `dagworks-sdk-0.0.12/src/dagworks/api/projecttypes.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/cli/__init__.py` & `dagworks-sdk-0.0.12/src/dagworks/parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/cli/cli.py` & `dagworks-sdk-0.0.12/src/dagworks/cli/cli.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/cli/initialize.py` & `dagworks-sdk-0.0.12/src/dagworks/cli/initialize.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/cli/templates/common/run.py.jinja2` & `dagworks-sdk-0.0.12/src/dagworks/cli/templates/common/run.py.jinja2`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/cli/templates/common/run.sh.jinja2` & `dagworks-sdk-0.0.12/src/dagworks/cli/templates/common/run.sh.jinja2`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/cli/templates/data_processing/components/common.py` & `dagworks-sdk-0.0.12/src/dagworks/cli/templates/data_processing/components/common.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/cli/templates/data_processing/components/data_loader.py` & `dagworks-sdk-0.0.12/src/dagworks/cli/templates/data_processing/components/data_loader.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/cli/templates/data_processing/template_data.json` & `dagworks-sdk-0.0.12/src/dagworks/cli/templates/data_processing/template_data.json`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/cli/templates/hello_world/components/transforms.py` & `dagworks-sdk-0.0.12/src/dagworks/cli/templates/hello_world/components/transforms.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/cli/templates/hello_world/template_data.json` & `dagworks-sdk-0.0.12/src/dagworks/cli/templates/hello_world/template_data.json`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/cli/templates/machine_learning/components/feature_transforms.py` & `dagworks-sdk-0.0.12/src/dagworks/cli/templates/machine_learning/components/feature_transforms.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/cli/templates/machine_learning/components/iris_loader.py` & `dagworks-sdk-0.0.12/src/dagworks/cli/templates/machine_learning/components/iris_loader.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/cli/templates/machine_learning/components/model_fitting.py` & `dagworks-sdk-0.0.12/src/dagworks/cli/templates/machine_learning/components/model_fitting.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/cli/templates/machine_learning/components/models.py` & `dagworks-sdk-0.0.12/src/dagworks/cli/templates/machine_learning/components/models.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/cli/templates/time_series_feature_engineering/components/_run.py` & `dagworks-sdk-0.0.12/src/dagworks/cli/templates/time_series_feature_engineering/components/_run.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_autoregression.py` & `dagworks-sdk-0.0.12/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_autoregression.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_calendar.py` & `dagworks-sdk-0.0.12/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_calendar.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_common_prep.py` & `dagworks-sdk-0.0.12/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_common_prep.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/cli/templates/time_series_feature_engineering/data/train_sample.csv` & `dagworks-sdk-0.0.12/src/dagworks/cli/templates/time_series_feature_engineering/data/train_sample.csv`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/cli/templates/time_series_feature_engineering/template_data.json` & `dagworks-sdk-0.0.12/src/dagworks/cli/templates/time_series_feature_engineering/template_data.json`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/driver.py` & `dagworks-sdk-0.0.12/src/dagworks/driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,18 @@
 import json
 import logging
 import os
 import uuid
 from types import ModuleType
 from typing import Any, Callable, Dict, List, Set, Tuple, Union
 
-import git
+try:
+    import git
+except ImportError:
+    git = None
 from hamilton import base, driver
 
 from dagworks.api import clients, constants
 from dagworks.api.projecttypes import GitInfo
 from dagworks.parsing.parse import parse_dag
 from dagworks.telemetry.telemetry import get_adapter_representation, global_tracker
 from dagworks.tracking.runs import Status, TrackingState, monkey_patch_adapter
@@ -55,19 +58,22 @@
     """
     # Check if we've already hashed this module
     if module in seen_modules:
         return hash_object
     else:
         seen_modules.add(module)
     # Update the hash with the module's source code
-    if hasattr(module, "__file__"):
+    if hasattr(module, "__file__") and module.__file__ is not None:
         with open(module.__file__, "rb") as f:
             hash_object.update(f.read())
     else:
-        logger.warning("Skipping hash for module %s because it has no __file__ attribute.", module)
+        logger.debug(
+            "Skipping hash for module %s because it has no __file__ attribute or it is None.",
+            module,
+        )
 
     # Loop through the module's attributes
     for name, value in inspect.getmembers(module):
         # Check if the attribute is a module
         if inspect.ismodule(value):
             # Check if the module is in the same top level package
             if value.__package__ != module.__package__ and not value.__package__.startswith(
@@ -110,35 +116,38 @@
 
 def _derive_version_control_info(module_hash: str) -> GitInfo:
     """Derive the git info for the current project.
     Currently, this decides whether we're in a git repository.
     This is not going to work for everything, but we'll see what the customers want.
     We might end up having to pass this data in...
     """
+    default = GitInfo(
+        branch="unknown",
+        commit_hash=module_hash,
+        committed=False,
+        repository="Error: No repository to link to.",
+        local_repo_base_path=os.getcwd(),
+    )
+    if git is None:
+        return default
     try:
         repo = git.Repo(".", search_parent_directories=True)
     except git.exc.InvalidGitRepositoryError:
         logger.warning(
             "Warning: We are not currently in a git repository. We recommend using that as a "
             "way to version the "
             "project *if* your hamilton code lives within this repository too. If it does not,"
             " then we'll try to "
             "version code based on the python modules passed to the Driver. "
             "Incase you want to get set up with git quickly you can run:\n "
             "git init && git add . && git commit -m 'Initial commit'\n"
             "Still have questions? Reach out to stefan @ dagworks.io, elijah @ dagworks.io "
             "and we'll try to help you as soon as possible."
         )
-        return GitInfo(
-            branch="unknown",
-            commit_hash=module_hash,
-            committed=False,
-            repository="Error: No repository to link to.",
-            local_repo_base_path=os.getcwd(),
-        )
+        return default
 
     commit = repo.head.commit
     try:
         repo_url = repo.remote().url
     except ValueError:
         # TODO: change this to point to our docs on what to do.
         repo_url = "Error: No repository to link to."
```

### Comparing `dagworks-sdk-0.0.11/src/dagworks/parsing/__init__.py` & `dagworks-sdk-0.0.12/src/dagworks/telemetry/__init__.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/parsing/dagtypes.py` & `dagworks-sdk-0.0.12/src/dagworks/parsing/dagtypes.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/parsing/parse.py` & `dagworks-sdk-0.0.12/src/dagworks/parsing/parse.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/telemetry/__init__.py` & `dagworks-sdk-0.0.12/src/dagworks/tracking/__init__.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/telemetry/telemetry.py` & `dagworks-sdk-0.0.12/src/dagworks/telemetry/telemetry.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/tracking/__init__.py` & `dagworks-sdk-0.0.12/src/dagworks/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,7 +13,9 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
+
+__version__ = (0, 0, 12)
```

### Comparing `dagworks-sdk-0.0.11/src/dagworks/tracking/dataframe_stats.py` & `dagworks-sdk-0.0.12/src/dagworks/tracking/dataframe_stats.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/tracking/example_tracking.py` & `dagworks-sdk-0.0.12/src/dagworks/tracking/example_tracking.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/tracking/pandas_col_stats.py` & `dagworks-sdk-0.0.12/src/dagworks/tracking/pandas_col_stats.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/tracking/pandas_stats.py` & `dagworks-sdk-0.0.12/src/dagworks/tracking/pandas_stats.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/tracking/polars_col_stats.py` & `dagworks-sdk-0.0.12/src/dagworks/tracking/polars_col_stats.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/tracking/polars_stats.py` & `dagworks-sdk-0.0.12/src/dagworks/tracking/polars_stats.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/tracking/runs.py` & `dagworks-sdk-0.0.12/src/dagworks/tracking/runs.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/tracking/stats.py` & `dagworks-sdk-0.0.12/src/dagworks/tracking/stats.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks/tracking/trackingtypes.py` & `dagworks-sdk-0.0.12/src/dagworks/tracking/trackingtypes.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/src/dagworks_sdk.egg-info/PKG-INFO` & `dagworks-sdk-0.0.12/src/dagworks_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagworks-sdk
-Version: 0.0.11
+Version: 0.0.12
 Summary: DAGWorks SDK.
 Author-email: Stefan Krawczyk <stefan@dagworks.io>, Elijah ben Izzy <elijah@dagworks.io>
 Project-URL: Homepage, https://www.dagworks.io
 Project-URL: Bug Reports, https://docs.google.com/forms/d/e/1FAIpQLScS9YvcuNOTretZWXUdur8XNcJPpkJwZwzxuGfbPJKc8IRS6A/viewform
 Project-URL: Source, https://github.com/dagworks-inc/dagworks-sdk/
 Project-URL: Documenation, https://docs.dagworks.io/
 Keywords: hamilton,dagworks,observability
```

### Comparing `dagworks-sdk-0.0.11/src/dagworks_sdk.egg-info/SOURCES.txt` & `dagworks-sdk-0.0.12/src/dagworks_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/tests/test_driver.py` & `dagworks-sdk-0.0.12/tests/test_driver.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import hashlib
+import logging
 from types import ModuleType
 from unittest.mock import mock_open, patch
 
 from dagworks.driver import _hash_module
 
 
 @patch("builtins.open", new_callable=mock_open, read_data=b"print('hello world')\n")
@@ -68,15 +69,29 @@
         "tests.test_package_to_hash.submodule2",
         "tests.test_package_to_hash.submodule1",
         "tests.test_package_to_hash.subpackage",
     }
 
 
 def test_hash_module_no_file(caplog):
-    """Tests that we successfully hash a module that has no file."""
+    """Tests that we successfully hash a module that has no file attribute."""
+    caplog.set_level(logging.DEBUG)
     module = ModuleType("mypackage")
     hash_object = hashlib.sha256()
     seen_modules = set()
     result = _hash_module(module, hash_object, seen_modules)
 
     assert "Skipping hash" in caplog.text
     assert result.hexdigest() == "e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855"
+
+
+def test_hash_module_file_is_none(caplog):
+    """Tests that we successfully hash a module that has a file attribute that is None."""
+    caplog.set_level(logging.DEBUG)
+    module = ModuleType("mypackage")
+    module.__file__ = None
+    hash_object = hashlib.sha256()
+    seen_modules = set()
+    result = _hash_module(module, hash_object, seen_modules)
+
+    assert "Skipping hash" in caplog.text
+    assert result.hexdigest() == "e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855"
```

### Comparing `dagworks-sdk-0.0.11/tests/test_telemetry.py` & `dagworks-sdk-0.0.12/tests/test_telemetry.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.11/tests/test_tracking.py` & `dagworks-sdk-0.0.12/tests/test_tracking.py`

 * *Files identical despite different names*

