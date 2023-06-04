# Comparing `tmp/mitzu-0.6.3.tar.gz` & `tmp/mitzu-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mitzu-0.6.3.tar", max compression
+gzip compressed data, was "mitzu-0.6.4.tar", max compression
```

## Comparing `mitzu-0.6.3.tar` & `mitzu-0.6.4.tar`

### file list

```diff
@@ -1,136 +1,136 @@
--rw-r--r--   0        0        0     1082 2023-05-31 12:07:13.017261 mitzu-0.6.3/LICENSE.txt
--rw-r--r--   0        0        0     2235 2023-05-31 12:07:13.017261 mitzu-0.6.3/README.md
--rw-r--r--   0        0        0     6148 2023-05-31 12:07:13.409266 mitzu-0.6.3/mitzu/.DS_Store
--rw-r--r--   0        0        0      752 2023-05-31 12:08:07.509981 mitzu-0.6.3/mitzu/__init__.py
--rw-r--r--   0        0        0        0 2023-05-31 12:07:13.409266 mitzu-0.6.3/mitzu/adapters/__init__.py
--rw-r--r--   0        0        0     1918 2023-05-31 12:07:13.409266 mitzu-0.6.3/mitzu/adapters/adapter_factory.py
--rw-r--r--   0        0        0     5148 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/adapters/athena_adapter.py
--rw-r--r--   0        0        0     6262 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/adapters/bigquery_adapter.py
--rw-r--r--   0        0        0     6026 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/adapters/databricks_adapter.py
--rw-r--r--   0        0        0     2261 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/adapters/file_adapter.py
--rw-r--r--   0        0        0     2533 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/adapters/generic_adapter.py
--rw-r--r--   0        0        0      898 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/adapters/helper.py
--rw-r--r--   0        0        0     3422 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/adapters/mysql_adapter.py
--rw-r--r--   0        0        0     2297 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/adapters/postgresql_adapter.py
--rw-r--r--   0        0        0     3765 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/adapters/redshift_adapter.py
--rw-r--r--   0        0        0     3298 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/adapters/snowflake_adapter.py
--rw-r--r--   0        0        0        0 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/adapters/sqlalchemy/__init__.py
--rw-r--r--   0        0        0        0 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/adapters/sqlalchemy/athena/__init__.py
--rw-r--r--   0        0        0      701 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/adapters/sqlalchemy/athena/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     5071 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/adapters/sqlalchemy/athena/sqlalchemy/compiler.py
--rw-r--r--   0        0        0     6415 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/adapters/sqlalchemy/athena/sqlalchemy/datatype.py
--rw-r--r--   0        0        0     9751 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/adapters/sqlalchemy/athena/sqlalchemy/dialect.py
--rw-r--r--   0        0        0     1844 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/adapters/sqlalchemy/athena/sqlalchemy/error.py
--rw-r--r--   0        0        0        0 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/adapters/sqlalchemy/bigquery/__init__.py
--rw-r--r--   0        0        0     2146 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     2412 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/_helpers.py
--rw-r--r--   0        0        0     5071 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/_struct.py
--rw-r--r--   0        0        0     4770 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/_types.py
--rw-r--r--   0        0        0    38550 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/dialect.py
--rw-r--r--   0        0        0     8638 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/geography.py
--rw-r--r--   0        0        0     9854 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/parse_url.py
--rw-r--r--   0        0        0     7361 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/requirements.py
--rw-r--r--   0        0        0     1131 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/version.py
--rw-r--r--   0        0        0        0 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/adapters/sqlalchemy/databricks/__init__.py
--rw-r--r--   0        0        0      713 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     5010 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/compiler.py
--rw-r--r--   0        0        0     6601 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/datatype.py
--rw-r--r--   0        0        0    10073 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/dialect.py
--rw-r--r--   0        0        0     1848 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/error.py
--rw-r--r--   0        0        0    40105 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/adapters/sqlalchemy_adapter.py
--rw-r--r--   0        0        0     4963 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/adapters/sqlite_adapter.py
--rw-r--r--   0        0        0     7705 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/adapters/trino_adapter.py
--rw-r--r--   0        0        0     1835 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/helper.py
--rw-r--r--   0        0        0    53055 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/model.py
--rw-r--r--   0        0        0        0 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/notebook/__init__.py
--rw-r--r--   0        0        0     6845 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/notebook/model_loader.py
--rw-r--r--   0        0        0     2550 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/project_discovery.py
--rw-r--r--   0        0        0     2102 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/project_serialization.py
--rw-r--r--   0        0        0      785 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/samples/__init__.py
--rw-r--r--   0        0        0     3794 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/samples/data_ingestion.py
--rw-r--r--   0        0        0    10141 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/samples/sample_data_generator.py
--rw-r--r--   0        0        0    11933 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/serialization.py
--rw-r--r--   0        0        0        0 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/visualization/__init__.py
--rw-r--r--   0        0        0     7305 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/visualization/charts.py
--rw-r--r--   0        0        0     1866 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/visualization/common.py
--rw-r--r--   0        0        0      941 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/visualization/labels.py
--rw-r--r--   0        0        0     7802 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/visualization/plot.py
--rw-r--r--   0        0        0     5767 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/visualization/titles.py
--rw-r--r--   0        0        0     3181 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/visualization/tooltips.py
--rw-r--r--   0        0        0     3289 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/visualization/transform_conv.py
--rw-r--r--   0        0        0     1222 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/visualization/transform_retention.py
--rw-r--r--   0        0        0     6148 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/webapp/.DS_Store
--rw-r--r--   0        0        0        0 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/webapp/__init__.py
--rw-r--r--   0        0        0     5347 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/webapp/assets/explore_page.css
--rw-r--r--   0        0        0   147145 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/webapp/assets/favicon.ico
--rw-r--r--   0        0        0    46702 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/webapp/assets/logo.png
--rw-r--r--   0        0        0    43472 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/assets/mitzu-logo-light.svg
--rw-r--r--   0        0        0    49422 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/assets/warehouse/athena.png
--rw-r--r--   0        0        0    20802 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/assets/warehouse/bigquery.png
--rw-r--r--   0        0        0    10321 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/assets/warehouse/clickhouse.png
--rw-r--r--   0        0        0   119554 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/assets/warehouse/databricks.png
--rw-r--r--   0        0        0     3008 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/assets/warehouse/mysql.png
--rw-r--r--   0        0        0     2446 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/assets/warehouse/pandas.png
--rw-r--r--   0        0        0     5338 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/assets/warehouse/postgresql.png
--rw-r--r--   0        0        0     8512 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/assets/warehouse/redshift.png
--rw-r--r--   0        0        0    93500 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/assets/warehouse/snowflake.png
--rw-r--r--   0        0        0    48681 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/assets/warehouse/sqlite.png
--rw-r--r--   0        0        0    34219 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/assets/warehouse/trino.png
--rw-r--r--   0        0        0    15538 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/auth/authorizer.py
--rw-r--r--   0        0        0     3557 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/auth/cognito.py
--rw-r--r--   0        0        0     1305 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/auth/decorator.py
--rw-r--r--   0        0        0     2777 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/auth/google.py
--rw-r--r--   0        0        0     7481 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/cache.py
--rw-r--r--   0        0        0     2920 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/caching_dataset_adapter.py
--rw-r--r--   0        0        0     1664 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/configs.py
--rw-r--r--   0        0        0     3432 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/dependencies.py
--rw-r--r--   0        0        0     4984 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/helper.py
--rw-r--r--   0        0        0     8631 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/model.py
--rw-r--r--   0        0        0      309 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/navbar.py
--rw-r--r--   0        0        0     5435 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/offcanvas.py
--rw-r--r--   0        0        0        0 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/pages/__init__.py
--rw-r--r--   0        0        0        0 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/pages/connections/__init__.py
--rw-r--r--   0        0        0    22704 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/pages/connections/manage_connections_component.py
--rw-r--r--   0        0        0     4428 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/pages/connections_page.py
--rw-r--r--   0        0        0        0 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/pages/dashboards/__init__.py
--rw-r--r--   0        0        0    20561 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/pages/dashboards/manage_dashboards_component.py
--rw-r--r--   0        0        0     9628 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/pages/dashboards_page.py
--rw-r--r--   0        0        0    14456 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/pages/edit_user.py
--rw-r--r--   0        0        0        0 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/pages/explore/__init__.py
--rw-r--r--   0        0        0     5738 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/pages/explore/complex_segment_handler.py
--rw-r--r--   0        0        0     6488 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/pages/explore/dates_selector_handler.py
--rw-r--r--   0        0        0     5564 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/pages/explore/event_segment_handler.py
--rw-r--r--   0        0        0    21704 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/pages/explore/explore_page.py
--rw-r--r--   0        0        0    10100 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/pages/explore/graph_handler.py
--rw-r--r--   0        0        0    10940 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/pages/explore/metric_config_handler.py
--rw-r--r--   0        0        0     2375 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/pages/explore/metric_segments_handler.py
--rw-r--r--   0        0        0     1565 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/pages/explore/metric_type_handler.py
--rw-r--r--   0        0        0     9772 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/pages/explore/simple_segment_handler.py
--rw-r--r--   0        0        0     4644 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/pages/explore/toolbar_handler.py
--rw-r--r--   0        0        0     1221 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/pages/explore_project.py
--rw-r--r--   0        0        0     1751 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/pages/home.py
--rw-r--r--   0        0        0     3947 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/pages/login.py
--rw-r--r--   0        0        0     5023 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/pages/manage_connection.py
--rw-r--r--   0        0        0     1288 2023-05-31 12:07:13.421266 mitzu-0.6.3/mitzu/webapp/pages/manage_dashboard.py
--rw-r--r--   0        0        0    10095 2023-05-31 12:07:13.421266 mitzu-0.6.3/mitzu/webapp/pages/manage_event_defs.py
--rw-r--r--   0        0        0    11845 2023-05-31 12:07:13.421266 mitzu-0.6.3/mitzu/webapp/pages/manage_project.py
--rw-r--r--   0        0        0     9470 2023-05-31 12:07:13.421266 mitzu-0.6.3/mitzu/webapp/pages/manage_saved_metrics.py
--rw-r--r--   0        0        0     1738 2023-05-31 12:07:13.421266 mitzu-0.6.3/mitzu/webapp/pages/paths.py
--rw-r--r--   0        0        0        0 2023-05-31 12:07:13.421266 mitzu-0.6.3/mitzu/webapp/pages/projects/__init__.py
--rw-r--r--   0        0        0    35694 2023-05-31 12:07:13.421266 mitzu-0.6.3/mitzu/webapp/pages/projects/event_tables_config.py
--rw-r--r--   0        0        0      587 2023-05-31 12:07:13.421266 mitzu-0.6.3/mitzu/webapp/pages/projects/helper.py
--rw-r--r--   0        0        0     9400 2023-05-31 12:07:13.421266 mitzu-0.6.3/mitzu/webapp/pages/projects/manage_project_component.py
--rw-r--r--   0        0        0     5090 2023-05-31 12:07:13.421266 mitzu-0.6.3/mitzu/webapp/pages/projects_page.py
--rw-r--r--   0        0        0     3114 2023-05-31 12:07:13.421266 mitzu-0.6.3/mitzu/webapp/pages/users.py
--rw-r--r--   0        0        0        0 2023-05-31 12:07:13.421266 mitzu-0.6.3/mitzu/webapp/service/__init__.py
--rw-r--r--   0        0        0     1955 2023-05-31 12:07:13.421266 mitzu-0.6.3/mitzu/webapp/service/events_service.py
--rw-r--r--   0        0        0     4974 2023-05-31 12:07:13.421266 mitzu-0.6.3/mitzu/webapp/service/navbar_service.py
--rw-r--r--   0        0        0      670 2023-05-31 12:07:13.421266 mitzu-0.6.3/mitzu/webapp/service/notification_service.py
--rw-r--r--   0        0        0     2105 2023-05-31 12:07:13.421266 mitzu-0.6.3/mitzu/webapp/service/secret_service.py
--rw-r--r--   0        0        0     6650 2023-05-31 12:07:13.421266 mitzu-0.6.3/mitzu/webapp/service/tracking_service.py
--rw-r--r--   0        0        0     4755 2023-05-31 12:07:13.421266 mitzu-0.6.3/mitzu/webapp/service/user_service.py
--rw-r--r--   0        0        0    24085 2023-05-31 12:07:13.421266 mitzu-0.6.3/mitzu/webapp/storage.py
--rw-r--r--   0        0        0    25095 2023-05-31 12:07:13.421266 mitzu-0.6.3/mitzu/webapp/storage_model.py
--rw-r--r--   0        0        0     4700 2023-05-31 12:07:13.421266 mitzu-0.6.3/mitzu/webapp/webapp.py
--rw-r--r--   0        0        0     3422 2023-05-31 12:08:07.509981 mitzu-0.6.3/pyproject.toml
--rw-r--r--   0        0        0     5152 1970-01-01 00:00:00.000000 mitzu-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-06-04 08:51:48.002334 mitzu-0.6.4/LICENSE.txt
+-rw-r--r--   0        0        0     2235 2023-06-04 08:51:48.002334 mitzu-0.6.4/README.md
+-rw-r--r--   0        0        0     6148 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/.DS_Store
+-rw-r--r--   0        0        0      752 2023-06-04 08:52:43.019065 mitzu-0.6.4/mitzu/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/__init__.py
+-rw-r--r--   0        0        0     1918 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/adapter_factory.py
+-rw-r--r--   0        0        0     5148 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/athena_adapter.py
+-rw-r--r--   0        0        0     6262 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/bigquery_adapter.py
+-rw-r--r--   0        0        0     6026 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/databricks_adapter.py
+-rw-r--r--   0        0        0     2261 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/file_adapter.py
+-rw-r--r--   0        0        0     2533 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/generic_adapter.py
+-rw-r--r--   0        0        0      898 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/helper.py
+-rw-r--r--   0        0        0     3422 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/mysql_adapter.py
+-rw-r--r--   0        0        0     2297 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/postgresql_adapter.py
+-rw-r--r--   0        0        0     3765 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/redshift_adapter.py
+-rw-r--r--   0        0        0     3298 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/snowflake_adapter.py
+-rw-r--r--   0        0        0        0 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/sqlalchemy/athena/__init__.py
+-rw-r--r--   0        0        0      701 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/sqlalchemy/athena/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     5071 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/sqlalchemy/athena/sqlalchemy/compiler.py
+-rw-r--r--   0        0        0     6415 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/sqlalchemy/athena/sqlalchemy/datatype.py
+-rw-r--r--   0        0        0     9751 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/sqlalchemy/athena/sqlalchemy/dialect.py
+-rw-r--r--   0        0        0     1844 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/sqlalchemy/athena/sqlalchemy/error.py
+-rw-r--r--   0        0        0        0 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/sqlalchemy/bigquery/__init__.py
+-rw-r--r--   0        0        0     2146 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     2412 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/_helpers.py
+-rw-r--r--   0        0        0     5071 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/_struct.py
+-rw-r--r--   0        0        0     4770 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/_types.py
+-rw-r--r--   0        0        0    38550 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/dialect.py
+-rw-r--r--   0        0        0     8638 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/geography.py
+-rw-r--r--   0        0        0     9854 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/parse_url.py
+-rw-r--r--   0        0        0     7361 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/requirements.py
+-rw-r--r--   0        0        0     1131 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/version.py
+-rw-r--r--   0        0        0        0 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/sqlalchemy/databricks/__init__.py
+-rw-r--r--   0        0        0      713 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     5010 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/compiler.py
+-rw-r--r--   0        0        0     6601 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/datatype.py
+-rw-r--r--   0        0        0    10073 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/dialect.py
+-rw-r--r--   0        0        0     1848 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/error.py
+-rw-r--r--   0        0        0    40105 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/sqlalchemy_adapter.py
+-rw-r--r--   0        0        0     4963 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/sqlite_adapter.py
+-rw-r--r--   0        0        0     7705 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/adapters/trino_adapter.py
+-rw-r--r--   0        0        0     1835 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/helper.py
+-rw-r--r--   0        0        0    53055 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/model.py
+-rw-r--r--   0        0        0        0 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/notebook/__init__.py
+-rw-r--r--   0        0        0     6845 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/notebook/model_loader.py
+-rw-r--r--   0        0        0     2550 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/project_discovery.py
+-rw-r--r--   0        0        0     2102 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/project_serialization.py
+-rw-r--r--   0        0        0      785 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/samples/__init__.py
+-rw-r--r--   0        0        0     3794 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/samples/data_ingestion.py
+-rw-r--r--   0        0        0    10141 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/samples/sample_data_generator.py
+-rw-r--r--   0        0        0    11933 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/serialization.py
+-rw-r--r--   0        0        0        0 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/visualization/__init__.py
+-rw-r--r--   0        0        0     7305 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/visualization/charts.py
+-rw-r--r--   0        0        0     1866 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/visualization/common.py
+-rw-r--r--   0        0        0      941 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/visualization/labels.py
+-rw-r--r--   0        0        0     7802 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/visualization/plot.py
+-rw-r--r--   0        0        0     5767 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/visualization/titles.py
+-rw-r--r--   0        0        0     3181 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/visualization/tooltips.py
+-rw-r--r--   0        0        0     3289 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/visualization/transform_conv.py
+-rw-r--r--   0        0        0     1222 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/visualization/transform_retention.py
+-rw-r--r--   0        0        0     6148 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/webapp/.DS_Store
+-rw-r--r--   0        0        0        0 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/webapp/__init__.py
+-rw-r--r--   0        0        0     5347 2023-06-04 08:51:48.398340 mitzu-0.6.4/mitzu/webapp/assets/explore_page.css
+-rw-r--r--   0        0        0   147145 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/assets/favicon.ico
+-rw-r--r--   0        0        0    46702 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/assets/logo.png
+-rw-r--r--   0        0        0    43472 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/assets/mitzu-logo-light.svg
+-rw-r--r--   0        0        0    49422 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/assets/warehouse/athena.png
+-rw-r--r--   0        0        0    20802 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/assets/warehouse/bigquery.png
+-rw-r--r--   0        0        0    10321 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/assets/warehouse/clickhouse.png
+-rw-r--r--   0        0        0   119554 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/assets/warehouse/databricks.png
+-rw-r--r--   0        0        0     3008 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/assets/warehouse/mysql.png
+-rw-r--r--   0        0        0     2446 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/assets/warehouse/pandas.png
+-rw-r--r--   0        0        0     5338 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/assets/warehouse/postgresql.png
+-rw-r--r--   0        0        0     8512 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/assets/warehouse/redshift.png
+-rw-r--r--   0        0        0    93500 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/assets/warehouse/snowflake.png
+-rw-r--r--   0        0        0    48681 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/assets/warehouse/sqlite.png
+-rw-r--r--   0        0        0    34219 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/assets/warehouse/trino.png
+-rw-r--r--   0        0        0    15538 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/auth/authorizer.py
+-rw-r--r--   0        0        0     3557 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/auth/cognito.py
+-rw-r--r--   0        0        0     1305 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/auth/decorator.py
+-rw-r--r--   0        0        0     2777 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/auth/google.py
+-rw-r--r--   0        0        0     7481 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/cache.py
+-rw-r--r--   0        0        0     2920 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/caching_dataset_adapter.py
+-rw-r--r--   0        0        0     1664 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/configs.py
+-rw-r--r--   0        0        0     3432 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/dependencies.py
+-rw-r--r--   0        0        0     4984 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/helper.py
+-rw-r--r--   0        0        0     8631 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/model.py
+-rw-r--r--   0        0        0      309 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/navbar.py
+-rw-r--r--   0        0        0     5435 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/offcanvas.py
+-rw-r--r--   0        0        0        0 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/pages/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/pages/connections/__init__.py
+-rw-r--r--   0        0        0    22704 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/pages/connections/manage_connections_component.py
+-rw-r--r--   0        0        0     4428 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/pages/connections_page.py
+-rw-r--r--   0        0        0        0 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/pages/dashboards/__init__.py
+-rw-r--r--   0        0        0    20561 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/pages/dashboards/manage_dashboards_component.py
+-rw-r--r--   0        0        0     9628 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/pages/dashboards_page.py
+-rw-r--r--   0        0        0    14456 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/pages/edit_user.py
+-rw-r--r--   0        0        0        0 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/pages/explore/__init__.py
+-rw-r--r--   0        0        0     5929 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/pages/explore/complex_segment_handler.py
+-rw-r--r--   0        0        0     6488 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/pages/explore/dates_selector_handler.py
+-rw-r--r--   0        0        0     5790 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/pages/explore/event_segment_handler.py
+-rw-r--r--   0        0        0    22007 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/pages/explore/explore_page.py
+-rw-r--r--   0        0        0    10100 2023-06-04 08:51:48.402340 mitzu-0.6.4/mitzu/webapp/pages/explore/graph_handler.py
+-rw-r--r--   0        0        0    10916 2023-06-04 08:51:48.406340 mitzu-0.6.4/mitzu/webapp/pages/explore/metric_config_handler.py
+-rw-r--r--   0        0        0     2382 2023-06-04 08:51:48.406340 mitzu-0.6.4/mitzu/webapp/pages/explore/metric_segments_handler.py
+-rw-r--r--   0        0        0     1553 2023-06-04 08:51:48.406340 mitzu-0.6.4/mitzu/webapp/pages/explore/metric_type_handler.py
+-rw-r--r--   0        0        0    10285 2023-06-04 08:51:48.406340 mitzu-0.6.4/mitzu/webapp/pages/explore/simple_segment_handler.py
+-rw-r--r--   0        0        0     4644 2023-06-04 08:51:48.406340 mitzu-0.6.4/mitzu/webapp/pages/explore/toolbar_handler.py
+-rw-r--r--   0        0        0     1221 2023-06-04 08:51:48.406340 mitzu-0.6.4/mitzu/webapp/pages/explore_project.py
+-rw-r--r--   0        0        0     1751 2023-06-04 08:51:48.406340 mitzu-0.6.4/mitzu/webapp/pages/home.py
+-rw-r--r--   0        0        0     3947 2023-06-04 08:51:48.406340 mitzu-0.6.4/mitzu/webapp/pages/login.py
+-rw-r--r--   0        0        0     5023 2023-06-04 08:51:48.406340 mitzu-0.6.4/mitzu/webapp/pages/manage_connection.py
+-rw-r--r--   0        0        0     1288 2023-06-04 08:51:48.406340 mitzu-0.6.4/mitzu/webapp/pages/manage_dashboard.py
+-rw-r--r--   0        0        0    10095 2023-06-04 08:51:48.406340 mitzu-0.6.4/mitzu/webapp/pages/manage_event_defs.py
+-rw-r--r--   0        0        0    11845 2023-06-04 08:51:48.406340 mitzu-0.6.4/mitzu/webapp/pages/manage_project.py
+-rw-r--r--   0        0        0     9470 2023-06-04 08:51:48.406340 mitzu-0.6.4/mitzu/webapp/pages/manage_saved_metrics.py
+-rw-r--r--   0        0        0     1738 2023-06-04 08:51:48.406340 mitzu-0.6.4/mitzu/webapp/pages/paths.py
+-rw-r--r--   0        0        0        0 2023-06-04 08:51:48.406340 mitzu-0.6.4/mitzu/webapp/pages/projects/__init__.py
+-rw-r--r--   0        0        0    35694 2023-06-04 08:51:48.406340 mitzu-0.6.4/mitzu/webapp/pages/projects/event_tables_config.py
+-rw-r--r--   0        0        0      587 2023-06-04 08:51:48.406340 mitzu-0.6.4/mitzu/webapp/pages/projects/helper.py
+-rw-r--r--   0        0        0     9400 2023-06-04 08:51:48.406340 mitzu-0.6.4/mitzu/webapp/pages/projects/manage_project_component.py
+-rw-r--r--   0        0        0     5090 2023-06-04 08:51:48.406340 mitzu-0.6.4/mitzu/webapp/pages/projects_page.py
+-rw-r--r--   0        0        0     3114 2023-06-04 08:51:48.406340 mitzu-0.6.4/mitzu/webapp/pages/users.py
+-rw-r--r--   0        0        0        0 2023-06-04 08:51:48.406340 mitzu-0.6.4/mitzu/webapp/service/__init__.py
+-rw-r--r--   0        0        0     1955 2023-06-04 08:51:48.406340 mitzu-0.6.4/mitzu/webapp/service/events_service.py
+-rw-r--r--   0        0        0     4974 2023-06-04 08:51:48.406340 mitzu-0.6.4/mitzu/webapp/service/navbar_service.py
+-rw-r--r--   0        0        0      670 2023-06-04 08:51:48.406340 mitzu-0.6.4/mitzu/webapp/service/notification_service.py
+-rw-r--r--   0        0        0     2105 2023-06-04 08:51:48.406340 mitzu-0.6.4/mitzu/webapp/service/secret_service.py
+-rw-r--r--   0        0        0     6708 2023-06-04 08:51:48.406340 mitzu-0.6.4/mitzu/webapp/service/tracking_service.py
+-rw-r--r--   0        0        0     4755 2023-06-04 08:51:48.406340 mitzu-0.6.4/mitzu/webapp/service/user_service.py
+-rw-r--r--   0        0        0    24085 2023-06-04 08:51:48.406340 mitzu-0.6.4/mitzu/webapp/storage.py
+-rw-r--r--   0        0        0    25095 2023-06-04 08:51:48.406340 mitzu-0.6.4/mitzu/webapp/storage_model.py
+-rw-r--r--   0        0        0     4700 2023-06-04 08:51:48.406340 mitzu-0.6.4/mitzu/webapp/webapp.py
+-rw-r--r--   0        0        0     3422 2023-06-04 08:52:43.015064 mitzu-0.6.4/pyproject.toml
+-rw-r--r--   0        0        0     5152 1970-01-01 00:00:00.000000 mitzu-0.6.4/PKG-INFO
```

### Comparing `mitzu-0.6.3/LICENSE.txt` & `mitzu-0.6.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/README.md` & `mitzu-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/.DS_Store` & `mitzu-0.6.4/mitzu/.DS_Store`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/__init__.py` & `mitzu-0.6.4/mitzu/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     TimeWindow,
     TimeGroup,
     DiscoverySettings,
     WebappSettings,
 )
 from mitzu.samples import get_sample_discovered_project
 
-__version__ = "0.6.3"
+__version__ = "0.6.4"
 
 
 __all__ = [
     "Connection",
     "ConnectionType",
     "Project",
     "EventDataTable",
```

