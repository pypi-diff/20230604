# Comparing `tmp/timeflux-ui-0.5.2.tar.gz` & `tmp/timeflux-ui-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timeflux-ui-0.5.2.tar", last modified: Sun Dec 18 13:39:32 2022, max compression
+gzip compressed data, was "timeflux-ui-0.6.0.tar", last modified: Sun Jun  4 12:56:42 2023, max compression
```

## Comparing `timeflux-ui-0.5.2.tar` & `timeflux-ui-0.6.0.tar`

### file list

```diff
@@ -1,121 +1,121 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 13:39:32.963050 timeflux-ui-0.5.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 13:39:32.947049 timeflux-ui-0.5.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 13:39:32.951049 timeflux-ui-0.5.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      962 2022-12-18 13:39:08.000000 timeflux-ui-0.5.2/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      605 2022-12-18 13:39:08.000000 timeflux-ui-0.5.2/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      131 2022-12-18 13:39:08.000000 timeflux-ui-0.5.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      205 2022-12-18 13:39:08.000000 timeflux-ui-0.5.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2022-12-18 13:39:08.000000 timeflux-ui-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       36 2022-12-18 13:39:08.000000 timeflux-ui-0.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2022-12-18 13:39:32.963050 timeflux-ui-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      767 2022-12-18 13:39:08.000000 timeflux-ui-0.5.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 13:39:32.951049 timeflux-ui-0.5.2/apps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 13:39:32.951049 timeflux-ui-0.5.2/apps/circle/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 13:39:32.951049 timeflux-ui-0.5.2/apps/circle/assets/
--rw-r--r--   0 runner    (1001) docker     (123)      895 2022-12-18 13:39:08.000000 timeflux-ui-0.5.2/apps/circle/assets/app.js
--rw-r--r--   0 runner    (1001) docker     (123)      247 2022-12-18 13:39:08.000000 timeflux-ui-0.5.2/apps/circle/assets/style.css
--rw-r--r--   0 runner    (1001) docker     (123)      487 2022-12-18 13:39:08.000000 timeflux-ui-0.5.2/apps/circle/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      364 2022-12-18 13:39:08.000000 timeflux-ui-0.5.2/apps/circle.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 13:39:32.951049 timeflux-ui-0.5.2/apps/demo/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2022-12-18 13:39:08.000000 timeflux-ui-0.5.2/apps/demo/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2022-12-18 13:39:08.000000 timeflux-ui-0.5.2/apps/demo.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 13:39:32.951049 timeflux-ui-0.5.2/apps/flicker/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 13:39:32.947049 timeflux-ui-0.5.2/apps/flicker/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 13:39:32.951049 timeflux-ui-0.5.2/apps/flicker/assets/css/
--rw-r--r--   0 runner    (1001) docker     (123)      554 2022-12-18 13:39:08.000000 timeflux-ui-0.5.2/apps/flicker/assets/css/style.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 13:39:32.951049 timeflux-ui-0.5.2/apps/flicker/assets/js/
--rw-r--r--   0 runner    (1001) docker     (123)      803 2022-12-18 13:39:08.000000 timeflux-ui-0.5.2/apps/flicker/assets/js/app.js
--rw-r--r--   0 runner    (1001) docker     (123)     6233 2022-12-18 13:39:08.000000 timeflux-ui-0.5.2/apps/flicker/assets/js/flicker.js
--rw-r--r--   0 runner    (1001) docker     (123)    18082 2022-12-18 13:39:08.000000 timeflux-ui-0.5.2/apps/flicker/assets/js/states.js
--rw-r--r--   0 runner    (1001) docker     (123)      636 2022-12-18 13:39:08.000000 timeflux-ui-0.5.2/apps/flicker/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2022-12-18 13:39:08.000000 timeflux-ui-0.5.2/apps/flicker.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 13:39:32.951049 timeflux-ui-0.5.2/apps/oddball/
--rw-r--r--   0 runner    (1001) docker     (123)      756 2022-12-18 13:39:08.000000 timeflux-ui-0.5.2/apps/oddball/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 13:39:32.947049 timeflux-ui-0.5.2/apps/oddball/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 13:39:32.951049 timeflux-ui-0.5.2/apps/oddball/assets/css/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-18 13:39:08.000000 timeflux-ui-0.5.2/apps/oddball/assets/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2022-12-18 13:39:08.000000 timeflux-ui-0.5.2/apps/oddball/assets/css/style.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 13:39:32.951049 timeflux-ui-0.5.2/apps/oddball/assets/js/
--rw-r--r--   0 runner    (1001) docker     (123)    12217 2022-12-18 13:39:08.000000 timeflux-ui-0.5.2/apps/oddball/assets/js/app.js
--rw-r--r--   0 runner    (1001) docker     (123)      541 2022-12-18 13:39:08.000000 timeflux-ui-0.5.2/apps/oddball/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      593 2022-12-18 13:39:08.000000 timeflux-ui-0.5.2/apps/oddball.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 13:39:32.951049 timeflux-ui-0.5.2/apps/operator/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 13:39:32.951049 timeflux-ui-0.5.2/apps/operator/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2022-12-18 13:39:08.000000 timeflux-ui-0.5.2/apps/operator/assets/app.js
--rw-r--r--   0 runner    (1001) docker     (123)     3849 2022-12-18 13:39:08.000000 timeflux-ui-0.5.2/apps/operator/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2022-12-18 13:39:08.000000 timeflux-ui-0.5.2/apps/operator.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 13:39:32.955049 timeflux-ui-0.5.2/apps/settings/
--rw-r--r--   0 runner    (1001) docker     (123)      302 2022-12-18 13:39:08.000000 timeflux-ui-0.5.2/apps/settings/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      325 2022-12-18 13:39:08.000000 timeflux-ui-0.5.2/apps/settings.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 13:39:32.955049 timeflux-ui-0.5.2/apps/speller/
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2022-12-18 13:39:08.000000 timeflux-ui-0.5.2/apps/speller/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 13:39:32.947049 timeflux-ui-0.5.2/apps/speller/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 13:39:32.955049 timeflux-ui-0.5.2/apps/speller/assets/css/
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2022-12-18 13:39:08.000000 timeflux-ui-0.5.2/apps/speller/assets/css/app.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 13:39:32.955049 timeflux-ui-0.5.2/apps/speller/assets/js/
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2022-12-18 13:39:08.000000 timeflux-ui-0.5.2/apps/speller/assets/js/app.js
--rw-r--r--   0 runner    (1001) docker     (123)    11371 2022-12-18 13:39:08.000000 timeflux-ui-0.5.2/apps/speller/assets/js/speller.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 13:39:32.955049 timeflux-ui-0.5.2/apps/speller/assets/wav/
--rw-r--r--   0 runner    (1001) docker     (123)     3424 2022-12-18 13:39:08.000000 timeflux-ui-0.5.2/apps/speller/assets/wav/beep.wav
--rw-r--r--   0 runner    (1001) docker     (123)      676 2022-12-18 13:39:08.000000 timeflux-ui-0.5.2/apps/speller/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      371 2022-12-18 13:39:08.000000 timeflux-ui-0.5.2/apps/speller.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 13:39:32.955049 timeflux-ui-0.5.2/apps/sqi/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 13:39:32.955049 timeflux-ui-0.5.2/apps/sqi/assets/
--rw-r--r--   0 runner    (1001) docker     (123)      775 2022-12-18 13:39:08.000000 timeflux-ui-0.5.2/apps/sqi/assets/app.js
--rw-r--r--   0 runner    (1001) docker     (123)    61205 2022-12-18 13:39:08.000000 timeflux-ui-0.5.2/apps/sqi/assets/eeg_10-20.svg
--rw-r--r--   0 runner    (1001) docker     (123)      381 2022-12-18 13:39:08.000000 timeflux-ui-0.5.2/apps/sqi/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      484 2022-12-18 13:39:08.000000 timeflux-ui-0.5.2/apps/sqi.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 13:39:32.955049 timeflux-ui-0.5.2/apps/stim/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 13:39:32.947049 timeflux-ui-0.5.2/apps/stim/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 13:39:32.955049 timeflux-ui-0.5.2/apps/stim/assets/js/
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2022-12-18 13:39:08.000000 timeflux-ui-0.5.2/apps/stim/assets/js/app.js
--rw-r--r--   0 runner    (1001) docker     (123)      317 2022-12-18 13:39:08.000000 timeflux-ui-0.5.2/apps/stim/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      146 2022-12-18 13:39:08.000000 timeflux-ui-0.5.2/apps/stim.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 13:39:32.947049 timeflux-ui-0.5.2/doc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 13:39:32.947049 timeflux-ui-0.5.2/doc/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 13:39:32.955049 timeflux-ui-0.5.2/doc/static/img/
--rw-r--r--   0 runner    (1001) docker     (123)  1275742 2022-12-18 13:39:08.000000 timeflux-ui-0.5.2/doc/static/img/screenshot.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 13:39:32.955049 timeflux-ui-0.5.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2022-12-18 13:39:08.000000 timeflux-ui-0.5.2/examples/custom.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 13:39:32.955049 timeflux-ui-0.5.2/examples/mywebapp/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2022-12-18 13:39:08.000000 timeflux-ui-0.5.2/examples/mywebapp/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      655 2022-12-18 13:39:08.000000 timeflux-ui-0.5.2/examples/options.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      838 2022-12-18 13:39:08.000000 timeflux-ui-0.5.2/examples/ui.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      326 2022-12-18 13:39:08.000000 timeflux-ui-0.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2022-12-18 13:39:32.963050 timeflux-ui-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      147 2022-12-18 13:39:08.000000 timeflux-ui-0.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 13:39:32.955049 timeflux-ui-0.5.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2022-12-18 13:39:08.000000 timeflux-ui-0.5.2/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       71 2022-12-18 13:39:08.000000 timeflux-ui-0.5.2/test/test_ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 13:39:32.955049 timeflux-ui-0.5.2/timeflux_ui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-18 13:39:08.000000 timeflux-ui-0.5.2/timeflux_ui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 13:39:32.959049 timeflux-ui-0.5.2/timeflux_ui/nodes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-18 13:39:08.000000 timeflux-ui-0.5.2/timeflux_ui/nodes/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12311 2022-12-18 13:39:08.000000 timeflux-ui-0.5.2/timeflux_ui/nodes/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 13:39:32.947049 timeflux-ui-0.5.2/timeflux_ui/www/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 13:39:32.947049 timeflux-ui-0.5.2/timeflux_ui/www/common/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 13:39:32.947049 timeflux-ui-0.5.2/timeflux_ui/www/common/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 13:39:32.959049 timeflux-ui-0.5.2/timeflux_ui/www/common/assets/css/
--rw-r--r--   0 runner    (1001) docker     (123)   229605 2022-12-18 13:39:08.000000 timeflux-ui-0.5.2/timeflux_ui/www/common/assets/css/bulma.css
--rw-r--r--   0 runner    (1001) docker     (123)    88231 2022-12-18 13:39:08.000000 timeflux-ui-0.5.2/timeflux_ui/www/common/assets/css/bulma.css.map
--rw-r--r--   0 runner    (1001) docker     (123)   194420 2022-12-18 13:39:08.000000 timeflux-ui-0.5.2/timeflux_ui/www/common/assets/css/bulma.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 13:39:32.959049 timeflux-ui-0.5.2/timeflux_ui/www/common/assets/js/
--rw-r--r--   0 runner    (1001) docker     (123)   914267 2022-12-18 13:39:08.000000 timeflux-ui-0.5.2/timeflux_ui/www/common/assets/js/fa.js
--rw-r--r--   0 runner    (1001) docker     (123)    13889 2022-12-18 13:39:08.000000 timeflux-ui-0.5.2/timeflux_ui/www/common/assets/js/timeflux.js
--rw-r--r--   0 runner    (1001) docker     (123)   341462 2022-12-18 13:39:08.000000 timeflux-ui-0.5.2/timeflux_ui/www/common/assets/js/vue.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 13:39:32.963050 timeflux-ui-0.5.2/timeflux_ui/www/monitor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 13:39:32.951049 timeflux-ui-0.5.2/timeflux_ui/www/monitor/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 13:39:32.963050 timeflux-ui-0.5.2/timeflux_ui/www/monitor/assets/css/
--rw-r--r--   0 runner    (1001) docker     (123)      397 2022-12-18 13:39:08.000000 timeflux-ui-0.5.2/timeflux_ui/www/monitor/assets/css/ui.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 13:39:32.963050 timeflux-ui-0.5.2/timeflux_ui/www/monitor/assets/img/
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2022-12-18 13:39:08.000000 timeflux-ui-0.5.2/timeflux_ui/www/monitor/assets/img/timeflux_logo_white.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 13:39:32.963050 timeflux-ui-0.5.2/timeflux_ui/www/monitor/assets/js/
--rw-r--r--   0 runner    (1001) docker     (123)    44509 2022-12-18 13:39:08.000000 timeflux-ui-0.5.2/timeflux_ui/www/monitor/assets/js/smoothie.js
--rw-r--r--   0 runner    (1001) docker     (123)     5085 2022-12-18 13:39:08.000000 timeflux-ui-0.5.2/timeflux_ui/www/monitor/assets/js/ui.js
--rw-r--r--   0 runner    (1001) docker     (123)     5472 2022-12-18 13:39:08.000000 timeflux-ui-0.5.2/timeflux_ui/www/monitor/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 13:39:32.959049 timeflux-ui-0.5.2/timeflux_ui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2022-12-18 13:39:32.000000 timeflux-ui-0.5.2/timeflux_ui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2022-12-18 13:39:32.000000 timeflux-ui-0.5.2/timeflux_ui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-18 13:39:32.000000 timeflux-ui-0.5.2/timeflux_ui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2022-12-18 13:39:32.000000 timeflux-ui-0.5.2/timeflux_ui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2022-12-18 13:39:32.000000 timeflux-ui-0.5.2/timeflux_ui.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:56:42.900623 timeflux-ui-0.6.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:56:42.876623 timeflux-ui-0.6.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:56:42.884623 timeflux-ui-0.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-06-04 12:56:16.000000 timeflux-ui-0.6.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-04 12:56:16.000000 timeflux-ui-0.6.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-04 12:56:16.000000 timeflux-ui-0.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-04 12:56:16.000000 timeflux-ui-0.6.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-04 12:56:16.000000 timeflux-ui-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-04 12:56:16.000000 timeflux-ui-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-06-04 12:56:42.900623 timeflux-ui-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-04 12:56:16.000000 timeflux-ui-0.6.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:56:42.884623 timeflux-ui-0.6.0/apps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:56:42.884623 timeflux-ui-0.6.0/apps/circle/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:56:42.884623 timeflux-ui-0.6.0/apps/circle/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-06-04 12:56:16.000000 timeflux-ui-0.6.0/apps/circle/assets/app.js
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-04 12:56:16.000000 timeflux-ui-0.6.0/apps/circle/assets/style.css
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-04 12:56:16.000000 timeflux-ui-0.6.0/apps/circle/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-04 12:56:16.000000 timeflux-ui-0.6.0/apps/circle.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:56:42.884623 timeflux-ui-0.6.0/apps/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-04 12:56:16.000000 timeflux-ui-0.6.0/apps/demo/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-06-04 12:56:16.000000 timeflux-ui-0.6.0/apps/demo.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:56:42.884623 timeflux-ui-0.6.0/apps/flicker/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:56:42.876623 timeflux-ui-0.6.0/apps/flicker/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:56:42.884623 timeflux-ui-0.6.0/apps/flicker/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-04 12:56:16.000000 timeflux-ui-0.6.0/apps/flicker/assets/css/style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:56:42.888623 timeflux-ui-0.6.0/apps/flicker/assets/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-04 12:56:16.000000 timeflux-ui-0.6.0/apps/flicker/assets/js/app.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-06-04 12:56:16.000000 timeflux-ui-0.6.0/apps/flicker/assets/js/flicker.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18082 2023-06-04 12:56:16.000000 timeflux-ui-0.6.0/apps/flicker/assets/js/states.js
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-06-04 12:56:16.000000 timeflux-ui-0.6.0/apps/flicker/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-06-04 12:56:16.000000 timeflux-ui-0.6.0/apps/flicker.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:56:42.888623 timeflux-ui-0.6.0/apps/oddball/
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-04 12:56:16.000000 timeflux-ui-0.6.0/apps/oddball/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:56:42.880623 timeflux-ui-0.6.0/apps/oddball/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:56:42.888623 timeflux-ui-0.6.0/apps/oddball/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:56:16.000000 timeflux-ui-0.6.0/apps/oddball/assets/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-06-04 12:56:16.000000 timeflux-ui-0.6.0/apps/oddball/assets/css/style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:56:42.888623 timeflux-ui-0.6.0/apps/oddball/assets/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    12217 2023-06-04 12:56:16.000000 timeflux-ui-0.6.0/apps/oddball/assets/js/app.js
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-06-04 12:56:16.000000 timeflux-ui-0.6.0/apps/oddball/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-04 12:56:16.000000 timeflux-ui-0.6.0/apps/oddball.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:56:42.888623 timeflux-ui-0.6.0/apps/operator/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:56:42.888623 timeflux-ui-0.6.0/apps/operator/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-06-04 12:56:16.000000 timeflux-ui-0.6.0/apps/operator/assets/app.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-06-04 12:56:16.000000 timeflux-ui-0.6.0/apps/operator/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-06-04 12:56:16.000000 timeflux-ui-0.6.0/apps/operator.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:56:42.888623 timeflux-ui-0.6.0/apps/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-04 12:56:16.000000 timeflux-ui-0.6.0/apps/settings/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-04 12:56:16.000000 timeflux-ui-0.6.0/apps/settings.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:56:42.888623 timeflux-ui-0.6.0/apps/speller/
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-06-04 12:56:16.000000 timeflux-ui-0.6.0/apps/speller/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:56:42.880623 timeflux-ui-0.6.0/apps/speller/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:56:42.888623 timeflux-ui-0.6.0/apps/speller/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-06-04 12:56:16.000000 timeflux-ui-0.6.0/apps/speller/assets/css/app.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:56:42.888623 timeflux-ui-0.6.0/apps/speller/assets/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-06-04 12:56:16.000000 timeflux-ui-0.6.0/apps/speller/assets/js/app.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11371 2023-06-04 12:56:16.000000 timeflux-ui-0.6.0/apps/speller/assets/js/speller.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:56:42.888623 timeflux-ui-0.6.0/apps/speller/assets/wav/
+-rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-06-04 12:56:16.000000 timeflux-ui-0.6.0/apps/speller/assets/wav/beep.wav
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-04 12:56:16.000000 timeflux-ui-0.6.0/apps/speller/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-04 12:56:16.000000 timeflux-ui-0.6.0/apps/speller.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:56:42.888623 timeflux-ui-0.6.0/apps/sqi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:56:42.888623 timeflux-ui-0.6.0/apps/sqi/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-04 12:56:16.000000 timeflux-ui-0.6.0/apps/sqi/assets/app.js
+-rw-r--r--   0 runner    (1001) docker     (123)    61205 2023-06-04 12:56:16.000000 timeflux-ui-0.6.0/apps/sqi/assets/eeg_10-20.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-04 12:56:16.000000 timeflux-ui-0.6.0/apps/sqi/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-04 12:56:16.000000 timeflux-ui-0.6.0/apps/sqi.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:56:42.888623 timeflux-ui-0.6.0/apps/stim/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:56:42.880623 timeflux-ui-0.6.0/apps/stim/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:56:42.888623 timeflux-ui-0.6.0/apps/stim/assets/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-04 12:56:16.000000 timeflux-ui-0.6.0/apps/stim/assets/js/app.js
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-04 12:56:16.000000 timeflux-ui-0.6.0/apps/stim/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-04 12:56:16.000000 timeflux-ui-0.6.0/apps/stim.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:56:42.880623 timeflux-ui-0.6.0/doc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:56:42.880623 timeflux-ui-0.6.0/doc/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:56:42.892623 timeflux-ui-0.6.0/doc/static/img/
+-rw-r--r--   0 runner    (1001) docker     (123)  1275742 2023-06-04 12:56:16.000000 timeflux-ui-0.6.0/doc/static/img/screenshot.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:56:42.892623 timeflux-ui-0.6.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-04 12:56:16.000000 timeflux-ui-0.6.0/examples/custom.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:56:42.892623 timeflux-ui-0.6.0/examples/mywebapp/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-04 12:56:16.000000 timeflux-ui-0.6.0/examples/mywebapp/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-04 12:56:16.000000 timeflux-ui-0.6.0/examples/options.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-04 12:56:16.000000 timeflux-ui-0.6.0/examples/ui.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-04 12:56:16.000000 timeflux-ui-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-04 12:56:42.900623 timeflux-ui-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-04 12:56:16.000000 timeflux-ui-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:56:42.892623 timeflux-ui-0.6.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-04 12:56:16.000000 timeflux-ui-0.6.0/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-04 12:56:16.000000 timeflux-ui-0.6.0/test/test_ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:56:42.892623 timeflux-ui-0.6.0/timeflux_ui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:56:16.000000 timeflux-ui-0.6.0/timeflux_ui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:56:42.896623 timeflux-ui-0.6.0/timeflux_ui/nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:56:16.000000 timeflux-ui-0.6.0/timeflux_ui/nodes/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12310 2023-06-04 12:56:16.000000 timeflux-ui-0.6.0/timeflux_ui/nodes/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:56:42.880623 timeflux-ui-0.6.0/timeflux_ui/www/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:56:42.880623 timeflux-ui-0.6.0/timeflux_ui/www/common/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:56:42.880623 timeflux-ui-0.6.0/timeflux_ui/www/common/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:56:42.896623 timeflux-ui-0.6.0/timeflux_ui/www/common/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   229605 2023-06-04 12:56:16.000000 timeflux-ui-0.6.0/timeflux_ui/www/common/assets/css/bulma.css
+-rw-r--r--   0 runner    (1001) docker     (123)    88231 2023-06-04 12:56:16.000000 timeflux-ui-0.6.0/timeflux_ui/www/common/assets/css/bulma.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)   194420 2023-06-04 12:56:16.000000 timeflux-ui-0.6.0/timeflux_ui/www/common/assets/css/bulma.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:56:42.896623 timeflux-ui-0.6.0/timeflux_ui/www/common/assets/js/
+-rw-r--r--   0 runner    (1001) docker     (123)   914267 2023-06-04 12:56:16.000000 timeflux-ui-0.6.0/timeflux_ui/www/common/assets/js/fa.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14437 2023-06-04 12:56:16.000000 timeflux-ui-0.6.0/timeflux_ui/www/common/assets/js/timeflux.js
+-rw-r--r--   0 runner    (1001) docker     (123)   341462 2023-06-04 12:56:16.000000 timeflux-ui-0.6.0/timeflux_ui/www/common/assets/js/vue.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:56:42.896623 timeflux-ui-0.6.0/timeflux_ui/www/monitor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:56:42.880623 timeflux-ui-0.6.0/timeflux_ui/www/monitor/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:56:42.900623 timeflux-ui-0.6.0/timeflux_ui/www/monitor/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-04 12:56:16.000000 timeflux-ui-0.6.0/timeflux_ui/www/monitor/assets/css/ui.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:56:42.900623 timeflux-ui-0.6.0/timeflux_ui/www/monitor/assets/img/
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-06-04 12:56:16.000000 timeflux-ui-0.6.0/timeflux_ui/www/monitor/assets/img/timeflux_logo_white.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:56:42.900623 timeflux-ui-0.6.0/timeflux_ui/www/monitor/assets/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    44509 2023-06-04 12:56:16.000000 timeflux-ui-0.6.0/timeflux_ui/www/monitor/assets/js/smoothie.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-06-04 12:56:16.000000 timeflux-ui-0.6.0/timeflux_ui/www/monitor/assets/js/ui.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-06-04 12:56:16.000000 timeflux-ui-0.6.0/timeflux_ui/www/monitor/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:56:42.892623 timeflux-ui-0.6.0/timeflux_ui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-06-04 12:56:42.000000 timeflux-ui-0.6.0/timeflux_ui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-04 12:56:42.000000 timeflux-ui-0.6.0/timeflux_ui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 12:56:42.000000 timeflux-ui-0.6.0/timeflux_ui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-04 12:56:42.000000 timeflux-ui-0.6.0/timeflux_ui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-04 12:56:42.000000 timeflux-ui-0.6.0/timeflux_ui.egg-info/top_level.txt
```

### Comparing `timeflux-ui-0.5.2/.github/workflows/build.yml` & `timeflux-ui-0.6.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `timeflux-ui-0.5.2/.github/workflows/publish.yml` & `timeflux-ui-0.6.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `timeflux-ui-0.5.2/LICENSE` & `timeflux-ui-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `timeflux-ui-0.5.2/PKG-INFO` & `timeflux-ui-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timeflux-ui
-Version: 0.5.2
+Version: 0.6.0
 Summary: Timeflux web app engine
 Home-page: https://timeflux.io
 Author: Pierre Clisson
 Author-email: contact@timeflux.io
 License: MIT
 Project-URL: Documentation, http://doc.timeflux.io/projects/timeflux-ui/
 Project-URL: Source Code, https://github.com/timeflux/timeflux_ui
```

