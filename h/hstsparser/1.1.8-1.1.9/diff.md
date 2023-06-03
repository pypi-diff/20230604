# Comparing `tmp/hstsparser-1.1.8.tar.gz` & `tmp/hstsparser-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hstsparser-1.1.8.tar", max compression
+gzip compressed data, was "hstsparser-1.1.9.tar", max compression
```

## Comparing `hstsparser-1.1.8.tar` & `hstsparser-1.1.9.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1070 2023-05-27 00:18:43.203215 hstsparser-1.1.8/LICENSE
--rw-r--r--   0        0        0     2949 2023-05-27 00:18:43.203215 hstsparser-1.1.8/README.md
--rwxr-xr-x   0        0        0     6552 2023-05-27 00:18:43.203215 hstsparser-1.1.8/hstsparser.py
--rw-r--r--   0        0        0     1368 2023-05-27 00:19:12.719627 hstsparser-1.1.8/pyproject.toml
--rw-r--r--   0        0        0     3866 1970-01-01 00:00:00.000000 hstsparser-1.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-03 23:16:54.445967 hstsparser-1.1.9/LICENSE
+-rw-r--r--   0        0        0     3180 2023-06-03 23:16:54.445967 hstsparser-1.1.9/README.md
+-rwxr-xr-x   0        0        0     7678 2023-06-03 23:16:54.449967 hstsparser-1.1.9/hstsparser.py
+-rw-r--r--   0        0        0     1407 2023-06-03 23:17:17.338171 hstsparser-1.1.9/pyproject.toml
+-rw-r--r--   0        0        0     4086 1970-01-01 00:00:00.000000 hstsparser-1.1.9/PKG-INFO
```

### Comparing `hstsparser-1.1.8/LICENSE` & `hstsparser-1.1.9/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2019 Daniel Milnes
+Copyright (c) 2023 Daniel Milnes
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `hstsparser-1.1.8/README.md` & `hstsparser-1.1.9/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -2,23 +2,36 @@
 
 [![Lint Codebase](https://github.com/thebeanogamer/hstsparser/actions/workflows/lint.yaml/badge.svg)](https://github.com/thebeanogamer/hstsparser/actions/workflows/lint.yaml) [![Build Releases](https://github.com/thebeanogamer/hstsparser/actions/workflows/build.yaml/badge.svg)](https://github.com/thebeanogamer/hstsparser/actions/workflows/build.yaml) [![Licence](https://img.shields.io/github/license/thebeanogamer/hstsparser)](./LICENSE) ![Python 3.11.x](https://img.shields.io/badge/python-3.11.x-yellow.svg) [![PyPI](https://img.shields.io/pypi/v/hstsparser)](https://pypi.org/project/hstsparser) [![Downloads](https://pepy.tech/badge/hstsparser)](https://pepy.tech/project/hstsparser) [![Copr build status](https://copr.fedorainfracloud.org/coprs/thebeanogamer/hstsparser/package/hstsparser/status_image/last_build.png)](https://copr.fedorainfracloud.org/coprs/thebeanogamer/hstsparser/package/hstsparser/)
 
 HSTS Parser is a simple tool to parse Firefox and Chrome's HSTS databases into actually helpful forensic artifacts! You can read more about the research behind this tool and potential uses for it over on [my blog](https://blog.daniel-milnes.uk/hsts-for-forensics-you-can-run-but-you-cant)!
 
 ## Installation
 
-HSTS Parser can be installed via pip, or with [Poetry](https://python-poetry.org/).
+HSTS Parser can be installed via pip, or as a native executable.
 
 ### From PyPi
 
+If you already have Python installed, you can install HSTS Parser using pip.
+
 ```bash
 pip install hstsparser
 ```
 
-Alternatively, if you're using Windows, you can use the executables on the [releases page](https://github.com/thebeanogamer/hstsparser/releases/latest) to not need to install anything at all.
+### On Fedora
+
+HSTS Parser is available through Fedora COPR for Fedora 38+.
+
+```bash
+dnf copr enable thebeanogamer/hstsparser
+dnf install hstsparser
+```
+
+### On Windows
+
+Windows binaries are published by GitHub Actions CI for each release of HSTS Parser. You can download these on the [releases page](https://github.com/thebeanogamer/hstsparser/releases/latest).
 
 ## Usage
 
 All of the below documentation is written for the Python version rather than the standalone executable, but the commands will be the same.
 
 ```shell
 $ hstsparser -h
