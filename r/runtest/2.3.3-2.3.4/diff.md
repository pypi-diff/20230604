# Comparing `tmp/runtest-2.3.3.tar.gz` & `tmp/runtest-2.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runtest-2.3.3.tar", last modified: Mon Jan 30 15:59:46 2023, max compression
+gzip compressed data, was "runtest-2.3.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `runtest-2.3.3.tar` & `runtest-2.3.4.tar`

### file list

```diff
@@ -1,51 +1,52 @@
--rw-r--r--   0        0        0      737 2023-01-30 15:59:35.932793 runtest-2.3.3/.github/workflows/coverage.yml
--rw-r--r--   0        0        0      774 2023-01-30 15:59:35.932793 runtest-2.3.3/.github/workflows/package.yml
--rw-r--r--   0        0        0      768 2023-01-30 15:59:35.932793 runtest-2.3.3/.github/workflows/test.yml
--rw-r--r--   0        0        0       72 2023-01-30 15:59:35.932793 runtest-2.3.3/.gitignore
--rw-r--r--   0        0        0       78 2023-01-30 15:59:35.932793 runtest-2.3.3/.mailmap
--rw-r--r--   0        0        0      224 2023-01-30 15:59:35.932793 runtest-2.3.3/.zenodo.json
--rw-r--r--   0        0        0    16725 2023-01-30 15:59:35.932793 runtest-2.3.3/LICENSE
--rw-r--r--   0        0        0     2045 2023-01-30 15:59:35.932793 runtest-2.3.3/README.rst
--rw-r--r--   0        0        0      799 2023-01-30 15:59:35.932793 runtest-2.3.3/doc/about/audience.rst
--rw-r--r--   0        0        0      880 2023-01-30 15:59:35.932793 runtest-2.3.3/doc/about/motivation.rst
--rw-r--r--   0        0        0      183 2023-01-30 15:59:35.932793 runtest-2.3.3/doc/about/similar.rst
--rw-r--r--   0        0        0     9688 2023-01-30 15:59:35.932793 runtest-2.3.3/doc/conf.py
--rw-r--r--   0        0        0     2096 2023-01-30 15:59:35.932793 runtest-2.3.3/doc/creating/configuration.rst
--rw-r--r--   0        0        0     3692 2023-01-30 15:59:35.932793 runtest-2.3.3/doc/creating/example.rst
--rw-r--r--   0        0        0     4906 2023-01-30 15:59:35.932793 runtest-2.3.3/doc/creating/filter_options.rst
--rw-r--r--   0        0        0     1557 2023-01-30 15:59:35.932793 runtest-2.3.3/doc/creating/general.rst
--rw-r--r--   0        0        0     1282 2023-01-30 15:59:35.932793 runtest-2.3.3/doc/creating/run_function.rst
--rw-r--r--   0        0        0      119 2023-01-30 15:59:35.932793 runtest-2.3.3/doc/developers/branches.rst
--rw-r--r--   0        0        0      640 2023-01-30 15:59:35.932793 runtest-2.3.3/doc/developers/contributing.rst
--rw-r--r--   0        0        0      797 2023-01-30 15:59:35.932793 runtest-2.3.3/doc/index.rst
--rw-r--r--   0        0        0     1105 2023-01-30 15:59:35.932793 runtest-2.3.3/doc/running/command_line_arguments.rst
--rw-r--r--   0        0        0      462 2023-01-30 15:59:35.932793 runtest-2.3.3/doc/running/generated_files.rst
--rw-r--r--   0        0        0    33406 2023-01-30 15:59:35.932793 runtest-2.3.3/img/xanathar.jpg
--rw-r--r--   0        0        0      344 2023-01-30 15:59:35.932793 runtest-2.3.3/pyproject.toml
--rw-r--r--   0        0        0       76 2023-01-30 15:59:35.932793 runtest-2.3.3/requirements.txt
--rw-r--r--   0        0        0      344 2023-01-30 15:59:35.932793 runtest-2.3.3/runtest/__init__.py
--rw-r--r--   0        0        0    14748 2023-01-30 15:59:35.932793 runtest-2.3.3/runtest/check.py
--rw-r--r--   0        0        0     1732 2023-01-30 15:59:35.932793 runtest-2.3.3/runtest/cli.py
--rw-r--r--   0        0        0      427 2023-01-30 15:59:35.932793 runtest-2.3.3/runtest/copy.py
--rw-r--r--   0        0        0      135 2023-01-30 15:59:35.932793 runtest-2.3.3/runtest/exceptions.py
--rw-r--r--   0        0        0     4332 2023-01-30 15:59:35.932793 runtest-2.3.3/runtest/extract.py
--rw-r--r--   0        0        0      702 2023-01-30 15:59:35.932793 runtest-2.3.3/runtest/filter_api.py
--rw-r--r--   0        0        0     2857 2023-01-30 15:59:35.932793 runtest-2.3.3/runtest/filter_constructor.py
--rw-r--r--   0        0        0     4601 2023-01-30 15:59:35.932793 runtest-2.3.3/runtest/run.py
--rw-r--r--   0        0        0     3498 2023-01-30 15:59:35.932793 runtest-2.3.3/runtest/scissors.py
--rw-r--r--   0        0        0        0 2023-01-30 15:59:35.936793 runtest-2.3.3/runtest/test/__init__.py
--rw-r--r--   0        0        0       16 2023-01-30 15:59:35.936793 runtest-2.3.3/runtest/test/different_length/out.txt
--rw-r--r--   0        0        0       13 2023-01-30 15:59:35.936793 runtest-2.3.3/runtest/test/different_length/ref.txt
--rw-r--r--   0        0        0       12 2023-01-30 15:59:35.936793 runtest-2.3.3/runtest/test/generic/out.txt
--rw-r--r--   0        0        0       13 2023-01-30 15:59:35.936793 runtest-2.3.3/runtest/test/generic/ref.txt
--rw-r--r--   0        0        0       20 2023-01-30 15:59:35.936793 runtest-2.3.3/runtest/test/ignore_order/out.txt
--rw-r--r--   0        0        0       20 2023-01-30 15:59:35.936793 runtest-2.3.3/runtest/test/ignore_order/ref.txt
--rw-r--r--   0        0        0       27 2023-01-30 15:59:35.936793 runtest-2.3.3/runtest/test/ignore_order_and_sign/out.txt
--rw-r--r--   0        0        0       27 2023-01-30 15:59:35.936793 runtest-2.3.3/runtest/test/ignore_order_and_sign/ref.txt
--rw-r--r--   0        0        0       18 2023-01-30 15:59:35.936793 runtest-2.3.3/runtest/test/integers/out.txt
--rw-r--r--   0        0        0       18 2023-01-30 15:59:35.936793 runtest-2.3.3/runtest/test/integers/ref.txt
--rw-r--r--   0        0        0        7 2023-01-30 15:59:35.936793 runtest-2.3.3/runtest/test/only_string/out.txt
--rw-r--r--   0        0        0        7 2023-01-30 15:59:35.936793 runtest-2.3.3/runtest/test/only_string/ref.txt
--rw-r--r--   0        0        0     2971 2023-01-30 15:59:35.936793 runtest-2.3.3/runtest/tuple_comparison.py
--rw-r--r--   0        0        0      392 2023-01-30 15:59:35.936793 runtest-2.3.3/runtest/version.py
--rw-r--r--   0        0        0     2395 1970-01-01 00:00:00.000000 runtest-2.3.3/PKG-INFO
+-rw-r--r--   0        0        0      740 2023-06-04 20:55:52.667240 runtest-2.3.4/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0      801 2023-06-04 20:55:52.667240 runtest-2.3.4/.github/workflows/package.yml
+-rw-r--r--   0        0        0      761 2023-06-04 20:55:52.667240 runtest-2.3.4/.github/workflows/test.yml
+-rw-r--r--   0        0        0       72 2023-06-04 20:55:52.667240 runtest-2.3.4/.gitignore
+-rw-r--r--   0        0        0       78 2023-06-04 20:55:52.667240 runtest-2.3.4/.mailmap
+-rw-r--r--   0        0        0      224 2023-06-04 20:55:52.667240 runtest-2.3.4/.zenodo.json
+-rw-r--r--   0        0        0    16725 2023-06-04 20:55:52.667240 runtest-2.3.4/LICENSE
+-rw-r--r--   0        0        0     2185 2023-06-04 20:55:52.667240 runtest-2.3.4/README.md
+-rw-r--r--   0        0        0      799 2023-06-04 20:55:52.667240 runtest-2.3.4/doc/about/audience.rst
+-rw-r--r--   0        0        0      880 2023-06-04 20:55:52.667240 runtest-2.3.4/doc/about/motivation.rst
+-rw-r--r--   0        0        0      183 2023-06-04 20:55:52.667240 runtest-2.3.4/doc/about/similar.rst
+-rw-r--r--   0        0        0     9725 2023-06-04 20:55:52.667240 runtest-2.3.4/doc/conf.py
+-rw-r--r--   0        0        0     2096 2023-06-04 20:55:52.667240 runtest-2.3.4/doc/creating/configuration.rst
+-rw-r--r--   0        0        0     3692 2023-06-04 20:55:52.667240 runtest-2.3.4/doc/creating/example.rst
+-rw-r--r--   0        0        0     4906 2023-06-04 20:55:52.667240 runtest-2.3.4/doc/creating/filter_options.rst
+-rw-r--r--   0        0        0     1557 2023-06-04 20:55:52.667240 runtest-2.3.4/doc/creating/general.rst
+-rw-r--r--   0        0        0     1282 2023-06-04 20:55:52.667240 runtest-2.3.4/doc/creating/run_function.rst
+-rw-r--r--   0        0        0      119 2023-06-04 20:55:52.667240 runtest-2.3.4/doc/developers/branches.rst
+-rw-r--r--   0        0        0      640 2023-06-04 20:55:52.667240 runtest-2.3.4/doc/developers/contributing.rst
+-rw-r--r--   0        0        0      797 2023-06-04 20:55:52.667240 runtest-2.3.4/doc/index.rst
+-rw-r--r--   0        0        0     1105 2023-06-04 20:55:52.667240 runtest-2.3.4/doc/running/command_line_arguments.rst
+-rw-r--r--   0        0        0      462 2023-06-04 20:55:52.667240 runtest-2.3.4/doc/running/generated_files.rst
+-rw-r--r--   0        0        0   200697 2023-06-04 20:55:52.667240 runtest-2.3.4/img/runtest-small.png
+-rw-r--r--   0        0        0  1218243 2023-06-04 20:55:52.671240 runtest-2.3.4/img/runtest.png
+-rw-r--r--   0        0        0      343 2023-06-04 20:55:52.671240 runtest-2.3.4/pyproject.toml
+-rw-r--r--   0        0        0       76 2023-06-04 20:55:52.671240 runtest-2.3.4/requirements.txt
+-rw-r--r--   0        0        0      344 2023-06-04 20:55:52.671240 runtest-2.3.4/runtest/__init__.py
+-rw-r--r--   0        0        0    14746 2023-06-04 20:55:52.671240 runtest-2.3.4/runtest/check.py
+-rw-r--r--   0        0        0     1732 2023-06-04 20:55:52.671240 runtest-2.3.4/runtest/cli.py
+-rw-r--r--   0        0        0      427 2023-06-04 20:55:52.671240 runtest-2.3.4/runtest/copy.py
+-rw-r--r--   0        0        0      135 2023-06-04 20:55:52.671240 runtest-2.3.4/runtest/exceptions.py
+-rw-r--r--   0        0        0     5411 2023-06-04 20:55:52.671240 runtest-2.3.4/runtest/extract.py
+-rw-r--r--   0        0        0      702 2023-06-04 20:55:52.671240 runtest-2.3.4/runtest/filter_api.py
+-rw-r--r--   0        0        0     2856 2023-06-04 20:55:52.671240 runtest-2.3.4/runtest/filter_constructor.py
+-rw-r--r--   0        0        0     4601 2023-06-04 20:55:52.671240 runtest-2.3.4/runtest/run.py
+-rw-r--r--   0        0        0     3491 2023-06-04 20:55:52.671240 runtest-2.3.4/runtest/scissors.py
+-rw-r--r--   0        0        0        0 2023-06-04 20:55:52.671240 runtest-2.3.4/runtest/test/__init__.py
+-rw-r--r--   0        0        0       16 2023-06-04 20:55:52.671240 runtest-2.3.4/runtest/test/different_length/out.txt
+-rw-r--r--   0        0        0       13 2023-06-04 20:55:52.671240 runtest-2.3.4/runtest/test/different_length/ref.txt
+-rw-r--r--   0        0        0       12 2023-06-04 20:55:52.671240 runtest-2.3.4/runtest/test/generic/out.txt
+-rw-r--r--   0        0        0       13 2023-06-04 20:55:52.671240 runtest-2.3.4/runtest/test/generic/ref.txt
+-rw-r--r--   0        0        0       20 2023-06-04 20:55:52.671240 runtest-2.3.4/runtest/test/ignore_order/out.txt
+-rw-r--r--   0        0        0       20 2023-06-04 20:55:52.671240 runtest-2.3.4/runtest/test/ignore_order/ref.txt
+-rw-r--r--   0        0        0       27 2023-06-04 20:55:52.671240 runtest-2.3.4/runtest/test/ignore_order_and_sign/out.txt
+-rw-r--r--   0        0        0       27 2023-06-04 20:55:52.671240 runtest-2.3.4/runtest/test/ignore_order_and_sign/ref.txt
+-rw-r--r--   0        0        0       18 2023-06-04 20:55:52.671240 runtest-2.3.4/runtest/test/integers/out.txt
+-rw-r--r--   0        0        0       18 2023-06-04 20:55:52.671240 runtest-2.3.4/runtest/test/integers/ref.txt
+-rw-r--r--   0        0        0        7 2023-06-04 20:55:52.671240 runtest-2.3.4/runtest/test/only_string/out.txt
+-rw-r--r--   0        0        0        7 2023-06-04 20:55:52.671240 runtest-2.3.4/runtest/test/only_string/ref.txt
+-rw-r--r--   0        0        0     2971 2023-06-04 20:55:52.671240 runtest-2.3.4/runtest/tuple_comparison.py
+-rw-r--r--   0        0        0      392 2023-06-04 20:55:52.671240 runtest-2.3.4/runtest/version.py
+-rw-r--r--   0        0        0     2538 1970-01-01 00:00:00.000000 runtest-2.3.4/PKG-INFO
```

