# Comparing `tmp/readfcs-1.1.1.tar.gz` & `tmp/readfcs-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readfcs-1.1.1.tar", last modified: Tue Feb  7 14:34:48 2023, max compression
+gzip compressed data, was "readfcs-1.1.2.tar", last modified: Sun Jun  4 13:48:23 2023, max compression
```

## Comparing `readfcs-1.1.1.tar` & `readfcs-1.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     2551 2023-01-12 16:27:09.495572 readfcs-1.1.1/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2022-07-25 08:22:00.201619 readfcs-1.1.1/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2022-07-25 08:22:00.201910 readfcs-1.1.1/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1207 2022-08-30 14:21:07.236348 readfcs-1.1.1/.gitignore
--rw-r--r--   0        0        0     1943 2022-07-10 14:01:24.300288 readfcs-1.1.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      624 2022-08-30 14:11:54.721602 readfcs-1.1.1/CITATION.cff
--rw-r--r--   0        0        0    11324 2022-05-28 11:31:06.237861 readfcs-1.1.1/LICENSE
--rw-r--r--   0        0        0      759 2023-02-07 14:32:21.099727 readfcs-1.1.1/README.md
--rw-r--r--   0        0        0       49 2022-05-28 10:53:31.440992 readfcs-1.1.1/docs/api.md
--rw-r--r--   0        0        0     3119 2023-02-07 14:33:21.052421 readfcs-1.1.1/docs/changelog.md
--rw-r--r--   0        0        0      277 2023-01-12 16:27:09.497287 readfcs-1.1.1/docs/index.md
--rw-r--r--   0        0        0     5188 2023-01-20 06:57:41.322794 readfcs-1.1.1/docs/quickstart.ipynb
--rw-r--r--   0        0        0      119 2022-08-30 14:11:54.723988 readfcs-1.1.1/lamin-project.yaml
--rw-r--r--   0        0        0      726 2023-01-12 16:27:09.497510 readfcs-1.1.1/noxfile.py
--rw-r--r--   0        0        0      924 2023-01-12 16:30:57.438715 readfcs-1.1.1/pyproject.toml
--rw-r--r--   0        0        0      390 2023-02-07 14:33:12.656108 readfcs-1.1.1/readfcs/__init__.py
--rw-r--r--   0        0        0     8353 2023-02-07 14:32:21.100131 readfcs-1.1.1/readfcs/_core.py
--rw-r--r--   0        0        0       94 2022-08-22 13:26:31.136399 readfcs-1.1.1/readfcs/datasets/__init__.py
--rw-r--r--   0        0        0      362 2022-08-22 13:56:28.582426 readfcs-1.1.1/readfcs/datasets/_datasets.py
--rw-r--r--   0        0        0       88 2022-07-11 14:13:41.976849 readfcs-1.1.1/tests/test_base.py
--rw-r--r--   0        0        0      511 2022-08-19 10:15:11.545755 readfcs-1.1.1/tests/test_notebooks.py
--rw-r--r--   0        0        0     1608 1970-01-01 00:00:00.000000 readfcs-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2680 2023-06-04 12:02:32.768855 readfcs-1.1.2/.github/workflows/build.yml
+-rw-r--r--   0        0        0      135 2023-06-04 12:02:32.784512 readfcs-1.1.2/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      622 2023-06-04 12:02:32.784512 readfcs-1.1.2/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1317 2023-06-04 12:02:32.800135 readfcs-1.1.2/.gitignore
+-rw-r--r--   0        0        0     2016 2023-06-04 12:02:32.800135 readfcs-1.1.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      647 2023-06-04 12:02:32.806645 readfcs-1.1.2/CITATION.cff
+-rw-r--r--   0        0        0    11525 2023-06-04 12:02:32.806645 readfcs-1.1.2/LICENSE
+-rw-r--r--   0        0        0      769 2023-06-04 12:02:32.822308 readfcs-1.1.2/README.md
+-rw-r--r--   0        0        0       54 2023-06-04 12:02:32.822308 readfcs-1.1.2/docs/api.md
+-rw-r--r--   0        0        0     3398 2023-06-04 13:47:53.407778 readfcs-1.1.2/docs/changelog.md
+-rw-r--r--   0        0        0      294 2023-06-04 12:02:32.837906 readfcs-1.1.2/docs/index.md
+-rw-r--r--   0        0        0     5457 2023-06-04 12:02:32.837906 readfcs-1.1.2/docs/quickstart.ipynb
+-rw-r--r--   0        0        0      124 2023-06-04 12:02:32.853531 readfcs-1.1.2/lamin-project.yaml
+-rw-r--r--   0        0        0      754 2023-06-04 12:02:32.853531 readfcs-1.1.2/noxfile.py
+-rw-r--r--   0        0        0      979 2023-06-04 13:47:05.474936 readfcs-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0      390 2023-06-04 13:47:54.147296 readfcs-1.1.2/readfcs/__init__.py
+-rw-r--r--   0        0        0     8610 2023-06-04 12:02:32.884781 readfcs-1.1.2/readfcs/_core.py
+-rw-r--r--   0        0        0      103 2023-06-04 12:02:32.884781 readfcs-1.1.2/readfcs/datasets/__init__.py
+-rw-r--r--   0        0        0      377 2023-06-04 12:02:32.900407 readfcs-1.1.2/readfcs/datasets/_datasets.py
+-rw-r--r--   0        0        0       93 2023-06-04 12:02:32.906917 readfcs-1.1.2/tests/test_base.py
+-rw-r--r--   0        0        0      526 2023-06-04 13:47:05.484968 readfcs-1.1.2/tests/test_notebooks.py
+-rw-r--r--   0        0        0     1631 1970-01-01 00:00:00.000000 readfcs-1.1.2/PKG-INFO
```

### Comparing `readfcs-1.1.1/.github/workflows/build.yml` & `readfcs-1.1.2/.github/workflows/build.yml`

 * *Files 14% similar despite different names*

```diff
@@ -1,82 +1,83 @@
-name: build
-
-on:
-  push:
-    branches: [main]
-  pull_request:
-    branches: [main]
-
-jobs:
-  build:
-    runs-on: ubuntu-latest
-    strategy:
-      fail-fast: false
-      matrix:
-        python-version: ["3.7", "3.8", "3.9", "3.10"]
-    timeout-minutes: 10
-
-    steps:
-      - name: Checkout main
-        uses: actions/checkout@v3
-        with:
-          fetch-depth: 0
-      - name: Checkout lndocs
-        uses: actions/checkout@v3
-        with:
-          repository: laminlabs/lndocs
-          path: lndocs
-          ref: main
-      - name: Setup Python
-        uses: actions/setup-python@v3
-        with:
-          python-version: ${{ matrix.python-version }}
-      - name: Cache
-        uses: actions/cache@v3
-        env:
-          cache-name: cache-all
-        with:
-          path: |
-            .nox
-            ~/.cache/pre-commit
-          key: ${{ runner.os }}-build-${{ env.cache-name }}-${{ hashFiles('.pre-commit-config.yaml') }}-${{ hashFiles('pyproject.yaml') }}
-      - name: Install pip and nox
-        run: |
-          python -m pip install --upgrade pip
-          pip install nox
-      - name: Lint
-        if: matrix.python-version == '3.9'
-        run: |
-          nox -s lint --python ${{ matrix.python-version }}
-      - name: Build
-        run: |
-          nox -s build --python ${{ matrix.python-version }}
-      - name: Read lamin-project.yaml
-        if: matrix.python-version == '3.9'
-        id: lamin-project
-        uses: CumulusDS/get-yaml-paths-action@v0.1.0
-        with:
-          file: lamin-project.yaml
-          project_slug: project_slug
-      - name: Change base URL to project-slug
-        if: github.event_name == 'push' && matrix.python-version == '3.9'
-        run: |
-          mv _build/html _build/${{ steps.lamin-project.outputs.project_slug }}
-          mkdir -p _build/html/docs
-          mv _build/${{ steps.lamin-project.outputs.project_slug }} _build/html/docs
-      - name: Deploy docs
-        if: matrix.python-version == '3.9'
-        id: netlify
-        uses: nwtgck/actions-netlify@v1.2
-        with:
-          publish-dir: "_build/html"
-          production-deploy: ${{ github.event_name == 'push' }}
-          github-token: ${{ secrets.GITHUB_TOKEN }}
-          enable-commit-comment: false
-        env:
-          NETLIFY_AUTH_TOKEN: ${{ secrets.NETLIFY_AUTH_TOKEN }}
-          NETLIFY_SITE_ID: ${{ secrets.NETLIFY_SITE_ID }}
-      - name: Codecov
-        if: matrix.python-version == '3.9'
-        uses: codecov/codecov-action@v2
-        with:
-          token: ${{ secrets.CODECOV_TOKEN }}
+name: build
+
+on:
+  push:
+    branches: [main]
+  pull_request:
+    branches: [main]
+
+jobs:
+  build:
+    runs-on: ubuntu-latest
+    strategy:
+      fail-fast: false
+      matrix:
+        python-version: ["3.7", "3.8", "3.9", "3.10"]
+    timeout-minutes: 10
+
+    steps:
+      - name: Checkout main
+        uses: actions/checkout@v3
+        with:
+          fetch-depth: 0
+      - name: Checkout lndocs
+        uses: actions/checkout@v3
+        with:
+          repository: laminlabs/lndocs
+          ssh-key: ${{ secrets.READ_LNDOCS }}
+          path: lndocs
+          ref: main
+      - name: Setup Python
+        uses: actions/setup-python@v3
+        with:
+          python-version: ${{ matrix.python-version }}
+      - name: Cache
+        uses: actions/cache@v3
+        env:
+          cache-name: cache-all
+        with:
+          path: |
+            .nox
+            ~/.cache/pre-commit
+          key: ${{ runner.os }}-build-${{ env.cache-name }}-${{ hashFiles('.pre-commit-config.yaml') }}-${{ hashFiles('pyproject.yaml') }}
+      - name: Install pip and nox
+        run: |
+          python -m pip install --upgrade pip
+          pip install nox
+      - name: Lint
+        if: matrix.python-version == '3.9'
+        run: |
+          nox -s lint --python ${{ matrix.python-version }}
+      - name: Build
+        run: |
+          nox -s build --python ${{ matrix.python-version }}
+      - name: Read lamin-project.yaml
+        if: matrix.python-version == '3.9'
+        id: lamin-project
+        uses: CumulusDS/get-yaml-paths-action@v0.1.0
+        with:
+          file: lamin-project.yaml
+          project_slug: project_slug
+      - name: Change base URL to project-slug
+        if: github.event_name == 'push' && matrix.python-version == '3.9'
+        run: |
+          mv _build/html _build/${{ steps.lamin-project.outputs.project_slug }}
+          mkdir -p _build/html/docs
+          mv _build/${{ steps.lamin-project.outputs.project_slug }} _build/html/docs
+      - name: Deploy docs
+        if: matrix.python-version == '3.9'
+        id: netlify
+        uses: nwtgck/actions-netlify@v1.2
+        with:
+          publish-dir: "_build/html"
+          production-deploy: ${{ github.event_name == 'push' }}
+          github-token: ${{ secrets.GITHUB_TOKEN }}
+          enable-commit-comment: false
+        env:
+          NETLIFY_AUTH_TOKEN: ${{ secrets.NETLIFY_AUTH_TOKEN }}
+          NETLIFY_SITE_ID: ${{ secrets.NETLIFY_SITE_ID }}
+      - name: Codecov
+        if: matrix.python-version == '3.9'
+        uses: codecov/codecov-action@v2
+        with:
+          token: ${{ secrets.CODECOV_TOKEN }}
```

### Comparing `readfcs-1.1.1/.pre-commit-config.yaml` & `readfcs-1.1.2/.pre-commit-config.yaml`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,73 +1,73 @@
-repos:
-  - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v3.2.0
-    hooks:
-      - id: trailing-whitespace
-      - id: end-of-file-fixer
-        exclude: |
-          (?x)(
-              .github/workflows/latest-changes.jinja2
-          )
-      - id: check-yaml
-      - id: check-added-large-files
-  - repo: https://github.com/psf/black
-    rev: 22.3.0
-    hooks:
-      - id: black-jupyter
-  - repo: https://github.com/pycqa/flake8
-    rev: 4.0.1
-    hooks:
-      - id: flake8
-        additional_dependencies:
-          - flake8-black>=0.1.1
-          - flake8-typing-imports==1.10.0
-        language_version: python3
-        args:
-          - --max-line-length=88
-          - --ignore=E203
-          - --min-python-version=3.8.0
-        exclude: |
-          (?x)(
-              __init__.py
-          )
-  - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: v2.6.2
-    hooks:
-      - id: prettier
-  - repo: https://github.com/kynan/nbstripout
-    rev: 0.3.9
-    hooks:
-      - id: nbstripout
-        exclude: |
-          (?x)(
-              docs/tasks/|
-              docs/examples/
-          )
-  - repo: https://github.com/Lucas-C/pre-commit-hooks
-    rev: v1.1.9
-    hooks:
-      - id: forbid-crlf
-      - id: remove-crlf
-  - repo: https://github.com/pre-commit/mirrors-isort
-    rev: v5.8.0
-    hooks:
-      - id: isort
-        args: ["--profile", "black"]
-        exclude: |
-          (?x)(
-              __init__.py
-          )
-  - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v0.940
-    hooks:
-      - id: mypy
-  - repo: https://github.com/pycqa/pydocstyle
-    rev: 6.1.1
-    hooks:
-      - id: pydocstyle
-        args: # google style + __init__, see http://www.pydocstyle.org/en/stable/error_codes.html
-          - --ignore=D100,D101,D102,D103,D105,D107,D203,D204,D213,D215,D400,D401,D402,D403,D404,D406,D407,D408,D409,D413
-        exclude: |
-          (?x)(
-              __init__.py
-          )
+repos:
+  - repo: https://github.com/pre-commit/pre-commit-hooks
+    rev: v3.2.0
+    hooks:
+      - id: trailing-whitespace
+      - id: end-of-file-fixer
+        exclude: |
+          (?x)(
+              .github/workflows/latest-changes.jinja2
+          )
+      - id: check-yaml
+      - id: check-added-large-files
+  - repo: https://github.com/psf/black
+    rev: 22.3.0
+    hooks:
+      - id: black-jupyter
+  - repo: https://github.com/pycqa/flake8
+    rev: 4.0.1
+    hooks:
+      - id: flake8
+        additional_dependencies:
+          - flake8-black>=0.1.1
+          - flake8-typing-imports==1.10.0
+        language_version: python3
+        args:
+          - --max-line-length=88
+          - --ignore=E203
+          - --min-python-version=3.8.0
+        exclude: |
+          (?x)(
+              __init__.py
+          )
+  - repo: https://github.com/pre-commit/mirrors-prettier
+    rev: v2.6.2
+    hooks:
+      - id: prettier
+  - repo: https://github.com/kynan/nbstripout
+    rev: 0.3.9
+    hooks:
+      - id: nbstripout
+        exclude: |
+          (?x)(
+              docs/tasks/|
+              docs/examples/
+          )
+  - repo: https://github.com/Lucas-C/pre-commit-hooks
+    rev: v1.1.9
+    hooks:
+      - id: forbid-crlf
+      - id: remove-crlf
+  - repo: https://github.com/pre-commit/mirrors-isort
+    rev: v5.8.0
+    hooks:
+      - id: isort
+        args: ["--profile", "black"]
+        exclude: |
+          (?x)(
+              __init__.py
+          )
+  - repo: https://github.com/pre-commit/mirrors-mypy
+    rev: v0.940
+    hooks:
+      - id: mypy
+  - repo: https://github.com/pycqa/pydocstyle
+    rev: 6.1.1
+    hooks:
+      - id: pydocstyle
+        args: # google style + __init__, see http://www.pydocstyle.org/en/stable/error_codes.html
+          - --ignore=D100,D101,D102,D103,D105,D107,D203,D204,D213,D215,D400,D401,D402,D403,D404,D406,D407,D408,D409,D413
+        exclude: |
+          (?x)(
+              __init__.py
+          )
```

