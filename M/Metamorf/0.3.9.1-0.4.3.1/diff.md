# Comparing `tmp/Metamorf-0.3.9.1.tar.gz` & `tmp/Metamorf-0.4.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Metamorf-0.3.9.1.tar", last modified: Wed Mar  8 18:23:35 2023, max compression
+gzip compressed data, was "Metamorf-0.4.3.1.tar", last modified: Sat Jun  3 22:04:56 2023, max compression
```

## Comparing `Metamorf-0.3.9.1.tar` & `Metamorf-0.4.3.1.tar`

### file list

```diff
@@ -1,79 +1,107 @@
-drwxrwxrwx   0        0        0        0 2023-03-08 18:23:35.498098 Metamorf-0.3.9.1/
--rw-rw-rw-   0        0        0    11582 2023-03-07 20:45:53.000000 Metamorf-0.3.9.1/LICENSE.md
-drwxrwxrwx   0        0        0        0 2023-03-08 18:23:35.237100 Metamorf-0.3.9.1/Metamorf.egg-info/
--rw-rw-rw-   0        0        0     6904 2023-03-08 18:23:35.000000 Metamorf-0.3.9.1/Metamorf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2298 2023-03-08 18:23:35.000000 Metamorf-0.3.9.1/Metamorf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-08 18:23:35.000000 Metamorf-0.3.9.1/Metamorf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-03-08 18:23:35.000000 Metamorf-0.3.9.1/Metamorf.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       40 2023-03-08 18:23:35.000000 Metamorf-0.3.9.1/Metamorf.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-03-08 18:23:35.000000 Metamorf-0.3.9.1/Metamorf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     6904 2023-03-08 18:23:35.497099 Metamorf-0.3.9.1/PKG-INFO
--rw-rw-rw-   0        0        0     6328 2023-03-07 20:54:13.000000 Metamorf-0.3.9.1/README.md
-drwxrwxrwx   0        0        0        0 2023-03-08 18:23:35.257100 Metamorf-0.3.9.1/metamorf/
--rw-rw-rw-   0        0        0       77 2023-01-31 18:29:02.000000 Metamorf-0.3.9.1/metamorf/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-08 18:23:35.281101 Metamorf-0.3.9.1/metamorf/configuration/
--rw-rw-rw-   0        0        0      230 2023-02-27 14:52:38.000000 Metamorf-0.3.9.1/metamorf/configuration/configuration.yml
--rw-rw-rw-   0        0        0      231 2023-03-07 17:17:45.000000 Metamorf-0.3.9.1/metamorf/configuration/configuration_data_snowflake.yml
--rw-rw-rw-   0        0        0       68 2023-02-05 12:43:57.000000 Metamorf-0.3.9.1/metamorf/configuration/configuration_data_sqlite.yml
--rw-rw-rw-   0        0        0      239 2023-03-07 17:17:50.000000 Metamorf-0.3.9.1/metamorf/configuration/configuration_metadata_snowflake.yml
--rw-rw-rw-   0        0        0       76 2023-01-31 18:29:02.000000 Metamorf-0.3.9.1/metamorf/configuration/configuration_metadata_sqlite.yml
--rw-rw-rw-   0        0        0     4194 2023-03-07 17:17:56.000000 Metamorf-0.3.9.1/metamorf/configuration/properties.yml
--rw-rw-rw-   0        0        0    10946 2023-03-07 17:16:44.000000 Metamorf-0.3.9.1/metamorf/constants.py
-drwxrwxrwx   0        0        0        0 2023-03-08 18:23:35.363101 Metamorf-0.3.9.1/metamorf/engines/
--rw-rw-rw-   0        0        0        0 2023-01-31 18:29:02.000000 Metamorf-0.3.9.1/metamorf/engines/__init__.py
--rw-rw-rw-   0        0        0     6943 2023-02-27 14:52:04.000000 Metamorf-0.3.9.1/metamorf/engines/engine.py
--rw-rw-rw-   0        0        0     4947 2023-03-06 18:49:53.000000 Metamorf-0.3.9.1/metamorf/engines/engine_api.py
--rw-rw-rw-   0        0        0     7689 2023-03-06 18:49:57.000000 Metamorf-0.3.9.1/metamorf/engines/engine_backup.py
--rw-rw-rw-   0        0        0     8121 2023-03-06 18:50:02.000000 Metamorf-0.3.9.1/metamorf/engines/engine_commit.py
--rw-rw-rw-   0        0        0     3772 2023-03-06 18:50:05.000000 Metamorf-0.3.9.1/metamorf/engines/engine_delete.py
--rw-rw-rw-   0        0        0     2341 2023-03-06 18:50:08.000000 Metamorf-0.3.9.1/metamorf/engines/engine_deploy.py
--rw-rw-rw-   0        0        0     3040 2023-03-06 18:50:15.000000 Metamorf-0.3.9.1/metamorf/engines/engine_deploy_example.py
--rw-rw-rw-   0        0        0     8195 2023-03-06 18:50:19.000000 Metamorf-0.3.9.1/metamorf/engines/engine_download.py
--rw-rw-rw-   0        0        0     5074 2023-03-06 18:50:22.000000 Metamorf-0.3.9.1/metamorf/engines/engine_init.py
--rw-rw-rw-   0        0        0      939 2023-03-06 18:50:26.000000 Metamorf-0.3.9.1/metamorf/engines/engine_manifest.py
--rw-rw-rw-   0        0        0     7574 2023-03-06 18:50:30.000000 Metamorf-0.3.9.1/metamorf/engines/engine_output.py
--rw-rw-rw-   0        0        0    94073 2023-03-06 18:48:18.000000 Metamorf-0.3.9.1/metamorf/engines/engine_process.py
--rw-rw-rw-   0        0        0    11368 2023-03-06 18:50:36.000000 Metamorf-0.3.9.1/metamorf/engines/engine_recover.py
--rw-rw-rw-   0        0        0    14806 2023-03-06 18:50:39.000000 Metamorf-0.3.9.1/metamorf/engines/engine_restore.py
--rw-rw-rw-   0        0        0     4631 2023-03-06 18:50:43.000000 Metamorf-0.3.9.1/metamorf/engines/engine_run.py
--rw-rw-rw-   0        0        0    13286 2023-03-06 18:50:47.000000 Metamorf-0.3.9.1/metamorf/engines/engine_upload.py
--rw-rw-rw-   0        0        0     1431 2023-03-06 18:50:50.000000 Metamorf-0.3.9.1/metamorf/engines/engine_validate.py
-drwxrwxrwx   0        0        0        0 2023-03-08 18:23:35.391100 Metamorf-0.3.9.1/metamorf/entry/
--rw-rw-rw-   0        0        0       40 2023-02-05 17:27:09.000000 Metamorf-0.3.9.1/metamorf/entry/ENTRY_AGGREGATORS.csv
--rw-rw-rw-   0        0        0      152 2023-02-05 17:26:42.000000 Metamorf-0.3.9.1/metamorf/entry/ENTRY_DATASET_MAPPINGS.csv
--rw-rw-rw-   0        0        0       91 2023-01-31 18:29:02.000000 Metamorf-0.3.9.1/metamorf/entry/ENTRY_DATASET_RELATIONSHIPS.csv
--rw-rw-rw-   0        0        0       42 2023-01-31 18:29:02.000000 Metamorf-0.3.9.1/metamorf/entry/ENTRY_ENTITY.csv
--rw-rw-rw-   0        0        0       34 2023-01-31 18:29:02.000000 Metamorf-0.3.9.1/metamorf/entry/ENTRY_FILTERS.csv
--rw-rw-rw-   0        0        0       34 2023-01-31 18:29:02.000000 Metamorf-0.3.9.1/metamorf/entry/ENTRY_HAVING.csv
--rw-rw-rw-   0        0        0       51 2023-02-05 17:26:55.000000 Metamorf-0.3.9.1/metamorf/entry/ENTRY_ORDER.csv
--rw-rw-rw-   0        0        0       34 2023-01-31 18:29:02.000000 Metamorf-0.3.9.1/metamorf/entry/ENTRY_PATH.csv
--rw-rw-rw-   0        0        0     1107 2023-02-05 13:37:55.000000 Metamorf-0.3.9.1/metamorf/help.py
-drwxrwxrwx   0        0        0        0 2023-03-08 18:23:35.423100 Metamorf-0.3.9.1/metamorf/initialization/
--rw-rw-rw-   0        0        0     5777 2023-03-03 17:18:44.000000 Metamorf-0.3.9.1/metamorf/initialization/init_example_data_snowflake.sql
--rw-rw-rw-   0        0        0     5426 2023-02-26 12:45:18.000000 Metamorf-0.3.9.1/metamorf/initialization/init_example_data_sqlite.sql
--rw-rw-rw-   0        0        0     7514 2023-03-03 17:18:51.000000 Metamorf-0.3.9.1/metamorf/initialization/init_example_metadata_snowflake.sql
--rw-rw-rw-   0        0        0     7337 2023-02-27 14:55:07.000000 Metamorf-0.3.9.1/metamorf/initialization/init_example_metadata_sqlite.sql
--rw-rw-rw-   0        0        0    15759 2023-03-07 17:17:04.000000 Metamorf-0.3.9.1/metamorf/initialization/init_snowflake.sql
--rw-rw-rw-   0        0        0    21006 2023-03-07 17:16:57.000000 Metamorf-0.3.9.1/metamorf/initialization/init_sqlite.sql
--rw-rw-rw-   0        0        0      139 2023-02-18 17:45:07.000000 Metamorf-0.3.9.1/metamorf/initialization/pre_init_snowflake.sql
--rw-rw-rw-   0        0        0        0 2023-02-18 17:54:01.000000 Metamorf-0.3.9.1/metamorf/initialization/pre_init_sqlite.sql
--rw-rw-rw-   0        0        0     3766 2023-03-02 19:28:34.000000 Metamorf-0.3.9.1/metamorf/main.py
-drwxrwxrwx   0        0        0        0 2023-03-08 18:23:35.480101 Metamorf-0.3.9.1/metamorf/tools/
--rw-rw-rw-   0        0        0        0 2023-01-31 18:29:02.000000 Metamorf-0.3.9.1/metamorf/tools/__init__.py
--rw-rw-rw-   0        0        0     4252 2023-02-19 13:10:33.000000 Metamorf-0.3.9.1/metamorf/tools/argparser.py
--rw-rw-rw-   0        0        0    13500 2023-02-26 16:07:46.000000 Metamorf-0.3.9.1/metamorf/tools/configvalidator.py
--rw-rw-rw-   0        0        0     8767 2023-03-06 17:56:23.000000 Metamorf-0.3.9.1/metamorf/tools/connection.py
--rw-rw-rw-   0        0        0    29174 2023-03-04 11:44:34.000000 Metamorf-0.3.9.1/metamorf/tools/database_objects.py
--rw-rw-rw-   0        0        0     6382 2023-02-27 14:09:12.000000 Metamorf-0.3.9.1/metamorf/tools/filecontroller.py
--rw-rw-rw-   0        0        0     2341 2023-03-02 10:57:38.000000 Metamorf-0.3.9.1/metamorf/tools/log.py
--rw-rw-rw-   0        0        0     4268 2023-03-03 17:48:59.000000 Metamorf-0.3.9.1/metamorf/tools/manifest.py
--rw-rw-rw-   0        0        0    33585 2023-03-06 18:34:23.000000 Metamorf-0.3.9.1/metamorf/tools/metadata.py
--rw-rw-rw-   0        0        0      831 2023-02-26 12:59:21.000000 Metamorf-0.3.9.1/metamorf/tools/node.py
--rw-rw-rw-   0        0        0    16778 2023-03-04 11:10:17.000000 Metamorf-0.3.9.1/metamorf/tools/query.py
--rw-rw-rw-   0        0        0    32376 2023-03-06 18:34:54.000000 Metamorf-0.3.9.1/metamorf/tools/utils.py
--rw-rw-rw-   0        0        0     1182 2023-03-08 18:22:58.000000 Metamorf-0.3.9.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-08 18:23:35.498098 Metamorf-0.3.9.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-08 18:23:35.496100 Metamorf-0.3.9.1/tests/
--rw-rw-rw-   0        0        0     2754 2023-01-31 23:34:10.000000 Metamorf-0.3.9.1/tests/tests.py
--rw-rw-rw-   0        0        0     2316 2023-01-31 19:38:51.000000 Metamorf-0.3.9.1/tests/tests_query.py
--rw-rw-rw-   0        0        0      643 2023-01-31 18:29:02.000000 Metamorf-0.3.9.1/tests/tests_validator.py
+drwxrwxrwx   0        0        0        0 2023-06-03 22:04:56.874250 Metamorf-0.4.3.1/
+-rw-rw-rw-   0        0        0    11582 2023-03-07 20:45:53.000000 Metamorf-0.4.3.1/LICENSE.md
+-rw-rw-rw-   0        0        0      487 2023-06-03 12:11:30.000000 Metamorf-0.4.3.1/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-06-03 22:04:56.806251 Metamorf-0.4.3.1/Metamorf.egg-info/
+-rw-rw-rw-   0        0        0     6903 2023-06-03 22:04:56.000000 Metamorf-0.4.3.1/Metamorf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3388 2023-06-03 22:04:56.000000 Metamorf-0.4.3.1/Metamorf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 22:04:56.000000 Metamorf-0.4.3.1/Metamorf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-06-03 22:04:56.000000 Metamorf-0.4.3.1/Metamorf.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       76 2023-06-03 22:04:56.000000 Metamorf-0.4.3.1/Metamorf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-03 22:04:56.000000 Metamorf-0.4.3.1/Metamorf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     6903 2023-06-03 22:04:56.874250 Metamorf-0.4.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6328 2023-03-07 20:54:13.000000 Metamorf-0.4.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-03 22:04:56.809249 Metamorf-0.4.3.1/metamorf/
+-rw-rw-rw-   0        0        0       77 2023-01-31 18:29:02.000000 Metamorf-0.4.3.1/metamorf/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-03 22:04:56.811250 Metamorf-0.4.3.1/metamorf/configuration/
+-rw-rw-rw-   0        0        0      228 2023-03-11 17:01:20.000000 Metamorf-0.4.3.1/metamorf/configuration/configuration.yml
+drwxrwxrwx   0        0        0        0 2023-06-03 22:04:56.813251 Metamorf-0.4.3.1/metamorf/configuration/mysql/
+-rw-rw-rw-   0        0        0      134 2023-03-21 20:57:39.000000 Metamorf-0.4.3.1/metamorf/configuration/mysql/configuration_data_mysql.yml
+-rw-rw-rw-   0        0        0      125 2023-03-30 10:47:46.000000 Metamorf-0.4.3.1/metamorf/configuration/mysql/configuration_metadata_mysql.yml
+drwxrwxrwx   0        0        0        0 2023-06-03 22:04:56.815249 Metamorf-0.4.3.1/metamorf/configuration/postgresql/
+-rw-rw-rw-   0        0        0      182 2023-06-03 11:17:50.000000 Metamorf-0.4.3.1/metamorf/configuration/postgresql/configuration_data_postgresql.yml
+-rw-rw-rw-   0        0        0      173 2023-06-03 11:17:50.000000 Metamorf-0.4.3.1/metamorf/configuration/postgresql/configuration_metadata_postgresql.yml
+-rw-rw-rw-   0        0        0     4667 2023-06-03 22:04:29.000000 Metamorf-0.4.3.1/metamorf/configuration/properties.yml
+drwxrwxrwx   0        0        0        0 2023-06-03 22:04:56.816249 Metamorf-0.4.3.1/metamorf/configuration/snowflake/
+-rw-rw-rw-   0        0        0      231 2023-03-07 17:17:45.000000 Metamorf-0.4.3.1/metamorf/configuration/snowflake/configuration_data_snowflake.yml
+-rw-rw-rw-   0        0        0      239 2023-03-07 17:17:50.000000 Metamorf-0.4.3.1/metamorf/configuration/snowflake/configuration_metadata_snowflake.yml
+drwxrwxrwx   0        0        0        0 2023-06-03 22:04:56.818251 Metamorf-0.4.3.1/metamorf/configuration/sqlite/
+-rw-rw-rw-   0        0        0       68 2023-02-05 12:43:57.000000 Metamorf-0.4.3.1/metamorf/configuration/sqlite/configuration_data_sqlite.yml
+-rw-rw-rw-   0        0        0       76 2023-01-31 18:29:02.000000 Metamorf-0.4.3.1/metamorf/configuration/sqlite/configuration_metadata_sqlite.yml
+-rw-rw-rw-   0        0        0    13022 2023-06-03 22:04:23.000000 Metamorf-0.4.3.1/metamorf/constants.py
+drwxrwxrwx   0        0        0        0 2023-06-03 22:04:56.835250 Metamorf-0.4.3.1/metamorf/engines/
+-rw-rw-rw-   0        0        0        0 2023-01-31 18:29:02.000000 Metamorf-0.4.3.1/metamorf/engines/__init__.py
+-rw-rw-rw-   0        0        0     6950 2023-06-03 21:44:06.000000 Metamorf-0.4.3.1/metamorf/engines/engine.py
+-rw-rw-rw-   0        0        0     4947 2023-03-11 15:54:33.000000 Metamorf-0.4.3.1/metamorf/engines/engine_api.py
+-rw-rw-rw-   0        0        0     8322 2023-06-03 21:44:06.000000 Metamorf-0.4.3.1/metamorf/engines/engine_backup.py
+-rw-rw-rw-   0        0        0    11239 2023-06-03 10:14:29.000000 Metamorf-0.4.3.1/metamorf/engines/engine_commit.py
+-rw-rw-rw-   0        0        0     4932 2023-06-03 10:14:29.000000 Metamorf-0.4.3.1/metamorf/engines/engine_delete.py
+-rw-rw-rw-   0        0        0     2432 2023-06-03 22:00:52.000000 Metamorf-0.4.3.1/metamorf/engines/engine_deploy.py
+-rw-rw-rw-   0        0        0     3129 2023-06-03 22:01:08.000000 Metamorf-0.4.3.1/metamorf/engines/engine_deploy_example.py
+-rw-rw-rw-   0        0        0    14348 2023-06-03 21:44:06.000000 Metamorf-0.4.3.1/metamorf/engines/engine_download.py
+-rw-rw-rw-   0        0        0     4347 2023-06-03 21:44:06.000000 Metamorf-0.4.3.1/metamorf/engines/engine_files.py
+-rw-rw-rw-   0        0        0     5207 2023-06-03 21:44:06.000000 Metamorf-0.4.3.1/metamorf/engines/engine_init.py
+-rw-rw-rw-   0        0        0      939 2023-03-06 18:50:26.000000 Metamorf-0.4.3.1/metamorf/engines/engine_manifest.py
+-rw-rw-rw-   0        0        0     1676 2023-06-03 10:14:29.000000 Metamorf-0.4.3.1/metamorf/engines/engine_metadata.py
+-rw-rw-rw-   0        0        0     7841 2023-06-03 21:44:06.000000 Metamorf-0.4.3.1/metamorf/engines/engine_output.py
+-rw-rw-rw-   0        0        0   368223 2023-06-03 10:14:29.000000 Metamorf-0.4.3.1/metamorf/engines/engine_process.py
+-rw-rw-rw-   0        0        0    16024 2023-06-03 10:14:29.000000 Metamorf-0.4.3.1/metamorf/engines/engine_recover.py
+-rw-rw-rw-   0        0        0    15830 2023-06-03 21:44:06.000000 Metamorf-0.4.3.1/metamorf/engines/engine_restore.py
+-rw-rw-rw-   0        0        0     4778 2023-06-03 10:14:29.000000 Metamorf-0.4.3.1/metamorf/engines/engine_run.py
+-rw-rw-rw-   0        0        0    18884 2023-06-03 21:44:06.000000 Metamorf-0.4.3.1/metamorf/engines/engine_upload.py
+-rw-rw-rw-   0        0        0     1431 2023-03-06 18:50:50.000000 Metamorf-0.4.3.1/metamorf/engines/engine_validate.py
+drwxrwxrwx   0        0        0        0 2023-06-03 22:04:56.844249 Metamorf-0.4.3.1/metamorf/entry/
+-rw-rw-rw-   0        0        0       58 2023-06-03 22:00:36.000000 Metamorf-0.4.3.1/metamorf/entry/ENTRY_AGGREGATORS.csv
+-rw-rw-rw-   0        0        0      166 2023-06-03 22:00:36.000000 Metamorf-0.4.3.1/metamorf/entry/ENTRY_DATASET_MAPPINGS.csv
+-rw-rw-rw-   0        0        0       91 2023-06-03 22:00:36.000000 Metamorf-0.4.3.1/metamorf/entry/ENTRY_DATASET_RELATIONSHIPS.csv
+-rw-rw-rw-   0        0        0      184 2023-06-03 22:00:36.000000 Metamorf-0.4.3.1/metamorf/entry/ENTRY_DV_ENTITY.csv
+-rw-rw-rw-   0        0        0      175 2023-06-03 22:00:36.000000 Metamorf-0.4.3.1/metamorf/entry/ENTRY_DV_MAPPINGS.csv
+-rw-rw-rw-   0        0        0       35 2023-06-03 22:00:36.000000 Metamorf-0.4.3.1/metamorf/entry/ENTRY_DV_PROPERTIES.csv
+-rw-rw-rw-   0        0        0       51 2023-06-03 22:00:36.000000 Metamorf-0.4.3.1/metamorf/entry/ENTRY_ENTITY.csv
+-rw-rw-rw-   0        0        0       40 2023-06-03 22:00:36.000000 Metamorf-0.4.3.1/metamorf/entry/ENTRY_FILES.csv
+-rw-rw-rw-   0        0        0       34 2023-06-03 22:00:36.000000 Metamorf-0.4.3.1/metamorf/entry/ENTRY_FILTERS.csv
+-rw-rw-rw-   0        0        0       34 2023-06-03 22:00:36.000000 Metamorf-0.4.3.1/metamorf/entry/ENTRY_HAVING.csv
+-rw-rw-rw-   0        0        0       69 2023-06-03 22:00:36.000000 Metamorf-0.4.3.1/metamorf/entry/ENTRY_ORDER.csv
+-rw-rw-rw-   0        0        0       34 2023-06-03 22:00:36.000000 Metamorf-0.4.3.1/metamorf/entry/ENTRY_PATH.csv
+-rw-rw-rw-   0        0        0     1124 2023-06-03 21:44:06.000000 Metamorf-0.4.3.1/metamorf/help.py
+drwxrwxrwx   0        0        0        0 2023-06-03 22:04:56.784250 Metamorf-0.4.3.1/metamorf/initialization/
+drwxrwxrwx   0        0        0        0 2023-06-03 22:04:56.848250 Metamorf-0.4.3.1/metamorf/initialization/mysql/
+-rw-rw-rw-   0        0        0     6164 2023-04-01 15:51:46.000000 Metamorf-0.4.3.1/metamorf/initialization/mysql/init_example_data_mysql.sql
+-rw-rw-rw-   0        0        0    13888 2023-04-01 15:50:11.000000 Metamorf-0.4.3.1/metamorf/initialization/mysql/init_example_metadata_mysql.sql
+-rw-rw-rw-   0        0        0    20854 2023-06-03 10:14:29.000000 Metamorf-0.4.3.1/metamorf/initialization/mysql/init_mysql.sql
+-rw-rw-rw-   0        0        0       39 2023-03-21 19:01:38.000000 Metamorf-0.4.3.1/metamorf/initialization/mysql/pre_init_mysql.sql
+drwxrwxrwx   0        0        0        0 2023-06-03 22:04:56.852250 Metamorf-0.4.3.1/metamorf/initialization/postgresql/
+-rw-rw-rw-   0        0        0     5699 2023-04-01 15:51:44.000000 Metamorf-0.4.3.1/metamorf/initialization/postgresql/init_example_data_postgresql.sql
+-rw-rw-rw-   0        0        0    12868 2023-06-03 11:17:50.000000 Metamorf-0.4.3.1/metamorf/initialization/postgresql/init_example_metadata_postgresql.sql
+-rw-rw-rw-   0        0        0    19601 2023-06-03 11:17:50.000000 Metamorf-0.4.3.1/metamorf/initialization/postgresql/init_postgresql.sql
+-rw-rw-rw-   0        0        0        0 2023-03-30 11:30:16.000000 Metamorf-0.4.3.1/metamorf/initialization/postgresql/pre_init_postgresql.sql
+drwxrwxrwx   0        0        0        0 2023-06-03 22:04:56.855250 Metamorf-0.4.3.1/metamorf/initialization/snowflake/
+-rw-rw-rw-   0        0        0     6625 2023-04-01 15:51:44.000000 Metamorf-0.4.3.1/metamorf/initialization/snowflake/init_example_data_snowflake.sql
+-rw-rw-rw-   0        0        0    13679 2023-04-01 15:50:03.000000 Metamorf-0.4.3.1/metamorf/initialization/snowflake/init_example_metadata_snowflake.sql
+-rw-rw-rw-   0        0        0    18039 2023-06-03 10:14:29.000000 Metamorf-0.4.3.1/metamorf/initialization/snowflake/init_snowflake.sql
+-rw-rw-rw-   0        0        0      139 2023-02-18 17:45:07.000000 Metamorf-0.4.3.1/metamorf/initialization/snowflake/pre_init_snowflake.sql
+drwxrwxrwx   0        0        0        0 2023-06-03 22:04:56.858252 Metamorf-0.4.3.1/metamorf/initialization/sqlite/
+-rw-rw-rw-   0        0        0     6086 2023-04-01 15:51:18.000000 Metamorf-0.4.3.1/metamorf/initialization/sqlite/init_example_data_sqlite.sql
+-rw-rw-rw-   0        0        0    13577 2023-04-01 15:50:00.000000 Metamorf-0.4.3.1/metamorf/initialization/sqlite/init_example_metadata_sqlite.sql
+-rw-rw-rw-   0        0        0    24483 2023-06-03 10:14:29.000000 Metamorf-0.4.3.1/metamorf/initialization/sqlite/init_sqlite.sql
+-rw-rw-rw-   0        0        0        0 2023-03-21 19:01:29.000000 Metamorf-0.4.3.1/metamorf/initialization/sqlite/pre_init_sqlite.sql
+-rw-rw-rw-   0        0        0     4110 2023-06-03 10:14:29.000000 Metamorf-0.4.3.1/metamorf/main.py
+drwxrwxrwx   0        0        0        0 2023-06-03 22:04:56.870253 Metamorf-0.4.3.1/metamorf/tools/
+-rw-rw-rw-   0        0        0        0 2023-01-31 18:29:02.000000 Metamorf-0.4.3.1/metamorf/tools/__init__.py
+-rw-rw-rw-   0        0        0     4269 2023-06-03 21:44:06.000000 Metamorf-0.4.3.1/metamorf/tools/argparser.py
+-rw-rw-rw-   0        0        0    14845 2023-06-03 10:14:29.000000 Metamorf-0.4.3.1/metamorf/tools/configvalidator.py
+-rw-rw-rw-   0        0        0    17228 2023-06-03 12:39:24.000000 Metamorf-0.4.3.1/metamorf/tools/connection.py
+-rw-rw-rw-   0        0        0    32970 2023-06-03 10:14:29.000000 Metamorf-0.4.3.1/metamorf/tools/database_objects.py
+-rw-rw-rw-   0        0        0     6654 2023-06-03 22:00:42.000000 Metamorf-0.4.3.1/metamorf/tools/filecontroller.py
+-rw-rw-rw-   0        0        0     2347 2023-06-03 21:44:06.000000 Metamorf-0.4.3.1/metamorf/tools/log.py
+-rw-rw-rw-   0        0        0     4310 2023-04-03 14:54:59.000000 Metamorf-0.4.3.1/metamorf/tools/manifest.py
+-rw-rw-rw-   0        0        0    43207 2023-06-03 10:14:29.000000 Metamorf-0.4.3.1/metamorf/tools/metadata.py
+-rw-rw-rw-   0        0        0    10605 2023-06-03 10:14:29.000000 Metamorf-0.4.3.1/metamorf/tools/metadata_validator.py
+-rw-rw-rw-   0        0        0      831 2023-02-26 12:59:21.000000 Metamorf-0.4.3.1/metamorf/tools/node.py
+-rw-rw-rw-   0        0        0    19573 2023-06-03 10:14:29.000000 Metamorf-0.4.3.1/metamorf/tools/query.py
+-rw-rw-rw-   0        0        0    35424 2023-06-03 10:14:29.000000 Metamorf-0.4.3.1/metamorf/tools/utils.py
+-rw-rw-rw-   0        0        0     1000 2023-06-03 22:04:23.000000 Metamorf-0.4.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-03 22:04:56.874250 Metamorf-0.4.3.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-03 22:04:56.873249 Metamorf-0.4.3.1/tests/
+-rw-rw-rw-   0        0        0     2754 2023-01-31 23:34:10.000000 Metamorf-0.4.3.1/tests/tests.py
+-rw-rw-rw-   0        0        0     2316 2023-01-31 19:38:51.000000 Metamorf-0.4.3.1/tests/tests_query.py
+-rw-rw-rw-   0        0        0      643 2023-01-31 18:29:02.000000 Metamorf-0.4.3.1/tests/tests_validator.py
```

### Comparing `Metamorf-0.3.9.1/LICENSE.md` & `Metamorf-0.4.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Metamorf-0.3.9.1/Metamorf.egg-info/PKG-INFO` & `Metamorf-0.4.3.1/Metamorf.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: Metamorf
-Version: 0.3.9.1
-Summary: Metadata Suite to build and control your Datawarehouse
+Version: 0.4.3.1
+Summary: Metadata Suite to build and manage your Datawarehouse
 Author-email: Guillermo Aumatell <gaumatellsalom@gmail.com>
 Project-URL: Homepage, https://github.com/gasalom/metamorf
 Project-URL: Bug Tracker, https://github.com/gasalom/metamorf/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.10
```

### Comparing `Metamorf-0.3.9.1/PKG-INFO` & `Metamorf-0.4.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: Metamorf
-Version: 0.3.9.1
-Summary: Metadata Suite to build and control your Datawarehouse
+Version: 0.4.3.1
+Summary: Metadata Suite to build and manage your Datawarehouse
 Author-email: Guillermo Aumatell <gaumatellsalom@gmail.com>
 Project-URL: Homepage, https://github.com/gasalom/metamorf
 Project-URL: Bug Tracker, https://github.com/gasalom/metamorf/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.10
```

### Comparing `Metamorf-0.3.9.1/README.md` & `Metamorf-0.4.3.1/README.md`

 * *Files identical despite different names*

### Comparing `Metamorf-0.3.9.1/metamorf/configuration/properties.yml` & `Metamorf-0.4.3.1/metamorf/configuration/properties.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 name: "Metamorf"
-description: "Metadata Suite to control all your Datawarehouse metadata-driven"
-version: "0.3.9b"
+description: "Metadata Suite to build and manage your Datawarehouse metadata-driven"
+version: "0.4.3.1"
 author: "Guillermo Aumatell Salom"
 contact: "guillermoaumatell@gmail.com"
 
 commands:
   - name: 'help'
     description: 'Shows all the commands available.'
   - name: 'manifest'
@@ -14,18 +14,18 @@
   - name: 'validate'
     description: 'Validates the configuration file.'
   - name: 'init'
     description: 'Metamorf Initialization on the current directory.'
     args:
       - name: 'database'
         options: ['-d', '--database']
-        values: ['SQLite', 'Snowflake']
+        values: ['SQLite', 'Snowflake', 'MySQL', 'PostgreSQL']
       - name: 'metadata'
         options: ['-m', '--metadata']
-        values: ['SQLite', 'Snowflake']
+        values: ['SQLite', 'Snowflake', 'MySQL', 'PostgreSQL']
   - name: 'deploy'
     description: 'Deploys on the metadata database all the requirements.'
   - name: 'deploy-example'
     description: 'Deploys on the metadata database all the requirement with metadata information and example data on the data database an example.'
   - name: 'download'
     description: 'Downloads the Metadata Entry of the Owner selected on CSV files, on the directory [entry].'
     args:
@@ -68,19 +68,23 @@
         values: [ '*', 'all']
   - name: 'delete'
     description: 'Deletes all the metadata from the owner.'
   - name: 'backup'
     description: 'Downloads all the Metadata onto CSV Files to backup all the system'
   - name: 'restore'
     description: 'Restores all the metadata from a backup.'
+  - name: 'files'
+    description: 'Upload all the files that are indicated on the metadata.'
+  - name: 'metadata'
+    description: 'Validates Metadata Entry.'
 
 
 options:
   log_print: 'Y'
-  print_debug: 'Y'
+  print_debug: 'N'
   max_commit_batch: 100
 
 modules:
   - name: "elt"
     description: "Module to load all the temporary tables."
     version: 0.5.1
     functions:
@@ -89,23 +93,27 @@
   - name: "datavault"
     description: "Module to load all the DataVault entities: Hubs, Links, Sats, Pits, Bridges..."
     version: 0.0.0
     functions:
       - name: "status"
         values: ['ACTIVE','INACTIVE']
       - name: "char_separator_naming"
-        values: ['_', '__', '$', '&', '/']
+        values: ['_', '__', '$', '&', '/', '|','||']
 
 database:
   - name: 'SQLite'
     mandatory_fields: ['sqlite_path']
   - name: 'Snowflake'
     mandatory_fields: ['snowflake_user', 'snowflake_password', 'snowflake_schema', 'snowflake_warehouse', 'snowflake_account', 'snowflake_database', 'snowflake_role']
   - name: 'Firebird'
     mandatory_fields: ['firebird_host', 'firebird_database', 'firebird_user', 'firebird_password']
