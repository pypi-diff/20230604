# Comparing `tmp/circuitpython-mag-cal-1.1.4.tar.gz` & `tmp/circuitpython-mag-cal-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitpython-mag-cal-1.1.4.tar", last modified: Thu Jun  1 21:27:55 2023, max compression
+gzip compressed data, was "circuitpython-mag-cal-1.2.0.tar", last modified: Sun Jun  4 12:19:23 2023, max compression
```

## Comparing `circuitpython-mag-cal-1.1.4.tar` & `circuitpython-mag-cal-1.2.0.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:27:55.527908 circuitpython-mag-cal-1.1.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:27:55.519908 circuitpython-mag-cal-1.1.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:27:55.519908 circuitpython-mag-cal-1.1.4/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-01 21:27:40.000000 circuitpython-mag-cal-1.1.4/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:27:55.519908 circuitpython-mag-cal-1.1.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-01 21:27:40.000000 circuitpython-mag-cal-1.1.4/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-01 21:27:40.000000 circuitpython-mag-cal-1.1.4/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-01 21:27:40.000000 circuitpython-mag-cal-1.1.4/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-01 21:27:40.000000 circuitpython-mag-cal-1.1.4/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-01 21:27:40.000000 circuitpython-mag-cal-1.1.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-01 21:27:40.000000 circuitpython-mag-cal-1.1.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-06-01 21:27:40.000000 circuitpython-mag-cal-1.1.4/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-06-01 21:27:40.000000 circuitpython-mag-cal-1.1.4/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-01 21:27:40.000000 circuitpython-mag-cal-1.1.4/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:27:55.523908 circuitpython-mag-cal-1.1.4/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-06-01 21:27:40.000000 circuitpython-mag-cal-1.1.4/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-01 21:27:40.000000 circuitpython-mag-cal-1.1.4/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-01 21:27:40.000000 circuitpython-mag-cal-1.1.4/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-06-01 21:27:55.527908 circuitpython-mag-cal-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-06-01 21:27:40.000000 circuitpython-mag-cal-1.1.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-01 21:27:40.000000 circuitpython-mag-cal-1.1.4/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:27:55.523908 circuitpython-mag-cal-1.1.4/circuitpython_mag_cal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-06-01 21:27:55.000000 circuitpython-mag-cal-1.1.4/circuitpython_mag_cal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-01 21:27:55.000000 circuitpython-mag-cal-1.1.4/circuitpython_mag_cal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 21:27:55.000000 circuitpython-mag-cal-1.1.4/circuitpython_mag_cal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-01 21:27:55.000000 circuitpython-mag-cal-1.1.4/circuitpython_mag_cal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-01 21:27:55.000000 circuitpython-mag-cal-1.1.4/circuitpython_mag_cal.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:27:55.523908 circuitpython-mag-cal-1.1.4/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:27:55.523908 circuitpython-mag-cal-1.1.4/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-01 21:27:40.000000 circuitpython-mag-cal-1.1.4/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-01 21:27:40.000000 circuitpython-mag-cal-1.1.4/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-01 21:27:40.000000 circuitpython-mag-cal-1.1.4/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-01 21:27:40.000000 circuitpython-mag-cal-1.1.4/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5656 2023-06-01 21:27:40.000000 circuitpython-mag-cal-1.1.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-01 21:27:40.000000 circuitpython-mag-cal-1.1.4/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-01 21:27:40.000000 circuitpython-mag-cal-1.1.4/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     7767 2023-06-01 21:27:40.000000 circuitpython-mag-cal-1.1.4/docs/howto.rst
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-01 21:27:40.000000 circuitpython-mag-cal-1.1.4/docs/howto.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-01 21:27:40.000000 circuitpython-mag-cal-1.1.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-01 21:27:40.000000 circuitpython-mag-cal-1.1.4/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-01 21:27:40.000000 circuitpython-mag-cal-1.1.4/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:27:55.523908 circuitpython-mag-cal-1.1.4/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-01 21:27:48.000000 circuitpython-mag-cal-1.1.4/examples/mag_cal_simpletest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:27:55.523908 circuitpython-mag-cal-1.1.4/mag_cal/
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-01 21:27:48.000000 circuitpython-mag-cal-1.1.4/mag_cal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-06-01 21:27:48.000000 circuitpython-mag-cal-1.1.4/mag_cal/axes.py
--rw-r--r--   0 runner    (1001) docker     (123)    25357 2023-06-01 21:27:48.000000 circuitpython-mag-cal-1.1.4/mag_cal/calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-06-01 21:27:48.000000 circuitpython-mag-cal-1.1.4/mag_cal/lstsq.py
--rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-06-01 21:27:48.000000 circuitpython-mag-cal-1.1.4/mag_cal/nm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-06-01 21:27:48.000000 circuitpython-mag-cal-1.1.4/mag_cal/rbf.py
--rw-r--r--   0 runner    (1001) docker     (123)     8756 2023-06-01 21:27:48.000000 circuitpython-mag-cal-1.1.4/mag_cal/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-06-01 21:27:48.000000 circuitpython-mag-cal-1.1.4/mag_cal/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-01 21:27:40.000000 circuitpython-mag-cal-1.1.4/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-01 21:27:48.000000 circuitpython-mag-cal-1.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-01 21:27:40.000000 circuitpython-mag-cal-1.1.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 21:27:55.527908 circuitpython-mag-cal-1.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:27:55.523908 circuitpython-mag-cal-1.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 21:27:48.000000 circuitpython-mag-cal-1.1.4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:27:55.519908 circuitpython-mag-cal-1.1.4/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:27:55.527908 circuitpython-mag-cal-1.1.4/tests/fixtures/cal_data/
--rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-06-01 21:27:40.000000 circuitpython-mag-cal-1.1.4/tests/fixtures/cal_data/ab.json
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-01 21:27:40.000000 circuitpython-mag-cal-1.1.4/tests/fixtures/cal_data/ab.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-06-01 21:27:40.000000 circuitpython-mag-cal-1.1.4/tests/fixtures/cal_data/ai.json
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-01 21:27:40.000000 circuitpython-mag-cal-1.1.4/tests/fixtures/cal_data/ai.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6144 2023-06-01 21:27:40.000000 circuitpython-mag-cal-1.1.4/tests/fixtures/cal_data/bh.json
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-01 21:27:40.000000 circuitpython-mag-cal-1.1.4/tests/fixtures/cal_data/bh.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-06-01 21:27:40.000000 circuitpython-mag-cal-1.1.4/tests/fixtures/cal_data/bi.json
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-01 21:27:40.000000 circuitpython-mag-cal-1.1.4/tests/fixtures/cal_data/bi.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-06-01 21:27:40.000000 circuitpython-mag-cal-1.1.4/tests/fixtures/cal_data/ee.json
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-01 21:27:40.000000 circuitpython-mag-cal-1.1.4/tests/fixtures/cal_data/ee.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-06-01 21:27:40.000000 circuitpython-mag-cal-1.1.4/tests/fixtures/cal_data/fb.json
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-01 21:27:40.000000 circuitpython-mag-cal-1.1.4/tests/fixtures/cal_data/fb.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6135 2023-06-01 21:27:40.000000 circuitpython-mag-cal-1.1.4/tests/fixtures/cal_data/hj.json
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-01 21:27:40.000000 circuitpython-mag-cal-1.1.4/tests/fixtures/cal_data/hj.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-06-01 21:27:40.000000 circuitpython-mag-cal-1.1.4/tests/fixtures/cal_data/hj2.json
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-01 21:27:40.000000 circuitpython-mag-cal-1.1.4/tests/fixtures/cal_data/hj2.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-06-01 21:27:40.000000 circuitpython-mag-cal-1.1.4/tests/fixtures/cal_data/jd.json
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-01 21:27:40.000000 circuitpython-mag-cal-1.1.4/tests/fixtures/cal_data/jd.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-06-01 21:27:48.000000 circuitpython-mag-cal-1.1.4/tests/test_axes.py
--rw-r--r--   0 runner    (1001) docker     (123)     7285 2023-06-01 21:27:48.000000 circuitpython-mag-cal-1.1.4/tests/test_calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-06-01 21:27:48.000000 circuitpython-mag-cal-1.1.4/tests/test_sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:19:23.269393 circuitpython-mag-cal-1.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:19:23.253393 circuitpython-mag-cal-1.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:19:23.257393 circuitpython-mag-cal-1.2.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-04 12:19:03.000000 circuitpython-mag-cal-1.2.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:19:23.257393 circuitpython-mag-cal-1.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-04 12:19:03.000000 circuitpython-mag-cal-1.2.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-04 12:19:03.000000 circuitpython-mag-cal-1.2.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-04 12:19:03.000000 circuitpython-mag-cal-1.2.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-04 12:19:03.000000 circuitpython-mag-cal-1.2.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-04 12:19:03.000000 circuitpython-mag-cal-1.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-04 12:19:03.000000 circuitpython-mag-cal-1.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-06-04 12:19:03.000000 circuitpython-mag-cal-1.2.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-06-04 12:19:03.000000 circuitpython-mag-cal-1.2.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-04 12:19:03.000000 circuitpython-mag-cal-1.2.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:19:23.257393 circuitpython-mag-cal-1.2.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-06-04 12:19:03.000000 circuitpython-mag-cal-1.2.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-04 12:19:03.000000 circuitpython-mag-cal-1.2.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-04 12:19:03.000000 circuitpython-mag-cal-1.2.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-06-04 12:19:23.269393 circuitpython-mag-cal-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-06-04 12:19:03.000000 circuitpython-mag-cal-1.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-04 12:19:03.000000 circuitpython-mag-cal-1.2.0/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:19:23.261392 circuitpython-mag-cal-1.2.0/circuitpython_mag_cal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-06-04 12:19:23.000000 circuitpython-mag-cal-1.2.0/circuitpython_mag_cal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-04 12:19:23.000000 circuitpython-mag-cal-1.2.0/circuitpython_mag_cal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 12:19:23.000000 circuitpython-mag-cal-1.2.0/circuitpython_mag_cal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-04 12:19:23.000000 circuitpython-mag-cal-1.2.0/circuitpython_mag_cal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-04 12:19:23.000000 circuitpython-mag-cal-1.2.0/circuitpython_mag_cal.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:19:23.261392 circuitpython-mag-cal-1.2.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:19:23.261392 circuitpython-mag-cal-1.2.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-04 12:19:03.000000 circuitpython-mag-cal-1.2.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-04 12:19:03.000000 circuitpython-mag-cal-1.2.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-04 12:19:03.000000 circuitpython-mag-cal-1.2.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-04 12:19:03.000000 circuitpython-mag-cal-1.2.0/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5656 2023-06-04 12:19:03.000000 circuitpython-mag-cal-1.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-04 12:19:03.000000 circuitpython-mag-cal-1.2.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-04 12:19:03.000000 circuitpython-mag-cal-1.2.0/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     7767 2023-06-04 12:19:03.000000 circuitpython-mag-cal-1.2.0/docs/howto.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-04 12:19:03.000000 circuitpython-mag-cal-1.2.0/docs/howto.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-04 12:19:03.000000 circuitpython-mag-cal-1.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-04 12:19:03.000000 circuitpython-mag-cal-1.2.0/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-04 12:19:03.000000 circuitpython-mag-cal-1.2.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:19:23.261392 circuitpython-mag-cal-1.2.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-04 12:19:13.000000 circuitpython-mag-cal-1.2.0/examples/mag_cal_simpletest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:19:23.265393 circuitpython-mag-cal-1.2.0/mag_cal/
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-04 12:19:13.000000 circuitpython-mag-cal-1.2.0/mag_cal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-06-04 12:19:13.000000 circuitpython-mag-cal-1.2.0/mag_cal/axes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29733 2023-06-04 12:19:13.000000 circuitpython-mag-cal-1.2.0/mag_cal/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-06-04 12:19:13.000000 circuitpython-mag-cal-1.2.0/mag_cal/lstsq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-06-04 12:19:13.000000 circuitpython-mag-cal-1.2.0/mag_cal/nm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-06-04 12:19:13.000000 circuitpython-mag-cal-1.2.0/mag_cal/rbf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10608 2023-06-04 12:19:13.000000 circuitpython-mag-cal-1.2.0/mag_cal/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-06-04 12:19:13.000000 circuitpython-mag-cal-1.2.0/mag_cal/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-04 12:19:03.000000 circuitpython-mag-cal-1.2.0/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-04 12:19:13.000000 circuitpython-mag-cal-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-04 12:19:03.000000 circuitpython-mag-cal-1.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 12:19:23.269393 circuitpython-mag-cal-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:19:23.265393 circuitpython-mag-cal-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:19:13.000000 circuitpython-mag-cal-1.2.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:19:23.253393 circuitpython-mag-cal-1.2.0/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:19:23.269393 circuitpython-mag-cal-1.2.0/tests/fixtures/cal_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-06-04 12:19:03.000000 circuitpython-mag-cal-1.2.0/tests/fixtures/cal_data/ab.json
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-04 12:19:03.000000 circuitpython-mag-cal-1.2.0/tests/fixtures/cal_data/ab.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-06-04 12:19:03.000000 circuitpython-mag-cal-1.2.0/tests/fixtures/cal_data/ai.json
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-04 12:19:03.000000 circuitpython-mag-cal-1.2.0/tests/fixtures/cal_data/ai.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6144 2023-06-04 12:19:03.000000 circuitpython-mag-cal-1.2.0/tests/fixtures/cal_data/bh.json
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-04 12:19:03.000000 circuitpython-mag-cal-1.2.0/tests/fixtures/cal_data/bh.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-06-04 12:19:03.000000 circuitpython-mag-cal-1.2.0/tests/fixtures/cal_data/bi.json
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-04 12:19:03.000000 circuitpython-mag-cal-1.2.0/tests/fixtures/cal_data/bi.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-06-04 12:19:03.000000 circuitpython-mag-cal-1.2.0/tests/fixtures/cal_data/ee.json
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-04 12:19:03.000000 circuitpython-mag-cal-1.2.0/tests/fixtures/cal_data/ee.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-06-04 12:19:03.000000 circuitpython-mag-cal-1.2.0/tests/fixtures/cal_data/fb.json
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-04 12:19:03.000000 circuitpython-mag-cal-1.2.0/tests/fixtures/cal_data/fb.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6135 2023-06-04 12:19:03.000000 circuitpython-mag-cal-1.2.0/tests/fixtures/cal_data/hj.json
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-04 12:19:03.000000 circuitpython-mag-cal-1.2.0/tests/fixtures/cal_data/hj.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-06-04 12:19:03.000000 circuitpython-mag-cal-1.2.0/tests/fixtures/cal_data/hj2.json
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-04 12:19:03.000000 circuitpython-mag-cal-1.2.0/tests/fixtures/cal_data/hj2.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-06-04 12:19:03.000000 circuitpython-mag-cal-1.2.0/tests/fixtures/cal_data/jd.json
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-04 12:19:03.000000 circuitpython-mag-cal-1.2.0/tests/fixtures/cal_data/jd.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-06-04 12:19:13.000000 circuitpython-mag-cal-1.2.0/tests/test_axes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-06-04 12:19:13.000000 circuitpython-mag-cal-1.2.0/tests/test_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-06-04 12:19:13.000000 circuitpython-mag-cal-1.2.0/tests/test_sensor.py
```

### Comparing `circuitpython-mag-cal-1.1.4/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `circuitpython-mag-cal-1.2.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.4/.gitignore` & `circuitpython-mag-cal-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.4/.pre-commit-config.yaml` & `circuitpython-mag-cal-1.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.4/.pylintrc` & `circuitpython-mag-cal-1.2.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.4/CODE_OF_CONDUCT.md` & `circuitpython-mag-cal-1.2.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.4/LICENSE` & `circuitpython-mag-cal-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.4/LICENSES/CC-BY-4.0.txt` & `circuitpython-mag-cal-1.2.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.4/LICENSES/MIT.txt` & `circuitpython-mag-cal-1.2.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.4/LICENSES/Unlicense.txt` & `circuitpython-mag-cal-1.2.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.4/PKG-INFO` & `circuitpython-mag-cal-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-mag-cal
-Version: 1.1.4
+Version: 1.2.0
 Summary: Calibrate magnetometer and accelerometer readings
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/furbrain/CircuitPython_mag_cal
 Keywords: adafruit,blinka,circuitpython,micropython,mag_cal,magnetometer,accelerometer,compass,calibrate,calibration,gravity,magnetism,magnetic
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `circuitpython-mag-cal-1.1.4/README.rst` & `circuitpython-mag-cal-1.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.4/circuitpython_mag_cal.egg-info/PKG-INFO` & `circuitpython-mag-cal-1.2.0/circuitpython_mag_cal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-mag-cal
-Version: 1.1.4
+Version: 1.2.0
 Summary: Calibrate magnetometer and accelerometer readings
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/furbrain/CircuitPython_mag_cal
 Keywords: adafruit,blinka,circuitpython,micropython,mag_cal,magnetometer,accelerometer,compass,calibrate,calibration,gravity,magnetism,magnetic
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `circuitpython-mag-cal-1.1.4/circuitpython_mag_cal.egg-info/SOURCES.txt` & `circuitpython-mag-cal-1.2.0/circuitpython_mag_cal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.4/docs/_static/favicon.ico` & `circuitpython-mag-cal-1.2.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.4/docs/conf.py` & `circuitpython-mag-cal-1.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.4/docs/howto.rst` & `circuitpython-mag-cal-1.2.0/docs/howto.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.4/docs/index.rst` & `circuitpython-mag-cal-1.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.4/examples/mag_cal_simpletest.py` & `circuitpython-mag-cal-1.2.0/examples/mag_cal_simpletest.py`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.4/mag_cal/__init__.py` & `circuitpython-mag-cal-1.2.0/mag_cal/__init__.py`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.4/mag_cal/axes.py` & `circuitpython-mag-cal-1.2.0/mag_cal/axes.py`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.4/mag_cal/calibration.py` & `circuitpython-mag-cal-1.2.0/mag_cal/calibration.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 """
 Calibration class: main class to use
 """
 from . import nm
 from .rbf import RBF
