# Comparing `tmp/caqui-1.0.6.tar.gz` & `tmp/caqui-1.0.7.tar.gz`

## Comparing `caqui-1.0.6.tar` & `caqui-1.0.7.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 caqui-1.0.6/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 caqui-1.0.6/CONTRIBUTING.md
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 caqui-1.0.6/sample.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 caqui-1.0.6/test-requirements.txt
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 caqui-1.0.6/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 caqui-1.0.6/.github/ISSUE_TEMPLATE/custom.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 caqui-1.0.6/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 caqui-1.0.6/.github/workflows/python-app.yml
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 caqui-1.0.6/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 caqui-1.0.6/.vscode/settings.json
--rw-r--r--   0        0        0    43559 2020-02-02 00:00:00.000000 caqui-1.0.6/caqui/__init__.py
--rw-r--r--   0        0        0     7055 2020-02-02 00:00:00.000000 caqui-1.0.6/caqui/asynchronous.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 caqui-1.0.6/caqui/constants.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 caqui-1.0.6/caqui/exceptions.py
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 caqui-1.0.6/caqui/helper.py
--rw-r--r--   0        0        0     6828 2020-02-02 00:00:00.000000 caqui-1.0.6/caqui/synchronous.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 caqui-1.0.6/tests/__init__.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 caqui-1.0.6/tests/constants.py
--rw-r--r--   0        0        0     3845 2020-02-02 00:00:00.000000 caqui-1.0.6/tests/fake_responses.py
--rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 caqui-1.0.6/tests/test_sniffer.py
--rw-r--r--   0        0        0     4515 2020-02-02 00:00:00.000000 caqui-1.0.6/tests/feature/test_sync_and_async.py
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 caqui-1.0.6/tests/html/playground.html
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 caqui-1.0.6/tests/integration/test_async_scenarios.py
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 caqui-1.0.6/tests/integration/test_sync_scenarios.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 caqui-1.0.6/tests/unit/__initi__.py
--rw-r--r--   0        0        0     3608 2020-02-02 00:00:00.000000 caqui-1.0.6/tests/unit/test_async_unit.py
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 caqui-1.0.6/tests/unit/test_helper.py
--rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 caqui-1.0.6/tests/unit/test_sync_unit.py
--rwxr-xr-x   0        0        0       77 2020-02-02 00:00:00.000000 caqui-1.0.6/utils/coverage.sh
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 caqui-1.0.6/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 caqui-1.0.6/LICENSE
--rw-r--r--   0        0        0     9801 2020-02-02 00:00:00.000000 caqui-1.0.6/README.md
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 caqui-1.0.6/pyproject.toml
--rw-r--r--   0        0        0    10401 2020-02-02 00:00:00.000000 caqui-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 caqui-1.0.7/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 caqui-1.0.7/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 caqui-1.0.7/sample.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 caqui-1.0.7/test-requirements.txt
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 caqui-1.0.7/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 caqui-1.0.7/.github/ISSUE_TEMPLATE/custom.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 caqui-1.0.7/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 caqui-1.0.7/.github/workflows/python-app.yml
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 caqui-1.0.7/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 caqui-1.0.7/.vscode/settings.json
+-rw-r--r--   0        0        0    43559 2020-02-02 00:00:00.000000 caqui-1.0.7/caqui/__init__.py
+-rw-r--r--   0        0        0     7796 2020-02-02 00:00:00.000000 caqui-1.0.7/caqui/asynchronous.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 caqui-1.0.7/caqui/constants.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 caqui-1.0.7/caqui/exceptions.py
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 caqui-1.0.7/caqui/helper.py
+-rw-r--r--   0        0        0     7546 2020-02-02 00:00:00.000000 caqui-1.0.7/caqui/synchronous.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 caqui-1.0.7/tests/__init__.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 caqui-1.0.7/tests/constants.py
+-rw-r--r--   0        0        0     4147 2020-02-02 00:00:00.000000 caqui-1.0.7/tests/fake_responses.py
+-rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 caqui-1.0.7/tests/test_sniffer.py
+-rw-r--r--   0        0        0     4515 2020-02-02 00:00:00.000000 caqui-1.0.7/tests/feature/test_sync_and_async.py
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 caqui-1.0.7/tests/html/playground.html
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 caqui-1.0.7/tests/integration/test_async_scenarios.py
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 caqui-1.0.7/tests/integration/test_sync_scenarios.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 caqui-1.0.7/tests/unit/__initi__.py
+-rw-r--r--   0        0        0     4155 2020-02-02 00:00:00.000000 caqui-1.0.7/tests/unit/test_async_unit.py
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 caqui-1.0.7/tests/unit/test_helper.py
+-rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 caqui-1.0.7/tests/unit/test_sync_unit.py
+-rwxr-xr-x   0        0        0       77 2020-02-02 00:00:00.000000 caqui-1.0.7/utils/coverage.sh
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 caqui-1.0.7/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 caqui-1.0.7/LICENSE
+-rw-r--r--   0        0        0     9801 2020-02-02 00:00:00.000000 caqui-1.0.7/README.md
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 caqui-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0    10401 2020-02-02 00:00:00.000000 caqui-1.0.7/PKG-INFO
```

### Comparing `caqui-1.0.6/CODE_OF_CONDUCT.md` & `caqui-1.0.7/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `caqui-1.0.6/sample.py` & `caqui-1.0.7/sample.py`

 * *Files identical despite different names*