+  - name: 'MySQL'
+    mandatory_fields: ['mysql_user', 'mysql_password', 'mysql_host', 'mysql_database']
+  - name: 'PostgreSQL'
+    mandatory_fields: ['postgres_user','postgres_password','postgres_host','postgres_database', 'postgres_schema']
 
 output:
   type: ['dbt', 'sql']
 
 api:
   port: 5555
   host: localhost
```

### Comparing `Metamorf-0.3.9.1/metamorf/constants.py` & `Metamorf-0.4.3.1/metamorf/constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 
 # METAMORF PROPERTIES
-VERSION = "0.3.9b"
+VERSION = "0.4.3.1"
 
 # Constants for QUERY TYPES
 QUERY_TYPE_INSERT = 0
 QUERY_TYPE_UPDATE = 1
 QUERY_TYPE_VIEW = 2
 QUERY_TYPE_DELETE = 3
 QUERY_TYPE_SELECT = 4
@@ -27,18 +27,21 @@
 FILE_TYPE_LOG = "log"
 FILE_TYPE_TXT = "txt"
 FILE_TYPE_CSV = "csv"
 FILE_TYPE_JSON = "json"
 
 # Constants for CONNECTION TYPES
 CONNECTION_SQLITE = "SQLITE"
+CONNECTION_MYSQL = "MYSQL"
 CONNECTION_SNOWFLAKE = "SNOWFLAKE"
 CONNECTION_FIREBIRD = "FIREBIRD"
 CONNECTION_POSTGRESQL = "POSTGRESQL"
 
+CONNECTIONS_WITHOUT_OUTER_JOIN = [CONNECTION_SQLITE, CONNECTION_MYSQL]
+
 # Constants for ENGINES
 MODULE_ELT = "ELT"
 MODULE_DV = "DATAVAULT"
 
 # Constants for Configuration Location
 LOG_FILE_NAME = "metamorf"
 CONFIGURATION_FILE_PATH = "configuration"
@@ -92,14 +95,18 @@
 FILE_ENTRY_DATASET_MAPPINGS = 'ENTRY_DATASET_MAPPINGS'
 FILE_ENTRY_DATASET_RELATIONSHIPS = 'ENTRY_DATASET_RELATIONSHIPS'
 FILE_ENTRY_ENTITY = 'ENTRY_ENTITY'
 FILE_ENTRY_FILTERS = 'ENTRY_FILTERS'
 FILE_ENTRY_ORDER = 'ENTRY_ORDER'
 FILE_ENTRY_PATH = 'ENTRY_PATH'
 FILE_ENTRY_HAVING = 'ENTRY_HAVING'
+FILE_ENTRY_DV_ENTITY = 'ENTRY_DV_ENTITY'
+FILE_ENTRY_DV_MAPPINGS = 'ENTRY_DV_MAPPINGS'
+FILE_ENTRY_DV_PROPERTIES = 'ENTRY_DV_PROPERTIES'
+FILE_ENTRY_FILES = 'ENTRY_FILES'
 
 # MANIFEST FILE
 FILE_MANIFEST = 'manifest'
 
 # TABLES
 TABLE_ENTRY_AGGREGATORS = 'ENTRY_AGGREGATORS'
 TABLE_ENTRY_DATASET_MAPPINGS = 'ENTRY_DATASET_MAPPINGS'
@@ -107,27 +114,31 @@
 TABLE_ENTRY_ENTITY = 'ENTRY_ENTITY'
 TABLE_ENTRY_FILTERS = 'ENTRY_FILTERS'
 TABLE_ENTRY_HAVING = 'ENTRY_HAVING'
 TABLE_ENTRY_ORDER = 'ENTRY_ORDER'
 TABLE_ENTRY_PATH = 'ENTRY_PATH'
 TABLE_ENTRY_DV_MAPPINGS = 'ENTRY_DV_MAPPINGS'
 TABLE_ENTRY_DV_ENTITY = 'ENTRY_DV_ENTITY'
+TABLE_ENTRY_DV_PROPERTIES = 'ENTRY_DV_PROPERTIES'
+TABLE_ENTRY_FILES = 'ENTRY_FILES'
 TABLE_OM_DATASET = 'OM_DATASET'
 TABLE_OM_DATASET_EXECUTION = 'OM_DATASET_EXECUTION'
 TABLE_OM_DATASET_T_ORDER = 'OM_DATASET_T_ORDER'
 TABLE_OM_DATASET_T_AGG = 'OM_DATASET_T_AGG'
 TABLE_OM_DATASET_T_DISTINCT = 'OM_DATASET_T_DISTINCT'
 TABLE_OM_DATASET_SPECIFICATION = 'OM_DATASET_SPECIFICATION'
 TABLE_OM_DATASET_RELATIONSHIPS = 'OM_DATASET_RELATIONSHIPS'
 TABLE_OM_DATASET_T_MAPPING = 'OM_DATASET_T_MAPPING'
 TABLE_OM_DATASET_T_FILTER = 'OM_DATASET_T_FILTER'
 TABLE_OM_DATASET_T_HAVING = 'OM_DATASET_T_HAVING'
 TABLE_OM_DATASET_PATH = 'OM_DATASET_PATH'
 TABLE_OM_PROPERTIES = 'OM_PROPERTIES'
 TABLE_OM_DATASET_HARDCODED = 'OM_DATASET_HARDCODED'
+TABLE_OM_DATASET_DV = 'OM_DATASET_DV'
+TABLE_OM_DATASET_FILE = 'OM_DATASET_FILE'
 TABLE_OM_REF_QUERY_TYPE = 'OM_REF_QUERY_TYPE'
 TABLE_OM_REF_KEY_TYPE = 'OM_REF_KEY_TYPE'
 TABLE_OM_REF_ENTITY_TYPE = 'OM_REF_ENTITY_TYPE'
 TABLE_OM_REF_JOIN_TYPE = 'OM_REF_JOIN_TYPE'
 TABLE_OM_REF_MODULES = 'OM_REF_MODULES'
 TABLE_OM_REF_ORDER_TYPE = 'OM_REF_ORDER_TYPE'
 
@@ -136,14 +147,18 @@
 TABLE_GIT_ENTRY_DATASET_MAPPINGS = 'GIT_ENTRY_DATASET_MAPPINGS'
 TABLE_GIT_ENTRY_DATASET_RELATIONSHIPS = 'GIT_ENTRY_DATASET_RELATIONSHIPS'
 TABLE_GIT_ENTRY_ENTITY = 'GIT_ENTRY_ENTITY'
 TABLE_GIT_ENTRY_FILTERS = 'GIT_ENTRY_FILTERS'
 TABLE_GIT_ENTRY_HAVING = 'GIT_ENTRY_HAVING'
 TABLE_GIT_ENTRY_ORDER = 'GIT_ENTRY_ORDER'
 TABLE_GIT_ENTRY_PATH = 'GIT_ENTRY_PATH'
+TABLE_GIT_ENTRY_DV_ENTITY = 'GIT_ENTRY_DV_ENTITY'
+TABLE_GIT_ENTRY_DV_MAPPINGS = 'GIT_ENTRY_DV_MAPPINGS'
+TABLE_GIT_ENTRY_DV_PROPERTIES = 'GIT_ENTRY_DV_PROPERTIES'
+TABLE_GIT_ENTRY_FILES = 'GIT_ENTRY_FILES'
 
 # TABLES IM
 TABLE_IM_OM_DATASET_INFORMATION = "OM_DATASET_INFORMATION"
 TABLE_IM_OM_RELATIONSHIPS = "OM_RELATIONSHIPS"
 TABLE_IM_OM_DATASET_SPECIFICATION_INFORMATION = "OM_DATASET_SPECIFICATION_INFORMATION"
 
 # COLUMNS METADATA
@@ -151,75 +166,91 @@
 COLUMNS_ENTRY_AGGREGATORS = ['COD_ENTITY_TARGET','COD_ENTITY_SOURCE', 'COLUMN_NAME', 'NUM_BRANCH', 'OWNER']
 COLUMNS_ENTRY_ORDER = ['COD_ENTITY_TARGET','COD_ENTITY_SOURCE', 'COLUMN_NAME', 'NUM_BRANCH', 'ORDER_TYPE', 'OWNER']
 COLUMNS_ENTRY_FILTERS = ['COD_ENTITY_TARGET', 'VALUE', 'NUM_BRANCH', 'OWNER']
 COLUMNS_ENTRY_HAVING = ['COD_ENTITY_TARGET', 'VALUE', 'NUM_BRANCH', 'OWNER']
 COLUMNS_ENTRY_PATH = ['COD_PATH', 'DATABASE_NAME', 'SCHEMA_NAME', 'OWNER']
 COLUMNS_ENTRY_DATASET_RELATIONSHIPS = ['COD_ENTITY_MASTER', 'COLUMN_NAME_MASTER', 'COD_ENTITY_DETAIL', 'COLUMN_NAME_DETAIL', 'RELATIONSHIP_TYPE', 'OWNER']
 COLUMNS_ENTRY_ENTITY = ['COD_ENTITY', 'TABLE_NAME', 'ENTITY_TYPE', 'COD_PATH', 'STRATEGY', 'OWNER']
-COLUMNS_ENTRY_DATASET_MAPPINGS = ['COD_ENTITY_SOURCE', 'VALUE_SOURCE', 'COD_ENTITY_TARGET', 'COLUMN_NAME_TARGET', 'COLUMN_TYPE_TARGET','ORDINAL_POSITION','LENGTH','PRECISION', 'NUM_BRANCH', 'KEY_TYPE', 'SW_DISTINCT', 'OWNER']
+COLUMNS_ENTRY_DATASET_MAPPINGS = ['COD_ENTITY_SOURCE', 'VALUE_SOURCE', 'COD_ENTITY_TARGET', 'COLUMN_NAME_TARGET', 'COLUMN_TYPE_TARGET','ORDINAL_POSITION','COLUMN_LENGTH','COLUMN_PRECISION', 'NUM_BRANCH', 'KEY_TYPE', 'SW_DISTINCT', 'OWNER']
 COLUMN_ENTRY_OWNER = 'OWNER'
-COLUMNS_ENTRY_DV_MAPPINGS = ['COD_ENTITY', 'COLUMN_NAME_SOURCE', 'COLUMN_NAME_TARGET', 'COLUMN_TYPE_TARGET', 'ORDINAL_POSITION', 'LENGTH', 'PRECISION', 'NUM_BRANCH', 'KEY_TYPE', 'SATELLITE_NAME']
-COLUMNS_ENTRY_DV_ENTITY = ['COD_ENTITY', 'SW_STATUS_TRACKING_SATELLITE', 'NAME_STATUS_TRACKING_SATELLITE', 'SW_RECORD_TRACKING_SATELLITE', 'NAME_RECORD_TRACKING_SATELLITE', 'SW_EFFECTIVITY_SATELLITE', 'NAME_EFFECTIVITY_SATELLITE', 'RECORD_SOURCE', 'ORIGIN_IS_INCREMENTAL', 'ORIGIN_IS_TOTAL', 'ORIGIN_IS_CDC']
+COLUMNS_ENTRY_DV_MAPPINGS = ['COD_ENTITY_SOURCE', 'COLUMN_NAME_SOURCE','COD_ENTITY_TARGET', 'COLUMN_NAME_TARGET', 'COLUMN_TYPE_TARGET', 'ORDINAL_POSITION', 'COLUMN_LENGTH', 'COLUMN_PRECISION', 'NUM_BRANCH', 'NUM_CONNECTION', 'KEY_TYPE', 'SATELLITE_NAME', 'ORIGIN_IS_INCREMENTAL', 'ORIGIN_IS_TOTAL', 'ORIGIN_IS_CDC', 'OWNER']
+COLUMNS_ENTRY_DV_ENTITY = ['COD_ENTITY', 'ENTITY_NAME', 'ENTITY_TYPE','COD_PATH', 'NAME_STATUS_TRACKING_SATELLITE', 'NAME_RECORD_TRACKING_SATELLITE', 'NAME_EFFECTIVITY_SATELLITE', 'OWNER']
+COLUMNS_ENTRY_DV_PROPERTIES = ['COD_ENTITY', 'NUM_CONNECTION', 'HASH_NAME', 'OWNER']
+COLUMNS_ENTRY_FILES = ['COD_ENTITY', 'FILE_PATH', 'FILE_NAME', 'DELIMITER_CHARACTER', 'OWNER']
 ## Git tables
 COLUMNS_GIT_ENTRY_AGGREGATORS = ['COD_ENTITY_TARGET','COD_ENTITY_SOURCE', 'COLUMN_NAME', 'NUM_BRANCH', 'OWNER']
 COLUMNS_GIT_ENTRY_ORDER = ['COD_ENTITY_TARGET','COD_ENTITY_SOURCE', 'COLUMN_NAME', 'NUM_BRANCH', 'ORDER_TYPE', 'OWNER']
 COLUMNS_GIT_ENTRY_FILTERS = ['COD_ENTITY_TARGET', 'VALUE', 'NUM_BRANCH', 'OWNER']
 COLUMNS_GIT_ENTRY_HAVING = ['COD_ENTITY_TARGET', 'VALUE', 'NUM_BRANCH', 'OWNER']
 COLUMNS_GIT_ENTRY_PATH = ['COD_PATH', 'DATABASE_NAME', 'SCHEMA_NAME', 'OWNER']
 COLUMNS_GIT_ENTRY_DATASET_RELATIONSHIPS = ['COD_ENTITY_MASTER', 'COLUMN_NAME_MASTER', 'COD_ENTITY_DETAIL', 'COLUMN_NAME_DETAIL', 'RELATIONSHIP_TYPE', 'OWNER']
 COLUMNS_GIT_ENTRY_ENTITY = ['COD_ENTITY', 'TABLE_NAME', 'ENTITY_TYPE', 'COD_PATH', 'STRATEGY', 'OWNER']
-COLUMNS_GIT_ENTRY_DATASET_MAPPINGS = ['COD_ENTITY_SOURCE', 'VALUE_SOURCE', 'COD_ENTITY_TARGET', 'COLUMN_NAME_TARGET', 'COLUMN_TYPE_TARGET','ORDINAL_POSITION','LENGTH','PRECISION', 'NUM_BRANCH', 'KEY_TYPE', 'SW_DISTINCT', 'OWNER']
+COLUMNS_GIT_ENTRY_DATASET_MAPPINGS = ['COD_ENTITY_SOURCE', 'VALUE_SOURCE', 'COD_ENTITY_TARGET', 'COLUMN_NAME_TARGET', 'COLUMN_TYPE_TARGET','ORDINAL_POSITION','COLUMN_LENGTH','COLUMN_PRECISION', 'NUM_BRANCH', 'KEY_TYPE', 'SW_DISTINCT', 'OWNER']
+COLUMNS_GIT_ENTRY_DV_ENTITY = ['COD_ENTITY', 'ENTITY_NAME', 'ENTITY_TYPE', 'COD_PATH', 'NAME_STATUS_TRACKING_SATELLITE', 'NAME_RECORD_TRACKING_SATELLITE', 'NAME_EFFECTIVITY_SATELLITE', 'OWNER']
+COLUMNS_GIT_ENTRY_DV_PROPERTIES = ['COD_ENTITY', 'NUM_CONNECTION', 'HASH_NAME', 'OWNER']
+COLUMNS_GIT_ENTRY_DV_MAPPINGS = ['COD_ENTITY_SOURCE', 'COLUMN_NAME_SOURCE', 'COD_ENTITY_TARGET', 'COLUMN_NAME_TARGET', 'COLUMN_TYPE_TARGET', 'ORDINAL_POSITION', 'COLUMN_LENGTH', 'COLUMN_PRECISION', 'NUM_BRANCH', 'NUM_CONNECTION', 'KEY_TYPE', 'SATELLITE_NAME', 'ORIGIN_IS_INCREMENTAL', 'ORIGIN_IS_TOTAL', 'ORIGIN_IS_CDC', 'OWNER']
+COLUMNS_GIT_ENTRY_FILES = ['COD_ENTITY', 'FILE_PATH',  'FILE_NAME', 'DELIMITER_CHARACTER', 'OWNER']
 COLUMN_GIT_ENTRY_OWNER = 'OWNER'
 ## Reference Metadata
 COLUMNS_OM_REF_ORDER_TYPE = ['ID_ORDER_TYPE', 'ORDER_TYPE_NAME', 'ORDER_TYPE_VALUE', 'ORDER_TYPE_DESCRIPTION']
 COLUMNS_OM_REF_MODULES = ['ID_MODULE','MODULE_NAME','MODULE_FULL_NAME', 'MODULE_DESCRIPTION']
 COLUMNS_OM_REF_JOIN_TYPE = ['ID_JOIN_TYPE', 'JOIN_NAME', 'JOIN_VALUE', 'JOIN_DESCRIPTION']
 COLUMNS_OM_REF_ENTITY_TYPE = ['ID_ENTITY_TYPE', 'ENTITY_TYPE_NAME', 'ENTITY_TYPE_DESCRIPTION', 'ENTITY_TYPE_FULL_NAME', 'ID_MODULE']
 COLUMNS_OM_REF_KEY_TYPE = ['ID_KEY_TYPE', 'KEY_TYPE_NAME', 'KEY_TYPE_DESCRIPTION']
 COLUMNS_OM_REF_QUERY_TYPE = ['ID_QUERY_TYPE', 'QUERY_TYPE_NAME', 'QUERY_TYPE_DESCRIPTION']
 ## Metadata
 COLUMNS_OM_DATASET = ['ID_DATASET', 'DATASET_NAME', 'ID_ENTITY_TYPE', 'ID_PATH' , 'META_OWNER', 'START_DATE', 'END_DATE']
 COLUMNS_OM_DATASET_EXECUTION = ['ID_DATASET', 'ID_QUERY_TYPE','META_OWNER', 'START_DATE', 'END_DATE']
 COLUMNS_OM_DATASET_T_ORDER = ['ID_T_ORDER', 'ID_DATASET', 'ID_BRANCH', 'ID_DATASET_SPEC', 'ID_ORDER_TYPE','META_OWNER', 'START_DATE', 'END_DATE']
 COLUMNS_OM_DATASET_T_AGG = ['ID_T_AGG', 'ID_DATASET', 'ID_BRANCH', 'ID_DATASET_SPEC','META_OWNER', 'START_DATE', 'END_DATE']
 COLUMNS_OM_DATASET_T_DISTINCT = ['ID_T_DISTINCT', 'ID_DATASET', 'ID_BRANCH', 'SW_DISTINCT','META_OWNER', 'START_DATE', 'END_DATE']
-COLUMNS_OM_DATASET_SPECIFICATION = ['ID_DATASET_SPEC', 'ID_DATASET', 'ID_KEY_TYPE', 'COLUMN_NAME', 'COLUMN_TYPE', 'ORDINAL_POSITION', 'IS_NULLABLE', 'LENGTH', 'PRECISION', 'SCALE','META_OWNER', 'START_DATE', 'END_DATE']
+COLUMNS_OM_DATASET_SPECIFICATION = ['ID_DATASET_SPEC', 'ID_DATASET', 'ID_KEY_TYPE', 'COLUMN_NAME', 'COLUMN_TYPE', 'ORDINAL_POSITION', 'IS_NULLABLE', 'COLUMN_LENGTH', 'COLUMN_PRECISION', 'COLUMN_SCALE','META_OWNER', 'START_DATE', 'END_DATE']
 COLUMNS_OM_DATASET_RELATIONSHIPS = ['ID_RELATIONSHIP', 'ID_DATASET_SPEC_MASTER', 'ID_DATASET_SPEC_DETAIL', 'ID_JOIN_TYPE','META_OWNER', 'START_DATE', 'END_DATE']
 COLUMNS_OM_DATASET_T_MAPPING = ['ID_T_MAPPING', 'ID_BRANCH', 'ID_DATASET_SPEC', 'VALUE_MAPPING','META_OWNER', 'START_DATE', 'END_DATE']
 COLUMNS_OM_DATASET_PATH = ['ID_PATH', 'DATABASE_NAME', 'SCHEMA_NAME','META_OWNER', 'START_DATE', 'END_DATE']
 COLUMNS_OM_DATASET_T_FILTER = ['ID_T_FILTER', 'ID_DATASET', 'ID_BRANCH', 'VALUE_FILTER','META_OWNER', 'START_DATE', 'END_DATE']
 COLUMNS_OM_DATASET_T_HAVING = ['ID_T_HAVING', 'ID_DATASET', 'ID_BRANCH', 'VALUE_HAVING','META_OWNER', 'START_DATE', 'END_DATE']
 COLUMNS_OM_DATASET_HARDCODED = ['ID_DATASET_HARDCODED', 'ID_DATASET', 'ID_BRANCH', 'CONTENT','META_OWNER', 'START_DATE', 'END_DATE']
 COLUMNS_OM_PROPERTIES = ['PROPERTY', 'VALUE', 'START_DATE']
+COLUMNS_OM_DATASET_DV = ['ID_DATASET', 'ID_ENTITY_TYPE', 'META_OWNER', 'START_DATE', 'END_DATE']
+COLUMNS_OM_DATASET_FILE = ['ID_DATASET', 'FILE_PATH', 'FILE_NAME', 'DELIMITER_CHARACTER', 'META_OWNER', 'START_DATE', 'END_DATE']
 COLUMN_OM_OWNER = 'META_OWNER'
 ## Information Mart
 COLUMNS_OM_DATASET_INFORMATION = ['META_OWNER','ENTITY_TYPE_FULL_NAME', 'ENTITY_TYPE_DESCRIPTION', 'MODULE_NAME', 'MODULE_FULL_NAME', 'MODULE_DESCRIPTION', 'DATASET_NAME', 'DATABASE_NAME', 'SCHEMA_NAME', 'QUERY_TYPE_NAME', 'QUERY_TYPE_DESCRIPTION', 'START_DATE']
 COLUMNS_OM_RELATIONSHIPS = ['META_OWNER', 'MASTER_DATABASE_NAME', 'MASTER_SCHEMA_NAME', 'MASTER_DATASET_NAME', 'MASTER_COLUMN_NAME', 'DETAIL_DATABASE_NAME', 'DETAIL_SCHEMA_NAME', 'DETAIL_DATASET_NAME', 'DETAIL_COLUMN_NAME', 'START_DATE']
-COLUMNS_OM_DATASET_SPECIFICATION_INFORMATION = ['META_OWNER', 'DATASET_NAME', 'COLUMN_NAME', 'COLUMN_TYPE', 'ORDINAL_POSITION', 'IS_NULLABLE', 'LENGTH', "PRECISION", "SCALE"]
+COLUMNS_OM_DATASET_SPECIFICATION_INFORMATION = ['META_OWNER', 'DATASET_NAME', 'COLUMN_NAME', 'COLUMN_TYPE', 'ORDINAL_POSITION', 'IS_NULLABLE', 'COLUMN_LENGTH', "COLUMN_PRECISION", "COLUMN_SCALE"]
 
 # ENGINES
 ## Entities
 ENTITY_SRC = "SRC"
 ENTITY_TB = "TB"
 ENTITY_WITH = "WITH"
 ENTITY_VIEW = "VIEW"
 ENTITY_HUB = "HUB"
 ENTITY_LINK = "LINK"
 ENTITY_SAT = "SAT"
+ENTITY_STS = "STS"
+ENTITY_RTS = "RTS"
+ENTITY_SATE = "SATE"
 
 ## Key Types
 KEY_TYPE_PRIMARY_KEY = "PK"
 KEY_TYPE_NULL = "NULL"
 KEY_TYPE_BUSINESS_KEY = "BK"
 KEY_TYPE_SEQUENCE = "SEQ"
 KEY_TYPE_FOREIGN_KEY = "FK"
 KEY_TYPE_HASH_KEY = "HK"
 KEY_TYPE_ATTRIBUTE = "AT"
 KEY_TYPE_STATUS = "ST"
-KEY_TYPE_DK = "DK"
+KEY_TYPE_DRIVENKEY = "DK"
+KEY_TYPE_RECORD_SOURCE = "RS"
+KEY_TYPE_TENANT = "TN"
+KEY_TYPE_HASHDIFF = "HD"
+KEY_TYPE_DEPENDENT_CHILD_KEY = "DCK"
+KEY_TYPE_APPLIED_DATE = "AD"
 
 ## Status Nodes
 NODE_STATUS_WAITING = "WAITING"
 NODE_STATUS_RUNNING = "RUNNING"
 NODE_STATUS_FINISHED_OK = "OK"
 NODE_STATUS_FINISHED_NOK = "NOK"
 NODE_STATUS_SKIP = "SKIP"
```

### Comparing `Metamorf-0.3.9.1/metamorf/engines/engine.py` & `Metamorf-0.4.3.1/metamorf/engines/engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
         file_controller_configuration.set_file_location(ACTUAL_PATH, CONFIGURATION_FILE_NAME)
         self.configuration_file = file_controller_configuration.read_file()
         if self.configuration_file is not None:
             self.configuration_file_loaded = True
 
         # Properties File
         file_controller_properties = FileControllerFactory().get_file_reader(FILE_TYPE_YML)
-        file_controller_properties.set_file_location(PACKAGE_PATH + '\\' + PROPERTIES_FILE_PATH, PROPERTIES_FILE_NAME)
+        file_controller_properties.set_file_location(os.path.join(PACKAGE_PATH , PROPERTIES_FILE_PATH), PROPERTIES_FILE_NAME)
         self.properties_file = file_controller_properties.read_file()
 
         # Properties and Configuration File
         configuration_validator = ConfigValidator(self.properties_file,self.configuration_file, self.log)
         result_configuration = configuration_validator.validate()
         if result_configuration: self.log.log(self.engine_name, 'Finished configuration file validation - Ok', LOG_LEVEL_OK)
         if not result_configuration: self.log.log(self.engine_name, 'Finished configuration file validation - Not Ok', LOG_LEVEL_ERROR)
```

### Comparing `Metamorf-0.3.9.1/metamorf/engines/engine_api.py` & `Metamorf-0.4.3.1/metamorf/engines/engine_api.py`

 * *Files identical despite different names*

### Comparing `Metamorf-0.3.9.1/metamorf/engines/engine_backup.py` & `Metamorf-0.4.3.1/metamorf/engines/engine_backup.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,125 +17,135 @@
 
         self.log.log(self.engine_name, "Start to backup the system for the owner ["+self.owner + "]", LOG_LEVEL_INFO)
         # OM_DATASET
         content = []
         content.append(COLUMNS_OM_DATASET)
         for registry in self.metadata_actual.om_dataset: content.append(registry.get())
         file_controller_final = FileControllerFactory().get_file_reader(FILE_TYPE_CSV)
-        file_controller_final.set_file_location(ACTUAL_PATH + '\\' + BACKUP_FILES_PATH, TABLE_OM_DATASET)
+        file_controller_final.set_file_location(os.path.join(ACTUAL_PATH , BACKUP_FILES_PATH), TABLE_OM_DATASET)
+        file_controller_final.setup_writer(FILE_WRITER_NEW_FILE)
+        file_controller_final.write_file(content)
+        file_controller_final.close()
+
+        # OM_DATASET_DV
+        content = []
+        content.append(COLUMNS_OM_DATASET_DV)
+        for registry in self.metadata_actual.om_dataset_dv: content.append(registry.get())
+        file_controller_final = FileControllerFactory().get_file_reader(FILE_TYPE_CSV)
+        file_controller_final.set_file_location(os.path.join(ACTUAL_PATH , BACKUP_FILES_PATH), TABLE_OM_DATASET_DV)
         file_controller_final.setup_writer(FILE_WRITER_NEW_FILE)
         file_controller_final.write_file(content)
         file_controller_final.close()
 
         # OM_DATASET_T_ORDER
         content = []
         content.append(COLUMNS_OM_DATASET_T_ORDER)
         for registry in self.metadata_actual.om_dataset_t_order: content.append(registry.get())
         file_controller_final = FileControllerFactory().get_file_reader(FILE_TYPE_CSV)
-        file_controller_final.set_file_location(ACTUAL_PATH + '\\' + BACKUP_FILES_PATH, TABLE_OM_DATASET_T_ORDER)
+        file_controller_final.set_file_location(os.path.join(ACTUAL_PATH , BACKUP_FILES_PATH), TABLE_OM_DATASET_T_ORDER)
         file_controller_final.setup_writer(FILE_WRITER_NEW_FILE)
         file_controller_final.write_file(content)
         file_controller_final.close()
 
         # OM_DATASET_SPECIFICATION
         content = []
         content.append(COLUMNS_OM_DATASET_SPECIFICATION)
         for registry in self.metadata_actual.om_dataset_specification: content.append(registry.get())
         file_controller_final = FileControllerFactory().get_file_reader(FILE_TYPE_CSV)
-        file_controller_final.set_file_location(ACTUAL_PATH + '\\' + BACKUP_FILES_PATH, TABLE_OM_DATASET_SPECIFICATION)
+        file_controller_final.set_file_location(os.path.join(ACTUAL_PATH , BACKUP_FILES_PATH), TABLE_OM_DATASET_SPECIFICATION)
         file_controller_final.setup_writer(FILE_WRITER_NEW_FILE)
         file_controller_final.write_file(content)
         file_controller_final.close()
 
         # OM_DATASET_T_MAPPING
         content = []
         content.append(COLUMNS_OM_DATASET_T_MAPPING)
         for registry in self.metadata_actual.om_dataset_t_mapping: content.append(registry.get())
         file_controller_final = FileControllerFactory().get_file_reader(FILE_TYPE_CSV)
-        file_controller_final.set_file_location(ACTUAL_PATH + '\\' + BACKUP_FILES_PATH, TABLE_OM_DATASET_T_MAPPING)
+        file_controller_final.set_file_location(os.path.join(ACTUAL_PATH , BACKUP_FILES_PATH), TABLE_OM_DATASET_T_MAPPING)
         file_controller_final.setup_writer(FILE_WRITER_NEW_FILE)
         file_controller_final.write_file(content)
         file_controller_final.close()
 
         # OM_DATASET_T_HAVING
         content = []
         content.append(COLUMNS_OM_DATASET_T_HAVING)
         for registry in self.metadata_actual.om_dataset_t_having: content.append(registry.get())
         file_controller_final = FileControllerFactory().get_file_reader(FILE_TYPE_CSV)
-        file_controller_final.set_file_location(ACTUAL_PATH + '\\' + BACKUP_FILES_PATH, TABLE_OM_DATASET_T_HAVING)
+        file_controller_final.set_file_location(os.path.join(ACTUAL_PATH , BACKUP_FILES_PATH), TABLE_OM_DATASET_T_HAVING)
         file_controller_final.setup_writer(FILE_WRITER_NEW_FILE)
         file_controller_final.write_file(content)
         file_controller_final.close()
 
         # OM_DATASET_T_AGG
         content = []
         content.append(COLUMNS_OM_DATASET_T_AGG)
         for registry in self.metadata_actual.om_dataset_t_agg: content.append(registry.get())
         file_controller_final = FileControllerFactory().get_file_reader(FILE_TYPE_CSV)
-        file_controller_final.set_file_location(ACTUAL_PATH + '\\' + BACKUP_FILES_PATH, TABLE_OM_DATASET_T_AGG)
+        file_controller_final.set_file_location(os.path.join(ACTUAL_PATH , BACKUP_FILES_PATH), TABLE_OM_DATASET_T_AGG)
         file_controller_final.setup_writer(FILE_WRITER_NEW_FILE)
         file_controller_final.write_file(content)
         file_controller_final.close()
 
         # OM_DATASET_T_FILTER
         content = []
         content.append(COLUMNS_OM_DATASET_T_FILTER)
         for registry in self.metadata_actual.om_dataset_t_filter: content.append(registry.get())
         file_controller_final = FileControllerFactory().get_file_reader(FILE_TYPE_CSV)
-        file_controller_final.set_file_location(ACTUAL_PATH + '\\' + BACKUP_FILES_PATH, TABLE_OM_DATASET_T_FILTER)
+        file_controller_final.set_file_location(os.path.join(ACTUAL_PATH , BACKUP_FILES_PATH), TABLE_OM_DATASET_T_FILTER)
         file_controller_final.setup_writer(FILE_WRITER_NEW_FILE)
         file_controller_final.write_file(content)
         file_controller_final.close()
 
         # OM_DATASET_RELATIONSHIPS
         content = []
         content.append(COLUMNS_OM_DATASET_RELATIONSHIPS)
         for registry in self.metadata_actual.om_dataset_relationships: content.append(registry.get())
         file_controller_final = FileControllerFactory().get_file_reader(FILE_TYPE_CSV)
-        file_controller_final.set_file_location(ACTUAL_PATH + '\\' + BACKUP_FILES_PATH, TABLE_OM_DATASET_RELATIONSHIPS)
+        file_controller_final.set_file_location(os.path.join(ACTUAL_PATH , BACKUP_FILES_PATH), TABLE_OM_DATASET_RELATIONSHIPS)
         file_controller_final.setup_writer(FILE_WRITER_NEW_FILE)
         file_controller_final.write_file(content)
         file_controller_final.close()
 
         # OM_DATASET_EXECUTION
         content = []
         content.append(COLUMNS_OM_DATASET_EXECUTION)
         for registry in self.metadata_actual.om_dataset_execution: content.append(registry.get())
         file_controller_final = FileControllerFactory().get_file_reader(FILE_TYPE_CSV)
