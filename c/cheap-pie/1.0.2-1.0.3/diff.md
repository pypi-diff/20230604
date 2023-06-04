# Comparing `tmp/cheap_pie-1.0.2.tar.gz` & `tmp/cheap_pie-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cheap_pie-1.0.2.tar", last modified: Wed May 24 22:08:35 2023, max compression
+gzip compressed data, was "cheap_pie-1.0.3.tar", last modified: Sun Jun  4 17:33:03 2023, max compression
```

## Comparing `cheap_pie-1.0.2.tar` & `cheap_pie-1.0.3.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-24 22:08:35.088389 cheap_pie-1.0.2/
--rwxrwxrwx   0 marco     (1000) marco     (1000)    11357 2022-12-10 01:01:26.000000 cheap_pie-1.0.2/LICENSE
--rwxrwxrwx   0 marco     (1000) marco     (1000)     8121 2023-05-24 22:08:35.088781 cheap_pie-1.0.2/PKG-INFO
--rwxrwxrwx   0 marco     (1000) marco     (1000)     7780 2023-05-24 22:06:57.000000 cheap_pie-1.0.2/README.md
--rwxrwxrwx   0 marco     (1000) marco     (1000)      103 2023-05-24 22:08:35.089857 cheap_pie-1.0.2/setup.cfg
--rwxrwxrwx   0 marco     (1000) marco     (1000)     1263 2023-05-24 22:07:39.000000 cheap_pie-1.0.2/setup.py
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-24 22:08:35.041053 cheap_pie-1.0.2/src/
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-24 22:08:35.047697 cheap_pie-1.0.2/src/cheap_pie/
--rwxrwxrwx   0 marco     (1000) marco     (1000)      207 2023-05-22 21:21:25.000000 cheap_pie-1.0.2/src/cheap_pie/__init__.py
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-24 22:08:35.065319 cheap_pie-1.0.2/src/cheap_pie/cheap_pie_core/
--rwxrwxrwx   0 marco     (1000) marco     (1000)      211 2023-05-22 20:58:17.000000 cheap_pie-1.0.2/src/cheap_pie/cheap_pie_core/__init__.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     7623 2023-05-21 17:00:23.000000 cheap_pie-1.0.2/src/cheap_pie/cheap_pie_core/cbitfield.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     2800 2023-05-21 16:18:51.000000 cheap_pie-1.0.2/src/cheap_pie/cheap_pie_core/cheap_pie_main.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     3232 2023-05-18 12:45:16.000000 cheap_pie-1.0.2/src/cheap_pie/cheap_pie_core/cp_banner.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     3388 2023-05-22 19:16:36.000000 cheap_pie-1.0.2/src/cheap_pie/cheap_pie_core/cp_builder.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     2691 2023-05-21 13:23:16.000000 cheap_pie-1.0.2/src/cheap_pie/cheap_pie_core/cp_cli.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     8613 2023-05-22 21:20:38.000000 cheap_pie-1.0.2/src/cheap_pie/cheap_pie_core/cp_hal.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)    15666 2023-05-22 20:39:24.000000 cheap_pie-1.0.2/src/cheap_pie/cheap_pie_core/cp_register.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     3669 2023-05-22 21:00:42.000000 cheap_pie-1.0.2/src/cheap_pie/cheap_pie_core/test.py
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-24 22:08:35.074285 cheap_pie-1.0.2/src/cheap_pie/parsers/
--rwxrwxrwx   0 marco     (1000) marco     (1000)      163 2023-05-22 20:56:30.000000 cheap_pie-1.0.2/src/cheap_pie/parsers/__init__.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     2427 2023-05-21 15:47:51.000000 cheap_pie-1.0.2/src/cheap_pie/parsers/cp_parsers_wrapper.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     3161 2023-05-21 16:42:25.000000 cheap_pie-1.0.2/src/cheap_pie/parsers/ipxact_parse.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     2643 2023-05-21 16:43:35.000000 cheap_pie-1.0.2/src/cheap_pie/parsers/ipyxact_parse.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     1166 2023-05-21 13:58:09.000000 cheap_pie-1.0.2/src/cheap_pie/parsers/rdl_parse.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     3133 2023-05-21 16:44:23.000000 cheap_pie-1.0.2/src/cheap_pie/parsers/svd_parse.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     3209 2023-05-21 16:45:01.000000 cheap_pie-1.0.2/src/cheap_pie/parsers/svd_parse_repo.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     2506 2023-05-21 13:40:46.000000 cheap_pie-1.0.2/src/cheap_pie/parsers/xml_xslt.py
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-24 22:08:35.080115 cheap_pie-1.0.2/src/cheap_pie/tools/
--rwxrwxrwx   0 marco     (1000) marco     (1000)       92 2023-05-21 15:55:01.000000 cheap_pie-1.0.2/src/cheap_pie/tools/__init__.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     4418 2023-05-22 21:15:24.000000 cheap_pie-1.0.2/src/cheap_pie/tools/hal2doc.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     2712 2023-05-22 19:30:55.000000 cheap_pie-1.0.2/src/cheap_pie/tools/rdl2any.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     2651 2023-05-22 21:20:52.000000 cheap_pie-1.0.2/src/cheap_pie/tools/search.py
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-24 22:08:35.087360 cheap_pie-1.0.2/src/cheap_pie/transport/
--rwxrwxrwx   0 marco     (1000) marco     (1000)      217 2023-05-24 22:02:54.000000 cheap_pie-1.0.2/src/cheap_pie/transport/__init__.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     2367 2023-05-21 15:28:36.000000 cheap_pie-1.0.2/src/cheap_pie/transport/cp_dummy_transport.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     2298 2023-05-21 15:27:18.000000 cheap_pie-1.0.2/src/cheap_pie/transport/cp_esptool_transport.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     1776 2023-05-21 16:01:42.000000 cheap_pie-1.0.2/src/cheap_pie/transport/cp_jlink_transport.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     1777 2023-05-21 16:11:06.000000 cheap_pie-1.0.2/src/cheap_pie/transport/cp_pyocd_transport.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     5573 2023-05-24 22:01:10.000000 cheap_pie-1.0.2/src/cheap_pie/transport/cp_pyverilator_transport.py
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-24 22:08:35.054668 cheap_pie-1.0.2/src/cheap_pie.egg-info/
--rwxrwxrwx   0 marco     (1000) marco     (1000)     8121 2023-05-24 22:08:34.000000 cheap_pie-1.0.2/src/cheap_pie.egg-info/PKG-INFO
--rwxrwxrwx   0 marco     (1000) marco     (1000)     1317 2023-05-24 22:08:35.000000 cheap_pie-1.0.2/src/cheap_pie.egg-info/SOURCES.txt
--rwxrwxrwx   0 marco     (1000) marco     (1000)        1 2023-05-24 22:08:34.000000 cheap_pie-1.0.2/src/cheap_pie.egg-info/dependency_links.txt
--rwxrwxrwx   0 marco     (1000) marco     (1000)      128 2023-05-24 22:08:34.000000 cheap_pie-1.0.2/src/cheap_pie.egg-info/requires.txt
--rwxrwxrwx   0 marco     (1000) marco     (1000)       10 2023-05-24 22:08:34.000000 cheap_pie-1.0.2/src/cheap_pie.egg-info/top_level.txt
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-06-04 17:33:03.836982 cheap_pie-1.0.3/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)    11357 2022-12-10 01:01:26.000000 cheap_pie-1.0.3/LICENSE
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     8121 2023-06-04 17:33:03.837324 cheap_pie-1.0.3/PKG-INFO
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     7780 2023-05-24 22:06:57.000000 cheap_pie-1.0.3/README.md
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      103 2023-06-04 17:33:03.839094 cheap_pie-1.0.3/setup.cfg
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     1263 2023-06-04 17:28:27.000000 cheap_pie-1.0.3/setup.py
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-06-04 17:33:03.750685 cheap_pie-1.0.3/src/
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-06-04 17:33:03.775369 cheap_pie-1.0.3/src/cheap_pie/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      207 2023-05-22 21:21:25.000000 cheap_pie-1.0.3/src/cheap_pie/__init__.py
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-06-04 17:33:03.809677 cheap_pie-1.0.3/src/cheap_pie/cheap_pie_core/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      211 2023-05-22 20:58:17.000000 cheap_pie-1.0.3/src/cheap_pie/cheap_pie_core/__init__.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     7623 2023-05-21 17:00:23.000000 cheap_pie-1.0.3/src/cheap_pie/cheap_pie_core/cbitfield.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     2800 2023-05-21 16:18:51.000000 cheap_pie-1.0.3/src/cheap_pie/cheap_pie_core/cheap_pie_main.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     3232 2023-05-18 12:45:16.000000 cheap_pie-1.0.3/src/cheap_pie/cheap_pie_core/cp_banner.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     3388 2023-05-22 19:16:36.000000 cheap_pie-1.0.3/src/cheap_pie/cheap_pie_core/cp_builder.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     2691 2023-05-21 13:23:16.000000 cheap_pie-1.0.3/src/cheap_pie/cheap_pie_core/cp_cli.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     8613 2023-05-22 21:20:38.000000 cheap_pie-1.0.3/src/cheap_pie/cheap_pie_core/cp_hal.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)    15666 2023-06-04 17:25:50.000000 cheap_pie-1.0.3/src/cheap_pie/cheap_pie_core/cp_register.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     3669 2023-05-22 21:00:42.000000 cheap_pie-1.0.3/src/cheap_pie/cheap_pie_core/test.py
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-06-04 17:33:03.820105 cheap_pie-1.0.3/src/cheap_pie/parsers/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      163 2023-05-22 20:56:30.000000 cheap_pie-1.0.3/src/cheap_pie/parsers/__init__.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     2427 2023-05-21 15:47:51.000000 cheap_pie-1.0.3/src/cheap_pie/parsers/cp_parsers_wrapper.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     3161 2023-05-21 16:42:25.000000 cheap_pie-1.0.3/src/cheap_pie/parsers/ipxact_parse.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     2643 2023-05-21 16:43:35.000000 cheap_pie-1.0.3/src/cheap_pie/parsers/ipyxact_parse.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     1166 2023-05-21 13:58:09.000000 cheap_pie-1.0.3/src/cheap_pie/parsers/rdl_parse.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     3133 2023-05-21 16:44:23.000000 cheap_pie-1.0.3/src/cheap_pie/parsers/svd_parse.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     3209 2023-05-21 16:45:01.000000 cheap_pie-1.0.3/src/cheap_pie/parsers/svd_parse_repo.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     2506 2023-05-21 13:40:46.000000 cheap_pie-1.0.3/src/cheap_pie/parsers/xml_xslt.py
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-06-04 17:33:03.824432 cheap_pie-1.0.3/src/cheap_pie/tools/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)       92 2023-05-21 15:55:01.000000 cheap_pie-1.0.3/src/cheap_pie/tools/__init__.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     4418 2023-05-22 21:15:24.000000 cheap_pie-1.0.3/src/cheap_pie/tools/hal2doc.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     2712 2023-05-22 19:30:55.000000 cheap_pie-1.0.3/src/cheap_pie/tools/rdl2any.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     2651 2023-05-22 21:20:52.000000 cheap_pie-1.0.3/src/cheap_pie/tools/search.py
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-06-04 17:33:03.836053 cheap_pie-1.0.3/src/cheap_pie/transport/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      217 2023-05-24 22:02:54.000000 cheap_pie-1.0.3/src/cheap_pie/transport/__init__.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     2367 2023-05-21 15:28:36.000000 cheap_pie-1.0.3/src/cheap_pie/transport/cp_dummy_transport.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     2298 2023-05-21 15:27:18.000000 cheap_pie-1.0.3/src/cheap_pie/transport/cp_esptool_transport.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     1776 2023-05-21 16:01:42.000000 cheap_pie-1.0.3/src/cheap_pie/transport/cp_jlink_transport.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     1777 2023-05-21 16:11:06.000000 cheap_pie-1.0.3/src/cheap_pie/transport/cp_pyocd_transport.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     5662 2023-05-24 22:15:55.000000 cheap_pie-1.0.3/src/cheap_pie/transport/cp_pyverilator_transport.py
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-06-04 17:33:03.783594 cheap_pie-1.0.3/src/cheap_pie.egg-info/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     8121 2023-06-04 17:33:03.000000 cheap_pie-1.0.3/src/cheap_pie.egg-info/PKG-INFO
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     1317 2023-06-04 17:33:03.000000 cheap_pie-1.0.3/src/cheap_pie.egg-info/SOURCES.txt
+-rwxrwxrwx   0 marco     (1000) marco     (1000)        1 2023-06-04 17:33:03.000000 cheap_pie-1.0.3/src/cheap_pie.egg-info/dependency_links.txt
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      128 2023-06-04 17:33:03.000000 cheap_pie-1.0.3/src/cheap_pie.egg-info/requires.txt
+-rwxrwxrwx   0 marco     (1000) marco     (1000)       10 2023-06-04 17:33:03.000000 cheap_pie-1.0.3/src/cheap_pie.egg-info/top_level.txt
```

### Comparing `cheap_pie-1.0.2/LICENSE` & `cheap_pie-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cheap_pie-1.0.2/PKG-INFO` & `cheap_pie-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cheap_pie
-Version: 1.0.2
+Version: 1.0.3
 Summary: A python tool for silicon validation.
 Home-page: https://github.com/bat52/cheap_pie
 Author: Marco Merlin
 Author-email: marcomerli@gmail.com
 License: Apache 2.0
 Keywords: python silicon validation
 Platform: UNKNOWN