@@ -67,8 +80,8 @@
 
 ![Screenshot of Chrome Processing with a wordlist](https://blog.daniel-milnes.uk/content/images/2019/11/image-4.png)
 
 ## Links
 
 - [My Blog Post](https://blog.daniel-milnes.uk/hsts-for-forensics-you-can-run-but-you-cant)
 - [MDN - HSTS](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Strict-Transport-Security)
-- [Chromium - HSTS](https://www.chromium.org/sts)
+- [Chromium - HSTS](https://www.chromium.org/hsts)
```

### Comparing `hstsparser-1.1.8/hstsparser.py` & `hstsparser-1.1.9/hstsparser.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,30 @@
 #!/usr/bin/env python3
+# SPDX-License-Identifier: MIT
+#
+# Copyright (c) 2023 Daniel Milnes
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
 
 import csv
 import datetime
 import importlib.metadata
 import json
 import os
 import re
```

### Comparing `hstsparser-1.1.8/pyproject.toml` & `hstsparser-1.1.9/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hstsparser"
-version = "1.1.8"
+version = "1.1.9"
 description = "A tool to parse Firefox and Chrome HSTS databases into forensic artifacts."
 authors = ["Daniel Milnes <daniel@daniel-milnes.uk>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/thebeanogamer/hstsparser"
 repository = "https://github.com/thebeanogamer/hstsparser"
 documentation = "https://github.com/thebeanogamer/hstsparser"
@@ -16,22 +16,22 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Security",
     "Topic :: Utilities"
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.9,<3.12"
-prettytable = ">=0.7.2,<3.8"
+python = ">=3.9"
+prettytable = ">=0.7.2"
 
 [tool.poetry.scripts]
 hstsparser = "hstsparser:main"
 
 [tool.poetry.group.windows.dependencies]
-pyinstaller = "^5.11.0"
+pyinstaller = [{ version = "^5.11.0", python = ">=3.9,<3.12" }]
 pywin32-ctypes = "^0.2.0"
 pefile = "^2023.2.7"
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "^6.0.0"
 flake8-bandit = "^4.1.1"
 flake8-bugbear = "^23.5.9"
@@ -39,10 +39,10 @@
 flake8-string-format = "^0.3.0"
 flake8-tidy-imports = "^4.8.0"
 flake8-todo = "^0.7"
 safety = "^2.3.5"
 flake8-formatter-junit-xml = "^0.0.6"
 
 [build-system]
-requires = ["poetry>=1.3"]
-build-backend = "poetry.masonry.api"
+requires = ["poetry-core>=1.3"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `hstsparser-1.1.8/PKG-INFO` & `hstsparser-1.1.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,47 +1,60 @@
 Metadata-Version: 2.1
 Name: hstsparser
-Version: 1.1.8
+Version: 1.1.9
 Summary: A tool to parse Firefox and Chrome HSTS databases into forensic artifacts.
 Home-page: https://github.com/thebeanogamer/hstsparser
 License: MIT
 Keywords: chrome,firefox,dfir,forensics,hsts
 Author: Daniel Milnes
 Author-email: daniel@daniel-milnes.uk
-Requires-Python: >=3.9,<3.12
+Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
-Requires-Dist: prettytable (>=0.7.2,<3.8)
+Requires-Dist: prettytable (>=0.7.2)
 Project-URL: Documentation, https://github.com/thebeanogamer/hstsparser
 Project-URL: Repository, https://github.com/thebeanogamer/hstsparser
 Description-Content-Type: text/markdown
 
 # HSTS Parser
 
 [![Lint Codebase](https://github.com/thebeanogamer/hstsparser/actions/workflows/lint.yaml/badge.svg)](https://github.com/thebeanogamer/hstsparser/actions/workflows/lint.yaml) [![Build Releases](https://github.com/thebeanogamer/hstsparser/actions/workflows/build.yaml/badge.svg)](https://github.com/thebeanogamer/hstsparser/actions/workflows/build.yaml) [![Licence](https://img.shields.io/github/license/thebeanogamer/hstsparser)](./LICENSE) ![Python 3.11.x](https://img.shields.io/badge/python-3.11.x-yellow.svg) [![PyPI](https://img.shields.io/pypi/v/hstsparser)](https://pypi.org/project/hstsparser) [![Downloads](https://pepy.tech/badge/hstsparser)](https://pepy.tech/project/hstsparser) [![Copr build status](https://copr.fedorainfracloud.org/coprs/thebeanogamer/hstsparser/package/hstsparser/status_image/last_build.png)](https://copr.fedorainfracloud.org/coprs/thebeanogamer/hstsparser/package/hstsparser/)
 
 HSTS Parser is a simple tool to parse Firefox and Chrome's HSTS databases into actually helpful forensic artifacts! You can read more about the research behind this tool and potential uses for it over on [my blog](https://blog.daniel-milnes.uk/hsts-for-forensics-you-can-run-but-you-cant)!
 
 ## Installation
 
-HSTS Parser can be installed via pip, or with [Poetry](https://python-poetry.org/).
+HSTS Parser can be installed via pip, or as a native executable.
 
 ### From PyPi
 
+If you already have Python installed, you can install HSTS Parser using pip.
+
 ```bash
 pip install hstsparser
 ```
 
-Alternatively, if you're using Windows, you can use the executables on the [releases page](https://github.com/thebeanogamer/hstsparser/releases/latest) to not need to install anything at all.
+### On Fedora
+
+HSTS Parser is available through Fedora COPR for Fedora 38+.
+
+```bash
+dnf copr enable thebeanogamer/hstsparser
+dnf install hstsparser
+```
+
+### On Windows
+
+Windows binaries are published by GitHub Actions CI for each release of HSTS Parser. You can download these on the [releases page](https://github.com/thebeanogamer/hstsparser/releases/latest).
 
 ## Usage
 
 All of the below documentation is written for the Python version rather than the standalone executable, but the commands will be the same.
 
 ```shell
 $ hstsparser -h
@@ -90,9 +103,9 @@
 
 ![Screenshot of Chrome Processing with a wordlist](https://blog.daniel-milnes.uk/content/images/2019/11/image-4.png)
 
 ## Links
 
 - [My Blog Post](https://blog.daniel-milnes.uk/hsts-for-forensics-you-can-run-but-you-cant)
 - [MDN - HSTS](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Strict-Transport-Security)
-- [Chromium - HSTS](https://www.chromium.org/sts)
+- [Chromium - HSTS](https://www.chromium.org/hsts)
```