### Comparing `readfcs-1.1.1/CITATION.cff` & `readfcs-1.1.2/CITATION.cff`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-cff-version: 1.2.0
-title: "readfcs: Read FCS files"
-authors:
-- family-names: Sun
-  given-names: Sunny
-  orcid: https://orcid.org/0000-0002-2365-0888
-- family-names: Wolf
-  given-names: F. Alexander
-  orcid: https://orcid.org/0000-0002-8760-7838
-url: https://github.com/laminlabs/readfcs
-preferred-citation:
-  type: article
-  title: "readfcs: Read FCS files"
-  authors:
-  - family-names: Sun
-    given-names: Sunny
-    orcid: https://orcid.org/0000-0002-2365-0888
-  - family-names: Wolf
-    given-names: F. Alexander
-    orcid: https://orcid.org/0000-0002-8760-7838
-  doi: 10.56528/rfcs
-  journal: Lamin Reports
-  year: 2022
+cff-version: 1.2.0
+title: "readfcs: Read FCS files"
+authors:
+- family-names: Sun
+  given-names: Sunny
+  orcid: https://orcid.org/0000-0002-2365-0888
+- family-names: Wolf
+  given-names: F. Alexander
+  orcid: https://orcid.org/0000-0002-8760-7838
+url: https://github.com/laminlabs/readfcs
+preferred-citation:
+  type: article
+  title: "readfcs: Read FCS files"
+  authors:
+  - family-names: Sun
+    given-names: Sunny
+    orcid: https://orcid.org/0000-0002-2365-0888
+  - family-names: Wolf
+    given-names: F. Alexander
+    orcid: https://orcid.org/0000-0002-8760-7838
+  doi: 10.56528/rfcs
+  journal: Lamin Reports
+  year: 2022
```

### Comparing `readfcs-1.1.1/LICENSE` & `readfcs-1.1.2/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `readfcs-1.1.1/README.md` & `readfcs-1.1.2/README.md`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-[![Stars](https://img.shields.io/github/stars/laminlabs/readfcs?logo=GitHub&color=yellow)](https://github.com/laminlabs/readfcs)
-[![codecov](https://codecov.io/gh/laminlabs/readfcs/branch/main/graph/badge.svg?token=6A5PYRX809)](https://codecov.io/gh/laminlabs/readfcs)
-[![pypi](https://img.shields.io/pypi/v/readfcs?color=blue&label=pypi%20package)](https://pypi.org/project/readfcs)
-[![doi](https://img.shields.io/badge/doi-10.56528%2Frfcs-lightgrey)](https://doi.org/10.56528/rfcs)
-
-# readfcs: Read FCS files
-
-_A lightweight open-source Python package that loads data and metadata from Flow Cytometry Standard (FCS) files into DataFrame and AnnData objects._
-
-Read the [docs](https://lamin.ai/docs/readfcs), [report](https://lamin.ai/reports/2022/readfcs).
+[![Stars](https://img.shields.io/github/stars/laminlabs/readfcs?logo=GitHub&color=yellow)](https://github.com/laminlabs/readfcs)
+[![codecov](https://codecov.io/gh/laminlabs/readfcs/branch/main/graph/badge.svg?token=6A5PYRX809)](https://codecov.io/gh/laminlabs/readfcs)
+[![pypi](https://img.shields.io/pypi/v/readfcs?color=blue&label=pypi%20package)](https://pypi.org/project/readfcs)
+[![doi](https://img.shields.io/badge/doi-10.56528%2Frfcs-lightgrey)](https://doi.org/10.56528/rfcs)
+
+# readfcs: Read FCS files
+
+_A lightweight open-source Python package that loads data and metadata from Flow Cytometry Standard (FCS) files into DataFrame and AnnData objects._
+
+Read the [docs](https://lamin.ai/docs/readfcs), [report](https://lamin.ai/reports/2022/readfcs).
```

### Comparing `readfcs-1.1.1/docs/changelog.md` & `readfcs-1.1.2/docs/changelog.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+➖ Remove nbproject from dependencies | [25](https://github.com/laminlabs/readfcs/pull/25) | [Koncopd](https://github.com/Koncopd) | 2023-06-04 | 1.1.2
+💚 Fix docs | [23](https://github.com/laminlabs/readfcs/pull/23) | [sunnyosun](https://github.com/sunnyosun) | 2023-02-07 |
 🩹 Fill nan with empty string in channels | [22](https://github.com/laminlabs/readfcs/pull/22) | [sunnyosun](https://github.com/sunnyosun) | 2023-02-07 | 1.1.1
 🚑 Wrote new channels formater | [21](https://github.com/laminlabs/readfcs/pull/21) | [sunnyosun](https://github.com/sunnyosun) | 2023-01-20 | 1.1.0
 👷 Extend CI to py3.8-3.10 | [20](https://github.com/laminlabs/readfcs/pull/20) | [sunnyosun](https://github.com/sunnyosun) | 2023-01-12 | 1.0.4
 🩹 Convert list columns to str so it saves properly | [19](https://github.com/laminlabs/readfcs/pull/19) | [sunnyosun](https://github.com/sunnyosun) | 2022-09-08 | 1.0.3
 🩹 Make sure `anndata` index is str | [18](https://github.com/laminlabs/readfcs/pull/18) | [sunnyosun](https://github.com/sunnyosun) | 2022-09-06 | 1.0.2
 🐛 Change `_channel_names_` to list for saving error | [17](https://github.com/laminlabs/readfcs/pull/17) | [sunnyosun](https://github.com/sunnyosun) | 2022-08-30 | 1.0.1
 🎨 Get coverage to 100% | [16](https://github.com/laminlabs/readfcs/pull/16) | [sunnyosun](https://github.com/sunnyosun) | 2022-08-22 | 1.0.0
```

### Comparing `readfcs-1.1.1/noxfile.py` & `readfcs-1.1.2/noxfile.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-from pathlib import Path
-
-import nox
-
-nox.options.reuse_existing_virtualenvs = True
-
-
-@nox.session(python=["3.7", "3.8", "3.9", "3.10", "3.11"])
-def lint(session: nox.Session) -> None:
-    session.install("pre-commit")
-    session.run("pre-commit", "install")
-    session.run("pre-commit", "run", "--all-files")
-
-
-@nox.session(python=["3.7", "3.8", "3.9", "3.10", "3.11"])
-def build(session):
-    session.install(".[dev,test]")
-    session.run(
-        "pytest",
-        "-s",
-        "--cov=readfcs",
-        "--cov-append",
-        "--cov-report=term-missing",
-    )
-    session.run("coverage", "xml")
-    prefix = "." if Path("./lndocs").exists() else ".."
-    session.install(f"{prefix}/lndocs")
-    session.run("lndocs")
+from pathlib import Path
+
+import nox
+
+nox.options.reuse_existing_virtualenvs = True
+
+
+@nox.session(python=["3.7", "3.8", "3.9", "3.10", "3.11"])
+def lint(session: nox.Session) -> None:
+    session.install("pre-commit")
+    session.run("pre-commit", "install")
+    session.run("pre-commit", "run", "--all-files")
+
+
+@nox.session(python=["3.7", "3.8", "3.9", "3.10", "3.11"])
+def build(session):
+    session.install(".[dev,test]")
+    session.run(
+        "pytest",
+        "-s",
+        "--cov=readfcs",
+        "--cov-append",
+        "--cov-report=term-missing",
+    )
+    session.run("coverage", "xml")
+    prefix = "." if Path("./lndocs").exists() else ".."
+    session.install(f"{prefix}/lndocs")
+    session.run("lndocs")
```

### Comparing `readfcs-1.1.1/readfcs/_core.py` & `readfcs-1.1.2/readfcs/_core.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,257 +1,257 @@
-import re
-from pathlib import Path
-from typing import Dict, Union
-
-import anndata as ad
-import fcsparser
-import numpy as np
-import pandas as pd
-
-
-def _channels_to_df(meta_raw: dict) -> dict:
-    """Format channels into a DataFrame.
-
-    Args:
-    meta_raw: dict
-        original metadata
-
-    Returns:
-        a dict of metadata with "channels"
-    """
-    meta = {}
-    channel_groups: Dict = {}
-
-    # channel groups are $PnB, $PnS, $PnN...
-    for k, v in meta_raw.items():
-        # Get all fields with $PnX pattern
-        if re.match("^\$P\d+[A-Z]$", k):  # noqa
-            group_key = f"$Pn{k[-1]}"
-            if group_key not in channel_groups:
-                channel_groups[group_key] = []
-            # The numeric index n
-            idx = int(k.lstrip("$P")[:-1])
-            channel_groups[group_key].append((idx, v))
-        else:
-            meta[k] = v
-
-    # format channels into a dataframe
-    k = "$PnN"
-    df_groups = pd.DataFrame(channel_groups.get(k), columns=["n", k]).set_index("n")
-
-    for k, group in channel_groups.items():
-        if k == "$PnN":
-            continue
-        df_group = pd.DataFrame(channel_groups.get(k), columns=["n", k]).set_index("n")
-        df_groups = df_groups.join(df_group)
-
-    # reorder df_groups columns
-    df_groups.insert(0, "$PnN", df_groups.pop("$PnN"))
-    if "$PnS" in df_groups.columns:
-        df_groups.insert(1, "$PnS", df_groups.pop("$PnS"))
-    # convert nan to '' otherwise saving to anndata will error
-    df_groups.fillna("", inplace=True)
-    meta["channels"] = df_groups
-
-    return meta
-
-
-def _get_spill_matrix(matrix_string: str) -> pd.DataFrame:
-    """Generate a spill matrix for string.
-
-    Code is modified from: https://github.com/whitews/FlowUtils
-    Pedersen NW, Chandran PA, Qian Y, et al. Automated Analysis of Flow Cytometry
-    Data to Reduce Inter-Lab Variation in the Detection of Major Histocompatibility
-    Complex Multimer-Binding T Cells. Front Immunol. 2017;8:858.
-    Published 2017 Jul 26. doi:10.3389/fimmu.2017.00858
-
-    Args:
-    matrix_string: str
-        string value extracted from the 'spill' parameter of the FCS file
-
-    Returns:
-        Pandas.DataFrame
-    """
-    matrix_list = matrix_string.split(",")
-    n = int(matrix_list[0])
-    header = matrix_list[1 : (n + 1)]
-    header = [i.strip().replace("\n", "") for i in header]
-    values = [i.strip().replace("\n", "") for i in matrix_list[n + 1 :]]
-    matrix = np.reshape(list(map(float, values)), (n, n))
-    matrix_df = pd.DataFrame(matrix)
-    matrix_df = matrix_df.rename(
-        index={k: v for k, v in zip(matrix_df.columns.to_list(), header)},
-        columns={k: v for k, v in zip(matrix_df.columns.to_list(), header)},
-    )
-    return matrix_df
-
-
-class ReadFCS:
-    """Read in fcs file using fcsparesr as preprocess the metadata.
-
-    Args:
-        filepath: str or Path
-            location of fcs file to parse
-        data_set: int
-            Index of retrieved data set in the fcs file.
-    """
-
-    def __init__(self, filepath: Union[str, Path], data_set: int = 0) -> None:
-        # No metadata formating using fcsparser
-        self._meta_raw, self._data = fcsparser.parse(
-            filepath, data_set=data_set, channel_naming="$PnN"
-        )
-
-        # Format channels into a dataframe as `self.meta["channels"]`
-        self._meta = _channels_to_df(self._meta_raw)
-
-        # header
-        self._meta["header"] = self.meta["__header__"]
-        self._meta["header"]["FCS format"] = self.meta["__header__"][
-            "FCS format"
-        ].decode()
-
-        # compensation matrix
-        self.spill_txt = None
-        self.spill = None
-        if "SPILL" in self.meta:
-            self._meta["spill"] = self._meta.pop("SPILL")
-        if "SPILLOVER" in self.meta:
-            self._meta["spillover"] = self._meta.pop("SPILLOVER")
-
-        spill_list = [
-            self.meta.get(key)
-            for key in ["spill", "spillover"]
-            if self.meta.get(key) is not None
-        ]
-        if len(spill_list) > 0:
-            self.spill_txt = spill_list[0]
-            if len(self.spill_txt) > 0:  # type:ignore
-                self._meta["spill"] = _get_spill_matrix(self.spill_txt)  # type:ignore
-
-    @property
-    def header(self) -> dict:
-        """Header."""
-        return self._meta["header"]
-
-    @property
-    def meta(self) -> dict:
-        """Metadata."""
-        return self._meta
-
-    @property
-    def data(self) -> pd.DataFrame:
-        """Data matrix."""
-        return self._data
-
-    def compensate(self) -> None:
-        """Apply compensation to event data."""
-        assert (
-            self.meta["spill"] is not None
-        ), f"Unable to locate spillover matrix, please provide a compensation matrix"  # noqa
-        channel_idx = [
-            i
-            for i, (idx, row) in enumerate(self._meta["channels"].iterrows())
-            if row["$PnS"] not in ["", " "]
-        ]
-
-        channel_idx = [
-            i
-            for i, (idx, row) in enumerate(self._meta["channels"].iterrows())
-            if all([z not in row["$PnN"].lower() for z in ["fsc", "ssc", "time"]])
-            and row["$PnN"] in self.meta["spill"].columns  # noqa
-        ]
-
-        comp_data = self.data.iloc[:, channel_idx]
-        comp_data = np.linalg.solve(self.meta["spill"].values.T, comp_data.T).T
-        self._data[self._data.columns[channel_idx]] = comp_data
-
-    def to_anndata(self, reindex=True) -> ad.AnnData:
-        """Convert the FCSFile instance to an AnnData.
-
-        Args:
-            reindex: variables will be reindexed with marker names if possible otherwise
-                channels
-        Returns:
-            an AnnData object
-        """
-        channels_mapping = {
-            "$PnN": "channel",
-            "$PnS": "marker",
-        }
-        if any([i for i in ["$PnN", "$PnS"] if i not in self.meta["channels"].columns]):
-            raise AssertionError(
-                "$PnN or $PnS field not found in the file!\nPlease check your file"
-                " content with `readfcs.view`!"
-            )
-
-        # AnnData only allows str index
-        var = self._meta["channels"]
-        X = self._data
-        var.index = var.index.astype(str)
-        X.columns = var.index
-        X.index = X.index.astype(str)
-
-        # convert list columns to str so it saves properly
-        for k in var.columns:
-            if isinstance(var[k].iloc[0], list):
-                var[k] = var[k].map(repr)
-
-        # create anndata with channel indexing variables
-        adata = ad.AnnData(
-            X,
-            var=var.rename(columns=channels_mapping),
-        )
-
-        # by default, we index variables with marker
-        # use channels for non-marker channels
-        if reindex:
-            adata.var = adata.var.reset_index()
-            adata.var.index = np.where(
-                adata.var["marker"].isin(["", " "]),
-                adata.var["channel"],
-                adata.var["marker"],
-            )
-            mapper = pd.Series(adata.var.index, index=adata.var["channel"])
-            if self.meta.get("spill") is not None:
-                self._meta["spill"].index = self.meta["spill"].index.map(mapper)
-                self._meta["spill"].columns = self.meta["spill"].columns.map(mapper)
-
-        # write metadata into adata.uns
-        adata.uns["meta"] = self.meta
-        return adata
-
-
-def read(filepath, reindex=True) -> ad.AnnData:
-    """Read in fcs file as AnnData.
-
-    Args:
-        filepath: str or Path
-            location of fcs file to parse
-        reindex: bool
-            variables will be reindexed with marker names if possible otherwise
-            channels
-    Returns:
-        an AnnData object
-    """
-    fcsfile = ReadFCS(filepath)
-    return fcsfile.to_anndata(reindex=reindex)
-
-
-def view(filepath: Union[str, Path], data_set: int = 0):
-    """Read in file content without preprocessing for debugging.
-
-    Args:
-        filepath: str or Path
-            location of fcs file to parse
-        data_set: int
-            Index of retrieved data set in the fcs file.
-
-    Returns:
-        a tuple of (data, metadata)
-        - data is a DataFrame
-        - metadata is a dictionary
-
-    See `fcsparser.parse`: https://github.com/eyurtsev/fcsparser
-    """
-    meta, data = fcsparser.parse(filepath, data_set=data_set, channel_naming="$PnN")
-    return meta, data
+import re
+from pathlib import Path
+from typing import Dict, Union
+
+import anndata as ad
+import fcsparser
+import numpy as np
+import pandas as pd
+
+
+def _channels_to_df(meta_raw: dict) -> dict:
+    """Format channels into a DataFrame.
+
+    Args:
+    meta_raw: dict
+        original metadata
+
+    Returns:
+        a dict of metadata with "channels"
+    """
+    meta = {}
+    channel_groups: Dict = {}
+
+    # channel groups are $PnB, $PnS, $PnN...
+    for k, v in meta_raw.items():
+        # Get all fields with $PnX pattern
+        if re.match("^\$P\d+[A-Z]$", k):  # noqa
+            group_key = f"$Pn{k[-1]}"
+            if group_key not in channel_groups:
+                channel_groups[group_key] = []
+            # The numeric index n
+            idx = int(k.lstrip("$P")[:-1])
+            channel_groups[group_key].append((idx, v))
+        else:
+            meta[k] = v
+
+    # format channels into a dataframe
+    k = "$PnN"
+    df_groups = pd.DataFrame(channel_groups.get(k), columns=["n", k]).set_index("n")
+
+    for k, group in channel_groups.items():
+        if k == "$PnN":
+            continue
+        df_group = pd.DataFrame(channel_groups.get(k), columns=["n", k]).set_index("n")
+        df_groups = df_groups.join(df_group)
+
+    # reorder df_groups columns
+    df_groups.insert(0, "$PnN", df_groups.pop("$PnN"))
+    if "$PnS" in df_groups.columns:
+        df_groups.insert(1, "$PnS", df_groups.pop("$PnS"))
+    # convert nan to '' otherwise saving to anndata will error
+    df_groups.fillna("", inplace=True)
+    meta["channels"] = df_groups
+
+    return meta
+
+
+def _get_spill_matrix(matrix_string: str) -> pd.DataFrame:
+    """Generate a spill matrix for string.
+
+    Code is modified from: https://github.com/whitews/FlowUtils
+    Pedersen NW, Chandran PA, Qian Y, et al. Automated Analysis of Flow Cytometry
+    Data to Reduce Inter-Lab Variation in the Detection of Major Histocompatibility
+    Complex Multimer-Binding T Cells. Front Immunol. 2017;8:858.
+    Published 2017 Jul 26. doi:10.3389/fimmu.2017.00858
+
+    Args:
+    matrix_string: str
+        string value extracted from the 'spill' parameter of the FCS file
+
+    Returns:
+        Pandas.DataFrame
+    """
+    matrix_list = matrix_string.split(",")
+    n = int(matrix_list[0])
+    header = matrix_list[1 : (n + 1)]
+    header = [i.strip().replace("\n", "") for i in header]
+    values = [i.strip().replace("\n", "") for i in matrix_list[n + 1 :]]
+    matrix = np.reshape(list(map(float, values)), (n, n))
+    matrix_df = pd.DataFrame(matrix)
+    matrix_df = matrix_df.rename(
+        index={k: v for k, v in zip(matrix_df.columns.to_list(), header)},
+        columns={k: v for k, v in zip(matrix_df.columns.to_list(), header)},
+    )
+    return matrix_df
+
+
+class ReadFCS:
+    """Read in fcs file using fcsparesr as preprocess the metadata.
+
+    Args:
+        filepath: str or Path
+            location of fcs file to parse
+        data_set: int
+            Index of retrieved data set in the fcs file.
+    """
+
+    def __init__(self, filepath: Union[str, Path], data_set: int = 0) -> None:
+        # No metadata formating using fcsparser
+        self._meta_raw, self._data = fcsparser.parse(
+            filepath, data_set=data_set, channel_naming="$PnN"
+        )
+
+        # Format channels into a dataframe as `self.meta["channels"]`
+        self._meta = _channels_to_df(self._meta_raw)
+
+        # header
+        self._meta["header"] = self.meta["__header__"]
+        self._meta["header"]["FCS format"] = self.meta["__header__"][
+            "FCS format"
+        ].decode()
+
+        # compensation matrix
+        self.spill_txt = None
+        self.spill = None
+        if "SPILL" in self.meta:
+            self._meta["spill"] = self._meta.pop("SPILL")
+        if "SPILLOVER" in self.meta:
+            self._meta["spillover"] = self._meta.pop("SPILLOVER")
+
+        spill_list = [
+            self.meta.get(key)
+            for key in ["spill", "spillover"]
+            if self.meta.get(key) is not None
+        ]
+        if len(spill_list) > 0:
+            self.spill_txt = spill_list[0]
+            if len(self.spill_txt) > 0:  # type:ignore
+                self._meta["spill"] = _get_spill_matrix(self.spill_txt)  # type:ignore
+
+    @property
+    def header(self) -> dict:
+        """Header."""
+        return self._meta["header"]
+
+    @property
+    def meta(self) -> dict:
+        """Metadata."""
+        return self._meta
+
+    @property
+    def data(self) -> pd.DataFrame:
+        """Data matrix."""
+        return self._data
+
+    def compensate(self) -> None:
+        """Apply compensation to event data."""
+        assert (
+            self.meta["spill"] is not None
+        ), f"Unable to locate spillover matrix, please provide a compensation matrix"  # noqa
+        channel_idx = [
+            i
+            for i, (idx, row) in enumerate(self._meta["channels"].iterrows())
+            if row["$PnS"] not in ["", " "]
+        ]
+
+        channel_idx = [
+            i
+            for i, (idx, row) in enumerate(self._meta["channels"].iterrows())
+            if all([z not in row["$PnN"].lower() for z in ["fsc", "ssc", "time"]])
+            and row["$PnN"] in self.meta["spill"].columns  # noqa
+        ]
+
+        comp_data = self.data.iloc[:, channel_idx]
+        comp_data = np.linalg.solve(self.meta["spill"].values.T, comp_data.T).T
+        self._data[self._data.columns[channel_idx]] = comp_data
+
+    def to_anndata(self, reindex=True) -> ad.AnnData:
+        """Convert the FCSFile instance to an AnnData.
+
+        Args:
+            reindex: variables will be reindexed with marker names if possible otherwise
+                channels
+        Returns:
+            an AnnData object
+        """
+        channels_mapping = {
+            "$PnN": "channel",
+            "$PnS": "marker",
+        }
+        if any([i for i in ["$PnN", "$PnS"] if i not in self.meta["channels"].columns]):
+            raise AssertionError(
+                "$PnN or $PnS field not found in the file!\nPlease check your file"
+                " content with `readfcs.view`!"
+            )
+
+        # AnnData only allows str index
+        var = self._meta["channels"]
+        X = self._data
+        var.index = var.index.astype(str)
+        X.columns = var.index
+        X.index = X.index.astype(str)
+
+        # convert list columns to str so it saves properly
+        for k in var.columns:
+            if isinstance(var[k].iloc[0], list):
+                var[k] = var[k].map(repr)
+
+        # create anndata with channel indexing variables
+        adata = ad.AnnData(
+            X,
+            var=var.rename(columns=channels_mapping),
+        )
+
+        # by default, we index variables with marker
+        # use channels for non-marker channels
+        if reindex:
+            adata.var = adata.var.reset_index()
+            adata.var.index = np.where(
+                adata.var["marker"].isin(["", " "]),
+                adata.var["channel"],
+                adata.var["marker"],
+            )
+            mapper = pd.Series(adata.var.index, index=adata.var["channel"])
+            if self.meta.get("spill") is not None:
+                self._meta["spill"].index = self.meta["spill"].index.map(mapper)
+                self._meta["spill"].columns = self.meta["spill"].columns.map(mapper)
+
+        # write metadata into adata.uns
+        adata.uns["meta"] = self.meta
+        return adata
+
+
+def read(filepath, reindex=True) -> ad.AnnData:
+    """Read in fcs file as AnnData.
+
+    Args:
+        filepath: str or Path
+            location of fcs file to parse
+        reindex: bool
+            variables will be reindexed with marker names if possible otherwise
+            channels
+    Returns:
+        an AnnData object
+    """
+    fcsfile = ReadFCS(filepath)
+    return fcsfile.to_anndata(reindex=reindex)
+
+
+def view(filepath: Union[str, Path], data_set: int = 0):
+    """Read in file content without preprocessing for debugging.
+
+    Args:
+        filepath: str or Path
+            location of fcs file to parse
+        data_set: int
+            Index of retrieved data set in the fcs file.
+
+    Returns:
+        a tuple of (data, metadata)
+        - data is a DataFrame
+        - metadata is a dictionary
+
+    See `fcsparser.parse`: https://github.com/eyurtsev/fcsparser
+    """
+    meta, data = fcsparser.parse(filepath, data_set=data_set, channel_naming="$PnN")
+    return meta, data
```

### Comparing `readfcs-1.1.1/PKG-INFO` & `readfcs-1.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: readfcs
-Version: 1.1.1
+Version: 1.1.2
 Summary: Parse fcs files into AnnData.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: nbproject
 Requires-Dist: lamin_logger
 Requires-Dist: fcsparser
 Requires-Dist: anndata
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: nox ; extra == "dev"
 Requires-Dist: pytest>=6.0 ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Requires-Dist: nbmake ; extra == "test"
+Requires-Dist: nbproject-test ; extra == "test"
 Project-URL: Home, https://github.com/laminlabs/readfcs
 Provides-Extra: dev
 Provides-Extra: test
 
 [![Stars](https://img.shields.io/github/stars/laminlabs/readfcs?logo=GitHub&color=yellow)](https://github.com/laminlabs/readfcs)
 [![codecov](https://codecov.io/gh/laminlabs/readfcs/branch/main/graph/badge.svg?token=6A5PYRX809)](https://codecov.io/gh/laminlabs/readfcs)
 [![pypi](https://img.shields.io/pypi/v/readfcs?color=blue&label=pypi%20package)](https://pypi.org/project/readfcs)
```

