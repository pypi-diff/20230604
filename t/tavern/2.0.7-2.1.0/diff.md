# Comparing `tmp/tavern-2.0.7.tar.gz` & `tmp/tavern-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tavern-2.0.7.tar", last modified: Sat Apr 15 15:36:11 2023, max compression
+gzip compressed data, was "tavern-2.1.0.tar", last modified: Sun Jun  4 10:29:00 2023, max compression
```

## Comparing `tavern-2.0.7.tar` & `tavern-2.1.0.tar`

### file list

```diff
@@ -1,188 +1,189 @@
--rw-r--r--   0        0        0     1271 2023-04-15 14:36:17.314374 tavern-2.0.7/.dockerignore
--rw-r--r--   0        0        0     2217 2023-04-15 14:36:17.314374 tavern-2.0.7/.github/workflows/main.yml
--rw-r--r--   0        0        0     1291 2023-04-15 14:36:17.314374 tavern-2.0.7/.gitignore
--rw-r--r--   0        0        0      434 2023-04-08 18:45:13.188074 tavern-2.0.7/.pre-commit-config.yaml
--rw-r--r--   0        0        0       43 2023-02-21 15:50:54.811198 tavern-2.0.7/.prettierignore
--rw-r--r--   0        0        0    16105 2023-04-15 15:35:53.610178 tavern-2.0.7/CHANGELOG.md
--rw-r--r--   0        0        0     1677 2023-04-08 18:45:13.188074 tavern-2.0.7/CONTRIBUTING.md
--rw-r--r--   0        0        0     1055 2023-02-21 15:50:54.811198 tavern-2.0.7/LICENSE
--rw-r--r--   0        0        0      111 2023-04-15 14:36:17.314374 tavern-2.0.7/MANIFEST.in
--rw-r--r--   0        0        0     8342 2023-02-21 15:50:54.811198 tavern-2.0.7/README.md
--rw-r--r--   0        0        0     5800 2023-04-15 15:35:19.443117 tavern-2.0.7/constraints.txt
--rw-r--r--   0        0        0        9 2019-12-13 13:22:50.199802 tavern-2.0.7/docs/.gitignore
--rw-r--r--   0        0        0      607 2020-04-05 16:12:15.549603 tavern-2.0.7/docs/Makefile
--rw-r--r--   0        0        0        6 2019-12-13 13:22:50.199802 tavern-2.0.7/docs/source/.gitignore
--rw-r--r--   0        0        0      851 2020-04-05 16:12:15.549603 tavern-2.0.7/docs/source/_static/favicon.png
--rw-r--r--   0        0        0     1448 2020-04-05 16:12:15.549603 tavern-2.0.7/docs/source/_static/icon.png
--rw-r--r--   0        0        0    67428 2023-02-21 15:50:54.811198 tavern-2.0.7/docs/source/basics.md
--rw-r--r--   0        0        0     5825 2023-04-15 15:35:52.443498 tavern-2.0.7/docs/source/conf.py
--rw-r--r--   0        0        0     4200 2023-02-21 15:50:54.811198 tavern-2.0.7/docs/source/cookbook.md
--rw-r--r--   0        0        0     7667 2023-02-21 15:50:54.811198 tavern-2.0.7/docs/source/debugging.md
--rw-r--r--   0        0        0     7883 2023-02-21 15:50:54.814531 tavern-2.0.7/docs/source/examples.md
--rw-r--r--   0        0        0    12310 2023-04-08 18:45:13.188074 tavern-2.0.7/docs/source/http.md
--rw-r--r--   0        0        0     1494 2023-02-21 15:50:54.814531 tavern-2.0.7/docs/source/index.md
--rw-r--r--   0        0        0     9433 2023-02-21 15:50:54.814531 tavern-2.0.7/docs/source/mqtt.md
--rw-r--r--   0        0        0    11359 2023-02-21 15:50:54.814531 tavern-2.0.7/docs/source/plugins.md
--rw-r--r--   0        0        0      130 2023-02-21 15:50:54.814531 tavern-2.0.7/docs/source/requirements.txt
--rw-r--r--   0        0        0     2895 2020-04-05 16:12:15.552937 tavern-2.0.7/docs/source/server.md
--rw-r--r--   0        0        0      213 2023-04-15 14:36:17.314374 tavern-2.0.7/example/advanced/Dockerfile
--rw-r--r--   0        0        0      401 2021-09-25 13:51:36.584969 tavern-2.0.7/example/advanced/advanced.md
--rw-r--r--   0        0        0      149 2021-09-25 13:51:36.584969 tavern-2.0.7/example/advanced/common.yaml
--rw-r--r--   0        0        0      126 2023-04-15 14:36:17.314374 tavern-2.0.7/example/advanced/docker-compose.yaml
--rw-r--r--   0        0        0     3552 2023-04-15 14:36:17.314374 tavern-2.0.7/example/advanced/server.py
--rw-r--r--   0        0        0     4046 2023-02-21 15:50:54.814531 tavern-2.0.7/example/advanced/test_server.tavern.yaml
--rw-r--r--   0        0        0      673 2023-02-21 15:50:54.814531 tavern-2.0.7/example/advanced/testing_utils.py
--rw-r--r--   0        0        0      210 2023-04-15 14:36:17.314374 tavern-2.0.7/example/components/Dockerfile
--rw-r--r--   0        0        0      168 2021-09-25 13:51:36.584969 tavern-2.0.7/example/components/common.yaml
--rw-r--r--   0        0        0      717 2021-09-25 13:51:36.584969 tavern-2.0.7/example/components/components.md
--rw-r--r--   0        0        0      594 2021-09-25 13:51:36.584969 tavern-2.0.7/example/components/components/auth_stage.yaml
--rw-r--r--   0        0        0      126 2023-04-15 14:36:17.314374 tavern-2.0.7/example/components/docker-compose.yaml
--rw-r--r--   0        0        0     1642 2023-04-15 14:36:17.314374 tavern-2.0.7/example/components/server.py
--rw-r--r--   0        0        0      633 2021-09-25 13:51:36.584969 tavern-2.0.7/example/components/test_hello.tavern.yaml
--rw-r--r--   0        0        0      612 2021-09-25 13:51:36.584969 tavern-2.0.7/example/components/test_ping.tavern.yaml
--rw-r--r--   0        0        0      195 2023-04-15 14:36:17.314374 tavern-2.0.7/example/cookies/Dockerfile
--rw-r--r--   0        0        0      117 2021-09-25 13:51:36.584969 tavern-2.0.7/example/cookies/common.yaml
--rw-r--r--   0        0        0      147 2021-09-25 13:51:36.584969 tavern-2.0.7/example/cookies/cookies.md
--rw-r--r--   0        0        0      126 2023-04-15 14:36:17.314374 tavern-2.0.7/example/cookies/docker-compose.yaml
--rw-r--r--   0        0        0     2964 2023-04-15 14:36:17.314374 tavern-2.0.7/example/cookies/server.py
--rw-r--r--   0        0        0     3245 2021-09-25 13:51:36.584969 tavern-2.0.7/example/cookies/test_server.tavern.yaml
--rw-r--r--   0        0        0      202 2020-04-05 16:12:15.552937 tavern-2.0.7/example/generate_from_openapi/Pipfile
--rw-r--r--   0        0        0    13687 2023-02-21 15:50:54.814531 tavern-2.0.7/example/generate_from_openapi/Pipfile.lock
--rw-r--r--   0        0        0     2101 2022-08-06 15:34:31.364607 tavern-2.0.7/example/generate_from_openapi/pub_tavern.py
--rw-r--r--   0        0        0      144 2020-04-05 16:12:15.552937 tavern-2.0.7/example/generate_from_openapi/readme.md
--rw-r--r--   0        0        0      566 2020-04-05 16:12:15.552937 tavern-2.0.7/example/generate_from_openapi/test_example_output.tavern.yaml
--rw-r--r--   0        0        0      195 2023-04-15 14:36:17.314374 tavern-2.0.7/example/hooks/Dockerfile
--rw-r--r--   0        0        0      990 2022-08-06 15:34:31.364607 tavern-2.0.7/example/hooks/conftest.py
--rw-r--r--   0        0        0      126 2023-04-15 14:36:17.314374 tavern-2.0.7/example/hooks/docker-compose.yaml
--rw-r--r--   0        0        0      465 2023-04-15 14:36:17.314374 tavern-2.0.7/example/hooks/server.py
--rw-r--r--   0        0        0      620 2023-02-21 15:50:54.814531 tavern-2.0.7/example/hooks/test_server.tavern.yaml
--rw-r--r--   0        0        0      844 2020-04-05 16:12:15.556270 tavern-2.0.7/example/mqtt/README.md
--rw-r--r--   0        0        0      158 2020-04-05 16:12:15.556270 tavern-2.0.7/example/mqtt/common.yaml
--rw-r--r--   0        0        0     2600 2023-04-08 18:45:13.188074 tavern-2.0.7/example/mqtt/conftest.py
--rw-r--r--   0        0        0      984 2023-04-15 14:36:17.314374 tavern-2.0.7/example/mqtt/docker-compose.yaml
--rw-r--r--   0        0        0      135 2020-04-05 16:12:15.556270 tavern-2.0.7/example/mqtt/fluent.conf
--rw-r--r--   0        0        0      158 2023-04-15 14:36:17.314374 tavern-2.0.7/example/mqtt/listener.Dockerfile
--rw-r--r--   0        0        0     4863 2023-04-15 15:04:25.003592 tavern-2.0.7/example/mqtt/listener.py
--rw-r--r--   0        0        0      169 2023-04-08 18:45:13.188074 tavern-2.0.7/example/mqtt/mosquitto.conf
--rw-r--r--   0        0        0      120 2023-04-08 18:45:13.188074 tavern-2.0.7/example/mqtt/mosquitto_passwd
--rw-r--r--   0        0        0      393 2023-04-15 14:36:17.314374 tavern-2.0.7/example/mqtt/server.Dockerfile
--rw-r--r--   0        0        0     4707 2023-04-15 15:04:25.003592 tavern-2.0.7/example/mqtt/server.py
--rw-r--r--   0        0        0    15165 2023-04-15 15:04:25.003592 tavern-2.0.7/example/mqtt/test_mqtt.tavern.yaml
--rw-r--r--   0        0        0     3381 2023-04-15 15:04:25.003592 tavern-2.0.7/example/mqtt/test_mqtt_failures.tavern.yaml
--rw-r--r--   0        0        0      193 2023-04-08 18:45:13.188074 tavern-2.0.7/example/mqtt/testing_utils.py
--rw-r--r--   0        0        0     1167 2021-09-25 13:51:36.584969 tavern-2.0.7/example/simple/running_tests.md
--rw-r--r--   0        0        0      465 2023-04-15 14:36:17.314374 tavern-2.0.7/example/simple/server.py
--rw-r--r--   0        0        0     1996 2021-09-25 13:51:36.584969 tavern-2.0.7/example/simple/test_server.tavern.yaml
--rw-r--r--   0        0        0     4038 2023-04-15 15:35:52.443498 tavern-2.0.7/pyproject.toml
--rw-r--r--   0        0        0    57165 2023-04-15 15:35:19.443117 tavern-2.0.7/requirements.txt
--rwxr-xr-x   0        0        0      222 2023-02-21 15:50:54.814531 tavern-2.0.7/scripts/coverage.sh
--rwxr-xr-x   0        0        0      407 2023-02-21 15:50:54.814531 tavern-2.0.7/scripts/release.sh
--rwxr-xr-x   0        0        0      374 2023-04-08 18:45:13.188074 tavern-2.0.7/scripts/smoke.bash
--rwxr-xr-x   0        0        0      616 2023-02-21 15:50:54.814531 tavern-2.0.7/scripts/update-changelog.bash
--rw-r--r--   0        0        0       99 2023-04-15 15:35:52.443498 tavern-2.0.7/tavern/__init__.py
--rw-r--r--   0        0        0        0 2023-02-21 16:06:58.930000 tavern-2.0.7/tavern/_core/__init__.py
--rw-r--r--   0        0        0    19780 2023-04-08 18:45:13.188074 tavern-2.0.7/tavern/_core/dict_util.py
--rw-r--r--   0        0        0     3842 2023-04-08 18:45:13.188074 tavern-2.0.7/tavern/_core/exceptions.py
--rw-r--r--   0        0        0     4737 2023-04-08 18:45:13.188074 tavern-2.0.7/tavern/_core/extfunctions.py
--rw-r--r--   0        0        0       96 2023-02-21 15:50:54.814531 tavern-2.0.7/tavern/_core/formatted_str.py
--rw-r--r--   0        0        0      951 2023-04-08 18:45:13.188074 tavern-2.0.7/tavern/_core/general.py
--rw-r--r--   0        0        0     2612 2023-04-08 18:45:13.188074 tavern-2.0.7/tavern/_core/jmesutils.py
--rw-r--r--   0        0        0    12257 2023-04-08 18:45:13.188074 tavern-2.0.7/tavern/_core/loader.py
--rw-r--r--   0        0        0     9200 2023-04-15 14:36:17.314374 tavern-2.0.7/tavern/_core/plugins.py
--rw-r--r--   0        0        0      275 2023-02-21 15:50:54.814531 tavern-2.0.7/tavern/_core/pytest/__init__.py
--rw-r--r--   0        0        0     1617 2023-04-15 14:36:17.314374 tavern-2.0.7/tavern/_core/pytest/config.py
--rw-r--r--   0        0        0     7393 2023-04-08 18:45:13.188074 tavern-2.0.7/tavern/_core/pytest/error.py
--rw-r--r--   0        0        0    13187 2023-04-15 14:36:17.314374 tavern-2.0.7/tavern/_core/pytest/file.py
--rw-r--r--   0        0        0     1471 2023-04-15 15:35:15.079734 tavern-2.0.7/tavern/_core/pytest/hooks.py
--rw-r--r--   0        0        0     9469 2023-04-15 15:35:15.079734 tavern-2.0.7/tavern/_core/pytest/item.py
--rw-r--r--   0        0        0     2101 2023-04-08 18:45:13.188074 tavern-2.0.7/tavern/_core/pytest/newhooks.py
--rw-r--r--   0        0        0     5941 2023-04-15 15:35:15.079734 tavern-2.0.7/tavern/_core/pytest/util.py
--rw-r--r--   0        0        0     1833 2023-04-08 18:45:13.188074 tavern-2.0.7/tavern/_core/report.py
--rw-r--r--   0        0        0    10800 2023-04-15 14:36:17.314374 tavern-2.0.7/tavern/_core/run.py
--rw-r--r--   0        0        0        0 2023-02-21 16:06:58.930081 tavern-2.0.7/tavern/_core/schema/__init__.py
--rw-r--r--   0        0        0    14523 2023-04-15 14:36:17.314374 tavern-2.0.7/tavern/_core/schema/extensions.py
--rw-r--r--   0        0        0     4350 2023-04-08 18:45:13.188074 tavern-2.0.7/tavern/_core/schema/files.py
--rw-r--r--   0        0        0     6245 2023-04-08 18:45:13.188074 tavern-2.0.7/tavern/_core/schema/jsonschema.py
--rw-r--r--   0        0        0     9057 2023-04-08 18:45:13.188074 tavern-2.0.7/tavern/_core/schema/tests.jsonschema.yaml
--rw-r--r--   0        0        0     6845 2023-04-08 18:44:26.927400 tavern-2.0.7/tavern/_core/schema/tests.schema.yaml
--rw-r--r--   0        0        0     1100 2023-02-21 15:50:54.817865 tavern-2.0.7/tavern/_core/stage_lines.py
--rw-r--r--   0        0        0     5171 2023-04-08 18:45:13.188074 tavern-2.0.7/tavern/_core/strict_util.py
--rw-r--r--   0        0        0      383 2023-04-08 18:45:13.188074 tavern-2.0.7/tavern/_core/strtobool.py
--rw-r--r--   0        0        0     3958 2023-04-15 14:36:17.314374 tavern-2.0.7/tavern/_core/testhelpers.py
--rw-r--r--   0        0        0        0 2023-02-21 16:06:58.930000 tavern-2.0.7/tavern/_plugins/__init__.py
--rw-r--r--   0        0        0        0 2023-02-21 16:06:58.930000 tavern-2.0.7/tavern/_plugins/mqtt/__init__.py
--rw-r--r--   0        0        0    17697 2023-04-08 18:45:13.188074 tavern-2.0.7/tavern/_plugins/mqtt/client.py
--rw-r--r--   0        0        0     4013 2023-02-21 15:50:54.817865 tavern-2.0.7/tavern/_plugins/mqtt/jsonschema.yaml
--rw-r--r--   0        0        0     2523 2023-04-15 14:36:17.317707 tavern-2.0.7/tavern/_plugins/mqtt/request.py
--rw-r--r--   0        0        0    11430 2023-04-15 15:04:25.003592 tavern-2.0.7/tavern/_plugins/mqtt/response.py
--rw-r--r--   0        0        0     3233 2023-02-21 15:50:54.817865 tavern-2.0.7/tavern/_plugins/mqtt/schema.yaml
--rw-r--r--   0        0        0     1267 2023-04-02 13:10:37.687090 tavern-2.0.7/tavern/_plugins/mqtt/tavernhook.py
--rw-r--r--   0        0        0        0 2023-02-21 16:06:58.930000 tavern-2.0.7/tavern/_plugins/rest/__init__.py
--rw-r--r--   0        0        0    19370 2023-04-15 14:36:17.317707 tavern-2.0.7/tavern/_plugins/rest/request.py
--rw-r--r--   0        0        0     8291 2023-04-08 18:45:13.188074 tavern-2.0.7/tavern/_plugins/rest/response.py
--rw-r--r--   0        0        0      860 2023-04-08 18:45:13.188074 tavern-2.0.7/tavern/_plugins/rest/tavernhook.py
--rw-r--r--   0        0        0     2969 2023-04-08 18:45:13.188074 tavern-2.0.7/tavern/core.py
--rw-r--r--   0        0        0     2739 2023-04-08 18:45:13.188074 tavern-2.0.7/tavern/entry.py
--rw-r--r--   0        0        0     7575 2023-04-08 18:45:13.188074 tavern-2.0.7/tavern/helpers.py
--rw-r--r--   0        0        0      466 2023-04-08 18:45:13.188074 tavern-2.0.7/tavern/request.py
--rw-r--r--   0        0        0     9571 2023-04-15 14:36:17.317707 tavern-2.0.7/tavern/response.py
--rw-r--r--   0        0        0      919 2023-04-02 12:34:26.285355 tavern-2.0.7/tests/conftest.py
--rw-r--r--   0        0        0      195 2023-04-15 14:36:17.317707 tavern-2.0.7/tests/integration/Dockerfile
--rw-r--r--   0        0        0       33 2023-02-21 15:50:54.817865 tavern-2.0.7/tests/integration/OK.json.gz
--rw-r--r--   0        0        0        3 2020-12-19 13:25:29.031794 tavern-2.0.7/tests/integration/OK.txt
--rw-r--r--   0        0        0      504 2021-09-25 13:51:36.591636 tavern-2.0.7/tests/integration/README.md
--rw-r--r--   0        0        0      608 2022-02-25 15:36:43.966205 tavern-2.0.7/tests/integration/common.yaml
--rw-r--r--   0        0        0      621 2023-04-08 18:45:13.191407 tavern-2.0.7/tests/integration/conftest.py
--rw-r--r--   0        0        0      126 2023-04-15 14:36:17.317707 tavern-2.0.7/tests/integration/docker-compose.yaml
--rw-r--r--   0        0        0      167 2023-02-21 15:50:54.817865 tavern-2.0.7/tests/integration/ext_functions.py
--rw-r--r--   0        0        0      203 2020-04-05 16:12:15.572937 tavern-2.0.7/tests/integration/extra.yaml
--rw-r--r--   0        0        0      254 2021-05-01 10:23:38.259754 tavern-2.0.7/tests/integration/global_cfg.yaml
--rw-r--r--   0        0        0       91 2021-03-07 14:36:40.846310 tavern-2.0.7/tests/integration/parametrize_includes.yaml
--rw-r--r--   0        0        0    11475 2023-04-15 14:36:17.317707 tavern-2.0.7/tests/integration/server.py
--rw-r--r--   0        0        0      297 2023-02-21 15:50:54.817865 tavern-2.0.7/tests/integration/test_allure.tavern.yaml
--rw-r--r--   0        0        0      659 2023-02-21 15:50:54.817865 tavern-2.0.7/tests/integration/test_auth_key.tavern.yaml
--rw-r--r--   0        0        0      624 2023-02-21 15:50:54.817865 tavern-2.0.7/tests/integration/test_certs.tavern.yaml
--rw-r--r--   0        0        0     1569 2023-02-21 15:50:54.817865 tavern-2.0.7/tests/integration/test_cookie_remember.tavern.yaml
--rw-r--r--   0        0        0     6106 2021-12-20 17:04:04.340877 tavern-2.0.7/tests/integration/test_cookies.tavern.yaml
--rw-r--r--   0        0        0     2448 2023-02-21 15:50:54.817865 tavern-2.0.7/tests/integration/test_data_key.tavern.yaml
--rw-r--r--   0        0        0       29 2022-08-06 15:34:18.544082 tavern-2.0.7/tests/integration/test_dummy.py
--rw-r--r--   0        0        0      331 2023-02-21 15:50:54.817865 tavern-2.0.7/tests/integration/test_env_var_format.tavern.yaml
--rw-r--r--   0        0        0      277 2023-02-21 15:50:54.817865 tavern-2.0.7/tests/integration/test_error.tavern.yaml
--rw-r--r--   0        0        0     3152 2023-02-21 15:50:54.817865 tavern-2.0.7/tests/integration/test_external_functions.tavern.yaml
--rw-r--r--   0        0        0     4086 2023-04-15 14:36:17.317707 tavern-2.0.7/tests/integration/test_files.tavern.yaml
--rw-r--r--   0        0        0     2398 2023-02-21 15:50:54.817865 tavern-2.0.7/tests/integration/test_fixtures.tavern.yaml
--rw-r--r--   0        0        0      799 2023-02-21 15:50:54.817865 tavern-2.0.7/tests/integration/test_follow_redirects.tavern.yaml
--rw-r--r--   0        0        0     1028 2023-02-21 15:50:54.817865 tavern-2.0.7/tests/integration/test_header_comparisons.tavern.yaml
--rw-r--r--   0        0        0     1269 2023-02-21 15:50:54.817865 tavern-2.0.7/tests/integration/test_helpers.tavern.yaml
--rw-r--r--   0        0        0     4837 2023-02-21 15:50:54.817865 tavern-2.0.7/tests/integration/test_jmes.tavern.yaml
--rw-r--r--   0        0        0      750 2023-02-21 15:50:54.817865 tavern-2.0.7/tests/integration/test_minimal.tavern.yaml
--rw-r--r--   0        0        0    14838 2023-02-21 15:50:54.817865 tavern-2.0.7/tests/integration/test_parametrize.tavern.yaml
--rw-r--r--   0        0        0     2167 2023-02-21 15:50:54.817865 tavern-2.0.7/tests/integration/test_regex.tavern.yaml
--rw-r--r--   0        0        0     2031 2023-02-21 15:50:54.817865 tavern-2.0.7/tests/integration/test_response_types.tavern.yaml
--rw-r--r--   0        0        0     2372 2023-02-21 15:50:54.817865 tavern-2.0.7/tests/integration/test_retry.tavern.yaml
--rw-r--r--   0        0        0      575 2023-02-21 15:50:54.817865 tavern-2.0.7/tests/integration/test_save_dict_value.tavern.yaml
--rw-r--r--   0        0        0      970 2023-02-21 15:50:54.817865 tavern-2.0.7/tests/integration/test_selective_tests.tavern.yaml
--rw-r--r--   0        0        0     2432 2023-02-21 15:50:54.817865 tavern-2.0.7/tests/integration/test_skipped_tests.tavern.yaml
--rw-r--r--   0        0        0     1506 2023-02-21 15:50:54.817865 tavern-2.0.7/tests/integration/test_status_codes.tavern.yaml
--rw-r--r--   0        0        0      235 2023-02-21 15:50:54.817865 tavern-2.0.7/tests/integration/test_stream.tavern.yaml
--rw-r--r--   0        0        0    10926 2023-02-21 15:50:54.817865 tavern-2.0.7/tests/integration/test_strict_key_checks.tavern.yaml
--rw-r--r--   0        0        0     1951 2023-02-21 15:50:54.817865 tavern-2.0.7/tests/integration/test_timeout.tavern.yaml
--rw-r--r--   0        0        0    12933 2023-04-08 18:45:13.191407 tavern-2.0.7/tests/integration/test_typetokens.tavern.yaml
--rw-r--r--   0        0        0     1415 2023-02-21 15:50:54.817865 tavern-2.0.7/tests/integration/test_validate_pykwalify.tavern.yaml
--rw-r--r--   0        0        0        0 2020-04-05 16:12:15.572937 tavern-2.0.7/tests/integration/testfile.txt
--rw-r--r--   0        0        0      650 2023-02-21 15:50:54.817865 tavern-2.0.7/tests/logging.yaml
--rw-r--r--   0        0        0      915 2023-04-15 14:36:17.317707 tavern-2.0.7/tests/unit/conftest.py
--rw-r--r--   0        0        0     9612 2023-04-08 18:45:13.191407 tavern-2.0.7/tests/unit/response/test_mqtt_response.py
--rw-r--r--   0        0        0    12296 2023-02-21 15:50:54.817865 tavern-2.0.7/tests/unit/response/test_rest.py
--rw-r--r--   0        0        0     1483 2023-04-08 18:44:26.930733 tavern-2.0.7/tests/unit/test_call_run.py
--rw-r--r--   0        0        0    16186 2023-04-09 16:32:29.620833 tavern-2.0.7/tests/unit/test_core.py
--rw-r--r--   0        0        0    14289 2023-04-15 14:36:17.317707 tavern-2.0.7/tests/unit/test_helpers.py
--rw-r--r--   0        0        0     7161 2023-04-08 18:45:13.191407 tavern-2.0.7/tests/unit/test_mqtt.py
--rw-r--r--   0        0        0     5791 2023-04-08 18:45:13.191407 tavern-2.0.7/tests/unit/test_pytest_hooks.py
--rw-r--r--   0        0        0    14990 2023-04-08 18:45:13.191407 tavern-2.0.7/tests/unit/test_request.py
--rw-r--r--   0        0        0     6131 2023-04-15 14:36:17.317707 tavern-2.0.7/tests/unit/test_schema.py
--rw-r--r--   0        0        0     1030 2023-02-21 15:50:54.817865 tavern-2.0.7/tests/unit/test_strict_util.py
--rw-r--r--   0        0        0    14898 2023-04-08 18:45:13.191407 tavern-2.0.7/tests/unit/test_utilities.py
--rw-r--r--   0        0        0     2434 2023-04-08 18:44:26.930733 tavern-2.0.7/tox-integration.ini
--rw-r--r--   0        0        0      625 2023-04-15 14:36:17.317707 tavern-2.0.7/tox.ini
--rw-r--r--   0        0        0    10617 1970-01-01 00:00:00.000000 tavern-2.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1271 2023-06-04 10:17:30.497109 tavern-2.1.0/.dockerignore
+-rw-r--r--   0        0        0     2217 2023-06-04 10:17:30.497109 tavern-2.1.0/.github/workflows/main.yml
+-rw-r--r--   0        0        0     1291 2023-06-04 10:17:30.497109 tavern-2.1.0/.gitignore
+-rw-r--r--   0        0        0      434 2023-06-04 10:25:13.431284 tavern-2.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       43 2023-06-04 10:17:30.497109 tavern-2.1.0/.prettierignore
+-rw-r--r--   0        0        0    16049 2023-06-04 10:25:17.324625 tavern-2.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1677 2023-06-04 10:17:30.497109 tavern-2.1.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1055 2023-06-04 10:17:30.497109 tavern-2.1.0/LICENSE
+-rw-r--r--   0        0        0      111 2023-06-04 10:17:30.497109 tavern-2.1.0/MANIFEST.in
+-rw-r--r--   0        0        0     8342 2023-06-04 10:17:30.497109 tavern-2.1.0/README.md
+-rw-r--r--   0        0        0     5936 2023-06-04 10:21:02.460826 tavern-2.1.0/constraints.txt
+-rw-r--r--   0        0        0        9 2023-06-04 10:17:30.497109 tavern-2.1.0/docs/.gitignore
+-rw-r--r--   0        0        0      607 2023-06-04 10:17:30.497109 tavern-2.1.0/docs/Makefile
+-rw-r--r--   0        0        0        6 2023-06-04 10:17:30.497109 tavern-2.1.0/docs/source/.gitignore
+-rw-r--r--   0        0        0      851 2023-06-04 10:17:30.497109 tavern-2.1.0/docs/source/_static/favicon.png
+-rw-r--r--   0        0        0     1448 2023-06-04 10:17:30.497109 tavern-2.1.0/docs/source/_static/icon.png
+-rw-r--r--   0        0        0    67428 2023-06-04 10:17:30.497109 tavern-2.1.0/docs/source/basics.md
+-rw-r--r--   0        0        0     5825 2023-06-04 10:25:16.227956 tavern-2.1.0/docs/source/conf.py
+-rw-r--r--   0        0        0     4200 2023-06-04 10:17:30.497109 tavern-2.1.0/docs/source/cookbook.md
+-rw-r--r--   0        0        0     7667 2023-06-04 10:17:30.497109 tavern-2.1.0/docs/source/debugging.md
+-rw-r--r--   0        0        0     7883 2023-06-04 10:17:30.497109 tavern-2.1.0/docs/source/examples.md
+-rw-r--r--   0        0        0    12310 2023-06-04 10:17:30.497109 tavern-2.1.0/docs/source/http.md
+-rw-r--r--   0        0        0     1494 2023-06-04 10:17:30.497109 tavern-2.1.0/docs/source/index.md
+-rw-r--r--   0        0        0     9433 2023-06-04 10:17:30.497109 tavern-2.1.0/docs/source/mqtt.md
+-rw-r--r--   0        0        0    11359 2023-06-04 10:17:30.497109 tavern-2.1.0/docs/source/plugins.md
+-rw-r--r--   0        0        0      130 2023-06-04 10:17:30.497109 tavern-2.1.0/docs/source/requirements.txt
+-rw-r--r--   0        0        0     2895 2023-06-04 10:17:30.497109 tavern-2.1.0/docs/source/server.md
+-rw-r--r--   0        0        0      213 2023-06-04 10:17:30.497109 tavern-2.1.0/example/advanced/Dockerfile
+-rw-r--r--   0        0        0      401 2023-06-04 10:17:30.497109 tavern-2.1.0/example/advanced/advanced.md
+-rw-r--r--   0        0        0      149 2023-06-04 10:17:30.497109 tavern-2.1.0/example/advanced/common.yaml
+-rw-r--r--   0        0        0      126 2023-06-04 10:17:30.497109 tavern-2.1.0/example/advanced/docker-compose.yaml
+-rw-r--r--   0        0        0     3552 2023-06-04 10:17:30.497109 tavern-2.1.0/example/advanced/server.py
+-rw-r--r--   0        0        0     4046 2023-06-04 10:17:30.497109 tavern-2.1.0/example/advanced/test_server.tavern.yaml
+-rw-r--r--   0        0        0      673 2023-06-04 10:17:30.497109 tavern-2.1.0/example/advanced/testing_utils.py
+-rw-r--r--   0        0        0      210 2023-06-04 10:17:30.497109 tavern-2.1.0/example/components/Dockerfile
+-rw-r--r--   0        0        0      168 2023-06-04 10:17:30.497109 tavern-2.1.0/example/components/common.yaml
+-rw-r--r--   0        0        0      717 2023-06-04 10:17:30.497109 tavern-2.1.0/example/components/components.md
+-rw-r--r--   0        0        0      594 2023-06-04 10:17:30.500442 tavern-2.1.0/example/components/components/auth_stage.yaml
+-rw-r--r--   0        0        0      126 2023-06-04 10:17:30.500442 tavern-2.1.0/example/components/docker-compose.yaml
+-rw-r--r--   0        0        0     1642 2023-06-04 10:17:30.500442 tavern-2.1.0/example/components/server.py
+-rw-r--r--   0        0        0      633 2023-06-04 10:17:30.500442 tavern-2.1.0/example/components/test_hello.tavern.yaml
+-rw-r--r--   0        0        0      612 2023-06-04 10:17:30.500442 tavern-2.1.0/example/components/test_ping.tavern.yaml
+-rw-r--r--   0        0        0      195 2023-06-04 10:17:30.500442 tavern-2.1.0/example/cookies/Dockerfile
+-rw-r--r--   0        0        0      117 2023-06-04 10:17:30.500442 tavern-2.1.0/example/cookies/common.yaml
+-rw-r--r--   0        0        0      147 2023-06-04 10:17:30.500442 tavern-2.1.0/example/cookies/cookies.md
+-rw-r--r--   0        0        0      126 2023-06-04 10:17:30.500442 tavern-2.1.0/example/cookies/docker-compose.yaml
+-rw-r--r--   0        0        0     2964 2023-06-04 10:17:30.500442 tavern-2.1.0/example/cookies/server.py
+-rw-r--r--   0        0        0     3245 2023-06-04 10:17:30.500442 tavern-2.1.0/example/cookies/test_server.tavern.yaml
+-rw-r--r--   0        0        0      202 2023-06-04 10:17:30.500442 tavern-2.1.0/example/generate_from_openapi/Pipfile
+-rw-r--r--   0        0        0    13687 2023-06-04 10:17:30.500442 tavern-2.1.0/example/generate_from_openapi/Pipfile.lock
+-rw-r--r--   0        0        0     2101 2023-06-04 10:17:30.500442 tavern-2.1.0/example/generate_from_openapi/pub_tavern.py
+-rw-r--r--   0        0        0      144 2023-06-04 10:17:30.500442 tavern-2.1.0/example/generate_from_openapi/readme.md
+-rw-r--r--   0        0        0      566 2023-06-04 10:17:30.500442 tavern-2.1.0/example/generate_from_openapi/test_example_output.tavern.yaml
+-rw-r--r--   0        0        0      195 2023-06-04 10:17:30.500442 tavern-2.1.0/example/hooks/Dockerfile
+-rw-r--r--   0        0        0      990 2023-06-04 10:17:30.500442 tavern-2.1.0/example/hooks/conftest.py
+-rw-r--r--   0        0        0      126 2023-06-04 10:17:30.500442 tavern-2.1.0/example/hooks/docker-compose.yaml
+-rw-r--r--   0        0        0      465 2023-06-04 10:17:30.500442 tavern-2.1.0/example/hooks/server.py
+-rw-r--r--   0        0        0      620 2023-06-04 10:17:30.500442 tavern-2.1.0/example/hooks/test_server.tavern.yaml
+-rw-r--r--   0        0        0      844 2023-06-04 10:17:30.500442 tavern-2.1.0/example/mqtt/README.md
+-rw-r--r--   0        0        0      158 2023-06-04 10:17:30.500442 tavern-2.1.0/example/mqtt/common.yaml
+-rw-r--r--   0        0        0     2600 2023-06-04 10:17:30.500442 tavern-2.1.0/example/mqtt/conftest.py
+-rw-r--r--   0        0        0      984 2023-06-04 10:17:30.500442 tavern-2.1.0/example/mqtt/docker-compose.yaml
+-rw-r--r--   0        0        0      135 2023-06-04 10:17:30.500442 tavern-2.1.0/example/mqtt/fluent.conf
+-rw-r--r--   0        0        0      158 2023-06-04 10:17:30.500442 tavern-2.1.0/example/mqtt/listener.Dockerfile
+-rw-r--r--   0        0        0     4863 2023-06-04 10:17:30.500442 tavern-2.1.0/example/mqtt/listener.py
+-rw-r--r--   0        0        0      169 2023-06-04 10:17:30.500442 tavern-2.1.0/example/mqtt/mosquitto.conf
+-rw-r--r--   0        0        0      120 2023-06-04 10:17:30.500442 tavern-2.1.0/example/mqtt/mosquitto_passwd
+-rw-r--r--   0        0        0      393 2023-06-04 10:17:30.500442 tavern-2.1.0/example/mqtt/server.Dockerfile
+-rw-r--r--   0        0        0     4701 2023-06-04 10:17:30.500442 tavern-2.1.0/example/mqtt/server.py
+-rw-r--r--   0        0        0    15165 2023-06-04 10:17:30.500442 tavern-2.1.0/example/mqtt/test_mqtt.tavern.yaml
+-rw-r--r--   0        0        0     3381 2023-06-04 10:17:30.500442 tavern-2.1.0/example/mqtt/test_mqtt_failures.tavern.yaml
+-rw-r--r--   0        0        0      193 2023-06-04 10:17:30.500442 tavern-2.1.0/example/mqtt/testing_utils.py
+-rw-r--r--   0        0        0     1167 2023-06-04 10:17:30.500442 tavern-2.1.0/example/simple/running_tests.md
+-rw-r--r--   0        0        0      465 2023-06-04 10:17:30.500442 tavern-2.1.0/example/simple/server.py
+-rw-r--r--   0        0        0     1996 2023-06-04 10:17:30.500442 tavern-2.1.0/example/simple/test_server.tavern.yaml
+-rw-r--r--   0        0        0     4109 2023-06-04 10:25:16.227956 tavern-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0    57811 2023-06-04 10:20:52.517475 tavern-2.1.0/requirements.txt
+-rwxr-xr-x   0        0        0      222 2023-06-04 10:17:30.500442 tavern-2.1.0/scripts/coverage.sh
+-rwxr-xr-x   0        0        0      407 2023-06-04 10:17:30.500442 tavern-2.1.0/scripts/release.sh
+-rwxr-xr-x   0        0        0      405 2023-06-04 10:17:30.500442 tavern-2.1.0/scripts/smoke.bash
+-rwxr-xr-x   0        0        0      616 2023-06-04 10:17:30.500442 tavern-2.1.0/scripts/update-changelog.bash
+-rw-r--r--   0        0        0       99 2023-06-04 10:25:16.227956 tavern-2.1.0/tavern/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:17:30.500442 tavern-2.1.0/tavern/_core/__init__.py
+-rw-r--r--   0        0        0    19780 2023-06-04 10:17:30.500442 tavern-2.1.0/tavern/_core/dict_util.py
+-rw-r--r--   0        0        0     3842 2023-06-04 10:17:30.500442 tavern-2.1.0/tavern/_core/exceptions.py
+-rw-r--r--   0        0        0     4737 2023-06-04 10:17:30.500442 tavern-2.1.0/tavern/_core/extfunctions.py
+-rw-r--r--   0        0        0       96 2023-06-04 10:17:30.500442 tavern-2.1.0/tavern/_core/formatted_str.py
+-rw-r--r--   0        0        0      951 2023-06-04 10:17:30.500442 tavern-2.1.0/tavern/_core/general.py
+-rw-r--r--   0        0        0     2612 2023-06-04 10:17:30.500442 tavern-2.1.0/tavern/_core/jmesutils.py
+-rw-r--r--   0        0        0    12257 2023-06-04 10:17:30.500442 tavern-2.1.0/tavern/_core/loader.py
+-rw-r--r--   0        0        0     9200 2023-06-04 10:17:30.500442 tavern-2.1.0/tavern/_core/plugins.py
+-rw-r--r--   0        0        0      275 2023-06-04 10:17:30.500442 tavern-2.1.0/tavern/_core/pytest/__init__.py
+-rw-r--r--   0        0        0     1617 2023-06-04 10:17:30.500442 tavern-2.1.0/tavern/_core/pytest/config.py
+-rw-r--r--   0        0        0     7393 2023-06-04 10:17:30.500442 tavern-2.1.0/tavern/_core/pytest/error.py
+-rw-r--r--   0        0        0    13187 2023-06-04 10:17:30.500442 tavern-2.1.0/tavern/_core/pytest/file.py
+-rw-r--r--   0        0        0     1471 2023-06-04 10:17:30.500442 tavern-2.1.0/tavern/_core/pytest/hooks.py
+-rw-r--r--   0        0        0     9469 2023-06-04 10:17:30.500442 tavern-2.1.0/tavern/_core/pytest/item.py
+-rw-r--r--   0        0        0     2101 2023-06-04 10:17:30.500442 tavern-2.1.0/tavern/_core/pytest/newhooks.py
+-rw-r--r--   0        0        0     5941 2023-06-04 10:17:30.500442 tavern-2.1.0/tavern/_core/pytest/util.py
+-rw-r--r--   0        0        0     1833 2023-06-04 10:17:30.500442 tavern-2.1.0/tavern/_core/report.py
+-rw-r--r--   0        0        0    10800 2023-06-04 10:17:30.500442 tavern-2.1.0/tavern/_core/run.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:17:30.500442 tavern-2.1.0/tavern/_core/schema/__init__.py
+-rw-r--r--   0        0        0    14810 2023-06-04 10:17:30.500442 tavern-2.1.0/tavern/_core/schema/extensions.py
+-rw-r--r--   0        0        0     4350 2023-06-04 10:17:30.500442 tavern-2.1.0/tavern/_core/schema/files.py
+-rw-r--r--   0        0        0     6245 2023-06-04 10:17:30.500442 tavern-2.1.0/tavern/_core/schema/jsonschema.py
+-rw-r--r--   0        0        0     9100 2023-06-04 10:17:30.500442 tavern-2.1.0/tavern/_core/schema/tests.jsonschema.yaml
+-rw-r--r--   0        0        0     6845 2023-06-04 10:17:30.500442 tavern-2.1.0/tavern/_core/schema/tests.schema.yaml
+-rw-r--r--   0        0        0     1100 2023-06-04 10:17:30.500442 tavern-2.1.0/tavern/_core/stage_lines.py
+-rw-r--r--   0        0        0     5171 2023-06-04 10:17:30.500442 tavern-2.1.0/tavern/_core/strict_util.py
+-rw-r--r--   0        0        0      383 2023-06-04 10:17:30.500442 tavern-2.1.0/tavern/_core/strtobool.py
+-rw-r--r--   0        0        0     3958 2023-06-04 10:17:30.500442 tavern-2.1.0/tavern/_core/testhelpers.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:17:30.500442 tavern-2.1.0/tavern/_plugins/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:17:30.500442 tavern-2.1.0/tavern/_plugins/mqtt/__init__.py
+-rw-r--r--   0        0        0    17697 2023-06-04 10:17:30.500442 tavern-2.1.0/tavern/_plugins/mqtt/client.py
+-rw-r--r--   0        0        0     4013 2023-06-04 10:17:30.500442 tavern-2.1.0/tavern/_plugins/mqtt/jsonschema.yaml
+-rw-r--r--   0        0        0     2523 2023-06-04 10:17:30.500442 tavern-2.1.0/tavern/_plugins/mqtt/request.py
+-rw-r--r--   0        0        0    11430 2023-06-04 10:17:30.500442 tavern-2.1.0/tavern/_plugins/mqtt/response.py
+-rw-r--r--   0        0        0     3233 2023-06-04 10:17:30.500442 tavern-2.1.0/tavern/_plugins/mqtt/schema.yaml
+-rw-r--r--   0        0        0     1267 2023-06-04 10:17:30.500442 tavern-2.1.0/tavern/_plugins/mqtt/tavernhook.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:17:30.500442 tavern-2.1.0/tavern/_plugins/rest/__init__.py
+-rw-r--r--   0        0        0     6596 2023-06-04 10:17:30.500442 tavern-2.1.0/tavern/_plugins/rest/files.py
+-rw-r--r--   0        0        0    16090 2023-06-04 10:17:30.500442 tavern-2.1.0/tavern/_plugins/rest/request.py
+-rw-r--r--   0        0        0     8291 2023-06-04 10:17:30.500442 tavern-2.1.0/tavern/_plugins/rest/response.py
+-rw-r--r--   0        0        0      860 2023-06-04 10:17:30.500442 tavern-2.1.0/tavern/_plugins/rest/tavernhook.py
+-rw-r--r--   0        0        0     2969 2023-06-04 10:17:30.500442 tavern-2.1.0/tavern/core.py
+-rw-r--r--   0        0        0     2739 2023-06-04 10:17:30.500442 tavern-2.1.0/tavern/entry.py
+-rw-r--r--   0        0        0     7575 2023-06-04 10:17:30.500442 tavern-2.1.0/tavern/helpers.py
+-rw-r--r--   0        0        0      466 2023-06-04 10:17:30.500442 tavern-2.1.0/tavern/request.py
+-rw-r--r--   0        0        0     9571 2023-06-04 10:17:30.500442 tavern-2.1.0/tavern/response.py
+-rw-r--r--   0        0        0      919 2023-06-04 10:17:30.500442 tavern-2.1.0/tests/conftest.py
+-rw-r--r--   0        0        0      195 2023-06-04 10:17:30.500442 tavern-2.1.0/tests/integration/Dockerfile
+-rw-r--r--   0        0        0       33 2023-06-04 10:17:30.500442 tavern-2.1.0/tests/integration/OK.json.gz
+-rw-r--r--   0        0        0        3 2023-06-04 10:17:30.500442 tavern-2.1.0/tests/integration/OK.txt
+-rw-r--r--   0        0        0      504 2023-06-04 10:17:30.500442 tavern-2.1.0/tests/integration/README.md
+-rw-r--r--   0        0        0      608 2023-06-04 10:17:30.500442 tavern-2.1.0/tests/integration/common.yaml
+-rw-r--r--   0        0        0      621 2023-06-04 10:17:30.500442 tavern-2.1.0/tests/integration/conftest.py
+-rw-r--r--   0        0        0      126 2023-06-04 10:17:30.500442 tavern-2.1.0/tests/integration/docker-compose.yaml
+-rw-r--r--   0        0        0      167 2023-06-04 10:17:30.500442 tavern-2.1.0/tests/integration/ext_functions.py
+-rw-r--r--   0        0        0      203 2023-06-04 10:17:30.500442 tavern-2.1.0/tests/integration/extra.yaml
+-rw-r--r--   0        0        0      254 2023-06-04 10:17:30.500442 tavern-2.1.0/tests/integration/global_cfg.yaml
+-rw-r--r--   0        0        0       91 2023-06-04 10:17:30.500442 tavern-2.1.0/tests/integration/parametrize_includes.yaml
+-rw-r--r--   0        0        0    13092 2023-06-04 10:17:30.500442 tavern-2.1.0/tests/integration/server.py
+-rw-r--r--   0        0        0      297 2023-06-04 10:17:30.500442 tavern-2.1.0/tests/integration/test_allure.tavern.yaml
+-rw-r--r--   0        0        0      659 2023-06-04 10:17:30.503775 tavern-2.1.0/tests/integration/test_auth_key.tavern.yaml
+-rw-r--r--   0        0        0      624 2023-06-04 10:17:30.503775 tavern-2.1.0/tests/integration/test_certs.tavern.yaml
+-rw-r--r--   0        0        0     1569 2023-06-04 10:17:30.503775 tavern-2.1.0/tests/integration/test_cookie_remember.tavern.yaml
+-rw-r--r--   0        0        0     6106 2023-06-04 10:17:30.503775 tavern-2.1.0/tests/integration/test_cookies.tavern.yaml
+-rw-r--r--   0        0        0     2448 2023-06-04 10:17:30.503775 tavern-2.1.0/tests/integration/test_data_key.tavern.yaml
+-rw-r--r--   0        0        0       29 2023-06-04 10:17:30.503775 tavern-2.1.0/tests/integration/test_dummy.py
+-rw-r--r--   0        0        0      331 2023-06-04 10:17:30.503775 tavern-2.1.0/tests/integration/test_env_var_format.tavern.yaml
+-rw-r--r--   0        0        0      277 2023-06-04 10:17:30.503775 tavern-2.1.0/tests/integration/test_error.tavern.yaml
+-rw-r--r--   0        0        0     3152 2023-06-04 10:17:30.503775 tavern-2.1.0/tests/integration/test_external_functions.tavern.yaml
+-rw-r--r--   0        0        0     5435 2023-06-04 10:17:30.503775 tavern-2.1.0/tests/integration/test_files.tavern.yaml
+-rw-r--r--   0        0        0     2398 2023-06-04 10:17:30.503775 tavern-2.1.0/tests/integration/test_fixtures.tavern.yaml
+-rw-r--r--   0        0        0      799 2023-06-04 10:17:30.503775 tavern-2.1.0/tests/integration/test_follow_redirects.tavern.yaml
+-rw-r--r--   0        0        0     1028 2023-06-04 10:17:30.503775 tavern-2.1.0/tests/integration/test_header_comparisons.tavern.yaml
+-rw-r--r--   0        0        0     1269 2023-06-04 10:17:30.503775 tavern-2.1.0/tests/integration/test_helpers.tavern.yaml
+-rw-r--r--   0        0        0     4837 2023-06-04 10:17:30.503775 tavern-2.1.0/tests/integration/test_jmes.tavern.yaml
+-rw-r--r--   0        0        0      750 2023-06-04 10:17:30.503775 tavern-2.1.0/tests/integration/test_minimal.tavern.yaml
+-rw-r--r--   0        0        0    14838 2023-06-04 10:17:30.503775 tavern-2.1.0/tests/integration/test_parametrize.tavern.yaml
+-rw-r--r--   0        0        0     2167 2023-06-04 10:17:30.503775 tavern-2.1.0/tests/integration/test_regex.tavern.yaml
+-rw-r--r--   0        0        0     2031 2023-06-04 10:17:30.503775 tavern-2.1.0/tests/integration/test_response_types.tavern.yaml
+-rw-r--r--   0        0        0     2372 2023-06-04 10:17:30.503775 tavern-2.1.0/tests/integration/test_retry.tavern.yaml
+-rw-r--r--   0        0        0      575 2023-06-04 10:17:30.503775 tavern-2.1.0/tests/integration/test_save_dict_value.tavern.yaml
+-rw-r--r--   0        0        0      970 2023-06-04 10:17:30.503775 tavern-2.1.0/tests/integration/test_selective_tests.tavern.yaml
+-rw-r--r--   0        0        0     2432 2023-06-04 10:17:30.503775 tavern-2.1.0/tests/integration/test_skipped_tests.tavern.yaml
+-rw-r--r--   0        0        0     1506 2023-06-04 10:17:30.503775 tavern-2.1.0/tests/integration/test_status_codes.tavern.yaml
+-rw-r--r--   0        0        0      235 2023-06-04 10:17:30.503775 tavern-2.1.0/tests/integration/test_stream.tavern.yaml
+-rw-r--r--   0        0        0    10926 2023-06-04 10:17:30.503775 tavern-2.1.0/tests/integration/test_strict_key_checks.tavern.yaml
+-rw-r--r--   0        0        0     1951 2023-06-04 10:17:30.503775 tavern-2.1.0/tests/integration/test_timeout.tavern.yaml
+-rw-r--r--   0        0        0    12933 2023-06-04 10:17:30.503775 tavern-2.1.0/tests/integration/test_typetokens.tavern.yaml
+-rw-r--r--   0        0        0     1415 2023-06-04 10:17:30.503775 tavern-2.1.0/tests/integration/test_validate_pykwalify.tavern.yaml
+-rw-r--r--   0        0        0        0 2023-06-04 10:17:30.503775 tavern-2.1.0/tests/integration/testfile.txt
+-rw-r--r--   0        0        0      650 2023-06-04 10:17:30.503775 tavern-2.1.0/tests/logging.yaml
+-rw-r--r--   0        0        0      915 2023-06-04 10:17:30.503775 tavern-2.1.0/tests/unit/conftest.py
+-rw-r--r--   0        0        0     9612 2023-06-04 10:17:30.503775 tavern-2.1.0/tests/unit/response/test_mqtt_response.py
+-rw-r--r--   0        0        0    12296 2023-06-04 10:17:30.503775 tavern-2.1.0/tests/unit/response/test_rest.py
+-rw-r--r--   0        0        0     1483 2023-06-04 10:17:30.503775 tavern-2.1.0/tests/unit/test_call_run.py
+-rw-r--r--   0        0        0    16186 2023-06-04 10:17:30.503775 tavern-2.1.0/tests/unit/test_core.py
+-rw-r--r--   0        0        0    14289 2023-06-04 10:17:30.503775 tavern-2.1.0/tests/unit/test_helpers.py
+-rw-r--r--   0        0        0     7161 2023-06-04 10:17:30.503775 tavern-2.1.0/tests/unit/test_mqtt.py
+-rw-r--r--   0        0        0     5791 2023-06-04 10:17:30.503775 tavern-2.1.0/tests/unit/test_pytest_hooks.py
+-rw-r--r--   0        0        0    16788 2023-06-04 10:17:30.503775 tavern-2.1.0/tests/unit/test_request.py
+-rw-r--r--   0        0        0     6131 2023-06-04 10:17:30.503775 tavern-2.1.0/tests/unit/test_schema.py
+-rw-r--r--   0        0        0     1030 2023-06-04 10:17:30.503775 tavern-2.1.0/tests/unit/test_strict_util.py
+-rw-r--r--   0        0        0    14898 2023-06-04 10:17:30.503775 tavern-2.1.0/tests/unit/test_utilities.py
+-rw-r--r--   0        0        0     2444 2023-06-04 10:17:30.503775 tavern-2.1.0/tox-integration.ini
+-rw-r--r--   0        0        0      625 2023-06-04 10:17:30.503775 tavern-2.1.0/tox.ini
+-rw-r--r--   0        0        0    10720 1970-01-01 00:00:00.000000 tavern-2.1.0/PKG-INFO
```

### Comparing `tavern-2.0.7/.dockerignore` & `tavern-2.1.0/.dockerignore`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/.github/workflows/main.yml` & `tavern-2.1.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/.gitignore` & `tavern-2.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/CHANGELOG.md` & `tavern-2.1.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -162,16 +162,14 @@
 
 ##  0.17.1          Dummy tag to attempt to make travis dpeloy, again (2018-08-07)
 
 ##  0.17.2          Stop wrapping responses/schemas in files for verification (2018-08-07)
 
 #  0.18.0          Add 'timeout' parameter for http requests (2018-08-24)
 
-##  show            Bump version: 0.17.2 → 0.18.0 (2018-08-24)
-
 ##  0.18.1          Add content type/encoding to uploaded files (2018-09-05)
 
 ##  0.18.2          Fix formatting environment variables in command line global config files (2018-09-21)
 
 ##  0.18.3          Fix 'anything' token in included test stages (2018-09-28)
 
 #  0.19.0          Add retries to stages (2018-10-07)
@@ -257,16 +255,14 @@
 
 ##  1.0.2           Fix incorrect logic checking request codes (2020-05-01)
 
 #  1.1.0           Add new global option to enable merging of keys from external functions (2020-05-01)
 
 ##  1.1.1           Travis fix (2020-05-23)
 
-##  travis-force    Attempt to force travis to commit (2020-05-23)
-
 ##  1.1.2           fforce new verison to make travis actually commit (2020-05-23)
 
 ##  1.1.3           travis (2020-05-23)
 
 ##  1.1.4           Bump version: 1.1.3 → 1.1.4 (2020-05-23)
 
 ##  1.1.5           travis (2020-05-23)
@@ -404,7 +400,9 @@
 ##  2.0.3           Add type annotations (internal change) (2023-02-10)
 
 ##  2.0.4           Fix using ext functions in MQTT publish (2023-02-16)
 
 ##  2.0.5           Attempt to fix deadlock in subscribe locks (2023-02-16)
 
 ##  2.0.6           Fix a few small MQTT issues (2023-03-13)
+
+##  2.0.7           Lock pytest to <7.3 to fix issue with marks (2023-04-15)
```

