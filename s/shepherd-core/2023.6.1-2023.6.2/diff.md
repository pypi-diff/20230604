# Comparing `tmp/shepherd_core-2023.6.1.tar.gz` & `tmp/shepherd_core-2023.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shepherd_core-2023.6.1.tar", last modified: Thu Jun  1 14:32:19 2023, max compression
+gzip compressed data, was "shepherd_core-2023.6.2.tar", last modified: Sun Jun  4 18:49:27 2023, max compression
```

## Comparing `shepherd_core-2023.6.1.tar` & `shepherd_core-2023.6.2.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:32:19.863205 shepherd_core-2023.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-06-01 14:32:19.863205 shepherd_core-2023.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-06-01 14:32:19.863205 shepherd_core-2023.6.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:32:19.851205 shepherd_core-2023.6.1/shepherd_core/
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/calibration_hw_def.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/commons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:32:19.851205 shepherd_core-2023.6.1/shepherd_core/data_models/
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:32:19.851205 shepherd_core-2023.6.1/shepherd_core/data_models/base/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/base/cal_measurement.py
--rw-r--r--   0 runner    (1001) docker     (123)     7946 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/base/calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/base/content.py
--rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/base/fixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/base/shepherd.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/base/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:32:19.855205 shepherd_core-2023.6.1/shepherd_core/data_models/content/
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/content/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/content/energy_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/content/energy_environment_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/content/firmware.py
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/content/firmware_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8861 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/content/virtual_harvester.py
--rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/content/virtual_harvester_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13641 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/content/virtual_source.py
--rw-r--r--   0 runner    (1001) docker     (123)    10404 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/content/virtual_source_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6807 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/doc_virtual_source.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:32:19.855205 shepherd_core-2023.6.1/shepherd_core/data_models/experiment/
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/experiment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/experiment/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/experiment/observer_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/experiment/target_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:32:19.855205 shepherd_core-2023.6.1/shepherd_core/data_models/task/
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/task/emulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/task/firmware_mod.py
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/task/harvest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/task/observer_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/task/programming.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/task/testbed_tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:32:19.855205 shepherd_core-2023.6.1/shepherd_core/data_models/testbed/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/testbed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/testbed/cape.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/testbed/cape_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/testbed/gpio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/testbed/gpio_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/testbed/mcu.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/testbed/mcu_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/testbed/observer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/testbed/observer_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/testbed/target.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/testbed/target_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/testbed/testbed.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/data_models/testbed/testbed_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    20835 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:32:19.859205 shepherd_core-2023.6.1/shepherd_core/vsource/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/vsource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10497 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/vsource/virtual_converter_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/vsource/virtual_harvester_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/vsource/virtual_source_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    13204 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/shepherd_core/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:32:19.863205 shepherd_core-2023.6.1/shepherd_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-06-01 14:32:19.000000 shepherd_core-2023.6.1/shepherd_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-06-01 14:32:19.000000 shepherd_core-2023.6.1/shepherd_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:32:19.000000 shepherd_core-2023.6.1/shepherd_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-01 14:32:19.000000 shepherd_core-2023.6.1/shepherd_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-01 14:32:19.000000 shepherd_core-2023.6.1/shepherd_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:32:19.000000 shepherd_core-2023.6.1/shepherd_core.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:32:19.859205 shepherd_core-2023.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:32:19.863205 shepherd_core-2023.6.1/tests/data_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/tests/data_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/tests/data_models/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/tests/data_models/example_cal_data.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/tests/data_models/example_cal_data_faulty.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5405 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/tests/data_models/example_cal_meas.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/tests/data_models/example_cal_meas_faulty1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/tests/data_models/example_cal_meas_faulty2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/tests/data_models/example_config_emulator.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/tests/data_models/example_config_experiment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/tests/data_models/example_config_experiment_alternative.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/tests/data_models/example_config_harvester.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/tests/data_models/example_config_testbed.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/tests/data_models/example_config_virtsource.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6207 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/tests/data_models/test_base_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/tests/data_models/test_content_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/tests/data_models/test_content_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/tests/data_models/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     9324 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/tests/data_models/test_experiment_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/tests/data_models/test_task_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/tests/data_models/test_task_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/tests/data_models/test_testbed_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/tests/data_models/test_testbed_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/tests/test_cal_hw.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/tests/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     9586 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/tests/test_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:32:19.863205 shepherd_core-2023.6.1/tests/vsource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/tests/vsource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/tests/vsource/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/tests/vsource/test_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-06-01 14:32:07.000000 shepherd_core-2023.6.1/tests/vsource/test_harvester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 18:49:27.115735 shepherd_core-2023.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-06-04 18:49:27.115735 shepherd_core-2023.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-06-04 18:49:27.115735 shepherd_core-2023.6.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 18:49:27.099735 shepherd_core-2023.6.2/shepherd_core/
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/calibration_hw_def.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/commons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 18:49:27.099735 shepherd_core-2023.6.2/shepherd_core/data_models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 18:49:27.099735 shepherd_core-2023.6.2/shepherd_core/data_models/base/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/base/cal_measurement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7946 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/base/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/base/content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/base/fixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/base/shepherd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/base/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 18:49:27.103735 shepherd_core-2023.6.2/shepherd_core/data_models/content/
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/content/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/content/energy_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/content/energy_environment_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/content/firmware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/content/firmware_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8861 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/content/virtual_harvester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/content/virtual_harvester_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13641 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/content/virtual_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10404 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/content/virtual_source_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6807 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/doc_virtual_source.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 18:49:27.103735 shepherd_core-2023.6.2/shepherd_core/data_models/experiment/
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/experiment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/experiment/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/experiment/observer_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/experiment/target_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 18:49:27.103735 shepherd_core-2023.6.2/shepherd_core/data_models/task/
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/task/emulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/task/firmware_mod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/task/harvest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/task/observer_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/task/programming.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/task/testbed_tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 18:49:27.107735 shepherd_core-2023.6.2/shepherd_core/data_models/testbed/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/testbed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/testbed/cape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/testbed/cape_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/testbed/gpio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/testbed/gpio_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/testbed/mcu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/testbed/mcu_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/testbed/observer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/testbed/observer_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/testbed/target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/testbed/target_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/testbed/testbed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/data_models/testbed/testbed_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20835 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 18:49:27.107735 shepherd_core-2023.6.2/shepherd_core/vsource/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/vsource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10497 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/vsource/virtual_converter_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/vsource/virtual_harvester_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/vsource/virtual_source_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13524 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/shepherd_core/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 18:49:27.115735 shepherd_core-2023.6.2/shepherd_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-06-04 18:49:27.000000 shepherd_core-2023.6.2/shepherd_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-06-04 18:49:27.000000 shepherd_core-2023.6.2/shepherd_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 18:49:27.000000 shepherd_core-2023.6.2/shepherd_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-04 18:49:27.000000 shepherd_core-2023.6.2/shepherd_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-04 18:49:27.000000 shepherd_core-2023.6.2/shepherd_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 18:49:26.000000 shepherd_core-2023.6.2/shepherd_core.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 18:49:27.107735 shepherd_core-2023.6.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 18:49:27.111735 shepherd_core-2023.6.2/tests/data_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/tests/data_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/tests/data_models/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/tests/data_models/example_cal_data.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/tests/data_models/example_cal_data_faulty.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5405 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/tests/data_models/example_cal_meas.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/tests/data_models/example_cal_meas_faulty1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/tests/data_models/example_cal_meas_faulty2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/tests/data_models/example_config_emulator.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/tests/data_models/example_config_experiment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/tests/data_models/example_config_experiment_alternative.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/tests/data_models/example_config_harvester.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/tests/data_models/example_config_testbed.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/tests/data_models/example_config_virtsource.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6207 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/tests/data_models/test_base_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/tests/data_models/test_content_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/tests/data_models/test_content_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/tests/data_models/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9324 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/tests/data_models/test_experiment_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/tests/data_models/test_task_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/tests/data_models/test_task_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/tests/data_models/test_testbed_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/tests/data_models/test_testbed_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/tests/test_cal_hw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9586 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/tests/test_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 18:49:27.111735 shepherd_core-2023.6.2/tests/vsource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/tests/vsource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/tests/vsource/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/tests/vsource/test_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-06-04 18:49:14.000000 shepherd_core-2023.6.2/tests/vsource/test_harvester.py
```

### Comparing `shepherd_core-2023.6.1/PKG-INFO` & `shepherd_core-2023.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shepherd_core
-Version: 2023.6.1
+Version: 2023.6.2
 Summary: Programming- and CLI-Interface for the h5-dataformat of the Shepherd-Testbed
 Home-page: https://pypi.org/project/shepherd-core/
 Author: Ingmar Splitt, Kai Geissdoerfer
 Author-email: ingmar.splitt@tu-dresden.de
 Maintainer-email: ingmar.splitt@tu-dresden.de
 License: MIT
 Project-URL: Tracker, https://github.com/orgua/shepherd-datalib/issues
