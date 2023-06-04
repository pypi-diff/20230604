# Comparing `tmp/flask-openapi3-2.4.0.tar.gz` & `tmp/flask-openapi3-2.4.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-openapi3-2.4.0.tar", last modified: Sun Jun  4 10:29:34 2023, max compression
+gzip compressed data, was "flask-openapi3-2.4.0rc1.tar", last modified: Wed May 31 09:01:07 2023, max compression
```

## Comparing `flask-openapi3-2.4.0.tar` & `flask-openapi3-2.4.0rc1.tar`

### file list

```diff
@@ -1,76 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 10:29:34.008916 flask-openapi3-2.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     7270 2023-06-04 10:29:23.000000 flask-openapi3-2.4.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-04 10:29:23.000000 flask-openapi3-2.4.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-04 10:29:23.000000 flask-openapi3-2.4.0/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-04 10:29:23.000000 flask-openapi3-2.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7538 2023-06-04 10:29:34.008916 flask-openapi3-2.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6446 2023-06-04 10:29:23.000000 flask-openapi3-2.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 10:29:33.992915 flask-openapi3-2.4.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-06-04 10:29:23.000000 flask-openapi3-2.4.0/examples/api_blueprint_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-06-04 10:29:23.000000 flask-openapi3-2.4.0/examples/api_view_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-04 10:29:23.000000 flask-openapi3-2.4.0/examples/async_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-06-04 10:29:23.000000 flask-openapi3-2.4.0/examples/custom_ui_templates_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-04 10:29:23.000000 flask-openapi3-2.4.0/examples/enum_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-04 10:29:23.000000 flask-openapi3-2.4.0/examples/header_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-04 10:29:23.000000 flask-openapi3-2.4.0/examples/image_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-06-04 10:29:23.000000 flask-openapi3-2.4.0/examples/init_oauth_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-04 10:29:23.000000 flask-openapi3-2.4.0/examples/just_flask.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-04 10:29:23.000000 flask-openapi3-2.4.0/examples/nested_apiblueprint_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-04 10:29:23.000000 flask-openapi3-2.4.0/examples/openapi_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-06-04 10:29:23.000000 flask-openapi3-2.4.0/examples/openapi_extra.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-06-04 10:29:23.000000 flask-openapi3-2.4.0/examples/orjson_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-06-04 10:29:23.000000 flask-openapi3-2.4.0/examples/pydantic_custom_root_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-06-04 10:29:23.000000 flask-openapi3-2.4.0/examples/response_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-06-04 10:29:23.000000 flask-openapi3-2.4.0/examples/rest_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-06-04 10:29:23.000000 flask-openapi3-2.4.0/examples/servers_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-04 10:29:23.000000 flask-openapi3-2.4.0/examples/simple_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-04 10:29:23.000000 flask-openapi3-2.4.0/examples/upload_file_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 10:29:33.996915 flask-openapi3-2.4.0/flask_openapi3/
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-04 10:29:23.000000 flask-openapi3-2.4.0/flask_openapi3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-04 10:29:23.000000 flask-openapi3-2.4.0/flask_openapi3/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8711 2023-06-04 10:29:23.000000 flask-openapi3-2.4.0/flask_openapi3/blueprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-06-04 10:29:23.000000 flask-openapi3-2.4.0/flask_openapi3/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-06-04 10:29:23.000000 flask-openapi3-2.4.0/flask_openapi3/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-06-04 10:29:23.000000 flask-openapi3-2.4.0/flask_openapi3/markdown.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 10:29:34.000916 flask-openapi3-2.4.0/flask_openapi3/models/
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-04 10:29:23.000000 flask-openapi3-2.4.0/flask_openapi3/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-06-04 10:29:23.000000 flask-openapi3-2.4.0/flask_openapi3/models/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-06-04 10:29:23.000000 flask-openapi3-2.4.0/flask_openapi3/models/component.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-04 10:29:23.000000 flask-openapi3-2.4.0/flask_openapi3/models/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-04 10:29:23.000000 flask-openapi3-2.4.0/flask_openapi3/models/info.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-04 10:29:23.000000 flask-openapi3-2.4.0/flask_openapi3/models/oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-06-04 10:29:23.000000 flask-openapi3-2.4.0/flask_openapi3/models/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-06-04 10:29:23.000000 flask-openapi3-2.4.0/flask_openapi3/models/security.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-04 10:29:23.000000 flask-openapi3-2.4.0/flask_openapi3/models/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-04 10:29:23.000000 flask-openapi3-2.4.0/flask_openapi3/models/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-04 10:29:23.000000 flask-openapi3-2.4.0/flask_openapi3/models/validation_error.py
--rw-r--r--   0 runner    (1001) docker     (123)    15621 2023-06-04 10:29:23.000000 flask-openapi3-2.4.0/flask_openapi3/openapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-06-04 10:29:23.000000 flask-openapi3-2.4.0/flask_openapi3/request.py
--rw-r--r--   0 runner    (1001) docker     (123)    25171 2023-06-04 10:29:23.000000 flask-openapi3-2.4.0/flask_openapi3/scaffold.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 10:29:34.000916 flask-openapi3-2.4.0/flask_openapi3/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-06-04 10:29:23.000000 flask-openapi3-2.4.0/flask_openapi3/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 10:29:33.984914 flask-openapi3-2.4.0/flask_openapi3/templates/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 10:29:34.000916 flask-openapi3-2.4.0/flask_openapi3/templates/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)   144726 2023-06-04 10:29:23.000000 flask-openapi3-2.4.0/flask_openapi3/templates/static/css/swagger-ui.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 10:29:34.004916 flask-openapi3-2.4.0/flask_openapi3/templates/static/images/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-04 10:29:23.000000 flask-openapi3-2.4.0/flask_openapi3/templates/static/images/apidoc.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-06-04 10:29:23.000000 flask-openapi3-2.4.0/flask_openapi3/templates/static/images/rapidoc.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-06-04 10:29:23.000000 flask-openapi3-2.4.0/flask_openapi3/templates/static/images/redoc.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-06-04 10:29:23.000000 flask-openapi3-2.4.0/flask_openapi3/templates/static/images/swagger.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 10:29:34.008916 flask-openapi3-2.4.0/flask_openapi3/templates/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)   620595 2023-06-04 10:29:23.000000 flask-openapi3-2.4.0/flask_openapi3/templates/static/js/rapidoc-min.js
--rw-r--r--   0 runner    (1001) docker     (123)  1042510 2023-06-04 10:29:23.000000 flask-openapi3-2.4.0/flask_openapi3/templates/static/js/redoc.standalone.js
--rw-r--r--   0 runner    (1001) docker     (123)  1061567 2023-06-04 10:29:23.000000 flask-openapi3-2.4.0/flask_openapi3/templates/static/js/swagger-ui-bundle.js
--rw-r--r--   0 runner    (1001) docker     (123)   312217 2023-06-04 10:29:23.000000 flask-openapi3-2.4.0/flask_openapi3/templates/static/js/swagger-ui-standalone-preset.js
--rw-r--r--   0 runner    (1001) docker     (123)    20601 2023-06-04 10:29:23.000000 flask-openapi3-2.4.0/flask_openapi3/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9637 2023-06-04 10:29:23.000000 flask-openapi3-2.4.0/flask_openapi3/view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 10:29:33.996915 flask-openapi3-2.4.0/flask_openapi3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7538 2023-06-04 10:29:33.000000 flask-openapi3-2.4.0/flask_openapi3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-06-04 10:29:33.000000 flask-openapi3-2.4.0/flask_openapi3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 10:29:33.000000 flask-openapi3-2.4.0/flask_openapi3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 10:29:33.000000 flask-openapi3-2.4.0/flask_openapi3.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-04 10:29:33.000000 flask-openapi3-2.4.0/flask_openapi3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-04 10:29:33.000000 flask-openapi3-2.4.0/flask_openapi3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-04 10:29:23.000000 flask-openapi3-2.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 10:29:34.008916 flask-openapi3-2.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-06-04 10:29:23.000000 flask-openapi3-2.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:01:07.896657 flask-openapi3-2.4.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)     6517 2023-05-31 09:00:57.000000 flask-openapi3-2.4.0rc1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-31 09:00:57.000000 flask-openapi3-2.4.0rc1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-31 09:00:57.000000 flask-openapi3-2.4.0rc1/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-31 09:00:57.000000 flask-openapi3-2.4.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7541 2023-05-31 09:01:07.896657 flask-openapi3-2.4.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6446 2023-05-31 09:00:57.000000 flask-openapi3-2.4.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:01:07.888656 flask-openapi3-2.4.0rc1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/examples/api_blueprint_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/examples/api_view_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/examples/async_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/examples/custom_ui_templates_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/examples/enum_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/examples/header_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/examples/image_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/examples/init_oauth_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/examples/just_flask.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/examples/nested_apiblueprint_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/examples/openapi_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/examples/orjson_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/examples/pydantic_custom_root_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/examples/response_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/examples/rest_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/examples/servers_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/examples/simple_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/examples/upload_file_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:01:07.888656 flask-openapi3-2.4.0rc1/flask_openapi3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8021 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/blueprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/markdown.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:01:07.888656 flask-openapi3-2.4.0rc1/flask_openapi3/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/models/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/models/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/models/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/models/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/models/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/models/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/models/security.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/models/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/models/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/models/validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13480 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/openapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20928 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/scaffold.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:01:07.888656 flask-openapi3-2.4.0rc1/flask_openapi3/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:01:07.884657 flask-openapi3-2.4.0rc1/flask_openapi3/templates/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:01:07.888656 flask-openapi3-2.4.0rc1/flask_openapi3/templates/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   144726 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/templates/static/css/swagger-ui.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:01:07.892657 flask-openapi3-2.4.0rc1/flask_openapi3/templates/static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/templates/static/images/apidoc.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/templates/static/images/rapidoc.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/templates/static/images/redoc.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/templates/static/images/swagger.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:01:07.892657 flask-openapi3-2.4.0rc1/flask_openapi3/templates/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)   620595 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/templates/static/js/rapidoc-min.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1042510 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/templates/static/js/redoc.standalone.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1061567 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/templates/static/js/swagger-ui-bundle.js
+-rw-r--r--   0 runner    (1001) docker     (123)   312217 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/templates/static/js/swagger-ui-standalone-preset.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15713 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8499 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:01:07.888656 flask-openapi3-2.4.0rc1/flask_openapi3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7541 2023-05-31 09:01:07.000000 flask-openapi3-2.4.0rc1/flask_openapi3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-05-31 09:01:07.000000 flask-openapi3-2.4.0rc1/flask_openapi3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 09:01:07.000000 flask-openapi3-2.4.0rc1/flask_openapi3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 09:01:07.000000 flask-openapi3-2.4.0rc1/flask_openapi3.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-31 09:01:07.000000 flask-openapi3-2.4.0rc1/flask_openapi3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-31 09:01:07.000000 flask-openapi3-2.4.0rc1/flask_openapi3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 09:01:07.896657 flask-openapi3-2.4.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/setup.py
```

### Comparing `flask-openapi3-2.4.0/CHANGELOG.md` & `flask-openapi3-2.4.0rc1/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,12 @@
-## v2.4.0 2023-06-04
+## v2.4.0 2023-??-??
 
 - [#72](https://github.com/luolingchun/flask-openapi3/pull/72) security_schemes(SecurityScheme) supports a json format.
 - [#68](https://github.com/luolingchun/flask-openapi3/pull/68) feat: Add operation_id_callback. Thanks, @BoyanYK.
-- [#64](https://github.com/luolingchun/flask-openapi3/pull/64) Explains the usage of flask openapi command more clearly. Thanks, @candleindark.
-- [#75](https://github.com/luolingchun/flask-openapi3/pull/75) Init view_class and pass view_kwargs. Thanks, @stufisher.
-- [#70](https://github.com/luolingchun/flask-openapi3/issues/70) Support for Specification Extensions in OpenAPI Object and Operation Object. Thanks, @simonblund.
-- [#73](https://github.com/luolingchun/flask-openapi3/issues/73) BaseModel Config support openapi_extra.
-- Merge `extra_responses` to `responses` and deprecate `extra_responses`.
-
-**DeprecationWarning:**
-
-- Add DeprecationWarning to `APIKey`, `HTTPBase`, `OAuth2`, `OpenIdConnect`, `HTTPBearer` that will be deprecated in v3.0.
-- Add DeprecationWarning to `extra_form`, `extra_body` and `extra_responses` that will be deprecated in v3.0.
+- Add DeprecationWarning to APIKey, HTTPBase, OAuth2, OpenIdConnect, HTTPBearer that will be deprecated in v3.0.
 
 
 ## v2.3.2 2023-04-03
 
 - [#61](https://github.com/luolingchun/flask-openapi3/issues/61) Fix headers with pydantic alias
 
 ## v2.3.1 2023-02-13
```

### Comparing `flask-openapi3-2.4.0/CONTRIBUTING.md` & `flask-openapi3-2.4.0rc1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.4.0/LICENSE.rst` & `flask-openapi3-2.4.0rc1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.4.0/PKG-INFO` & `flask-openapi3-2.4.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-openapi3
-Version: 2.4.0
+Version: 2.4.0rc1
 Summary: Generate REST API and OpenAPI documentation for your Flask project.
 Home-page: https://github.com/luolingchun/flask-openapi3
 Author: llc
 Author-email: luolingchun@outlook.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `flask-openapi3-2.4.0/README.md` & `flask-openapi3-2.4.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.4.0/examples/api_blueprint_demo.py` & `flask-openapi3-2.4.0rc1/examples/api_blueprint_demo.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
 
 @api.get('/book', doc_ui=False)
 def get_book():
     return {"code": 0, "message": "ok"}
 
 
-@api.post('/book', responses={"200": {"content": {"text/csv": {"schema": {"type": "string"}}}}})
+@api.post('/book', extra_responses={"200": {"content": {"text/csv": {"schema": {"type": "string"}}}}})
 def create_book(body: BookBody):
     assert body.age == 3
     return {"code": 0, "message": "ok"}
 
 
 @api.put('/book/<int:bid>', operation_id='update')
 def update_book(path: Path, body: BookBody):
```

### Comparing `flask-openapi3-2.4.0/examples/api_view_demo.py` & `flask-openapi3-2.4.0rc1/examples/api_view_demo.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.4.0/examples/async_demo.py` & `flask-openapi3-2.4.0rc1/examples/async_demo.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.4.0/examples/custom_ui_templates_demo.py` & `flask-openapi3-2.4.0rc1/examples/custom_ui_templates_demo.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.4.0/examples/enum_demo.py` & `flask-openapi3-2.4.0rc1/examples/enum_demo.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.4.0/examples/header_demo.py` & `flask-openapi3-2.4.0rc1/examples/header_demo.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.4.0/examples/init_oauth_demo.py` & `flask-openapi3-2.4.0rc1/examples/init_oauth_demo.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.4.0/examples/nested_apiblueprint_demo.py` & `flask-openapi3-2.4.0rc1/examples/nested_apiblueprint_demo.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.4.0/examples/openapi_extensions.py` & `flask-openapi3-2.4.0rc1/examples/openapi_extensions.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.4.0/examples/orjson_demo.py` & `flask-openapi3-2.4.0rc1/examples/orjson_demo.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.4.0/examples/pydantic_custom_root_types.py` & `flask-openapi3-2.4.0rc1/examples/pydantic_custom_root_types.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.4.0/examples/response_demo.py` & `flask-openapi3-2.4.0rc1/examples/response_demo.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,54 +1,34 @@
 # -*- coding: utf-8 -*-
-# @Author  : llc
+# @Author  : [martinatseequent](https://github.com/martinatseequent)
 # @Time    : 2021/6/22 9:32
 
 import json
 from http import HTTPStatus
 
 from flask import make_response
 from pydantic import BaseModel, Field
 
 from flask_openapi3 import Info
 from flask_openapi3 import OpenAPI, APIBlueprint
 
-app = OpenAPI(__name__, info=Info(title="Hello API", version="1.0.0"))
+app = OpenAPI(__name__, info=Info(title="Hello API", version="1.0.0"), )
 
 bp = APIBlueprint("Hello BP", __name__)
 
 
 class HelloPath(BaseModel):
     name: str = Field(..., description="The name")
 
 
 class Message(BaseModel):
     message: str = Field(..., description="The message")
 
-    class Config:
-        openapi_extra = {
-            # "example": {"message": "aaa"},
-            "examples": {
-                "example1": {
-                    "summary": "example1 summary",
-                    "value": {
-                        "message": "bbb"
-                    }
-                },
-                "example2": {
-                    "summary": "example2 summary",
-                    "value": {
-                        "message": "ccc"
-                    }
-                }
-            }
-        }
 
-
-@bp.get("/hello/<string:name>",
-        responses={"200": Message, "201": {"content": {"text/csv": {"schema": {"type": "string"}}}}})
+@bp.get("/hello/<string:name>", responses={"200": Message})
 def hello(path: HelloPath):
     message = {"message": f"""Hello {path.name}!"""}
 
     response = make_response(json.dumps(message), HTTPStatus.OK)
     # response = make_response("sss", HTTPStatus.OK)
     response.mimetype = "application/json"
     return response
```

### Comparing `flask-openapi3-2.4.0/examples/rest_demo.py` & `flask-openapi3-2.4.0rc1/examples/rest_demo.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # @Author  : llc
 # @Time    : 2021/4/28 11:24
 from http import HTTPStatus
 from typing import Optional, List
 
 from pydantic import BaseModel, Field
 
-from flask_openapi3 import ExternalDocumentation
+from flask_openapi3 import ExternalDocumentation, ExtraRequestBody, Example
 from flask_openapi3 import Info, Tag, Server
 from flask_openapi3 import OpenAPI
 
 info = Info(title='book API', version='1.0.0')
 
 # Basic Authentication Sample
 basic = {
@@ -91,15 +91,17 @@
     tags=[book_tag],
     summary='new summary',
     description='new description',
     operation_id="get_book_id",
     external_docs=ExternalDocumentation(
         url="https://www.openapis.org/",
         description="Something great got better, get excited!"),
+
     responses={"200": BookResponse},
+    extra_responses={"200": {"content": {"text/csv": {"schema": {"type": "string"}}}}},
     security=security,
     servers=[Server(url="https://www.openapis.org/", description="openapi")]
 )
 def get_book(path: BookPath):
     """Get a book
     to Get some book by id, like:
     http://localhost:5000/book/3
@@ -122,15 +124,40 @@
         "data": [
             {"bid": 1, "age": query.age, "author": 'a1'},
             {"bid": 2, "age": query.age, "author": 'a2'}
         ]
     }
 
 
-@app.post('/book', tags=[book_tag], responses={"200": BookResponse})
+extra_body = ExtraRequestBody(
+    description="This is post RequestBody",
+    required=True,
+    example="ttt",
+    examples={
+        "example1": Example(
+            summary="example summary1",
+            description="example description1",
+            value={
+                "age": 24,
+                "author": "author1"
+            }
+        ),
+        "example2": Example(
+            summary="example summary2",
+            description="example description2",
+            value={
+                "age": 48,
+                "author": "author2"
+            }
+        )
+    }
+)
+
+
+@app.post('/book', tags=[book_tag], responses={"200": BookResponse}, extra_body=extra_body)
 def create_book(body: BookBody):
     print(body)
     return {"code": 0, "message": "ok"}, HTTPStatus.OK
 
 
 @app.put('/book/<int:bid>', tags=[book_tag])
 def update_book(path: BookPath, body: BookBody):
```

### Comparing `flask-openapi3-2.4.0/examples/servers_demo.py` & `flask-openapi3-2.4.0rc1/examples/servers_demo.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.4.0/examples/simple_demo.py` & `flask-openapi3-2.4.0rc1/examples/simple_demo.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.4.0/examples/upload_file_demo.py` & `flask-openapi3-2.4.0rc1/examples/upload_file_demo.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 # @Author  : llc
 # @Time    : 2021/5/11 14:03
 
 from typing import List
 
 from pydantic import BaseModel, Field
 
-from flask_openapi3 import OpenAPI, FileStorage
+from flask_openapi3 import OpenAPI, FileStorage, ExtraRequestBody
+from flask_openapi3 import Encoding
 
 app = OpenAPI(__name__)
 
 
 class UploadFileForm(BaseModel):
     file: FileStorage
     file_type: str = Field(None, description="File Type")
@@ -18,23 +19,31 @@
 
 class UploadFilesForm(BaseModel):
     files: List[FileStorage]
     str_list: List[str]
     int_list: List[int]
 
 
+extra_form = ExtraRequestBody(
+    description="This is form RequestBody",
+    required=True,
+    # replace style (default to form)
+    encoding={"str_list": Encoding(style="simple")}
+)
+
+
 @app.post('/upload/file')
 def upload_file(form: UploadFileForm):
     print(form.file.filename)
     print(form.file_type)
     form.file.save('test.jpg')
     return {"code": 0, "message": "ok"}
 
 
-@app.post('/upload/files')
+@app.post('/upload/files', extra_form=extra_form)
 def upload_files(form: UploadFilesForm):
     print(form.files)
     print(form.str_list)
     print(form.int_list)
     return {"code": 0, "message": "ok"}
```

### Comparing `flask-openapi3-2.4.0/flask_openapi3/__init__.py` & `flask-openapi3-2.4.0rc1/flask_openapi3/__init__.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.4.0/flask_openapi3/blueprint.py` & `flask-openapi3-2.4.0rc1/flask_openapi3/blueprint.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 # @Author  : llc
 # @Time    : 2022/4/1 16:54
 import re
 from copy import deepcopy
-from typing import Optional, List, Dict, Any, Type, Callable, Tuple, Union
+from typing import Optional, List, Dict, Any, Type, Callable, Tuple
 
 from flask import Blueprint
 from pydantic import BaseModel
 
 from .http import HTTPMethod
 from .models import Tag, ExternalDocumentation
 from .models.common import ExtraRequestBody
@@ -21,174 +21,159 @@
     def __init__(
             self,
             name: str,
             import_name: str,
             *,
             abp_tags: Optional[List[Tag]] = None,
             abp_security: Optional[List[Dict[str, List[str]]]] = None,
-            abp_responses: Optional[Dict[str, Union[Type[BaseModel], Dict[Any, Any], None]]] = None,
+            abp_responses: Optional[Dict[str, Optional[Type[BaseModel]]]] = None,
             doc_ui: bool = True,
             operation_id_callback: Callable = get_operation_id_for_path,
             **kwargs: Any
     ) -> None:
         """
         Based on Flask Blueprint
 
         Arguments:
             name: The name of the blueprint. It Will be prepared to each endpoint name.
-            import_name: The name of the blueprint package, usually ``__name__``.
-                         This helps locate the ``root_path`` for the blueprint.
-            abp_tags: APIBlueprint tags for every API.
-            abp_security: APIBlueprint security for every API.
-            abp_responses: API responses should be either a subclass of BaseModel, a dictionary, or None.
-            doc_ui: Enable OpenAPI document UI (Swagger UI, Redoc and Rapidoc). Defaults to True.
+            import_name: The name of the blueprint package, usually
+                         ``__name__``. This helps locate the ``root_path`` for the blueprint.
+            abp_tags: APIBlueprint tags for every api
+            abp_security: APIBlueprint security for every api
+            abp_responses: APIBlueprint response model
+            doc_ui: Add openapi document UI(swagger, rapidoc and redoc). Defaults to True.
             operation_id_callback: Callback function for custom operation_id generation.
-                                   Receives name (str), path (str) and method (str) parameters.
-                                   Defaults to `get_operation_id_for_path` from utils
+                Receives name (str), path (str) and method (str) parameters.
+                Defaults to `get_operation_id_for_path` from utils
             **kwargs: Flask Blueprint kwargs
         """
         super(APIBlueprint, self).__init__(name, import_name, **kwargs)
-
-        # Initialize instance variables
         self.paths: Dict = dict()
         self.components_schemas: Dict = dict()
         self.tags: List[Tag] = []
         self.tag_names: List[str] = []
 
-        # Set values from arguments or default values
         self.abp_tags = abp_tags or []
         self.abp_security = abp_security or []
         self.abp_responses = abp_responses or {}
         self.doc_ui = doc_ui
-
-        # Set the operation ID callback function
         self.operation_id_callback: Callable = operation_id_callback
 
     def register_api(self, api: "APIBlueprint") -> None:
         """Register a nested APIBlueprint"""
-
-        # Check if the APIBlueprint is being registered on itself
         if api is self:
             raise ValueError("Cannot register a api blueprint on itself")
 
-        # Merge tags from the nested APIBlueprint
         for tag in api.tags:
             if tag.name not in self.tag_names:
                 self.tags.append(tag)
 
-        # Merge paths from the nested APIBlueprint
         for path_url, path_item in api.paths.items():
             trail_slash = path_url.endswith("/")
-
-            # Merge url_prefix and new API blueprint path url
+            # merge url_prefix and new api blueprint path url
             uri = self.url_prefix.rstrip("/") + "/" + path_url.lstrip("/") if self.url_prefix else path_url
-
-            # Strip the right slash
+            # strip the right slash
             if not trail_slash:
                 uri = uri.rstrip("/")
-
             self.paths[uri] = path_item
 
-        # Merge component schemas from the nested APIBlueprint
         self.components_schemas.update(**api.components_schemas)
 
-        # Register the nested APIBlueprint as a blueprint
         self.register_blueprint(api)
 
     def _do_decorator(
             self,
             rule: str,
             func: Callable,
             *,
             tags: Optional[List[Tag]] = None,
             summary: Optional[str] = None,
             description: Optional[str] = None,
             external_docs: Optional[ExternalDocumentation] = None,
             operation_id: Optional[str] = None,
             extra_form: Optional[ExtraRequestBody] = None,
             extra_body: Optional[ExtraRequestBody] = None,
-            responses: Optional[Dict[str, Union[Type[BaseModel], Dict[Any, Any], None]]] = None,
+            responses: Optional[Dict[str, Optional[Type[BaseModel]]]] = None,
             extra_responses: Optional[Dict[str, Dict]] = None,
             deprecated: Optional[bool] = None,
             security: Optional[List[Dict[str, List[Any]]]] = None,
             servers: Optional[List[Server]] = None,
             openapi_extensions: Optional[Dict[str, Any]] = None,
             doc_ui: bool = True,
             method: str = HTTPMethod.GET
     ) -> Tuple[Type[BaseModel], Type[BaseModel], Type[BaseModel], Type[BaseModel], Type[BaseModel], Type[BaseModel]]:
         """
-        Collects OpenAPI specification information for Flask routes and view functions.
-
+        Collect openapi specification information
         Arguments:
             rule: Flask route
             func: Flask view_func
             tags: Adds metadata to a single tag.
             summary: A short summary of what the operation does.
             description: A verbose explanation of the operation behavior.
             external_docs: Additional external documentation for this operation.
             operation_id: Unique string used to identify the operation.
             extra_form: Extra information describing the request body(application/form).
             extra_body: Extra information describing the request body(application/json).
-            responses: API responses should be either a subclass of BaseModel, a dictionary, or None.
+            responses: response's model must be pydantic BaseModel.
             extra_responses: Extra information for responses.
             deprecated: Declares this operation to be deprecated.
             security: A declaration of which security mechanisms can be used for this operation.
             servers: An alternative server array to service this operation.
             openapi_extensions: Allows extensions to the OpenAPI Schema.
             doc_ui: Add openapi document UI(swagger, rapidoc and redoc). Defaults to True.
         """
         if self.doc_ui is True and doc_ui is True:
             if responses is None:
                 responses = {}
             if extra_responses is None:
                 extra_responses = {}
-            # Global response: combine API responses
+            # global response combine api responses
             combine_responses = deepcopy(self.abp_responses)
             combine_responses.update(**responses)
-            # Create operation
+            # create operation
             operation = get_operation(
                 func,
                 summary=summary,
                 description=description,
                 openapi_extensions=openapi_extensions
             )
-            # Set external docs
+            # set external docs
             operation.externalDocs = external_docs
             # Unique string used to identify the operation.
             operation.operationId = operation_id or self.operation_id_callback(
                 name=func.__name__, path=rule, method=method
             )
-            # Only set `deprecated` if True, otherwise leave it as None
+            # only set `deprecated` if True otherwise leave it as None
             operation.deprecated = deprecated
-            # Add security
+            # add security
             if security is None:
                 security = []
             operation.security = security + self.abp_security or None
-            # Add servers
+            # add servers
             operation.servers = servers
-            # Store tags
+            # store tags
             tags = tags + self.abp_tags if tags else self.abp_tags
             parse_and_store_tags(tags, self.tags, self.tag_names, operation)
-            # Parse parameters
+            # parse parameters
             header, cookie, path, query, form, body = parse_parameters(
                 func,
                 extra_form=extra_form,
                 extra_body=extra_body,
                 components_schemas=self.components_schemas,
                 operation=operation
             )
-            # Parse response
+            # parse response
             get_responses(combine_responses, extra_responses, self.components_schemas, operation)
-            # Convert route parameter format from /pet/<petId> to /pet/{petId}
+            # /pet/<petId> --> /pet/{petId}
             uri = re.sub(r"<([^<:]+:)?", "{", rule).replace(">", "}")
             trail_slash = uri.endswith("/")
-            # Merge url_prefix and uri
+            # merge url_prefix and uri
             uri = self.url_prefix.rstrip("/") + "/" + uri.lstrip("/") if self.url_prefix else uri
             if not trail_slash:
                 uri = uri.rstrip("/")
-            # Parse method
+            # parse method
             parse_method(uri, method, self.paths, operation)
             return header, cookie, path, query, form, body
         else:
-            # Parse parameters
+            # parse parameters
             header, cookie, path, query, form, body = parse_parameters(func, doc_ui=False)
             return header, cookie, path, query, form, body
```

### Comparing `flask-openapi3-2.4.0/flask_openapi3/commands.py` & `flask-openapi3-2.4.0rc1/flask_openapi3/commands.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,39 +6,33 @@
 from flask import current_app
 from flask.cli import click
 from flask.cli import with_appcontext
 
 from .markdown import openapi_to_markdown
 
 
-@click.command(name="openapi")
-@click.option("--output", "-o", type=click.Path(), help="The output file path.")
-@click.option("--format", "-f", type=click.Choice(["json", "yaml", "markdown"]), help="The output file format.")
-@click.option("--indent", "-i", type=int, help="The indentation for JSON dumps.")
-@click.option("--ensure_ascii", "-a", is_flag=True, help="Ensure ASCII characters or not. Defaults to False.")
+@click.command(name='openapi')
+@click.option('--output', '-o', type=click.Path(), help='The output file path.')
+@click.option('--format', '-f', type=click.Choice(['json', 'yaml', 'markdown']), help='The output file format.')
+@click.option('--indent', '-i', type=int, help='The indentation for JSON dumps.')
+@click.option('--ensure_ascii', '-a', is_flag=True, help='Ensure ASCII characters or not. Defaults to False.')
 @with_appcontext
 def openapi_command(output, format, indent, ensure_ascii):
     """Export the OpenAPI Specification to console or a file"""
-
-    # Check if the current app has an api_doc attribute
-    if hasattr(current_app, "api_doc"):
+    if hasattr(current_app, 'api_doc'):
         obj = current_app.api_doc
-
-        # Generate the OpenAPI Specification based on the specified format
-        if format == "yaml":
+        if format == 'yaml':
             try:
                 import yaml  # type: ignore
             except ImportError:
                 raise ImportError("pyyaml must be installed.")
             openapi = yaml.safe_dump(obj, allow_unicode=True)
-        elif format == "markdown":
+        elif format == 'markdown':
             openapi = openapi_to_markdown(obj)
         else:
             openapi = json.dumps(obj, indent=indent, ensure_ascii=ensure_ascii)
-
-        # Save the OpenAPI Specification to a file if the output path is provided
         if output:
-            with open(output, "w", encoding="utf8") as f:
+            with open(output, 'w', encoding='utf8') as f:
                 f.write(openapi)
             click.echo(f"Saved to {output}.")
         else:
             click.echo(openapi)
```

### Comparing `flask-openapi3-2.4.0/flask_openapi3/http.py` & `flask-openapi3-2.4.0rc1/flask_openapi3/http.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.4.0/flask_openapi3/markdown.py` & `flask-openapi3-2.4.0rc1/flask_openapi3/markdown.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.4.0/flask_openapi3/models/__init__.py` & `flask-openapi3-2.4.0rc1/flask_openapi3/models/__init__.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.4.0/flask_openapi3/models/common.py` & `flask-openapi3-2.4.0rc1/flask_openapi3/models/common.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 # -*- coding: utf-8 -*-
 # @Author  : llc
 # @Time    : 2021/4/30 11:46
-import warnings
 from typing import Optional, List, Any, Union, Dict
 
 from pydantic import BaseModel, Field
 
-warnings.simplefilter("once")
-
 
 class ExternalDocumentation(BaseModel):
     description: Optional[str] = None
     url: str
 
     class Config:
         extra = "allow"
@@ -128,11 +125,7 @@
 class ExtraRequestBody(BaseModel):
     description: Optional[str] = None
     required: Optional[bool] = True
     # For MediaType
     example: Optional[Any] = None
     examples: Optional[Dict[str, Union[Example, Reference]]] = None
     encoding: Optional[Dict[str, Encoding]] = None
-
-    def __new__(cls, *args, **kwargs):
-        warnings.warn(f"""\n{cls.__name__} will be deprecated in v3.x.""", DeprecationWarning)
-        return super().__new__(cls)
```

### Comparing `flask-openapi3-2.4.0/flask_openapi3/models/component.py` & `flask-openapi3-2.4.0rc1/flask_openapi3/models/component.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.4.0/flask_openapi3/models/file.py` & `flask-openapi3-2.4.0rc1/flask_openapi3/models/file.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.4.0/flask_openapi3/models/info.py` & `flask-openapi3-2.4.0rc1/flask_openapi3/models/info.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.4.0/flask_openapi3/models/oauth.py` & `flask-openapi3-2.4.0rc1/flask_openapi3/models/oauth.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.4.0/flask_openapi3/models/path.py` & `flask-openapi3-2.4.0rc1/flask_openapi3/models/path.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.4.0/flask_openapi3/models/security.py` & `flask-openapi3-2.4.0rc1/flask_openapi3/models/security.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.4.0/flask_openapi3/models/server.py` & `flask-openapi3-2.4.0rc1/flask_openapi3/models/server.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.4.0/flask_openapi3/models/validation_error.py` & `flask-openapi3-2.4.0rc1/flask_openapi3/models/validation_error.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.4.0/flask_openapi3/openapi.py` & `flask-openapi3-2.4.0rc1/flask_openapi3/openapi.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     def __init__(
             self,
             import_name: str,
             *,
             info: Optional[Info] = None,
             security_schemes: Optional[Dict[str, Union[SecurityScheme, Dict[str, Any]]]] = None,
             oauth_config: Optional[OAuthConfig] = None,
-            responses: Optional[Dict[str, Union[Type[BaseModel], Dict[Any, Any], None]]] = None,
+            responses: Optional[Dict[str, Optional[Type[BaseModel]]]] = None,
             doc_ui: bool = True,
             doc_expansion: str = "list",
             doc_prefix: str = "/openapi",
             api_doc_url: str = "/openapi.json",
             swagger_url: str = "/swagger",
             redoc_url: str = "/redoc",
             rapidoc_url: str = "/rapidoc",
@@ -44,327 +44,258 @@
             servers: Optional[List[Server]] = None,
             external_docs: Optional[ExternalDocumentation] = None,
             operation_id_callback: Callable = get_operation_id_for_path,
             openapi_extensions: Optional[Dict[str, Any]] = None,
             **kwargs: Any
     ) -> None:
         """
-        OpenAPI class that provides REST API functionality along with Swagger UI and Redoc.
+        Based on Flask. Provide REST api, swagger-ui and redoc.
 
         Arguments:
-            import_name: The import name for the Flask application.
-            info: Information about the API (title, version, etc.).
-                  See https://spec.openapis.org/oas/v3.0.3#info-object.
-            security_schemes: Security schemes for the API.
-                              See https://spec.openapis.org/oas/v3.0.3#security-scheme-object.
-            oauth_config: OAuth 2.0 configuration for authentication.
-                          See https://github.com/swagger-api/swagger-ui/blob/master/docs/usage/oauth2.md.
-            responses: API responses should be either a subclass of BaseModel, a dictionary, or None.
-            doc_ui: Enable OpenAPI document UI (Swagger UI and Redoc). Defaults to True.
-            doc_expansion: Default expansion setting for operations and tags ("list", "full", or "none").
-                           See https://github.com/swagger-api/swagger-ui/blob/master/docs/usage/configuration.md.
+            import_name: Just flask import_name
+            info: See https://spec.openapis.org/oas/v3.0.3#info-object
+            security_schemes: See https://spec.openapis.org/oas/v3.0.3#security-scheme-object
+            oauth_config: OAuth 2.0 configuration,
+                          see https://github.com/swagger-api/swagger-ui/blob/master/docs/usage/oauth2.md
+            responses: OpenAPI response model
+            doc_ui: Add openapi document UI(swagger and redoc). Defaults to True.
+            doc_expansion: String=["list"*, "full", "none"].
+                          Controls the default expansion setting for the operations and tags.
+                          It can be "list" (expands only the tags),
+                         "full" (expands the tags and operations) or "none" (expands nothing).
+                         see https://github.com/swagger-api/swagger-ui/blob/master/docs/usage/configuration.md
             doc_prefix: URL prefix used for OpenAPI document and UI. Defaults to "/openapi".
-            api_doc_url: URL for accessing the OpenAPI specification document in JSON format.
-                         Defaults to "/openapi.json".
-            swagger_url: URL for accessing the Swagger UI documentation. Defaults to "/swagger".
-            redoc_url: URL for accessing the Redoc UI documentation. Defaults to "/redoc".
-            rapidoc_url: URL for accessing the RapiDoc UI documentation. Defaults to "/rapidoc".
-            ui_templates: Custom UI templates to override or add UI documents.
-            servers: An array of Server objects providing connectivity information to a target server.
-            external_docs: External documentation for the API.
-                           See: https://spec.openapis.org/oas/v3.0.3#external-documentation-object.
-            operation_id_callback: Callback function for custom operation ID generation.
-                                   Receives name (str), path (str), and method (str) parameters.
-                                   Defaults to `get_operation_id_for_path` from utils.
-            openapi_extensions: Extensions to the OpenAPI Schema.
-                                See https://spec.openapis.org/oas/v3.0.3#specification-extensions.
-            **kwargs: Additional kwargs to be passed to Flask.
+            api_doc_url: The OpenAPI Spec documentation. Defaults to "/openapi.json".
+            swagger_url: The Swagger UI documentation. Defaults to `/swagger`.
+            redoc_url: The Redoc UI documentation. Defaults to `/redoc`.
+            rapidoc_url: The RapiDoc UI documentation. Defaults to `/rapidoc`.
+            ui_templates: Custom UI templates, which are used to overwrite or add UI documents.
+            servers: An array of Server Objects, which provide connectivity information to a target server.
+            external_docs: Allows referencing an external resource for extended documentation.
+                           See: https://spec.openapis.org/oas/v3.0.3#external-documentation-object
+            operation_id_callback: Callback function for custom operation_id generation.
+                          Receives name (str), path (str) and method (str) parameters.
+                          Default to `get_operation_id_for_path` from utils
+            openapi_extensions: Allows extensions to the OpenAPI Schema.
+                                See https://spec.openapis.org/oas/v3.0.3#specification-extensions
+            **kwargs: Flask kwargs
         """
         super(OpenAPI, self).__init__(import_name, **kwargs)
-
-        # Set OpenAPI version and API information
         self.openapi_version = "3.0.3"
         self.info = info or Info(title="OpenAPI", version="1.0.0")
-
-        # Set security schemes, responses, paths and components
         self.security_schemes = security_schemes
         self.responses = responses or {}
         self.paths: Dict = dict()
         self.components_schemas: Dict = dict()
         self.components = Components()
-
-        # Initialize lists for tags and tag names
         self.tags: List[Tag] = []
         self.tag_names: List[str] = []
-
-        # Set URL prefixes and endpoints
         self.doc_prefix = doc_prefix
         self.api_doc_url = api_doc_url
         self.swagger_url = swagger_url
         self.redoc_url = redoc_url
         self.rapidoc_url = rapidoc_url
-
-        # Set OAuth configuration and documentation expansion
         self.oauth_config = oauth_config
         self.doc_expansion = doc_expansion
-
-        # Set UI templates for customization
         self.ui_templates = ui_templates or dict()
-
-        # Set servers and external documentation
         self.severs = servers
         self.external_docs = external_docs
-
-        # Set the operation ID callback function
         self.operation_id_callback: Callable = operation_id_callback
-
-        # Set OpenAPI extensions
         self.openapi_extensions = openapi_extensions or dict()
-
-        # Initialize the OpenAPI documentation UI
         if doc_ui:
             self._init_doc()
-
-        # Add the OpenAPI command
+        # add openapi command
         self.cli.add_command(openapi_command)
 
     def _init_doc(self) -> None:
         """
         Provide Swagger UI, Redoc, and Rapidoc
         """
         _here = os.path.dirname(__file__)
         template_folder = os.path.join(_here, "templates")
         static_folder = os.path.join(template_folder, "static")
 
-        # Create the blueprint for OpenAPI documentation
         blueprint = Blueprint(
             "openapi",
             __name__,
             url_prefix=self.doc_prefix,
             template_folder=template_folder,
             static_folder=static_folder
         )
-
-        # Add the API documentation URL rule
         blueprint.add_url_rule(
             rule=self.api_doc_url,
             endpoint="api_doc",
             view_func=lambda: self.api_doc
         )
-
-        # Combine built-in templates and user-defined templates
         builtins_templates = {
             self.swagger_url.strip("/"): swagger_html_string,
             self.redoc_url.strip("/"): redoc_html_string,
-            self.rapidoc_url.strip("/"): rapidoc_html_string,
-            **self.ui_templates
+            self.rapidoc_url.strip("/"): rapidoc_html_string
         }
-
-        # Add URL rules for the templates
+        # update builtins_templates
+        builtins_templates.update(**self.ui_templates)
+        # iter builtins_templates
         for key, value in builtins_templates.items():
             blueprint.add_url_rule(
                 rule=f"/{key}",
                 endpoint=key,
-                # Pass default value to source
+                # pass default value to source
                 view_func=lambda source=value: render_template_string(
                     source,
                     api_doc_url=self.api_doc_url.lstrip("/"),
                     # The following parameters are only for swagger ui
                     doc_expansion=self.doc_expansion,
                     oauth_config=self.oauth_config.dict() if self.oauth_config else None
                 )
             )
-
-        # Add URL rule for the home page
+        # home page
         blueprint.add_url_rule(
             rule="/",
             endpoint="openapi",
             view_func=lambda: render_template_string(
                 openapi_html_string,
                 swagger_url=self.swagger_url.lstrip("/"),
                 redoc_url=self.redoc_url.lstrip("/"),
                 rapidoc_url=self.rapidoc_url.lstrip("/")
             )
         )
-
-        # Register the blueprint with the Flask application
         self.register_blueprint(blueprint)
 
     @property
     def api_doc(self) -> Dict:
-        """
-        Generate the OpenAPI specification JSON.
-
-        Returns:
-            The OpenAPI specification JSON as a dictionary.
-
-        """
+        """Generate Specification json"""
         spec = APISpec(
             openapi=self.openapi_version,
             info=self.info,
             servers=self.severs,
             externalDocs=self.external_docs
         )
-        # Set tags
         spec.tags = self.tags or None
-
-        # Set paths
         spec.paths = self.paths
-
-        # Set components
         self.components.schemas = self.components_schemas
         self.components.securitySchemes = self.security_schemes
         spec.components = self.components
 
-        # Convert spec to JSON
         spec_json = json.loads(spec.json(by_alias=True, exclude_none=True))
-
-        # Update with OpenAPI extensions
         spec_json.update(**self.openapi_extensions)
 
         return spec_json
 
     def register_api(self, api: APIBlueprint) -> None:
-        """
-        Register an APIBlueprint.
-
-        Arguments:
-            api: The APIBlueprint instance to register.
-
-        """
+        """Register APIBlueprint"""
         for tag in api.tags:
             if tag.name not in self.tag_names:
-                # Append tag to the list of tags
                 self.tags.append(tag)
-                # Append tag name to the list of tag names
                 self.tag_names.append(tag.name)
-
-        # Update paths with the APIBlueprint's paths
         self.paths.update(**api.paths)
-
-        # Update components schemas with the APIBlueprint's components schemas
         self.components_schemas.update(**api.components_schemas)
-
-        # Register the APIBlueprint with the current instance
         self.register_blueprint(api)
 
     def register_api_view(self, api_view: APIView, view_kwargs: Optional[Dict[Any, Any]] = None) -> None:
         """
         Register APIView
 
         Arguments:
-            api_view: The APIView instance to register.
-            view_kwargs: Additional keyword arguments to pass to the API views.
+            api_view: APIView
+            view_kwargs: extra view kwargs
         """
         if view_kwargs is None:
             view_kwargs = {}
-
-        # Iterate through tags of the APIView
         for tag in api_view.tags:
             if tag.name not in self.tag_names:
-                # Append tag to the list of tags
                 self.tags.append(tag)
-                # Append tag name to the list of tag names
                 self.tag_names.append(tag.name)
-
-        # Update paths with the APIView's paths
         self.paths.update(**api_view.paths)
-
-        # Update components schemas with the APIView's components schemas
         self.components_schemas.update(**api_view.components_schemas)
-
-        # Register the APIView with the current instance
         api_view.register(self, view_kwargs=view_kwargs)
 
     def _do_decorator(
             self,
             rule: str,
             func: Callable,
             *,
             tags: Optional[List[Tag]] = None,
             summary: Optional[str] = None,
             description: Optional[str] = None,
             external_docs: Optional[ExternalDocumentation] = None,
             operation_id: Optional[str] = None,
             extra_form: Optional[ExtraRequestBody] = None,
             extra_body: Optional[ExtraRequestBody] = None,
-            responses: Optional[Dict[str, Union[Type[BaseModel], Dict[Any, Any], None]]] = None,
+            responses: Optional[Dict[str, Optional[Type[BaseModel]]]] = None,
             extra_responses: Optional[Dict[str, Dict]] = None,
             deprecated: Optional[bool] = None,
             security: Optional[List[Dict[str, List[Any]]]] = None,
             servers: Optional[List[Server]] = None,
             openapi_extensions: Optional[Dict[str, Any]] = None,
             doc_ui: bool = True,
             method: str = HTTPMethod.GET
     ) -> Tuple[Type[BaseModel], Type[BaseModel], Type[BaseModel], Type[BaseModel], Type[BaseModel], Type[BaseModel]]:
         """
-        Collects OpenAPI specification information for Flask routes and view functions.
-
+        Collect openapi specification information
         Arguments:
-            rule: Flask route.
-            func: Flask view_func.
+            rule: Flask route
+            func: Flask view_func
             tags: Adds metadata to a single tag.
             summary: A short summary of what the operation does.
             description: A verbose explanation of the operation behavior.
             external_docs: Additional external documentation for this operation.
             operation_id: Unique string used to identify the operation.
             extra_form: Extra information describing the request body(application/form).
             extra_body: Extra information describing the request body(application/json).
-            responses: API responses should be either a subclass of BaseModel, a dictionary, or None.
+            responses: response's model must be pydantic BaseModel.
             extra_responses: Extra information for responses.
             deprecated: Declares this operation to be deprecated.
             security: A declaration of which security mechanisms can be used for this operation.
             servers: An alternative server array to service this operation.
             openapi_extensions: Allows extensions to the OpenAPI Schema.
-            doc_ui: Add OpenAPI document UI (swagger, rapidoc, and redoc). Defaults to True.
-            method: HTTP method for the operation. Defaults to GET.
+            doc_ui: Add openapi document UI(swagger, rapidoc and redoc). Defaults to True.
         """
         if doc_ui is True:
             if responses is None:
                 responses = {}
             if extra_responses is None:
                 extra_responses = {}
-            # Global response: combine API responses
+            # global response combine api responses
             combine_responses = deepcopy(self.responses)
             combine_responses.update(**responses)
-            # Create operation
+            # create operation
             operation = get_operation(
                 func,
                 summary=summary,
                 description=description,
                 openapi_extensions=openapi_extensions
             )
-            # Set external docs
+            # set external docs
             operation.externalDocs = external_docs
             # Unique string used to identify the operation.
             operation.operationId = operation_id or self.operation_id_callback(
                 name=func.__name__, path=rule, method=method
             )
-            # Only set `deprecated` if True, otherwise leave it as None
+            # only set `deprecated` if True otherwise leave it as None
             operation.deprecated = deprecated
-            # Add security
+            # add security
             operation.security = security
-            # Add servers
+            # add servers
             operation.servers = servers
-            # Store tags
+            # store tags
             if tags is None:
                 tags = []
             parse_and_store_tags(tags, self.tags, self.tag_names, operation)
-            # Parse parameters
+            # parse parameters
             header, cookie, path, query, form, body = parse_parameters(
                 func,
                 extra_form=extra_form,
                 extra_body=extra_body,
                 components_schemas=self.components_schemas,
                 operation=operation
             )
-            # Parse response
+            # parse response
             get_responses(combine_responses, extra_responses, self.components_schemas, operation)
-            # Convert route parameter format from /pet/<petId> to /pet/{petId}
+            # /pet/<petId> --> /pet/{petId}
             uri = re.sub(r"<([^<:]+:)?", "{", rule).replace(">", "}")
-            # Parse method
+            # parse method
             parse_method(uri, method, self.paths, operation)
             return header, cookie, path, query, form, body
         else:
-            # Parse parameters
+            # parse parameters
             header, cookie, path, query, form, body = parse_parameters(func, doc_ui=False)
             return header, cookie, path, query, form, body
```

### Comparing `flask-openapi3-2.4.0/flask_openapi3/scaffold.py` & `flask-openapi3-2.4.0rc1/flask_openapi3/scaffold.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # -*- coding: utf-8 -*-
 # @Author  : llc
 # @Time    : 2022/8/30 9:40
 import functools
 import inspect
 import sys
-import warnings
 from abc import ABC
 from functools import wraps
-from typing import Callable, List, Optional, Dict, Type, Any, Tuple, Union
+from typing import Callable, List, Optional, Dict, Type, Any, Tuple
 
 from flask.scaffold import Scaffold
 from flask.wrappers import Response
 from pydantic import BaseModel
 
 from .http import HTTPMethod
 from .models import ExternalDocumentation
@@ -28,31 +27,29 @@
             func = func.__func__
 
         while isinstance(func, functools.partial):
             func = func.func
 
         return inspect.iscoroutinefunction(func)
 
-warnings.simplefilter("once")
-
 
 class APIScaffold(Scaffold, ABC):
     def _do_decorator(
             self,
             rule: str,
             func: Callable,
             *,
             tags: Optional[List[Tag]] = None,
             summary: Optional[str] = None,
             description: Optional[str] = None,
             external_docs: Optional[ExternalDocumentation] = None,
             operation_id: Optional[str] = None,
             extra_form: Optional[ExtraRequestBody] = None,
             extra_body: Optional[ExtraRequestBody] = None,
-            responses: Optional[Dict[str, Union[Type[BaseModel], Dict[Any, Any], None]]] = None,
+            responses: Optional[Dict[str, Optional[Type[BaseModel]]]] = None,
             extra_responses: Optional[Dict[str, dict]] = None,
             deprecated: Optional[bool] = None,
             security: Optional[List[Dict[str, List[Any]]]] = None,
             servers: Optional[List[Server]] = None,
             openapi_extensions: Optional[Dict[str, Any]] = None,
             doc_ui: bool = True,
             method: str = HTTPMethod.GET
@@ -70,71 +67,53 @@
             path,
             query,
             form,
             body,
             view_class=None,
             view_kwargs=None
     ):
-        """
-        Create a view function that can be used with Flask to handle API requests.
-
-        Arguments:
-            func: The original function to be called when handling the API request.
-            header: The header parameter for the API request.
-            cookie: The cookie parameter for the API request.
-            path: The path parameter for the API request.
-            query: The query parameter for the API request.
-            form: The form parameter for the API request.
-            body: The body parameter for the API request.
-            view_class: The class of the API view (if applicable).
-            view_kwargs: Additional keyword arguments to pass to the API view.
-
-        Returns:
-            The view function that can be registered with Flask.
-
-        """
         is_coroutine_function = iscoroutinefunction(func)
         if is_coroutine_function:
             @wraps(func)
             async def view_func(**kwargs) -> Response:
-                func_kwargs = _do_request(
+                result = _do_request(
                     header=header,
                     cookie=cookie,
                     path=path,
                     query=query,
                     form=form,
                     body=body,
-                    path_kwargs=kwargs
+                    **kwargs
                 )
-                if isinstance(func_kwargs, Response):
+                if isinstance(result, Response):
                     # 422
-                    return func_kwargs
+                    return result
                 # handle async request
                 if view_class:
                     signature = inspect.signature(view_class.__init__)
                     parameters = signature.parameters
                     if parameters.get("view_kwargs"):
                         view_object = view_class(view_kwargs=view_kwargs)
                     else:
                         view_object = view_class()
-                    response = await func(view_object, **func_kwargs)
+                    response = await func(view_object, **result)
                 else:
-                    response = await func(**func_kwargs)
+                    response = await func(**result)
                 return response
         else:
             @wraps(func)
             def view_func(**kwargs) -> Response:
                 result = _do_request(
                     header=header,
                     cookie=cookie,
                     path=path,
                     query=query,
                     form=form,
                     body=body,
-                    path_kwargs=kwargs
+                    **kwargs
                 )
                 if isinstance(result, Response):
                     # 422
                     return result
                 # handle request
                 if view_class:
                     signature = inspect.signature(view_class.__init__)
@@ -160,58 +139,45 @@
             tags: Optional[List[Tag]] = None,
             summary: Optional[str] = None,
             description: Optional[str] = None,
             external_docs: Optional[ExternalDocumentation] = None,
             operation_id: Optional[str] = None,
             extra_form: Optional[ExtraRequestBody] = None,
             extra_body: Optional[ExtraRequestBody] = None,
-            responses: Optional[Dict[str, Union[Type[BaseModel], Dict[Any, Any], None]]] = None,
+            responses: Optional[Dict[str, Optional[Type[BaseModel]]]] = None,
             extra_responses: Optional[Dict[str, dict]] = None,
             deprecated: Optional[bool] = None,
             security: Optional[List[Dict[str, List[Any]]]] = None,
             servers: Optional[List[Server]] = None,
             openapi_extensions: Optional[Dict[str, Any]] = None,
             doc_ui: bool = True,
             **options: Any
     ) -> Callable:
         """
-        Decorator for defining a REST API endpoint with the HTTP GET method.
+        Decorator for rest api, like: app.route(methods=["GET"])
         More information goto https://spec.openapis.org/oas/v3.0.3#operation-object
 
         Arguments:
             rule: The URL rule string.
             tags: Adds metadata to a single tag.
             summary: A short summary of what the operation does.
             description: A verbose explanation of the operation behavior.
             external_docs: Additional external documentation for this operation.
             operation_id: Unique string used to identify the operation.
             extra_form: Extra information describing the request body(application/form).
             extra_body: Extra information describing the request body(application/json).
-            responses: API responses should be either a subclass of BaseModel, a dictionary, or None.
+            responses: response's model must be pydantic BaseModel.
             extra_responses: Extra information for responses.
             deprecated: Declares this operation to be deprecated.
             security: A declaration of which security mechanisms can be used for this operation.
             servers: An alternative server array to service this operation.
             openapi_extensions: Allows extensions to the OpenAPI Schema.
             doc_ui: Add openapi document UI(swagger, rapidoc and redoc). Defaults to True.
         """
 
-        if extra_form is not None:
-            warnings.warn(
-                """`extra_form` will be deprecated in v3.x, please use `openapi_extra` instead.""",
-                DeprecationWarning)
-        if extra_body is not None:
-            warnings.warn(
-                """`extra_body` will be deprecated in v3.x, please use `openapi_extra` instead.""",
-                DeprecationWarning)
-        if extra_responses is not None:
-            warnings.warn(
-                """`extra_responses` will be deprecated in v3.x, please use `responses` instead.""",
-                DeprecationWarning)
-
         def decorator(func) -> Callable:
             header, cookie, path, query, form, body = \
                 self._do_decorator(
                     rule,
                     func,
                     tags=tags,
                     summary=summary,
@@ -245,56 +211,44 @@
             tags: Optional[List[Tag]] = None,
             summary: Optional[str] = None,
             description: Optional[str] = None,
             external_docs: Optional[ExternalDocumentation] = None,
             operation_id: Optional[str] = None,
             extra_form: Optional[ExtraRequestBody] = None,
             extra_body: Optional[ExtraRequestBody] = None,
-            responses: Optional[Dict[str, Union[Type[BaseModel], Dict[Any, Any], None]]] = None,
+            responses: Optional[Dict[str, Optional[Type[BaseModel]]]] = None,
             extra_responses: Optional[Dict[str, dict]] = None,
             deprecated: Optional[bool] = None,
             security: Optional[List[Dict[str, List[Any]]]] = None,
             servers: Optional[List[Server]] = None,
             openapi_extensions: Optional[Dict[str, Any]] = None,
             doc_ui: bool = True,
             **options: Any
     ) -> Callable:
         """
-        Decorator for defining a REST API endpoint with the HTTP POST method.
+        Decorator for rest api, like: app.route(methods=["POST"])
         More information goto https://spec.openapis.org/oas/v3.0.3#operation-object
 
         Arguments:
             rule: The URL rule string.
             tags: Adds metadata to a single tag.
             summary: A short summary of what the operation does.
             description: A verbose explanation of the operation behavior.
             external_docs: Additional external documentation for this operation.
             operation_id: Unique string used to identify the operation.
             extra_form: Extra information describing the request body(application/form).
             extra_body: Extra information describing the request body(application/json).
-            responses: API responses should be either a subclass of BaseModel, a dictionary, or None.
+            responses: response's model must be pydantic BaseModel.
             extra_responses: Extra information for responses.
             deprecated: Declares this operation to be deprecated.
             security: A declaration of which security mechanisms can be used for this operation.
             servers: An alternative server array to service this operation.
             openapi_extensions: Allows extensions to the OpenAPI Schema.
             doc_ui: Declares this operation to be shown.
         """
-        if extra_form is not None:
-            warnings.warn(
-                """`extra_form` will be deprecated in v3.x, please use `openapi_extra` instead.""",
-                DeprecationWarning)
-        if extra_body is not None:
-            warnings.warn(
-                """`extra_body` will be deprecated in v3.x, please use `openapi_extra` instead.""",
-                DeprecationWarning)
-        if extra_responses is not None:
-            warnings.warn(
-                """`extra_responses` will be deprecated in v3.x, please use `responses` instead.""",
-                DeprecationWarning)
 
         def decorator(func) -> Callable:
             header, cookie, path, query, form, body = \
                 self._do_decorator(
                     rule,
                     func,
                     tags=tags,
@@ -329,56 +283,44 @@
             tags: Optional[List[Tag]] = None,
             summary: Optional[str] = None,
             description: Optional[str] = None,
             external_docs: Optional[ExternalDocumentation] = None,
             operation_id: Optional[str] = None,
             extra_form: Optional[ExtraRequestBody] = None,
             extra_body: Optional[ExtraRequestBody] = None,
-            responses: Optional[Dict[str, Union[Type[BaseModel], Dict[Any, Any], None]]] = None,
+            responses: Optional[Dict[str, Optional[Type[BaseModel]]]] = None,
             extra_responses: Optional[Dict[str, dict]] = None,
             deprecated: Optional[bool] = None,
             security: Optional[List[Dict[str, List[Any]]]] = None,
             servers: Optional[List[Server]] = None,
             openapi_extensions: Optional[Dict[str, Any]] = None,
             doc_ui: bool = True,
             **options: Any
     ) -> Callable:
         """
-        Decorator for defining a REST API endpoint with the HTTP PUT method.
+        Decorator for rest api, like: app.route(methods=["PUT"])
         More information goto https://spec.openapis.org/oas/v3.0.3#operation-object
 
         Arguments:
             rule: The URL rule string.
             tags: Adds metadata to a single tag.
             summary: A short summary of what the operation does.
             description: A verbose explanation of the operation behavior.
             external_docs: Additional external documentation for this operation.
             operation_id: Unique string used to identify the operation.
             extra_form: Extra information describing the request body(application/form).
             extra_body: Extra information describing the request body(application/json).
-            responses: API responses should be either a subclass of BaseModel, a dictionary, or None.
+            responses: response's model must be pydantic BaseModel.
             extra_responses: Extra information for responses.
             deprecated: Declares this operation to be deprecated.
             security: A declaration of which security mechanisms can be used for this operation.
             servers: An alternative server array to service this operation.
             openapi_extensions: Allows extensions to the OpenAPI Schema.
             doc_ui: Declares this operation to be shown.
         """
-        if extra_form is not None:
-            warnings.warn(
-                """`extra_form` will be deprecated in v3.x, please use `openapi_extra` instead.""",
-                DeprecationWarning)
-        if extra_body is not None:
-            warnings.warn(
-                """`extra_body` will be deprecated in v3.x, please use `openapi_extra` instead.""",
-                DeprecationWarning)
-        if extra_responses is not None:
-            warnings.warn(
-                """`extra_responses` will be deprecated in v3.x, please use `responses` instead.""",
-                DeprecationWarning)
 
         def decorator(func) -> Callable:
             header, cookie, path, query, form, body = \
                 self._do_decorator(
                     rule,
                     func,
                     tags=tags,
@@ -413,56 +355,44 @@
             tags: Optional[List[Tag]] = None,
             summary: Optional[str] = None,
             description: Optional[str] = None,
             external_docs: Optional[ExternalDocumentation] = None,
             operation_id: Optional[str] = None,
             extra_form: Optional[ExtraRequestBody] = None,
             extra_body: Optional[ExtraRequestBody] = None,
-            responses: Optional[Dict[str, Union[Type[BaseModel], Dict[Any, Any], None]]] = None,
+            responses: Optional[Dict[str, Optional[Type[BaseModel]]]] = None,
             extra_responses: Optional[Dict[str, dict]] = None,
             deprecated: Optional[bool] = None,
             security: Optional[List[Dict[str, List[Any]]]] = None,
             servers: Optional[List[Server]] = None,
             openapi_extensions: Optional[Dict[str, Any]] = None,
             doc_ui: bool = True,
             **options: Any
     ) -> Callable:
         """
-        Decorator for defining a REST API endpoint with the HTTP DELETE method.
+        Decorator for rest api, like: app.route(methods=["DELETE"])
         More information goto https://spec.openapis.org/oas/v3.0.3#operation-object
 
         Arguments:
             rule: The URL rule string.
             tags: Adds metadata to a single tag.
             summary: A short summary of what the operation does.
             description: A verbose explanation of the operation behavior.
             external_docs: Additional external documentation for this operation.
             operation_id: Unique string used to identify the operation.
             extra_form: Extra information describing the request body(application/form).
             extra_body: Extra information describing the request body(application/json).
-            responses: API responses should be either a subclass of BaseModel, a dictionary, or None.
+            responses: response's model must be pydantic BaseModel.
             extra_responses: Extra information for responses.
             deprecated: Declares this operation to be deprecated.
             security: A declaration of which security mechanisms can be used for this operation.
             servers: An alternative server array to service this operation.
             openapi_extensions: Allows extensions to the OpenAPI Schema.
             doc_ui: Declares this operation to be shown.
         """
-        if extra_form is not None:
-            warnings.warn(
-                """`extra_form` will be deprecated in v3.x, please use `openapi_extra` instead.""",
-                DeprecationWarning)
-        if extra_body is not None:
-            warnings.warn(
-                """`extra_body` will be deprecated in v3.x, please use `openapi_extra` instead.""",
-                DeprecationWarning)
-        if extra_responses is not None:
-            warnings.warn(
-                """`extra_responses` will be deprecated in v3.x, please use `responses` instead.""",
-                DeprecationWarning)
 
         def decorator(func) -> Callable:
             header, cookie, path, query, form, body = \
                 self._do_decorator(
                     rule,
                     func,
                     tags=tags,
@@ -497,56 +427,44 @@
             tags: Optional[List[Tag]] = None,
             summary: Optional[str] = None,
             description: Optional[str] = None,
             external_docs: Optional[ExternalDocumentation] = None,
             operation_id: Optional[str] = None,
             extra_form: Optional[ExtraRequestBody] = None,
             extra_body: Optional[ExtraRequestBody] = None,
-            responses: Optional[Dict[str, Union[Type[BaseModel], Dict[Any, Any], None]]] = None,
+            responses: Optional[Dict[str, Optional[Type[BaseModel]]]] = None,
             extra_responses: Optional[Dict[str, dict]] = None,
             deprecated: Optional[bool] = None,
             security: Optional[List[Dict[str, List[Any]]]] = None,
             servers: Optional[List[Server]] = None,
             openapi_extensions: Optional[Dict[str, Any]] = None,
             doc_ui: bool = True,
             **options: Any
     ) -> Callable:
         """
-        Decorator for defining a REST API endpoint with the HTTP PATCH method.
+        Decorator for rest api, like: app.route(methods=["PATCH"])
         More information goto https://spec.openapis.org/oas/v3.0.3#operation-object
 
         Arguments:
             rule: The URL rule string.
             tags: Adds metadata to a single tag.
             summary: A short summary of what the operation does.
             description: A verbose explanation of the operation behavior.
             external_docs: Additional external documentation for this operation.
             operation_id: Unique string used to identify the operation.
             extra_form: Extra information describing the request body(application/form).
             extra_body: Extra information describing the request body(application/json).
-            responses: API responses should be either a subclass of BaseModel, a dictionary, or None.
+            responses: response's model must be pydantic BaseModel.
             extra_responses: Extra information for responses.
             deprecated: Declares this operation to be deprecated.
             security: A declaration of which security mechanisms can be used for this operation.
             servers: An alternative server array to service this operation.
             openapi_extensions: Allows extensions to the OpenAPI Schema.
             doc_ui: Declares this operation to be shown.
         """
-        if extra_form is not None:
-            warnings.warn(
-                """`extra_form` will be deprecated in v3.x, please use `openapi_extra` instead.""",
-                DeprecationWarning)
-        if extra_body is not None:
-            warnings.warn(
-                """`extra_body` will be deprecated in v3.x, please use `openapi_extra` instead.""",
-                DeprecationWarning)
-        if extra_responses is not None:
-            warnings.warn(
-                """`extra_responses` will be deprecated in v3.x, please use `responses` instead.""",
-                DeprecationWarning)
 
         def decorator(func) -> Callable:
             header, cookie, path, query, form, body = \
                 self._do_decorator(
                     rule,
                     func,
                     tags=tags,
```

### Comparing `flask-openapi3-2.4.0/flask_openapi3/templates/__init__.py` & `flask-openapi3-2.4.0rc1/flask_openapi3/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.4.0/flask_openapi3/templates/static/css/swagger-ui.css` & `flask-openapi3-2.4.0rc1/flask_openapi3/templates/static/css/swagger-ui.css`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.4.0/flask_openapi3/templates/static/images/apidoc.svg` & `flask-openapi3-2.4.0rc1/flask_openapi3/templates/static/images/apidoc.svg`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.4.0/flask_openapi3/templates/static/images/rapidoc.svg` & `flask-openapi3-2.4.0rc1/flask_openapi3/templates/static/images/rapidoc.svg`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.4.0/flask_openapi3/templates/static/images/redoc.svg` & `flask-openapi3-2.4.0rc1/flask_openapi3/templates/static/images/redoc.svg`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.4.0/flask_openapi3/templates/static/images/swagger.svg` & `flask-openapi3-2.4.0rc1/flask_openapi3/templates/static/images/swagger.svg`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.4.0/flask_openapi3/templates/static/js/rapidoc-min.js` & `flask-openapi3-2.4.0rc1/flask_openapi3/templates/static/js/rapidoc-min.js`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.4.0/flask_openapi3/templates/static/js/redoc.standalone.js` & `flask-openapi3-2.4.0rc1/flask_openapi3/templates/static/js/redoc.standalone.js`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.4.0/flask_openapi3/templates/static/js/swagger-ui-bundle.js` & `flask-openapi3-2.4.0rc1/flask_openapi3/templates/static/js/swagger-ui-bundle.js`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.4.0/flask_openapi3/templates/static/js/swagger-ui-standalone-preset.js` & `flask-openapi3-2.4.0rc1/flask_openapi3/templates/static/js/swagger-ui-standalone-preset.js`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.4.0/flask_openapi3/utils.py` & `flask-openapi3-2.4.0rc1/flask_openapi3/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 # @Author  : llc
 # @Time    : 2021/5/1 21:34
 
 import inspect
 import re
-from typing import get_type_hints, Dict, Type, Callable, List, Tuple, Optional, Any, Union
+from typing import get_type_hints, Dict, Type, Callable, List, Tuple, Optional, Any
 
 from pydantic import BaseModel
 
 from .http import HTTP_STATUS, HTTPMethod
 from .models import OPENAPI3_REF_TEMPLATE, OPENAPI3_REF_PREFIX, Tag
 from .models.common import Schema, MediaType, Encoding, ExtraRequestBody
 from .models.path import Operation, RequestBody, PathItem, Response
@@ -18,211 +18,179 @@
 
 def get_operation(
         func: Callable, *,
         summary: Optional[str] = None,
         description: Optional[str] = None,
         openapi_extensions: Optional[Dict[str, Any]] = None,
 ) -> Operation:
-    """
-    Return an Operation object with the specified summary and description.
-
-    Arguments:
-        func: The function or method for which the operation is being defined.
-        summary: A short summary of what the operation does.
-        description: A verbose explanation of the operation behavior.
-        openapi_extensions: Additional extensions to the OpenAPI Schema.
-
-    Returns:
-        An Operation object representing the operation.
-
-    """
-    # Get the docstring of the function
+    """Return an Operation object with summary and description."""
     doc = inspect.getdoc(func) or ""
     doc = doc.strip()
     lines = doc.split("\n")
     doc_summary = lines[0] or None
-
-    # Determine the summary and description based on provided arguments or docstring
     if summary is None:
         doc_description = lines[0] if len(lines) == 0 else "</br>".join(lines[1:]) or None
     else:
         doc_description = "</br>".join(lines) or None
 
-    # Create the operation dictionary with summary and description
     operation_dict = dict(
         summary=summary or doc_summary,
         description=description or doc_description
     )
-
-    # Add any additional openapi_extensions to the operation dictionary
+    # update openapi_extensions
     openapi_extensions = openapi_extensions or {}
     operation_dict.update(**openapi_extensions)
 
-    # Create and return the Operation object
     operation = Operation(**operation_dict)
 
     return operation
 
 
 def get_operation_id_for_path(*, name: str, path: str, method: str) -> str:
-    """
-    Generate a unique operation ID based on the name, path, and method.
-
-    Arguments:
-        name: The name or identifier for the operation.
-        path: The URL path for the operation.
-        method: The HTTP method for the operation.
-
-    Returns:
-        A unique operation ID generated based on the provided name, path, and method.
-
-    """
     operation_id = name + path
-    # Replace non-word characters with underscores
     operation_id = re.sub(r"\W", "_", operation_id)
     operation_id = operation_id + "_" + method.lower()
     return operation_id
 
 
 def get_schema(obj: Type[BaseModel]) -> dict:
-    """Converts a Pydantic model to an OpenAPI schema."""
-
+    """Pydantic model conversion to openapi schema"""
     assert inspect.isclass(obj) and issubclass(obj, BaseModel), \
         f"{obj} is invalid `pydantic.BaseModel`"
 
     return obj.schema(ref_template=OPENAPI3_REF_TEMPLATE)
 
 
 def parse_header(header: Type[BaseModel]) -> Tuple[List[Parameter], dict]:
-    """Parses a header model and returns a list of parameters and component schemas."""
+    """Parse header model"""
     schema = get_schema(header)
     parameters = []
     components_schemas: Dict = dict()
     properties = schema.get("properties", {})
 
     for name, value in properties.items():
         data = {
             "name": name,
             "in": ParameterInType.header,
             "description": value.get("description"),
             "required": name in schema.get("required", []),
             "schema": Schema(**value)
         }
-        # Parse extra values
+        # parse extra values
         data.update(**value)
         parameters.append(Parameter(**data))
 
-    # Parse definitions
+    # parse definitions
     definitions = schema.get("definitions", {})
     for name, value in definitions.items():
         components_schemas[name] = Schema(**value)
 
     return parameters, components_schemas
 
 
 def parse_cookie(cookie: Type[BaseModel]) -> Tuple[List[Parameter], dict]:
-    """Parses a cookie model and returns a list of parameters and component schemas."""
+    """Parse cookie model"""
     schema = get_schema(cookie)
     parameters = []
     components_schemas: Dict = dict()
     properties = schema.get("properties", {})
 
     for name, value in properties.items():
         data = {
             "name": name,
             "in": ParameterInType.cookie,
             "description": value.get("description"),
             "required": name in schema.get("required", []),
             "schema": Schema(**value)
         }
-        # Parse extra values
+        # parse extra values
         data.update(**value)
         parameters.append(Parameter(**data))
 
-    # Parse definitions
+    # parse definitions
     definitions = schema.get("definitions", {})
     for name, value in definitions.items():
         components_schemas[name] = Schema(**value)
 
     return parameters, components_schemas
 
 
 def parse_path(path: Type[BaseModel]) -> Tuple[List[Parameter], dict]:
-    """Parses a path model and returns a list of parameters and component schemas."""
+    """Parse path model"""
     schema = get_schema(path)
     parameters = []
     components_schemas: Dict = dict()
     properties = schema.get("properties", {})
 
     for name, value in properties.items():
         data = {
             "name": name,
             "in": ParameterInType.path,
             "description": value.get("description"),
             "required": True,
             "schema": Schema(**value)
         }
-        # Parse extra values
+        # parse extra values
         data.update(**value)
         parameters.append(Parameter(**data))
 
-    # Parse definitions
+    # parse definitions
     definitions = schema.get("definitions", {})
     for name, value in definitions.items():
         components_schemas[name] = Schema(**value)
 
     return parameters, components_schemas
 
 
 def parse_query(query: Type[BaseModel]) -> Tuple[List[Parameter], dict]:
-    """Parses a query model and returns a list of parameters and component schemas."""
+    """Parse query model"""
     schema = get_schema(query)
     parameters = []
     components_schemas: Dict = dict()
     properties = schema.get("properties", {})
 
     for name, value in properties.items():
         data = {
             "name": name,
             "in": ParameterInType.query,
             "description": value.get("description"),
             "required": name in schema.get("required", []),
             "schema": Schema(**value)
         }
-        # Parse extra values
+        # parse extra values
         data.update(**value)
         parameters.append(Parameter(**data))
 
-    # Parse definitions
+    # parse definitions
     definitions = schema.get("definitions", {})
     for name, value in definitions.items():
         components_schemas[name] = Schema(**value)
 
     return parameters, components_schemas
 
 
 def parse_form(
         form: Type[BaseModel],
         extra_form: Optional[ExtraRequestBody] = None,
 ) -> Tuple[Dict[str, MediaType], dict]:
-    """Parses a form model and returns a list of parameters and component schemas."""
+    """Parse form model"""
     schema = get_schema(form)
     components_schemas = dict()
     properties = schema.get("properties", {})
 
     assert properties, f"{form.__name__}'s properties cannot be empty."
 
     title = schema.get("title")
     components_schemas[title] = Schema(**schema)
     encoding = {}
     for k, v in properties.items():
         if v.get("type") == "array":
             encoding[k] = Encoding(style="form")
     if extra_form:
-        # Update encoding
+        # update encoding
         if extra_form.encoding:
             encoding.update(**extra_form.encoding)
         content = {
             "multipart/form-data": MediaType(
                 schema=Schema(**{"$ref": f"{OPENAPI3_REF_PREFIX}/{title}"}),
                 example=extra_form.example,
                 examples=extra_form.examples,
@@ -233,27 +201,27 @@
         content = {
             "multipart/form-data": MediaType(
                 schema=Schema(**{"$ref": f"{OPENAPI3_REF_PREFIX}/{title}"}),
                 encoding=encoding or None
             )
         }
 
-    # Parse definitions
+    # parse definitions
     definitions = schema.get("definitions", {})
     for name, value in definitions.items():
         components_schemas[name] = Schema(**value)
 
     return content, components_schemas
 
 
 def parse_body(
         body: Type[BaseModel],
         extra_body: Optional[ExtraRequestBody] = None,
 ) -> Tuple[Dict[str, MediaType], dict]:
-    """Parses a body model and returns a list of parameters and component schemas."""
+    """Parse body model"""
     schema = get_schema(body)
     components_schemas = dict()
 
     title = schema.get("title")
     components_schemas[title] = Schema(**schema)
     if extra_body:
         content = {
@@ -267,34 +235,39 @@
     else:
         content = {
             "application/json": MediaType(
                 schema=Schema(**{"$ref": f"{OPENAPI3_REF_PREFIX}/{title}"})
             )
         }
 
-    # Parse definitions
+    # parse definitions
     definitions = schema.get("definitions", {})
     for name, value in definitions.items():
         components_schemas[name] = Schema(**value)
 
     return content, components_schemas
 
 
 def get_responses(
-        responses: Optional[Dict[str, Union[Type[BaseModel], Dict[Any, Any], None]]],
+        responses: dict,
         extra_responses: Dict[str, dict],
         components_schemas: dict,
         operation: Operation
 ) -> None:
+    """
+    :param responses: Dict[str, BaseModel]
+    :param extra_responses: Dict[str, dict]
+    :param components_schemas: `models.component.py` `Components.schemas`
+    :param operation: `models.path.py` Operation
+    """
     if responses is None:
         responses = {}
     _responses = {}
     _schemas = {}
     if not responses.get("422"):
-        # Handle 422 response for Unprocessable Entity
         _responses["422"] = Response(
             description=HTTP_STATUS["422"],
             content={
                 "application/json": MediaType(
                     **{
                         "schema": Schema(
                             **{
@@ -304,21 +277,16 @@
                         )
                     }
                 )
             }
         )
         _schemas[UnprocessableEntity.__name__] = Schema(**UnprocessableEntity.schema())
     for key, response in responses.items():
-        if response is None:
-            # If the response is None, it means HTTP status code "204" (No Content)
-            _responses[key] = Response(description=HTTP_STATUS.get(key, ""))
-            continue
-        if isinstance(response, dict):
-            _responses[key] = response  # type: ignore
-        else:
+        # Verify that the response is a class and that class is a subclass of `pydantic.BaseModel`
+        if inspect.isclass(response) and issubclass(response, BaseModel):
             schema = response.schema(ref_template=OPENAPI3_REF_TEMPLATE)
             _responses[key] = Response(
                 description=HTTP_STATUS.get(key, ""),
                 content={
                     "application/json": MediaType(
                         **{
                             "schema": Schema(
@@ -326,35 +294,26 @@
                                     "$ref": f"{OPENAPI3_REF_PREFIX}/{response.__name__}"
                                 }
                             )
                         }
                     )
                 }
             )
-
-            model_config = response.Config
-            if hasattr(model_config, "openapi_extra"):
-                # Add additional information from model_config to the response
-                _responses[key].description = model_config.openapi_extra.get("description")
-                _responses[key].headers = model_config.openapi_extra.get("headers")
-                _responses[key].links = model_config.openapi_extra.get("links")
-                _content = _responses[key].content
-                _content["application/json"].example = model_config.openapi_extra.get("example")  # type: ignore
-                _content["application/json"].examples = model_config.openapi_extra.get("examples")  # type: ignore
-                _content["application/json"].encoding = model_config.openapi_extra.get("encoding")  # type: ignore
-                if model_config.openapi_extra.get("content"):
-                    _responses[key].content.update(model_config.openapi_extra.get("content"))  # type: ignore
-
             _schemas[response.__name__] = Schema(**schema)
             definitions = schema.get("definitions")
             if definitions:
-                # Add schema definitions to _schemas
                 for name, value in definitions.items():
                     _schemas[name] = Schema(**value)
-
+        # Verify that if the response is None, because http status code "204" means return "No Content"
+        elif response is None:
+            _responses[key] = Response(
+                description=HTTP_STATUS.get(key, ""),
+            )
+        else:
+            raise TypeError(f"{response} is invalid `pydantic.BaseModel`.")
     # handle extra_responses
     for key, value in extra_responses.items():
         # key "200" value {"content":{"text/csv":{"schema":{"type": "string"}}}}
         new_response = Response(
             # Best effort to ensure there is always a description
             description=value.pop("description", HTTP_STATUS.get(key, "")),
             **value
@@ -367,173 +326,116 @@
 
 def parse_and_store_tags(
         new_tags: List[Tag],
         old_tags: List[Tag],
         old_tag_names: List[str],
         operation: Operation
 ) -> None:
-    """
-    Parses new tags, stores them in old_tags list if they are not already present,
-    and updates the tags attribute of the operation object.
-
-    Arguments:
-        new_tags: A list of new Tag objects to be parsed and stored.
-        old_tags: The list of existing Tag objects.
-        old_tag_names: The list of names of existing tags.
-        operation: The operation object whose tags attribute needs to be updated.
-
-    Returns:
-        None
+    """Store tags
+    :param new_tags: api tag
+    :param old_tags: openapi doc tags
+    :param old_tag_names: openapi doc tag names
+    :param operation: `models.path.py` Operation
     """
     if new_tags is None:
         new_tags = []
-
-    # Iterate over each tag in new_tags
     for tag in new_tags:
         if tag.name not in old_tag_names:
             old_tag_names.append(tag.name)
             old_tags.append(tag)
-
-    # Set the tags attribute of the operation object to a list of unique tag names from new_tags
-    # If the resulting list is empty, set it to None
     operation.tags = list(set([tag.name for tag in new_tags])) or None
 
 
 def parse_parameters(
         func: Callable,
         *,
         extra_form: Optional[ExtraRequestBody] = None,
         extra_body: Optional[ExtraRequestBody] = None,
         components_schemas: Optional[Dict] = None,
         operation: Optional[Operation] = None,
         doc_ui: bool = True,
 ) -> Tuple[Type[BaseModel], Type[BaseModel], Type[BaseModel], Type[BaseModel], Type[BaseModel], Type[BaseModel]]:
     """
-    Parses the parameters of a given function and returns the types for header, cookie, path,
-    query, form, and body parameters. Also populates the Operation object with the parsed parameters.
-
-    Arguments:
-        func: The function to parse the parameters from.
-        extra_form: Additional form data for the request body (default: None).
-        extra_body: Additional body data for the request body (default: None).
-        components_schemas: Dictionary to store the parsed components schemas (default: None).
-        operation: Operation object to populate with parsed parameters (default: None).
-        doc_ui: Flag indicating whether to return types for documentation UI (default: True).
-
-    Returns:
-        Tuple[Type[BaseModel], Type[BaseModel], Type[BaseModel], Type[BaseModel], Type[BaseModel], Type[BaseModel]]:
-        The types for header, cookie, path, query, form, and body parameters respectively.
-
+    :param func: Flask view func
+    :param extra_form: Extra information describing the request body(application/form).
+    :param extra_body: Extra information describing the request body(application/json).
+    :param components_schemas: `models.component.py` Components.schemas
+    :param operation: `models.path.py` Operation
+    :param doc_ui: add openapi document UI(swagger and redoc). Defaults to True.
     """
-    # Get the type hints from the function
     annotations = get_type_hints(func)
-
-    # Get the types for header, cookie, path, query, form, and body parameters
     header = annotations.get("header")
     cookie = annotations.get("cookie")
     path = annotations.get("path")
     query = annotations.get("query")
     form = annotations.get("form")
     body = annotations.get("body")
-
-    # If doc_ui is False, return the types without further processing
     if doc_ui is False:
         return header, cookie, path, query, form, body  # type: ignore
-
     parameters = []
-
-    # If components_schemas is None, initialize it as an empty dictionary
     if components_schemas is None:
         components_schemas = dict()
-
-    # If operation is None, initialize it as an Operation object
     if operation is None:
         operation = Operation()
-
     if header:
         _parameters, _components_schemas = parse_header(header)
         parameters.extend(_parameters)
         components_schemas.update(**_components_schemas)
-
     if cookie:
         _parameters, _components_schemas = parse_cookie(cookie)
         parameters.extend(_parameters)
         components_schemas.update(**_components_schemas)
-
     if path:
+        # get args from a route path
         _parameters, _components_schemas = parse_path(path)
         parameters.extend(_parameters)
         components_schemas.update(**_components_schemas)
-
     if query:
+        # get args from route query
         _parameters, _components_schemas = parse_query(query)
         parameters.extend(_parameters)
         components_schemas.update(**_components_schemas)
-
     if form:
         _content, _components_schemas = parse_form(form, extra_form)
         components_schemas.update(**_components_schemas)
         if extra_form:
             request_body = RequestBody(
                 description=extra_form.description,
                 content=_content,
                 required=extra_form.required
             )
         else:
             request_body = RequestBody(**{
                 "content": _content,
             })
-        model_config = form.Config
-        if hasattr(model_config, "openapi_extra"):
-            request_body.description = model_config.openapi_extra.get("description")
-            request_body.content["multipart/form-data"].example = model_config.openapi_extra.get("example")
-            request_body.content["multipart/form-data"].examples = model_config.openapi_extra.get("examples")
-            if model_config.openapi_extra.get("encoding"):
-                request_body.content["multipart/form-data"].encoding = model_config.openapi_extra.get("encoding")
         operation.requestBody = request_body
-
     if body:
         _content, _components_schemas = parse_body(body, extra_body)
         components_schemas.update(**_components_schemas)
         if extra_body:
             request_body = RequestBody(
                 description=extra_body.description,
                 content=_content,
                 required=extra_body.required
             )
         else:
             request_body = RequestBody(content=_content)
-        model_config = body.Config
-        if hasattr(model_config, "openapi_extra"):
-            request_body.description = model_config.openapi_extra.get("description")
-            request_body.content["application/json"].example = model_config.openapi_extra.get("example")
-            request_body.content["application/json"].examples = model_config.openapi_extra.get("examples")
-            request_body.content["application/json"].encoding = model_config.openapi_extra.get("encoding")
         operation.requestBody = request_body
-
-    # Set the parsed parameters in the operation object
     operation.parameters = parameters if parameters else None
 
     return header, cookie, path, query, form, body  # type: ignore
 
 
 def parse_method(uri: str, method: str, paths: dict, operation: Operation) -> None:
     """
-    Parses the HTTP method and updates the corresponding PathItem object in the paths' dictionary.
-
-    Arguments:
-        uri: The URI of the API endpoint.
-        method: The HTTP method for the API endpoint.
-        paths: A dictionary containing the API paths and their corresponding PathItem objects.
-        operation: The Operation object to assign to the PathItem.
-
-    Returns:
-        None
+    :param uri: api route path
+    :param method: get post put delete patch
+    :param paths: openapi doc paths
+    :param operation: `models.path.py` Operation
     """
-    # Check the HTTP method and update the PathItem object in the paths dictionary
     if method == HTTPMethod.GET:
         if not paths.get(uri):
             paths[uri] = PathItem(get=operation)
         else:
             paths[uri].get = operation
     elif method == HTTPMethod.POST:
         if not paths.get(uri):
```

### Comparing `flask-openapi3-2.4.0/flask_openapi3/view.py` & `flask-openapi3-2.4.0rc1/flask_openapi3/view.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,54 +1,51 @@
 # -*- coding: utf-8 -*-
 # @Author  : llc
 # @Time    : 2022/10/14 16:09
 import re
 import typing
-import warnings
 
 if typing.TYPE_CHECKING:
     from .openapi import OpenAPI
 
 from copy import deepcopy
-from typing import Optional, List, Dict, Type, Any, Callable, Union
+from typing import Optional, List, Dict, Type, Any, Callable
 
 from pydantic import BaseModel
 
 from .http import HTTPMethod
 from .models.common import ExternalDocumentation, ExtraRequestBody
 from .models.server import Server
 from .models.tag import Tag
 from .utils import get_operation, parse_and_store_tags, parse_parameters, get_responses, parse_method, \
     get_operation_id_for_path
 
-warnings.simplefilter("once")
-
 
 class APIView:
     def __init__(
             self,
             url_prefix: Optional[str] = None,
             view_tags: Optional[List[Tag]] = None,
             view_security: Optional[List[Dict[str, List[str]]]] = None,
-            view_responses: Optional[Dict[str, Union[Type[BaseModel], Dict[Any, Any], None]]] = None,
+            view_responses: Optional[Dict[str, Optional[Type[BaseModel]]]] = None,
             doc_ui: bool = True,
             operation_id_callback: Callable = get_operation_id_for_path,
     ):
         """
         Create a class-based view
 
         Arguments:
             url_prefix: A path to prepend to all the APIView's urls
-            view_tags: APIView tags for every API.
-            view_security: APIView security for every API.
-            view_responses: API responses should be either a subclass of BaseModel, a dictionary, or None.
-            doc_ui: Enable OpenAPI document UI (Swagger UI and Redoc). Defaults to True.
+            view_tags: APIView tags for every api
+            view_security: APIView security for every api
+            view_responses: APIView response models
+            doc_ui: Add openapi document UI(swagger, rapidoc and redoc). Defaults to True.
             operation_id_callback: Callback function for custom operation_id generation.
-                                   Receives name (str), path (str) and method (str) parameters.
-                                   Defaults to `get_operation_id_for_path` from utils
+                Receives name (str), path (str) and method (str) parameters.
+                Defaults to `get_operation_id_for_path` from utils
         """
         self.url_prefix = url_prefix
         self.view_tags = view_tags or []
         self.view_security = view_security or []
         self.view_responses = view_responses or {}
         self.doc_ui = doc_ui
         self.operation_id_callback: Callable = operation_id_callback
@@ -62,40 +59,40 @@
     def route(self, rule: str):
         """Decorator for view class"""
 
         def wrapper(cls):
             if self.views.get(rule):
                 raise ValueError(f"malformed url rule: {rule!r}")
             methods = []
-            # Convert route parameter format from /pet/<petId> to /pet/{petId}
+            # /pet/<petId> --> /pet/{petId}
             uri = re.sub(r"<([^<:]+:)?", "{", rule).replace(">", "}")
             trail_slash = uri.endswith("/")
-            # Merge url_prefix and uri
+            # merge url_prefix and uri
             uri = self.url_prefix.rstrip("/") + "/" + uri.lstrip("/") if self.url_prefix else uri
             if not trail_slash:
                 uri = uri.rstrip("/")
             for method in HTTPMethod:
                 cls_method = getattr(cls, method.lower(), None)
                 if not cls_method:
                     continue
                 methods.append(method)
                 if self.doc_ui is False:
                     continue
                 if not getattr(cls_method, "operation", None):
                     continue
-                # Parse method
+                # parse method
                 parse_method(uri, method, self.paths, cls_method.operation)
-                # Update operation_id
+                # update operation_id
                 if not cls_method.operation.operationId:
                     cls_method.operation.operationId = self.operation_id_callback(
                         name=cls_method.__qualname__,
                         path=rule,
                         method=method
                     )
-            # Convert route parameters from <param> to {param}
+            # /pet/{petId} --> /pet/<petId>
             _rule = uri.replace("{", "<").replace("}", ">")
             self.views[_rule] = (cls, methods)
 
             return cls
 
         return wrapper
 
@@ -105,15 +102,15 @@
             tags: Optional[List[Tag]] = None,
             summary: Optional[str] = None,
             description: Optional[str] = None,
             external_docs: Optional[ExternalDocumentation] = None,
             operation_id: Optional[str] = None,
             extra_form: Optional[ExtraRequestBody] = None,
             extra_body: Optional[ExtraRequestBody] = None,
-            responses: Optional[Dict[str, Union[Type[BaseModel], Dict[Any, Any], None]]] = None,
+            responses: Optional[Dict[str, Optional[Type[BaseModel]]]] = None,
             extra_responses: Optional[Dict[str, dict]] = None,
             deprecated: Optional[bool] = None,
             security: Optional[List[Dict[str, List[Any]]]] = None,
             servers: Optional[List[Server]] = None,
             openapi_extensions: Optional[Dict[str, Any]] = None,
             doc_ui: bool = True
     ) -> Callable:
@@ -125,96 +122,73 @@
             tags: Adds metadata to a single tag.
             summary: A short summary of what the operation does.
             description: A verbose explanation of the operation behavior.
             external_docs: Additional external documentation for this operation.
             operation_id: Unique string used to identify the operation.
             extra_form: Extra information describing the request body(application/form).
             extra_body: Extra information describing the request body(application/json).
-            responses: API responses should be either a subclass of BaseModel, a dictionary, or None.
+            responses: response's model must be pydantic BaseModel.
             extra_responses: Extra information for responses.
             deprecated: Declares this operation to be deprecated.
             security: A declaration of which security mechanisms can be used for this operation.
             servers: An alternative server array to service this operation.
             openapi_extensions: Allows extensions to the OpenAPI Schema.
             doc_ui: Add openapi document UI(swagger, rapidoc and redoc). Defaults to True.
         """
 
-        if extra_form is not None:
-            warnings.warn(
-                """`extra_form` will be deprecated in v3.x, please use `openapi_extra` instead.""",
-                DeprecationWarning)
-        if extra_body is not None:
-            warnings.warn(
-                """`extra_body` will be deprecated in v3.x, please use `openapi_extra` instead.""",
-                DeprecationWarning)
-        if extra_responses is not None:
-            warnings.warn(
-                """`extra_responses` will be deprecated in v3.x, please use `responses` instead.""",
-                DeprecationWarning)
-
         if responses is None:
             responses = {}
         if extra_responses is None:
             extra_responses = {}
         if security is None:
             security = []
         tags = tags + self.view_tags if tags else self.view_tags
 
         def decorator(func):
             if self.doc_ui is False or doc_ui is False:
                 return
-            # Global response combines API responses
+            # global response combine api responses
             combine_responses = deepcopy(self.view_responses)
             combine_responses.update(**responses)
-            # Create operation
+            # create operation
             operation = get_operation(
                 func,
                 summary=summary,
                 description=description,
                 openapi_extensions=openapi_extensions
             )
-            # Set external docs
+            # set external docs
             operation.externalDocs = external_docs
             # Unique string used to identify the operation.
             operation.operationId = operation_id
-            # Only set `deprecated` if True, otherwise leave it as None
+            # only set `deprecated` if True otherwise leave it as None
             operation.deprecated = deprecated
-            # Add security
+            # add security
             operation.security = security + self.view_security or None
-            # Add servers
+            # add servers
             operation.servers = servers
-            # Store tags
+            # store tags
             parse_and_store_tags(tags, self.tags, self.tag_names, operation)
-            # Parse parameters
+            # parse parameters
             parse_parameters(
                 func,
                 extra_form=extra_form,
                 extra_body=extra_body,
                 components_schemas=self.components_schemas,
                 operation=operation
             )
-            # Parse response
+            # parse response
             get_responses(combine_responses, extra_responses, self.components_schemas, operation)
             func.operation = operation
 
             return func
 
         return decorator
 
     def register(self, app: "OpenAPI", view_kwargs: Optional[Dict[Any, Any]] = None):
-        """
-        Register the API views with the given OpenAPI app.
-
-        Args:
-            app: An instance of the OpenAPI app.
-            view_kwargs: Additional keyword arguments to pass to the API views.
-
-        Returns:
-            None
-        """
         if view_kwargs is None:
             view_kwargs = {}
         for rule, (cls, methods) in self.views.items():
             for method in methods:
                 func = getattr(cls, method.lower())
                 header, cookie, path, query, form, body = parse_parameters(func, doc_ui=False)
                 view_func = app.create_view_func(
```

### Comparing `flask-openapi3-2.4.0/flask_openapi3.egg-info/PKG-INFO` & `flask-openapi3-2.4.0rc1/flask_openapi3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-openapi3
-Version: 2.4.0
+Version: 2.4.0rc1
 Summary: Generate REST API and OpenAPI documentation for your Flask project.
 Home-page: https://github.com/luolingchun/flask-openapi3
 Author: llc
 Author-email: luolingchun@outlook.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `flask-openapi3-2.4.0/flask_openapi3.egg-info/SOURCES.txt` & `flask-openapi3-2.4.0rc1/flask_openapi3.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 examples/enum_demo.py
 examples/header_demo.py
 examples/image_demo.py
 examples/init_oauth_demo.py
 examples/just_flask.py
 examples/nested_apiblueprint_demo.py
 examples/openapi_extensions.py
-examples/openapi_extra.py
 examples/orjson_demo.py
 examples/pydantic_custom_root_types.py
 examples/response_demo.py
 examples/rest_demo.py
 examples/servers_demo.py
 examples/simple_demo.py
 examples/upload_file_demo.py
```

### Comparing `flask-openapi3-2.4.0/setup.py` & `flask-openapi3-2.4.0rc1/setup.py`

 * *Files identical despite different names*