```

### Comparing `cheap_pie-1.0.2/README.md` & `cheap_pie-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `cheap_pie-1.0.2/setup.py` & `cheap_pie-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf8') as fh:
     long_description = fh.read()
 
 setup(
     name='cheap_pie',
-    version='1.0.2',
+    version='1.0.3',
     license='Apache 2.0',
     author="Marco Merlin",
     author_email='marcomerli@gmail.com',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     description="A python tool for silicon validation.",
     long_description=long_description,
```

### Comparing `cheap_pie-1.0.2/src/cheap_pie/cheap_pie_core/cbitfield.py` & `cheap_pie-1.0.3/src/cheap_pie/cheap_pie_core/cbitfield.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-1.0.2/src/cheap_pie/cheap_pie_core/cheap_pie_main.py` & `cheap_pie-1.0.3/src/cheap_pie/cheap_pie_core/cheap_pie_main.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-1.0.2/src/cheap_pie/cheap_pie_core/cp_banner.py` & `cheap_pie-1.0.3/src/cheap_pie/cheap_pie_core/cp_banner.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-1.0.2/src/cheap_pie/cheap_pie_core/cp_builder.py` & `cheap_pie-1.0.3/src/cheap_pie/cheap_pie_core/cp_builder.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-1.0.2/src/cheap_pie/cheap_pie_core/cp_cli.py` & `cheap_pie-1.0.3/src/cheap_pie/cheap_pie_core/cp_cli.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-1.0.2/src/cheap_pie/cheap_pie_core/cp_hal.py` & `cheap_pie-1.0.3/src/cheap_pie/cheap_pie_core/cp_hal.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-1.0.2/src/cheap_pie/cheap_pie_core/cp_register.py` & `cheap_pie-1.0.3/src/cheap_pie/cheap_pie_core/cp_register.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -189,25 +189,25 @@
         """ Set a custom byte within a register """
         byte = CpBitfield(regaddr=self.addr, width=8, bit_offset=byte_offset*8, hif=self.hif)
         return byte.setbit(byteval)
 
     def help(self,width=25):
         """ function ret = help(self)
         # displays register comments """
