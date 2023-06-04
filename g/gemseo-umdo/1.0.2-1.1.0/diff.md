# Comparing `tmp/gemseo-umdo-1.0.2.tar.gz` & `tmp/gemseo-umdo-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gemseo-umdo-1.0.2.tar", last modified: Thu Feb  9 17:50:16 2023, max compression
+gzip compressed data, was "gemseo-umdo-1.1.0.tar", last modified: Sun Jun  4 18:29:24 2023, max compression
```

## Comparing `gemseo-umdo-1.0.2.tar` & `gemseo-umdo-1.1.0.tar`

### file list

```diff
@@ -1,106 +1,180 @@
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-09 17:50:16.880750 gemseo-umdo-1.0.2/
--rw-r--r--   0 ad        (1000) ad        (1000)      450 2022-07-01 08:15:59.000000 gemseo-umdo-1.0.2/.gitattributes
--rw-r--r--   0 ad        (1000) ad        (1000)      190 2022-07-25 06:23:25.000000 gemseo-umdo-1.0.2/.gitignore
--rw-r--r--   0 ad        (1000) ad        (1000)       87 2023-02-09 15:49:15.000000 gemseo-umdo-1.0.2/.gitlab-ci.yml
--rw-r--r--   0 ad        (1000) ad        (1000)     2933 2023-02-09 15:09:36.000000 gemseo-umdo-1.0.2/.pre-commit-config.yaml
--rw-r--r--   0 ad        (1000) ad        (1000)     9105 2022-07-01 08:15:59.000000 gemseo-umdo-1.0.2/.pylintrc
--rw-r--r--   0 ad        (1000) ad        (1000)     1605 2023-02-09 15:52:00.000000 gemseo-umdo-1.0.2/CHANGELOG.rst
--rw-r--r--   0 ad        (1000) ad        (1000)     1763 2022-07-25 06:47:03.000000 gemseo-umdo-1.0.2/CREDITS.rst
--rw-r--r--   0 ad        (1000) ad        (1000)     7652 2022-03-24 13:18:51.000000 gemseo-umdo-1.0.2/LICENSE.txt
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-09 17:50:16.868750 gemseo-umdo-1.0.2/LICENSES/
--rw-r--r--   0 ad        (1000) ad        (1000)     7652 2022-03-24 13:18:51.000000 gemseo-umdo-1.0.2/LICENSES/LGPLv3.txt
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-09 17:50:16.869750 gemseo-umdo-1.0.2/LICENSES/headers/
--rw-r--r--   0 ad        (1000) ad        (1000)      729 2022-03-24 13:18:51.000000 gemseo-umdo-1.0.2/LICENSES/headers/BSD-0-Clause.txt
--rw-r--r--   0 ad        (1000) ad        (1000)      334 2022-03-24 13:18:51.000000 gemseo-umdo-1.0.2/LICENSES/headers/CC-BY-SA-4.0.txt
--rw-r--r--   0 ad        (1000) ad        (1000)      710 2022-03-24 13:18:51.000000 gemseo-umdo-1.0.2/LICENSES/headers/LGPL-3.0.txt
--rw-r--r--   0 ad        (1000) ad        (1000)     2482 2023-02-09 17:50:16.880750 gemseo-umdo-1.0.2/PKG-INFO
--rw-r--r--   0 ad        (1000) ad        (1000)     1388 2022-07-27 19:25:53.000000 gemseo-umdo-1.0.2/README.rst
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-09 17:50:16.856750 gemseo-umdo-1.0.2/doc_src/
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-09 17:50:16.856750 gemseo-umdo-1.0.2/doc_src/examples/
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-09 17:50:16.856750 gemseo-umdo-1.0.2/doc_src/examples/udoe/
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-09 17:50:16.869750 gemseo-umdo-1.0.2/doc_src/examples/udoe/quadratic/
--rw-r--r--   0 ad        (1000) ad        (1000)      426 2023-02-09 15:09:36.000000 gemseo-umdo-1.0.2/doc_src/examples/udoe/quadratic/README.rst
--rw-r--r--   0 ad        (1000) ad        (1000)     2452 2023-02-09 15:09:36.000000 gemseo-umdo-1.0.2/doc_src/examples/udoe/quadratic/sampling.py
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-09 17:50:16.869750 gemseo-umdo-1.0.2/doc_src/examples/umdo/
--rw-r--r--   0 ad        (1000) ad        (1000)      402 2023-02-09 15:09:36.000000 gemseo-umdo-1.0.2/doc_src/examples/umdo/README.rst
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-09 17:50:16.870750 gemseo-umdo-1.0.2/doc_src/examples/umdo/quadratic/
--rw-r--r--   0 ad        (1000) ad        (1000)      426 2023-02-09 15:09:36.000000 gemseo-umdo-1.0.2/doc_src/examples/umdo/quadratic/README.rst
--rw-r--r--   0 ad        (1000) ad        (1000)     2441 2023-02-09 15:09:36.000000 gemseo-umdo-1.0.2/doc_src/examples/umdo/quadratic/sampling.py
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-09 17:50:16.870750 gemseo-umdo-1.0.2/doc_src/examples/umdo/rosenbrock/
--rw-r--r--   0 ad        (1000) ad        (1000)      428 2023-02-09 15:09:36.000000 gemseo-umdo-1.0.2/doc_src/examples/umdo/rosenbrock/README.rst
--rw-r--r--   0 ad        (1000) ad        (1000)     2709 2023-02-09 15:09:36.000000 gemseo-umdo-1.0.2/doc_src/examples/umdo/rosenbrock/sampling.py
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-09 17:50:16.871750 gemseo-umdo-1.0.2/doc_src/examples/umdo/sellar/
--rw-r--r--   0 ad        (1000) ad        (1000)      420 2023-02-09 15:09:36.000000 gemseo-umdo-1.0.2/doc_src/examples/umdo/sellar/README.rst
--rw-r--r--   0 ad        (1000) ad        (1000)     2330 2023-02-09 15:09:36.000000 gemseo-umdo-1.0.2/doc_src/examples/umdo/sellar/deterministic.py
--rw-r--r--   0 ad        (1000) ad        (1000)     2809 2023-02-09 15:09:36.000000 gemseo-umdo-1.0.2/doc_src/examples/umdo/sellar/sampling.py
--rw-r--r--   0 ad        (1000) ad        (1000)     3451 2023-02-09 15:09:36.000000 gemseo-umdo-1.0.2/doc_src/examples/umdo/sellar/sampling_with_repetitions.py
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-09 17:50:16.871750 gemseo-umdo-1.0.2/doc_src/examples/umdo/sobieski/
--rw-r--r--   0 ad        (1000) ad        (1000)      424 2023-02-09 15:09:36.000000 gemseo-umdo-1.0.2/doc_src/examples/umdo/sobieski/README.rst
--rw-r--r--   0 ad        (1000) ad        (1000)     3130 2023-02-09 15:09:36.000000 gemseo-umdo-1.0.2/doc_src/examples/umdo/sobieski/sampling.py
--rw-r--r--   0 ad        (1000) ad        (1000)      611 2022-07-19 15:02:00.000000 gemseo-umdo-1.0.2/pyproject.toml
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-09 17:50:16.873750 gemseo-umdo-1.0.2/requirements/
--rw-r--r--   0 ad        (1000) ad        (1000)       79 2022-07-01 08:15:59.000000 gemseo-umdo-1.0.2/requirements/check.in
--rw-r--r--   0 ad        (1000) ad        (1000)      573 2023-02-09 15:09:36.000000 gemseo-umdo-1.0.2/requirements/check.txt
--rw-r--r--   0 ad        (1000) ad        (1000)       12 2022-07-01 08:15:59.000000 gemseo-umdo-1.0.2/requirements/dist.in
--rw-r--r--   0 ad        (1000) ad        (1000)     1453 2023-02-09 15:09:36.000000 gemseo-umdo-1.0.2/requirements/dist.txt
--rw-r--r--   0 ad        (1000) ad        (1000)     2253 2023-02-09 15:09:36.000000 gemseo-umdo-1.0.2/requirements/doc.txt
--rw-r--r--   0 ad        (1000) ad        (1000)     2863 2023-02-09 15:59:28.000000 gemseo-umdo-1.0.2/requirements/test-python3.10.txt
--rw-r--r--   0 ad        (1000) ad        (1000)     3020 2023-02-09 17:13:39.000000 gemseo-umdo-1.0.2/requirements/test-python3.7.txt
--rw-r--r--   0 ad        (1000) ad        (1000)     2861 2023-02-09 15:58:46.000000 gemseo-umdo-1.0.2/requirements/test-python3.8.txt
--rw-r--r--   0 ad        (1000) ad        (1000)     2861 2023-02-09 15:59:07.000000 gemseo-umdo-1.0.2/requirements/test-python3.9.txt
--rw-r--r--   0 ad        (1000) ad        (1000)     1661 2023-02-09 17:50:16.880750 gemseo-umdo-1.0.2/setup.cfg
--rw-r--r--   0 ad        (1000) ad        (1000)      839 2022-07-25 06:47:03.000000 gemseo-umdo-1.0.2/setup.py
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-09 17:50:16.857750 gemseo-umdo-1.0.2/src/
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-09 17:50:16.873750 gemseo-umdo-1.0.2/src/gemseo_umdo/
--rw-r--r--   0 ad        (1000) ad        (1000)      834 2023-02-09 15:09:36.000000 gemseo-umdo-1.0.2/src/gemseo_umdo/__init__.py
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-09 17:50:16.874750 gemseo-umdo-1.0.2/src/gemseo_umdo/estimators/
--rw-r--r--   0 ad        (1000) ad        (1000)      838 2023-02-09 15:09:36.000000 gemseo-umdo-1.0.2/src/gemseo_umdo/estimators/__init__.py
--rw-r--r--   0 ad        (1000) ad        (1000)     2401 2023-02-09 15:09:36.000000 gemseo-umdo-1.0.2/src/gemseo_umdo/estimators/estimator.py
--rw-r--r--   0 ad        (1000) ad        (1000)     3914 2023-02-09 15:09:36.000000 gemseo-umdo-1.0.2/src/gemseo_umdo/estimators/sampling.py
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-09 17:50:16.875750 gemseo-umdo-1.0.2/src/gemseo_umdo/formulations/
--rw-r--r--   0 ad        (1000) ad        (1000)     2236 2023-02-09 15:09:36.000000 gemseo-umdo-1.0.2/src/gemseo_umdo/formulations/__init__.py
--rw-r--r--   0 ad        (1000) ad        (1000)     1285 2023-02-09 15:09:36.000000 gemseo-umdo-1.0.2/src/gemseo_umdo/formulations/factory.py
--rw-r--r--   0 ad        (1000) ad        (1000)    11882 2023-02-09 15:48:34.000000 gemseo-umdo-1.0.2/src/gemseo_umdo/formulations/formulation.py
--rw-r--r--   0 ad        (1000) ad        (1000)     5725 2023-02-09 15:09:36.000000 gemseo-umdo-1.0.2/src/gemseo_umdo/formulations/sampling.py
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-09 17:50:16.876750 gemseo-umdo-1.0.2/src/gemseo_umdo/scenarios/
--rw-r--r--   0 ad        (1000) ad        (1000)      850 2023-02-09 15:09:36.000000 gemseo-umdo-1.0.2/src/gemseo_umdo/scenarios/__init__.py
--rw-r--r--   0 ad        (1000) ad        (1000)     8645 2023-02-09 15:53:37.000000 gemseo-umdo-1.0.2/src/gemseo_umdo/scenarios/_scenario.py
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-09 17:50:16.877750 gemseo-umdo-1.0.2/src/gemseo_umdo/scenarios/udoe/
--rw-r--r--   0 ad        (1000) ad        (1000)      444 2022-07-01 08:15:59.000000 gemseo-umdo-1.0.2/src/gemseo_umdo/scenarios/udoe/UDOEScenario_input.json
--rw-r--r--   0 ad        (1000) ad        (1000)      198 2022-07-01 08:15:59.000000 gemseo-umdo-1.0.2/src/gemseo_umdo/scenarios/udoe/UDOEScenario_output.json
--rw-r--r--   0 ad        (1000) ad        (1000)     1211 2023-02-09 15:48:34.000000 gemseo-umdo-1.0.2/src/gemseo_umdo/scenarios/udoe_scenario.py
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-09 17:50:16.877750 gemseo-umdo-1.0.2/src/gemseo_umdo/scenarios/umdo/
--rw-r--r--   0 ad        (1000) ad        (1000)      399 2022-07-01 08:15:59.000000 gemseo-umdo-1.0.2/src/gemseo_umdo/scenarios/umdo/UMDOScenario_input.json
--rw-r--r--   0 ad        (1000) ad        (1000)      198 2022-07-01 08:15:59.000000 gemseo-umdo-1.0.2/src/gemseo_umdo/scenarios/umdo/UMDOScenario_output.json
--rw-r--r--   0 ad        (1000) ad        (1000)     1222 2023-02-09 15:48:34.000000 gemseo-umdo-1.0.2/src/gemseo_umdo/scenarios/umdo_scenario.py
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-09 17:50:16.877750 gemseo-umdo-1.0.2/src/gemseo_umdo/use_cases/
--rw-r--r--   0 ad        (1000) ad        (1000)      940 2023-02-09 15:49:03.000000 gemseo-umdo-1.0.2/src/gemseo_umdo/use_cases/__init__.py
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-09 17:50:16.878750 gemseo-umdo-1.0.2/src/gemseo_umdo/use_cases/spring_mass_model/
--rw-r--r--   0 ad        (1000) ad        (1000)      818 2023-02-09 15:49:03.000000 gemseo-umdo-1.0.2/src/gemseo_umdo/use_cases/spring_mass_model/__init__.py
--rw-r--r--   0 ad        (1000) ad        (1000)     2943 2023-02-09 15:49:03.000000 gemseo-umdo-1.0.2/src/gemseo_umdo/use_cases/spring_mass_model/discipline.py
--rw-r--r--   0 ad        (1000) ad        (1000)     3493 2023-02-09 15:49:03.000000 gemseo-umdo-1.0.2/src/gemseo_umdo/use_cases/spring_mass_model/model.py
--rw-r--r--   0 ad        (1000) ad        (1000)     1282 2023-02-09 15:49:03.000000 gemseo-umdo-1.0.2/src/gemseo_umdo/use_cases/spring_mass_model/uncertain_space.py
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-09 17:50:16.874750 gemseo-umdo-1.0.2/src/gemseo_umdo.egg-info/
--rw-r--r--   0 ad        (1000) ad        (1000)     2482 2023-02-09 17:50:16.000000 gemseo-umdo-1.0.2/src/gemseo_umdo.egg-info/PKG-INFO
--rw-r--r--   0 ad        (1000) ad        (1000)     2736 2023-02-09 17:50:16.000000 gemseo-umdo-1.0.2/src/gemseo_umdo.egg-info/SOURCES.txt
--rw-r--r--   0 ad        (1000) ad        (1000)        1 2023-02-09 17:50:16.000000 gemseo-umdo-1.0.2/src/gemseo_umdo.egg-info/dependency_links.txt
--rw-r--r--   0 ad        (1000) ad        (1000)       43 2023-02-09 17:50:16.000000 gemseo-umdo-1.0.2/src/gemseo_umdo.egg-info/entry_points.txt
--rw-r--r--   0 ad        (1000) ad        (1000)       87 2023-02-09 17:50:16.000000 gemseo-umdo-1.0.2/src/gemseo_umdo.egg-info/requires.txt
--rw-r--r--   0 ad        (1000) ad        (1000)       12 2023-02-09 17:50:16.000000 gemseo-umdo-1.0.2/src/gemseo_umdo.egg-info/top_level.txt
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-09 17:50:16.878750 gemseo-umdo-1.0.2/tests/
--rw-r--r--   0 ad        (1000) ad        (1000)      770 2023-02-09 15:09:36.000000 gemseo-umdo-1.0.2/tests/__init__.py
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-09 17:50:16.879750 gemseo-umdo-1.0.2/tests/formulations/
--rw-r--r--   0 ad        (1000) ad        (1000)      770 2023-02-09 15:09:36.000000 gemseo-umdo-1.0.2/tests/formulations/__init__.py
--rw-r--r--   0 ad        (1000) ad        (1000)     2786 2023-02-09 15:09:36.000000 gemseo-umdo-1.0.2/tests/formulations/conftest.py
--rw-r--r--   0 ad        (1000) ad        (1000)     1614 2023-02-09 15:09:36.000000 gemseo-umdo-1.0.2/tests/formulations/test_factory.py
--rw-r--r--   0 ad        (1000) ad        (1000)     8492 2023-02-09 15:09:36.000000 gemseo-umdo-1.0.2/tests/formulations/test_sampling.py
--rw-r--r--   0 ad        (1000) ad        (1000)     7055 2023-02-09 15:52:58.000000 gemseo-umdo-1.0.2/tests/formulations/test_u_formulation.py
--rw-r--r--   0 ad        (1000) ad        (1000)     7550 2023-02-09 15:49:03.000000 gemseo-umdo-1.0.2/tests/test_scenario.py
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-09 17:50:16.879750 gemseo-umdo-1.0.2/tests/use_cases/
--rw-r--r--   0 ad        (1000) ad        (1000)      770 2023-02-09 15:49:03.000000 gemseo-umdo-1.0.2/tests/use_cases/__init__.py
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-09 17:50:16.879750 gemseo-umdo-1.0.2/tests/use_cases/spring_mass_model/
--rw-r--r--   0 ad        (1000) ad        (1000)      770 2023-02-09 15:49:03.000000 gemseo-umdo-1.0.2/tests/use_cases/spring_mass_model/__init__.py
--rw-r--r--   0 ad        (1000) ad        (1000)     3926 2023-02-09 15:49:03.000000 gemseo-umdo-1.0.2/tests/use_cases/spring_mass_model/test_discipline.py
--rw-r--r--   0 ad        (1000) ad        (1000)     2788 2023-02-09 15:49:03.000000 gemseo-umdo-1.0.2/tests/use_cases/spring_mass_model/test_model.py
--rw-r--r--   0 ad        (1000) ad        (1000)     1359 2023-02-09 15:49:03.000000 gemseo-umdo-1.0.2/tests/use_cases/spring_mass_model/test_uncertain_space.py
--rw-r--r--   0 ad        (1000) ad        (1000)     3256 2023-02-09 15:09:36.000000 gemseo-umdo-1.0.2/tox.ini
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:29:24.040987 gemseo-umdo-1.1.0/
+-rw-r--r--   0 ad        (1000) ad        (1000)      450 2023-05-25 19:11:28.000000 gemseo-umdo-1.1.0/.gitattributes
+-rw-r--r--   0 ad        (1000) ad        (1000)      190 2023-05-25 19:11:28.000000 gemseo-umdo-1.1.0/.gitignore
+-rw-r--r--   0 ad        (1000) ad        (1000)       87 2023-06-02 16:29:58.000000 gemseo-umdo-1.1.0/.gitlab-ci.yml
+-rw-r--r--   0 ad        (1000) ad        (1000)     3051 2023-05-25 19:11:28.000000 gemseo-umdo-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 ad        (1000) ad        (1000)     9105 2023-05-25 19:11:28.000000 gemseo-umdo-1.1.0/.pylintrc
+-rw-r--r--   0 ad        (1000) ad        (1000)     2182 2023-06-02 16:29:58.000000 gemseo-umdo-1.1.0/CHANGELOG.rst
+-rw-r--r--   0 ad        (1000) ad        (1000)     1763 2023-05-29 07:12:22.000000 gemseo-umdo-1.1.0/CREDITS.rst
+-rw-r--r--   0 ad        (1000) ad        (1000)     7652 2023-05-25 19:10:50.000000 gemseo-umdo-1.1.0/LICENSE.txt
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:29:24.015987 gemseo-umdo-1.1.0/LICENSES/
+-rw-r--r--   0 ad        (1000) ad        (1000)     7652 2023-05-25 19:10:50.000000 gemseo-umdo-1.1.0/LICENSES/LGPLv3.txt
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:29:24.016987 gemseo-umdo-1.1.0/LICENSES/headers/
+-rw-r--r--   0 ad        (1000) ad        (1000)      729 2023-05-25 19:10:50.000000 gemseo-umdo-1.1.0/LICENSES/headers/BSD-0-Clause.txt
+-rw-r--r--   0 ad        (1000) ad        (1000)      334 2023-05-25 19:10:50.000000 gemseo-umdo-1.1.0/LICENSES/headers/CC-BY-SA-4.0.txt
+-rw-r--r--   0 ad        (1000) ad        (1000)      710 2023-05-25 19:10:50.000000 gemseo-umdo-1.1.0/LICENSES/headers/LGPL-3.0.txt
+-rw-r--r--   0 ad        (1000) ad        (1000)     2432 2023-06-04 18:29:24.040987 gemseo-umdo-1.1.0/PKG-INFO
+-rw-r--r--   0 ad        (1000) ad        (1000)     1388 2023-05-29 07:12:22.000000 gemseo-umdo-1.1.0/README.rst
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:29:24.011987 gemseo-umdo-1.1.0/doc_src/
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:29:24.011987 gemseo-umdo-1.1.0/doc_src/examples/
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:29:24.011987 gemseo-umdo-1.1.0/doc_src/examples/udoe/
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:29:24.017987 gemseo-umdo-1.1.0/doc_src/examples/udoe/quadratic/
+-rw-r--r--   0 ad        (1000) ad        (1000)      426 2023-02-09 15:09:36.000000 gemseo-umdo-1.1.0/doc_src/examples/udoe/quadratic/README.rst
+-rw-r--r--   0 ad        (1000) ad        (1000)     2448 2023-06-02 16:29:58.000000 gemseo-umdo-1.1.0/doc_src/examples/udoe/quadratic/sampling.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     2562 2023-06-02 16:29:58.000000 gemseo-umdo-1.1.0/doc_src/examples/udoe/quadratic/sequential_sampling.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     2415 2023-06-02 16:29:58.000000 gemseo-umdo-1.1.0/doc_src/examples/udoe/quadratic/taylor_polynomial.py
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:29:24.017987 gemseo-umdo-1.1.0/doc_src/examples/umdo/
+-rw-r--r--   0 ad        (1000) ad        (1000)      402 2023-02-09 15:09:36.000000 gemseo-umdo-1.1.0/doc_src/examples/umdo/README.rst
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:29:24.017987 gemseo-umdo-1.1.0/doc_src/examples/umdo/quadratic/
+-rw-r--r--   0 ad        (1000) ad        (1000)      426 2023-02-09 15:09:36.000000 gemseo-umdo-1.1.0/doc_src/examples/umdo/quadratic/README.rst
+-rw-r--r--   0 ad        (1000) ad        (1000)     2437 2023-06-02 16:29:58.000000 gemseo-umdo-1.1.0/doc_src/examples/umdo/quadratic/sampling.py
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:29:24.018987 gemseo-umdo-1.1.0/doc_src/examples/umdo/rosenbrock/
+-rw-r--r--   0 ad        (1000) ad        (1000)      428 2023-02-09 15:09:36.000000 gemseo-umdo-1.1.0/doc_src/examples/umdo/rosenbrock/README.rst
+-rw-r--r--   0 ad        (1000) ad        (1000)     2705 2023-06-02 16:29:58.000000 gemseo-umdo-1.1.0/doc_src/examples/umdo/rosenbrock/sampling.py
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:29:24.019987 gemseo-umdo-1.1.0/doc_src/examples/umdo/sellar/
+-rw-r--r--   0 ad        (1000) ad        (1000)      420 2023-02-09 15:09:36.000000 gemseo-umdo-1.1.0/doc_src/examples/umdo/sellar/README.rst
+-rw-r--r--   0 ad        (1000) ad        (1000)     2326 2023-06-02 16:29:58.000000 gemseo-umdo-1.1.0/doc_src/examples/umdo/sellar/deterministic.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     2949 2023-06-02 16:29:58.000000 gemseo-umdo-1.1.0/doc_src/examples/umdo/sellar/first_order_taylor_polynomial.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     2805 2023-06-02 16:29:58.000000 gemseo-umdo-1.1.0/doc_src/examples/umdo/sellar/sampling.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     3466 2023-06-02 16:29:58.000000 gemseo-umdo-1.1.0/doc_src/examples/umdo/sellar/sampling_with_repetitions.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     2951 2023-06-02 16:29:58.000000 gemseo-umdo-1.1.0/doc_src/examples/umdo/sellar/second_order_taylor_polynomial.py
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:29:24.019987 gemseo-umdo-1.1.0/doc_src/examples/umdo/sobieski/
+-rw-r--r--   0 ad        (1000) ad        (1000)      424 2023-02-09 15:09:36.000000 gemseo-umdo-1.1.0/doc_src/examples/umdo/sobieski/README.rst
+-rw-r--r--   0 ad        (1000) ad        (1000)     3259 2023-06-02 16:29:58.000000 gemseo-umdo-1.1.0/doc_src/examples/umdo/sobieski/first_order_taylor_polynomial.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     3126 2023-06-02 16:29:58.000000 gemseo-umdo-1.1.0/doc_src/examples/umdo/sobieski/sampling.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     3294 2023-06-02 16:29:58.000000 gemseo-umdo-1.1.0/doc_src/examples/umdo/sobieski/second_order_taylor_polynomial.py
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:29:24.020987 gemseo-umdo-1.1.0/doc_src/examples/use_cases/
+-rw-r--r--   0 ad        (1000) ad        (1000)      384 2023-06-02 16:29:58.000000 gemseo-umdo-1.1.0/doc_src/examples/use_cases/README.rst
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:29:24.020987 gemseo-umdo-1.1.0/doc_src/examples/use_cases/beam_model/
+-rw-r--r--   0 ad        (1000) ad        (1000)      392 2023-06-02 16:29:58.000000 gemseo-umdo-1.1.0/doc_src/examples/use_cases/beam_model/README.rst
+-rw-r--r--   0 ad        (1000) ad        (1000)     2171 2023-06-02 16:29:58.000000 gemseo-umdo-1.1.0/doc_src/examples/use_cases/beam_model/deterministic_doe.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     1773 2023-06-02 16:29:58.000000 gemseo-umdo-1.1.0/doc_src/examples/use_cases/beam_model/deterministic_optimization.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     2255 2023-06-02 16:29:58.000000 gemseo-umdo-1.1.0/doc_src/examples/use_cases/beam_model/robust_optimization.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     2002 2023-06-02 16:29:58.000000 gemseo-umdo-1.1.0/doc_src/examples/use_cases/beam_model/sensitivity_analysis.py
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:29:24.020987 gemseo-umdo-1.1.0/doc_src/examples/visualizations/
+-rw-r--r--   0 ad        (1000) ad        (1000)      396 2023-06-02 16:29:58.000000 gemseo-umdo-1.1.0/doc_src/examples/visualizations/README.rst
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:29:24.021987 gemseo-umdo-1.1.0/doc_src/examples/visualizations/sobol_graph/
+-rw-r--r--   0 ad        (1000) ad        (1000)      384 2023-06-02 16:29:58.000000 gemseo-umdo-1.1.0/doc_src/examples/visualizations/sobol_graph/README.rst
+-rw-r--r--   0 ad        (1000) ad        (1000)     2186 2023-06-02 16:29:58.000000 gemseo-umdo-1.1.0/doc_src/examples/visualizations/sobol_graph/ishigami.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     1918 2023-06-02 16:29:58.000000 gemseo-umdo-1.1.0/doc_src/examples/visualizations/sobol_graph/sellar.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     2581 2023-06-02 16:29:58.000000 gemseo-umdo-1.1.0/doc_src/examples/visualizations/sobol_graph/sobieski.py
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:29:24.021987 gemseo-umdo-1.1.0/doc_src/examples/visualizations/uncertain_coupling_graph/
+-rw-r--r--   0 ad        (1000) ad        (1000)      408 2023-06-02 16:29:58.000000 gemseo-umdo-1.1.0/doc_src/examples/visualizations/uncertain_coupling_graph/README.rst
+-rw-r--r--   0 ad        (1000) ad        (1000)     2558 2023-06-02 16:29:58.000000 gemseo-umdo-1.1.0/doc_src/examples/visualizations/uncertain_coupling_graph/sobieski.py
+-rw-r--r--   0 ad        (1000) ad        (1000)      611 2023-05-25 19:11:12.000000 gemseo-umdo-1.1.0/pyproject.toml
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:29:24.023987 gemseo-umdo-1.1.0/requirements/
+-rw-r--r--   0 ad        (1000) ad        (1000)       79 2023-05-25 19:11:12.000000 gemseo-umdo-1.1.0/requirements/check.in
+-rw-r--r--   0 ad        (1000) ad        (1000)      573 2023-05-16 08:26:16.000000 gemseo-umdo-1.1.0/requirements/check.txt
+-rw-r--r--   0 ad        (1000) ad        (1000)       12 2023-05-25 19:11:12.000000 gemseo-umdo-1.1.0/requirements/dist.in
+-rw-r--r--   0 ad        (1000) ad        (1000)     1491 2023-05-16 08:26:16.000000 gemseo-umdo-1.1.0/requirements/dist.txt
+-rw-r--r--   0 ad        (1000) ad        (1000)     2253 2023-02-09 15:09:36.000000 gemseo-umdo-1.1.0/requirements/doc.txt
+-rw-r--r--   0 ad        (1000) ad        (1000)     2747 2023-05-16 08:26:16.000000 gemseo-umdo-1.1.0/requirements/test-python3.10.txt
+-rw-r--r--   0 ad        (1000) ad        (1000)     2837 2023-05-16 08:26:16.000000 gemseo-umdo-1.1.0/requirements/test-python3.8.txt
+-rw-r--r--   0 ad        (1000) ad        (1000)     2837 2023-05-16 08:26:16.000000 gemseo-umdo-1.1.0/requirements/test-python3.9.txt
+-rw-r--r--   0 ad        (1000) ad        (1000)     1649 2023-06-04 18:29:24.041987 gemseo-umdo-1.1.0/setup.cfg
+-rw-r--r--   0 ad        (1000) ad        (1000)      839 2022-07-25 06:47:03.000000 gemseo-umdo-1.1.0/setup.py
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:29:24.012987 gemseo-umdo-1.1.0/src/
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:29:24.023987 gemseo-umdo-1.1.0/src/gemseo_umdo/
+-rw-r--r--   0 ad        (1000) ad        (1000)      834 2023-02-09 15:09:36.000000 gemseo-umdo-1.1.0/src/gemseo_umdo/__init__.py
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:29:24.024987 gemseo-umdo-1.1.0/src/gemseo_umdo/estimators/
+-rw-r--r--   0 ad        (1000) ad        (1000)      838 2023-02-09 15:09:36.000000 gemseo-umdo-1.1.0/src/gemseo_umdo/estimators/__init__.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     2278 2023-05-16 08:26:16.000000 gemseo-umdo-1.1.0/src/gemseo_umdo/estimators/estimator.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     3916 2023-05-16 08:26:16.000000 gemseo-umdo-1.1.0/src/gemseo_umdo/estimators/sampling.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     4714 2023-06-02 16:29:58.000000 gemseo-umdo-1.1.0/src/gemseo_umdo/estimators/taylor_polynomial.py
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:29:24.026987 gemseo-umdo-1.1.0/src/gemseo_umdo/formulations/
+-rw-r--r--   0 ad        (1000) ad        (1000)     2240 2023-05-16 08:26:16.000000 gemseo-umdo-1.1.0/src/gemseo_umdo/formulations/__init__.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     1172 2023-05-16 08:26:16.000000 gemseo-umdo-1.1.0/src/gemseo_umdo/formulations/factory.py
+-rw-r--r--   0 ad        (1000) ad        (1000)    12190 2023-06-01 15:57:10.000000 gemseo-umdo-1.1.0/src/gemseo_umdo/formulations/formulation.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     5757 2023-05-16 08:28:35.000000 gemseo-umdo-1.1.0/src/gemseo_umdo/formulations/sampling.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     3896 2023-06-02 16:29:58.000000 gemseo-umdo-1.1.0/src/gemseo_umdo/formulations/sequential_sampling.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     9723 2023-06-02 16:29:58.000000 gemseo-umdo-1.1.0/src/gemseo_umdo/formulations/taylor_polynomial.py
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:29:24.027987 gemseo-umdo-1.1.0/src/gemseo_umdo/scenarios/
+-rw-r--r--   0 ad        (1000) ad        (1000)      850 2023-02-09 15:09:36.000000 gemseo-umdo-1.1.0/src/gemseo_umdo/scenarios/__init__.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     8753 2023-05-16 08:26:16.000000 gemseo-umdo-1.1.0/src/gemseo_umdo/scenarios/_scenario.py
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:29:24.027987 gemseo-umdo-1.1.0/src/gemseo_umdo/scenarios/udoe/
+-rw-r--r--   0 ad        (1000) ad        (1000)      444 2022-07-01 08:15:59.000000 gemseo-umdo-1.1.0/src/gemseo_umdo/scenarios/udoe/UDOEScenario_input.json
+-rw-r--r--   0 ad        (1000) ad        (1000)      198 2022-07-01 08:15:59.000000 gemseo-umdo-1.1.0/src/gemseo_umdo/scenarios/udoe/UDOEScenario_output.json
+-rw-r--r--   0 ad        (1000) ad        (1000)     1211 2023-02-09 17:52:38.000000 gemseo-umdo-1.1.0/src/gemseo_umdo/scenarios/udoe_scenario.py
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:29:24.027987 gemseo-umdo-1.1.0/src/gemseo_umdo/scenarios/umdo/
+-rw-r--r--   0 ad        (1000) ad        (1000)      399 2022-07-01 08:15:59.000000 gemseo-umdo-1.1.0/src/gemseo_umdo/scenarios/umdo/UMDOScenario_input.json
+-rw-r--r--   0 ad        (1000) ad        (1000)      198 2022-07-01 08:15:59.000000 gemseo-umdo-1.1.0/src/gemseo_umdo/scenarios/umdo/UMDOScenario_output.json
+-rw-r--r--   0 ad        (1000) ad        (1000)     1222 2023-02-09 17:52:38.000000 gemseo-umdo-1.1.0/src/gemseo_umdo/scenarios/umdo_scenario.py
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:29:24.027987 gemseo-umdo-1.1.0/src/gemseo_umdo/use_cases/
+-rw-r--r--   0 ad        (1000) ad        (1000)      940 2023-02-09 15:49:03.000000 gemseo-umdo-1.1.0/src/gemseo_umdo/use_cases/__init__.py
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:29:24.029987 gemseo-umdo-1.1.0/src/gemseo_umdo/use_cases/beam_model/
+-rw-r--r--   0 ad        (1000) ad        (1000)      792 2023-06-02 16:29:58.000000 gemseo-umdo-1.1.0/src/gemseo_umdo/use_cases/beam_model/__init__.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     4249 2023-06-02 16:29:58.000000 gemseo-umdo-1.1.0/src/gemseo_umdo/use_cases/beam_model/advanced_uncertain_space.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     2144 2023-06-02 16:29:58.000000 gemseo-umdo-1.1.0/src/gemseo_umdo/use_cases/beam_model/constraints.py
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:29:24.031987 gemseo-umdo-1.1.0/src/gemseo_umdo/use_cases/beam_model/core/
+-rw-r--r--   0 ad        (1000) ad        (1000)      819 2023-06-02 16:29:58.000000 gemseo-umdo-1.1.0/src/gemseo_umdo/use_cases/beam_model/core/__init__.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     1601 2023-06-02 16:29:58.000000 gemseo-umdo-1.1.0/src/gemseo_umdo/use_cases/beam_model/core/design_space.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     9029 2023-06-02 16:29:58.000000 gemseo-umdo-1.1.0/src/gemseo_umdo/use_cases/beam_model/core/model.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     1685 2023-06-02 16:29:58.000000 gemseo-umdo-1.1.0/src/gemseo_umdo/use_cases/beam_model/core/output_data.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     2095 2023-06-02 16:29:58.000000 gemseo-umdo-1.1.0/src/gemseo_umdo/use_cases/beam_model/core/variables.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     1373 2023-06-02 16:29:58.000000 gemseo-umdo-1.1.0/src/gemseo_umdo/use_cases/beam_model/design_space.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     3023 2023-06-02 16:29:58.000000 gemseo-umdo-1.1.0/src/gemseo_umdo/use_cases/beam_model/discipline.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     3095 2023-06-02 16:29:58.000000 gemseo-umdo-1.1.0/src/gemseo_umdo/use_cases/beam_model/uncertain_space.py
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:29:24.032987 gemseo-umdo-1.1.0/src/gemseo_umdo/use_cases/spring_mass_model/
+-rw-r--r--   0 ad        (1000) ad        (1000)      818 2023-02-09 15:49:03.000000 gemseo-umdo-1.1.0/src/gemseo_umdo/use_cases/spring_mass_model/__init__.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     2961 2023-05-16 08:26:16.000000 gemseo-umdo-1.1.0/src/gemseo_umdo/use_cases/spring_mass_model/discipline.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     3493 2023-02-09 15:49:03.000000 gemseo-umdo-1.1.0/src/gemseo_umdo/use_cases/spring_mass_model/model.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     1282 2023-02-09 15:49:03.000000 gemseo-umdo-1.1.0/src/gemseo_umdo/use_cases/spring_mass_model/uncertain_space.py
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:29:24.033987 gemseo-umdo-1.1.0/src/gemseo_umdo/visualizations/
+-rw-r--r--   0 ad        (1000) ad        (1000)      796 2023-06-02 16:29:58.000000 gemseo-umdo-1.1.0/src/gemseo_umdo/visualizations/__init__.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     6590 2023-06-02 16:29:58.000000 gemseo-umdo-1.1.0/src/gemseo_umdo/visualizations/sobol_graph.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     7884 2023-06-02 16:29:58.000000 gemseo-umdo-1.1.0/src/gemseo_umdo/visualizations/uncertain_coupling_graph.py
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:29:24.024987 gemseo-umdo-1.1.0/src/gemseo_umdo.egg-info/
+-rw-r--r--   0 ad        (1000) ad        (1000)     2432 2023-06-04 18:29:23.000000 gemseo-umdo-1.1.0/src/gemseo_umdo.egg-info/PKG-INFO
+-rw-r--r--   0 ad        (1000) ad        (1000)     6009 2023-06-04 18:29:24.000000 gemseo-umdo-1.1.0/src/gemseo_umdo.egg-info/SOURCES.txt
+-rw-r--r--   0 ad        (1000) ad        (1000)        1 2023-06-04 18:29:23.000000 gemseo-umdo-1.1.0/src/gemseo_umdo.egg-info/dependency_links.txt
+-rw-r--r--   0 ad        (1000) ad        (1000)       43 2023-06-04 18:29:23.000000 gemseo-umdo-1.1.0/src/gemseo_umdo.egg-info/entry_points.txt
+-rw-r--r--   0 ad        (1000) ad        (1000)       89 2023-06-04 18:29:23.000000 gemseo-umdo-1.1.0/src/gemseo_umdo.egg-info/requires.txt
+-rw-r--r--   0 ad        (1000) ad        (1000)       12 2023-06-04 18:29:23.000000 gemseo-umdo-1.1.0/src/gemseo_umdo.egg-info/top_level.txt
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:29:24.033987 gemseo-umdo-1.1.0/tests/
+-rw-r--r--   0 ad        (1000) ad        (1000)      770 2023-02-09 15:09:36.000000 gemseo-umdo-1.1.0/tests/__init__.py
+-rw-r--r--   0 ad        (1000) ad        (1000)      934 2023-06-02 16:29:58.000000 gemseo-umdo-1.1.0/tests/conftest.py
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:29:24.035987 gemseo-umdo-1.1.0/tests/formulations/
+-rw-r--r--   0 ad        (1000) ad        (1000)      770 2023-02-09 15:09:36.000000 gemseo-umdo-1.1.0/tests/formulations/__init__.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     2786 2023-02-09 15:09:36.000000 gemseo-umdo-1.1.0/tests/formulations/conftest.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     1614 2023-02-09 15:09:36.000000 gemseo-umdo-1.1.0/tests/formulations/test_factory.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     8492 2023-05-16 08:26:16.000000 gemseo-umdo-1.1.0/tests/formulations/test_sampling.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     1871 2023-06-02 16:29:58.000000 gemseo-umdo-1.1.0/tests/formulations/test_sequential_sampling.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     8758 2023-06-02 16:29:58.000000 gemseo-umdo-1.1.0/tests/formulations/test_taylor_polynomial.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     7063 2023-06-01 06:54:19.000000 gemseo-umdo-1.1.0/tests/formulations/test_u_formulation.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     7547 2023-05-16 08:26:16.000000 gemseo-umdo-1.1.0/tests/test_scenario.py
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:29:24.035987 gemseo-umdo-1.1.0/tests/use_cases/
+-rw-r--r--   0 ad        (1000) ad        (1000)      770 2023-02-09 15:49:03.000000 gemseo-umdo-1.1.0/tests/use_cases/__init__.py
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:29:24.036987 gemseo-umdo-1.1.0/tests/use_cases/beam_model/
+-rw-r--r--   0 ad        (1000) ad        (1000)      770 2023-06-02 16:29:58.000000 gemseo-umdo-1.1.0/tests/use_cases/beam_model/__init__.py
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:29:24.037987 gemseo-umdo-1.1.0/tests/use_cases/beam_model/core/
+-rw-r--r--   0 ad        (1000) ad        (1000)      770 2023-06-02 16:29:58.000000 gemseo-umdo-1.1.0/tests/use_cases/beam_model/core/__init__.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     1375 2023-06-02 16:29:58.000000 gemseo-umdo-1.1.0/tests/use_cases/beam_model/core/test_design_space.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     4352 2023-06-02 16:29:58.000000 gemseo-umdo-1.1.0/tests/use_cases/beam_model/core/test_model.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     1165 2023-06-02 16:29:58.000000 gemseo-umdo-1.1.0/tests/use_cases/beam_model/core/test_output_data.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     4236 2023-06-02 16:29:58.000000 gemseo-umdo-1.1.0/tests/use_cases/beam_model/test_advanced_uncertain_space.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     2218 2023-06-02 16:29:58.000000 gemseo-umdo-1.1.0/tests/use_cases/beam_model/test_constraints.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     1730 2023-06-02 16:29:58.000000 gemseo-umdo-1.1.0/tests/use_cases/beam_model/test_design_space.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     3541 2023-06-02 16:29:58.000000 gemseo-umdo-1.1.0/tests/use_cases/beam_model/test_discipline.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     2469 2023-06-02 16:29:58.000000 gemseo-umdo-1.1.0/tests/use_cases/beam_model/test_uncertain_space.py
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:29:24.038987 gemseo-umdo-1.1.0/tests/use_cases/spring_mass_model/
+-rw-r--r--   0 ad        (1000) ad        (1000)      770 2023-02-09 15:49:03.000000 gemseo-umdo-1.1.0/tests/use_cases/spring_mass_model/__init__.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     3926 2023-02-09 15:49:03.000000 gemseo-umdo-1.1.0/tests/use_cases/spring_mass_model/test_discipline.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     2788 2023-02-09 15:49:03.000000 gemseo-umdo-1.1.0/tests/use_cases/spring_mass_model/test_model.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     1359 2023-02-09 15:49:03.000000 gemseo-umdo-1.1.0/tests/use_cases/spring_mass_model/test_uncertain_space.py
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:29:24.038987 gemseo-umdo-1.1.0/tests/visualizations/
+-rw-r--r--   0 ad        (1000) ad        (1000)      796 2023-06-02 16:29:58.000000 gemseo-umdo-1.1.0/tests/visualizations/__init__.py
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:29:24.039987 gemseo-umdo-1.1.0/tests/visualizations/sobol_graph/
+-rw-r--r--   0 ad        (1000) ad        (1000)      411 2023-06-02 16:29:58.000000 gemseo-umdo-1.1.0/tests/visualizations/sobol_graph/default.dot
+-rw-r--r--   0 ad        (1000) ad        (1000)      601 2023-06-02 16:29:58.000000 gemseo-umdo-1.1.0/tests/visualizations/sobol_graph/from_analysis.dot
+-rw-r--r--   0 ad        (1000) ad        (1000)      413 2023-06-02 16:29:58.000000 gemseo-umdo-1.1.0/tests/visualizations/sobol_graph/maximum_thickness.dot
+-rw-r--r--   0 ad        (1000) ad        (1000)      314 2023-06-02 16:29:58.000000 gemseo-umdo-1.1.0/tests/visualizations/sobol_graph/threshold.dot
+-rw-r--r--   0 ad        (1000) ad        (1000)     4637 2023-06-02 16:29:58.000000 gemseo-umdo-1.1.0/tests/visualizations/test_sobol_graph.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     5733 2023-06-02 16:29:58.000000 gemseo-umdo-1.1.0/tests/visualizations/test_uncertain_coupling_graph.py
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:29:24.040987 gemseo-umdo-1.1.0/tests/visualizations/uncertain_coupling_graph/
+-rw-r--r--   0 ad        (1000) ad        (1000)     1481 2023-06-02 16:29:58.000000 gemseo-umdo-1.1.0/tests/visualizations/uncertain_coupling_graph/default.dot
+-rw-r--r--   0 ad        (1000) ad        (1000)     1480 2023-06-02 16:29:58.000000 gemseo-umdo-1.1.0/tests/visualizations/uncertain_coupling_graph/dispersion_measure.dot
+-rw-r--r--   0 ad        (1000) ad        (1000)      488 2023-06-02 16:29:58.000000 gemseo-umdo-1.1.0/tests/visualizations/uncertain_coupling_graph/filter_names.dot
+-rw-r--r--   0 ad        (1000) ad        (1000)     1482 2023-06-02 16:29:58.000000 gemseo-umdo-1.1.0/tests/visualizations/uncertain_coupling_graph/maximum_thickness.dot
+-rw-r--r--   0 ad        (1000) ad        (1000)      488 2023-06-02 16:29:58.000000 gemseo-umdo-1.1.0/tests/visualizations/uncertain_coupling_graph/output_names.dot
+-rw-r--r--   0 ad        (1000) ad        (1000)      312 2023-06-02 16:29:58.000000 gemseo-umdo-1.1.0/tests/visualizations/uncertain_coupling_graph/self_coupled.dot
+-rw-r--r--   0 ad        (1000) ad        (1000)     3272 2023-05-25 19:10:50.000000 gemseo-umdo-1.1.0/tox.ini
```

### Comparing `gemseo-umdo-1.0.2/.pre-commit-config.yaml` & `gemseo-umdo-1.1.0/.pre-commit-config.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -19,15 +19,15 @@
   rev: v1.10.0
   hooks:
     - id: rst-backticks
     - id: rst-directive-colons
     - id: rst-inline-touching-normal
 
 - repo: https://github.com/PyCQA/autoflake