### Comparing `runtest-2.3.3/.github/workflows/coverage.yml` & `runtest-2.3.4/.github/workflows/coverage.yml`

 * *Files 16% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 jobs:
   build:
 
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
-        python-version: [3.7]
+        python-version: ["3.10"]
         os: [ubuntu-latest]
 
     steps:
     - name: Checkout
       uses: actions/checkout@v2
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v1
```

### Comparing `runtest-2.3.3/.github/workflows/package.yml` & `runtest-2.3.4/.github/workflows/package.yml`

 * *Files 17% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 on:
   release:
     types: [created]
 
 jobs:
   build:
-
+    permissions: write-all
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
-        python-version: ["3.7"]
+        python-version: ["3.10"]
         os: [ubuntu-latest]
 
     steps:
     - name: Switch branch
       uses: actions/checkout@v2
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v1
```

### Comparing `runtest-2.3.3/.github/workflows/test.yml` & `runtest-2.3.4/.github/workflows/test.yml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 jobs:
   build:
 
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
-        python-version: ["3.7", "3.8", "3.9", "3.10"]
+        python-version: ["3.8", "3.9", "3.10"]
         os: [ubuntu-latest, macOS-latest, windows-latest]
 
     steps:
     - name: Checkout
       uses: actions/checkout@v2
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v1
```

### Comparing `runtest-2.3.3/LICENSE` & `runtest-2.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `runtest-2.3.3/doc/about/audience.rst` & `runtest-2.3.4/doc/about/audience.rst`

 * *Files identical despite different names*