-        file_controller_final.set_file_location(ACTUAL_PATH + '\\' + BACKUP_FILES_PATH, TABLE_OM_DATASET_EXECUTION)
+        file_controller_final.set_file_location(os.path.join(ACTUAL_PATH , BACKUP_FILES_PATH), TABLE_OM_DATASET_EXECUTION)
         file_controller_final.setup_writer(FILE_WRITER_NEW_FILE)
         file_controller_final.write_file(content)
         file_controller_final.close()
 
         # OM_DATASET_PATH
         content = []
         content.append(COLUMNS_OM_DATASET_PATH)
         for registry in self.metadata_actual.om_dataset_path: content.append(registry.get())
         file_controller_final = FileControllerFactory().get_file_reader(FILE_TYPE_CSV)
-        file_controller_final.set_file_location(ACTUAL_PATH + '\\' + BACKUP_FILES_PATH, TABLE_OM_DATASET_PATH)
+        file_controller_final.set_file_location(os.path.join(ACTUAL_PATH , BACKUP_FILES_PATH), TABLE_OM_DATASET_PATH)
         file_controller_final.setup_writer(FILE_WRITER_NEW_FILE)
         file_controller_final.write_file(content)
         file_controller_final.close()
 
         # OM_DATASET_T_DISTINCT
         content = []
         content.append(COLUMNS_OM_DATASET_T_DISTINCT)
         for registry in self.metadata_actual.om_dataset_t_distinct: content.append(registry.get())
         file_controller_final = FileControllerFactory().get_file_reader(FILE_TYPE_CSV)
-        file_controller_final.set_file_location(ACTUAL_PATH + '\\' + BACKUP_FILES_PATH, TABLE_OM_DATASET_T_DISTINCT)
+        file_controller_final.set_file_location(os.path.join(ACTUAL_PATH , BACKUP_FILES_PATH), TABLE_OM_DATASET_T_DISTINCT)
         file_controller_final.setup_writer(FILE_WRITER_NEW_FILE)
         file_controller_final.write_file(content)
         file_controller_final.close()
 
         # OM_PROPERTIES
         content = []
         content.append(COLUMNS_OM_PROPERTIES)
         for registry in self.metadata_actual.om_properties: content.append(registry.get())
         file_controller_final = FileControllerFactory().get_file_reader(FILE_TYPE_CSV)
-        file_controller_final.set_file_location(ACTUAL_PATH + '\\' + BACKUP_FILES_PATH, TABLE_OM_PROPERTIES)
+        file_controller_final.set_file_location(os.path.join(ACTUAL_PATH , BACKUP_FILES_PATH), TABLE_OM_PROPERTIES)
         file_controller_final.setup_writer(FILE_WRITER_NEW_FILE)
         file_controller_final.write_file(content)
         file_controller_final.close()
 
         self.log.log(self.engine_name, "Finish to backup the system for the owner [" + self.owner + "]", LOG_LEVEL_INFO)
 
         super().finish_execution()
```

### Comparing `Metamorf-0.3.9.1/metamorf/engines/engine_commit.py` & `Metamorf-0.4.3.1/metamorf/engines/engine_commit.py`

 * *Files 16% similar despite different names*

```diff
@@ -94,14 +94,46 @@
         query = Query()
         query.set_database(connection_type)
         query.set_type(QUERY_TYPE_DELETE)
         query.set_target_table(TABLE_GIT_ENTRY_AGGREGATORS)
         query.set_where_filters(where_filter)
         self.connection.execute(str(query))
 
+        # GIT_ENTRY_DV_ENTITY
+        query = Query()
+        query.set_database(connection_type)
+        query.set_type(QUERY_TYPE_DELETE)
+        query.set_target_table(TABLE_GIT_ENTRY_DV_ENTITY)
+        query.set_where_filters(where_filter)
+        self.connection.execute(str(query))
+
+        # GIT_ENTRY_DV_MAPPINGS
+        query = Query()
+        query.set_database(connection_type)
+        query.set_type(QUERY_TYPE_DELETE)
+        query.set_target_table(TABLE_GIT_ENTRY_DV_MAPPINGS)
+        query.set_where_filters(where_filter)
+        self.connection.execute(str(query))
+
+        # GIT_ENTRY_DV_PROPERTIES
+        query = Query()
+        query.set_database(connection_type)
+        query.set_type(QUERY_TYPE_DELETE)
+        query.set_target_table(TABLE_GIT_ENTRY_DV_PROPERTIES)
+        query.set_where_filters(where_filter)
+        self.connection.execute(str(query))
+
+        # GIT_ENTRY_DV_PROPERTIES
+        query = Query()
+        query.set_database(connection_type)
+        query.set_type(QUERY_TYPE_DELETE)
+        query.set_target_table(TABLE_GIT_ENTRY_FILES)
+        query.set_where_filters(where_filter)
+        self.connection.execute(str(query))
+
         self.log.log(self.engine_name, "Finished to delete previous metadata version", LOG_LEVEL_INFO)
 
     def copy_metadata_git(self):
         self.log.log(self.engine_name, "Starting to load active metadata version", LOG_LEVEL_INFO)
         where_filter = COLUMN_ENTRY_OWNER + "='" + self.owner + "'"
         connection_type = (self.configuration_file['metadata']['connection_type']).upper()
 
@@ -189,9 +221,53 @@
         query.set_where_filters(where_filter)
         query.set_target_table(TABLE_GIT_ENTRY_AGGREGATORS)
         query.set_insert_columns(COLUMNS_GIT_ENTRY_AGGREGATORS)
         query.set_select_columns(COLUMNS_ENTRY_AGGREGATORS)
         query.set_from_tables([TABLE_ENTRY_AGGREGATORS])
         self.connection.execute(str(query))
 
+        # GIT_ENTRY_DV_ENTITY
+        query = Query()
+        query.set_type(QUERY_TYPE_INSERT)
+        query.set_database(connection_type)
+        query.set_where_filters(where_filter)
+        query.set_target_table(TABLE_GIT_ENTRY_DV_ENTITY)
+        query.set_insert_columns(COLUMNS_GIT_ENTRY_DV_ENTITY)
+        query.set_select_columns(COLUMNS_ENTRY_DV_ENTITY)
+        query.set_from_tables([TABLE_ENTRY_DV_ENTITY])
+        self.connection.execute(str(query))
+
+        # GIT_ENTRY_DV_MAPPINGS
+        query = Query()
+        query.set_type(QUERY_TYPE_INSERT)
+        query.set_database(connection_type)
+        query.set_where_filters(where_filter)
+        query.set_target_table(TABLE_GIT_ENTRY_DV_MAPPINGS)
+        query.set_insert_columns(COLUMNS_GIT_ENTRY_DV_MAPPINGS)
+        query.set_select_columns(COLUMNS_ENTRY_DV_MAPPINGS)
+        query.set_from_tables([TABLE_ENTRY_DV_MAPPINGS])
+        self.connection.execute(str(query))
+
+        # GIT_ENTRY_DV_PROPERTIES
+        query = Query()
+        query.set_type(QUERY_TYPE_INSERT)
+        query.set_database(connection_type)
+        query.set_where_filters(where_filter)
+        query.set_target_table(TABLE_GIT_ENTRY_DV_PROPERTIES)
+        query.set_insert_columns(COLUMNS_GIT_ENTRY_DV_PROPERTIES)
+        query.set_select_columns(COLUMNS_ENTRY_DV_PROPERTIES)
+        query.set_from_tables([TABLE_ENTRY_DV_PROPERTIES])
+        self.connection.execute(str(query))
+
+        # GIT_ENTRY_DV_PROPERTIES
+        query = Query()
+        query.set_type(QUERY_TYPE_INSERT)
+        query.set_database(connection_type)
+        query.set_where_filters(where_filter)
+        query.set_target_table(TABLE_GIT_ENTRY_FILES)
+        query.set_insert_columns(COLUMNS_GIT_ENTRY_FILES)
+        query.set_select_columns(COLUMNS_ENTRY_FILES)
+        query.set_from_tables([TABLE_ENTRY_FILES])
+        self.connection.execute(str(query))
+
 
         self.log.log(self.engine_name, "Finished to load active metadata version", LOG_LEVEL_INFO)
```

### Comparing `Metamorf-0.3.9.1/metamorf/engines/engine_delete.py` & `Metamorf-0.4.3.1/metamorf/engines/engine_delete.py`

 * *Files 19% similar despite different names*

```diff
@@ -92,8 +92,40 @@
         query = Query()
         query.set_database(connection_type)
         query.set_type(QUERY_TYPE_DELETE)
         query.set_target_table(TABLE_ENTRY_AGGREGATORS)
         query.set_where_filters(where_filter)
         self.connection.execute(str(query))
 
+        # ENTRY_FILES
+        query = Query()
+        query.set_database(connection_type)
+        query.set_type(QUERY_TYPE_DELETE)
+        query.set_target_table(TABLE_ENTRY_FILES)
+        query.set_where_filters(where_filter)
+        self.connection.execute(str(query))
+
+        # ENTRY_DV_MAPPINGS
+        query = Query()
+        query.set_database(connection_type)
+        query.set_type(QUERY_TYPE_DELETE)
+        query.set_target_table(TABLE_ENTRY_DV_MAPPINGS)
+        query.set_where_filters(where_filter)
+        self.connection.execute(str(query))
+
+        # ENTRY_DV_ENTITY
+        query = Query()
+        query.set_database(connection_type)
+        query.set_type(QUERY_TYPE_DELETE)
+        query.set_target_table(TABLE_ENTRY_DV_ENTITY)
+        query.set_where_filters(where_filter)
+        self.connection.execute(str(query))
+
+        # ENTRY_DV_PROPERTIES
+        query = Query()
+        query.set_database(connection_type)
+        query.set_type(QUERY_TYPE_DELETE)
+        query.set_target_table(TABLE_ENTRY_DV_PROPERTIES)
+        query.set_where_filters(where_filter)
+        self.connection.execute(str(query))
+
         self.log.log(self.engine_name, "Finished to delete actual metadata", LOG_LEVEL_INFO)
```

### Comparing `Metamorf-0.3.9.1/metamorf/engines/engine_deploy.py` & `Metamorf-0.4.3.1/metamorf/engines/engine_deploy.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from metamorf.engines.engine import Engine
 from metamorf.tools.filecontroller import FileControllerFactory
 from metamorf.tools.connection import ConnectionFactory
 from metamorf.constants import *
+import os
 
 class EngineDeploy(Engine):
 
     def _initialize_engine(self):
         self.engine_name = "Engine Deploy"
         self.engine_command = "deploy"
 
@@ -14,30 +15,30 @@
         # Starts the execution loading the Configuration File. If there is an error it finishes the execution.
         super().start_execution()
 
         # ARCHITECTURE INSTALATION
         connection_type = self.configuration_file['metadata']['connection_type']
         # Get File that will be executed
         file_controller_init_sql = FileControllerFactory().get_file_reader(FILE_TYPE_SQL)
-        file_controller_init_sql.set_file_location(PACKAGE_PATH + "\\" + INITIALIZATION_FILE_PATH, "pre_init_" + connection_type + ".sql")
+        file_controller_init_sql.set_file_location(os.path.join(PACKAGE_PATH , INITIALIZATION_FILE_PATH , connection_type.lower()), "pre_init_" + connection_type.lower() + ".sql")
         file_init_sql = file_controller_init_sql.read_file()
 
         # Get Connection and Execute the Initialization
         self.log.log(self.engine_name, "Deploying Metamorf Architecture on the Metadata Database", LOG_LEVEL_INFO)
         connection = ConnectionFactory().get_connection(connection_type)
         connection.setup_connection(self.configuration_file['metadata'], self.log)
         connection.execute(file_init_sql)
         connection.commit()
         connection.close()
 
         # METAMORF INSTALATION
         connection_type = self.configuration_file['metadata']['connection_type']
         # Get File that will be executed
         file_controller_init_sql = FileControllerFactory().get_file_reader(FILE_TYPE_SQL)
-        file_controller_init_sql.set_file_location(PACKAGE_PATH + "\\" + INITIALIZATION_FILE_PATH, "init_" + connection_type + ".sql")
+        file_controller_init_sql.set_file_location(os.path.join(PACKAGE_PATH, INITIALIZATION_FILE_PATH, connection_type.lower()), "init_" + connection_type.lower() + ".sql")
         file_init_sql = file_controller_init_sql.read_file()
 
         # Get Connection and Execute the Initialization
         self.log.log(self.engine_name, "Deploying Metamorf on the Database indicated on Configuration File", LOG_LEVEL_INFO)
         connection = ConnectionFactory().get_connection(connection_type)
         connection.setup_connection(self.configuration_file['metadata'], self.log)
         connection.execute(file_init_sql)
```

### Comparing `Metamorf-0.3.9.1/metamorf/engines/engine_deploy_example.py` & `Metamorf-0.4.3.1/metamorf/engines/engine_deploy_example.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from metamorf.engines.engine import Engine
 from metamorf.tools.filecontroller import FileControllerFactory
 from metamorf.tools.connection import ConnectionFactory
 from metamorf.constants import *
+import os
 
 class EngineDeployExample(Engine):
 
     def _initialize_engine(self):
         self.engine_name = "Engine Deploy Example"
         self.engine_command = "deploy-example"
 
@@ -15,15 +16,15 @@
         super().start_execution()
 
         # METADATA DEPLOYMENT EXAMPLE
         connection_type = self.configuration_file['metadata']['connection_type']
         connection_type_data = self.configuration_file['data']['connection_type']
         # Get File that will be executed
         file_controller_init_sql = FileControllerFactory().get_file_reader(FILE_TYPE_SQL)
-        file_controller_init_sql.set_file_location(PACKAGE_PATH + "\\" + INITIALIZATION_FILE_PATH, "init_example_metadata_" + connection_type_data + ".sql")
+        file_controller_init_sql.set_file_location(os.path.join(PACKAGE_PATH, INITIALIZATION_FILE_PATH, connection_type.lower()), "init_example_metadata_" + connection_type_data.lower() + ".sql")
         file_init_sql = file_controller_init_sql.read_file()
 
         # Get Connection and Execute the Deployment
         self.log.log(self.engine_name, "Deploying Metamorf Metadata Example on the Database indicated on Configuration File", LOG_LEVEL_INFO)
         connection = ConnectionFactory().get_connection(connection_type)
         connection.setup_connection(self.configuration_file['metadata'], self.log)
         result = connection.execute(file_init_sql)
@@ -34,15 +35,15 @@
         self.log.log(self.engine_name, "Deployment Metamorf Metadata Example Finished", LOG_LEVEL_INFO)
         connection.close()
 
         # DATA DEPLOYMENT EXAMPLE
         connection_type = self.configuration_file['data']['connection_type']
         # Get File that will be executed
         file_controller_init_sql = FileControllerFactory().get_file_reader(FILE_TYPE_SQL)
-        file_controller_init_sql.set_file_location(PACKAGE_PATH + "\\" + INITIALIZATION_FILE_PATH, "init_example_data_" + connection_type + ".sql")
+        file_controller_init_sql.set_file_location(os.path.join(PACKAGE_PATH, INITIALIZATION_FILE_PATH, connection_type.lower()), "init_example_data_" + connection_type.lower() + ".sql")
         file_init_sql = file_controller_init_sql.read_file()
 
         # Get Connection and Execute the Deployment
         self.log.log(self.engine_name, "Deploying Metamorf Data Example on the Database indicated on Configuration File", LOG_LEVEL_INFO)
         connection = ConnectionFactory().get_connection(connection_type)
         connection.setup_connection(self.configuration_file['data'], self.log)
         result = connection.execute(file_init_sql)
```

### Comparing `Metamorf-0.3.9.1/metamorf/engines/engine_init.py` & `Metamorf-0.4.3.1/metamorf/engines/engine_init.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 
 class EngineInit(Engine):
 
     def _initialize_engine(self):
         self.engine_name = "Engine Init"
         self.engine_command = "init"
-        self.database_default = "sqlite"
+        self.database_default = CONNECTION_SQLITE.lower()
 
         self.metadata_database = None
         self.data_database = None
         if 'metadata' in self.arguments:
             self.metadata_database = self.arguments['metadata']
         if 'database' in self.arguments:
             self.data_database = self.arguments['database']
@@ -42,44 +42,44 @@
         # Create Configuration File
         file_controller_configuration = FileControllerFactory().get_file_reader(FILE_TYPE_YML)
         file_controller_configuration.set_file_location(ACTUAL_PATH, CONFIGURATION_FILE_NAME)
         file_controller_configuration.setup_writer(FILE_WRITER_NEW_FILE)
 
         # Read Template OUTPUT & MODULES
         file_controller_configuration_template = FileControllerFactory().get_file_reader(FILE_TYPE_YML)
-        file_controller_configuration_template.set_file_location(PACKAGE_PATH + '\\' + CONFIGURATION_FILE_PATH, CONFIGURATION_FILE_NAME)
+        file_controller_configuration_template.set_file_location(os.path.join(PACKAGE_PATH, CONFIGURATION_FILE_PATH), CONFIGURATION_FILE_NAME)
         self.configuration_file = file_controller_configuration_template.read_file()
         file_controller_configuration.write_file(self.configuration_file)
 
         # Read Template DATA
         file_controller_configuration_template = FileControllerFactory().get_file_reader(FILE_TYPE_YML)
-        file_controller_configuration_template.set_file_location(PACKAGE_PATH + '\\' + CONFIGURATION_FILE_PATH, CONFIGURATION_FILE_DATA + self.data_database + "." + FILE_TYPE_YML)
+        file_controller_configuration_template.set_file_location(os.path.join(PACKAGE_PATH, CONFIGURATION_FILE_PATH, self.data_database.lower()), CONFIGURATION_FILE_DATA + self.data_database + "." + FILE_TYPE_YML)
         self.configuration_file = file_controller_configuration_template.read_file()
         file_controller_configuration.write_file(self.configuration_file)
 
         # Read Template METADATA
         file_controller_configuration_template = FileControllerFactory().get_file_reader(FILE_TYPE_YML)
-        file_controller_configuration_template.set_file_location(PACKAGE_PATH + '\\' + CONFIGURATION_FILE_PATH, CONFIGURATION_FILE_METADATA + self.metadata_database + "." + FILE_TYPE_YML)
+        file_controller_configuration_template.set_file_location(os.path.join(PACKAGE_PATH, CONFIGURATION_FILE_PATH, self.metadata_database.lower()), CONFIGURATION_FILE_METADATA + self.metadata_database + "." + FILE_TYPE_YML)
         self.configuration_file = file_controller_configuration_template.read_file()
         file_controller_configuration.write_file(self.configuration_file)
 
         # Create folder
-        if not os.path.exists(ACTUAL_PATH + '\\' + ENTRY_FILES_PATH):
-            os.mkdir(ACTUAL_PATH + '\\' + ENTRY_FILES_PATH)
-        if not os.path.exists(ACTUAL_PATH + '\\'+OUTPUT_FILES_PATH +'\\'):
-            os.mkdir(ACTUAL_PATH + '\\'+OUTPUT_FILES_PATH +'\\')
-        if not os.path.exists(ACTUAL_PATH + '\\'+BACKUP_FILES_PATH +'\\'):
-            os.mkdir(ACTUAL_PATH + '\\'+BACKUP_FILES_PATH +'\\')
+        if not os.path.exists(os.path.join(ACTUAL_PATH, ENTRY_FILES_PATH)):
+            os.mkdir(os.path.join(ACTUAL_PATH, ENTRY_FILES_PATH))
+        if not os.path.exists(os.path.join(ACTUAL_PATH, OUTPUT_FILES_PATH)):
+            os.mkdir(os.path.join(ACTUAL_PATH, OUTPUT_FILES_PATH))
+        if not os.path.exists(os.path.join(ACTUAL_PATH, BACKUP_FILES_PATH)):
+            os.mkdir(os.path.join(ACTUAL_PATH, BACKUP_FILES_PATH))
 
         # Create files - Metadata Entry
-        all_entry_files = os.listdir(PACKAGE_PATH + '\\' + ENTRY_FILES_PATH)
+        all_entry_files = os.listdir(os.path.join(PACKAGE_PATH, ENTRY_FILES_PATH))
         for file in all_entry_files:
             file_controller = FileControllerFactory().get_file_reader(FILE_TYPE_CSV)
-            file_controller.set_file_location(PACKAGE_PATH + '\\' + ENTRY_FILES_PATH, file)
+            file_controller.set_file_location(os.path.join(PACKAGE_PATH, ENTRY_FILES_PATH), file)
             file_to_write = file_controller.read_file()
 
             file_controller_final = FileControllerFactory().get_file_reader(FILE_TYPE_CSV)
-            file_controller_final.set_file_location(ACTUAL_PATH + '\\' + ENTRY_FILES_PATH, file)
+            file_controller_final.set_file_location(os.path.join(ACTUAL_PATH, ENTRY_FILES_PATH), file)
             file_controller_final.setup_writer(FILE_WRITER_NEW_FILE)
             file_controller_final.write_file(file_to_write)
 
         super().finish_execution()
```

### Comparing `Metamorf-0.3.9.1/metamorf/engines/engine_manifest.py` & `Metamorf-0.4.3.1/metamorf/engines/engine_manifest.py`

 * *Files identical despite different names*

### Comparing `Metamorf-0.3.9.1/metamorf/engines/engine_output.py` & `Metamorf-0.4.3.1/metamorf/engines/engine_output.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from metamorf.engines.engine import Engine
 from metamorf.tools.filecontroller import FileControllerFactory
 from metamorf.tools.connection import ConnectionFactory
 from metamorf.constants import *
 from metamorf.tools.utils import get_list_nodes_from_metadata, get_node_with_with_query_execution_settings
 import re
+import os
 
 class EngineOutput(Engine):
 
     def _initialize_engine(self):
         self.engine_name = "Engine Output"
         self.engine_command = "output"
 
@@ -35,30 +36,34 @@
             connection.setup_connection(configuration, self.log)
 
             # Select Strategy of Materialization
             if output_type.upper() == OUTPUT_TYPE_DBT.upper():
                 node.query.set_type(QUERY_TYPE_SELECT)
                 content = str(node.query)
                 content = self.dbt_create_config_for_models(node) + "\n\n" + content
-                for table in node.predecessors:
+                all_substitutions = node.predecessors
+                all_substitutions.append(node.name)
+                for table in all_substitutions:
                     dataset = self.metadata.get_dataset_from_dataset_name(table)
                     fqdn = self.metadata.get_dataset_fqdn_from_dataset_name(table)
                     if dataset.id_entity_type == self.metadata.get_entity_type_from_entity_type_name(ENTITY_SRC).id_entity_type:
                         path = self.metadata.get_path_from_id_path(dataset.id_path)
                         content = re.sub("\s+"+fqdn+"\s+|\r", " {{source('"+self.get_source_dbt_name_from_path(path)+"','"+table+"')}} ", content )
+                    elif table == node.name:
+                        content = re.sub("\s+" + fqdn + "\s+|\r", " {{this}} ", content)
                     else:
                         content = re.sub("\s+" + fqdn + "\s|\r+", " {{ref('" + table + "')}} ", content)
 
             else:
                 node = get_node_with_with_query_execution_settings(connection, self.metadata, node)
                 content = str(node.query)
 
 
             file_controller = FileControllerFactory().get_file_reader(FILE_TYPE_SQL)
-            file_controller.set_file_location(ACTUAL_PATH + '\\' + OUTPUT_FILES_PATH, node.name)
+            file_controller.set_file_location(os.path.join(ACTUAL_PATH, OUTPUT_FILES_PATH), node.name)
             file_controller.setup_writer(FILE_WRITER_NEW_FILE)
             file_controller.write_file(content)
 
 
         # Create source files for DBT
         if output_type.upper() == OUTPUT_TYPE_DBT.upper():
             self.dbt_create_source_yml()
@@ -121,15 +126,15 @@
                 yml_table = dict()
                 yml_table['name'] = src
                 yml_name['tables'].append(yml_table)
 
             yml_content['sources'].append(yml_name)
 
         file_controller = FileControllerFactory().get_file_reader(FILE_TYPE_YML)
-        file_controller.set_file_location(ACTUAL_PATH + '\\' + OUTPUT_FILES_PATH, "sources_metamorf")
+        file_controller.set_file_location(os.path.join(ACTUAL_PATH, OUTPUT_FILES_PATH), "sources_metamorf")
         file_controller.setup_writer(FILE_WRITER_NEW_FILE)
         file_controller.write_file(yml_content)
 
     def dbt_create_config_for_models(self, node):
         id_query_type = self.metadata.get_dataset_execution_from_id_dataset(self.metadata.get_dataset_from_dataset_name(node.name).id_dataset).id_query_type
         config = "{{ config(materialized='"
         #TODO: Add more options to config DBT
```

### Comparing `Metamorf-0.3.9.1/metamorf/engines/engine_recover.py` & `Metamorf-0.4.3.1/metamorf/engines/engine_recover.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,20 +8,24 @@
 
     def _initialize_engine(self):
         self.engine_name = "Engine Recover"
         self.engine_command = "recover"
 
         self.tables_to_load = [TABLE_ENTRY_AGGREGATORS, TABLE_ENTRY_DATASET_MAPPINGS,
                                TABLE_ENTRY_DATASET_RELATIONSHIPS, TABLE_ENTRY_ENTITY, TABLE_ENTRY_FILTERS,
-                               TABLE_ENTRY_ORDER, TABLE_ENTRY_PATH, TABLE_ENTRY_HAVING, TABLE_ENTRY_AGGREGATORS]
+                               TABLE_ENTRY_ORDER, TABLE_ENTRY_PATH, TABLE_ENTRY_HAVING,
+                               TABLE_ENTRY_DV_ENTITY, TABLE_ENTRY_DV_MAPPINGS, TABLE_ENTRY_DV_PROPERTIES,
+                               TABLE_ENTRY_FILES]
         if 'select' in self.arguments:
             if self.arguments['select'] == "all" or self.arguments['select'] == "*":
                 self.tables_to_load = [TABLE_ENTRY_AGGREGATORS, TABLE_ENTRY_DATASET_MAPPINGS,
                                        TABLE_ENTRY_DATASET_RELATIONSHIPS, TABLE_ENTRY_ENTITY, TABLE_ENTRY_FILTERS,
-                                       TABLE_ENTRY_ORDER, TABLE_ENTRY_PATH, TABLE_ENTRY_HAVING, TABLE_ENTRY_AGGREGATORS]
+                                       TABLE_ENTRY_ORDER, TABLE_ENTRY_PATH, TABLE_ENTRY_HAVING,
+                                       TABLE_ENTRY_DV_ENTITY, TABLE_ENTRY_DV_MAPPINGS, TABLE_ENTRY_DV_PROPERTIES,
+                                       TABLE_ENTRY_FILES]
             if self.arguments['select'].lower() == TABLE_ENTRY_DATASET_MAPPINGS.lower():
                 self.tables_to_load = [TABLE_ENTRY_DATASET_MAPPINGS]
             if self.arguments['select'].lower() == TABLE_ENTRY_DATASET_RELATIONSHIPS.lower():
                 self.tables_to_load = [TABLE_ENTRY_DATASET_RELATIONSHIPS]
             if self.arguments['select'].lower() == TABLE_ENTRY_ENTITY.lower():
                 self.tables_to_load = [TABLE_ENTRY_ENTITY]
             if self.arguments['select'].lower() == TABLE_ENTRY_FILTERS.lower():
@@ -30,14 +34,22 @@
                 self.tables_to_load = [TABLE_ENTRY_ORDER]
             if self.arguments['select'].lower() == TABLE_ENTRY_PATH.lower():
                 self.tables_to_load = [TABLE_ENTRY_PATH]
             if self.arguments['select'].lower() == TABLE_ENTRY_HAVING.lower():
                 self.tables_to_load = [TABLE_ENTRY_HAVING]
             if self.arguments['select'].lower() == TABLE_ENTRY_AGGREGATORS.lower():
                 self.tables_to_load = [TABLE_ENTRY_AGGREGATORS]
+            if self.arguments['select'].lower() == TABLE_ENTRY_DV_ENTITY.lower():
+                self.tables_to_load = [TABLE_ENTRY_DV_ENTITY]
+            if self.arguments['select'].lower() == TABLE_ENTRY_DV_MAPPINGS.lower():
+                self.tables_to_load = [TABLE_ENTRY_DV_MAPPINGS]
+            if self.arguments['select'].lower() == TABLE_ENTRY_DV_PROPERTIES.lower():
+                self.tables_to_load = [TABLE_ENTRY_DV_PROPERTIES]
+            if self.arguments['select'].lower() == TABLE_ENTRY_FILES.lower():
+                self.tables_to_load = [TABLE_ENTRY_FILES]
 
     def run(self):
         # Starts the execution loading the Configuration File. If there is an error it finishes the execution.
         super().start_execution()
 
         self.log.log(self.engine_name, "Starting to commit metadata from owner ["+self.owner+"]", LOG_LEVEL_INFO)
         connection_type = self.configuration_file['metadata']['connection_type']
@@ -127,14 +139,50 @@
             query = Query()
             query.set_database(connection_type)
             query.set_type(QUERY_TYPE_DELETE)
             query.set_target_table(TABLE_ENTRY_AGGREGATORS)
             query.set_where_filters(where_filter)
             self.connection.execute(str(query))
 
+        # ENTRY_DV_ENTITY
+        if TABLE_ENTRY_DV_ENTITY in self.tables_to_load:
+            query = Query()
+            query.set_database(connection_type)
+            query.set_type(QUERY_TYPE_DELETE)
+            query.set_target_table(TABLE_ENTRY_DV_ENTITY)
+            query.set_where_filters(where_filter)
+            self.connection.execute(str(query))
+
+        # ENTRY_DV_MAPPINGS
+        if TABLE_ENTRY_DV_MAPPINGS in self.tables_to_load:
+            query = Query()
+            query.set_database(connection_type)
+            query.set_type(QUERY_TYPE_DELETE)
+            query.set_target_table(TABLE_ENTRY_DV_MAPPINGS)
+            query.set_where_filters(where_filter)
+            self.connection.execute(str(query))
+
+        # ENTRY_DV_PROPERTIES
+        if TABLE_ENTRY_DV_PROPERTIES in self.tables_to_load:
+            query = Query()
+            query.set_database(connection_type)
+            query.set_type(QUERY_TYPE_DELETE)
+            query.set_target_table(TABLE_ENTRY_DV_PROPERTIES)
+            query.set_where_filters(where_filter)
+            self.connection.execute(str(query))
+
+        # ENTRY_FILES
+        if TABLE_ENTRY_FILES in self.tables_to_load:
+            query = Query()
+            query.set_database(connection_type)
+            query.set_type(QUERY_TYPE_DELETE)
+            query.set_target_table(TABLE_ENTRY_FILES)
+            query.set_where_filters(where_filter)
+            self.connection.execute(str(query))
+
         self.log.log(self.engine_name, "Finished to delete actual metadata", LOG_LEVEL_INFO)
 
     def copy_metadata_git(self):
         self.log.log(self.engine_name, "Starting to load backup metadata", LOG_LEVEL_INFO)
         where_filter = COLUMN_GIT_ENTRY_OWNER + "='" + self.owner + "'"
         connection_type = self.configuration_file['metadata']['connection_type']
 
@@ -230,8 +278,56 @@
             query.set_where_filters(where_filter)
             query.set_target_table(TABLE_ENTRY_AGGREGATORS)
             query.set_insert_columns(COLUMNS_ENTRY_AGGREGATORS)
             query.set_select_columns(COLUMNS_GIT_ENTRY_AGGREGATORS)
             query.set_from_tables([TABLE_GIT_ENTRY_AGGREGATORS])
             self.connection.execute(str(query))
 
+        # GIT_ENTRY_DV_ENTITY
+        if TABLE_ENTRY_DV_ENTITY in self.tables_to_load:
+            query = Query()
+            query.set_database(connection_type)
+            query.set_type(QUERY_TYPE_INSERT)
+            query.set_where_filters(where_filter)
+            query.set_target_table(TABLE_ENTRY_DV_ENTITY)
+            query.set_insert_columns(COLUMNS_ENTRY_DV_ENTITY)
+            query.set_select_columns(COLUMNS_GIT_ENTRY_DV_ENTITY)
+            query.set_from_tables([TABLE_GIT_ENTRY_DV_ENTITY])
+            self.connection.execute(str(query))
+
+        # GIT_ENTRY_DV_MAPPINGS
+        if TABLE_ENTRY_DV_MAPPINGS in self.tables_to_load:
+            query = Query()
+            query.set_database(connection_type)
+            query.set_type(QUERY_TYPE_INSERT)
+            query.set_where_filters(where_filter)
+            query.set_target_table(TABLE_ENTRY_DV_MAPPINGS)
+            query.set_insert_columns(COLUMNS_ENTRY_DV_MAPPINGS)
+            query.set_select_columns(COLUMNS_GIT_ENTRY_DV_MAPPINGS)
+            query.set_from_tables([TABLE_GIT_ENTRY_DV_MAPPINGS])
+            self.connection.execute(str(query))
+
+        # GIT_ENTRY_DV_PROPERTIES
+        if TABLE_ENTRY_DV_PROPERTIES in self.tables_to_load:
+            query = Query()
+            query.set_database(connection_type)
+            query.set_type(QUERY_TYPE_INSERT)
+            query.set_where_filters(where_filter)
+            query.set_target_table(TABLE_ENTRY_DV_PROPERTIES)
+            query.set_insert_columns(COLUMNS_ENTRY_DV_PROPERTIES)
+            query.set_select_columns(COLUMNS_GIT_ENTRY_DV_PROPERTIES)
+            query.set_from_tables([TABLE_GIT_ENTRY_DV_PROPERTIES])
+            self.connection.execute(str(query))
+
+        # GIT_ENTRY_DV_PROPERTIES
+        if TABLE_ENTRY_FILES in self.tables_to_load:
+            query = Query()
+            query.set_database(connection_type)
+            query.set_type(QUERY_TYPE_INSERT)
+            query.set_where_filters(where_filter)
+            query.set_target_table(TABLE_ENTRY_FILES)
+            query.set_insert_columns(COLUMNS_ENTRY_FILES)
+            query.set_select_columns(COLUMNS_GIT_ENTRY_FILES)
+            query.set_from_tables([TABLE_GIT_ENTRY_FILES])
+            self.connection.execute(str(query))
+
         self.log.log(self.engine_name, "Finished to load backup metadata", LOG_LEVEL_INFO)