### Comparing `caqui-1.0.6/.github/ISSUE_TEMPLATE/bug_report.md` & `caqui-1.0.7/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `caqui-1.0.6/.github/ISSUE_TEMPLATE/feature_request.md` & `caqui-1.0.7/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `caqui-1.0.6/.github/workflows/python-app.yml` & `caqui-1.0.7/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `caqui-1.0.6/.github/workflows/python-publish.yml` & `caqui-1.0.7/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `caqui-1.0.6/caqui/__init__.py` & `caqui-1.0.7/caqui/__init__.py`

 * *Files identical despite different names*

### Comparing `caqui-1.0.6/caqui/asynchronous.py` & `caqui-1.0.7/caqui/asynchronous.py`

 * *Files 4% similar despite different names*

```diff
@@ -118,24 +118,40 @@
     try:
         url = f"{driver_url}/session/{session}/element/{element}/property/{property}"
         response = await __get(url)
         return response.get("value")
     except Exception as error:
         raise WebDriverError("Failed to get value from element.") from error
 
+async def get_attribute(driver_url, session, element, attribute):
+    """Get the given HTML attribute of an element, for example, 'aria-valuenow'"""
+    try:
+        url = f"{driver_url}/session/{session}/element/{element}/attribute/{attribute}"
+        response = await __get(url)
+        return response.get("value")
+    except Exception as error:
+        raise WebDriverError("Failed to get value from element.") from error
 
 async def get_text(driver_url, session, element):
     """Get the text of an element"""
     try:
         url = f"{driver_url}/session/{session}/element/{element}/text"
         response = await __get(url)
         return response.get("value")
     except Exception as error:
         raise WebDriverError("Failed to get text from element.") from error
 
+async def get_cookies(driver_url, session):
+    """Get the page cookies"""
+    try:
+        url = f"{driver_url}/session/{session}/cookie"
+        response = await __get(url)
+        return response.get("value")
+    except Exception as error:
+        raise WebDriverError("Failed to get page cookies.") from error
 
 async def close_session(driver_url, session):
     """Close an opened session and close the browser"""
     try:
         url = f"{driver_url}/session/{session}"
         await __delete(url)
         return True
```

### Comparing `caqui-1.0.6/caqui/synchronous.py` & `caqui-1.0.7/caqui/synchronous.py`

 * *Files 8% similar despite different names*