### Comparing `timeflux-ui-0.5.2/README.rst` & `timeflux-ui-0.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `timeflux-ui-0.5.2/apps/circle/assets/app.js` & `timeflux-ui-0.6.0/apps/circle/assets/app.js`

 * *Files identical despite different names*

### Comparing `timeflux-ui-0.5.2/apps/demo/index.html` & `timeflux-ui-0.6.0/apps/demo/index.html`

 * *Files identical despite different names*

### Comparing `timeflux-ui-0.5.2/apps/demo.yaml` & `timeflux-ui-0.6.0/apps/demo.yaml`

 * *Files identical despite different names*

### Comparing `timeflux-ui-0.5.2/apps/flicker/assets/css/style.css` & `timeflux-ui-0.6.0/apps/flicker/assets/css/style.css`

 * *Files identical despite different names*

### Comparing `timeflux-ui-0.5.2/apps/flicker/assets/js/app.js` & `timeflux-ui-0.6.0/apps/flicker/assets/js/app.js`

 * *Files identical despite different names*

### Comparing `timeflux-ui-0.5.2/apps/flicker/assets/js/flicker.js` & `timeflux-ui-0.6.0/apps/flicker/assets/js/flicker.js`

 * *Files identical despite different names*

### Comparing `timeflux-ui-0.5.2/apps/flicker/assets/js/states.js` & `timeflux-ui-0.6.0/apps/flicker/assets/js/states.js`

 * *Files identical despite different names*

