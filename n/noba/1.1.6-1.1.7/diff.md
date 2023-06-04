# Comparing `tmp/noba-1.1.6.tar.gz` & `tmp/noba-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "noba-1.1.6.tar", last modified: Thu Jun  1 11:48:07 2023, max compression
+gzip compressed data, was "noba-1.1.7.tar", last modified: Sun Jun  4 01:33:20 2023, max compression
```

## Comparing `noba-1.1.6.tar` & `noba-1.1.7.tar`

### file list

```diff
@@ -1,213 +1,213 @@
-drwxr-xr-x   0 metaer     (501) staff       (20)        0 2023-06-01 11:48:07.601836 noba-1.1.6/
--rw-r--r--   0 metaer     (501) staff       (20)    35149 2023-04-17 09:57:21.000000 noba-1.1.6/LICENSE
--rw-r--r--   0 metaer     (501) staff       (20)     5008 2023-06-01 11:48:07.601494 noba-1.1.6/PKG-INFO
--rw-r--r--   0 metaer     (501) staff       (20)     3556 2023-05-30 02:52:10.000000 noba-1.1.6/README.md
-drwxr-xr-x   0 metaer     (501) staff       (20)        0 2023-06-01 11:48:07.479158 noba-1.1.6/noba/
--rw-r--r--   0 metaer     (501) staff       (20)     1403 2023-04-24 15:35:06.000000 noba-1.1.6/noba/Core.py
--rw-r--r--   0 metaer     (501) staff       (20)       28 2023-04-24 15:35:06.000000 noba-1.1.6/noba/__init__.py
-drwxr-xr-x   0 metaer     (501) staff       (20)        0 2023-06-01 11:48:07.490296 noba-1.1.6/noba/analyzer_tables/
--rw-r--r--   0 metaer     (501) staff       (20)     1756 2023-04-24 15:35:06.000000 noba-1.1.6/noba/analyzer_tables/__init__.py
--rw-r--r--   0 metaer     (501) staff       (20)      312 2023-04-24 15:35:06.000000 noba-1.1.6/noba/analyzer_tables/annualreturn.py
--rw-r--r--   0 metaer     (501) staff       (20)      308 2023-04-24 15:35:06.000000 noba-1.1.6/noba/analyzer_tables/calmar.py
--rw-r--r--   0 metaer     (501) staff       (20)      587 2023-04-24 15:35:06.000000 noba-1.1.6/noba/analyzer_tables/drawdown.py
--rw-r--r--   0 metaer     (501) staff       (20)      319 2023-04-24 15:35:06.000000 noba-1.1.6/noba/analyzer_tables/leverage.py
--rw-r--r--   0 metaer     (501) staff       (20)      713 2023-04-24 15:35:06.000000 noba-1.1.6/noba/analyzer_tables/periodstats.py
--rw-r--r--   0 metaer     (501) staff       (20)      347 2023-04-24 15:35:06.000000 noba-1.1.6/noba/analyzer_tables/sharperatio.py
--rw-r--r--   0 metaer     (501) staff       (20)      367 2023-04-24 15:35:06.000000 noba-1.1.6/noba/analyzer_tables/sqn.py
--rw-r--r--   0 metaer     (501) staff       (20)      314 2023-04-24 15:35:06.000000 noba-1.1.6/noba/analyzer_tables/timereturn.py
--rw-r--r--   0 metaer     (501) staff       (20)     6081 2023-04-24 15:35:06.000000 noba-1.1.6/noba/analyzer_tables/tradeanalyzers.py
--rw-r--r--   0 metaer     (501) staff       (20)     2191 2023-04-24 15:35:06.000000 noba-1.1.6/noba/analyzer_tables/tradelist.py
--rw-r--r--   0 metaer     (501) staff       (20)      699 2023-04-24 15:35:06.000000 noba-1.1.6/noba/analyzer_tables/transactions.py
--rw-r--r--   0 metaer     (501) staff       (20)      296 2023-04-24 15:35:06.000000 noba-1.1.6/noba/analyzer_tables/vwr.py
-drwxr-xr-x   0 metaer     (501) staff       (20)        0 2023-06-01 11:48:07.492665 noba-1.1.6/noba/analyzers/
--rw-r--r--   0 metaer     (501) staff       (20)      115 2023-04-24 15:35:06.000000 noba-1.1.6/noba/analyzers/__init__.py
--rw-r--r--   0 metaer     (501) staff       (20)     3700 2023-04-24 15:35:06.000000 noba-1.1.6/noba/analyzers/plot.py
--rw-r--r--   0 metaer     (501) staff       (20)     2325 2023-04-24 15:35:06.000000 noba-1.1.6/noba/analyzers/recorder.py
--rw-r--r--   0 metaer     (501) staff       (20)     3009 2023-04-24 15:35:06.000000 noba-1.1.6/noba/analyzers/tradelist.py
--rw-r--r--   0 metaer     (501) staff       (20)    47581 2023-04-24 15:35:06.000000 noba-1.1.6/noba/app.py
--rw-r--r--   0 metaer     (501) staff       (20)     7430 2023-04-24 15:35:06.000000 noba-1.1.6/noba/cds.py
--rw-r--r--   0 metaer     (501) staff       (20)     6028 2023-04-24 15:35:06.000000 noba-1.1.6/noba/clock.py
--rw-r--r--   0 metaer     (501) staff       (20)     4983 2023-05-30 02:25:28.000000 noba-1.1.6/noba/command.py
-drwxr-xr-x   0 metaer     (501) staff       (20)        0 2023-06-01 11:48:07.493654 noba-1.1.6/noba/config/
--rw-r--r--   0 metaer     (501) staff       (20)     1797 2023-04-24 15:35:06.000000 noba-1.1.6/noba/config/config.default.json
--rw-r--r--   0 metaer     (501) staff       (20)     1797 2023-04-24 15:35:06.000000 noba-1.1.6/noba/config/config.json
--rw-r--r--   0 metaer     (501) staff       (20)    16949 2023-04-24 15:35:06.000000 noba-1.1.6/noba/confighandler.py
-drwxr-xr-x   0 metaer     (501) staff       (20)        0 2023-06-01 11:48:07.507715 noba-1.1.6/noba/dber/
--rw-r--r--   0 metaer     (501) staff       (20)      301 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/__init__.py
--rw-r--r--   0 metaer     (501) staff       (20)     5440 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/_compat.py
--rw-r--r--   0 metaer     (501) staff       (20)      466 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/_gae.py
--rw-r--r--   0 metaer     (501) staff       (20)      208 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/_globals.py
--rw-r--r--   0 metaer     (501) staff       (20)      396 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/_load.py
-drwxr-xr-x   0 metaer     (501) staff       (20)        0 2023-06-01 11:48:07.521962 noba-1.1.6/noba/dber/adapters/
--rw-r--r--   0 metaer     (501) staff       (20)     2372 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/adapters/__init__.py
--rw-r--r--   0 metaer     (501) staff       (20)    39366 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/adapters/base.py
--rw-r--r--   0 metaer     (501) staff       (20)     5691 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/adapters/couchdb.py
--rw-r--r--   0 metaer     (501) staff       (20)     2000 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/adapters/db2.py
--rw-r--r--   0 metaer     (501) staff       (20)     3145 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/adapters/firebird.py
--rw-r--r--   0 metaer     (501) staff       (20)    18365 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/adapters/google.py
--rw-r--r--   0 metaer     (501) staff       (20)     2076 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/adapters/informix.py
--rw-r--r--   0 metaer     (501) staff       (20)     1882 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/adapters/ingres.py
--rw-r--r--   0 metaer     (501) staff       (20)    37772 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/adapters/mongo.py
--rw-r--r--   0 metaer     (501) staff       (20)     6161 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/adapters/mssql.py
--rw-r--r--   0 metaer     (501) staff       (20)     3412 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/adapters/mysql.py
--rw-r--r--   0 metaer     (501) staff       (20)     9170 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/adapters/oracle.py
--rw-r--r--   0 metaer     (501) staff       (20)     9327 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/adapters/postgres.py
--rw-r--r--   0 metaer     (501) staff       (20)     1460 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/adapters/sap.py
--rw-r--r--   0 metaer     (501) staff       (20)     4894 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/adapters/snowflake.py
--rw-r--r--   0 metaer     (501) staff       (20)     4392 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/adapters/sqlite.py
--rw-r--r--   0 metaer     (501) staff       (20)      799 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/adapters/teradata.py
--rw-r--r--   0 metaer     (501) staff       (20)    40162 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/base.py
--rw-r--r--   0 metaer     (501) staff       (20)     6429 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/connection.py
-drwxr-xr-x   0 metaer     (501) staff       (20)        0 2023-06-01 11:48:07.527419 noba-1.1.6/noba/dber/contrib/
--rw-r--r--   0 metaer     (501) staff       (20)        1 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/contrib/__init__.py
--rw-r--r--   0 metaer     (501) staff       (20)    44550 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/contrib/imap_adapter.py
--rw-r--r--   0 metaer     (501) staff       (20)    79374 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/contrib/ipaddress.py
--rw-r--r--   0 metaer     (501) staff       (20)    10686 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/contrib/mockimaplib.py
--rw-r--r--   0 metaer     (501) staff       (20)     4071 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/contrib/ordereddict.py
--rw-r--r--   0 metaer     (501) staff       (20)     5586 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/contrib/portalocker.py
--rw-r--r--   0 metaer     (501) staff       (20)    33372 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/contrib/reserved_sql_keywords.py
--rw-r--r--   0 metaer     (501) staff       (20)     3544 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/default_validators.py
-drwxr-xr-x   0 metaer     (501) staff       (20)        0 2023-06-01 11:48:07.540469 noba-1.1.6/noba/dber/dialects/
--rw-r--r--   0 metaer     (501) staff       (20)     3803 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/dialects/__init__.py
--rw-r--r--   0 metaer     (501) staff       (20)    23536 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/dialects/base.py
--rw-r--r--   0 metaer     (501) staff       (20)     1390 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/dialects/couchdb.py
--rw-r--r--   0 metaer     (501) staff       (20)     3374 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/dialects/db2.py
--rw-r--r--   0 metaer     (501) staff       (20)     4307 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/dialects/firebird.py
--rw-r--r--   0 metaer     (501) staff       (20)     5953 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/dialects/google.py
--rw-r--r--   0 metaer     (501) staff       (20)     3275 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/dialects/informix.py
--rw-r--r--   0 metaer     (501) staff       (20)     3929 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/dialects/ingres.py
--rw-r--r--   0 metaer     (501) staff       (20)    22074 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/dialects/mongo.py
--rw-r--r--   0 metaer     (501) staff       (20)    15736 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/dialects/mssql.py
--rw-r--r--   0 metaer     (501) staff       (20)     3391 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/dialects/mysql.py
--rw-r--r--   0 metaer     (501) staff       (20)     8895 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/dialects/oracle.py
--rw-r--r--   0 metaer     (501) staff       (20)    14382 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/dialects/postgre.py
--rw-r--r--   0 metaer     (501) staff       (20)     3001 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/dialects/sap.py
--rw-r--r--   0 metaer     (501) staff       (20)    12059 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/dialects/snowflake.py
--rw-r--r--   0 metaer     (501) staff       (20)     4273 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/dialects/sqlite.py
--rw-r--r--   0 metaer     (501) staff       (20)     3400 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/dialects/teradata.py
--rw-r--r--   0 metaer     (501) staff       (20)     3179 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/drivers.py
--rw-r--r--   0 metaer     (501) staff       (20)      347 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/exceptions.py
-drwxr-xr-x   0 metaer     (501) staff       (20)        0 2023-06-01 11:48:07.546103 noba-1.1.6/noba/dber/helpers/
--rw-r--r--   0 metaer     (501) staff       (20)        1 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/helpers/__init__.py
--rw-r--r--   0 metaer     (501) staff       (20)      652 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/helpers/_internals.py
--rw-r--r--   0 metaer     (501) staff       (20)    16698 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/helpers/classes.py
--rw-r--r--   0 metaer     (501) staff       (20)      971 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/helpers/gae.py
--rw-r--r--   0 metaer     (501) staff       (20)    14800 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/helpers/methods.py
--rw-r--r--   0 metaer     (501) staff       (20)     1144 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/helpers/regex.py
--rw-r--r--   0 metaer     (501) staff       (20)    16447 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/helpers/rest.py
--rw-r--r--   0 metaer     (501) staff       (20)     1839 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/helpers/serializers.py
--rw-r--r--   0 metaer     (501) staff       (20)    27227 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/migrator.py
--rw-r--r--   0 metaer     (501) staff       (20)   130689 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/objects.py
-drwxr-xr-x   0 metaer     (501) staff       (20)        0 2023-06-01 11:48:07.550500 noba-1.1.6/noba/dber/parsers/
--rw-r--r--   0 metaer     (501) staff       (20)     3394 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/parsers/__init__.py
--rw-r--r--   0 metaer     (501) staff       (20)     4718 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/parsers/base.py
--rw-r--r--   0 metaer     (501) staff       (20)      360 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/parsers/google.py
--rw-r--r--   0 metaer     (501) staff       (20)     1605 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/parsers/mongo.py
--rw-r--r--   0 metaer     (501) staff       (20)     1654 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/parsers/oracle.py
--rw-r--r--   0 metaer     (501) staff       (20)      815 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/parsers/postgre.py
--rw-r--r--   0 metaer     (501) staff       (20)     1064 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/parsers/sqlite.py
-drwxr-xr-x   0 metaer     (501) staff       (20)        0 2023-06-01 11:48:07.560569 noba-1.1.6/noba/dber/representers/
--rw-r--r--   0 metaer     (501) staff       (20)     8831 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/representers/__init__.py
--rw-r--r--   0 metaer     (501) staff       (20)     8810 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/representers/base.py
--rw-r--r--   0 metaer     (501) staff       (20)     1210 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/representers/couchdb.py
--rw-r--r--   0 metaer     (501) staff       (20)      680 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/representers/db2.py
--rw-r--r--   0 metaer     (501) staff       (20)     1446 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/representers/google.py
--rw-r--r--   0 metaer     (501) staff       (20)      884 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/representers/informix.py
--rw-r--r--   0 metaer     (501) staff       (20)     1757 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/representers/mongo.py
--rw-r--r--   0 metaer     (501) staff       (20)      948 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/representers/mssql.py
--rw-r--r--   0 metaer     (501) staff       (20)      214 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/representers/mysql.py
--rw-r--r--   0 metaer     (501) staff       (20)     1286 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/representers/oracle.py
--rw-r--r--   0 metaer     (501) staff       (20)     1643 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/representers/postgre.py
--rw-r--r--   0 metaer     (501) staff       (20)      752 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/representers/sqlite.py
--rw-r--r--   0 metaer     (501) staff       (20)    22878 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/restapi.py
-drwxr-xr-x   0 metaer     (501) staff       (20)        0 2023-06-01 11:48:07.561678 noba-1.1.6/noba/dber/tools/
--rw-r--r--   0 metaer     (501) staff       (20)        1 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/tools/__init__.py
--rw-r--r--   0 metaer     (501) staff       (20)     1946 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/tools/tags.py
--rw-r--r--   0 metaer     (501) staff       (20)     1904 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/utils.py
--rw-r--r--   0 metaer     (501) staff       (20)   158800 2023-04-24 15:35:06.000000 noba-1.1.6/noba/dber/validators.py
-drwxr-xr-x   0 metaer     (501) staff       (20)        0 2023-06-01 11:48:07.562990 noba-1.1.6/noba/feeds/
--rw-r--r--   0 metaer     (501) staff       (20)       31 2023-04-24 15:35:06.000000 noba-1.1.6/noba/feeds/__init__.py
--rw-r--r--   0 metaer     (501) staff       (20)     6937 2023-04-24 15:35:06.000000 noba-1.1.6/noba/feeds/fakefeed.py
--rw-r--r--   0 metaer     (501) staff       (20)    83641 2023-04-24 15:35:06.000000 noba-1.1.6/noba/figure.py
-drwxr-xr-x   0 metaer     (501) staff       (20)        0 2023-06-01 11:48:07.567546 noba-1.1.6/noba/helper/
--rw-r--r--   0 metaer     (501) staff       (20)        0 2023-04-24 15:35:06.000000 noba-1.1.6/noba/helper/__init__.py
--rw-r--r--   0 metaer     (501) staff       (20)     1797 2023-04-24 15:35:06.000000 noba-1.1.6/noba/helper/bokeh.py
--rw-r--r--   0 metaer     (501) staff       (20)      875 2023-04-24 15:35:06.000000 noba-1.1.6/noba/helper/cds_ops.py
--rw-r--r--   0 metaer     (501) staff       (20)     4639 2023-04-24 15:35:06.000000 noba-1.1.6/noba/helper/datatable.py
--rw-r--r--   0 metaer     (501) staff       (20)     2578 2023-04-24 15:35:06.000000 noba-1.1.6/noba/helper/label.py
--rw-r--r--   0 metaer     (501) staff       (20)     4665 2023-04-24 15:35:06.000000 noba-1.1.6/noba/helper/marker.py
--rw-r--r--   0 metaer     (501) staff       (20)     1069 2023-04-24 15:35:06.000000 noba-1.1.6/noba/helper/params.py
-drwxr-xr-x   0 metaer     (501) staff       (20)        0 2023-06-01 11:48:07.568848 noba-1.1.6/noba/indicators/
--rw-r--r--   0 metaer     (501) staff       (20)      762 2023-04-24 15:35:06.000000 noba-1.1.6/noba/indicators/__init__.py
--rw-r--r--   0 metaer     (501) staff       (20)     1011 2023-04-24 15:35:06.000000 noba-1.1.6/noba/indicators/extraline.py
-drwxr-xr-x   0 metaer     (501) staff       (20)        0 2023-06-01 11:48:07.570203 noba-1.1.6/noba/ioc/
--rw-r--r--   0 metaer     (501) staff       (20)      827 2023-04-24 15:35:06.000000 noba-1.1.6/noba/ioc/__init__.py
--rw-r--r--   0 metaer     (501) staff       (20)     6196 2023-05-24 08:58:39.000000 noba-1.1.6/noba/ioc/container.py
-drwxr-xr-x   0 metaer     (501) staff       (20)        0 2023-06-01 11:48:07.571919 noba-1.1.6/noba/live/
--rw-r--r--   0 metaer     (501) staff       (20)        0 2023-04-24 15:35:06.000000 noba-1.1.6/noba/live/__init__.py
--rw-r--r--   0 metaer     (501) staff       (20)     7969 2023-04-24 15:35:06.000000 noba-1.1.6/noba/live/client.py
--rw-r--r--   0 metaer     (501) staff       (20)     8765 2023-04-24 15:35:06.000000 noba-1.1.6/noba/live/datahandler.py
--rw-r--r--   0 metaer     (501) staff       (20)     4522 2023-04-24 15:35:06.000000 noba-1.1.6/noba/optbrowser.py
-drwxr-xr-x   0 metaer     (501) staff       (20)        0 2023-06-01 11:48:07.577602 noba-1.1.6/noba/plugin/
--rw-r--r--   0 metaer     (501) staff       (20)      157 2023-04-24 15:35:06.000000 noba-1.1.6/noba/plugin/__init__.py
--rw-r--r--   0 metaer     (501) staff       (20)     5673 2023-04-24 15:35:06.000000 noba-1.1.6/noba/plugin/annualreturn.py
--rw-r--r--   0 metaer     (501) staff       (20)    12489 2023-04-24 15:35:06.000000 noba-1.1.6/noba/plugin/bbroker.py
--rw-r--r--   0 metaer     (501) staff       (20)     5885 2023-04-24 15:35:06.000000 noba-1.1.6/noba/plugin/cerebro.py
--rw-r--r--   0 metaer     (501) staff       (20)     2997 2023-04-24 15:35:06.000000 noba-1.1.6/noba/plugin/logger.py
--rw-r--r--   0 metaer     (501) staff       (20)     7241 2023-04-24 15:35:06.000000 noba-1.1.6/noba/plugin/model.py
--rw-r--r--   0 metaer     (501) staff       (20)     6237 2023-04-24 15:35:06.000000 noba-1.1.6/noba/plugin/order.py
--rw-r--r--   0 metaer     (501) staff       (20)    15765 2023-04-24 15:35:06.000000 noba-1.1.6/noba/plugin/plot.py
--rw-r--r--   0 metaer     (501) staff       (20)     6713 2023-04-24 15:35:06.000000 noba-1.1.6/noba/plugin/writer.py
-drwxr-xr-x   0 metaer     (501) staff       (20)        0 2023-06-01 11:48:07.580210 noba-1.1.6/noba/schemes/
--rw-r--r--   0 metaer     (501) staff       (20)       88 2023-04-24 15:35:06.000000 noba-1.1.6/noba/schemes/__init__.py
--rw-r--r--   0 metaer     (501) staff       (20)     1507 2023-04-24 15:35:06.000000 noba-1.1.6/noba/schemes/blackly.py
--rw-r--r--   0 metaer     (501) staff       (20)    23589 2023-04-24 15:35:06.000000 noba-1.1.6/noba/schemes/scheme.py
--rw-r--r--   0 metaer     (501) staff       (20)     1633 2023-04-24 15:35:06.000000 noba-1.1.6/noba/schemes/tradimo.py
-drwxr-xr-x   0 metaer     (501) staff       (20)        0 2023-06-01 11:48:07.585710 noba-1.1.6/noba/service/
--rw-r--r--   0 metaer     (501) staff       (20)      843 2023-04-24 15:35:06.000000 noba-1.1.6/noba/service/__init__.py
--rw-r--r--   0 metaer     (501) staff       (20)     2563 2023-04-24 15:35:06.000000 noba-1.1.6/noba/service/abs.py
--rw-r--r--   0 metaer     (501) staff       (20)     2256 2023-04-24 15:35:06.000000 noba-1.1.6/noba/service/backtest.py
--rw-r--r--   0 metaer     (501) staff       (20)     2751 2023-04-24 15:35:06.000000 noba-1.1.6/noba/service/config.py
--rw-r--r--   0 metaer     (501) staff       (20)     4442 2023-05-09 02:41:47.000000 noba-1.1.6/noba/service/core.py
--rw-r--r--   0 metaer     (501) staff       (20)    26670 2023-05-01 02:19:18.000000 noba-1.1.6/noba/service/dber.py
--rw-r--r--   0 metaer     (501) staff       (20)     3528 2023-04-24 15:35:06.000000 noba-1.1.6/noba/service/event.py
--rw-r--r--   0 metaer     (501) staff       (20)     4929 2023-04-24 15:35:06.000000 noba-1.1.6/noba/service/pipeline.py
--rw-r--r--   0 metaer     (501) staff       (20)     4482 2023-04-24 15:35:06.000000 noba-1.1.6/noba/snippet.py
--rw-r--r--   0 metaer     (501) staff       (20)     1045 2023-04-24 15:35:06.000000 noba-1.1.6/noba/tab.py
-drwxr-xr-x   0 metaer     (501) staff       (20)        0 2023-06-01 11:48:07.591060 noba-1.1.6/noba/tabs/
--rw-r--r--   0 metaer     (501) staff       (20)      184 2023-04-24 15:35:06.000000 noba-1.1.6/noba/tabs/__init__.py
--rw-r--r--   0 metaer     (501) staff       (20)     5629 2023-04-24 15:35:06.000000 noba-1.1.6/noba/tabs/analyzer.py
--rw-r--r--   0 metaer     (501) staff       (20)    35301 2023-04-24 15:35:06.000000 noba-1.1.6/noba/tabs/config.py
--rw-r--r--   0 metaer     (501) staff       (20)    24285 2023-04-24 15:35:06.000000 noba-1.1.6/noba/tabs/liveconfig.py
--rw-r--r--   0 metaer     (501) staff       (20)    15581 2023-04-24 15:35:06.000000 noba-1.1.6/noba/tabs/log.py
--rw-r--r--   0 metaer     (501) staff       (20)    13453 2023-04-24 15:35:06.000000 noba-1.1.6/noba/tabs/metadata.py
--rw-r--r--   0 metaer     (501) staff       (20)     2805 2023-04-24 15:35:06.000000 noba-1.1.6/noba/tabs/source.py
-drwxr-xr-x   0 metaer     (501) staff       (20)        0 2023-06-01 11:48:07.592069 noba-1.1.6/noba/templates/
--rw-r--r--   0 metaer     (501) staff       (20)     3670 2023-04-24 15:35:06.000000 noba-1.1.6/noba/templates/basic.css.j2
--rw-r--r--   0 metaer     (501) staff       (20)     8280 2023-04-24 15:35:06.000000 noba-1.1.6/noba/templates/basic.html.j2
-drwxr-xr-x   0 metaer     (501) staff       (20)        0 2023-06-01 11:48:07.595453 noba-1.1.6/noba/templates/bootstrap/
--rw-r--r--   0 metaer     (501) staff       (20)      917 2023-04-24 15:35:06.000000 noba-1.1.6/noba/templates/bootstrap/__init__.py
--rw-r--r--   0 metaer     (501) staff       (20)     1149 2023-06-01 06:12:00.000000 noba-1.1.6/noba/templates/bootstrap/boot_providers.py
--rw-r--r--   0 metaer     (501) staff       (20)      145 2023-04-24 15:35:06.000000 noba-1.1.6/noba/templates/bootstrap/main.py
--rw-r--r--   0 metaer     (501) staff       (20)     1621 2023-04-24 15:35:06.000000 noba-1.1.6/noba/templates/bootstrap/register_alias.py
--rw-r--r--   0 metaer     (501) staff       (20)     1069 2023-06-01 11:33:43.000000 noba-1.1.6/noba/templates/bootstrap/register_providers.py
-drwxr-xr-x   0 metaer     (501) staff       (20)        0 2023-06-01 11:48:07.597753 noba-1.1.6/noba/templates/config/
--rw-r--r--   0 metaer     (501) staff       (20)      377 2023-04-24 15:35:06.000000 noba-1.1.6/noba/templates/config/core_config.json
--rw-r--r--   0 metaer     (501) staff       (20)     1742 2023-04-24 15:35:06.000000 noba-1.1.6/noba/templates/config/project_config.json
-drwxr-xr-x   0 metaer     (501) staff       (20)        0 2023-06-01 11:48:07.600777 noba-1.1.6/noba/templates/js/
--rw-r--r--   0 metaer     (501) staff       (20)    55424 2023-04-24 15:35:06.000000 noba-1.1.6/noba/templates/js/handler.js
--rw-r--r--   0 metaer     (501) staff       (20)      966 2023-04-24 15:35:06.000000 noba-1.1.6/noba/templates/js/hover_tooltips.js
--rw-r--r--   0 metaer     (501) staff       (20)     1000 2023-04-24 15:35:06.000000 noba-1.1.6/noba/templates/js/tick_formatter.js
--rw-r--r--   0 metaer     (501) staff       (20)     7957 2023-04-24 15:35:06.000000 noba-1.1.6/noba/utils.py
--rw-r--r--   0 metaer     (501) staff       (20)       22 2023-06-01 11:35:24.000000 noba-1.1.6/noba/version.py
--rw-r--r--   0 metaer     (501) staff       (20)    10645 2023-04-24 15:35:06.000000 noba-1.1.6/noba/web.py
--rw-r--r--   0 metaer     (501) staff       (20)    10509 2023-04-24 15:35:06.000000 noba-1.1.6/noba/webapp.py
-drwxr-xr-x   0 metaer     (501) staff       (20)        0 2023-06-01 11:48:07.482164 noba-1.1.6/noba.egg-info/
--rw-r--r--   0 metaer     (501) staff       (20)     5008 2023-06-01 11:48:06.000000 noba-1.1.6/noba.egg-info/PKG-INFO
--rw-r--r--   0 metaer     (501) staff       (20)     4893 2023-06-01 11:48:07.000000 noba-1.1.6/noba.egg-info/SOURCES.txt
--rw-r--r--   0 metaer     (501) staff       (20)        1 2023-06-01 11:48:06.000000 noba-1.1.6/noba.egg-info/dependency_links.txt
--rw-r--r--   0 metaer     (501) staff       (20)       43 2023-06-01 11:48:06.000000 noba-1.1.6/noba.egg-info/entry_points.txt
--rw-r--r--   0 metaer     (501) staff       (20)       63 2023-06-01 11:48:07.000000 noba-1.1.6/noba.egg-info/requires.txt
--rw-r--r--   0 metaer     (501) staff       (20)        5 2023-06-01 11:48:07.000000 noba-1.1.6/noba.egg-info/top_level.txt
--rw-r--r--   0 metaer     (501) staff       (20)       38 2023-06-01 11:48:07.601976 noba-1.1.6/setup.cfg
--rw-r--r--   0 metaer     (501) staff       (20)     2367 2023-04-25 02:31:31.000000 noba-1.1.6/setup.py
+drwxr-xr-x   0 metaer     (501) staff       (20)        0 2023-06-04 01:33:20.472357 noba-1.1.7/
+-rw-r--r--   0 metaer     (501) staff       (20)    35149 2023-04-17 09:57:21.000000 noba-1.1.7/LICENSE
+-rw-r--r--   0 metaer     (501) staff       (20)     5008 2023-06-04 01:33:20.472047 noba-1.1.7/PKG-INFO
+-rw-r--r--   0 metaer     (501) staff       (20)     3556 2023-05-30 02:52:10.000000 noba-1.1.7/README.md
+drwxr-xr-x   0 metaer     (501) staff       (20)        0 2023-06-04 01:33:20.362028 noba-1.1.7/noba/
+-rw-r--r--   0 metaer     (501) staff       (20)     1403 2023-04-24 15:35:06.000000 noba-1.1.7/noba/Core.py
+-rw-r--r--   0 metaer     (501) staff       (20)       28 2023-04-24 15:35:06.000000 noba-1.1.7/noba/__init__.py
+drwxr-xr-x   0 metaer     (501) staff       (20)        0 2023-06-04 01:33:20.372265 noba-1.1.7/noba/analyzer_tables/
+-rw-r--r--   0 metaer     (501) staff       (20)     1756 2023-04-24 15:35:06.000000 noba-1.1.7/noba/analyzer_tables/__init__.py
+-rw-r--r--   0 metaer     (501) staff       (20)      312 2023-04-24 15:35:06.000000 noba-1.1.7/noba/analyzer_tables/annualreturn.py
+-rw-r--r--   0 metaer     (501) staff       (20)      308 2023-04-24 15:35:06.000000 noba-1.1.7/noba/analyzer_tables/calmar.py
+-rw-r--r--   0 metaer     (501) staff       (20)      587 2023-04-24 15:35:06.000000 noba-1.1.7/noba/analyzer_tables/drawdown.py
+-rw-r--r--   0 metaer     (501) staff       (20)      319 2023-04-24 15:35:06.000000 noba-1.1.7/noba/analyzer_tables/leverage.py
+-rw-r--r--   0 metaer     (501) staff       (20)      713 2023-04-24 15:35:06.000000 noba-1.1.7/noba/analyzer_tables/periodstats.py
+-rw-r--r--   0 metaer     (501) staff       (20)      347 2023-04-24 15:35:06.000000 noba-1.1.7/noba/analyzer_tables/sharperatio.py
+-rw-r--r--   0 metaer     (501) staff       (20)      367 2023-04-24 15:35:06.000000 noba-1.1.7/noba/analyzer_tables/sqn.py
+-rw-r--r--   0 metaer     (501) staff       (20)      314 2023-04-24 15:35:06.000000 noba-1.1.7/noba/analyzer_tables/timereturn.py
+-rw-r--r--   0 metaer     (501) staff       (20)     6081 2023-04-24 15:35:06.000000 noba-1.1.7/noba/analyzer_tables/tradeanalyzers.py
+-rw-r--r--   0 metaer     (501) staff       (20)     2191 2023-04-24 15:35:06.000000 noba-1.1.7/noba/analyzer_tables/tradelist.py
+-rw-r--r--   0 metaer     (501) staff       (20)      699 2023-04-24 15:35:06.000000 noba-1.1.7/noba/analyzer_tables/transactions.py
+-rw-r--r--   0 metaer     (501) staff       (20)      296 2023-04-24 15:35:06.000000 noba-1.1.7/noba/analyzer_tables/vwr.py
+drwxr-xr-x   0 metaer     (501) staff       (20)        0 2023-06-04 01:33:20.374350 noba-1.1.7/noba/analyzers/
+-rw-r--r--   0 metaer     (501) staff       (20)      115 2023-04-24 15:35:06.000000 noba-1.1.7/noba/analyzers/__init__.py
+-rw-r--r--   0 metaer     (501) staff       (20)     3700 2023-04-24 15:35:06.000000 noba-1.1.7/noba/analyzers/plot.py
+-rw-r--r--   0 metaer     (501) staff       (20)     2325 2023-04-24 15:35:06.000000 noba-1.1.7/noba/analyzers/recorder.py
+-rw-r--r--   0 metaer     (501) staff       (20)     3009 2023-04-24 15:35:06.000000 noba-1.1.7/noba/analyzers/tradelist.py
+-rw-r--r--   0 metaer     (501) staff       (20)    47581 2023-04-24 15:35:06.000000 noba-1.1.7/noba/app.py
+-rw-r--r--   0 metaer     (501) staff       (20)     7430 2023-04-24 15:35:06.000000 noba-1.1.7/noba/cds.py
+-rw-r--r--   0 metaer     (501) staff       (20)     6028 2023-04-24 15:35:06.000000 noba-1.1.7/noba/clock.py
+-rw-r--r--   0 metaer     (501) staff       (20)     4983 2023-05-30 02:25:28.000000 noba-1.1.7/noba/command.py
+drwxr-xr-x   0 metaer     (501) staff       (20)        0 2023-06-04 01:33:20.375159 noba-1.1.7/noba/config/
+-rw-r--r--   0 metaer     (501) staff       (20)     1797 2023-04-24 15:35:06.000000 noba-1.1.7/noba/config/config.default.json
+-rw-r--r--   0 metaer     (501) staff       (20)     1797 2023-04-24 15:35:06.000000 noba-1.1.7/noba/config/config.json
+-rw-r--r--   0 metaer     (501) staff       (20)    16949 2023-04-24 15:35:06.000000 noba-1.1.7/noba/confighandler.py
+drwxr-xr-x   0 metaer     (501) staff       (20)        0 2023-06-04 01:33:20.385730 noba-1.1.7/noba/dber/
+-rw-r--r--   0 metaer     (501) staff       (20)      301 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/__init__.py
+-rw-r--r--   0 metaer     (501) staff       (20)     5440 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/_compat.py
+-rw-r--r--   0 metaer     (501) staff       (20)      466 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/_gae.py
+-rw-r--r--   0 metaer     (501) staff       (20)      208 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/_globals.py
+-rw-r--r--   0 metaer     (501) staff       (20)      396 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/_load.py
+drwxr-xr-x   0 metaer     (501) staff       (20)        0 2023-06-04 01:33:20.401552 noba-1.1.7/noba/dber/adapters/
+-rw-r--r--   0 metaer     (501) staff       (20)     2372 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/adapters/__init__.py
+-rw-r--r--   0 metaer     (501) staff       (20)    39366 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/adapters/base.py
+-rw-r--r--   0 metaer     (501) staff       (20)     5691 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/adapters/couchdb.py
+-rw-r--r--   0 metaer     (501) staff       (20)     2000 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/adapters/db2.py
+-rw-r--r--   0 metaer     (501) staff       (20)     3145 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/adapters/firebird.py
+-rw-r--r--   0 metaer     (501) staff       (20)    18365 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/adapters/google.py
+-rw-r--r--   0 metaer     (501) staff       (20)     2076 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/adapters/informix.py
+-rw-r--r--   0 metaer     (501) staff       (20)     1882 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/adapters/ingres.py
+-rw-r--r--   0 metaer     (501) staff       (20)    37772 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/adapters/mongo.py
+-rw-r--r--   0 metaer     (501) staff       (20)     6161 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/adapters/mssql.py
+-rw-r--r--   0 metaer     (501) staff       (20)     3412 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/adapters/mysql.py
+-rw-r--r--   0 metaer     (501) staff       (20)     9170 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/adapters/oracle.py
+-rw-r--r--   0 metaer     (501) staff       (20)     9327 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/adapters/postgres.py
+-rw-r--r--   0 metaer     (501) staff       (20)     1460 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/adapters/sap.py
+-rw-r--r--   0 metaer     (501) staff       (20)     4894 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/adapters/snowflake.py
+-rw-r--r--   0 metaer     (501) staff       (20)     4392 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/adapters/sqlite.py
+-rw-r--r--   0 metaer     (501) staff       (20)      799 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/adapters/teradata.py
+-rw-r--r--   0 metaer     (501) staff       (20)    40162 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/base.py
+-rw-r--r--   0 metaer     (501) staff       (20)     6429 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/connection.py
+drwxr-xr-x   0 metaer     (501) staff       (20)        0 2023-06-04 01:33:20.407150 noba-1.1.7/noba/dber/contrib/
+-rw-r--r--   0 metaer     (501) staff       (20)        1 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/contrib/__init__.py
+-rw-r--r--   0 metaer     (501) staff       (20)    44550 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/contrib/imap_adapter.py
+-rw-r--r--   0 metaer     (501) staff       (20)    79374 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/contrib/ipaddress.py
+-rw-r--r--   0 metaer     (501) staff       (20)    10686 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/contrib/mockimaplib.py
+-rw-r--r--   0 metaer     (501) staff       (20)     4071 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/contrib/ordereddict.py
+-rw-r--r--   0 metaer     (501) staff       (20)     5586 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/contrib/portalocker.py
+-rw-r--r--   0 metaer     (501) staff       (20)    33372 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/contrib/reserved_sql_keywords.py
+-rw-r--r--   0 metaer     (501) staff       (20)     3544 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/default_validators.py
+drwxr-xr-x   0 metaer     (501) staff       (20)        0 2023-06-04 01:33:20.418666 noba-1.1.7/noba/dber/dialects/
+-rw-r--r--   0 metaer     (501) staff       (20)     3803 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/dialects/__init__.py
+-rw-r--r--   0 metaer     (501) staff       (20)    23536 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/dialects/base.py
+-rw-r--r--   0 metaer     (501) staff       (20)     1390 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/dialects/couchdb.py
+-rw-r--r--   0 metaer     (501) staff       (20)     3374 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/dialects/db2.py
+-rw-r--r--   0 metaer     (501) staff       (20)     4307 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/dialects/firebird.py
+-rw-r--r--   0 metaer     (501) staff       (20)     5953 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/dialects/google.py
+-rw-r--r--   0 metaer     (501) staff       (20)     3275 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/dialects/informix.py
+-rw-r--r--   0 metaer     (501) staff       (20)     3929 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/dialects/ingres.py
+-rw-r--r--   0 metaer     (501) staff       (20)    22074 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/dialects/mongo.py
+-rw-r--r--   0 metaer     (501) staff       (20)    15736 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/dialects/mssql.py
+-rw-r--r--   0 metaer     (501) staff       (20)     3391 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/dialects/mysql.py
+-rw-r--r--   0 metaer     (501) staff       (20)     8895 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/dialects/oracle.py
+-rw-r--r--   0 metaer     (501) staff       (20)    14382 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/dialects/postgre.py
+-rw-r--r--   0 metaer     (501) staff       (20)     3001 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/dialects/sap.py
+-rw-r--r--   0 metaer     (501) staff       (20)    12059 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/dialects/snowflake.py
+-rw-r--r--   0 metaer     (501) staff       (20)     4273 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/dialects/sqlite.py
+-rw-r--r--   0 metaer     (501) staff       (20)     3400 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/dialects/teradata.py
+-rw-r--r--   0 metaer     (501) staff       (20)     3179 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/drivers.py
+-rw-r--r--   0 metaer     (501) staff       (20)      347 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/exceptions.py
+drwxr-xr-x   0 metaer     (501) staff       (20)        0 2023-06-04 01:33:20.425344 noba-1.1.7/noba/dber/helpers/
+-rw-r--r--   0 metaer     (501) staff       (20)        1 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/helpers/__init__.py
+-rw-r--r--   0 metaer     (501) staff       (20)      652 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/helpers/_internals.py
+-rw-r--r--   0 metaer     (501) staff       (20)    16698 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/helpers/classes.py
+-rw-r--r--   0 metaer     (501) staff       (20)      971 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/helpers/gae.py
+-rw-r--r--   0 metaer     (501) staff       (20)    14800 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/helpers/methods.py
+-rw-r--r--   0 metaer     (501) staff       (20)     1144 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/helpers/regex.py
+-rw-r--r--   0 metaer     (501) staff       (20)    16447 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/helpers/rest.py
+-rw-r--r--   0 metaer     (501) staff       (20)     1839 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/helpers/serializers.py
+-rw-r--r--   0 metaer     (501) staff       (20)    27227 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/migrator.py
+-rw-r--r--   0 metaer     (501) staff       (20)   130689 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/objects.py
+drwxr-xr-x   0 metaer     (501) staff       (20)        0 2023-06-04 01:33:20.429597 noba-1.1.7/noba/dber/parsers/
+-rw-r--r--   0 metaer     (501) staff       (20)     3394 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/parsers/__init__.py
+-rw-r--r--   0 metaer     (501) staff       (20)     4718 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/parsers/base.py
+-rw-r--r--   0 metaer     (501) staff       (20)      360 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/parsers/google.py
+-rw-r--r--   0 metaer     (501) staff       (20)     1605 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/parsers/mongo.py
+-rw-r--r--   0 metaer     (501) staff       (20)     1654 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/parsers/oracle.py
+-rw-r--r--   0 metaer     (501) staff       (20)      815 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/parsers/postgre.py
+-rw-r--r--   0 metaer     (501) staff       (20)     1064 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/parsers/sqlite.py
+drwxr-xr-x   0 metaer     (501) staff       (20)        0 2023-06-04 01:33:20.436198 noba-1.1.7/noba/dber/representers/
+-rw-r--r--   0 metaer     (501) staff       (20)     8831 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/representers/__init__.py
+-rw-r--r--   0 metaer     (501) staff       (20)     8810 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/representers/base.py
+-rw-r--r--   0 metaer     (501) staff       (20)     1210 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/representers/couchdb.py
+-rw-r--r--   0 metaer     (501) staff       (20)      680 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/representers/db2.py
+-rw-r--r--   0 metaer     (501) staff       (20)     1446 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/representers/google.py
+-rw-r--r--   0 metaer     (501) staff       (20)      884 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/representers/informix.py
+-rw-r--r--   0 metaer     (501) staff       (20)     1757 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/representers/mongo.py
+-rw-r--r--   0 metaer     (501) staff       (20)      948 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/representers/mssql.py
+-rw-r--r--   0 metaer     (501) staff       (20)      214 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/representers/mysql.py
+-rw-r--r--   0 metaer     (501) staff       (20)     1286 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/representers/oracle.py
+-rw-r--r--   0 metaer     (501) staff       (20)     1643 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/representers/postgre.py
+-rw-r--r--   0 metaer     (501) staff       (20)      752 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/representers/sqlite.py
+-rw-r--r--   0 metaer     (501) staff       (20)    22878 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/restapi.py
+drwxr-xr-x   0 metaer     (501) staff       (20)        0 2023-06-04 01:33:20.437162 noba-1.1.7/noba/dber/tools/
+-rw-r--r--   0 metaer     (501) staff       (20)        1 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/tools/__init__.py
+-rw-r--r--   0 metaer     (501) staff       (20)     1946 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/tools/tags.py
+-rw-r--r--   0 metaer     (501) staff       (20)     1904 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/utils.py
+-rw-r--r--   0 metaer     (501) staff       (20)   158800 2023-04-24 15:35:06.000000 noba-1.1.7/noba/dber/validators.py
+drwxr-xr-x   0 metaer     (501) staff       (20)        0 2023-06-04 01:33:20.438407 noba-1.1.7/noba/feeds/
+-rw-r--r--   0 metaer     (501) staff       (20)       31 2023-04-24 15:35:06.000000 noba-1.1.7/noba/feeds/__init__.py
+-rw-r--r--   0 metaer     (501) staff       (20)     6937 2023-04-24 15:35:06.000000 noba-1.1.7/noba/feeds/fakefeed.py
+-rw-r--r--   0 metaer     (501) staff       (20)    83641 2023-04-24 15:35:06.000000 noba-1.1.7/noba/figure.py
+drwxr-xr-x   0 metaer     (501) staff       (20)        0 2023-06-04 01:33:20.442633 noba-1.1.7/noba/helper/
+-rw-r--r--   0 metaer     (501) staff       (20)        0 2023-04-24 15:35:06.000000 noba-1.1.7/noba/helper/__init__.py
+-rw-r--r--   0 metaer     (501) staff       (20)     1797 2023-04-24 15:35:06.000000 noba-1.1.7/noba/helper/bokeh.py
+-rw-r--r--   0 metaer     (501) staff       (20)      875 2023-04-24 15:35:06.000000 noba-1.1.7/noba/helper/cds_ops.py
+-rw-r--r--   0 metaer     (501) staff       (20)     4639 2023-04-24 15:35:06.000000 noba-1.1.7/noba/helper/datatable.py
+-rw-r--r--   0 metaer     (501) staff       (20)     2578 2023-04-24 15:35:06.000000 noba-1.1.7/noba/helper/label.py
+-rw-r--r--   0 metaer     (501) staff       (20)     4665 2023-04-24 15:35:06.000000 noba-1.1.7/noba/helper/marker.py
+-rw-r--r--   0 metaer     (501) staff       (20)     1069 2023-04-24 15:35:06.000000 noba-1.1.7/noba/helper/params.py
+drwxr-xr-x   0 metaer     (501) staff       (20)        0 2023-06-04 01:33:20.443534 noba-1.1.7/noba/indicators/
+-rw-r--r--   0 metaer     (501) staff       (20)      762 2023-04-24 15:35:06.000000 noba-1.1.7/noba/indicators/__init__.py
+-rw-r--r--   0 metaer     (501) staff       (20)     1011 2023-04-24 15:35:06.000000 noba-1.1.7/noba/indicators/extraline.py
+drwxr-xr-x   0 metaer     (501) staff       (20)        0 2023-06-04 01:33:20.444594 noba-1.1.7/noba/ioc/
+-rw-r--r--   0 metaer     (501) staff       (20)      827 2023-04-24 15:35:06.000000 noba-1.1.7/noba/ioc/__init__.py
+-rw-r--r--   0 metaer     (501) staff       (20)     6196 2023-05-24 08:58:39.000000 noba-1.1.7/noba/ioc/container.py
+drwxr-xr-x   0 metaer     (501) staff       (20)        0 2023-06-04 01:33:20.445945 noba-1.1.7/noba/live/
+-rw-r--r--   0 metaer     (501) staff       (20)        0 2023-04-24 15:35:06.000000 noba-1.1.7/noba/live/__init__.py
+-rw-r--r--   0 metaer     (501) staff       (20)     7969 2023-04-24 15:35:06.000000 noba-1.1.7/noba/live/client.py
+-rw-r--r--   0 metaer     (501) staff       (20)     8765 2023-04-24 15:35:06.000000 noba-1.1.7/noba/live/datahandler.py
+-rw-r--r--   0 metaer     (501) staff       (20)     4522 2023-04-24 15:35:06.000000 noba-1.1.7/noba/optbrowser.py
+drwxr-xr-x   0 metaer     (501) staff       (20)        0 2023-06-04 01:33:20.450410 noba-1.1.7/noba/plugin/
+-rw-r--r--   0 metaer     (501) staff       (20)      157 2023-04-24 15:35:06.000000 noba-1.1.7/noba/plugin/__init__.py
+-rw-r--r--   0 metaer     (501) staff       (20)     5673 2023-04-24 15:35:06.000000 noba-1.1.7/noba/plugin/annualreturn.py
+-rw-r--r--   0 metaer     (501) staff       (20)    12489 2023-04-24 15:35:06.000000 noba-1.1.7/noba/plugin/bbroker.py
+-rw-r--r--   0 metaer     (501) staff       (20)     5885 2023-04-24 15:35:06.000000 noba-1.1.7/noba/plugin/cerebro.py
+-rw-r--r--   0 metaer     (501) staff       (20)     2997 2023-04-24 15:35:06.000000 noba-1.1.7/noba/plugin/logger.py
+-rw-r--r--   0 metaer     (501) staff       (20)     7241 2023-04-24 15:35:06.000000 noba-1.1.7/noba/plugin/model.py
+-rw-r--r--   0 metaer     (501) staff       (20)     6237 2023-04-24 15:35:06.000000 noba-1.1.7/noba/plugin/order.py
+-rw-r--r--   0 metaer     (501) staff       (20)    15765 2023-04-24 15:35:06.000000 noba-1.1.7/noba/plugin/plot.py
+-rw-r--r--   0 metaer     (501) staff       (20)     6713 2023-04-24 15:35:06.000000 noba-1.1.7/noba/plugin/writer.py
+drwxr-xr-x   0 metaer     (501) staff       (20)        0 2023-06-04 01:33:20.452589 noba-1.1.7/noba/schemes/
+-rw-r--r--   0 metaer     (501) staff       (20)       88 2023-04-24 15:35:06.000000 noba-1.1.7/noba/schemes/__init__.py
+-rw-r--r--   0 metaer     (501) staff       (20)     1507 2023-04-24 15:35:06.000000 noba-1.1.7/noba/schemes/blackly.py
+-rw-r--r--   0 metaer     (501) staff       (20)    23589 2023-04-24 15:35:06.000000 noba-1.1.7/noba/schemes/scheme.py
+-rw-r--r--   0 metaer     (501) staff       (20)     1633 2023-04-24 15:35:06.000000 noba-1.1.7/noba/schemes/tradimo.py
+drwxr-xr-x   0 metaer     (501) staff       (20)        0 2023-06-04 01:33:20.457051 noba-1.1.7/noba/service/
+-rw-r--r--   0 metaer     (501) staff       (20)      843 2023-04-24 15:35:06.000000 noba-1.1.7/noba/service/__init__.py
+-rw-r--r--   0 metaer     (501) staff       (20)     2563 2023-04-24 15:35:06.000000 noba-1.1.7/noba/service/abs.py
+-rw-r--r--   0 metaer     (501) staff       (20)     2256 2023-04-24 15:35:06.000000 noba-1.1.7/noba/service/backtest.py
+-rw-r--r--   0 metaer     (501) staff       (20)     2751 2023-04-24 15:35:06.000000 noba-1.1.7/noba/service/config.py
+-rw-r--r--   0 metaer     (501) staff       (20)     4442 2023-05-09 02:41:47.000000 noba-1.1.7/noba/service/core.py
+-rw-r--r--   0 metaer     (501) staff       (20)    26670 2023-05-01 02:19:18.000000 noba-1.1.7/noba/service/dber.py
+-rw-r--r--   0 metaer     (501) staff       (20)     3567 2023-06-04 01:00:48.000000 noba-1.1.7/noba/service/event.py
+-rw-r--r--   0 metaer     (501) staff       (20)     4929 2023-04-24 15:35:06.000000 noba-1.1.7/noba/service/pipeline.py
+-rw-r--r--   0 metaer     (501) staff       (20)     4482 2023-04-24 15:35:06.000000 noba-1.1.7/noba/snippet.py
+-rw-r--r--   0 metaer     (501) staff       (20)     1045 2023-04-24 15:35:06.000000 noba-1.1.7/noba/tab.py
+drwxr-xr-x   0 metaer     (501) staff       (20)        0 2023-06-04 01:33:20.464715 noba-1.1.7/noba/tabs/
+-rw-r--r--   0 metaer     (501) staff       (20)      184 2023-04-24 15:35:06.000000 noba-1.1.7/noba/tabs/__init__.py
+-rw-r--r--   0 metaer     (501) staff       (20)     5629 2023-04-24 15:35:06.000000 noba-1.1.7/noba/tabs/analyzer.py
+-rw-r--r--   0 metaer     (501) staff       (20)    35301 2023-04-24 15:35:06.000000 noba-1.1.7/noba/tabs/config.py
+-rw-r--r--   0 metaer     (501) staff       (20)    24285 2023-04-24 15:35:06.000000 noba-1.1.7/noba/tabs/liveconfig.py
+-rw-r--r--   0 metaer     (501) staff       (20)    15581 2023-04-24 15:35:06.000000 noba-1.1.7/noba/tabs/log.py
+-rw-r--r--   0 metaer     (501) staff       (20)    13453 2023-04-24 15:35:06.000000 noba-1.1.7/noba/tabs/metadata.py
+-rw-r--r--   0 metaer     (501) staff       (20)     2805 2023-04-24 15:35:06.000000 noba-1.1.7/noba/tabs/source.py
+drwxr-xr-x   0 metaer     (501) staff       (20)        0 2023-06-04 01:33:20.465572 noba-1.1.7/noba/templates/
+-rw-r--r--   0 metaer     (501) staff       (20)     3670 2023-04-24 15:35:06.000000 noba-1.1.7/noba/templates/basic.css.j2
+-rw-r--r--   0 metaer     (501) staff       (20)     8280 2023-04-24 15:35:06.000000 noba-1.1.7/noba/templates/basic.html.j2
+drwxr-xr-x   0 metaer     (501) staff       (20)        0 2023-06-04 01:33:20.468001 noba-1.1.7/noba/templates/bootstrap/
+-rw-r--r--   0 metaer     (501) staff       (20)      917 2023-04-24 15:35:06.000000 noba-1.1.7/noba/templates/bootstrap/__init__.py
+-rw-r--r--   0 metaer     (501) staff       (20)     1149 2023-06-01 06:12:00.000000 noba-1.1.7/noba/templates/bootstrap/boot_providers.py
+-rw-r--r--   0 metaer     (501) staff       (20)      145 2023-04-24 15:35:06.000000 noba-1.1.7/noba/templates/bootstrap/main.py
+-rw-r--r--   0 metaer     (501) staff       (20)     1621 2023-04-24 15:35:06.000000 noba-1.1.7/noba/templates/bootstrap/register_alias.py
+-rw-r--r--   0 metaer     (501) staff       (20)     1069 2023-06-01 11:33:43.000000 noba-1.1.7/noba/templates/bootstrap/register_providers.py
+drwxr-xr-x   0 metaer     (501) staff       (20)        0 2023-06-04 01:33:20.469112 noba-1.1.7/noba/templates/config/
+-rw-r--r--   0 metaer     (501) staff       (20)      377 2023-04-24 15:35:06.000000 noba-1.1.7/noba/templates/config/core_config.json
+-rw-r--r--   0 metaer     (501) staff       (20)     1742 2023-04-24 15:35:06.000000 noba-1.1.7/noba/templates/config/project_config.json
+drwxr-xr-x   0 metaer     (501) staff       (20)        0 2023-06-04 01:33:20.471503 noba-1.1.7/noba/templates/js/
+-rw-r--r--   0 metaer     (501) staff       (20)    55424 2023-04-24 15:35:06.000000 noba-1.1.7/noba/templates/js/handler.js
+-rw-r--r--   0 metaer     (501) staff       (20)      966 2023-04-24 15:35:06.000000 noba-1.1.7/noba/templates/js/hover_tooltips.js
+-rw-r--r--   0 metaer     (501) staff       (20)     1000 2023-04-24 15:35:06.000000 noba-1.1.7/noba/templates/js/tick_formatter.js
+-rw-r--r--   0 metaer     (501) staff       (20)     7957 2023-04-24 15:35:06.000000 noba-1.1.7/noba/utils.py
+-rw-r--r--   0 metaer     (501) staff       (20)       22 2023-06-04 01:07:23.000000 noba-1.1.7/noba/version.py
+-rw-r--r--   0 metaer     (501) staff       (20)    10645 2023-04-24 15:35:06.000000 noba-1.1.7/noba/web.py
+-rw-r--r--   0 metaer     (501) staff       (20)    10509 2023-04-24 15:35:06.000000 noba-1.1.7/noba/webapp.py
+drwxr-xr-x   0 metaer     (501) staff       (20)        0 2023-06-04 01:33:20.364731 noba-1.1.7/noba.egg-info/
+-rw-r--r--   0 metaer     (501) staff       (20)     5008 2023-06-04 01:33:19.000000 noba-1.1.7/noba.egg-info/PKG-INFO
+-rw-r--r--   0 metaer     (501) staff       (20)     4893 2023-06-04 01:33:20.000000 noba-1.1.7/noba.egg-info/SOURCES.txt
+-rw-r--r--   0 metaer     (501) staff       (20)        1 2023-06-04 01:33:19.000000 noba-1.1.7/noba.egg-info/dependency_links.txt
+-rw-r--r--   0 metaer     (501) staff       (20)       43 2023-06-04 01:33:19.000000 noba-1.1.7/noba.egg-info/entry_points.txt
+-rw-r--r--   0 metaer     (501) staff       (20)       63 2023-06-04 01:33:20.000000 noba-1.1.7/noba.egg-info/requires.txt
+-rw-r--r--   0 metaer     (501) staff       (20)        5 2023-06-04 01:33:20.000000 noba-1.1.7/noba.egg-info/top_level.txt
+-rw-r--r--   0 metaer     (501) staff       (20)       38 2023-06-04 01:33:20.472510 noba-1.1.7/setup.cfg
+-rw-r--r--   0 metaer     (501) staff       (20)     2367 2023-04-25 02:31:31.000000 noba-1.1.7/setup.py
```

### Comparing `noba-1.1.6/LICENSE` & `noba-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/PKG-INFO` & `noba-1.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: noba
-Version: 1.1.6
+Version: 1.1.7
 Summary: Noba is not only Backtrader
 Home-page: https://github.com/iniself/noba
 Author: Metaer
 Author-email: 
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: Bug Tracker, https://github.com/iniself/noba/issues
 Project-URL: Documentation, https://github.com/iniself/noba