-from .sensor import Sensor
+from .sensor import Sensor, DEFAULT_SIGMA
 from .utils import normalise, solve_least_squares, cross
 
 try:
     from typing import Tuple, Dict
 except ImportError:
     # ignore if running in CircuitPython/MicroPython
     pass
@@ -18,22 +18,46 @@
 try:
     # work with normal numpy
     import numpy as np
 except ImportError:
     # or work with ulab if we are in CircuitPython
     from ulab import numpy as np
 
-__version__ = "1.1.4"
+__version__ = "1.2.0"
 __repo__ = "https://github.com/furbrain/CircuitPython_mag_cal.git"
 
 
 def _vector_from_matrices(matrix: np.ndarray, i: int, j: int):
     return np.array([x[i, j] for x in matrix])
 
 
+class CalibrationError(Exception):
+    """
+    Some sort of error from the Calibration Module
+    """
+
+
+class DipAnomalyError(CalibrationError):
+    """
+    Dip is not what we would expect it to be
+    """
+
+
+class MagneticAnomalyError(CalibrationError):
+    """
+    Magnetic field strength is not what we would expect it to be
+    """
+
+
+class GravityAnomalyError(CalibrationError):
+    """
+    Gravity field strength is not what we would expect it to be - device moving during shot?
+    """
+
+
 class Calibration:
     """
     Object representing a magnetometer and accelerometer calibration
     """
 
     MAGNETOMETER = 1
     ACCELEROMETER = 2
