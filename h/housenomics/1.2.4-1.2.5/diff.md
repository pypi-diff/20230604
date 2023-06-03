# Comparing `tmp/housenomics-1.2.4.tar.gz` & `tmp/housenomics-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "housenomics-1.2.4.tar", max compression
+gzip compressed data, was "housenomics-1.2.5.tar", max compression
```

## Comparing `housenomics-1.2.4.tar` & `housenomics-1.2.5.tar`

### file list

```diff
@@ -1,24 +1,21 @@
--rw-r--r--   0        0        0     1211 2023-04-05 20:39:03.022505 housenomics-1.2.4/LICENSE
--rw-r--r--   0        0        0     1311 2023-06-03 19:45:48.704560 housenomics-1.2.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-05 20:39:03.032709 housenomics-1.2.4/src/housenomics/__init__.py
--rw-r--r--   0        0        0        0 2023-04-05 20:39:03.033041 housenomics-1.2.4/src/housenomics/application/__init__.py
--rw-r--r--   0        0        0      787 2023-04-06 08:51:23.764662 housenomics-1.2.4/src/housenomics/application/import_transactions.py
--rw-r--r--   0        0        0      572 2023-05-28 21:46:38.921062 housenomics-1.2.4/src/housenomics/application/import_transactions_test.py
--rw-r--r--   0        0        0      758 2023-04-14 20:32:53.007626 housenomics-1.2.4/src/housenomics/application/repositories/transactions.py
--rw-r--r--   0        0        0     1803 2023-04-05 20:39:03.034847 housenomics-1.2.4/src/housenomics/application/views/transactions.py
--rw-r--r--   0        0        0     4981 2023-05-22 14:25:53.731138 housenomics-1.2.4/src/housenomics/application/views/transactions_test.py
--rw-r--r--   0        0        0     2983 2023-04-07 14:24:59.019481 housenomics-1.2.4/src/housenomics/infrastructure/gateway_cgd_file.py
--rw-r--r--   0        0        0     2045 2023-04-14 20:32:53.007236 housenomics-1.2.4/src/housenomics/infrastructure/gateway_cgd_file_test.py
--rw-r--r--   0        0        0      494 2023-04-14 20:32:53.008002 housenomics-1.2.4/src/housenomics/transaction.py
--rw-r--r--   0        0        0        0 2023-04-05 20:39:03.038982 housenomics-1.2.4/src/housenomics/ui/cli/__init__.py
--rw-r--r--   0        0        0     2451 2023-05-22 14:25:53.732424 housenomics-1.2.4/src/housenomics/ui/cli/main.py
--rw-r--r--   0        0        0      670 2023-04-05 20:39:03.039671 housenomics-1.2.4/src/housenomics/ui/cli/report.py
--rw-r--r--   0        0        0      323 2023-04-05 20:39:03.039911 housenomics-1.2.4/src/housenomics/ui/cli/version.py
--rw-r--r--   0        0        0      479 2023-04-05 20:39:03.041120 housenomics-1.2.4/src/toolbox/cli.py
--rw-r--r--   0        0        0     2288 2023-05-22 14:25:53.743334 housenomics-1.2.4/src/toolbox/database.py
--rw-r--r--   0        0        0     1649 2023-05-22 14:25:53.747558 housenomics-1.2.4/src/toolbox/database_test.py
--rw-r--r--   0        0        0      607 2023-06-03 18:46:28.056797 housenomics-1.2.4/src/toolbox/project.py
--rw-r--r--   0        0        0     1482 2023-06-03 18:51:23.522195 housenomics-1.2.4/src/toolbox/projects_test.py
--rw-r--r--   0        0        0       64 2023-04-05 20:39:03.042194 housenomics-1.2.4/src/toolbox/views.py
--rw-r--r--   0        0        0      143 2023-04-05 20:39:03.042641 housenomics-1.2.4/src/toolbox/views_test.py
--rw-r--r--   0        0        0      625 1970-01-01 00:00:00.000000 housenomics-1.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-04-05 20:39:03.022505 housenomics-1.2.5/LICENSE
+-rw-r--r--   0        0        0     1311 2023-06-03 23:17:27.019530 housenomics-1.2.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-05 20:39:03.032709 housenomics-1.2.5/src/housenomics/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-05 20:39:03.033041 housenomics-1.2.5/src/housenomics/application/__init__.py
+-rw-r--r--   0        0        0      787 2023-04-06 08:51:23.764662 housenomics-1.2.5/src/housenomics/application/import_transactions.py
+-rw-r--r--   0        0        0      572 2023-05-28 21:46:38.921062 housenomics-1.2.5/src/housenomics/application/import_transactions_test.py
+-rw-r--r--   0        0        0      758 2023-04-14 20:32:53.007626 housenomics-1.2.5/src/housenomics/application/repositories/transactions.py
+-rw-r--r--   0        0        0     1803 2023-04-05 20:39:03.034847 housenomics-1.2.5/src/housenomics/application/views/transactions.py
+-rw-r--r--   0        0        0     4981 2023-06-03 23:16:04.690593 housenomics-1.2.5/src/housenomics/application/views/transactions_test.py
+-rw-r--r--   0        0        0     2983 2023-04-07 14:24:59.019481 housenomics-1.2.5/src/housenomics/infrastructure/gateway_cgd_file.py
+-rw-r--r--   0        0        0     2045 2023-04-14 20:32:53.007236 housenomics-1.2.5/src/housenomics/infrastructure/gateway_cgd_file_test.py
+-rw-r--r--   0        0        0      494 2023-06-03 23:13:55.270918 housenomics-1.2.5/src/housenomics/transaction.py
+-rw-r--r--   0        0        0        0 2023-04-05 20:39:03.038982 housenomics-1.2.5/src/housenomics/ui/cli/__init__.py
+-rw-r--r--   0        0        0     2451 2023-06-03 23:16:04.686939 housenomics-1.2.5/src/housenomics/ui/cli/main.py
+-rw-r--r--   0        0        0      670 2023-06-03 23:16:04.691822 housenomics-1.2.5/src/housenomics/ui/cli/report.py
+-rw-r--r--   0        0        0      323 2023-04-05 20:39:03.039911 housenomics-1.2.5/src/housenomics/ui/cli/version.py
+-rw-r--r--   0        0        0      479 2023-04-05 20:39:03.041120 housenomics-1.2.5/src/toolbox/cli.py
+-rw-r--r--   0        0        0       83 2023-06-03 23:15:36.706123 housenomics-1.2.5/src/toolbox/database.py
+-rw-r--r--   0        0        0       64 2023-04-05 20:39:03.042194 housenomics-1.2.5/src/toolbox/views.py
+-rw-r--r--   0        0        0      143 2023-04-05 20:39:03.042641 housenomics-1.2.5/src/toolbox/views_test.py
+-rw-r--r--   0        0        0      625 1970-01-01 00:00:00.000000 housenomics-1.2.5/PKG-INFO
```

### Comparing `housenomics-1.2.4/LICENSE` & `housenomics-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `housenomics-1.2.4/pyproject.toml` & `housenomics-1.2.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.bandit]
 exclude_dirs = ["tests", "features"]
 
 [tool.poetry]
 name = "housenomics"
-version = "1.2.4"
+version = "1.2.5"
 description = "Manage your personal finances"
 authors = ["Luís Miranda <luistm@gmail.com>"]
 license = "MIT"
 
 [[tool.poetry.packages]]
 include = "toolbox"
 from = "src"
@@ -37,15 +37,15 @@
 [tool.poetry.dependencies]
 python = "^3.10"
 rich = "^13.3.5"
 typer = "^0.9.0"
 pendulum = "^2.1.2"
 sqlalchemy = "^2.0.15"
 toml = "^0.10.2"
-toolcat = "0.0.2"
+toolcat = "0.0.3"
 
 [tool.pytest.ini_options]
 markers = ["integration: tags a test as integration tests"]
 
 [tool.poetry.dev-dependencies.bandit]
 extras = ["toml"]
 version = "^1.7.5"
```