```diff
@@ -114,14 +114,31 @@
     try:
         url = f"{driver_url}/session/{session}/element/{element}/property/{property}"
         response = __get(url)
         return response.get("value")
     except Exception as error:
         raise WebDriverError("Failed to get value from element.") from error
 
+def get_attribute(driver_url, session, element, attribute):
+    """Get the given HTML attribute of an element, for example, 'aria-valuenow'"""
+    try:
+        url = f"{driver_url}/session/{session}/element/{element}/attribute/{attribute}"
+        response = __get(url)
+        return response.get("value")
+    except Exception as error:
+        raise WebDriverError("Failed to get value from element.") from error
+
+def get_cookies(driver_url, session):
+    """Get the page cookies"""
+    try:
+        url = f"{driver_url}/session/{session}/cookie"
+        response = __get(url)
+        return response.get("value")
+    except Exception as error:
+        raise WebDriverError("Failed to get page cookies.") from error
 
 def go_to_page(driver_url, session, page_url):
     """Navigate to 'page_url'"""
     try:
         url = f"{driver_url}/session/{session}/url"
         payload = json.dumps({"url": page_url})
         __post(url, payload)
```

### Comparing `caqui-1.0.6/tests/fake_responses.py` & `caqui-1.0.7/tests/fake_responses.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,14 +63,23 @@
     {
         "sessionId": "07b00b2e94be84920495d83890c82b60",
         "status": 0,
         "value": "Sample page",
     }
 )
 
