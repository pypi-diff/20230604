# Comparing `tmp/jekyll_to_hugo-0.0.5.tar.gz` & `tmp/jekyll_to_hugo-0.0.6.tar.gz`

## Comparing `jekyll_to_hugo-0.0.5.tar` & `jekyll_to_hugo-0.0.6.tar`

### file list

```diff
@@ -1,35 +1,36 @@
--rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.5/.DS_Store
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.5/Dockerfile
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.5/Makefile
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.5/config.yaml
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.5/main.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.5/requirements-dev.txt
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.5/requirements-test.txt
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.5/requirements.txt
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.5/.idea/.gitignore
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.5/.idea/jekyll-to-hugo.iml
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.5/.idea/misc.xml
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.5/.idea/modules.xml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.5/.idea/vcs.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.5/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.5/app/__init__.py
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.5/app/config.py
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.5/app/utils.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.5/app/converter/__init__.py
--rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.5/app/converter/converter.py
--rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.5/app/converter/regex_heuristics.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.5/app/converter/tags_heuristics.py
--rw-r--r--   0        0        0     7633 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.5/app/converter/wordpress_markdown.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.5/app/io/__init__.py
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.5/app/io/reader.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.5/app/io/writer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.5/app/tests/__init__.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.5/app/tests/utils.py
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.5/app/tests/utils_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.5/app/tests/converter/__init__.py
--rw-r--r--   0        0        0     6589 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.5/app/tests/converter/wordpress_markdown_test.py
--rw-r--r--   0        0        0     6055 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.5/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.5/LICENSE
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.5/readme.md
--rw-r--r--   0        0        0     4257 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.6/Makefile
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.6/config.yaml
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.6/main.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.6/requirements-dev.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.6/requirements-test.txt
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.6/requirements.txt
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.6/tox.ini
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.6/.idea/.gitignore
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.6/.idea/jekyll-to-hugo.iml
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.6/.idea/misc.xml
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.6/.idea/modules.xml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.6/.idea/vcs.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.6/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.6/app/__init__.py
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.6/app/config.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.6/app/utils.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.6/app/converter/__init__.py
+-rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.6/app/converter/converter.py
+-rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.6/app/converter/regex_heuristics.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.6/app/converter/tags_heuristics.py
+-rw-r--r--   0        0        0     7633 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.6/app/converter/wordpress_markdown.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.6/app/io/__init__.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.6/app/io/reader.py
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.6/app/io/writer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.6/app/tests/__init__.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.6/app/tests/utils.py
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.6/app/tests/utils_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.6/app/tests/converter/__init__.py
+-rw-r--r--   0        0        0     6583 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.6/app/tests/converter/wordpress_markdown_test.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.6/docker/Dockerfile
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.6/docker/Tox.Dockerfile
+-rw-r--r--   0        0        0     6055 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.6/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.6/LICENSE
+-rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.6/readme.md
+-rw-r--r--   0        0        0     4131 2020-02-02 00:00:00.000000 jekyll_to_hugo-0.0.6/PKG-INFO
```

### Comparing `jekyll_to_hugo-0.0.5/config.yaml` & `jekyll_to_hugo-0.0.6/config.yaml`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.5/main.py` & `jekyll_to_hugo-0.0.6/main.py`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.5/app/config.py` & `jekyll_to_hugo-0.0.6/app/config.py`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.5/app/utils.py` & `jekyll_to_hugo-0.0.6/app/utils.py`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.5/app/converter/converter.py` & `jekyll_to_hugo-0.0.6/app/converter/converter.py`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.5/app/converter/regex_heuristics.py` & `jekyll_to_hugo-0.0.6/app/converter/regex_heuristics.py`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.5/app/converter/wordpress_markdown.py` & `jekyll_to_hugo-0.0.6/app/converter/wordpress_markdown.py`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.5/app/io/reader.py` & `jekyll_to_hugo-0.0.6/app/io/reader.py`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.5/app/io/writer.py` & `jekyll_to_hugo-0.0.6/app/io/writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         output_path.parent.mkdir(parents=True, exist_ok=True)
 
     def write(self, data: str):
         with open(self.output_path, "w") as fo:
             fo.write(data)
 
 
-class TestingWriter(IoWriter):
+class MockWriter(IoWriter):
     """
     Writes a post to a string.
     """
 
     def __init__(self):
         self.content = ""