@@ -62,14 +86,16 @@
         :param str grav_axes: Same format as ``mag_axes`` but for the accelerometer. Default is copy
           of mag_axes.
         """
         if grav_axes is None:
             grav_axes = mag_axes
         self.mag = Sensor(axes=mag_axes)
         self.grav = Sensor(axes=grav_axes)
+        self.dip_avg: float = None
+        self.dip_std: float = None
         self.ready = False
 
     def calibrate(
         self,
         mag_data: np.ndarray,
         grav_data: np.ndarray,
         routine: int = FAST_NON_LINEAR,
@@ -84,15 +110,15 @@
         :param np.ndarray grav_data: Numpy array of gravity readings of shape (M,3)
         :param routine: what level of calibration to perform:
 
           * `ELLIPSOID`: Simplest form of calibration, very fast, does not require any sets of
             readings to be aligned. Does not correct for misalignment between pointer and sensors.
           * `AXIS_CORRECTION`: This routine performs the `ELLIPSOID` and then applies a
             rotation to offset any misalignment between the pointer and sensors (and also
-            misalignment between accelrometer and magnetometer if relevant). This process will
+            misalignment between accelerometer and magnetometer if relevant). This process will
             automatically identify which shots have been taken in the same direction
           * `NON_LINEAR`: Performs calibration as per `AXIS_CORRECTION`, then uses an
             optimisation process to account for non-linear sensor response. See `fit_non_linear`
             for details.
           * `FAST_NON_LINEAR`: Performs calibration as per `AXIS_CORRECTION`, then uses a
             least-squares process to account for non-linear sensor response. A lot faster than
             `NON_LINEAR`, but slightly less accurate. See `fit_non_linear_quick` for details
@@ -108,16 +134,18 @@
                 raise ValueError("No runs of shots all in the same direction found")
             paired_data = [(mag_data[a:b], grav_data[a:b]) for a, b in runs]
             self.fit_to_axis(paired_data)
             if routine == self.NON_LINEAR:
                 self.fit_non_linear(paired_data)
             elif routine == self.FAST_NON_LINEAR:
                 self.fit_non_linear_quick(paired_data)
+            self.set_field_characteristics(mag_data, grav_data)
             return self.accuracy(paired_data)
         # just ellipsod fit done, so use uniformity measure
+        self.set_field_characteristics(mag_data, grav_data)
         return np.mean(self.uniformity(mag_data, grav_data))
 
     def get_angles(self, mag, grav) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
         """
         Get device azimuth(bearing), inclination, and roll, given the magnetic and gravity readings
 
         :param np.ndarray mag: Magnetic readings, either as numpy array or sequence of 3 floats