```

### Comparing `noba-1.1.6/README.md` & `noba-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/Core.py` & `noba-1.1.7/noba/Core.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/analyzer_tables/__init__.py` & `noba-1.1.7/noba/analyzer_tables/__init__.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/analyzer_tables/drawdown.py` & `noba-1.1.7/noba/analyzer_tables/drawdown.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/analyzer_tables/periodstats.py` & `noba-1.1.7/noba/analyzer_tables/periodstats.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/analyzer_tables/tradeanalyzers.py` & `noba-1.1.7/noba/analyzer_tables/tradeanalyzers.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/analyzer_tables/tradelist.py` & `noba-1.1.7/noba/analyzer_tables/tradelist.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/analyzer_tables/transactions.py` & `noba-1.1.7/noba/analyzer_tables/transactions.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/analyzers/plot.py` & `noba-1.1.7/noba/analyzers/plot.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/analyzers/recorder.py` & `noba-1.1.7/noba/analyzers/recorder.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/analyzers/tradelist.py` & `noba-1.1.7/noba/analyzers/tradelist.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/app.py` & `noba-1.1.7/noba/app.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/cds.py` & `noba-1.1.7/noba/cds.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/clock.py` & `noba-1.1.7/noba/clock.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/command.py` & `noba-1.1.7/noba/command.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/config/config.default.json` & `noba-1.1.7/noba/config/config.default.json`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/config/config.json` & `noba-1.1.7/noba/config/config.json`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/confighandler.py` & `noba-1.1.7/noba/confighandler.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/dber/_compat.py` & `noba-1.1.7/noba/dber/_compat.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/dber/adapters/__init__.py` & `noba-1.1.7/noba/dber/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/dber/adapters/base.py` & `noba-1.1.7/noba/dber/adapters/base.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/dber/adapters/couchdb.py` & `noba-1.1.7/noba/dber/adapters/couchdb.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/dber/adapters/db2.py` & `noba-1.1.7/noba/dber/adapters/db2.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/dber/adapters/firebird.py` & `noba-1.1.7/noba/dber/adapters/firebird.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/dber/adapters/google.py` & `noba-1.1.7/noba/dber/adapters/google.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/dber/adapters/informix.py` & `noba-1.1.7/noba/dber/adapters/informix.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/dber/adapters/ingres.py` & `noba-1.1.7/noba/dber/adapters/ingres.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/dber/adapters/mongo.py` & `noba-1.1.7/noba/dber/adapters/mongo.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/dber/adapters/mssql.py` & `noba-1.1.7/noba/dber/adapters/mssql.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/dber/adapters/mysql.py` & `noba-1.1.7/noba/dber/adapters/mysql.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/dber/adapters/oracle.py` & `noba-1.1.7/noba/dber/adapters/oracle.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/dber/adapters/postgres.py` & `noba-1.1.7/noba/dber/adapters/postgres.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/dber/adapters/sap.py` & `noba-1.1.7/noba/dber/adapters/sap.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/dber/adapters/snowflake.py` & `noba-1.1.7/noba/dber/adapters/snowflake.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/dber/adapters/sqlite.py` & `noba-1.1.7/noba/dber/adapters/sqlite.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/dber/adapters/teradata.py` & `noba-1.1.7/noba/dber/adapters/teradata.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/dber/base.py` & `noba-1.1.7/noba/dber/base.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/dber/connection.py` & `noba-1.1.7/noba/dber/connection.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/dber/contrib/imap_adapter.py` & `noba-1.1.7/noba/dber/contrib/imap_adapter.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/dber/contrib/ipaddress.py` & `noba-1.1.7/noba/dber/contrib/ipaddress.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/dber/contrib/mockimaplib.py` & `noba-1.1.7/noba/dber/contrib/mockimaplib.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/dber/contrib/ordereddict.py` & `noba-1.1.7/noba/dber/contrib/ordereddict.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/dber/contrib/portalocker.py` & `noba-1.1.7/noba/dber/contrib/portalocker.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/dber/contrib/reserved_sql_keywords.py` & `noba-1.1.7/noba/dber/contrib/reserved_sql_keywords.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/dber/default_validators.py` & `noba-1.1.7/noba/dber/default_validators.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/dber/dialects/__init__.py` & `noba-1.1.7/noba/dber/dialects/__init__.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/dber/dialects/base.py` & `noba-1.1.7/noba/dber/dialects/base.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/dber/dialects/couchdb.py` & `noba-1.1.7/noba/dber/dialects/couchdb.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/dber/dialects/db2.py` & `noba-1.1.7/noba/dber/dialects/db2.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/dber/dialects/firebird.py` & `noba-1.1.7/noba/dber/dialects/firebird.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/dber/dialects/google.py` & `noba-1.1.7/noba/dber/dialects/google.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/dber/dialects/informix.py` & `noba-1.1.7/noba/dber/dialects/informix.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/dber/dialects/ingres.py` & `noba-1.1.7/noba/dber/dialects/ingres.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/dber/dialects/mongo.py` & `noba-1.1.7/noba/dber/dialects/mongo.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/dber/dialects/mssql.py` & `noba-1.1.7/noba/dber/dialects/mssql.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/dber/dialects/mysql.py` & `noba-1.1.7/noba/dber/dialects/mysql.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/dber/dialects/oracle.py` & `noba-1.1.7/noba/dber/dialects/oracle.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/dber/dialects/postgre.py` & `noba-1.1.7/noba/dber/dialects/postgre.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/dber/dialects/sap.py` & `noba-1.1.7/noba/dber/dialects/sap.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/dber/dialects/snowflake.py` & `noba-1.1.7/noba/dber/dialects/snowflake.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/dber/dialects/sqlite.py` & `noba-1.1.7/noba/dber/dialects/sqlite.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/dber/dialects/teradata.py` & `noba-1.1.7/noba/dber/dialects/teradata.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/dber/drivers.py` & `noba-1.1.7/noba/dber/drivers.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/dber/helpers/_internals.py` & `noba-1.1.7/noba/dber/helpers/_internals.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/dber/helpers/classes.py` & `noba-1.1.7/noba/dber/helpers/classes.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/dber/helpers/gae.py` & `noba-1.1.7/noba/dber/helpers/gae.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/dber/helpers/methods.py` & `noba-1.1.7/noba/dber/helpers/methods.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/dber/helpers/regex.py` & `noba-1.1.7/noba/dber/helpers/regex.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/dber/helpers/rest.py` & `noba-1.1.7/noba/dber/helpers/rest.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/dber/helpers/serializers.py` & `noba-1.1.7/noba/dber/helpers/serializers.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/dber/migrator.py` & `noba-1.1.7/noba/dber/migrator.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/dber/objects.py` & `noba-1.1.7/noba/dber/objects.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/dber/parsers/__init__.py` & `noba-1.1.7/noba/dber/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/dber/parsers/base.py` & `noba-1.1.7/noba/dber/parsers/base.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/dber/parsers/mongo.py` & `noba-1.1.7/noba/dber/parsers/mongo.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/dber/parsers/oracle.py` & `noba-1.1.7/noba/dber/parsers/oracle.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/dber/parsers/postgre.py` & `noba-1.1.7/noba/dber/parsers/postgre.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/dber/parsers/sqlite.py` & `noba-1.1.7/noba/dber/parsers/sqlite.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/dber/representers/__init__.py` & `noba-1.1.7/noba/dber/representers/__init__.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/dber/representers/base.py` & `noba-1.1.7/noba/dber/representers/base.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/dber/representers/couchdb.py` & `noba-1.1.7/noba/dber/representers/couchdb.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/dber/representers/db2.py` & `noba-1.1.7/noba/dber/representers/db2.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/dber/representers/google.py` & `noba-1.1.7/noba/dber/representers/google.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/dber/representers/informix.py` & `noba-1.1.7/noba/dber/representers/informix.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/dber/representers/mongo.py` & `noba-1.1.7/noba/dber/representers/mongo.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/dber/representers/mssql.py` & `noba-1.1.7/noba/dber/representers/mssql.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/dber/representers/oracle.py` & `noba-1.1.7/noba/dber/representers/oracle.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/dber/representers/postgre.py` & `noba-1.1.7/noba/dber/representers/postgre.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/dber/representers/sqlite.py` & `noba-1.1.7/noba/dber/representers/sqlite.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/dber/restapi.py` & `noba-1.1.7/noba/dber/restapi.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/dber/tools/tags.py` & `noba-1.1.7/noba/dber/tools/tags.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/dber/utils.py` & `noba-1.1.7/noba/dber/utils.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/dber/validators.py` & `noba-1.1.7/noba/dber/validators.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/feeds/fakefeed.py` & `noba-1.1.7/noba/feeds/fakefeed.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/figure.py` & `noba-1.1.7/noba/figure.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/helper/bokeh.py` & `noba-1.1.7/noba/helper/bokeh.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/helper/cds_ops.py` & `noba-1.1.7/noba/helper/cds_ops.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/helper/datatable.py` & `noba-1.1.7/noba/helper/datatable.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/helper/label.py` & `noba-1.1.7/noba/helper/label.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/helper/marker.py` & `noba-1.1.7/noba/helper/marker.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/helper/params.py` & `noba-1.1.7/noba/helper/params.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/indicators/__init__.py` & `noba-1.1.7/noba/indicators/__init__.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/indicators/extraline.py` & `noba-1.1.7/noba/indicators/extraline.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/ioc/__init__.py` & `noba-1.1.7/noba/ioc/__init__.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/ioc/container.py` & `noba-1.1.7/noba/ioc/container.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/live/client.py` & `noba-1.1.7/noba/live/client.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/live/datahandler.py` & `noba-1.1.7/noba/live/datahandler.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/optbrowser.py` & `noba-1.1.7/noba/optbrowser.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/plugin/annualreturn.py` & `noba-1.1.7/noba/plugin/annualreturn.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/plugin/bbroker.py` & `noba-1.1.7/noba/plugin/bbroker.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/plugin/cerebro.py` & `noba-1.1.7/noba/plugin/cerebro.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/plugin/logger.py` & `noba-1.1.7/noba/plugin/logger.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/plugin/model.py` & `noba-1.1.7/noba/plugin/model.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/plugin/order.py` & `noba-1.1.7/noba/plugin/order.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/plugin/plot.py` & `noba-1.1.7/noba/plugin/plot.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/plugin/writer.py` & `noba-1.1.7/noba/plugin/writer.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/schemes/blackly.py` & `noba-1.1.7/noba/schemes/blackly.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/schemes/scheme.py` & `noba-1.1.7/noba/schemes/scheme.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/schemes/tradimo.py` & `noba-1.1.7/noba/schemes/tradimo.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/service/__init__.py` & `noba-1.1.7/noba/service/__init__.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/service/abs.py` & `noba-1.1.7/noba/service/abs.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/service/backtest.py` & `noba-1.1.7/noba/service/backtest.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/service/config.py` & `noba-1.1.7/noba/service/config.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/service/core.py` & `noba-1.1.7/noba/service/core.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/service/dber.py` & `noba-1.1.7/noba/service/dber.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/service/event.py` & `noba-1.1.7/noba/service/event.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,21 +18,17 @@
 #
 
 from __future__ import (absolute_import, division, print_function, unicode_literals)
 from noba.snippet import *
 
 class EventHub:
     hubs = {}
