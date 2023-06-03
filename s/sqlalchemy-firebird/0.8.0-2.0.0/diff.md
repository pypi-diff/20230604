# Comparing `tmp/sqlalchemy-firebird-0.8.0.tar.gz` & `tmp/sqlalchemy-firebird-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy-firebird-0.8.0.tar", last modified: Tue Apr 11 05:50:23 2023, max compression
+gzip compressed data, was "sqlalchemy-firebird-2.0.0.tar", last modified: Sat Jun  3 23:40:56 2023, max compression
```

## Comparing `sqlalchemy-firebird-0.8.0.tar` & `sqlalchemy-firebird-2.0.0.tar`

### file list

```diff
@@ -1,29 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 05:50:23.479142 sqlalchemy-firebird-0.8.0/
--rw-rw-rw-   0        0        0     1117 2023-01-02 01:08:06.000000 sqlalchemy-firebird-0.8.0/LICENSE
--rw-rw-rw-   0        0        0     2271 2023-04-11 05:50:23.479642 sqlalchemy-firebird-0.8.0/PKG-INFO
--rw-rw-rw-   0        0        0     1349 2023-01-02 01:08:06.000000 sqlalchemy-firebird-0.8.0/README.rst
--rw-rw-rw-   0        0        0      896 2023-04-11 05:26:28.000000 sqlalchemy-firebird-0.8.0/pyproject.toml
--rw-rw-rw-   0        0        0      374 2023-04-11 05:50:23.482142 sqlalchemy-firebird-0.8.0/setup.cfg
--rw-rw-rw-   0        0        0     1944 2023-04-11 05:26:28.000000 sqlalchemy-firebird-0.8.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-11 05:50:23.449643 sqlalchemy-firebird-0.8.0/sqlalchemy_firebird/
--rw-rw-rw-   0        0        0     1109 2023-04-11 05:34:11.000000 sqlalchemy-firebird-0.8.0/sqlalchemy_firebird/__init__.py
--rw-rw-rw-   0        0        0    35223 2023-04-02 20:53:51.000000 sqlalchemy-firebird-0.8.0/sqlalchemy_firebird/base.py
--rw-rw-rw-   0        0        0     4082 2023-04-11 05:26:28.000000 sqlalchemy-firebird-0.8.0/sqlalchemy_firebird/fdb.py
--rw-rw-rw-   0        0        0     6415 2023-01-16 16:40:52.000000 sqlalchemy-firebird-0.8.0/sqlalchemy_firebird/kinterbasdb.py
--rw-rw-rw-   0        0        0      348 2023-04-11 05:26:28.000000 sqlalchemy-firebird-0.8.0/sqlalchemy_firebird/provision.py
--rw-rw-rw-   0        0        0     2984 2023-04-11 05:26:28.000000 sqlalchemy-firebird-0.8.0/sqlalchemy_firebird/requirements.py
-drwxrwxrwx   0        0        0        0 2023-04-11 05:50:23.464145 sqlalchemy-firebird-0.8.0/sqlalchemy_firebird.egg-info/
--rw-rw-rw-   0        0        0     2271 2023-04-11 05:50:23.000000 sqlalchemy-firebird-0.8.0/sqlalchemy_firebird.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      687 2023-04-11 05:50:23.000000 sqlalchemy-firebird-0.8.0/sqlalchemy_firebird.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 05:50:23.000000 sqlalchemy-firebird-0.8.0/sqlalchemy_firebird.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      124 2023-04-11 05:50:23.000000 sqlalchemy-firebird-0.8.0/sqlalchemy_firebird.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-01-14 23:50:33.000000 sqlalchemy-firebird-0.8.0/sqlalchemy_firebird.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       22 2023-04-11 05:50:23.000000 sqlalchemy-firebird-0.8.0/sqlalchemy_firebird.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-04-11 05:50:23.000000 sqlalchemy-firebird-0.8.0/sqlalchemy_firebird.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-11 05:50:23.477144 sqlalchemy-firebird-0.8.0/test/
--rw-rw-rw-   0        0        0     4463 2023-01-16 16:40:52.000000 sqlalchemy-firebird-0.8.0/test/test_domain_reflection.py
--rw-rw-rw-   0        0        0     1629 2023-01-02 01:08:06.000000 sqlalchemy-firebird-0.8.0/test/test_fb_argument.py
--rw-rw-rw-   0        0        0     7646 2023-01-16 16:40:52.000000 sqlalchemy-firebird-0.8.0/test/test_fb_compile.py
--rw-rw-rw-   0        0        0     4094 2023-01-16 16:40:52.000000 sqlalchemy-firebird-0.8.0/test/test_fb_misc.py
--rw-rw-rw-   0        0        0      624 2023-01-02 01:08:06.000000 sqlalchemy-firebird-0.8.0/test/test_fb_types.py
--rw-rw-rw-   0        0        0     9471 2023-04-11 05:26:28.000000 sqlalchemy-firebird-0.8.0/test/test_suite.py
+drwxrwxrwx   0        0        0        0 2023-06-03 23:40:56.107075 sqlalchemy-firebird-2.0.0/
+-rw-rw-rw-   0        0        0     1117 2023-05-10 05:21:54.000000 sqlalchemy-firebird-2.0.0/LICENSE
+-rw-rw-rw-   0        0        0     3544 2023-06-03 23:40:56.107575 sqlalchemy-firebird-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2584 2023-06-03 23:38:26.000000 sqlalchemy-firebird-2.0.0/README.rst
+-rw-rw-rw-   0        0        0      486 2023-05-31 05:04:17.000000 sqlalchemy-firebird-2.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1523 2023-06-03 23:40:56.108575 sqlalchemy-firebird-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     2272 2023-06-03 22:51:36.000000 sqlalchemy-firebird-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 23:40:56.080731 sqlalchemy-firebird-2.0.0/sqlalchemy_firebird/
+-rw-rw-rw-   0        0        0      240 2023-05-31 05:02:12.000000 sqlalchemy-firebird-2.0.0/sqlalchemy_firebird/__init__.py
+-rw-rw-rw-   0        0        0    36833 2023-05-18 00:05:12.000000 sqlalchemy-firebird-2.0.0/sqlalchemy_firebird/base.py
+-rw-rw-rw-   0        0        0     4747 2023-05-18 00:05:12.000000 sqlalchemy-firebird-2.0.0/sqlalchemy_firebird/fb_info25.py
+-rw-rw-rw-   0        0        0     5498 2023-05-18 00:05:12.000000 sqlalchemy-firebird-2.0.0/sqlalchemy_firebird/fb_info30.py
+-rw-rw-rw-   0        0        0     6423 2023-05-18 00:05:12.000000 sqlalchemy-firebird-2.0.0/sqlalchemy_firebird/fb_info40.py
+-rw-rw-rw-   0        0        0     1587 2023-05-30 01:22:53.000000 sqlalchemy-firebird-2.0.0/sqlalchemy_firebird/fdb.py
+-rw-rw-rw-   0        0        0     3989 2023-05-18 00:05:12.000000 sqlalchemy-firebird-2.0.0/sqlalchemy_firebird/firebird.py
+-rw-rw-rw-   0        0        0     1044 2023-05-28 18:26:53.000000 sqlalchemy-firebird-2.0.0/sqlalchemy_firebird/provision.py
+-rw-rw-rw-   0        0        0     7635 2023-05-17 03:00:51.000000 sqlalchemy-firebird-2.0.0/sqlalchemy_firebird/requirements.py
+-rw-rw-rw-   0        0        0      810 2023-05-17 02:46:52.000000 sqlalchemy-firebird-2.0.0/sqlalchemy_firebird/types.py
+drwxrwxrwx   0        0        0        0 2023-06-03 23:40:56.095073 sqlalchemy-firebird-2.0.0/sqlalchemy_firebird.egg-info/
+-rw-rw-rw-   0        0        0     3544 2023-06-03 23:40:55.000000 sqlalchemy-firebird-2.0.0/sqlalchemy_firebird.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      787 2023-06-03 23:40:55.000000 sqlalchemy-firebird-2.0.0/sqlalchemy_firebird.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 23:40:55.000000 sqlalchemy-firebird-2.0.0/sqlalchemy_firebird.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      202 2023-06-03 23:40:55.000000 sqlalchemy-firebird-2.0.0/sqlalchemy_firebird.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-05-28 18:10:47.000000 sqlalchemy-firebird-2.0.0/sqlalchemy_firebird.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      112 2023-06-03 23:40:55.000000 sqlalchemy-firebird-2.0.0/sqlalchemy_firebird.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-06-03 23:40:55.000000 sqlalchemy-firebird-2.0.0/sqlalchemy_firebird.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-03 23:40:56.105075 sqlalchemy-firebird-2.0.0/test/
+-rw-rw-rw-   0        0        0     4463 2023-05-10 05:21:54.000000 sqlalchemy-firebird-2.0.0/test/test_domain_reflection.py
+-rw-rw-rw-   0        0        0     7328 2023-05-17 02:44:49.000000 sqlalchemy-firebird-2.0.0/test/test_fb_compile.py
+-rw-rw-rw-   0        0        0     3239 2023-05-17 02:44:49.000000 sqlalchemy-firebird-2.0.0/test/test_fb_misc.py
+-rw-rw-rw-   0        0        0      624 2023-05-10 05:21:54.000000 sqlalchemy-firebird-2.0.0/test/test_fb_types.py
+-rw-rw-rw-   0        0        0    11354 2023-05-18 00:14:53.000000 sqlalchemy-firebird-2.0.0/test/test_suite.py
```

### Comparing `sqlalchemy-firebird-0.8.0/LICENSE` & `sqlalchemy-firebird-2.0.0/LICENSE`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright 2005-2020 SQLAlchemy authors and contributors <see AUTHORS file>.
+Copyright 2005-2023 SQLAlchemy authors and contributors <see AUTHORS file>.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
 of the Software, and to permit persons to whom the Software is furnished to do
 so, subject to the following conditions:
```

### Comparing `sqlalchemy-firebird-0.8.0/PKG-INFO` & `sqlalchemy-firebird-2.0.0/README.rst`

 * *Files 21% similar despite different names*

