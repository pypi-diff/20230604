# Comparing `tmp/jj-2.7.2.tar.gz` & `tmp/jj-2.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jj-2.7.2.tar", last modified: Sun Feb 26 15:49:56 2023, max compression
+gzip compressed data, was "jj-2.7.3.tar", last modified: Sun Jun  4 08:42:24 2023, max compression
```

## Comparing `jj-2.7.2.tar` & `jj-2.7.3.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 15:49:56.565441 jj-2.7.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-02-26 15:49:48.000000 jj-2.7.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14520 2023-02-26 15:49:56.565441 jj-2.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13899 2023-02-26 15:49:48.000000 jj-2.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 15:49:56.557441 jj-2.7.2/jj/
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-02-26 15:49:48.000000 jj-2.7.2/jj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-02-26 15:49:48.000000 jj-2.7.2/jj/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-02-26 15:49:48.000000 jj-2.7.2/jj/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 15:49:56.557441 jj-2.7.2/jj/apps/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-02-26 15:49:48.000000 jj-2.7.2/jj/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-02-26 15:49:48.000000 jj-2.7.2/jj/apps/_abstract_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-02-26 15:49:48.000000 jj-2.7.2/jj/apps/_base_app.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-02-26 15:49:48.000000 jj-2.7.2/jj/apps/_default_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 15:49:56.557441 jj-2.7.2/jj/expiration_policy/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-02-26 15:49:48.000000 jj-2.7.2/jj/expiration_policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-02-26 15:49:48.000000 jj-2.7.2/jj/expiration_policy/_expiration_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-02-26 15:49:48.000000 jj-2.7.2/jj/expiration_policy/_expire_after_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-02-26 15:49:48.000000 jj-2.7.2/jj/expiration_policy/_expire_never.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 15:49:56.557441 jj-2.7.2/jj/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-02-26 15:49:48.000000 jj-2.7.2/jj/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-02-26 15:49:48.000000 jj-2.7.2/jj/handlers/_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-02-26 15:49:48.000000 jj-2.7.2/jj/handlers/_handler_function.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 15:49:56.557441 jj-2.7.2/jj/http/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-02-26 15:49:48.000000 jj-2.7.2/jj/http/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 15:49:56.557441 jj-2.7.2/jj/http/codes/
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-02-26 15:49:48.000000 jj-2.7.2/jj/http/codes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 15:49:56.557441 jj-2.7.2/jj/http/headers/
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-02-26 15:49:48.000000 jj-2.7.2/jj/http/headers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 15:49:56.557441 jj-2.7.2/jj/http/methods/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-02-26 15:49:48.000000 jj-2.7.2/jj/http/methods/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 15:49:56.557441 jj-2.7.2/jj/logs/
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-02-26 15:49:48.000000 jj-2.7.2/jj/logs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-02-26 15:49:48.000000 jj-2.7.2/jj/logs/_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-02-26 15:49:48.000000 jj-2.7.2/jj/logs/_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 15:49:56.557441 jj-2.7.2/jj/logs/formatters/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-02-26 15:49:48.000000 jj-2.7.2/jj/logs/formatters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-02-26 15:49:48.000000 jj-2.7.2/jj/logs/formatters/_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-02-26 15:49:48.000000 jj-2.7.2/jj/logs/formatters/_simple_formatter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 15:49:56.557441 jj-2.7.2/jj/matchers/
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-02-26 15:49:48.000000 jj-2.7.2/jj/matchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-02-26 15:49:48.000000 jj-2.7.2/jj/matchers/_resolvable_matcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 15:49:56.561441 jj-2.7.2/jj/matchers/attribute_matchers/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-02-26 15:49:48.000000 jj-2.7.2/jj/matchers/attribute_matchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-02-26 15:49:48.000000 jj-2.7.2/jj/matchers/attribute_matchers/_attribute_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-02-26 15:49:48.000000 jj-2.7.2/jj/matchers/attribute_matchers/_contain_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-02-26 15:49:48.000000 jj-2.7.2/jj/matchers/attribute_matchers/_equal_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-02-26 15:49:48.000000 jj-2.7.2/jj/matchers/attribute_matchers/_exist_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-02-26 15:49:48.000000 jj-2.7.2/jj/matchers/attribute_matchers/_multi_dict_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-02-26 15:49:48.000000 jj-2.7.2/jj/matchers/attribute_matchers/_regex_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-02-26 15:49:48.000000 jj-2.7.2/jj/matchers/attribute_matchers/_route_matcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 15:49:56.561441 jj-2.7.2/jj/matchers/logical_matchers/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-02-26 15:49:48.000000 jj-2.7.2/jj/matchers/logical_matchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-02-26 15:49:48.000000 jj-2.7.2/jj/matchers/logical_matchers/_all_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-02-26 15:49:48.000000 jj-2.7.2/jj/matchers/logical_matchers/_any_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-02-26 15:49:48.000000 jj-2.7.2/jj/matchers/logical_matchers/_logical_matcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 15:49:56.561441 jj-2.7.2/jj/matchers/request_matchers/
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-02-26 15:49:48.000000 jj-2.7.2/jj/matchers/request_matchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-02-26 15:49:48.000000 jj-2.7.2/jj/matchers/request_matchers/_header_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-02-26 15:49:48.000000 jj-2.7.2/jj/matchers/request_matchers/_method_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-02-26 15:49:48.000000 jj-2.7.2/jj/matchers/request_matchers/_param_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-02-26 15:49:48.000000 jj-2.7.2/jj/matchers/request_matchers/_path_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-02-26 15:49:48.000000 jj-2.7.2/jj/matchers/request_matchers/_request_matcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 15:49:56.561441 jj-2.7.2/jj/middlewares/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-02-26 15:49:48.000000 jj-2.7.2/jj/middlewares/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-02-26 15:49:48.000000 jj-2.7.2/jj/middlewares/_abstract_middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-02-26 15:49:48.000000 jj-2.7.2/jj/middlewares/_base_middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-02-26 15:49:48.000000 jj-2.7.2/jj/middlewares/_logger_middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-02-26 15:49:48.000000 jj-2.7.2/jj/middlewares/_middleware_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-02-26 15:49:48.000000 jj-2.7.2/jj/middlewares/_root_middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-02-26 15:49:48.000000 jj-2.7.2/jj/middlewares/_self_middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 15:49:56.561441 jj-2.7.2/jj/mock/
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-02-26 15:49:48.000000 jj-2.7.2/jj/mock/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 15:49:56.565441 jj-2.7.2/jj/mock/_history/
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-02-26 15:49:48.000000 jj-2.7.2/jj/mock/_history/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-02-26 15:49:48.000000 jj-2.7.2/jj/mock/_history/_body_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-02-26 15:49:48.000000 jj-2.7.2/jj/mock/_history/_history_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-02-26 15:49:48.000000 jj-2.7.2/jj/mock/_history/_history_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-02-26 15:49:48.000000 jj-2.7.2/jj/mock/_history/_history_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-02-26 15:49:48.000000 jj-2.7.2/jj/mock/_history/_history_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-02-26 15:49:48.000000 jj-2.7.2/jj/mock/_history/_history_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-02-26 15:49:48.000000 jj-2.7.2/jj/mock/_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-02-26 15:49:48.000000 jj-2.7.2/jj/mock/_mocked.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-02-26 15:49:48.000000 jj-2.7.2/jj/mock/_remote_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-02-26 15:49:48.000000 jj-2.7.2/jj/mock/_remote_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-02-26 15:49:48.000000 jj-2.7.2/jj/mock/_remote_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-02-26 15:49:48.000000 jj-2.7.2/jj/mock/_stacked.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-02-26 15:49:48.000000 jj-2.7.2/jj/mock/_system_log_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-02-26 15:49:48.000000 jj-2.7.2/jj/mock/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-26 15:49:48.000000 jj-2.7.2/jj/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 15:49:56.565441 jj-2.7.2/jj/requests/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-02-26 15:49:48.000000 jj-2.7.2/jj/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-02-26 15:49:48.000000 jj-2.7.2/jj/requests/_request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 15:49:56.565441 jj-2.7.2/jj/resolvers/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-02-26 15:49:48.000000 jj-2.7.2/jj/resolvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-02-26 15:49:48.000000 jj-2.7.2/jj/resolvers/_matcher_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-02-26 15:49:48.000000 jj-2.7.2/jj/resolvers/_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-02-26 15:49:48.000000 jj-2.7.2/jj/resolvers/_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-02-26 15:49:48.000000 jj-2.7.2/jj/resolvers/_reversed_resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 15:49:56.565441 jj-2.7.2/jj/responses/
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-02-26 15:49:48.000000 jj-2.7.2/jj/responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-02-26 15:49:48.000000 jj-2.7.2/jj/responses/_relay_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-02-26 15:49:48.000000 jj-2.7.2/jj/responses/_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-02-26 15:49:48.000000 jj-2.7.2/jj/responses/_static_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-02-26 15:49:48.000000 jj-2.7.2/jj/responses/_stream_response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 15:49:56.565441 jj-2.7.2/jj/runners/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-02-26 15:49:48.000000 jj-2.7.2/jj/runners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-02-26 15:49:48.000000 jj-2.7.2/jj/runners/_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 15:49:56.565441 jj-2.7.2/jj/servers/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-02-26 15:49:48.000000 jj-2.7.2/jj/servers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-02-26 15:49:48.000000 jj-2.7.2/jj/servers/_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 15:49:56.557441 jj-2.7.2/jj.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14520 2023-02-26 15:49:56.000000 jj-2.7.2/jj.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-02-26 15:49:56.000000 jj-2.7.2/jj.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-26 15:49:56.000000 jj-2.7.2/jj.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-02-26 15:49:56.000000 jj-2.7.2/jj.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-02-26 15:49:56.000000 jj-2.7.2/jj.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-02-26 15:49:56.565441 jj-2.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-02-26 15:49:48.000000 jj-2.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 08:42:24.052106 jj-2.7.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-04 08:42:14.000000 jj-2.7.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14519 2023-06-04 08:42:24.052106 jj-2.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13898 2023-06-04 08:42:14.000000 jj-2.7.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 08:42:24.040105 jj-2.7.3/jj/
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-04 08:42:14.000000 jj-2.7.3/jj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-06-04 08:42:14.000000 jj-2.7.3/jj/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-04 08:42:14.000000 jj-2.7.3/jj/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 08:42:24.044106 jj-2.7.3/jj/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-04 08:42:14.000000 jj-2.7.3/jj/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-04 08:42:14.000000 jj-2.7.3/jj/apps/_abstract_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-06-04 08:42:14.000000 jj-2.7.3/jj/apps/_base_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-04 08:42:14.000000 jj-2.7.3/jj/apps/_default_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 08:42:24.044106 jj-2.7.3/jj/expiration_policy/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-04 08:42:14.000000 jj-2.7.3/jj/expiration_policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-04 08:42:14.000000 jj-2.7.3/jj/expiration_policy/_expiration_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-04 08:42:14.000000 jj-2.7.3/jj/expiration_policy/_expire_after_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-04 08:42:14.000000 jj-2.7.3/jj/expiration_policy/_expire_never.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 08:42:24.044106 jj-2.7.3/jj/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-04 08:42:14.000000 jj-2.7.3/jj/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-04 08:42:14.000000 jj-2.7.3/jj/handlers/_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-04 08:42:14.000000 jj-2.7.3/jj/handlers/_handler_function.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 08:42:24.044106 jj-2.7.3/jj/http/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-04 08:42:14.000000 jj-2.7.3/jj/http/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 08:42:24.044106 jj-2.7.3/jj/http/codes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-04 08:42:14.000000 jj-2.7.3/jj/http/codes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 08:42:24.044106 jj-2.7.3/jj/http/headers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-06-04 08:42:14.000000 jj-2.7.3/jj/http/headers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 08:42:24.044106 jj-2.7.3/jj/http/methods/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-04 08:42:14.000000 jj-2.7.3/jj/http/methods/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 08:42:24.044106 jj-2.7.3/jj/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-04 08:42:14.000000 jj-2.7.3/jj/logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-04 08:42:14.000000 jj-2.7.3/jj/logs/_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-04 08:42:14.000000 jj-2.7.3/jj/logs/_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 08:42:24.044106 jj-2.7.3/jj/logs/formatters/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-04 08:42:14.000000 jj-2.7.3/jj/logs/formatters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-04 08:42:14.000000 jj-2.7.3/jj/logs/formatters/_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-04 08:42:14.000000 jj-2.7.3/jj/logs/formatters/_simple_formatter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 08:42:24.044106 jj-2.7.3/jj/matchers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-06-04 08:42:14.000000 jj-2.7.3/jj/matchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-04 08:42:14.000000 jj-2.7.3/jj/matchers/_resolvable_matcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 08:42:24.048106 jj-2.7.3/jj/matchers/attribute_matchers/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-04 08:42:14.000000 jj-2.7.3/jj/matchers/attribute_matchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-04 08:42:14.000000 jj-2.7.3/jj/matchers/attribute_matchers/_attribute_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-04 08:42:14.000000 jj-2.7.3/jj/matchers/attribute_matchers/_contain_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-04 08:42:14.000000 jj-2.7.3/jj/matchers/attribute_matchers/_equal_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-04 08:42:14.000000 jj-2.7.3/jj/matchers/attribute_matchers/_exist_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-04 08:42:14.000000 jj-2.7.3/jj/matchers/attribute_matchers/_multi_dict_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-04 08:42:14.000000 jj-2.7.3/jj/matchers/attribute_matchers/_regex_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-06-04 08:42:14.000000 jj-2.7.3/jj/matchers/attribute_matchers/_route_matcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 08:42:24.048106 jj-2.7.3/jj/matchers/logical_matchers/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-04 08:42:14.000000 jj-2.7.3/jj/matchers/logical_matchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-06-04 08:42:14.000000 jj-2.7.3/jj/matchers/logical_matchers/_all_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-06-04 08:42:14.000000 jj-2.7.3/jj/matchers/logical_matchers/_any_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-04 08:42:14.000000 jj-2.7.3/jj/matchers/logical_matchers/_logical_matcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 08:42:24.048106 jj-2.7.3/jj/matchers/request_matchers/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-04 08:42:14.000000 jj-2.7.3/jj/matchers/request_matchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-06-04 08:42:14.000000 jj-2.7.3/jj/matchers/request_matchers/_header_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-06-04 08:42:14.000000 jj-2.7.3/jj/matchers/request_matchers/_method_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-06-04 08:42:14.000000 jj-2.7.3/jj/matchers/request_matchers/_param_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-04 08:42:14.000000 jj-2.7.3/jj/matchers/request_matchers/_path_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-04 08:42:14.000000 jj-2.7.3/jj/matchers/request_matchers/_request_matcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 08:42:24.048106 jj-2.7.3/jj/middlewares/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-04 08:42:14.000000 jj-2.7.3/jj/middlewares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-04 08:42:14.000000 jj-2.7.3/jj/middlewares/_abstract_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-04 08:42:14.000000 jj-2.7.3/jj/middlewares/_base_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-06-04 08:42:14.000000 jj-2.7.3/jj/middlewares/_logger_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-04 08:42:14.000000 jj-2.7.3/jj/middlewares/_middleware_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-04 08:42:14.000000 jj-2.7.3/jj/middlewares/_root_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-04 08:42:14.000000 jj-2.7.3/jj/middlewares/_self_middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 08:42:24.048106 jj-2.7.3/jj/mock/
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-06-04 08:42:14.000000 jj-2.7.3/jj/mock/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 08:42:24.052106 jj-2.7.3/jj/mock/_history/
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-04 08:42:14.000000 jj-2.7.3/jj/mock/_history/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-04 08:42:14.000000 jj-2.7.3/jj/mock/_history/_body_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-04 08:42:14.000000 jj-2.7.3/jj/mock/_history/_history_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-04 08:42:14.000000 jj-2.7.3/jj/mock/_history/_history_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-04 08:42:14.000000 jj-2.7.3/jj/mock/_history/_history_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-06-04 08:42:14.000000 jj-2.7.3/jj/mock/_history/_history_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-06-04 08:42:14.000000 jj-2.7.3/jj/mock/_history/_history_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-06-04 08:42:14.000000 jj-2.7.3/jj/mock/_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-06-04 08:42:14.000000 jj-2.7.3/jj/mock/_mocked.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-04 08:42:14.000000 jj-2.7.3/jj/mock/_remote_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-06-04 08:42:14.000000 jj-2.7.3/jj/mock/_remote_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-04 08:42:14.000000 jj-2.7.3/jj/mock/_remote_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-04 08:42:14.000000 jj-2.7.3/jj/mock/_stacked.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-04 08:42:14.000000 jj-2.7.3/jj/mock/_system_log_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-04 08:42:14.000000 jj-2.7.3/jj/mock/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 08:42:14.000000 jj-2.7.3/jj/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 08:42:24.052106 jj-2.7.3/jj/requests/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-04 08:42:14.000000 jj-2.7.3/jj/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-04 08:42:14.000000 jj-2.7.3/jj/requests/_request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 08:42:24.052106 jj-2.7.3/jj/resolvers/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-04 08:42:14.000000 jj-2.7.3/jj/resolvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-04 08:42:14.000000 jj-2.7.3/jj/resolvers/_matcher_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-06-04 08:42:14.000000 jj-2.7.3/jj/resolvers/_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-06-04 08:42:14.000000 jj-2.7.3/jj/resolvers/_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-04 08:42:14.000000 jj-2.7.3/jj/resolvers/_reversed_resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 08:42:24.052106 jj-2.7.3/jj/responses/
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-04 08:42:14.000000 jj-2.7.3/jj/responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-06-04 08:42:14.000000 jj-2.7.3/jj/responses/_relay_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-06-04 08:42:14.000000 jj-2.7.3/jj/responses/_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-04 08:42:14.000000 jj-2.7.3/jj/responses/_static_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-04 08:42:14.000000 jj-2.7.3/jj/responses/_stream_response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 08:42:24.052106 jj-2.7.3/jj/runners/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-04 08:42:14.000000 jj-2.7.3/jj/runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-06-04 08:42:14.000000 jj-2.7.3/jj/runners/_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 08:42:24.052106 jj-2.7.3/jj/servers/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-04 08:42:14.000000 jj-2.7.3/jj/servers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-06-04 08:42:14.000000 jj-2.7.3/jj/servers/_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 08:42:24.040105 jj-2.7.3/jj.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14519 2023-06-04 08:42:24.000000 jj-2.7.3/jj.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-06-04 08:42:24.000000 jj-2.7.3/jj.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 08:42:24.000000 jj-2.7.3/jj.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-04 08:42:24.000000 jj-2.7.3/jj.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-04 08:42:24.000000 jj-2.7.3/jj.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-04 08:42:24.052106 jj-2.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-04 08:42:14.000000 jj-2.7.3/setup.py
```

### Comparing `jj-2.7.2/LICENSE.txt` & `jj-2.7.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jj-2.7.2/PKG-INFO` & `jj-2.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jj
-Version: 2.7.2
+Version: 2.7.3
 Summary: Remote HTTP Mock
 Home-page: https://github.com/tsv1/jj
 Author: Nikita Tsvetkov
 Author-email: tsv1@fastmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