### Comparing `housenomics-1.2.4/src/housenomics/application/import_transactions.py` & `housenomics-1.2.5/src/housenomics/application/import_transactions.py`

 * *Files identical despite different names*

### Comparing `housenomics-1.2.4/src/housenomics/application/import_transactions_test.py` & `housenomics-1.2.5/src/housenomics/application/import_transactions_test.py`

 * *Files identical despite different names*

### Comparing `housenomics-1.2.4/src/housenomics/application/repositories/transactions.py` & `housenomics-1.2.5/src/housenomics/application/repositories/transactions.py`

 * *Files identical despite different names*

### Comparing `housenomics-1.2.4/src/housenomics/application/views/transactions.py` & `housenomics-1.2.5/src/housenomics/application/views/transactions.py`

 * *Files identical despite different names*

### Comparing `housenomics-1.2.4/src/housenomics/application/views/transactions_test.py` & `housenomics-1.2.5/src/housenomics/application/views/transactions_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pytest
 from sqlalchemy import text
 from sqlalchemy.orm import Session
+from toolcat.database import Database
 
 from housenomics.application.views.transactions import ViewTransactions
-from toolbox.database import Database
 
 
 @pytest.fixture
 def tmp_db_session(tmp_path):
     """
     Crates a database in the path define by tmpdir.
     """