```

### Comparing `jekyll_to_hugo-0.0.5/app/tests/utils.py` & `jekyll_to_hugo-0.0.6/app/tests/utils.py`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.5/app/tests/utils_test.py` & `jekyll_to_hugo-0.0.6/app/tests/utils_test.py`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.5/app/tests/converter/wordpress_markdown_test.py` & `jekyll_to_hugo-0.0.6/app/tests/converter/wordpress_markdown_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pytest
 
 from app.config import ConverterOptions
 from app.converter import WordpressMarkdownConverter
 from app.io.reader import StringReader
-from app.io.writer import TestingWriter
+from app.io.writer import MockWriter
 from app.tests.utils import make_fake_configurator
 
 
 @pytest.mark.parametrize(
     "author_rewrite, input_header, expected_header",
     [
         ("", {"author": "author"}, {"author": ""}),
@@ -179,10 +179,10 @@
 
 def test_write_hugo_post():
     configurator = make_fake_configurator(
         "wordpress_markdown_converter",
         ConverterOptions(),
     )
     converter = WordpressMarkdownConverter(configurator)
-    writer = TestingWriter()
+    writer = MockWriter()
     converter.write_hugo_post(writer, {"title": "Test"}, "Test\nLine 2")
     assert writer.content == "---\ntitle: Test\n---\nTest\nLine 2"
```

### Comparing `jekyll_to_hugo-0.0.5/.gitignore` & `jekyll_to_hugo-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.5/LICENSE` & `jekyll_to_hugo-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `jekyll_to_hugo-0.0.5/pyproject.toml` & `jekyll_to_hugo-0.0.6/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "jekyll-to-hugo"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Denis Nutiu", email="nuculabs@outlook.com" },
 ]
 description = "Python library for converting jekyll md files to Hugo."
 readme = "readme.md"
-requires-python = ">=3.7"
+requires-python = ">=3.10"
 classifiers = [
   "Environment :: Console",
   "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3 :: Only",
-  "Programming Language :: Python :: 3.7",
-  "Programming Language :: Python :: 3.8",
-  "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
   "beautifulsoup4>=4.12, <5",
   "PyYAML",
   "soupsieve>=2.4, <3",
```

### Comparing `jekyll_to_hugo-0.0.5/readme.md` & `jekyll_to_hugo-0.0.6/readme.md`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 ### Docker
 
 If you don't have Python installed, you can use Docker:
 
 1. Build the image.
 
 ```bash
-docker build -t jekyll-to-hugo .
+docker build -t jekyll-to-hugo -f ./docker/Dockerfile .
 ```
 
 2. Run the image. You will need to mount the following directories: config file, Jekyll posts directory, Hugo posts directory.
 
 ```bash
 docker run -it --rm -v $(pwd):/app jekyll-to-hugo
 ```
```

### Comparing `jekyll_to_hugo-0.0.5/PKG-INFO` & `jekyll_to_hugo-0.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 Metadata-Version: 2.1
 Name: jekyll-to-hugo
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python library for converting jekyll md files to Hugo.
 Project-URL: Homepage, https://github.com/dnutiu/jekyll-to-hugo
 Project-URL: Bug Tracker, https://github.com/dnutiu/jekyll-to-hugo/issues
 Author-email: Denis Nutiu <nuculabs@outlook.com>
 License-File: LICENSE
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Requires-Dist: beautifulsoup4<5,>=4.12
 Requires-Dist: pydantic<2,>=1.10
 Requires-Dist: pyyaml
 Requires-Dist: soupsieve<3,>=2.4
 Provides-Extra: dev
 Requires-Dist: autoflake; extra == 'dev'
 Requires-Dist: black; extra == 'dev'
@@ -86,15 +83,15 @@
 ### Docker
 
 If you don't have Python installed, you can use Docker:
 
 1. Build the image.
 
 ```bash
-docker build -t jekyll-to-hugo .
+docker build -t jekyll-to-hugo -f ./docker/Dockerfile .
 ```
 
 2. Run the image. You will need to mount the following directories: config file, Jekyll posts directory, Hugo posts directory.
 
 ```bash
 docker run -it --rm -v $(pwd):/app jekyll-to-hugo
 ```
```