```

### Comparing `shepherd_core-2023.6.1/README.md` & `shepherd_core-2023.6.2/README.md`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.1/setup.cfg` & `shepherd_core-2023.6.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.1/shepherd_core/__init__.py` & `shepherd_core-2023.6.2/shepherd_core/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from .data_models.task import Compression
 from .logger import get_verbose_level
 from .logger import logger
 from .logger import set_verbose_level
 from .reader import BaseReader
 from .writer import BaseWriter
 
-__version__ = "2023.6.1"
+__version__ = "2023.6.2"
 
 __all__ = [
     "BaseReader",
     "BaseWriter",
     "get_verbose_level",
     "set_verbose_level",
     "logger",
```

### Comparing `shepherd_core-2023.6.1/shepherd_core/calibration_hw_def.py` & `shepherd_core-2023.6.2/shepherd_core/calibration_hw_def.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.1/shepherd_core/data_models/__init__.py` & `shepherd_core-2023.6.2/shepherd_core/data_models/__init__.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.1/shepherd_core/data_models/base/cal_measurement.py` & `shepherd_core-2023.6.2/shepherd_core/data_models/base/cal_measurement.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.1/shepherd_core/data_models/base/calibration.py` & `shepherd_core-2023.6.2/shepherd_core/data_models/base/calibration.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.1/shepherd_core/data_models/base/content.py` & `shepherd_core-2023.6.2/shepherd_core/data_models/base/content.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.1/shepherd_core/data_models/base/fixture.py` & `shepherd_core-2023.6.2/shepherd_core/data_models/base/fixture.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.1/shepherd_core/data_models/base/shepherd.py` & `shepherd_core-2023.6.2/shepherd_core/data_models/base/shepherd.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import hashlib
 import pathlib
 from datetime import datetime