### Comparing `mitzu-0.6.3/mitzu/adapters/adapter_factory.py` & `mitzu-0.6.4/mitzu/adapters/adapter_factory.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/adapters/athena_adapter.py` & `mitzu-0.6.4/mitzu/adapters/athena_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/adapters/bigquery_adapter.py` & `mitzu-0.6.4/mitzu/adapters/bigquery_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/adapters/databricks_adapter.py` & `mitzu-0.6.4/mitzu/adapters/databricks_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/adapters/file_adapter.py` & `mitzu-0.6.4/mitzu/adapters/file_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/adapters/generic_adapter.py` & `mitzu-0.6.4/mitzu/adapters/generic_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/adapters/helper.py` & `mitzu-0.6.4/mitzu/adapters/helper.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/adapters/mysql_adapter.py` & `mitzu-0.6.4/mitzu/adapters/mysql_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/adapters/postgresql_adapter.py` & `mitzu-0.6.4/mitzu/adapters/postgresql_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/adapters/redshift_adapter.py` & `mitzu-0.6.4/mitzu/adapters/redshift_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/adapters/snowflake_adapter.py` & `mitzu-0.6.4/mitzu/adapters/snowflake_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/adapters/sqlalchemy/athena/sqlalchemy/__init__.py` & `mitzu-0.6.4/mitzu/adapters/sqlalchemy/athena/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/adapters/sqlalchemy/athena/sqlalchemy/compiler.py` & `mitzu-0.6.4/mitzu/adapters/sqlalchemy/athena/sqlalchemy/compiler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/adapters/sqlalchemy/athena/sqlalchemy/datatype.py` & `mitzu-0.6.4/mitzu/adapters/sqlalchemy/athena/sqlalchemy/datatype.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/adapters/sqlalchemy/athena/sqlalchemy/dialect.py` & `mitzu-0.6.4/mitzu/adapters/sqlalchemy/athena/sqlalchemy/dialect.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/adapters/sqlalchemy/athena/sqlalchemy/error.py` & `mitzu-0.6.4/mitzu/adapters/sqlalchemy/athena/sqlalchemy/error.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/__init__.py` & `mitzu-0.6.4/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/_helpers.py` & `mitzu-0.6.4/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/_helpers.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/_struct.py` & `mitzu-0.6.4/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/_struct.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/_types.py` & `mitzu-0.6.4/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/_types.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/dialect.py` & `mitzu-0.6.4/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/dialect.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/geography.py` & `mitzu-0.6.4/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/geography.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/parse_url.py` & `mitzu-0.6.4/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/parse_url.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/requirements.py` & `mitzu-0.6.4/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/requirements.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/version.py` & `mitzu-0.6.4/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/version.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/__init__.py` & `mitzu-0.6.4/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/compiler.py` & `mitzu-0.6.4/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/compiler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/datatype.py` & `mitzu-0.6.4/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/datatype.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/dialect.py` & `mitzu-0.6.4/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/dialect.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/error.py` & `mitzu-0.6.4/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/error.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/adapters/sqlalchemy_adapter.py` & `mitzu-0.6.4/mitzu/adapters/sqlalchemy_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/adapters/sqlite_adapter.py` & `mitzu-0.6.4/mitzu/adapters/sqlite_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/adapters/trino_adapter.py` & `mitzu-0.6.4/mitzu/adapters/trino_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/helper.py` & `mitzu-0.6.4/mitzu/helper.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/model.py` & `mitzu-0.6.4/mitzu/model.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/notebook/model_loader.py` & `mitzu-0.6.4/mitzu/notebook/model_loader.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/project_discovery.py` & `mitzu-0.6.4/mitzu/project_discovery.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/project_serialization.py` & `mitzu-0.6.4/mitzu/project_serialization.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/samples/__init__.py` & `mitzu-0.6.4/mitzu/samples/__init__.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/samples/data_ingestion.py` & `mitzu-0.6.4/mitzu/samples/data_ingestion.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/samples/sample_data_generator.py` & `mitzu-0.6.4/mitzu/samples/sample_data_generator.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/serialization.py` & `mitzu-0.6.4/mitzu/serialization.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/visualization/charts.py` & `mitzu-0.6.4/mitzu/visualization/charts.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/visualization/common.py` & `mitzu-0.6.4/mitzu/visualization/common.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/visualization/labels.py` & `mitzu-0.6.4/mitzu/visualization/labels.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/visualization/plot.py` & `mitzu-0.6.4/mitzu/visualization/plot.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/visualization/titles.py` & `mitzu-0.6.4/mitzu/visualization/titles.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/visualization/tooltips.py` & `mitzu-0.6.4/mitzu/visualization/tooltips.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/visualization/transform_conv.py` & `mitzu-0.6.4/mitzu/visualization/transform_conv.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/visualization/transform_retention.py` & `mitzu-0.6.4/mitzu/visualization/transform_retention.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/webapp/.DS_Store` & `mitzu-0.6.4/mitzu/webapp/.DS_Store`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/webapp/assets/explore_page.css` & `mitzu-0.6.4/mitzu/webapp/assets/explore_page.css`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/webapp/assets/favicon.ico` & `mitzu-0.6.4/mitzu/webapp/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/webapp/assets/logo.png` & `mitzu-0.6.4/mitzu/webapp/assets/logo.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/webapp/assets/mitzu-logo-light.svg` & `mitzu-0.6.4/mitzu/webapp/assets/mitzu-logo-light.svg`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/webapp/assets/warehouse/athena.png` & `mitzu-0.6.4/mitzu/webapp/assets/warehouse/athena.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/webapp/assets/warehouse/bigquery.png` & `mitzu-0.6.4/mitzu/webapp/assets/warehouse/bigquery.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/webapp/assets/warehouse/clickhouse.png` & `mitzu-0.6.4/mitzu/webapp/assets/warehouse/clickhouse.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/webapp/assets/warehouse/databricks.png` & `mitzu-0.6.4/mitzu/webapp/assets/warehouse/databricks.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/webapp/assets/warehouse/mysql.png` & `mitzu-0.6.4/mitzu/webapp/assets/warehouse/mysql.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/webapp/assets/warehouse/pandas.png` & `mitzu-0.6.4/mitzu/webapp/assets/warehouse/pandas.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/webapp/assets/warehouse/postgresql.png` & `mitzu-0.6.4/mitzu/webapp/assets/warehouse/postgresql.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/webapp/assets/warehouse/redshift.png` & `mitzu-0.6.4/mitzu/webapp/assets/warehouse/redshift.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/webapp/assets/warehouse/snowflake.png` & `mitzu-0.6.4/mitzu/webapp/assets/warehouse/snowflake.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/webapp/assets/warehouse/sqlite.png` & `mitzu-0.6.4/mitzu/webapp/assets/warehouse/sqlite.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/webapp/assets/warehouse/trino.png` & `mitzu-0.6.4/mitzu/webapp/assets/warehouse/trino.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/webapp/auth/authorizer.py` & `mitzu-0.6.4/mitzu/webapp/auth/authorizer.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/webapp/auth/cognito.py` & `mitzu-0.6.4/mitzu/webapp/auth/cognito.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/webapp/auth/decorator.py` & `mitzu-0.6.4/mitzu/webapp/auth/decorator.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/webapp/auth/google.py` & `mitzu-0.6.4/mitzu/webapp/auth/google.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/webapp/cache.py` & `mitzu-0.6.4/mitzu/webapp/cache.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/webapp/caching_dataset_adapter.py` & `mitzu-0.6.4/mitzu/webapp/caching_dataset_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/webapp/configs.py` & `mitzu-0.6.4/mitzu/webapp/configs.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/webapp/dependencies.py` & `mitzu-0.6.4/mitzu/webapp/dependencies.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/webapp/helper.py` & `mitzu-0.6.4/mitzu/webapp/helper.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/webapp/model.py` & `mitzu-0.6.4/mitzu/webapp/model.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/webapp/offcanvas.py` & `mitzu-0.6.4/mitzu/webapp/offcanvas.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/webapp/pages/connections/manage_connections_component.py` & `mitzu-0.6.4/mitzu/webapp/pages/connections/manage_connections_component.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/webapp/pages/connections_page.py` & `mitzu-0.6.4/mitzu/webapp/pages/connections_page.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/webapp/pages/dashboards/manage_dashboards_component.py` & `mitzu-0.6.4/mitzu/webapp/pages/dashboards/manage_dashboards_component.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/webapp/pages/dashboards_page.py` & `mitzu-0.6.4/mitzu/webapp/pages/dashboards_page.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/webapp/pages/edit_user.py` & `mitzu-0.6.4/mitzu/webapp/pages/edit_user.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/webapp/pages/explore/complex_segment_handler.py` & `mitzu-0.6.4/mitzu/webapp/pages/explore/complex_segment_handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -97,15 +97,15 @@
     discovered_project: M.DiscoveredProject,
     funnel_step: int,
     metric: Optional[M.Metric],
     segment: Optional[M.Segment],
     metric_type: MTH.MetricType,
 ) -> bc.Component:
     type_index = str(funnel_step)