### Comparing `timeflux-ui-0.5.2/apps/flicker/index.html` & `timeflux-ui-0.6.0/apps/flicker/index.html`

 * *Files identical despite different names*

### Comparing `timeflux-ui-0.5.2/apps/flicker.yaml` & `timeflux-ui-0.6.0/apps/flicker.yaml`

 * *Files identical despite different names*

### Comparing `timeflux-ui-0.5.2/apps/oddball/README.md` & `timeflux-ui-0.6.0/apps/oddball/README.md`

 * *Files identical despite different names*

### Comparing `timeflux-ui-0.5.2/apps/oddball/assets/css/style.css` & `timeflux-ui-0.6.0/apps/oddball/assets/css/style.css`

 * *Files identical despite different names*

### Comparing `timeflux-ui-0.5.2/apps/oddball/assets/js/app.js` & `timeflux-ui-0.6.0/apps/oddball/assets/js/app.js`

 * *Files identical despite different names*

### Comparing `timeflux-ui-0.5.2/apps/oddball/index.html` & `timeflux-ui-0.6.0/apps/oddball/index.html`

 * *Files identical despite different names*

### Comparing `timeflux-ui-0.5.2/apps/oddball.yaml` & `timeflux-ui-0.6.0/apps/oddball.yaml`

 * *Files identical despite different names*