```diff
@@ -1,62 +1,62 @@
-Metadata-Version: 2.1
-Name: sqlalchemy-firebird
-Version: 0.8.0
-Summary: Firebird for SQLAlchemy
-Home-page: https://github.com/pauldex/sqlalchemy-firebird
-Author: Paul Graves-DesLauriers
-Author-email: paul@dexmicro.com
-License: MIT
-Project-URL: Documentation, https://github.com/pauldex/sqlalchemy-firebird/wiki
-Project-URL: Source, https://github.com/pauldex/sqlalchemy-firebird
-Project-URL: Tracker, https://github.com/pauldex/sqlalchemy-firebird/issues
-Keywords: SQLAlchemy Firebird
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Topic :: Database :: Front-Ends
-Classifier: Operating System :: OS Independent
-License-File: LICENSE
-
 sqlalchemy-firebird
 ###################
 
 An external SQLAlchemy dialect for Firebird
 ===========================================
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
 .. image:: https://github.com/pauldex/sqlalchemy-firebird/workflows/sqlalchemy-firebird/badge.svg
     :target: https://github.com/pauldex/sqlalchemy-firebird
 
 ----
 
-| This replaces SQLAlchemy's internal Firebird dialect which is not being maintained
- and will be removed in a future version.
+| This package provides a `Firebird <https://firebirdsql.org/en/start/>`_ dialect for `SQLAlchemy <https://www.sqlalchemy.org>`_ using the `firebird-driver <https://firebird-driver.readthedocs.io/en/latest>`_ and/or `fdb <https://fdb.readthedocs.io/en/latest>`_ driver.
 
 ****
 
 **Installation**
 
 ::
 
     pip install sqlalchemy-firebird
 
-|
-|  Connection URI samples for Firebird server installed on local machine using default port (3050):
+If you are using Python 3.8 or greater, SQLAlchemy 2.0+ and firebird-driver will be automatically installed.
+Python 3.6 and 3.7 will automatically install and use SQLAlchemy < 2.0 and fdb instead.
+
+Connection URI samples for Firebird server installed on local machine using default port (3050):
 
 ::
 
     [Linux]
-    firebird://username:password@localhost///home/paulgd/projects/databases/my_project.fdb
+    # Use the fdb driver (Python 3.6/3.7)
+    firebird+fdb://username:password@localhost///home/testuser/projects/databases/my_project.fdb
+    # Use the firebird-driver driver (Python 3.8+)
+    firebird+firebird://username:password@localhost///home/testuser/projects/databases/my_project.fdb
 
     [Windows]
-    firebird://username:password@localhost/c:/projects/databases/my_project.fdb
+    # Use the fdb driver (Python 3.6/3.7)
+    firebird+fdb://username:password@localhost/c:/projects/databases/my_project.fdb
+    # Use the firebird-driver driver (Python 3.8+)
+    firebird+firebird://username:password@localhost/c:/projects/databases/my_project.fdb
+
+****
+
+**Usage**
+
+For example, to connect to a Firebird server installed on a local Windows machine using the default port and firebird-driver:
+
+::
+
+    db_uri = "firebird+firebird://username:password@localhost/c:/projects/databases/my_project.fdb"
+    from sqlalchemy import create_engine
+    engine = create_engine(db_uri, echo=True)
+
+Connecting to different types of Firebird servers, databases, or drivers is done simply by changing the db_uri string
+used in the call to create_engine.
 
 ----
 
 **Code of Conduct**
 
 As with SQLAlchemy, sqlalchemy-firebird places great emphasis on polite, thoughtful, and
 constructive communication between users and developers.