### Comparing `tavern-2.0.7/CONTRIBUTING.md` & `tavern-2.1.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/LICENSE` & `tavern-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/README.md` & `tavern-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/constraints.txt` & `tavern-2.1.0/constraints.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# This file is autogenerated by pip-compile with Python 3.9
+# This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
 #    pip-compile --all-extras --output-file=constraints.txt --resolver=backtracking --strip-extras pyproject.toml
 #
 allure-pytest==2.12.0
     # via tavern (pyproject.toml)
 allure-python-commons==2.12.0
@@ -74,29 +74,28 @@
     # via pytest-xdist
 faker==15.3.4
     # via tavern (pyproject.toml)
 filelock==3.8.2
     # via
     #   tox
     #   virtualenv
-flask==2.2.2
+flask==2.2.5
     # via tavern (pyproject.toml)
 flit==3.8.0
     # via tavern (pyproject.toml)
 flit-core==3.8.0
     # via flit
 fluent-logger==0.10.0
     # via tavern (pyproject.toml)
 identify==2.5.10
     # via pre-commit
 idna==3.4
     # via requests
 importlib-metadata==5.2.0
     # via
-    #   flask
     #   keyring
     #   twine
 iniconfig==1.1.1
     # via pytest
 itsdangerous==2.1.2
     # via
     #   flask