+from datetime import timedelta
 from pathlib import Path
 from typing import Optional
 from typing import Union
 
 import yaml
 from pydantic import BaseModel
 from pydantic import Extra
@@ -15,14 +16,15 @@
 def repr_str(dumper, data):
     return dumper.represent_scalar("tag:yaml.org,2002:str", str(data))
 
 
 yaml.add_representer(pathlib.PosixPath, repr_str)
 yaml.add_representer(pathlib.WindowsPath, repr_str)
 yaml.add_representer(pathlib.Path, repr_str)
+yaml.add_representer(timedelta, repr_str)
 
 
 class ShpModel(BaseModel):
     """Pre-configured Pydantic Base-Model (specifically for shepherd)
 
     Inheritable Features:
     - constant / frozen, hashable .get_hash()
@@ -82,14 +84,15 @@
             comment=comment,
             created=datetime.now(),
             parameters=model_dict,
         )
         model_yaml = yaml.dump(
             model_wrap.dict(), default_flow_style=False, sort_keys=False
         )
+        # TODO: handle directory
         model_path = Path(path).with_suffix(".yaml")
         with open(model_path, "w") as f:
             f.write(model_yaml)
         return model_path
         # TODO: it would be useful to store a minimal set
         #    - current dict cleaned from default values
         #    - better: the init-args (probably name or id)
```

### Comparing `shepherd_core-2023.6.1/shepherd_core/data_models/content/energy_environment.py` & `shepherd_core-2023.6.2/shepherd_core/data_models/content/energy_environment.py`

 * *Files 16% similar despite different names*

```diff
@@ -27,12 +27,14 @@
     data_path: Path
     data_type: EnergyDType
 
     duration: PositiveFloat
     energy_Ws: PositiveFloat
     valid: bool = False
 
+    # TODO: scale up/down voltage/current
+
     @root_validator(pre=True)
     def query_database(cls, values: dict) -> dict:
         values = fixtures.lookup(values)
         values, _ = fixtures.inheritance(values)
         return values
```

### Comparing `shepherd_core-2023.6.1/shepherd_core/data_models/content/energy_environment_fixture.yaml` & `shepherd_core-2023.6.2/shepherd_core/data_models/content/energy_environment_fixture.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.1/shepherd_core/data_models/content/firmware.py` & `shepherd_core-2023.6.2/shepherd_core/data_models/content/firmware.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.1/shepherd_core/data_models/content/firmware_fixture.yaml` & `shepherd_core-2023.6.2/shepherd_core/data_models/content/firmware_fixture.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.1/shepherd_core/data_models/content/virtual_harvester.py` & `shepherd_core-2023.6.2/shepherd_core/data_models/content/virtual_harvester.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.1/shepherd_core/data_models/content/virtual_harvester_fixture.yaml` & `shepherd_core-2023.6.2/shepherd_core/data_models/content/virtual_harvester_fixture.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.1/shepherd_core/data_models/content/virtual_source.py` & `shepherd_core-2023.6.2/shepherd_core/data_models/content/virtual_source.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.1/shepherd_core/data_models/content/virtual_source_fixture.yaml` & `shepherd_core-2023.6.2/shepherd_core/data_models/content/virtual_source_fixture.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.1/shepherd_core/data_models/doc_virtual_source.py` & `shepherd_core-2023.6.2/shepherd_core/data_models/doc_virtual_source.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.1/shepherd_core/data_models/experiment/__init__.py` & `shepherd_core-2023.6.2/shepherd_core/data_models/experiment/__init__.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.1/shepherd_core/data_models/experiment/experiment.py` & `shepherd_core-2023.6.2/shepherd_core/data_models/experiment/experiment.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.1/shepherd_core/data_models/experiment/observer_features.py` & `shepherd_core-2023.6.2/shepherd_core/data_models/experiment/observer_features.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.1/shepherd_core/data_models/experiment/target_config.py` & `shepherd_core-2023.6.2/shepherd_core/data_models/experiment/target_config.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.1/shepherd_core/data_models/task/emulation.py` & `shepherd_core-2023.6.2/shepherd_core/data_models/task/emulation.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.1/shepherd_core/data_models/task/firmware_mod.py` & `shepherd_core-2023.6.2/shepherd_core/data_models/task/firmware_mod.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.1/shepherd_core/data_models/task/harvest.py` & `shepherd_core-2023.6.2/shepherd_core/data_models/task/harvest.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     use_cal_default: bool = False
     # ⤷ Use default calibration values, skip loading from EEPROM
 
     virtual_harvester: VirtualHarvesterConfig = VirtualHarvesterConfig(name="mppt_opt")
     # ⤷ Choose one of the predefined virtual harvesters
     #   or configure a new one
 
-    power_tracing: Optional[PowerTracing] = PowerTracing()
+    power_tracing: PowerTracing = PowerTracing()
     sys_logging: Optional[SystemLogging] = SystemLogging()
 
     # TODO: there is an unused DAC-Output patched to the harvesting-port
 
     @root_validator(pre=False)
     def post_validation(cls, values: dict) -> dict:
         # TODO: limit paths
```

### Comparing `shepherd_core-2023.6.1/shepherd_core/data_models/task/observer_tasks.py` & `shepherd_core-2023.6.2/shepherd_core/data_models/task/observer_tasks.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.1/shepherd_core/data_models/task/programming.py` & `shepherd_core-2023.6.2/shepherd_core/data_models/task/programming.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.1/shepherd_core/data_models/task/testbed_tasks.py` & `shepherd_core-2023.6.2/shepherd_core/data_models/task/testbed_tasks.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.1/shepherd_core/data_models/testbed/__init__.py` & `shepherd_core-2023.6.2/shepherd_core/data_models/testbed/__init__.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.1/shepherd_core/data_models/testbed/cape.py` & `shepherd_core-2023.6.2/shepherd_core/data_models/testbed/cape.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.1/shepherd_core/data_models/testbed/cape_fixture.yaml` & `shepherd_core-2023.6.2/shepherd_core/data_models/testbed/cape_fixture.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.1/shepherd_core/data_models/testbed/gpio.py` & `shepherd_core-2023.6.2/shepherd_core/data_models/testbed/gpio.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.1/shepherd_core/data_models/testbed/gpio_fixture.yaml` & `shepherd_core-2023.6.2/shepherd_core/data_models/testbed/gpio_fixture.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.1/shepherd_core/data_models/testbed/mcu.py` & `shepherd_core-2023.6.2/shepherd_core/data_models/testbed/mcu.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,16 +15,19 @@
 fixture_path = Path(__file__).resolve().with_name("mcu_fixture.yaml")
 fixtures = Fixtures(fixture_path, "mcu")
 
 
 class ProgrammerProtocol(str, Enum):
     SWD = "SWD"
     swd = "SWD"
+    SBW = "SBW"
     sbw = "SBW"
+    JTAG = "JTAG"
     jtag = "JTAG"
+    UART = "UART"
     uart = "UART"
 
 
 class MCU(ShpModel, title="Microcontroller of the Target Node"):
     """meta-data representation of a testbed-component (physical object)"""
 
     id: IdInt  # noqa: A003
```

### Comparing `shepherd_core-2023.6.1/shepherd_core/data_models/testbed/mcu_fixture.yaml` & `shepherd_core-2023.6.2/shepherd_core/data_models/testbed/mcu_fixture.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.1/shepherd_core/data_models/testbed/observer.py` & `shepherd_core-2023.6.2/shepherd_core/data_models/testbed/observer.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.1/shepherd_core/data_models/testbed/observer_fixture.yaml` & `shepherd_core-2023.6.2/shepherd_core/data_models/testbed/observer_fixture.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.1/shepherd_core/data_models/testbed/target.py` & `shepherd_core-2023.6.2/shepherd_core/data_models/testbed/target.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.1/shepherd_core/data_models/testbed/target_fixture.yaml` & `shepherd_core-2023.6.2/shepherd_core/data_models/testbed/target_fixture.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.1/shepherd_core/data_models/testbed/testbed.py` & `shepherd_core-2023.6.2/shepherd_core/data_models/testbed/testbed.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.1/shepherd_core/logger.py` & `shepherd_core-2023.6.2/shepherd_core/logger.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,50 +1,51 @@
 import logging
 
 import chromalog
-from pydantic import validate_arguments
 
 chromalog.basicConfig(format="%(message)s")
 logger = logging.getLogger("SHPCore")
 logger.addHandler(logging.NullHandler())
 
 verbose_level: int = 2
 
 
 def get_verbose_level() -> int:
     return verbose_level
 
 
-@validate_arguments
-def set_verbose_level(verbose: int) -> None:
-    global verbose_level
-    verbose_level = min(max(verbose, 0), 3)
-
-    if verbose_level == 0:
-        logger.setLevel(logging.ERROR)
+def set_log_verbose_level(log_: logging.Logger, verbose: int) -> None:
+    if verbose == 0:
+        log_.setLevel(logging.ERROR)
         logging.basicConfig(level=logging.ERROR)
-    elif verbose_level == 1:
-        logger.setLevel(logging.WARNING)
-    elif verbose_level == 2:
-        logger.setLevel(logging.INFO)
-    elif verbose_level > 2:
-        logger.setLevel(logging.DEBUG)
+    elif verbose == 1:
+        log_.setLevel(logging.WARNING)
+    elif verbose == 2:
+        log_.setLevel(logging.INFO)
+    elif verbose > 2:
+        log_.setLevel(logging.DEBUG)
 
-    if verbose_level < 3:
+    if verbose < 3:
         # reduce log-overhead when not debugging, also more user-friendly exceptions
         logging._srcfile = None
         logging.logThreads = 0
         logging.logProcesses = 0
 
-    if verbose_level > 2:
+    if verbose > 2:
         chromalog.basicConfig(format="%(name)s %(levelname)s: %(message)s")
     else:
         chromalog.basicConfig(format="%(message)s")  # reduce internals
 
 
+def set_verbose_level(verbose: int) -> None:
+    global verbose_level
+    verbose_level = min(max(verbose, 0), 3)
+    set_log_verbose_level(logger, verbose_level)
+
+
 set_verbose_level(2)
 
 # short reminder for format-strings:
 # %s    string
 # %d    decimal
 # %f    float
 # %o    decimal as octal
```

### Comparing `shepherd_core-2023.6.1/shepherd_core/reader.py` & `shepherd_core-2023.6.2/shepherd_core/reader.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.1/shepherd_core/vsource/virtual_converter_model.py` & `shepherd_core-2023.6.2/shepherd_core/vsource/virtual_converter_model.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.1/shepherd_core/vsource/virtual_harvester_model.py` & `shepherd_core-2023.6.2/shepherd_core/vsource/virtual_harvester_model.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.1/shepherd_core/vsource/virtual_source_model.py` & `shepherd_core-2023.6.2/shepherd_core/vsource/virtual_source_model.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.1/shepherd_core/writer.py` & `shepherd_core-2023.6.2/shepherd_core/writer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Writer that inherits from Reader-Baseclass
 """
 import logging
 import math
