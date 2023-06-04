# Comparing `tmp/rfswarm-reporter-1.1.2.tar.gz` & `tmp/rfswarm-reporter-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rfswarm-reporter-1.1.2.tar", last modified: Fri May 19 05:26:26 2023, max compression
+gzip compressed data, was "rfswarm-reporter-1.1.3.tar", last modified: Sun Jun  4 05:25:59 2023, max compression
```

## Comparing `rfswarm-reporter-1.1.2.tar` & `rfswarm-reporter-1.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-19 05:26:26.530295 rfswarm-reporter-1.1.2/
--rw-r--r--   0 dave      (1000) dave      (1000)    35149 2023-02-10 08:46:44.000000 rfswarm-reporter-1.1.2/LICENSE
--rw-rw-r--   0 dave      (1000) dave      (1000)     3110 2023-05-19 05:26:26.530295 rfswarm-reporter-1.1.2/PKG-INFO
--rw-r--r--   0 dave      (1000) dave      (1000)     5809 2023-05-19 05:23:33.000000 rfswarm-reporter-1.1.2/README.md
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-19 05:26:26.526295 rfswarm-reporter-1.1.2/rfswarm_reporter/
--rw-r--r--   0 dave      (1000) dave      (1000)       53 2023-05-19 05:26:24.000000 rfswarm-reporter-1.1.2/rfswarm_reporter/__init__.py
--rw-r--r--   0 dave      (1000) dave      (1000)   311404 2023-05-19 05:26:24.000000 rfswarm-reporter-1.1.2/rfswarm_reporter/rfswarm_reporter.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-19 05:26:26.530295 rfswarm-reporter-1.1.2/rfswarm_reporter.egg-info/
--rw-rw-r--   0 dave      (1000) dave      (1000)     3110 2023-05-19 05:26:26.000000 rfswarm-reporter-1.1.2/rfswarm_reporter.egg-info/PKG-INFO
--rw-rw-r--   0 dave      (1000) dave      (1000)      343 2023-05-19 05:26:26.000000 rfswarm-reporter-1.1.2/rfswarm_reporter.egg-info/SOURCES.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-05-19 05:26:26.000000 rfswarm-reporter-1.1.2/rfswarm_reporter.egg-info/dependency_links.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)       80 2023-05-19 05:26:26.000000 rfswarm-reporter-1.1.2/rfswarm_reporter.egg-info/entry_points.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)       85 2023-05-19 05:26:26.000000 rfswarm-reporter-1.1.2/rfswarm_reporter.egg-info/requires.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)       17 2023-05-19 05:26:26.000000 rfswarm-reporter-1.1.2/rfswarm_reporter.egg-info/top_level.txt
--rw-r--r--   0 dave      (1000) dave      (1000)     1504 2023-05-19 05:26:24.000000 rfswarm-reporter-1.1.2/setup-reporter.py
--rw-rw-r--   0 dave      (1000) dave      (1000)       38 2023-05-19 05:26:26.530295 rfswarm-reporter-1.1.2/setup.cfg
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-04 05:25:59.893687 rfswarm-reporter-1.1.3/
+-rw-r--r--   0 dave      (1000) dave      (1000)    35149 2023-02-10 08:46:44.000000 rfswarm-reporter-1.1.3/LICENSE
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3158 2023-06-04 05:25:59.893687 rfswarm-reporter-1.1.3/PKG-INFO
+-rw-r--r--   0 dave      (1000) dave      (1000)     5809 2023-06-04 04:58:34.000000 rfswarm-reporter-1.1.3/README.md
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-04 05:25:59.893687 rfswarm-reporter-1.1.3/rfswarm_reporter/
+-rw-r--r--   0 dave      (1000) dave      (1000)       53 2023-06-04 05:25:57.000000 rfswarm-reporter-1.1.3/rfswarm_reporter/__init__.py
+-rw-r--r--   0 dave      (1000) dave      (1000)   312855 2023-06-04 05:25:57.000000 rfswarm-reporter-1.1.3/rfswarm_reporter/rfswarm_reporter.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-04 05:25:59.893687 rfswarm-reporter-1.1.3/rfswarm_reporter.egg-info/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3158 2023-06-04 05:25:59.000000 rfswarm-reporter-1.1.3/rfswarm_reporter.egg-info/PKG-INFO
+-rw-rw-r--   0 dave      (1000) dave      (1000)      343 2023-06-04 05:25:59.000000 rfswarm-reporter-1.1.3/rfswarm_reporter.egg-info/SOURCES.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-06-04 05:25:59.000000 rfswarm-reporter-1.1.3/rfswarm_reporter.egg-info/dependency_links.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       80 2023-06-04 05:25:59.000000 rfswarm-reporter-1.1.3/rfswarm_reporter.egg-info/entry_points.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       85 2023-06-04 05:25:59.000000 rfswarm-reporter-1.1.3/rfswarm_reporter.egg-info/requires.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       17 2023-06-04 05:25:59.000000 rfswarm-reporter-1.1.3/rfswarm_reporter.egg-info/top_level.txt
+-rw-r--r--   0 dave      (1000) dave      (1000)     1504 2023-06-04 05:25:57.000000 rfswarm-reporter-1.1.3/setup-reporter.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)       38 2023-06-04 05:25:59.897687 rfswarm-reporter-1.1.3/setup.cfg
```

### Comparing `rfswarm-reporter-1.1.2/LICENSE` & `rfswarm-reporter-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rfswarm-reporter-1.1.2/PKG-INFO` & `rfswarm-reporter-1.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rfswarm-reporter
-Version: 1.1.2
+Version: 1.1.3
 Summary: rfswarm reporter
 Home-page: https://github.com/damies13/rfswarm
 Author: damies13
 Author-email: damies13+rfswarm@gmail.com
 License: UNKNOWN
 Project-URL: Getting Help, https://github.com/damies13/rfswarm#getting-help
 Project-URL: Say Thanks!, https://github.com/damies13/rfswarm#donations
