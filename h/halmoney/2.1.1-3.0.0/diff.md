# Comparing `tmp/halmoney-2.1.1.tar.gz` & `tmp/halmoney-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "halmoney-2.1.1.tar", last modified: Thu Dec  1 12:07:48 2022, max compression
+gzip compressed data, was "halmoney-3.0.0.tar", last modified: Sun Jun  4 09:00:48 2023, max compression
```

## Comparing `halmoney-2.1.1.tar` & `halmoney-3.0.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxrwxrwx   0        0        0        0 2022-12-01 12:07:48.823538 halmoney-2.1.1/
--rw-rw-rw-   0        0        0      372 2022-12-01 11:19:44.000000 halmoney-2.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     9034 2022-12-01 12:07:48.823538 halmoney-2.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     8503 2022-12-01 12:04:55.000000 halmoney-2.1.1/README.md
--rw-rw-rw-   0        0        0        0 2021-06-11 06:00:16.000000 halmoney-2.1.1/requirements.txt
--rw-rw-rw-   0        0        0       86 2022-12-01 12:07:48.826250 halmoney-2.1.1/setup.cfg
--rw-rw-rw-   0        0        0      905 2022-12-01 12:07:29.000000 halmoney-2.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2022-12-01 12:07:48.763253 halmoney-2.1.1/src/
-drwxrwxrwx   0        0        0        0 2022-12-01 12:07:48.802251 halmoney-2.1.1/src/halmoney/
--rw-rw-rw-   0        0        0      476 2022-12-01 11:17:11.000000 halmoney-2.1.1/src/halmoney/__init__.py
--rw-rw-rw-   0        0        0    21644 2022-11-20 08:04:33.000000 halmoney-2.1.1/src/halmoney/anydb.py
--rw-rw-rw-   0        0        0    20275 2022-11-27 12:05:08.000000 halmoney-2.1.1/src/halmoney/basic_data.py
--rw-rw-rw-   0        0        0    15583 2022-11-25 11:29:47.000000 halmoney-2.1.1/src/halmoney/jfinder.py
--rw-rw-rw-   0        0        0     5206 2022-11-17 10:14:09.000000 halmoney-2.1.1/src/halmoney/mail.py
--rw-rw-rw-   0        0        0   120735 2022-11-28 14:09:19.000000 halmoney-2.1.1/src/halmoney/pcell.py
--rw-rw-rw-   0        0        0     5681 2022-10-28 12:07:57.000000 halmoney-2.1.1/src/halmoney/pcell_event.py
--rw-rw-rw-   0        0        0    17559 2022-11-22 13:17:58.000000 halmoney-2.1.1/src/halmoney/pynal.py
--rw-rw-rw-   0        0        0    42831 2022-11-27 13:16:44.000000 halmoney-2.1.1/src/halmoney/scolor.py
--rw-rw-rw-   0        0        0     5235 2022-11-20 08:04:33.000000 halmoney-2.1.1/src/halmoney/word.py
--rw-rw-rw-   0        0        0    72610 2022-11-28 10:57:32.000000 halmoney-2.1.1/src/halmoney/youtil.py
-drwxrwxrwx   0        0        0        0 2022-12-01 12:07:48.821252 halmoney-2.1.1/src/halmoney.egg-info/
--rw-rw-rw-   0        0        0     9034 2022-12-01 12:07:48.000000 halmoney-2.1.1/src/halmoney.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      494 2022-12-01 12:07:48.000000 halmoney-2.1.1/src/halmoney.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-01 12:07:48.000000 halmoney-2.1.1/src/halmoney.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-12-01 11:49:45.000000 halmoney-2.1.1/src/halmoney.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2022-12-01 12:07:48.000000 halmoney-2.1.1/src/halmoney.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-04 09:00:48.720870 halmoney-3.0.0/
+-rw-rw-rw-   0        0        0      410 2023-06-04 08:57:31.000000 halmoney-3.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     9258 2023-06-04 09:00:48.721064 halmoney-3.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     8724 2023-06-04 08:56:16.000000 halmoney-3.0.0/README.md
+-rw-rw-rw-   0        0        0        0 2021-06-11 06:00:16.000000 halmoney-3.0.0/requirements.txt
+-rw-rw-rw-   0        0        0       86 2023-06-04 09:00:48.723879 halmoney-3.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      905 2023-06-04 08:50:05.000000 halmoney-3.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 09:00:48.642866 halmoney-3.0.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-04 09:00:48.687844 halmoney-3.0.0/src/halmoney/
+-rw-rw-rw-   0        0        0      476 2023-06-04 08:47:42.000000 halmoney-3.0.0/src/halmoney/__init__.py
+-rw-rw-rw-   0        0        0    23159 2023-05-14 09:19:38.000000 halmoney-3.0.0/src/halmoney/anydb.py
+-rw-rw-rw-   0        0        0    80419 2023-06-03 06:07:50.000000 halmoney-3.0.0/src/halmoney/basic_data.py
+-rw-rw-rw-   0        0        0    24552 2023-05-23 21:32:30.000000 halmoney-3.0.0/src/halmoney/ganada.py
+-rw-rw-rw-   0        0        0    19604 2023-05-22 13:41:17.000000 halmoney-3.0.0/src/halmoney/jfinder.py
+-rw-rw-rw-   0        0        0    24532 2023-05-23 21:32:30.000000 halmoney-3.0.0/src/halmoney/mailmail.py
+-rw-rw-rw-   0        0        0   141238 2023-06-04 07:04:32.000000 halmoney-3.0.0/src/halmoney/pcell.py
+-rw-rw-rw-   0        0        0     5736 2023-04-08 04:25:55.000000 halmoney-3.0.0/src/halmoney/pcell_event.py
+-rw-rw-rw-   0        0        0    11415 2023-05-22 13:34:23.000000 halmoney-3.0.0/src/halmoney/pyclick.py
+-rw-rw-rw-   0        0        0    36331 2023-05-23 20:51:47.000000 halmoney-3.0.0/src/halmoney/pynal.py
+-rw-rw-rw-   0        0        0    34869 2023-05-29 02:11:51.000000 halmoney-3.0.0/src/halmoney/scolor.py
+-rw-rw-rw-   0        0        0    52683 2023-06-04 07:06:03.000000 halmoney-3.0.0/src/halmoney/youtil.py
+drwxrwxrwx   0        0        0        0 2023-06-04 09:00:48.717814 halmoney-3.0.0/src/halmoney.egg-info/
+-rw-rw-rw-   0        0        0     9258 2023-06-04 09:00:48.000000 halmoney-3.0.0/src/halmoney.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      524 2023-06-04 09:00:48.000000 halmoney-3.0.0/src/halmoney.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 09:00:48.000000 halmoney-3.0.0/src/halmoney.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-12-01 11:49:45.000000 halmoney-3.0.0/src/halmoney.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        9 2023-06-04 09:00:48.000000 halmoney-3.0.0/src/halmoney.egg-info/top_level.txt
```

### Comparing `halmoney-2.1.1/PKG-INFO` & `halmoney-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: halmoney
-Version: 2.1.1
+Version: 3.0.0
 Summary: Easy Read / Write for Excel, Word, Color, Etc using Python
 Home-page: https://github.com/sjpark/halmoney
-Download-URL: https://github.com/sjpark/halmoney/archive/v2.1.1.tar.gz
+Download-URL: https://github.com/sjpark/halmoney/archive/v3.0.0.tar.gz
 Author: sjpark
 Author-email: sjpkorea@yahoo.com
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 
 ## Halmoney 모듈에 대하여
@@ -24,22 +24,25 @@
 또한 보통 많이 사용하는 코드들은 첨부된 sample코드를 보시거나 저의 사이트에 와서 비슷한것을 다운 받은후
 변경해서 사용하시기를 추천 드립니다
 
 좀더 편한 업무의 일을 하기위한 것입니다
 
 ### 구성은 
 
+    - anydb : sqlite와 pandas 를 좀더 쉽게 사용할수있도록 만든것
+    - basic_data : halmoney패키지에서 사용되는 전반적인 공유 자료들을 저장하는 곳
+    - ganada : 워드를 다루기위해 만든 것
+    - jfinder : 정규표현식을 좀더 편하게 사용하도록 만든 것
+    - mailmail : outlook을 다루는것
     - pcell : 엑셀을 다루는 것
     - pcell_event : 엑셀의 이벤트를 다루는것
+    - pyclick : 키보드와 마우스를 다루는 모듈
+    - pynal : 시간과 날짜를 다루는것
     - scolor : 색의 RGB값을 편하게 사용가능하도록 만든 것
-    - jfinder : 정규표현식을 좀더 편하게 사용하도록 만든 것
     - youtil : 이러저런 문장이나 시간등을 변환하는데 도움이되는 것
-    - mail : outlook을 다루는것
-    - pynal : 시간과 날짜를 다루는것
-    - anydb : sqlite와 pandas 를 좀더 쉽게 사용할수있도록 만든것
 
 각 사용사용방법들에 대해서는 아래의 사이트를 참고하세요
 
 * https://cafe.naver.com/pycell
 * www.halmoney.com
```

### Comparing `halmoney-2.1.1/README.md` & `halmoney-3.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -12,22 +12,25 @@
 또한 보통 많이 사용하는 코드들은 첨부된 sample코드를 보시거나 저의 사이트에 와서 비슷한것을 다운 받은후
 변경해서 사용하시기를 추천 드립니다
 
 좀더 편한 업무의 일을 하기위한 것입니다
 
 ### 구성은 
 
+    - anydb : sqlite와 pandas 를 좀더 쉽게 사용할수있도록 만든것
+    - basic_data : halmoney패키지에서 사용되는 전반적인 공유 자료들을 저장하는 곳
+    - ganada : 워드를 다루기위해 만든 것
+    - jfinder : 정규표현식을 좀더 편하게 사용하도록 만든 것
+    - mailmail : outlook을 다루는것
     - pcell : 엑셀을 다루는 것
     - pcell_event : 엑셀의 이벤트를 다루는것
+    - pyclick : 키보드와 마우스를 다루는 모듈
+    - pynal : 시간과 날짜를 다루는것
     - scolor : 색의 RGB값을 편하게 사용가능하도록 만든 것
-    - jfinder : 정규표현식을 좀더 편하게 사용하도록 만든 것
     - youtil : 이러저런 문장이나 시간등을 변환하는데 도움이되는 것
-    - mail : outlook을 다루는것
-    - pynal : 시간과 날짜를 다루는것
-    - anydb : sqlite와 pandas 를 좀더 쉽게 사용할수있도록 만든것
 
 각 사용사용방법들에 대해서는 아래의 사이트를 참고하세요
 
 * https://cafe.naver.com/pycell
 * www.halmoney.com