-  rev: v2.0.0
+  rev: v2.1.1
   hooks:
     - id: autoflake
       args: [
         --in-place,
         --remove-all-unused-imports,
       ]
 
@@ -36,73 +36,83 @@
   hooks:
     - id: reorder-python-imports
       name: reorder python imports in src
       files: ^src
       args: [
         --application-directories,
         src,
-        --py37-plus,
+        --py38-plus,
         --add-import,
         "from __future__ import annotations",
-        --replace-import,
-        "typing=gemseo.utils.python_compatibility:Final"
       ]
     - id: reorder-python-imports
       name: reorder python imports out of src
       exclude: ^src
       args: [
-        --py37-plus,
+        --py38-plus,
         --add-import,
         "from __future__ import annotations",
-        --replace-import,
-        "typing=gemseo.utils.python_compatibility:Final"
       ]
 
 - repo: https://github.com/myint/docformatter
-  rev: v1.5.1
+  rev: v1.6.5
   hooks:
     - id: docformatter
       args: [
         --in-place,
         --wrap-summaries,
-        "89",
+        "88",
         --wrap-descriptions,
-        "89",
+        "88",
       ]
 
 - repo: https://github.com/asottile/pyupgrade
-  rev: v3.3.1
+  rev: v3.4.0
   hooks:
     - id: pyupgrade