@@ -440,15 +440,15 @@
 from jj.mock import Mock
 
 jj.serve(Mock(), port=8080)
 ```
 
 or via docker
 ```shell
-docker run -p 8080:80 vedro-universe/jj
+docker run -p 8080:80 vedrouniverse/jj
 ```
 
 #### Client Side
 
 ```python
 import asyncio
```

### Comparing `jj-2.7.2/README.md` & `jj-2.7.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -421,15 +421,15 @@
 from jj.mock import Mock
 
 jj.serve(Mock(), port=8080)
 ```
 
 or via docker
 ```shell
-docker run -p 8080:80 vedro-universe/jj
+docker run -p 8080:80 vedrouniverse/jj
 ```
 
 #### Client Side
 
 ```python
 import asyncio
```

### Comparing `jj-2.7.2/jj/__init__.py` & `jj-2.7.3/jj/__init__.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.2/jj/_core.py` & `jj-2.7.3/jj/_core.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.2/jj/apps/_base_app.py` & `jj-2.7.3/jj/apps/_base_app.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.2/jj/expiration_policy/_expire_after_requests.py` & `jj-2.7.3/jj/expiration_policy/_expire_after_requests.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.2/jj/expiration_policy/_expire_never.py` & `jj-2.7.3/jj/expiration_policy/_expire_never.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.2/jj/http/codes/__init__.py` & `jj-2.7.3/jj/http/codes/__init__.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.2/jj/http/headers/__init__.py` & `jj-2.7.3/jj/http/headers/__init__.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.2/jj/logs/__init__.py` & `jj-2.7.3/jj/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.2/jj/logs/_filter.py` & `jj-2.7.3/jj/logs/_filter.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.2/jj/logs/formatters/_formatter.py` & `jj-2.7.3/jj/logs/formatters/_formatter.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.2/jj/matchers/__init__.py` & `jj-2.7.3/jj/matchers/__init__.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.2/jj/matchers/_resolvable_matcher.py` & `jj-2.7.3/jj/matchers/_resolvable_matcher.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.2/jj/matchers/attribute_matchers/__init__.py` & `jj-2.7.3/jj/matchers/attribute_matchers/__init__.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.2/jj/matchers/attribute_matchers/_contain_matcher.py` & `jj-2.7.3/jj/matchers/attribute_matchers/_contain_matcher.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.2/jj/matchers/attribute_matchers/_equal_matcher.py` & `jj-2.7.3/jj/matchers/attribute_matchers/_equal_matcher.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.2/jj/matchers/attribute_matchers/_multi_dict_matcher.py` & `jj-2.7.3/jj/matchers/attribute_matchers/_multi_dict_matcher.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.2/jj/matchers/attribute_matchers/_regex_matcher.py` & `jj-2.7.3/jj/matchers/attribute_matchers/_regex_matcher.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.2/jj/matchers/attribute_matchers/_route_matcher.py` & `jj-2.7.3/jj/matchers/attribute_matchers/_route_matcher.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.2/jj/matchers/logical_matchers/_all_matcher.py` & `jj-2.7.3/jj/matchers/logical_matchers/_all_matcher.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.2/jj/matchers/logical_matchers/_any_matcher.py` & `jj-2.7.3/jj/matchers/logical_matchers/_any_matcher.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.2/jj/matchers/request_matchers/_header_matcher.py` & `jj-2.7.3/jj/matchers/request_matchers/_header_matcher.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.2/jj/matchers/request_matchers/_method_matcher.py` & `jj-2.7.3/jj/matchers/request_matchers/_method_matcher.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.2/jj/matchers/request_matchers/_param_matcher.py` & `jj-2.7.3/jj/matchers/request_matchers/_param_matcher.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.2/jj/matchers/request_matchers/_path_matcher.py` & `jj-2.7.3/jj/matchers/request_matchers/_path_matcher.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.2/jj/middlewares/_abstract_middleware.py` & `jj-2.7.3/jj/middlewares/_abstract_middleware.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.2/jj/middlewares/_base_middleware.py` & `jj-2.7.3/jj/middlewares/_base_middleware.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.2/jj/middlewares/_logger_middleware.py` & `jj-2.7.3/jj/middlewares/_logger_middleware.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.2/jj/middlewares/_self_middleware.py` & `jj-2.7.3/jj/middlewares/_self_middleware.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.2/jj/mock/__init__.py` & `jj-2.7.3/jj/mock/__init__.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.2/jj/mock/_history/_body_parser.py` & `jj-2.7.3/jj/mock/_history/_body_parser.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.2/jj/mock/_history/_history_repository.py` & `jj-2.7.3/jj/mock/_history/_history_repository.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.2/jj/mock/_history/_history_request.py` & `jj-2.7.3/jj/mock/_history/_history_request.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.2/jj/mock/_history/_history_response.py` & `jj-2.7.3/jj/mock/_history/_history_response.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.2/jj/mock/_mock.py` & `jj-2.7.3/jj/mock/_mock.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.2/jj/mock/_mocked.py` & `jj-2.7.3/jj/mock/_mocked.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.2/jj/mock/_remote_handler.py` & `jj-2.7.3/jj/mock/_remote_handler.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.2/jj/mock/_remote_mock.py` & `jj-2.7.3/jj/mock/_remote_mock.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.2/jj/mock/_stacked.py` & `jj-2.7.3/jj/mock/_stacked.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.2/jj/mock/_utils.py` & `jj-2.7.3/jj/mock/_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import asyncio
 import threading
 from asyncio import Future