+GET_COOKIES = dict_to_json(
+    {
+        "sessionId": "07b00b2e94be84920495d83890c82b60",
+        "status": 0,
+        "value": [],
+    }
+)
+
+
 FIND_ELEMENTS = dict_to_json(
     {
         "sessionId": "9be93a374d185216134bf0c3fafee52e",
         "status": 0,
         "value": [
             {"ELEMENT": "C230605181E69CB2C4C36B8E83FE1245_element_1"},
             {"ELEMENT": "C230605181E69CB2C4C36B8E83FE1245_element_2"},
@@ -83,14 +92,22 @@
     {
         "sessionId": "5be82d4cd17af92d7ea53a36900d78cb",
         "status": 0,
         "value": "any_value",
     }
 )
 
+GET_ATTRIBUTE_VALUE = dict_to_json(
+    {
+        "sessionId": "5be82d4cd17af92d7ea53a36900d78cb",
+        "status": 0,
+        "value": "any_value",
+    }
+)
+
 GET_TEXT = dict_to_json(
     {"sessionId": "5be82d4cd17af92d7ea53a36900d78cb", "status": 0, "value": "any"}
 )
 
 GET_SESSION = dict_to_json(
     {
         "sessionId": "4358a5b53794586af59678fc1653dc40",
```

### Comparing `caqui-1.0.6/tests/test_sniffer.py` & `caqui-1.0.7/tests/test_sniffer.py`

 * *Files identical despite different names*

### Comparing `caqui-1.0.6/tests/feature/test_sync_and_async.py` & `caqui-1.0.7/tests/feature/test_sync_and_async.py`

 * *Files identical despite different names*

### Comparing `caqui-1.0.6/tests/html/playground.html` & `caqui-1.0.7/tests/html/playground.html`

 * *Files identical despite different names*

### Comparing `caqui-1.0.6/tests/integration/test_async_scenarios.py` & `caqui-1.0.7/tests/integration/test_async_scenarios.py`

 * *Files identical despite different names*

### Comparing `caqui-1.0.6/tests/integration/test_sync_scenarios.py` & `caqui-1.0.7/tests/integration/test_sync_scenarios.py`

 * *Files identical despite different names*

### Comparing `caqui-1.0.6/tests/unit/test_async_unit.py` & `caqui-1.0.7/tests/unit/test_async_unit.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,14 +23,23 @@
 
     async def mock_post(*args):
         return fake_responses.GET_PROPERTY_VALUE
 
     with patch("caqui.asynchronous.__get", mock_post):
         assert await asynchronous.get_property("", "", "", "") == expected
 
+@mark.asyncio
+async def test_get_attribute():
+    expected = "any_value"
+
+    async def mock_post(*args):
+        return fake_responses.GET_ATTRIBUTE_VALUE
+
+    with patch("caqui.asynchronous.__get", mock_post):
+        assert await asynchronous.get_attribute("", "", "", "") == expected
 
 @mark.asyncio
 async def test_get_url():
     expected = "playground.html"
 
     async def mock_post(*args):
         return fake_responses.GET_URL
@@ -68,14 +77,23 @@
 
     async def mock_post(*args):
         return fake_responses.GET_TITLE
 
     with patch("caqui.asynchronous.__get", mock_post):
         assert await asynchronous.get_title("", "") == expected
 
+@mark.asyncio
+async def test_get_cookies():
+    expected = []
+
+    async def mock_post(*args):
+        return fake_responses.GET_COOKIES
+
+    with patch("caqui.asynchronous.__get", mock_post):
+        assert await asynchronous.get_cookies("", "") == expected
 
 @mark.asyncio
 async def test_get_text():
     expected = "any"
 
     async def mock_post(*args):
         return fake_responses.GET_TEXT
```

### Comparing `caqui-1.0.6/tests/unit/test_helper.py` & `caqui-1.0.7/tests/unit/test_helper.py`

 * *Files identical despite different names*

### Comparing `caqui-1.0.6/tests/unit/test_sync_unit.py` & `caqui-1.0.7/tests/unit/test_sync_unit.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,19 @@
 
 @patch("requests.request", return_value=fake_responses.GET_TITLE)
 def test_get_title(*args):
     expected = "Sample page"
 
     assert synchronous.get_title("", "") == expected
 
+@patch("requests.request", return_value=fake_responses.GET_COOKIES)
+def test_get_cookies(*args):
+    expected = []
+
+    assert synchronous.get_cookies("", "") == expected
 
 @patch("requests.request", return_value=fake_responses.FIND_ELEMENTS)
 def test_find_elements(*args):
     element = "C230605181E69CB2C4C36B8E83FE1245_element_2"
 
     elements = synchronous.find_elements("", "", "", "")
 
@@ -41,14 +46,19 @@
 
 @patch("requests.request", return_value=fake_responses.GET_PROPERTY_VALUE)
 def test_get_property(*args):
     expected = "any_value"
 
     assert synchronous.get_property("", "", "", "") == expected
 
+@patch("requests.request", return_value=fake_responses.GET_ATTRIBUTE_VALUE)
+def test_get_attribute(*args):
+    expected = "any_value"
+
+    assert synchronous.get_attribute("", "", "", "") == expected
 
 @patch("requests.request", return_value=fake_responses.GO_TO_PAGE)
 def test_go_to_page(*args):
     assert synchronous.go_to_page("", "", "") is True
 
 
 @patch("requests.request", return_value=fake_responses.CLOSE_SESSION)
```

### Comparing `caqui-1.0.6/.gitignore` & `caqui-1.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `caqui-1.0.6/LICENSE` & `caqui-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `caqui-1.0.6/README.md` & `caqui-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `caqui-1.0.6/pyproject.toml` & `caqui-1.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.setuptools.packages.find]
 include = ["caqui*"]
 exclude = ["tests*", "utils", ".vscode", ".git*", "dist"]
 
 [project]
 name = "caqui"
-version = "1.0.6"
+version = "1.0.7"
 authors = [
   { name="Douglas Cardoso", email="noemail@noemail.com" },
 ]
 description = "Run asynchronous commands in WebDrivers"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -25,8 +25,8 @@
 dependencies = [
   "requests",
   "aiohttp"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/douglasdcm/caqui"
-"Bug Tracker" = "https://github.com/douglasdcm/caqui/issues"
+"Bug Tracker" = "https://github.com/douglasdcm/caqui/issues"
```

### Comparing `caqui-1.0.6/PKG-INFO` & `caqui-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caqui
-Version: 1.0.6
+Version: 1.0.7
 Summary: Run asynchronous commands in WebDrivers
 Project-URL: Homepage, https://github.com/douglasdcm/caqui
 Project-URL: Bug Tracker, https://github.com/douglasdcm/caqui/issues
 Author-email: Douglas Cardoso <noemail@noemail.com>
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: caqui Version: 1.0.6 Summary: Run asynchronous
+Metadata-Version: 2.1 Name: caqui Version: 1.0.7 Summary: Run asynchronous
 commands in WebDrivers Project-URL: Homepage, https://github.com/douglasdcm/
 caqui Project-URL: Bug Tracker, https://github.com/douglasdcm/caqui/issues
 Author-email: Douglas Cardoso
 noemail.com> License-File: LICENSE Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python :: 3 Requires-
 Python: >=3.7 Requires-Dist: aiohttp Requires-Dist: requests Description-
```