### Comparing `timeflux-ui-0.5.2/apps/operator/assets/app.js` & `timeflux-ui-0.6.0/apps/operator/assets/app.js`

 * *Files identical despite different names*

### Comparing `timeflux-ui-0.5.2/apps/operator/index.html` & `timeflux-ui-0.6.0/apps/operator/index.html`

 * *Files identical despite different names*

### Comparing `timeflux-ui-0.5.2/apps/operator.yaml` & `timeflux-ui-0.6.0/apps/operator.yaml`

 * *Files identical despite different names*

### Comparing `timeflux-ui-0.5.2/apps/speller/README.md` & `timeflux-ui-0.6.0/apps/speller/README.md`

 * *Files identical despite different names*

### Comparing `timeflux-ui-0.5.2/apps/speller/assets/css/app.css` & `timeflux-ui-0.6.0/apps/speller/assets/css/app.css`

 * *Files identical despite different names*

### Comparing `timeflux-ui-0.5.2/apps/speller/assets/js/app.js` & `timeflux-ui-0.6.0/apps/speller/assets/js/app.js`

 * *Files identical despite different names*

### Comparing `timeflux-ui-0.5.2/apps/speller/assets/js/speller.js` & `timeflux-ui-0.6.0/apps/speller/assets/js/speller.js`

 * *Files identical despite different names*