-      args: [--py37-plus]
+      args: [--py38-plus]
 
 - repo: https://github.com/psf/black
-  rev: 22.12.0
+  rev: 23.3.0
   hooks:
     - id: black
 
 - repo: https://github.com/PyCQA/flake8
   rev: 6.0.0
   hooks:
     - id: flake8
       additional_dependencies:
-        - flake8-bugbear==22.12.6
-        - flake8-docstrings==1.6.0
+        - flake8-annotations==3.0.1
+        - flake8-bugbear==23.5.9
+        - flake8-docstrings==1.7.0
         - flake8-logging-format==0.9.0
         - flake8-print==5.0.0
         - pep8-naming==0.13.3
 
 - repo: https://github.com/commitizen-tools/commitizen
-  rev: v2.39.1
+  rev: 3.2.2
   hooks:
     - id: commitizen
       stages: [commit-msg]
 
+- repo: https://github.com/kynan/nbstripout
+  rev: 0.6.1
+  hooks:
+    - id: nbstripout
+
+- repo: https://github.com/nbQA-dev/nbQA
+  rev: 1.7.0
+  hooks:
+    - id: nbqa-black
+    - id: nbqa-pyupgrade
+      args: [ "--py38-plus" ]
+    - id: nbqa-autopep8
+
 - repo: https://github.com/Lucas-C/pre-commit-hooks