```

### Comparing `Metamorf-0.3.9.1/metamorf/engines/engine_restore.py` & `Metamorf-0.4.3.1/metamorf/engines/engine_restore.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from metamorf.engines.engine import Engine
 from metamorf.tools.filecontroller import FileControllerFactory
 from metamorf.tools.connection import ConnectionFactory
 from metamorf.constants import *
 from metamorf.tools.metadata import Metadata
 from metamorf.tools.query import Query
+import os
 
 class EngineRestore(Engine):
 
     def _initialize_engine(self):
         self.engine_name = "Engine Restore"
         self.engine_command = "restore"
 
@@ -31,15 +32,15 @@
     def delete_all_entry_from_owner(self):
         result = True
         self.log.log(self.engine_name, "Starting deleting Metadata on database" , LOG_LEVEL_INFO)
         connection_type = self.configuration_file['metadata']['connection_type']
         metadata_tables = [TABLE_OM_DATASET, TABLE_OM_DATASET_EXECUTION, TABLE_OM_DATASET_T_ORDER,
                            TABLE_OM_DATASET_T_AGG, TABLE_OM_DATASET_T_DISTINCT, TABLE_OM_DATASET_SPECIFICATION,
                            TABLE_OM_DATASET_RELATIONSHIPS, TABLE_OM_DATASET_T_MAPPING, TABLE_OM_DATASET_T_FILTER,
-                           TABLE_OM_DATASET_T_HAVING, TABLE_OM_DATASET_PATH , TABLE_OM_PROPERTIES]
+                           TABLE_OM_DATASET_T_HAVING, TABLE_OM_DATASET_PATH , TABLE_OM_PROPERTIES, TABLE_OM_DATASET_DV]
         for file in metadata_tables:
             self.log.log(self.engine_name, "Deleting: " + file, LOG_LEVEL_INFO)
             query = Query()
             query.set_database(connection_type)
             query.set_target_table(file)
             query.set_is_truncate(True)
             res = self.connection.execute(str(query))
@@ -61,32 +62,49 @@
         self.log.log(self.engine_name, "Starting uploading Metadata Entry on database", LOG_LEVEL_INFO)
         result = True
         metadata = Metadata(self.log)
         connection_type = self.configuration_file['metadata']['connection_type']
 
         # TABLE_OM_DATASET
         file_reader = FileControllerFactory().get_file_reader(FILE_TYPE_CSV)
-        file_reader.set_file_location(ACTUAL_PATH + '\\' + BACKUP_FILES_PATH, TABLE_OM_DATASET + "." + FILE_TYPE_CSV)
+        file_reader.set_file_location(os.path.join(ACTUAL_PATH, BACKUP_FILES_PATH), TABLE_OM_DATASET + "." + FILE_TYPE_CSV)
         file = file_reader.read_file()
         res = metadata.add_om_dataset(self.refactor_file(file))
         result = result and res
         query_values = Query()
         query_values.set_database(connection_type)
         query_values.set_has_header(True)
         query_values.set_type(QUERY_TYPE_VALUES)
         query_values.set_target_table(TABLE_OM_DATASET)
         query_values.set_insert_columns(COLUMNS_OM_DATASET)
         query_values.set_values(metadata.om_dataset)
         self.log.log(self.engine_name, "Loading: " + TABLE_OM_DATASET, LOG_LEVEL_INFO)
         res = self.connection.execute(str(query_values))
         result = result and res
 
+        # TABLE_OM_DATASET_DV
+        file_reader = FileControllerFactory().get_file_reader(FILE_TYPE_CSV)
+        file_reader.set_file_location(os.path.join(ACTUAL_PATH, BACKUP_FILES_PATH), TABLE_OM_DATASET_DV + "." + FILE_TYPE_CSV)
+        file = file_reader.read_file()
+        res = metadata.add_om_dataset_dv(self.refactor_file(file))
+        result = result and res
+        query_values = Query()
+        query_values.set_database(connection_type)
+        query_values.set_has_header(True)
+        query_values.set_type(QUERY_TYPE_VALUES)
+        query_values.set_target_table(TABLE_OM_DATASET_DV)
+        query_values.set_insert_columns(COLUMNS_OM_DATASET_DV)
+        query_values.set_values(metadata.om_dataset_dv)
+        self.log.log(self.engine_name, "Loading: " + TABLE_OM_DATASET_DV, LOG_LEVEL_INFO)
+        res = self.connection.execute(str(query_values))
+        result = result and res
+
         # TABLE_OM_DATASET_EXECUTION
         file_reader = FileControllerFactory().get_file_reader(FILE_TYPE_CSV)
-        file_reader.set_file_location(ACTUAL_PATH + '\\' + BACKUP_FILES_PATH, TABLE_OM_DATASET_EXECUTION + "." + FILE_TYPE_CSV)
+        file_reader.set_file_location(os.path.join(ACTUAL_PATH, BACKUP_FILES_PATH), TABLE_OM_DATASET_EXECUTION + "." + FILE_TYPE_CSV)
         file = file_reader.read_file()
         res = metadata.add_om_dataset_execution(self.refactor_file(file))
         result = result and res
         query_values = Query()
         query_values.set_database(connection_type)
         query_values.set_has_header(True)
         query_values.set_type(QUERY_TYPE_VALUES)
@@ -95,15 +113,15 @@
         query_values.set_values(metadata.om_dataset_execution)
         self.log.log(self.engine_name, "Loading: " + TABLE_OM_DATASET_EXECUTION, LOG_LEVEL_INFO)
         res = self.connection.execute(str(query_values))
         result = result and res
 
         # TABLE_OM_DATASET_T_ORDER
         file_reader = FileControllerFactory().get_file_reader(FILE_TYPE_CSV)
-        file_reader.set_file_location(ACTUAL_PATH + '\\' + BACKUP_FILES_PATH, TABLE_OM_DATASET_T_ORDER + "." + FILE_TYPE_CSV)
+        file_reader.set_file_location(os.path.join(ACTUAL_PATH, BACKUP_FILES_PATH), TABLE_OM_DATASET_T_ORDER + "." + FILE_TYPE_CSV)
         file = file_reader.read_file()
         res = metadata.add_om_dataset_t_order(self.refactor_file(file))
         result = result and res
         query_values = Query()
         query_values.set_database(connection_type)
         query_values.set_has_header(True)
         query_values.set_type(QUERY_TYPE_VALUES)
@@ -112,15 +130,15 @@
         query_values.set_values(metadata.om_dataset_t_order)
         self.log.log(self.engine_name, "Loading: " + TABLE_OM_DATASET_T_ORDER, LOG_LEVEL_INFO)
         res = self.connection.execute(str(query_values))
         result = result and res
 
         # TABLE_OM_DATASET_T_AGG
         file_reader = FileControllerFactory().get_file_reader(FILE_TYPE_CSV)
-        file_reader.set_file_location(ACTUAL_PATH + '\\' + BACKUP_FILES_PATH, TABLE_OM_DATASET_T_AGG + "." + FILE_TYPE_CSV)
+        file_reader.set_file_location(os.path.join(ACTUAL_PATH, BACKUP_FILES_PATH), TABLE_OM_DATASET_T_AGG + "." + FILE_TYPE_CSV)
         file = file_reader.read_file()
         res = metadata.add_om_dataset_t_agg(self.refactor_file(file))
         result = result and res
         query_values = Query()
         query_values.set_database(connection_type)
         query_values.set_has_header(True)
         query_values.set_type(QUERY_TYPE_VALUES)
@@ -129,15 +147,15 @@
         query_values.set_values(metadata.om_dataset_t_agg)
         self.log.log(self.engine_name, "Loading: " + TABLE_OM_DATASET_T_AGG, LOG_LEVEL_INFO)
         res = self.connection.execute(str(query_values))
         result = result and res
 
         # TABLE_OM_DATASET_T_DISTINCT
         file_reader = FileControllerFactory().get_file_reader(FILE_TYPE_CSV)