### Comparing `timeflux-ui-0.5.2/apps/speller/assets/wav/beep.wav` & `timeflux-ui-0.6.0/apps/speller/assets/wav/beep.wav`

 * *Files identical despite different names*

### Comparing `timeflux-ui-0.5.2/apps/speller/index.html` & `timeflux-ui-0.6.0/apps/speller/index.html`

 * *Files identical despite different names*

### Comparing `timeflux-ui-0.5.2/apps/sqi/assets/app.js` & `timeflux-ui-0.6.0/apps/sqi/assets/app.js`

 * *Files identical despite different names*

### Comparing `timeflux-ui-0.5.2/apps/sqi/assets/eeg_10-20.svg` & `timeflux-ui-0.6.0/apps/sqi/assets/eeg_10-20.svg`

 * *Files identical despite different names*

### Comparing `timeflux-ui-0.5.2/apps/stim/assets/js/app.js` & `timeflux-ui-0.6.0/apps/stim/assets/js/app.js`

 * *Files identical despite different names*

### Comparing `timeflux-ui-0.5.2/doc/static/img/screenshot.png` & `timeflux-ui-0.6.0/doc/static/img/screenshot.png`

 * *Files identical despite different names*

### Comparing `timeflux-ui-0.5.2/examples/options.yaml` & `timeflux-ui-0.6.0/examples/options.yaml`

 * *Files identical despite different names*