@@ -206,15 +205,15 @@
 pyyaml==5.4.1
     # via
     #   docker-compose
     #   pre-commit
     #   tavern (pyproject.toml)
 readme-renderer==37.3
     # via twine
-requests==2.28.1
+requests==2.31.0
     # via
     #   docker
     #   docker-compose
     #   flit
     #   requests-toolbelt
     #   tavern (pyproject.toml)
     #   twine
@@ -266,18 +265,22 @@
     #   tox-travis
 tox-travis==0.12
     # via tavern (pyproject.toml)
 twine==4.0.2
     # via tavern (pyproject.toml)
 types-pyyaml==6.0.12.2
     # via tavern (pyproject.toml)
+types-requests==2.31.0.0
+    # via tavern (pyproject.toml)
+types-setuptools==67.8.0.0
+    # via tavern (pyproject.toml)
+types-urllib3==1.26.25.13
+    # via types-requests
 typing-extensions==4.4.0
-    # via
-    #   black
-    #   mypy
+    # via mypy
 urllib3==1.26.13
     # via
     #   docker
     #   requests
     #   twine
 virtualenv==20.17.1
     # via
```

### Comparing `tavern-2.0.7/docs/Makefile` & `tavern-2.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/docs/source/_static/favicon.png` & `tavern-2.1.0/docs/source/_static/favicon.png`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/docs/source/_static/icon.png` & `tavern-2.1.0/docs/source/_static/icon.png`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/docs/source/basics.md` & `tavern-2.1.0/docs/source/basics.md`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/docs/source/conf.py` & `tavern-2.1.0/docs/source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
 version = "1.0"
 # The full version, including alpha/beta/rc tags.
-release = "2.0.7"
+release = "2.1.0"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 language = None
```