-    def __init__(self, event, name=None):
-        if not is_list(event):
-            event = [event]
-        self._event = event
+    def __init__(self):
+        self._event = list()
         self._listeners = list()
-        if name and self._single(name):
-            EventHub.hubs[name] = self
 
     def _single(self, name):
         if name in EventHub.hubs:
             print(f"[Error] EventHub '{name}' already exists!")
             exit()
         else:
             return True
@@ -41,15 +37,22 @@
         if name and self._single(name):
             self._name = name
             EventHub.hubs[name] = self
         return self
 
     @classmethod
     def hub(cls, event, name=None):
-        return cls(event, name)
+        hub_obj = cls()
+        
+        if not is_list(event):
+            event = [event]
+        hub_obj._event = event
+        if name and hub_obj._single(name):
+            cls.hubs[name] = hub_obj
+        return hub_obj
 
     @classmethod
     def get_all_hub(cls):
         return cls.hubs
 
     @classmethod
     def drop(cls, name):
```

### Comparing `noba-1.1.6/noba/service/pipeline.py` & `noba-1.1.7/noba/service/pipeline.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/snippet.py` & `noba-1.1.7/noba/snippet.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/tab.py` & `noba-1.1.7/noba/tab.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/tabs/analyzer.py` & `noba-1.1.7/noba/tabs/analyzer.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/tabs/config.py` & `noba-1.1.7/noba/tabs/config.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/tabs/liveconfig.py` & `noba-1.1.7/noba/tabs/liveconfig.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/tabs/log.py` & `noba-1.1.7/noba/tabs/log.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/tabs/metadata.py` & `noba-1.1.7/noba/tabs/metadata.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/tabs/source.py` & `noba-1.1.7/noba/tabs/source.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/templates/basic.css.j2` & `noba-1.1.7/noba/templates/basic.css.j2`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/templates/basic.html.j2` & `noba-1.1.7/noba/templates/basic.html.j2`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/templates/bootstrap/__init__.py` & `noba-1.1.7/noba/templates/bootstrap/__init__.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/templates/bootstrap/boot_providers.py` & `noba-1.1.7/noba/templates/bootstrap/boot_providers.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/templates/bootstrap/register_alias.py` & `noba-1.1.7/noba/templates/bootstrap/register_alias.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/templates/bootstrap/register_providers.py` & `noba-1.1.7/noba/templates/bootstrap/register_providers.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/templates/config/project_config.json` & `noba-1.1.7/noba/templates/config/project_config.json`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/templates/js/handler.js` & `noba-1.1.7/noba/templates/js/handler.js`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/templates/js/hover_tooltips.js` & `noba-1.1.7/noba/templates/js/hover_tooltips.js`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/templates/js/tick_formatter.js` & `noba-1.1.7/noba/templates/js/tick_formatter.js`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/utils.py` & `noba-1.1.7/noba/utils.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/web.py` & `noba-1.1.7/noba/web.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba/webapp.py` & `noba-1.1.7/noba/webapp.py`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/noba.egg-info/PKG-INFO` & `noba-1.1.7/noba.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: noba
-Version: 1.1.6
+Version: 1.1.7
 Summary: Noba is not only Backtrader
 Home-page: https://github.com/iniself/noba
 Author: Metaer
 Author-email: 
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: Bug Tracker, https://github.com/iniself/noba/issues
 Project-URL: Documentation, https://github.com/iniself/noba
```

### Comparing `noba-1.1.6/noba.egg-info/SOURCES.txt` & `noba-1.1.7/noba.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `noba-1.1.6/setup.py` & `noba-1.1.7/setup.py`

 * *Files identical despite different names*