@@ -41,15 +41,15 @@
 ### Community Support
 
 - [rfswarm Documentation](https://github.com/damies13/rfswarm/blob/master/Doc/README.md)
 - [Discord](https://discord.gg/jJfCMrqCsT)
 - [Reporting Issues / Known Issues](https://github.com/damies13/rfswarm/issues)
 
 <kbd align="centre">
-<img align="centre" height="350" src="Doc/Images/Manager&Agent_Example.png">
+<img align="centre" height="350" src="https://github.com/damies13/rfswarm/blob/master/Doc/Images/Manager&Agent_Example.png">
 </kbd><br>
 An example of how your rfswarm setup might look.
 
 ### Commercial Support
 - The easiest way to get commercial support is to sponsor this project on [GitHub](https://github.com/sponsors/damies13?frequency=recurring&sponsor=damies13)
```

### Comparing `rfswarm-reporter-1.1.2/README.md` & `rfswarm-reporter-1.1.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 |Version|Manager|Agent|Reporter|
 |---|---|---|---|
 |[![Latest PyPI version](https://img.shields.io/pypi/v/rfswarm-manager.svg)](https://pypi.python.org/pypi/rfswarm-manager/) | [![Number of Manager PyPI downloads](https://img.shields.io/pypi/dm/rfswarm-manager.svg)](https://pypi.python.org/pypi/rfswarm-manager/) | [![Number of Agent PyPI downloads](https://img.shields.io/pypi/dm/rfswarm-agent.svg)](https://pypi.python.org/pypi/rfswarm-agent/) | [![Number of Reporter PyPI downloads](https://img.shields.io/pypi/dm/rfswarm-reporter.svg)](https://pypi.python.org/pypi/rfswarm-reporter/) |
 
 | Master | Branch |
 | -- | -- |
-| [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/superlinter.yml?branch=master&label=Linter)](https://github.com/damies13/rfswarm/actions/workflows/superlinter.yml) | ![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/superlinter.yml?branch=v1.1.2&label=Linter) |
-| [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/Regression_Tests.yml?branch=master&label=Regression%20Tests)](https://github.com/damies13/rfswarm/actions/workflows/Regression_Tests.yml) | ![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/Regression_Tests.yml?branch=v1.1.2&label=Regression%20Tests) |
+| [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/superlinter.yml?branch=master&label=Linter)](https://github.com/damies13/rfswarm/actions/workflows/superlinter.yml) | ![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/superlinter.yml?branch=v1.1.3&label=Linter) |
+| [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/Regression_Tests.yml?branch=master&label=Regression%20Tests)](https://github.com/damies13/rfswarm/actions/workflows/Regression_Tests.yml) | ![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/Regression_Tests.yml?branch=v1.1.3&label=Regression%20Tests) |
 
 <img align="right" src="Doc/Images/Icon_Information.png">
 
 ## About
 rfswarm is a testing tool that allows you use [Robot Framework](https://robotframework.org/) test cases for performance or load testing.
 
 > _Swarm being the collective noun for Robots, just as Flock is for Birds and Herd for Sheep, so it made sense to use swarm for a performance testing tool using Robot Framework, hence rfswarm_
```

### Comparing `rfswarm-reporter-1.1.2/rfswarm_reporter/rfswarm_reporter.py` & `rfswarm-reporter-1.1.3/rfswarm_reporter/rfswarm_reporter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 #
 # 	Robot Framework Swarm
 # 		Reporter
-#    Version 1.1.2
+#    Version 1.1.3
 #
 
 import argparse
 import base64  # used for embedding images  # used for xhtml export
 import configparser
 import inspect
 import math
@@ -114,15 +114,15 @@
 			base.debugmsg(8, "res:", res)
 			return res
 		except Exception as e:
 			base.debugmsg(5, "Exception:", e)
 
 
 class ReporterBase():
-	version = "1.1.2"
+	version = "1.1.3"
 	debuglvl = 0
 
 	save_ini = True
 	running = True
 	displaygui = True
 	gui = None
 	darkmode = False
@@ -643,14 +643,15 @@
 
 	def report_subsection_parent(self, id):
 		pid = id
 		last = id[-1:]
 		if last in ['G', 'H', 'I', 'J', 'k', 'L', 'M', 'N', 'O', 'P', 'Q', 'R', 'S', 'T', 'U', 'V', 'W', 'X', 'Y', 'Z']:
 			pid = id[0:-1]
 			self.report_add_subsection(id)
+		base.debugmsg(8, "id:", id, "	pid:", pid)
 		return pid
 
 	def report_add_section(self, parent, id, name):
 		base.debugmsg(7, "parent: ", parent)
 		if id not in base.report:
 			base.report[id] = {}
 		base.report[id]['Name'] = base.whitespace_set_ini_value(name)
@@ -938,14 +939,17 @@
 			EnFA = self.rt_table_get_enfa(id)
 			FAType = self.rt_table_get_fa(id)
 			FNType = self.rt_table_get_fn(id)
 			inpFP = self.rt_table_get_fp(id)
 			colname = "Name"
 
 			sql = "SELECT "
+
+			base.debugmsg(8, "RType:", RType, "sql:", sql)
+
 			if RType == "Response Time":
 				sql += "end_time as 'Time' "
 				sql += ", elapsed_time as 'Value' "
 				# sql += ", result_name as 'Name' "
 				sql += ", result_name"
 				if EnFR and FRType in [None, "", "None"]:
 					sql += " || ' - ' || result"
@@ -988,25 +992,29 @@
 				# sql += ", result as 'Name' "
 				sql += ", result"
 				if EnFR and FRType in [None, "", "None"]:
 					sql += " || ' - ' || result"
 				if EnFA and FAType in [None, "", "None"]:
 					sql += " || ' - ' || agent"
 				sql += " as [" + colname + "] "
-			if RType is None:
+
+			if RType in [None, "", "None"]:
+				base.debugmsg(8, "RType:", RType, "sql:", sql)
 				sql += "end_time as 'Time'"
 				sql += ", count(result) as 'Value' "
 				# sql += ", result_name as 'Name' "
 				sql += ", result_name"
 				if EnFR and FRType in [None, "", "None"]:
 					sql += " || ' - ' || result"
 				if EnFA and FAType in [None, "", "None"]:
 					sql += " || ' - ' || agent"
 				sql += " as [" + colname + "] "
 
+			base.debugmsg(8, "RType:", RType, "sql:", sql)
+
 			sql += "FROM Results "
 
 			lwhere = []
 			if FRType == "Pass":
 				# sql += "WHERE result == 'PASS' "
 				lwhere.append("result == 'PASS'")
 			if FRType == "Fail":
@@ -1046,15 +1054,15 @@
 			for iwhere in lwhere:
 				if i == 0:
 					sql += "WHERE {} ".format(iwhere)
 				else:
 					sql += "AND {} ".format(iwhere)
 				i += 1
 
-			if RType is not None:
+			if RType not in [None, "", "None"]:
 				# sql += "GROUP by "
 				# sql += 		", result "
 				pass
 			if RType == "Response Time":
 				# sql += 		"result_name "
 				pass
 
@@ -1086,45 +1094,48 @@
 			mnamecolumns = []
 			# mcolumns = ["MetricTime as 'Time'", "MetricValue as 'Value'", "PrimaryMetric as 'Name'", "MetricType as 'Name'", "SecondaryMetric as 'Name'"]
 			mcolumns = ["MetricTime as 'Time'", "MetricValue as 'Value'"]
 			wherelst = []
 			# grouplst = ["PrimaryMetric", "MetricType", "SecondaryMetric"]
 			grouplst = []
 
-			if MType is not None and len(MType) > 0:
+			if MType not in [None, "", "None"] and len(MType) > 0:
 				# if "MetricType as 'Name'" in mcolumns:
 				# 	mcolumns.remove("MetricType as 'Name'")
 				wherelst.append("MetricType == '{}'".format(MType.replace("'", "''")))
 				if "MetricType" in grouplst:
 					grouplst.remove("MetricType")
 			else:
 				mnamecolumns.append("MetricType")
-			if PM is not None and len(PM) > 0:
+			if PM not in [None, "", "None"] and len(PM) > 0:
 				# if "PrimaryMetric as 'Name'" in mcolumns:
 				# 	mcolumns.remove("PrimaryMetric as 'Name'")
 				wherelst.append("PrimaryMetric == '{}'".format(PM.replace("'", "''")))
 				if "PrimaryMetric" in grouplst:
 					grouplst.remove("PrimaryMetric")
 			else:
 				mnamecolumns.append("PrimaryMetric")
-			if SM is not None and len(SM) > 0:
+			if SM not in [None, "", "None"] and len(SM) > 0:
 				# if "SecondaryMetric as 'Name'" in mcolumns:
 				# 	mcolumns.remove("SecondaryMetric as 'Name'")
 				wherelst.append("SecondaryMetric == '{}'".format(SM.replace("'", "''")))
 				if "SecondaryMetric" in grouplst:
 					grouplst.remove("SecondaryMetric")
 			else:
 				mnamecolumns.append("SecondaryMetric")
 
 			if EnFA:
 				if FAType in [None, "", "None"]:
 					mnamecolumns.append("DataSource")
 				else:
 					wherelst.append("DataSource == '{}'".format(FAType))
 
+			if len(mnamecolumns) < 1:
+				mnamecolumns.append("'" + SM + "'")
+
 			# Construct Name Column
 			mnamecolumn = " || ' - ' || ".join(mnamecolumns)
 			mnamecolumn += " as [" + colname + "] "
 			mcolumns.append(mnamecolumn)
 
 			if FNType not in [None, "", "None"] and len(inpFP) > 0:
 				# construct pattern
@@ -1298,15 +1309,15 @@
 			if RType == "Total TPS":
 				colname = "Result "
 				sql += "result "
 				if EnFA and FAType in [None, "", "None"]:
 					sql += " || ' - ' || agent"
 				sql += " as [" + colname + "] "
 				sql += ", count(result)  as 'Count' "
-			if RType is None:
+			if RType in [None, "", "None"]:
 				sql = ""
 				return sql
 
 			sql += "FROM Results "
 
 			lwhere = []
 			if EnFR:
@@ -1350,15 +1361,15 @@
 			for iwhere in lwhere:
 				if i == 0:
 					sql += "WHERE {} ".format(iwhere)
 				else:
 					sql += "AND {} ".format(iwhere)
 				i += 1
 
-			if RType is not None:
+			if RType not in [None, "", "None"]:
 				sql += "GROUP by "
 
 			if RType == "Response Time":
 				sql += "[" + colname + "] "
 			if RType == "TPS":
 				sql += "[" + colname + "] "
 				sql += ", result "
@@ -1389,33 +1400,39 @@
 			if EnFA:
 				if FAType in [None, "", "None"]:
 					mcolumns.append("DataSource 'Agent'")
 					grouplst.append("DataSource")
 				else:
 					wherelst.append("DataSource == '{}'".format(FAType))
 
-			if MType is not None and len(MType) > 0:
+			if MType not in [None, "", "None"] and len(MType) > 0:
 				if "MetricType" in mcolumns:
 					mcolumns.remove("MetricType")
 				wherelst.append("MetricType == '{}'".format(MType))
 				if "MetricType" in grouplst:
 					grouplst.remove("MetricType")
-			if PM is not None and len(PM) > 0:
+			if PM not in [None, "", "None"] and len(PM) > 0:
 				if "PrimaryMetric" in mcolumns:
 					mcolumns.remove("PrimaryMetric")
 				wherelst.append("PrimaryMetric == '{}'".format(PM))
 				if "PrimaryMetric" in grouplst:
 					grouplst.remove("PrimaryMetric")
-			if SM is not None and len(SM) > 0:
+			if SM not in [None, "", "None"] and len(SM) > 0:
 				if "SecondaryMetric" in mcolumns:
 					mcolumns.remove("SecondaryMetric")
 				wherelst.append("SecondaryMetric == '{}'".format(SM))
 				if "SecondaryMetric" in grouplst:
 					grouplst.remove("SecondaryMetric")
 
+
+			if len(mcolumns) < 1:
+				# mcolumns.append("'" + SM + "'")
+				mcolumns.append("SecondaryMetric")
+				grouplst.append("SecondaryMetric")
+
 			if colours:
 				colourcolumn = " || ' - ' || ".join(grouplst)
 				colourcolumn += " as [Colour] "
 				mcolumns.append(colourcolumn)
 
 			if FNType not in [None, "", "None"] and len(inpFP) > 0:
 				# construct pattern
@@ -5651,15 +5668,15 @@
 			cp.start()
 
 	#
 	# Settings	-	DataTable
 	#
 
 	def cs_datatable(self, id):
-		base.debugmsg(9, "id:", id)
+		base.debugmsg(8, "id:", id)
 		colours = base.rt_table_get_colours(id)
 		datatype = base.rt_table_get_dt(id)
 		self.contentdata[id]["LFrame"].columnconfigure(99, weight=1)
 		rownum = 0
 
 		rownum += 1
 		self.contentdata[id]["lblColours"] = ttk.Label(self.contentdata[id]["LFrame"], text="Show graph colours:")
@@ -5680,17 +5697,20 @@
 		self.contentdata[id]["strDT"].set(datatype)
 		self.contentdata[id]["omDT"].grid(column=1, row=rownum, sticky="nsew")
 
 		rownum += 1
 		self.contentdata[id]["DTFrame"] = rownum
 		self.cs_datatable_switchdt(id)
 
-	def cs_datatable_update(self, _event=None):
-		base.debugmsg(5, "_event:", _event)
+	def cs_datatable_update(self, _event=None, *args):
+		base.debugmsg(5, "_event:", _event, "	args:", args)
 		changes = 0
+		# if len(args) > 0:
+		# 	base.debugmsg(8, "args[0]:", args[0])
+		# 	changes += args[0]
 		id = self.sectionstree.focus()
 		if _event is not None:
 			name = base.report_item_get_name(_event)
 			if name is not None:
 				id = _event
 		base.debugmsg(9, "id:", id)
 		if "intColours" in self.contentdata[id]:
@@ -5752,21 +5772,26 @@
 			changes += base.rt_table_set_fp(id, value)
 
 		base.debugmsg(5, "changes:", changes)
 		if "strDT" in self.contentdata[id]:
 			datatype = self.contentdata[id]["strDT"].get()
 			changes += base.rt_table_set_dt(id, datatype)
 
+			base.debugmsg(8, "datatype:", datatype)
+
 			if datatype == "Metric":
 				self.cs_datatable_update_metrics(id)
 
 			if datatype != "SQL":
 				time.sleep(0.1)
 				base.rt_table_generate_sql(id)
 
+			# if changes > 0:
+			# 	self.cs_datatable_switchdt(id)
+
 		base.debugmsg(5, "changes:", changes)
 		if "tSQL" in self.contentdata[id]:
 			data = self.contentdata[id]["tSQL"].get('0.0', tk.END).strip()
 			base.debugmsg(5, "data:", data)
 			changes += base.rt_table_set_sql(id, data)
 		else:
 			time.sleep(0.1)
@@ -5865,35 +5890,41 @@
 		base.debugmsg(5, "_event:", _event)
 		rownum = 0
 		id = self.sectionstree.focus()
 		if _event is not None:
 			name = base.report_item_get_name(_event)
 			if name is not None:
 				id = _event
-		base.debugmsg(9, "id:", id)
+		base.debugmsg(8, "id:", id)
+		# self.cs_datatable_update(id, 1)
 		self.cs_datatable_update(id)
 		datatype = self.contentdata[id]["strDT"].get()
 		base.debugmsg(5, "datatype:", datatype)
 		if "Frames" not in self.contentdata[id]:
 			self.contentdata[id]["Frames"] = {}
 
 		# Forget
 		for frame in self.contentdata[id]["Frames"].keys():
 			self.contentdata[id]["Frames"][frame].grid_forget()
-			self.contentdata[id]["Frames"] = {}
+			# self.contentdata[id]["Frames"] = {}
+			# del self.contentdata[id]["Frames"][frame]
+		self.contentdata[id]["Frames"] = {}
 
+		base.debugmsg(8, "id:", id, "Frames:", self.contentdata[id]["Frames"])
+
+		base.debugmsg(8, "id:", id, "Construct")
 		# Construct
 		if datatype not in self.contentdata[id]["Frames"]:
 			rownum = 0
 			self.contentdata[id]["Frames"][datatype] = tk.Frame(self.contentdata[id]["LFrame"])
 			# self.contentdata[id]["Frames"][datatype].config(bg="SlateBlue3")
 			# self.contentdata[id]["Frames"][datatype].columnconfigure(0, weight=1)
 			self.contentdata[id]["Frames"][datatype].columnconfigure(99, weight=1)
 
-			# "Metric", "Result", "SQL"
+			base.debugmsg(8, "datatype:", datatype)
 
 			if datatype == "Metric":
 
 				showmetricagents = 0
 				if "DBTable" in base.settings and "Metrics" in base.settings["DBTable"] and "DataSource" in base.settings["DBTable"]["Metrics"]:
 					showmetricagents = base.settings["DBTable"]["Metrics"]["DataSource"]
 
@@ -6083,14 +6114,15 @@
 				rownum += 1
 				self.contentdata[id]["tSQL"] = tk.Text(self.contentdata[id]["Frames"][datatype])
 				self.contentdata[id]["tSQL"].grid(column=0, row=rownum, columnspan=100, sticky="nsew")
 				# data = self.contentdata[id]["tSQL"].insert('0.0', sql)
 				self.contentdata[id]["tSQL"].bind('<Leave>', self.cs_datatable_update)
 				self.contentdata[id]["tSQL"].bind('<FocusOut>', self.cs_datatable_update)
 
+		base.debugmsg(8, "id:", id, "renamecols 1")
 		if "renamecols" not in self.contentdata[id]["Frames"] and datatype not in ["SQL"]:
 			base.debugmsg(5, "create renamecols frame")
 			rownum = 0
 			self.contentdata[id]["Frames"]["renamecols"] = tk.Frame(self.contentdata[id]["LFrame"])
 			self.contentdata[id]["Frames"]["renamecols"].columnconfigure(99, weight=1)
 
 			self.contentdata[id]["lblspacer"] = ttk.Label(self.contentdata[id]["Frames"]["renamecols"], text=" ")
@@ -6107,20 +6139,24 @@
 			self.contentdata[id]["lbldispnme"] = ttk.Label(self.contentdata[id]["Frames"]["renamecols"], text="Display Name")
 			self.contentdata[id]["lbldispnme"].grid(column=1, row=rownum, sticky="nsew")
 
 			self.contentdata[id]["renamecolumns"] = {}
 			self.contentdata[id]["renamecolumns"]["startrow"] = rownum + 1
 			self.contentdata[id]["renamecolumns"]["rownum"] = rownum + 1
 
+		base.debugmsg(8, "id:", id, "renamecols 2")
 		if datatype not in ["SQL"]:
 			self.cs_datatable_add_renamecols(id)
+			base.debugmsg(8, "id:", id, "renamecols 2 debug 1")
 			# cp = threading.Thread(target=lambda: self.cs_datatable_add_renamecols(id))
 			# cp.start()
 			self.contentdata[id]["Frames"]["renamecols"].grid(column=0, row=self.contentdata[id]["DTFrame"] + 1, columnspan=100, sticky="nsew")
+			base.debugmsg(8, "id:", id, "renamecols 2 debug 2")
 
+		base.debugmsg(8, "id:", id, "Update")
 		# Update
 		if datatype == "SQL":
 			sql = base.rt_table_get_sql(id)
 			self.contentdata[id]["tSQL"].delete('0.0', tk.END)
 			self.contentdata[id]["tSQL"].insert('0.0', sql)
 
 		if datatype == "Result":
@@ -6150,26 +6186,31 @@
 			self.contentdata[id]["PMetric"].set(base.rt_table_get_pm(id))
 			self.contentdata[id]["SMetric"].set(base.rt_table_get_sm(id))
 			self.contentdata[id]["intFA"].set(base.rt_table_get_enfa(id))
 			self.contentdata[id]["FAType"].set(base.rt_table_get_fa(id))
 			self.contentdata[id]["FNType"].set(base.rt_table_get_fn(id))
 			self.contentdata[id]["FPattern"].set(base.rt_table_get_fp(id))
 
+		base.debugmsg(8, "id:", id, "Show")
 		# Show
 		self.contentdata[id]["Frames"][datatype].grid(column=0, row=self.contentdata[id]["DTFrame"], columnspan=100, sticky="nsew")
 
 	def cs_datatable_add_renamecols(self, id):
 		base.debugmsg(5, "id:", id)
 		if "renamecolumns" in self.contentdata[id]:
 			datatype = base.rt_table_get_dt(id)
 
 			if datatype == "SQL":
 				sql = base.rt_table_get_sql(id)
+				if len(sql.strip()) < 1:
+					return None
 			else:
 				sql = base.rt_table_generate_sql(id)
+				if len(sql.strip()) < 1:
+					return None
 				sql += " LIMIT 1 "
 
 			base.debugmsg(5, "sql:", sql)
 			key = "{}_{}_{}".format(id, base.report_item_get_changed(id), datetime.now().timestamp())
 			base.dbqueue["Read"].append({"SQL": sql, "KEY": key})
 
 			if "colnames" not in self.contentdata[id]["renamecolumns"]:
@@ -6897,14 +6938,15 @@
 			self.contentdata[itm]["Changed"] = 0
 		self.content_preview("TOP")
 
 	def cp_generate_preview(self, id):
 		base.debugmsg(8, "id:", id)
 		pid, idl, idr = base.rt_graph_LR_Ids(id)
 
+		base.debugmsg(8, "pid:", pid, "	idl:", idl, "	idr:", idr)
 		# if id not in self.contentdata:
 		while id not in self.contentdata:
 			time.sleep(0.1)
 			self.contentdata[pid] = {}
 		if "Changed" not in self.contentdata[pid]:
 			self.contentdata[pid]["Changed"] = 0
 		while idl not in self.contentdata:
```

### Comparing `rfswarm-reporter-1.1.2/rfswarm_reporter.egg-info/PKG-INFO` & `rfswarm-reporter-1.1.3/rfswarm_reporter.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rfswarm-reporter
-Version: 1.1.2
+Version: 1.1.3
 Summary: rfswarm reporter
 Home-page: https://github.com/damies13/rfswarm
 Author: damies13
 Author-email: damies13+rfswarm@gmail.com
 License: UNKNOWN
 Project-URL: Getting Help, https://github.com/damies13/rfswarm#getting-help
 Project-URL: Say Thanks!, https://github.com/damies13/rfswarm#donations
@@ -41,15 +41,15 @@
 ### Community Support
 
 - [rfswarm Documentation](https://github.com/damies13/rfswarm/blob/master/Doc/README.md)
 - [Discord](https://discord.gg/jJfCMrqCsT)
 - [Reporting Issues / Known Issues](https://github.com/damies13/rfswarm/issues)
 
 <kbd align="centre">
-<img align="centre" height="350" src="Doc/Images/Manager&Agent_Example.png">
+<img align="centre" height="350" src="https://github.com/damies13/rfswarm/blob/master/Doc/Images/Manager&Agent_Example.png">
 </kbd><br>
 An example of how your rfswarm setup might look.
 
 ### Commercial Support
 - The easiest way to get commercial support is to sponsor this project on [GitHub](https://github.com/sponsors/damies13?frequency=recurring&sponsor=damies13)
```

### Comparing `rfswarm-reporter-1.1.2/setup-reporter.py` & `rfswarm-reporter-1.1.3/setup-reporter.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README_PyPi.md", "r") as fh:
 	long_description = fh.read()
 
 setuptools.setup(
 	name="rfswarm-reporter",
-	version="1.1.2",
+	version="1.1.3",
 	author="damies13",
 	author_email="damies13+rfswarm@gmail.com",
 	description="rfswarm reporter",
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	url="https://github.com/damies13/rfswarm",
 	packages=setuptools.find_packages(exclude=["*fswarm_manag*", "*fswarm_agen*", "build/*"]),
```