-    if metric_type == MTH.MetricType.CONVERSION:
+    if metric_type == MTH.MetricType.FUNNEL:
         title = f"{funnel_step+1}. Step"
     elif metric_type == MTH.MetricType.RETENTION:
         title = "Initial Step" if funnel_step == 0 else "Retaining Step"
     else:
         title = "Events"
 
     header = dbc.CardHeader(title, class_name="p-2 fw-bold")
@@ -146,20 +146,27 @@
         className=COMPLEX_SEGMENT + " p-0",
     )
 
 
 def from_all_inputs(
     discovered_project: M.DiscoveredProject,
     complex_segment: Dict[str, Any],
+    complex_segment_index: int,
 ) -> Optional[M.Segment]:
     res_segment: Optional[M.Segment] = None
     event_segments = complex_segment.get(CHILDREN, {})
-
+    event_segment_index = 0
     for _, event_segment in event_segments.items():
-        event_segment = ES.from_all_inputs(discovered_project, event_segment)
+        event_segment = ES.from_all_inputs(
+            discovered_project,
+            event_segment,
+            complex_segment_index,
+            event_segment_index,
+        )
+        event_segment_index += 1
         if event_segment is None:
             continue
         if res_segment is None:
             res_segment = event_segment
         else:
             res_segment = res_segment | event_segment