```

### Comparing `housenomics-1.2.4/src/housenomics/infrastructure/gateway_cgd_file.py` & `housenomics-1.2.5/src/housenomics/infrastructure/gateway_cgd_file.py`

 * *Files identical despite different names*

### Comparing `housenomics-1.2.4/src/housenomics/infrastructure/gateway_cgd_file_test.py` & `housenomics-1.2.5/src/housenomics/infrastructure/gateway_cgd_file_test.py`

 * *Files identical despite different names*

### Comparing `housenomics-1.2.4/src/housenomics/ui/cli/main.py` & `housenomics-1.2.5/src/housenomics/ui/cli/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import logging
 from datetime import datetime
 from pathlib import Path
 from typing import Optional
 
 from sqlalchemy.orm import Session
+from toolcat.database import Database
 
 from housenomics.application.import_transactions import ServiceImportTransactions
 from housenomics.application.repositories.transactions import Transactions
 from housenomics.infrastructure.gateway_cgd_file import GatewayCGDFile
 from housenomics.ui.cli.report import report
 from housenomics.ui.cli.version import CommandVersion
 from toolbox import cli
 from toolbox.cli import CLIApplication
-from toolbox.database import Database
 
 logging_format: dict = {
     "level": logging.CRITICAL,
     "format": "%(asctime)s - %(name)s - %(levelname)s - %(message)s",
 }
 
 logging.basicConfig(**logging_format)
```

### Comparing `housenomics-1.2.4/src/housenomics/ui/cli/report.py` & `housenomics-1.2.5/src/housenomics/ui/cli/report.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from sqlalchemy.orm import Session
+from toolcat.database import Database
 
 from housenomics.application.views.transactions import ViewTransactions
-from toolbox.database import Database
 
 
 def report(database_path, seller, since, on):
     with Session(Database(database_path).engine) as session:
         view = ViewTransactions(session, seller, since, on)
 
     transactions, total = view.data
```

### Comparing `housenomics-1.2.4/PKG-INFO` & `housenomics-1.2.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: housenomics
-Version: 1.2.4
+Version: 1.2.5
 Summary: Manage your personal finances
 License: MIT
 Author: Luís Miranda
 Author-email: luistm@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pendulum (>=2.1.2,<3.0.0)
 Requires-Dist: rich (>=13.3.5,<14.0.0)
 Requires-Dist: sqlalchemy (>=2.0.15,<3.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
-Requires-Dist: toolcat (==0.0.2)
+Requires-Dist: toolcat (==0.0.3)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
```

