# Comparing `tmp/lesscode_database-0.0.3.tar.gz` & `tmp/lesscode_database-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lesscode_database-0.0.3.tar", last modified: Sat Jun  3 07:13:07 2023, max compression
+gzip compressed data, was "dist/lesscode_database-0.0.4.tar", last modified: Sun Jun  4 08:12:39 2023, max compression
```

## Comparing `lesscode_database-0.0.3.tar` & `lesscode_database-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 navy      (1000) navy      (1000)        0 2023-06-03 07:13:07.000000 lesscode_database-0.0.3/
--rw-r--r--   0 navy      (1000) navy      (1000)    11357 2023-06-01 13:04:22.000000 lesscode_database-0.0.3/LICENSE
--rw-r--r--   0 navy      (1000) navy      (1000)     6933 2023-06-03 07:13:07.000000 lesscode_database-0.0.3/PKG-INFO
--rw-r--r--   0 navy      (1000) navy      (1000)     6567 2023-06-03 07:09:07.000000 lesscode_database-0.0.3/README.md
-drwxr-xr-x   0 navy      (1000) navy      (1000)        0 2023-06-03 07:13:07.000000 lesscode_database-0.0.3/lesscode_database/
--rw-r--r--   0 navy      (1000) navy      (1000)        0 2023-06-01 13:04:45.000000 lesscode_database-0.0.3/lesscode_database/__init__.py
--rw-r--r--   0 navy      (1000) navy      (1000)    26428 2023-06-03 06:57:13.000000 lesscode_database-0.0.3/lesscode_database/connect_pool.py
--rw-r--r--   0 navy      (1000) navy      (1000)     1194 2023-06-03 05:01:48.000000 lesscode_database-0.0.3/lesscode_database/connection_info.py
--rw-r--r--   0 navy      (1000) navy      (1000)     1900 2023-06-01 13:32:42.000000 lesscode_database-0.0.3/lesscode_database/options.py
--rw-r--r--   0 navy      (1000) navy      (1000)       22 2023-06-03 07:10:39.000000 lesscode_database-0.0.3/lesscode_database/version.py
-drwxr-xr-x   0 navy      (1000) navy      (1000)        0 2023-06-03 07:13:07.000000 lesscode_database-0.0.3/lesscode_database.egg-info/
--rw-r--r--   0 navy      (1000) navy      (1000)     6933 2023-06-03 07:13:07.000000 lesscode_database-0.0.3/lesscode_database.egg-info/PKG-INFO
--rw-r--r--   0 navy      (1000) navy      (1000)      349 2023-06-03 07:13:07.000000 lesscode_database-0.0.3/lesscode_database.egg-info/SOURCES.txt
--rw-r--r--   0 navy      (1000) navy      (1000)        1 2023-06-03 07:13:07.000000 lesscode_database-0.0.3/lesscode_database.egg-info/dependency_links.txt
--rw-r--r--   0 navy      (1000) navy      (1000)       18 2023-06-03 07:13:07.000000 lesscode_database-0.0.3/lesscode_database.egg-info/top_level.txt
--rw-r--r--   0 navy      (1000) navy      (1000)       38 2023-06-03 07:13:07.000000 lesscode_database-0.0.3/setup.cfg
--rw-r--r--   0 navy      (1000) navy      (1000)     1194 2023-06-01 13:04:45.000000 lesscode_database-0.0.3/setup.py
+drwxr-xr-x   0 navy      (1000) navy      (1000)        0 2023-06-04 08:12:39.000000 lesscode_database-0.0.4/
+-rw-r--r--   0 navy      (1000) navy      (1000)    11357 2023-06-01 13:04:22.000000 lesscode_database-0.0.4/LICENSE
+-rw-r--r--   0 navy      (1000) navy      (1000)    10787 2023-06-04 08:12:39.000000 lesscode_database-0.0.4/PKG-INFO
+-rw-r--r--   0 navy      (1000) navy      (1000)    10421 2023-06-04 08:12:11.000000 lesscode_database-0.0.4/README.md
+drwxr-xr-x   0 navy      (1000) navy      (1000)        0 2023-06-04 08:12:39.000000 lesscode_database-0.0.4/lesscode_database/
+-rw-r--r--   0 navy      (1000) navy      (1000)        0 2023-06-01 13:04:45.000000 lesscode_database-0.0.4/lesscode_database/__init__.py
+-rw-r--r--   0 navy      (1000) navy      (1000)    39136 2023-06-04 08:12:11.000000 lesscode_database-0.0.4/lesscode_database/connect_pool.py
+-rw-r--r--   0 navy      (1000) navy      (1000)     1194 2023-06-03 05:01:48.000000 lesscode_database-0.0.4/lesscode_database/connection_info.py
+-rw-r--r--   0 navy      (1000) navy      (1000)     1900 2023-06-01 13:32:42.000000 lesscode_database-0.0.4/lesscode_database/options.py
+-rw-r--r--   0 navy      (1000) navy      (1000)       22 2023-06-04 05:48:56.000000 lesscode_database-0.0.4/lesscode_database/version.py
+drwxr-xr-x   0 navy      (1000) navy      (1000)        0 2023-06-04 08:12:39.000000 lesscode_database-0.0.4/lesscode_database.egg-info/
+-rw-r--r--   0 navy      (1000) navy      (1000)    10787 2023-06-04 08:12:39.000000 lesscode_database-0.0.4/lesscode_database.egg-info/PKG-INFO
+-rw-r--r--   0 navy      (1000) navy      (1000)      349 2023-06-04 08:12:39.000000 lesscode_database-0.0.4/lesscode_database.egg-info/SOURCES.txt
+-rw-r--r--   0 navy      (1000) navy      (1000)        1 2023-06-04 08:12:39.000000 lesscode_database-0.0.4/lesscode_database.egg-info/dependency_links.txt
+-rw-r--r--   0 navy      (1000) navy      (1000)       18 2023-06-04 08:12:39.000000 lesscode_database-0.0.4/lesscode_database.egg-info/top_level.txt
+-rw-r--r--   0 navy      (1000) navy      (1000)       38 2023-06-04 08:12:39.000000 lesscode_database-0.0.4/setup.cfg
+-rw-r--r--   0 navy      (1000) navy      (1000)     1198 2023-06-03 08:00:48.000000 lesscode_database-0.0.4/setup.py
```

### Comparing `lesscode_database-0.0.3/LICENSE` & `lesscode_database-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lesscode_database-0.0.3/README.md` & `lesscode_database-0.0.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,47 +1,74 @@
+Metadata-Version: 2.1
+Name: lesscode_database
+Version: 0.0.4
+Summary: lesscode_database是数据库连接工具包
+Author: navysummer
+Author-email: navysummer@yeah.net
+Platform: python
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # lesscode_database
 
 数据库连接工具包
 
 示例代码
 
 ```python
 import asyncio
 
-from sqlalchemy import MetaData, Table, Column, VARCHAR, INTEGER, select
+from sqlalchemy import select, Column, VARCHAR, INTEGER, Table, MetaData
 from sqlalchemy.ext.asyncio import async_sessionmaker
 from sqlalchemy.orm import sessionmaker
 
 from lesscode_database.connection_info import ConnectionInfo
 from lesscode_database.options import options
 
 options.conn_list = [
     ConnectionInfo(dialect="mysql", name="mysql", host="127.0.0.1", port=3306, user="root",
-                   password="root", db_name="test", enable=True, params={"pool_recycle": 3600},
+                   password="root", db_name="test", enable=False, params={"pool_recycle": 3600},
+                   async_enable=True),
+    ConnectionInfo(dialect="doris", name="doris", host="127.0.0.1", port=9030, user="root",
+                   password="root", db_name="test", enable=False, params={"pool_recycle": 3600},
+                   async_enable=True),
+    ConnectionInfo(dialect="ocean_base", name="ocean_base", host="127.0.0.1", port=2883, user="root",
+                   password="root", db_name="test", enable=False, params={"pool_recycle": 3600},
+                   async_enable=True),
+    ConnectionInfo(dialect="tidb", name="tidb", host="127.0.0.1", port=4000, user="root",
+                   password="root", db_name="test", enable=False, params={"pool_recycle": 3600},
                    async_enable=True),
+    ConnectionInfo(dialect="mssql", name="mssql", host="127.0.0.1", port=1433, user="root",
+                   password="root", db_name="test", enable=False, async_enable=False),
+    ConnectionInfo(dialect="oracle", name="oracle", host="127.0.0.1", port=1521, user="root",
+                   password="root", db_name="test", enable=False, async_enable=False),
+    ConnectionInfo(dialect="sqlite3", name="sqlite3", dsn="/test/test.db", async_enable=False),
     ConnectionInfo(dialect="elasticsearch", name="es", host="127.0.0.1", port=9210, user="root",
-                   password="root", enable=True, async_enable=True),
+                   password="root", enable=False, async_enable=True),
     ConnectionInfo(dialect="mongo", name="mongo", host="127.0.0.1", port=27027, user="root",
-                   password="root", enable=True, async_enable=True),
+                   password="root", enable=False, async_enable=True),
     ConnectionInfo(dialect="nebula", name="nebula", host="127.0.0.1", port=9669, user="root",
-                   password="nebula", db_name="nebula", enable=True),
+                   password="nebula", db_name="nebula", enable=False),
     ConnectionInfo(dialect="postgresql", host="127.0.0.1", port=5454, user="root", password="root",
-                   db_name="root", enable=True, async_enable=True),
+                   db_name="root", enable=False, async_enable=True),
     ConnectionInfo(dialect="redis", name="redis", host="127.0.0.1", port=6379, user=None,
-                   password=None, db_name=1, enable=True, async_enable=True),
+                   password=None, db_name=1, enable=False, async_enable=True),
+    # sqlalchemy 异步支持mysql，postgresql，tidb，ocean_base，doris;
+    # 同步支持mysql，postgresql，tidb，ocean_base，doris，sqlite3，mssql，oracle
     ConnectionInfo(dialect="sqlalchemy", name="sqlalchemy", host="127.0.0.1", port=3306, user="root",
-                   password="root", db_name="test", enable=True, async_enable=True),
+                   password="root", db_name="test", enable=False, async_enable=False, params={"db_type": "mysql"}),
     ConnectionInfo(dialect="neo4j", name="neo4j", host="127.0.0.1", port=7687, user="neo4j",
-                   password="neo4j", db_name=None, enable=True, async_enable=True),
+                   password="neo4j", db_name=None, enable=False, async_enable=True),
     ConnectionInfo(dialect="clickhouse", name="clickhouse", dsn="clickhouse://localhost", host="127.0.0.1", port=9000,
                    user="default", password="", db_name='', enable=True, async_enable=False),
 
 ]
-# 获取数据库连接池的方式
-## options.name    name是ConnectionInfo的name，options.conn_list里所有的name不可重复
 
 # mysql 同步测试，async_enable=False
 with options.mysql.dedicated_connection() as conn:
     conn.ping(reconnect=True)
     with conn.cursor() as cursor:
         cursor.execute("select 1")
         description = cursor.description
@@ -57,14 +84,98 @@
             rs = await cursor.fetchone()
             print(rs)
 
 
 loop = asyncio.get_event_loop()
 loop.run_until_complete(async_mysql_test())
 
+# doris 同步测试，async_enable=False
+with options.doris.dedicated_connection() as conn:
+    conn.ping(reconnect=True)
+    with conn.cursor() as cursor:
+        cursor.execute("select 1")
+        description = cursor.description
+        rs = cursor.fetchone()
+        print(rs)
+
+
+# doris 异步测试，async_enable=True
+async def async_doris_test():
+    async with options.doris.acquire() as conn:
+        async with conn.cursor() as cursor:
+            await cursor.execute("select 1")
+            rs = await cursor.fetchone()
+            print(rs)
+
+
+loop = asyncio.get_event_loop()
+loop.run_until_complete(async_doris_test())
+
+# ocean_base 同步测试，async_enable=False
+with options.ocean_base.dedicated_connection() as conn:
+    conn.ping(reconnect=True)
+    with conn.cursor() as cursor:
+        cursor.execute("select 1")
+        description = cursor.description
+        rs = cursor.fetchone()
+        print(rs)
+
+
+# ocean_base 异步测试，async_enable=True
+async def async_ocean_base_test():
+    async with options.ocean_base.acquire() as conn:
+        async with conn.cursor() as cursor:
+            await cursor.execute("select 1")
+            rs = await cursor.fetchone()
+            print(rs)
+
+
+loop = asyncio.get_event_loop()
+loop.run_until_complete(async_ocean_base_test())
+
+# tidb 同步测试，async_enable=False
+with options.tidb.dedicated_connection() as conn:
+    conn.ping(reconnect=True)
+    with conn.cursor() as cursor:
+        cursor.execute("select 1")
+        description = cursor.description
+        rs = cursor.fetchone()
+        print(rs)
+
+
+# tidb 异步测试，async_enable=True
+async def async_tidb_test():
+    async with options.tidb.acquire() as conn:
+        async with conn.cursor() as cursor:
+            await cursor.execute("select 1")
+            rs = await cursor.fetchone()
+            print(rs)
+
+
+loop = asyncio.get_event_loop()
+loop.run_until_complete(async_tidb_test())
+
+
+# sqlite3 异步测试
+async def async_sqlite3_test():
+    cur = await options.sqlite3.cursor()
+    await cur.execute("SELECT 1")
+    row = await cur.fetchone()
+    print(row)
+
+
+loop = asyncio.get_event_loop()
+loop.run_until_complete(async_sqlite3_test())
+
+# sqlite3 同步测试
+cursor = options.sqlite3.cursor()
+cursor.execute('select 1')
+row = cursor.fetchone()
+print(row)
+
 # es同步测试，async_enable=False
 body = {
     "query": {
         "bool": {
             "must": []
         }
     },
@@ -86,14 +197,31 @@
     )
     print(resp)
 
 
 loop = asyncio.get_event_loop()
 loop.run_until_complete(async_es_test())
 
+# sql server同步测试
+cursor = options.mssql.cursor()
+cursor.execute('SELECT 1')
+row = cursor.fetchone()
+print(row)
+
+# sql server暂不支持异步测试
+
+# oracle 同步测试
+cursor = options.oracle.cursor()
+cursor.execute('select 1')
+row = cursor.fetchone()
+print(row)
+
+# oracle暂不支持异步测试
+
+
 # mongo同步测试，async_enable=False
 print(options.mongo.test.test.find_one())
 
 
 # mongo异步测试，async_enable=True
 async def async_mongo_test():
     resp = await options.mongo.test.test.find_one()
@@ -142,15 +270,15 @@
 
 
 loop = asyncio.get_event_loop()
 loop.run_until_complete(async_redis_test())
 
 # sqlalchemy table
 meta = MetaData()
-t1 = Table("test", meta, Column("name", VARCHAR(collation='utf8mb3_bin', length=255)),
+t1 = Table("test_user", meta, Column("name", VARCHAR(collation='utf8mb3_bin', length=255)),
            Column(name='id', comment=None, nullable=False, autoincrement=False, primary_key=True, type_=INTEGER(),
                   server_default=None))
 
 # sqlalchemy同步测试，async_enable=False
 with sessionmaker(bind=options.sqlalchemy)() as session:
     cur = session.execute(select(t1))
     print(cur.fetchall())
@@ -166,33 +294,33 @@
 
 loop = asyncio.get_event_loop()
 loop.run_until_complete(async_sqlalchemy_test())
 
 
 # neo4j同步测试
 def query(tx):
-    nql = "MATCH (t:Test) return t limit 1"
+    nql = "MATCH (c:Company) return c limit 1"
     for record in tx.run(nql):
         print(record)
 
 
-with options.neo4j.session(database="test") as session:
+with options.neo4j.session(database="invest") as session:
     session.execute_read(query)
 
 
 # neo4j异步测试
 async def query(tx):
-    nql = "MATCH (t:Test) return t limit 1"
+    nql = "MATCH (c:Company) return c limit 1"
     res = await tx.run(nql)
     async for record in res:
         print(record)
 
 
 async def async_neo4j_test():
-    async with options.neo4j.session(database="test") as session:
+    async with options.neo4j.session(database="invest") as session:
         await session.execute_read(query)
 
 
 loop = asyncio.get_event_loop()
 loop.run_until_complete(async_neo4j_test())
 
 # clickhouse 同步测试
@@ -210,8 +338,9 @@
             ret = await cursor.fetchone()
             print(ret)
 
 
 loop = asyncio.get_event_loop()
 loop.run_until_complete(async_clickhouse_test())
 
+
 ```