-  rev: v1.3.1
+  rev: v1.5.1
   hooks:
     - id: insert-license
       name: insert LGPL license
       exclude: ^doc_src
       files: \.py$
       args:
         - --license-filepath
```

### Comparing `gemseo-umdo-1.0.2/.pylintrc` & `gemseo-umdo-1.1.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `gemseo-umdo-1.0.2/CHANGELOG.rst` & `gemseo-umdo-1.1.0/CHANGELOG.rst`

 * *Files 19% similar despite different names*

```diff
@@ -21,21 +21,27 @@
 All notable changes of this project will be documented here.
 
 The format is based on
 `Keep a Changelog <https://keepachangelog.com/en/1.0.0/>`_
 and this project adheres to
 `Semantic Versioning <https://semver.org/spec/v2.0.0.html>`_.
 
-Version 1.0.2 (February 2023)
-*****************************
+
+Version 1.1.0 (June 2023)
+*************************
 
 Added
 -----
 
-- :class:`.SpringMassModel`, :class:`.SpringMassDiscipline` and :class:`.SpringMassUncertainSpace` is a use case based on a spring-mass system.
+- The beam problem (:class:`.Beam`, :class:`.BeamConstraints`, :class:`BeamUncertainSpace` and :class:`.BeamDesignSpace` to benchmark robust optimization algorithms.
+- :class:`.TaylorPolynomial`, a new :class:`.UMDOFormulation` estimating the statistics with Taylor polynomials.
+- :class:`.SequentialSampling`, a new :class:`.UMDOFormulation` estimating the statistics with sequential sampling.
+- :class:`.UncertainCouplingGraph` to visualize the dispersion of the coupling variables.
+- :class:`.SobolGraph` to visualize the first-, second- and total-order Sobol' indices.
+- The set of :class:`.SpringMassModel`, :class:`.SpringMassDiscipline` and :class:`.SpringMassUncertainSpace` is a use case based on a spring-mass system.
 
 Fixed
 -----
 
 - The :class:`._UScenario` no longer changes the list of disciplines passed by the user.
 
 Version 1.0.1 (January 2023)
```

### Comparing `gemseo-umdo-1.0.2/CREDITS.rst` & `gemseo-umdo-1.1.0/CREDITS.rst`

 * *Files identical despite different names*

### Comparing `gemseo-umdo-1.0.2/LICENSE.txt` & `gemseo-umdo-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gemseo-umdo-1.0.2/LICENSES/LGPLv3.txt` & `gemseo-umdo-1.1.0/LICENSES/LGPLv3.txt`

 * *Files identical despite different names*

### Comparing `gemseo-umdo-1.0.2/LICENSES/headers/BSD-0-Clause.txt` & `gemseo-umdo-1.1.0/LICENSES/headers/BSD-0-Clause.txt`

 * *Files identical despite different names*

### Comparing `gemseo-umdo-1.0.2/LICENSES/headers/LGPL-3.0.txt` & `gemseo-umdo-1.1.0/LICENSES/headers/LGPL-3.0.txt`

 * *Files identical despite different names*

### Comparing `gemseo-umdo-1.0.2/PKG-INFO` & `gemseo-umdo-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: gemseo-umdo
-Version: 1.0.2
+Version: 1.1.0
 Summary: Capability for MDO under uncertainty.
 Home-page: https://gitlab.com/gemseo
 Author: Matthias De Lozzo
 Author-email: contact@gemseo.org
 License: GNU Lesser General Public License v3
 Project-URL: Source, https://gitlab.com/gemseo/dev/gemseo-umdo
 Project-URL: Tracker, https://gitlab.com/gemseo/dev/gemseo-umdo/-/issues
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: <3.11,>=3.7
+Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 License-File: LICENSE.txt
 License-File: CREDITS.rst
 
 ..
     Copyright 2021 IRT Saint Exupéry, https://www.irt-saintexupery.com
```

### Comparing `gemseo-umdo-1.0.2/README.rst` & `gemseo-umdo-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `gemseo-umdo-1.0.2/doc_src/examples/udoe/quadratic/sampling.py` & `gemseo-umdo-1.1.0/doc_src/examples/udoe/quadratic/sampling.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 # WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 """
 Robust DOE - Sampling - Quadratic function
 ==========================================
 """
 from __future__ import annotations
 
+from gemseo import configure_logger
 from gemseo.algos.design_space import DesignSpace
 from gemseo.algos.parameter_space import ParameterSpace
-from gemseo.api import configure_logger
 from gemseo.disciplines.analytic import AnalyticDiscipline
 from gemseo_umdo.scenarios.udoe_scenario import UDOEScenario
 
 configure_logger()
 
 # %%
 # Firstly,
```

### Comparing `gemseo-umdo-1.0.2/doc_src/examples/umdo/quadratic/sampling.py` & `gemseo-umdo-1.1.0/doc_src/examples/umdo/quadratic/sampling.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 # WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 """
 Robust OPT - Sampling - Quadratic function
 ==========================================
 """
 from __future__ import annotations
 
+from gemseo import configure_logger
 from gemseo.algos.design_space import DesignSpace
 from gemseo.algos.parameter_space import ParameterSpace
-from gemseo.api import configure_logger
 from gemseo.disciplines.analytic import AnalyticDiscipline
 from gemseo_umdo.scenarios.umdo_scenario import UMDOScenario
 
 configure_logger()
 
 # %%
 # Firstly,
```

### Comparing `gemseo-umdo-1.0.2/doc_src/examples/umdo/rosenbrock/sampling.py` & `gemseo-umdo-1.1.0/doc_src/examples/umdo/rosenbrock/sampling.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 # WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 """
 Robust OPT - Sampling - Rosenbrock function
 ===========================================
 """
 from __future__ import annotations
 
+from gemseo import configure_logger
 from gemseo.algos.design_space import DesignSpace
 from gemseo.algos.parameter_space import ParameterSpace
-from gemseo.api import configure_logger
 from gemseo.disciplines.analytic import AnalyticDiscipline
 from gemseo_umdo.scenarios.umdo_scenario import UMDOScenario
 
 configure_logger()
 
 # %%
 # Firstly,
```

### Comparing `gemseo-umdo-1.0.2/doc_src/examples/umdo/sellar/deterministic.py` & `gemseo-umdo-1.1.0/doc_src/examples/umdo/sellar/deterministic.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 # WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 """
 OPT - Deterministic - Sellar problem
 ====================================
 """
 from __future__ import annotations
 
+from gemseo import configure_logger
 from gemseo.algos.design_space import DesignSpace
-from gemseo.api import configure_logger
 from gemseo.core.mdo_scenario import MDOScenario
 from gemseo.disciplines.analytic import AnalyticDiscipline
 
 configure_logger()
 
 # %%
 # Firstly,
```

### Comparing `gemseo-umdo-1.0.2/doc_src/examples/umdo/sellar/sampling.py` & `gemseo-umdo-1.1.0/doc_src/examples/umdo/sellar/sampling.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 # WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 """
 Robust OPT - Sampling - Sellar problem
 ======================================
 """
 from __future__ import annotations
 
+from gemseo import configure_logger
 from gemseo.algos.design_space import DesignSpace
 from gemseo.algos.parameter_space import ParameterSpace
-from gemseo.api import configure_logger
 from gemseo.disciplines.analytic import AnalyticDiscipline
 from gemseo_umdo.scenarios.umdo_scenario import UMDOScenario
 
 configure_logger()
 
 # %%
 # Firstly,
```

### Comparing `gemseo-umdo-1.0.2/doc_src/examples/umdo/sellar/sampling_with_repetitions.py` & `gemseo-umdo-1.1.0/doc_src/examples/umdo/sellar/sampling_with_repetitions.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 # WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 """
 Robust OPT - Sampling with repetitions - Sellar problem
 =======================================================
 """
 from __future__ import annotations
 
+from gemseo import configure_logger
 from gemseo.algos.design_space import DesignSpace
 from gemseo.algos.parameter_space import ParameterSpace
-from gemseo.api import configure_logger
 from gemseo.disciplines.analytic import AnalyticDiscipline
 from gemseo_umdo.scenarios.umdo_scenario import UMDOScenario
 from matplotlib import pyplot as plt
 from numpy import load
 from numpy import save
 from numpy import stack
 from numpy import vstack
@@ -89,15 +89,17 @@
             "n_samples": 100,
             "seed": i + 1,
         },
     )
     scenario.add_constraint("c1", "Margin", factor=3.0)
     scenario.add_constraint("c2", "Margin", factor=3.0)
     scenario.execute({"algo": "NLOPT_COBYLA", "max_iter": 100})
-    x_hist.append(vstack(scenario.formulation.opt_problem.database.get_x_history()))
+    x_hist.append(
+        vstack(scenario.formulation.opt_problem.database.get_x_vect_history())
+    )
 
 # %%
 # Lastly,
 # we plot the variability of the optimization history with boxplots:
 print(x_hist)
 x_hist = stack(x_hist)
 save("x_hist.npy", x_hist)
```

### Comparing `gemseo-umdo-1.0.2/doc_src/examples/umdo/sobieski/sampling.py` & `gemseo-umdo-1.1.0/doc_src/examples/umdo/sobieski/sampling.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 # WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 """
 Robust MDO - Sampling - Sobieski
 ================================
 """
 from __future__ import annotations
 
+from gemseo import configure_logger
 from gemseo.algos.parameter_space import ParameterSpace
-from gemseo.api import configure_logger
 from gemseo.problems.sobieski.core.problem import SobieskiProblem
 from gemseo.problems.sobieski.disciplines import SobieskiAerodynamics
 from gemseo.problems.sobieski.disciplines import SobieskiMission
 from gemseo.problems.sobieski.disciplines import SobieskiPropulsion
 from gemseo.problems.sobieski.disciplines import SobieskiStructure
 from gemseo_umdo.scenarios.umdo_scenario import UMDOScenario
```

### Comparing `gemseo-umdo-1.0.2/pyproject.toml` & `gemseo-umdo-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -15,8 +15,8 @@
 # logging settings identical to the defaults of gemseo.api.configure_logger()
 log_file_level = "INFO"
 log_file_date_format = "%H:%M:%S"
 log_file_format = "%(levelname)8s - %(asctime)s: %(message)s"
 # filterwarnings = ignore::pytest.PytestExperimentalApiWarning
 
 [tool.black]
-target-version = ['py37']
+target-version = ['py38']
```

### Comparing `gemseo-umdo-1.0.2/requirements/check.txt` & `gemseo-umdo-1.1.0/requirements/check.txt`

 * *Files 23% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 #
 #    pip-compile requirements/check.in
 #
 cfgv==3.3.1
     # via pre-commit
 distlib==0.3.6
     # via virtualenv
-filelock==3.9.0
+filelock==3.12.0
     # via virtualenv
-identify==2.5.13
+identify==2.5.24
     # via pre-commit
-nodeenv==1.7.0
+nodeenv==1.8.0
     # via pre-commit
-platformdirs==2.6.2
+platformdirs==3.5.1
     # via virtualenv
-pre-commit==2.21.0
+pre-commit==3.3.1
     # via -r requirements/check.in
 pyyaml==6.0
     # via pre-commit
-virtualenv==20.17.1
+virtualenv==20.23.0
     # via pre-commit
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `gemseo-umdo-1.0.2/requirements/doc.txt` & `gemseo-umdo-1.1.0/requirements/doc.txt`

 * *Files identical despite different names*

### Comparing `gemseo-umdo-1.0.2/requirements/test-python3.10.txt` & `gemseo-umdo-1.1.0/requirements/test-python3.9.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,159 +1,153 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --extra=test --output-file=requirements/test-python3.10.txt
+#    pip-compile --extra=test --output-file=requirements/test-python3.9.txt
 #
-attrs==22.2.0
-    # via pytest
-certifi==2022.12.7
+certifi==2023.5.7
     # via requests
-charset-normalizer==3.0.1
+charset-normalizer==3.1.0
     # via requests
 contourpy==1.0.7
     # via matplotlib
-covdefaults==2.2.2
+covdefaults==2.3.0
     # via gemseo-umdo (setup.py)
-coverage[toml]==7.1.0
+coverage[toml]==7.2.5
     # via
     #   covdefaults
     #   pytest-cov
 cycler==0.11.0
     # via matplotlib
 dill==0.3.6
     # via openturns
 docstring-inheritance==1.0.0
     # via gemseo
 et-xmlfile==1.1.0
     # via openpyxl
-exceptiongroup==1.1.0
+exceptiongroup==1.1.1
     # via pytest
 execnet==1.9.0
     # via pytest-xdist
-fastjsonschema==2.16.2
+fastjsonschema==2.16.3
     # via gemseo
-fonttools==4.38.0
+fonttools==4.39.4
     # via matplotlib
-gemseo[all]==4.3.0
+gemseo @ git+https://gitlab.com/gemseo/dev/gemseo.git@develop
     # via gemseo-umdo (setup.py)
 genson==1.2.2
     # via gemseo
 graphviz==0.20.1
     # via gemseo
-h5py==3.7.0
+h5py==3.8.0
     # via gemseo
 idna==3.4
     # via requests
+importlib-resources==5.12.0
+    # via matplotlib
 iniconfig==2.0.0
     # via pytest
 jinja2==3.1.2
     # via gemseo
 joblib==1.2.0
     # via scikit-learn
 kiwisolver==1.4.4
     # via matplotlib
 markupsafe==2.1.2
     # via jinja2
-matplotlib==3.6.2
+matplotlib==3.7.1
     # via
     #   gemseo
     #   gemseo-umdo (setup.py)
-mpmath==1.2.1
+mpmath==1.3.0
     # via sympy
-networkx==2.8.8
+networkx==3.1
     # via gemseo
 nlopt==2.7.1
     # via gemseo
-numpy==1.23.4
+numpy==1.24.3
     # via
     #   contourpy
     #   gemseo
     #   gemseo-umdo (setup.py)
     #   h5py
     #   matplotlib
     #   nlopt
     #   pandas
-    #   pdfo
     #   pydoe2
     #   pyxdsm
     #   scikit-learn
     #   scipy
-openpyxl==3.0.10
+openpyxl==3.1.2
     # via gemseo
 openturns==1.20.post3
     # via gemseo
-packaging==21.3
+packaging==23.1
     # via
     #   gemseo
     #   matplotlib
     #   pytest
-pandas==1.5.1
-    # via gemseo
-pdfo==1.2
+pandas==2.0.0
     # via gemseo
-pillow==9.4.0
+pillow==9.5.0
     # via matplotlib
 pluggy==1.0.0
     # via pytest
-psutil==5.9.4
+psutil==5.9.5
     # via openturns
 pydoe2==1.3.0
     # via gemseo
 pyparsing==3.0.9
-    # via
-    #   matplotlib
-    #   packaging
-pyside6==6.3.1
-    # via gemseo
-pyside6-addons==6.3.1
-    # via pyside6
-pyside6-essentials==6.3.1
-    # via pyside6
-pytest==7.2.1
+    # via matplotlib
+pytest==7.3.1
     # via
     #   gemseo-umdo (setup.py)
     #   pytest-cov
     #   pytest-xdist
 pytest-cov==4.0.0
     # via gemseo-umdo (setup.py)
-pytest-xdist==3.2.0
+pytest-xdist==3.3.0
     # via gemseo-umdo (setup.py)
 python-dateutil==2.8.2
     # via
     #   matplotlib
     #   pandas
-pytz==2022.7.1
+pytz==2023.3
     # via pandas
 pyxdsm==2.2.2
     # via gemseo
-requests==2.28.2
+requests==2.30.0
     # via gemseo
-scikit-learn==1.1.3
+scikit-learn==1.2.2
     # via gemseo
-scipy==1.9.1
+scipy==1.10.1
     # via
     #   gemseo
+    #   gemseo-umdo (setup.py)
     #   pydoe2
     #   scikit-learn
-shiboken6==6.3.1
-    # via pyside6
 six==1.16.0
     # via python-dateutil
+strenum==0.4.10
+    # via gemseo
 sympy==1.11.1
     # via gemseo
 threadpoolctl==3.1.0
     # via scikit-learn
 tomli==2.0.1
     # via
     #   coverage
     #   pytest
-tqdm==4.64.1
+tqdm==4.65.0
     # via gemseo
-typing-extensions==4.4.0
+typing-extensions==4.5.0
     # via gemseo
-urllib3==1.26.14
+tzdata==2023.3
+    # via pandas
+urllib3==2.0.2
     # via requests
-xdsmjs==1.0.1
+xdsmjs==2.0.0
     # via gemseo
-xxhash==3.1.0
+xxhash==3.2.0
     # via gemseo
+zipp==3.15.0
+    # via importlib-resources
```

### Comparing `gemseo-umdo-1.0.2/requirements/test-python3.7.txt` & `gemseo-umdo-1.1.0/requirements/test-python3.10.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,168 +1,149 @@
 #
-# This file is autogenerated by pip-compile with Python 3.7
+# This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --extra=test --output-file=requirements/test-python3.7.txt
+#    pip-compile --extra=test --output-file=requirements/test-python3.10.txt
 #
-attrs==22.2.0
-    # via pytest
-certifi==2022.12.7
+certifi==2023.5.7
     # via requests
-charset-normalizer==3.0.1
+charset-normalizer==3.1.0
     # via requests
-covdefaults==2.2.2
+contourpy==1.0.7
+    # via matplotlib
+covdefaults==2.3.0
     # via gemseo-umdo (setup.py)
-coverage[toml]==7.1.0
+coverage[toml]==7.2.5
     # via
     #   covdefaults
     #   pytest-cov
 cycler==0.11.0
     # via matplotlib
 dill==0.3.6
     # via openturns
 docstring-inheritance==1.0.0
     # via gemseo
 et-xmlfile==1.1.0
     # via openpyxl
-exceptiongroup==1.1.0
+exceptiongroup==1.1.1
     # via pytest
 execnet==1.9.0
     # via pytest-xdist
-fastjsonschema==2.16.2
+fastjsonschema==2.16.3
     # via gemseo
-fonttools==4.38.0
+fonttools==4.39.4
     # via matplotlib
-gemseo[all]==4.3.0
+gemseo @ git+https://gitlab.com/gemseo/dev/gemseo.git@develop
     # via gemseo-umdo (setup.py)
 genson==1.2.2
     # via gemseo
 graphviz==0.20.1
     # via gemseo
-h5py==3.7.0
+h5py==3.8.0
     # via gemseo
 idna==3.4
     # via requests
-importlib-metadata==4.13.0
-    # via
-    #   gemseo
-    #   pluggy
-    #   pytest
 iniconfig==2.0.0
     # via pytest
 jinja2==3.1.2
     # via gemseo
 joblib==1.2.0
     # via scikit-learn
 kiwisolver==1.4.4
     # via matplotlib
 markupsafe==2.1.2
     # via jinja2
-matplotlib==3.5.3
+matplotlib==3.7.1
     # via
     #   gemseo
     #   gemseo-umdo (setup.py)
-mpmath==1.2.1
+mpmath==1.3.0
     # via sympy
-networkx==2.6.3
+networkx==3.1
     # via gemseo
 nlopt==2.7.1
     # via gemseo
-numpy==1.21.6
+numpy==1.24.3
     # via
+    #   contourpy
     #   gemseo
     #   gemseo-umdo (setup.py)
     #   h5py
     #   matplotlib
     #   nlopt
     #   pandas
-    #   pdfo
     #   pydoe2
     #   pyxdsm
     #   scikit-learn
     #   scipy
-openpyxl==3.0.10
+openpyxl==3.1.2
     # via gemseo
-openturns==1.19
+openturns==1.20.post3
     # via gemseo
-packaging==21.3
+packaging==23.1
     # via
     #   gemseo
     #   matplotlib
     #   pytest
-pandas==1.3.5
+pandas==2.0.0
     # via gemseo
-pdfo==1.2
-    # via gemseo
-pillow==9.4.0
+pillow==9.5.0
     # via matplotlib
 pluggy==1.0.0
     # via pytest
-psutil==5.9.4
+psutil==5.9.5
     # via openturns
 pydoe2==1.3.0
     # via gemseo
 pyparsing==3.0.9
-    # via
-    #   matplotlib
-    #   packaging
-pyside6==6.3.1
-    # via gemseo
-pyside6-addons==6.3.1
-    # via pyside6
-pyside6-essentials==6.3.1
-    # via pyside6
-pytest==7.2.1
+    # via matplotlib
+pytest==7.3.1
     # via
     #   gemseo-umdo (setup.py)
     #   pytest-cov
     #   pytest-xdist
 pytest-cov==4.0.0
     # via gemseo-umdo (setup.py)
-pytest-xdist==3.2.0
+pytest-xdist==3.3.0
     # via gemseo-umdo (setup.py)
 python-dateutil==2.8.2
     # via
     #   matplotlib
     #   pandas
-pytz==2022.7.1
+pytz==2023.3
     # via pandas
 pyxdsm==2.2.2
     # via gemseo
-requests==2.28.2
+requests==2.30.0
     # via gemseo
-scikit-learn==1.0.2
+scikit-learn==1.2.2
     # via gemseo
-scipy==1.7.3
+scipy==1.10.1
     # via
     #   gemseo
+    #   gemseo-umdo (setup.py)
     #   pydoe2
     #   scikit-learn
-shiboken6==6.3.1
-    # via pyside6
-singledispatchmethod==1.0
-    # via gemseo
 six==1.16.0
     # via python-dateutil
-sympy==1.10.1
+strenum==0.4.10
+    # via gemseo
+sympy==1.11.1
     # via gemseo
 threadpoolctl==3.1.0
     # via scikit-learn
 tomli==2.0.1
     # via
     #   coverage
     #   pytest
-tqdm==4.64.1
+tqdm==4.65.0
     # via gemseo
-typing-extensions==4.4.0
-    # via
-    #   gemseo
-    #   importlib-metadata
-    #   kiwisolver
-urllib3==1.26.14
+typing-extensions==4.5.0
+    # via gemseo
+tzdata==2023.3
+    # via pandas
+urllib3==2.0.2
     # via requests
-xdsmjs==1.0.1
+xdsmjs==2.0.0
     # via gemseo
-xxhash==3.1.0
+xxhash==3.2.0
     # via gemseo
-zipp==3.12.1
-    # via importlib-metadata
```

### Comparing `gemseo-umdo-1.0.2/requirements/test-python3.8.txt` & `gemseo-umdo-1.1.0/requirements/test-python3.8.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,159 +1,153 @@
 #
 # This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
 #    pip-compile --extra=test --output-file=requirements/test-python3.8.txt
 #
-attrs==22.2.0
-    # via pytest
-certifi==2022.12.7
+certifi==2023.5.7
     # via requests
-charset-normalizer==3.0.1
+charset-normalizer==3.1.0
     # via requests
 contourpy==1.0.7
     # via matplotlib
-covdefaults==2.2.2
+covdefaults==2.3.0
     # via gemseo-umdo (setup.py)
-coverage[toml]==7.1.0
+coverage[toml]==7.2.5
     # via
     #   covdefaults
     #   pytest-cov
 cycler==0.11.0
     # via matplotlib
 dill==0.3.6
     # via openturns
 docstring-inheritance==1.0.0
     # via gemseo
 et-xmlfile==1.1.0
     # via openpyxl
-exceptiongroup==1.1.0
+exceptiongroup==1.1.1
     # via pytest
 execnet==1.9.0
     # via pytest-xdist
-fastjsonschema==2.16.2
+fastjsonschema==2.16.3
     # via gemseo
-fonttools==4.38.0
+fonttools==4.39.4
     # via matplotlib
-gemseo[all]==4.3.0
+gemseo @ git+https://gitlab.com/gemseo/dev/gemseo.git@develop
     # via gemseo-umdo (setup.py)
 genson==1.2.2
     # via gemseo
 graphviz==0.20.1
     # via gemseo
-h5py==3.7.0
+h5py==3.8.0
     # via gemseo
 idna==3.4
     # via requests
+importlib-resources==5.12.0
+    # via matplotlib
 iniconfig==2.0.0
     # via pytest
 jinja2==3.1.2
     # via gemseo
 joblib==1.2.0
     # via scikit-learn
 kiwisolver==1.4.4
     # via matplotlib
 markupsafe==2.1.2
     # via jinja2
-matplotlib==3.6.2
+matplotlib==3.7.1
     # via
     #   gemseo
     #   gemseo-umdo (setup.py)
-mpmath==1.2.1
+mpmath==1.3.0
     # via sympy
-networkx==2.8.8
+networkx==3.1
     # via gemseo
 nlopt==2.7.1
     # via gemseo
-numpy==1.23.4
+numpy==1.24.3
     # via
     #   contourpy
     #   gemseo
     #   gemseo-umdo (setup.py)
     #   h5py
     #   matplotlib
     #   nlopt
     #   pandas
-    #   pdfo
     #   pydoe2
     #   pyxdsm
     #   scikit-learn
     #   scipy
-openpyxl==3.0.10
+openpyxl==3.1.2
     # via gemseo
 openturns==1.20.post3
     # via gemseo
-packaging==21.3
+packaging==23.1
     # via
     #   gemseo
     #   matplotlib
     #   pytest
-pandas==1.5.1
-    # via gemseo
-pdfo==1.2
+pandas==2.0.0
     # via gemseo
-pillow==9.4.0
+pillow==9.5.0
     # via matplotlib
 pluggy==1.0.0
     # via pytest
-psutil==5.9.4
+psutil==5.9.5
     # via openturns
 pydoe2==1.3.0
     # via gemseo
 pyparsing==3.0.9
-    # via
-    #   matplotlib
-    #   packaging
-pyside6==6.3.1
-    # via gemseo
-pyside6-addons==6.3.1
-    # via pyside6
-pyside6-essentials==6.3.1
-    # via pyside6
-pytest==7.2.1
+    # via matplotlib
+pytest==7.3.1
     # via
     #   gemseo-umdo (setup.py)
     #   pytest-cov
     #   pytest-xdist
 pytest-cov==4.0.0
     # via gemseo-umdo (setup.py)
-pytest-xdist==3.2.0
+pytest-xdist==3.3.0
     # via gemseo-umdo (setup.py)
 python-dateutil==2.8.2
     # via
     #   matplotlib
     #   pandas
-pytz==2022.7.1
+pytz==2023.3
     # via pandas
 pyxdsm==2.2.2
     # via gemseo
-requests==2.28.2
+requests==2.30.0
     # via gemseo
-scikit-learn==1.1.3
+scikit-learn==1.2.2
     # via gemseo
-scipy==1.9.1
+scipy==1.10.1
     # via
     #   gemseo
+    #   gemseo-umdo (setup.py)
     #   pydoe2
     #   scikit-learn
-shiboken6==6.3.1
-    # via pyside6
 six==1.16.0
     # via python-dateutil
+strenum==0.4.10
+    # via gemseo
 sympy==1.11.1
     # via gemseo
 threadpoolctl==3.1.0
     # via scikit-learn
 tomli==2.0.1
     # via
     #   coverage
     #   pytest
-tqdm==4.64.1
+tqdm==4.65.0
     # via gemseo
-typing-extensions==4.4.0
+typing-extensions==4.5.0
     # via gemseo
-urllib3==1.26.14
+tzdata==2023.3
+    # via pandas
+urllib3==2.0.2
     # via requests
-xdsmjs==1.0.1
+xdsmjs==2.0.0
     # via gemseo
-xxhash==3.1.0
+xxhash==3.2.0
     # via gemseo
+zipp==3.15.0
+    # via importlib-resources
```

### Comparing `gemseo-umdo-1.0.2/setup.cfg` & `gemseo-umdo-1.1.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -17,29 +17,29 @@
 	License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 	Intended Audience :: Science/Research
 	Topic :: Scientific/Engineering
 	Operating System :: POSIX :: Linux
 	Operating System :: MacOS
 	Operating System :: Microsoft :: Windows
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 
 [options]
 package_dir = 
 	=src
 packages = find:
 include_package_data = true
-python_requires = >=3.7, <3.11
+python_requires = >=3.8, <3.11
 install_requires = 
-	gemseo[all] >=4.1.0
+	gemseo[all] >=5
 	matplotlib
 	numpy
+	scipy
 
 [options.packages.find]
 where = src
 
 [options.extras_require]
 test = 
 	covdefaults
@@ -63,18 +63,21 @@
 
 [flake8]
 ignore = 
 	E501
 	D105
 	E203
 	W503
-select = B,C,D,E,F,G,N,T,W,B950
+	ANN101
+	ANN102
+	ANN401
+select = ANN,B,C,D,E,F,G,N,T,W,B950
 max-line-length = 88
 docstring-convention = google
 per-file-ignores = 
-	tests/*.py:D100,D104,D417
-	doc_src/*.py:D,T001,T201
+	tests/*.py: D100,D104,ANN
+	doc_src/*.py: D,T201
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `gemseo-umdo-1.0.2/setup.py` & `gemseo-umdo-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `gemseo-umdo-1.0.2/src/gemseo_umdo/__init__.py` & `gemseo-umdo-1.1.0/src/gemseo_umdo/__init__.py`

 * *Files identical despite different names*

### Comparing `gemseo-umdo-1.0.2/src/gemseo_umdo/estimators/__init__.py` & `gemseo-umdo-1.1.0/src/gemseo_umdo/estimators/__init__.py`

 * *Files identical despite different names*

### Comparing `gemseo-umdo-1.0.2/src/gemseo_umdo/estimators/estimator.py` & `gemseo-umdo-1.1.0/src/gemseo_umdo/estimators/estimator.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,60 +11,57 @@
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 """Base estimator of statistic associated with a U-MDO formulation."""
 from __future__ import annotations
 
+from abc import ABC
 from abc import abstractmethod
 from typing import Any
 from typing import TYPE_CHECKING
 
-from gemseo.core.factory import Factory
+from gemseo.core.base_factory import BaseFactory
 from numpy import ndarray
 
 if TYPE_CHECKING:
     from gemseo_umdo.formulations.formulation import UMDOFormulation
 
 
-class BaseStatisticEstimator:
+class BaseStatisticEstimator(ABC):
     """The base estimator of statistics associated with a U-MDO formulation."""
 
     _formulation: UMDOFormulation
     """The U-MDO formulation."""
 
     def __init__(self, formulation: UMDOFormulation) -> None:
-        """# noqa: D205 D212 D415
+        """
         Args:
             formulation: The U-MDO formulation.
-        """
+        """  # noqa: D205 D212 D415
         self._formulation = formulation
 
     @abstractmethod
     def __call__(self, *args: Any, **kwargs: Any) -> float | ndarray:  # noqa: D102
         ...
 
 
-class BaseStatisticEstimatorFactory(Factory):
+class BaseStatisticEstimatorFactory(BaseFactory):
     """The factory of :class:`.BaseStatisticEstimator`."""
 
-    def __init__(self, cls: type = BaseStatisticEstimator) -> None:
-        """# noqa: D205 D212 D415
-        Args:
-            cls: The class of statistic estimators.
-        """
-        super().__init__(cls, ("gemseo_umdo.estimators",))
+    _CLASS = BaseStatisticEstimator
+    _MODULE_NAMES = ("gemseo_umdo.estimators",)
 
     def create(
         self,
         name: str,
         formulation: UMDOFormulation,
         **options: Any,
     ) -> BaseStatisticEstimator:
         """Create a statistic estimator.
 
         Args:
             name: The class name of the statistic estimator.
             formulation: The U-MDO formulation.
             **options: The options of the statistic estimator.
         """
-        return self.factory.create(name, formulation=formulation, **options)
+        return self.create(name, formulation=formulation, **options)
```

### Comparing `gemseo-umdo-1.0.2/src/gemseo_umdo/estimators/sampling.py` & `gemseo-umdo-1.1.0/src/gemseo_umdo/estimators/sampling.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 """Estimators of statistic for sampling-based U-MDO formulation."""
 from __future__ import annotations
 
 from typing import Any
 from typing import TYPE_CHECKING
 
-from gemseo.core.factory import Factory
+from gemseo.core.base_factory import BaseFactory
 
 if TYPE_CHECKING:
     from gemseo_umdo.formulations.sampling import Sampling
 
 from numpy import ndarray
 
 from gemseo_umdo.estimators.estimator import BaseStatisticEstimator
@@ -31,76 +31,76 @@
 class SamplingEstimator(BaseStatisticEstimator):
     """Base statistic estimator for a U-MDO formulation using sampling."""
 
     def __init__(self, formulation: Sampling) -> None:  # noqa: D107
         super().__init__(formulation)
 
 
-class SamplingEstimatorFactory(Factory):
+class SamplingEstimatorFactory(BaseFactory):
     """The factory of :class:`.SamplingEstimator`."""
 
-    def __init__(self) -> None:  # noqa: D107
-        super().__init__(SamplingEstimator)
+    _CLASS = SamplingEstimator
+    _MODULE_NAMES = ()
 
 
 class Mean(SamplingEstimator):
     """Estimator of the expectation, a.k.a.
 
     mean.
     """
 
     def __call__(self, samples: ndarray, **kwargs: Any) -> float | ndarray:
-        """# noqa: D205 D212 D415
+        """
         Args:
             samples: The output evaluations arranged in rows.
-        """
+        """  # noqa: D205 D212 D415
         return samples.mean(0)
 
 
 class Variance(SamplingEstimator):
     """Estimator of the variance."""
 
-    def __call__(self, samples: ndarray, **kwargs) -> float | ndarray:
-        """# noqa: D205 D212 D415
+    def __call__(self, samples: ndarray, **kwargs: Any) -> float | ndarray:
+        """
         Args:
             samples: The output evaluations arranged in rows.
-        """
+        """  # noqa: D205 D212 D415
         return samples.var(0)
 
 
 class Probability(SamplingEstimator):
     """Estimator of a probability."""
 
     def __call__(
         self,
         samples: ndarray,
         threshold: float,
         greater: bool = True,
         **kwargs: Any,
     ) -> float | ndarray:
-        """# noqa: D205 D212 D415
+        """
         Args:
             samples: The output evaluations arranged in rows.
             threshold: The threshold against which the probability is estimated.
             greater: Whether to compute the probability of exceeding the threshold.
-        """
+        """  # noqa: D205 D212 D415
         if greater:
             return (samples >= threshold).mean(0)
         else:
             return (samples <= threshold).mean(0)
 
 
 class StandardDeviation(Variance):
     """Estimator of the standard deviation."""
 
-    def __call__(self, samples: ndarray, **kwargs) -> float | ndarray:
-        """# noqa: D205 D212 D415
+    def __call__(self, samples: ndarray, **kwargs: Any) -> float | ndarray:
+        """
         Args:
             samples: The output evaluations arranged in rows.
-        """
+        """  # noqa: D205 D212 D415
         return super().__call__(samples, **kwargs) ** 0.5
 
 
 class Margin(SamplingEstimator):
     """Estimator of a margin, i.e. mean + factor * deviation."""
 
     def __init__(self, formulation: Sampling) -> None:  # noqa: D107
@@ -108,17 +108,17 @@
         self.__mean = Mean(formulation)
         self.__standard_deviation = StandardDeviation(formulation)
 
     def __call__(
         self,
         samples: ndarray,
         factor: float = 2.0,
-        **kwargs,
+        **kwargs: Any,
     ) -> float | ndarray:
-        """# noqa: D205 D212 D415
+        """
         Args:
             samples: The output evaluations arranged in rows.
             factor: The factor related to the standard deviation.
-        """
+        """  # noqa: D205 D212 D415
         return self.__mean(samples, **kwargs) + factor * self.__standard_deviation(
             samples, **kwargs
         )
```

### Comparing `gemseo-umdo-1.0.2/src/gemseo_umdo/formulations/__init__.py` & `gemseo-umdo-1.1.0/src/gemseo_umdo/formulations/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 an objective and constraints.
 The objective can be either minimized (default) or maximized.
 
 In the context of deterministic MDO,
 the :class:`~gemseo.algos.opt_problem.OptimizationProblem`
 is handled by a driver (see :class:`~gemseo.algos.driver_lib.DriverLib`),
 typically an optimizer (see :class:`~gemseo.algos.opt.opt_lib.OptimizationLibrary`),
-or a design of experiments (DOE, see :class:`~gemseo.algos.doe.doe_lib.DOELibrary`).
+or a design of experiments (DOE, see :class:`~gemseo.algos.doe.doe_library.DOELibrary`).
 
 In the frame of robust MDO,
 the :class:`~gemseo_umdo.formulations.formulation.UMDOFormulation`
 uses a :class:`~gemseo.core.formulation.MDOFormulation`
 with a :class:`~gemseo.algos.parameter_space.ParameterSpace`
 defining the uncertain variables
 and executes the corresponding :class:`~gemseo.algos.opt_problem.OptimizationProblem`
```

### Comparing `gemseo-umdo-1.0.2/src/gemseo_umdo/formulations/factory.py` & `gemseo-umdo-1.1.0/src/gemseo_umdo/formulations/factory.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,19 +11,17 @@
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 """Formulate a multidisciplinary design problem under uncertainty."""
 from __future__ import annotations
 
-from gemseo.core.factory import Factory
 from gemseo.formulations.formulations_factory import MDOFormulationsFactory
 
 from gemseo_umdo.formulations.formulation import UMDOFormulation
 
 
 class UMDOFormulationsFactory(MDOFormulationsFactory):
     """The factory of :class:`.UMDOFormulation`."""
 
-    def __init__(self) -> None:  # noqa: D107
-        super().__init__()
-        self.factory = Factory(UMDOFormulation, ("gemseo_umdo.formulations",))
+    _CLASS = UMDOFormulation
+    _MODULE_NAMES = ("gemseo_umdo.formulations",)
```

### Comparing `gemseo-umdo-1.0.2/src/gemseo_umdo/formulations/formulation.py` & `gemseo-umdo-1.1.0/src/gemseo_umdo/formulations/formulation.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from typing import ClassVar
 from typing import Iterable
 from typing import Mapping
 from typing import Sequence
 
 from gemseo.algos.design_space import DesignSpace
 from gemseo.algos.parameter_space import ParameterSpace
+from gemseo.core.base_factory import BaseFactory
 from gemseo.core.base_formulation import BaseFormulation
 from gemseo.core.discipline import MDODiscipline
 from gemseo.core.execution_sequence import ExecutionSequence
 from gemseo.core.formulation import MDOFormulation
 from gemseo.core.mdofunctions.mdo_function import MDOFunction
 from gemseo.uncertainty.statistics.statistics import Statistics
 from gemseo.utils.data_conversion import split_array_to_dict_of_arrays
@@ -43,41 +44,41 @@
 
 class UMDOFormulation(BaseFormulation):
     """Base formulation of a multidisciplinary design problem under uncertainty."""
 
     _processed_functions: list[str]
     """The names of the functions whose statistics have been estimated."""
 
-    _STATISTIC_FACTORY: ClassVar = BaseStatisticEstimatorFactory()
+    _STATISTIC_FACTORY: ClassVar[BaseFactory] = BaseStatisticEstimatorFactory()
 
     def __init__(
         self,
         disciplines: Sequence[MDODiscipline],
         objective_name: str,
         design_space: DesignSpace,
         mdo_formulation: MDOFormulation,
         uncertain_space: ParameterSpace,
         objective_statistic_name: str,
         objective_statistic_parameters: Mapping[str, Any] | None = None,
         maximize_objective: bool = False,
-        grammar_type: str = MDODiscipline.JSON_GRAMMAR_TYPE,
+        grammar_type: MDODiscipline.GrammarType = MDODiscipline.GrammarType.JSON,
         **options: Any,
     ) -> None:
-        """# noqa: D205 D212 D415
+        """
         Args:
             mdo_formulation: The class name of the MDO formulation, e.g. "MDF".
             uncertain_space: The uncertain variables
                 with their probability distributions.
             objective_statistic_name: The name of the statistic
                 to be applied to the objective.
             objective_statistic_parameters: The values of the parameters
                 of the statistic to be applied to the objective, if any.
-        """
-        design_variables = ", ".join(design_space.variables_names)
-        uncertain_variables = ", ".join(uncertain_space.variables_names)
+        """  # noqa: D205 D212 D415
+        design_variables = ", ".join(design_space.variable_names)
+        uncertain_variables = ", ".join(uncertain_space.variable_names)
         self.__signature = f"({design_variables}; {uncertain_variables})"
         if objective_statistic_parameters is None:
             objective_statistic_parameters = {}
 
         objective_expression, objective_name = self.__compute_name(
             objective_name,
             objective_statistic_name,
@@ -89,19 +90,19 @@
             disciplines,
             objective_name,
             design_space,
             maximize_objective=maximize_objective,
             grammar_type=grammar_type,
             **options,
         )
-        self.__available_statistics = self._STATISTIC_FACTORY.classes
+        self.__available_statistics = self._STATISTIC_FACTORY.class_names
         self.opt_problem.objective = self._StatisticFunction(
             self,
             self._mdo_formulation.opt_problem.objective,
-            MDOFunction.TYPE_OBJ,
+            MDOFunction.FunctionType.OBJ,
             objective_statistic_name,
             **objective_statistic_parameters,
         )
         if self._maximize_objective:
             objective_name = f"-{objective_name}"
             self.opt_problem.minimize_objective = False
 
@@ -129,20 +130,20 @@
         self,
         output_names: Sequence[str],
         statistic_name: str,
         observable_name: Sequence[str] | None = None,
         discipline: MDODiscipline | None = None,
         **statistic_parameters: Any,
     ) -> None:
-        """# noqa: D205 D212 D415
+        """
         Args:
             statistic_name: The name of the statistic to be applied to the observable.
             statistic_parameters: The values of the parameters
                 of the statistic to be applied to the observable, if any.
-        """
+        """  # noqa: D205 D212 D415
         self._mdo_formulation.add_observable(
             output_names,
             observable_name=observable_name,
             discipline=discipline,
         )
         observable = self._StatisticFunction(
             self,
@@ -157,26 +158,26 @@
         self.opt_problem.add_observable(observable)
         self._post_add_observable()
 
     def add_constraint(
         self,
         output_name: str | Sequence[str],
         statistic_name: str,
-        constraint_type: str = MDOFunction.TYPE_INEQ,
+        constraint_type: str = MDOFunction.ConstraintType.INEQ,
         constraint_name: str | None = None,
         value: float | None = None,
         positive: bool = False,
-        **statistic_parameters,
+        **statistic_parameters: Any,
     ) -> None:
-        """# noqa: D205 D212 D415
+        """
         Args:
             statistic_name: The name of the statistic to be applied to the constraint.
             statistic_parameters: The values of the parameters of the statistic
                 to be applied to the constraint, if any.
-        """
+        """  # noqa: D205 D212 D415
         self._mdo_formulation.add_constraint(
             output_name,
             constraint_name=constraint_name,
         )
         constraint = self._StatisticFunction(
             self,
             self._mdo_formulation.opt_problem.constraints[-1],
@@ -191,18 +192,18 @@
             constraint,
             value=value,
             positive=positive,
             cstr_type=constraint_type,
         )
         self._post_add_constraint()
 
-    def _post_add_constraint(self):
+    def _post_add_constraint(self) -> None:
         """Apply actions after adding a constraint."""
 
-    def _post_add_observable(self):
+    def _post_add_observable(self) -> None:
         """Apply actions after adding an observable."""
 
     def __compute_name(
         self,
         output_name: str | Iterable[str],
         statistic_name: str,
         **statistic_parameters: Any,
@@ -228,28 +229,34 @@
             f"{output_name}{self.__signature}", statistic_name, **statistic_parameters
         )
         name = Statistics.compute_expression(
             output_name, statistic_name, **statistic_parameters
         )
         return name_with_signature, name
 
-    def update_top_level_disciplines(self, design_values: ndarray) -> None:
+    def update_top_level_disciplines(self, design_values: Mapping[str, Any]) -> None:
         """Update the default input values of the top-level disciplines.
 
         Args:
             design_values: The values of the design variables
                 to update the default input values of the top-level disciplines.
         """
         design_values = split_array_to_dict_of_arrays(
             design_values,
-            self.design_space.variables_sizes,
-            self.design_space.variables_names,
+            self.design_space.variable_sizes,
+            self.design_space.variable_names,
         )
         for discipline in self._mdo_formulation.get_top_level_disc():
-            discipline.default_inputs.update(design_values)
+            discipline.default_inputs.update(
+                {
+                    k: v
+                    for k, v in design_values.items()
+                    if k in discipline.input_grammar
+                }
+            )
 
     def get_top_level_disc(self) -> list[MDODiscipline]:  # noqa: D102
         return self._mdo_formulation.get_top_level_disc()
 
     def get_expected_workflow(  # noqa: D102
         self,
     ) -> list[ExecutionSequence, tuple[ExecutionSequence]]:
@@ -279,22 +286,22 @@
             self,
             formulation: UMDOFormulation,
             func: MDOFunction,
             function_type: str,
             name: str,
             **parameters: Any,
         ) -> None:
-            """# noqa: D205 D212 D415
+            """
             Args:
                 formulation: The U-MDO formulation.
                 func: The function for which to calculate the statistic.
                 function_type: The type of function.
                 name: The name of the statistic.
                 **parameters: The parameters of the statistic.
-            """
+            """  # noqa: D205 D212 D415
             self._estimate_statistic = formulation._STATISTIC_FACTORY.create(
                 name, formulation=formulation
             )
             self._function_name = func.name
             self._formulation = formulation
             self._statistic_parameters = parameters
             super().__init__(self._func, name=func.name, f_type=function_type)
```

### Comparing `gemseo-umdo-1.0.2/src/gemseo_umdo/formulations/sampling.py` & `gemseo-umdo-1.1.0/src/gemseo_umdo/formulations/sampling.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 from typing import Any
 from typing import ClassVar
 from typing import Mapping
 from typing import Sequence
 
 from gemseo.algos.design_space import DesignSpace
 from gemseo.algos.doe.doe_factory import DOEFactory
-from gemseo.algos.doe.doe_lib import DOELibrary
+from gemseo.algos.doe.doe_library import DOELibrary
 from gemseo.algos.opt_problem import OptimizationProblem
 from gemseo.algos.parameter_space import ParameterSpace
 from gemseo.core.discipline import MDODiscipline
 from gemseo.core.formulation import MDOFormulation
 from gemseo.utils.logging_tools import LoggingContext
 from numpy import ndarray
 
@@ -65,26 +65,26 @@
         design_space: DesignSpace,
         mdo_formulation: MDOFormulation,
         uncertain_space: ParameterSpace,
         objective_statistic_name: str,
         n_samples: int,
         objective_statistic_parameters: Mapping[str, Any] | None = None,
         maximize_objective: bool = False,
-        grammar_type: str = MDODiscipline.JSON_GRAMMAR_TYPE,
+        grammar_type: MDODiscipline.GrammarType = MDODiscipline.GrammarType.JSON,
         algo: str = "OT_OPT_LHS",
         algo_options: Mapping[str, Any] | None = None,
         seed: int = 1,
         **options: Any,
     ) -> None:
-        """# noqa: D205 D212 D415
+        """
         Args:
             n_samples: The number of samples, i.e. the size of the DOE.
             algo: The name of the DOE algorithm.
             algo_options: The options of the DOE algorithm.
-        """
+        """  # noqa: D205 D212 D415
         self.__doe_algo = DOEFactory().create(algo)
         self.__doe_algo_options = algo_options or {}
         self.__doe_algo_options["n_samples"] = n_samples
         self.__n_samples = n_samples
         self.processed_functions = []
         self.__seed = seed
         super().__init__(
@@ -140,10 +140,10 @@
             database = problem.database
             if not database:
                 formulation.update_top_level_disciplines(input_data)
                 formulation.compute_samples(problem)
 
             formulation._processed_functions.append(self._function_name)
             samples, _, _ = database.get_history_array(
-                [self._function_name], add_dv=False
+                [self._function_name], with_x_vect=False
             )
             return self._estimate_statistic(samples, **self._statistic_parameters)
```

### Comparing `gemseo-umdo-1.0.2/src/gemseo_umdo/scenarios/__init__.py` & `gemseo-umdo-1.1.0/src/gemseo_umdo/scenarios/__init__.py`

 * *Files identical despite different names*

### Comparing `gemseo-umdo-1.0.2/src/gemseo_umdo/scenarios/_scenario.py` & `gemseo-umdo-1.1.0/src/gemseo_umdo/scenarios/_scenario.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,26 +13,26 @@
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 """Scenarios to address multidisciplinary design problems under uncertainty."""
 from __future__ import annotations
 
 import logging
 from typing import Any
+from typing import Final
 from typing import Mapping
 from typing import Sequence
 
 from gemseo.algos.design_space import DesignSpace
 from gemseo.algos.parameter_space import ParameterSpace
 from gemseo.core.discipline import MDODiscipline
 from gemseo.core.formulation import MDOFormulation
 from gemseo.core.mdofunctions.mdo_function import MDOFunction
 from gemseo.core.scenario import Scenario
 from gemseo.disciplines.analytic import AnalyticDiscipline
 from gemseo.formulations.formulations_factory import MDOFormulationsFactory
-from gemseo.utils.python_compatibility import Final
 
 from gemseo_umdo.formulations.factory import UMDOFormulationsFactory
 
 LOGGER = logging.getLogger(__name__)
 
 
 class _UScenario(Scenario):
@@ -51,18 +51,18 @@
         uncertain_space: ParameterSpace,
         objective_statistic_name: str,
         objective_statistic_parameters: Mapping[str, Any] | None = None,
         statistic_estimation: str = "Sampling",
         statistic_estimation_parameters: Mapping[str, Any] | None = None,
         uncertain_design_variables: Mapping[str, str] | None = None,
         name: str | None = None,
-        grammar_type: str = MDODiscipline.JSON_GRAMMAR_TYPE,
+        grammar_type: MDODiscipline.GrammarType = MDODiscipline.GrammarType.JSON,
         **formulation_options: Any,
     ) -> None:
-        """# noqa: D205 D212 D415
+        """
         Args:
             uncertain_space: The uncertain variables
                 with their probability distributions.
             objective_statistic_name: The name of the statistic
                 to be applied to the objective, e.g. "margin".
             objective_statistic_parameters: The parameters of the statistics
                 to be applied to the objective,
@@ -77,15 +77,15 @@
                 ``"u"`` is the name of the uncertain variable
                 defined in the ``uncertain_space``
                 and ``"{}"`` is the optimization variable.
                 Leave ``"{}"`` as is; it will be automatically replaced by ``"dv_x"``.
                 If ``None``,
                 do not consider other variable relations
                 than those defined by ``disciplines``.
-        """
+        """  # noqa: D205 D212 D415
         all_disciplines = [discipline for discipline in disciplines]
 
         if statistic_estimation_parameters is None:
             statistic_estimation_parameters = {}
 
         maximize_objective = formulation_options.get(self.__MAXIMIZE_OBJECTIVE)
         if maximize_objective is not None:
@@ -142,32 +142,35 @@
     def _formulation_factory(self) -> UMDOFormulationsFactory:
         return UMDOFormulationsFactory()
 
     def add_constraint(
         self,
         output_name: str | Sequence[str],
         statistic_name: str,
-        constraint_type: str = MDOFunction.TYPE_INEQ,
+        constraint_type: MDOFunction.ConstraintType = MDOFunction.ConstraintType.INEQ,
         constraint_name: str | None = None,
         value: float | None = None,
         positive: bool = False,
         **statistic_parameters: Any,
     ) -> None:
-        """# noqa: D205 D212 D415
+        """
         Args:
             statistic_name: The name of the statistic
                 to be applied to the constraint, e.g. "margin".
             statistic_parameters: The parameters of the statistics
                 to be applied to the constraint,
                 ``{"factor": 2.}`` when ``objective_statistic="margin"``.
-        """
-        if constraint_type not in [MDOFunction.TYPE_EQ, MDOFunction.TYPE_INEQ]:
+        """  # noqa: D205 D212 D415
+        if constraint_type not in [
+            MDOFunction.ConstraintType.EQ,
+            MDOFunction.ConstraintType.INEQ,
+        ]:
             raise ValueError(
-                f"Constraint type must be either '{MDOFunction.TYPE_EQ}' "
-                f"or '{MDOFunction.TYPE_INEQ}'; "
+                f"Constraint type must be either '{MDOFunction.ConstraintType.EQ}' "
+                f"or '{MDOFunction.ConstraintType.INEQ}'; "
                 f"got '{constraint_type}' instead."
             )
         self.formulation.add_constraint(
             output_name,
             statistic_name,
             constraint_type=constraint_type,
             constraint_name=constraint_name,
@@ -180,22 +183,22 @@
         self,
         output_names: Sequence[str],
         statistic_name: str,
         observable_name: Sequence[str] | None = None,
         discipline: MDODiscipline | None = None,
         **statistic_parameters: Any,
     ) -> None:
-        """# noqa: D205 D212 D415
+        """
         Args:
             statistic_name: The name of the statistic
                 to be applied to the constraint, e.g. "margin".
             statistic_parameters: The parameters of the statistics
                 to be applied to the constraint,
                 ``{"factor": 2.}`` when ``objective_statistic="margin"``.
-        """
+        """  # noqa: D205 D212 D415
         self.formulation.add_observable(
             output_names,
             statistic_name,
             observable_name=observable_name,
             discipline=discipline,
             **statistic_parameters,
         )
```

### Comparing `gemseo-umdo-1.0.2/src/gemseo_umdo/scenarios/udoe_scenario.py` & `gemseo-umdo-1.1.0/src/gemseo_umdo/scenarios/udoe_scenario.py`

 * *Files identical despite different names*

### Comparing `gemseo-umdo-1.0.2/src/gemseo_umdo/scenarios/umdo_scenario.py` & `gemseo-umdo-1.1.0/src/gemseo_umdo/scenarios/umdo_scenario.py`

 * *Files identical despite different names*

### Comparing `gemseo-umdo-1.0.2/src/gemseo_umdo/use_cases/__init__.py` & `gemseo-umdo-1.1.0/src/gemseo_umdo/use_cases/__init__.py`

 * *Files identical despite different names*

### Comparing `gemseo-umdo-1.0.2/src/gemseo_umdo/use_cases/spring_mass_model/__init__.py` & `gemseo-umdo-1.1.0/src/gemseo_umdo/use_cases/spring_mass_model/__init__.py`

 * *Files identical despite different names*

### Comparing `gemseo-umdo-1.0.2/src/gemseo_umdo/use_cases/spring_mass_model/discipline.py` & `gemseo-umdo-1.1.0/src/gemseo_umdo/use_cases/spring_mass_model/discipline.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,16 +11,17 @@
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 """The spring-mass model use case."""
 from __future__ import annotations
 
+from typing import Final
+
 from gemseo.core.discipline import MDODiscipline
-from gemseo.utils.python_compatibility import Final
 from numpy import array
 
 from gemseo_umdo.use_cases.spring_mass_model.model import SpringMassModel
 
 
 class SpringMassDiscipline(MDODiscipline):
     r"""The |g|-based spring-mass model :math:`m\frac{d^2z(t)}{dt^2} = -kz(t) + mg`.
@@ -50,16 +51,18 @@
             initial_state: The initial position and velocity of the object.
             initial_time: The initial time.
             final_time: The final time.
             time_step: The time step.
             gravity: The gravity acceleration.
         """  # noqa: D205 D212 D415
         super().__init__(name=f"{self.__class__.__name__}({time_step})")
-        self.input_grammar.update([self.__STIFFNESS])
-        self.output_grammar.update([self.__MAX_DISPLACEMENT, self.__DISPLACEMENT])
+        self.input_grammar.update_from_names([self.__STIFFNESS])
+        self.output_grammar.update_from_names(
+            [self.__MAX_DISPLACEMENT, self.__DISPLACEMENT]
+        )
         self.__model = SpringMassModel(
             mass=mass,
             initial_state=initial_state,
             initial_time=initial_time,
             final_time=final_time,
             time_step=time_step,
             gravity=gravity,
```

### Comparing `gemseo-umdo-1.0.2/src/gemseo_umdo/use_cases/spring_mass_model/model.py` & `gemseo-umdo-1.1.0/src/gemseo_umdo/use_cases/spring_mass_model/model.py`

 * *Files identical despite different names*

### Comparing `gemseo-umdo-1.0.2/src/gemseo_umdo/use_cases/spring_mass_model/uncertain_space.py` & `gemseo-umdo-1.1.0/src/gemseo_umdo/use_cases/spring_mass_model/uncertain_space.py`

 * *Files identical despite different names*

### Comparing `gemseo-umdo-1.0.2/src/gemseo_umdo.egg-info/PKG-INFO` & `gemseo-umdo-1.1.0/src/gemseo_umdo.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: gemseo-umdo
-Version: 1.0.2
+Version: 1.1.0
 Summary: Capability for MDO under uncertainty.
 Home-page: https://gitlab.com/gemseo
 Author: Matthias De Lozzo
 Author-email: contact@gemseo.org
 License: GNU Lesser General Public License v3
 Project-URL: Source, https://gitlab.com/gemseo/dev/gemseo-umdo
 Project-URL: Tracker, https://gitlab.com/gemseo/dev/gemseo-umdo/-/issues
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: <3.11,>=3.7
+Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 License-File: LICENSE.txt
 License-File: CREDITS.rst
 
 ..
     Copyright 2021 IRT Saint Exupéry, https://www.irt-saintexupery.com
```

### Comparing `gemseo-umdo-1.0.2/tests/__init__.py` & `gemseo-umdo-1.1.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gemseo-umdo-1.0.2/tests/formulations/__init__.py` & `gemseo-umdo-1.1.0/tests/formulations/__init__.py`

 * *Files identical despite different names*

### Comparing `gemseo-umdo-1.0.2/tests/formulations/conftest.py` & `gemseo-umdo-1.1.0/tests/formulations/conftest.py`

 * *Files identical despite different names*

### Comparing `gemseo-umdo-1.0.2/tests/formulations/test_factory.py` & `gemseo-umdo-1.1.0/tests/formulations/test_factory.py`

 * *Files identical despite different names*

### Comparing `gemseo-umdo-1.0.2/tests/formulations/test_sampling.py` & `gemseo-umdo-1.1.0/tests/formulations/test_sampling.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,18 +82,18 @@
             "n_samples": None,
             "algo_options": {"samples": array([[0.0] * 3, [1.0] * 3])},
         },
     )
     scn.add_constraint("c", "Margin", factor=3.0)
     scn.add_observable("o", "Variance")
     file_path = tmp_path / "scenario.h5"
-    scn.serialize(file_path)
+    scn.to_pickle(file_path)
     algo_data = {"algo": "CustomDOE", "algo_options": {"samples": array([[0.0] * 3])}}
     scn.execute(algo_data)
-    saved_scn = UDOEScenario.deserialize(file_path)
+    saved_scn = UDOEScenario.from_pickle(file_path)
     saved_scn.execute(algo_data)
     assert_equal(scn.optimization_result.x_opt, array([0.0] * 3))
     assert scn.optimization_result.f_opt == -2.0
     assert_equal(saved_scn.optimization_result.x_opt, array([0.0] * 3))
     assert saved_scn.optimization_result.f_opt == -2.0
```

### Comparing `gemseo-umdo-1.0.2/tests/formulations/test_u_formulation.py` & `gemseo-umdo-1.1.0/tests/formulations/test_u_formulation.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         func: MDOFunction,
         function_type: str,
         name: str,
         **parameters: Any,
     ) -> None:
         super().__init__(lambda u: array([1.0]), name="func")
         self.mock = f"{func.name}_statistics"
-        self.f_type = func.TYPE_INEQ
+        self.f_type = func.ConstraintType.INEQ
 
 
 class MyUMDOFormulation(UMDOFormulation):
     """A dummy UMDOFormulation."""
 
 
 MyUMDOFormulation._StatisticFunction = _StatisticFunction
@@ -99,15 +99,15 @@
     form.add_constraint("c", "Margin", factor=3.0)
     form.add_observable("o", "Mean")
     return form
 
 
 def test_uncertain_space(formulation):
     """Check that the uncertain space contains the uncertain variable."""
-    assert formulation.uncertain_space.variables_names == ["u"]
+    assert formulation.uncertain_space.variable_names == ["u"]
 
 
 def test_name(formulation):
     """Check the name of the UMDOFormulation."""
     assert formulation.name == "MyUMDOFormulation[MDF]"
 
 
@@ -170,15 +170,15 @@
     sub_form = formulation.mdo_formulation
     assert sub_form.__class__.__name__ == "MDF"
     assert sub_form.mda.inner_mdas[0].name == "MDAGaussSeidel"
     assert sub_form.disciplines == formulation.disciplines
     assert sub_form.opt_problem.objective.name == "f"
     assert sub_form.opt_problem.constraints[0].name == "c"
     assert sub_form.opt_problem.observables[0].name == "o"
-    assert sub_form.design_space.variables_names == ["u"]
+    assert sub_form.design_space.variable_names == ["u"]
 
 
 def test_get_expected_workflow(formulation):
     """Check the expected workflow."""
     expected_workflow = formulation.get_expected_workflow()
     # The expected workflow of a MDF with a MDAChain as main MDA
     # is a SerialExecSequence.
```

### Comparing `gemseo-umdo-1.0.2/tests/test_scenario.py` & `gemseo-umdo-1.1.0/tests/test_scenario.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,20 +98,20 @@
     assert scenario.formulation_name == "Sampling[MDF; OT_OPT_LHS(3)]"
     assert scenario.formulation._algo.algo_name
     assert scenario.formulation._n_samples == 3
 
 
 def test_design_space(scenario):
     """Check that the design space contains the design variables."""
-    assert set(scenario.design_space.variables_names) == {"x0", "x1", "x2"}
+    assert set(scenario.design_space.variable_names) == {"x0", "x1", "x2"}
 
 
 def test_uncertain_space(scenario):
     """Check that the uncertain space contains the uncertain variables."""
-    assert set(scenario.uncertain_space.variables_names) == {"u"}
+    assert set(scenario.uncertain_space.variable_names) == {"u"}
 
 
 def test_repr(scenario):
     """Check the text representation of the formulation section of the scenario."""
     expected = f"   Formulation: {scenario.formulation.name}"
     assert repr(scenario).split("\n")[2] == expected
 
@@ -120,15 +120,15 @@
     """Check the content of the MDO formulation."""
     assert scenario.mdo_formulation.__class__.__name__ == "MDF"
     assert scenario.mdo_formulation.mda.inner_mdas[0].name == "MDAGaussSeidel"
     assert scenario.mdo_formulation.disciplines == scenario.disciplines
     assert scenario.mdo_formulation.opt_problem.objective.name == "f"
     assert scenario.mdo_formulation.opt_problem.observables[0].name == "o"
     assert scenario.mdo_formulation.opt_problem.constraints[0].name == "c"
-    assert scenario.mdo_formulation.design_space.variables_names == ["u"]
+    assert scenario.mdo_formulation.design_space.variable_names == ["u"]
 
 
 def test_constraint_wrong_type(disciplines, design_space, uncertain_space):
     """Check that a ValueError is raised when the constraint has a wrong type."""
     scn = UMDOScenario(
         disciplines,
         "MDF",
```

### Comparing `gemseo-umdo-1.0.2/tests/use_cases/__init__.py` & `gemseo-umdo-1.1.0/tests/use_cases/__init__.py`

 * *Files identical despite different names*

### Comparing `gemseo-umdo-1.0.2/tests/use_cases/spring_mass_model/__init__.py` & `gemseo-umdo-1.1.0/tests/use_cases/beam_model/__init__.py`

 * *Files identical despite different names*

### Comparing `gemseo-umdo-1.0.2/tests/use_cases/spring_mass_model/test_discipline.py` & `gemseo-umdo-1.1.0/tests/use_cases/spring_mass_model/test_discipline.py`

 * *Files identical despite different names*

### Comparing `gemseo-umdo-1.0.2/tests/use_cases/spring_mass_model/test_model.py` & `gemseo-umdo-1.1.0/tests/use_cases/spring_mass_model/test_model.py`

 * *Files identical despite different names*

### Comparing `gemseo-umdo-1.0.2/tests/use_cases/spring_mass_model/test_uncertain_space.py` & `gemseo-umdo-1.1.0/tests/use_cases/spring_mass_model/test_uncertain_space.py`

 * *Files identical despite different names*

### Comparing `gemseo-umdo-1.0.2/tox.ini` & `gemseo-umdo-1.1.0/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -33,16 +33,15 @@
     pytest {env:__COVERAGE_POSARGS:} {posargs}
 
 [testenv:check]
 description = run code formatting and checking
 basepython = python3.9
 deps = -r requirements/check.txt
 skip_install = true
-whitelist_externals =
-    pre-commit
+whitelist_externals = pre-commit
 commands =
     pre-commit install
     pre-commit run --all-files
 
 [testenv:doc]
 description = build documentation
 basepython = python3.9
@@ -66,36 +65,38 @@
 whitelist_externals = rm
 commands =
     rm -rf dist build
     python -m build
     twine check dist/*
     python setup.py check --metadata
 
-[testenv:pypi-py{37,38,39,310}]
+[testenv:pypi-py{38,39,310}]
 description = test the pypi distribution
 deps = gemseo-umdo[test]
 skip_install = true
 
 [testenv:update-deps-{doc,dist,check}]
 description = update the non test envs dependencies
 basepython = python3.9
 extras =
     doc: {[testenv:doc]extras}
 setenv =
 passenv =
 deps = pip-tools
 skip_install = true
-whitelist_externals = pip-compile
+whitelist_externals =
+    pip-compile
+    check: pre-commit
 commands =
     doc: pip-compile --upgrade --upgrade-package {[deps]gemseo} --extra doc -o requirements/doc.txt
     dist: pip-compile --upgrade requirements/dist.in
     check: pip-compile --upgrade requirements/check.in
     check: pre-commit autoupdate
 
-[testenv:update-deps-test-py{37,38,39,310}]
+[testenv:update-deps-test-py{38,39,310}]
 description = update the test envs dependencies
 extras = {[testenv]extras}
 setenv =
 passenv =
 deps = pip-tools
 skip_install = true
 commands =
```