+import pathlib
 from itertools import product
 from pathlib import Path
 from typing import Any
 from typing import Optional
 from typing import Union
 
 import h5py
@@ -20,14 +21,24 @@
 from .data_models.base.calibration import CalibrationSeries as CalSeries
 from .data_models.content.energy_environment import EnergyDType
 from .data_models.task import Compression
 from .data_models.task.emulation import c_translate
 from .reader import BaseReader
 
 
+# copy of core/models/base/shepherd - needed also here
+def repr_str(dumper, data):
+    return dumper.represent_scalar("tag:yaml.org,2002:str", str(data))
+
+
+yaml.add_representer(pathlib.PosixPath, repr_str)
+yaml.add_representer(pathlib.WindowsPath, repr_str)
+yaml.add_representer(pathlib.Path, repr_str)
+
+
 def unique_path(base_path: Union[str, Path], suffix: str) -> Path:
     """finds an unused filename in case it already exists
 
     :param base_path: file-path to test
     :param suffix: file-suffix
     :return: new non-existing path
     """
```

### Comparing `shepherd_core-2023.6.1/shepherd_core.egg-info/PKG-INFO` & `shepherd_core-2023.6.2/shepherd_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shepherd-core
-Version: 2023.6.1
+Version: 2023.6.2
 Summary: Programming- and CLI-Interface for the h5-dataformat of the Shepherd-Testbed
 Home-page: https://pypi.org/project/shepherd-core/
 Author: Ingmar Splitt, Kai Geissdoerfer
 Author-email: ingmar.splitt@tu-dresden.de
 Maintainer-email: ingmar.splitt@tu-dresden.de
 License: MIT
 Project-URL: Tracker, https://github.com/orgua/shepherd-datalib/issues