```

### Comparing `lesscode_database-0.0.3/lesscode_database/connect_pool.py` & `lesscode_database-0.0.4/lesscode_database/connect_pool.py`

 * *Files 22% similar despite different names*

```diff
@@ -120,15 +120,15 @@
         创建mysql 异步连接池
         :param conn_info: 连接信息
         :return:
         """
         try:
             aiomysql = importlib.import_module("aiomysql")
         except ImportError:
-            raise Exception(f"pymysql is not exist,run:pip install aiomysql")
+            raise Exception(f"aiomysql is not exist,run:pip install aiomysql")
         pool = await aiomysql.create_pool(host=conn_info.host, port=conn_info.port,
                                           user=conn_info.user,
                                           password=conn_info.password,
                                           pool_recycle=conn_info.params.get("pool_recycle", 3600)
                                           if conn_info.params else 3600,
                                           db=conn_info.db_name, autocommit=True,
                                           minsize=conn_info.min_size,
@@ -156,14 +156,235 @@
                                   mincached=conn_info.min_size, blocking=True, maxusage=conn_info.min_size,
                                   maxshared=conn_info.max_size, maxcached=conn_info.max_size,
                                   ping=1, maxconnections=conn_info.max_size, charset="utf8mb4", autocommit=True,
                                   read_timeout=30)
         return pool
 
     @staticmethod
+    async def create_sqlite3_pool(conn_info: ConnectionInfo):
+        """
+        创建mysql 异步连接池
+        :param conn_info: 连接信息
+        :return:
+        """
+        try:
+            aiosqlite3 = importlib.import_module("aiosqlite3")
+        except ImportError:
+            raise Exception(f"aiosqlite3 is not exist,run:pip install aiosqlite3")
+        pool = await aiosqlite3.connect(database=conn_info.dsn)
+        return pool
+
+    @staticmethod
+    def sync_create_sqlite3_pool(conn_info: ConnectionInfo):
+        """
+        创建mysql 同步连接池
+        :param conn_info: 连接信息
+        :return:
+        """
+        try:
+            sqlite3 = importlib.import_module("sqlite3")
+        except ImportError:
+            raise Exception(f"sqlite3 is not exist,run:pip install sqlite3")
+        try:
+            pooled_db = importlib.import_module("dbutils.pooled_db")
+        except ImportError:
+            raise Exception(f"DBUtils is not exist,run:pip install DBUtils")
+        pool = pooled_db.PooledDB(creator=sqlite3, host=conn_info.host, port=conn_info.port,
+                                  user=conn_info.user,
+                                  passwd=conn_info.password, db=conn_info.db_name,
+                                  mincached=conn_info.min_size, blocking=True, maxusage=conn_info.min_size,
+                                  maxshared=conn_info.max_size, maxcached=conn_info.max_size,
+                                  ping=1, maxconnections=conn_info.max_size, charset="utf8mb4", autocommit=True,
+                                  read_timeout=30)
+        return pool
+
+    @staticmethod
+    def sync_create_mssql_pool(conn_info: ConnectionInfo):
+        """
+        创建mysql 同步连接池
+        :param conn_info: 连接信息
+        :return:
+        """
+        try:
+            pymssql = importlib.import_module("pymssql")
+        except ImportError:
+            raise Exception(f"pymssql is not exist,run:pip install pymssql")
+        try:
+            pooled_db = importlib.import_module("dbutils.pooled_db")
+        except ImportError:
+            raise Exception(f"DBUtils is not exist,run:pip install DBUtils")
+        pool = pooled_db.PooledDB(creator=pymssql, host=conn_info.host, port=conn_info.port,
+                                  user=conn_info.user,
+                                  passwd=conn_info.password, db=conn_info.db_name,
+                                  mincached=conn_info.min_size, blocking=True, maxusage=conn_info.min_size,
+                                  maxshared=conn_info.max_size, maxcached=conn_info.max_size,
+                                  ping=1, maxconnections=conn_info.max_size, charset="utf8mb4", autocommit=True,
+                                  read_timeout=30)
+        return pool
+
+    @staticmethod
+    def sync_create_oracle_pool(conn_info: ConnectionInfo):
+        """
+        创建mysql 同步连接池
+        :param conn_info: 连接信息
+        :return:
+        """
+        try:
+            cx_oracle = importlib.import_module("cx_Oracle")
+        except ImportError:
+            raise Exception(f"cx_Oracle is not exist,run:pip install cx_Oracle")
+        try:
+            pooled_db = importlib.import_module("dbutils.pooled_db")
+        except ImportError:
+            raise Exception(f"DBUtils is not exist,run:pip install DBUtils")
+        pool = pooled_db.PooledDB(creator=cx_oracle, host=conn_info.host, port=conn_info.port,
+                                  user=conn_info.user,
+                                  passwd=conn_info.password, db=conn_info.db_name,
+                                  mincached=conn_info.min_size, blocking=True, maxusage=conn_info.min_size,
+                                  maxshared=conn_info.max_size, maxcached=conn_info.max_size,
+                                  ping=1, maxconnections=conn_info.max_size, charset="utf8mb4", autocommit=True,
+                                  read_timeout=30)
+        return pool
+
+    @staticmethod
+    async def create_doris_pool(conn_info: ConnectionInfo):
+        """
+        创建doris 异步连接池
+        :param conn_info: 连接信息
+        :return:
+        """
+        try:
+            aiomysql = importlib.import_module("aiomysql")
+        except ImportError:
+            raise Exception(f"aiomysql is not exist,run:pip install aiomysql")
+        pool = await aiomysql.create_pool(host=conn_info.host, port=conn_info.port,
+                                          user=conn_info.user,
+                                          password=conn_info.password,
+                                          pool_recycle=conn_info.params.get("pool_recycle", 3600)
+                                          if conn_info.params else 3600,
+                                          db=conn_info.db_name, autocommit=True,
+                                          minsize=conn_info.min_size,
+                                          maxsize=conn_info.max_size)
+        return pool
+
+    @staticmethod
+    def sync_create_doris_pool(conn_info: ConnectionInfo):
+        """
+        创建doris 同步连接池
+        :param conn_info: 连接信息
+        :return:
+        """
+        try:
+            pymysql = importlib.import_module("pymysql")
+        except ImportError:
+            raise Exception(f"pymysql is not exist,run:pip install pymysql")
+        try:
+            pooled_db = importlib.import_module("dbutils.pooled_db")
+        except ImportError:
+            raise Exception(f"DBUtils is not exist,run:pip install DBUtils")
+        pool = pooled_db.PooledDB(creator=pymysql, host=conn_info.host, port=conn_info.port,
+                                  user=conn_info.user,
+                                  passwd=conn_info.password, db=conn_info.db_name,
+                                  mincached=conn_info.min_size, blocking=True, maxusage=conn_info.min_size,
+                                  maxshared=conn_info.max_size, maxcached=conn_info.max_size,
+                                  ping=1, maxconnections=conn_info.max_size, charset="utf8mb4", autocommit=True,
+                                  read_timeout=30)
+        return pool
+
+    @staticmethod
+    async def create_tidb_pool(conn_info: ConnectionInfo):
+        """
+        创建tidb 异步连接池
+        :param conn_info: 连接信息
+        :return:
+        """
+        try:
+            aiomysql = importlib.import_module("aiomysql")
+        except ImportError:
+            raise Exception(f"aiomysql is not exist,run:pip install aiomysql")
+        pool = await aiomysql.create_pool(host=conn_info.host, port=conn_info.port,
+                                          user=conn_info.user,
+                                          password=conn_info.password,
+                                          pool_recycle=conn_info.params.get("pool_recycle", 3600)
+                                          if conn_info.params else 3600,
+                                          db=conn_info.db_name, autocommit=True,
+                                          minsize=conn_info.min_size,
+                                          maxsize=conn_info.max_size)
+        return pool
+
+    @staticmethod
+    def sync_create_tidb_pool(conn_info: ConnectionInfo):
+        """
+        创建tidb 同步连接池
+        :param conn_info: 连接信息
+        :return:
+        """
+        try:
+            pymysql = importlib.import_module("pymysql")
+        except ImportError:
+            raise Exception(f"pymysql is not exist,run:pip install pymysql")
+        try:
+            pooled_db = importlib.import_module("dbutils.pooled_db")
+        except ImportError:
+            raise Exception(f"DBUtils is not exist,run:pip install DBUtils")
+        pool = pooled_db.PooledDB(creator=pymysql, host=conn_info.host, port=conn_info.port,
+                                  user=conn_info.user,
+                                  passwd=conn_info.password, db=conn_info.db_name,
+                                  mincached=conn_info.min_size, blocking=True, maxusage=conn_info.min_size,
+                                  maxshared=conn_info.max_size, maxcached=conn_info.max_size,
+                                  ping=1, maxconnections=conn_info.max_size, charset="utf8mb4", autocommit=True,
+                                  read_timeout=30)
+        return pool
+
+    @staticmethod
+    async def create_ocean_base_pool(conn_info: ConnectionInfo):
+        """
+        创建ocean_base 异步连接池
+        :param conn_info: 连接信息
+        :return:
+        """
+        try:
+            aiomysql = importlib.import_module("aiomysql")
+        except ImportError:
+            raise Exception(f"aiomysql is not exist,run:pip install aiomysql")
+        pool = await aiomysql.create_pool(host=conn_info.host, port=conn_info.port,
+                                          user=conn_info.user,
+                                          password=conn_info.password,
+                                          pool_recycle=conn_info.params.get("pool_recycle", 3600)
+                                          if conn_info.params else 3600,
+                                          db=conn_info.db_name, autocommit=True,
+                                          minsize=conn_info.min_size,
+                                          maxsize=conn_info.max_size)
+        return pool
+
+    @staticmethod
+    def sync_create_ocean_base_pool(conn_info: ConnectionInfo):
+        """
+        创建ocean_base 同步连接池
+        :param conn_info: 连接信息
+        :return:
+        """
+        try:
+            pymysql = importlib.import_module("pymysql")
+        except ImportError:
+            raise Exception(f"pymysql is not exist,run:pip install pymysql")
+        try:
+            pooled_db = importlib.import_module("dbutils.pooled_db")
+        except ImportError:
+            raise Exception(f"DBUtils is not exist,run:pip install DBUtils")
+        pool = pooled_db.PooledDB(creator=pymysql, host=conn_info.host, port=conn_info.port,
+                                  user=conn_info.user,
+                                  passwd=conn_info.password, db=conn_info.db_name,
+                                  mincached=conn_info.min_size, blocking=True, maxusage=conn_info.min_size,
+                                  maxshared=conn_info.max_size, maxcached=conn_info.max_size,
+                                  ping=1, maxconnections=conn_info.max_size, charset="utf8mb4", autocommit=True,
+                                  read_timeout=30)
+        return pool
+
+    @staticmethod
     def sync_create_nebula_pool(conn_info: ConnectionInfo):
         """
         创建nebula3连接池
         :param conn_info: 连接信息
         :return: 
         """
         try:
@@ -423,14 +644,18 @@
                 url = 'mysql+aiomysql://{}:{}@{}:{}/{}?charset=utf8mb4'.format(
                     conn_info.user, conn_info.password, conn_info.host, conn_info.port,
                     conn_info.db_name)
             elif db_type == "ocean_base":
                 url = 'mysql+aiomysql://{}:{}@{}:{}/{}?charset=utf8mb4'.format(
                     conn_info.user, conn_info.password, conn_info.host, conn_info.port,
                     conn_info.db_name)
+            elif db_type == "doris":
+                url = 'mysql+aiomysql://{}:{}@{}:{}/{}?charset=utf8mb4'.format(
+                    conn_info.user, conn_info.password, conn_info.host, conn_info.port,
+                    conn_info.db_name)
             else:
                 raise Exception("UNSUPPORTED DB TYPE")
         try:
             sqlalchemy = importlib.import_module("sqlalchemy.ext.asyncio")
         except ImportError:
             raise Exception(f"sqlalchemy is not exist,run:pip install sqlalchemy")
         engine = sqlalchemy.create_async_engine(url, echo=conn_info.params.get("echo",
@@ -472,14 +697,28 @@
                 url = 'mysql+pymysql://{}:{}@{}:{}/{}?charset=utf8mb4'.format(
                     conn_info.user, conn_info.password, conn_info.host, conn_info.port,
                     conn_info.db_name)
             elif db_type == "ocean_base":
                 url = 'mysql+pymysql://{}:{}@{}:{}/{}?charset=utf8mb4'.format(
                     conn_info.user, conn_info.password, conn_info.host, conn_info.port,
                     conn_info.db_name)
+            elif db_type == "doris":
+                url = 'mysql+pymysql://{}:{}@{}:{}/{}?charset=utf8mb4'.format(
+                    conn_info.user, conn_info.password, conn_info.host, conn_info.port,
+                    conn_info.db_name)
+            elif db_type == "sqlite3":
+                url = conn_info.dsn
+            elif db_type == "mssql":
+                url = "mssql+pymssql://{}:{}@{}:{}/{}?charset=utf8mb4".format(
+                    conn_info.user, conn_info.password, conn_info.host, conn_info.port,
+                    conn_info.db_name)
+            elif db_type == "oracle":
+                url = "oracle+cx_oracle://{}:{}@{}:{}/{}?charset=utf8mb4".format(
+                    conn_info.user, conn_info.password, conn_info.host, conn_info.port,
+                    conn_info.db_name)
             else:
                 raise Exception("UNSUPPORTED DB TYPE")
         try:
             sqlalchemy = importlib.import_module("sqlalchemy")
         except ImportError:
             raise Exception(f"sqlalchemy is not exist,run:pip install sqlalchemy")
         engine = sqlalchemy.create_engine(url, echo=conn_info.params.get("echo",
@@ -521,14 +760,38 @@
 
     elif conn_info.dialect == "mysql":
         if conn_info.async_enable:
             return run_sync(Pool.create_mysql_pool(conn_info))
         else:
             return run_sync(Pool.sync_create_mysql_pool(conn_info))
 
+    elif conn_info.dialect == "doris":
+        if conn_info.async_enable:
+            return run_sync(Pool.create_doris_pool(conn_info))
+        else:
+            return run_sync(Pool.sync_create_doris_pool(conn_info))
+
+    elif conn_info.dialect == "ocean_base":
+        if conn_info.async_enable:
+            return run_sync(Pool.create_ocean_base_pool(conn_info))
+        else:
+            return run_sync(Pool.sync_create_ocean_base_pool(conn_info))
+
+    elif conn_info.dialect == "tidb":
+        if conn_info.async_enable:
+            return run_sync(Pool.create_tidb_pool(conn_info))
+        else:
+            return run_sync(Pool.sync_create_tidb_pool(conn_info))
+
+    elif conn_info.dialect == "mssql":
+        return run_sync(Pool.sync_create_mssql_pool(conn_info))
+
+    elif conn_info.dialect == "oracle":
+        return run_sync(Pool.sync_create_oracle_pool(conn_info))
+
     elif conn_info.dialect == "nebula":
         return run_sync(Pool.sync_create_nebula_pool(conn_info))
 
     elif conn_info.dialect == "neo4j":
         if conn_info.async_enable:
             return run_sync(Pool.create_neo4j_pool(conn_info))
         else:
@@ -536,14 +799,20 @@
 
     elif conn_info.dialect == "postgresql":
         if conn_info.async_enable:
             return run_sync(Pool.create_postgresql_pool(conn_info))
         else:
             return run_sync(Pool.sync_create_postgresql_pool(conn_info))
 
+    elif conn_info.dialect == "sqlite3":
+        if conn_info.async_enable:
+            return run_sync(Pool.create_sqlite3_pool(conn_info))
+        else:
+            return run_sync(Pool.sync_create_sqlite3_pool(conn_info))
+
     elif conn_info.dialect == "redis":
         if conn_info.async_enable:
             return run_sync(Pool.create_redis_pool(conn_info))
         else:
             return run_sync(Pool.sync_create_redis_pool(conn_info))
 
     elif conn_info.dialect == "redis_cluster":
```

### Comparing `lesscode_database-0.0.3/lesscode_database/connection_info.py` & `lesscode_database-0.0.4/lesscode_database/connection_info.py`

 * *Files identical despite different names*

### Comparing `lesscode_database-0.0.3/lesscode_database/options.py` & `lesscode_database-0.0.4/lesscode_database/options.py`

 * *Files identical despite different names*

### Comparing `lesscode_database-0.0.3/setup.py` & `lesscode_database-0.0.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,10 +38,10 @@
 # 检查
 twine check dist/*
 
 # 上传pypi
 twine upload dist/*
 twine upload dist/* --repository-url https://pypi.chanyeos.com/ -u admin -p shangqi
 # 安装最新的版本测试
-pip install -U lesscode_charts -i https://pypi.org/simple
-pip install -U lesscode_charts -i https://pypi.chanyeos.com/simple
+pip install -U lesscode_database -i https://pypi.org/simple
+pip install -U lesscode_database -i https://pypi.chanyeos.com/simple
 """
```