+        self.print_wavedrom()
         print(self.comments)
 
         fmtstr = '%%%ds: %%s' % width # pylint: disable=C0209
         for field in self.bitfields:
             print( fmtstr % (field.fieldname,''))
 
             for line in textwrap.wrap(field.comments):
                 print( fmtstr % ('',line))
 
     def __repr__(self,regval = None ):
-        self.print_wavedrom()
         if len(self.bitfields) > 0:
             reg = []
             for field in self.bitfields :
                 # field.display(regval)
                 reg.append(field.__repr__(regval=regval))
             outstr = "\n".join(reg)
         else:
```

### Comparing `cheap_pie-1.0.2/src/cheap_pie/cheap_pie_core/test.py` & `cheap_pie-1.0.3/src/cheap_pie/cheap_pie_core/test.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-1.0.2/src/cheap_pie/parsers/cp_parsers_wrapper.py` & `cheap_pie-1.0.3/src/cheap_pie/parsers/cp_parsers_wrapper.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-1.0.2/src/cheap_pie/parsers/ipxact_parse.py` & `cheap_pie-1.0.3/src/cheap_pie/parsers/ipxact_parse.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-1.0.2/src/cheap_pie/parsers/ipyxact_parse.py` & `cheap_pie-1.0.3/src/cheap_pie/parsers/ipyxact_parse.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-1.0.2/src/cheap_pie/parsers/rdl_parse.py` & `cheap_pie-1.0.3/src/cheap_pie/parsers/rdl_parse.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-1.0.2/src/cheap_pie/parsers/svd_parse.py` & `cheap_pie-1.0.3/src/cheap_pie/parsers/svd_parse.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-1.0.2/src/cheap_pie/parsers/svd_parse_repo.py` & `cheap_pie-1.0.3/src/cheap_pie/parsers/svd_parse_repo.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-1.0.2/src/cheap_pie/parsers/xml_xslt.py` & `cheap_pie-1.0.3/src/cheap_pie/parsers/xml_xslt.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-1.0.2/src/cheap_pie/tools/hal2doc.py` & `cheap_pie-1.0.3/src/cheap_pie/tools/hal2doc.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-1.0.2/src/cheap_pie/tools/rdl2any.py` & `cheap_pie-1.0.3/src/cheap_pie/tools/rdl2any.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-1.0.2/src/cheap_pie/tools/search.py` & `cheap_pie-1.0.3/src/cheap_pie/tools/search.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-1.0.2/src/cheap_pie/transport/cp_dummy_transport.py` & `cheap_pie-1.0.3/src/cheap_pie/transport/cp_dummy_transport.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-1.0.2/src/cheap_pie/transport/cp_esptool_transport.py` & `cheap_pie-1.0.3/src/cheap_pie/transport/cp_esptool_transport.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-1.0.2/src/cheap_pie/transport/cp_jlink_transport.py` & `cheap_pie-1.0.3/src/cheap_pie/transport/cp_jlink_transport.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-1.0.2/src/cheap_pie/transport/cp_pyocd_transport.py` & `cheap_pie-1.0.3/src/cheap_pie/transport/cp_pyocd_transport.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-1.0.2/src/cheap_pie/transport/cp_pyverilator_transport.py` & `cheap_pie-1.0.3/src/cheap_pie/transport/cp_pyverilator_transport.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,15 +57,15 @@
             # sim.send_signal_to_gtkwave(sim.internals)
 
             # add all the io and internal signals to gtkwave
             # self.sim.send_to_gtkwave(self.sim.io)
             # self.sim.send_to_gtkwave(self.sim.internals)
 
             self.sim.clock.send_to_gtkwave()