```

### Comparing `mitzu-0.6.3/mitzu/webapp/pages/explore/dates_selector_handler.py` & `mitzu-0.6.4/mitzu/webapp/pages/explore/dates_selector_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/webapp/pages/explore/event_segment_handler.py` & `mitzu-0.6.4/mitzu/webapp/pages/explore/event_segment_handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -143,26 +143,36 @@
     )
     return component
 
 
 def from_all_inputs(
     discovered_project: Optional[M.DiscoveredProject],
     event_segment: Dict[str, Any],
+    complex_segment_index: int,
+    event_segment_index: int,
 ) -> Optional[M.Segment]:
     if discovered_project is None:
         return None
     event_name_dd_value = event_segment.get(EVENT_NAME_DROPDOWN)
     simple_segments = event_segment.get(CHILDREN, {})
 
     if event_name_dd_value is None:
         return None
 
     res_segment: Optional[M.Segment] = None
+    ss_index = 0
     for _, simple_segment in simple_segments.items():
-        simple_seg = SS.from_all_inputs(discovered_project, simple_segment)
+        simple_seg = SS.from_all_inputs(
+            discovered_project,
+            simple_segment,
+            complex_segment_index,
+            event_segment_index,
+            ss_index,
+        )
+        ss_index += 1
 
         if simple_seg is None:
             continue
         if simple_seg._left._event_name != event_name_dd_value:
             continue
 
         if res_segment is None:
```

### Comparing `mitzu-0.6.3/mitzu/webapp/pages/explore/explore_page.py` & `mitzu-0.6.4/mitzu/webapp/pages/explore/explore_page.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 import mitzu.webapp.storage as S
 from mitzu.webapp.helper import MITZU_LOCATION, find_event_field_def, CHILDREN
 import mitzu.webapp.pages.paths as P
 import traceback
 from dash import ctx, html, callback, no_update, dcc
 from dash.dependencies import ALL, Input, Output, State
 from mitzu.webapp.auth.decorator import restricted
-
+import flask
 
 from mitzu.webapp.helper import (
     get_final_all_inputs,
 )
 
 NAVBAR_ID = "explore_navbar"
 SHARE_BUTTON = "share_button"
@@ -104,32 +104,35 @@
         size="sm",
         color="success",
         id=METRIC_SAVE_NAVBAR_BUTTON,
     )
 
 
 def share_button_navbar_provider(
-    id: str, notebook_mode: bool = True, **kwargs
+    id: str, show_share_button=False, path="", **kwargs
 ) -> Optional[bc.Component]:
+    if not show_share_button:
+        return None
+    url = flask.request.host_url.strip("/") + path
     return (
         dbc.Button(
             [
                 html.B(className="bi bi-link-45deg"),
                 " Share",
                 dcc.Clipboard(
                     id=CLIPBOARD,
-                    content="",
+                    content=url,
                     className="position-absolute start-0 top-0 w-100 h-100 opacity-0",
                 ),
             ],
             id=SHARE_BUTTON,
             className="position-relative top-0 start-0 text-nowrap",
             color="light",
             size="sm",
-            style={"display": "none" if notebook_mode else "inline-block"},
+            style={"display": "inline-block"},
         ),
     )
 
 
 def create_saved_metric_dialog(saved_metric: Optional[WM.SavedMetric]) -> dbc.Modal:
     return dbc.Modal(
         [
@@ -193,15 +196,14 @@
     )
 
 
 def create_explore_page(
     query_params: Dict[str, str],
     discovered_project: M.DiscoveredProject,
     storage: S.MitzuStorage,
-    notebook_mode: bool = False,
 ) -> bc.Component:
     metric: Optional[M.Metric] = None
     saved_metric: Optional[WM.SavedMetric] = None
     if P.PROJECTS_EXPLORE_METRIC_QUERY in query_params:
         try:
             metric = SE.from_compressed_string(
                 query_params[P.PROJECTS_EXPLORE_METRIC_QUERY],
@@ -215,21 +217,29 @@
             query_params[P.PROJECTS_EXPLORE_SAVED_METRIC_QUERY]
         )
         metric = saved_metric.metric
 
     metric_segments_div = MS.from_metric(metric, discovered_project)
     graph_container = create_graph_container(metric, discovered_project.project)
     save_metric_dialog = create_saved_metric_dialog(saved_metric)
+    path = P.create_path(
+        P.PROJECTS_EXPLORE_PATH, project_id=discovered_project.project.id
+    )
+    if metric is not None:
+        url_params = "m=" + quote(SE.to_compressed_string(metric))
+        path = f"{path}?{url_params}"
+
     navbar = NB.create_mitzu_navbar(
         id=NAVBAR_ID,
         show_metric_type=True,
         show_metric_name=True,
         metric=metric,
         saved_metric=saved_metric,
-        notebook_mode=notebook_mode,
+        show_share_button=True,
+        path=path,
     )
 
     metric_id = H.create_unique_id() if saved_metric is None else saved_metric.id
     res = html.Div(
         children=[
             navbar,
             html.Div(children=metric_id, id=METRIC_ID_VALUE, className="d-none"),
@@ -261,15 +271,15 @@
     ret_or_conv_window = M.DEF_CONV_WINDOW
     if metric is not None:
         if isinstance(metric, M.ConversionMetric):
             ret_or_conv_window = metric._conv_window
         elif isinstance(metric, M.RetentionMetric):
             ret_or_conv_window = metric._retention_window
     else:
-        if metric_type == MTH.MetricType.CONVERSION:
+        if metric_type == MTH.MetricType.FUNNEL:
             ret_or_conv_window = M.DEF_CONV_WINDOW
         elif metric_type == MTH.MetricType.RETENTION:
             ret_or_conv_window = M.DEF_CONV_WINDOW
 
     metrics_config_card = MC.from_metric(metric_config, metric_type, ret_or_conv_window)
     graph_handler = GH.create_graph_container()
     toolbar_handler = TH.from_metric(metric, project)
@@ -316,15 +326,15 @@
     segments = MS.from_all_inputs(discovered_project, all_inputs)
     metric_type = MTH.MetricType.parse(all_inputs[MTH.METRIC_TYPE_DROPDOWN])
 
     metric_config, time_window = MC.from_all_inputs(
         discovered_project, all_inputs, metric_type
     )
     metric: Optional[M.Metric] = None
-    if metric_type == MTH.MetricType.CONVERSION:
+    if metric_type == MTH.MetricType.FUNNEL:
         if len(segments) >= 1:
             metric = M.Conversion(segments)
     elif metric_type == MTH.MetricType.SEGMENTATION:
         if len(segments) == 1:
             metric = segments[0]
     elif metric_type == MTH.MetricType.RETENTION:
         if len(segments) == 2:
@@ -343,15 +353,14 @@
     discovered_project: M.DiscoveredProject,
 ) -> Dict[str, Any]:
     metric, metric_config, time_window = create_metric_from_all_inputs(
         all_inputs, discovered_project
     )
     parse_result = urlparse(all_inputs[MITZU_LOCATION])
     if metric is not None:
-
         url_params = "m=" + quote(SE.to_compressed_string(metric))
         parse_result = parse_result._replace(query=url_params)
     url = parse_result.geturl()
 
     metric_segments = MS.from_metric(
         discovered_project=discovered_project,
         metric=metric,
@@ -455,14 +464,15 @@
             project_id = P.get_path_value(
                 P.PROJECTS_EXPLORE_PATH, url.path, P.PROJECT_ID_PATH_PART
             )
             depenedencies = DEPS.Dependencies.get()
             project = depenedencies.storage.get_project(project_id)
             if project is None:
                 return no_update_response
+
             all_inputs = get_final_all_inputs(all_inputs, ctx.inputs_list)
             all_inputs[METRIC_NAME_INPUT] = metric_name
             all_inputs[METRIC_ID_VALUE] = metric_id
             all_inputs[MITZU_LOCATION] = href
             discovered_project = project._discovered_project.get_value()
             if discovered_project is None:
                 return no_update_response
```

### Comparing `mitzu-0.6.3/mitzu/webapp/pages/explore/graph_handler.py` & `mitzu-0.6.4/mitzu/webapp/pages/explore/graph_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/webapp/pages/explore/metric_config_handler.py` & `mitzu-0.6.4/mitzu/webapp/pages/explore/metric_config_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
             return "Max Time To Convert"
         return f"P{p_val} Time To Convert"
     raise ValueError(f"Unsupported aggregation type {agg_type}")
 
 
 def get_time_window_options(metric_type: MTH.MetricType) -> List[Dict[str, int]]:
     res: List[Dict[str, Any]] = []
-    if metric_type == MTH.MetricType.CONVERSION:
+    if metric_type == MTH.MetricType.FUNNEL:
         for tg in M.TimeGroup:
             if tg in (M.TimeGroup.TOTAL, M.TimeGroup.QUARTER):
                 continue
             res.append({"label": tg.name.lower().title(), "value": tg.value})
     elif metric_type == MTH.MetricType.RETENTION:
         for tg in [
             M.TimeGroup.DAY,
@@ -71,15 +71,15 @@
                 continue
             res.append({"label": tg.name.lower().title(), "value": tg.value})
 
     return res
 
 
 def get_agg_type_options(metric_type: MTH.MetricType) -> List[Dict[str, str]]:
-    if metric_type == MTH.MetricType.CONVERSION:
+    if metric_type == MTH.MetricType.FUNNEL:
         res: List[Dict[str, Any]] = [
             {
                 "label": agg_type_to_str(M.AggType.CONVERSION),
                 "value": M.AggType.CONVERSION.to_agg_str(),
             },
             {
                 "label": agg_type_to_str(M.AggType.AVERAGE_TIME_TO_CONV),
@@ -126,15 +126,15 @@
     if metric_type == MTH.MetricType.SEGMENTATION:
         tw_value = 1
         tw_g_value = M.TimeGroup.DAY
         agg_type = metric_config.agg_type
         agg_param = metric_config.agg_param
         if agg_type not in (M.AggType.COUNT_UNIQUE_USERS, M.AggType.COUNT_EVENTS):
             agg_type = M.AggType.COUNT_UNIQUE_USERS
-    elif metric_type == MTH.MetricType.CONVERSION:
+    elif metric_type == MTH.MetricType.FUNNEL:
         tw_value = time_window.value
         tw_g_value = time_window.period
         agg_type = metric_config.agg_type
         agg_param = metric_config.agg_param
         if agg_type not in (
             M.AggType.PERCENTILE_TIME_TO_CONV,
             M.AggType.AVERAGE_TIME_TO_CONV,
@@ -197,15 +197,15 @@
                 size="xs",
                 data=get_time_window_options(metric_type),
                 style={"width": "100px", "display": "inline-block"},
             ),
         ],
         style={
             "visibility": "visible"
-            if metric_type in [MTH.MetricType.RETENTION, MTH.MetricType.CONVERSION]
+            if metric_type in [MTH.MetricType.RETENTION, MTH.MetricType.FUNNEL]
             else "hidden"
         },
     )
 
     resolution_ig = dmc.Select(
         id=RESOLUTION_DD,
         className="rounded-right",
@@ -214,15 +214,15 @@
         size="xs",
         label="Resolution",
         data=[{"label": value_to_label(v.name), "value": v.name} for v in M.Resolution],
         style={
             "width": "204px",
             "visibility": (
                 "visible"
-                if metric_type in [MTH.MetricType.RETENTION, MTH.MetricType.CONVERSION]
+                if metric_type in [MTH.MetricType.RETENTION, MTH.MetricType.FUNNEL]
                 else "hidden"
             ),
         },
     )
 
     return html.Div(children=[aggregation_comp, time_window, resolution_ig])
 
@@ -272,15 +272,15 @@
         start_dt = None
         end_dt = None
         if metric_type == MTH.MetricType.RETENTION:
             time_group = M.TimeGroup.WEEK
             resolution = M.Resolution.ONE_USER_EVENT_PER_MINUTE
             lookback_days = M.TimeWindow(2, M.TimeGroup.MONTH)
             time_window = M.TimeWindow(1, M.TimeGroup.WEEK)
-        elif metric_type == MTH.MetricType.CONVERSION:
+        elif metric_type == MTH.MetricType.FUNNEL:
             time_group = M.TimeGroup.DAY
             resolution = M.Resolution.EVERY_EVENT
             lookback_days = M.TimeWindow(1, M.TimeGroup.MONTH)
             time_window = M.TimeWindow(1, M.TimeGroup.DAY)
         else:
             time_group = M.TimeGroup.DAY
             resolution = M.Resolution.EVERY_EVENT
```

### Comparing `mitzu-0.6.3/mitzu/webapp/pages/explore/metric_segments_handler.py` & `mitzu-0.6.4/mitzu/webapp/pages/explore/metric_segments_handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     if isinstance(metric, M.SegmentationMetric):
         limit = 1
         segments = [metric._segment]
         metric_type = MNB.MetricType.SEGMENTATION
     elif isinstance(metric, M.ConversionMetric):
         limit = 10
         segments = metric._conversion._segments
-        metric_type = MNB.MetricType.CONVERSION
+        metric_type = MNB.MetricType.FUNNEL
     elif isinstance(metric, M.RetentionMetric):
         limit = 2
         segments = [metric._initial_segment, metric._retaining_segment]
         metric_type = MNB.MetricType.RETENTION
     elif metric is None:
         limit = 1
         segments = []
@@ -66,12 +66,13 @@
     discovered_project: Optional[M.DiscoveredProject],
     all_inputs: Dict[str, Any],
 ) -> List[M.Segment]:
     res: List[M.Segment] = []
     if discovered_project is None:
         return res
     complex_segments = all_inputs.get(METRIC_SEGMENTS, {}).get(CHILDREN, {})
+
     for _, complex_segment in complex_segments.items():
-        csh = CS.from_all_inputs(discovered_project, complex_segment)
+        csh = CS.from_all_inputs(discovered_project, complex_segment, len(res))
         if csh is not None:
             res.append(csh)
     return res
```

### Comparing `mitzu-0.6.3/mitzu/webapp/pages/explore/metric_type_handler.py` & `mitzu-0.6.4/mitzu/webapp/pages/explore/metric_type_handler.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,26 +9,26 @@
 
 
 METRIC_TYPE_DROPDOWN = "metric-type-dropdown"
 
 
 class MetricType(Enum):
     SEGMENTATION = auto()
-    CONVERSION = auto()
+    FUNNEL = auto()
     RETENTION = auto()
     USER_JOURNEYS = auto()
     REVENUE = auto()
     AB_TEST_ANALYSIS = auto()
     COHORTS = auto()
     CHURN_ANALYSIS = auto()
 
     @classmethod
     def from_metric(cls, metric: Optional[M.Metric]) -> MetricType:
         if isinstance(metric, M.ConversionMetric):
-            return MetricType.CONVERSION
+            return MetricType.FUNNEL
         elif isinstance(metric, M.RetentionMetric):
             return MetricType.RETENTION
         else:
             return MetricType.SEGMENTATION
 
     @classmethod
     def parse(cls, val_str: str) -> MetricType:
@@ -41,15 +41,15 @@
             {
                 "label": m_type.name.upper().replace("_", " "),
                 "value": m_type.name.upper(),
                 "disabled": m_type
                 not in (
                     MetricType.SEGMENTATION,
                     MetricType.RETENTION,
-                    MetricType.CONVERSION,
+                    MetricType.FUNNEL,
                 ),
             }
             for m_type in MetricType
         ],
         id=METRIC_TYPE_DROPDOWN,
         clearable=False,
         value=metric_type.name.upper(),
```

### Comparing `mitzu-0.6.3/mitzu/webapp/pages/explore/simple_segment_handler.py` & `mitzu-0.6.4/mitzu/webapp/pages/explore/simple_segment_handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from __future__ import annotations
 
 from typing import Any, Dict, List, Optional, Tuple
 
 import dash.development.base_component as bc
 import mitzu.model as M
-from dash import Input, MATCH, Output, callback, dcc, html
+from dash import Input, MATCH, Output, callback, dcc, html, ctx
 from mitzu.webapp.helper import (
     find_event_field_def,
     get_enums,
     get_property_name_label,
     WITH_VALUE_CLS,
 )
+from dash._utils import AttributeDict
 import dash_mantine_components as dmc
 from mitzu.webapp.auth.decorator import restricted
 
 SIMPLE_SEGMENT = "simple_segment"
 SIMPLE_SEGMENT_WITH_VALUE = "simple_segment_with_value"
 PROPERTY_NAME_DROPDOWN = "property_name_dropdown"
 PROPERTY_OPERATOR_DROPDOWN = "property_operator_dropdown"
@@ -190,16 +191,18 @@
     else:
         return tuple([fix_custom_value(value, data_type)])
 
 
 def from_all_inputs(
     discovered_project: Optional[M.DiscoveredProject],
     simple_segment: Dict[str, Any],
+    complex_segment_index: int,
+    event_segment_index: int,
+    simple_segment_index: int,
 ) -> Optional[M.SimpleSegment]:
-
     if discovered_project is None:
         return None
 
     property_path = simple_segment.get(PROPERTY_NAME_DROPDOWN)
     if property_path is None:
         return None
 
@@ -209,14 +212,23 @@
         return M.SimpleSegment(event_field_def, M.Operator.ANY_OF, None)
 
     if property_operator == OPERATOR_MAPPING[M.Operator.IS_NULL]:
         return M.SimpleSegment(event_field_def, M.Operator.IS_NULL, None)
     elif property_operator == OPERATOR_MAPPING[M.Operator.IS_NOT_NULL]:
         return M.SimpleSegment(event_field_def, M.Operator.IS_NOT_NULL, None)
 
+    if (
+        type(ctx.triggered_id) == AttributeDict
+        and ctx.triggered_id["type"] == PROPERTY_NAME_DROPDOWN
+        and ctx.triggered_id["index"]
+        == f"{complex_segment_index}-{event_segment_index}-{simple_segment_index}"
+    ):
+        # Changing property name should reset the value
+        return M.SimpleSegment(event_field_def, M.Operator.ANY_OF, None)
+
     property_value = simple_segment.get(PROPERTY_VALUE_INPUT)
     data_type = event_field_def._field._type
 
     if property_operator == OPERATOR_MAPPING[M.Operator.ANY_OF]:
         return M.SimpleSegment(
             event_field_def,
             M.Operator.ANY_OF,
```

### Comparing `mitzu-0.6.3/mitzu/webapp/pages/explore/toolbar_handler.py` & `mitzu-0.6.4/mitzu/webapp/pages/explore/toolbar_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/webapp/pages/explore_project.py` & `mitzu-0.6.4/mitzu/webapp/pages/explore_project.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/webapp/pages/home.py` & `mitzu-0.6.4/mitzu/webapp/pages/home.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/webapp/pages/login.py` & `mitzu-0.6.4/mitzu/webapp/pages/login.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/webapp/pages/manage_connection.py` & `mitzu-0.6.4/mitzu/webapp/pages/manage_connection.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/webapp/pages/manage_dashboard.py` & `mitzu-0.6.4/mitzu/webapp/pages/manage_dashboard.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/webapp/pages/manage_event_defs.py` & `mitzu-0.6.4/mitzu/webapp/pages/manage_event_defs.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/webapp/pages/manage_project.py` & `mitzu-0.6.4/mitzu/webapp/pages/manage_project.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/webapp/pages/manage_saved_metrics.py` & `mitzu-0.6.4/mitzu/webapp/pages/manage_saved_metrics.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/webapp/pages/paths.py` & `mitzu-0.6.4/mitzu/webapp/pages/paths.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/webapp/pages/projects/event_tables_config.py` & `mitzu-0.6.4/mitzu/webapp/pages/projects/event_tables_config.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/webapp/pages/projects/helper.py` & `mitzu-0.6.4/mitzu/webapp/pages/projects/helper.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/webapp/pages/projects/manage_project_component.py` & `mitzu-0.6.4/mitzu/webapp/pages/projects/manage_project_component.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/webapp/pages/projects_page.py` & `mitzu-0.6.4/mitzu/webapp/pages/projects_page.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/webapp/pages/users.py` & `mitzu-0.6.4/mitzu/webapp/pages/users.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/webapp/service/events_service.py` & `mitzu-0.6.4/mitzu/webapp/service/events_service.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/webapp/service/navbar_service.py` & `mitzu-0.6.4/mitzu/webapp/service/navbar_service.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/webapp/service/notification_service.py` & `mitzu-0.6.4/mitzu/webapp/service/notification_service.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/webapp/service/secret_service.py` & `mitzu-0.6.4/mitzu/webapp/service/secret_service.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/webapp/service/tracking_service.py` & `mitzu-0.6.4/mitzu/webapp/service/tracking_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 
 def log_error_message(error, items):
     H.LOGGER.warn(f"Tracking error: {error}")
 
 
 def init_analytics():
+    H.LOGGER.debug(f"Tracking init: {C.TRACKING_HOST}")
     analytics.write_key = C.TRACKING_API_KEY
     analytics.host = C.TRACKING_HOST
     analytics.on_error = log_error_message
     analytics.sync_mode = True
 
 
 class TrackingService(ABC):
@@ -68,20 +69,21 @@
 
     def _get_current_user_id(self) -> Optional[str]:
         return self._authorizer.get_current_user_id()
 
     def _track_event(
         self, event_name: str, event_properties: Dict[str, Any], flush: bool = True
     ):
+
         if not C.ENABLE_USAGE_TRACKING or not C.TRACKING_HOST:
             return
         try:
             user_id = self._get_current_user_id()
             if user_id is None:
-                H.LOGGER.warn("Unauthenticated user, tracking disabled")
+                H.LOGGER.debug("Unauthenticated user, tracking disabled")
                 return
             event_properties["app_version"] = __version__
             event_properties["environment"] = C.ENVIRONMENT
 
             analytics.track(
                 user_id=user_id, event=event_name, properties=event_properties
             )
```

### Comparing `mitzu-0.6.3/mitzu/webapp/service/user_service.py` & `mitzu-0.6.4/mitzu/webapp/service/user_service.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/webapp/storage.py` & `mitzu-0.6.4/mitzu/webapp/storage.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/webapp/storage_model.py` & `mitzu-0.6.4/mitzu/webapp/storage_model.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/mitzu/webapp/webapp.py` & `mitzu-0.6.4/mitzu/webapp/webapp.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.3/pyproject.toml` & `mitzu-0.6.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mitzu"
-version = "0.6.3"
+version = "0.6.4"
 description = "Product analytics over your data warehouse"
 authors = ["Istvan Meszaros <istvan.meszaros.88@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://mitzu.io"
 repository = "https://github.com/mitzu-io/mitzu"
 documentation = "https://mitzu.io/documentation/"
```

### Comparing `mitzu-0.6.3/PKG-INFO` & `mitzu-0.6.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mitzu
-Version: 0.6.3
+Version: 0.6.4
 Summary: Product analytics over your data warehouse
 Home-page: https://mitzu.io
 License: MIT
 Author: Istvan Meszaros
 Author-email: istvan.meszaros.88@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
```