### Comparing `tavern-2.0.7/docs/source/cookbook.md` & `tavern-2.1.0/docs/source/cookbook.md`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/docs/source/debugging.md` & `tavern-2.1.0/docs/source/debugging.md`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/docs/source/examples.md` & `tavern-2.1.0/docs/source/examples.md`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/docs/source/http.md` & `tavern-2.1.0/docs/source/http.md`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/docs/source/index.md` & `tavern-2.1.0/docs/source/index.md`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/docs/source/mqtt.md` & `tavern-2.1.0/docs/source/mqtt.md`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/docs/source/plugins.md` & `tavern-2.1.0/docs/source/plugins.md`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/docs/source/server.md` & `tavern-2.1.0/docs/source/server.md`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/example/advanced/server.py` & `tavern-2.1.0/example/advanced/server.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/example/advanced/test_server.tavern.yaml` & `tavern-2.1.0/example/advanced/test_server.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/example/advanced/testing_utils.py` & `tavern-2.1.0/example/advanced/testing_utils.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/example/components/components.md` & `tavern-2.1.0/example/components/components.md`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/example/components/components/auth_stage.yaml` & `tavern-2.1.0/example/components/components/auth_stage.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/example/components/server.py` & `tavern-2.1.0/example/components/server.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/example/components/test_hello.tavern.yaml` & `tavern-2.1.0/example/components/test_hello.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/example/components/test_ping.tavern.yaml` & `tavern-2.1.0/example/components/test_ping.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/example/cookies/server.py` & `tavern-2.1.0/example/cookies/server.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/example/cookies/test_server.tavern.yaml` & `tavern-2.1.0/example/cookies/test_server.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/example/generate_from_openapi/Pipfile.lock` & `tavern-2.1.0/example/generate_from_openapi/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/example/generate_from_openapi/pub_tavern.py` & `tavern-2.1.0/example/generate_from_openapi/pub_tavern.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/example/generate_from_openapi/test_example_output.tavern.yaml` & `tavern-2.1.0/example/generate_from_openapi/test_example_output.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/example/hooks/conftest.py` & `tavern-2.1.0/example/hooks/conftest.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/example/hooks/test_server.tavern.yaml` & `tavern-2.1.0/example/hooks/test_server.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/example/mqtt/README.md` & `tavern-2.1.0/example/mqtt/README.md`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/example/mqtt/conftest.py` & `tavern-2.1.0/example/mqtt/conftest.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/example/mqtt/docker-compose.yaml` & `tavern-2.1.0/example/mqtt/docker-compose.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/example/mqtt/listener.py` & `tavern-2.1.0/example/mqtt/listener.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/example/mqtt/server.py` & `tavern-2.1.0/example/mqtt/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,14 @@
     db = getattr(g, "_database", None)
     if db is None:
         db = g._database = get_db()
 
     return db
 
 