```

### Comparing `sqlalchemy-firebird-0.8.0/setup.py` & `sqlalchemy-firebird-2.0.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 
 setup(
     name="sqlalchemy-firebird",
     version=VERSION,
     description="Firebird for SQLAlchemy",
     long_description=open(readme).read(),
+    long_description_content_type="text/x-rst",
     url="https://github.com/pauldex/sqlalchemy-firebird",
     author="Paul Graves-DesLauriers",
     author_email="paul@dexmicro.com",
     license="MIT",
     classifiers=[
         # 'Development Status :: 1 - Planning',
         # "Development Status :: 2 - Pre-Alpha",
@@ -41,16 +42,22 @@
     project_urls={
         "Documentation": "https://github.com/pauldex/sqlalchemy-firebird/wiki",
         "Source": "https://github.com/pauldex/sqlalchemy-firebird",
         "Tracker": "https://github.com/pauldex/sqlalchemy-firebird/issues",
     },
     packages=find_packages(include=["sqlalchemy_firebird"]),
     include_package_data=True,
-    install_requires=["SQLAlchemy>1.3.16", "fdb"],
+    install_requires=[
+        "SQLAlchemy >= 1.4, < 2.0; python_version < '3.8'",
+        "fdb; python_version < '3.8'",
+        "SQLAlchemy >= 2.0; python_version >= '3.8'",
+        "firebird-driver; python_version >= '3.8'",
+],
     zip_safe=False,
     entry_points={
         "sqlalchemy.dialects": [
-            "firebird = sqlalchemy_firebird.fdb:FBDialect_fdb",
+            "firebird = sqlalchemy_firebird.firebird:FBDialect_firebird",
             "firebird.fdb = sqlalchemy_firebird.fdb:FBDialect_fdb",
+            "firebird.firebird = sqlalchemy_firebird.firebird:FBDialect_firebird",
         ]
     },
 )
```

### Comparing `sqlalchemy-firebird-0.8.0/sqlalchemy_firebird/base.py` & `sqlalchemy-firebird-2.0.0/sqlalchemy_firebird/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,935 +1,629 @@
-"""
-
-.. dialect:: firebird
-    :name: Firebird
-
-.. note::
-
-    The Firebird dialect within SQLAlchemy **is not currently supported**. The
-    dialect is not tested within continuous integration and is likely to have
-    many issues and caveats not currently handled.
-
-Firebird Dialects
------------------
-
-Firebird offers two distinct dialects_ (not to be confused with a
-SQLAlchemy ``Dialect``):
-
-dialect 1
-  This is the old syntax and behaviour, inherited from Interbase pre-6.0.
-
-dialect 3
-  This is the newer and supported syntax, introduced in Interbase 6.0.
-
-The SQLAlchemy Firebird dialect detects these versions and
-adjusts its representation of SQL accordingly.  However,
-support for dialect 1 is not well tested and probably has
-incompatibilities.
-
-Locking Behavior
-----------------
-
-Firebird locks tables aggressively.  For this reason, a DROP TABLE may
-hang until other transactions are released.  SQLAlchemy does its best
-to release transactions as quickly as possible.  The most common cause
-of hanging transactions is a non-fully consumed result set, i.e.::
-
-    result = engine.execute("select * from table")
-    row = result.fetchone()
-    return
-
-Where above, the ``ResultProxy`` has not been fully consumed.  The
-connection will be returned to the pool and the transactional state
-rolled back once the Python garbage collector reclaims the objects
-which hold onto the connection, which often occurs asynchronously.
-The above use case can be alleviated by calling ``first()`` on the
-``ResultProxy`` which will fetch the first row and immediately close
-all remaining cursor/connection resources.
-
-RETURNING support
------------------
-
-Firebird 2.0 supports returning a result set from inserts, and 2.1
-extends that to deletes and updates. This is generically exposed by
-the SQLAlchemy ``returning()`` method, such as::
-
-    # INSERT..RETURNING
-    result = table.insert().returning(table.c.col1, table.c.col2).\
-                   values(name='foo')
-    print result.fetchall()
-
-    # UPDATE..RETURNING
-    raises = empl.update().returning(empl.c.id, empl.c.salary).\
-                  where(empl.c.sales>100).\
-                  values(dict(salary=empl.c.salary * 1.1))
-    print raises.fetchall()
-
-
-.. _dialects: http://mc-computing.com/Databases/Firebird/SQL_Dialect.html
-
-"""  # noqa
-
-import datetime
+from packaging import version
 
+from sqlalchemy import __version__ as SQLALCHEMY_VERSION
 from sqlalchemy import exc
 from sqlalchemy import schema as sa_schema
 from sqlalchemy import sql
 from sqlalchemy import text
 from sqlalchemy import types as sqltypes
 from sqlalchemy import util
 from sqlalchemy.engine import default
 from sqlalchemy.engine import reflection
 from sqlalchemy.sql import compiler
 from sqlalchemy.sql import expression
-from sqlalchemy.types import BIGINT
 from sqlalchemy.types import BLOB
-from sqlalchemy.types import DATE
-from sqlalchemy.types import FLOAT
-from sqlalchemy.types import INTEGER
 from sqlalchemy.types import Integer
 from sqlalchemy.types import NUMERIC
-from sqlalchemy.types import SMALLINT
 from sqlalchemy.types import TEXT
-from sqlalchemy.types import TIME
-from sqlalchemy.types import TIMESTAMP
-
-RESERVED_WORDS = set(
-    [
-        "active",
-        "add",
-        "admin",
-        "after",
-        "all",
-        "alter",
-        "and",
-        "any",
-        "as",
-        "asc",
-        "ascending",
-        "at",
-        "auto",
-        "avg",
-        "before",
-        "begin",
-        "between",
-        "bigint",
-        "bit_length",
-        "blob",
-        "both",
-        "by",
-        "case",
-        "cast",
-        "char",
-        "character",
-        "character_length",
-        "char_length",
-        "check",
-        "close",
-        "collate",
-        "column",
-        "commit",
-        "committed",
-        "computed",
-        "conditional",
-        "connect",
-        "constraint",
-        "containing",
-        "count",
-        "create",
-        "cross",
-        "cstring",
-        "current",
-        "current_connection",
-        "current_date",
-        "current_role",
-        "current_time",
-        "current_timestamp",
-        "current_transaction",
-        "current_user",
-        "cursor",
-        "database",
-        "date",
-        "day",
-        "dec",
-        "decimal",
-        "declare",
-        "default",
-        "delete",
-        "desc",
-        "descending",
-        "disconnect",
-        "distinct",
-        "do",
-        "domain",
-        "double",
-        "drop",
-        "else",
-        "end",
-        "entry_point",
-        "escape",
-        "exception",
-        "execute",
-        "exists",
-        "exit",
-        "external",
-        "extract",
-        "fetch",
-        "file",
-        "filter",
-        "float",
-        "for",
-        "foreign",
-        "from",
-        "full",
-        "function",
-        "gdscode",
-        "generator",
-        "gen_id",
-        "global",
-        "grant",
-        "group",
-        "having",
-        "hour",
-        "if",
-        "in",
-        "inactive",
-        "index",
-        "inner",
-        "input_type",
-        "insensitive",
-        "insert",
-        "int",
-        "integer",
-        "into",
-        "is",
-        "isolation",
-        "join",
-        "key",
-        "leading",
-        "left",
-        "length",
-        "level",
-        "like",
-        "long",
-        "lower",
-        "manual",
-        "max",
-        "maximum_segment",
-        "merge",
-        "min",
-        "minute",
-        "module_name",
-        "month",
-        "names",
-        "national",
-        "natural",
-        "nchar",
-        "no",
-        "not",
-        "null",
-        "numeric",
-        "octet_length",
-        "of",
-        "on",
-        "only",
-        "open",
-        "option",
-        "or",
-        "order",
-        "outer",
-        "output_type",
-        "overflow",
-        "page",
-        "pages",
-        "page_size",
-        "parameter",
-        "password",
-        "plan",
-        "position",
-        "post_event",
-        "precision",
-        "primary",
-        "privileges",
-        "procedure",
-        "protected",
-        "rdb$db_key",
-        "read",
-        "real",
-        "record_version",
-        "recreate",
-        "recursive",
-        "references",
-        "release",
-        "reserv",
-        "reserving",
-        "retain",
-        "returning_values",
-        "returns",
-        "revoke",
-        "right",
-        "rollback",
-        "rows",
-        "row_count",
-        "savepoint",
-        "schema",
-        "second",
-        "segment",
-        "select",
-        "sensitive",
-        "set",
-        "shadow",
-        "shared",
-        "singular",
-        "size",
-        "smallint",
-        "snapshot",
-        "some",
-        "sort",
-        "sqlcode",
-        "stability",
-        "start",
-        "starting",
-        "starts",
-        "statistics",
-        "sub_type",
-        "sum",
-        "suspend",
-        "table",
-        "then",
-        "time",
-        "timestamp",
-        "to",
-        "trailing",
-        "transaction",
-        "trigger",
-        "trim",
-        "uncommitted",
-        "union",
-        "unique",
-        "update",
-        "upper",
-        "user",
-        "using",
-        "value",
-        "values",
-        "varchar",
-        "variable",
-        "varying",
-        "view",
-        "wait",
-        "when",
-        "where",
-        "while",
-        "with",
-        "work",
-        "write",
-        "year",
-    ]
-)
-
-
-class _StringType(sqltypes.String):
-    """Base for Firebird string types."""
-
-    def __init__(self, charset=None, **kw):
-        self.charset = charset
-        super(_StringType, self).__init__(**kw)
-
-
-class VARCHAR(_StringType, sqltypes.VARCHAR):
-    """Firebird VARCHAR type"""
-
-    __visit_name__ = "VARCHAR"
-
-    def __init__(self, length=None, **kwargs):
-        super(VARCHAR, self).__init__(length=length, **kwargs)
-
-
-class CHAR(_StringType, sqltypes.CHAR):
-    """Firebird CHAR type"""
-
-    __visit_name__ = "CHAR"
-
-    def __init__(self, length=None, **kwargs):
-        super(CHAR, self).__init__(length=length, **kwargs)
-
-
-class _FBDateTime(sqltypes.DateTime):
-    def bind_processor(self, dialect):
-        def process(value):
-            if type(value) == datetime.date:
-                return datetime.datetime(value.year, value.month, value.day)
-            else:
-                return value
 
-        return process
-
-
-colspecs = {sqltypes.DateTime: _FBDateTime}
-
-ischema_names = {
-    "SHORT": SMALLINT,
-    "LONG": INTEGER,
-    "QUAD": FLOAT,
-    "FLOAT": FLOAT,
-    "DATE": DATE,
-    "TIME": TIME,
-    "TEXT": TEXT,
-    "INT64": BIGINT,
-    "DOUBLE": FLOAT,
-    "TIMESTAMP": TIMESTAMP,
-    "VARYING": VARCHAR,
-    "CSTRING": CHAR,
-    "BLOB": BLOB,
-}
-
-
-# TODO: date conversion types (should be implemented as _FBDateTime,
-# _FBDate, etc. as bind/result functionality is required)
-
-
-class FBTypeCompiler(compiler.GenericTypeCompiler):
-    def visit_boolean(self, type_, **kw):
-        return self.visit_SMALLINT(type_, **kw)
-
-    def visit_datetime(self, type_, **kw):
-        return self.visit_TIMESTAMP(type_, **kw)
-
-    def visit_TEXT(self, type_, **kw):
-        return "BLOB SUB_TYPE 1"
-
-    def visit_BLOB(self, type_, **kw):
-        return "BLOB SUB_TYPE 0"
-
-    def _extend_string(self, type_, basic):
-        charset = getattr(type_, "charset", None)
-        if charset is None:
-            return basic
-        else:
-            return "%s CHARACTER SET %s" % (basic, charset)
-
-    def visit_CHAR(self, type_, **kw):
-        basic = super(FBTypeCompiler, self).visit_CHAR(type_, **kw)
-        return self._extend_string(type_, basic)
-
-    def visit_VARCHAR(self, type_, **kw):
-        if not type_.length:
-            raise exc.CompileError(
-                "VARCHAR requires a length on dialect %s" % self.dialect.name
-            )
-        basic = super(FBTypeCompiler, self).visit_VARCHAR(type_, **kw)
-        return self._extend_string(type_, basic)
+EXPRESSION_SEPARATOR = "||"
 
 
 class FBCompiler(sql.compiler.SQLCompiler):
-    """Firebird specific idiosyncrasies"""
-
     ansi_bind_rules = True
 
-    # def visit_contains_op_binary(self, binary, operator, **kw):
-    # cant use CONTAINING b.c. it's case insensitive.
+    def visit_empty_set_expr(self, element_types, **kw):
+        return "SELECT 1 FROM rdb$database WHERE 1 != 1"
 
-    # def visit_notcontains_op_binary(self, binary, operator, **kw):
-    # cant use NOT CONTAINING b.c. it's case insensitive.
+    def visit_sequence(self, sequence, **kw):
+        return "GEN_ID(%s, 1)" % self.preparer.format_sequence(sequence)
 
-    def visit_empty_set_expr(self, type_):
-        # FB equivalent of Oracle's FROM DUAL courtesy of
-        # http://www.firebirdfaq.org/faq30/
-        return "SELECT 1 FROM RDB$DATABASE WHERE 0=1"
+    def limit_clause(self, select, **kw):
+        return self._handle_limit_fetch_clause(
+            None, select._offset_clause, select._limit_clause, **kw
+        )
 
-    def visit_now_func(self, fn, **kw):
-        return "CURRENT_TIMESTAMP"
+    def fetch_clause(
+        self,
+        select,
+        fetch_clause=None,
+        require_offset=False,
+        use_literal_execute_for_simple_int=False,
+        **kw,
+    ):
+        if fetch_clause is None:
+            fetch_clause = select._fetch_clause
 
-    def visit_mod_binary(self, binary, operator, **kw):
-        return "mod(%s, %s)" % (
-            self.process(binary.left, **kw),
-            self.process(binary.right, **kw),
+        return self._handle_limit_fetch_clause(
+            fetch_clause, select._offset_clause, None, **kw
         )
 
-    def visit_alias(self, alias, asfrom=False, **kwargs):
-        if self.dialect._version_two:
-            return super(FBCompiler, self).visit_alias(
-                alias, asfrom=asfrom, **kwargs
+    def _handle_limit_fetch_clause(
+        self, fetch_clause, offset_clause, limit_clause, **kw
+    ):
+        # Albeit non-standard, ROWS is a better choice than OFFSET / FETCH in Firebird since
+        #   it is supported since Firebird 2.5 and it works with expressions.
+        # https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-dml-select-rows
+        text = ""
+
+        if (fetch_clause is not None) and (offset_clause is not None):
+            # OFFSET 2 ROWS FETCH NEXT 5 ROWS ONLY  =>  ROWS 2 + 1 TO 2 + 5
+            text += (
+                " \n ROWS "
+                + self.process(offset_clause, **kw)
+                + " + 1 TO "
+                + self.process(offset_clause, **kw)
+                + " + "
+                + self.process(fetch_clause, **kw)
+            )
+        elif (limit_clause is not None) and (offset_clause is not None):
+            # LIMIT 5 OFFSET 2  =>  ROWS 2 + 1 TO 2 + 5
+            text += (
+                " \n ROWS "
+                + self.process(offset_clause, **kw)
+                + " + 1 TO "
+                + self.process(offset_clause, **kw)
+                + " + "
+                + self.process(limit_clause, **kw)
+            )
+        elif fetch_clause is not None:
+            # FETCH NEXT 5 ROWS ONLY  =>  ROWS 1 TO 5
+            text += " \n ROWS 1 TO " + self.process(fetch_clause, **kw)
+        elif limit_clause is not None:
+            # LIMIT 5  =>  ROWS 1 TO 5
+            text += " \n ROWS 1 TO " + self.process(limit_clause, **kw)
+        elif offset_clause is not None:
+            # OFFSET 2 ROWS  =>  ROWS 2 + 1 TO 9223372036854775807
+            text += (
+                " \n ROWS "
+                + self.process(offset_clause, **kw)
+                + " + 1 TO 9223372036854775807"
             )
-        else:
-            # Override to not use the AS keyword which FB 1.5 does not like
-            if asfrom:
-                alias_name = (
-                    isinstance(alias.name, expression._truncated_label)
-                    and self._truncated_identifier("alias", alias.name)
-                    or alias.name
-                )
 
-                return (
-                    self.process(alias.element, asfrom=asfrom, **kwargs)
-                    + " "
-                    + self.preparer.format_alias(alias, alias_name)
-                )
-            else:
-                return self.process(alias.element, **kwargs)
+        return text
 
     def visit_substring_func(self, func, **kw):
         s = self.process(func.clauses.clauses[0])
         start = self.process(func.clauses.clauses[1])
         if len(func.clauses.clauses) > 2:
             length = self.process(func.clauses.clauses[2])
-            return "SUBSTRING(%s FROM %s FOR %s)" % (s, start, length)
-        else:
-            return "SUBSTRING(%s FROM %s)" % (s, start)
+            return f"SUBSTRING({s} FROM {start} FOR {length})"
 
-    def visit_length_func(self, function, **kw):
-        return "char_length" + self.function_argspec(function)
+        return f"SUBSTRING({s} FROM {start})"
 
-    visit_char_length_func = visit_length_func
+    def visit_truediv_binary(self, binary, operator, **kw):
+        return (
+            self.process(binary.left, **kw)
+            + " / "
+            + "(%s + 0.0)" % self.process(binary.right, **kw)
+        )
 
-    def function_argspec(self, func, **kw):
-        # TODO: this probably will need to be
-        # narrowed to a fixed list, some no-arg functions
-        # may require parens - see similar example in the oracle
-        # dialect
-        if func.clauses is not None and len(func.clauses):
-            return self.process(func.clause_expr, **kw)
-        else:
-            return ""
+    def visit_mod_binary(self, binary, operator, **kw):
+        return "MOD(%s, %s)" % (
+            self.process(binary.left, **kw),
+            self.process(binary.right, **kw),
+        )
 
-    def default_from(self):
-        return " FROM rdb$database"
+    def visit_now_func(self, fn, **kw):
+        return "CURRENT_TIMESTAMP"
 
-    def visit_sequence(self, seq, **kw):
-        return "gen_id(%s, 1)" % self.preparer.format_sequence(seq)
+    def function_argspec(self, fn, **kw):
+        if fn.clauses is not None and len(fn.clauses) > 0:
+            return self.process(fn.clause_expr, **kw)
 
-    def get_select_precolumns(self, select, **kw):
-        """
-        Called when building a ``SELECT`` statement, position is just
-        before column list Firebird puts the limit and offset right
-        after the ``SELECT``...
-
-        In Firebird, FIRST and SKIP require parentheses
-        for an integer expression.
-
-        Including parentheses for an integer literal or query parameter works,
-        even though they aren't needed,
-        """  # noqa
-        result = super(FBCompiler, self).get_select_precolumns(select, **kw)
-
-        if select._limit_clause is not None:
-            result += "FIRST (%s) " % self.process(select._limit_clause, **kw)
-        if select._offset_clause is not None:
-            result += "SKIP (%s) " % self.process(select._offset_clause, **kw)
+        return ""
 
-        return result
+    def visit_char_length_func(self, fn, **kw):
+        return "CHAR_LENGTH" + self.function_argspec(fn, **kw)
 
-    def limit_clause(self, select, **kw):
-        """Already taken care of in the `get_select_precolumns` method."""
-        return ""
+    def visit_length_func(self, fn, **kw):
+        return "CHAR_LENGTH" + self.function_argspec(fn, **kw)
 
-    def returning_clause(self, stmt, returning_cols):
+    def default_from(self):
+        return " FROM rdb$database"
+
+    def returning_clause(self, stmt, returning_cols, **kw):
+        if self.dialect.using_sqlalchemy2:
+            return super().returning_clause(stmt, returning_cols, **kw)
+
+        # For SQLAlchemy 1.4 compatibility only. Unneeded in 2.0.
         columns = [
-            self._label_select_column(None, c, True, False, {})
+            self._label_returning_column(stmt, c)
             for c in expression._select_iterables(returning_cols)
         ]
 
         return "RETURNING " + ", ".join(columns)
 
 
 class FBDDLCompiler(sql.compiler.DDLCompiler):
-    """Firebird syntactic idiosyncrasies"""
-
     def get_column_specification(self, column, **kwargs):
         colspec = self.preparer.format_column(column)
 
-        # FB is okay with or without an explicit type for a computed column.
-        # However, CompileTest.test_column_computed wants the type in there.
-        if column.computed is not None:
-            colspec += (
-                " " + str(column.type) + " " + self.process(column.computed)
-            )
-        else:
-            colspec += " " + self.dialect.type_compiler.process(
-                column.type, type_expression=column
-            )
+        impl_type = column.type.dialect_impl(self.dialect)
+        if isinstance(impl_type, sqltypes.TypeDecorator):
+            impl_type = impl_type.impl
+
+        has_identity = column.identity is not None
 
         if (
-            column is column.table._autoincrement_column
-            or column.autoincrement is True
-        ):
-            start = column.dialect_options["firebird"]["identity_start"]
-            colspec += " GENERATED BY DEFAULT AS IDENTITY (START WITH %s)" % (
-                start
+            column.primary_key
+            and column is column.table._autoincrement_column
+            and not has_identity
+            and (
+                column.default is None
+                or (
+                    isinstance(column.default, sa_schema.Sequence)
+                    and column.default.optional
+                )
             )
+            and self.dialect.supports_identity_columns
+        ):
+            colspec += " INTEGER GENERATED BY DEFAULT AS IDENTITY"
         else:
-            default = self.get_column_default_string(column)
-            if default is not None:
-                colspec += " DEFAULT " + default
-
-        if column.nullable is not None:
-            if (
-                not column.nullable
-                or column.primary_key
-                or isinstance(column.default, sa_schema.Sequence)
-                or column.autoincrement is True
-            ):
+            type_compiler_instance = (
+                self.dialect.type_compiler_instance
+                if self.dialect.using_sqlalchemy2
+                else self.dialect.type_compiler
+            )
+
+            colspec += " " + type_compiler_instance.process(
+                column.type,
+                type_expression=column,
+                identifier_preparer=self.preparer,
+            )
+            default_ = self.get_column_default_string(column)
+            if default_ is not None:
+                colspec += " DEFAULT " + default_
+
+            if column.computed is not None:
+                colspec += " " + self.process(column.computed)
+            if has_identity:
+                colspec += " " + self.process(column.identity)
+
+            if not column.nullable and not has_identity:
                 colspec += " NOT NULL"
+            elif column.nullable and has_identity:
+                colspec += " NULL"
 
         return colspec
 
-    def visit_create_sequence(self, create):
-        """Generate a ``CREATE GENERATOR`` statement for the sequence."""
-        # no syntax for these
-        # http://www.firebirdsql.org/manual/generatorguide-sqlsyntax.html
-        if create.element.start is not None:
-            raise NotImplementedError(
-                "Firebird SEQUENCE doesn't support START WITH"
-            )
-        if create.element.increment is not None:
-            raise NotImplementedError(
-                "Firebird SEQUENCE doesn't support INCREMENT BY"
-            )
+    def visit_create_index(
+        self, create, include_schema=False, include_table_schema=True, **kw
+    ):
+        preparer = self.preparer
+        index = create.element
+        self._verify_index_table(index)
 
-        if self.dialect._version_two:
-            return "CREATE SEQUENCE %s" % self.preparer.format_sequence(
-                create.element
+        if index.name is None:
+            raise exc.CompileError(
+                "CREATE INDEX requires that the index have a name."
             )
-        else:
-            return "CREATE GENERATOR %s" % self.preparer.format_sequence(
-                create.element
+
+        txt = "CREATE "
+        if index.unique:
+            txt += "UNIQUE "
+
+        txt += "INDEX %s ON %s " % (
+            self._prepared_index_name(index, include_schema=include_schema),
+            preparer.format_table(
+                index.table, use_schema=include_table_schema
+            ),
+        )
+
+        if index.expressions is None:
+            raise exc.CompileError(
+                "CREATE INDEX requires at least one column or expression."
             )
 
-    def visit_drop_sequence(self, drop):
-        """Generate a ``DROP GENERATOR`` statement for the sequence."""
-        if self.dialect._version_two:
-            return "DROP SEQUENCE %s" % self.preparer.format_sequence(
-                drop.element
+        first_expression = (
+            index.expressions[0]
+            if len(index.expressions) > 0
+            else index.expressions
+        )
+
+        if isinstance(first_expression, expression.ColumnClause):
+            # INDEX on columns
+            txt += ", ".join(
+                self.sql_compiler.process(
+                    expr, include_table=False, literal_binds=True
+                )
+                for expr in index.expressions
             )
         else:
-            return "DROP GENERATOR %s" % self.preparer.format_sequence(
-                drop.element
+            # INDEX on expression
+            txt += "COMPUTED BY (%s)" % EXPRESSION_SEPARATOR.join(
+                self.sql_compiler.process(
+                    expr, include_table=False, literal_binds=True
+                )
+                for expr in index.expressions
             )
+        return txt
+
+    def post_create_table(self, table):
+        table_opts = []
+        fb_opts = table.dialect_options[self.dialect.name]
+
+        if fb_opts["on_commit"]:
+            on_commit_options = fb_opts["on_commit"].replace("_", " ").upper()
+            table_opts.append("\n ON COMMIT %s" % on_commit_options)
 
-    def visit_computed_column(self, generated):
+        return "".join(table_opts)
+
+    def visit_computed_column(self, generated, **kw):
+        # TODO: Support GENERATED BY DEFAULT AS ...
         if generated.persisted is not None:
             raise exc.CompileError(
                 "Firebird computed columns do not support a persistence "
                 "method setting; set the 'persisted' flag to None for "
                 "Firebird support."
             )
         return "GENERATED ALWAYS AS (%s)" % self.sql_compiler.process(
             generated.sqltext, include_table=False, literal_binds=True
         )
 
-    def post_create_table(self, table):
-        table_opts = []
-        opts = table.dialect_options["firebird"]
+    def get_identity_options(self, identity_options):
+        txt = []
+        if identity_options.start is not None:
+            start = identity_options.start
+            if self.dialect.server_version_info < (4,):
+                # https://firebirdsql.org/file/documentation/release_notes/html/en/4_0/rlsnotes40.html#rnfb40-compat-sql-sequence-start-value
+                start -= (
+                    identity_options.increment
+                    if identity_options.increment is not None
+                    else 1
+                )
+            txt.append("START WITH %d" % start)
 
-        if opts["on_commit"]:
-            on_commit_options = opts["on_commit"].replace("_", " ").upper()
-            table_opts.append("\n ON COMMIT %s" % on_commit_options)
+        if identity_options.increment is not None:
+            txt.append("INCREMENT BY %d" % identity_options.increment)
 
-        return "".join(table_opts)
+        return " ".join(txt)
 
 
-class FBIdentifierPreparer(sql.compiler.IdentifierPreparer):
-    """Install Firebird specific reserved words."""
+class FBTypeCompiler(compiler.GenericTypeCompiler):
+    def visit_boolean(self, type_, **kw):
+        if self.dialect.server_version_info < (3,):
+            return self.visit_SMALLINT(type_, **kw)
+
+        return self.visit_BOOLEAN(type_, **kw)
+
+    def visit_datetime(self, type_, **kw):
+        return self.visit_TIMESTAMP(type_, **kw)
+
+    def visit_TEXT(self, type_, **kw):
+        return "BLOB SUB_TYPE 1"
 
-    reserved_words = RESERVED_WORDS
+    def visit_BLOB(self, type_, **kw):
+        return "BLOB SUB_TYPE 0"
+
+    def _render_string_type(self, type_, name, length_override=None):
+        text = name
+
+        length = (
+            length_override
+            if length_override
+            else getattr(type_, "length", None)
+        )
+        if length is not None:
+            text += f"({length})"
+
+        charset = getattr(type_, "charset", None)
+        if charset is not None:
+            text += f" CHARACTER SET {charset}"
+
+        collation = getattr(type_, "collation", None)
+        if collation is not None:
+            text += f" COLLATE {collation}"
+
+        return text
+
+    def visit_VARCHAR(self, type_, **kw):
+        if not type_.length:
+            raise exc.CompileError(
+                f"VARCHAR requires a length on dialect {self.dialect.name}."
+            )
+        return super().visit_VARCHAR(type_, **kw)
+
+    def visit_TIMESTAMP(self, type_, **kw):
+        if self.dialect.server_version_info < (4,):
+            return super().visit_TIMESTAMP(type_, **kw)
+
+        return "TIMESTAMP%s %s" % (
+            "(%d)" % type_.precision
+            if getattr(type_, "precision", None) is not None
+            else "",
+            (type_.timezone and "WITH" or "WITHOUT") + " TIME ZONE",
+        )
+
+    def visit_TIME(self, type_, **kw):
+        if self.dialect.server_version_info < (4,):
+            return super().visit_TIME(type_, **kw)
+
+        return "TIME%s %s" % (
+            "(%d)" % type_.precision
+            if getattr(type_, "precision", None) is not None
+            else "",
+            (type_.timezone and "WITH" or "WITHOUT") + " TIME ZONE",
+        )
+
+
+class FBIdentifierPreparer(sql.compiler.IdentifierPreparer):
     illegal_initial_characters = compiler.ILLEGAL_INITIAL_CHARACTERS.union(
         ["_"]
     )
 
     def __init__(self, dialect):
-        super(FBIdentifierPreparer, self).__init__(dialect, omit_schema=True)
+        super().__init__(dialect, omit_schema=True)
 
 
 class FBExecutionContext(default.DefaultExecutionContext):
     def fire_sequence(self, seq, type_):
-        """Get the next value from the sequence using ``gen_id()``."""
         return self._execute_scalar(
-            "SELECT gen_id(%s, 1) FROM rdb$database"
-            % self.dialect.identifier_preparer.format_sequence(seq),
+            (
+                "SELECT GEN_ID(%s, 1) FROM rdb$database"
+                % self.dialect.identifier_preparer.format_sequence(seq)
+            ),
             type_,
         )
 
 
 class FBDialect(default.DefaultDialect):
-    """Firebird dialect"""
-
-    name = "firebird"
-
-    """
-        Firebird version 4.0 and greater have a maximum identifier length of
-        63 characters character set UTF8 (252 bytes).  Prior versions have a
-        maximum identifier length of 31 bytes.
+    supports_alter = True
+    supports_sane_rowcount = True
+    supports_sane_multi_rowcount = False
 
-    max_identifier_length = 31
-
-    """
+    supports_native_boolean = True
+    supports_native_decimal = True
 
     supports_schemas = False
     supports_sequences = True
     sequences_optional = False
-    supports_default_values = True
     postfetch_lastrowid = False
+    use_insertmanyvalues = False
 
     supports_comments = True
-    inline_comments = True
-
-    supports_native_boolean = False
-
-    requires_name_normalize = True
-    supports_unicode_binds = True
-    supports_empty_insert = False
-
-    supports_statement_cache = True
+    inline_comments = False
+    supports_default_values = True
+    supports_default_metavalue = True
+    supports_identity_columns = True
 
     statement_compiler = FBCompiler
     ddl_compiler = FBDDLCompiler
+    type_compiler_cls = FBTypeCompiler
+    type_compiler = FBTypeCompiler  # For SQLAlchemy 1.4 compatibility only. Unneeded in 2.0.
     preparer = FBIdentifierPreparer
-    type_compiler = FBTypeCompiler
     execution_ctx_cls = FBExecutionContext
 
-    colspecs = colspecs
-    ischema_names = ischema_names
+    update_returning = True
+    delete_returning = True
+    insert_returning = True
+
+    requires_name_normalize = True
+    supports_unicode_binds = True
+    supports_empty_insert = False
+    supports_is_distinct_from = True
 
     construct_arguments = [
         (
             sa_schema.Table,
-            {"on_commit": None},
+            {
+                "on_commit": None,
+            },
         ),
-        (sa_schema.Column, {"identity_start": 0}),
     ]
 
-    # defaults to dialect ver. 3,
-    # will be autodetected off upon
-    # first connect
-    _version_two = True
+    using_sqlalchemy2 = version.parse(SQLALCHEMY_VERSION).major >= 2
 
     def initialize(self, connection):
-        super(FBDialect, self).initialize(connection)
-        self._version_two = (
-            "firebird" in self.server_version_info
-            and self.server_version_info >= (2,)
-        ) or (
-            "interbase" in self.server_version_info
-            and self.server_version_info >= (6,)
-        )
-
-        if not self._version_two:
-            # TODO: whatever other pre < 2.0 stuff goes here
-            self.ischema_names = ischema_names.copy()
-            self.ischema_names["TIMESTAMP"] = sqltypes.DATE
-            self.colspecs = {sqltypes.DateTime: sqltypes.DATE}
+        super().initialize(connection)
 
-        self.implicit_returning = self._version_two and self.__dict__.get(
-            "implicit_returning", True
-        )
-
-        if connection.connection.engine_version < 4.0:
-            self.max_identifier_length = 31
+        if self.server_version_info < (3,):
+            # Firebird 2.5
+            self.supports_identity_columns = False
+            self.supports_native_boolean = False
+
+            from .fb_info25 import (
+                MAX_IDENTIFIER_LENGTH,
+                RESERVED_WORDS,
+                ISCHEMA_NAMES,
+            )
+        elif self.server_version_info < (4,):
+            # Firebird 3.0
+            from .fb_info30 import (
+                MAX_IDENTIFIER_LENGTH,
+                RESERVED_WORDS,
+                ISCHEMA_NAMES,
+            )
         else:
-            self.max_identifier_length = 252
-
-    def has_table(self, connection, table_name, schema=None):
-        """Return ``True`` if the given table exists, ignoring the `schema`."""
+            # Firebird 4.0 or higher
+            from .fb_info40 import (
+                MAX_IDENTIFIER_LENGTH,
+                RESERVED_WORDS,
+                ISCHEMA_NAMES,
+            )
 
-        # Can't have a table whose name is too long.
-        if len(table_name) > self.max_identifier_length:
-            return False
+        self.max_identifier_length = MAX_IDENTIFIER_LENGTH
+        self.preparer.reserved_words = RESERVED_WORDS
+        self.ischema_names = ISCHEMA_NAMES
 
-        tblqry = text(
-            """
-            SELECT 1 AS has_table FROM rdb$database
-            WHERE EXISTS (SELECT rdb$relation_name
-                          FROM rdb$relations
-                          WHERE rdb$relation_name=:tbl_name)
-            """
-        )
-        c = connection.execute(
-            tblqry, {"tbl_name": self.denormalize_name(table_name)}
-        )
+    @reflection.cache
+    def has_table(self, connection, table_name, schema=None, **kw):
+        has_table_query = """
+            SELECT 1 AS has_table
+            FROM rdb$relations
+            WHERE rdb$relation_name = ?
+        """
+        tablename = self.denormalize_name(table_name)
+        c = connection.exec_driver_sql(has_table_query, (tablename,))
         return c.first() is not None
 
-    def has_sequence(self, connection, sequence_name, schema=None):
-        """Return ``True`` if the given sequence (generator) exists."""
-        genqry = """
-        SELECT 1 AS has_sequence FROM rdb$database
-        WHERE EXISTS (SELECT rdb$generator_name
-                      FROM rdb$generators
-                      WHERE rdb$generator_name=?)
+    @reflection.cache
+    def has_sequence(self, connection, sequence_name, schema=None, **kw):
+        has_sequence_query = """
+            SELECT 1 AS has_sequence 
+            FROM rdb$generators
+            WHERE rdb$generator_name = ?
         """
-        c = connection.exec_driver_sql(
-            genqry, (self.denormalize_name(sequence_name),)
-        )
+        sequencename = self.denormalize_name(sequence_name)
+        c = connection.exec_driver_sql(has_sequence_query, (sequencename,))
         return c.first() is not None
 
     @reflection.cache
     def get_table_names(self, connection, schema=None, **kw):
-        # there are two queries commonly mentioned for this.
-        # this one, using view_blr, is at the Firebird FAQ among other places:
-        # http://www.firebirdfaq.org/faq174/
-        s = """
-        select TRIM(rdb$relation_name) AS relation_name
-        from rdb$relations
-        where rdb$view_blr is null
-        and (rdb$system_flag is null or rdb$system_flag = 0)
-        and rdb$relation_type = 0;
+        tables_query = """
+            SELECT TRIM(rdb$relation_name) AS relation_name
+            FROM rdb$relations
+            WHERE rdb$relation_type IN (0 /* TABLE */)
+              AND COALESCE(rdb$system_flag, 0) = 0
+            ORDER BY rdb$relation_name
         """
 
-        # the other query is this one.  It's not clear if there's really
-        # any difference between these two.  This link:
-        # http://www.alberton.info/firebird_sql_meta_info.html#.Ur3vXfZGni8
-        # states them as interchangeable.  Some discussion at [ticket:2898]
-        # SELECT DISTINCT rdb$relation_name
-        # FROM rdb$relation_fields
-        # WHERE rdb$system_flag=0 AND rdb$view_context IS NULL
-
         return [
             self.normalize_name(row.relation_name)
-            for row in connection.exec_driver_sql(s)
+            for row in connection.exec_driver_sql(tables_query)
         ]
 
     @reflection.cache
     def get_temp_table_names(self, connection, schema=None, **kw):
-        s = """
-        select TRIM(rdb$relation_name) AS relation_name
-        from rdb$relations
-        where rdb$view_blr is null
-        and (rdb$system_flag is null or rdb$system_flag = 0)
-        and rdb$relation_type in (4, 5);
+        temp_tables_query = """
+            SELECT TRIM(rdb$relation_name) AS relation_name
+            FROM rdb$relations
+            WHERE rdb$relation_type IN (4 /* TEMPORARY_TABLE_PRESERVE */, 
+                                        5 /* TEMPORARY_TABLE_DELETE */)
+              AND COALESCE(rdb$system_flag, 0) = 0
+            ORDER BY rdb$relation_name
         """
         return [
             self.normalize_name(row.relation_name)
-            for row in connection.exec_driver_sql(s)
+            for row in connection.exec_driver_sql(temp_tables_query)
         ]
 
     @reflection.cache
-    def get_sequence_names(self, connection, schema=None, **kw):
-        s = """
-        select TRIM(rdb$generator_name) AS generator_name
-        from rdb$generators
-        where (rdb$system_flag is null or rdb$system_flag = 0);
+    def get_view_names(self, connection, schema=None, **kw):
+        views_query = """
+            SELECT TRIM(rdb$relation_name) AS relation_name
+            FROM rdb$relations
+            WHERE rdb$relation_type IN (1 /* VIEW */)
+              AND COALESCE(rdb$system_flag, 0) = 0
+            ORDER BY rdb$relation_name
         """
         return [
-            self.normalize_name(row.generator_name)
-            for row in connection.exec_driver_sql(s)
+            self.normalize_name(row.relation_name)
+            for row in connection.exec_driver_sql(views_query)
         ]
 
     @reflection.cache
-    def get_view_names(self, connection, schema=None, **kw):
-        # see http://www.firebirdfaq.org/faq174/
-        s = """
-        select TRIM(rdb$relation_name) AS relation_name
-        from rdb$relations
-        where rdb$view_blr is not null
-        and (rdb$system_flag is null or rdb$system_flag = 0);
+    def get_sequence_names(self, connection, schema=None, **kw):
+        sequences_query = """
+            SELECT TRIM(rdb$generator_name) AS generator_name
+            FROM rdb$generators
+            WHERE COALESCE(rdb$system_flag, 0) = 0
         """
+        # Do not need ORDER BY
         return [
-            self.normalize_name(row.relation_name)
-            for row in connection.exec_driver_sql(s)
+            self.normalize_name(row.generator_name)
+            for row in connection.exec_driver_sql(sequences_query)
         ]
 
     @reflection.cache
     def get_view_definition(self, connection, view_name, schema=None, **kw):
-        qry = """
-        SELECT rdb$view_source AS view_source
-        FROM rdb$relations
-        WHERE rdb$relation_name=?
+        view_query = """
+            SELECT rdb$view_source AS view_source
+            FROM rdb$relations
+            WHERE rdb$relation_type IN (1 /* VIEW */)
+              AND rdb$relation_name = ?
         """
-        rp = connection.exec_driver_sql(
-            qry, (self.denormalize_name(view_name),)
-        )
-        row = rp.first()
+        viewname = self.denormalize_name(view_name)
+        c = connection.exec_driver_sql(view_query, (viewname,))
+        row = c.fetchone()
         if row:
             return row.view_source
-        else:
-            return None
 
-    @reflection.cache
-    def get_pk_constraint(self, connection, table_name, schema=None, **kw):
-        # Query to extract the PK/FK constrained fields of the given table
-        keyqry = """
-        SELECT TRIM(se.rdb$field_name) AS fname
-        FROM rdb$relation_constraints rc
-             JOIN rdb$index_segments se ON rc.rdb$index_name=se.rdb$index_name
-        WHERE rc.rdb$constraint_type=? AND rc.rdb$relation_name=?
-        """
-        tablename = self.denormalize_name(table_name)
-        # get primary key fields
-        c = connection.exec_driver_sql(keyqry, ("PRIMARY KEY", tablename))
-        pkfields = [self.normalize_name(r.fname) for r in c.fetchall()]
-        return {"constrained_columns": pkfields, "name": None}
-
-    @reflection.cache
-    def get_column_sequence(
-        self, connection, table_name, column_name, schema=None, **kw
-    ):
-        tablename = self.denormalize_name(table_name)
-        colname = self.denormalize_name(column_name)
-        # Heuristic-query to determine the generator associated to a PK field
-        genqry = """
-        SELECT trigdep.rdb$depended_on_name AS fgenerator
-        FROM rdb$dependencies tabdep
-             JOIN rdb$dependencies trigdep
-                  ON tabdep.rdb$dependent_name=trigdep.rdb$dependent_name
-                     AND trigdep.rdb$depended_on_type=14
-                     AND trigdep.rdb$dependent_type=2
-             JOIN rdb$triggers trig ON
-                    trig.rdb$trigger_name=tabdep.rdb$dependent_name
-        WHERE tabdep.rdb$depended_on_name=?
-          AND tabdep.rdb$depended_on_type=0
-          AND trig.rdb$trigger_type=1
-          AND tabdep.rdb$field_name=?
-          AND (SELECT count(*)
-           FROM rdb$dependencies trigdep2
-           WHERE trigdep2.rdb$dependent_name = trigdep.rdb$dependent_name) = 2
-        """
-        genr = connection.exec_driver_sql(genqry, (tablename, colname)).first()
-        if genr is not None:
-            return dict(name=self.normalize_name(genr.fgenerator))
+        raise exc.NoSuchTableError(view_name)
 
     @reflection.cache
     def get_columns(  # noqa: C901
         self, connection, table_name, schema=None, **kw
     ):
-        # Query to extract the details of all the fields of the given table
-        tblqry = """
-        SELECT TRIM(r.rdb$field_name) AS fname,
-                        r.rdb$null_flag AS null_flag,
-                        t.rdb$type_name AS ftype,
-                        f.rdb$field_sub_type AS stype,
-                        f.rdb$field_length/
-                            COALESCE(cs.rdb$bytes_per_character,1) AS flen,
-                        f.rdb$field_precision AS fprec,
-                        f.rdb$field_scale AS fscale,
-                        COALESCE(r.rdb$default_source,
-                                f.rdb$default_source) AS fdefault,
-                        f.rdb$computed_source AS computed_source
-        FROM rdb$relation_fields r
-             JOIN rdb$fields f ON r.rdb$field_source=f.rdb$field_name
-             JOIN rdb$types t
-              ON t.rdb$type=f.rdb$field_type AND
-                    t.rdb$field_name='RDB$FIELD_TYPE'
-             LEFT JOIN rdb$character_sets cs ON
-                    f.rdb$character_set_id=cs.rdb$character_set_id
-        WHERE f.rdb$system_flag=0 AND r.rdb$relation_name=?
-        ORDER BY r.rdb$field_position
-        """
-        # get the PK, used to determine the eventual associated sequence
-        pk_constraint = self.get_pk_constraint(connection, table_name)
-        pkey_cols = pk_constraint["constrained_columns"]
+        is_firebird_25 = self.server_version_info < (3,)
+
+        columns_query = """
+            SELECT TRIM(r.rdb$field_name) AS fname,
+                   r.rdb$null_flag AS null_flag,
+                   t.rdb$type_name AS ftype,
+                   f.rdb$field_sub_type AS stype,
+                   f.rdb$field_length / COALESCE(cs.rdb$bytes_per_character, 1) AS flen,
+                   f.rdb$field_precision AS fprec,
+                   f.rdb$field_scale AS fscale,
+                   COALESCE(r.rdb$default_source, f.rdb$default_source) AS fdefault,
+                   TRIM(r.rdb$description) AS fcomment,
+                   f.rdb$computed_source AS computed_source,
+                   r.rdb$identity_type AS identity_type,
+                   g.rdb$initial_value AS identity_start,
+                   g.rdb$generator_increment AS identity_increment
+            FROM rdb$relation_fields r
+                 JOIN rdb$fields f
+                   ON f.rdb$field_name = r.rdb$field_source
+                 JOIN rdb$types t
+                   ON t.rdb$type = f.rdb$field_type 
+                  AND t.rdb$field_name = 'RDB$FIELD_TYPE'
+                 LEFT JOIN rdb$character_sets cs
+                        ON cs.rdb$character_set_id = f.rdb$character_set_id
+                 LEFT JOIN rdb$generators g
+                        ON g.rdb$generator_name = r.rdb$generator_name
+            WHERE f.rdb$system_flag = 0 
+              AND r.rdb$relation_name = ?
+            ORDER BY r.rdb$field_position
+        """
+
+        if is_firebird_25:
+            # Firebird 2.5 doesn't have RDB$GENERATOR_NAME nor RDB$IDENTITY_TYPE in RDB$RELATION_FIELDS
+            columns_query = """
+                SELECT TRIM(r.rdb$field_name) AS fname,
+                       r.rdb$null_flag AS null_flag,
+                       t.rdb$type_name AS ftype,
+                       f.rdb$field_sub_type AS stype,
+                       f.rdb$field_length / COALESCE(cs.rdb$bytes_per_character, 1) AS flen,
+                       f.rdb$field_precision AS fprec,
+                       f.rdb$field_scale AS fscale,
+                       COALESCE(r.rdb$default_source, f.rdb$default_source) AS fdefault,
+                       TRIM(r.rdb$description) AS fcomment,
+                       f.rdb$computed_source AS computed_source
+                FROM rdb$relation_fields r
+                     JOIN rdb$fields f 
+                       ON f.rdb$field_name = r.rdb$field_source
+                     JOIN rdb$types t
+                       ON t.rdb$type = f.rdb$field_type
+                      AND t.rdb$field_name = 'RDB$FIELD_TYPE'
+                      LEFT JOIN rdb$character_sets cs
+                             ON cs.rdb$character_set_id = f.rdb$character_set_id
+                WHERE f.rdb$system_flag = 0
+                  AND r.rdb$relation_name = ?
+                ORDER BY r.rdb$field_position
+            """
 
         tablename = self.denormalize_name(table_name)
-        # get all of the fields for this table
-        c = [row for row in connection.exec_driver_sql(tblqry, (tablename,))]
+        c = list(connection.exec_driver_sql(columns_query, (tablename,)))
+
         cols = []
         for row in c:
             name = self.normalize_name(row.fname)
-            orig_colname = row.fname
 
-            # get the data type
+            # Extract data type
             colspec = row.ftype.rstrip()
             coltype = self.ischema_names.get(colspec)
             if coltype is None:
                 util.warn(
                     "Did not recognize type '%s' of column '%s'"
                     % (colspec, name)
                 )
@@ -937,142 +631,357 @@
             elif issubclass(coltype, Integer) and row.fprec != 0:
                 coltype = NUMERIC(precision=row.fprec, scale=row.fscale * -1)
             elif colspec in ("VARYING", "CSTRING"):
                 coltype = coltype(row.flen)
             elif colspec == "TEXT":
                 coltype = TEXT(row.flen)
             elif colspec == "BLOB":
-                if row.stype == 1:
-                    coltype = TEXT()
-                else:
-                    coltype = BLOB()
+                coltype = TEXT() if row.stype == 1 else BLOB()
             else:
                 coltype = coltype()
 
-            # does it have a default value?
+            # Extract default value
             defvalue = None
             if row.fdefault is not None:
                 # the value comes down as "DEFAULT 'value'": there may be
                 # more than one whitespace around the "DEFAULT" keyword
                 # and it may also be lower case
                 # (see also http://tracker.firebirdsql.org/browse/CORE-356)
                 defexpr = row.fdefault.lstrip()
                 assert defexpr[:8].rstrip().upper() == "DEFAULT", (
                     "Unrecognized default value: %s" % defexpr
                 )
                 defvalue = defexpr[8:].strip()
-                if defvalue == "NULL":
-                    # Redundant
-                    defvalue = None
+                defvalue = defvalue if defvalue != "NULL" else None
+
             col_d = {
                 "name": name,
                 "type": coltype,
                 "nullable": not bool(row.null_flag),
                 "default": defvalue,
-                "autoincrement": "auto",
             }
 
+            orig_colname = row.fname
             if orig_colname.lower() == orig_colname:
                 col_d["quote"] = True
 
             if row.computed_source is not None:
                 col_d["computed"] = {"sqltext": row.computed_source}
 
-            # if the PK is a single field, try to see if its linked to
-            # a sequence thru a trigger
-            if len(pkey_cols) == 1 and name == pkey_cols[0]:
-                seq_d = self.get_column_sequence(connection, tablename, name)
-                if seq_d is not None:
-                    col_d["sequence"] = seq_d
+            if row.fcomment is not None:
+                col_d["comment"] = row.fcomment
+
+            if (not is_firebird_25) and row.identity_type is not None:
+                col_d["identity"] = {
+                    "always": row.identity_type == 0,
+                    "start": row.identity_start,
+                    "increment": row.identity_increment,
+                }
+
+            if not self.using_sqlalchemy2:
+                # For SQLAlchemy 1.4 compatibility only. Unneeded in 2.0.
+                col_d["autoincrement"] = "auto"
 
             cols.append(col_d)
-        return cols
+
+        if cols:
+            return cols
+
+        if not self.has_table(connection, table_name, schema):
+            raise exc.NoSuchTableError(table_name)
+
+        return (
+            reflection.ReflectionDefaults.columns()
+            if self.using_sqlalchemy2
+            else []
+        )
+
+    @reflection.cache
+    def get_pk_constraint(self, connection, table_name, schema=None, **kw):
+        pk_query = """
+            SELECT TRIM(se.rdb$field_name) AS fname
+            FROM rdb$relation_constraints rc
+                 JOIN rdb$index_segments se
+                   ON se.rdb$index_name = rc.rdb$index_name
+            WHERE rc.rdb$constraint_type = 'PRIMARY KEY'
+              AND rc.rdb$relation_name = ?
+            ORDER BY se.rdb$field_position
+        """
+        tablename = self.denormalize_name(table_name)
+        c = connection.exec_driver_sql(pk_query, (tablename,))
+
+        pkfields = [self.normalize_name(r.fname) for r in c.fetchall()]
+        if pkfields:
+            return {"constrained_columns": pkfields, "name": None}
+
+        if not self.has_table(connection, table_name, schema):
+            raise exc.NoSuchTableError(table_name)
+
+        return (
+            reflection.ReflectionDefaults.pk_constraint()
+            if self.using_sqlalchemy2
+            else {"constrained_columns": [], "name": None}
+        )
 
     @reflection.cache
     def get_foreign_keys(self, connection, table_name, schema=None, **kw):
-        # Query to extract the details of each UK/FK of the given table
-        fkqry = """
-        SELECT TRIM(rc.rdb$constraint_name) AS cname,
-               TRIM(cse.rdb$field_name) AS fname,
-               TRIM(ix2.rdb$relation_name) AS targetrname,
-               TRIM(se.rdb$field_name) AS targetfname
-        FROM rdb$relation_constraints rc
-             JOIN rdb$indices ix1 ON ix1.rdb$index_name=rc.rdb$index_name
-             JOIN rdb$indices ix2 ON ix2.rdb$index_name=ix1.rdb$foreign_key
-             JOIN rdb$index_segments cse ON
-                        cse.rdb$index_name=ix1.rdb$index_name
-             JOIN rdb$index_segments se
-                  ON se.rdb$index_name=ix2.rdb$index_name
-                     AND se.rdb$field_position=cse.rdb$field_position
-        WHERE rc.rdb$constraint_type=? AND rc.rdb$relation_name=?
-        ORDER BY se.rdb$index_name, se.rdb$field_position
+        fk_query = """
+            SELECT TRIM(rc.rdb$constraint_name) AS cname,
+                   TRIM(cse.rdb$field_name) AS fname,
+                   TRIM(ix2.rdb$relation_name) AS targetrname,
+                   TRIM(se.rdb$field_name) AS targetfname,
+                   TRIM(rfc.rdb$update_rule) AS update_rule,
+                   TRIM(rfc.rdb$delete_rule) AS delete_rule
+            FROM rdb$relation_constraints rc
+                 JOIN rdb$ref_constraints rfc 
+                   ON rfc.rdb$constraint_name = rc.rdb$constraint_name
+                 JOIN rdb$indices ix1 
+                   ON ix1.rdb$index_name = rc.rdb$index_name
+                 JOIN rdb$indices ix2 
+                   ON ix2.rdb$index_name = ix1.rdb$foreign_key
+                 JOIN rdb$index_segments cse 
+                   ON cse.rdb$index_name = ix1.rdb$index_name
+                 JOIN rdb$index_segments se 
+                   ON se.rdb$index_name = ix2.rdb$index_name
+                  AND se.rdb$field_position = cse.rdb$field_position
+            WHERE rc.rdb$constraint_type = 'FOREIGN KEY'
+              AND rc.rdb$relation_name = ?
+            ORDER BY rc.rdb$constraint_name, se.rdb$field_position
         """
         tablename = self.denormalize_name(table_name)
+        c = connection.exec_driver_sql(fk_query, (tablename,))
 
-        c = connection.exec_driver_sql(fkqry, ("FOREIGN KEY", tablename))
         fks = util.defaultdict(
             lambda: {
                 "name": None,
                 "constrained_columns": [],
                 "referred_schema": None,
                 "referred_table": None,
                 "referred_columns": [],
+                "options": {},
             }
         )
 
         for row in c:
             cname = self.normalize_name(row.cname)
             fk = fks[cname]
             if not fk["name"]:
                 fk["name"] = cname
                 fk["referred_table"] = self.normalize_name(row.targetrname)
             fk["constrained_columns"].append(self.normalize_name(row.fname))
             fk["referred_columns"].append(self.normalize_name(row.targetfname))
-        return list(fks.values())
+            if row.update_rule not in ["NO ACTION", "RESTRICT"]:
+                fk["options"]["onupdate"] = row.update_rule
+            if row.delete_rule not in ["NO ACTION", "RESTRICT"]:
+                fk["options"]["ondelete"] = row.delete_rule
+
+        result = list(fks.values())
+        if result:
+            return result
+
+        if not self.has_table(connection, table_name, schema):
+            raise exc.NoSuchTableError(table_name)
+
+        return (
+            reflection.ReflectionDefaults.foreign_keys()
+            if self.using_sqlalchemy2
+            else []
+        )
 
     @reflection.cache
     def get_indexes(self, connection, table_name, schema=None, **kw):
-        qry = """
-        SELECT TRIM(ix.rdb$index_name) AS index_name,
-               ix.rdb$unique_flag AS unique_flag,
-               TRIM(ic.rdb$field_name) AS field_name
-        FROM rdb$indices ix
-             JOIN rdb$index_segments ic
-                  ON ix.rdb$index_name=ic.rdb$index_name
-             LEFT OUTER JOIN rdb$relation_constraints
-                  ON rdb$relation_constraints.rdb$index_name =
-                        ic.rdb$index_name
-        WHERE ix.rdb$relation_name=? AND ix.rdb$foreign_key IS NULL
-          AND rdb$relation_constraints.rdb$constraint_type IS NULL
-        ORDER BY index_name, ic.rdb$field_position
+        indexes_query = """
+            SELECT TRIM(ix.rdb$index_name) AS index_name,
+                   ix.rdb$unique_flag AS unique_flag,
+                   TRIM(ic.rdb$field_name) AS field_name,
+                   TRIM(ix.rdb$expression_source) expression_source
+            FROM rdb$indices ix
+                LEFT OUTER JOIN rdb$index_segments ic
+                  ON ic.rdb$index_name = ix.rdb$index_name
+                LEFT OUTER JOIN rdb$relation_constraints rc
+                             ON rc.rdb$index_name = ic.rdb$index_name
+            WHERE ix.rdb$relation_name = :relation_name
+              AND ix.rdb$foreign_key IS NULL
+              AND COALESCE(rc.rdb$constraint_type, '') <> 'PRIMARY KEY'
+            ORDER BY ix.rdb$index_name, ic.rdb$field_position
         """
-        c = connection.exec_driver_sql(
-            qry, (self.denormalize_name(table_name),)
+        tablename = self.denormalize_name(table_name)
+
+        # Do not use connection.exec_driver_sql() here.
+        #    During tests we need to commit CREATE INDEX before this query. See provision.py listener.
+        c = connection.execute(
+            text(indexes_query), {"relation_name": tablename}
         )
 
         indexes = util.defaultdict(dict)
         for row in c:
             indexrec = indexes[row.index_name]
             if "name" not in indexrec:
                 indexrec["name"] = self.normalize_name(row.index_name)
                 indexrec["column_names"] = []
+                indexrec["dialect_options"] = {}
                 indexrec["unique"] = bool(row.unique_flag)
+                if row.expression_source is not None:
+                    expr = row.expression_source[
+                        1:-1
+                    ]  # Remove outermost parenthesis added by Firebird
+                    indexrec["expressions"] = expr.split(EXPRESSION_SEPARATOR)
 
             indexrec["column_names"].append(
                 self.normalize_name(row.field_name)
             )
 
-        return list(indexes.values())
+        def _get_column_set(tablename):
+            colqry = """
+                SELECT TRIM(r.rdb$field_name) AS fname
+                FROM rdb$relation_fields r
+                WHERE r.rdb$relation_name = ?
+            """
+            return {
+                self.normalize_name(row.fname)
+                for row in connection.exec_driver_sql(colqry, (tablename,))
+            }
+
+        def _adjust_column_names_for_expressions(result, tablename):
+            # Identify which expression elements are columns
+            colset = _get_column_set(tablename)
+            for i in result:
+                expr = i.get("expressions")
+                if expr is not None:
+                    i["column_names"] = [
+                        x if self.normalize_name(x) in colset else None
+                        for x in expr
+                    ]
+            return result
+
+        result = list(indexes.values())
+        if result:
+            return _adjust_column_names_for_expressions(result, tablename)
+
+        if not self.has_table(connection, table_name, schema):
+            raise exc.NoSuchTableError(table_name)
+
+        return (
+            reflection.ReflectionDefaults.indexes()
+            if self.using_sqlalchemy2
+            else []
+        )
+
+    @reflection.cache
+    def get_unique_constraints(
+        self, connection, table_name, schema=None, **kw
+    ):
+        unique_constraints_query = """
+            SELECT TRIM(rc.rdb$constraint_name) AS cname,
+                   TRIM(se.rdb$field_name) AS column_name
+            FROM rdb$index_segments se
+                 JOIN rdb$relation_constraints rc
+                   ON rc.rdb$index_name = se.rdb$index_name
+                 JOIN rdb$relations r
+                   ON r.rdb$relation_name = rc.rdb$relation_name
+                  AND r.rdb$system_flag = 0
+            WHERE rc.rdb$constraint_type = 'UNIQUE' AND
+                  r.rdb$relation_name = ?
+            ORDER BY rc.rdb$constraint_name, se.rdb$field_position
+        """
+        tablename = self.denormalize_name(table_name)
+        c = connection.exec_driver_sql(unique_constraints_query, (tablename,))
+
+        ucs = util.defaultdict(lambda: {"name": None, "column_names": []})
+
+        for row in c:
+            cname = self.normalize_name(row.cname)
+            cc = ucs[cname]
+            if not cc["name"]:
+                cc["name"] = cname
+            cc["column_names"].append(self.normalize_name(row.column_name))
+
+        result = list(ucs.values())
+        if result:
+            return result
+
+        if not self.has_table(connection, table_name, schema):
+            raise exc.NoSuchTableError(table_name)
+
+        return (
+            reflection.ReflectionDefaults.unique_constraints()
+            if self.using_sqlalchemy2
+            else []
+        )
 
     @reflection.cache
     def get_table_comment(self, connection, table_name, schema=None, **kw):
-        qry = text(
-            """
-            SELECT RDB$DESCRIPTION AS comment
+        table_comment_query = """
+            SELECT TRIM(rdb$description) AS comment
             FROM rdb$relations
-            WHERE rdb$relation_name=:tbl_name
-            """
-        )
-        c = connection.execute(
-            qry, {"tbl_name": self.denormalize_name(table_name)}
+            WHERE rdb$relation_name = ?
+        """
+        tablename = self.denormalize_name(table_name)
+        c = connection.exec_driver_sql(table_comment_query, (tablename,))
+
+        row = c.fetchone()
+        if row:
+            return {"text": row[0]}
+
+        raise exc.NoSuchTableError(table_name)
+
+    @reflection.cache
+    def get_check_constraints(self, connection, table_name, schema=None, **kw):
+        check_constraints_query = """
+            SELECT TRIM(rc.rdb$constraint_name) AS cname,
+                   TRIM(SUBSTRING(tr.rdb$trigger_source FROM 8 FOR CHAR_LENGTH(tr.rdb$trigger_source) - 8)) AS sqltext
+            FROM rdb$relation_constraints rc
+                 JOIN rdb$check_constraints ck
+                   ON ck.rdb$constraint_name = rc.rdb$constraint_name
+                 JOIN rdb$triggers tr
+                   ON tr.rdb$trigger_name = ck.rdb$trigger_name AND
+                      tr.rdb$trigger_type = 1 /* BEFORE UPDATE */
+            WHERE rc.rdb$constraint_type = 'CHECK' AND
+                  rc.rdb$relation_name = ?
+            ORDER BY rc.rdb$constraint_name
+        """
+        tablename = self.denormalize_name(table_name)
+        c = connection.exec_driver_sql(check_constraints_query, (tablename,))
+
+        ccs = util.defaultdict(
+            lambda: {
+                "name": None,
+                "sqltext": None,
+            }
         )
-        return {"text": c.scalar()}
+
+        for row in c:
+            cname = self.normalize_name(row.cname)
+            cc = ccs[cname]
+            if not cc["name"]:
+                cc["name"] = cname
+                cc["sqltext"] = row.sqltext
+
+        result = list(ccs.values())
+        if result:
+            return result
+
+        if not self.has_table(connection, table_name, schema):
+            raise exc.NoSuchTableError(table_name)
+
+        return (
+            reflection.ReflectionDefaults.check_constraints()
+            if self.using_sqlalchemy2
+            else []
+        )
+
+    def is_disconnect(self, e, connection, cursor):
+        if isinstance(
+            e, (self.dbapi.OperationalError, self.dbapi.ProgrammingError)
+        ):
+            # TODO: Review these messages for Firebird 3+
+            for msg in (
+                "Error writing data to the connection",
+                "Unable to complete network request to host",
+                "Invalid connection state",
+                "Invalid cursor state",
+                "connection shutdown",
+            ):
+                if msg in str(e):
+                    return True
+
+        return False
```

### Comparing `sqlalchemy-firebird-0.8.0/sqlalchemy_firebird.egg-info/PKG-INFO` & `sqlalchemy-firebird-2.0.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-firebird
-Version: 0.8.0
+Version: 2.0.0
 Summary: Firebird for SQLAlchemy
 Home-page: https://github.com/pauldex/sqlalchemy-firebird
 Author: Paul Graves-DesLauriers
 Author-email: paul@dexmicro.com
 License: MIT
 Project-URL: Documentation, https://github.com/pauldex/sqlalchemy-firebird/wiki
 Project-URL: Source, https://github.com/pauldex/sqlalchemy-firebird
@@ -14,49 +14,72 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Database :: Front-Ends
 Classifier: Operating System :: OS Independent
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 sqlalchemy-firebird
 ###################
 
 An external SQLAlchemy dialect for Firebird
 ===========================================
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
 .. image:: https://github.com/pauldex/sqlalchemy-firebird/workflows/sqlalchemy-firebird/badge.svg
     :target: https://github.com/pauldex/sqlalchemy-firebird
 
 ----
 
-| This replaces SQLAlchemy's internal Firebird dialect which is not being maintained
- and will be removed in a future version.
+| This package provides a `Firebird <https://firebirdsql.org/en/start/>`_ dialect for `SQLAlchemy <https://www.sqlalchemy.org>`_ using the `firebird-driver <https://firebird-driver.readthedocs.io/en/latest>`_ and/or `fdb <https://fdb.readthedocs.io/en/latest>`_ driver.
 
 ****
 
 **Installation**
 
 ::
 
     pip install sqlalchemy-firebird
 
-|
-|  Connection URI samples for Firebird server installed on local machine using default port (3050):
+If you are using Python 3.8 or greater, SQLAlchemy 2.0+ and firebird-driver will be automatically installed.
+Python 3.6 and 3.7 will automatically install and use SQLAlchemy < 2.0 and fdb instead.
+
+Connection URI samples for Firebird server installed on local machine using default port (3050):
 
 ::
 
     [Linux]
-    firebird://username:password@localhost///home/paulgd/projects/databases/my_project.fdb
+    # Use the fdb driver (Python 3.6/3.7)
+    firebird+fdb://username:password@localhost///home/testuser/projects/databases/my_project.fdb
+    # Use the firebird-driver driver (Python 3.8+)
+    firebird+firebird://username:password@localhost///home/testuser/projects/databases/my_project.fdb
 
     [Windows]
-    firebird://username:password@localhost/c:/projects/databases/my_project.fdb
+    # Use the fdb driver (Python 3.6/3.7)
+    firebird+fdb://username:password@localhost/c:/projects/databases/my_project.fdb
+    # Use the firebird-driver driver (Python 3.8+)
+    firebird+firebird://username:password@localhost/c:/projects/databases/my_project.fdb
+
+****
+
+**Usage**
+
+For example, to connect to a Firebird server installed on a local Windows machine using the default port and firebird-driver:
+
+::
+
+    db_uri = "firebird+firebird://username:password@localhost/c:/projects/databases/my_project.fdb"
+    from sqlalchemy import create_engine
+    engine = create_engine(db_uri, echo=True)
+
+Connecting to different types of Firebird servers, databases, or drivers is done simply by changing the db_uri string
+used in the call to create_engine.
 
 ----
 
 **Code of Conduct**
 
 As with SQLAlchemy, sqlalchemy-firebird places great emphasis on polite, thoughtful, and
 constructive communication between users and developers.
```

### Comparing `sqlalchemy-firebird-0.8.0/sqlalchemy_firebird.egg-info/SOURCES.txt` & `sqlalchemy-firebird-2.0.0/sqlalchemy_firebird.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 LICENSE
 README.rst
 pyproject.toml
 setup.cfg
 setup.py
 sqlalchemy_firebird/__init__.py
 sqlalchemy_firebird/base.py
+sqlalchemy_firebird/fb_info25.py
+sqlalchemy_firebird/fb_info30.py
+sqlalchemy_firebird/fb_info40.py
 sqlalchemy_firebird/fdb.py
-sqlalchemy_firebird/kinterbasdb.py
+sqlalchemy_firebird/firebird.py
 sqlalchemy_firebird/provision.py
 sqlalchemy_firebird/requirements.py
+sqlalchemy_firebird/types.py
 sqlalchemy_firebird.egg-info/PKG-INFO
 sqlalchemy_firebird.egg-info/SOURCES.txt
 sqlalchemy_firebird.egg-info/dependency_links.txt
 sqlalchemy_firebird.egg-info/entry_points.txt
 sqlalchemy_firebird.egg-info/not-zip-safe
 sqlalchemy_firebird.egg-info/requires.txt
 sqlalchemy_firebird.egg-info/top_level.txt
 test/test_domain_reflection.py
-test/test_fb_argument.py
 test/test_fb_compile.py
 test/test_fb_misc.py
 test/test_fb_types.py
 test/test_suite.py
```

### Comparing `sqlalchemy-firebird-0.8.0/test/test_domain_reflection.py` & `sqlalchemy-firebird-2.0.0/test/test_domain_reflection.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-firebird-0.8.0/test/test_fb_compile.py` & `sqlalchemy-firebird-2.0.0/test/test_fb_compile.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,39 +16,30 @@
 from sqlalchemy import update
 from sqlalchemy import VARCHAR
 from sqlalchemy.sql import sqltypes
 from sqlalchemy.testing import assert_raises_message
 from sqlalchemy.testing import AssertsCompiledSQL
 from sqlalchemy.testing import fixtures
 
-from sqlalchemy_firebird import fdb as firebird
-from sqlalchemy_firebird import base as fb_base
+import sqlalchemy_firebird.types as FbTypes
+
 from sqlalchemy_firebird.fdb import FBDialect_fdb
 
 
 class CompileTest(fixtures.TablesTest, AssertsCompiledSQL):
-
     __dialect__ = FBDialect_fdb()
 
     def test_alias(self):
         t = table("sometable", column("col1"), column("col2"))
         s = select(t.alias())
         self.assert_compile(
             s,
             "SELECT sometable_1.col1, sometable_1.col2 "
             "FROM sometable AS sometable_1",
         )
-        dialect = self.__dialect__
-        dialect._version_two = False
-        self.assert_compile(
-            s,
-            "SELECT sometable_1.col1, sometable_1.col2 "
-            "FROM sometable sometable_1",
-            dialect=dialect,
-        )
 
     def test_varchar_raise(self):
         for type_ in (
             String,
             VARCHAR,
             String(),
             VARCHAR(),
@@ -126,15 +117,15 @@
             update(table1)
             .values(dict(name="foo"))
             .returning(func.length(table1.c.name))
         )
         self.assert_compile(
             u,
             "UPDATE mytable SET name=:name RETURNING "
-            "char_length(mytable.name) AS length_1",
+            "CHAR_LENGTH(mytable.name) AS length_1",
         )
 
     def test_insert_returning(self):
         table1 = table(
             "mytable",
             column("myid", Integer),
             column("name", String(128)),
@@ -161,31 +152,31 @@
             insert(table1)
             .values(dict(name="foo"))
             .returning(func.length(table1.c.name))
         )
         self.assert_compile(
             i,
             "INSERT INTO mytable (name) VALUES (:name) "
-            "RETURNING char_length(mytable.name) AS "
+            "RETURNING CHAR_LENGTH(mytable.name) AS "
             "length_1",
         )
 
     def test_charset(self):
-        """Exercise CHARACTER SET  options on string types."""
+        """Exercise CHARACTER SET options on string types."""
         columns = [
-            (fb_base.CHAR, [1], {}, "CHAR(1)"),
+            (FbTypes.CHAR, [1], {}, "CHAR(1)"),
             (
-                fb_base.CHAR,
+                FbTypes.CHAR,
                 [1],
                 {"charset": "OCTETS"},
                 "CHAR(1) CHARACTER SET OCTETS",
             ),
-            (fb_base.VARCHAR, [1], {}, "VARCHAR(1)"),
+            (FbTypes.VARCHAR, [1], {}, "VARCHAR(1)"),
             (
-                fb_base.VARCHAR,
+                FbTypes.VARCHAR,
                 [1],
                 {"charset": "OCTETS"},
                 "VARCHAR(1) CHARACTER SET OCTETS",
             ),
         ]
         for type_, args, kw, res in columns:
             self.assert_compile(type_(*args, **kw), res)
@@ -223,9 +214,9 @@
             Column("x", Integer),
             Column("y", Integer, Computed("x + 2", persisted=persisted)),
         )
         assert_raises_message(
             exc.CompileError,
             "Firebird computed columns do not support a persistence method",
             schema.CreateTable(t).compile,
-            dialect=firebird.dialect(),
+            dialect=self.__dialect__,
         )
```

### Comparing `sqlalchemy-firebird-0.8.0/test/test_fb_types.py` & `sqlalchemy-firebird-2.0.0/test/test_fb_types.py`

 * *Files identical despite different names*