```

### Comparing `shepherd_core-2023.6.1/shepherd_core.egg-info/SOURCES.txt` & `shepherd_core-2023.6.2/shepherd_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.1/tests/conftest.py` & `shepherd_core-2023.6.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.1/tests/data_models/example_cal_data.yaml` & `shepherd_core-2023.6.2/tests/data_models/example_cal_data.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.1/tests/data_models/example_cal_data_faulty.yaml` & `shepherd_core-2023.6.2/tests/data_models/example_cal_data_faulty.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.1/tests/data_models/example_cal_meas.yaml` & `shepherd_core-2023.6.2/tests/data_models/example_cal_meas.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.1/tests/data_models/example_cal_meas_faulty1.yaml` & `shepherd_core-2023.6.2/tests/data_models/example_cal_meas_faulty1.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.1/tests/data_models/example_cal_meas_faulty2.yaml` & `shepherd_core-2023.6.2/tests/data_models/example_cal_meas_faulty2.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.1/tests/data_models/example_config_emulator.yaml` & `shepherd_core-2023.6.2/tests/data_models/example_config_emulator.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.1/tests/data_models/example_config_harvester.yaml` & `shepherd_core-2023.6.2/tests/data_models/example_config_harvester.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.1/tests/data_models/example_config_virtsource.yaml` & `shepherd_core-2023.6.2/tests/data_models/example_config_virtsource.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.1/tests/data_models/test_base_models.py` & `shepherd_core-2023.6.2/tests/data_models/test_base_models.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.1/tests/data_models/test_content_fixtures.py` & `shepherd_core-2023.6.2/tests/data_models/test_content_fixtures.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.1/tests/data_models/test_content_models.py` & `shepherd_core-2023.6.2/tests/data_models/test_content_models.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.1/tests/data_models/test_examples.py` & `shepherd_core-2023.6.2/tests/data_models/test_examples.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.1/tests/data_models/test_experiment_models.py` & `shepherd_core-2023.6.2/tests/data_models/test_experiment_models.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.1/tests/data_models/test_task_generation.py` & `shepherd_core-2023.6.2/tests/data_models/test_task_generation.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.1/tests/data_models/test_task_models.py` & `shepherd_core-2023.6.2/tests/data_models/test_task_models.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.1/tests/data_models/test_testbed_fixtures.py` & `shepherd_core-2023.6.2/tests/data_models/test_testbed_fixtures.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.1/tests/data_models/test_testbed_models.py` & `shepherd_core-2023.6.2/tests/data_models/test_testbed_models.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.1/tests/test_cal_hw.py` & `shepherd_core-2023.6.2/tests/test_cal_hw.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.1/tests/test_reader.py` & `shepherd_core-2023.6.2/tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.1/tests/test_writer.py` & `shepherd_core-2023.6.2/tests/test_writer.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.1/tests/vsource/conftest.py` & `shepherd_core-2023.6.2/tests/vsource/conftest.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.1/tests/vsource/test_converter.py` & `shepherd_core-2023.6.2/tests/vsource/test_converter.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.1/tests/vsource/test_harvester.py` & `shepherd_core-2023.6.2/tests/vsource/test_harvester.py`

 * *Files identical despite different names*