@@ -542,7 +570,91 @@
             return False
         if max(azimuths) > 360 - precision:
             # rotate by 180 degs if shots near 359/0 degs
             azimuths = [(azimuth + 180) % 360 for azimuth in azimuths]
         if max(azimuths) - min(azimuths) > precision:
             return False
         return True
+
+    def get_field_strengths(self, mag, grav):
+        """
+        Get field strength for magnetic and gravity components
+
+        :param numpy.ndarray mag: Magnetic readings, either as numpy array or sequence of 3
+          floats
+        :param numpy.ndarray grav: Gravity readings, either as numpy array or sequence of 3
+          floats
+        :return: mag_field, grav_field
+        :rtype: numpy.ndarrays if multiple readings given or floats
+        """
+        return self.mag.get_field_strength(mag), self.grav.get_field_strength(grav)
+
+    def get_dips(self, mag, grav):
+        """
+        Get the magnetic field dip
+        :param numpy.ndarray mag: Magnetic readings, either as numpy array or sequence of 3
+          floats
+        :param numpy.ndarray grav: Gravity readings, either as numpy array or sequence of 3
+          floats
+        :return: dip angle(s) in degrees
+        :rtype: numpy.ndarrays if multiple readings given or floats
+        """
+        normalised_mags = normalise(self.mag.apply(mag))
+        normalised_gravs = normalise(self.grav.apply(grav))
+        if len(normalised_gravs.shape) > 1:
+            dot_products = [
+                np.dot(m, g) for m, g in zip(normalised_mags, normalised_gravs)
+            ]
+            dot_products = np.array(dot_products)
+        else:
+            dot_products = np.dot(normalised_mags, normalised_gravs)
+        dips = 90 - np.degrees(np.arccos(dot_products))
+        return dips
+
+    def set_expected_mean_dip_and_std(self, mag, grav):
+        """
+        Store an expected dip and standard deviations. This will be used for
+        magnetic and (gravitational!!) anomaly detection
+
+        :param numpy.ndarray mag: Magnetic readings, either as numpy array or sequence of 3
+          floats
+        :param numpy.ndarray grav: Gravity readings, either as numpy array or sequence of 3
+          floats
+        """
+        dips = self.get_dips(mag, grav)
+        self.dip_avg = np.mean(dips)
+        self.dip_std = np.std(dips)
+
+    def set_field_characteristics(self, mag, grav):
+        """
+        Store magnetic and gravity field strengths and also dip angles. This will be used for
+        magnetic and (gravitational!!) anomaly detection
+        :param numpy.ndarray mag: Magnetic readings, either as numpy array or sequence of 3
+          floats
+        :param numpy.ndarray grav: Gravity readings, either as numpy array or sequence of 3
+          floats
+        :return:
+        """
+        self.mag.set_expected_field_strengths(mag)
+        self.grav.set_expected_field_strengths(grav)
+        self.set_expected_mean_dip_and_std(mag, grav)
+
+    def raise_if_anomaly(self, mag, grav, sigma=DEFAULT_SIGMA):
+        """
+
+        :param numpy.ndarray mag: Magnetic readings, sequence of 3 floats
+        :param numpy.ndarray grav: Gravity readings, sequence of 3 floats
+        :param sigma: number of standard deviations to accept, default is 3
+        :return: None
+        :raises:
+          * `MagneticAnomalyError` if magnetic field strength too big or small
+          * `GravityAnomalyError` if gravity field strength too big or small - this should be rare
+          * `DipAnomalyError` if magnetic field dip too big or small
+        """
+        if self.mag.reading_is_anomalous(mag):
+            raise MagneticAnomalyError("Magnetic field strength out of limits")
+        if self.grav.reading_is_anomalous(grav):
+            raise GravityAnomalyError("Gravity field strength out of limits")
+        dip = self.get_dips(mag, grav)
+        variation = abs(self.dip_avg - dip)
+        if variation > sigma * self.dip_std:
+            raise DipAnomalyError("Magnetic dip out of limits")
```

### Comparing `circuitpython-mag-cal-1.1.4/mag_cal/lstsq.py` & `circuitpython-mag-cal-1.2.0/mag_cal/lstsq.py`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.4/mag_cal/nm.py` & `circuitpython-mag-cal-1.2.0/mag_cal/nm.py`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.4/mag_cal/rbf.py` & `circuitpython-mag-cal-1.2.0/mag_cal/rbf.py`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.4/mag_cal/sensor.py` & `circuitpython-mag-cal-1.2.0/mag_cal/sensor.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 except ImportError:
     from ulab import numpy as np
 
 from .axes import Axes
 from .utils import solve_least_squares, normalise, NotCalibrated, cross
 from .rbf import RBF
 
+DEFAULT_SIGMA = 3
+
 
 class Sensor:
     """
     This represents the calibration coefficients for a single sensor
     """
 
     def __init__(self, axes="+X+Y+Z"):
@@ -35,14 +37,16 @@
           points to the left of the device, the X is forwards and Z is down, specify this as
           ``"-Y+X+Z"``. Default is ``+X+Y+Z``
         """
         self.axes = Axes(axes)
         self.transform: np.ndarray = None
         self.centre: np.ndarray = None
         self.rbfs: List[RBF] = []
+        self.field_avg: float = None
+        self.field_std: float = None
 
     def fit_ellipsoid(self, data: np.ndarray) -> float:
         # pylint: disable=too-many-locals, invalid-name
         """
         Take multiple sets of readings in various directions. You can then use this function
         to determine an ideal set of calibration coefficients.
 
@@ -208,14 +212,16 @@
         :return: Dict containing all the calibration data for this sensor
         """
         results = {
             "axes": str(self.axes),
             "transform": self.transform.tolist(),
             "centre": self.centre.tolist(),
             "rbfs": [x.as_list() for x in self.rbfs],
+            "field_avg": self.field_avg,
+            "field_std": self.field_std,
         }
         return results
 
     @classmethod
     def from_dict(cls, dct: dict) -> "Sensor":
         """
         Create a new `Sensor` instance from the given dict, which should have been created
@@ -224,8 +230,44 @@
         :param dict dct: Dict of values as created by `as_dict`
         :return: New Sensor object, initialised with given data
         """
         instance = cls(dct["axes"])
         instance.transform = np.array(dct["transform"])
         instance.centre = np.array(dct["centre"])
         instance.rbfs = [RBF(x) for x in dct["rbfs"]]
+        instance.field_avg = dct["field_avg"]
+        instance.field_std = dct["field_std"]
         return instance
+
+    def get_field_strength(self, data):
+        """
+        Get the field strength from this sensor, using the original units that
+        the data was provided in.
+        :param numpy.ndarray data: Sensor readings, either as numpy array or sequence of 3 floats
+        :return: Single float or numpy array of field strengths
+        """
+        corrected_data = self.apply(data)
+        # convert back to original units using scale elements from transform
+        scaled_data = corrected_data / np.mean(np.diag(self.transform))
+        strengths = np.linalg.norm(scaled_data, axis=-1)
+        return strengths
+
+    def set_expected_field_strengths(self, data):
+        """
+        Store an expected field strength and standard deviations. This will be used for
+        magnetic and (gravitational!!) anomaly detection
+        :param numpy.ndarray data: Sensor readings, either as numpy array or sequence of 3 floats
+        """
+        strengths = self.get_field_strength(data)
+        self.field_avg = np.mean(strengths)
+        self.field_std = np.std(strengths)
+
+    def reading_is_anomalous(self, data, sigma=DEFAULT_SIGMA):
+        """
+        Returns True if given reading is not within expected range
+        :param data: sequence of 3 floats
+        :param sigma: NUmber of standard deviations that must be exceeded
+        :return: True if field strenght is greater than sigma standard deviations from the mean
+        """
+        strength = self.get_field_strength(data)
+        variation = abs(self.field_avg - strength)
+        return variation > sigma * self.field_std
```