-        file_reader.set_file_location(ACTUAL_PATH + '\\' + BACKUP_FILES_PATH,
+        file_reader.set_file_location(os.path.join(ACTUAL_PATH, BACKUP_FILES_PATH),
                                       TABLE_OM_DATASET_T_DISTINCT + "." + FILE_TYPE_CSV)
         file = file_reader.read_file()
         res = metadata.add_om_dataset_t_distinct(self.refactor_file(file))
         result = result and res
         query_values = Query()
         query_values.set_database(connection_type)
         query_values.set_has_header(True)
@@ -147,15 +165,15 @@
         query_values.set_values(metadata.om_dataset_t_distinct)
         self.log.log(self.engine_name, "Loading: " + TABLE_OM_DATASET_T_DISTINCT, LOG_LEVEL_INFO)
         res = self.connection.execute(str(query_values))
         result = result and res
 
         # TABLE_OM_DATASET_SPECIFICATION
         file_reader = FileControllerFactory().get_file_reader(FILE_TYPE_CSV)
-        file_reader.set_file_location(ACTUAL_PATH + '\\' + BACKUP_FILES_PATH,
+        file_reader.set_file_location(os.path.join(ACTUAL_PATH, BACKUP_FILES_PATH),
                                       TABLE_OM_DATASET_SPECIFICATION + "." + FILE_TYPE_CSV)
         file = file_reader.read_file()
         res = metadata.add_om_dataset_specification(self.refactor_file(file))
         result = result and res
         query_values = Query()
         query_values.set_database(connection_type)
         query_values.set_has_header(True)
@@ -165,15 +183,15 @@
         query_values.set_values(metadata.om_dataset_specification)
         self.log.log(self.engine_name, "Loading: " + TABLE_OM_DATASET_SPECIFICATION, LOG_LEVEL_INFO)
         res = self.connection.execute(str(query_values))
         result = result and res
 
         # TABLE_OM_DATASET_RELATIONSHIPS
         file_reader = FileControllerFactory().get_file_reader(FILE_TYPE_CSV)
-        file_reader.set_file_location(ACTUAL_PATH + '\\' + BACKUP_FILES_PATH,
+        file_reader.set_file_location(os.path.join(ACTUAL_PATH, BACKUP_FILES_PATH),
                                       TABLE_OM_DATASET_RELATIONSHIPS + "." + FILE_TYPE_CSV)
         file = file_reader.read_file()
         res = metadata.add_om_dataset_relationships(self.refactor_file(file))
         result = result and res
         query_values = Query()
         query_values.set_database(connection_type)
         query_values.set_has_header(True)
@@ -183,15 +201,15 @@
         query_values.set_values(metadata.om_dataset_relationships)
         self.log.log(self.engine_name, "Loading: " + TABLE_OM_DATASET_RELATIONSHIPS, LOG_LEVEL_INFO)
         res = self.connection.execute(str(query_values))
         result = result and res
 
         # TABLE_OM_DATASET_T_MAPPING
         file_reader = FileControllerFactory().get_file_reader(FILE_TYPE_CSV)
-        file_reader.set_file_location(ACTUAL_PATH + '\\' + BACKUP_FILES_PATH,
+        file_reader.set_file_location(os.path.join(ACTUAL_PATH, BACKUP_FILES_PATH),
                                       TABLE_OM_DATASET_T_MAPPING + "." + FILE_TYPE_CSV)
         file = file_reader.read_file()
         res = metadata.add_om_dataset_t_mapping(self.refactor_file(file))
         result = result and res
         query_values = Query()
         query_values.set_database(connection_type)
         query_values.set_has_header(True)
@@ -201,15 +219,15 @@
         query_values.set_values(metadata.om_dataset_t_mapping)
         self.log.log(self.engine_name, "Loading: " + TABLE_OM_DATASET_T_MAPPING, LOG_LEVEL_INFO)
         res = self.connection.execute(str(query_values))
         result = result and res
 
         # TABLE_OM_DATASET_T_FILTER
         file_reader = FileControllerFactory().get_file_reader(FILE_TYPE_CSV)
-        file_reader.set_file_location(ACTUAL_PATH + '\\' + BACKUP_FILES_PATH,
+        file_reader.set_file_location(os.path.join(ACTUAL_PATH, BACKUP_FILES_PATH),
                                       TABLE_OM_DATASET_T_FILTER + "." + FILE_TYPE_CSV)
         file = file_reader.read_file()
         res = metadata.add_om_dataset_t_filter(self.refactor_file(file))
         result = result and res
         query_values = Query()
         query_values.set_database(connection_type)
         query_values.set_has_header(True)
@@ -219,15 +237,15 @@
         query_values.set_values(metadata.om_dataset_t_filter)
         self.log.log(self.engine_name, "Loading: " + TABLE_OM_DATASET_T_FILTER, LOG_LEVEL_INFO)
         res = self.connection.execute(str(query_values))
         result = result and res
 
         # TABLE_OM_DATASET_T_HAVING
         file_reader = FileControllerFactory().get_file_reader(FILE_TYPE_CSV)
-        file_reader.set_file_location(ACTUAL_PATH + '\\' + BACKUP_FILES_PATH,
+        file_reader.set_file_location(os.path.join(ACTUAL_PATH, BACKUP_FILES_PATH),
                                       TABLE_OM_DATASET_T_HAVING + "." + FILE_TYPE_CSV)
         file = file_reader.read_file()
         res = metadata.add_om_dataset_t_having(self.refactor_file(file))
         result = result and res
         query_values = Query()
         query_values.set_database(connection_type)
         query_values.set_has_header(True)
@@ -237,15 +255,15 @@
         query_values.set_values(metadata.om_dataset_t_having)
         self.log.log(self.engine_name, "Loading: " + TABLE_OM_DATASET_T_HAVING, LOG_LEVEL_INFO)
         res = self.connection.execute(str(query_values))
         result = result and res
 
         # TABLE_OM_DATASET_PATH
         file_reader = FileControllerFactory().get_file_reader(FILE_TYPE_CSV)
-        file_reader.set_file_location(ACTUAL_PATH + '\\' + BACKUP_FILES_PATH,
+        file_reader.set_file_location(os.path.join(ACTUAL_PATH, BACKUP_FILES_PATH),
                                       TABLE_OM_DATASET_PATH + "." + FILE_TYPE_CSV)
         file = file_reader.read_file()
         res = metadata.add_om_dataset_path(self.refactor_file(file))
         result = result and res
         query_values = Query()
         query_values.set_database(connection_type)
         query_values.set_has_header(True)
@@ -255,15 +273,15 @@
         query_values.set_values(metadata.om_dataset_path)
         self.log.log(self.engine_name, "Loading: " + TABLE_OM_DATASET_PATH, LOG_LEVEL_INFO)
         res = self.connection.execute(str(query_values))
         result = result and res
 
         # TABLE_OM_PROPERTIES
         file_reader = FileControllerFactory().get_file_reader(FILE_TYPE_CSV)
-        file_reader.set_file_location(ACTUAL_PATH + '\\' + BACKUP_FILES_PATH,
+        file_reader.set_file_location(os.path.join(ACTUAL_PATH, BACKUP_FILES_PATH),
                                       TABLE_OM_PROPERTIES + "." + FILE_TYPE_CSV)
         file = file_reader.read_file()
         res = metadata.add_om_properties(self.refactor_file_last_col(file))
         result = result and res
         query_values = Query()
         query_values.set_database(connection_type)
         query_values.set_has_header(True)
```

### Comparing `Metamorf-0.3.9.1/metamorf/engines/engine_run.py` & `Metamorf-0.4.3.1/metamorf/engines/engine_run.py`

 * *Files 10% similar despite different names*

```diff
@@ -57,15 +57,17 @@
                 results_nodes.append(node)
                 nodes.remove(node)
 
             index += 1
             if index>=len(nodes): index = 0
 
         self.log.log(self.engine_name, "Finish the execution", LOG_LEVEL_INFO)
-        self.show_results(results_nodes)
+        if len(self.metadata.om_dataset)==0:
+            self.log.log(self.engine_name, "There is no nodes to execute", LOG_LEVEL_WARNING)
+        else: self.show_results(results_nodes)
         super().finish_execution()
 
     def show_results(self, nodes):
         self.log.log("RESULT EXECUTION", "**********************************************", LOG_LEVEL_INFO)
         self.log.log("RESULT EXECUTION", "Summary of the execution", LOG_LEVEL_INFO)
         for node in nodes:
             if node.status == NODE_STATUS_FINISHED_OK:
```

### Comparing `Metamorf-0.3.9.1/metamorf/engines/engine_upload.py` & `Metamorf-0.4.3.1/metamorf/engines/engine_upload.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,54 @@
 from metamorf.engines.engine import Engine
 from metamorf.tools.filecontroller import FileControllerFactory
 from metamorf.tools.connection import ConnectionFactory
 from metamorf.constants import *
 from metamorf.tools.metadata import Metadata
 from metamorf.tools.query import Query
+import os
 
 class EngineUpload(Engine):
 
     def _initialize_engine(self):
         self.engine_name = "Engine Upload"
         self.engine_command = "upload"
 
-        self.entry_files_to_load = [FILE_ENTRY_AGGREGATORS, FILE_ENTRY_DATASET_MAPPINGS, FILE_ENTRY_DATASET_RELATIONSHIPS, FILE_ENTRY_ENTITY, FILE_ENTRY_FILTERS, FILE_ENTRY_ORDER, FILE_ENTRY_PATH,FILE_ENTRY_HAVING, TABLE_ENTRY_AGGREGATORS]
+        self.entry_files_to_load = [FILE_ENTRY_AGGREGATORS, FILE_ENTRY_DATASET_MAPPINGS, FILE_ENTRY_DATASET_RELATIONSHIPS,
+                                    FILE_ENTRY_ENTITY, FILE_ENTRY_FILTERS, FILE_ENTRY_ORDER, FILE_ENTRY_PATH,
+                                    FILE_ENTRY_HAVING, FILE_ENTRY_DV_ENTITY, FILE_ENTRY_DV_PROPERTIES,
+                                    FILE_ENTRY_DV_MAPPINGS, FILE_ENTRY_FILES]
         if 'select' in self.arguments:
             if self.arguments['select'] == "all" or self.arguments['select'] == "*":
-                self.entry_files_to_load = [FILE_ENTRY_AGGREGATORS, FILE_ENTRY_DATASET_MAPPINGS, FILE_ENTRY_DATASET_RELATIONSHIPS, FILE_ENTRY_ENTITY, FILE_ENTRY_FILTERS, FILE_ENTRY_ORDER, FILE_ENTRY_PATH,FILE_ENTRY_HAVING, FILE_ENTRY_AGGREGATORS]
+                self.entry_files_to_load = [FILE_ENTRY_AGGREGATORS, FILE_ENTRY_DATASET_MAPPINGS, FILE_ENTRY_DATASET_RELATIONSHIPS,
+                                            FILE_ENTRY_ENTITY, FILE_ENTRY_FILTERS, FILE_ENTRY_ORDER, FILE_ENTRY_PATH,
+                                            FILE_ENTRY_HAVING, FILE_ENTRY_DV_ENTITY, FILE_ENTRY_DV_PROPERTIES,
+                                            FILE_ENTRY_DV_MAPPINGS, FILE_ENTRY_FILES]
             if self.arguments['select'].lower() == FILE_ENTRY_DATASET_MAPPINGS.lower():
                 self.entry_files_to_load = [FILE_ENTRY_DATASET_MAPPINGS]
             if self.arguments['select'].lower() == FILE_ENTRY_DATASET_RELATIONSHIPS.lower():
                 self.entry_files_to_load = [FILE_ENTRY_DATASET_RELATIONSHIPS]
             if self.arguments['select'].lower() == FILE_ENTRY_ENTITY.lower():
                 self.entry_files_to_load = [FILE_ENTRY_ENTITY]
             if self.arguments['select'].lower() == FILE_ENTRY_FILTERS.lower():
                 self.entry_files_to_load = [FILE_ENTRY_FILTERS]
             if self.arguments['select'].lower() == FILE_ENTRY_ORDER.lower():
                 self.entry_files_to_load = [FILE_ENTRY_ORDER]
             if self.arguments['select'].lower() == FILE_ENTRY_PATH.lower():
                 self.entry_files_to_load = [FILE_ENTRY_PATH]
             if self.arguments['select'].lower() == FILE_ENTRY_HAVING.lower():
                 self.entry_files_to_load = [FILE_ENTRY_HAVING]
-            if self.arguments['select'].lower() == TABLE_ENTRY_AGGREGATORS.lower():
-                self.tables_to_load = [TABLE_ENTRY_AGGREGATORS]
+            if self.arguments['select'].lower() == FILE_ENTRY_DV_ENTITY.lower():
+                self.tables_to_load = [FILE_ENTRY_DV_ENTITY]
+            if self.arguments['select'].lower() == FILE_ENTRY_DV_PROPERTIES.lower():
+                self.tables_to_load = [FILE_ENTRY_DV_PROPERTIES]
+            if self.arguments['select'].lower() == FILE_ENTRY_DV_MAPPINGS.lower():
+                self.tables_to_load = [FILE_ENTRY_DV_MAPPINGS]
+            if self.arguments['select'].lower() == FILE_ENTRY_FILES.lower():
+                self.tables_to_load = [FILE_ENTRY_FILES]
+
 
     def run(self):
         # Starts the execution loading the Configuration File. If there is an error it finishes the execution.
         super().start_execution()
         connection_type = self.configuration_file['metadata']['connection_type']
         self.connection = ConnectionFactory().get_connection(connection_type)
         self.connection.setup_connection(self.configuration_file['metadata'], self.log)
@@ -58,14 +72,15 @@
             query = Query()
             query.set_database(connection_type)
             query.set_type(QUERY_TYPE_DELETE)
             query.set_target_table(file)
             query.set_where_filters([COLUMN_ENTRY_OWNER + "='" + self.owner + "'"])
             res = self.connection.execute(str(query))
             result = result and res
+        self.log.log(self.engine_name, "Finished deleting Metadata Entry on database", LOG_LEVEL_INFO)
         return result
 
     def add_owner_at_end_each_row(self, file: list[list]):
         result = []
         for f in file:
             s = f
             s.append(self.configuration_file['owner'])
@@ -77,17 +92,18 @@
         result = True
         metadata = Metadata(self.log)
         connection_type = self.configuration_file['metadata']['connection_type']
 
         # ENTRY_AGGREGATORS
         if FILE_ENTRY_AGGREGATORS in self.entry_files_to_load:
             file_reader = FileControllerFactory().get_file_reader(FILE_TYPE_CSV)
-            file_reader.set_file_location(ACTUAL_PATH + '\\' + ENTRY_FILES_PATH,
+            file_reader.set_file_location(os.path.join(ACTUAL_PATH, ENTRY_FILES_PATH),
                                           FILE_ENTRY_AGGREGATORS + "." + FILE_TYPE_CSV)
             file = file_reader.read_file()
+
             all_rows = self.add_owner_at_end_each_row(file)
             res = metadata.add_entry_aggregators(all_rows)
             result = result and res
             query_values = Query()
             query_values.set_database(connection_type)
             query_values.set_has_header(True)
             query_values.set_type(QUERY_TYPE_VALUES)
@@ -97,15 +113,15 @@
             self.log.log(self.engine_name, "Loading: " + TABLE_ENTRY_AGGREGATORS, LOG_LEVEL_INFO)
             res = self.connection.execute(str(query_values))
             result = result and res
 
         # ENTRY_DATASET_MAPPINGS
         if FILE_ENTRY_DATASET_MAPPINGS in self.entry_files_to_load:
             file_reader = FileControllerFactory().get_file_reader(FILE_TYPE_CSV)
-            file_reader.set_file_location(ACTUAL_PATH + '\\' + ENTRY_FILES_PATH,
+            file_reader.set_file_location(os.path.join(ACTUAL_PATH, ENTRY_FILES_PATH),
                                           FILE_ENTRY_DATASET_MAPPINGS + "." + FILE_TYPE_CSV)
             file = file_reader.read_file()
             all_rows = self.add_owner_at_end_each_row(file)
             res = metadata.add_entry_dataset_mappings(all_rows)
             result = result and res
             query_values = Query()
             query_values.set_database(connection_type)
@@ -117,15 +133,15 @@
             self.log.log(self.engine_name, "Loading: " + TABLE_ENTRY_DATASET_MAPPINGS, LOG_LEVEL_INFO)
             res = self.connection.execute(str(query_values))
             result = result and res
 
         # ENTRY_DATASET_RELATIONSHIPS
         if FILE_ENTRY_DATASET_RELATIONSHIPS in self.entry_files_to_load:
             file_reader = FileControllerFactory().get_file_reader(FILE_TYPE_CSV)
-            file_reader.set_file_location(ACTUAL_PATH + '\\' + ENTRY_FILES_PATH,
+            file_reader.set_file_location(os.path.join(ACTUAL_PATH, ENTRY_FILES_PATH),
                                           FILE_ENTRY_DATASET_RELATIONSHIPS + "." + FILE_TYPE_CSV)
             file = file_reader.read_file()
             all_rows = self.add_owner_at_end_each_row(file)
             res = metadata.add_entry_dataset_relationship(all_rows)
             result = result and res
             query_values = Query()
             query_values.set_database(connection_type)
@@ -137,15 +153,15 @@
             self.log.log(self.engine_name, "Loading: " + TABLE_ENTRY_DATASET_RELATIONSHIPS, LOG_LEVEL_INFO)
             res = self.connection.execute(str(query_values))
             result = result and res
 
         # ENTRY_ENTITY
         if FILE_ENTRY_ENTITY in self.entry_files_to_load:
             file_reader = FileControllerFactory().get_file_reader(FILE_TYPE_CSV)
-            file_reader.set_file_location(ACTUAL_PATH + '\\' + ENTRY_FILES_PATH, FILE_ENTRY_ENTITY + "." + FILE_TYPE_CSV)
+            file_reader.set_file_location(os.path.join(ACTUAL_PATH, ENTRY_FILES_PATH), FILE_ENTRY_ENTITY + "." + FILE_TYPE_CSV)
             file = file_reader.read_file()
             all_rows = self.add_owner_at_end_each_row(file)
             res = metadata.add_entry_entity(all_rows)
             result = result and res
             query_values = Query()
             query_values.set_database(connection_type)
             query_values.set_has_header(True)
@@ -156,15 +172,15 @@
             self.log.log(self.engine_name, "Loading: " + TABLE_ENTRY_ENTITY, LOG_LEVEL_INFO)
             res = self.connection.execute(str(query_values))
             result = result and res
 
         # ENTRY_FILTERS
         if FILE_ENTRY_FILTERS in self.entry_files_to_load:
             file_reader = FileControllerFactory().get_file_reader(FILE_TYPE_CSV)
-            file_reader.set_file_location(ACTUAL_PATH + '\\' + ENTRY_FILES_PATH, FILE_ENTRY_FILTERS + "." + FILE_TYPE_CSV)
+            file_reader.set_file_location(os.path.join(ACTUAL_PATH, ENTRY_FILES_PATH), FILE_ENTRY_FILTERS + "." + FILE_TYPE_CSV)
             file = file_reader.read_file()
             all_rows = self.add_owner_at_end_each_row(file)
             res = metadata.add_entry_filters(all_rows)
             result = result and res
             query_values = Query()
             query_values.set_database(connection_type)
             query_values.set_has_header(True)
@@ -175,15 +191,15 @@
             self.log.log(self.engine_name, "Loading: " + TABLE_ENTRY_FILTERS, LOG_LEVEL_INFO)
             res = self.connection.execute(str(query_values))
             result = result and res
 
         # ENTRY_HAVING
         if FILE_ENTRY_HAVING in self.entry_files_to_load:
             file_reader = FileControllerFactory().get_file_reader(FILE_TYPE_CSV)
-            file_reader.set_file_location(ACTUAL_PATH + '\\' + ENTRY_FILES_PATH,
+            file_reader.set_file_location(os.path.join(ACTUAL_PATH, ENTRY_FILES_PATH),
                                           FILE_ENTRY_HAVING + "." + FILE_TYPE_CSV)
             file = file_reader.read_file()
             all_rows = self.add_owner_at_end_each_row(file)
             res = metadata.add_entry_having(all_rows)
             result = result and res
             query_values = Query()
             query_values.set_database(connection_type)
@@ -195,15 +211,15 @@
             self.log.log(self.engine_name, "Loading: " + TABLE_ENTRY_HAVING, LOG_LEVEL_INFO)
             res = self.connection.execute(str(query_values))
             result = result and res
 
         # ENTRY_ORDER
         if FILE_ENTRY_ORDER in self.entry_files_to_load:
             file_reader = FileControllerFactory().get_file_reader(FILE_TYPE_CSV)
-            file_reader.set_file_location(ACTUAL_PATH + '\\' + ENTRY_FILES_PATH, FILE_ENTRY_ORDER + "." + FILE_TYPE_CSV)
+            file_reader.set_file_location(os.path.join(ACTUAL_PATH, ENTRY_FILES_PATH), FILE_ENTRY_ORDER + "." + FILE_TYPE_CSV)
             file = file_reader.read_file()
             all_rows = self.add_owner_at_end_each_row(file)
             res = metadata.add_entry_order(all_rows)
             result = result and res
             query_values = Query()
             query_values.set_database(connection_type)
             query_values.set_has_header(True)
@@ -214,15 +230,15 @@
             self.log.log(self.engine_name, "Loading: " + TABLE_ENTRY_ORDER, LOG_LEVEL_INFO)
             res = self.connection.execute(str(query_values))
             result = result and res
 
         # ENTRY_PATH
         if FILE_ENTRY_PATH in self.entry_files_to_load:
             file_reader = FileControllerFactory().get_file_reader(FILE_TYPE_CSV)
-            file_reader.set_file_location(ACTUAL_PATH + '\\' + ENTRY_FILES_PATH, FILE_ENTRY_PATH + "." + FILE_TYPE_CSV)
+            file_reader.set_file_location(os.path.join(ACTUAL_PATH, ENTRY_FILES_PATH), FILE_ENTRY_PATH + "." + FILE_TYPE_CSV)
             file = file_reader.read_file()
             all_rows = self.add_owner_at_end_each_row(file)
             res = metadata.add_entry_path(all_rows)
             result = result and res
             query_values = Query()
             query_values.set_database(connection_type)
             query_values.set_has_header(True)
@@ -230,8 +246,88 @@
             query_values.set_target_table(TABLE_ENTRY_PATH)
             query_values.set_insert_columns(COLUMNS_ENTRY_PATH)
             query_values.set_values(metadata.entry_path)
             self.log.log(self.engine_name, "Loading: " + TABLE_ENTRY_PATH, LOG_LEVEL_INFO)
             res = self.connection.execute(str(query_values))
             result = result and res
 
+        # ENTRY_DV_ENTITY
+        if FILE_ENTRY_DV_ENTITY in self.entry_files_to_load:
+            file_reader = FileControllerFactory().get_file_reader(FILE_TYPE_CSV)
+            file_reader.set_file_location(os.path.join(ACTUAL_PATH, ENTRY_FILES_PATH),
+                                          FILE_ENTRY_DV_ENTITY + "." + FILE_TYPE_CSV)
+            file = file_reader.read_file()
+            all_rows = self.add_owner_at_end_each_row(file)
+            res = metadata.add_entry_dv_entity(all_rows)
+            result = result and res
+            query_values = Query()
+            query_values.set_database(connection_type)
+            query_values.set_has_header(True)
+            query_values.set_type(QUERY_TYPE_VALUES)
+            query_values.set_target_table(TABLE_ENTRY_DV_ENTITY)
+            query_values.set_insert_columns(COLUMNS_ENTRY_DV_ENTITY)
+            query_values.set_values(metadata.entry_dv_entity)
+            self.log.log(self.engine_name, "Loading: " + TABLE_ENTRY_DV_ENTITY, LOG_LEVEL_INFO)
+            res = self.connection.execute(str(query_values))
+            result = result and res
+
+        # ENTRY_DV_MAPPINGS
+        if FILE_ENTRY_DV_MAPPINGS in self.entry_files_to_load:
+            file_reader = FileControllerFactory().get_file_reader(FILE_TYPE_CSV)
+            file_reader.set_file_location(os.path.join(ACTUAL_PATH, ENTRY_FILES_PATH), FILE_ENTRY_DV_MAPPINGS + "." + FILE_TYPE_CSV)
+            file = file_reader.read_file()
+            all_rows = self.add_owner_at_end_each_row(file)
+            res = metadata.add_entry_dv_mappings(all_rows)
+            result = result and res
+            query_values = Query()
+            query_values.set_database(connection_type)
+            query_values.set_has_header(True)
+            query_values.set_type(QUERY_TYPE_VALUES)
+            query_values.set_target_table(TABLE_ENTRY_DV_MAPPINGS)
+            query_values.set_insert_columns(COLUMNS_ENTRY_DV_MAPPINGS)
+            query_values.set_values(metadata.entry_dv_mappings)
+            self.log.log(self.engine_name, "Loading: " + TABLE_ENTRY_DV_MAPPINGS, LOG_LEVEL_INFO)
+            res = self.connection.execute(str(query_values))
+            result = result and res
+
+        # ENTRY_DV_PROPERTIES
+        if FILE_ENTRY_DV_PROPERTIES in self.entry_files_to_load:
+            file_reader = FileControllerFactory().get_file_reader(FILE_TYPE_CSV)
+            file_reader.set_file_location(os.path.join(ACTUAL_PATH, ENTRY_FILES_PATH),
+                                          FILE_ENTRY_DV_PROPERTIES + "." + FILE_TYPE_CSV)
+            file = file_reader.read_file()
+            all_rows = self.add_owner_at_end_each_row(file)
+            res = metadata.add_entry_dv_properties(all_rows)
+            result = result and res
+            query_values = Query()
+            query_values.set_database(connection_type)
+            query_values.set_has_header(True)
+            query_values.set_type(QUERY_TYPE_VALUES)
+            query_values.set_target_table(TABLE_ENTRY_DV_PROPERTIES)
+            query_values.set_insert_columns(COLUMNS_ENTRY_DV_PROPERTIES)
+            query_values.set_values(metadata.entry_dv_properties)
+            self.log.log(self.engine_name, "Loading: " + TABLE_ENTRY_DV_PROPERTIES, LOG_LEVEL_INFO)
+            res = self.connection.execute(str(query_values))
+            result = result and res
+
+        # ENTRY_FILES
+        if FILE_ENTRY_FILES in self.entry_files_to_load:
+            file_reader = FileControllerFactory().get_file_reader(FILE_TYPE_CSV)
+            file_reader.set_file_location(os.path.join(ACTUAL_PATH, ENTRY_FILES_PATH),
+                                          FILE_ENTRY_FILES + "." + FILE_TYPE_CSV)
+            file = file_reader.read_file()
+            all_rows = self.add_owner_at_end_each_row(file)
+            res = metadata.add_entry_files(all_rows)
+            result = result and res
+            query_values = Query()
+            query_values.set_database(connection_type)
+            query_values.set_has_header(True)
+            query_values.set_type(QUERY_TYPE_VALUES)
+            query_values.set_target_table(TABLE_ENTRY_FILES)
+            query_values.set_insert_columns(COLUMNS_ENTRY_FILES)
+            query_values.set_values(metadata.entry_files)
+            self.log.log(self.engine_name, "Loading: " + TABLE_ENTRY_FILES, LOG_LEVEL_INFO)
+            res = self.connection.execute(str(query_values))
+            result = result and res
+
+        self.log.log(self.engine_name, "Finished uploading Metadata Entry on database", LOG_LEVEL_INFO)
         return result
```

### Comparing `Metamorf-0.3.9.1/metamorf/engines/engine_validate.py` & `Metamorf-0.4.3.1/metamorf/engines/engine_validate.py`

 * *Files identical despite different names*

### Comparing `Metamorf-0.3.9.1/metamorf/help.py` & `Metamorf-0.4.3.1/metamorf/help.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from metamorf.tools.filecontroller import FileControllerFactory
 from metamorf.constants import *
+import os
 
 def print_help():
     file_controller_properties = FileControllerFactory().get_file_reader(FILE_TYPE_YML)
-    file_controller_properties.set_file_location(PACKAGE_PATH + '\\' + PROPERTIES_FILE_PATH, PROPERTIES_FILE_NAME)
+    file_controller_properties.set_file_location(os.path.join(PACKAGE_PATH, PROPERTIES_FILE_PATH), PROPERTIES_FILE_NAME)
     properties_file = file_controller_properties.read_file()
 
     print()
     print(properties_file['description'])
     print()
     print('usage: metamorf [command] [arguments]')
     print()
```

### Comparing `Metamorf-0.3.9.1/metamorf/initialization/init_example_data_snowflake.sql` & `Metamorf-0.4.3.1/metamorf/initialization/mysql/init_example_data_mysql.sql`

 * *Files 15% similar despite different names*

```diff
@@ -1,80 +1,97 @@
 /********************** CREATE DATABASE ***********************/
-create database if not exists METAMORF;
-create or replace SCHEMA DATA;
+create database if not exists metamorf_data_example;
 
 /********************** RESET DATABASE ***********************/
-drop table if exists METAMORF.DATA.AIRCRAFTS;
-drop table if exists METAMORF.DATA.AIRPORTS;
-drop table if exists METAMORF.DATA.CARRIERS;
-drop table if exists METAMORF.DATA.FLIGHTS;
-drop table if exists METAMORF.DATA.CUSTOMERS;
-drop table if exists METAMORF.DATA.USERS_WEB;
-drop table if exists METAMORF.DATA.FLIGHTS_TMP;
+drop table if exists AIRCRAFTS;
+drop table if exists AIRPORTS;
+drop table if exists CARRIERS;
+drop table if exists FLIGHTS;
+drop table if exists CUSTOMERS;
+drop table if exists USERS_WEB;
+drop table if exists FLIGHTS_TMP;
+drop table if exists AIRCRAFTS_TMP;
+drop table if exists CUSTOMERS_TMP;
+drop table if exists HUB_CUSTOMER;
+drop table if exists HUB_FLIGHTS;
+drop table if exists SAT_CUSTOMER_INFO;
+drop table if exists SAT_FLIGHTS_ICAO;
+drop table if exists SAT_CUSTOMER_LEGAL;
+drop table if exists LINK_SELLS;
+drop table if exists SAT_FLIGHTS_ICAO;
+drop table if exists SAT_SELL_EVENT;
+drop table if exists SAT_SELL_PROPERTIES;
+drop table if exists SAT_LAST_APPEAR_DATE;
+drop table if exists HUB_AIRPORTS;
+drop table if exists LINK_AIRPORTS_FLIGHTS;
+drop table if exists RTS_AIRPORTS;
+drop table if exists RTS_CUSTOMER;
+drop table if exists RTS_SELLS;
+drop table if exists SATE_AIRPORTS_FLIGHTS;
 
 /******************** CREATION DATABASE **********************/
-CREATE TABLE METAMORF.DATA.AIRCRAFTS (
+CREATE TABLE AIRCRAFTS (
 	LICENSE VARCHAR(50),
 	MODEL_ICAO VARCHAR(50),
 	NAME VARCHAR(50),
 	AIRCRAFTS_BY VARCHAR(50),
 	AIRCRAFTS_TYPE VARCHAR(50),
 	APC VARCHAR(50),
 	WTC VARCHAR(50),
 	ALTERNATIVE_NAME VARCHAR(50),
 	CARRIER_IATA VARCHAR(50)
 );
 
-INSERT INTO METAMORF.DATA.AIRCRAFTS (LICENSE,MODEL_ICAO,NAME,AIRCRAFTS_BY,AIRCRAFTS_TYPE,APC,WTC,ALTERNATIVE_NAME,CARRIER_IATA) VALUES
+INSERT INTO AIRCRAFTS (LICENSE,MODEL_ICAO,NAME,AIRCRAFTS_BY,AIRCRAFTS_TYPE,APC,WTC,ALTERNATIVE_NAME,CARRIER_IATA) VALUES
  ('EC-GAS','A320','A320','AIRBUS','L2J','C','M','AIRBUS A-320','VY'),
  ('EC-ZOO','A320','A320','AIRBUS','L2J','C','M','AIRBUS A-320','VY'),
  ('I-RES','B738','737-800','BOEING','L2J','D','M','BOEING 737-800','FR'),
  ('G-YAK','A35K','A350-1000 XWB','AIRBUS','L2J','D','H','A-350-1000 XWB Prestige','BA'),
  ('I-HHH','A320','A320','AIRBUS','L2J','C','M','AIRBUS A-320','FR');
 
-CREATE TABLE METAMORF.DATA.AIRPORTS (
+CREATE TABLE AIRPORTS (
 	IDENT VARCHAR(50),
 	AIRPORTS_TYPE VARCHAR(50),
 	NAME VARCHAR(50),
 	ELEVATION INTEGER,
 	CONTINENT VARCHAR(50),
 	ISO_COUNTRY VARCHAR(50),
 	ISO_REGION VARCHAR(50),
 	MUNICIPALITY VARCHAR(50),
 	GPS_CODE VARCHAR(50),
 	IATA_CODE VARCHAR(50),
 	LOCAL_CODE VARCHAR(50),
 	COORDINATES VARCHAR(50)
 );
 
-INSERT INTO METAMORF.DATA.AIRPORTS (IDENT,AIRPORTS_TYPE,NAME,ELEVATION,CONTINENT,ISO_COUNTRY,ISO_REGION,MUNICIPALITY,GPS_CODE,IATA_CODE,LOCAL_CODE,COORDINATES) VALUES
+INSERT INTO AIRPORTS (IDENT,AIRPORTS_TYPE,NAME,ELEVATION,CONTINENT,ISO_COUNTRY,ISO_REGION,MUNICIPALITY,GPS_CODE,IATA_CODE,LOCAL_CODE,COORDINATES) VALUES
  ('LEBL','large_airport','Barcelona International Airport',12,'EU','ES','ES-CT','Barcelona','LEBL','BCN','','41.2971, 2.07846'),
  ('LEPA','large_airport','Palma De Mallorca Airport',27,'EU','ES','ES-PM','Palma De Mallorca','LEPA','PMI','','39.551700592, 2.73881006241'),
  ('LIPE','large_airport','Bologna Guglielmo Marconi Airport',123,'EU','IT','IT-45','Bologna','LIPE','BLQ','BO08','44.5354, 11.2887'),
  ('LEIB','medium_airport','Ibiza Airport',24,'EU','ES','ES-PM','Ibiza','LEIB','IBZ','','38.872898101800004, 1.3731199502899998'),
  ('LEVC','medium_airport','Valencia Airport',240,'EU','ES','ES-V','Valencia','LEVC','VLC','','39.4893, -0.481625');
 
-CREATE TABLE METAMORF.DATA.CARRIERS (
+CREATE TABLE CARRIERS (
 	ICAO VARCHAR(50),
 	IATA VARCHAR(50),
 	CALLSIGN VARCHAR(50),
 	NAME VARCHAR(50),
 	FOUNDED VARCHAR(50),
 	COMMENCED_OPERATIONS VARCHAR(50),
 	PARENT_COMPANY VARCHAR(50),
 	FLEET_SIZE INTEGER,
 	DESTINATIONS INTEGER
 );
 
-INSERT INTO METAMORF.DATA.CARRIERS (ICAO,IATA,CALLSIGN,NAME,FOUNDED,COMMENCED_OPERATIONS,PARENT_COMPANY,FLEET_SIZE,DESTINATIONS) VALUES
+INSERT INTO CARRIERS (ICAO,IATA,CALLSIGN,NAME,FOUNDED,COMMENCED_OPERATIONS,PARENT_COMPANY,FLEET_SIZE,DESTINATIONS) VALUES
  ('VLG','VY','VUELING','Vueling Airlines','10/02/2004','01/07/2004','IAG',126,148),
  ('RYR','FR','RYAN','Ryanair','28/11/1984','08/07/1985','Ryanair Holdings plc',514,225),
  ('BAW','BA','SPEEDBIRD','Brithish Aiwrways','31/03/1974','31/03/1974','International Airlines Group',257,183);
 
-CREATE TABLE METAMORF.DATA.FLIGHTS (
+CREATE TABLE FLIGHTS (
 	UNIQUE_FLIGHT_CODE VARCHAR(50),
 	FLIGHT_CODE VARCHAR(50),
 	AIRPORT_ORIGIN_CODE VARCHAR(50),
 	AIRPORT_DEST_CODE VARCHAR(50),
 	DEPARTURE_GATE VARCHAR(50),
 	BOARDING_TIME VARCHAR(50),
 	DEPARTURE_TIME VARCHAR(50),
@@ -84,42 +101,39 @@
 	BOARDING_TIME_REAL VARCHAR(50),
 	DEPARTURE_TIME_REAL VARCHAR(50),
 	LANDING_TIME_REAL VARCHAR(50),
 	ARRIVAL_TIME_REAL VARCHAR(50),
 	OPERATION VARCHAR(50)
 );
 
-INSERT INTO METAMORF.DATA.FLIGHTS (UNIQUE_FLIGHT_CODE,FLIGHT_CODE,AIRPORT_ORIGIN_CODE,AIRPORT_DEST_CODE,DEPARTURE_GATE,BOARDING_TIME,DEPARTURE_TIME,LANDING_TIME,ARRIVAL_TIME,AIRCRAFT,BOARDING_TIME_REAL,DEPARTURE_TIME_REAL,LANDING_TIME_REAL,ARRIVAL_TIME_REAL,OPERATION) VALUES
+INSERT INTO FLIGHTS (UNIQUE_FLIGHT_CODE,FLIGHT_CODE,AIRPORT_ORIGIN_CODE,AIRPORT_DEST_CODE,DEPARTURE_GATE,BOARDING_TIME,DEPARTURE_TIME,LANDING_TIME,ARRIVAL_TIME,AIRCRAFT,BOARDING_TIME_REAL,DEPARTURE_TIME_REAL,LANDING_TIME_REAL,ARRIVAL_TIME_REAL,OPERATION) VALUES
  ('VLG390820221008','VLG3908','BCN','PMI','B39','08/10/2022 11:45','08/10/2022 11:55','08/10/2022 12:31','08/10/2022 12:40','EC-GAS','','','','','I'),
  ('VLG390920221008','VLG3909','PMI','BCN','D86','08/10/2022 13:15','08/10/2022 13:25','08/10/2022 14:01','08/10/2022 14:10','EC-ZOO','','','','','I'),
  ('RYR936620221008','RYR9366','BCN','BLQ','Terminal 2','08/10/2022 15:30','08/10/2022 15:40','08/10/2022 17:03','08/10/2022 17:13','I-RES','','','','','I'),
  ('BAW19020221007','BAW190','AUS','LHR','Terminal 5','07/10/2022 18:20','07/10/2022 18:30','07/10/2022 15:27','07/10/2022 15:45','G-YAK','','','','','I'),
  ('VLG369420221006','VLG3694','IBZ','VLC','Puerta 6','06/10/2022 13:25','06/10/2022 13:35','06/10/2022 14:06','06/10/2022 14:15','I-HHH','','','','','I');
 
 
-CREATE TABLE METAMORF.DATA.CUSTOMERS (
+CREATE TABLE CUSTOMERS (
     ID_CUSTOMER INTEGER,
-    CUSTOMER_NAME VARCHAR(50),
+    NAME VARCHAR(50),
     NIE VARCHAR(50),
     PRICE INTEGER,
     SELL_DATE VARCHAR(50),
     ADDRESS VARCHAR(50),
     NATIONALITY VARCHAR(10),
     FLIGHT_CODE VARCHAR(50)
 );
 
-INSERT INTO METAMORF.DATA.CUSTOMERS (ID_CUSTOMER, CUSTOMER_NAME, NIE, PRICE, SELL_DATE, ADDRESS, NATIONALITY, FLIGHT_CODE) VALUES
-(0, 'Guillermo Aumatell', 'ZAB000000', 30, '28/09/2022 16:03', 'Avda. Principal, 3o 4a', 'ES', 'VLG3694'),
-(1, 'William Smith', '123456789', 28.50, '03/05/2022 12:24', 'Main Street, 48', 'UK', 'VLG3908');
+INSERT INTO CUSTOMERS (ID_CUSTOMER, NAME, NIE, PRICE, SELL_DATE, ADDRESS, NATIONALITY, FLIGHT_CODE) VALUES
+(0, "Guillermo Aumatell", "ZAB000000", 30, '28/09/2022 16:03', 'Avda. Principal, 3o 4a', 'ES', 'VLG3694'),
+(1, "William Smith", "123456789", 28.50, '03/05/2022 12:24', 'Main Street, 48', 'UK', 'VLG3908');
 
-CREATE TABLE METAMORF.DATA.USERS_WEB (
+CREATE TABLE USERS_WEB (
     ID_CUSTOMER INTEGER,
     VISIT_DATE VARCHAR(50),
     TIME_ONLINE_SECONDS INTEGER
 );
 
-insert into METAMORF.DATA.USERS_WEB (ID_CUSTOMER, VISIT_DATE, TIME_ONLINE_SECONDS) VALUES
+insert into USERS_WEB (ID_CUSTOMER, VISIT_DATE, TIME_ONLINE_SECONDS) VALUES
 (0, '26/09/2022 06:03', 124),(0, '27/09/2022 11:48', 82),(0, '28/09/2022 16:00', 501),
-(1, '03/05/2022 12:23', 258), (1, '03/05/2022 12:22', 0);
-
-
-
+(1, '03/05/2022 12:23', 258), (1, '03/05/2022 12:22', 0);
```

### Comparing `Metamorf-0.3.9.1/metamorf/initialization/init_example_data_sqlite.sql` & `Metamorf-0.4.3.1/metamorf/initialization/sqlite/init_example_data_sqlite.sql`

 * *Files 22% similar despite different names*

```diff
@@ -4,14 +4,31 @@
 drop table if exists CARRIERS;
 drop table if exists FLIGHTS;
 drop table if exists CUSTOMERS;
 drop table if exists USERS_WEB;
 drop table if exists FLIGHTS_TMP;
 drop table if exists AIRCRAFTS_TMP;
 drop table if exists CUSTOMERS_TMP;
+drop table if exists HUB_CUSTOMER;
+drop table if exists HUB_FLIGHTS;
+drop table if exists SAT_CUSTOMER_INFO;
+drop table if exists SAT_FLIGHTS_ICAO;
+drop table if exists SAT_CUSTOMER_LEGAL;
+drop table if exists LINK_SELLS;
+drop table if exists SAT_FLIGHTS_ICAO;
+drop table if exists SAT_SELL_EVENT;
+drop table if exists SAT_SELL_PROPERTIES;
+drop table if exists STS_CUSTOMER;
+drop table if exists SAT_LAST_APPEAR_DATE;
+drop table if exists HUB_AIRPORTS;
+drop table if exists LINK_AIRPORTS_FLIGHTS;
+drop table if exists RTS_AIRPORTS;
+drop table if exists RTS_CUSTOMER;
+drop table if exists RTS_SELLS;
+drop table if exists SATE_AIRPORTS_FLIGHTS;
 
 /******************** CREATION DATABASE **********************/
 CREATE TABLE AIRCRAFTS (
 	LICENSE VARCHAR(50),
 	MODEL_ICAO VARCHAR(50),
 	NAME VARCHAR(50),
 	AIRCRAFTS_BY VARCHAR(50),
```

### Comparing `Metamorf-0.3.9.1/metamorf/initialization/init_snowflake.sql` & `Metamorf-0.4.3.1/metamorf/initialization/snowflake/init_snowflake.sql`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,56 @@
 /********************** RESET DATABASE ***********************/
-DROP TABLE IF EXISTS ENTRY_PATH;
 DROP TABLE IF EXISTS OM_DATASET_HARDCODED;
 DROP TABLE IF EXISTS OM_DATASET_PATH;
 DROP TABLE IF EXISTS OM_PROPERTIES;
 DROP TABLE IF EXISTS OM_REF_JOIN_TYPE;
 DROP TABLE IF EXISTS OM_REF_KEY_TYPE;
 DROP TABLE IF EXISTS OM_REF_MODULES;
 DROP TABLE IF EXISTS OM_REF_ORDER_TYPE;
 DROP TABLE IF EXISTS OM_REF_QUERY_TYPE;
 DROP TABLE IF EXISTS OM_REF_ENTITY_TYPE;
 DROP TABLE IF EXISTS ENTRY_ENTITY;
 DROP TABLE IF EXISTS ENTRY_FILTERS;
 DROP TABLE IF EXISTS ENTRY_ORDER;
+DROP TABLE IF EXISTS ENTRY_HAVING;
+DROP TABLE IF EXISTS ENTRY_PATH;
+DROP TABLE IF EXISTS ENTRY_AGGREGATORS;
+DROP TABLE IF EXISTS ENTRY_DATASET_MAPPINGS;
+DROP TABLE IF EXISTS ENTRY_DATASET_RELATIONSHIPS;
 DROP TABLE IF EXISTS OM_DATASET;
+DROP TABLE IF EXISTS OM_DATASET_DV;
 DROP TABLE IF EXISTS OM_DATASET_EXECUTION;
 DROP TABLE IF EXISTS OM_DATASET_SPECIFICATION;
 DROP TABLE IF EXISTS OM_DATASET_T_AGG;
 DROP TABLE IF EXISTS OM_DATASET_T_DISTINCT;
 DROP TABLE IF EXISTS OM_DATASET_T_FILTER;
 DROP TABLE IF EXISTS OM_DATASET_T_HAVING;
 DROP TABLE IF EXISTS OM_DATASET_T_MAPPING;
 DROP TABLE IF EXISTS OM_DATASET_T_ORDER;
-DROP TABLE IF EXISTS ENTRY_AGGREGATORS;
-DROP TABLE IF EXISTS ENTRY_DATASET_MAPPINGS;
-DROP TABLE IF EXISTS ENTRY_DATASET_RELATIONSHIPS;
 DROP TABLE IF EXISTS OM_DATASET_RELATIONSHIPS;
-DROP TABLE IF EXISTS ENTRY_HAVING;
+DROP TABLE IF EXISTS GIT_ENTRY_ENTITY;
+DROP TABLE IF EXISTS GIT_ENTRY_FILTERS;
+DROP TABLE IF EXISTS GIT_ENTRY_ORDER;
+DROP TABLE IF EXISTS GIT_ENTRY_HAVING;
+DROP TABLE IF EXISTS GIT_ENTRY_PATH;
+DROP TABLE IF EXISTS GIT_ENTRY_AGGREGATORS;
+DROP TABLE IF EXISTS GIT_ENTRY_DATASET_MAPPINGS;
+DROP TABLE IF EXISTS GIT_ENTRY_DATASET_RELATIONSHIPS;
 DROP VIEW IF EXISTS OM_DATASET_INFORMATION;
+DROP VIEW IF EXISTS OM_RELATIONSHIPS;
 DROP VIEW IF EXISTS OM_DATASET_SPECIFICATION_INFORMATION;
-drop view if exists OM_RELATIONSHIPS;
+DROP TABLE IF EXISTS ENTRY_DV_MAPPINGS;
+DROP TABLE IF EXISTS ENTRY_DV_ENTITY;
+drop table if exists ENTRY_DV_PROPERTIES;
+drop table if exists GIT_ENTRY_DV_ENTITY;
+drop table if exists GIT_ENTRY_DV_MAPPINGS;
+drop table if exists GIT_ENTRY_DV_PROPERTIES;
+drop table if exists ENTRY_FILES;
+drop table if exists GIT_ENTRY_FILES;
+drop table if exists OM_DATASET_FILE;
 
 /********************** CREATION TABLES **********************/
 CREATE TABLE ENTRY_PATH (
 	COD_PATH             text NOT NULL  PRIMARY KEY  ,
 	DATABASE_NAME        text     ,
 	SCHEMA_NAME          text     ,
 	OWNER                text
@@ -341,42 +359,85 @@
 	COD_ENTITY_DETAIL    text     ,
 	COLUMN_NAME_DETAIL   text     ,
 	RELATIONSHIP_TYPE    text     ,
 	OWNER                text
  );
 
 CREATE TABLE ENTRY_DV_ENTITY (
-	COD_ENTITY           text     ,
-	SW_STATUS_TRACKING_SATELLITE integer     ,
+	COD_ENTITY           text NOT NULL  PRIMARY KEY  ,
+	ENTITY_NAME          text     ,
+	ENTITY_TYPE          text     ,
+	COD_PATH             text     ,
 	NAME_STATUS_TRACKING_SATELLITE text     ,
-	SW_RECORD_TRACKING_SATELLITE integer     ,
 	NAME_RECORD_TRACKING_SATELLITE text     ,
-	SW_EFFECTIVITY_SATELLITE integer     ,
 	NAME_EFFECTIVITY_SATELLITE text     ,
-	RECORD_SOURCE        text     ,
-	ORIGIN_IS_INCREMENTAL integer     ,
-	ORIGIN_IS_TOTAL      integer     ,
-	ORIGIN_IS_CDC        integer     ,
 	OWNER                text
  );
 
 CREATE TABLE ENTRY_DV_MAPPINGS (
-	COD_ENTITY           text     ,
+	COD_ENTITY_SOURCE    text     ,
 	COLUMN_NAME_SOURCE   text     ,
+	COD_ENTITY_TARGET    text     ,
 	COLUMN_NAME_TARGET   text     ,
 	COLUMN_TYPE_TARGET   text     ,
 	ORDINAL_POSITION     text     ,
 	LENGTH               integer     ,
 	PRECISION            integer     ,
 	NUM_BRANCH           integer     ,
-	KEY_TYPE             integer     ,
+	NUM_CONNECTION       integer     ,
+	KEY_TYPE             text     ,
 	SATELLITE_NAME       text     ,
+	ORIGIN_IS_INCREMENTAL integer     ,
+	ORIGIN_IS_TOTAL      integer     ,
+	ORIGIN_IS_CDC        integer     ,
+	OWNER                text
+ );
+
+CREATE TABLE ENTRY_DV_PROPERTIES (
+    COD_ENTITY           text     ,
+    NUM_CONNECTION       text     ,
+    HASH_NAME            text     ,
+    OWNER                text
+);
+
+ CREATE TABLE OM_DATASET_DV (
+	ID_DATASET           integer     ,
+	ID_ENTITY_TYPE       integer     ,
+	META_OWNER           text     ,
+	START_DATE           timestamp     ,
+	END_DATE             timestamp
+ );
+
+CREATE TABLE ENTRY_FILES (
+	COD_ENTITY           text     ,
+	FILE_PATH            text     ,
+	FILE_NAME            text     ,
+	DELIMITER_CHARACTER  text     ,
+	OWNER                text
+ );
+
+CREATE TABLE GIT_ENTRY_FILES (
+	COD_ENTITY           text     ,
+	FILE_PATH            text     ,
+	FILE_NAME            text     ,
+	DELIMITER_CHARACTER  text     ,
 	OWNER                text
  );
 
+CREATE TABLE OM_DATASET_FILE (
+	ID_DATASET           integer     ,
+	FILE_PATH            text     ,
+	FILE_NAME            text     ,
+	DELIMITER_CHARACTER  text     ,
+	META_OWNER           text     ,
+	START_DATE           date     ,
+	END_DATE             date
+ );
+
+
 
 
 
 CREATE VIEW OM_DATASET_INFORMATION AS select A.META_OWNER, B.ENTITY_TYPE_FULL_NAME, B.ENTITY_TYPE_DESCRIPTION, C.MODULE_NAME, C.MODULE_FULL_NAME, C.MODULE_DESCRIPTION, A.DATASET_NAME,  D.DATABASE_NAME, D.SCHEMA_NAME, F.QUERY_TYPE_NAME , F.QUERY_TYPE_DESCRIPTION , A.START_DATE
 From OM_DATASET A
 LEFT JOIN OM_REF_ENTITY_TYPE B on A.ID_ENTITY_TYPE = B.ID_ENTITY_TYPE
 LEFT JOIN OM_REF_MODULES C on B.ID_MODULE = C.ID_MODULE
@@ -413,26 +474,30 @@
 INSERT INTO OM_REF_ENTITY_TYPE (ID_ENTITY_TYPE, ENTITY_TYPE_NAME, ENTITY_TYPE_DESCRIPTION, ENTITY_TYPE_FULL_NAME, ID_MODULE) VALUES
 (0, 'SRC', 'Source of the run. It need to be loaded from other sources', 'Source', 0),
 (1, 'VIEW', 'Temporary table. It will be not materialized', 'Temporary', 0),
 (2, 'TB', 'Table. It''s the result of a process', 'Table', 0),
 (3, 'WITH', 'With Clause', 'With', 0),
 (4, 'HUB', 'Datavault - Hub', 'Hub', 1),
 (5, 'LINK', 'Datavault - Link', 'Link', 1),
-(6, 'SAT', ' Datavault - Satellite', 'Satellite', '1');
+(6, 'SAT', ' Datavault - Satellite', 'Satellite', 1),
+(7, 'STS', 'Datavault - Status Tracking Satellite', 'Status Tracking Satellite', 1),
+(8, 'RTS', 'Datavault - Satellite', 'Record Tracking Satellite', 1),
+(9, 'SATE', 'Datavault - Effectivity Satellite', 'Effectivity Satellite', 1);
 
 INSERT INTO OM_REF_JOIN_TYPE(ID_JOIN_TYPE, JOIN_NAME, JOIN_VALUE, JOIN_DESCRIPTION) VALUES
 (0, 'INNER JOIN', 'INNER JOIN', 'Returns only those rows that have matching values'),
 (1, 'MASTER JOIN', 'LEFT JOIN', 'Returns those rows from the left table plus those that have matching values'),
 (2, 'DETAIL JOIN', 'RIGHT JOIN', 'Returns those rows from the right table plus those that have matching values'),
 (3, 'OUTER JOIN', 'OUTER JOIN', 'Returns rows from both tables');
 
 INSERT INTO OM_REF_KEY_TYPE(ID_KEY_TYPE, KEY_TYPE_NAME, KEY_TYPE_DESCRIPTION) VALUES
 (0, 'PK', 'Primary Key'), (1, 'BK', 'Business Key'), (2,'NULL', 'Nothing'), (3,'SEQ', 'Sequence'),
 (4, 'FK', 'Foreign Key'), (5, 'HK', 'Hash Key'), (6, 'AT', 'Attribute'), (7 ,'ST','Status'),
-(8, 'DK', 'Driven Key');
+(8, 'DK', 'Driven Key'), (9, 'RS', 'Record Source'), (10, 'TN', 'Tenant'), (11,'HD', 'Hashdiff'),
+(12, 'DCK', 'Dependent-child key'), (13, 'AD', 'Applied Date');
 
 INSERT INTO OM_REF_ORDER_TYPE(ID_ORDER_TYPE, ORDER_TYPE_NAME, ORDER_TYPE_VALUE, ORDER_TYPE_DESCRIPTION) VALUES
 (0, 'Ascendant', 'ASC', 'Ascending order'),
 (1, 'Descendant', 'DESC', 'Descending order');
 
 INSERT INTO OM_REF_QUERY_TYPE(ID_QUERY_TYPE, QUERY_TYPE_NAME, QUERY_TYPE_DESCRIPTION) VALUES
 (0, 'INSERT', 'Insert on the target table'),
@@ -441,8 +506,9 @@
 (3, 'DELETE', 'Deletes based on the Primary Key'),
 (4, 'SELECT', 'Select the target query'),
 (5, 'MERGE', 'Select the target query'),
 (6, 'TRUNCATE AND INSERT', 'Truncate the target table and inserts');
 
 INSERT INTO OM_PROPERTIES(PROPERTY, "VALUE", START_DATE) VALUES
 ('Version', '0.3.9b', CURRENT_TIMESTAMP()),
-('Module Deployed', 'ELT', CURRENT_TIMESTAMP());
+('Module Deployed', 'ELT', CURRENT_TIMESTAMP()),
+('Module Deployed', 'DV', CURRENT_TIMESTAMP());
```

### Comparing `Metamorf-0.3.9.1/metamorf/initialization/init_sqlite.sql` & `Metamorf-0.4.3.1/metamorf/initialization/sqlite/init_sqlite.sql`

 * *Files 10% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 DROP TABLE IF EXISTS ENTRY_ORDER;
 DROP TABLE IF EXISTS ENTRY_HAVING;
 DROP TABLE IF EXISTS ENTRY_PATH;
 DROP TABLE IF EXISTS ENTRY_AGGREGATORS;
 DROP TABLE IF EXISTS ENTRY_DATASET_MAPPINGS;
 DROP TABLE IF EXISTS ENTRY_DATASET_RELATIONSHIPS;
 DROP TABLE IF EXISTS OM_DATASET;
+DROP TABLE IF EXISTS OM_DATASET_DV;
 DROP TABLE IF EXISTS OM_DATASET_EXECUTION;
 DROP TABLE IF EXISTS OM_DATASET_SPECIFICATION;
 DROP TABLE IF EXISTS OM_DATASET_T_AGG;
 DROP TABLE IF EXISTS OM_DATASET_T_DISTINCT;
 DROP TABLE IF EXISTS OM_DATASET_T_FILTER;
 DROP TABLE IF EXISTS OM_DATASET_T_HAVING;
 DROP TABLE IF EXISTS OM_DATASET_T_MAPPING;
@@ -35,14 +36,21 @@
 DROP TABLE IF EXISTS GIT_ENTRY_DATASET_MAPPINGS;
 DROP TABLE IF EXISTS GIT_ENTRY_DATASET_RELATIONSHIPS;
 DROP VIEW IF EXISTS OM_DATASET_INFORMATION;
 DROP VIEW IF EXISTS OM_RELATIONSHIPS;
 DROP VIEW IF EXISTS OM_DATASET_SPECIFICATION_INFORMATION;
 DROP TABLE IF EXISTS ENTRY_DV_MAPPINGS;
 DROP TABLE IF EXISTS ENTRY_DV_ENTITY;
+drop table if exists ENTRY_DV_PROPERTIES;
+drop table if exists GIT_ENTRY_DV_ENTITY;
+drop table if exists GIT_ENTRY_DV_MAPPINGS;
+drop table if exists GIT_ENTRY_DV_PROPERTIES;
+drop table if exists ENTRY_FILES;
+drop table if exists GIT_ENTRY_FILES;
+drop table if exists OM_DATASET_FILE;
 
 /********************** CREATION TABLES **********************/
 CREATE TABLE ENTRY_PATH (
 	COD_PATH             text NOT NULL    ,
 	DATABASE_NAME        text     ,
 	SCHEMA_NAME          text     ,
 	OWNER                text NOT NULL    ,
@@ -128,14 +136,34 @@
 	ENTITY_TYPE_DESCRIPTION text     ,
 	ENTITY_TYPE_FULL_NAME text     ,
 	ID_MODULE            integer     ,
 	CONSTRAINT Idx_OM_REF_ENTITY_TYPE UNIQUE ( ENTITY_TYPE_NAME ) ,
 	FOREIGN KEY ( ID_MODULE ) REFERENCES OM_REF_MODULES( ID_MODULE )
  );
 
+CREATE TABLE ENTRY_DV_ENTITY (
+	COD_ENTITY           text NOT NULL  PRIMARY KEY  ,
+	ENTITY_NAME          text     ,
+	ENTITY_TYPE          text     ,
+	COD_PATH             text     ,
+	NAME_STATUS_TRACKING_SATELLITE text     ,
+	NAME_RECORD_TRACKING_SATELLITE text     ,
+	NAME_EFFECTIVITY_SATELLITE text     ,
+	OWNER                text     ,
+	FOREIGN KEY ( ENTITY_TYPE ) REFERENCES OM_REF_ENTITY_TYPE( ENTITY_TYPE_NAME )
+ );
+
+CREATE TABLE ENTRY_DV_PROPERTIES (
+	COD_ENTITY           text     ,
+	NUM_CONNECTION       text     ,
+	HASH_NAME            text     ,
+	OWNER                text     ,
+	FOREIGN KEY ( COD_ENTITY ) REFERENCES ENTRY_DV_ENTITY( COD_ENTITY )
+ );
+
 CREATE TABLE ENTRY_ENTITY (
 	COD_ENTITY           text NOT NULL    ,
 	TABLE_NAME           text     ,
 	ENTITY_TYPE          text     ,
 	COD_PATH             text     ,
 	STRATEGY             text     ,
 	OWNER                text NOT NULL    ,
@@ -170,14 +198,55 @@
 	NUM_BRANCH           integer     ,
 	OWNER                text     ,
 	FOREIGN KEY ( COD_ENTITY_TARGET ) REFERENCES ENTRY_ENTITY( COD_ENTITY )  ,
 	FOREIGN KEY ( ORDER_TYPE ) REFERENCES OM_REF_ORDER_TYPE( ORDER_TYPE_VALUE )  ,
 	FOREIGN KEY ( COD_ENTITY_SOURCE ) REFERENCES ENTRY_ENTITY( COD_ENTITY )
  );
 
+CREATE TABLE GIT_ENTRY_DV_ENTITY (
+	COD_ENTITY           text NOT NULL  PRIMARY KEY  ,
+	ENTITY_NAME          text     ,
+	ENTITY_TYPE          text     ,
+	COD_PATH             text     ,
+	NAME_STATUS_TRACKING_SATELLITE text     ,
+	NAME_RECORD_TRACKING_SATELLITE text     ,
+	NAME_EFFECTIVITY_SATELLITE text     ,
+	OWNER                text     ,
+	FOREIGN KEY ( ENTITY_TYPE ) REFERENCES OM_REF_ENTITY_TYPE( ENTITY_TYPE_NAME )
+ );
+
+CREATE TABLE GIT_ENTRY_DV_MAPPINGS (
+	COD_ENTITY_SOURCE    text     ,
+	COLUMN_NAME_SOURCE   text     ,
+	COD_ENTITY_TARGET    text     ,
+	COLUMN_NAME_TARGET   text     ,
+	COLUMN_TYPE_TARGET   text     ,
+	ORDINAL_POSITION     text     ,
+	COLUMN_LENGTH        integer     ,
+	COLUMN_PRECISION     integer     ,
+	NUM_BRANCH           integer     ,
+	NUM_CONNECTION       integer     ,
+	KEY_TYPE             text     ,
+	SATELLITE_NAME       text     ,
+	ORIGIN_IS_INCREMENTAL integer     ,
+	ORIGIN_IS_TOTAL      integer     ,
+	ORIGIN_IS_CDC        integer     ,
+	OWNER                text     ,
+	FOREIGN KEY ( COD_ENTITY_SOURCE ) REFERENCES ENTRY_ENTITY( COD_ENTITY )  ,
+	FOREIGN KEY ( COD_ENTITY_TARGET ) REFERENCES ENTRY_DV_ENTITY( COD_ENTITY )
+ );
+
+CREATE TABLE GIT_ENTRY_DV_PROPERTIES (
+	COD_ENTITY           text     ,
+	NUM_CONNECTION       text     ,
+	HASH_NAME            text     ,
+	OWNER                text     ,
+	FOREIGN KEY ( COD_ENTITY ) REFERENCES ENTRY_DV_ENTITY( COD_ENTITY )
+ );
+
 CREATE TABLE GIT_ENTRY_ENTITY (
 	COD_ENTITY           text NOT NULL    ,
 	TABLE_NAME           text     ,
 	ENTITY_TYPE          text     ,
 	COD_PATH             text     ,
 	STRATEGY             text     ,
 	OWNER                text NOT NULL    ,
@@ -240,17 +309,17 @@
 	ID_DATASET_SPEC      integer NOT NULL  PRIMARY KEY  ,
 	ID_DATASET           integer     ,
 	ID_KEY_TYPE          integer     ,
 	COLUMN_NAME          text     ,
 	COLUMN_TYPE          text     ,
 	ORDINAL_POSITION     integer     ,
 	IS_NULLABLE          integer     ,
-	LENGTH               integer     ,
-	PRECISION            integer     ,
-	SCALE                integer     ,
+	COLUMN_LENGTH        integer     ,
+	COLUMN_PRECISION     integer     ,
+	COLUMN_SCALE         integer     ,
 	META_OWNER           text     ,
 	START_DATE           date     ,
 	END_DATE             date     ,
 	FOREIGN KEY ( ID_DATASET ) REFERENCES OM_DATASET( ID_DATASET )  ,
 	FOREIGN KEY ( ID_KEY_TYPE ) REFERENCES OM_REF_KEY_TYPE( ID_KEY_TYPE )
  );
 
@@ -336,16 +405,16 @@
 CREATE TABLE ENTRY_DATASET_MAPPINGS (
 	COD_ENTITY_SOURCE    text     ,
 	VALUE_SOURCE         text     ,
 	COD_ENTITY_TARGET    text     ,
 	COLUMN_NAME_TARGET   text     ,
 	COLUMN_TYPE_TARGET   text     ,
 	ORDINAL_POSITION     integer     ,
-	LENGTH               integer     ,
-	PRECISION            integer     ,
+	COLUMN_LENGTH        integer     ,
+	COLUMN_PRECISION     integer     ,
 	NUM_BRANCH           integer     ,
 	KEY_TYPE             text     ,
 	SW_DISTINCT          integer     ,
 	OWNER                text     ,
 	FOREIGN KEY ( COD_ENTITY_SOURCE ) REFERENCES ENTRY_ENTITY( COD_ENTITY )  ,
 	FOREIGN KEY ( COD_ENTITY_TARGET ) REFERENCES ENTRY_ENTITY( COD_ENTITY )  ,
 	FOREIGN KEY ( KEY_TYPE ) REFERENCES OM_REF_KEY_TYPE( KEY_TYPE_NAME )
@@ -359,43 +428,33 @@
 	RELATIONSHIP_TYPE    text     ,
 	OWNER                text     ,
 	FOREIGN KEY ( COD_ENTITY_MASTER ) REFERENCES ENTRY_ENTITY( COD_ENTITY )  ,
 	FOREIGN KEY ( COD_ENTITY_DETAIL ) REFERENCES ENTRY_ENTITY( COD_ENTITY )  ,
 	FOREIGN KEY ( RELATIONSHIP_TYPE ) REFERENCES OM_REF_JOIN_TYPE( JOIN_NAME )
  );
 
-CREATE TABLE ENTRY_DV_ENTITY (
-	COD_ENTITY           text     ,
-	SW_STATUS_TRACKING_SATELLITE integer     ,
-	NAME_STATUS_TRACKING_SATELLITE text     ,
-	SW_RECORD_TRACKING_SATELLITE integer     ,
-	NAME_RECORD_TRACKING_SATELLITE text     ,
-	SW_EFFECTIVITY_SATELLITE integer     ,
-	NAME_EFFECTIVITY_SATELLITE text     ,
-	RECORD_SOURCE        text     ,
-	ORIGIN_IS_INCREMENTAL integer     ,
-	ORIGIN_IS_TOTAL      integer     ,
-	ORIGIN_IS_CDC        integer     ,
-	OWNER                text     ,
-	FOREIGN KEY ( COD_ENTITY ) REFERENCES ENTRY_ENTITY( COD_ENTITY )
- );
-
 CREATE TABLE ENTRY_DV_MAPPINGS (
-	COD_ENTITY           text     ,
+	COD_ENTITY_SOURCE    text     ,
 	COLUMN_NAME_SOURCE   text     ,
+	COD_ENTITY_TARGET    text     ,
 	COLUMN_NAME_TARGET   text     ,
 	COLUMN_TYPE_TARGET   text     ,
 	ORDINAL_POSITION     text     ,
-	LENGTH               integer     ,
-	PRECISION            integer     ,
+	COLUMN_LENGTH        integer     ,
+	COLUMN_PRECISION     integer     ,
 	NUM_BRANCH           integer     ,
-	KEY_TYPE             integer     ,
+	NUM_CONNECTION       integer     ,
+	KEY_TYPE             text     ,
 	SATELLITE_NAME       text     ,
+	ORIGIN_IS_INCREMENTAL integer     ,
+	ORIGIN_IS_TOTAL      integer     ,
+	ORIGIN_IS_CDC        integer     ,
 	OWNER                text     ,
-	FOREIGN KEY ( COD_ENTITY ) REFERENCES ENTRY_ENTITY( COD_ENTITY )
+	FOREIGN KEY ( COD_ENTITY_SOURCE ) REFERENCES ENTRY_ENTITY( COD_ENTITY )  ,
+	FOREIGN KEY ( COD_ENTITY_TARGET ) REFERENCES ENTRY_DV_ENTITY( COD_ENTITY )
  );
 
 CREATE TABLE GIT_ENTRY_AGGREGATORS (
 	COD_ENTITY_TARGET    text     ,
 	COD_ENTITY_SOURCE    text     ,
 	COLUMN_NAME          text     ,
 	NUM_BRANCH           integer     ,
@@ -407,16 +466,16 @@
 CREATE TABLE GIT_ENTRY_DATASET_MAPPINGS (
 	COD_ENTITY_SOURCE    text     ,
 	VALUE_SOURCE         text     ,
 	COD_ENTITY_TARGET    text     ,
 	COLUMN_NAME_TARGET   text     ,
 	COLUMN_TYPE_TARGET   text     ,
 	ORDINAL_POSITION     integer     ,
-	LENGTH               integer     ,
-	PRECISION            integer     ,
+	COLUMN_LENGTH        integer     ,
+	COLUMN_PRECISION     integer     ,
 	NUM_BRANCH           integer     ,
 	KEY_TYPE             text     ,
 	SW_DISTINCT          integer     ,
 	OWNER                text     ,
 	FOREIGN KEY ( KEY_TYPE ) REFERENCES OM_REF_KEY_TYPE( KEY_TYPE_NAME )  ,
 	FOREIGN KEY ( COD_ENTITY_SOURCE ) REFERENCES GIT_ENTRY_ENTITY( COD_ENTITY )  ,
 	FOREIGN KEY ( COD_ENTITY_TARGET ) REFERENCES GIT_ENTRY_ENTITY( COD_ENTITY )
@@ -443,24 +502,62 @@
 	START_DATE           date     ,
 	END_DATE             date     ,
 	FOREIGN KEY ( ID_DATASET_SPEC_MASTER ) REFERENCES OM_DATASET_SPECIFICATION( ID_DATASET_SPEC )  ,
 	FOREIGN KEY ( ID_DATASET_SPEC_DETAIL ) REFERENCES OM_DATASET_SPECIFICATION( ID_DATASET_SPEC )  ,
 	FOREIGN KEY ( ID_JOIN_TYPE ) REFERENCES OM_REF_JOIN_TYPE( ID_JOIN_TYPE )
  );
 
+ CREATE TABLE OM_DATASET_DV (
+	ID_DATASET           integer     ,
+	ID_ENTITY_TYPE       integer     ,
+	META_OWNER           text     ,
+	START_DATE           date     ,
+	END_DATE             date
+ );
+
+CREATE TABLE ENTRY_FILES (
+	COD_ENTITY           text     ,
+	FILE_PATH            text     ,
+	FILE_NAME            text     ,
+	DELIMITER_CHARACTER  text     ,
+	OWNER                text
+ );
+
+CREATE TABLE GIT_ENTRY_FILES (
+	COD_ENTITY           text     ,
+	FILE_PATH            text     ,
+	FILE_NAME            text     ,
+	DELIMITER_CHARACTER  text     ,
+	OWNER                text
+ );
+
+ CREATE TABLE OM_DATASET_FILE (
+	ID_DATASET           integer     ,
+	FILE_PATH            text     ,
+	FILE_NAME            text     ,
+	DELIMITER_CHARACTER  text     ,
+	META_OWNER           text     ,
+	START_DATE           date     ,
+	END_DATE             date
+ );
+
+
+
+
+
 CREATE VIEW OM_DATASET_INFORMATION AS select A.META_OWNER, B.ENTITY_TYPE_FULL_NAME, B.ENTITY_TYPE_DESCRIPTION, C.MODULE_NAME, C.MODULE_FULL_NAME, C.MODULE_DESCRIPTION, A.DATASET_NAME,  D.DATABASE_NAME, D.SCHEMA_NAME, F.QUERY_TYPE_NAME , F.QUERY_TYPE_DESCRIPTION , A.START_DATE
 From OM_DATASET A
 LEFT JOIN OM_REF_ENTITY_TYPE B on A.ID_ENTITY_TYPE = B.ID_ENTITY_TYPE
 LEFT JOIN OM_REF_MODULES C on B.ID_MODULE = C.ID_MODULE
 LEFT JOIN OM_DATASET_PATH D on A.ID_PATH = D.ID_PATH
 LEFT JOIN OM_DATASET_EXECUTION E on A.ID_DATASET = E.ID_DATASET
 LEFT JOIN OM_REF_QUERY_TYPE F on E.ID_QUERY_TYPE = F.ID_QUERY_TYPE
 WHERE A.END_DATE is null and D.END_DATE is null and E.END_DATE is null;
 
-CREATE VIEW OM_DATASET_SPECIFICATION_INFORMATION AS select A.META_OWNER , A.DATASET_NAME , B.COLUMN_NAME , B.COLUMN_TYPE , B.ORDINAL_POSITION , B.IS_NULLABLE , B."LENGTH" , B."PRECISION" , B."SCALE"
+CREATE VIEW OM_DATASET_SPECIFICATION_INFORMATION AS select A.META_OWNER , A.DATASET_NAME , B.COLUMN_NAME , B.COLUMN_TYPE , B.ORDINAL_POSITION , B.IS_NULLABLE , B.COLUMN_LENGTH , B.COLUMN_PRECISION , B.COLUMN_SCALE
 FROM OM_DATASET A
 LEFT JOIN OM_DATASET_SPECIFICATION B on A.ID_DATASET = B.ID_DATASET
 WHERE A.END_DATE is null and B.END_DATE is null;
 
 CREATE VIEW OM_RELATIONSHIPS AS select A.META_OWNER , D.DATABASE_NAME as MASTER_DATABASE_NAME, D.SCHEMA_NAME as MASTER_SCHEMA_NAME, C.DATASET_NAME as MASTER_DATASET_NAME, B.COLUMN_NAME as MASTER_COLUMN_NAME,
  G.DATABASE_NAME as DETAIL_DATABASE_NAME , G.SCHEMA_NAME as DETAIL_SCHEMA_NAME, F.DATASET_NAME  as DETAIL_DATASET_NAME, E.COLUMN_NAME as DETAIL_COLUMN_NAME, A.START_DATE
 from OM_DATASET_RELATIONSHIPS A
@@ -480,26 +577,30 @@
 INSERT INTO OM_REF_ENTITY_TYPE (ID_ENTITY_TYPE, ENTITY_TYPE_NAME, ENTITY_TYPE_DESCRIPTION, ENTITY_TYPE_FULL_NAME, ID_MODULE) VALUES
 (0, 'SRC', 'Source of the run. It need to be loaded from other sources', 'Source', 0),
 (1, 'VIEW', 'Temporary table. It will be not materialized', 'Temporary', 0),
 (2, 'TB', 'Table. It''s the result of a process', 'Table', 0),
 (3, 'WITH', 'With Clause', 'With', 0),
 (4, 'HUB', 'Datavault - Hub', 'Hub', 1),
 (5, 'LINK', 'Datavault - Link', 'Link', 1),
-(6, 'SAT', ' Datavault - Satellite', 'Satellite', '1');
+(6, 'SAT', 'Datavault - Satellite', 'Satellite', '1'),
+(7, 'STS', 'Datavault - Status Tracking Satellite', 'Status Tracking Satellite', 1),
+(8, 'RTS', 'Datavault - Satellite', 'Record Tracking Satellite', 1),
+(9, 'SATE', 'Datavault - Effectivity Satellite', 'Effectivity Satellite', 1);
 
 INSERT INTO OM_REF_JOIN_TYPE(ID_JOIN_TYPE, JOIN_NAME, JOIN_VALUE, JOIN_DESCRIPTION) VALUES
 (0, 'INNER JOIN', 'INNER JOIN', 'Returns only those rows that have matching values'),
 (1, 'MASTER JOIN', 'LEFT JOIN', 'Returns those rows from the left table plus those that have matching values'),
 (2, 'DETAIL JOIN', 'RIGHT JOIN', 'Returns those rows from the right table plus those that have matching values'),
 (3, 'OUTER JOIN', 'OUTER JOIN', 'Returns rows from both tables');
 
 INSERT INTO OM_REF_KEY_TYPE(ID_KEY_TYPE, KEY_TYPE_NAME, KEY_TYPE_DESCRIPTION) VALUES
 (0, 'PK', 'Primary Key'), (1, 'BK', 'Business Key'), (2,'NULL', 'Nothing'), (3,'SEQ', 'Sequence'),
 (4, 'FK', 'Foreign Key'), (5, 'HK', 'Hash Key'), (6, 'AT', 'Attribute'), (7 ,'ST','Status'),
-(8, 'DK', 'Driven Key');
+(8, 'DK', 'Driven Key'), (9, 'RS', 'Record Source'), (10, 'TN', 'Tenant'), (11,'HD', 'Hashdiff'),
+(12, 'DCK', 'Dependent-child key'), (13, 'AD', 'Applied Date');
 
 INSERT INTO OM_REF_ORDER_TYPE(ID_ORDER_TYPE, ORDER_TYPE_NAME, ORDER_TYPE_VALUE, ORDER_TYPE_DESCRIPTION) VALUES
 (0, 'Ascendant', 'ASC', 'Ascending order'),
 (1, 'Descendant', 'DESC', 'Descending order');
 
 INSERT INTO OM_REF_QUERY_TYPE(ID_QUERY_TYPE, QUERY_TYPE_NAME, QUERY_TYPE_DESCRIPTION) VALUES
 (0, 'INSERT', 'Insert on the target table'),
@@ -507,9 +608,10 @@
 (2, 'VIEW', 'Creates a View'),
 (3, 'DELETE', 'Deletes based on the Primary Key'),
 (4, 'SELECT', 'Select the target query'),
 (5, 'MERGE', 'Select the target query'),
 (6, 'TRUNCATE AND INSERT', 'Truncate the target table and inserts');
 
 INSERT INTO OM_PROPERTIES(PROPERTY, VALUE, START_DATE) VALUES
-('Version', '0.3.9b', date('now')),
-('Module Deployed', 'ELT', date('now'));
+('Version', '0.4', date('now')),
+('Module Deployed', 'ELT', date('now')),
+('Module Deployed', 'DV', date('now'));
```

### Comparing `Metamorf-0.3.9.1/metamorf/main.py` & `Metamorf-0.4.3.1/metamorf/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 from metamorf.engines.engine_delete import EngineDelete
 from metamorf.engines.engine_output import EngineOutput
 from metamorf.engines.engine_run import EngineRun
 from metamorf.engines.engine_backup import EngineBackup
 from metamorf.engines.engine_manifest import EngineManifest
 from metamorf.engines.engine_api import EngineApi
 from metamorf.engines.engine_restore import EngineRestore
+from metamorf.engines.engine_files import EngineFiles
+from metamorf.engines.engine_metadata import EngineMetadata
 from metamorf.tools.argparser import ArgParser
 from metamorf.engines.engine_commit import EngineCommit
 from metamorf.help import print_help
 
 def main():
     os.system('')
     argp = ArgParser(sys.argv[1:])
@@ -81,14 +83,20 @@
         engine.run()
     elif arguments['command'] == 'manifest':
         engine = EngineManifest(log, arguments)
         engine.run()
     elif arguments['command'] == 'restore':
         engine = EngineRestore(log, arguments)
         engine.run()
+    elif arguments['command'] == 'files':
+        engine = EngineFiles(log, arguments)
+        engine.run()
+    elif arguments['command'] == 'metadata':
+        engine = EngineMetadata(log, arguments)
+        engine.run()
     else:
         log.log('METAMORF', 'Command under development. More information at https://www.metamorf.io', LOG_LEVEL_CRITICAL)
 
     log.close()
 
 if __name__ == "__main__":
    main()
```

### Comparing `Metamorf-0.3.9.1/metamorf/tools/argparser.py` & `Metamorf-0.4.3.1/metamorf/tools/argparser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from metamorf.tools.filecontroller import FileControllerFactory
 from metamorf.constants import *
+import os
 
 class ArgParser:
 
     def __init__(self, arguments: list):
         self.arguments = arguments
         file_controller_properties = FileControllerFactory().get_file_reader(FILE_TYPE_YML)
-        file_controller_properties.set_file_location(PACKAGE_PATH + '\\' + PROPERTIES_FILE_PATH, PROPERTIES_FILE_NAME)
+        file_controller_properties.set_file_location(os.path.join(PACKAGE_PATH, PROPERTIES_FILE_PATH), PROPERTIES_FILE_NAME)
         self.properties_file = file_controller_properties.read_file()
         self.all_commands = self.get_all_commands()
 
     def get_arguments_parsed(self):
         """Returns a dictionary with all the arguments parsed"""
         result = {}
         if len(self.arguments)==0:
```

### Comparing `Metamorf-0.3.9.1/metamorf/tools/configvalidator.py` & `Metamorf-0.4.3.1/metamorf/tools/configvalidator.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,29 +107,39 @@
         if self.configuration_file is None:
             return
 
         #Properties
         if 'name' not in self.configuration_file:
             self.log.log(self.configvalidator_name, "ConfigurationFile - Missing Value: name", LOG_LEVEL_ERROR)
             return False
+        if self.configuration_file['name'] is None:
+            self.log.log(self.configvalidator_name, "ConfigurationFile - Missing Value: name", LOG_LEVEL_ERROR)
+            return False
+
         if 'owner' not in self.configuration_file:
             self.log.log(self.configvalidator_name, "ConfigurationFile - Missing Value: owner", LOG_LEVEL_CRITICAL)
             return False
+        if self.configuration_file['owner'] is None:
+            self.log.log(self.configvalidator_name, "ConfigurationFile - Missing Value: owner", LOG_LEVEL_CRITICAL)
+            return False
 
         if 'output' not in self.configuration_file:
             self.log.log(self.configvalidator_name, "ConfigurationFile - Missing Value: output", LOG_LEVEL_CRITICAL)
             return False
 
         # Validation OUTPUT get_type_options_for_output
         if 'type' not in self.configuration_file['output']:
             self.log.log(self.configvalidator_name, "ConfigurationFile - Output: The attribute [type] needs to be indicated", LOG_LEVEL_CRITICAL)
             return False
 
         if self.configuration_file['output']['type'] not in self.get_type_options_for_output():
-            self.log.log(self.configvalidator_name, 'ConfigurationFile - Output: The attribute [type] has an impossible value', LOG_LEVEL_CRITICAL)
+            self.log.log(self.configvalidator_name, 'ConfigurationFile - Output: The attribute [output][type] has an impossible value', LOG_LEVEL_CRITICAL)
+            return False
+        if self.configuration_file['output']['type'] is None:
+            self.log.log(self.configvalidator_name, "ConfigurationFile - Output: The attribute [output][type] needs to be indicated", LOG_LEVEL_CRITICAL)
             return False
 
         # Validation MODULES
         if 'modules' not in self.configuration_file:
             self.log.log(self.configvalidator_name, 'Configuration File - Modules: [modules] section is mandatory on the Configuration File.', LOG_LEVEL_ERROR)
             return False
 
@@ -160,38 +170,48 @@
             self.log.log(self.configvalidator_name, 'ConfigurationFile - Metadata: [metadata] section is mandatory on the Configuration File.', LOG_LEVEL_ERROR)
             return False
 
         metadata_information = self.configuration_file['metadata']
         if 'connection_type' not in metadata_information:
             self.log.log(self.configvalidator_name, 'ConfigurationFile - Metadata: The attribute [connection_type] needs to be indicated', LOG_LEVEL_ERROR)
             return False
+        if metadata_information['connection_type'] is None:
+            self.log.log(self.configvalidator_name, "[ERROR] ConfigurationFile - Metadata: The attribute [connection_type] needs to be indicated", LOG_LEVEL_CRITICAL)
+            return False
         mandatory_fields = self.get_mandatory_fields_from_database(metadata_information['connection_type'])
             #First validation: All the fields are OK
         for key,value in metadata_information.items():
             if key=='connection_type': continue
             if key not in mandatory_fields:
                 self.log.log(self.configvalidator_name, 'ConfigurationFile - Metadata: Field ' + key + ' is not an option for this database.', LOG_LEVEL_ERROR)
                 return False
             #Second validation: There are all the fields indicated
         for key,value in metadata_information.items():
             if key=='connection_type': continue
+            if value == None:
+                self.log.log(self.configvalidator_name, 'ConfigurationFile - Metadata: Field ' + key + ' has not a value', LOG_LEVEL_ERROR)
+                return False
             mandatory_fields.remove(key)
         if len(mandatory_fields)>0:
             self.log.log(self.configvalidator_name, 'ConfigurationFile - Metadata: The following attributes needs to be indicated to permit the connection: ' + str(mandatory_fields), LOG_LEVEL_ERROR)
             return False
 
         # Validation Data
         if 'data' not in self.configuration_file:
             self.log.log(self.configvalidator_name, 'ConfigurationFile - Data: [data] section is mandatory on the Configuration File.', LOG_LEVEL_ERROR)
             return False
 
         data_information = self.configuration_file['data']
         if 'connection_type' not in data_information:
-            self.log.log(self.configvalidator_name, '[ERROR] ConfigurationFile - Metadata: The attribute [connection_type] needs to be indicated', LOG_LEVEL_ERROR)
+            self.log.log(self.configvalidator_name, '[ERROR] ConfigurationFile - Data: The attribute [connection_type] needs to be indicated', LOG_LEVEL_ERROR)
             return False
+        if data_information['connection_type'] is None:
+            self.log.log(self.configvalidator_name, "[ERROR] ConfigurationFile - Data: The attribute [connection_type] needs to be indicated", LOG_LEVEL_CRITICAL)
+            return False
+
         mandatory_fields = self.get_mandatory_fields_from_database(data_information['connection_type'])
         # First validation: All the fields are OK
         for key, value in data_information.items():
             if key == 'connection_type': continue
             if key not in mandatory_fields:
                 self.log.log(self.configvalidator_name, 'ConfigurationFile - Metadata: Field ' + key + ' is not an option for this database.', LOG_LEVEL_ERROR)
                 return False
```

### Comparing `Metamorf-0.3.9.1/metamorf/tools/database_objects.py` & `Metamorf-0.4.3.1/metamorf/tools/database_objects.py`

 * *Files 20% similar despite different names*

```diff
@@ -111,86 +111,118 @@
     def __str__(self):
         database_name = 'NULL'
         if self.database_name is not None and self.database_name != '': database_name = "'"+self.database_name + "'"
         schema_name = 'NULL'
         if self.schema_name is not None and self.schema_name != '': schema_name = "'" + self.schema_name + "'"
         return "'"+self.cod_path+"'," + database_name+","+schema_name+",'"+self.owner + "'"
 
+class EntryFiles:
+
+    def __init__(self, cod_entity: str, file_path: str, file_name: str, delimiter_character: str, owner: str):
+        self.cod_entity = cod_entity
+        self.file_path = file_path
+        self.file_name = file_name
+        self.delimiter_character = delimiter_character
+        self.owner = owner
+
+    def get(self):
+        return [self.cod_entity, self.file_path, self.file_name, self.delimiter_character, self.owner]
+
+    def __str__(self):
+        delimiter_character = 'NULL'
+        if self.delimiter_character is not None and self.delimiter_character != '': delimiter_character = "'"+self.delimiter_character + "'"
+        return "'"+self.cod_entity+"','" + self.file_path + "','" + self.file_name+"',"+delimiter_character+",'"+self.owner + "'"
+
 
 class EntryDatasetMappings:
 
-    def __init__(self, cod_entity_source: str, value_source: str, cod_entity_target: str, column_name_target: str, column_type_target: str, ordinal_position: int, length : int, precision: int, num_branch: int, key_type: str, sw_distinct: int, owner: str):
+    def __init__(self, cod_entity_source: str, value_source: str, cod_entity_target: str, column_name_target: str, column_type_target: str, ordinal_position: int, column_length : int, column_precision: int, num_branch: int, key_type: str, sw_distinct: int, owner: str):
         self.cod_entity_source = cod_entity_source
         self.value_source = value_source
         self.cod_entity_target = cod_entity_target
         self.column_name_target = column_name_target
         self.column_type_target = column_type_target
         self.ordinal_position = ordinal_position
-        self.length = length
-        self.precision = precision
+        self.column_length = column_length
+        self.column_precision = column_precision
         self.num_branch = num_branch
         self.key_type = key_type
         self.sw_distinct = sw_distinct
         self.owner = owner
 
     def get(self):
         return [self.cod_entity_source, self.value_source, self.cod_entity_target, self.column_name_target,
-                self.column_type_target, self.ordinal_position, self.length, self.precision, self.num_branch,
+                self.column_type_target, self.ordinal_position, self.column_length, self.column_precision, self.num_branch,
                 self.key_type, self.sw_distinct, self.owner]
 
     def __str__(self):
         key_type = 'NULL'
         if self.key_type is not None and self.key_type != '': key_type = "'"+self.key_type+"'"
-        return "'"+self.cod_entity_source+"','"+self.value_source.replace("'","''")+"','"+self.cod_entity_target+"','" + self.column_name_target+"','"+self.column_type_target+"',"+str(self.ordinal_position) + "," + str(self.length)+","+str(self.precision)+","+str(self.num_branch)+","+key_type+","+str(self.sw_distinct)+",'"+self.owner+"'"
+        return "'"+self.cod_entity_source+"','"+self.value_source.replace("'","''")+"','"+self.cod_entity_target+"','" + self.column_name_target+"','"+self.column_type_target+"',"+str(self.ordinal_position) + "," + str(self.column_length)+","+str(self.column_precision)+","+str(self.num_branch)+","+key_type+","+str(self.sw_distinct)+",'"+self.owner+"'"
 
 class EntryDvMappings:
 
-    def __init__(self, cod_entity, column_name_source, column_name_target, column_type_target, ordinal_position, length, precision, num_branch, key_type, satellite_name, owner):
-        self.cod_entity = cod_entity
+    def __init__(self, cod_entity_source, column_name_source, cod_entity_target,column_name_target, column_type_target, ordinal_position, column_length, column_precision, num_branch,num_connection, key_type, satellite_name, origin_is_incremental, origin_is_total, origin_is_cdc, owner):
+        self.cod_entity_source = cod_entity_source
         self.column_name_source = column_name_source
+        self.cod_entity_target = cod_entity_target
         self.column_name_target = column_name_target
         self.column_type_target = column_type_target
         self.ordinal_position = ordinal_position
-        self.length = length
-        self.precision = precision
+        self.column_length = column_length
+        self.column_precision = column_precision
         self.num_branch = num_branch
+        self.num_connection = num_connection
         self.key_type = key_type
         self.satellite_name = satellite_name
+        self.origin_is_incremental = origin_is_incremental
+        self.origin_is_total = origin_is_total
+        self.origin_is_cdc = origin_is_cdc
         self.owner = owner
 
     def get(self):
-        return [self.cod_entity, self.column_name_source, self.column_name_target,self.column_type_target,self.ordinal_position,self.length, self.precision,self.num_branch,self.key_type,self.satellite_name, self.owner]
+        return [self.cod_entity_source, self.column_name_source, self.cod_entity_target, self.column_name_target,self.column_type_target,self.ordinal_position,self.column_length, self.column_precision,self.num_branch, self.num_connection, self.key_type,self.satellite_name,self.origin_is_incremental, self.origin_is_total, self.origin_is_cdc, self.owner]
 
     def __str__(self):
-        return "'" + self.cod_entity +"','"+self.column_name_source+"','"+ self.column_name_target+"','"+self.column_type_target+"',"+self.ordinal_position+","+self.length+\
-                ","+self.precision + ","+ self.num_branch+",'"+self.key_type+"','"+self.satellite_name+"','"+self.owner+"'"
+        return "'" + self.cod_entity_source +"','"+self.column_name_source.replace("'","''")+"','"+self.cod_entity_target+"','"+self.column_name_target+"','"+self.column_type_target+"',"+str(self.ordinal_position)+","+str(self.column_length)+\
+                ","+str(self.column_precision) + ","+ str(self.num_branch)+","+str(self.num_connection)+",'"+self.key_type+"','"+self.satellite_name+"',"+str(self.origin_is_incremental)+","+str(self.origin_is_total)+","+str(self.origin_is_cdc)+",'"+self.owner+"'"
 
 class EntryDvEntry:
 
-    def __init__(self, cod_entity, sw_status_tracking_satellite, name_status_tracking_satellite, sw_record_tracking_satellite, name_record_tracking_satellite,
-                 sw_effectivity_satellite, name_effectivity_satellite, record_source, origin_is_incremental, origin_is_total, origin_is_cdc, owner):
+    def __init__(self, cod_entity, entity_name, entity_type, cod_path, name_status_tracking_satellite, name_record_tracking_satellite,
+                name_effectivity_satellite, owner):
         self.cod_entity = cod_entity
-        self.sw_status_tracking_satellite = sw_status_tracking_satellite
+        self.entity_name = entity_name
+        self.entity_type = entity_type
+        self.cod_path = cod_path
         self.name_status_tracking_satellite = name_status_tracking_satellite
-        self.sw_record_tracking_satellite = sw_record_tracking_satellite
         self.name_record_tracking_satellite = name_record_tracking_satellite
-        self.sw_effectivity_satellite = sw_effectivity_satellite
         self.name_effectivity_satellite = name_effectivity_satellite
-        self.record_source = record_source
-        self.origin_is_incremental = origin_is_incremental
-        self.origin_is_total = origin_is_total
-        self.origin_is_cdc = origin_is_cdc
         self.owner = owner
 
     def get(self):
-        return[self.cod_entity,self.sw_status_tracking_satellite,self.name_status_tracking_satellite,self.sw_record_tracking_satellite,self.name_record_tracking_satellite,self.sw_effectivity_satellite,self.name_effectivity_satellite,self.record_source,self.origin_is_incremental,self.origin_is_total,self.origin_is_cdc, self.owner]
+        return[self.cod_entity, self.entity_name, self.entity_type, self.cod_path, self.name_status_tracking_satellite,self.name_record_tracking_satellite,self.name_effectivity_satellite, self.owner]
 
     def __str__(self):
-        return "'"+self.cod_entity+"',"+self.sw_status_tracking_satellite+",'"+self.name_status_tracking_satellite+"',"+self.sw_record_tracking_satellite+",'"+self.name_record_tracking_satellite+"',"+ \
-               self.sw_effectivity_satellite+",'"+self.name_effectivity_satellite+"','"+self.record_source+"',"+self.origin_is_incremental+","+self.origin_is_total+","+self.origin_is_cdc+",'"+self.owner+"'"
+        return "'"+self.cod_entity+"','"+self.entity_name+"','"+self.entity_type+"','"+self.cod_path+"','"+self.name_status_tracking_satellite+"','"+self.name_record_tracking_satellite+"',"+ \
+               "'"+self.name_effectivity_satellite+"','"+self.owner+"'"
+
+class EntryDvProperties:
+
+    def __init__(self, cod_entity, num_connection, hash_name, owner):
+        self.cod_entity = cod_entity
+        self.num_connection = num_connection
+        self.hash_name = hash_name
+        self.owner = owner
+
+    def get(self):
+        return [self.cod_entity, self.num_connection, self.hash_name, self.owner]
+
+    def __str__(self):
+        return "'" + self.cod_entity + "'," + self.num_connection + ",'" + self.hash_name + "','" + self.owner + "'"
 
 # METADATA - Metamorf Tables
 class OmDataset:
 
     def __init__(self, id_dataset, dataset_name, id_entity_type, id_path, meta_owner, start_date, end_date):
         if isinstance(start_date, datetime.datetime): start_date = start_date.strftime("%Y-%m-%d %H:%M:%S")
         if isinstance(end_date, datetime.datetime): end_date = end_date.strftime("%Y-%m-%d %H:%M:%S")
@@ -206,41 +238,59 @@
         return [self.id_dataset, self.dataset_name, self.id_entity_type, self.id_path, self.meta_owner, self.start_date, self.end_date]
 
     def __str__(self):
         if self.end_date is None or self.end_date == '' or self.end_date=='NULL': end_date = "NULL"
         else: end_date = self.end_date
         return str(self.id_dataset) + ",'" + self.dataset_name + "'," + str(self.id_entity_type) + "," + str(self.id_path) + ",'" + self.meta_owner + "'," + self.start_date + "," + end_date
 
+class OmDatasetDv:
+
+    def __init__(self, id_dataset, id_entity_type, meta_owner, start_date, end_date):
+        if isinstance(start_date, datetime.datetime): start_date = start_date.strftime("%Y-%m-%d %H:%M:%S")
+        if isinstance(end_date, datetime.datetime): end_date = end_date.strftime("%Y-%m-%d %H:%M:%S")
+        self.id_dataset =  id_dataset
+        self.id_entity_type = id_entity_type
+        self.meta_owner = meta_owner
+        self.start_date = start_date
+        self.end_date = end_date
+
+    def get(self):
+        return [self.id_dataset, self.id_entity_type, self.meta_owner, self.start_date, self.end_date]
+
+    def __str__(self):
+        if self.end_date is None or self.end_date == '' or self.end_date=='NULL': end_date = "NULL"
+        else: end_date = self.end_date
+        return str(self.id_dataset) + ","+ str(self.id_entity_type) +",'"+self.meta_owner +"'," + self.start_date + "," + end_date
 
 class OmDatasetSpecification:
 
-    def __init__(self, id_dataset_spec, id_dataset, id_key_type, column_name, column_type, ordinal_position, is_nullable, length, precision, scale, meta_owner, start_date, end_date):
+    def __init__(self, id_dataset_spec, id_dataset, id_key_type, column_name, column_type, ordinal_position, is_nullable, column_length, column_precision, column_scale, meta_owner, start_date, end_date):
         if isinstance(start_date, datetime.datetime): start_date = start_date.strftime("%Y-%m-%d %H:%M:%S")
         if isinstance(end_date, datetime.datetime): end_date = end_date.strftime("%Y-%m-%d %H:%M:%S")
         self.id_dataset_spec = id_dataset_spec
         self.id_dataset = id_dataset
         self.id_key_type = id_key_type
         self.column_name = column_name
         self.column_type = column_type
         self.ordinal_position = ordinal_position
         self.is_nullable = is_nullable
-        self.length = length
-        self.precision = precision
-        self.scale = scale
+        self.column_length = column_length
+        self.column_precision = column_precision
+        self.column_scale = column_scale
         self.meta_owner = meta_owner
         self.start_date = start_date
         self.end_date = end_date
 
     def get(self):
-        return [self.id_dataset_spec, self.id_dataset, self.id_key_type, self.column_name, self.column_type, self.ordinal_position, self.is_nullable, self.length, self.precision, self.scale, self.meta_owner, self.start_date, self.end_date]
+        return [self.id_dataset_spec, self.id_dataset, self.id_key_type, self.column_name, self.column_type, self.ordinal_position, self.is_nullable, self.column_length, self.column_precision, self.column_scale, self.meta_owner, self.start_date, self.end_date]
 
     def __str__(self):
         if self.end_date is None or self.end_date == '' or self.end_date=='NULL': end_date = "NULL"
         else: end_date = self.end_date
-        return str(self.id_dataset_spec) + ","+ str(self.id_dataset)+","+str(self.id_key_type)+",'"+str(self.column_name)+"','"+str(self.column_type)+"',"+str(self.ordinal_position)+","+str(self.is_nullable)+","+str(self.length)+","+str(self.precision)+","+str(self.scale)+",'"+str(self.meta_owner) + "'," + self.start_date + "," + end_date
+        return str(self.id_dataset_spec) + ","+ str(self.id_dataset)+","+str(self.id_key_type)+",'"+str(self.column_name)+"','"+str(self.column_type)+"',"+str(self.ordinal_position)+","+str(self.is_nullable)+","+str(self.column_length)+","+str(self.column_precision)+","+str(self.column_scale)+",'"+str(self.meta_owner) + "'," + self.start_date + "," + end_date
 
 
 class OmDatasetTAgg:
 
     def __init__(self, id_t_agg, id_dataset, id_branch, id_dataset_spec, meta_owner, start_date, end_date):
         if isinstance(start_date, datetime.datetime): start_date = start_date.strftime("%Y-%m-%d %H:%M:%S")
         if isinstance(end_date, datetime.datetime): end_date = end_date.strftime("%Y-%m-%d %H:%M:%S")
@@ -405,14 +455,35 @@
         else: database = "NULL"
         if self.schema_name != None and self.schema_name != '': schema = "'"+self.schema_name+"'"
         else: schema = "NULL"
         if self.end_date is None or self.end_date == '' or self.end_date=='NULL': end_date = "NULL"
         else: end_date = self.end_date
         return str(self.id_path)+","+database+","+schema+",'"+self.meta_owner+"',"+self.start_date+","+end_date
 
+class OmDatasetFile:
+
+    def __init__(self, id_dataset, file_path, file_name, delimiter_character, meta_owner, start_date, end_date):
+        if isinstance(start_date, datetime.datetime): start_date = start_date.strftime("%Y-%m-%d %H:%M:%S")
+        if isinstance(end_date, datetime.datetime): end_date = end_date.strftime("%Y-%m-%d %H:%M:%S")
+        self.id_dataset = id_dataset
+        self.file_path = file_path
+        self.file_name = file_name
+        self.delimiter_character = delimiter_character
+        self.meta_owner = meta_owner
+        self.start_date = start_date
+        self.end_date = end_date
+
+    def get(self):
+        return [self.id_dataset, self.file_path ,self.file_name ,self.delimiter_character ,self.meta_owner ,self.start_date ,self.end_date]
+
+    def __str__(self):
+        if self.end_date is None or self.end_date == '' or self.end_date=='NULL': end_date = "NULL"
+        else: end_date = self.end_date
+        return str(self.id_dataset)+",'"+str(self.file_path)+"','"+self.file_name+"','"+str(self.delimiter_character)+"','"+self.meta_owner+"',"+self.start_date +","+end_date
+
 
 class OmDatasetTFilter:
 
     def __init__(self, id_t_filter, id_dataset, id_branch, value_filter, meta_owner, start_date, end_date):
         if isinstance(start_date, datetime.datetime): start_date = start_date.strftime("%Y-%m-%d %H:%M:%S")
         if isinstance(end_date, datetime.datetime): end_date = end_date.strftime("%Y-%m-%d %H:%M:%S")
         self.id_t_filter = id_t_filter
@@ -425,15 +496,15 @@
 
     def get(self):
         return [self.id_t_filter, self.id_dataset, self.id_branch, self.value_filter, self.meta_owner, self.start_date, self.end_date]
 
     def __str__(self):
         if self.end_date is None or self.end_date == '' or self.end_date=='NULL': end_date = "NULL"
         else: end_date = self.end_date
-        return str(self.id_t_filter)+","+str(self.id_dataset)+","+str(self.id_branch)+",'"+self.value_filter+"','"+self.meta_owner+"',"+self.start_date+","+end_date
+        return str(self.id_t_filter)+","+str(self.id_dataset)+","+str(self.id_branch)+",'"+self.value_filter.replace("'","''")+"','"+self.meta_owner+"',"+self.start_date+","+end_date
 
 
 class OmDatasetTHaving:
 
     def __init__(self, id_t_having, id_dataset, id_branch, value_having, meta_owner, start_date, end_date):
         if isinstance(start_date, datetime.datetime): start_date = start_date.strftime("%Y-%m-%d %H:%M:%S")
         if isinstance(end_date, datetime.datetime): end_date = end_date.strftime("%Y-%m-%d %H:%M:%S")
@@ -558,41 +629,41 @@
         self.detail_schema_name = detail_schema_name
         self.detail_dataset_name = detail_dataset_name
         self.detail_column_name = detail_column_name
         self.start_date = start_date
 
 class OmDatasetSpecificationInformation:
 
-    def __init__(self, meta_owner, dataset_name, column_name, column_type, ordinal_position, is_nullable, length, precision, scale):
+    def __init__(self, meta_owner, dataset_name, column_name, column_type, ordinal_position, is_nullable, column_length, column_precision, column_scale):
         self.meta_owner = meta_owner
         self.dataset_name = dataset_name
         self.column_name = column_name
         self.column_type = column_type
         self.ordinal_position = ordinal_position
         self.is_nullable = is_nullable
-        self.length = length
-        self.precision = precision
-        self.scale = scale
+        self.column_length = column_length
+        self.column_precision = column_precision
+        self.column_scale = column_scale
 
 
 class Column:
 
-    def __init__(self, id, column_name, column_type, default_value, is_pk, is_nullable, length, precision, scale):
+    def __init__(self, id, column_name, column_type, default_value, key_type, is_nullable, column_length, column_precision, column_scale):
         self.id = id
         self.column_name = column_name
         self.column_type = column_type
         self.default_value = default_value
-        self.is_pk = is_pk
+        self.key_type = key_type
         self.is_nullable = is_nullable
-        self.length = length
-        self.precision = precision
-        self.scale = scale
+        self.column_length = column_length
+        self.column_precision = column_precision
+        self.column_scale = column_scale
 
     def __str__(self):
-        return str(self.id) + ","+str(self.column_name)+","+str(self.column_type)+","+str(self.default_value)+","+str(self.is_pk)+","+ self.is_nullable+","+self.length+","+self.precision+","+self.scale
+        return str(self.id) + "," + str(self.column_name) +"," + str(self.column_type) +"," + str(self.default_value) +"," + str(self.key_type) + "," + self.is_nullable + "," + self.column_length + "," + self.column_precision + "," + self.column_scale
```

### Comparing `Metamorf-0.3.9.1/metamorf/tools/filecontroller.py` & `Metamorf-0.4.3.1/metamorf/tools/filecontroller.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from abc import ABC, abstractmethod
 import yaml
 from metamorf.constants import *
 import csv
 import json
+import os
 
 
 class FileController(ABC):
     @abstractmethod
     def __init__(self):
         pass
 
     def set_file_location(self, path: str, file_name: str):
-        self.path = path
-        self.file_name = file_name
+        self.path = str(path)
+        self.file_name = str(file_name)
 
     @abstractmethod
     def read_file(self):
         pass
 
     def setup_writer(self, append: str):
         if self.path is None or self.path == "":
@@ -38,15 +39,15 @@
 class FileControllerYML(FileController):
     def __init__(self):
         self.extension = FILE_TYPE_YML
         self.file = None
 
     def read_file(self):
         if len(self.file_name) == 0 or self.file_name is None: raise ValueError("FileController_YML: Trying to read a file with null name")
-        final_path = self.path + "\\" + self.file_name
+        final_path = os.path.join(self.path, self.file_name)
         if final_path[-4:] != "." + self.extension:
             final_path += "." + self.extension
         try:
             with open(final_path) as file:
                 file = yaml.full_load(file)
             return file
         except:
@@ -60,15 +61,15 @@
 class FileControllerJSON(FileController):
     def __init__(self):
         self.extension = FILE_TYPE_JSON
         self.file = None
 
     def read_file(self):
         if len(self.file_name) == 0 or self.file_name is None: raise ValueError("FileController_JSON: Trying to read a file with null name")
-        final_path = self.path + "\\" + self.file_name
+        final_path = os.path.join(self.path, self.file_name)
         if final_path[-4:] != "." + self.extension:
             final_path += "." + self.extension
         try:
             with open(final_path) as file:
                 file = json.load(file)
             return file
         except:
@@ -81,16 +82,16 @@
 class FileControllerSQL(FileController):
     def __init__(self):
         self.extension = FILE_TYPE_SQL
         self.file = None
 
     def read_file(self):
         if len(self.file_name)==0 or self.file_name==None: raise ValueError("FileController_SQL: Trying to read a file with None null")
-        final_path = self.path + '\\' + self.file_name
-        if final_path[-4:] != "." + self.extension:
+        final_path = os.path.join(self.path, self.file_name)
+        if str(final_path[-4:]) != "." + self.extension:
             final_path += "." + self.extension
         try:
             with open(final_path, encoding='utf-8') as file:
                 result = file.read()
             return result
         except:
             return None
@@ -100,15 +101,15 @@
 class FileControllerLOG(FileController):
     def __init__(self):
         self.extension = FILE_TYPE_LOG
         self.file = None
 
     def read_file(self):
         if len(self.file_name)==0 or self.file_name==None: raise ValueError("FileController_SQL: Trying to read a file with None null")
-        final_path = self.path + '\\' + self.file_name
+        final_path = os.path.join(self.path, self.file_name)
         if final_path[-4:] != "." + self.extension:
             final_path += "." + self.extension
         try:
             with open(final_path, encoding='utf-8') as file:
                 result = file.read()
             return result
         except:
@@ -119,15 +120,15 @@
 class FileControllerTXT(FileController):
     def __init__(self):
         self.extension = FILE_TYPE_TXT
         self.file = None
 
     def read_file(self):
         if len(self.file_name) == 0 or self.file_name is None: raise ValueError("FileController_SQL: Trying to read a file with None null")
-        final_path = self.path + '\\' + self.file_name
+        final_path = os.path.join(self.path, self.file_name)
         if final_path[-4:] != "." + self.extension:
             final_path += "." + self.extension
         try:
             with open(final_path, encoding='utf-8') as file:
                 result = file.read()
             return result
         except:
@@ -135,24 +136,28 @@
         return
 
 
 class FileControllerCSV(FileController):
     def __init__(self):
         self.extension = FILE_TYPE_CSV
         self.file = None
+        self.delimiter = ','
+
+    def set_delimiter(self, delimiter_character):
+        self.delimiter = delimiter_character
 
     def read_file(self):
-        if len(self.file_name) == 0 or self.file_name is None: raise ValueError(
-            "FileController_SQL: Trying to read a file with None null")
-        final_path = self.path + '\\' + self.file_name
+        if len(self.file_name) == 0 or self.file_name is None: raise ValueError("FileController_SQL: Trying to read a file with None null")
+        if self.path is None or self.path == '': final_path = self.file_name
+        else: final_path = os.path.join(self.path, self.file_name)
         if final_path[-4:] != "." + self.extension:
             final_path += "." + self.extension
         try:
             with open(final_path, encoding='utf-8') as file:
-                reader = csv.reader(file, delimiter=',', quotechar = '"')
+                reader = csv.reader(file, delimiter=self.delimiter, quotechar = '"')
                 result = []
                 for row in reader:
                     result.append(row)
             return result
         except:
             return None
         return None
```

### Comparing `Metamorf-0.3.9.1/metamorf/tools/log.py` & `Metamorf-0.4.3.1/metamorf/tools/log.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     def __init__(self):
         os.system('')
         self.file_log = FileControllerFactory().get_file_reader(FILE_TYPE_LOG)
         self.file_log.set_file_location(ACTUAL_PATH, LOG_FILE_NAME)
         self.file_log.setup_writer(FILE_WRITER_APPEND)
 
         file_controller_properties = FileControllerFactory().get_file_reader(FILE_TYPE_YML)
-        file_controller_properties.set_file_location(PACKAGE_PATH + "\\" + PROPERTIES_FILE_PATH, PROPERTIES_FILE_NAME)
+        file_controller_properties.set_file_location(os.path.join(PACKAGE_PATH, PROPERTIES_FILE_PATH), PROPERTIES_FILE_NAME)
         self.properties_file = file_controller_properties.read_file()
 
     def log(self, subject: str, message: str, level: int):
         date_now = datetime.now().strftime("%Y-%m-%d %H:%M:%S")
         self.file_log.write_file(date_now + " [" + subject + "] " + message + "\n")
         message = self._get_message_with_color(level, message)
         if 'options' not in self.properties_file: return
```

### Comparing `Metamorf-0.3.9.1/metamorf/tools/manifest.py` & `Metamorf-0.4.3.1/metamorf/tools/manifest.py`

 * *Files 7% similar despite different names*

```diff
@@ -75,17 +75,17 @@
         for col in metadata.om_dataset_specification_information:
             if col.dataset_name == dataset.dataset_name:
                 d_col = dict()
                 d_col['column_name'] = col.column_name
                 d_col['column_type'] = col.column_type
                 d_col['ordinal_position'] = col.ordinal_position
                 d_col['is_nullable'] = col.is_nullable
-                d_col['length'] = col.length
-                d_col['precision'] = col.precision
-                d_col['scale'] = col.scale
+                d_col['column_length'] = col.column_length
+                d_col['column_precision'] = col.column_precision
+                d_col['column_scale'] = col.column_scale
                 d_columns.append(d_col)
         d_info['columns'] = d_columns
 
         d[dataset.dataset_name] = d_info
         datasets.append(d)
 
     manifest['metadata'] = manifest_metadata
```

### Comparing `Metamorf-0.3.9.1/metamorf/tools/metadata.py` & `Metamorf-0.4.3.1/metamorf/tools/metadata.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,28 +14,32 @@
         self.entry_dataset_relationship = []
         self.entry_entity = []
         self.entry_having = []
         self.entry_path = []
         self.entry_dataset_mappings = []
         self.entry_dv_entity = []
         self.entry_dv_mappings = []
+        self.entry_dv_properties = []
+        self.entry_files = []
         # Metamorf Tables
         self.om_dataset = []
+        self.om_dataset_dv = []
         self.om_dataset_execution = []
         self.om_dataset_t_order = []
         self.om_dataset_t_agg = []
         self.om_dataset_t_distinct = []
         self.om_dataset_specification = []
         self.om_dataset_relationships = []
         self.om_dataset_t_filter = []
         self.om_dataset_t_mapping = []
         self.om_dataset_path = []
         self.om_dataset_t_having = []
         self.om_properties = []
         self.om_dataset_hardcoded = []
+        self.om_dataset_file = []
         # Reference Tables
         self.om_ref_query_type = []
         self.om_ref_order_type = []
         self.om_ref_join_type = []
         self.om_ref_modules = []
         self.om_ref_entity_type = []
         self.om_ref_key_type = []
@@ -69,29 +73,38 @@
             try:
                 self.entry_filters.append(EntryFilters(entry_filters[0], entry_filters[1], entry_filters[2], entry_filters[3]))
             except Exception as e:
                 self.log.log("Metadata Loader", "Error loading [Entry Filters]: " + str(e), LOG_LEVEL_ERROR)
                 return False
         return True
 
+    def add_entry_files(self, entry_files_list: list):
+        for entry_files in entry_files_list:
+            try:
+                self.entry_files.append(EntryFiles(entry_files[0], entry_files[1], entry_files[2], entry_files[3], entry_files[4]))
+            except Exception as e:
+                self.log.log("Metadata Loader", "Error loading [Entry Files]: " + str(e), LOG_LEVEL_ERROR)
+                return False
+        return True
+
     def add_entry_having(self, entry_having_list: list):
         for entry_having in entry_having_list:
             try:
                 self.entry_having.append(EntryHaving(entry_having[0], entry_having[1], entry_having[2], entry_having[3]))
             except Exception as e:
                 self.log.log("Metadata Loader", "Error loading [Entry Having]: " + str(e), LOG_LEVEL_ERROR)
                 return False
         return True
 
     def add_entry_dataset_relationship(self, entry_dataset_relationship_list: list):
         for entry_dataset_relationship in entry_dataset_relationship_list:
             try:
                 self.entry_dataset_relationship.append(EntryDatasetRelationships(entry_dataset_relationship[0], entry_dataset_relationship[1], entry_dataset_relationship[2], entry_dataset_relationship[3], entry_dataset_relationship[4], entry_dataset_relationship[5]))
             except Exception as e:
-                self.log.log("Metadata Loader", "Error loading [Entry Order]: " + str(e), LOG_LEVEL_ERROR)
+                self.log.log("Metadata Loader", "Error loading [Entry Relationship]: " + str(e), LOG_LEVEL_ERROR)
                 return False
         return True
 
     def add_entry_entity(self, entry_entity_list: list):
         for entry_entity in entry_entity_list:
             try:
                 self.entry_entity.append(EntryEntity(entry_entity[0], entry_entity[1], entry_entity[2], entry_entity[3], entry_entity[4], entry_entity[5]))
@@ -117,38 +130,56 @@
                 self.log.log("Metadata Loader", "Error loading [Entry Order]: " + str(e), LOG_LEVEL_ERROR)
                 return False
         return True
 
     def add_entry_dv_entity(self, entry_dv_entity_list: list):
         for entry_dv_entity in entry_dv_entity_list:
             try:
-                self.entry_dv_entity.append(EntryDvEntry(entry_dv_entity[0],entry_dv_entity[1],entry_dv_entity[2],entry_dv_entity[3],entry_dv_entity[4],entry_dv_entity[5],entry_dv_entity[6],entry_dv_entity[7],entry_dv_entity[8],entry_dv_entity[9],entry_dv_entity[10]))
+                self.entry_dv_entity.append(EntryDvEntry(entry_dv_entity[0],entry_dv_entity[1],entry_dv_entity[2],entry_dv_entity[3],entry_dv_entity[4],entry_dv_entity[5],entry_dv_entity[6],entry_dv_entity[7]))
             except Exception as e:
                 self.log.log("Metadata Loader", "Error loading [Entry DV Entity]: " + str(e), LOG_LEVEL_ERROR)
                 return False
         return True
 
     def add_entry_dv_mappings(self, entry_dv_mappings_list: list):
         for entry_dv_mappings in entry_dv_mappings_list:
             try:
-                self.entry_dv_mappings.append(EntryDvMappings(entry_dv_mappings[0],entry_dv_mappings[1],entry_dv_mappings[2],entry_dv_mappings[3],entry_dv_mappings[4],entry_dv_mappings[5],entry_dv_mappings[6],entry_dv_mappings[7],entry_dv_mappings[8],entry_dv_mappings[9]))
+                self.entry_dv_mappings.append(EntryDvMappings(entry_dv_mappings[0],entry_dv_mappings[1],entry_dv_mappings[2],entry_dv_mappings[3],entry_dv_mappings[4],entry_dv_mappings[5],entry_dv_mappings[6],entry_dv_mappings[7],entry_dv_mappings[8],entry_dv_mappings[9],entry_dv_mappings[10],entry_dv_mappings[11],entry_dv_mappings[12],entry_dv_mappings[13],entry_dv_mappings[14],entry_dv_mappings[15]))
+            except Exception as e:
+                self.log.log("Metadata Loader", "Error loading [Entry DV Mappings]: " + str(e), LOG_LEVEL_ERROR)
+                return False
+        return True
+
+    def add_entry_dv_properties(self, entry_dv_properties_list: list):
+        for entry_dv_properties in entry_dv_properties_list:
+            try:
+                self.entry_dv_properties.append(EntryDvProperties(entry_dv_properties[0],entry_dv_properties[1],entry_dv_properties[2],entry_dv_properties[3]))
             except Exception as e:
                 self.log.log("Metadata Loader", "Error loading [Entry DV Mappings]: " + str(e), LOG_LEVEL_ERROR)
                 return False
         return True
 
     def add_om_dataset(self, om_dataset_list: list):
         for om_dataset in om_dataset_list:
             try:
                 self.om_dataset.append(OmDataset(om_dataset[0],om_dataset[1],om_dataset[2],om_dataset[3],om_dataset[4],om_dataset[5],om_dataset[6]))
             except Exception as e:
                 self.log.log("Metadata Loader", "Error loading [Dataset]: " + str(e), LOG_LEVEL_ERROR)
                 return False
         return True
 
+    def add_om_dataset_dv(self, om_dataset_dv_list: list):
+        for om_dataset_dv in om_dataset_dv_list:
+            try:
+                self.om_dataset_dv.append(OmDatasetDv(om_dataset_dv[0],om_dataset_dv[1],om_dataset_dv[2],om_dataset_dv[3],om_dataset_dv[4]))
+            except Exception as e:
+                self.log.log("Metadata Loader", "Error loading [Dataset DV]: " + str(e), LOG_LEVEL_ERROR)
+                return False
+        return True
+
     def add_om_dataset_execution(self, om_dataset_execution_list: list):
         for om_dataset_execution in om_dataset_execution_list:
             try:
                 self.om_dataset_execution.append(OmDatasetExecution(om_dataset_execution[0],om_dataset_execution[1],om_dataset_execution[2],om_dataset_execution[3],om_dataset_execution[4]))
             except Exception as e:
                 self.log.log("Metadata Loader", "Error loading [Dataset Execution]: " + str(e), LOG_LEVEL_ERROR)
                 return False
@@ -317,38 +348,86 @@
         return True
 
     def add_om_relationships(self, om_relationships_list):
         for om_relationships in om_relationships_list:
             try:
                 self.om_relationships.append(OmRelationships(om_relationships[0],om_relationships[1],om_relationships[2],om_relationships[3],om_relationships[4],om_relationships[5],om_relationships[6],om_relationships[7],om_relationships[8],om_relationships[9]))
             except Exception as e:
-                self.log.log("Metadata Loader", "Error loading [Relationships]: " + str(e), LOG_LEVEL_ERROR)
+                self.log.log("Metadata Loader", "Error loading [Dataset Relationships]: " + str(e), LOG_LEVEL_ERROR)
+                return False
+        return True
+
+    def add_om_dataset_file(self, om_dataset_file_list):
+        for om_dataset_file in om_dataset_file_list:
+            try:
+                self.om_dataset_file.append(OmDatasetFile(om_dataset_file[0],om_dataset_file[1],om_dataset_file[2],om_dataset_file[3],om_dataset_file[4],om_dataset_file[5],om_dataset_file[6]))
+            except Exception as e:
+                self.log.log("Metadata Loader", "Error loading [Dataset File]: " + str(e), LOG_LEVEL_ERROR)
                 return False
         return True
 
     def add_om_dataset_specification_information(self, om_dataset_specification_information_list):
         for om_dataset_specification_information in om_dataset_specification_information_list:
             try:
                 self.om_dataset_specification_information.append(OmDatasetSpecificationInformation(om_dataset_specification_information[0],om_dataset_specification_information[1],om_dataset_specification_information[2],om_dataset_specification_information[3],om_dataset_specification_information[4],om_dataset_specification_information[5],om_dataset_specification_information[6],om_dataset_specification_information[7],om_dataset_specification_information[8]))
             except Exception as e:
                 self.log.log("Metadata Loader", "Error loading [Dataset Specification Information]: " + str(e), LOG_LEVEL_ERROR)
                 return False
         return True
 
     def get_dataset_from_dataset_name(self, dataset):
-        """Return ID_DATASET from DATASET_NAME. If not exists returns -1"""
+        """Return ID_DATASET from DATASET_NAME. If not exists returns None"""
         for d in self.om_dataset:
             if d.dataset_name == dataset and (d.end_date is None or d.end_date == 'NULL'): return d
         return None
 
+    def get_entry_entity_from_cod_entity(self, cod_entity):
+        for d in self.entry_entity:
+            if d.cod_entity == cod_entity: return d
+        return None
+
+    def get_num_branches_on_entry_dv_from_cod_entity_name(self, cod_entity_name):
+        num_branches = 0
+        for d in self.entry_dv_mappings:
+            if d.cod_entity_target != cod_entity_name: continue
+            if d.num_branch > num_branches: num_branches = d.num_branch
+        return num_branches
+
+    def get_num_connections_on_entry_dv_from_cod_entity_name(self, cod_entity_name):
+        num_connection = 0
+        for d in self.entry_dv_mappings:
+            if d.cod_entity_target != cod_entity_name: continue
+            if d.num_connection > num_connection: num_connection = d.num_connection
+        return num_connection
+
+    def get_all_bk_from_entry_dv_cod_entity_target_and_num_branch(self, cod_entity, num_branch):
+        all_bk = []
+        for d in self.entry_dv_mappings:
+            if d.cod_entity_target != cod_entity or d.num_branch != num_branch: continue
+            if d.key_type.upper() == KEY_TYPE_BUSINESS_KEY or d.key_type.upper() == KEY_TYPE_DRIVENKEY: all_bk.append(d)
+        return all_bk
+
+    def get_all_bk_from_entry_dv_cod_entity_target_and_num_branch_and_num_connection(self, cod_entity, num_branch, num_connection):
+        all_bk = []
+        for d in self.entry_dv_mappings:
+            if d.cod_entity_target != cod_entity or d.num_branch != num_branch or d.num_connection != num_connection: continue
+            if d.key_type.upper() == KEY_TYPE_BUSINESS_KEY or d.key_type.upper() == KEY_TYPE_DRIVENKEY:all_bk.append(d)
+        return all_bk
+
+
     def get_dataset_execution_from_id_dataset(self, id_dataset):
         for execution in self.om_dataset_execution:
             if execution.id_dataset == id_dataset and (execution.end_date is None or execution.end_date == 'NULL'): return execution
         return None
 
+    def get_dataset_dv_from_id_dataset(self, id_dataset):
+        for dataset_dv in self.om_dataset_dv:
+            if dataset_dv.id_dataset == id_dataset and (dataset_dv.end_date is None or dataset_dv.end_date == 'NULL'): return dataset_dv
+        return None
+
     def get_path_from_database_and_schema(self, database, schema):
         """Return PATH from DATABASE and SCHEMA names. If not exists returns None"""
         for path in self.om_dataset_path:
             if str(path.database_name) == str(database) and str(path.schema_name) == str(schema) and (path.end_date is None or path.end_date == 'NULL'): return path
         return None
 
     def get_path_from_id_path(self, id_path):
@@ -380,17 +459,16 @@
         return None
 
     def get_cols_from_cod_entity_on_entry(self,cod_entity):
         all_cols = []
         columns_name_added = []
         for col in self.entry_dataset_mappings:
             if col.cod_entity_target == cod_entity:
-                pk = 0
-                if col.key_type == KEY_TYPE_PRIMARY_KEY: pk = 1
-                columna = Column(col.ordinal_position, col.column_name_target, col.column_type_target, None, pk, 0,col.length,col.precision,0)
+                if col.key_type is None: col.key_type = "NULL"
+                columna = Column(col.ordinal_position, col.column_name_target, col.column_type_target, None, col.key_type, 0,col.column_length,col.column_precision,0)
                 if col.column_name_target not in columns_name_added:
                     all_cols.append(columna)
                     columns_name_added.append(col.column_name_target)
         return all_cols
 
     def get_order_from_id_dataset_and_id_dataset_spec_and_id_branch(self, id_dataset, id_dataset_spec, id_branch):
         for order in self.om_dataset_t_order:
@@ -539,15 +617,15 @@
         return fqdn
 
     def get_num_branches_from_dataset_name(self, dataset_name):
         dataset = self.get_dataset_from_dataset_name(dataset_name)
         max_num_branch = 0
         for dataset_spec in [x for x in self.om_dataset_specification if x.end_date is None]:
             if dataset_spec.id_dataset == dataset.id_dataset:
-                for map in [x for x in self.om_dataset_t_mapping if x.end_date is None and x.id_dataset_spec == dataset_spec.id_dataset_spec]:
+                for map in [x for x in self.om_dataset_t_mapping if (x.end_date is None or x.end_date == '') and x.id_dataset_spec == dataset_spec.id_dataset_spec]:
                     if map.id_branch>max_num_branch: max_num_branch=map.id_branch
         return max_num_branch
 
     def get_list_id_dataset_spec_from_dataset_name(self, dataset_name):
         dataset = self.get_dataset_from_dataset_name(dataset_name)
         list_id_dataset_spec = []
         for dataset_spec in [x for x in self.om_dataset_specification if x.end_date is None]:
@@ -572,12 +650,114 @@
 
     def get_dataset_fqdn_from_dataset_name(self, dataset_name):
         path = self.get_path_from_dataset_name(dataset_name)
         fqdn = self.get_fqdn_from_path(path)
         if fqdn != "": fqdn += "."
         return fqdn + dataset_name
 
-
-
+    def get_record_source_on_dv_from_cod_entity_target_and_num_branch(self, cod_entity_target, num_branch):
+        for d in self.entry_dv_mappings:
+            if d.key_type != KEY_TYPE_RECORD_SOURCE: continue
+            if d.cod_entity_target == cod_entity_target and d.num_branch == num_branch:
+                return d
+        return None
+
+    def get_applied_date_on_dv_from_cod_entity_target(self, cod_entity_target, num_branch):
+        for d in self.entry_dv_mappings:
+            if d.key_type != KEY_TYPE_APPLIED_DATE: continue
+            if d.cod_entity_target == cod_entity_target and d.num_branch == num_branch:
+                return d
+        return None
+
+    def get_dependent_child_key_on_dv_from_satellite_name(self, satellite_name):
+        all_dck = []
+        for d in self.entry_dv_mappings:
+            if d.key_type != KEY_TYPE_DEPENDENT_CHILD_KEY: continue
+            if d.satellite_name == satellite_name: all_dck.append(d)
+        return all_dck
+
+    def get_tenant_on_dv_from_cod_entity_target_and_num_branch(self, cod_entity_target, num_branch):
+        all_tenant = []
+        for d in self.entry_dv_mappings:
+            if d.key_type != KEY_TYPE_TENANT: continue
+            if d.cod_entity_target == cod_entity_target and d.num_branch == num_branch:
+                all_tenant.append(d)
+        return all_tenant
+
+    def get_seq_on_dv_from_cod_entity_target_and_num_branch(self, cod_entity_target, num_branch):
+        all_seq = []
+        for d in self.entry_dv_mappings:
+            if d.key_type != KEY_TYPE_SEQUENCE: continue
+            if d.cod_entity_target == cod_entity_target and d.num_branch == num_branch:
+                all_seq.append(d)
+        return all_seq
+
+    def get_tenant_on_dv_from_cod_entity_target_and_num_branch_and_num_connection(self, cod_entity_target, num_branch, num_connection):
+        all_tenant = []
+        for d in self.entry_dv_mappings:
+            if d.key_type != KEY_TYPE_TENANT: continue
+            if d.cod_entity_target == cod_entity_target and d.num_branch == num_branch and d.num_connection == num_connection:
+                all_tenant.append(d)
+        return all_tenant
+
+    def get_attributes_on_dv_from_satellite_name(self, satellite_name):
+        all_attributes = []
+        for d in self.entry_dv_mappings:
+            if d.key_type != KEY_TYPE_ATTRIBUTE and d.key_type != KEY_TYPE_STATUS: continue
+            if d.satellite_name == satellite_name: all_attributes.append(d)
+        return all_attributes
+
+    def get_all_satellites_info_from_hub(self, cod_entity_target):
+        all_satellites = []
+        for d in self.entry_dv_mappings:
+            if d.cod_entity_target == cod_entity_target:
+                if d.satellite_name != '' and d.satellite_name != None and (d.cod_entity_source, d.cod_entity_target,d.satellite_name, d.num_branch, d.origin_is_incremental, d.origin_is_total, d.origin_is_cdc) not in all_satellites:
+                    all_satellites.append((d.cod_entity_source, d.cod_entity_target,d.satellite_name, d.num_branch, d.origin_is_incremental, d.origin_is_total, d.origin_is_cdc))
+        return all_satellites
+
+    def get_dv_properties_from_cod_entity_and_num_connection(self,cod_entity, num_connection):
+        for d in self.entry_dv_properties:
+            if d.cod_entity == cod_entity and int(d.num_connection) == int(num_connection):
+                return d
+        return None
+
+    def get_all_cod_entity_source_from_cod_entity_target_on_entry_dv(self, cod_entity):
+        all_cod_entity = []
+        all_entities = []
+        for d in self.entry_dv_mappings:
+            if d.cod_entity_target == cod_entity and d.cod_entity_source not in all_cod_entity:
+                all_cod_entity.append(d.cod_entity_source)
+                all_entities.append(d)
+        return all_entities
+
+    def get_first_entry_dv_mappings_from_cod_entity_target_and_key_type_and_num_branch(self, cod_entity, key_type, num_branch):
+        for d in self.entry_dv_mappings:
+            if d.num_branch != num_branch: continue
+            if d.cod_entity_target == cod_entity and key_type == d.key_type: return d
+        return None
+
+    def get_dict_origin_type_from_cod_entity_on_dv(self, cod_entity):
+        source_options = dict()
+        source_options['origin_is_cdc'] = 0
+        source_options['origin_is_incremental'] = 0
+        source_options['origin_is_total'] = 0
+        for d in self.entry_dv_mappings:
+            if d.cod_entity_target == cod_entity:
+                if d.origin_is_cdc == 1: source_options['origin_is_cdc'] = 1
+                if d.origin_is_incremental == 1: source_options['origin_is_incremental'] = 1
+                if d.origin_is_total == 1: source_options['origin_is_total'] = 1
+        return source_options
+
+    def get_list_num_connection_with_driven_key_from_cod_entity_target(self, cod_entity):
+        all_connections_with_dk = []
+        for d in self.entry_dv_mappings:
+            if d.cod_entity_target == cod_entity and d.key_type == KEY_TYPE_DRIVENKEY:
+                if d.num_connection not in all_connections_with_dk: all_connections_with_dk.append(d.num_connection)
+        return all_connections_with_dk
+
+    def get_om_dataset_file_from_id_dataset(self, id_dataset):
+        for d in self.om_dataset_file:
+            if d.id_dataset == id_dataset: return d
+        return None
```

### Comparing `Metamorf-0.3.9.1/metamorf/tools/node.py` & `Metamorf-0.4.3.1/metamorf/tools/node.py`

 * *Files identical despite different names*

### Comparing `Metamorf-0.3.9.1/metamorf/tools/query.py` & `Metamorf-0.4.3.1/metamorf/tools/query.py`

 * *Files 13% similar despite different names*

```diff
@@ -23,22 +23,26 @@
         self.values = []
         self.has_header = False
         self.values_batch = 1000 # Num of values that an insert can execute
         self.columns_and_specs = []
         self.database = None
         self.is_truncate = False
         self.need_create_table = False
+        self.need_drop_table = False
 
     def set_database(self, database: str):
         '''Set the Target database of the query. Use the constants CONNECTION_[X]'''
         self.database = database
 
     def set_need_create_table(self, option):
         self.need_create_table = option
 
+    def set_need_drop_table(self, option):
+        self.need_drop_table = option
+
     def set_is_truncate(self, is_truncate):
         self.is_truncate = is_truncate
 
     def set_type(self, type: int):
         self.type = type
 
     def set_values_batch(self, values_batch: int):
@@ -123,27 +127,63 @@
     def set_has_header(self, option: bool):
         self.has_header = option
 
     def get_dataset_name_from_fqdn(self, dataset_name):
         dataset = dataset_name.split(".")
         return dataset[len(dataset)-1]
 
+    def _get_all_from_tables_from_query(self, query: Query):
+        all_from_tables = []
+        for x in query.from_tables:
+            if x not in all_from_tables: all_from_tables.append(x)
+        for x in query.from_tables_and_relations:
+            if x.master_table not in all_from_tables: all_from_tables.append(x.master_table)
+            if x.detail_table not in all_from_tables: all_from_tables.append(x.detail_table)
+        return all_from_tables
+
     def __str__(self):
         query = ""
         all_from_tables = ""
         all_group_by_columns = ""
         all_having_columns = ""
         all_select_columns = ""
         all_insert_columns = ""
         all_where_filters = ""
         all_order_by = ""
         all_values = ""
 
         self.validate_query_elements()
 
+        # Order WITH queries
+        all_with_queries = self.subqueries.copy()
+        all_with_to_be_processed = [] # all with that need to be processed
+        for q in self.subqueries:
+            if q.name_query not in all_with_to_be_processed: all_with_to_be_processed.append(q.name_query)
+        all_with_to_be_processed = set(all_with_to_be_processed)
+        index = 0
+        all_with_ordered = [] # all_query_objects ordered
+        with_added = [] # all with names that have been already added
+        while all_with_queries:
+            with_query = all_with_queries[index]
+            all_from_tab = self._get_all_from_tables_from_query(with_query)
+            for with_processed in with_added:
+                if with_processed in all_from_tab: all_from_tab.remove(with_processed)
+            set_all_from_tables = set(all_from_tab)
+            result_intersection = list(set_all_from_tables.intersection(all_with_to_be_processed))
+            if len(result_intersection)==0:
+                all_with_ordered.append(with_query)
+                with_added.append(with_query.name_query)
+                all_with_queries.remove(with_query)
+                index = 0
+            else:
+                index +=1
+
+        self.subqueries = all_with_ordered.copy()
+        self.subqueries.reverse()
+
         # SELECT
         all_select_columns += ','.join([str(col) for col in self.select_columns])
 
         # INSERT
         all_insert_columns += ','.join([str(col) for col in self.insert_columns])
 
         # FROM
@@ -155,40 +195,43 @@
         includedTables = []
         all_relation_to_include = self.from_tables_and_relations
         pos = 0
 
         while len(all_relation_to_include) > 0:
             relation = all_relation_to_include[pos]
             if not includedTables: # If it's the first relation, we include it
-
                 all_relations_same_tables = []
+                relations_to_delete = []
                 for rel in all_relation_to_include:
                     if relation.master_table == rel.master_table and relation.detail_table == rel.detail_table:
-                        if rel!=relation: all_relation_to_include.remove(rel)
+                        if rel != relation: relations_to_delete.append(rel)
                         all_relations_same_tables.append(rel)
+                for rel in relations_to_delete: all_relation_to_include.remove(rel)
 
                 all_from_tables += relation.master_table + " "+ self.get_dataset_name_from_fqdn(relation.master_table) + " " + self.get_join_from_id(relation.join_type) + " " + relation.detail_table + " " + self.get_dataset_name_from_fqdn(relation.detail_table) + " ON "
 
                 for rel in all_relations_same_tables:
-                   all_from_tables += self.get_dataset_name_from_fqdn(rel.master_table) + "." + rel.master_column + " " + rel.join_sign + " " + self.get_dataset_name_from_fqdn(rel.detail_table) + "." + rel.detail_column + " AND "
+                    all_from_tables += self.get_dataset_name_from_fqdn(rel.master_table) + "." + rel.master_column + " " + rel.join_sign + " " + self.get_dataset_name_from_fqdn(rel.detail_table) + "." + rel.detail_column + " AND "
 
                 all_from_tables = all_from_tables[:-4] + "\n"
                 includedTables.append(relation.master_table)
                 includedTables.append(relation.detail_table)
                 all_relation_to_include.remove(relation)
                 pos = 0
                 continue
             else:
 
                 if relation.master_table in includedTables:
                     all_relations_same_tables = []
+                    relations_to_delete = []
                     for rel in all_relation_to_include:
                         if relation.master_table == rel.master_table and relation.detail_table == rel.detail_table:
-                            if rel != relation: all_relation_to_include.remove(rel)
+                            if rel != relation: relations_to_delete.append(rel)
                             all_relations_same_tables.append(rel)
+                    for rel in relations_to_delete: all_relation_to_include.remove(rel)
 
                     all_from_tables += self.get_join_from_id(relation.join_type) + " " + relation.detail_table + " " + self.get_dataset_name_from_fqdn(relation.detail_table) + " ON "
                     for rel in all_relations_same_tables:
                         all_from_tables += self.get_dataset_name_from_fqdn(rel.master_table) + "." + rel.master_column + " " + rel.join_sign + " " + self.get_dataset_name_from_fqdn(rel.detail_table) + "." + rel.detail_column + " AND "
                     all_from_tables = all_from_tables[:-4] + "\n"
 
                     includedTables.append(relation.detail_table)
@@ -198,18 +241,20 @@
                 if relation.detail_table in includedTables:
 
                     if relation.join_type == 1: joinType = 2
                     elif relation.join_type == 2: joinType = 1
                     else: joinType = relation.join_type
 
                     all_relations_same_tables = []
+                    relations_to_delete = []
                     for rel in all_relation_to_include:
                         if relation.master_table == rel.master_table and relation.detail_table == rel.detail_table:
-                            if rel != relation: all_relation_to_include.remove(rel)
+                            if rel != relation: relations_to_delete.append(rel)
                             all_relations_same_tables.append(rel)
+                    for rel in relations_to_delete: all_relation_to_include.remove(rel)
 
                     all_from_tables += self.get_join_from_id(joinType) + " " + relation.master_table + " " + self.get_dataset_name_from_fqdn(relation.master_table)+ " ON "
                     for rel in all_relations_same_tables:
                         all_from_tables += self.get_dataset_name_from_fqdn(rel.detail_table) + "." + rel.detail_column + " " + rel.join_sign + " " + self.get_dataset_name_from_fqdn(rel.master_table) + "." + rel.master_column + " AND "
                     all_from_tables = all_from_tables[:-4] + "\n"
 
                     includedTables.append(relation.master_table)
@@ -258,19 +303,21 @@
             all_values += "(" + str(value) + "),"
             index += 1
         all_values = all_values[:-1]
         if all_values!="VALUES":
             values_list.append(all_values)
 
         #######################################################################################
+        if self.need_drop_table:
+            query += "DROP TABLE " + self.target_table + ";\n\n"
+
         if self.need_create_table:
             query += "CREATE TABLE "+ self.target_table +" (\n"
             for col in self.columns_and_specs:
                 query += col + ",\n"
-            pass
             query = query[:-2]
             query+=");\n\n"
 
         if self.is_truncate:
             if self.database.upper() == CONNECTION_SQLITE.upper():
                 query += "DELETE FROM " + self.target_table +";\n\n"
             else:
@@ -315,14 +362,21 @@
             for x in values_list:
                 query += "INSERT INTO " + self.target_table + "(" + all_insert_columns + ")\n"
                 query += x
                 query += ";"
             if len(self.values) <= 1 and self.has_header: query = ""
             if len(values_list)==0: query = ""
 
+            if (len(self.values) <= 1 and self.has_header) or len(values_list)==0:
+                if self.need_drop_table:
+                    if self.database.upper() == CONNECTION_SQLITE.upper():
+                        query += "DELETE FROM " + self.target_table + ";\n\n"
+                    else:
+                        query += "TRUNCATE TABLE " + self.target_table + ";\n\n"
+
         if self.type == QUERY_TYPE_DELETE:
             where = ""
             if len(self.where_filters)>1:
                 for where_filter in self.where_filters:
                     where += where_filter + " AND "
                 where = where[:-4]
             else:
@@ -349,15 +403,15 @@
         if id == JOIN_TYPE_INNER:
             result = "INNER JOIN"
         elif id == JOIN_TYPE_MASTER:
             result = "LEFT JOIN"
         elif id == JOIN_TYPE_DETAIL:
             result = "RIGHT JOIN"
         elif id == JOIN_TYPE_OUTER:
-            result = "OUTER JOIN"
+            result = "FULL OUTER JOIN"
         else:
             raise ValueError("Join doesn't exist")
         return result
 
 class FromRelationQuery:
     def __init__(self, master_table: str, master_column: str, detail_table: str, detail_column: str, join_type: str, join_sign: str):
         self.master_table = master_table
```

### Comparing `Metamorf-0.3.9.1/metamorf/tools/utils.py` & `Metamorf-0.4.3.1/metamorf/tools/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,25 @@
         res = connection.execute(str(query))
         if res is False: return None
         data = connection.get_query_result()
         res= metadata.add_om_dataset(data)
         if res is False: return None
         log.log("Metadata Loader", "Finished to load [OM_DATASET]", LOG_LEVEL_DEBUG)
 
+        # OM_DATASET_DV
+        log.log("Metadata Loader", "Start to load [OM_DATASET_DV]", LOG_LEVEL_DEBUG)
+        query.set_from_tables(TABLE_OM_DATASET_DV)
+        query.set_select_columns(COLUMNS_OM_DATASET_DV)
+        res = connection.execute(str(query))
+        if res is False: return None
+        data = connection.get_query_result()
+        res = metadata.add_om_dataset_dv(data)
+        if res is False: return None
+        log.log("Metadata Loader", "Finished to load [OM_DATASET_DV]", LOG_LEVEL_DEBUG)
+
         # OM_DATASET_EXECUTION
         log.log("Metadata Loader", "Start to load [OM_DATASET_EXECUTION]", LOG_LEVEL_DEBUG)
         query.set_from_tables(TABLE_OM_DATASET_EXECUTION)
         query.set_select_columns(COLUMNS_OM_DATASET_EXECUTION)
         res = connection.execute(str(query))
         if res is False: return None
         data = connection.get_query_result()
@@ -140,14 +151,25 @@
         res = connection.execute(str(query))
         if res is False: return None
         data = connection.get_query_result()
         res = metadata.add_om_dataset_relationships(data)
         if res is False: return None
         log.log("Metadata Loader", "Finished to load [OM_DATASET_RELATIONSHIPS]", LOG_LEVEL_DEBUG)
 
+        # OM_DATASET_FILE
+        log.log("Metadata Loader", "Start to load [OM_DATASET_FILE]", LOG_LEVEL_DEBUG)
+        query.set_from_tables(TABLE_OM_DATASET_FILE)
+        query.set_select_columns(COLUMNS_OM_DATASET_FILE)
+        res = connection.execute(str(query))
+        if res is False: return None
+        data = connection.get_query_result()
+        res = metadata.add_om_dataset_file(data)
+        if res is False: return None
+        log.log("Metadata Loader", "Finished to load [OM_DATASET_FILE]", LOG_LEVEL_DEBUG)
+
         # OM_DATASET_HARDCODED
         log.log("Metadata Loader", "Start to load [OM_DATASET_HARDCODED]", LOG_LEVEL_DEBUG)
         query.set_from_tables(TABLE_OM_DATASET_HARDCODED)
         query.set_select_columns(COLUMNS_OM_DATASET_HARDCODED)
         res = connection.execute(str(query))
         if res is False: return None
         data = connection.get_query_result()
@@ -163,14 +185,15 @@
         res = connection.execute(str(query))
         if res is False: return None
         data = connection.get_query_result()
         res = metadata.add_om_properties(data)
         if res is False: return None
         log.log("Metadata Loader", "Finished to load [OM_PROPERTIES]", LOG_LEVEL_DEBUG)
 
+
     if load_ref:
         query.set_where_filters(None)
 
         # OM_REF_QUERY_TYPE
         log.log("Metadata Loader", "Start to load [OM_REF_QUERY_TYPE]", LOG_LEVEL_DEBUG)
         query.set_from_tables(TABLE_OM_REF_QUERY_TYPE)
         query.set_select_columns(COLUMNS_OM_REF_QUERY_TYPE)
@@ -324,35 +347,57 @@
         res = connection.execute(str(query))
         if res is False: return None
         data = connection.get_query_result()
         res = metadata.add_entry_dataset_mappings(data)
         if res is False: return None
         log.log("Metadata Loader", "Finished to load [ENTRY_DATASET_MAPPINGS]", LOG_LEVEL_DEBUG)
 
-        # ENTRY_DATASET_MAPPINGS
+        # ENTRY_DV_MAPPINGS
         log.log("Metadata Loader", "Start to load [ENTRY_DV_MAPPINGS]", LOG_LEVEL_DEBUG)
         query.set_from_tables(TABLE_ENTRY_DV_MAPPINGS)
         query.set_select_columns(COLUMNS_ENTRY_DV_MAPPINGS)
         res = connection.execute(str(query))
         if res is False: return None
         data = connection.get_query_result()
         res = metadata.add_entry_dv_mappings(data)
         if res is False: return None
         log.log("Metadata Loader", "Finished to load [ENTRY_DV_MAPPINGS]", LOG_LEVEL_DEBUG)
 
-        # ENTRY_DATASET_MAPPINGS
-        log.log("Metadata Loader", "Start to load [ENTRY_DV_MAPPINGS]", LOG_LEVEL_DEBUG)
+        # ENTRY_DV_ENTITY
+        log.log("Metadata Loader", "Start to load [TABLE_ENTRY_DV_ENTITY]", LOG_LEVEL_DEBUG)
         query.set_from_tables(TABLE_ENTRY_DV_ENTITY)
         query.set_select_columns(COLUMNS_ENTRY_DV_ENTITY)
         res = connection.execute(str(query))
         if res is False: return None
         data = connection.get_query_result()
         res = metadata.add_entry_dv_entity(data)
         if res is False: return None
-        log.log("Metadata Loader", "Finished to load [ENTRY_DV_MAPPINGS]", LOG_LEVEL_DEBUG)
+        log.log("Metadata Loader", "Finished to load [TABLE_ENTRY_DV_ENTITY]", LOG_LEVEL_DEBUG)
+
+        # ENTRY_DV_PROPERTIES
+        log.log("Metadata Loader", "Start to load [TABLE_ENTRY_DV_PROPERTIES]", LOG_LEVEL_DEBUG)
+        query.set_from_tables(TABLE_ENTRY_DV_PROPERTIES)
+        query.set_select_columns(COLUMNS_ENTRY_DV_PROPERTIES)
+        res = connection.execute(str(query))
+        if res is False: return None
+        data = connection.get_query_result()
+        res = metadata.add_entry_dv_properties(data)
+        if res is False: return None
+        log.log("Metadata Loader", "Finished to load [TABLE_ENTRY_DV_PROPERTIES]", LOG_LEVEL_DEBUG)
+
+        # ENTRY_FILES
+        log.log("Metadata Loader", "Start to load [TABLE_ENTRY_FILES]", LOG_LEVEL_DEBUG)
+        query.set_from_tables(TABLE_ENTRY_FILES)
+        query.set_select_columns(COLUMNS_ENTRY_FILES)
+        res = connection.execute(str(query))
+        if res is False: return None
+        data = connection.get_query_result()
+        res = metadata.add_entry_files(data)
+        if res is False: return None
+        log.log("Metadata Loader", "Finished to load [TABLE_ENTRY_FILES]", LOG_LEVEL_DEBUG)
 
     if load_im:
         where_filter = COLUMN_OM_OWNER + "='" + owner + "'"
         query.set_where_filters(where_filter)
 
         # OM_DATASET_INFORMATION
         log.log("Metadata Loader", "Start to load [OM_DATASET_INFORMATION]", LOG_LEVEL_DEBUG)
@@ -422,15 +467,15 @@
             if data.id_entity_type != metadata.get_entity_type_from_entity_type_name(ENTITY_WITH).id_entity_type:
                 from_tables.append(src)
             else:
                 with_tables.append(src)
                 with_to_get_source = metadata.get_dataset_from_dataset_name(src)
                 from_tables.extend(get_sources_from_dataset_with(metadata, with_to_get_source))
 
-        if dataset.dataset_name in from_tables: from_tables.remove(dataset.dataset_name)
+        if dataset.dataset_name in from_tables: from_tables = [i for i in from_tables if i != dataset.dataset_name]
         from_tables = list(dict.fromkeys(from_tables))
 
 
         main_query = get_query_object_from_dataset(dataset, False, metadata)
 
         for with_table in list(set(with_tables)):
             with_dataset = metadata.get_dataset_from_dataset_name(with_table)
@@ -464,17 +509,26 @@
     # PK Columns
     pk_columns = []
     for dataset_spec in [x for x in metadata.om_dataset_specification if x.end_date is None and x.id_dataset == dataset.id_dataset and x.id_key_type == metadata.get_key_type_from_key_type_name(KEY_TYPE_PRIMARY_KEY)]:
         pk_columns.append(metadata.get_tables_dot_column_from_id_dataset_spec(dataset_spec.id_dataset_spec))
 
     # Create table
     columns_specs = []
-    for dataset_spec in [x for x in metadata.om_dataset_specification if x.end_date is None and x.id_dataset == dataset.id_dataset]:
-        columns_specs.append(dataset_spec.column_name + " " + dataset_spec.column_type)
-
+    all_dataset_specs_from_dataset = [x for x in metadata.om_dataset_specification if x.end_date is None and x.id_dataset == dataset.id_dataset]
+    all_dataset_specs_from_dataset.sort(key=lambda x: x.ordinal_position)
+    for dataset_spec in all_dataset_specs_from_dataset:
+        length_details = ''
+        if dataset_spec.column_length != 0 and dataset_spec.column_length is not None:
+            length_details = "(" + str(dataset_spec.column_length) + ")"
+        if dataset_spec.column_precision != 0 and dataset_spec.column_precision is not None:
+            if dataset_spec.column_scale != 0 and dataset_spec.column_scale is not None:
+                length_details = "(" + str(dataset_spec.column_scale) + ","+str(dataset_spec.column_scale)+")"
+            else:
+                length_details = "(" + str(dataset_spec.column_scale)+ ")"
+        columns_specs.append(dataset_spec.column_name + " " + dataset_spec.column_type+length_details)
     query = Query()
 
     for num_branch in range(0,num_branches):
 
         from_tables = metadata.get_all_source_tables_from_target_table_name_and_branch(dataset.dataset_name, num_branch+1)
         # Sources and Relationships
         tables_and_relations = []
@@ -509,28 +563,29 @@
                 from_tables.remove(relations.detail_table)
 
         # SELECT Columns
         select_columns = []
         new_dataset = metadata.get_dataset_from_dataset_name(dataset.dataset_name)
         for dataset_spec in Sort_Dataset_Specification_By_Ordinal_Position([x for x in metadata.om_dataset_specification if x.end_date is None and new_dataset.id_dataset == x.id_dataset]):
             dataset_t_mapping = metadata.get_dataset_t_mapping_from_id_branch_and_id_dataset_spec(num_branch+1, dataset_spec.id_dataset_spec)
+            if dataset_t_mapping is None: continue # If the mapping on that branch has been closed
             new_select_column = dataset_t_mapping.value_mapping
             all_columns = re.findall(r'\[(\d+)\]', new_select_column)
             for col in all_columns:
                 new_select_column = new_select_column.replace("[" + col + "]",
-                                                              metadata.get_tables_dot_column_from_id_dataset_spec(
-                                                                  col))
+                                                              metadata.get_tables_dot_column_from_id_dataset_spec(col))
             new_select_column += ' AS ' + metadata.get_dataset_spec_from_id_dataset_spec(dataset_t_mapping.id_dataset_spec).column_name
             select_columns.append(new_select_column)
 
+
         # DISTINCT option
-        distinct = False
+        is_distinct = False
         for distinct in [x for x in metadata.om_dataset_t_distinct if x.end_date is None]:
             if distinct.id_dataset == dataset.id_dataset and distinct.id_branch == (num_branch+1):
-                if distinct.sw_distinct == 1: distinct = True
+                if distinct.sw_distinct == 1: is_distinct = True
 
         # ORDER Columns
         all_id_dataset_spec = metadata.get_list_id_dataset_spec_from_dataset_name(dataset.dataset_name)
         order_columns = []
         for order in [x for x in metadata.om_dataset_t_order if x.end_date is None]:
             if order.id_dataset_spec in all_id_dataset_spec and order.id_branch == (num_branch+1):
                 order_type = metadata.get_order_type_from_id_order_type(order.id_order_type)
@@ -577,39 +632,40 @@
             query.set_name_query(target_table)
             query.set_target_table(target_table)
             query.set_columns_and_specs(columns_specs)
             query.set_is_with(is_with)
             if is_with: query.set_type(QUERY_TYPE_SELECT)
             query.set_select_columns(select_columns)
             query.set_from_tables(from_tables)
-            query.set_is_distinct(distinct)
+            query.set_is_distinct(is_distinct)
             query.set_from_tables_and_relations(tables_and_relations)
             query.set_insert_columns(insert_columns)
             query.set_order_by_columns(order_columns)
             query.set_having_filters(having_filters)
             query.set_group_by_columns(agg_columns)
             query.set_primary_key(pk_columns)
             query.set_where_filters(where_filters)
         else:
+
             query_union = Query()
             query_union.set_name_query(target_table)
             query_union.set_target_table(target_table)
             query_union.set_is_with(False)
             query_union.set_select_columns(select_columns)
             query_union.set_from_tables(from_tables)
-            query.set_is_distinct(distinct)
+            query_union.set_is_distinct(is_distinct)
             query_union.set_from_tables_and_relations(tables_and_relations)
             query_union.set_order_by_columns(order_columns)
-            query.set_having_filters(having_filters)
+            query_union.set_having_filters(having_filters)
             query_union.set_group_by_columns(agg_columns)
-            query.set_primary_key(pk_columns)
+            query_union.set_primary_key(pk_columns)
             query_union.set_type(QUERY_TYPE_SELECT)
-            query.set_where_filters(where_filters)
-
-            query.add_unionquery(query_union)
+            query_union.set_where_filters(where_filters)
+            if len(select_columns) != 0:
+                query.add_unionquery(query_union)
 
 
     return query
 
 def get_node_with_with_query_execution_settings(connection, metadata, node):
     ''' Returns the node object with query execution settings configured '''
     does_table_exists = connection.does_table_exists(node.name)
```

### Comparing `Metamorf-0.3.9.1/pyproject.toml` & `Metamorf-0.4.3.1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,36 @@
 [project]
 name = "Metamorf"
-version = "0.3.9.1"
+version = "0.4.3.1"
 authors = [
   { name="Guillermo Aumatell", email="gaumatellsalom@gmail.com" },
 ]
-description = "Metadata Suite to build and control your Datawarehouse"
+description = "Metadata Suite to build and manage your Datawarehouse"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: Microsoft :: Windows",
 ]
 dependencies = [
     "snowflake-connector-python",
     "PyYAML",
-    "Flask"
+    "Flask",
+    "psycopg2",
+    "mysql-connector-python",
+    "fdb"
 ]
 
 [tool.setuptools]
-packages = ["metamorf", "metamorf.engines", "metamorf.tools", "metamorf.configuration", "metamorf.initialization", "metamorf.entry"]
-
-[tool.setuptools.package-data]
-"metamorf.configuration" = ["*.yml"]
-"metamorf.initialization" = ["*.sql"]
-"metamorf.entry" = ["*.csv"]
-"metamorf.example" = ["*.csv", "*.sql"]
+packages = ["metamorf", "metamorf.engines", "metamorf.tools"]
 
 [project.urls]
 "Homepage" = "https://github.com/gasalom/metamorf"
 "Bug Tracker" = "https://github.com/gasalom/metamorf/issues"
 
 [project.scripts]
 metamorf = "metamorf.main:main"
 
 [build-system]
-requires = ["setuptools>=61.0", "snowflake-connector-python", "fdb", "PyYAML", "Flask"]
+requires = ["setuptools>=61.0", "snowflake-connector-python", "fdb", "PyYAML", "Flask", "psycopg2"]
 build-backend = "setuptools.build_meta"
```

### Comparing `Metamorf-0.3.9.1/tests/tests.py` & `Metamorf-0.4.3.1/tests/tests.py`

 * *Files identical despite different names*

### Comparing `Metamorf-0.3.9.1/tests/tests_query.py` & `Metamorf-0.4.3.1/tests/tests_query.py`

 * *Files identical despite different names*

### Comparing `Metamorf-0.3.9.1/tests/tests_validator.py` & `Metamorf-0.4.3.1/tests/tests_validator.py`

 * *Files identical despite different names*