-            self.sim.io.resetn.send_to_gtkwave()
+            self.sim.io.resetn.send_to_gtkwave() # pylint: disable=E1101
             self.sim.io.addr.send_to_gtkwave()
             self.sim.io.wdata.send_to_gtkwave()
             self.sim.io.rdata.send_to_gtkwave()
 
         self.reset_release()
 
     def reset_release(self):
@@ -162,21 +162,22 @@
     return (
             version.parse(ver) < version.parse("4.036") or
             version.parse(ver) > version.parse("4.102")
             )
 
 def test_cp_pyverilator(args=[]): # pylint: disable=W0102
     """ Test pyverilator transport """
-    if True: # verilator_version_ok():
+    if True: # verilator_version_ok(): pylint: disable=W0125
         prms = cli(args)
         hif = CpPyverilatorTransport(prms.fname)
         val = literal_eval('0x5A5A5A5A')
         hif.hifwrite(val = val)
         print( hex(hif.hifread()) )
         assert hif.hifread() == val
     else:
+        # this was fixed by pyverilator-mm
         print('Warning: pyverilator not working anymore \
               with verilator versions between 4.036 and 4.102.')
         print('https://github.com/chipsalliance/chisel3/issues/1565')
 
 if __name__ == '__main__':
     test_cp_pyverilator(sys.argv[1:])
```

### Comparing `cheap_pie-1.0.2/src/cheap_pie.egg-info/PKG-INFO` & `cheap_pie-1.0.3/src/cheap_pie.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cheap-pie
-Version: 1.0.2
+Version: 1.0.3
 Summary: A python tool for silicon validation.
 Home-page: https://github.com/bat52/cheap_pie
 Author: Marco Merlin
 Author-email: marcomerli@gmail.com
 License: Apache 2.0
 Keywords: python silicon validation
 Platform: UNKNOWN
```

### Comparing `cheap_pie-1.0.2/src/cheap_pie.egg-info/SOURCES.txt` & `cheap_pie-1.0.3/src/cheap_pie.egg-info/SOURCES.txt`

 * *Files identical despite different names*