### Comparing `timeflux-ui-0.5.2/examples/ui.yaml` & `timeflux-ui-0.6.0/examples/ui.yaml`

 * *Files identical despite different names*

### Comparing `timeflux-ui-0.5.2/setup.cfg` & `timeflux-ui-0.6.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `timeflux-ui-0.5.2/timeflux_ui/nodes/ui.py` & `timeflux-ui-0.6.0/timeflux_ui/nodes/ui.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,14 @@
            :language: yaml
 
     """
 
     def __init__(
         self, host="localhost", port=8000, routes={}, settings={}, debug=False
     ):
-
         """
         Args:
             host (string): The host to bind to.
             port (int): The port to listen to.
             routes (dict): A dictionary of custom web apps. Key is the name, value is the path.
             settings (dict): An arbitrary configuration file that will be exposed to web apps.
             debug (bool): Show dependencies debug information.
```

### Comparing `timeflux-ui-0.5.2/timeflux_ui/www/common/assets/css/bulma.css` & `timeflux-ui-0.6.0/timeflux_ui/www/common/assets/css/bulma.css`

 * *Files identical despite different names*

### Comparing `timeflux-ui-0.5.2/timeflux_ui/www/common/assets/css/bulma.css.map` & `timeflux-ui-0.6.0/timeflux_ui/www/common/assets/css/bulma.css.map`

 * *Files identical despite different names*

### Comparing `timeflux-ui-0.5.2/timeflux_ui/www/common/assets/css/bulma.min.css` & `timeflux-ui-0.6.0/timeflux_ui/www/common/assets/css/bulma.min.css`

 * *Files identical despite different names*

### Comparing `timeflux-ui-0.5.2/timeflux_ui/www/common/assets/js/fa.js` & `timeflux-ui-0.6.0/timeflux_ui/www/common/assets/js/fa.js`

 * *Files identical despite different names*

### Comparing `timeflux-ui-0.5.2/timeflux_ui/www/common/assets/js/timeflux.js` & `timeflux-ui-0.6.0/timeflux_ui/www/common/assets/js/timeflux.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -517,14 +517,42 @@
             }
         };
         document.addEventListener('keydown', handler);
     });
 }
 
 /**
+ * Resolve promise on event
+ *
+ * @param {string} name - event name
+ * @returns {Promise}
+ */
+function flag(name) {
+    return new Promise((resolve) => {
+        const handler = (event) => {
+            document.removeEventListener(event.type, handler);
+            resolve(event.detail);
+        };
+        document.addEventListener(name, handler);
+    });
+}
+
+/**
+ * Trigger an event
+ *
+ * @param {string} name - Event name
+ * @param {object} [data] - Optional data
+ */
+function trigger(name, data) {
+    document.dispatchEvent(new CustomEvent(name, {
+        detail: data
+    }));
+}
+
+/**
  * Load settings
  *
  * Use like this: load_settings().then(settings => { doSomething(); });
  *
  * @returns {Promise<Object>} a promise that contains the settings object
  */
 async function load_settings() {
```

### Comparing `timeflux-ui-0.5.2/timeflux_ui/www/common/assets/js/vue.js` & `timeflux-ui-0.6.0/timeflux_ui/www/common/assets/js/vue.js`

 * *Files identical despite different names*

### Comparing `timeflux-ui-0.5.2/timeflux_ui/www/monitor/assets/img/timeflux_logo_white.png` & `timeflux-ui-0.6.0/timeflux_ui/www/monitor/assets/img/timeflux_logo_white.png`

 * *Files identical despite different names*

### Comparing `timeflux-ui-0.5.2/timeflux_ui/www/monitor/assets/js/smoothie.js` & `timeflux-ui-0.6.0/timeflux_ui/www/monitor/assets/js/smoothie.js`

 * *Files identical despite different names*

### Comparing `timeflux-ui-0.5.2/timeflux_ui/www/monitor/assets/js/ui.js` & `timeflux-ui-0.6.0/timeflux_ui/www/monitor/assets/js/ui.js`

 * *Files identical despite different names*

### Comparing `timeflux-ui-0.5.2/timeflux_ui/www/monitor/index.html` & `timeflux-ui-0.6.0/timeflux_ui/www/monitor/index.html`

 * *Files identical despite different names*

### Comparing `timeflux-ui-0.5.2/timeflux_ui.egg-info/PKG-INFO` & `timeflux-ui-0.6.0/timeflux_ui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timeflux-ui
-Version: 0.5.2
+Version: 0.6.0
 Summary: Timeflux web app engine
 Home-page: https://timeflux.io
 Author: Pierre Clisson
 Author-email: contact@timeflux.io
 License: MIT
 Project-URL: Documentation, http://doc.timeflux.io/projects/timeflux-ui/
 Project-URL: Source Code, https://github.com/timeflux/timeflux_ui
```

### Comparing `timeflux-ui-0.5.2/timeflux_ui.egg-info/SOURCES.txt` & `timeflux-ui-0.6.0/timeflux_ui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