-from typing import Any, Awaitable, Callable, TypeVar
+from typing import Any, Callable, Coroutine, TypeVar
 
 __all__ = ("Thread",)
 
 T = TypeVar("T")
-TargetType = Callable[..., Awaitable[T]]
+TargetType = Callable[..., Coroutine[None, None, T]]
 
 
 class Thread(threading.Thread):
     def __init__(self, future: "Future[T]", target: TargetType[T],
                  *args: Any, **kwargs: Any) -> None:
         super().__init__()
         self._future = future
```

### Comparing `jj-2.7.2/jj/requests/_request.py` & `jj-2.7.3/jj/requests/_request.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.2/jj/resolvers/_registry.py` & `jj-2.7.3/jj/resolvers/_registry.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.2/jj/resolvers/_resolver.py` & `jj-2.7.3/jj/resolvers/_resolver.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.2/jj/responses/_relay_response.py` & `jj-2.7.3/jj/responses/_relay_response.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.2/jj/responses/_response.py` & `jj-2.7.3/jj/responses/_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,11 +126,11 @@
                      chunked: bool,
                      compression: Optional[ContentCoding],
                      **kwargs: Any) -> "Response":
         response = cls(status=status, reason=reason, headers=headers, body=body)  # type: ignore
         for cookie in cookies:
             response.set_cookie(**cookie)  # type: ignore
         if compression:
-            response.enable_compression(compression)
+            response.enable_compression(ContentCoding(compression))
         if chunked:
             response.enable_chunked_encoding()
         return response
```

### Comparing `jj-2.7.2/jj/responses/_static_response.py` & `jj-2.7.3/jj/responses/_static_response.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.2/jj/responses/_stream_response.py` & `jj-2.7.3/jj/responses/_stream_response.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.2/jj/runners/_runner.py` & `jj-2.7.3/jj/runners/_runner.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.2/jj/servers/_server.py` & `jj-2.7.3/jj/servers/_server.py`

 * *Files identical despite different names*

### Comparing `jj-2.7.2/jj.egg-info/PKG-INFO` & `jj-2.7.3/jj.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jj
-Version: 2.7.2
+Version: 2.7.3
 Summary: Remote HTTP Mock
 Home-page: https://github.com/tsv1/jj
 Author: Nikita Tsvetkov
 Author-email: tsv1@fastmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
@@ -440,15 +440,15 @@
 from jj.mock import Mock
 
 jj.serve(Mock(), port=8080)
 ```
 
 or via docker
 ```shell
-docker run -p 8080:80 vedro-universe/jj
+docker run -p 8080:80 vedrouniverse/jj
 ```
 
 #### Client Side
 
 ```python
 import asyncio
```

### Comparing `jj-2.7.2/jj.egg-info/SOURCES.txt` & `jj-2.7.3/jj.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jj-2.7.2/setup.cfg` & `jj-2.7.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 2.7.2
+current_version = 2.7.3
 message = bump version → {new_version}
 commit = True
 tag = True
 sign_tags = True
 
 [bumpversion:file:setup.py]
```

### Comparing `jj-2.7.2/setup.py` & `jj-2.7.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 def find_dev_required():
     with open("requirements-dev.txt") as f:
         return f.read().splitlines()
 
 
 setup(
     name="jj",
-    version="2.7.2",
+    version="2.7.3",
     description="Remote HTTP Mock",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Nikita Tsvetkov",
     author_email="tsv1@fastmail.com",
     python_requires=">=3.7.0",
     url="https://github.com/tsv1/jj",
```