### Comparing `runtest-2.3.3/doc/about/motivation.rst` & `runtest-2.3.4/doc/about/motivation.rst`

 * *Files identical despite different names*

### Comparing `runtest-2.3.3/doc/conf.py` & `runtest-2.3.4/doc/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # autogenerated file.
 #
 # All configuration values have a default; values that are commented out
 # serve to show the default.
 
 import sys
 import os
+import datetime
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 sys.path.insert(0, os.path.abspath(".."))
 from runtest import __version__ as _version
 
@@ -46,15 +47,15 @@
 # source_encoding = 'utf-8-sig'
 
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
 project = u"runtest"
-copyright = u"2014-2017, Radovan Bast"
+copyright = f"{datetime.datetime.now().year}, Radovan Bast"
 author = u"Radovan Bast"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The full version, including alpha/beta/rc tags.
```

### Comparing `runtest-2.3.3/doc/creating/configuration.rst` & `runtest-2.3.4/doc/creating/configuration.rst`

 * *Files identical despite different names*

### Comparing `runtest-2.3.3/doc/creating/example.rst` & `runtest-2.3.4/doc/creating/example.rst`

 * *Files identical despite different names*

### Comparing `runtest-2.3.3/doc/creating/filter_options.rst` & `runtest-2.3.4/doc/creating/filter_options.rst`

 * *Files identical despite different names*

### Comparing `runtest-2.3.3/doc/creating/general.rst` & `runtest-2.3.4/doc/creating/general.rst`

 * *Files identical despite different names*

### Comparing `runtest-2.3.3/doc/creating/run_function.rst` & `runtest-2.3.4/doc/creating/run_function.rst`

 * *Files identical despite different names*

### Comparing `runtest-2.3.3/doc/developers/contributing.rst` & `runtest-2.3.4/doc/developers/contributing.rst`

 * *Files identical despite different names*

### Comparing `runtest-2.3.3/doc/index.rst` & `runtest-2.3.4/doc/index.rst`

 * *Files identical despite different names*

### Comparing `runtest-2.3.3/doc/running/command_line_arguments.rst` & `runtest-2.3.4/doc/running/command_line_arguments.rst`

 * *Files identical despite different names*

### Comparing `runtest-2.3.3/runtest/check.py` & `runtest-2.3.4/runtest/check.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,17 +48,15 @@
     name_out = os.path.join(log_dir, out_name + ".filtered")
     name_ref = os.path.join(log_dir, out_name + ".reference")
     name_diff = os.path.join(log_dir, out_name + ".diff")
 
     with open(name_out, "w") as log_out:
         with open(name_ref, "w") as log_ref:
             with open(name_diff, "w") as log_diff:
-
                 for f in filter_list:
-
                     out_filtered = cut_sections(
                         open(out_name).readlines(),
                         from_string=f.from_string,
                         from_is_re=f.from_is_re,
                         to_string=f.to_string,
                         to_is_re=f.to_is_re,
                         num_lines=f.num_lines,
```

### Comparing `runtest-2.3.3/runtest/cli.py` & `runtest-2.3.4/runtest/cli.py`

 * *Files identical despite different names*

### Comparing `runtest-2.3.3/runtest/filter_api.py` & `runtest-2.3.4/runtest/filter_api.py`

 * *Files identical despite different names*

### Comparing `runtest-2.3.3/runtest/filter_constructor.py` & `runtest-2.3.4/runtest/filter_constructor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import sys
 from collections import namedtuple
 from .exceptions import FilterKeywordError
 from .filter_api import recognized_kw, incompatible_pairs
 
 
 def get_filter(**kwargs):
-
     _filter = namedtuple(
         "_filter",
         [
             "from_is_re",
             "from_string",
             "skip_above",
             "skip_below",
```

### Comparing `runtest-2.3.3/runtest/run.py` & `runtest-2.3.4/runtest/run.py`

 * *Files identical despite different names*

### Comparing `runtest-2.3.3/runtest/scissors.py` & `runtest-2.3.4/runtest/scissors.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 
     Returns:
         output - list of remaining lines
     """
     output = []
 
     for i, _ in enumerate(text):
-
         start_line_matches = False
         if from_is_re:
             start_line_matches = re.match(r".*{0}".format(from_string), text[i])
         else:
             if from_string is None:
                 # we are comparing entire file
                 return text
@@ -31,15 +30,14 @@
 
         if start_line_matches:
             if num_lines > 0:
                 for n in range(i, i + num_lines):
                     output.append(text[n])
             else:
                 for j in range(i, len(text)):
-
                     end_line_matches = False
                     if to_is_re:
                         end_line_matches = re.match(r".*{0}".format(to_string), text[j])
                     else:
                         end_line_matches = to_string in text[j]
 
                     if end_line_matches:
@@ -47,15 +45,14 @@
                             output.append(text[n])
                         break
 
     return output
 
 
 def test_cut_sections():
-
     text = """
 1.0 2.0 3.0
 1.0 2.0 3.0
 1.0 2.0 3.0
 1.0 2.0 3.0
 1.0 2.0 3.0
 1.0 2.0 3.0
@@ -77,15 +74,14 @@
         "       1.0 3.0 7.0",
         "       1.0 3.0 7.0",
         "       1.0 3.0 7.0",
     ]
 
 
 def test_cut_sections_re():
-
     text = """
 1.0
 1.0
     raboof
 2.0
 2.0
     raboof2
@@ -100,15 +96,14 @@
         to_is_re=True,
     )
 
     assert res == ["    raboof", "2.0", "2.0", "    raboof2", "    raboof2"]
 
 
 def test_cut_sections_all():
-
     text = """first line
 1.0 2.0 3.0
 1.0 2.0 3.0
 1.0 2.0 3.0
 last line"""
 
     res = cut_sections(text=text.splitlines())
@@ -119,15 +114,14 @@
         "1.0 2.0 3.0",
         "1.0 2.0 3.0",
         "last line",
     ]
 
 
 def test_cut_sections_from_string_to_string_2_matches():
-
     text = """first line
 1.0 2.0 3.0
 start
 0.1234
 end
 start
 1.2345
@@ -148,15 +142,14 @@
         "start",
         "1.2345",
         "end",
     ]
 
 
 def test_cut_sections_from_re_to_re_2_matches():
-
     text = """first line
 1.0 2.0 3.0
   raboof
 0.1234
     raboof2
    raboof
 1.2345
```

### Comparing `runtest-2.3.3/runtest/tuple_comparison.py` & `runtest-2.3.4/runtest/tuple_comparison.py`

 * *Files identical despite different names*

### Comparing `runtest-2.3.3/PKG-INFO` & `runtest-2.3.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,87 +1,76 @@
 Metadata-Version: 2.1
 Name: runtest
-Version: 2.3.3
+Version: 2.3.4
 Summary: runtest: Numerically tolerant end-to-end test library for research software.
 Home-page: https://github.com/bast/runtest
 Author: Radovan Bast
 Author-email: radovan.bast@uit.no
-Description-Content-Type: text/x-rst
+Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 
-.. image:: https://github.com/bast/runtest/workflows/Test/badge.svg
-   :target: https://github.com/bast/runtest/actions
-.. image:: https://coveralls.io/repos/bast/runtest/badge.png?branch=main
-   :target: https://coveralls.io/r/bast/runtest?branch=main
-.. image:: https://readthedocs.org/projects/runtest/badge/?version=latest
-   :target: http://runtest.readthedocs.io
-.. image:: https://img.shields.io/badge/license-%20MPL--v2.0-blue.svg
-   :target: LICENSE
-.. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.1069004.svg
-   :target: https://doi.org/10.5281/zenodo.1069004
-.. image:: https://badge.fury.io/py/runtest.svg
-   :target: https://badge.fury.io/py/runtest
+[![image](https://github.com/bast/runtest/workflows/Test/badge.svg)](https://github.com/bast/runtest/actions)
+[![image](https://coveralls.io/repos/bast/runtest/badge.png?branch=main)](https://coveralls.io/r/bast/runtest?branch=main)
+[![image](https://readthedocs.org/projects/runtest/badge/?version=latest)](http://runtest.readthedocs.io)
+[![image](https://img.shields.io/badge/license-%20MPL--v2.0-blue.svg)](LICENSE)
+[![image](https://zenodo.org/badge/DOI/10.5281/zenodo.1069004.svg)](https://doi.org/10.5281/zenodo.1069004)
+[![image](https://badge.fury.io/py/runtest.svg)](https://badge.fury.io/py/runtest)
 
 
-runtest
-=======
+# runtest
 
 Numerically tolerant end-to-end test library for research software.
 
-Tested with Python 3.7, 3.8, 3.9, 3.10.
+![image of a hardware circuit with red and green light bulbs](img/runtest-small.png)
 
-.. figure:: https://github.com/bast/runtest/raw/main/img/xanathar.jpg
-   :alt: Xanathar
+Image: [Midjourney](https://midjourney.com/), [CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/legalcode)
 
 
-Installation
-------------
+## Installation
 
-::
+```
+$ pip install runtest
+```
 
-  $ pip install runtest
 
+## Supported Python versions
 
-Documentation
--------------
+The library is tested with Python 3.7, 3.8, 3.9, 3.10.  If you want to test
+runtest itself on your computer, you can follow what we do in the [CI
+workflow](https://github.com/bast/runtest/blob/main/.github/workflows/test.yml).
 
--  `Latest code <http://runtest.readthedocs.io/en/latest/>`__ (main
-   branch)
 
+## Documentation
+
+- [Latest code](http://runtest.readthedocs.io/en/latest/) (main branch)
 
-Past versions
-~~~~~~~~~~~~~
 
--  `1.3.z <http://runtest.readthedocs.io/en/release-1.3.z/>`__
-   (`release-1.3.z
-   branch <https://github.com/bast/runtest/tree/release-1.3.z>`__)
+Past versions
+- [1.3.z](http://runtest.readthedocs.io/en/release-1.3.z/) ([release-1.3.z branch](https://github.com/bast/runtest/tree/release-1.3.z))
 
 
-Citation
---------
+## Citation
 
-For a recommended citation, please check the at the bottom-right of https://zenodo.org/record/3893712.
+For a recommended citation, please check the at the bottom-right of
+<https://zenodo.org/record/3893712>.
 
 
-Projects using runtest
-----------------------
+## Projects using runtest
 
--  `DIRAC <http://diracprogram.org>`__
--  `Dalton <http://daltonprogram.org>`__ and
-   `LSDalton <http://daltonprogram.org>`__
--  `GIMIC <https://github.com/qmcurrents/gimic>`__
--  `OpenRSP <http://openrsp.org>`__
--  `MRChem <https://mrchem.readthedocs.io/en/latest/>`__
--  GRASP (General-purpose Relativistic Atomic Structure Program)
--  `eT <https://etprogram.org>`__
+- [DIRAC](http://diracprogram.org)
+- [Dalton](http://daltonprogram.org) and [LSDalton](http://daltonprogram.org)
+- [GIMIC](https://github.com/qmcurrents/gimic)
+- [OpenRSP](http://openrsp.org)
+- [MRChem](https://mrchem.readthedocs.io/en/latest/)
+- GRASP (General-purpose Relativistic Atomic Structure Program)
+- [eT](https://etprogram.org)
 
 If you use runtest, please add a link to your project via a pull
 request.
 
 
-Similar projects
-----------------
+## Similar projects
 
--  `testcode <http://testcode.readthedocs.io>`__ is a python module for
-   testing for regression errors in numerical (principally scientific)
-   software.
+- [testcode](http://testcode.readthedocs.io) is a python module for
+  testing for regression errors in numerical (principally scientific)
+  software.
```

