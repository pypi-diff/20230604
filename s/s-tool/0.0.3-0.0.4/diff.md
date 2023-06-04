# Comparing `tmp/s-tool-0.0.3.tar.gz` & `tmp/s_tool-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s-tool-0.0.3.tar", max compression
+gzip compressed data, was "s_tool-0.0.4.tar", max compression
```

## Comparing `s-tool-0.0.3.tar` & `s_tool-0.0.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1069 2021-07-16 19:04:34.262567 s-tool-0.0.3/LICENSE
--rw-r--r--   0        0        0     3360 2021-08-02 18:58:28.281590 s-tool-0.0.3/README.md
--rw-r--r--   0        0        0     1502 2021-08-05 16:37:54.657791 s-tool-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      187 2021-07-16 19:04:34.262567 s-tool-0.0.3/s_tool/__init__.py
--rw-r--r--   0        0        0     4822 2021-08-02 20:07:59.076018 s-tool-0.0.3/s_tool/driver.py
--rw-r--r--   0        0        0      406 2021-07-27 18:59:56.013435 s-tool-0.0.3/s_tool/exceptions.py
--rw-r--r--   0        0        0     1912 2021-08-02 17:18:34.815181 s-tool-0.0.3/s_tool/parser.py
--rw-r--r--   0        0        0    11040 2021-08-04 18:32:10.051824 s-tool-0.0.3/s_tool/utils.py
--rw-r--r--   0        0        0     4190 2021-08-05 16:41:37.979561 s-tool-0.0.3/setup.py
--rw-r--r--   0        0        0     4294 2021-08-05 16:41:37.980021 s-tool-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-04 18:38:21.227674 s_tool-0.0.4/LICENSE
+-rw-r--r--   0        0        0     3682 2023-06-04 18:38:21.227674 s_tool-0.0.4/README.rst
+-rw-r--r--   0        0        0     1488 2023-06-04 18:38:21.227674 s_tool-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      187 2023-06-04 18:38:21.227674 s_tool-0.0.4/s_tool/__init__.py
+-rw-r--r--   0        0        0    28280 2023-06-04 18:38:21.227674 s_tool-0.0.4/s_tool/core.py
+-rw-r--r--   0        0        0     2407 2023-06-04 18:38:21.227674 s_tool-0.0.4/s_tool/driver.py
+-rw-r--r--   0        0        0      537 2023-06-04 18:38:21.227674 s_tool-0.0.4/s_tool/exceptions.py
+-rw-r--r--   0        0        0       95 2023-06-04 18:38:21.227674 s_tool-0.0.4/s_tool/logger.py
+-rw-r--r--   0        0        0     1334 2023-06-04 18:38:21.227674 s_tool-0.0.4/s_tool/parser.py
+-rw-r--r--   0        0        0     4655 1970-01-01 00:00:00.000000 s_tool-0.0.4/PKG-INFO
```

### Comparing `s-tool-0.0.3/LICENSE` & `s_tool-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `s-tool-0.0.3/pyproject.toml` & `s_tool-0.0.4/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 [tool.poetry]
 name = "s-tool"
-version = "0.0.3"
+version = "0.0.4"
 description = "Selenium wrapper to make your life easy."
-authors = ["Ravishankar Chavare", "Aahnik Daw <daw@aahnik.dev>"]
+authors = ["Ravishankar Chavare <chavare.ravi123@gmail.com>", "Aahnik Daw <daw@aahnik.dev>"]
+packages = [{include = "s_tool"}]
+
 license = "MIT"
-readme = "README.md"
+readme = "README.rst"
 repository = "https://github.com/Python-World/s-tool"
-keywords = ["python","selenium","wrapper",'web-driver']
+keywords = ["Python","Selenium","wrapper",'Webdriver',"Tools","Utilities"]
 classifiers = [
   "License :: OSI Approved :: MIT License",
   "Natural Language :: English",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
   "Intended Audience :: Education",
   "Intended Audience :: Information Technology",
   "Development Status :: 4 - Beta",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.8"
-selenium = "^3.141.0"
-webdriver-manager = "^3.4.2"
+python = "^3.11"
+selenium = "^4.9.1"
+lxml    = "^4.9.2"
+webdriver-manager = "^3.8.5"
 
 [tool.poetry.dev-dependencies]
-tox = "^3.23.1"
-black = "^21.6b0"
-isort = "^5.9.1"
+tox = "^4.5.1"
+black = "^23.3.0"
+isort = "^5.12.0"
 pre-commit = "^2.13.0"
-pytest = "^6.2.4"
-pytest-cov = "^2.12.1"
+pytest = "^7.3.0"
+pytest-cov = "^4.1.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
@@ -55,9 +58,7 @@
     | dist
   )/
   | foo.py           # also separately exclude a file named foo.py in
                      # the root of the project
 )
 '''
 
-[tool.pytest.ini_options]
-addopts = "--cov=./s_tool --cov-report=term-missing --cov-report=xml --cov-report=html"
```