```

### Comparing `halmoney-2.1.1/setup.py` & `halmoney-3.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup, find_packages
 #with open("README.md", "rt", encoding='UTF8') as fh:
 #    long_description = fh.read()
 setup(
     name='halmoney',
-    version='2.1.1',
+    version='3.0.0',
     url='https://github.com/sjpark/halmoney',
-    download_url='https://github.com/sjpark/halmoney/archive/v2.1.1.tar.gz',
+    download_url='https://github.com/sjpark/halmoney/archive/v3.0.0.tar.gz',
     author='sjpark',
     author_email='sjpkorea@yahoo.com',
     description='Easy Read / Write for Excel, Word, Color, Etc using Python',
     packages=find_packages("src"),
     package_dir={"": "src"},
     include_package_data=True,
     package_data={
```

### Comparing `halmoney-2.1.1/src/halmoney/anydb.py` & `halmoney-3.0.0/src/halmoney/anydb.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,659 +1,661 @@
 # -*- coding: utf-8 -*-
-import os
-import sqlite3
-import pandas as pd
-from halmoney import youtil, pcell
-
-vars = {}
+import os  # 내장모듈
+import sqlite3  # 내장모듈
+import pickle #내장모듈
 
-class anydb:
-	def __init__(self, db_name="", path=""):
-		"""
-		databse가 있는 화일의 위치를 알려주면 시작이 된다
-		pandas의 장점
-		1. 대용량 데이터(GB 단위 이상)를 다룰 수 있습니다. 엑셀은 데이터 용량이 100MB을 넘어가거나, 데이터가 100만 행이 넘어가면 정상적으로 작동하지 않는 현상을 겪기도 합니다.
-		2. 복잡한 처리 작업들을 비교적 손쉽게 할 수 있습니다. 소위 말하는 엑셀 노가다를 할 필요가 없습니다.
-		3. 손쉽게 데이터를 결합하고 분리할 수 있습니다. SQL처럼 데이터를 합치고 관계 연산을 수행할 수 있습니다.
+import youtil  # halmoney 모듈
+import pcell  # halmoney 모듈
 
-		df.index, df.columns, df.values
-		df["col1"], df[1:3]
+import pandas as pd
+import numpy as np
 
-		index는 숫자만 가능하지 않고, String(문자열) 일 수도 있다.
-		index가 숫자여도 순서대로 정렬될 필요가 없다. 그리고 index는 중복될 수 있다.
-		print(df.loc[:3, ['Surv', 'N']])
+class anydb:
+	"""
+	database를 사용하기 쉽게 만든것
+	table, df의 자료는 [제일 첫컬럼에 컬럼이름을 넣는다]
+	"""
 
-		df[val]	Select single column or sequence of columns from the DataFrame
-		df.loc[val]	Selects single row or subset of rows from the DataFrame by label
-		df.loc[:, val]	Selects single column or subset of columns by label
-		df.loc[val1, val2]	Select both rows and columns by label
-		df.iloc[where]	Selects single row or subset of rows from the DataFrame by integer position
-		df.iloc[:, where]	Selects single column or subset of columns by integer position
-		df.iloc[where_i, whe	re_j] Select both rows and columns by integer position
-		df.at[label_i, label	_j] Select a single scalar value by row and column label
-		df.iat[i, j]	Select a single scalar value by row and column position (integers)
-		get_value(), set_val	ue() Select single value by row and column label
-		"""
+	def __init__(self, db_name=""):
 		self.yt = youtil.youtil()
 		self.db_name = db_name
 		self.table_name = ""
 
-		self.con = ""
-		self.curs = ""
-		self.path = path
-		self.connect_db(db_name, path)
+		self.con = ""  # sqlite db에 연결되는 것
+		self.cursor = ""
+		self.make_connection_with_sqlite_db(self.db_name)
 
-	def add_df1_to_df2(self, input_df_1, input_df_2):
+	def append_df1_df2(self, df_obj_1, df_obj_2):
 		"""
-		input_df_1의 자료에 input_df_2를 맨끝에 추가하는것
+		dataframe끝에 dataframe형태의 자료를 추가하는것
 		"""
-		input_df_1 = pd.concat([input_df_1, input_df_2])
-		return input_df_1
+		result = pd.concat([df_obj_1, df_obj_2])
+		return result
 
 	def change_df_to_dic(self, input_df, style="split"):
 		"""
 		입력형태 : data = {"calory": [123, 456, 789], "기간": [10, 40, 20]}
 		출력형태 : dataframe
+		dict :    {'제목1': {'가로제목1': 1, '가로제목2': 3}, '제목2': {'가로제목1': 2, '가로제목2': 4}}
+		list :    {'제목1': [1, 2], '제목2': [3, 4]}
+		series :  {열 : Series, 열 : Series}
+		split :   {'index': ['가로제목1', '가로제목2'], 'columns': ['제목1', '제목2'], 'data': [[1, 2], [3, 4]]}
+		records : [{'제목1': 1, '제목2': 2}, {'제목1': 3, '제목2': 4}]
+		index :   {'가로제목1': {'제목1': 1, '제목2': 2}, '가로제목2': {'제목1': 3, '제목2': 4}}
 		"""
 		checked_style = style
 		if not style in ["split", "list", 'series', 'records', 'index']:
 			checked_style = "split"
 		result = input_df.to_dict(checked_style)
 		return result
 
-	def change_list_to_df(self, list2d="", col_list=""):
+	def change_df_to_list(self, df_obj):
+		"""
+		df자료를 커럼과 값을 기준으로 나누어서 결과를 리스트로 돌려주는 것이다
+		"""
+		col_list = df_obj.columns.values.tolist()
+		value_list = df_obj.values.tolist()
+		col_list.extend(value_list)
+		return col_list
+
+	def change_dic_to_sql_data(self, dic_data):
+		"""
+		사전의 자료를 sql에 입력이 가능한 형식으로 만드는 것
+		결과 : [[컬럼리스트], [자료1], [자료2]....]
+		"""
+		col_list = list(dic_data[0].keys())
+		value_list =[]
+		for one_col in col_list:
+			value_list.append(dic_data[one_col])
+		result = [col_list, value_list]
+		return result
+
+	def change_list2d_to_df(self, col_list="", list2d=""):
 		"""
 		리스트 자료를 dataframe로 만드는것
 		입력형태 : 제목리스트, 2차원 값리스트형
 		출력형태 : dataframe로 바꾼것
 		"""
 		checked_list2d = self.yt.change_list1d_to_list2d(list2d)
 		checked_col_list = []
-		#컬럼의 이름이 없거나하면 기본적인 이름을 만드는 것이다
+		# 컬럼의 이름이 없거나하면 기본적인 이름을 만드는 것이다
 		if col_list == "" or col_list == []:
 			for num in range(len(checked_list2d)):
-				checked_col_list.append("col"+str(num))
+				checked_col_list.append("col" + str(num))
 		else:
 			checked_col_list = col_list
 		input_df = pd.DataFrame(data=checked_list2d, columns=col_list)
 		return input_df
 
-	def change_table_name(self, table_name_old, table_name_new):
-		"""
-		입력형태 :
-		출력형태 :
-		"""
-		new_sql = "alter table %s rename to %s" % (table_name_old, table_name_new)
-		self.run_sql(new_sql)
-
-	def change_tabledata_to_df(self, db_name, table_name):
+	def change_sqlite_table_to_df(self, table_name, db_name=""):
 		"""
-		sqlite를 df로 만드는것
-		입력형태 :
-		출력형태 :
+		sqlite의 테이블을 df로 변경
 		"""
-		if self.con == "":
-			self.con = sqlite3.connect(db_name, isolation_level=None)
-		self.curs = self.con.cursor()
-		sql = ("SELECT * From {}").format(table_name)
-		query = self.curs.execute(sql)
-		cols = [column[0] for column in query.description]
-		input_df = pd.DataFrame.from_records(data=query.fetchall(), columns=cols)
+		self.check_cursor(db_name)
+		sql = "SELECT * From {}".format(table_name)
+		sql_result = self.cursor.execute(sql)
+		cols = []
+		for column in sql_result.description:
+			cols.append(column[0])
+		input_df = pd.DataFrame.from_records(data=sql_result.fetchall(), columns=cols)
 		return input_df
 
-	def change_tabledata_to_list(self, db_name, table_name):
+	def change_sqlite_table_to_list(self, table_name, db_name=""):
 		"""
-		sqlite를 df로 만드는것
-		입력형태 :
+		sqlite의 테이블 자료를 리스트로 변경
 		출력형태 :[2차원리스트(제목), 2차원리스트(값들)]
 		"""
-		if self.con == "":
-			self.con = sqlite3.connect(db_name, isolation_level=None)
-		self.con.row_factory = sqlite3.Row
-		self.curs = self.con.cursor()
-		sql = "SELECT * From {}".format(table_name)
-		query = self.curs.execute(sql)
-		cols = [column[0] for column in query.description]
-
-		aaa = []
-		for one in query.fetchall():
-			aaa.append(list(one))
-		result =[cols, aaa]
+		self.check_cursor(db_name)
+		sql_result = self.cursor.execute("SELECT * From {}".format(table_name))
+		cols = []
+		for column in sql_result.description:
+			cols.append(column[0])
+		temp = []
+		for one in sql_result.fetchall():
+			temp.append(list(one))
+		result = [cols, temp]
 		return result
 
-	def check_col_name(self, col_name):
-		for data1, data2 in [["'", ""], ["/", ""], ["\\", ""], [".", ""]]:
-				col_name = col_name.replace(data1, data2)
-		return col_name
-
-	def check_db_name(self, db_name, path="."):
+	def change_table_name_in_sqlite_db(self, table_name_old, table_name_new, db_name=""):
 		"""
-		database는 파일의 형태이므로 폴더에서 화일이름들을 확인한다
-		입력형태 :
-		출력형태 :
+		테이블 이름을 변경
 		"""
-		result = False
-		db_name_all = self.yt.read_filename_folder_all(path)
-		if db_name in db_name_all:
-			result = True
-		else:
-			print("db_name을 다시 확인하세요")
-			result = None
-		return result
+		self.check_cursor(db_name)
+		sql_sentence = "alter table %s rename to %s" % (table_name_old, table_name_new)
+		self.cursor.execute(sql_sentence)
 
-	def check_df_range(self, input_list):
+	def check_col_name(self, col_name):
 		"""
-		내가만든 입력형태를 사용할수있도록 만든것
-		입력형태 : ["3~4"], ["all"],[1,2,3,4], [3:4]
-		출력형태 : [3:4], [:], [1:4], [3:4]
+		컬럼의 이름으로 쓰이는 것에 이상한 글자들이 들어가지 않도록 확인하는 것이다
 		"""
-		result = self.yt.check_df_range(input_list)
-		return result
+		for data1, data2 in [["'", ""], ["/", ""], ["\\", ""], [".", ""],[" ", "_"] ]:
+			col_name = col_name.replace(data1, data2)
+		return col_name
 
-	def connect_db(self, db_name=""):
+	def check_col_name_all_in_sqlite_table(self, table_name, db_name =""):
 		"""
-		입력형태 :
-		출력형태 :
+		현재 있는 테이블의 이름에 특수문자들을 지우는 것이다
+		공백을 _로 변경하는것, Column의 이름을 변경한다
 		"""
-		#기본적으로 test_db.db를 만든다
-		#memory로 쓰면, sqlite3를 메모리에 넣도록 한다
-		if db_name == "memory":
-			self.connect_db_in_memory(db_name)
-		#데이터베이스를 넣으면 화일로 만든다
-		elif self.db_name == "" or self.db_name == "test":
-			self.db_name = "test_db.db"
-			self.con = sqlite3.connect(self.db_name, isolation_level=None)
+		self.check_cursor(db_name)
+		all_col_names = self.read_col_name_all_in_sqlite_table(db_name, table_name)
+		for col_name in all_col_names:
+			col_name_new = self.check_col_name(col_name)
+			if not col_name_new == col_name:
+				self.cursor.execute("alter table {} RENAME COLUMN {} to {}".format(table_name, col_name, col_name_new))
+
+	def check_cursor(self, db_name=""):
+		if db_name =="":
+			pass
 		else:
-			self.con = sqlite3.connect(self.db_name, isolation_level=None)
-		self.curs = self.con.cursor()
+			self.con = sqlite3.connect(db_name, isolation_level=None)
+			self.cursor = self.con.cursor()
 
-	def connect_db_in_memory(self, table_name=""):
+	def check_db_name_in_folder(self, db_name="", path="."):
 		"""
-		#self.curs.execute("CREATE TABLE " + self.table_name + " (auto_no integer primary key AUTOINCREMENT)")
-		입력형태 :
-		출력형태 :
+		경로안에 sqlite의 database가 있는지 확인하는 것이다
+		database는 파일의 형태이므로 폴더에서 화일이름들을 확인한다
 		"""
-		self.db_name = "memory_db"
-		self.con = sqlite3.connect(":memory:")
-		self.con = sqlite3.connect(self.db_name, isolation_level=None)
-		print("DB이름은 ==> ", self.db_name)
+		db_name_all = self.yt.read_all_filename_in_folder(path)
+		if db_name in db_name_all:
+			result = db_name
+		else:
+			result = ""
+		return result
 
-	def connect_db_with_table_name(self, db_name="", table_name=""):
+	def check_df_range(self, input_df):
 		"""
-		입력형태 :
-		출력형태 :
+		개인적으로 만든 이용형태를 것으로,
+		check로 시작하는 메소드는 자료형태의 변경이나 맞는지를 확인하는 것이다
+		dataframe의 영역을 나타내는 방법을 dataframe에 맞도록 변경하는 것이다
+		x=["1:2", "1~2"] ===> 1, 2열
+		x=["1,2,3,4"] ===> 1,2,3,4열
+		x=[1,2,3,4]  ===> 1,2,3,4열
+		x=""또는 "all" ===> 전부
 		"""
-		self.connect_db(db_name)
-		self.make_table(table_name)
+		temp = []
+		for one in input_df:
+			if ":" in one:
+				pass
+			elif "~" in one:
+				one = one.replace("〜", ":")
+			elif "all" in one:
+				one = one.replace("all", ":")
+			else:
+				changed_one = one.split(",")
+				temp_1 = []
+				for item in changed_one:
+					temp_1.append(int(item))
+				one = temp_1
+			temp.append(one)
+		return temp
 
-	def delete_columns(self, table_name, col_name_list):
+	def delete_column_in_sqlite_table(self, table_name, col_name_list, db_name=""):
 		"""
-		컬럼을 삭제한다
+		컬럼 삭제
 		입력형태 : ["col_1","col_2","col_3"]
 		"""
+		self.check_cursor(db_name)
 		if col_name_list:
 			for col_name in col_name_list:
 				sql = ("ALTER TABLE %s DROP COLUMN %s " % (table_name, col_name))
-				self.curs.execute(sql)
+				self.cursor.execute(sql)
 
-	def delete_df_emptycolumn(self, input_df):
+	def delete_empty_column_in_df(self, input_df):
 		"""
 		dataframe의 빈열을 삭제
 		제목이 있는 경우에만 해야 문제가 없을것이다
 		"""
 		nan_value = float("NaN")
 		input_df.replace(0, nan_value, inplace=True)
 		input_df.replace("", nan_value, inplace=True)
 		input_df.dropna(how="all", axis=1, inplace=True)
 		return input_df
 
-	def delete_empty_column(self, table_name):
+	def delete_empty_column_in_sqlite_table(self, table_name, db_name=""):
 		"""
 		테이블의 컬럼중에서 아무런 값도 없는 컬럼을 삭제한다
-		입력형태 :
-		출력형태 :
 		"""
-		col_list = []
-		for column_data in self.read_col_name_all(table_name):
-			sql = ("select COUNT(*) from %s where %s is not null" % (table_name, column_data))
-			self.curs.execute(sql)
-			if self.curs.fetchall()[0][0] == 0:
-				col_list.append(column_data)
-		self.delete_columns()
+		self.check_cursor(db_name)
+		col_name_all = self.read_col_name_all_in_sqlite_table(db_name, table_name)
 
-	def delete_table(self, table_name):
+		for col_name in col_name_all:
+			sql = ("select COUNT(*) from %s where %s is not null" % (table_name, col_name))
+			self.cursor.execute(sql)
+			if self.cursor.fetchall()[0][0] == 0:
+				#입력값이 없으면 0개이고, 그러면 삭제를 하는 것이다
+				sql = ("ALTER TABLE %s DROP COLUMN %s " % (table_name, col_name))
+				self.cursor.execute(sql)
+
+	def delete_sqlite_table(self, table_name, db_name=""):
 		"""
 		입력형태 : 테이블이름
 		"""
-		self.curs.execute("DROP TABLE " + table_name)
+		self.check_cursor(db_name)
+		self.cursor.execute("DROP TABLE " + table_name)
 
-	def insert_cols(self, table_name, col_data_list):
+	def insert_cols_in_sqlite_table(self, table_name, col_data_list_s, db_name=""):
 		"""
 		새로운 컬럼을 만든다
-		입력형태 : 테이블이름, [["이름1","int"],["이름2","text"]]
-		출력형태 :
+		col_data_list_s : [["이름1","int"],["이름2","text"]]
+		["이름2",""] => ["이름2","text"]
+		"""
+		self.check_cursor(db_name)
+		for one_list in col_data_list_s:
+			if type(one_list) == type([]):
+				col_name = self.check_col_name(one_list[0])
+				col_type = one_list[1]
+			else:
+				col_name = self.check_col_name(one_list)
+				col_type = "text"
+			self.cursor.execute("alter table %s add column '%s' '%s'" % (table_name, col_name, col_type))
+
+	def make_connection_with_sqlite_db(self, db_name=""):
+		"""
+		기본적으로 test_db.db를 만든다
+		memory로 쓰면, sqlite3를 메모리에 넣도록 한다
 		"""
-		for col_name, col_type in col_data_list:
-			col_name = self.check_col_name(col_name)
-			self.curs.execute("alter table %s add column '%s' '%s'" % (table_name, col_name, col_type))
+		if db_name == "memory":
+			self.con = sqlite3.connect(":memory:")
+		elif db_name == "" or db_name == "test": # 데이터베이스를 넣으면 화일로 만든다
+			db_name = "test_db.db"
+			self.con = sqlite3.connect(db_name, isolation_level=None)
+		else:
+			self.con = sqlite3.connect(db_name, isolation_level=None)
+		self.cursor = self.con.cursor()
 
-	def make_database(self, db_name):
+	def make_cursor_for_sqlite_db(self, db_name=""):
 		"""
-		새로운 데이터베이스를 만든다
-		입력형태 : 이름
+		기본적으로 test_db.db를 만든다
+		memory로 쓰면, sqlite3를 메모리에 넣도록 한다
 		"""
+
 		self.db_name = db_name
-		new_sql = "CREATE DATABASE %s;" % (self.db_name)
-		print(new_sql)
 
-	def make_table(self, table_name):
+		if self.db_name == "memory":
+			self.make_memory_db_for_sqlite()
+		# 데이터베이스를 넣으면 화일로 만든다
+		elif self.db_name == "" or self.db_name == "test":
+			self.db_name = "test_db.db"
+			self.con = sqlite3.connect(self.db_name, isolation_level=None)
+		else:
+			self.con = sqlite3.connect(self.db_name, isolation_level=None)
+		self.cursor = self.con.cursor()
+
+	def make_insert_sql_by_col_names(self, table_name, col_list):
+		sql_columns = self.yt.change_list1d_to_text_with_chainword(col_list, ", ")
+		sql_values = "?," * len(col_list)
+		result = "insert into %s (%s) values (%s)" % (table_name, sql_columns, sql_values[:-1])
+		return result
+
+	def make_memory_db_for_sqlite(self):
+		self.con = sqlite3.connect(":memory:")
+
+	def make_new_sqlite_db(self, db_name=""):
 		"""
-		새로운 테이블을 만든다
-		입력형태 : 테이블이름
+		새로운 데이터베이스를 만든다
+		입력형태 : 이름
 		"""
-		tables = []
-		self.curs.execute("select name from sqlite_master where type = 'table'; ")
-		for one_table_name in self.curs.fetchall():
-			tables.append(one_table_name[0])
-		if not table_name in tables:
-			self.curs.execute("CREATE TABLE " + table_name + " (Item text)")
+		self.make_connection_with_sqlite_db(db_name)
 
-	def make_table_with_column(self, table_name, column_data_list):
+	def make_new_sqlite_table_with_column(self, table_name, column_data_list, db_name=""):
 		"""
 		어떤 형태의 자료가 입력이 되어도 테이블을 만드는 sql을 만드는 것이다
 		입력형태 1 : 테이블이름, [['번호1',"text"], ['번호2',"text"],['번호3',"text"],['번호4',"text"]]
 		입력형태 2 : 테이블이름, ['번호1','번호2','번호3','번호4']
 		입력형태 3 : 테이블이름, [['번호1',"text"], '번호2','번호3','번호4']
-		입력형태 :
-		출력형태 :
 		"""
-
+		self.check_cursor(db_name)
 		sql_1 = "CREATE TABLE IF NOT EXISTS {}".format(table_name)
 		sql_2 = sql_1 + " ("
 		for one_list in column_data_list:
 			if type(one_list) == type([]):
-				if len(one_list)== 2:
+				if len(one_list) == 2:
 					col_name = one_list[0]
 					col_type = one_list[1]
 				elif len(one_list) == 1:
 					col_name = one_list[0]
 					col_type = "text"
 			elif type(one_list) == type("string"):
 				col_name = one_list
 				col_type = "text"
 			sql_2 = sql_2 + "{} {}, ".format(col_name, col_type)
 		sql_2 = sql_2[:-2] + ")"
-		self.curs.execute(sql_2)
+		self.cursor.execute(sql_2)
 		return sql_2
 
-	def pick_unique__table_col_names__new_col_names(self, table_name, col_names):
+	def make_new_table_in_sqlite_db(self, table_name, db_name=""):
 		"""
-		기존 테이블의 컬럼중에서 새로운 컬럼이름이 고유한것만 추출
-		입력형태 :
-		출력형태 :
+		새로운 테이블을 만든다
+		입력형태 : 테이블이름
+		"""
+		self.check_cursor(db_name)
+		#현재 db안의 테이블에 같은 이름이 없는지 확인 하는 것
+		tables = []
+		self.cursor.execute("select name from sqlite_master where type = 'table'; ")
+		all_table_name = self.cursor.fetchall()
+		if not table_name in all_table_name:
+			self.cursor.execute("CREATE TABLE " + table_name + " (Item text)")
+
+	def make_sqlite_db_in_memory(self):
+		"""
+		self.cursor.execute("CREATE TABLE " + self.table_name + " (auto_no integer primary key AUTOINCREMENT)")
+		memory에 생성하는 것은 바로 connection 이 만들어 진다
+		"""
+		self.con = sqlite3.connect(":memory:")
+
+	def manual(self):
+		result = """
+		databse가 있는 화일의 위치를 알려주면 시작이 된다
+		pandas의 장점
+		1. 대용량 데이터(GB 단위 이상)를 다룰 수 있습니다. 엑셀은 데이터 용량이 100MB을 넘어가거나, 데이터가 100만 행이 넘어가면 정상적으로 작동하지 않는 현상을 겪기도 합니다.
+		2. 복잡한 처리 작업들을 비교적 손쉽게 할 수 있습니다. 소위 말하는 엑셀 노가다를 할 필요가 없습니다.
+		3. 손쉽게 데이터를 결합하고 분리할 수 있습니다. SQL처럼 데이터를 합치고 관계 연산을 수행할 수 있습니다.
+
+		df.index, df.columns, df.values
+		df["col1"], df[1:3]
+
+		index는 숫자만 가능하지 않고, String(문자열) 일 수도 있다.
+		index가 숫자여도 순서대로 정렬될 필요가 없다. 그리고 index는 중복될 수 있다.
+		print(df.loc[:3, ['Surv', 'N']])
+
+		df[val]	Select single column or sequence of columns from the DataFrame
+		df.loc[val]	Selects single row or subset of rows from the DataFrame by label
+		df.loc[:, val]	Selects single column or subset of columns by label
+		df.loc[val1, val2]	Select both rows and columns by label
+		df.iloc[where]	Selects single row or subset of rows from the DataFrame by integer position
+		df.iloc[:, where]	Selects single column or subset of columns by integer position
+		df.iloc[where_i, whe	re_j] Select both rows and columns by integer position
+		df.at[label_i, label	_j] Select a single scalar value by row and column label
+		df.iat[i, j]	Select a single scalar value by row and column position (integers)
+		get_value(), set_val	ue() Select single value by row and column label
 		"""
-		result = []
-		columns = self.read_col_name_all(table_name)
-		update_col_names = self.yt.change_waste_data(col_names)
-		for one_col_name in update_col_names:
-			if not one_col_name.lower() in columns:
-				result.append(one_col_name)
 		return result
 
-	def read_col_name_all(self, table_name=""):
+	def read_col_name_all_in_sqlite_table(self, table_name, db_name=""):
 		"""
 		해당하는 테이의 컬럼구조를 갖고온다
 		입력형태 : 테이블이름
 		출력형태 : 컬럼이름들
 		"""
-		if table_name =="":
-			table_name = self.table_name
-		self.curs.execute("PRAGMA table_info('%s')" % table_name)
+		self.check_cursor(db_name)
+		self.cursor.execute("PRAGMA table_info('%s')" % table_name)
+		sql_result =self.cursor.fetchall()
 		result = []
-		for temp_2 in self.curs.fetchall():
-			result.append(temp_2[1].lower())
+		for one_list in sql_result:
+			result.append(one_list[1])
 		return result
 
-	def read_colproperty_all_for_table(self, table_name):
+	def read_col_property_all_in_sqlite_table(self, table_name, db_name=""):
 		"""
 		해당하는 테이블의 컬럼의 모든 구조를 갖고온다
-		입력형태 :
-		출력형태 :
 		"""
 
-		self.curs.execute("PRAGMA table_info('%s')" % table_name)
+		self.check_cursor(db_name)
+		self.cursor.execute("PRAGMA table_info('%s')" % table_name)
 		result = []
-		for temp_2 in self.curs.fetchall():
+		for temp_2 in self.cursor.fetchall():
 			result.append(temp_2)
 		return result
 
-	def read_db_name_all(self, path=".\\"):
+	def read_columns_data_from_no1_to_no2_in_sqlite_table(self, table_name, offset=0, row_count=100, db_name=""):
+		"""
+		테이블의 자료중 원하는 갯수만 읽어오는 것
+		"""
+		self.check_cursor(db_name)
+		self.cursor.execute(("select * from %s LIMIT %s, %s;") % (table_name, str(offset), str(row_count)))
+		result = self.cursor.fetchall()
+		return result
+
+	def read_db_name_all_in_path(self, path=".\\"):
 		"""
 		모든 database의 이름을 갖고온다
 		모든이 붙은것은 맨뒤에 all을 붙인다
-		입력형태 :
-		출력형태 :
 		"""
 		result = []
 		for fname in os.listdir(path):
-			if fname[-3:] ==".db":
+			if fname[-3:] == ".db":
 				result.append(fname)
 		return result
 
-	def read_table_data(self, table_name=""):
+	def read_df_by_name(self, df_obj, x, y):
 		"""
-		테이블의 모든 자료를 읽어온다
-		입력형태 : 테이블 이름
-		출력형태 :
+		열이나 행의 이름으로 pandas의 dataframe의 일부를 불러오는 것이다
+		이것은 리스트를 기본으로 사용한다
+		list_x=["가"~"다"] ===> "가"~"다"열
+		list_x=["가","나","다","4"] ===> 가,나,다, 4 열
+		x=""또는 "all" ===> 전부
+		"""
+
+		temp = []
+		for one in [x, y]:
+			if ":" in one[0]:
+				changed_one = one[0]
+			elif "~" in one[0]:
+				ed_one = one[0].split("~")
+				changed_one = "'" + str(ed_one[0]) + "'" + ":" + "'" + str(ed_one[1]) + "'"
+
+			elif "all" in one[0]:
+				changed_one = one[0].replace("all", ":")
+			else:
+				changed_one = one
+			temp.append(changed_one)
+		# 이것중에 self를 사용하지 않으면 오류가 발생한다
+		print(temp)
+		exec("self.result = df_obj.loc[{}, {}]".format(temp[0], temp[1]))
+		return self.result
+
+	def read_df_by_no(self, df_obj, x, y):
+		"""
+		숫자번호로 pandas의 dataframe의 일부를 불러오는 것
+		단, 모든것을 문자로 넣어주어야 한다
+		x=["1:2", "1~2"] ===> 1, 2열
+		x=["1,2,3,4"] ===> 1,2,3,4열
+		x=[1,2,3,4]  ===> 1,2,3,4열
+		x=""또는 "all" ===> 전부
+		"""
+
+		x_list = self.check_df_range(x)
+		y_list = self.check_df_range(y)
+		exec("self.result = df_obj.iloc[{}, {}]".format(x_list, y_list))
+		return self.result
+
+	def read_df_by_xy(self, df_obj, xy=[0, 0]):
+		"""
+		위치를 기준으로 값을 읽어오는 것이다
+		숫자를 넣으면 된다
 		"""
-		self.curs.execute(("select * from {}").format(table_name))
-		result = self.curs.fetchall()
+		result = df_obj.iat[int(xy[0]), int(xy[1])]
 		return result
 
-	def read_table_data_by_col_names(self, col_name_s="", condition="all"):
+	def read_table_data_by_col_names_at_sqlite(self, col_name_s="", condition="all", db_name=""):
 		"""
 		문자는 컬럼이름으로, 숫자는 몇번째인것으로...
-		입력형태 :
-		출력형태 :
 		"""
+		self.check_cursor(db_name)
 		if col_name_s == "":
 			sql_columns = "*"
 		else:
-			sql_columns = self.yt.chain_list1d_text_word(col_name_s, ", ")
+			sql_columns = self.yt.change_list1d_to_text_with_chainword(col_name_s, ", ")
 
-		if condition=="all":
+		if condition == "all":
 			lim_no = 100
 		else:
 			lim_no = condition
 		limit_text = "limit {}".format(lim_no)
 		sql = "SELECT {} FROM {} ORDER BY auto_no {}".format(sql_columns, self.table_name, limit_text)
-		self.curs.execute(sql)
-		result = self.curs.fetchall()
+		self.cursor.execute(sql)
+		result = self.cursor.fetchall()
 		return result
 
-	def read_table_data_from_no1_to_no2(self, table_name, offset=0, row_count=100):
+	def read_table_data_for_sqlite_table(self, table_name, db_name=""):
 		"""
-		테이블의 자료중 원하는 갯수만 읽어오는 것
-		입력형태 :
-		출력형태 :
+		테이블의 모든 자료를 읽어온다
+		입력형태 : 테이블 이름
 		"""
-		self.curs.execute(("select * from %s LIMIT %s, %s;") % (table_name, str(offset), str(row_count)))
-		result = self.curs.fetchall()
+		self.check_cursor(db_name)
+		self.cursor.execute(("select * from {}").format(table_name))
+		result = self.cursor.fetchall()
 		return result
 
-	def read_table_names(self):
+	def read_table_name_all_at_sqlite_db(self, db_name=""):
 		"""
 		해당하는 테이의 컬럼구조를 갖고온다
 		입력형태 : 데이터베이스 이름
 		출력형태 : 테이블이름들
 		"""
-		self.curs.execute("SELECT name FROM sqlite_master WHERE type='table' ORDER BY name;")
+		self.check_cursor(db_name)
+		self.cursor.execute("SELECT name FROM sqlite_master WHERE type='table' ORDER BY name;")
 		result = []
-		for temp_2 in self.curs.fetchall():
+		for temp_2 in self.cursor.fetchall():
 			result.append(temp_2[0])
 		return result
 
-	def run_sql(self, sql):
+	def run_sql_for_sqlite(self, sql, db_name=""):
 		"""
-		입력형태 :
-		출력형태 :
-		"""
-		self.curs.execute(sql)
-		result = self.curs.fetchall()
+		sqlite의 sql문을 실행하는 것이다
+		fetchall는
+		첫번째 : (1, '이름1', 1, '값1')
+		두번째 : (2, '이름2', 2, '값2')
+		"""
+		self.check_cursor(db_name)
+		self.cursor.execute(sql)
+		result = self.cursor.fetchall()
 		self.con.commit()
 		return result
 
-	def save_memorydb_to_diskdb(self, db_name):
+	def save_sqlite_memorydb_to_diskdb(self, db_name=""):
 		"""
 		memory에 저장된것을 화일로 저장하는것
 		python 3.7부터는 backup이 가능
-		입력형태 :
-		출력형태 :
 		"""
 		db_disk = sqlite3.connect(db_name)
 		self.con.backup(db_disk)
 
+	def set_database(self, db_name):
+		self.check_cursor(db_name)
+
 	def split_path_n_name(self, input_value=""):
 		"""
 		입력값을 경로와 이름으로 분리
 		"""
 		file_name = ""
 		path = ""
 		input_value = input_value.replace("/", "\\")
 		temp_1 = input_value.split("\\")
 		if "." in temp_1[-1]:
 			file_name = temp_1[-1]
-		if len(temp_1) >1 and "\\" in temp_1[:len(temp_1[-1])]:
+		if len(temp_1) > 1 and "\\" in temp_1[:len(temp_1[-1])]:
 			path = input_value[:len(temp_1[-1])]
 		result = [file_name, path]
 		return result
 
-	def write_data_to_sqlite_table(self, table_name, col_name_s, col_value_s):
+	def terms(self):
+		"""
+		이 클래스에서 중요하게 사용되는 용어들에 대한 설명입니다
+		"""
+		result = """
+		df : dataframe
+		con : Connection, 외부환경과 Database를 연결하는 것. 즉 db가 위치한 곳들을 연결하는 것이지요
+		cursor : DB에 어떤 일을 시키면, Db에서 Item이라는 객체가 만들어진다. 그 만들어진곳을 가리키는 객체
+		"""
+		return result
+
+	def write_data_in_sqlite_table(self, table_name, col_name_s, col_value_s, db_name=""):
 		"""
-		입력형태 :
-		출력형태 :
 		"""
+		self.check_cursor(db_name)
 		sql_columns = ""
 		sql_values = ""
 		for column_data in col_name_s:
 			sql_columns = sql_columns + column_data + ", "
 			sql_values = "?," * len(col_name_s)
 		sql = "insert into %s(%s) values (%s)" % (table_name, sql_columns[:-2], sql_values[:-1])
 		if type(col_value_s[0]) == type([]):
-			self.curs.executemany(sql, col_value_s)
+			self.cursor.executemany(sql, col_value_s)
 		else:
-			self.curs.execute(sql, col_value_s)
+			self.cursor.execute(sql, col_value_s)
 		self.con.commit()
 
-	def write_df_to_excel(self, input_df, xy = [1,1]):
+	def write_df_to_excel(self, input_df, xy=[1, 1]):
 		"""
 		df자료를 커럼과 값을 기준으로 나누어서 결과를 돌려주는 것이다
-		입력형태 :
-		출력형태 :
 		"""
 		col_list = input_df.columns.values.tolist()
 		value_list = input_df.values.tolist()
-		excel=pcell.pcell()
-		excel.write_value("", xy, [col_list])
-		excel.dump_value("", [xy[0]+1, xy[1]], value_list)
+		excel = pcell.pcell()
+		excel.write_list1d_in_yline("", xy, col_list)
+		excel.write_value_in_range_as_speedy("", [xy[0] + 1, xy[1]], value_list)
 
-	def write_df_to_sqlite(self, table_name, df_data):
+	def write_df_to_sqlite_table(self, table_name, df_data, db_name=""):
 		"""
 		df자료를 sqlite에 새로운 테이블로 만들어서 넣는 것
-		입력형태 :
-		출력형태 :
 		"""
+		self.check_cursor(db_name)
 		df_data.to_sql(table_name, self.con)
 
-	def write_dic_to_table(self, dic_data):
+	def write_dic_in_sqlite_table(self, table_name, dic_data, db_name=""):
 		"""
 		사전의 키를 y이름으로 해서 값을 입력한다
-		입력형태 :
-		출력형태 :
 		"""
+		self.check_cursor(db_name)
+
 		for one_col in list(dic_data[0].keys()):
-			if not one_col in self.read_col_name_all():
-				self.new_y(one_col)
-		sql_columns = self.yt.chain_list1d_text_word(list(dic_data[0].keys()), ", ")
-		sql_values = "?," * len(list(dic_data[0].keys()))
-		sql = "insert into %s (%s) values (%s)" % (self.table_name, sql_columns, sql_values[:-1])
+			if not one_col in self.read_col_name_all_in_sqlite_table(table_name):
+				self.insert_cols_in_sqlite_table(table_name, [one_col])
+
+		sql = self.make_insert_sql_by_col_names(table_name, list(dic_data[0].keys()))
 		value_list = []
 		for one_dic in dic_data:
 			value_list.append(list(one_dic.values()))
-		self.curs.executemany(sql, value_list)
+		self.cursor.executemany(sql, value_list)
 
-	def write_list_to_table(self, table_name,col_name_s, list_values):
+	def write_list_to_sqlite_table(self, table_name, col_name_s, list_values, db_name=""):
 		"""
 		리스트의 형태로 넘어오는것중에 y이름과 값을 분리해서 얻는 것이다
-		입력형태 :
-		출력형태 :
 		"""
-		sql_columns = self.yt.chain_list1d_text_word(col_name_s, ", ")
-		sql_values = "?," * len(list_values[0])
-		sql = "insert into %s (%s) values (%s)" % (table_name, sql_columns, sql_values[:-1])
-		self.curs.executemany(sql, list_values)
+		self.check_cursor(db_name)
+		sql = self.make_insert_sql_by_col_names(table_name, col_name_s)
+		self.cursor.executemany(sql, list_values)
 
-	def write_table_data_to_df(self, table_name):
+	def write_sqlite_table_data_all_to_df(self, table_name, db_name=""):
 		"""
 		sqlite를 df로 만드는것
-		입력형태 :
-		출력형태 :
 		"""
-
+		self.check_cursor(db_name)
 		sql = "SELECT * From %s" % (table_name)
-		query = self.cur.execute(sql)
+		query = self.cursor.execute(sql)
 		cols = [column[0] for column in query.description]
 		input_df = pd.DataFrame.from_records(data=query.fetchall(), columns=cols)
 		return input_df
 
-	def append_df1_df2(self, df_obj_1, df_obj_2):
-		"""
-		dataframe의 끝에 dataframe로 만든 것을 맨끝에 추가하는것
-		"""
-		df_obj_1 = pd.concat([df_obj_1, df_obj_2])
-		return df_obj_1
-
-	def insert_df1_df2(self, df_obj_1, df_obj_2):
-		"""
-		df_obj_1의 자료에 df_obj_2를 맨끝에 추가하는것
-		"""
-		df_obj_1 = pd.concat([df_obj_1, df_obj_2])
-		return df_obj_1
-
-	def read_df_by_no(self, df_obj, x, y):
+	def write_value_in_df_by_xy(self, df, xy, value):
 		"""
-		숫자번호로 pandas의 dataframe의 일부를 불러오는 것
-		단, 모든것을 문자로 넣어주어야 한다
-		x=["1:2", "1~2"] ===> 1, 2열
-		x=["1,2,3,4"] ===> 1,2,3,4열
-		x=[1,2,3,4]  ===> 1,2,3,4열
-		x=""또는 "all" ===> 전부
+		dataframe에 좌표로 값을 저장
 		"""
+		x_max = df.index.size
+		y_max = df.columns.size
+		if xy[1] > y_max:
+			for no in range(y_max, xy[1]):
+				df[len(df.columns)] = np.NaN
+		if xy[0] > x_max:
+			data_set = [(lambda x: np.NaN)(a) for a in range(len(df.columns))]
+			for no in range(xy[0] - x_max):
+				df.loc[len(df.index)] = data_set
+		df.iat[int(xy[0]), int(xy[1])] = value
 
-		x_list = self.check_df_range(x)
-		y_list = self.check_df_range(y)
-		exec("self.result = df_obj.iloc[{}, {}]".format(x_list, y_list))
-		return self.result
-
-	def read_df_by_xy(self, df_obj, xy=[0, 0]):
+	def read_pickle_file(self, path_n_name=""):
 		"""
-		위치를 기준으로 값을 읽어오는 것이다
-		숫자를 넣으면 된다
+		pickle로 자료를 만든것을 읽어오는 것이다
 		"""
-		result = df_obj.iat[int(xy[0]), int(xy[1])]
+		with open(path_n_name, "rb") as fr:
+			result = pickle.load(fr)
 		return result
 
-	def read_df_by_name(self, df_obj, x, y):
+	def save_input_data_to_pickle_file(self, source_data = "", file_name = "", path = "D:\\"):
 		"""
-		열이나 행의 이름으로 pandas의 dataframe의 일부를 불러오는 것이다
-		이것은 리스트를 기본으로 사용한다
-		list_x=["가"~"다"] ===> "가"~"다"열
-		list_x=["가","나","다","4"] ===> 가,나,다, 4 열
-		x=""또는 "all" ===> 전부
+		자료를 pickle 로 저장하는것
 		"""
-
-		temp = []
-		for one in [x, y]:
-			if ":" in one[0]:
-				changed_one = one[0]
-			elif "~" in one[0]:
-				ed_one = one[0].split("~")
-				changed_one = "'" + str(ed_one[0]) + "'" + ":" + "'" + str(ed_one[1]) + "'"
-
-			elif "all" in one[0]:
-				changed_one = one[0].replace("all", ":")
-			else:
-				changed_one = one
-			temp.append(changed_one)
-		# 이것중에 self를 사용하지 않으면 오류가 발생한다
-		print(temp)
-		exec("self.result = df_obj.loc[{}, {}]".format(temp[0], temp[1]))
-		return self.result
-
-
-	class sqlite:
-
-		class db:
-			def __init__(self, db_name=""):
-				vars["db_name"] = db_name
-
-			def change_col_name(self, table_name):
-				"""
-				공백을 _로 변경하는것, Column의 이름을 변경한다
-				입력형태 :
-				출력형태 :
-				"""
-				for column_data in self.read_col_name_all(table_name):
-					column_data_new = column_data.replace(" ", "_")
-					if not column_data_new == column_data:
-						tem_2 = self.curs.execute(
-							"alter table {} RENAME COLUMN {} to {}".format(table_name, column_data, column_data_new))
-
-			def connect(self, db_name=""):
-				vars["con"] = sqlite3.connect(db_name, isolation_level=None)
-				vars["curs"] = vars["con"].cursor()
-
-			def create(self, db_name=""):
-				# 기본적으로 test_db.db를 만든다
-				# memory로 쓰면, sqlite3를 메모리에 넣도록 한다
-
-				vars["db_name"] = db_name
-
-				if vars["db_name"] == "memory":
-					self.connect_db_in_memory(db_name)
-				# 데이터베이스를 넣으면 화일로 만든다
-				elif vars["db_name"] == "" or vars["db_name"] == "test":
-					vars["db_name"] = "test_db.db"
-					vars["con"] = sqlite3.connect(vars["db_name"], isolation_level=None)
-				else:
-					vars["con"] = sqlite3.connect(vars["db_name"], isolation_level=None)
-				vars["curs"] = vars["con"].cursor()
-
-			def connect_db_in_memory(self, table_name=""):
-				vars["db_name"] = "memory_db"
-				vars["con"] = sqlite3.connect(":memory:")
-				vars["con"] = sqlite3.connect(vars["db_name"], isolation_level=None)
-
-			class table:
-				def __init__(self, table_name=""):
-					vars["table_name"] = table_name
-
-				def create_table(self, table_name):
-					tables = []
-					self.curs.execute("select name from sqlite_master where type = 'table'; ")
-					for one_table_name in self.curs.fetchall():
-						tables.append(one_table_name[0])
-					if not table_name in tables:
-						self.curs.execute("CREATE TABLE " + table_name + " (Item text)")
-
-				def insert_cols(self, table_name, col_data_list):
-					"""
-					새로운 컬럼을 만든다
-					입력형태 : 테이블이름, [["이름1","int"],["이름2","text"]]
-					출력형태 :
-					"""
-					for one_list in col_data_list:
-						if type(one_list) ==type([]):
-							col_name = self.check_col_name(one_list[0])
-							col_type = one_list[1]
-						else:
-							col_name = self.check_col_name(one_list)
-							col_type = "text"
-						vars["curs"].execute("alter table %s add column '%s' '%s'" % (table_name, col_name, col_type))
-
-				def check_col_name(self, col_name):
-					for data1, data2 in [["'", ""], ["/", ""], ["\\", ""], [".", ""]]:
-							col_name = col_name.replace(data1, data2)
-					return col_name
-
-				def write_data(self, table_name, col_name_s, col_value_s):
-					sql_columns = ""
-					sql_values = ""
-					for column_data in col_name_s:
-						sql_columns = sql_columns + column_data + ", "
-						sql_values = "?," * len(col_name_s)
-					sql = "insert into %s(%s) values (%s)" % (table_name, sql_columns[:-2], sql_values[:-1])
-					if type(col_value_s[0]) == type([]):
-						vars["curs"].executemany(sql, col_value_s)
-					else:
-						vars["curs"].execute(sql, col_value_s)
-					vars["con"].commit()
+		if not "." in file_name:
+			file_name = file_name +".pickle"
+		with open(path+file_name, "wb") as fr:
+			pickle.dump(source_data, fr)
```

### Comparing `halmoney-2.1.1/src/halmoney/jfinder.py` & `halmoney-3.0.0/src/halmoney/jfinder.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,75 +1,105 @@
 # -*- coding: utf-8 -*-
-import re
+
+import re #내장모듈
 
 class jfinder:
+    def manual(self):
+        result = """
+        1. sql을 제일 처음에, input_text를 제일 나중에
+        
+        """
+        return result
+
+    def history(self):
+        result = """
+    		"""
+        return result
+
+    def terms(self):
+        result = """
+        search : 찾기
+        replace : 바꾸기
+        change : 바꾸기
+        delete : 
+        get : 
+        is : True, False로 구분
+    		"""
+        return result
+
     def jfinder (self, input_text=""):
-        print(input_text)
-        result = input_text.replace(" ", "")
+        """
+        기본저긴 jfsql -> resql형식으로 만들어 주는것
+		"""
+
+        re_sql = input_text.replace(" ", "")
 
         setup_list = [
             ["(대소문자무시)", "(?!)"], #re.IGNORECASE 대소문자 무시
             ["(여러줄)", "(?m)"], # re.MULITILINE 여러줄도 실행
             ["(개행문자포함)", "(?s)"], # re.DOTALL 개행문자도 포함
             ]
 
         for one in setup_list:
-            result = result.replace(one[0], one[1])
+            re_sql = re_sql.replace(one[0], one[1])
 
         basic_list = [
-            [":(\d+)[~](\d*)[\]]",             "]{\\1,\\2}"], # :3~4] ==> ]{3,4}
-            ["[\[](\d+)[~](\d*)[\]]",          "{\\1,\\2}"], # [3~4] ==> {3,4}
+            ["[\[](\d+)[~](\d*)[\]]", "{\\1,\\2}"],  # [3~4] ==> {3,4}
+            [":(\d+)[~](\d*)[\]]", "]{\\1,\\2}"],  # :3~4] ==> ]{3,4}
 
             ["\(뒤에있음:(.*)\)",                "(?=\\1)" ], #(뒤에있음:(abc)) => (?=abc)
             ["\(뒤에없음:(.*)\)",                "(?!\\1)" ], #(뒤에없음:(abc)) => (?!abc)
             ["\((.*):뒤에있음\)",                "(?=\\1)" ], #(뒤에있음:(abc)) => (?=abc)
             ["\((.*):뒤에없음\)",                "(?!\\1)" ], #(뒤에없음:(abc)) => (?!abc)
             ["\(앞에있음:(.*)\)",                "(?<=\\1)"], #(앞에있음:(abc)) => (?<=abc)
             ["\(앞에없음:(.*)\)",                "(?<!\\1)"], #(앞에없음:(abc)) => (?<!abc)
 
-            ["([\[]?)한글모음[&]?([\]]?)",       "\\1ㅏ-ㅣ\\2"], #[ㅏ-ㅣ]
-            ["([\[]?)한글[&]?([\]]?)",          "\\1ㄱ-ㅎ|ㅏ-ㅣ|가-힣\\2"],
-            ["([\[]?)숫자[&]?([\]]?)",          "\\1 0-9 \\2"],
             ["([\[]?)영어대문자[&]?([\]]?)",     "\\1A-Z\\2"],
             ["([\[]?)영어소문자[&]?([\]]?)",     "\\1a-z\\2"],
-            ["([\[]?)영어[&]?([\]]?)",          "\\1a-zA-Z\\2"],
+            #["([\[]?)특수문자(.+?)([\]]?)",     "\\1 \\ \\2\\3"],
+            ["([\[]?)특수문자(.+?)([\]]?)",      "\\1\\2\\3"],
+            ["([\[]?)한글모음[&]?([\]]?)",       "\\1ㅏ-ㅣ\\2"], #[ㅏ-ㅣ]
+            ["([\[]?)모든문자[&]?([\]]?)",      "\\1.\n\\2"],
             ["([\[]?)일본어[&]?([\]]?)",        "\\1ぁ-ゔ|ァ-ヴー|々〆〤\\2"],
+            ["([\[]?)한글[&]?([\]]?)",          "\\1ㄱ-ㅎ|ㅏ-ㅣ|가-힣\\2"],
+            ["([\[]?)숫자[&]?([\]]?)",          "\\1\\\d\\2"],
+            ["([\[]?)영어[&]?([\]]?)",          "\\1a-zA-Z\\2"],
             ["([\[]?)한자[&]?([\]]?)",          "\\1一-龥\\2"],
-            ["([\[]?)특수문자[&]?([\]]?)",       "\\1 @#$&-_ \\2"],
-            ["([\[]?)모든문자[&]?([\]]?)",      "\\1.\n\\2"],
             ["([\[]?)문자[&]?([\]]?)",          "\\1.\\2"],
             ["([\[]?)공백[&]?([\]]?)",          "\\1\\\s\\2"],
 
             ["[\[]단어([(].*?[)])([\]]?)",      "\\1"],
             ["[\[]또는([(].*?[)])([\]]?)",      "\\1|"],
             ["[\(]이름<(.+?)>(.+?)[\)]",        "?P<\\1>\\2"], #[이름<abc>표현식]
-            ]
+
+        ]
+
 
         for one in basic_list:
-            result = re.sub(one[0], one[1], result)
-            result = result.replace(" ", "")
+            re_sql = re.sub(one[0], one[1], re_sql)
+            re_sql = re_sql.replace(" ", "")
 
         simple_list = [
             ['[처음]', '^'], ['[맨앞]', '^'], ['[시작]', '^'],
             ['[맨뒤]', '$'], ['[맨끝]', '$'], ['[끝]', '$'],
             ['[또는]', '|'], ['또는', '|'],['or', '|'],
             ['not', '^'],
             ]
 
         for one in simple_list:
-            result = result.replace(one[0], one[1])
+            re_sql = re_sql.replace(one[0], one[1])
 
         #최대탐색을 할것인지 최소탐색을 할것인지 설정하는 것이다
-        if "(최소찾기)" in result:
-            result = result.replace("[1,]","+")
-            result = result.replace("[1,]","*")
-
-            result = result.replace("+","+?")
-            result = result.replace("*","*?")
-            result = result.replace("(최소찾기)","")
+        if "(최소찾기)" in re_sql:
+            re_sql = re_sql.replace("[1,]","+")
+            re_sql = re_sql.replace("[1,]","*")
+
+            re_sql = re_sql.replace("+","+?")
+            re_sql = re_sql.replace("*","*?")
+            re_sql = re_sql.replace("(최소찾기)","")
 
 
         #이단계를 지워도 실행되는데는 문제 없으며, 실행 시키지 않았을때가 약간 더 읽기는 편하다
         high_list = [
             ['[^a-zA-Z0-9]', '\W'],
             ['[^0-9a-zA-Z]', '\W'],
             ['[a-zA-Z0-9]', '\w'],
@@ -77,53 +107,216 @@
             ['[^0-9]', '\D'],
             ['[0-9]', '\d'],
             ['{0,}', '*'],
             ['{1,}', '+'],
             ]
 
         for one in high_list:
-            result = result.replace(one[0], one[1])
-        return result
+            re_sql = re_sql.replace(one[0], one[1])
+
+        #print ("result ==> ", result)
+
+        if "[.]" in re_sql:
+            re_sql = re_sql.replace("[.]", ".")
+
+        return re_sql
 
     def change_jfsql_to_resql (self, jf_sql):
+        """
+        jfsql을 regex스타일로 바꾸는것
+        """
         result = self.jfinder(jf_sql)
         return result
 
-    def search (self, jf_sql, input_text):
-        re_sql = self.jfinder(jf_sql)
-        re_compiled = re.compile(re_sql)
-        result = re_compiled.findall(input_text)
+    def delete_except_num_eng(self, input_text):
+        """
+        영문과 숫자와 공백을 제외하고 다 제거를 하는것
+        """
+        result = []
+        for one_data in input_text:
+            temp = ""
+            for one in one_data:
+                if str(one) in ' 0123456789abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ_':
+                    temp = temp + str(one)
+            result.append(temp)
         return result
 
-    def search_by_resql (self, re_sql, input_text):
-        re_compiled = re.compile(re_sql)
-        result = re_compiled.findall(input_text)
+    def delete_eng_num(self, input_text):
+        """
+        알파벳과 숫자만 있는것을 확인하는것
+		"""
+        re_com = re.compile("[A-Za-z0-9]*")
+        if (re_com.search(input_text) == None):
+            new_text = input_text
+        else:
+            new_text = re_com.sub("", input_text)
+        return new_text
+
+    def delete_koren_gnum(self, input_text):
+        """
+        한글, 영어, 숫자만 남기고 나머지는 모두 지우는 것이다
+		"""
+        re_com = re.compile("[A-Za-z0-9ㄱ-ㅎㅏ-ㅣ가-힣]*")
+        if (re_com.search(input_text) == None):
+            new_text = input_text
+        else:
+            new_text = re_com.sub("", input_text)
+        return new_text
+
+    def delete_num_comma(self, input_text):
+        """
+        숫자중에서 ,로 분비리된것중에서 ,만 없애는것
+        1,234,567 => 1234567
+		"""
+        re_com = re.compile("[0-9,]*\.?[0-9]*")
+        new_text = re_com.sub("", input_text)
+        return new_text
+
+    def delete_specialchar(self, input_text):
+        """
+        공백과 특수문자등을 제외하고 같으면 새로운 y열에 1을 넣는 함수
+        리스트의 사이즈를 조정한다
+		"""
+        re_com = re.compile("[\s!@#$%^*()\-_=+\\\|\[\]{};:'\",.<>\/?]*")
+        if (re_com.search(input_text) == None):
+            new_text = input_text
+        else:
+            new_text = re_com.sub("", input_text)
+        return new_text
+
+    def delete_except_specialchar(self, input_text):
+        """
+		공백과 특수문자등을 제외하고 같으면 새로운 y열에 1을 넣는 함수
+		리스트의 사이즈를 조정한다
+		"""
+        re_com = re.compile("[^\s!@#$%^*()\-_=+\\\|\[\]{};:'\",.<>\/?]*")
+        if (re_com.search(input_text) == None):
+            new_text = input_text
+        else:
+            new_text = re_com.sub("", input_text)
+        return new_text
+
+    def delete_text_specialletter(self, input_list):
+        """
+        입력받은 텍스트로된 리스트의 자료를 전부 특수문자를 없앤후 돌려주는 것이다
+        입력된 자료가 1차원 리스트인지 판단한다
+		"""
+        result = []
+        if type(input_list) == type([]) and type(input_list[0]) != type([]):
+            for one in input_list:
+                if one != "" or one != None:
+                    temp = self.delete_except_specialchar(one)
+                    result.append(temp)
         return result
 
-    def replace (self, jf_sql, input_text, replace_word):
+
+    def delete_by_jfsql (self, jf_sql, input_text):
+        """
+		입력자료에서 삭제
+		"""
         re_sql = self.jfinder(jf_sql)
-        result = re.sub(re_sql, replace_word, input_text)
+        result = self.delete_by_resql (re_sql, input_text)
         return result
 
-    def delete (self, jf_sql, input_text, replace_word=""):
-        re_sql = self.jfinder(jf_sql)
+    def delete_by_resql (self, re_sql, input_text):
+        """
+		입력자료에서 삭제
+		"""
         result = re.sub(re_sql, "", input_text)
         return result
 
-    def delete_by_resql (self, re_sql, input_text, replace_word=""):
-        result = re.sub(re_sql, "", input_text)
+    def is_number_only(self, input_text):
+        """
+        소슷점까지는 포함한것이다
+		"""
+        result = False
+        temp = re.match("^[0-9.]+$", input_text)
+        if temp : result = True
+
+        return result
+
+    def is_korean_only(self, input_text):
+        """
+		모두 한글인지
+		"""
+        re_basic = "^[ㄱ-ㅎ|ㅏ-ㅣ|가-힣]+$"
+        result = False
+        temp = re.match(re_basic, input_text)
+        if temp : result = True
+        return result
+
+    def is_special_char(self, input_text):
+        """
+		특수문자가들어가있는지
+		"""
+        re_basic = "^[a-zA-Z0-9]+$"
+        result = False
+        temp = re.match(re_basic, input_text)
+        if temp : result = True
+        return result
+
+    def is_handphone_only(self, input_text):
+        """
+		특수문자가들어가있는지
+    	"""
+        re_basic = "^(010|019|011)-\d{4}-\d{4}+$"
+        result = False
+        temp = re.match(re_basic, input_text)
+        if temp : result = True
+        return result
+
+    def make_list_on_re_compile(self, re_txt, file_name):
+        """
+        텍스트화일을 읽어서 re에 맞도록 한것을 리스트로 만드는 것이다
+        함수인 def를 기준으로 저장을 하며, [[공백을없앤자료, 원래자료, 시작줄번호].....]
+		"""
+        re_com = re.compile(re_txt)
+        f = open(file_name, 'r', encoding='UTF8')
+        lines = f.readlines()
+        num = 0
+        temp = ""
+        temp_original = ""
+        result = []
+        for one_line in lines:
+            aaa = re.findall(re_com, str(one_line))
+            original_line = one_line
+            changed_line = one_line.replace(" ", "")
+            changed_line = changed_line.replace("\n", "")
+
+            if aaa:
+                result.append([temp, temp_original, num])
+                temp = changed_line
+                temp_original = original_line
+            # print("발견", num)
+            else:
+                temp = temp + changed_line
+                temp_original = temp_original + one_line
         return result
 
-    def replace_by_resql (self, re_sql, input_text, replace_word):
+    def replace (self, re_sql, replace_word, input_text):
+        """
+        입력자료를 원하는 문자로 바꾸는것
+        """
+        result = re.sub(re_sql, replace_word, input_text, flags=re.MULTILINE)
+        return result
+
+    def replace_by_jfsql (self, jf_sql, replace_word, input_text):
+        """
+        입력자료를 원하는 문자로 바꾸는것
+        """
+        re_sql = self.jfinder(jf_sql)
+        #print(re_sql)
         result = re.sub(re_sql, replace_word, input_text)
         return result
 
-    def run (self, jf_sql, input_text):
-        #결과값을 얻는것이 여러조건들이 있어서 이것을 하나로 만듦
-        # [[결과값, 시작순서, 끝순서, [그룹1, 그룹2...], match결과].....]
+    def run_by_jfsql (self, jf_sql, input_text):
+        """
+        결과값을 얻는것이 여러조건들이 있어서 이것을 하나로 만듦
+        [[결과값, 시작순서, 끝순서, [그룹1, 그룹2...], match결과].....]
+		"""
         re_sql = self.jfinder(jf_sql)
         re_com = re.compile(re_sql)
         result_match = re_com.match(input_text)
         result_finditer = re_com.finditer(input_text)
 
         final_result = []
         num=0
@@ -146,260 +339,218 @@
             #제일 첫번째 결과값에 match랑 같은 결과인지 넣는것
             if num == 0: temp.append(result_match)
             final_result.append(temp)
             num+=1
         return final_result
 
     def run_by_resql(self, input_sql, input_text):
+        """
+		regex의 스타일을 실행시키는것
+		"""
         re_com = re.compile(input_sql)
         re_results = re_com.finditer(input_text)
         result = []
         if re_results:
             for one in re_results:
                 result.append([one.group(), one.start(), one.end()])
         return result
 
-
-    def make_list_on_re_compile(self, re_txt, file_name):
-        # 텍스트화일을 읽어서 re에 맞도록 한것을 리스트로 만드는 것이다
-        # 함수인 def를 기준으로 저장을 하며, [[공백을없앤자료, 원래자료, 시작줄번호].....]
-        re_com = re.compile(re_txt)
-        f = open(file_name, 'r', encoding='UTF8')
-        lines = f.readlines()
-        num = 0
-        temp = ""
-        temp_original = ""
-        result = []
-        for one_line in lines:
-            aaa = re.findall(re_com, str(one_line))
-            original_line = one_line
-            changed_line = one_line.replace(" ", "")
-            changed_line = changed_line.replace("\n", "")
-
-            if aaa:
-                result.append([temp, temp_original, num])
-                temp = changed_line
-                temp_original = original_line
-            # print("발견", num)
-            else:
-                temp = temp + changed_line
-                temp_original = temp_original + one_line
+    def search_all_cap(self, input_text):
+        """
+        모두 알파벳대문자
+		"""
+        re_basic = "^[A-Z]+$"
+        result = re.findall(re_basic, input_text)
         return result
 
-    def get_between_number_length(self, input_text, m, n):
-        # m,n개사이인것만 추출
-        re_basic = "^\d{" + str(m) + "," + str(n) + "}$"
+    def search_handphone_only(self, input_text):
+        """
+        특수문자가들어가있는지
+		"""
+        re_basic = "^(010|019|011)-\d{4}-\d{4}"
         result = re.findall(re_basic, input_text)
         return result
 
-    def get_between_text_length(self, input_text, m, n):
-        # 문자수제한 : m다 크고 n보다 작은 문자
-        re_basic = "^.{" + str(m) + "," + str(n) + "}$"
+    def search_ip_address(self, input_text):
+        """
+        이메일주소 입력
+		"""
+        re_basic = "((?:(?:25[0-5]|2[0-4]\\d|[01]?\\d?\\d)\\.){3}(?:25[0-5]|2[0-4]\\d|[01]?\\d?\\d))"
         result = re.findall(re_basic, input_text)
         return result
 
-    def get_text_between_ab(self, input_text, text_a, text_b):
-        # 입력된 자료에서 두개문자사이의 글자를 갖고오는것
-        replace_lists = [
-            ["(", "\("],
-            [")", "\)"],
-        ]
-        origin_a = text_a
-        origin_b = text_b
-
-        for one_list in replace_lists:
-            text_a = text_a.replace(one_list[0], one_list[1])
-            text_b = text_b.replace(one_list[0], one_list[1])
-        re_basic = text_a + "[^" + str(origin_b) + "]*" + text_b
+    def search_korean_only(self, input_text):
+        """
+        모두 한글인지
+		"""
+        re_basic = "[ㄱ-ㅣ가-힣]"
         result = re.findall(re_basic, input_text)
         return result
 
+    def search_special_char(self, input_text):
+        """
+        특수문자가들어가있는지
+		"""
+        re_basic = "^[a-zA-Z0-9]"
+        result = re.findall(re_basic, input_text)
+        return result
 
-    def check_hangul_jamo(self, text):
-        # 한글자의 한글을 자음과 모음으로 구분해 주는것
-        one_byte_data = text.encode("utf-8")
-        value_sum = 0
-        char_type = ""
-
-        if str(text) in "0123456789":
-            char_type = "숫자"
-
-        # compile_1 = re.compile("\d")
-        # if str(text) in re.:
-        #    char_type = "숫자"
-
-        compile_1 = re.compile("\d+")
-        no = compile_1.findall(text)
-
-        try:
-            no_1 = int(one_byte_data[0])
-            no_2 = int(one_byte_data[1])
-            no_3 = int(one_byte_data[2])
-            new_no_1 = (no_1 - 234) * 64 * 64
-            new_no_2 = (no_2 - 128) * 64
-            new_no_3 = (no_3 - 128)
-            value_sum = new_no_1 + new_no_2 + new_no_3
-
-            if value_sum >= -28367 and value_sum <= -28338:
-                char_type = "ja_only"
-            if value_sum >= -28337 and value_sum <= -28317:
-                char_type = "mo_only"
-
-        except:
-            char_type = "no_han"
-            # 이것은 영어나 숫자, 특수문자라는 뜻이다
-            no_1 = one_byte_data
-            no_2 = ""
-            no_3 = ""
-
-        return [char_type, text]
-
-
-    def check_all_cap(self, input_text):
-        # 모두 알파벳대문자
-        re_basic = "^[A-Z]+$"
+    def search_number_between_len1_len2(self, m, n, input_text):
+        """
+        m,n개사이인것만 추출
+		"""
+        re_basic = "^\d{" + str(m) + "," + str(n) + "}$"
         result = re.findall(re_basic, input_text)
         return result
 
-    def check_dash_date(self, input_text):
-        # 모두 알파벳대문자
+    def search_dash_date(self, input_text):
+        """
+        모두 알파벳대문자
+		"""
         re_basic = "^\d{4}-\d{1,2}-\d{1,2}$"
         result = re.findall(re_basic, input_text)
         return result
 
-    def check_email_address(self, input_text):
-        # 이메일주소 입력
+    def search_email_address(self, input_text):
+        """
+        이메일주소 입력
+		"""
         re_basic = "^\w+([-+.]\w+)*@\w+([-.]\w+)*\.\w+([-.]\w+)*$"
         result = re.findall(re_basic, input_text)
         return result
 
-    def check_eng_only(self, input_text):
-        # 모두 영문인지
+    def search_eng_only(self, input_text):
+        """
+        모두 영문인지
+		"""
         re_basic = "^[a-zA-Z]+$"
         result = re.findall(re_basic, input_text)
         return result
 
-    def check_handphone_only(self, input_text):
-        # 특수문자가들어가있는지
-        re_basic = "^(010|019|011)-\d{4}-\d{4}"
+    def search_between_len1_len2(self, m, n , input_text):
+        """
+        문자수제한 : m다 크고 n보다 작은 문자
+		"""
+        re_basic = "^.{" + str(m) + "," + str(n) + "}$"
         result = re.findall(re_basic, input_text)
         return result
 
-    def check_ip_address(self, input_text):
-        # 이메일주소 입력
-        re_basic = "((?:(?:25[0-5]|2[0-4]\\d|[01]?\\d?\\d)\\.){3}(?:25[0-5]|2[0-4]\\d|[01]?\\d?\\d))"
-        result = re.findall(re_basic, input_text)
-        return result
+    def search_num_only(self, input_text):
+        """
+		단어중에 나와있는 숫자만 분리하는기능
+		"""
+        re_compile = re.compile(r"([0-9]+)")
+        result = re_compile.findall(input_text)
+        new_result = []
+        for dim1_data in result:
+            for dim2_data in dim1_data:
+                new_result.append(dim2_data)
+        return new_result
 
-    def check_korean_only(self, input_text):
-        # 모두 한글인지
-        re_basic = "[ㄱ-ㅣ가-힣]"
-        result = re.findall(re_basic, input_text)
+    def search_between_word1_word2_by_jfsql(self, word_a, word_b, input_text):
+        """
+        두 단어사이의 글자를 갖고오는 것
+        """
+        jf_sql = "(?<=\\" + str(word_a) + ")(.*?)(?="+str(word_b) + ")"
+        result = self.search_all_by_resql(jf_sql, input_text)
         return result
 
-    def check_special_char(self, input_text):
-        # 특수문자가들어가있는지
-        re_basic = "^[a-zA-Z0-9]"
-        result = re.findall(re_basic, input_text)
+    def search_between_brackets_by_jfsql(self, input_text):
+        """
+        괄호안의 문자 갖고오기
+        """
+        jf_sql = "(?<=\\()(.*?)(?=\\))"
+        result = self.search_all_by_resql(jf_sql, input_text)
         return result
 
-    def delete_except_engnum(self, input_text):
-        # 알파벳과 숫자만 있는것을 확인하는것
-        re_com = re.compile("[^A-Za-z0-9]")
-        if (re_com.search(input_text) == None):
-            new_text = input_text
-        else:
-            print(re_com.search(input_text))
-            new_text = re_com.sub("", input_text)
-            print(new_text)
-        return new_text
+    def search_by_jfsql (self, jf_sql, input_text):
+        re_sql = self.jfinder(jf_sql)
+        #print(re_sql)
+        result = self.search_all_by_resql(re_sql, input_text)
+        return result
 
-    def delete_except_korengnum(self, input_text):
-        # 한글, 영어, 숫자만 남기고 나머지는 모두 지우는 것이다
-        re_com = re.compile("[^A-Za-z0-9ㄱ-ㅎㅏ-ㅣ가-힣]")
-        if (re_com.search(input_text) == None):
-            new_text = input_text
-        else:
-            print(re_com.search(input_text))
-            new_text = re_com.sub("", input_text)
-            print(new_text)
-        return new_text
+    def search_by_resql (self, re_sql, input_text):
+        result = self.search_all_by_resql(re_sql, input_text)
+        return result
 
-    def delete_except_numcomma(self, input_text):
-        # 숫자중에서 ,로 분비리된것중에서 ,만 없애는것
-        # 1,234,567 => 1234567
-        re_com = re.compile("[0-9,]")
-        re_com_1 = re.compile("[,]")
-        if (re_com.search(input_text) == None):
-            new_text = input_text
-        else:
-            new_text = re_com_1.sub("", input_text)
-            print(new_text)
-        return new_text
+    def search_all_by_jfsql (self, jf_sql, input_text):
+        re_sql = self.jfinder(jf_sql)
+        result = self.search_all_by_resql(re_sql, input_text)
+        return result
 
-    def delete_except_specialchar(self, input_text):
-        # 공백과 특수문자등을 제외하고 같으면 새로운 y열에 1을 넣는 함수
-        # 리스트의 사이즈를 조정한다
-        re_com = re.compile("[\s!@#$%^*()\-_=+\\\|\[\]{};:'\",.<>\/?]")
-        if (re_com.search(input_text) == None):
-            new_text = input_text
-        else:
-            new_text = re_com.sub("", input_text)
-            print(new_text)
-        return new_text
+    def search_all_by_resql (self, re_sql, input_text):
+        """
+        결과값을 얻는것이 여러조건들이 있어서 이것을 하나로 만듦
+        [[결과값, 시작순서, 끝순서, [그룹1, 그룹2...], match결과].....]
+        """
+        #print("re문장은 : ", re_sql)
+        #print("결과값의 의미 : [[결과값, 시작순서, 끝순서, [그룹1, 그룹2...], match결과].....]")
+        re_com = re.compile(re_sql)
+        result_match = re_com.match(input_text)
+        result_finditer = re_com.finditer(input_text)
 
-    def delete_text_specialletter(self, input_list):
-        # 입력받은 텍스트로된 리스트의 자료를 전부 특수문자를 없앤후 돌려주는 것이다
-        # 입력된 자료가 1차원 리스트인지 판단한다
-        if type(input_list) == type([]) and type(input_list[0]) != type([]):
-            result = []
-            for one in input_list:
-                if one != "" or one != None:
-                    temp = self.re_delete_specialletter(one)
-                    result.append(temp)
-        return result
+        final_result = []
+        num=0
+        for one_iter in result_finditer:
+            temp=[]
+            #찾은 결과값과 시작과 끝의 번호를 넣는다
+            temp.append(one_iter.group())
+            temp.append(one_iter.start())
+            temp.append(one_iter.end())
 
-    def delete_all_explanation(self, input_text):
-        input_text = re.sub(re.compile(r"'''.*'''", re.DOTALL), "", input_text)
-        input_text = re.sub(re.compile(r'""".*"""', re.DOTALL), "", input_text)
-        result = re.sub(re.compile(r"#.*[\n]"), "\n", input_text)
-        return result
+            #그룹으로 된것을 넣는것이다
+            temp_sub = []
+            if len(one_iter.group()):
+                for one in one_iter.groups():
+                    temp_sub.append(one)
+                temp.append(temp_sub)
+            else:
+                temp.append(temp_sub)
 
+            #제일 첫번째 결과값에 match랑 같은 결과인지 넣는것
+            if num == 0: temp.append(result_match)
+            final_result.append(temp)
+            num+=1
+        return final_result
 
-    def pick_eng_in_text(self, input_text):
-        """
-		단어중에 나와있는 영어만 분리하는기능
-		"""
-        re_compile = re.compile(r"([a-zA-Z]+)")
-        result = re_compile.findall(input_text)
-        new_result = []
-        for dim1_data in result:
-            for dim2_data in dim1_data:
-                new_result.append(dim2_data)
-        return new_result
 
-    def pick_num_in_text(self, input_text):
+    def delete_all_explanation(self, input_text):
         """
-		단어중에 나와있는 숫자만 분리하는기능
+		py화일의 설명문의 줄들을 제거하는 코드
 		"""
-        re_compile = re.compile(r"([0-9]+)")
-        result = re_compile.findall(input_text)
-        new_result = []
-        for dim1_data in result:
-            for dim2_data in dim1_data:
-                new_result.append(dim2_data)
-        return new_result
-
-    def convert_data_except_num_n_eng(self, original_data):
-        """
-        영문과 숫자와 공백을 제외하고 다 제거를 하는것
-        입력형태 :
-        출력형태 :
-        """
-        result = []
-        for one_data in original_data:
-            temp = ""
-            for one in one_data:
-                if str(one) in ' 0123456789abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ_':
-                    temp = temp + str(one)
-            result.append(temp)
-        return result
+        input_text = re.sub(re.compile(r"[\s]*#.*[\n]"), "\\n", input_text)
+        input_text = re.sub(re.compile(r"[\s]*'''.*?'''", re.DOTALL | re.MULTILINE), "\n", input_text)
+        input_text = re.sub(re.compile(r'[\s]*""".*?"""', re.DOTALL | re.MULTILINE), "\n", input_text)
+        input_text = re.sub(re.compile(r'^[\s]*[\n]'), "", input_text)
+        return input_text
+
+
+    def delete_over_2_empty_lines(self, input_text):
+        input_text = re.sub(re.compile(r"([\s]*\\n){2,}"), "\\n", input_text)
+        return input_text
+
+
+    ####################################################################
+
+    def change_number_to_tel_style(self, input_value):
+       # 전화번호나 핸드폰 번호 스타일을 바꿔주는것
+       # 전화번호를 21345678 =>02-134-5678 로 변경하는 것
+       result = input_value
+       value = str(int(input_value))
+       if len(value) == 8 and value[0] == "2":
+          # 22345678 => 02-234-5678
+          result = "0" + value[0:1] +"-"+ value[1:4] +"-"+ value[4:]
+       elif len(value) == 9:
+          if value[0:2] == "2":
+             # 223456789 => 02-2345-6789
+             result = "0" + value[0:1] +"-"+ value[1:5] +"-"+ value[5:]
+          elif value[0:2] == "11":
+             # 113456789 => 011-345-6789
+             result = "0" + value[0:2] +"-"+ value[2:5] +"-"+ value[5:]
+          else:
+             # 523456789 => 052-345-6789
+             result = "0" + value[0:2] +"-"+ value[2:5] +"-"+ value[5:]
+       elif len(value) == 10:
+          # 5234567890 => 052-3456-7890
+          # 1034567890 => 010-3456-7890
+          result = "0" + value[0:2] +"-"+ value[2:6] +"-"+ value[6:]
+       return result
```

### Comparing `halmoney-2.1.1/src/halmoney/pcell.py` & `halmoney-3.0.0/src/halmoney/pcell.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 # -*- coding: utf-8 -*-
-
-import win32gui
-import win32com.client
-from halmoney import basic_data, scolor
-import re
-import math
-import string
-import random
-import time
+import re #내장모듈
+import os #내장모듈
+import math #내장모듈
+import string #내장모듈
+import random #내장모듈
+from itertools import combinations_with_replacement #내장모듈
+
+import scolor  # halmoney 모듈
+import basic_data  # halmoney 모듈
+
+import win32gui #pywin32의 모듈
+import win32api #pywin32의 모듈
+import win32com.client #pywin32의 모듈
 
 class pcell:
-
+	"""
+	엑셀을 컨트롤 할수있는 모듈
+	"""
 	def __init__(self, filename=""):
 		#공통으로 사용할 변수들을 설정하는 것
 		self.color = scolor.scolor()
-		self.basic = basic_data.basic_data()
-		self.common_data = self.basic.basic_data()
-
+		self.data_set_basic = basic_data.basic_data()
 		# 만약 화일의 경로가 있으면 그 화일을 열도록 한다
 		self.xlapp = win32com.client.dynamic.Dispatch('Excel.Application')
 		self.xlapp.Visible = 1
 
 		if filename != None:
 			self.filename = filename.lower()
 
@@ -47,151 +51,103 @@
 				win32gui.MessageBox(0, "Please check file path", "xxw.halmoney.com", 0)
 
 	def add_button_with_macro(self, sheet_name="", xyxy="", macro_code="", title=""):
 		"""
 		매크로랑 연결된 버튼을 만드는것
 		버튼을 만들어서 그 버튼에 매크로를 연결하는 것이다
 		매크로와 같은것을 특정한 버튼에 연결하여 만드는것을 보여주기위한 것이다
+		Add(왼쪽의 Pixel, 위쪽 Pixce, 넓이, 높이)
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 		new_btn = sheet_object.Buttons()
-		new_btn.Add(x1, x2, y1, y2)
+		sheet_object.Cells(x1, y1).Select()
+		left_px, top_px, width_px, height_px = self.read_coord_in_cell("", [x1, y1])
+		new_btn.Add(left_px, top_px, width_px, height_px)
 		new_btn.OnAction = macro_code
 		new_btn.Text = title
 
 	def add_sheet_new(self):
 		"""
 		시트하나 추가하기
 		위치는 자동으로 제일 뒤에 추가되는것이며, 시트이름이 없어 자동으로 만들어지는 이름입니다
 		"""
 		self.xlbook.Worksheets.Add()
 
+	def add_sheet_new_with_name(self, input_name=""):
+		"""
+		시트하나 추가하기
+		위치는 자동으로 제일 뒤에 추가되는것이며, 시트이름이 없어 자동으로 만들어지는 이름입니다
+		"""
+		self.xlbook.Worksheets.Add()
+		Sheet = self.xlbook.ActiveSheet
+		if input_name != "":
+			Sheet.Name = input_name
+
 	def add_text_in_range_at_left(self, sheet_name="", xyxy="", input_text="입력필요"):
 		"""
 		선택한 영역의 왼쪽에 입력한 글자를 추가
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 		for x in range(x1, x2 + 1):
 			for y in range(y1, y2 + 1):
-				cell_value = str(sheet_object.Cells(x, y).Value)
-				if cell_value == None: cell_value = ""
+				cell_value = sheet_object.Cells(x, y).Value
+				if cell_value == None:
+					cell_value = ""
 				sheet_object.Cells(x, y).Value = str(input_text)+cell_value
 
 	def add_text_in_range_at_right(self, sheet_name="", xyxy="", input_text="입력필요"):
 		"""
 		선택한 영역의 오른쪽에 입력한 글자를 추가
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 		for x in range(x1, x2 + 1):
 			for y in range(y1, y2 + 1):
-				cell_value = str(sheet_object.Cells(x, y).Value)
-				if cell_value == None: cell_value = ""
+				cell_value = sheet_object.Cells(x, y).Value
+				if cell_value == None:
+					cell_value = ""
 				sheet_object.Cells(x, y).Value = cell_value+str(input_text)
 
-	def add_text_in_range_bystep(self, sheet_name="", xyxy="", input_text="", step=""):
+	def add_text_in_range_by_step(self, sheet_name="", xyxy="", input_text="", step=""):
 		"""
 		선택한 영역의 시작점부터 n번째 셀마다 값을 넣기
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 		basic_list = []
 		for one_data in input_text.split(","):
 			basic_list.append(one_data.strip())
-
-		for x in range(int(basic_list[0]), int(basic_list[1]) + 1, int(basic_list[2])):
+		num = 1
+		for x in range(x1, x2+1):
 			for y in range(y1, y2 + 1):
-				cell_value = str(sheet_object.Cells(x, y).Value)
-				if cell_value == None: cell_value = ""
-				sheet_object.Cells(x, y).Value = cell_value+str(input_text)
+				if divmod(num, int(step))[1] == 0:
+					sheet_object.Cells(x, y).Value = str(input_text)
+				num = num +1
 
 	def add_text_in_range_by_xystep(self, sheet_name="", xyxy="", input_text="", xystep=[1, 1]):
 		"""
 		선택한 영역의 시작점부터 x,y 번째 셀마다 값을 넣기
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 
-		for x in range(x1, x2 + 1):
-			if divmod(x, xystep[0])[1] == 0:
-				for y in range(y1, y2 + 1):
-					if divmod(y, xystep[1])[1] == 0:
-						cell_value = str(sheet_object.Cells(x, y).Value)
+		for x in range(x1, x2 +1):
+			if divmod(x, xystep[0])[1] ==0:
+				for y in range(y1, y2+1):
+					if divmod(x, xystep[1])[1] == 0:
+						cell_value = sheet_object.Cells(x, y).Value
 						if cell_value == None:
-							cell_value = ""
-						# self.write_value_in_cell(sheet_name, [x, y], cell_value + str(input_text))
-						sheet_object.Cells(x, y).Value = cell_value + str(input_text)
-
-	def check_address_with_datas(self, xyxy="", input_datas="입력필요"):
-		"""
-		입력주소와 자료를 받아서 최소로할것인지 최대로 할것인지를 골라서 나타낼려고 한다
-		[$A$1], [$A$1:$B$2], [$1:$7], [$A:$B] ["A1"],[2,1,3,2], [1,2]이 경우가 가능
-		Output Style :  [["$A$2:$B$3"],["A1","B2],[2,1,3,2]]무조건 3개의 형태로 나오도록 만든다
-		"""
-		x1, y1, x2, y2 = self.check_address_value(xyxy)
-		result = {}
-		y_len = len(input_datas)
-		x_len = len(input_datas[0])
-		y_len_rng = y2 - y1
-		x_len_rng = x2 - x1
-		max_num = max(map(lambda y: len(y), input_datas))
-		min_num = min(map(lambda y: len(y), input_datas))
-		max_y = max(y_len, y_len_rng)
-		max_x = max(max_num, x_len_rng)
-		min_y = max(y_len, y_len_rng)
-		min_x = max(x_len, x_len_rng)
-		# 입력할것중 가장 적은것을 기준으로 적용
-		result["xyxy_min"] = [x1, y1, x1 + min_y, y1 + min_num]
-		# 입력할것중 가장 큰것을 기준으로 적용
-		result["xyxy_max"] = [x1, y1, x1 + max_y, y1 + max_y]
-		# 일반적인기준으로 적용하는것
-		result["xyxy_basic"] = [x1, y1, x1 + x_len, y1 + max_num]
-		return result
-
-	def change_address_to_xyxy_v1(self, address):
-		"""
-		들어오는 값은 #$E$13, $4:$12, $B:$I, $C$4:$F$11 이런 형태만 한다
-		Output Style :  [y1, x1, y2, x2] ==> [원래값, [1,2,3,4]]
-		"""
-		temp_list_0 = []
-		temp_list_1 = []
-		temp_list_0 = address.split(":")
-		for one in temp_list_0:
-			temp_list_1.append(one.split("$"))
-		if len(temp_list_1[0]) == 2:
-			if temp_list_1[0][1].isdigit():
-				address_list = [0, temp_list_1[0][1], 0, temp_list_1[1][1]]
-			else:
-				address_list = [temp_list_1[0][1], 0, temp_list_1[1][1], 0]
-		if len(temp_list_1[0]) == 3:
-			address_list = [temp_list_1[0][1], temp_list_1[0][2], temp_list_1[1][1], temp_list_1[1][2]]
-		if address_list[0] != 0: address_list[0] = self.change_char_to_num(address_list[0])
-		if address_list[2] != 0: address_list[2] = self.change_char_to_num(address_list[2])
-		address_list = [int(address_list[0]), int(address_list[1]), int(address_list[2]), int(address_list[3])]
-		return [address, address_list]
-
-	def change_address_to_xyxy(self, xyxy):
-		"""
-		셀의 $aa$10 --> aa10,으로 바꾸어주는 함수
-		문자, 숫자, :만을 남겨놓고 나머지는 모두 삭제하는 것이다
-		*** $를 없애는 코드를 별도로 만든다
-		"""
-		char_in_start_cell = ""
-		eng_spell = string.ascii_lowercase + string.digits + ':'
-		list_cell = list(xyxy)
-		for one_word in list_cell:
-			one_word = str(one_word).lower()
-			if one_word in eng_spell:
-				char_in_start_cell = char_in_start_cell + one_word
-		return char_in_start_cell
+							cell_value=""
+						sheet_object.Cells(x, y).Value = cell_value+str(input_text)
 
 	def change_char_to_num(self, input_text="입력필요"):
 		"""
+		주소를 바꿔주는 것이다
 		문자가 오던 숫자가 오던 숫자로 변경하는 것이다
 		 b를 2로 바꾸어 주는것
 		"""
 		aaa = re.compile("^[a-zA-Z]+$")  # 처음부터 끝가지 알파벳일때
 		result_str = aaa.findall(str(input_text))
 
 		bbb = re.compile("^[0-9]+$")  # 처음부터 끝가지 숫자일때
@@ -206,14 +162,27 @@
 				no = no + 1
 		elif result_num != []:
 			result = int(input_text)
 		else:
 			result = "error"
 		return result
 
+	def change_inputcolor_to_rgb(self, input_color):
+		"""
+		입력된 색깔을 rgb로 바꾸는 것
+		"""
+		input_type = type(input_color)
+		if input_type == type(123):
+			result = self.color.change_rgbint_to_rgb(input_color)
+		elif input_type == type("abc"):
+			result = self.color.change_scolor_to_rgb(input_color)
+		elif input_type == type([]):
+			result = input_color
+		return result
+
 	def change_inputdata_to_list2d(self, input_data):
 		"""
 		입력된 자료형에 따라서 2차원으로 만들어 주는것
 		1차원의 리스트는 [1,2,3,4]의 형태이며
 		이것은 같은 가로에 세로의 글자가 다른것이다
 		"""
 		if type(input_data) == type([]) or type(input_data) == type(()):
@@ -221,32 +190,34 @@
 				result = input_data
 			else:
 				result = [input_data]
 		elif type(input_data) == type("123") or type(input_data) == type(123):
 			result = [[input_data]]
 		return result
 
-	def change_list1d_to_list2d(self, input_data):
+	def change_list1d_to_list2d(self, input_list1d):
 		"""
-		1차원의 리스트가 오면 2차원으로 만들어주는 것
+		1차원의 리스트를  2차원으로 만드는 것
+		입력 : [1,2,3,4]
+		출력 : [[1], [2], [3], [4],]
 		"""
 		result = []
-		if len(input_data) > 0:
-			if type(input_data[0]) != type([]):
-				for one in input_data:
+		if len(input_list1d) > 0:
+			if type(input_list1d[0]) != type([]):
+				for one in input_list1d:
 					result.append([one, ])
 		return result
 
 	def change_list1d_to_list2d_with_yline_style(self, input_list1d):
 		"""
-		1차원의 리스트를 세로열에 출력이 되도록 2차원으로 만든다
+		1차원의 리스트를  2차원으로 만드는 것
+		입력 : [1,2,3,4]
+		출력 : [[1], [2], [3], [4],]
 		"""
-		result = []
-		for one in input_list1d:
-			result.append([one])
+		result = self.change_list1d_to_list2d(input_list1d)
 		return result
 
 	def change_list2d_as_samelen(self, input_list2d="입력필요"):
 		"""
 		2차원 리스트의 최대 길이로 같게 만드는 것
 		가끔 자료의 갯수가 달라서 생기는 문제가 발생할 가능성이 있는것을 맞추는것
 		추가할때는 ""를 맞는갯수를 채워넣는다
@@ -259,14 +230,28 @@
 			if max_num == one_len:
 				result.append(one)
 			else:
 				one.extend([input_text] * (max_num - one_len))
 				result.append(one)
 		return result
 
+	def change_data_position_for_list2d_by_2_index(self, input_list2d, input_no_list):
+		"""
+		2차원 리스트의 자료에서 각 라인별 2개의 위치를 바꾼는것
+		change_position_for_list2d_by_2_index([[1,2,3], [4,5,6]], [0,2])
+		[[1,2,3], [4,5,6]] ==> [[3,2,1], [6,5,4]]
+		"""
+		for before, after in input_no_list:
+			for no in range(len(input_list2d)):
+				value1 = input_list2d[no][before]
+				value2 = input_list2d[no][after]
+				input_list2d[no][before] = value2
+				input_list2d[no][after] = value1
+		return input_list2d
+
 	def change_num_to_char(self, input_data="입력필요"):
 		"""
 		입력값 : 27 => 출력값 : aa
 		숫자를 문자로 바꿔주는 것
 		"""
 		re_com = re.compile(r"([0-9]+)")
 		result_num = re_com.match(str(input_data))
@@ -286,19 +271,42 @@
 			for one_data in result:
 				result_01 = string.ascii_lowercase[one_data - 1] + result_01
 			final_result = result_01
 		else:
 			final_result = input_data
 		return final_result
 
-	def change_rgb_to_rgbint(self, input_data):
+	def change_rgb_to_rgbint(self, input_rgb):
 		"""
 		rgb인 값을 color에서 인식이 가능한 정수값으로 변경
 		"""
-		result = (int(input_data[2])) * (256 ** 2) + (int(input_data[1])) * 256 + int(input_data[0])
+		result = (int(input_rgb[2])) * (256 ** 2) + (int(input_rgb[1])) * 256 + int(input_rgb[0])
+		return result
+
+	def change_rgbint_to_colorname(self, rgbint ):
+		"""
+		rgb의 정수값을 color이름으로 변경
+		"""
+		try :
+			rgblist = self.change_rgbint_to_rgb(rgbint)
+			print("rgblist", rgblist)
+			color_index = self.data_dic_colorindex_to_rgblist(rgblist)
+			print("color_index", color_index)
+			colorname = self.data_dic_colorname_to_colorindex(color_index)
+		except:
+			colorname = None
+		return colorname
+
+	def change_rgbint_to_rgb(self, input_int):
+		"""
+		rgb의 int값을 rgb 리슽형으로 바꾸는 것이다
+		"""
+		mok0, namuji0 = divmod(input_int, 256*256)
+		mok1, namuji1 = divmod(namuji0, 256)
+		result = [namuji1, mok1, mok0]
 		return result
 
 	def change_sheet_name(self, old_name="입력필요", new_name="입력필요"):
 		"""
 		시트이름을 변경하는 것
 		"""
 		self.xlbook.Worksheets(old_name).Name = new_name
@@ -336,218 +344,305 @@
 			result = [temp[1][0], temp[0][0], temp[1][0], temp[0][0]]
 		elif len(temp) == 4 and temp[0][1] != temp[1][1] and temp[0][1] == "num":
 			# "a2b3"일때
 			result = [temp[0][0], temp[1][0], temp[2][0], temp[3][0]]
 		elif len(temp) == 4 and temp[0][1] != temp[1][1] and temp[0][1] == "string":
 			# "2a3c"일때
 			result = [temp[1][0], temp[0][0], temp[3][0], temp[2][0]]
+		return result
 
+	def change_string_to_address(self, input_text="입력필요"):
+		result = self.change_string_address(input_text)
 		return result
 
-	def change_range_value_to_capital(self, sheet_name, xyxy):
+	def change_string_address_to_xyxy(self, input_text="입력필요"):
+		result = self.change_string_address(input_text)
+		return result
+
+	def change_value_in_range_as_lower(self, sheet_name="", xyxy=""):
+		"""
+		선택영역안의 모든글자를 소문자로 만들어 주는것
+		screen update를 off로 사용
+		값 읽어오는것을 range형태로 변경
+		"""
+		sheet_object = self.check_sheet_name(sheet_name)
+		x1, y1, x2, y2 = self.check_address_value(xyxy)
+		list_2d = self.read_value_in_range(sheet_name, xyxy)
+		print(list_2d[0:3])
+		self.screen_update_off()
+		for x in range(x1, x2 + 1):
+			for y in range(y1, y2 + 1):
+				print(x, y)
+				try:
+					sheet_object.Cells(x, y).Value = (list_2d[x - x1][y - y1]).lower()
+				except:
+					pass
+		self.screen_update_on()
+
+	def change_value_in_range_to_capital(self, sheet_name, xyxy):
 		"""
 		change_text_as_capital(sheet_name, xyxy)
 		선택한 영역의 값들을 첫글자만 대문자로 변경
 		입력값 : 입력값없이 사용가능
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 
 		for x in range(x1, x2 + 1):
 			for y in range(y1, y2 + 1):
 				value = str(sheet_object.Cells(x, y).Value)
-				if value == None: value = ""
-				value = str(sheet_object.Cells(x, y).Value)
-
-				sheet_object.Cells(x, y).Value = value.capitalize()
+				if value == None:
+					pass
+				else:
+					sheet_object.Cells(x, y).Value = value.capitalize()
 
-	def change_range_value_to_lower(self, sheet_name="", xyxy=""):
+	def change_value_in_range_to_lower(self, sheet_name="", xyxy=""):
 		"""
 		선택영역안의 모든글자를 소문자로 만들어 주는것
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
+
 		for x in range(x1, x2 + 1):
 			for y in range(y1, y2 + 1):
 				value = str(sheet_object.Cells(x, y).Value)
-				if value == None: value = ""
-				value = str(sheet_object.Cells(x, y).Value)
-
-				sheet_object.Cells(x, y).Value = value.lower()
+				if value == None:
+					pass
+				else:
+					sheet_object.Cells(x, y).Value = value.lower()
 
-	def change_range_value_to_ltrim(self, sheet_name="", xyxy=""):
+	def change_value_in_range_to_ltrim(self, sheet_name="", xyxy=""):
 		"""
 		왼쪽끝의 공백을 삭제하는 것
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 
 		for x in range(x1, x2 + 1):
 			for y in range(y1, y2 + 1):
 				cell_value = str(sheet_object.Cells(x, y).Value)
-				changed_data = str(cell_value).lstrip()
-				if cell_value == changed_data or cell_value == None or type(cell_value) == type(123):
+				if cell_value == None:
 					pass
 				else:
-					sheet_object.Cells(x, y).Value = changed_data
-					self.paint_color_in_cell(sheet_name, [x, y], 16)
+					changed_data = str(cell_value).lstrip()
+					if cell_value != changed_data:
+						sheet_object.Cells(x, y).Value = changed_data
+						self.paint_cell_by_scolor(sheet_name, [x, y], "yel+")
 
-	def change_range_value_to_rtrim(self, sheet_name="", xyxy=""):
+	def change_value_in_range_to_rtrim(self, sheet_name="", xyxy="", scolor_name = "yel+"):
+		"""
+		선택한 영역의 셀 값들의 오른쪽 공백을 없앤것
+		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
+
 		for x in range(x1, x2 + 1):
 			for y in range(y1, y2 + 1):
 				cell_value = str(sheet_object.Cells(x, y).Value)
-				changed_data = str(cell_value).rstrip()
-				if cell_value == changed_data or cell_value == None or type(cell_value) == type(123):
+				if cell_value == None:
 					pass
 				else:
-					sheet_object.Cells(x, y).Value = changed_data
-
-					self.paint_color_in_cell(sheet_name, [x, y], 16)
+					changed_data = str(cell_value).rstrip()
+					if cell_value != changed_data:
+						sheet_object.Cells(x, y).Value = changed_data
+						self.paint_cell_by_scolor(sheet_name, [x, y], scolor_name)
 
-	def change_range_value_to_strikethrough(self, sheet_name="", xyxy=""):
+	def change_value_in_range_to_strikethrough(self, sheet_name="", xyxy=""):
+		"""
+		선택한 영역의 셀 값들을 취소선으로 만드는것
+		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
 		my_range.Font.Strikethrough = True
 
-	def change_range_value_to_swapcase(self, sheet_name="", xyxy=""):
+	def change_value_in_range_to_swapcase(self, sheet_name="", xyxy=""):
 		"""
 		선택한 영역의 값들을 대소문자를 변경
-		입력값 : 입력값없이 사용가능
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 		for x in range(x1, x2 + 1):
 			for y in range(y1, y2 + 1):
 				value = str(sheet_object.Cells(x, y).Value)
-				if value == None: value = ""
-				value = str(sheet_object.Cells(x, y).Value)
-				sheet_object.Cells(x, y).Value = value.swapcase()
+				if value == None:
+					pass
+				else:
+					sheet_object.Cells(x, y).Value = value.swapcase()
 
-	def change_range_value_to_trim(self, sheet_name="", xyxy=""):
+	def change_value_in_range_to_trim(self, sheet_name="", xyxy="", scolor_name = "yel"):
 		"""
 		왼쪽끝의 공백을 삭제하는 것
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 		for x in range(x1, x2 + 1):
 			for y in range(y1, y2 + 1):
-				cell_value = str(sheet_object.Cells(x, y).Value)
-				changed_data = self.fun_trim(cell_value)
+				cell_value = sheet_object.Cells(x, y).Value
+				changed_data = self.excel_fun_trim(cell_value)
 				if cell_value == changed_data or cell_value == None:
 					pass
 				else:
 					sheet_object.Cells(x, y).Value = changed_data
-					self.paint_color_in_cell(sheet_name, [x, y], 16)
+					self.paint_cell_by_scolor(sheet_name, [x, y], scolor_name)
 
-	def change_range_value_to_underline(self, sheet_name="", xyxy=""):
+	def change_value_in_range_to_underline(self, sheet_name="", xyxy=""):
+		"""
+		선택한 영역의 셀 값들에 밑줄을 넣는 것
+		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
-
 		my_range.Font.Underline = True
 
-	def change_range_value_to_upper(self, sheet_name="", xyxy=""):
+	def change_value_in_range_to_upper(self, sheet_name="", xyxy=""):
 		"""
 		선택한 영역의 값들을 대문자로 변경
 		입력값 : 입력값없이 사용가능
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 		for x in range(x1, x2 + 1):
 			for y in range(y1, y2 + 1):
 				value = str(sheet_object.Cells(x, y).Value)
-				if value == None: value = ""
-
-				value = str(sheet_object.Cells(x, y).Value)
-				sheet_object.Cells(x, y).Value = value.upper()
+				if value == None:
+					pass
+				else:
+					sheet_object.Cells(x, y).Value = value.upper()
 
 	def change_xy_to_a1(self, xy=[3, 4]):
+		"""
+		xy의 형태로 넘어온 셀값을 A1형식으로 바꾸는 것
+		"""
 		x_char = self.change_num_to_char(xy[0])
 		result = str(x_char[0]) + str(xy[1])
 		return result
 
 	def change_xylist_to_addresschar(self, xy_list=[[1, 1], [2, 3], [2, 4]]):
 		result = ""
 		for one_data in xy_list:
 			y_char = self.change_num_to_char(one_data[1])
 			result = result + str(y_char[0]) + str(one_data[0]) + ', '
 		return result[:-2]
 
+	def change_xyxy_to_pxyxy(self, xyxy):
+		"""
+		셀의 번호를 주면, 셀의 왼쪽과 오른쪽아래의 픽셀 주소를 돌려준다
+		픽샐의 값으로 돌려주는것
+		"""
+		x1, y1, x2, y2 = self.check_address_value(xyxy)
+		px1, py1, px1_w, py1_h = self.read_coord_in_cell("", [x1, y1])
+		px2, py2, px2_w, py2_h = self.read_coord_in_cell("", [x2, y2])
+
+		result = [px1, py1, px2+px2_w-px1, py2+py2_h-py1]
+		return result
+
 	def change_xyxy_to_r1r1(self, xyxy=""):
 		"""
-		Input Style :   [1,2,3,4]
-		Output Style : "b1:d3"
+		입력값 :	[1,2,3,4]
+		출력값 : "b1:d3"
 		"""
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 		str_1 = self.change_num_to_char(y1)
 		str_2 = self.change_num_to_char(y2)
-		result = str_1 + str(x1) + ":" + str_2 + str(y1)
+		result = str_1 + str(x1) + ":" + str_2 + str(x2)
 		return result
 
 	def check_address_value(self, input_data=""):
 		"""
 		입력형태 :, "", [1,2], [1,2,3,4], "$1:$8", "1", "a","a1", "a1b1", "2:3", "b:b"
 		입력된 주소값을 [x1, y1, x2, y2]의 형태로 만들어 주는 것이다
 		입력된 자료의 형태에 따라서 구분을 한다
 		"""
 		if input_data == "" or input_data == None:  # 아무것도 입력하지 않을때
-			input_type = self.read_address_in_selection()
-			result = self.change_string_address(input_type)
+			result = self.read_address_in_selection()
 
 		elif type(input_data) == type("string"):  # 문자열일때
 			result = self.change_string_address(input_data)
 
 		elif type(input_data) == type([]):  # 리스트형태 일때
 			if len(input_data) == 2:
 				result = input_data + input_data
 			elif len(input_data) == 4:
 				result = input_data
+		else:
+			result = self.read_address_in_selection()
+		return result
+
+	def check_address_with_datas(self, xyxy="", input_datas="입력필요"):
+		"""
+		입력주소와 자료를 받아서 최소로할것인지 최대로 할것인지를 골라서 나타낼려고 한다
+		[$A$1], [$A$1:$B$2], [$1:$7], [$A:$B] ["A1"],[2,1,3,2], [1,2]이 경우가 가능
+		Output Style :  [["$A$2:$B$3"],["A1","B2],[2,1,3,2]]무조건 3개의 형태로 나오도록 만든다
+		"""
+		x1, y1, x2, y2 = self.check_address_value(xyxy)
+		result = {}
+		x_len = len(input_datas)
+		y_len = len(input_datas[0])
+
+		y_len_rng = y2 - y1 + 1
+		x_len_rng = x2 - x1 + 1
+
+		max_num = max(map(lambda y: len(y), input_datas))
+		min_num = min(map(lambda y: len(y), input_datas))
+
+		max_y = max(y_len, y_len_rng)
+		max_x = max(max_num, x_len_rng)
+		min_y = max(y_len, y_len_rng)
+		min_x = max(x_len, x_len_rng)
+
+		# 입력할것중 가장 적은것을 기준으로 적용
+		result["xyxy_min"] = [x1, y1, x1 + min_y, y1 + min_num]
+		# 입력할것중 가장 큰것을 기준으로 적용
+		result["xyxy_max"] = [x1, y1, x1 + max_y, y1 + max_y]
+		# 일반적인기준으로 적용하는것
+		result["xyxy_basic"] = [x1, y1, x1 + x_len, y1 + max_num]
 		return result
 
 	def check_cell_type(self, input_data="입력필요"):
 		"""
 		check_cell_type( input_data="입력필요")
 		주소형태의 문자열이 어떤 형태인지 알아 내는 것
 		입력값 : 주소형태의 문자열
-		Output Style : "a1", "aa", "11"
+		출려값 : "a1", "aa", "11"
 		"""
 		result = ""
 		if input_data[0][0] in string.ascii_lowercase and input_data[1][0] in string.digits:
 			result = "a1"
 		if input_data[0][0] in string.ascii_lowercase and input_data[1][0] in string.ascii_lowercase:
 			result = "aa"
 		if input_data[0][0] in string.digits and input_data[1][0] in string.digits:
 			result = "11"
 		return result
 
+	def check_colorname_by_rgbint(self, rgbint ):
+		#예전 코드를 위해 남겨 놓는것
+		result = self.change_rgbint_to_colorname(rgbint )
+		return result
+
 	def check_data_type(self, input_data="입력필요"):
 		"""
 		영역으로 입력된 자료의 형태를 확인해서 돌려주는 것
 		입력값으로 들어온것이 리스트형태인지, 영역의 형태인지, 값의 형태인지를 알아보는것이다
-		Input Style :   1개의 입력값
+		Input Style :	1개의 입력값
 		Output Style : "list", "range", "value", "error"
 		"""
 		if type(input_data) == type([]):
 			result = "list"
 		elif len(str(input_data).split(":")) > 1:
 			result = "range"
 		elif type(input_data) == type("aaa"):
 			result = "value"
 		else:
 			result = "error"
 		return result
 
-	def check_inputdata(self, input_data):
+	def check_datatype_for_inputdata(self, input_data):
 		"""
 		입력된 자료형을 확인하는것
-		입렫된 자료를 2차원으로 만드는 것
-		입력자료는 리스트나 듀플이어야 한다
 		"""
 		if type(input_data) == type([]):
 			if type(input_data[0]) == type([]):
 				# 2차원의 자료이므로 입력값 그대로를 돌려준다
 				result = "list2d_list"
 			elif type(input_data[0]) == type(()):
 				result = "list_tuple"
@@ -563,14 +658,52 @@
 				result = "tuple1d"
 		elif type(input_data) == type(123):
 			result = "int"
 		elif type(input_data) == type("123"):
 			result = "string"
 		return result
 
+	def check_differ_at_2_area(self, input_sa1, input_sa2):
+		"""
+		2개의 같은 크기의 영역의 2개 자료를 비교하여
+		첫번째 같은입력된 자료형을 확인하는것
+		"""
+		datal = self.read_value_in_range(input_sa1[0], input_sa1[1])
+		data2 = self.read_value_in_range(input_sa2[0], input_sa2[1])
+		start_x = input_sa2[1][0]
+		start_y = input_sa2[1][1]
+		for x in range(len(datal)):
+			for y in range(len(datal[0])):
+				if datal[x][y] == data2[x][y]:
+					pass
+				else:
+					self.paint_cell_by_excel_colorno(input_sa2[0], [x + start_x, y + start_y], 3)
+
+	def check_inputcolor_rgb(self, input_color):
+		"""
+		입력값 : 색깔이름
+		출력값 : rgb값
+		"""
+		result = self.change_inputcolor_to_rgb(input_color)
+		return result
+
+	def check_inputdata(self, input_data):
+		"""
+		입력값을 확인하는 것
+		"""
+		result = self.check_datatype_for_inputdata(input_data)
+		return result
+
+	def check_intersect_address(self, xyxy="", input_datas="입력필요"):
+		"""
+		이름을 좀더 사용하기 쉽도록 만든것
+		"""
+		result = self.check_address_with_datas(xyxy, input_datas)
+		return result
+
 	def check_list_address(self, input_list="입력필요"):
 		"""
 		주소값을 4자리 리스트로 만들기 위하여 사용하는것
 		"""
 		result = []
 		if len(input_list) == 1:
 			xy = str(input_list[0]).lower()
@@ -615,15 +748,16 @@
 			else:
 				aaa = str(one)
 			final_result.append(aaa)
 		return final_result
 
 	def check_one_address(self, input_text=""):
 		"""
-		입력된 1개의 주소를 문자인지, 숫자인지와 숫자로 변경하는 것이다
+		입력된 1개의 주소를 문자인지, 숫자인지
+		숫자로 변경하는 것이다
 		"""
 		re_com_1 = re.compile("^[a-zA-Z]+$")  # 처음부터 끝가지 알파벳일때
 		result_str = re_com_1.findall(str(input_text))
 
 		re_com_2 = re.compile("^[0-9]+$")  # 처음부터 끝가지 숫자일때
 		result_num = re_com_2.findall(str(input_text))
 
@@ -642,122 +776,175 @@
 			address_int = "error"
 			address_type = "error"
 		return [address_int, address_type, input_text]
 
 	def check_sheet_name(self, sheet_name=""):
 		"""
 		시트이름으로 객체를 만들어서 돌려주는 것이다
+		이름이 없으면 현재 활성화된 시트를 객체로 만들어 사용한다
 		"""
-		sheet_name = str(sheet_name).lower()
-		if sheet_name == "" or sheet_name == None or sheet_name == "activesheet":
+		if sheet_name == "" or sheet_name == None or str(sheet_name).lower() == "activesheet":
 			sheet_object = self.xlapp.ActiveSheet
 		else:
-			sheet_object = self.xlbook.Worksheets(sheet_name)
+			sheet_object = self.xlbook.Worksheets(str(sheet_name))
 		return sheet_object
 
+	def check_sheet_password(self, isnum="yes", istext_small="yes", istext_big="yes", isspecial="no", len_num=10):
+		"""
+		시트의 암호를 찾아주는것
+		"""
+		check_char = []
+		if isnum == "yes":
+			check_char.extend(list(string.digits))
+		if istext_small == "yes":
+			check_char.extend(list(string.ascii_lowercase))
+		if istext_big == "yes":
+			check_char.extend(list(string.ascii_uppercase))
+		if isspecial == "yes":
+			for one in "!@#$%^*M-":
+				check_char.extend(one)
+		zz = combinations_with_replacement(check_char, len_num)
+		for aa in zz:
+			try:
+				pswd = "".join(aa)
+				self.unlock_sheet("", pswd)
+				print("발견", pswd)
+				break
+			except:
+				pass
+
 	def check_string_address(self, input_text="입력필요"):
 		"""
-		Input Style :   "$1:$8", "1", "a","a1", "a1b1", "2:3", "b:b"
+		Input Style :	"$1:$8", "1", "a","a1", "a1b1", "2:3", "b:b"
 		Output Style :숫자와 문자로 된부분을 구분하는 것
 		string형태의 address를 문자와 숫자로 나누는것
 		"""
 		aaa = re.compile("[a-zA-Z]+|\d+")
 		result = aaa.findall(str(input_text))
 		return result
 
+	def check_x_address(self, input_data="입력필요"):
+		temp = self.check_xx_address(input_data)
+		result = temp[0]
+		return result
+
 	def check_xx_address(self, xyxy="입력필요"):
 		"""
 		입력 주소중 xx가 맞는 형식인지를 확인하는것
 		결과= [2, 2]의 형태로 만들어 주는것
 		"""
-		x1, y1, x2, y2 = self.check_address_value(xyxy)
-		result = [x1, x2]
+		if type(xyxy) ==type([]):
+			if len(xyxy) == 1:
+				result = [xyxy[0], xyxy[0]]
+			elif len(xyxy) == 2:
+				result = xyxy
+		else:
+			x = self.change_char_to_num(xyxy)
+			result = [x,x]
 		return result
 
 	def check_xy_address(self, xyxy=""):
 		"""
 		x나 y의 하나를 확인할때 입력을 잘못하는 경우를 방지하기위해 사용
-		Input Style :   3, [3], [2,3], D, [A,D], [D]
+		Input Style :	3, [3], [2,3], D, [A,D], [D]
 		Output Style : [3,3], [2,3], [4,4], [1,4]
 		"""
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 		result = [x1, y1]
 		return result
 
-	def check_yy_address(self, yy="입력필요"):
+	def check_y_address(self, input_data="입력필요"):
 		"""
 		결과= ["b", "b"]의 형태로 만들어 주는것
 		"""
-		y1, y2 = self.check_address_value(yy)
-		result = [y1, y2]
+		temp = self.check_yy_address(input_data)
+		result = temp[0]
 		return result
 
-	def check_inputcolor_rgb(self, input_value):
-		input_type = type(input_value)
-		if input_type == type(123):
-			result = self.color.change_rgbint_to_rgb(input_value)
-		elif input_type == type("abc"):
-			result = self.color.change_scolor_to_rgb(input_value)
-		elif input_type == type([]):
-			if input_value[0] > 100 or input_value[1] > 100 or input_value[2] > 100:
-				# 리스트는 2가지 형태로 rgb나 hsv가 가능하니 100이상이 되면 hsv이니, 전부 100이하이면 hsv로 하도록 한다
-				result = input_value
-			else:
-				result = self.color.change_hsl_to_rgb(input_value)
-		return result
+	def check_yy_address(self, input_data="입력필요"):
+		"""
+		결과= ["b", "b"]의 형태로 만들어 주는것
+		"""
+		if input_data == "" or input_data == None:
+			temp = self.read_address_in_selection()
+			result = [temp[1], temp[3]]
+		elif type(input_data) == type("string") or type(input_data) == type(123):
+			temp = self.change_num_to_char(input_data)
+			result = [temp, temp]
+		elif type(input_data) == type([]):
+			if len(input_data) == 2:
+				result = input_data #이부분이 check_address_value와 틀린것이다
+			elif len(input_data) == 4:
+				temp = input_data
+				result = [temp[1], temp[3]]
+		else:
+			temp = self.read_address_in_selection()
+			result = [temp[1], temp[3]]
 
-	def compare_two_value(self, raw_data, req_number, project_name, vendor_name, nal):
-		self.data = list(raw_data)
-		self.data_set = []
-		self.data_set_final = []
-		for self.a in range(0, len(self.data), 2):
-			for self.b in range(len(self.data[1])):
-				if not (self.data[self.a + 1][self.b] == self.data[self.a][self.b]) and self.data[self.a + 1][
-					self.b] != None and self.data[self.a + 1][self.b] != 0:
-					self.data_set.append(self.data[self.a + 1][self.b])
-				else:
-					self.data_set.append(self.data[self.a][self.b])
-			self.data_set.append(req_number)
-			self.data_set.append(project_name)
-			self.data_set.append(vendor_name)
-			self.data_set.append(nal)
-			self.data_set_final.append(self.data_set)
-			self.data_set = []
-		return self.data_set_final
+		new_y1 = self.change_num_to_char(result[0])
+		new_y2 = self.change_num_to_char(result[1])
+
+		return [new_y1, new_y2]
 
 	def close(self):
+		"""
+		열려진 화일을 닫는것
+		"""
+		self.xlbook.Close(SaveChanges=0)
+		del self.xlapp
+
+	def close_workbook(self):
+		"""
+		현재는 close를 시키면 엑셀워크북만이 아니라 엑셀자체도 종료 시킵니다
+		"""
 		self.xlbook.Close(SaveChanges=0)
 		del self.xlapp
 
 	def copy_range(self, sheet_name="", xyxy=""):
+		"""
+		영역의 복사까지만 하는 기능이다
+		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		self.check_address_value(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 		sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2)).Copy()
 
 	def copy_xxline(self, sheet_name="", xyxy=""):
 		"""
-		세로의 값을 복사
+		가로영역을 복사
 		"""
-		self.copy_range(sheet_name, xyxy)
+		sheet_object = self.check_sheet_name(sheet_name)
+		x1, x2 = self.check_xx_address(xyxy)
+		sheet_object.Rows(str(x1)+":"+str(x2)).Copy()
 
 	def copy_yyline(self, sheet_name="", xyxy=""):
-		self.copy_range(sheet_name, xyxy)
+		"""
+		세로영역을 복사
+		"""
+		sheet_object = self.check_sheet_name(sheet_name)
+		y1, y2 = self.check_yy_address(xyxy)
+		sheet_object.Columns(str(y1)+":"+str(y2)).Copy()
 
 	def count_range_samevalue(self, sheet_name="", xyxy=""):
 		"""
+		보관용
+		"""
+		self.count_samevalue_in_range(sheet_name, xyxy)
+
+	def count_samevalue_in_range(self, sheet_name="", xyxy=""):
+		"""
 		 입력값 : 입력값없이 사용가능
 		 선택한 영역의 반복되는 갯수를 구한다
 		 1. 선택한 영역에서 값을 읽어온다
 		 2. 사전으로 읽어온 값을 넣는다
 		 3. 열을 2개를 추가해서 하나는 값을 다른하나는 반복된 숫자를 넣는다
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
-		all_data = self.write_value_in_range("", [x1, y1, x2, y2])
+		all_data = self.read_value_in_range("", [x1, y1, x2, y2])
 		py_dic = {}
 		# 읽어온 값을 하나씩 대입한다
 		for line_data in all_data:
 			for one_data in line_data:
 				# 키가와 값을 확인
 				if one_data in py_dic:
 					py_dic[one_data] = py_dic[one_data] + 1
@@ -772,41 +959,174 @@
 
 	def count_sheet_nos(self):
 		"""
 		시트의 갯수를 돌려준다
 		"""
 		return self.xlbook.Worksheets.Count
 
+	def count_worksheet_all(self):
+		"""
+		출력값 : 시트의 갯수
+		"""
+		result = self.read_worksheet_numbers()
+		return result
+
+	def data_dic_colorindex_to_colorname(self, input_colorindex):
+		"""
+		색이름으로 엑셀 색번호를 돌려주는것
+		"""
+		dic_colorname_colorindex = self.data_set_basic.vars["excel_colorindex_vs_color_name"]
+
+		result = dic_colorname_colorindex[int(input_colorindex)]
+		return result
+
+	def data_dic_colorindex_to_rgbint(self, input_rgbint):
+		"""
+		rgb int값으로 엑셀의 색번호를 돌려주는것
+		"""
+		dic_colorindex_rgbint = self.data_set_basic.vars["excel_colorindex_vs_rgbint"]
+		result = dic_colorindex_rgbint[int(input_rgbint)]
+		return result
+
+	def data_dic_colorindex_to_rgblist(self, rgblist):
+		"""
+		rgb값으로 엑셀의 색번호를 돌려주는것
+		"""
+		basic = self.data_set_basic.vars["excel_rgblist_vs_colorindex"]
+		result = basic[rgblist]
+		return result
+
+	def data_dic_colorname_to_colorindex(self, input_colorindex):
+		"""
+		색번호로 색이름을 돌려주는것
+		"""
+		dic_colorname_colorindex = self.data_set_basic.vars["excel_colorname_vs_colorindex"]
+
+		result = dic_colorname_colorindex[int(input_colorindex)]
+		return result
+
+	def data_dic_line_position(self, input_data=""):
+		"""
+		라인 위치에 대한 자료를 돌려준디
+		"""
+		line_position = self.data_set_basic.vars["excel_line_position"]
+
+		if input_data in line_position.keys():
+			result = line_position[input_data]
+		else:
+			result = [9]
+		return result
+
+	def data_dic_line_style(self, input_data=""):
+		"""
+		라인 스타일에 대한 자료를 돌려준디
+		"""
+		line_style_dic = self.data_set_basic.vars["excel_line_style_dic"]
+
+		if input_data in line_style_dic.keys():
+			result = line_style_dic[input_data]
+		else:
+			result = 1
+		return result
+
+	def data_dic_line_thickness(self, input_data=""):
+		"""
+		라인 두께에 대한 자료를 돌려준디
+		"""
+		line_thickness_dic = self.data_set_basic.vars["excel_line_thickness_dic"]
+
+		if input_data in line_thickness_dic.keys():
+			result = line_thickness_dic[input_data]
+		else:
+			result = 2
+		return result
+
+	def data_dic_rgblist_to_colorindex(self, input_colorindex):
+		"""
+		엑셀의 색번호로 rgb값을 돌려주는것
+		"""
+		dic_colorindex_rgblist = self.data_set_basic.vars["excel_colorindex_vs_rgb_no"]
+
+		result = dic_colorindex_rgblist[int(input_colorindex)]
+		return result
+
+	def delete_all_draw_line_in_range(self, sheet_name="", xyxy=""):
+		"""
+		시트의 모든 라인을 지우는 것
+		"""
+		self.delete_all_line_in_range(sheet_name, xyxy)
+
 	def delete_all_drawing_in_sheet(self, sheet_name=""):
 		"""
 		시트안의 모든 객체를 삭제하는 것
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
-		drawings_no = sheet_object.Shapes.Count
-		if drawings_no > 0:
-			for aa in range(sheet_object.Shapes.Count, 0, -1):
+		drawings_nos = sheet_object.Shapes.Count
+		if drawings_nos > 0:
+			for num in range(sheet_object.Shapes.Count, 0, -1):
 				# Range를 앞에서부터하니 삭제하자마자 번호가 다시 매겨져서, 뒤에서부터 삭제하니 잘된다
-				sheet_object.Shapes(aa).Delete()
-		return drawings_no
+				sheet_object.Shapes(num).Delete()
+		return drawings_nos
 
 	def delete_all_line_in_range(self, sheet_name="", xyxy=""):
 		"""
 		영역의 모든선을 지운다
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
 		for each in [5, 6, 7, 8, 9, 10, 11, 12]:
 			my_range.Borders(each).LineStyle = -4142
 
-	def delete_all_value_in_sheet(self, sheet_name=""):
+	def delete_all_rangename(self):
 		"""
-		시트안의 모든 값을 삭제한다
+		영역이름을 다 삭제한다
 		"""
+		self.delete_rangename_all()
 
+	def delete_all_samevalue_in_range(self, sheet_name="", xyxy=""):
+		"""
+		영역안에서 같은것이 있으면 모두 지우고, 고유한것만 남기는것
+		2개가 같으면 2개모두 지우는 것이다
+		"""
+		temp_dic = {}
+		sheet_object = self.check_sheet_name(sheet_name)
+		x1, y1, x2, y2 = self.check_address_value(xyxy)
+		all_datas = self.read_value_in_range(sheet_name, xyxy)
+
+		#모든 자료의 반복 갯수와 셀주소를 저장한다
+		for x in range(x1, x2 + 1):
+			for y in range(y1, y2+1):
+				value = sheet_object.Cells(x, y).Value
+				if value == None or value == "":
+					pass
+				else:
+					if value in temp_dic.keys():
+						temp_dic[value] = temp_dic[value]["num"] + 1
+						temp_dic[value]["xy"].append([x,y])
+					else:
+						temp_dic[value] = {"num" : 1, "xy":[[x,y]]}
+
+		#1개이상 반복된것을 모두 지우도록 한다
+		for one in temp_dic.keys():
+			if temp_dic[one]["num"] > 1:
+				for xy_address in temp_dic[one]["xy"]:
+					sheet_object.Cells(xy_address[0], xy_address[1]).Value = ""
+
+	def delete_all_shape_in_sheet(self, sheet_name=""):
+		"""
+		시트의 모든 객체를 지우는 것
+		"""
+		self.delete_all_drawing_in_sheet(sheet_name)
+
+	def delete_all_value_in_sheet(self, sheet_name=""):
+		"""
+		시트안의 모든 값만을 삭제
+		시트를 그대로 둬야하는 경우에 사용
+		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		sheet_object.Cells.ClearContents()
 
 	def delete_color_in_range(self, sheet_name="", xyxy=""):
 		"""
 		영역의 색을 지우는 것
 		"""
@@ -815,102 +1135,111 @@
 		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
 		my_range.Interior.Pattern = -4142
 		my_range.Interior.TintAndShade = 0
 		my_range.Interior.PatternTintAndShade = 0
 
 	def delete_continious_samevalue_in_range(self, sheet_name="", xyxy=""):
 		"""
-		아래로 같은 값들을 지울때
+		대상 : 선택한 영역
+		밑으로 같은 값들이 있으면 지우는것
 		"""
+
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
-		for y in range(y2, y1, -1):
-			for x in range(x1, x2 + 1):
+		for y in range(y1, y2+1):
+			for x in range(x2, x1 + 1, -1):
 				base_value = sheet_object.Cells(x, y).Value
-				up_value = str(sheet_object.Cells(x, y - 1).Value)
+				up_value = str(sheet_object.Cells(x-1, y).Value)
 				if base_value == up_value:
 					# self.write_value_in_cell(sheet_name, [x, y], "")
 					sheet_object.Cells(x, y).Value = ""
 
+	def delete_line_in_list2d_by_index(self, input_list2d, no_list):
+		#입력형태 : 2차원리스트, [2,5,7]
+		no_list.sort()
+		no_list.reverse()
+		for one in no_list:
+			for x in range(len(input_list2d)):
+				del input_list2d[x][one]
+		return input_list2d
+
 	def delete_linecolor_in_range(self, sheet_name="", xyxy=""):
+		"""
+		영역안의 라인의 색을 지우는 것
+		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
 		my_range.Interior.Pattern = 0
 		my_range.Interior.PatternTintAndShade = 0
 
 	def delete_link_in_range(self, sheet_name="", xyxy=""):
 		"""
 		영역안의 링크를 삭제하는 것
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
-
 		my_range.Hyperlinks.Delete()
 
 	def delete_memo_in_range(self, sheet_name="", xyxy=""):
 		"""
 		영역안의 메모를 삭제하는 것
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
 		my_range.ClearComments()
 
 	def delete_panthom_rangname(self):
 		"""
-		엑셀의 이름영역중에서 연결이 끊긴것을 삭제하는 것이다
+		이름영역중에서 연결이 끊긴것을 삭제하는 것
 		"""
 		cnt = self.xlapp.Names.Count
 		for num in range(1, cnt + 1):
 			aaa = self.xlapp.Names(num).Name
 			if aaa.find("!") < 0:
 				self.xlapp.Names(aaa).Delete()
 
 	def delete_patial_value_in_range_as_0toN(self, sheet_name="", xyxy="", num="입력필요"):
 		"""
 		선택영역의 값중에서 일부분만 지우는것
+		앞에서부터 N개까지의 글자를 삭제하는것
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 
 		for x in range(x1, x2 + 1):
 			for y in range(y1, y2 + 1):
 
-				cell_value = str(sheet_object.Cells(x, y).Value)
+				cell_value = sheet_object.Cells(x, y).Value
 				if cell_value != "" or cell_value != None or cell_value != None:
 					sheet_object.Cells(x, y).Value = cell_value[int(num):]
 
-	def delete_rangename_by_name(self, range_name):
-		"""
-		rangename을  삭제하는 것
-		"""
-		self.xlapp.Names(range_name).Delete()
-
 	def delete_rangename_all(self):
 		"""
-		rangename을  삭제하는 것
+		모든 rangename을 삭제하는 것
 		"""
 		aaa = self.xlapp.Names
 		for one in aaa:
 			ddd = str(one.Name)
 			if ddd.find("!") < 0:
 				print(one.Name)
 				self.xlapp.Names(aaa).Delete()
 
-	def delete_rangname_panthom(self):
+	def delete_rangename_by_name(self, sheet_name, range_name):
 		"""
-		연결이 끊긴 이름영역을 제거한다
+		입력한 이름을 삭제한다
+		name은 workbook으로 되지만 동일하게 하기위하여 sheet_name을 넣은 것이다
 		"""
-		cnt = self.xlapp.Names.Count
-		for num in range(1, cnt + 1):
-			aaa = self.xlapp.Names(num).Name
-			if aaa.find("!") < 0:
-				self.xlapp.Names(aaa).Delete()
+		result = self.xlbook.Names(range_name).Delete()
+		return result
+
+	def delete_rangname_for_panthom(self):
+		self.delete_panthom_rangname()
 
 	def delete_samevalue_in_range(self, sheet_name="", xyxy=""):
 		"""
 		영역안의 같은 값을 지우는 것이다
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
@@ -923,66 +1252,41 @@
 				else:
 					len_old = len(set_a)
 					set_a.add(value)
 					len_new = len(set_a)
 					if len_old == len_new:
 						sheet_object.Cells(x, y).Value = ""
 
-	def delete_samevalue_in_range_by_many_column_are_same(self, sheet_name="", xyxy="", input_list="입력필요"):
-		sheet_object = self.check_sheet_name(sheet_name)
-		x1, y1, x2, y2 = self.check_address_value(xyxy)
-		base_data_1 = self.write_value_in_range(sheet_name, xyxy)
-		base_data_2 = base_data_1
-		same_num = len(input_list)
-		del_list = []
-		for x in range(x1, x2 + 1):
-			line_data = base_data_1[x]
-			for x_2 in range(x + 1, x2 + 1):
-				count = 0
-				com_one_line = base_data_1[x_2]
-				for one_num in input_list:
-					if line_data[one_num] == com_one_line[one_num]:
-						count = count + 1
-				if count == same_num:
-					del_list.append(x_2)
-					sheet_object.Range(sheet_object.Cells(x1 + x, y1),
-					                   sheet_object.Cells(x1 + x, y2)).ClearContents()
+	def delete_samevalue_in_range_by_many_column_are_same(self, sheet_name="", xyxy=""):
+		self.delete_xxline_value_in_range_by_same_line(sheet_name, xyxy)
 
-	def delete_shape_in_sheet_by_name(self, sheet_name="", shape_name="입력필요"):
+	def delete_shape_by_name(self, sheet_name="", shape_name="입력필요"):
 		"""
 		객체의 이름으로 제거하는것
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		sheet_object.Shapes(shape_name).Delete()
 
 	def delete_sheet(self, sheet_name=""):
+		self.delete_sheet_by_name(sheet_name)
+
+	def delete_sheet_by_name(self, sheet_name=""):
 		"""
 		시트하나 삭제하기
 		"""
 		try:
 			sheet_object = self.check_sheet_name(sheet_name)
 			self.xlapp.DisplayAlerts = False
 			sheet_object.Delete()
 			self.xlapp.DisplayAlerts = True
 		except:
 			pass
 
 	def delete_sheet_name(self, sheet_name):
-		"""
-		셀의 줄바꿈을 설정할때 사용한다
-		만약 status를 false로 하면 줄바꿈이 실행되지 않는다.
-		self.check_sheet_name (sheet_name)
-		"""
-		sheet_object = self.check_sheet_name(sheet_name)
-		ddd = sheet_object.Cells
-		aaa = self.xlapp.Names
-		for one in aaa:
-			ddd = str(one.Name)
-			if ddd.find("!") < 0:
-				print(one.Name)
+		self.delete_sheet_by_name(sheet_name)
 
 	def delete_value_in_cell(self, sheet_name="", xyxy=""):
 		"""
 		셀안의 값을 삭제하는것
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
@@ -994,147 +1298,92 @@
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
 		my_range.ClearContents()
 
 	def delete_value_in_range_between_a_and_b(self, sheet_name="", xyxy="", input_list=["(", ")"]):
-		sheet_object = self.check_sheet_name(sheet_name)
-		x1, y1, x2, y2 = self.check_address_value(xyxy)
-		# re_basic = "\\"+str(input_new[0]) + "[\^" + str(input_new[0]) +"]*\\" + str(input_new[1])
-		input_list[0] = str(input_list[0]).strip()
-		input_list[1] = str(input_list[1]).strip()
-		special_char = ".^$*+?{}[]\|()"
-		# 특수문자는 역슬래시를 붙이도록
-		if input_list[0] in special_char: input_list[0] = "\\" + input_list[0]
-		if input_list[1] in special_char: input_list[1] = "\\" + input_list[1]
-		re_basic = str(input_list[0]) + ".*" + str(input_list[1])
-		# 찾은값을 넣을 y열을 추가한다
-		new_x = int(x2) + 1
-		self.insert_xline(sheet_name, new_x)
-		for y in range(y1, y2 + 1):
-			temp = ""
-			for x in range(x1, x2 + 1):
-				cell_value = str(sheet_object.Cells(x, y).Value)
-				result_list = re.findall(re_basic, cell_value)
-				if result_list == None or result_list == []:
-					pass
-				else:
-					# print("result_list == >", result_list)
-					temp = temp + str(result_list)
-					# 발견된곳에 색을 칠한다
-					self.paint_color_in_cell("", [x, y], "yel++")
-			sheet_object.Cells(y, new_x).Value = temp
+		self.delete_value_in_range_between_specific_letter(sheet_name, xyxy, input_list)
 
 	def delete_value_in_range_between_specific_letter(self, sheet_name="", xyxy="", input_list=["(", ")"]):
 		"""
 		(sheet_name="", yxyx="", input_list=["(",")"])
 		입력형식 : ["(",")"]
 		입력자료의 두사이의 자료를 포함하여 삭제하는것
 		예: abc(def)gh ==>abcgh
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 
-		# re_basic = "\\"+str(input_new[0]) + "[\^" + str(input_new[0]) +"]*\\" + str(input_new[1])
 		input_list[0] = str(input_list[0]).strip()
 		input_list[1] = str(input_list[1]).strip()
+
 		special_char = ".^$*+?{}[]\|()"
 		# 특수문자는 역슬래시를 붙이도록
 		if input_list[0] in special_char: input_list[0] = "\\" + input_list[0]
 		if input_list[1] in special_char: input_list[1] = "\\" + input_list[1]
 		re_basic = str(input_list[0]) + ".*" + str(input_list[1])
+
 		# 찾은값을 넣을 y열을 추가한다
-		new_y = int(y2) + 1
-		self.insert_yline(sheet_name, new_y)
-		for x in range(x1, x2 + 1):
+		new_x = int(x2) + 1
+		self.insert_yline(sheet_name, new_x)
+		for y in range(y1, y2 + 1):
 			temp = ""
-			for y in range(y1, y2 + 1):
-				cell_value = str(sheet_object.Cells(x, y).Value)
-				result_list = re.findall(re_basic, cell_value)
+			for x in range(x1, x2 + 1):
+				cell_value = sheet_object.Cells(x, y).Value
+				print("셀 값", cell_value, re_basic)
+				result_list = re.findall(re_basic, str(cell_value))
+
 				if result_list == None or result_list == []:
 					pass
 				else:
 					temp = temp + str(result_list)
-					# 발견된곳에 색을 칠한다
-					self.paint_color_in_range("", [x, y], "yel++")
-			sheet_object.Cells(x, new_y).Value = temp
+					self.paint_cell_by_scolor("", [x, y], "yel++")
+			sheet_object.Cells(y, new_x).Value = temp
 
 	def delete_value_in_range_by_continious_samevalue(self, sheet_name="", xyxy=""):
-		sheet_object = self.check_sheet_name(sheet_name)
-		x1, y1, x2, y2 = self.check_address_value(xyxy)
-
-		for y in range(y2, y1, -1):
-			for x in range(x1, x2 + 1):
-				base_value = sheet_object.Cells(x, y).Value
-				up_value = sheet_object.Cells(x, y - 1).Value
-				if base_value == up_value:
-					# self.write_value_in_cell(sheet_name, [x, y], "")
-					sheet_object.Cells(x, y).Value = ""
-
-	def delete_value_in_range_by_no(self, sheet_name="", xyxy="", input_no=""):
 		"""
-		선택한 영역에서 각셀마다 왼쪽에서 N번째까지의글자삭제하기
+		영역안에서 연속된 같은 값을 삭제 한다
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
+		print(x1, y1, x2, y2)
+		for y in range(y1, y2 +1):
+			for x in range(x2, x1 - 1, -1):
+				up_value = sheet_object.Cells(x-1, y).Value
+				down_value = sheet_object.Cells(x, y).Value
+				if down_value == up_value:
+					sheet_object.Cells(x, y).Value = ""
 
-		for x in range(x1, x2 + 1):
-			for y in range(y1, y2 + 1):
-				cell_value = str(sheet_object.Cells(x, y).Value)
-				if cell_value == "" or cell_value == None or cell_value == None:
-					pass
-				else:
-					# self.write_value_in_cell(sheet_name, [x, y], cell_value[int(input_no):])
-					sheet_object.Cells(x, y).Value = cell_value[int(input_no):]
+	def delete_value_in_range_by_no(self, sheet_name="", xyxy="", input_no=""):
+		self.delete_patial_value_in_range_as_0toN(sheet_name, xyxy, input_no)
 
-	def delete_value_in_range_by_step(self, sheet_name="", xyxy="", input_list=""):
+	def delete_value_in_range_by_step(self, sheet_name="", xyxy="", step_no=""):
 		"""
 		삭제 : 선택자료중 n번째 가로열의 자료를 값만 삭제하는것
 		일하다보면 3번째 줄만 삭제하고싶은경우가 있다, 이럴때 사용하는 것이다
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 
-		base_data_1 = self.write_value_in_range(sheet_name, xyxy)
-		base_data_2 = base_data_1
-		same_num = len(input_list)
-		del_list = []
-		for x in range(x1, x2 + 1):
-			line_data = base_data_1[x]
-			for x_2 in range(x + 1, x2 + 1):
-				count = 0
-				com_one_line = base_data_1[x_2]
-				for one_num in input_list:
-					if line_data[one_num] == com_one_line[one_num]:
-						count = count + 1
-				if count == same_num:
-					del_list.append(x_2)
-					sheet_object.Range(sheet_object.Cells(x1 + x, y1),
-					                   sheet_object.Cells(x1 + x, y2)).ClearContents()
+		for x in range(x1, x2 + 1):
+			if divmod(x-x1+1, step_no)[1] == 0:
+				sheet_object.Range(sheet_object.Cells(x, y1), sheet_object.Cells(x, y2)).ClearContents()
 
 	def delete_value_in_usedrange(self, sheet_name=""):
 		"""
-		자주사용하는 것 같아서 usedrange의 값을 지우는것을 만들어 보았다
+		자주사용하는 것 같아서 만들어 봄
+		usedrange의 값을 지우는것을 만들어 보았다
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
-		aaa = self.read_usedrange_address(sheet_name)
+		aaa = self.read_address_usedrange(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(aaa)
 		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
 		my_range.ClearContents()
 
-	def delete_rangename(self, sheet_name, range_name):
-		"""
-		입력한 이름을 삭제한다
-		name은 workbook으로 되지만 동일하게 하기위하여 sheet_name을 넣은 것이다
-		"""
-
-		result = self.xlbook.Names(range_name).Delete()
-		return result
-
 	def delete_xline(self, sheet_name="", xx=""):
 		"""
 		선택한영역에서 x줄의 값이 없으면 x줄을 삭제한다
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		new_xx = self.check_xx_address(xx)
 		sheet_object.Rows(str(new_xx[0]) + ':' + str(new_xx[1])).Delete()
@@ -1142,212 +1391,233 @@
 	def delete_xline_in_range_as_empty(self, sheet_name="", xyxy=""):
 		"""
 		선택한영역에서 x줄의 값이 없으면 x줄을 삭제한다
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 
-		for y in range(y2, y1, -1):
-			changed_address = str(y) + ":" + str(y)
+		for x in range(x2, x1, -1):
+			changed_address = str(x) + ":" + str(x)
 			num = self.xlapp.WorksheetFunction.CountA(sheet_object.Range(changed_address))
 			if num == 0:
-				self.delete_xline(sheet_name, y)
+				sheet_object.Rows(changed_address).Delete()
 
-	def delete_xline_in_range_by_samevalue(self, sheet_name="", xyxy="", input_list="입력필요"):
-		sheet_object = self.check_sheet_name(sheet_name)
-		x1, y1, x2, y2 = self.check_address_value(xyxy)
-		base_data_1 = self.read_value_in_range(sheet_name, xyxy)
-		base_data_2 = base_data_1
-		same_num = len(input_list)
-		del_list = []
-		for y in range(y1, y2 + 1):
-			line_data = base_data_1[y]
-			for x_2 in range(x1 + 1, x2 + 1):
-				count = 0
-				com_one_line = base_data_1[x_2]
-				for one_num in input_list:
-					if line_data[one_num] == com_one_line[one_num]:
-						count = count + 1
-				if count == same_num:
-					del_list.append(x_2)
-					sheet_object.Range(sheet_object.Cells(y1 + y, x1),
-					                   sheet_object.Cells(y1 + y, x2)).ClearContents()
+	def delete_xline_in_range_by_samevalue(self, sheet_name="", xyxy=""):
+		self.delete_samevalue_in_range_by_many_column_are_same(sheet_name, xyxy)
 
 	def delete_xline_in_range_by_step(self, sheet_name="", xyxy="", step_no="입력필요"):
+		"""
+		영역안의 자료에서 선택한 가로행을 삭제한다
+		값만 삭제하는것이 아니다
+		위에서부터 삭제가 되게 만든것
+		"""
+
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
-		mok, namuji = divmod(y2 - y1 + 1, int(step_no))
-		end_no = y2 - namuji
-		start_no = y1
-		for y in range(end_no, start_no, -1):
-			if divmod(y, int(step_no))[1] == 0:
-				self.delete_xline(sheet_name, [y, y])
+		del_no = 0 #삭제된 줄수
+		total_no = 1 #천체 라인수
+		for x in range(x1, x2 + 1):
+			if x2 == total_no:
+				break
+			if divmod(total_no, step_no)[1] == 0:
+				current_x = total_no - del_no
+				self.delete_xline(sheet_name, [current_x, current_x])
+				del_no = del_no +1
+			total_no = total_no +1
 
 	def delete_xline_value_in_range_by_step(self, sheet_name="", xyxy="", step_no="입력필요"):
 		"""
 		삭제 : 2 ==> 기존의 2번째 마다 삭제 (1,2,3,4,5,6,7 => 1,3,5,7)
-		삽입 : 2 ==> 2번째에 새로운것 추가 (1,2,3,4,5,6,7 => 1,2,2,3,4,4,5,6,6,7)
 		삭제 : 선택자료중 n번째 세로줄의 자료를 값만 삭제하는것
 		일하다보면 3번째 줄만 삭제하고싶은경우가 있다, 이럴때 사용하는 것
 		"""
+
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 
-		mok, namuji = divmod(y2 - y1 + 1, int(step_no))
-		end_no = y2 - namuji
-		start_no = y1
-
-		for y in range(end_no, start_no, -1):
-			if divmod(y, int(step_no))[1] == 0:
-				self.delete_value_in_range(sheet_name, [y, x1, y, x2])
+		for x in range(x1, x2 + 1):
+			if divmod(x-x1+1, step_no)[1] == 0:
+				sheet_object.Range(sheet_object.Cells(x, y1), sheet_object.Cells(x, y2)).ClearContents()
 
 	def delete_xxline_in_sheet(self, sheet_name, xx):
 		"""
 		가로 한줄삭제하기
 		입력형태는 2, [2,3]의 두가지가 가능하다
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
-		new_xx = self.check_xy_address(xx)
+		new_xx = self.check_xx_address(xx)
 		sheet_object.Rows(str(new_xx[0]) + ':' + str(new_xx[1])).Delete(-4121)
 
-	def delete_yline(self, sheet_name="", yy=""):
+	def delete_xxline_value_in_range_by_same_line(self, sheet_name="", xyxy=""):
 		"""
-		선택한영역에서 x줄의 값이 없으면 x줄을 삭제한다
+		한줄씩 비교를 해서
+		줄의 모든 값이 똑같으면 처음것을 제외하고 다음 자료부터 값만 삭제하는 것이다
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
-		new_yy = self.check_yy_address(yy)
-		sheet_object.Rows(str(new_yy[0]) + ':' + str(new_yy[1])).Delete()
-
-	def delete_yline_in_range_bystep(self, sheet_name="", xyxy="", step_no="입력필요"):
-		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
+		all_values = self.read_value_in_range(sheet_name, xyxy)
 
-		mok, namuji = divmod(y2 - y1 + 1, int(step_no))
-		end_no = y2 - namuji
-		start_no = y1
-		for y in range(end_no, start_no, -1):
-			if divmod(y, int(step_no))[1] == 0:
-				self.delete_yline(sheet_name, [y, y])
+		same_nos = self.get_nos_in_input_list2d_by_same_xline(all_values)
+		for no in same_nos:
+			sheet_object.Range(sheet_object.Cells(no + x1, y1),
+								sheet_object.Cells(no + x1, y2)).ClearContents()
 
-	def delete_yline_value_in_range_bystep(self, sheet_name="", xyxy="", step_no="입력필요"):
-		sheet_object = self.check_sheet_name(sheet_name)
-		x1, y1, x2, y2 = self.check_address_value(xyxy)
-
-		mok, namuji = divmod(y2 - y1 + 1, int(step_no))
-		end_no = y2 - namuji
-		start_no = y1
-		for y in range(end_no, start_no, -1):
-			if divmod(y, int(step_no))[1] == 0:
-				self.delete_value_in_range(sheet_name, [x1, y, x2, y])
-
-	def delete_yyline_in_sheet(self, sheet_name, yy):
+	def delete_yline(self, sheet_name="", yy=""):
 		"""
-		세로 한줄삭제하기
+		선택한영역에서 x줄의 값이 없으면 x줄을 삭제한다
+		여러줄의 라인이 들어오더라도, 한줄만 삭제하는 것이다
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
-		new_yy = self.check_xy_address(yy)
-		sheet_object.Columns(str(new_yy[0]) + ':' + str(new_yy[1])).Delete()
+		y1, y2 = self.check_yy_address(yy)
+		sheet_object.Columns(y1 + ':' + y1).Delete()
 
-	def draw_bottomline_in_range(self, sheet_name="", xyxy="", line_style="", thickness="입력필요", color="입력필요"):
-		sheet_object = self.check_sheet_name(sheet_name)
+	def delete_yline_in_range_by_step(self, sheet_name="", xyxy="", step_no="입력필요"):
+		"""
+		선택한 영역안의 세로줄중에서 선택한 몇번째마다 y라인을 삭제하는것
+		(선택한 영역안에서 3번째 마다의 y라인을 삭제하는것)
+		"""
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
-		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
-
-		rgb_list = self.color.change_scolor_to_rgb(color)
-		my_range.Borders(9).Color = self.color.change_rgb_to_rgbint(rgb_list)
-		my_range.Borders(9).Weight = thickness
-		my_range.Borders(9).LineStyle = line_style
+		del_no = 0 #삭제된 줄수
+		total_no = 1 #천체 라인수
+		for y in range(y1, y2 + 1):
+			if y2 == total_no:
+				break
+			if divmod(total_no, step_no)[1] == 0:
+				current_y = total_no - del_no
+				self.delete_yline(sheet_name, current_y)
+				del_no = del_no +1
+			total_no = total_no +1
 
-	def draw_innerx_line_in_range(self, sheet_name="", xyxy="", line_style="", thickness="입력필요", color="입력필요"):
+	def delete_yline_value_in_range_by_step(self, sheet_name="", xyxy="", step_no="입력필요"):
+		"""
+		선택한 영역안의 세로줄중에서 선택한 몇번째마다 y라인의 값을 삭제하는것
+		(선택한 영역안에서 3번째 마다의 y라인의 값을 삭제하는것)
+		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
-		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
 
-		rgb_list = self.color.change_scolor_to_rgb(color)
-		my_range.Borders(12).Color = self.color.change_rgb_to_rgbint(rgb_list)
-		my_range.Borders(12).Weight = thickness
-		my_range.Borders(12).LineStyle = line_style
+		for y in range(y1, y2 + 1):
+			if divmod(y-y1+1, step_no)[1] == 0:
+				sheet_object.Range(sheet_object.Cells(x1, y), sheet_object.Cells(x2, y)).ClearContents()
 
-	def draw_innery_line_in_range(self, sheet_name="", xyxy="", line_style="", thickness="입력필요", color="입력필요"):
+	def delete_yyline(self, sheet_name="", yy=""):
+		"""
+		선택한영역에서 여러개의 y줄을 삭제한다
+		"""
 		sheet_object = self.check_sheet_name(sheet_name)
-		x1, y1, x2, y2 = self.check_address_value(xyxy)
-		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
+		y1, y2 = self.check_yy_address(yy)
+		sheet_object.Columns(y1 + ':' + y2).Delete()
 
-		rgb_list = self.color.change_scolor_to_rgb(color)
-		my_range.Borders(11).Color = self.color.change_rgb_to_rgbint(rgb_list)
-		my_range.Borders(11).Weight = thickness
-		my_range.Borders(11).LineStyle = line_style
+	def delete_yyline_in_sheet(self, sheet_name="", yy=""):
+		self.delete_yyline(sheet_name, yy)
 
-	def draw_left_line_in_range(self, sheet_name="", xyxy="", line_style="", thickness="입력필요", color="입력필요"):
-		sheet_object = self.check_sheet_name(sheet_name)
-		x1, y1, x2, y2 = self.check_address_value(xyxy)
-		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
+	def draw_bottomline_in_range(self, sheet_name="", xyxy="", line_style="basic", thickness="basic", color="blu"):
+		"""
+		선택영역에서 선을 긋는것, 맨마지막 라인에 선긋기
+		"""
+		self.draw_line_one_in_range(sheet_name, xyxy, line_style, thickness, color, 9)
 
-		rgb_list = self.color.change_scolor_to_rgb(color)
-		my_range.Borders(7).Color = self.color.change_rgb_to_rgbint(rgb_list)
-		my_range.Borders(7).Weight = thickness
-		my_range.Borders(7).LineStyle = line_style
+	def draw_detail_line_in_range(self, **input):
+		"""
+		선택영역에서 선을 긋는것
+		선긋기를 좀더 상세하게 사용할수 있도록 만든것
+		밐의 base_data의 값들을 이용해서 입력하면 된다
+		"""
+		enum_line = self.data_set_basic.vars["enum_line"]
+		base_data = self.data_set_basic.vars["base_cell_data"]
+		# 기본자료에 입력받은값을 update하는것이다
+		sheet_object = self.check_sheet_name("")
+		base_data.update(input)
+		sheet = self.check_sheet_name(base_data["sheet_name"])
+		set_line = sheet_object.Shapes.AddLine(base_data["xyxy"][0], base_data["xyxy"][1], base_data["xyxy"][2], base_data["xyxy"][3])
+		set_line.Select()
+		set_line.Line.ForeColor.RGB = base_data["color"]
+		set_line.Line.DashStyle = enum_line[base_data["line_style"]]
+		set_line.Line.Weight = base_data["thickness"]
+		set_line.Line.Transparency = base_data["transparency"]
+		# 엑셀에서는 Straight Connector 63의 형태로 이름이 자동적으로 붙여진다
+		set_line.Line.BeginArrowheadStyle = enum_line[base_data["head_style"]]
+		set_line.Line.BeginArrowheadLength = enum_line[base_data["head_length"]]
+		set_line.Line.BeginArrowheadWidth = enum_line[base_data["head_width"]]
+		set_line.Line.EndArrowheadStyle = enum_line[base_data["tail_style"]]  # 화살표의 머리의 모양
+		set_line.Line.EndArrowheadLength = enum_line[base_data["tail_length"]]  # 화살표의 길이
+		set_line.Line.EndArrowheadWidth = enum_line[base_data["tail_width"]]  # 화살표의 넓이
+		result = set_line.Name
+		return result
 
-	def draw_line_in_pxyxy_range(self, sheet_name, line_xyxy, rgb_int):
+	def draw_innerx_line_in_range(self, sheet_name="", xyxy="", line_style="basic", thickness="basic", color="blu"):
+		"""	선택영역에서 선을 긋는것, 안쪽에 x라인 선긋기 """
+		self.draw_line_one_in_range(sheet_name, xyxy, line_style, thickness, color, 12)
+
+	def draw_innery_line_in_range(self, sheet_name="", xyxy="", line_style="basic", thickness="basic", color="blu"):
+		"""	선택영역에서 선을 긋는것, 안쪽에 y라인 선긋기 """
+		self.draw_line_one_in_range(sheet_name, xyxy, line_style, thickness, color, 11)
+
+	def draw_left_line_in_range(self, sheet_name="", xyxy="", line_style="basic", thickness="basic", color="blu"):
+		"""	선택영역에서 선을 긋는것, 왼쪽에 선긋기 """
+		self.draw_line_one_in_range(sheet_name, xyxy, line_style, thickness, color, 7)
+
+	def draw_line_in_pxyxy_range(self, sheet_name, line_xyxy, rgb_list):
+		"""
+		선택영역에서 선을 긋는것
+		pixel을 기준으로 선긋기
+		선을 그을때는 위치와 넓이 높이로 긋는데, change_xyxy_to_pxyxy을 사용하면 셀위치를 그렇게 바꾸게 만든다
+		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(line_xyxy)
-
-		sheet_object.Shapes.AddLine(x1, y1, x2, y2).Select()
-		self.xlapp.Selection.ShapeRange.Line.ForeColor.RGB = rgb_int
+		pxyxy = self.change_xyxy_to_pxyxy([x1, y1, x2, y2])
+		print(pxyxy)
+		sheet_object.Shapes.AddLine(pxyxy[0], pxyxy[1], pxyxy[2], pxyxy[3]).Select()
+		self.xlapp.Selection.ShapeRange.Line.ForeColor.RGB = self.color.change_rgb_to_rgbint(rgb_list)
 		self.xlapp.Selection.ShapeRange.Line.Weight = 5
 
-	def draw_line_in_range(self, sheet_name="", xyxy="", input_list=""):
+	def draw_line_in_range(self, sheet_name="", xyxy="", position="", scolor="", line_style="", thickness=""):
 		"""
-		입력예 : [선의위치, 라인스타일, 굵기, 색깔] ==> [7,1,2,1], ["o","","4","bla"]
+		입력예 : [선의위치, 색깔, 라인스타일, 굵기] ==> [7,1,2,1], "", "",""
 		""으로 된것이 기본으로 설정하는 것이다
 		"l": left, "t": top, "b": bottom, "r": right, "h": horizental, "v": vertical, "a": all,"o": outside,"/": "/","\\": "\",
+		""으로 된것이 기본으로 설정하는 것이다
+		color = rgb 값
 		"""
+		line_position = self.data_set_basic.vars["excel_line_position"]
+		line_thickness_dic = self.data_set_basic.vars["excel_line_thickness_dic"]
+		line_style_dic = self.data_set_basic.vars["excel_line_style_dic"]
+
 
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
+
 		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
+		print(scolor)
+		rgb_list = self.color.change_scolor_to_rgb(scolor)
+		colorint = self.color.change_rgb_to_rgbint(rgb_list)
+		aa = []
+		if type(position) == type([]):
+			for one in position:
+				aa.extend(line_position[one])
+		else:
+			aa.extend(line_position[position])
 
-		line_position = {"l": [7], "t": [8], "b": [9], "r": [10], "h": [11], "v": [12], "a": [7, 8, 9, 10, 11, 12],
-		                 "o": [7, 8, 9, 10],
-		                 "/": [6], "\\": [5], "left": [7], "top": [8], "bottom": [9], "right": [10], "inside-h": [11],
-		                 "inside-v": [12],
-		                 "대각선오른쪽": [6], "대각선왼쪽": [5], "왼쪽": [7], "위쪽": [8], "아래쪽": [9], "오른쪽": [10], "안쪽세로": [11],
-		                 "안쪽가로": [12],
-		                 }
-		line_style_dic = {"": 1, "-": -4115, "-.": 4, "-..": 5, ".": -4142, " = ": -4119, "no": -4118, "/.": 13,
-		                  }
-		weight_dic = {"": 2, "4": 1, "5": 2, "6": -4138, "7": 4,
-		              "basic": -4138, "실선": -4138, "매우가는선": 1, "가는선": 2, "굵은선": 4, "진한선": 4,
-		              }
-		rgb_list = self.color.change_scolor_to_rgb(input_list[3])
-		color_int = self.color.change_rgb_to_rgbint(rgb_list)
-		for po_no in line_position[input_list[0]]:
-			my_range.Borders(po_no).Color = color_int
-			my_range.Borders(po_no).Weight = weight_dic[input_list[2]]
-			my_range.Borders(po_no).LineStyle = line_style_dic[input_list[1]]
+		for po_no in aa:
+			my_range.Borders(po_no).Color = colorint
+			my_range.Borders(po_no).Weight = line_thickness_dic[str(thickness)]
+			my_range.Borders(po_no).LineStyle = line_style_dic[line_style]
 
-	def draw_user_style_02(self, sheet_name="", xyxy=""):
+	def draw_line_one_in_range(self, sheet_name="", xyxy="", line_style="basic", thickness="basic", color="blu", line_position = ""):
+		"""
+		선택영역에서 선을 긋는것
+		라인의 위치에 따라서 선을 긋는것이다
+		"""
+		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
-		range_head = [x1, y1, x1, y2]
-		range_body = [x1 + 1, y1, x2 - 1, y2]
-		range_tail = [x2, y1, x2, y2]
-		range_outside = [x1, y1, x2, y2]
-
-		line_list_head = [["o", "", "5", "bla"], ["h", "", "5", "bla"], ]
-		line_list_body = [["v", "", "4", "bla"], ["h", "", "5", "bla"], ]
-		line_list_tail = [["o", "", "5", "bla"], ["h", "", "5", "bla"], ]
-		line_list_outside = [["o", "", "6", "red"], ]
+		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
 
-		for one in line_list_head:
-			self.draw_line_in_range(sheet_name, range_head, one)
-		for one in line_list_body:
-			self.draw_line_in_range(sheet_name, range_body, one)
-		for one in line_list_tail:
-			self.draw_line_in_range(sheet_name, range_tail, one)
-		for one in line_list_outside:
-			self.draw_line_in_range(sheet_name, range_outside, one)
+		rgb_list = self.color.change_scolor_to_rgb(color)
+		my_range.Borders(line_position).Color = self.color.change_rgb_to_rgbint(rgb_list)
+		my_range.Borders(line_position).Weight = self.data_dic_line_thickness(thickness)
+		my_range.Borders(line_position).LineStyle = self.data_dic_line_style(line_style)
 
 	def draw_triangle(self, xyxy, per=100, reverse=1, size=100):
 		"""
 		직각삼각형
 		정삼각형에서 오른쪽이나 왼쪽으로 얼마나 더 간것인지
 		100이나 -100이면 직삼각형이다
 		사각형은 왼쪽위에서 오른쪽 아래로 만들어 진다
@@ -1364,97 +1634,98 @@
 		rm = [int(x1 + height / 2), y1]  # 윗쪽의 중간
 		bm = [x2, int(y1 + width / 2)]  # 윗쪽의 중간
 		center = [int(x1 + width / 2), int(y1 + height / 2)]
 
 		result = [lb, rb, rt]
 		return result
 
-	def draw_detail_line_in_range(self, **input):
-		enum_line = {
-			"msoArrowheadNone": 1, "msoArrowheadTriangle": 2, "msoArrowheadOpen": 3, "msoArrowheadStealth": 4,
-			"msoArrowheadDiamond": 5, "msoArrowheadOval": 6,
-			"": 1, "<": 2, ">o": 3, ">>": 4, ">": 2, "<>": 5, "o": 6,
-			"basic": 1, "none": 1, "triangle": 2, "open": 3, "stealth": 4, "diamond": 5, "oval": 6,
-			"msoArrowheadNarrow": 1, "msoArrowheadWidthMedium": 2, "msoArrowheadWide": 3,
-			"msoArrowheadShort": 1, "msoArrowheadLengthMedium": 2, "msoArrowheadLong": 3,
-			"short": 1, "narrow": 1, "medium": 2, "long": 3, "wide": 3,
-			"-1": 1, "0": 2, "1": 3,
-			"dash": 4, "dashdot": 5, "dashdotdot": 6, "rounddot": 3, "longdash": 7, "longdashdot": 8,
-			"longdashdotdot": 9,
-			"squaredot": 2,
-			"-": 4, "-.": 5, "-..": 6, ".": 3, "--": 7, "--.": 8, "--..": 9, "ㅁ": 2,
-		}
-		base_data = {
-			"sheet_name": "",
-			"xyxy": [100, 100, 0, 0],
-			"color": 10058239,
-			"line_style": "-.",
-			"thickness": 0.5,
-			"transparency": 0,
-			"head_style": ">",
-			"head_length": "0",
-			"head_width": "0",
-			"tail_style": ">",
-			"tail_length": "0",
-			"tail_width": "0",
-		}
-		# 기본자료에 입력받은값을 update하는것이다
-		sheet_object = self.check_sheet_name("")
-		base_data.update(input)
-		sheet = self.check_sheet_name(base_data["sheet_name"])
-		set_line = sheet_object.Shapes.AddLine(base_data["xyxy"][0], base_data["xyxy"][1], base_data["xyxy"][2], base_data["xyxy"][3])
-		set_line.Select()
-		set_line.Line.ForeColor.RGB = base_data["color"]
-		set_line.Line.DashStyle = enum_line[base_data["line_style"]]
-		set_line.Line.Weight = base_data["thickness"]
-		set_line.Line.Transparency = base_data["transparency"]
-		# 엑셀에서는 Straight Connector 63의 형태로 이름이 자동적으로 붙여진다
-		set_line.Line.BeginArrowheadStyle = enum_line[base_data["head_style"]]
-		set_line.Line.BeginArrowheadLength = enum_line[base_data["head_length"]]
-		set_line.Line.BeginArrowheadWidth = enum_line[base_data["head_width"]]
-		set_line.Line.EndArrowheadStyle = enum_line[base_data["tail_style"]]  # 화살표의 머리의 모양
-		set_line.Line.EndArrowheadLength = enum_line[base_data["tail_length"]]  # 화살표의 길이
-		set_line.Line.EndArrowheadWidth = enum_line[base_data["tail_width"]]  # 화살표의 넓이
-		result = set_line.Name
-		return result
+	def draw_user_style_02(self, sheet_name="", xyxy=""):
+		"""
+		선택영역에서 선을 긋는것
+		사용자가 만든 스타일의 선긋기
+		"""
+		x1, y1, x2, y2 = self.check_address_value(xyxy)
+		range_head = [x1, y1, x1, y2]
+		range_body = [x1 + 1, y1, x2 - 1, y2]
+		range_tail = [x2, y1, x2, y2]
+		range_outside = [x1, y1, x2, y2]
+
+		line_list_head = [["o", "bla", "", "5"], ["h", "bla", "", "5"], ]
+		line_list_body = [["v", "bla", "", "4"], ["h", "bla", "", "5"], ]
+		line_list_tail = [["o", "bla", "", "5"], ["h", "bla", "", "5"], ]
+		line_list_outside = [["o", "bla", "", "6"], ]
+
+		for one in line_list_head:
+			self.draw_line_in_range(sheet_name, range_head, one[0], one[1],one[2],one[3])
+		for one in line_list_body:
+			self.draw_line_in_range(sheet_name, range_body, one[0], one[1],one[2],one[3])
+		for one in line_list_tail:
+			self.draw_line_in_range(sheet_name, range_tail, one[0], one[1],one[2],one[3])
+		for one in line_list_outside:
+			self.draw_line_in_range(sheet_name, range_outside, one[0], one[1],one[2],one[3])
 
 	def dump_value_in_range_at_newsheet(self, input_datas):
 		self.add_sheet_new()
 		self.write_value_in_range("", [1, 1], input_datas)
 
 	def excel_fun_ltrim(self, input_data):
 		aaa = self.xlapp.WorksheetFunction.LTrim(input_data)
 		return aaa
 
 	def excel_fun_rtrim(self, input_data):
+		"""
+		엑셀의 함수를 사용해서 값을 바꾸는 것이다
+		"""
 		aaa = self.xlapp.WorksheetFunction.RTrim(input_data)
 		return aaa
 
 	def excel_fun_trim(self, input_data="입력필요"):
+		"""
+		엑셀의 함수를 사용해서 값을 바꾸는 것이다
+		"""
 		aaa = self.xlapp.WorksheetFunction.Trim(input_data)
 		return aaa
 
 	def fill_emptycell_in_range_as_uppercell(self, sheet_name="", xyxy=""):
+		"""
+		빈셀을 위의것으로 채우는 것
+		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
-		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
 		old_data = ""
 		for x in range(x1, x2 + 1):
 			for y in range(y1, y2 + 1):
-				cell_value = str(sheet_object.Cells(x, y).Value)
+				cell_value = sheet_object.Cells(x, y).Value
 				if y == y1:
 					# 만약 자료가 제일 처음이라면
 					old_data = cell_value
 				else:
 					if cell_value == None or cell_value == "":
 						sheet_object.Cells(x, y).Value = old_data
 
 					else:
 						old_data = cell_value
 
+	def find_word_in_range(self, sheet_name="", xyxy="", input_text = ""):
+		"""
+		영역안의 글자를 찾는다
+		"""
+		sheet_object = self.check_sheet_name(sheet_name)
+		x1, y1, x2, y2 = self.check_address_value(xyxy)
+		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
+		first_range = my_range.Find(input_text)
+		temp_range = first_range
+		if first_range != None:
+			while 1:
+				temp_range = my_range.FindNext(temp_range)
+				if temp_range == None or temp_range == first_range.Address:
+					break
+				else:
+					temp_range = temp_range
+
 	def get_activesheet_object(self):
 		sheet_name = self.xlapp.ActiveSheet.Name
 		sheet_object = self.check_sheet_name(sheet_name)
 		return sheet_object
 
 	def get_diagonal_xy(self, xyxy=[5, 9, 12, 21]):
 		"""
@@ -1491,27 +1762,51 @@
 				temp_no = int(x)
 
 				if temp != final_x:
 					temp = final_x
 					result.append([final_x, final_y])
 		return result
 
+	def get_nos_in_input_list2d_by_same_xline(self, input_2dlist =""):
+		"""
+		2dlist의 자료의 형태로 된것중에서
+		위에서 부터 같은것을 삭제 한다
+		0,3,5의 3개가 같은것이라면 제일 앞의 1개는 제외하고 [3,5]를 돌려준다
+		"""
+
+		all_datas = input_2dlist
+		total_len = len(all_datas)
+		same_nos = []
+		for no in range(total_len):
+			if no in same_nos:
+				pass
+			else:
+				one_list = all_datas[no]
+				print(one_list)
+				for num in range(no+1, total_len):
+					if num in same_nos:
+						pass
+					else:
+						if one_list == all_datas[num]:
+							same_nos.append(num)
+		return same_nos
+
 	def get_sheet_object(self, sheet_name=""):
 		if str(sheet_name).lower() == "activesheet" or sheet_name == "":
 			sheet = self.xlapp.ActiveSheet
 		elif sheet_name in self.read_activesheet_name():
 			sheet_object = self.check_sheet_name(sheet_name)
 		else:
-			self.insert_workbook_sheet()
+			self.insert_sheet()
 			old_sheet_name = self.read_activesheet_name()
 			self.change_sheet_name(old_sheet_name, sheet_name)
 			sheet_object = self.check_sheet_name(sheet_name)
 		return sheet_object
 
-	def get_vba_module_name(self, ):
+	def get_vba_module_name_all(self, ):
 		"""
 		현재 열려진 엑셀 화일안의 매크로모듈 이름을 찾아서 돌려주는 것
 		아래에 1,2,3을 쓴것은 모듈의 종류를 여러가지인데, 해당하는 모듈의 종류이며.
 		이것을 하지 않으면 다른 종류의 것들도 돌려쥬기 때문이다
 
 		 xlapp.Close(SaveChanges=False)
 		 xlapp.Quit()
@@ -1520,202 +1815,220 @@
 		result = []
 		for i in self.xlbook.VBProject.VBComponents:
 			if i.type in [1, 2, 3]:
 				result.append(i.Name)
 		return result
 
 	def get_xxline_object(self, sheet_name, xx):
+		"""
+		xx영역을 객체로 돌려주는것
+		"""
 		new_x = self.check_xx_address(xx)
 		sheet_object = self.check_sheet_name(sheet_name)
 		result = sheet_object.Rows(str(new_x[0]) + ':' + str(new_x[1]))
 		return result
 
 	def get_yyline_object(self, sheet_name, yy):
 		"""
-		yy영역을 돌려주는것
+		yy영역을 객체로 돌려주는것
 		"""
 		new_y = self.check_yy_address(yy)
 		sheet_object = self.check_sheet_name(sheet_name)
 		result = sheet_object.Columns(str(new_y[0]) + ':' + str(new_y[1]))
 		return result
 
 	def hide_sheet(self, sheet_name, hide=0):
-		"""
-		시트 숨기기
-		"""
+		""" 시트 숨기기 """
 		sheet_object = self.check_sheet_name(sheet_name)
 		sheet_object.Visible = hide
 
 	def hide_workbook(self):
+		""" 실행되어있는 엑셀을 화면에 보이지 않도록 설정합니다 """
+		self.xlapp.Visible = 0
+
+	def history(self):
 		"""
-		실행되어있는 엑셀을 화면에 보이지 않도록 설정합니다
+		revision에대한 간략한 설명을 넣을 것입니다
 		"""
-		self.xlapp.Visible = 0
+		result = 	"""
+			2023-03-02 : 전반적으로 이름을 수정함
+			2023-05-09 : 이름과 부족한 것을 추가함
+			"""
+		return result
 
-	def input_messagebox_value(self, text_01="Pyofficer"):
+	def input_messagebox_value(self, text_01="halmoney"):
 		"""
 		입력창을 만들어서 입력값을 받는것
 		"""
 		result = self.xlapp.InputBox(text_01)
 		return result
 
 	def insert_image_in_sheet(self, sheet_name, file_path, xywh, link=0, image_in_file=1):
+		self.insert_picture_in_sheet(self, sheet_name, file_path, xywh, link, image_in_file)
+
+	def insert_image_in_xyxy(self, sheet_name, xyxy, file_path):
 		"""
 		image화일을 넣는것
+		선택한 영역안에 자동으로 올수있도록 만들어 보자
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
-		rng = sheet_object.Cells(xywh[0], xywh[1])
-		# sh.Shapes.AddPicture("화일이름", "링크가있나", "문서에저장", "x좌표", "y좌표", "넓이","높이")
-		sheet_object.Shapes.AddPicture(file_path, link, image_in_file, rng.Left, rng.Top, xywh[2], xywh[3])
+		xywh = self.change_xyxy_to_pxyxy(xyxy)
+		sheet_object.Shapes.AddPicture(file_path, 0, 1, xywh[0], xywh[1], xywh[2], xywh[3])
+
+	def insert_line_in_sheet(self, sheet_name, xx):
+		self.insert_xxline(sheet_name, xx)
 
-	def insert_line_in_sheet(self, data, number=1, input_data=[]):
+	def insert_list2d_blank_by_index(self, input_list2d, no_list):
+		#입력형태 : 2차원리스트, [2,5,7]
+		no_list.sort()
+		no_list.reverse()
+		for one in no_list:
+			for x in range(len(input_list2d)):
+				input_list2d[x].insert(int(one), "")
+		return input_list2d
+
+	def insert_picture_in_sheet(self, sheet_name, file_path, xywh, link=0, image_in_file=1):
 		"""
-		리스트에 일정한 간격으로 자료삽입
+		image화일을 넣는것
+		선택한 영역안에 자동으로 올수있도록 만들어 보자
 		"""
-		total_number = len(data)
-		dd = 0
-		for a in range(len(data)):
-			if a % number == 0 and a != 0:
-				if total_number != a:
-					data.insert(dd, input_data)
-					dd = dd + 1
-			dd = dd + 1
-		return data
+		sheet_object = self.check_sheet_name(sheet_name)
+		rng = sheet_object.Cells(xywh[0], xywh[1])
+		# sh.Shapes.AddPicture("화일이름", "링크가있나", "문서에저장", "x좌표", "y좌표", "넓이","높이")
+		sheet_object.Shapes.AddPicture(file_path, link, image_in_file, rng.Left, rng.Top, xywh[2], xywh[3])
 
 	def insert_sheet(self, sheet_name=""):
 		"""
 		시트하나 추가하기
 		"""
-		if sheet_name == "":
-			self.xlbook.Worksheets.Add()
-		else:
-			self.xlbook.Worksheets.Add()
+		self.xlbook.Worksheets.Add()
+		if sheet_name:
 			old_name = self.xlapp.ActiveSheet.Name
 			self.xlbook.Worksheets(old_name).Name = sheet_name
 
-	def insert_sheet_with_name(self, new_name="입력필요"):
+	def insert_sheet_with_name(self, sheet_name="입력필요"):
 		"""
-		 입력값 : 입력값없이 사용가능
-		 시트하나 추가하기
+		시트이름과 함께 시트하나 추가하기
+		함수의 공통적인 이름을 위해서 만든것
 		"""
-		if new_name == "":
-			self.xlbook.Worksheets.Add()
-		else:
-			self.xlbook.Worksheets.Add()
-			old_name = self.xlapp.ActiveSheet.Name
-			self.xlbook.Worksheets(old_name).Name = new_name
+		self.insert_sheet(sheet_name)
 
-	def insert_picture_in_sheet(self, sheet_name):
-		sheet_object = self.check_sheet_name(sheet_name)
-		sheet_object.Shapes.AddPicture("c:\icon_sujun.gif", 0, 1, 541.5, 92.25, 192.75, 180)
-
-	def insert_xline(self, sheet_name, xx):
-		"""
-		가로열을 한줄삽입하기
-		"""
-		self.insert_xxline(sheet_name, xx)
-
-	def insert_xxline(self, sheet_name, xx):
+	def insert_xline(self, sheet_name, x):
 		"""
 		가로열을 한줄삽입하기
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
-		value_list = self.split_value_as_engnum(xx)
-		num_1 = self.change_char_to_num(value_list[0])
-		if len(value_list) == 2:
-			num_2 = self.change_char_to_num(value_list[1])
-		else:
-			num_2 = num_1
-		print("insert_yyline ==> ", num_1, num_2)
-		sheet_object.Range(str(num_1) + ':' + str(num_2)).Insert(-4121)
+		num_r1 = self.change_char_to_num(x)
+		sheet_object.Rows(str(num_r1) + ':' + str(num_r1)).Insert(-4121)
 
-	def insert_xline_in_range_bystep(self, sheet_name="", xyxy="", step_no="입력필요"):
+	def insert_xline_in_range_by_step(self, sheet_name="", xyxy="", step_no="입력필요"):
 		"""
 		n번째마다 열을 추가하는것
 		새로운 가로열을 선택한 영역에 1개씩 추가하는것
 		n번째마다는 n+1번째가 추가되는 것
 		"""
+
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
 
 		for x in range(0, x2 - x1 + 1):
 			mok, namuji = divmod(x, int(step_no))
 			if namuji == step_no - 1:
 				print("===>", x + x1)
 				x_no = self.change_char_to_num(x + x1)
 				print("===>", x_no)
 				sheet_object.Range(str(x_no) + ':' + str(x_no)).Insert(-4121)
 
-	def insert_xxline_in_range(self, sheet_name="", xx="입력필요"):
-		"""
-		가로열을 한줄삽입하기
-		"""
+	def insert_excel_function_in_cell(self, sheet_name, xy, input_fucntion, input_xyxy):
+		result = ""
 		sheet_object = self.check_sheet_name(sheet_name)
-		xx = self.check_xx_address(xx)
-		sheet_object.Rows(str(xx[0]) + ':' + str(xx[1])).Insert()
+		range = self.change_xyxy_to_r1r1(input_xyxy)
+		x1, y1, x2, y2 = self.check_address_value(xy)
+		result = "="+input_fucntion+"("+range+")"
 
-	def insert_yline(self, sheet_name, y):
+		sheet_object.Cells(x1, y1).Value = result
+
+	def insert_xxline(self, sheet_name, xx_list):
 		"""
-		 세로행을 한줄삽입하기
+		가로열을 한줄삽입하기
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
-		num_r1 = self.change_num_to_char(y)
-		sheet_object.Columns(str(num_r1) + ':' + str(num_r1)).Insert(-4121)
+		x1 = self.change_char_to_num(xx_list[0])
+		x2 = self.change_char_to_num(xx_list[1])
+		min_x1 = min(x1, x2)
+		max_x2 = max(x1, x2)
+		for num in range(max_x2+1, min_x1, -1):
+			sheet_object.Range(str(num) + ':' + str(num)).Insert(-4121)
 
-	def split_value_as_engnum(self, data):
+	def insert_xxline_in_range(self, sheet_name="", xx_list="입력필요"):
 		"""
-		 단어중에 나와있는 숫자, 영어를 분리하는기능
+		가로열을 한줄삽입하기
 		"""
-		re_compile = re.compile(r"[a-zA-Z0-9]+")
-		result = re_compile.findall(data)
-
-		new_result = []
-		for dim1_data in result:
-			for dim2_data in dim1_data:
-				new_result.append(dim2_data)
-		return new_result
+		sheet_object = self.check_sheet_name(sheet_name)
+		if type(xx_list) == type([]) and len(xx_list) == 1:
+			x2 = x1 = self.change_char_to_num(xx_list[0])
+		elif type(xx_list) == type([]) and len(xx_list) == 2:
+			x1 = self.change_char_to_num(xx_list[0])
+			x2 = self.change_char_to_num(xx_list[1])
+		else:
+			x2 = x1 = self.change_char_to_num(xx_list)
+		sheet_object.Rows(str(x1) + ':' + str(x2)).Insert()
 
-	def insert_yyline(self, sheet_name, yy):
+	def insert_yline(self, sheet_name, y):
 		"""
 		 세로행을 한줄삽입하기
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
-		value_list = self.split_value_as_engnum(yy)
-
-		num_1 = self.change_num_to_char(value_list[0])
-		if len(value_list) == 2:
-			num_2 = self.change_num_to_char(value_list[1])
-		else:
-			num_2 = num_1
-		sheet_object.Columns(str(num_1) + ':' + str(num_2)).Insert()
+		num_r1 = self.change_num_to_char(y)
+		sheet_object.Columns(str(num_r1) + ':' + str(num_r1)).Insert(-4121)
 
-	def insert_yline_in_range_bystep(self, sheet_name="", xyxy="", step_no="입력필요"):
+	def insert_yline_in_range_by_step(self, sheet_name="", xyxy="", step_no="입력필요"):
 		"""
 		 n번째마다 열을 추가하는것
 		 새로운 가로열을 선택한 영역에 1개씩 추가하는것
 		"""
-		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 
 		# 일정부분으로 추가되는것을 앞에서부터 적용
 		step_no = int(step_no)
 		add_y = 0
 		for no in range(0, y2 - y1 + 1):
 			y = add_y + no
 			if divmod(y, step_no)[1] == step_no - 1:
-				self.insert_yyline_in_range(sheet_name, y + y1)
+				self.insert_yyline(sheet_name, y + y1)
 				add_y = add_y + 1
 
+	def insert_yyline(self, sheet_name, yy_list):
+		"""
+		 세로행을 한줄삽입하기
+		"""
+		sheet_object = self.check_sheet_name(sheet_name)
+		if type(yy_list) == type([]) and len(yy_list) == 1:
+			x2 = x1 = self.change_num_to_char(yy_list[0])
+		elif type(yy_list) == type([]) and len(yy_list) == 2:
+			x1 = self.change_num_to_char(yy_list[0])
+			x2 = self.change_num_to_char(yy_list[1])
+		else:
+			x2 = x1 = self.change_num_to_char(yy_list)
+		sheet_object.Columns(str(x1) + ':' + str(x2)).Insert()
+
 	def insert_yyline_in_range(self, sheet_name="", yy="입력필요"):
 		"""
 		 가로열을 한줄삽입하기
 		"""
 		self.insert_yyline(sheet_name, yy)
 
+	def intersect_address_and_inputdata(self, xyxy="", input_datas="입력필요"):
+		"""
+		이름을 좀더 사용하기 쉽도록 만든것
+		"""
+		result = self.check_address_with_datas(xyxy, input_datas)
+		return result
+
 	def intersect_range1_range2(self, rng1="입력필요", rng2="입력필요"):
 		"""
 		두개의 영역에서 교차하는 구간을 돌려준다
 		만약 교차하는게 없으면 ""을 돌려준다
 		"""
 		range_1 = self.check_address_value(rng1)
 		range_2 = self.check_address_value(rng2)
@@ -1756,570 +2069,583 @@
 	def is_empty_yline(self, sheet_name, no):
 		"""
 		열전체가 빈 것인지 확인해서 돌려준다
 		현재의 기능은 한줄만 가능하도록 하였다
 		다음엔 영역이 가능하도록 하여야 겠다
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
-		result = self.xlapp.WorksheetFunction.CountA(sheet_object.Rows(no).EntireColumn)
+		result = self.xlapp.WorksheetFunction.CountA(sheet_object.Columns(no).EntireColumn)
 		return result
 
 	def lock_sheet(self, sheet_name="", password="1234"):
 		sheet_object = self.check_sheet_name(sheet_name)
 		sheet_object.protect(password)
 
+	def make_vba_module(self, vba_code, macro_name):
+		"""
+		텍스트로 만든 매크로 코드를 실행하는 코드이다
+		"""
+		new_vba_code = "Sub " + macro_name + "()" + vba_code + "End Sub"
+		mod = self.xlbook.VBProject.VBComponents.Add(1)
+		mod.CodeModule.AddFromString(new_vba_code)
+
 	def make_y_value(self, input_data):
-		result = []
-		if len(input_data) > 0:
-			if type(input_data[0]) != type([]):
-				for one in input_data:
-					result.append([one, ])
+		#1차원리스트를 2차원으로 만들면, 세로입력을 가로입력으로 바꾸는 것이다
+		result = self.change_list1d_to_list2d(input_data)
 		return result
 
-	def making_tag(self, ):
-		import pcell
-		excel = pcell.pcell('activeworkbook')
-		all_data = self.write_value_in_range("Sheet1", [1, 1, 90, 15])
-		for no_1 in range(len(all_data)):
-			x = int((no_1 + 1) / 5)
-			y = (no_1 + 1) - x * 5
-			for no_2 in range(15):
-				self.write_value_in_cell("Tag", [x * 20 + no_2 + 4, y * 3 + 3], all_data[no_1][no_2])
+	def manual(self):
+		#간략한 이 모듈에 대한 설명입니다
+		result = 	"""
+			"""
+		return result
 
-	def move_bottom_in_range(self, sheet_name="", xyxy=""):
+	def merge_top_2_xlines_in_range(self, sheet_name="", xyxy=""):  # 셀들을 합하는 것이다
 		"""
-		선택한 위치에서 끝부분으로 이동하는것
-		xlDown: - 4121,xlToLeft : - 4159, xlToRight: - 4161, xlUp : - 4162
+		선택 영역중 바로 위의것과 아랫것만 병합하는것
+		제일위의 2줄만 세로씩 병합하는 것이다
+		가로줄 갯수만큰 병합하는것
+		위와 아래에 값이 있으면 알람이 뜰것이다
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
-		sheet_object.Cells(x1, y1).End(- 4121).Select()
-
-	def move_cell_to_another_sheet(self, sheet_list="입력필요", xy_list="입력필요"):
-		sheet1 = self.check_sheet_name(sheet_list[0])
-		sheet2 = self.check_sheet_name(sheet_list[1])
-		range_old = sheet1.Cells(xy_list[0][0], xy_list[0][1])
-		range_new = sheet2.Cells(xy_list[1][0], xy_list[1][1])
-		range_old.Select()
-		range_old.Cut()
-		range_new.Select()
-		range_new.Paste()
+		if y1 == y2:
+			pass
+		else:
+			for y in range(y1, y2+1):
+				sheet_object.Range(sheet_object.Cells(x1, y), sheet_object.Cells(x1+1, y)).Merge(0)
 
-	def move_degree_distance(self, degree="입력필요", distance="입력필요"):
+	def merge_top_2_ylines_in_range(self, sheet_name="", xyxy=""):  # 셀들을 합하는 것이다
 		"""
-		move_degree_distance( degree="입력필요", distance="입력필요")
-		현재 위치 x,y에서 30도로 20만큼 떨어진 거리의 위치를 돌려주는 것
+		선택 영역중 바로 위의것과 아랫것만 병합하는것
+		제일위의 2줄만 가로씩 병합하는 것이다
+		세로줄 갯수만큰 병합하는것
+		위와 아래에 값이 있으면 알람이 뜰것이다
 		"""
-		degree = degree * 3.141592 / 180
-		y = distance * math.cos(degree)
-		x = distance * math.sin(degree)
-		return [x, y]
+		sheet_object = self.check_sheet_name(sheet_name)
+		x1, y1, x2, y2 = self.check_address_value(xyxy)
+		if x1 == x2:
+			pass
+		else:
+			for x in range(x1, x2+1):
+				sheet_object.Range(sheet_object.Cells(x, y1), sheet_object.Cells(x, y1+1)).Merge(0)
 
-	def move_activecell_to_leftend_in_range(self, sheet_name="", xyxy=""):
+	def move_activecell_in_range_to_leftend(self, sheet_name="", xyxy=""):
 		"""
 		입력값 : 입력값없이 사용가능
 		선택한 위치에서 끝부분으로 이동하는것
 		xlDown : - 4121, xlToLeft : - 4159, xlToRight : - 4161, xlUp : - 4162
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
-		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
-		sheet_object.Cells(x1, y1).End(- 4159).Select()
+		sheet_object.Cells(x1, y1).Select()
 
-	def move_activecell_to_rightend_in_range(self, sheet_name="", xyxy=""):
+	def move_activecell_in_range_to_rightend(self, sheet_name="", xyxy=""):
 		"""
 		선택한 위치에서 끝부분으로 이동하는것
 		xlDown: - 4121,xlToLeft : - 4159, xlToRight: - 4161, xlUp : - 4162
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
-		my_range.End(- 4161).Select()
+		sheet_object.Cells(x1, y2).Select()
 
-	def move_activecell_to_top_in_range(self, sheet_name="", xyxy=""):
-		sheet_object = self.check_sheet_name(sheet_name)
+	def move_activecell_in_range_to_top(self, sheet_name="", xyxy=""):
 		"""
 		선택한 위치에서 끝부분으로 이동하는것
 		xlDown: - 4121,xlToLeft : - 4159, xlToRight: - 4161, xlUp : - 4162
 		"""
+		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
-		my_range.End(- 4162).Select()
+		sheet_object.Cells(x1, y1).Select()
 		return "ok"
 
+	def move_bottom_in_range(self, sheet_name="", xyxy=""):
+		"""
+		선택한 위치에서 제일왼쪽, 제일아래로 이동
+		xlDown: - 4121,xlToLeft : - 4159, xlToRight: - 4161, xlUp : - 4162
+		"""
+		sheet_object = self.check_sheet_name(sheet_name)
+		x1, y1, x2, y2 = self.check_address_value(xyxy)
+		sheet_object.Cells(x1, y2).Select()
+
+	def move_cell_to_another_sheet(self, sheet_list="입력필요", xy_list="입력필요"):
+		"""
+		다른시트로 값1개 옮기기
+		입력형태 : [시트이름1, 시트이름2], [[2,3]. [4,5]]
+		"""
+		sheet_object_1 = self.check_sheet_name(sheet_list[0])
+		x1, y1 = xy_list[0]
+		sheet_object_1.Cells(x1, y1).Cut()
+
+		sheet_object_2 = self.check_sheet_name(sheet_list[1])
+		x2, y2 = xy_list[1]
+		sheet_object_2.Cells(x2, y2).Insert()
+
+	def move_degree_distance(self, degree="입력필요", distance="입력필요"):
+		"""
+		move_degree_distance( degree="입력필요", distance="입력필요")
+		현재 위치 x,y에서 30도로 20만큼 떨어진 거리의 위치를 돌려주는 것
+		"""
+		degree = degree * 3.141592 / 180
+		y = distance * math.cos(degree)
+		x = distance * math.sin(degree)
+		return [x, y]
+
+	def move_list2d_by_index(self, input_list2d, input_no_list):
+		#입력형태 : 2차원리스트, [[옮길것, 옮기고싶은자리].....]
+
+		ori_no_dic = {}
+		for one in range(len(input_list2d[0])):
+			ori_no_dic[one] = one
+		for before, after in input_no_list:
+			new_before = ori_no_dic[before]
+			new_after = ori_no_dic[after]
+
+			for no in range(len(input_list2d)):
+				if new_before < new_after:
+					new_after = after -1
+				value = input_list2d[no][new_before]
+				del input_list2d[no][new_before]
+				input_list2d[no].insert(int(new_after), value)
+		return input_list2d
+
+	def move_list2d_by_index_old(self, input_list2d, input_no_list):
+		#입력형태 : 2차원리스트, [[옮길것, 옮기고싶은자리].....]
+		input_no_list.sort()
+		input_no_list.reverse()
+		for before, after in input_no_list:
+			for no in range(len(input_list2d)):
+				if before < after:
+					after = after -1
+				value = input_list2d[no][before]
+				del input_list2d[no][before]
+				input_list2d[no].insert(int(after), value)
+		return input_list2d
+
 	def move_value_in_range_to_left_except_emptycell(self, sheet_name="", xyxy=""):
 		"""
-		선택한 영역에서 세로의 값중에서 빈셀을 만나면, 아래의 값중 있는것을 위로 올리기
+		x열을 기준으로 값이 없는것은 왼쪽으로 옮기기
 		전체영역의 값을 읽어오고, 하나씩 다시 쓴다
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
-		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
 		value_2d = self.read_value_in_range(sheet_name, xyxy)
 		self.delete_value_in_range(sheet_name, xyxy)
 		for x in range(0, x2 - x1 + 1):
 			new_y = 0
 			for y in range(0, y2 - y1 + 1):
 				value = value_2d[x][y]
 				if value == "" or value == None:
 					pass
 				else:
 					sheet_object.Cells(x + x1, new_y + y1).Value = value
 					new_y = new_y + 1
 
-	def move_xxline_to_another_sheet(self, sheet_list="입력필요", xx_list="입력필요"):
-		sheet1 = self.check_sheet_name(sheet_list[0])
-		sheet2 = self.check_sheet_name(sheet_list[1])
-		xx0_1, xx0_2 = self.check_xy_address(xx_list[0])
-		xx1_1, xx1_2 = self.check_xy_address(xx_list[1])
-		xx0_1 = self.change_char_to_num(xx0_1)
-		xx0_2 = self.change_char_to_num(xx0_2)
-		xx1_1 = self.change_char_to_num(xx1_1)
-		xx1_2 = self.change_char_to_num(xx1_2)
-		sheet1.Select()
-		sheet1.Columns(str(xx0_1) + ':' + str(xx0_2)).Select()
-		sheet1.Columns(str(xx0_1) + ':' + str(xx0_2)).Copy()
-		sheet2.Select()
-		sheet2.Columns(str(xx1_1) + ':' + str(xx1_2)).Select()
-		sheet2.Columns(str(xx1_1) + ':' + str(xx1_2)).Insert()
-		if sheet1 == sheet2:
-			if xx0_1 <= xx1_1:
-				sheet1.Columns(str(xx0_1) + ':' + str(xx0_2)).Delete()
-			else:
-				new_xx0_1 = self.change_num_to_char(xx0_1 + xx1_2 - xx1_1)
-				new_xx0_2 = self.change_num_to_char(xx0_2 + xx1_2 - xx1_1)
-				sheet1.Columns(str(new_xx0_1) + ':' + str(new_xx0_2)).Delete()
-		else:
-			sheet1.Columns(str(xx0_1) + ':' + str(xx0_2)).Delete()
-
-	def move_yyline(self, sheet_list="입력필요", yy_list="입력필요"):
-		range_1 = self.select_range(sheet_list[0], yy_list[0])
-		range_1.Select()
-		range_1.Cut()
-
-		range_2 = self.select_range(sheet_list[1], yy_list[1])
-		range_2.Select()
-		range_2.Insert()
+	def move_xline_value_to_multi_lines(self, input_xyxy, repeat_no, start_xy):
+		"""
+		x라인의 가로 한줄의 자료를 여반복갯수에 따라서 시작점에서부터 아래로 복사하는것
+		입력자료 :  1줄의 영역, 반복하는 갯수, 자료가 옮겨갈 시작주소
+		"""
+		all_data_set = self.read_value_in_range("", input_xyxy)
+		for no in range(len(all_data_set[0])):
+			mok, namuji = divmod(no, repeat_no)
+			new_x = mok + start_xy[0]
+			new_y = namuji + start_xy[1]
+			self.write_value_in_cell("", [new_x, new_y], all_data_set[0][no])
 
-	def move_yyline_to_another_sheet(self, sheet_name_list, yy_list):
+	def move_xxline_to_another_sheet(self, sheet_list="입력필요", xx_list="입력필요"):
 		"""
-		세로의 값을 이동시킵니다
+		다른 시트로 이동시키기 위해서는 다른 시트를 활성화 시켜야 한다
 		"""
-		sheet1 = self.check_sheet_name(sheet_name_list[0])
-		sheet2 = self.check_sheet_name(sheet_name_list[1])
-		yy0_1, yy0_2 = self.check_xy_address(yy_list[0])
-		yy1_1, yy1_2 = self.check_xy_address(yy_list[1])
-		yy0_1 = self.change_num_to_char(yy0_1)
-		yy0_2 = self.change_num_to_char(yy0_2)
-		yy1_1 = self.change_num_to_char(yy1_1)
-		yy1_2 = self.change_num_to_char(yy1_2)
-		sheet1.Select()
-		sheet1.Columns(str(yy0_1) + ':' + str(yy0_2)).Select()
-		sheet1.Columns(str(yy0_1) + ':' + str(yy0_2)).Cut()
-		sheet2.Select()
-		sheet2.Columns(str(yy1_1) + ':' + str(yy1_2)).Select()
-		sheet2.Columns(str(yy1_1) + ':' + str(yy1_2)).Insert()
+		sheet_object_1 = self.check_sheet_name(sheet_list[0])
+		x1, x2 = self.check_xx_address(xx_list[0])
+		sheet_object_1.Rows(str(x1) + ':' + str(x2)).Cut()
 
-	def merge_eachline_in_range(self, sheet_name="", xyxy=""):  # 셀들을 합하는 것이다
-		sheet_object = self.check_sheet_name(sheet_name)
-		x1, y1, x2, y2 = self.check_address_value(xyxy)
-		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
+		sheet_object_2 = self.check_sheet_name(sheet_list[1])
+		self.select_sheet(sheet_list[1])
+		x21, x22 = self.check_xx_address(xx_list[1])
+		sheet_object_2.Rows(str(x21) + ':' + str(x22)).Insert()
 
-		if y1 == y2:
-			my_range.Merge(0)
-		else:
-			for a in range(y2 - y1 + 1):
-				sheet_object.Range(sheet_object.Cells(y1 + a, x1), sheet_object.Cells(y1 + a, x2)).Merge(0)
+	def move_yline_value_to_multi_lines(self, input_xyxy, repeat_no, start_xy):
+		"""
+		y라인의 가로 한줄의 자료를 여반복갯수에 따라서 시작점에서부터 아래로 복사하는것
+		입력자료 :  1줄의 영역, 반복하는 갯수, 자료가 옮겨갈 시작주소
+		"""
+		all_data_set = self.read_value_in_range("", input_xyxy)
+		for no in range(len(all_data_set)):
+			mok, namuji = divmod(no, repeat_no)
+			new_x = mok + start_xy[0]
+			new_y = namuji + start_xy[1]
+			self.write_value_in_cell("", [new_x, new_y], all_data_set[no][0])
+
+	def move_yyline(self, sheet_name="", yy_list="입력필요"):
+		self.move_yyline_in_sheet(sheet_name, yy_list)
 
-	def move_rangevalue_linevalue(self, sheet_name="", xyxy=""):
+	def move_yyline_in_sheet(self, sheet_name="", yy_list="입력필요"):
+		"""
+		같은 시트안에서 y라인을 이동시키는것
+		"""
 		sheet_object = self.check_sheet_name(sheet_name)
-		x1, y1, x2, y2 = self.check_address_value(xyxy)
-		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
+		y1, y2 = self.check_yy_address(yy_list[0])
+		sheet_object.Columns(y1 + ':' + y2).Cut()
 
-		output_list = self.read_value(sheet_name, xyxy)
-		make_one_list = self.yt.change_list1d_to_list2d(output_list)
-		self.insert_cols(sheet_name, x2 + 1)
-		self.write_value_from_top_to_down(sheet_name, [y1, x2 + 1], make_one_list)
-
-	def move_compare_2sheets(self):
-		"""
-		전체가 빈 가로열 삭제
-		두개의 시트에서 기준시트와 똑같은 열로 다른 시트를 옮기는것이름으로
-		1. 현재의 시트 이름을 알아온다
-		2. 옮길 시트이름을 얻는다
-		3. 기준시트의 사용된영역중 첫번째 열의 모든 내용을 읽어온다
-		4. 옮길시트의 사용된영역중 첫번째 열의 모든 내용을 읽어온다
-		5. 두개를 비교해서 몇번째로 이동을 할것인지 새로운 기준시트의 첫번째 열의 모든 내용을 읽어와서 하나씩 비교를 한다
-		"""
-
-		sheet_name_1 = self.read_activesheet_name()
-		sheet_name_2 = self.read_inputbox_value()
-		var_1 = self.read_usedrange_address(sheet_name_1)[2]
-		var_2 = self.read_usedrange_address(sheet_name_2)[2]
-		sheet_1_end_num = self.change_address_to_xyxy(var_1)[1][2]
-		sheet_2_end_num = self.change_address_to_xyxy(var_1)[1][2]
-		for x1 in range(1, sheet_1_end_num + 1):
-			var_3 = self.read_value_in_cell(sheet_name_1, [1, x1])
-			var_5 = 0
-			for x2 in range(1, sheet_2_end_num):
-				var_4 = self.read_value_in_cell(sheet_name_2, [1, x2])
-				if var_3 == var_4 and var_5 == 0:
-					self.insert_xline(sheet_name_2, x1)
-					self.copy_range(sheet_name_2, sheet_name_2, x2 + 1, x1)
-					self.delete_xline(sheet_name_2, x2 + 1)
-					var_5 = 1
-			if var_5 == 0:
-				self.insert_xline(sheet_name_2, x1)
-				sheet_2_end_num = sheet_2_end_num + 1
-
-	def move_arrange_two_sheet_y_02(self, sheet_name="", xyxy=""):
-		sheet_object = self.check_sheet_name(sheet_name)
-		x1, y1, x2, y2 = self.check_address_value(xyxy)
-		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
-		input_list = []
-		# 기준시트와 옮길시트의 이름을 갖고온다
-		input_data = self.input_messagebox_value("Please input specific char : ex) sheet_a, sheet_b")
-		sheet_names = input_data.split(",")
-		# sheet_names = ["aaa", "bbb"]
-		# 사용한 범위를 갖고온다
-		range_1 = self.read_usedrange_address(sheet_names[0])
-		range_2 = self.read_usedrange_address(sheet_names[1])
-		no_title2 = range_2[2]
-		# 기준 시트의 제목을 읽어와서 저장한다
-		title_1 = self.write_value_in_range(sheet_names[0], [1, range_1[1], 1, range_1[3]])
-		title_1_list = []
-		for no in range(1, len(title_1[0]) + 1):
-			title_1_list.append([no, title_1[0][no - 1]])
-		# 하나씩 옮길시트의 값을 읽어와서 비교한후 맞게 정렬한다
-		for y1 in range(len(title_1_list)):
-			found = 0
-			basic_title = title_1_list[y1][1]
-			# print("기준자료 == >", basic_title)
-			# 기준자료의 제목이 비어잇으면 새로이 한칸을 추가한다
-			if basic_title == None or basic_title == "":
-				self.insert_yyline_in_range(sheet_names[1], y1 + 1)
-				no_title2 = no_title2 + 1
-			else:
-				# 만약 기준시트의 제목보다 더 넘어가면 그냥 넘긴다
-				if y1 > no_title2:
-					pass
-				else:
-					for y2 in range(y1, no_title2 + 1):
-						move_title = self.read_value_in_cell(sheet_names[1], [1, y2 + 1])
-						if found == 0 and move_title == basic_title:
-							# print("발견자료 == >", move_title)
-							found = 1
-							if y1 == y2:
-								pass
-							else:
-								self.move_yyline(sheet_names[1], sheet_names[1], y2 + 1, y1 + 1)
-					if found == 0:
-						# 빈칸을 하나 넣는다
-						self.insert_yline(sheet_names[1], y1 + 1)
+		y1_new, y2_new = self.check_yy_address(yy_list[1])
+		sheet_object.Columns(y1_new + ':' + y2_new).Insert()
 
-	def set_cell_color(self, sheet_name, xy, input_color="입력필요"):
-		self.paint_color_in_cell(sheet_name, xy, input_color)
+	def move_yyline_to_another_sheet(self, sheet_name_list, yy_list):
+		"""
+		세로의 값을 이동시킵니다
+		"""
+		sheet_object_1 = self.check_sheet_name(sheet_name_list[0])
+		y1, y2 = self.check_yy_address(yy_list[0])
+		sheet_object_1.Columns(y1 + ':' + y2).Cut()
+
+		sheet_object_2 = self.check_sheet_name(sheet_name_list[1])
+		y1_new, y2_new = self.check_yy_address(yy_list[1])
+		sheet_object_2.Columns(y1_new + ':' + y2_new).Insert()
 
-	def paint_color_in_cell(self, sheet_name, xy, input_color="입력필요"):
+	def paint_cell_by_excel_colorno(self, sheet_name, xy, excel_color_no="입력필요"):
 		"""
 		paint_color(sheet_name, xyxy, input_data="입력필요")
 		선택 셀에 색깔을 넣는다
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		self.check_address_value(xy)
 
-		rgbvalue = self.color.change_scolor_to_rgb(input_color)
+		rgbvalue = self.data_set_basic.vars["rgb_56_for_excel"][excel_color_no]
+
 		rgb_to_int = (int(rgbvalue[2])) * (256 ** 2) + (int(rgbvalue[1])) * 256 + int(rgbvalue[0])
 		sheet_object.Cells(xy[0], xy[1]).Interior.Color = int(rgb_to_int)
 
-	def paint_rgbcolor_in_cell(self, sheet_name, xy, input_color="입력필요"):
+	def paint_cell_by_rgb(self, sheet_name, xy, input_color="입력필요"):
 		"""
 		paint_color(sheet_name, xyxy, input_data="입력필요")
 		선택 셀에 색깔을 넣는다
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		self.check_address_value(xy)
+		rgb_value = self.check_inputcolor_rgb(input_color)
 
-		rgb_to_int = (int(input_color[2])) * (256 ** 2) + (int(input_color[1])) * 256 + int(input_color[0])
+		rgb_to_int = self.color.change_rgb_to_rgbint(rgb_value)
 		sheet_object.Cells(xy[0], xy[1]).Interior.Color = int(rgb_to_int)
 
-	def paint_color_in_cell_as_emptycell(self, sheet_name="", xyxy=""):
+	def paint_cell_by_scolor(self, sheet_name, xy, input_color="입력필요"):
 		"""
-		빈셀의 갯수를 계산
+		paint_color(sheet_name, xyxy, input_data="입력필요")
+		선택 셀에 색깔을 넣는다
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
-		x1, y1, x2, y2 = self.check_address_value(xyxy)
-		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
-		temp_result = 0
-		for x in range(x1, x2 + 1):
-			for y in range(y1, y2 + 1):
-				cell_value = sheet_object.Cells(x, y).Value
-				if cell_value == None:
-					self.paint_color_in_cell(sheet_name, [x, y], 16)
-					temp_result = temp_result + 1
-		return temp_result
+		self.check_address_value(xy)
 
-	def paint_color_in_sheet_tab(self, sheet_name, input_color="입력필요"):
+		rgbvalue = self.color.change_scolor_to_rgb(input_color)
+		rgb_to_int = (int(rgbvalue[2])) * (256 ** 2) + (int(rgbvalue[1])) * 256 + int(rgbvalue[0])
+		sheet_object.Cells(xy[0], xy[1]).Interior.Color = int(rgb_to_int)
+
+	def paint_cell_in_range_by_specific_text(self, sheet_name="", xyxy="", input_text="입력필요", input_color="입력필요"):
 		"""
-		시트탭의색을 넣는것
+		영역안에 입력받은 글자와 같은것이 있으면 색칠하는것
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
-		rgbvalue = self.color.change_scolor_to_rgb(input_color)
-		rgb_to_int = (int(rgbvalue[2])) * (256 ** 2) + (int(rgbvalue[1])) * 256 + int(rgbvalue[0])
-		sheet_object.Tab.Color = rgb_to_int
+		x1, y1, x2, y2 = self.check_address_value(xyxy)
+
+		for x in range(x1, x2 + 1):
+			for y in range(y1, y2 + 1):
+				value = sheet_object.Cells(x, y).Value
+				if input_text in value:
+					self.paint_cell_by_scolor(sheet_name, [x,y], input_color)
 
 	def paint_color_in_range(self, sheet_name, xyxy, input_color="입력필요"):
 		"""
 		paint_color(sheet_name, xyxy, input_data="입력필요")
-		선택 셀에 색깔을 넣는다
+		선택 영역에 색깔을 넣는다
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
 
 		rgbvalue = self.color.change_scolor_to_rgb(input_color)
 		rgb_to_int = (int(rgbvalue[2])) * (256 ** 2) + (int(rgbvalue[1])) * 256 + int(rgbvalue[0])
 		my_range.Interior.Color = rgb_to_int
 
-	def paint_color_in_range_as_samevalue_by_excelcolorno(self, sheet_name="", xyxy="", excelcolorno=4):
-		sheet_object = self.check_sheet_name(sheet_name)
-		x1, y1, x2, y2 = self.check_address_value(xyxy)
-		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
-		set_a = set([])
-		for x in range(x1, x2 + 1):
-			for y in range(y1, y2 + 1):
-				value = str(sheet_object.Cells(x, y).Value)
-				if value == "" or value == None:
-					pass
-				else:
-					len_old = len(set_a)
-					set_a.add(value)
-					len_new = len(set_a)
-					if len_old == len_new:
-						self.paint_color_in_cell(sheet_name, [x, y], excelcolorno)
-
 	def paint_color_in_range_bywords(self, sheet_name="", xyxy=""):
+		"""
+		입력값을 받는데
+		영역안에 입력받은 글자가 있으면 색칠하는것
+		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 
 		bbb = self.input_messagebox_value("Please input text : in, to, his, with")
 		basic_list = []
 		for one_data in bbb.split(","):
 			basic_list.append(one_data.strip())
 		total_no = len(basic_list)
 		for x in range(x1, x2 + 1):
 			for y in range(y1, y2 + 1):
-				cell_value = str(sheet_object.Cells(x, y).Value)
+				cell_value = sheet_object.Cells(x, y).Value
 				temp_int = 0
 				for one_word in basic_list:
-					if re.match('(.*)' + one_word + '(.*)', cell_value):
+					if re.match('(.*)' + one_word + '(.*)', str(cell_value)):
 						temp_int = temp_int + 1
 				if temp_int == total_no:
-					self.paint_color_in_range(sheet_name, [x, y], 4)
+					self.paint_color_in_range(sheet_name, [x, y], "yel")
 
-	def paint_color_in_range_in_maxvalue_in_each_xline(self, sheet_name="", xyxy=""):
+	def paint_font_in_cell_by_rgb(self, sheet_name="", xyxy="", rgb=""):
+		"""
+		셀안의 폰트 색깔을 넣는 것
+		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
+		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
+		my_range.Font.Color = int(rgb[0]) + int(rgb[1]) * 256 + int(rgb[2]) * 65536
 
-		all_data = self.write_value_in_range(sheet_name, [x1, y1, x2, y2])
+	def paint_font_in_range_by_scolor(self, sheet_name="", xyxy="", font_color=""):
+		"""
+		영역안의 폰트 색깔을 넣는 것
+		"""
+		sheet_object = self.check_sheet_name(sheet_name)
+		x1, y1, x2, y2 = self.check_address_value(xyxy)
+		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
+
+		input_data = self.color.change_scolor_to_rgb(font_color)
+		rgb_to_int = (int(input_data[2])) * (256 ** 2) + (int(input_data[1])) * 256 + int(input_data[0])
+		my_range.Font.Color = rgb_to_int
+
+	def paint_maxvalue_in_range_in_each_xline(self, sheet_name="", xyxy=""):
+		"""
+		각 x라인별로 최대값에 색칠하는 것
+		"""
+		x1, y1, x2, y2 = self.check_address_value(xyxy)
+
+		all_data = self.read_value_in_range(sheet_name, [x1, y1, x2, y2])
 		if not (x1 == x2 and y1 == y2):
 			for line_no in range(len(all_data)):
 				line_data = all_data[line_no]
 				filteredList = list(filter(lambda x: type(x) == type(1) or type(x) == type(1.0), line_data))
 				if filteredList == []:
 					pass
 				else:
 					max_value = max(filteredList)
 					x_location = x1 + line_no
 					for no in range(len(line_data)):
 						y_location = y1 + no
 						if (line_data[no]) == max_value:
-							self.paint_color_in_cell(sheet_name, [x_location, y_location], 16)
+							self.paint_cell_by_scolor(sheet_name, [x_location, y_location], "yel")
 		else:
 			print("Please re-check selection area")
 
-	def paint_color_in_range_in_samevalue(self, sheet_name="", xyxy="", input_color="gray"):
+	def paint_minvalue_in_range_in_each_xline(self, sheet_name="", xyxy=""):
 		"""
-		paint_range_samevalue(sheet_name="", xyxy="")
-		선택한 영역에서 2번이상 반복된것만 색칠하기
+		각 x라인별로 최소값에 색칠하는 것
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
-
-		set_a = set([])
-		for x in range(x1, x2 + 1):
-			for y in range(y1, y2 + 1):
-				value = str(sheet_object.Cells(x, y).Value)
-				if value == "" or value == None:
-					pass
-				else:
-					len_old = len(set_a)
-					set_a.add(value)
-					len_new = len(set_a)
-					if len_old == len_new:
-						self.paint_color_in_cell(sheet_name, [x, y], input_color)
-
-	def paint_color_in_range_in_spacecell(self, sheet_name="", xyxy="", input_color="입력필요"):
-		"""
-		빈셀처럼 보이는데 space문자가 들어가 있는것 찾기
-		선택한 영역의 셀을 하나씩 읽어와서 re모듈을 이용해서 공백만 있는지 확인한다
-		"""
-		sheet_object = self.check_sheet_name(sheet_name)
-		x1, y1, x2, y2 = self.check_address_value(xyxy)
-		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
-		for x in range(x1, x2 + 1):
-			for y in range(y1, y2 + 1):
-				cell_value = str(sheet_object.Cells(x, y).Value)
-				com = re.compile("^\s+")
-				if cell_value != None:
-					if com.search(cell_value):
-						self.paint_color_in_cell(sheet_name, [x, y], input_color)
-
-	def paint_color_in_range_in_specific_text(self, sheet_name="", xyxy="", input_list="입력필요", input_color="입력필요"):
-		sheet_object = self.check_sheet_name(sheet_name)
-		x1, y1, x2, y2 = self.check_address_value(xyxy)
-		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
-		selection_range = x1, y1, x2, y2
-		datas = list(self.write_value_in_range(sheet_name, selection_range))
-		temp = []
-		result = []
-		min_value = []
-		input_text = input_list
-		for data_xx in datas:
-			temp_list = []
-			temp_num = 0
-			for data_x in data_xx:
-				if str(input_text) in str(data_x) and data_x != None:
-					self.paint_color_in_range(sheet_name, [x1, y1 + temp_num, x1, y1 + temp_num],
-					                          input_color)
-				temp_num = temp_num + 1
-			x1 = x1 + 1
-
-	def paint_color_in_range_with_minvalue_in_each_xline(self, sheet_name="", xyxy=""):
-		sheet_object = self.check_sheet_name(sheet_name)
-		x1, y1, x2, y2 = self.check_address_value(xyxy)
-		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
-		all_data = self.write_value_in_range(sheet_name, [x1, y1, x2, y2])
+		all_data = self.read_value_in_range(sheet_name, [x1, y1, x2, y2])
 		if not (x1 == x2 and y1 == y2):
 			for line_no in range(len(all_data)):
 				line_data = all_data[line_no]
 				filteredList = list(filter(lambda x: type(x) == type(1) or type(x) == type(1.0), line_data))
 				if filteredList == []:
 					pass
 				else:
 					max_value = min(filteredList)
 					x_location = x1 + line_no
 					for no in range(len(line_data)):
 						y_location = y1 + no
 						if (line_data[no]) == max_value:
-							self.paint_color_in_cell(sheet_name, [x_location, y_location], 3)
+							self.paint_cell_by_scolor(sheet_name, [x_location, y_location], "red")
 		else:
 			print("Please re-check selection area")
 
-	def paint_fontcolor_in_cell_byrgb(self, sheet_name="", xyxy="", rgb=""):
+	def paint_range_by_rgb(self, sheet_name="", xyxy="", input_data=""):
+		"""
+		영역에 색깔을 입힌다
+		엑셀에서의 색깔의 번호는 아래의 공식처럼 만들어 진다
+		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
-		my_range.Font.Color = int(rgb[0]) + int(rgb[1]) * 256 + int(rgb[2]) * 65536
+		rgb_value = self.check_inputcolor_rgb(input_data)
+		rgb_to_int = (int(rgb_value[2])) * (256 ** 2) + (int(rgb_value[1])) * 256 + int(rgb_value[0])
+		my_range.Interior.Color = rgb_to_int
 
-	def paint_fontcolor_in_range(self, sheet_name="", xyxy="", font_color=""):
+	def paint_range_by_scolor(self, sheet_name, xyxy, input_color="입력필요"):
+		self.paint_color_in_range(sheet_name, xyxy, input_color)
+
+	def paint_range_for_empty_cell(self, sheet_name="", xyxy=""):
+		"""
+		빈셀일때 색칠하는 것
+		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
-		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
+		temp_result = 0
+		for x in range(x1, x2 + 1):
+			for y in range(y1, y2 + 1):
+				cell_value = sheet_object.Cells(x, y).Value
+				if cell_value == None:
+					self.paint_cell_by_scolor(sheet_name, [x, y], "yel")
+					temp_result = temp_result + 1
+		return temp_result
 
-		input_data = self.color.change_scolor_to_rgb(font_color)
-		rgb_to_int = (int(input_data[2])) * (256 ** 2) + (int(input_data[1])) * 256 + int(input_data[0])
-		my_range.Font.Color = rgb_to_int
+	def paint_range_for_samevalue_by_excel_colorno(self, sheet_name="", xyxy="", excelcolorno=4):
+		"""
+		영역에서 같은 값을 색칠하는 것
+		"""
+		sheet_object = self.check_sheet_name(sheet_name)
+		x1, y1, x2, y2 = self.check_address_value(xyxy)
+		set_a = set([])
+		for x in range(x1, x2 + 1):
+			for y in range(y1, y2 + 1):
+				value = str(sheet_object.Cells(x, y).Value)
+				if value == "" or value == None:
+					pass
+				else:
+					len_old = len(set_a)
+					set_a.add(value)
+					len_new = len(set_a)
+					if len_old == len_new:
+						self.paint_cell_by_excel_colorno(sheet_name, [x, y], excelcolorno)
 
-	def paint_rgbcolor_in_range(self, sheet_name="", xyxy="", input_data=""):
+	def paint_samevalue_in_range_by_scolor(self, sheet_name="", xyxy="", input_color="gray"):
 		"""
-		영역에 색깔을 입힌다
-		엑셀에서의 색깔의 번호는 아래의 공식처럼 만들어 진다
+		선택한 영역에서 2번이상 반복된것만 색칠하기
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
-		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
 
-		rgb_to_int = (int(input_data[2])) * (256 ** 2) + (int(input_data[1])) * 256 + int(input_data[0])
-		my_range.Interior.Color = rgb_to_int
+		set_a = set([])
+		for x in range(x1, x2 + 1):
+			for y in range(y1, y2 + 1):
+				value = str(sheet_object.Cells(x, y).Value)
+				if value == "" or value == None:
+					pass
+				else:
+					len_old = len(set_a)
+					set_a.add(value)
+					len_new = len(set_a)
+					if len_old == len_new:
+						self.paint_cell_by_scolor(sheet_name, [x, y], input_color)
+
+	def paint_sheet_tab_by_scolor(self, sheet_name, input_color="입력필요"):
+		"""
+		시트탭의 색을 넣는것
+		"""
+		sheet_object = self.check_sheet_name(sheet_name)
+		rgbvalue = self.color.change_scolor_to_rgb(input_color)
+		rgb_to_int = (int(rgbvalue[2])) * (256 ** 2) + (int(rgbvalue[1])) * 256 + int(rgbvalue[0])
+		sheet_object.Tab.Color = rgb_to_int
 
-	def paint_textcolor_in_range(self, sheet_name="", xyxy="", input_color="입력필요"):
+	def paint_spacecell_in_range_by_scolor(self, sheet_name="", xyxy="", input_color="입력필요"):
+		"""
+		빈셀처럼 보이는데 space문자가 들어가 있는것 찾기
+		선택한 영역의 셀을 하나씩 읽어와서 re모듈을 이용해서 공백만 있는지 확인한다
+		"""
+		sheet_object = self.check_sheet_name(sheet_name)
+		x1, y1, x2, y2 = self.check_address_value(xyxy)
+		for x in range(x1, x2 + 1):
+			for y in range(y1, y2 + 1):
+				cell_value = sheet_object.Cells(x, y).Value
+				com = re.compile("^\s+")
+				if cell_value != None:
+					if com.search(cell_value):
+						self.paint_cell_by_scolor(sheet_name, [x, y], input_color)
+
+	def paint_text_in_range_by_scolor(self, sheet_name="", xyxy="", input_color="입력필요"):
+		"""
+		영역에 글자색을 넣는다
+		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
 
 		rgbvalue = self.color.change_scolor_to_rgb(input_color)
 		rgb_to_int = (int(rgbvalue[2])) * (256 ** 2) + (int(rgbvalue[1])) * 256 + int(rgbvalue[0])
 		my_range.Font.Color = rgb_to_int
 
 	def paste_range(self, sheet_name="", xyxy=""):
+		"""
+		영역에 붙여넣기 하는것
+		"""
+
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 		sheet_object.Cells(x1, y1).Select()
 		sheet_object.Paste()
 
-	def pick_unique_value_in_range(self, xyxy):
+	def pick_unique_value_in_range(self, sheet_name="", xyxy=""):
 		"""
 		선택한 자료중에서 고유한 자료만을 골라내는 것이다
 		1. 관련 자료를 읽어온다
 		2. 자료중에서 고유한것을 찾아낸다
 		3. 선택영역에 다시 쓴다
 		"""
-		sheet_object = self.check_sheet_name("")
+		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 
-		temp_datas = self.write_value_in_range("", xyxy)
+		temp_datas = self.read_value_in_range("", xyxy)
 		temp_result = []
 		for one_list_data in temp_datas:
 			for one_data in one_list_data:
 				if one_data in temp_result or type(one_data) == type(None):
 					pass
 				else:
 					temp_result.append(one_data)
 		self.delete_value_in_range("", xyxy)
 		for num in range(len(temp_result)):
 			mox, namuji = divmod(num, x2 - x1 + 1)
 			sheet_object.Cells(x1 + namuji, y1 + mox).Value = temp_result[num]
 
 	def print_page(self, sheet_name, **var_dic):
-		sheet_object = self.check_sheet_name(sheet_name)
-		sheet_object.PageSetup.Zoom = False
-		sheet_object.PageSetup.FitToPagesTall = 1
-		sheet_object.PageSetup.FitToPagesWide = 1
-		# sheet_object.PageSetup.PrintArea = print_area
-		sheet_object.PageSetup.LeftMargin = 25
-		sheet_object.PageSetup.RightMargin = 25
-		sheet_object.PageSetup.TopMargin = 50
-		sheet_object.PageSetup.BottomMargin = 50
-		# sheet_object.ExportAsFixedFormat(0, path_to_pdf)
-		sheet_object.PageSetup.LeftFooter = "&D"  # 날짜
-		sheet_object.PageSetup.LeftHeader = "&T"  # 시간
-		sheet_object.PageSetup.CenterHeader = "&F"  # 화일명
-		sheet_object.PageSetup.CenterFooter = "&P/&N"  # 현 page/ 총 page
-		sheet_object.PageSetup.RightHeader = "&Z"  # 화일 경로
-		sheet_object.PageSetup.RightFooter = "&P+33"  # 현재 페이지 + 33
+		self.set_print_page(sheet_name, **var_dic)
 
 	def print_preview(self, sheet_name=""):
 		sheet_object = self.check_sheet_name(sheet_name)
 		sheet_object.PrintPreview()
 
 	def read_activesheet_name(self):
 		sheet_name = self.xlapp.ActiveSheet.Name
 		return sheet_name
 
+	def read_activeworkbook_filename(self):
+		# 현재 활성화된 엑셀화일의 이름을 갖고읍니다
+		result = self.xlapp.ActiveWorkbook.Name
+		return result
+
+	def read_address_for_rangename(self, sheet_name="", range_name="입력필요"):
+		result = self.read_address_rangename(sheet_name, range_name)
+		return result
+
+	def read_address_for_selection(self):
+		result = self.read_selection_address()
+		return result
+
+	def read_address_for_usedrange(self, sheet_name=""):
+		result = self.read_address_usedrange(sheet_name)
+		return result
+
+	def read_address_in_activecell(self):
+		"""
+		현재 활성화된 셀의 주소를 돌려준다
+		"""
+		result = self.check_address_value(self.xlapp.ActiveCell.Address)
+		return result
+
+
 	def read_address_in_currentregion(self, sheet_name="", xy=""):
 		"""
 		이것은 현재의 셀에서 공백과 공백열로 둘러싸인 활성셀영역을 돌려준다
 		"""
-		result = self.check_address_value(self.xlapp.ActiveCell.CurrentRegion.Address)
+		sheet_object = self.check_sheet_name(sheet_name)
+		my_range = sheet_object.Cells(xy[0], xy[1])
+		# self.select_cell(sheet_name, xy)
+		result = self.check_address_value(my_range.CurrentRegion.Address)
 		return result
 
-	def read_address_in_activecell(self, sheet_name="", xy=""):
-		result = self.check_address_value(self.xlapp.ActiveCell.Address)
-		return result
 
 	def read_address_in_selection(self):
 		"""
 		현재선택된 영역의 주소값을 돌려준다
 		"""
 		result = ""
 		temp_address = self.xlapp.Selection.Address
@@ -2328,15 +2654,35 @@
 			result = self.check_address_value(temp_address)
 		if len(temp_list) > 1:
 			result = []
 			for one_address in temp_list:
 				result.append(self.check_address_value(one_address))
 		return result
 
+	def read_address_rangename(self, sheet_name="", range_name="입력필요"):
+		"""
+		rangename의 주소를 돌려주는것
+		"""
+		sheet_object = self.check_sheet_name(sheet_name)
+		temp = sheet_object.Range(range_name).Address
+		result = self.check_address_value(temp)
+		return result
+
+	def read_address_usedrange(self, sheet_name=""):
+		"""
+		사용자영역을 돌려주는것
+		"""
+		sheet_object = self.check_sheet_name(sheet_name)
+		result = self.check_address_value(sheet_object.UsedRange.address)
+		return result
+
 	def read_all_property_in_cell(self, sheet_name="", xy=[7, 7]):
+		"""
+		셀의 모든 속성을 돌려주는것
+		"""
 		basic_cell = basic_data.basic_cell_class()
 		sheet_object = self.check_sheet_name(sheet_name)
 		one_cell = sheet_object.Cells(xy[0], xy[1])
 		result = basic_cell.values
 		y = result["y"] = xy[0]
 		x = result["x"] = xy[1]
 		result["value"] = one_cell.Value
@@ -2405,15 +2751,23 @@
 				result["line_x2_dic"]["style"] = one_cell.Borders(12).LineStyle
 				result["line_x2_dic"]["color"] = one_cell.Borders(12).Color
 				result["line_x2_dic"]["colorindex"] = one_cell.Borders(12).ColorIndex
 				result["line_x2_dic"]["thick"] = one_cell.Borders(12).Weight
 				result["line_x2_dic"]["tintandshade"] = one_cell.Borders(12).TintAndShade
 		return result
 
+	def read_cell_value(self, sheet_name="", xyxy=""):
+		#보관용
+		result = self.read_value_in_cell(sheet_name, xyxy)
+		return result
+
 	def read_color_in_cell(self, sheet_name="", xyxy=""):
+		"""
+		셀의 색을 돌려주는것
+		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
 
 		result = my_range.Interior.Color
 		return result
 
@@ -2427,233 +2781,346 @@
 
 		rng_x_coord = my_range.Left
 		rng_y_coord = my_range.Top
 		rng_width = my_range.Width
 		rng_height = my_range.Height
 		return [rng_x_coord, rng_y_coord, rng_width, rng_height]
 
+	def read_filename_for_activeworkbook(self):
+		result = self.read_activeworkbook_filename()
+		return result
+
+	def read_folder_filename_all(self, directory):
+		"""
+		폴더 안의 화일을 읽어오는것
+		"""
+		result = []
+		filenames = os.listdir(directory)
+		for filename in filenames:
+			full_filename = os.path.join(directory, filename)
+			result.append(filename)
+		return result
+
+	def read_fontcolor_in_cell(self, sheet_name="", xyxy=""):
+		"""
+		셀의 폰트 색을 돌려주는것
+		"""
+		sheet_object = self.check_sheet_name(sheet_name)
+		x1, y1, x2, y2 = self.check_address_value(xyxy)
+		my_range = sheet_object.Cells(x1, y1)
+		result = my_range.Font.Color
+		return result
+
 	def read_general_value(self):
 		"""
 		몇가지 엑셀에서 자주사용하는 것들정의
 		엑셀의 사용자, 현재의 경로, 화일이름, 현재시트의 이름
 		"""
 		result = []
 		result.append(self.xlapp.ActiveWorkbook.Name)
 		result.append(self.xlapp.Username)
 		result.append(self.xlapp.ActiveWorkbook.ActiveSheet.Name)
 		return result
 
 	def read_inputbox_value(self, title="Please Input Value"):
+		"""
+		inputbox를 사용하고 싶을때
+		"""
 		result = self.xlapp.Application.InputBox(title)
 		return result
 
 	def read_memo_in_cell(self, sheet_name="", xyxy=""):
+		"""
+		셀의 메모를 돌려주는것
+		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
 
 		result = my_range.Comment.Text()
 		return result
 
-	def read_rangename_address(self, sheet_name="", range_name="입력필요"):
-		sheet_object = self.check_sheet_name(sheet_name)
-		temp = sheet_object.Range(range_name).Address
-		result = self.check_address_value(temp)
+	def read_name_for_workbook(self):
+		""" 워크북의 이름을 읽어온다 """
+		return self.xlbook.Name
+
+	def read_opened_workbook_filename_all(self):
+		# 모든 열려있는 엑셀화일의 이름을 갖고옵니다
+		result = []
+		for one in self.xlapp.Workbooks:
+			result.append(one.Name)
+		return result
+
+	def read_range_value(self, sheet_name="", xyxy=""):
+		#보관용
+		result = self.read_value_in_range(sheet_name, xyxy)
 		return result
 
 	def read_rangename_all(self):
+		"""
+		모든 rangename을 돌려주는것
+		"""
 		names_count = self.xlbook.Names.Count
 		result = []
 		if names_count > 0:
 			for aaa in range(1, names_count + 1):
 				name_name = self.xlbook.Names(aaa).Name
 				name_range = self.xlbook.Names(aaa)
 				result.append([aaa, str(name_name), str(name_range)])
 		return result
 
-	def read_shape_in_sheet_name_by_no(self, sheet_name="", shape_no="입력필요"):
+	def read_selection_address(self):
+		"""
+		영문으로 되어있는 주소를 아라비아숫자로 변경하는 것이다
+		예전이름 : def address_all (self, input_datas)
+		"""
+		input_datas = str(self.xlapp.Selection.Address)
+		input_datas = str(input_datas).lower()
+		arange = str(input_datas).replace("$", "").split(":")
+		if len(arange) == 1:	arange.append(arange[0])
+		if str(arange[0]).lower() in string.ascii_lowercase and str(arange[1]).lower() in string.ascii_lowercase:
+			arange[0] = arange[0] + "0"
+			arange[1] = arange[1] + "65536"
+		if str(arange[0]).lower() in string.digits and str(arange[1]).lower() in string.digits:
+			arange[0] = "a" + arange[0]
+			arange[1] = "iv" + arange[1]
+		result = []
+		for a in arange:
+			if str(a[0]).lower() in string.ascii_lowercase and str(a[1]).lower() in string.ascii_lowercase:
+				result.append(a[0:2])
+				result.append(a[2:])
+			else:
+				result.append(a[0])
+				result.append(a[1:])
+		if result[0]:
+			if len(result[0]) == 1:
+				result[0] = (string.ascii_lowercase.index(result[0]) + 1)
+			else:
+				aaa = (string.ascii_lowercase.index(result[0][0]) + 1) * 26
+				result[0] = aaa + (string.ascii_lowercase.index(result[0][1]) + 1)
+		if result[2]:
+			if len(result[2]) == 1:
+				result[2] = (string.ascii_lowercase.index(result[2]) + 1)
+			else:
+				aaa = (string.ascii_lowercase.index(result[2][0]) + 1) * 26
+				result[2] = aaa + (string.ascii_lowercase.index(result[2][1]) + 1)
+		final_data = [int(result[1]), int(result[0]), int(result[3]), int(result[2])]  # 2005-02-17 추가
+		return final_data
+
+	def read_shape_name_in_sheet_by_no(self, sheet_name="", shape_no="입력필요"):
+		"""
+		번호로 객체의 이름을 갖고오는것
+		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		result = sheet_object.Shapes(shape_no).Name
 		return result
 
-	def read_usedrange_address(self, sheet_name=""):
-		sheet_object = self.check_sheet_name(sheet_name)
-		result = self.check_address_value(sheet_object.UsedRange.address)
+	def read_sheet_name_all(self):
+		"""
+		워크시트의 모든 이름을 읽어온다
+		"""
+		result = []
+		for a in range(1, self.xlbook.Worksheets.Count + 1):
+			result.append(self.xlbook.Worksheets(a).Name)
 		return result
 
 	def read_username(self):
-		result = self.xlapp.Username
+		"""	사용자 이름을 읽어온다	"""
+		return self.xlapp.Username
+
+	def read_value2_in_cell(self, sheet_name, xyxy):
+		result = self.read_value_in_cell_as_value2(sheet_name, xyxy)
+		return result
+
+	def read_value2_in_range(self, sheet_name, xyxy):
+		result = self.read_value_in_range_as_value2(sheet_name, xyxy)
 		return result
 
 	def read_value_in_activecell(self):
+		"""
+		현재셀의 값을 돌려주는것
+		"""
 		result = [self.xlapp.ActiveCell.Row, self.xlapp.ActiveCell.Column, self.xlapp.ActiveCell.Value]
 		return result
 
-	def read_cell_value(self, sheet_name="", xyxy=""):
-		self.read_value_in_cell(sheet_name, xyxy)
-
 	def read_value_in_cell(self, sheet_name="", xyxy=""):
 		"""
-		# 값을 일정한 영역에서 갖고온다
+		값을 일정한 영역에서 갖고온다
 		만약 영역을 두개만 주면 처음과 끝의 영역을 받은것으로 간주해서 알아서 처리하도록 변경하였다
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 		result = sheet_object.Cells(x1, y1).Value
 
 		if type(result) == type(123):
 			result = int(result)
 		elif result == None:
 			result = ""
 		return result
 
-	def read_value_in_continous_range(self, sheet_name="", xyxy=""):
+	def read_value_in_cell_as_text(self, sheet_name="", xyxy=""):
 		"""
-		# 현재선택된 셀을 기준으로 연속된 영역을 가지고 오는 것입니다
+		읽어온값 자체를 변경하지 않고 그대로 읽어오는 것
+		그자체로 text형태로 돌려주는것
+		만약 스캔을 한 숫자가 ,를 잘못 .으로 읽었다면
+		48,100 => 48.1로 엑셀이 바로 인식을 하는데
+		이럴때 48.100으로 읽어와서 바꾸는 방법을 하기위해 사용하는 방법
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
-		row = xyxy
-		col = xyxy
+		result = sheet_object.Cells(x1, y1).Text
+		if result == None:
+			result = ""
+		return result
+
+	def read_value_in_cell_as_value2(self, sheet_name="", xyxy=""):
+		"""
+		값을 일정한 영역에서 갖고온다
+		만약 영역을 두개만 주면 처음과 끝의 영역을 받은것으로 간주해서 알아서 처리하도록 변경하였다
+		"""
 		sheet_object = self.check_sheet_name(sheet_name)
-		bottom = row  # 아래의 행을 찾는다
-		while sheet_object.Cells(bottom + 1, col).Value not in [None, '']:
-			bottom = bottom + 1
-		right = col  # 오른쪽 열
-		while sheet_object.Cells(row, right + 1).Value not in [None, '']:
-			right = right + 1
-		return sheet_object.Range(sheet_object.Cells(row, col), sheet_object.Cells(bottom, right)).Value
+		x1, y1, x2, y2 = self.check_address_value(xyxy)
+		result = sheet_object.Cells(x1, y1).Value2
+		if result == None:
+			result = ""
+		return result
+
+	def read_value_in_continuous_range(self, sheet_name="", xyxy=""):
+		"""
+		현재선택된 셀을 기준으로 연속된 영역을 가지고 오는 것입니다
+		"""
+		sheet_object = self.check_sheet_name(sheet_name)
+		x1, y1, x2, y2 = self.check_address_value(xyxy)
+		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
+		address = my_range.CurrentRegion()
+		result = self.read_value_in_range(sheet_name, address)
+		return result
+
+	def read_value_in_currentregion(self, sheet_name="", xyxy=""):
+		result = self.read_value_in_continuous_range(sheet_name, xyxy)
+		return result
+
 
 	def read_value_in_range(self, sheet_name, xyxy):
 		"""
-		# 값을 일정한 영역에서 갖고온다
-		만약 영역을 두개만 주면 처음과 끝의 영역을 받은것으로 간주해서 알아서 처리하도록 변경하였다
+		영역의 값을 갖고온다
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
 		if x1 == -1:
 			return sheet_object.Range(x1, y1).Value
 		return my_range.Value
 
+	def read_value_in_range_as_value2(self, sheet_name, xyxy):
+		"""
+		영역의 값을 갖고온다
+		"""
+		sheet_object = self.check_sheet_name(sheet_name)
+		x1, y1, x2, y2 = self.check_address_value(xyxy)
+		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
+		if x1 == -1:
+			return sheet_object.Range(x1, y1).Value2
+		return my_range.Value2
+
 	def read_value_in_selection(self, sheet_name="", xyxy=""):
 		"""
 		값을 일정한 영역에서 갖고온다
 		만약 영역을 두개만 주면 처음과 끝의 영역을 받은것으로 간주해서 알아서 처리하도록 변경하였다
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
 		self.get_activesheet_object()
 		self.check_address_value(self.xlapp.Selection.Address)
 		result = my_range.Value
 		return result
 
+	def read_value_in_xline(self, sheet_name="", xx="입력필요"):
+		"""
+		한줄인 x라인 의 모든값을 읽어온다
+		"""
+		sheet_object = self.check_sheet_name(sheet_name)
+		x1, x2 = self.check_xx_address(xx)
+		return sheet_object.Range(sheet_object.Cells(x1, 1), sheet_object.Cells(x1, 1)).EntireRow.Value
+
 	def read_value_in_xxline(self, sheet_name="", xx="입력필요"):
+		"""
+		xx라인의 모든값을 읽어온다
+		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		return sheet_object.Range(sheet_object.Cells(xx[0], 1), sheet_object.Cells(xx[1], 1)).EntireRow.Value
 
+	def read_value_in_yline(self, sheet_name="", yy="입력필요"):
+		"""	한줄인 y라인의 모든값을 읽어온다	"""
+		sheet_object = self.check_sheet_name(sheet_name)
+		y1, y2 = self.check_yy_address(yy)
+		return sheet_object.Range(sheet_object.Cells(1, y1), sheet_object.Cells(1, y1)).EntireColumn.Value
+
 	def read_value_in_yyline(self, sheet_name="", yy="입력필요"):
+		"""	yy라인의 모든값을 읽어온다	"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		return sheet_object.Range(sheet_object.Cells(1, yy[0]), sheet_object.Cells(1, yy[1])).EntireColumn.Value
 
 	def read_workbook_fullname(self):
+		"""	워크북의 전체 경로와 이름을 읽어온다	"""
 		return self.xlbook.FullName
 
-	def read_workbook_name(self):
-		return self.xlbook.Name
-
 	def read_workbook_path(self):
+		"""	워크북의 경로를 읽어온다	"""
 		return self.xlbook.Path
 
 	def read_workbook_username(self):
+		"""	사용자 이름을 읽어온다	"""
 		return self.xlapp.Username
 
 	def read_worksheet_count(self):
+		""" 워크시트의 갯수를 읽어온다 """
 		return self.xlbook.Worksheets.Count
 
-	def read_sheet_name_all(self):
-		result = []
-		for a in range(1, self.xlbook.Worksheets.Count + 1):
-			result.append(self.xlbook.Worksheets(a).Name)
-		return result
-
 	def read_worksheet_numbers(self):
-		return self.xlbook.Worksheets.Count
+		result = self.read_worksheet_count()
+		return result
 
 	def remove_vba_module(self, module_name_list):
 		"""
 		입력형태 : 리스트형, 메크로 모듈이름
 		역활 : 열려있는 화일안에서 입력리스트의 메크로를 삭제를 하는 것
 		"""
 		for module_name in module_name_list:
 			xlmodule = self.xlbook.VBProject.VBComponents(module_name)
 			self.xlbook.VBProject.VBComponents.Remove(xlmodule)
 
-	def read_selection_address(self):
+	def replace_word_in_range_by_list2d_style(self, sheet_name="", xyxy="", from_to_list2d = []):
 		"""
-		영문으로 되어있는 주소를 아라비아숫자로 변경하는 것이다
-		예전이름 : def address_all (self, input_datas)
+		영역안의 글자들을 바꾸기 한다
 		"""
-		input_datas = str(self.xlapp.Selection.Address)
-		input_datas = str(input_datas).lower()
-		arange = str(input_datas).replace("$", "").split(":")
-		if len(arange) == 1:    arange.append(arange[0])
-		if str(arange[0]).lower() in string.ascii_lowercase and str(arange[1]).lower() in string.ascii_lowercase:
-			arange[0] = arange[0] + "0"
-			arange[1] = arange[1] + "65536"
-		if str(arange[0]).lower() in string.digits and str(arange[1]).lower() in string.digits:
-			arange[0] = "a" + arange[0]
-			arange[1] = "iv" + arange[1]
-		result = []
-		for a in arange:
-			if str(a[0]).lower() in string.ascii_lowercase and str(a[1]).lower() in string.ascii_lowercase:
-				result.append(a[0:2])
-				result.append(a[2:])
-			else:
-				result.append(a[0])
-				result.append(a[1:])
-		if result[0]:
-			if len(result[0]) == 1:
-				result[0] = (string.ascii_lowercase.index(result[0]) + 1)
-			else:
-				aaa = (string.ascii_lowercase.index(result[0][0]) + 1) * 26
-				result[0] = aaa + (string.ascii_lowercase.index(result[0][1]) + 1)
-		if result[2]:
-			if len(result[2]) == 1:
-				result[2] = (string.ascii_lowercase.index(result[2]) + 1)
-			else:
-				aaa = (string.ascii_lowercase.index(result[2][0]) + 1) * 26
-				result[2] = aaa + (string.ascii_lowercase.index(result[2][1]) + 1)
-		final_data = [int(result[1]), int(result[0]), int(result[3]), int(result[2])]  # 2005-02-17 추가
-		return final_data
+		sheet_object = self.check_sheet_name(sheet_name)
+		x1, y1, x2, y2 = self.check_address_value(xyxy)
+		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
+		for list1d in from_to_list2d:
+			my_range.Replace(list1d[0], list1d[1])
 
-	def remove_emptyvalue(self, sheet_name="", xyxy="", condition=[None, ""]):
+	def replace_word_many_in_range(self, sheet_name="", xyxy="", input_list="입력필요"):
 		"""
-		이상하게 이것을 다시 설정하지 않으면 에러가 난다
+		한번에 여러 갯수를 바꾸는 것이다
 		"""
-		condition = [None, ""]
-		values = self.read_value_in_range(sheet_name, xyxy)
-		time.sleep(2)
-		self.delete_value_in_range(sheet_name, xyxy)
-		values_checked = self.yt.delete_emptyvalue_in_list(values, condition)
-		self.write_value_in_range(sheet_name, xyxy, values_checked)
-
-	def replace_word_many_in_range(self, sheet_name="", xyxy="", input_list="입력필요"):
-		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 
 		for y in range(y1, y2 + 1):
 			for x in range(x1, x2 + 1):
 				cell_value = str(self.read_cell_value(sheet_name, [x, y]))
 				for one_list in input_list:
 					cell_value = cell_value.replace(one_list[0], one_list[1])
 				self.write_cell_value(sheet_name, [y, x + 1], cell_value)
 
 	def resize_list(self, xy_list, resize=[1, 1]):
+		"""
+		리스트의 크기를 다시 설정하는 것
+		"""
 		result = []
 		# 자료의 x갯수를 요청한것과 비교
 		if len(xy_list) < resize[0] or resize[0] == 0:
 			pass
 		else:
 			xy_list = xy_list[:resize[0]]
 		# 자료의 y갯수를 요청한것과 비교
@@ -2665,74 +3132,98 @@
 			result.append(x_list)
 		return result
 
 	def run_vba_module(self, vba_code, macro_name):
 		"""
 		텍스트로 만든 매크로 코드를 실행하는 코드이다
 		"""
-		new_vba_code = "Sub " + macro_name + "()" + vba_code + " End Sub"
+		new_vba_code = "Sub " + macro_name + "()//n" + vba_code + "End Sub"
 		mod = self.xlbook.VBProject.VBComponents.Add(1)
 		mod.CodeModule.AddFromString(new_vba_code)
 		self.xlapp.Run(macro_name)
 
-	def save(self, newfilename):
+	def save(self, newfilename=""):
+		"""
+		엑셀화일을 저장하는것
+		"""
 		if newfilename == "":
 			self.xlbook.Save()
 		else:
-			self.xlbook.SaveAs(newfilename)
+			#wb.SaveAs(Filename="C:\\NewFileName.xlsx")
+			self.xlbook.SaveAs(newfilename, 6)
 
 	def screen_update_off(self):
+		"""
+		화면 변화를 잠시 멈추는것
+		"""
 		self.xlapp.ScreenUpdating = False
 
 	def screen_update_on(self):
+		"""
+		화면 변화를 시작
+		"""
 		self.xlapp.ScreenUpdating = True
 
+	def select_cell(self, sheet_name="", xyxy=""):
+		"""
+		영역을 선택한다
+		"""
+		sheet_object = self.check_sheet_name(sheet_name)
+		x1, y1, x2, y2 = self.check_address_value(xyxy)
+		sheet_object.Cells(x1, y1).Select()
+
 	def select_range(self, sheet_name="", xyxy=""):
 		"""
 		영역을 선택한다
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
 		my_range.Select()
 
 	def select_sheet(self, sheet_name=""):
 		"""
 		현재의 엑셀중에서 활성화된 시트의 이름을 돌려준다
 		"""
 		if sheet_name == None or sheet_name == "":
-			self.show_messagebox_value("시트이름을 다시한번 확인 해 주십시요")
+			self.show_messagebox_with_value("시트이름을 다시한번 확인 해 주십시요")
 		elif sheet_name in self.read_sheet_name_all():
 			self.xlbook.Worksheets(sheet_name).Select()
 
-	def select_top_in_range(self, sheet_name="", xyxy=""):
+	def select_top_line_in_range(self, sheet_name="", xyxy=""):
+		""" 영역의 제일 위로 이동 """
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
-		sheet_object.Cells(x1, y1).End(- 4162).Select()
+		sheet_object.Cells(x1, y1).Select()
 
 	def set_autofit_in_range(self, sheet_name="", xyxy="all"):
+		""" 자동 맞춤을 실시 """
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 		new_y1 = self.change_num_to_char(y1)
 		new_y2 = self.change_num_to_char(y2)
 		if xyxy == "" or xyxy == "all":
-			sheet_object.EntireColumn.AutoFit()
+			sheet_object.Columns.AutoFit()
 		else:
-			sheet_object.Columns(str(new_y1) + ':' + str(new_y2)).AutoFit()
+			sheet_object.Columns(new_y1 + ':' + new_y2).AutoFit()
 
 	def set_bold_in_range(self, sheet_name="", xyxy=""):
 		"""
 		영역안의 글씨체를 진하게 만든다
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
 		my_range.Font.Bold = True
 
+	def set_cell_color(self, sheet_name, xy, input_color="입력필요"):
+		self.paint_cell_by_scolor(sheet_name, xy, input_color)
+
 	def set_conditional_in_range(self):
+		""" 조건부서식을 좀더 사용하기 쉽도록 변경이 필요 """
 		sheet_object = self.check_sheet_name("")
 		my_range = sheet_object.Range(sheet_object.Cells(1, 1), sheet_object.Cells(20, 20))
 		formula1 = ' = IF($A1 = "", TRUE, FALSE)'
 		# win32com.client.constants.xlCellValue = > 1
 		# win32com.client.constants.xlGreaterEqual = > 7
 		my_range.FormatConditions.Add(1, 7, formula1)
 		my_range.FormatConditions(my_range.FormatConditions.Count).SetFirstPriority()
@@ -2740,42 +3231,66 @@
 		my_range.FormatConditions(1).Font.Strikethrough = False
 		my_range.FormatConditions(1).Font.TintAndShade = 0
 		my_range.FormatConditions(1).Interior.PatternColorIndex = 1
 		my_range.FormatConditions(1).Interior.Color = 5296274
 		my_range.FormatConditions(1).Interior.TintAndShade = 0
 		my_range.FormatConditions(1).StopIfTrue = False
 
+
+	def check_filepath(self, file_name):
+		"""
+		경로를 구분하는 \\과 /의 혼돈 삽입으로 다시 확인하고자 한다 가능하면 /를 사용하기를 권장 한다
+		"""
+		file_name = file_name.replace("\\\\","/")
+		file_name = file_name.replace("\\", "/")
+		return file_name
+
+
 	def set_font_in_range(self, sheet_name="", xyxy="", font="입력필요"):
 		"""
 		영역에 글씨체를 설정한다
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
 		my_range.Font.Name = font
 
-	def set_fontcolor_in_range(self, sheet_name="", xyxy="", font_name=""):
+	def set_fontcolor_in_cell(self, sheet_name="", xy="", font_color=""):
+		"""
+		셀에 글씨체를 설정한다
+		"""
+		sheet_object = self.check_sheet_name(sheet_name)
+		x1, y1, x2, y2 = self.check_address_value(xy)
+		rgb_value = self.check_inputcolor_rgb(font_color)
+		rgb_int = self.color.change_rgb_to_rgbint(rgb_value)
+		my_range = sheet_object.Cells(x1, y1)
+		my_range.Font.Color = rgb_int
+
+	def set_fontcolor_in_range(self, sheet_name="", xyxy="", font_color=""):
 		"""
 		영역에 글씨체를 설정한다
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
-		my_range.Font.Color = font_name
+		rgb_value = self.check_inputcolor_rgb(font_color)
+		rgb_int = self.color.change_rgb_to_rgbint(rgb_value)
+		#my_range = sheet_object.Cells(x1, y1)
+		my_range.Font.Color = rgb_int
 
 	def set_fontsize_in_range(self, sheet_name="", xyxy="", size="입력필요"):
 		"""
 		영역에 글씨크기를 설정한다
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
 		my_range.Font.Size = int(size)
 
-	def set_formula_in_range(self, sheet_name="", xyxy="", input_data=" = Now()"):
+	def set_formula_in_range(self, sheet_name="", xyxy="", input_data="=Now()"):
 		"""
 		set_range_formula(sheet_name="", xyxy="", input_data="=Now()")
 		영역에 수식을 넣는것
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
@@ -2783,80 +3298,64 @@
 
 	def set_fullscreen(self, fullscreen=1):
 		"""
 		전체화면으로 보기
 		"""
 		self.xlapp.DisplayFullScreen = fullscreen
 
+	def set_fullscreen_for_workbook(self, fullscreen=1):
+		""" 전체화면으로 보이게 하는 것 """
+		self.xlapp.DisplayFullScreen = fullscreen
+
 	def set_gridline_off(self):
+		""" 그리드라인을 없애는것 """
 		self.xlapp.ActiveWindow.DisplayGridlines = 0
 
 	def set_gridline_on(self):
+		""" 그리드라인을 나탄게 하는것 """
 		self.xlapp.ActiveWindow.DisplayGridlines = 1
 
 	def set_gridline_onoff(self):
+		""" 그리드라인을 껏다 켰다하는 것 """
 		if self.xlapp.ActiveWindow.DisplayGridlines == 0:
 			self.xlapp.ActiveWindow.DisplayGridlines = 1
 		else:
 			self.xlapp.ActiveWindow.DisplayGridlines = 0
 
 	def set_height_in_xxline(self, sheet_name, xx, height=13.5):
 		"""
 		가로줄의 높이를 설정
 		"""
-		my_range = self.check_xx_address(sheet_name, xx)
+		sheet_object = self.check_sheet_name(sheet_name)
+		my_range = sheet_object.Range(sheet_object.Cells(xx[0], 1), sheet_object.Cells(xx[1], 1))
 		my_range.RowHeight = height
 
 	def set_merge_in_range(self, sheet_name="", xyxy=""):
 		"""
 		셀들을 병합하는 것
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
 		my_range.Merge(0)
 
-	def set_numberformat_in_cell(self, type="general", number=0):
-		"""
-		셀의 숫자에대한 형식을 설정
-		"""
-		if type == 'general':
-			format = "#,##0.00_ "
-		elif type == 'number':
-			format = "US$#,##0.00"
-		elif type == 'account':
-			format = "_-""US$""* #,##0.00_ ;_-""US$""* -#,##0.00 ;_-""US$""* ""-""??_ ;_-@_ "
-		elif type == 'date':
-			format = "mm""/""dd""/""yy"
-		elif type == 'datetime':
-			format = "yyyy""-""m""-""d h:mm AM/PM"
-		elif type == 'percent':
-			format = "0.00%"
-		elif type == 'bunsu':
-			format = "# ?/?"
-		elif type == 'jisu':
-			format = "0.00E+00"
-		elif type == 'text':
-			format = "@"
-		elif type == 'etc':
-			format = "000-000"
-		elif type == 'other':
-			format = "$#,##0.00_);[빨강]($#,##0.00)"
-		range.NumberFormatLocal = format
+	def set_numberformat_in_cell(self, sheet_name="", xyxy="", numberformat="#,##0.00_ "):
+		self.set_numberformat_in_range(sheet_name, xyxy, numberformat)
 
-	def set_numberformat_in_range(self, sheet_name="", xyxy="", numberformat="입력필요"):
+	def set_numberformat_in_range(self, sheet_name="", xyxy="", numberformat="#,##0.00_ "):
 		"""
 		영역에 숫자형식을 지정하는 것
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
 		my_range.NumberFormat = numberformat
 
 	def set_numberproperty_in_range(self, sheet_name="", xyxy="", type1="입력필요"):
+		""" 좀더 사용하기 쉽도록 변경이 필요 """
 		if type1 == 'general':
 			result = "#,##0.00_ "
 		elif type1 == 'number':
 			result = "US$""#,##0.00"
 		elif type1 == 'account':
 			result = "_-""US$""* #,##0.00_ ;_-""US$""* -#,##0.00 ;_-""US$""* ""-""??_ ;_-@_ "
 		elif type1 == 'date':
@@ -2877,21 +3376,18 @@
 			result = "$#,##0.00_);[빨강]($#,##0.00)"
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
 		my_range.NumberFormat = result
 
 	def set_picture_in_cell(self, sheet_name, xy, full_path):
-		sheet_object = self.check_sheet_name(sheet_name)
-		x1, y1, x2, y2 = self.check_address_value(xy)
-		sheet_object.Cells(x1, y1).Select()
-		aaa = sheet_object.Pictures
-		aaa.Insert(full_path).Select()
+		self.insert_image_in_xyxy(sheet_name, xy, full_path)
 
 	def set_print_page(self, sheet_name="", **var_dic):
+		""" 좀더 사용하기 쉽도록 변경이 필요 """
 		sheet_object = self.check_sheet_name(sheet_name)
 		sheet_object.PageSetup.Zoom = False
 		sheet_object.PageSetup.FitToPagesTall = 1
 		sheet_object.PageSetup.FitToPagesWide = 1
 		# sheet_object.PageSetup.PrintArea = print_area
 		sheet_object.PageSetup.LeftMargin = 25
 		sheet_object.PageSetup.RightMargin = 25
@@ -2902,165 +3398,251 @@
 		sheet_object.PageSetup.LeftHeader = "&T"  # 시간
 		sheet_object.PageSetup.CenterHeader = "&F"  # 화일명
 		sheet_object.PageSetup.CenterFooter = "&P/&N"  # 현 page/ 총 page
 		sheet_object.PageSetup.RightHeader = "&Z"  # 화일 경로
 		sheet_object.PageSetup.RightFooter = "&P+33"  # 현재 페이지 + 33
 
 	def set_rangename(self, sheet_name="", xyxy="", name=""):
+		"""
+		rangename을 설정하는 것
+		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
 		self.xlbook.Names.Add(name, my_range)
 
-	def set_sheet_visible(self, input_data=0):
-		self.xlapp.Visible = input_data
-
 	def set_unmerge_in_range(self, sheet_name="", xyxy=""):
 		"""
 		영역안의 병합된 것을 푸는 것이다
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
 		my_range.UnMerge()
 
-	def set_workbook_close(self):
+	def set_visible_for_sheet(self, input_data=0):
 		"""
-		현재는 close를 시키면 엑셀워크북만이 아니라 엑셀자체도 종료 시킵니다
+		시트를 감추는것
 		"""
-		self.xlbook.Close(SaveChanges=0)
-		del self.xlapp
-
-	def set_workbook_fullscreen(self, fullscreen=1):
-		self.xlapp.DisplayFullScreen = fullscreen
+		self.xlapp.Visible = input_data
 
-	def set_workbook_visible(self, value=1):
+	def set_visible_for_workbook(self, value=1):
 		"""
 		실행되어있는 엑셀을 화면에 보이지 않도록 설정합니다
 		기본설정은 보이는 것으로 되너 있읍니다
 		"""
 		self.xlapp.Visible = value
 
+	def set_width_in_yyline(self, sheet_name, yy, width=5):
+		"""
+		가로줄의 높이를 설정
+		"""
+		sheet_object = self.check_sheet_name(sheet_name)
+		my_range = sheet_object.Range(sheet_object.Cells(1, yy[0]), sheet_object.Cells(1, yy[1]))
+		my_range.ColumnWidth = width
+
 	def set_wrap_in_range(self, sheet_name="", xyxy="", input_data=""):
 		"""
 		셀의 줄바꿈을 설정할때 사용한다
 		만약 status를 false로 하면 줄바꿈이 실행되지 않는다.
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		sheet_object.Range(xyxy).WrapText = input_data
 
-	def show_messagebox_value(self, input_text="입력필요", input_title="pcell"):
+	def show_messagebox_with_value(self, input_text="입력필요", input_title="pcell"):
 		"""
 		메세지박스를 보여주는것
 		"""
 		win32gui.MessageBox(0, input_text, input_title, 0)
 
-	def split_value_to_special_string(self, sheet_name="", input_text="입력필요"):
+	def sound_beep(self, sec = 1000, hz = 500):
+		"""
+		beep 음을 내는 것
+		"""
+		win32api.Beep(hz, sec)
+
+	def split_value_as_engnum(self, data):
+		"""
+		 단어중에 나와있는 숫자, 영어를 분리하는기능
+		"""
+		re_compile = re.compile(r"[a-zA-Z0-9]+")
+		result = re_compile.findall(data)
+
+		new_result = []
+		for dim1_data in result:
+			for dim2_data in dim1_data:
+				new_result.append(dim2_data)
+		return new_result
+
+	def split_value_by_special_string(self, sheet_name="", input_text="입력필요"):
 		"""
 		split_inputvalue_as_special_string( input_text="입력필요"):
 		선택한 1줄의 영역에서 원하는 문자나 글자를 기준으로 분리할때
 		2개의 세로행을 추가해서 결과값을 쓴다
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		rng_select = self.read_address_in_selection()
-		rng_used = self.read_usedrange_address()
+		rng_used = self.read_address_usedrange()
 		[x1, y1, x2, y2] = self.intersect_range1_range2(rng_select, rng_used)
 		self.insert_xline("", x1 + 1)
 		self.insert_xline("", x1 + 1)
 		result = []
 		length = 2
 		# 자료를 분리하여 리스트에 집어 넣는다
 		for x in range(x1, x2 + 1):
 			for y in range(y1, y2 + 1):
-				cell_value = str(sheet_object.Cells(x, y).Value)
+				cell_value = sheet_object.Cells(x, y).Value
 				list_data = cell_value.split(input_text)
 				result.append(list_data)
 		# 집어넣은 자료를 다시 새로운 세로줄에 넣는다
 		for y_no in range(len(result)):
 			if len(result[x_no]) > length:
 				for a in range(len(result[x_no]) - length):
 					self.insert_xline("", x1 + length)
 				length = len(result[x_no])
 			for x_no in range(len(result[x_no])):
 				sheet_object.Cells(x1 + x_no, y1 + y_no + 1).Value = result[x_no][y_no]
 
-	def split_value_to_str_num(self, input_text):
-		re_com_num = re.compile("[a-zA-Z]+|\d+")
-		result = re_com_num.findall(input_text)
-		return result
-
 	def swap_cap_small(self, sheet_name="", xyxy=""):
-		sheet_object = self.check_sheet_name(sheet_name)
+		""" 영역안의 값을 대/소문자를 바꾸는 것 """
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 		for y in range(y1, y2 + 1):
 			for x in range(x1, x2 + 1):
 				temp_data = self.read_cell_value(sheet_name, [x, y])
-				self.write_cell_value(sheet_name, [x, y], string.swapcase(temp_data))
+				self.write_cell_value(sheet_name, [x, y], str(temp_data).swapcase())
+
+	def terms(self):
+		""" 용어들에 대한 정리 """
+		result = 	"""
+			"""
+		return result
 
 	def unlock_sheet(self, sheet_name="", password="1234"):
+		""" 시트 보호를 설정 하는 것 """
 		sheet_object = self.check_sheet_name(sheet_name)
 		sheet_object.Unprotect(password)
 
+
+	def vlookup_with_multi_line(self, input_data1, input_data2):
+		"""
+		보통 vlookup은 한줄을 비교해서 다른 자료를 찾는데
+		이것은 여러항목이 같은 값을 기준으로 원하는 것을 찾는 것이다
+		input_datal = [자료의영역, 같은것이있는위치, 결과값의위치]
+		"""
+		base_data2d = self.read_value_in_range("", input_data1[0])
+		compare_data2d = self.read_value_in_range("", input_data2[0])
+		result = ""
+		for one_data_1 in base_data2d:
+			gijun = []
+			one_data_1 = list(one_data_1)
+			for no in input_data1[1]:
+				gijun.append(one_data_1[no - 1])
+			x = 0
+
+			for value_1d in compare_data2d:
+				value_1d = list(value_1d)
+				x = x + 1
+				bikyo = []
+
+				for no in input_data2[1]:
+					bikyo.append(value_1d[no-1])
+
+				if gijun == bikyo:
+					result = one_data_1[input_data1[2] - 1]
+				self.write_value_in_cell("", [x, input_data2[2]], result)
+	def write_cell_value(self, sheet_name="", xyxy="", value="입력필요"):
+		"""
+		"""
+		self.write_value_in_cell(sheet_name, xyxy, value)
+
 	def write_df_to_excel(self, sheet_name="", df_obj="입력필요", xyxy=[1, 1]):
-		sheet_object = self.check_sheet_name(sheet_name)
+		"""
+		dataframe의 자료를 엑셀로 넘기는 것
+		"""
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 
 		col_list = df_obj.columns.values.tolist()
 		value_list = df_obj.values.tolist()
 		self.write_value_in_range(sheet_name, xyxy, [col_list])
 		self.write_value_in_range(sheet_name, [x1 + 1, y1], value_list)
 
 	def write_list1d_in_range(self, sheet_name="", xyxy="", input_list="입력필요"):
+		"""
+		1줄의 리스트는 가로로 나열된다
+		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
+		if x1==x2 and y1==y2:
+			min_y = len(input_list)
+		else:
+			min_y = min(len(input_list), y2-y1+1)
+		for y in range(min_y):
+			sheet_object.Cells(x1, y1+y).Value = input_list[y]
 
-		for x in range(len(input_list)):
-			sheet_object.Cells(x1 + x, y1).Value = input_list[x]
+	def write_list1d_in_yline(self, sheet_name="", xyxy="", input_datas="입력 필요"):
+		"""
+		"""
+		# 아래의 예제는 엑셀의 값중에서 y라인으로 자동으로 한줄을 넣는 기능이 없어서，만들어 보았다
+		#영역에 값는 넣기
+		sheet_object = self.check_sheet_name(sheet_name)
+		x1, y1, x2, y2 = self.check_address_value(xyxy)
+		for x in range(0, len(input_datas)):
+			sheet_object.Cells(x + x1, y1).Value = input_datas[x]
+
+	def write_list2d_in_range(self, sheet_name="", xyxy="", input_list="입력필요"):
+		"""
+		"""
+		self.write_list_in_range(sheet_name="", xyxy="", input_list="입력필요")
 
 	def write_list_in_range(self, sheet_name="", xyxy="", input_list="입력필요"):
+		"""
+		2차원의 값만 입력할 수 있다
+		"""
 		if type(input_list[0]) == type([]):
 			self.write_value_in_range(sheet_name, xyxy, input_list)
 		else:
-			self.write_value_in_range(sheet_name, xyxy, input_list)
+			self.write_value_in_range(sheet_name, xyxy, [input_list])
 
 	def write_memo_in_cell(self, sheet_name="", xyxy="", text="입력필요"):
+		"""
+		셀에 메모를 넣는것
+		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
 
 		my_range.AddComment(text)
 
-	def write_nansu_in_range(self, sheet_name="", xyxy="", input_data="입력필요"):
-		sheet_object = self.check_sheet_name(sheet_name)
+	def write_nansu_in_range(self, sheet_name="", xyxy="", input_list=[1,100]):
+		"""
+		입력한 숫자범위에서 난수를 만들어서 영역에 써주는것
+		"""
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 
-		no_start, no_end = input_data.split(",")
-		no_start = int(no_start.strip())
-		no_end = int(no_end.strip())
+		no_start, no_end = input_list
 		basic_data = list(range(no_start, no_end + 1))
 		random.shuffle(basic_data)
 		temp_no = 0
 		for x in range(x1, x2 + 1):
 			for y in range(y1, y2 + 1):
 				self.write_cell_value(sheet_name, [x, y], basic_data[temp_no])
 				if temp_no >= no_end - no_start:
 					random.shuffle(basic_data)
 					temp_no = 0
 				else:
 					temp_no = temp_no + 1
 
 	def write_value_in_activecell(self, value="입력필요"):
+		""" 활성화된 셀에 값는 넣기 """
 		self.get_activesheet_object()
-		x1, y1, x2, y2 = self.read_value_in_activecell()
-		self.write_value_in_cell("", [x1, y1], value)
-
-	def write_cell_value(self, sheet_name="", xyxy="", value="입력필요"):
-		self.write_value_in_cell(sheet_name, xyxy, value)
+		xy = self.read_address_in_activecell()
+		self.write_value_in_cell("", [xy[0], xy[1]], value)
 
 	def write_value_in_cell(self, sheet_name="", xyxy="", value="입력필요"):
+		""" 셀에 값는 넣기 """
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 
 		# 문자형식의 숫자인지를 확인하는 것
 		# 숫자와 문자가 모두 숫자형으로 인식하여서 첨가해야하는 것
 		if type(value) == type("abc"):
 			re_com = re.compile("^[0-9.]+$")
@@ -3070,30 +3652,67 @@
 			else:
 				changed_value = value
 		else:
 			changed_value = value
 		sheet_object.Cells(x1, y1).Value = changed_value
 
 	def write_value_in_range(self, sheet_name="", xyxy="", input_datas="입력필요"):
+		""" 영역에 값는 넣기 """
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 		changed_input_datas = self.change_inputdata_to_list2d(input_datas)
 
 		for x in range(0, len(changed_input_datas)):
 			for y in range(0, len(changed_input_datas[x])):
 				sheet_object.Cells(x + x1, y + y1).Value = changed_input_datas[x][y]
 
+	def write_dic_key_in_cell(self, sheet_name="", xyxy="", input_dic="입력필요"):
+		"""
+		사전으로 입력된 키값을 엑셀에 쓰는것
+		"""
+		sheet_object = self.check_sheet_name(sheet_name)
+		x1, y1, x2, y2 = self.check_address_value(xyxy)
+		changed_input_datas = list(input_dic.keys())
+
+		for x in range(0, len(changed_input_datas)):
+			sheet_object.Cells(x + x1, y1).Value = changed_input_datas[x]
+
+	def write_value_in_range_as_speedy(self, sheet_name="", xyxy="", input_datas="입력필요"):
+		"""
+		2022-12-23 : x1, y1이 잘못되어서 변경함
+		영역과 자료의 갯수중에서 작은것을 기준으로 값을 쓰는데
+		만약 영역이 셀하나이면 자료를 전부 쓴다
+		"""
+		sheet_object = self.check_sheet_name(sheet_name)
+		x1, y1, x2, y2 = self.check_address_value(xyxy)
+
+		min_x = min(x2-x1+1, len(input_datas))
+		min_y = min(y2-y1+1, len(input_datas[0]))
+
+		if x1 == x2 and y1 ==y2:
+			#셀이 영역을 선택하지 않았다면, 전체 자료를 전부 넣는다
+			changed_datas = input_datas
+			sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x1 + len(input_datas) - 1, y1 + len(input_datas[0]) - 1)).Value = changed_datas
+		else:
+			#영역을 선택하면, 두 영역중에 작은 부분을 기준으로 자료를 넣는다
+			changed_datas = []
+			for x in range(min_x):
+				changed_datas.append(input_datas[x][:min_y])
+			sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x1 + min_x - 1, y1 + min_y - 1)).Value = changed_datas
+
 	def write_value_in_range_by_range_priority(self, sheet_name="", xyxy="", input_datas="입력필요"):
 		"""
 		영역이 더 우선하는 것
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		checked_datas = self.change_inputdata_to_list2d(input_datas)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 
+		address_list = self.check_intersect_address(xyxy, input_datas)
+
 		x_len = len(checked_datas)
 		if (x2 - x1) <= x_len:
 			x_len = x2 - x1
 
 		y_len = len(checked_datas[0])
 		if (y2 - y1) <= y_len:
 			y_len = y2 - y1
@@ -3102,41 +3721,181 @@
 			for y in range(0, y_len):
 				sheet_object.Cells(x + x1, y + y1).Value = input_datas[x][y]
 
 	def write_value_in_range_by_trans(self, sheet_name="", xyxy="", input_list2d=""):
 		"""
 		입력자료의 xy를 바꿔서 입력하는 것
 		"""
+
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
-		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
-		aaa = self.write_value_in_range_by_trans(input_list2d)
-		for y in range(len(aaa)):
-			sheet_object.Range(sheet_object.Cells(x1, y + y1), sheet_object.Cells(x2, y + y1)).Value = input_list2d[y]
+
+		for x in range(x1, x2 + 1):
+			for y in range(y1, y2 + 1):
+				sheet_object.Cells(y, x).Value = input_list2d[x][y]
 
 	def write_value_in_range_xystep(self, sheet_name="", xyxy="", input_text="", xystep=[1, 1]):
 		"""
 		선택한 영역의 시작점부터 x,y 번째 셀마다 값을 넣기
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
-		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
 
 		for x in range(x1, x2 + 1):
 			if divmod(x, xystep[0])[1] == 0:
 				for y in range(y1, y2 + 1):
 					if divmod(y, xystep[1])[1] == 0:
 						sheet_object.Cells(x, y).Value = str(input_text)
 
-	def write_value_in_range_as_speedy(self, sheet_name="", xyxy="", input_datas="입력필요"):
-		sheet_object = self.check_sheet_name(sheet_name)
-		x1, y1, x2, y2 = self.check_address_value(xyxy)
-		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
-		checked_input_datas = self.yt.change_list1d_to_list2d(input_datas)
-		if y1 == y2 and x1 == x2:
-			sheet_object.Range(sheet_object.Cells(x1, y1),
-			                 sheet_object.Cells(y1 + len(checked_input_datas) - 1,
-			                                  x1 + len(checked_input_datas[0]) - 1)).Value = checked_input_datas
-		else:
-			if (y2 - y1) <= len(checked_input_datas[0]) and (y2 - y1) <= len(
-					checked_input_datas[0]):
-				pass
+	def open_file(self, filename=""):
+		"""
+		"""
+		self.path_full = self.check_filepath(filename)
+		self.file_name_only = self.path_full.split("/")[-1]
+		if filename.lower() == 'new'or filename == "":
+			#빈것으로 된 경우는 새로운 workbook < 연다는 뜻으로 해석
+			try:
+				self.xlapp.Windowstate = -4137
+				self.xlbook = self.xlapp.WorkBooks.Add()
+			except:
+				win32gui.MessageBox(0, "There is no Activeworkbook", "www.halmoney.com", 0)
+		else:
+				#	열린 화일중에 같은것이 있는지 확인하는 것
+				file_name_list = self.read_opened_workbook_filename_all()
+				if self.file_name_only in file_name_list:
+					pass
+				else:
+					try:
+						self.xlbook = self.xlapp.Workbooks.Open(self.path_full)
+					except:
+						win32gui.MessageBox(0, "화일이름이나 경로를 다시한번 확인해 보시기 바랍니다”, .halmoney.com", 0)
+
+	################################################################
+
+	def close_excel(self):
+		"""
+		열려진 화일을 닫는것
+		"""
+		self.xlbook.Close(SaveChanges=0)
+		del self.xlapp
+
+	def close_activeworkbook(self):
+		"""
+		열려진 화일을 닫는것
+		"""
+		self.xlbook.Close(SaveChanges=0)
+
+	def change_active_workbook(self, input_file_name):
+		"""
+		열려진 워드 화일중 이름으로 선택하는것
+		"""
+		self.xlapp.Visible = True
+		win32gui.SetForegroundWindow(self.xlapp.hwnd)
+		self.xlapp.WorkBooks(input_file_name).Activate()
+		self.xlapp.WindowState = win32com.client.constants.xlMaximized
+
+	def make_password(self, isnum="yes", istext_small="yes", istext_big="yes", isspecial="no", len_num=10):
+		"""
+		엑셀시트의 암호를 풀기위해 암호를 계속 만들어서 확인하는 것
+		"""
+		check_char = []
+		if isnum == "yes":
+			check_char.extend(list(string.digits))
+		if istext_small == "yes":
+			check_char.extend(list(string.ascii_lowercase))
+		if istext_big == "yes":
+			check_char.extend(list(string.ascii_uppercase))
+		if isspecial == "yes":
+			for one in "!@#$%^*_-":
+				check_char.extend(one)
+
+		zz = combinations_with_replacement(check_char, len_num)
+		for aa in zz:
+			try:
+				pswd = "".join(aa)
+				#print(pswd)
+				self.unlock_sheet("", pswd)
+				break
+				print("발견", pswd)
+			except:
+				pass
+
+
+	def check_same_data(self, input_list, check_line = 10):
+		"""
+		엑셀의 선택한 자료에서 여러줄을 기준으로 같은 자료만 갖고오기
+		"""
+		result = []
+		base_value = ""
+		xy = self.read_address_in_activecell()
+		for no in input_list:
+			base_value = base_value + str(self.read_cell_value("", [xy[0], no]))
+
+		# 혹시 1보다 작은 숫자가 나올 수있으므로, 최소시작점을 1로하기위해
+		start_x = max(int(xy[0]) - check_line, 1)
+
+		# 위로10개 아래로 10개의 자료를 확인한다
+		for no in range(start_x, start_x+20):
+			cell_value=""
+			for one in input_list:
+				cell_value = cell_value + str(self.read_cell_value("", [no, one]))
+			if base_value == cell_value:
+				# 보통 50개이상의 줄을 사용하지 않으므로 50개를 갖고온다
+				temp = self.read_value_in_range("", [no, 1, no, 50])
+				result.append(temp[0])
+		return result
+
+	def check_differ_at_same_area(self, input_sa1, input_sa2):
+		"""
+		동일한 사이즈의 다른 영역에서 다른 것만 색칠하기
+		"""
+		datal = self.read_value_in_range(input_sa1[0], input_sa1[1])
+		data2 = self.read_value_in_range(input_sa2[0], input_sa2[1])
+		start_x = input_sa2[1][0]
+		start_y = input_sa2[1][1]
+		for x in range(len(datal)):
+			for y in range(len(datal[0])):
+				if datal[x][y] == data2[x][y]:
+					pass
+				else:
+					self.paint_cell_by_excel_colorno(input_sa2[0], [x + start_x, y + start_y], 3)
+
+	def concate_xlne(self, input_list2d, xy):
+		"""
+		# 선택한 영역의 세로자료들을 다 더해서 제일위의 셀에 다시 넣는것
+		"""
+		x_len = len(input_list2d)
+		y_len = len(input_list2d[0])
+		for y in range(y_len):
+			temp = ""
+			for x in range(x_len):
+				self.write_value_in_cell("", [x + xy[0], y + xy[1]], "")
+				if input_list2d[x][y]:
+					print(input_list2d[x][y])
+					temp = temp + " " + input_list2d[x][y]
+			print(temp)
+			self.write_value_in_cell("", [xy[0], y + xy[1]], str(temp).strip())
+
+	def write_serial_no_by_step(self, xyxy, start_no, step = 1):
+		"""
+		선택한 영역에 시작번호, 간격으로 이루어진 연속된 숫자를 쓰는것
+		"""
+		new_no = start_no
+		for no in range(0, xyxy[2]-xyxy[0]+1):
+			self.write_value_in_cell("", [xyxy[0]+no, xyxy[1]], new_no)
+			new_no = new_no + step
+			print([xyxy[0]+no, xyxy[1]], new_no)
+
+	def split_partial_value_in_range_by_step_from_start(self, sheet_name, xyxy, n_char):
+		"""
+		어떤 자료중에 앞에서 몇번째것들만 갖고오고 싶을때
+		예:시군구 자료에서 앞의 2글자만 분리해서 얻어오는 코드
+		"""
+		list_2d = self.read_value_in_range(sheet_name, xyxy)
+		result = set()
+		for list_1d in list_2d:
+			for one in list_1d:
+				try:
+					result.add(one[0:n_char])
+				except:
+					pass
+		return list(result)
```

### Comparing `halmoney-2.1.1/src/halmoney/pcell_event.py` & `halmoney-3.0.0/src/halmoney/pcell_event.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
-import time
-import pythoncom
-import win32com.client as win32
+import time  #내장모듈
+
+import pythoncom #pywin32의 모듈
+import win32com.client as win32 #pywin32의 모듈
 
 class ApplicationEvents:
     def OnNewWorkbook(self, *args):
         print("Application Event => OnNewWorkbook, 엑셀->새로운 워크북")
 
     def OnSheetActivate(self, *args):
         print("Application Event => OnSheetActivate, 엑셀->다른 시트로 이동")
```

### Comparing `halmoney-2.1.1/src/halmoney.egg-info/PKG-INFO` & `halmoney-3.0.0/src/halmoney.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: halmoney
-Version: 2.1.1
+Version: 3.0.0
 Summary: Easy Read / Write for Excel, Word, Color, Etc using Python
 Home-page: https://github.com/sjpark/halmoney
-Download-URL: https://github.com/sjpark/halmoney/archive/v2.1.1.tar.gz
+Download-URL: https://github.com/sjpark/halmoney/archive/v3.0.0.tar.gz
 Author: sjpark
 Author-email: sjpkorea@yahoo.com
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 
 ## Halmoney 모듈에 대하여
@@ -24,22 +24,25 @@
 또한 보통 많이 사용하는 코드들은 첨부된 sample코드를 보시거나 저의 사이트에 와서 비슷한것을 다운 받은후
 변경해서 사용하시기를 추천 드립니다
 
 좀더 편한 업무의 일을 하기위한 것입니다
 
 ### 구성은 
 
+    - anydb : sqlite와 pandas 를 좀더 쉽게 사용할수있도록 만든것
+    - basic_data : halmoney패키지에서 사용되는 전반적인 공유 자료들을 저장하는 곳
+    - ganada : 워드를 다루기위해 만든 것
+    - jfinder : 정규표현식을 좀더 편하게 사용하도록 만든 것
+    - mailmail : outlook을 다루는것
     - pcell : 엑셀을 다루는 것
     - pcell_event : 엑셀의 이벤트를 다루는것
+    - pyclick : 키보드와 마우스를 다루는 모듈
+    - pynal : 시간과 날짜를 다루는것
     - scolor : 색의 RGB값을 편하게 사용가능하도록 만든 것
-    - jfinder : 정규표현식을 좀더 편하게 사용하도록 만든 것
     - youtil : 이러저런 문장이나 시간등을 변환하는데 도움이되는 것
-    - mail : outlook을 다루는것
-    - pynal : 시간과 날짜를 다루는것
-    - anydb : sqlite와 pandas 를 좀더 쉽게 사용할수있도록 만든것
 
 각 사용사용방법들에 대해서는 아래의 사이트를 참고하세요
 
 * https://cafe.naver.com/pycell
 * www.halmoney.com
```