### Comparing `circuitpython-mag-cal-1.1.4/mag_cal/utils.py` & `circuitpython-mag-cal-1.2.0/mag_cal/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -71,24 +71,41 @@
     grav = grav.reshape((grav.shape[0] // 3, 3))
     mag_aligned = [mag[8:16], mag[16:24]]
     grav_aligned = [grav[8:16], grav[16:24]]
     aligned_data = list(zip(mag_aligned, grav_aligned))
     return aligned_data, grav, mag
 
 
+def _cross(a: np.ndarray, b: np.ndarray) -> np.ndarray:
+    # pylint: disable=invalid-name
+    """
+    implement cross product ourselves as ulabs implementation is broken
+    :param a:
+    :param b:
+    :return:
+    """
+    return np.array(
+        [
+            a[1] * b[2] - a[2] * b[1],
+            a[2] * b[0] - a[0] * b[2],
+            a[0] * b[1] - a[1] * b[0],
+        ]
+    )
+
+
 def cross(a: np.ndarray, b: np.ndarray):
     # pylint: disable=invalid-name
     """
     Return a x b where x is the cross-product operator
     :param np.ndarray a: Numpy array of shape (3,) or (N,3)
     :param np.ndarray b: Numpy array of shape (3,) or (N,3)
     :return: a x b
     """
     len_a = len(a.shape)
     len_b = len(b.shape)
     if len_a == 1 and len_b == 1:
-        return np.cross(a, b)
+        return _cross(a, b)
     if len_a == 1:
-        return np.array([np.cross(a, x) for x in b])
+        return np.array([_cross(a, x) for x in b])
     if len_b == 1:
-        return np.array([np.cross(x, b) for x in a])
-    return np.array([np.cross(x, y) for x, y in zip(a, b)])
+        return np.array([_cross(x, b) for x in a])
+    return np.array([_cross(x, y) for x, y in zip(a, b)])
```

### Comparing `circuitpython-mag-cal-1.1.4/pyproject.toml` & `circuitpython-mag-cal-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "circuitpython-mag-cal"
 description = "Calibrate magnetometer and accelerometer readings"
-version = "1.1.4"
+version = "1.2.0"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/furbrain/CircuitPython_mag_cal"}
 keywords = [
     "adafruit",
```

### Comparing `circuitpython-mag-cal-1.1.4/tests/fixtures/cal_data/ab.json` & `circuitpython-mag-cal-1.2.0/tests/fixtures/cal_data/ab.json`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.4/tests/fixtures/cal_data/ai.json` & `circuitpython-mag-cal-1.2.0/tests/fixtures/cal_data/ai.json`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.4/tests/fixtures/cal_data/bh.json` & `circuitpython-mag-cal-1.2.0/tests/fixtures/cal_data/bh.json`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.4/tests/fixtures/cal_data/bi.json` & `circuitpython-mag-cal-1.2.0/tests/fixtures/cal_data/bi.json`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.4/tests/fixtures/cal_data/ee.json` & `circuitpython-mag-cal-1.2.0/tests/fixtures/cal_data/ee.json`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.4/tests/fixtures/cal_data/fb.json` & `circuitpython-mag-cal-1.2.0/tests/fixtures/cal_data/fb.json`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.4/tests/fixtures/cal_data/hj.json` & `circuitpython-mag-cal-1.2.0/tests/fixtures/cal_data/hj.json`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.4/tests/fixtures/cal_data/hj2.json` & `circuitpython-mag-cal-1.2.0/tests/fixtures/cal_data/hj2.json`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.4/tests/fixtures/cal_data/jd.json` & `circuitpython-mag-cal-1.2.0/tests/fixtures/cal_data/jd.json`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.4/tests/test_axes.py` & `circuitpython-mag-cal-1.2.0/tests/test_axes.py`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.1.4/tests/test_calibration.py` & `circuitpython-mag-cal-1.2.0/tests/test_calibration.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import unittest
 from pathlib import Path
 from unittest import TestCase
 from unittest.mock import patch
 
 import numpy as np
 
-from mag_cal.calibration import Calibration
+from mag_cal.calibration import Calibration, CalibrationError
 from mag_cal.utils import read_fixture
 
 
 class TestCalibration(TestCase):
     def setUp(self) -> None:
         np.set_printoptions(precision=4, suppress=True)
         self.fixtures = {}
@@ -126,14 +126,29 @@
 
     def test_integration_calibrate(self):
         for mag, grav, _ in self.fixtures.values():
             calib = Calibration()
             accuracy = calib.calibrate(mag, grav)
             self.assertGreater(0.5, accuracy)
 
+    def test_calibration_readings_not_anomalous(self):
+        # pylint: disable=invalid-name
+        for mag, grav, _ in self.fixtures.values():
+            calib = Calibration()
+            for m, g in zip(mag, grav):
+                calib.raise_if_anomaly(m, g)
+
+    def test_calibration_readings_anomalous_with_low_sigma(self):
+        # pylint: disable=invalid-name
+        for mag, grav, _ in self.fixtures.values():
+            calib = Calibration()
+            with self.assertRaises(CalibrationError):
+                for m, g in zip(mag, grav):
+                    calib.raise_if_anomaly(m, g, sigma=1)
+
     @unittest.skip
     def test_display_non_linear_maps(self):
         # pylint: disable=invalid-name,import-outside-toplevel,cell-var-from-loop
         import matplotlib.pyplot as plt
 
         mag, grav, aligned_data = list(self.fixtures.values())[3]
         calib = Calibration()
```

### Comparing `circuitpython-mag-cal-1.1.4/tests/test_sensor.py` & `circuitpython-mag-cal-1.2.0/tests/test_sensor.py`

 * *Files identical despite different names*