-@app.before_first_request
 def setup_logging():
     log_cfg = """
 version: 1
 disable_existing_loggers: true
 formatters:
     fluent_fmt:
         (): fluent.handler.FluentRecordFormatter
@@ -204,9 +203,10 @@
             "CREATE TABLE devices_table (device_id TEXT NOT NULL, lights_on INTEGER NOT NULL)"
         )
 
     return "", 204
 
 
 if __name__ == "__main__":
+    setup_logging()
     db = get_db()
     _reset_db(db)
```

### Comparing `tavern-2.0.7/example/mqtt/test_mqtt.tavern.yaml` & `tavern-2.1.0/example/mqtt/test_mqtt.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/example/mqtt/test_mqtt_failures.tavern.yaml` & `tavern-2.1.0/example/mqtt/test_mqtt_failures.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/example/simple/running_tests.md` & `tavern-2.1.0/example/simple/running_tests.md`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/example/simple/test_server.tavern.yaml` & `tavern-2.1.0/example/simple/test_server.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/pyproject.toml` & `tavern-2.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     "License :: OSI Approved :: MIT License",
 ]
 
 keywords = ["testing", "pytest"]
 
 name = "tavern"
 description = "Simple testing of RESTful APIs"
-version = "2.0.7"
+version = "2.1.0"
 
 dependencies = [
     "PyYAML>=5.3.1,<7",
     "jmespath>=1,<2",
     "jsonschema>=3.2.0,<5",
     "paho-mqtt>=1.3.1,<=1.6.1",
     "pyjwt>=2.4.0,<3",
@@ -57,15 +57,15 @@
 dev = [
     "Faker",
     "allure-pytest",
     "black==23.1.0",
     "bump2version",
     "colorlog",
     "docker-compose",
-    "flask",
+    "flask>=2.2.3",
     "fluent-logger",
     "itsdangerous",
     "mypy",
     "mypy-extensions",
     "coverage[toml]",
     "types-PyYAML",
     "flit >=3.2,<4",
@@ -76,14 +76,16 @@
     "ruff>=0.0.246",
     "pytest-xdist",
     "py",
     "tox>=3,<4",
     "tox-travis",
     "twine",
     "wheel",
+    "types-setuptools",
+    "types-requests",
     # This has to be installed separately, otherwise you can't upload to pypi
     # "tbump@https://github.com/michaelboulton/tbump/archive/714ba8957a3c84b625608ceca39811ebe56229dc.zip",
 ]
 
 
 [project.scripts]
 
@@ -128,14 +130,15 @@
 addopts = [
     "--doctest-modules",
     "-r", "xs",
     "-vv",
     "--strict-markers",
     "-p", "no:logging",
     "--tb=short",
+    "--color=yes"
 ]
 norecursedirs = [
     ".git",
     ".tox",
     "example",
 ]
 
@@ -154,15 +157,15 @@
 [tool.ruff.per-file-ignores]
 "tests/*" = ["S"]
 
 [tool.ruff.isort]
 known-first-party = ["tavern"]
 
 [tool.tbump.version]
-current = "2.0.7"
+current = "2.1.0"
 
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
```

### Comparing `tavern-2.0.7/requirements.txt` & `tavern-2.1.0/requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# This file is autogenerated by pip-compile with Python 3.9
+# This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
 #    pip-compile --all-extras --generate-hashes --output-file=requirements.txt --resolver=backtracking pyproject.toml
 #
 allure-pytest==2.12.0 \
     --hash=sha256:1a10b2b78334443097d7be890a53c991e857e13d14781377c2f8d11eb4b5582c \
     --hash=sha256:85b73b1dbe9908ba4f84b80118a93e1049c02dd593209260d8c1c950cf286f6c
@@ -300,17 +300,17 @@
     # via tavern (pyproject.toml)
 filelock==3.8.2 \
     --hash=sha256:7565f628ea56bfcd8e54e42bdc55da899c85c1abfe1b5bcfd147e9188cebb3b2 \
     --hash=sha256:8df285554452285f79c035efb0c861eb33a4bcfa5b7a137016e32e6a90f9792c
     # via
     #   tox
     #   virtualenv
-flask==2.2.2 \
-    --hash=sha256:642c450d19c4ad482f96729bd2a8f6d32554aa1e231f4f6b4e7e5264b16cca2b \
-    --hash=sha256:b9c46cc36662a7949f34b52d8ec7bb59c0d74ba08ba6cb9ce9adc1d8676d9526
+flask==2.2.5 \
+    --hash=sha256:58107ed83443e86067e41eff4631b058178191a355886f8e479e347fa1285fdf \
+    --hash=sha256:edee9b0a7ff26621bd5a8c10ff484ae28737a2410d99b0bb9a6850c7fb977aa0
     # via tavern (pyproject.toml)
 flit==3.8.0 \
     --hash=sha256:5ee0f88fd1cfa4160d1a8fa01237e96d06d677ae0403a0bbabbb277cb37c5e9c \
     --hash=sha256:d0f2a8f4bd45dc794befbf5839ecc0fd3830d65a57bd52b5997542fac5d5e937
     # via tavern (pyproject.toml)
 flit-core==3.8.0 \
     --hash=sha256:64a29ec845164a6abe1136bf4bc5ae012bdfe758ed42fc7571a9059a7c80bd83 \
@@ -328,15 +328,14 @@
     --hash=sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4 \
     --hash=sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2
     # via requests
 importlib-metadata==5.2.0 \
     --hash=sha256:0eafa39ba42bf225fc00e67f701d71f85aead9f878569caf13c3724f704b970f \
     --hash=sha256:404d48d62bba0b7a77ff9d405efd91501bef2e67ff4ace0bed40a0cf28c3c7cd
     # via
-    #   flask
     #   keyring
     #   twine
 iniconfig==1.1.1 \
     --hash=sha256:011e24c64b7f47f6ebd835bb12a743f2fbe9a26d4cecaa7f53bc4f35ee9da8b3 \
     --hash=sha256:bc3af051d7d14b2ee5ef9969666def0cd1a000e121eaea580d4a313df4b37f32
     # via pytest
 itsdangerous==2.1.2 \
@@ -711,17 +710,17 @@
     #   docker-compose
     #   pre-commit
     #   tavern (pyproject.toml)
 readme-renderer==37.3 \
     --hash=sha256:cd653186dfc73055656f090f227f5cb22a046d7f71a841dfa305f55c9a513273 \
     --hash=sha256:f67a16caedfa71eef48a31b39708637a6f4664c4394801a7b0d6432d13907343
     # via twine
-requests==2.28.1 \
-    --hash=sha256:7c5599b102feddaa661c826c56ab4fee28bfd17f5abca1ebbe3e7f19d7c97983 \
-    --hash=sha256:8fefa2a1a1365bf5520aac41836fbee479da67864514bdb821f31ce07ce65349
+requests==2.31.0 \
+    --hash=sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f \
+    --hash=sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1
     # via
     #   docker
     #   docker-compose
     #   flit
     #   requests-toolbelt
     #   tavern (pyproject.toml)
     #   twine
@@ -853,20 +852,30 @@
     --hash=sha256:929bc3c280033347a00f847236564d1c52a3e61b1ac2516c97c48f3ceab756d8 \
     --hash=sha256:9e102ef5fdd5a20661eb88fad46338806c3bd32cf1db729603fe3697b1bc83c8
     # via tavern (pyproject.toml)
 types-pyyaml==6.0.12.2 \
     --hash=sha256:1e94e80aafee07a7e798addb2a320e32956a373f376655128ae20637adb2655b \
     --hash=sha256:6840819871c92deebe6a2067fb800c11b8a063632eb4e3e755914e7ab3604e83
     # via tavern (pyproject.toml)
+types-requests==2.31.0.0 \
+    --hash=sha256:7c5cea7940f8e92ec560bbc468f65bf684aa3dcf0554a6f8c4710f5f708dc598 \
+    --hash=sha256:c1c29d20ab8d84dff468d7febfe8e0cb0b4664543221b386605e14672b44ea25
+    # via tavern (pyproject.toml)
+types-setuptools==67.8.0.0 \
+    --hash=sha256:6df73340d96b238a4188b7b7668814b37e8018168aef1eef94a3b1872e3f60ff \
+    --hash=sha256:95c9ed61871d6c0e258433373a4e1753c0a7c3627a46f4d4058c7b5a08ab844f
+    # via tavern (pyproject.toml)
+types-urllib3==1.26.25.13 \
+    --hash=sha256:3300538c9dc11dad32eae4827ac313f5d986b8b21494801f1bf97a1ac6c03ae5 \
+    --hash=sha256:5dbd1d2bef14efee43f5318b5d36d805a489f6600252bb53626d4bfafd95e27c
+    # via types-requests
 typing-extensions==4.4.0 \
     --hash=sha256:1511434bb92bf8dd198c12b1cc812e800d4181cfcb867674e0f8279cc93087aa \
     --hash=sha256:16fa4864408f655d35ec496218b85f79b3437c829e93320c7c9215ccfd92489e
-    # via
-    #   black
-    #   mypy
+    # via mypy
 urllib3==1.26.13 \
     --hash=sha256:47cc05d99aaa09c9e72ed5809b60e7ba354e64b59c9c173ac3018642d8bb41fc \
     --hash=sha256:c083dd0dce68dbfbe1129d5271cb90f9447dea7d52097c6e0126120c521ddea8
     # via
     #   docker
     #   requests
     #   twine
```

### Comparing `tavern-2.0.7/scripts/update-changelog.bash` & `tavern-2.1.0/scripts/update-changelog.bash`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/tavern/_core/dict_util.py` & `tavern-2.1.0/tavern/_core/dict_util.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/tavern/_core/exceptions.py` & `tavern-2.1.0/tavern/_core/exceptions.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/tavern/_core/extfunctions.py` & `tavern-2.1.0/tavern/_core/extfunctions.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/tavern/_core/general.py` & `tavern-2.1.0/tavern/_core/general.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/tavern/_core/jmesutils.py` & `tavern-2.1.0/tavern/_core/jmesutils.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/tavern/_core/loader.py` & `tavern-2.1.0/tavern/_core/loader.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/tavern/_core/plugins.py` & `tavern-2.1.0/tavern/_core/plugins.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/tavern/_core/pytest/config.py` & `tavern-2.1.0/tavern/_core/pytest/config.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/tavern/_core/pytest/error.py` & `tavern-2.1.0/tavern/_core/pytest/error.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/tavern/_core/pytest/file.py` & `tavern-2.1.0/tavern/_core/pytest/file.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/tavern/_core/pytest/hooks.py` & `tavern-2.1.0/tavern/_core/pytest/hooks.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/tavern/_core/pytest/item.py` & `tavern-2.1.0/tavern/_core/pytest/item.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/tavern/_core/pytest/newhooks.py` & `tavern-2.1.0/tavern/_core/pytest/newhooks.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/tavern/_core/pytest/util.py` & `tavern-2.1.0/tavern/_core/pytest/util.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/tavern/_core/report.py` & `tavern-2.1.0/tavern/_core/report.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/tavern/_core/run.py` & `tavern-2.1.0/tavern/_core/run.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/tavern/_core/schema/extensions.py` & `tavern-2.1.0/tavern/_core/schema/extensions.py`

 * *Files 4% similar despite different names*

```diff
@@ -364,26 +364,33 @@
 
     return True
 
 
 def validate_file_spec(value, rule_obj, path) -> bool:
     """Validate file upload arguments"""
 
+    logger = get_pykwalify_logger("tavern.schema.extensions")
+
     if not isinstance(value, dict):
         raise BadSchemaError(
             "File specification must be a mapping of file names to file specs, got {}".format(
                 value
             )
         )
 
+    if value.get("file_path"):
+        # If the file spec was a list, this function will be called for each item. Just call this
+        # function recursively to check each item.
+        return validate_file_spec({"file": value}, rule_obj, path)
+
     for _, filespec in value.items():
         if isinstance(filespec, str):
             file_path = filespec
         elif isinstance(filespec, dict):
-            valid = {"file_path", "content_type", "content_encoding"}
+            valid = {"file_path", "content_type", "content_encoding", "form_field_name"}
             extra = set(filespec.keys()) - valid
             if extra:
                 raise BadSchemaError(
                     "Invalid extra keys passed to file upload block: {}".format(extra)
                 )
 
             try:
@@ -395,15 +402,15 @@
         else:
             raise BadSchemaError(
                 "File specification must be a file path or a dictionary"
             )
 
         if not os.path.exists(file_path):
             if re.search(".*{.+}.*", file_path):
-                get_pykwalify_logger("tavern.schemas.extensions").debug(
+                logger.debug(
                     "Could not find file path, but it might be a format variable, so continuing"
                 )
             else:
                 raise BadSchemaError(
                     "Path to file to upload '{}' was not found".format(file_path)
                 )
```

### Comparing `tavern-2.0.7/tavern/_core/schema/files.py` & `tavern-2.1.0/tavern/_core/schema/files.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/tavern/_core/schema/jsonschema.py` & `tavern-2.1.0/tavern/_core/schema/jsonschema.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/tavern/_core/schema/tests.jsonschema.yaml` & `tavern-2.1.0/tavern/_core/schema/tests.jsonschema.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -158,15 +158,17 @@
               type: number
 
       file_body:
         type: string
         description: Path to a file to upload as the request body
 
       files:
-        type: object
+        oneOf:
+          - type: object
+          - type: array
         description: Files to send as part of the request
 
       clear_session_cookies:
         description: Whether to clear sesion cookies before running this request
         type: boolean
 
   mqtt_publish:
```

### Comparing `tavern-2.0.7/tavern/_core/schema/tests.schema.yaml` & `tavern-2.1.0/tavern/_core/schema/tests.schema.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/tavern/_core/stage_lines.py` & `tavern-2.1.0/tavern/_core/stage_lines.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/tavern/_core/strict_util.py` & `tavern-2.1.0/tavern/_core/strict_util.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/tavern/_core/testhelpers.py` & `tavern-2.1.0/tavern/_core/testhelpers.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/tavern/_plugins/mqtt/client.py` & `tavern-2.1.0/tavern/_plugins/mqtt/client.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/tavern/_plugins/mqtt/jsonschema.yaml` & `tavern-2.1.0/tavern/_plugins/mqtt/jsonschema.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/tavern/_plugins/mqtt/request.py` & `tavern-2.1.0/tavern/_plugins/mqtt/request.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/tavern/_plugins/mqtt/response.py` & `tavern-2.1.0/tavern/_plugins/mqtt/response.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/tavern/_plugins/mqtt/schema.yaml` & `tavern-2.1.0/tavern/_plugins/mqtt/schema.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/tavern/_plugins/mqtt/tavernhook.py` & `tavern-2.1.0/tavern/_plugins/mqtt/tavernhook.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/tavern/_plugins/rest/request.py` & `tavern-2.1.0/tavern/_plugins/rest/request.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 import contextlib
 import json
 import logging
-import mimetypes
-import os
 import warnings
 from contextlib import ExitStack
 from itertools import filterfalse, tee
-from typing import Mapping, MutableMapping, Optional, Union
+from typing import Mapping, MutableMapping, Optional
 from urllib.parse import quote_plus
 
 import requests
 from box.box import Box
 from requests.cookies import cookiejar_from_dict
 from requests.utils import dict_from_cookiejar
 
 from tavern._core import exceptions
 from tavern._core.dict_util import check_expected_keys, deep_dict_merge, format_keys
 from tavern._core.extfunctions import update_from_ext
 from tavern._core.general import valid_http_methods
 from tavern._core.pytest.config import TestConfig
 from tavern._core.report import attach_yaml
+from tavern._plugins.rest.files import get_file_arguments, guess_filespec
 from tavern.request import BaseRequest
 
 logger = logging.getLogger(__name__)
 
 
 def get_request_args(rspec: MutableMapping, test_block_config: TestConfig) -> dict:
     """Format the test spec given values inthe global config
@@ -90,15 +89,22 @@
             "Unknown HTTP method {}".format(fspec["method"])
         )
 
     # If the user is using the file_body key, try to guess what type of file/encoding it is.
     filename = fspec.get("file_body")
     if filename:
         with ExitStack() as stack:
-            file_spec = guess_filespec(filename, stack, test_block_config)
+            file_spec, group_name = guess_filespec(filename, stack, test_block_config)
+
+            # Group name doesn't matter here as it's a single file
+            if group_name:
+                logger.warning(
+                    f"'group_name' for the 'file_body' key was specified as '{group_name}' but this will be ignored "
+                )
+
             fspec["file_body"] = filename
             if len(file_spec) == 2:
                 logger.debug(
                     "No content type or encoding inferred from file_body for %s",
                     filename,
                 )
 
@@ -322,122 +328,14 @@
         )
 
     from_cookiejar = {c: existing_cookies.get(c) for c in expected}
 
     return deep_dict_merge(from_cookiejar, from_extra)
 
 
-def _read_filespec(filespec: Union[str, dict]):
-    """
-    Get configuration for uploading file
-
-    Can either be just a path to a file or a 'long' format including content type/encoding
-
-    Args:
-        filespec: Either a string with the path to a file or a dictionary with file_path and possible content_type and/or content_encoding
-
-    Returns:
-        (file path, content type, content encoding)
-    """
-    if isinstance(filespec, str):
-        return filespec, None, None
-    elif isinstance(filespec, dict):
-        return (
-            filespec.get("file_path"),
-            filespec.get("content_type"),
-            filespec.get("content_encoding"),
-        )
-    else:
-        # Could remove, also done in schema check
-        raise exceptions.BadSchemaError(
-            "File specification must be a path or a dictionary"
-        )
-
-
-def _get_file_arguments(
-    request_args: dict, stack: ExitStack, test_block_config: TestConfig
-) -> dict:
-    """Get corect arguments for anything that should be passed as a file to
-    requests
-
-    Args:
-        request_args: args passed to requests
-        test_block_config: config for test
-        stack: context stack to add file objects to so they're
-            closed correctly after use
-
-    Returns:
-        mapping of 'files' block to pass directly to requests
-    """
-
-    files_to_send = {}
-
-    for key, filespec in request_args.get("files", {}).items():
-        file_spec = guess_filespec(filespec, stack, test_block_config)
-
-        files_to_send[key] = tuple(file_spec)
-
-    if files_to_send:
-        return {"files": files_to_send}
-    else:
-        return {}
-
-
-def guess_filespec(
-    filespec: Union[str, dict], stack: ExitStack, test_block_config: TestConfig
-):
-    """tries to guess the content type and encoding from a file.
-
-    Args:
-        test_block_config: config for test/stage
-        stack: exit stack to add open files context to
-        filespec: a string path to a file or a dictionary of the file path, content type, and encoding.
-
-    Returns:
-        tuple: A tuple of either length 2 (filename and file object), 3 (as before, with ceontent type), or 4 (as before, with with content encoding)
-
-    Notes:
-        If a 4-tuple is returned, the last element is a dictionary of headers to send to requests, _not_ the raw encoding value.
-    """
-    if not mimetypes.inited:
-        mimetypes.init()
-
-    filepath, content_type, encoding = _read_filespec(filespec)
-
-    filepath = format_keys(filepath, test_block_config.variables)
-    filename = os.path.basename(filepath)
-
-    # a 2-tuple ('filename', fileobj)
-    file_spec = [
-        filename,
-        stack.enter_context(open(filepath, "rb")),
-    ]
-
-    # Try to guess as well, but don't override what the user specified
-    guessed_content_type, guessed_encoding = mimetypes.guess_type(filepath)
-    content_type = content_type or guessed_content_type
-    encoding = encoding or guessed_encoding
-
-    # If it doesn't have a mimetype, or can't guess it, don't
-    # send the content type for the file
-    if content_type:
-        # a 3-tuple ('filename', fileobj, 'content_type')
-        logger.debug("content_type for '%s' = '%s'", filename, content_type)
-        file_spec.append(content_type)
-        if encoding:
-            # or a 4-tuple ('filename', fileobj, 'content_type', custom_headers)
-            logger.debug("encoding for '%s' = '%s'", filename, encoding)
-            # encoding is None for no encoding or the name of the
-            # program used to encode (e.g. compress or gzip). The
-            # encoding is suitable for use as a Content-Encoding header.
-            file_spec.append({"Content-Encoding": encoding})
-
-    return file_spec
-
-
 class RestRequest(BaseRequest):
     optional_in_file = [
         "json",
         "data",
         "params",
         "headers",
         "files",
@@ -526,17 +424,18 @@
 
                 # These are mutually exclusive
                 if file_body:
                     # Any headers will have been set in the above function
                     file = stack.enter_context(open(file_body, "rb"))
                     request_args.update(data=file)
                 else:
-                    self._request_args.update(
-                        _get_file_arguments(request_args, stack, test_block_config)
-                    )
+                    files = get_file_arguments(request_args, stack, test_block_config)
+                    if files:
+                        logger.debug("Sending %d files in request", len(files["files"]))
+                        self._request_args.update(files)
 
                 headers = self._request_args.get("headers", {})
                 for k, v in headers.items():
                     headers[str(k)] = str(v)
 
                 return session.request(**self._request_args)
```

### Comparing `tavern-2.0.7/tavern/_plugins/rest/response.py` & `tavern-2.1.0/tavern/_plugins/rest/response.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/tavern/_plugins/rest/tavernhook.py` & `tavern-2.1.0/tavern/_plugins/rest/tavernhook.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/tavern/core.py` & `tavern-2.1.0/tavern/core.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/tavern/entry.py` & `tavern-2.1.0/tavern/entry.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/tavern/helpers.py` & `tavern-2.1.0/tavern/helpers.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/tavern/response.py` & `tavern-2.1.0/tavern/response.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/tests/conftest.py` & `tavern-2.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/tests/integration/common.yaml` & `tavern-2.1.0/tests/integration/common.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/tests/integration/conftest.py` & `tavern-2.1.0/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/tests/integration/server.py` & `tavern-2.1.0/tests/integration/server.py`

 * *Files 16% similar despite different names*

```diff
@@ -83,16 +83,14 @@
     if not request.files:
         return "", 401
 
     return _handle_files()
 
 
 def _handle_files():
-    if not mimetypes.inited:
-        mimetypes.init()
     for item in request.files.values():
         if item.filename:
             filetype = ".{}".format(item.filename.split(".")[-1])
             if filetype in mimetypes.suffix_map:
                 if not item.content_type:
                     return "", 400
     # Try to download each of the files downloaded to /tmp and
@@ -100,29 +98,80 @@
     for key in request.files:
         file_to_save = request.files[key]
         path = os.path.join("/tmp", file_to_save.filename)
         file_to_save.save(path)
     return "", 200
 
 
+class BadFileUploadException(Exception):
+    """Something wrong when uploading files"""
+
+
+def _verify_is_file_multipart():
+    if not mimetypes.inited:
+        mimetypes.init()
+
+    if not request.content_type.startswith("multipart/form-data"):
+        raise BadFileUploadException("Was not a multipart form upload")
+
+    if not request.files:
+        raise BadFileUploadException("No files in request")
+
+
 @app.route("/fake_upload_file_data", methods=["POST"])
 def upload_fake_file_and_data():
-    if not request.files:
-        return "", 401
+    try:
+        _verify_is_file_multipart()
+    except BadFileUploadException as e:
+        return jsonify({"error": str(e)}), 400
 
     if not request.form.to_dict():
-        return "", 402
-
-    # Verify that the content type is `multipart`
-    if not request.content_type.startswith("multipart/form-data"):
-        return "", 403
+        return "", 400
 
     return _handle_files()
 
 
+@app.route("/files_expect_in_order", methods=["POST"])
+def upload_specific_files_in_order():
+    """Expects a multipart form upload with files in the correct order
+
+    See test_files.tavern.yaml for expected list of files here
+    """
+
+    try:
+        _verify_is_file_multipart()
+    except BadFileUploadException as e:
+        return jsonify({"error": str(e)}), 400
+
+    try:
+        group_1 = request.files.getlist("group_1")
+        if len(group_1) != 2:
+            raise Exception(f"expected 2 files in group 1, got {len(group_1)}")
+        if group_1[0].filename != "OK.txt":
+            raise Exception(
+                f"First file in group 1 should be OK.txt, was {group_1[0].filename}"
+            )
+        if group_1[1].filename != "OK.json.gz":
+            raise Exception(
+                f"Second file in group 1 should be OK.json.gz, was {group_1[1].filename}"
+            )
+
+        group_2 = request.files.getlist("group_2")
+        if len(group_2) != 1:
+            raise Exception(f"expected 1 files in group 2, got {len(group_2)}")
+        if group_2[0].filename != "OK.txt":
+            raise Exception(
+                f"First file in group 2 should be OK.txt, was {group_2[0].filename}"
+            )
+    except Exception as e:
+        return jsonify({"error": str(e)}), 400
+
+    return "", 200
+
+
 @app.route("/nested/again", methods=["GET"])
 def multiple_path_items_response():
     response = {"status": "OK"}
     return jsonify(response), 200
 
 
 @app.route("/pi", methods=["GET"])
```

### Comparing `tavern-2.0.7/tests/integration/test_auth_key.tavern.yaml` & `tavern-2.1.0/tests/integration/test_auth_key.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/tests/integration/test_certs.tavern.yaml` & `tavern-2.1.0/tests/integration/test_certs.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/tests/integration/test_cookie_remember.tavern.yaml` & `tavern-2.1.0/tests/integration/test_cookie_remember.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/tests/integration/test_cookies.tavern.yaml` & `tavern-2.1.0/tests/integration/test_cookies.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/tests/integration/test_data_key.tavern.yaml` & `tavern-2.1.0/tests/integration/test_data_key.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/tests/integration/test_external_functions.tavern.yaml` & `tavern-2.1.0/tests/integration/test_external_functions.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/tests/integration/test_fixtures.tavern.yaml` & `tavern-2.1.0/tests/integration/test_fixtures.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/tests/integration/test_follow_redirects.tavern.yaml` & `tavern-2.1.0/tests/integration/test_follow_redirects.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/tests/integration/test_header_comparisons.tavern.yaml` & `tavern-2.1.0/tests/integration/test_header_comparisons.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/tests/integration/test_helpers.tavern.yaml` & `tavern-2.1.0/tests/integration/test_helpers.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/tests/integration/test_jmes.tavern.yaml` & `tavern-2.1.0/tests/integration/test_jmes.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/tests/integration/test_minimal.tavern.yaml` & `tavern-2.1.0/tests/integration/test_minimal.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/tests/integration/test_parametrize.tavern.yaml` & `tavern-2.1.0/tests/integration/test_parametrize.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/tests/integration/test_regex.tavern.yaml` & `tavern-2.1.0/tests/integration/test_regex.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/tests/integration/test_response_types.tavern.yaml` & `tavern-2.1.0/tests/integration/test_response_types.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/tests/integration/test_retry.tavern.yaml` & `tavern-2.1.0/tests/integration/test_retry.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/tests/integration/test_save_dict_value.tavern.yaml` & `tavern-2.1.0/tests/integration/test_save_dict_value.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/tests/integration/test_selective_tests.tavern.yaml` & `tavern-2.1.0/tests/integration/test_selective_tests.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/tests/integration/test_skipped_tests.tavern.yaml` & `tavern-2.1.0/tests/integration/test_skipped_tests.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/tests/integration/test_status_codes.tavern.yaml` & `tavern-2.1.0/tests/integration/test_status_codes.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/tests/integration/test_strict_key_checks.tavern.yaml` & `tavern-2.1.0/tests/integration/test_strict_key_checks.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/tests/integration/test_timeout.tavern.yaml` & `tavern-2.1.0/tests/integration/test_timeout.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/tests/integration/test_typetokens.tavern.yaml` & `tavern-2.1.0/tests/integration/test_typetokens.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/tests/integration/test_validate_pykwalify.tavern.yaml` & `tavern-2.1.0/tests/integration/test_validate_pykwalify.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/tests/logging.yaml` & `tavern-2.1.0/tests/logging.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/tests/unit/conftest.py` & `tavern-2.1.0/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/tests/unit/response/test_mqtt_response.py` & `tavern-2.1.0/tests/unit/response/test_mqtt_response.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/tests/unit/response/test_rest.py` & `tavern-2.1.0/tests/unit/response/test_rest.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/tests/unit/test_call_run.py` & `tavern-2.1.0/tests/unit/test_call_run.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/tests/unit/test_core.py` & `tavern-2.1.0/tests/unit/test_core.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/tests/unit/test_helpers.py` & `tavern-2.1.0/tests/unit/test_helpers.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/tests/unit/test_mqtt.py` & `tavern-2.1.0/tests/unit/test_mqtt.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/tests/unit/test_pytest_hooks.py` & `tavern-2.1.0/tests/unit/test_pytest_hooks.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/tests/unit/test_request.py` & `tavern-2.1.0/tests/unit/test_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import dataclasses
 import os
 import tempfile
 from contextlib import ExitStack
+from textwrap import dedent
 from unittest.mock import Mock
 
 import pytest
 import requests
+import yaml
 from requests.cookies import RequestsCookieJar
 
 from tavern._core import exceptions
 from tavern._core.extfunctions import update_from_ext
+from tavern._plugins.rest.files import get_file_arguments
 from tavern._plugins.rest.request import (
     RestRequest,
     _check_allow_redirects,
-    _get_file_arguments,
     _read_expected_cookies,
     get_request_args,
 )
 
 
 @pytest.fixture(name="req")
 def fix_example_request():
@@ -396,30 +398,30 @@
         return Mock(spec=ExitStack)
 
     def test_get_no_files(self, mock_stack, includes):
         """No files in request -> no files"""
 
         request_args = {}
 
-        assert _get_file_arguments(request_args, mock_stack, includes) == {}
+        assert get_file_arguments(request_args, mock_stack, includes) == {}
 
     def test_get_empty_files_list(self, mock_stack, includes):
         """No specific files specified -> no files"""
 
         request_args = {"files": {}}
 
-        assert _get_file_arguments(request_args, mock_stack, includes) == {}
+        assert get_file_arguments(request_args, mock_stack, includes) == {}
 
     def test_a_file(self, mock_stack, includes):
         """Json file should have the correct mimetype etc."""
 
         with tempfile.NamedTemporaryFile(suffix=".json") as tfile:
             request_args = {"files": {"file1": tfile.name}}
 
-            file_spec = _get_file_arguments(request_args, mock_stack, includes)
+            file_spec = get_file_arguments(request_args, mock_stack, includes)
 
         file = file_spec["files"]["file1"]
         assert file[0] == os.path.basename(tfile.name)
         assert file[2] == "application/json"
 
     def test_use_long_form_content_type(self, mock_stack, includes):
         """Use custom content type"""
@@ -431,15 +433,15 @@
                         "file_path": tfile.name,
                         "content_type": "abc123",
                         "content_encoding": "def456",
                     }
                 }
             }
 
-            file_spec = _get_file_arguments(request_args, mock_stack, includes)
+            file_spec = get_file_arguments(request_args, mock_stack, includes)
 
         file = file_spec["files"]["file1"]
         assert file[0] == os.path.basename(tfile.name)
         assert file[2] == "abc123"
         assert file[3] == {"Content-Encoding": "def456"}
 
     @pytest.mark.parametrize(
@@ -458,11 +460,57 @@
     def test_format_filename(self, mock_stack, includes, file_args):
         """Filenames should be formatted in short and long styles"""
 
         with tempfile.NamedTemporaryFile(suffix=".json") as tfile:
             includes.variables["tmpname"] = tfile.name
             request_args = {"files": {"file1": tfile.name}}
 
-            file_spec = _get_file_arguments(request_args, mock_stack, includes)
+            file_spec = get_file_arguments(request_args, mock_stack, includes)
 
         file = file_spec["files"]["file1"]
         assert file[0] == os.path.basename(tfile.name)
+
+    def test_grouped_file_names(self, mock_stack, includes):
+        """Parse grouped names appropriately"""
+        with tempfile.NamedTemporaryFile() as tfile:
+            raw_yaml_args = """
+                # Send file_1.txt and file_2.txt, both with name="input_files", in the multipart data.
+                - form_field_name: "input_files"
+                  file_path: "%FILENAME%"
+                  content_type: "application/customtype"
+                  content_encoding: "UTF16"
+                - form_field_name: "input_files"
+                  file_path: "%FILENAME%"
+                  content_type: "application/json"
+                """
+
+            raw_yaml_args = raw_yaml_args.replace("%FILENAME%", tfile.name)
+
+            file_args = yaml.safe_load(dedent(raw_yaml_args))
+
+            request_args = {"files": file_args}
+
+            parsed = get_file_arguments(request_args, mock_stack, includes)
+
+            parsed_into = {
+                "files": [
+                    (
+                        "input_files",
+                        (
+                            os.path.basename(tfile.name),
+                            mock_stack.enter_context.return_value,
+                            "application/customtype",
+                            {"Content-Encoding": "UTF16"},
+                        ),
+                    ),
+                    (
+                        "input_files",
+                        (
+                            os.path.basename(tfile.name),
+                            mock_stack.enter_context.return_value,
+                            "application/json",
+                        ),
+                    ),
+                ],
+            }
+
+        assert parsed_into == parsed
```

### Comparing `tavern-2.0.7/tests/unit/test_schema.py` & `tavern-2.1.0/tests/unit/test_schema.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/tests/unit/test_strict_util.py` & `tavern-2.1.0/tests/unit/test_strict_util.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/tests/unit/test_utilities.py` & `tavern-2.1.0/tests/unit/test_utilities.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/tox-integration.ini` & `tavern-2.1.0/tox-integration.ini`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     colorlog
     mqtt: fluent-logger
 commands =
 ;    docker-compose stop
 ;    docker-compose build
     docker-compose up --build -d
     python -m pytest --collect-only
-    python -m pytest --tavern-global-cfg={toxinidir}/tests/integration/global_cfg.yaml --cov tavern
+    python -m pytest --tavern-global-cfg={toxinidir}/tests/integration/global_cfg.yaml --cov tavern {posargs}
 
     generic: py.test --tavern-global-cfg={toxinidir}/tests/integration/global_cfg.yaml -n 3
     generic: tavern-ci --stdout . --tavern-global-cfg={toxinidir}/tests/integration/global_cfg.yaml
     generic: python -c "from tavern.core import run; exit(run('.', '{toxinidir}/tests/integration/global_cfg.yaml', pytest_args=[]))"
     generic: python -c "from tavern.core import run; exit(run('.', pytest_args=['--tavern-global-cfg={toxinidir}/tests/integration/global_cfg.yaml']))"
 
     cookies: tavern-ci --stdout test_server.tavern.yaml
```

### Comparing `tavern-2.0.7/tox.ini` & `tavern-2.1.0/tox.ini`

 * *Files identical despite different names*

### Comparing `tavern-2.0.7/PKG-INFO` & `tavern-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tavern
-Version: 2.0.7
+Version: 2.1.0
 Summary: Simple testing of RESTful APIs
 Keywords: testing,pytest
 Author: Michael Boulton
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -28,15 +28,15 @@
 Requires-Dist: stevedore>=4,<5
 Requires-Dist: Faker ; extra == "dev"
 Requires-Dist: allure-pytest ; extra == "dev"
 Requires-Dist: black==23.1.0 ; extra == "dev"
 Requires-Dist: bump2version ; extra == "dev"
 Requires-Dist: colorlog ; extra == "dev"
 Requires-Dist: docker-compose ; extra == "dev"
-Requires-Dist: flask ; extra == "dev"
+Requires-Dist: flask>=2.2.3 ; extra == "dev"
 Requires-Dist: fluent-logger ; extra == "dev"
 Requires-Dist: itsdangerous ; extra == "dev"
 Requires-Dist: mypy ; extra == "dev"
 Requires-Dist: mypy-extensions ; extra == "dev"
 Requires-Dist: coverage[toml] ; extra == "dev"
 Requires-Dist: types-PyYAML ; extra == "dev"
 Requires-Dist: flit >=3.2,<4 ; extra == "dev"
@@ -47,14 +47,16 @@
 Requires-Dist: ruff>=0.0.246 ; extra == "dev"
 Requires-Dist: pytest-xdist ; extra == "dev"
 Requires-Dist: py ; extra == "dev"
 Requires-Dist: tox>=3,<4 ; extra == "dev"
 Requires-Dist: tox-travis ; extra == "dev"
 Requires-Dist: twine ; extra == "dev"
 Requires-Dist: wheel ; extra == "dev"
+Requires-Dist: types-setuptools ; extra == "dev"
+Requires-Dist: types-requests ; extra == "dev"
 Project-URL: Documentation, https://tavern.readthedocs.io/en/latest/
 Project-URL: Home, https://taverntesting.github.io/
 Project-URL: Source, https://github.com/taverntesting/tavern
 Provides-Extra: dev
 
 [![pypi](https://img.shields.io/pypi/v/tavern.svg)](https://pypi.org/project/tavern/)
 [![docs](https://readthedocs.org/projects/pip/badge/?version=latest&style=flat)](https://tavern.readthedocs.io/en/latest/)
```

