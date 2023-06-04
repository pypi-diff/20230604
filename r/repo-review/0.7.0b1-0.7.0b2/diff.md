# Comparing `tmp/repo_review-0.7.0b1.tar.gz` & `tmp/repo_review-0.7.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, last modified: Sun Jun  4 00:22:47 2023, max compression
```

## Comparing `repo_review-0.7.0b1.tar` & `repo_review-0.7.0b2.tar`

### file list

```diff
@@ -1,54 +1,36 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 repo_review-0.7.0b1/.DS_Store
--rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 repo_review-0.7.0b1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 repo_review-0.7.0b1/noxfile.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 repo_review-0.7.0b1/tmp.html
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 repo_review-0.7.0b1/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 repo_review-0.7.0b1/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 repo_review-0.7.0b1/.github/dependabot.yml
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 repo_review-0.7.0b1/.github/matchers/pylint.json
--rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 repo_review-0.7.0b1/.github/workflows/ci.yml
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 repo_review-0.7.0b1/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 repo_review-0.7.0b1/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repo_review-0.7.0b1/docs/.nojekyll
--rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 repo_review-0.7.0b1/docs/index.html
--rw-r--r--   0        0        0     9739 2020-02-02 00:00:00.000000 repo_review-0.7.0b1/docs/webapp.js
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 repo_review-0.7.0b1/src/repo_review/__init__.py
--rw-r--r--   0        0        0     5170 2020-02-02 00:00:00.000000 repo_review-0.7.0b1/src/repo_review/__main__.py
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 repo_review-0.7.0b1/src/repo_review/checks.py
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 repo_review-0.7.0b1/src/repo_review/families.py
--rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 repo_review-0.7.0b1/src/repo_review/fixtures.py
--rw-r--r--   0        0        0     3412 2020-02-02 00:00:00.000000 repo_review-0.7.0b1/src/repo_review/ghpath.py
--rw-r--r--   0        0        0     3553 2020-02-02 00:00:00.000000 repo_review-0.7.0b1/src/repo_review/processor.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repo_review-0.7.0b1/src/repo_review/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repo_review-0.7.0b1/src/repo_review/_compat/__init__.py
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 repo_review-0.7.0b1/src/repo_review/_compat/tomllib.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repo_review-0.7.0b1/src/repo_review/_compat/importlib/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repo_review-0.7.0b1/src/repo_review/_compat/importlib/resources/__init__.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 repo_review-0.7.0b1/src/repo_review/_compat/importlib/resources/abc.py
--rw-r--r--   0        0        0     2680 2020-02-02 00:00:00.000000 repo_review-0.7.0b1/tests/test_checks.py
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 repo_review-0.7.0b1/tests/test_cmd.py
--rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 repo_review-0.7.0b1/tests/test_fixtures.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 repo_review-0.7.0b1/tests/test_package.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 repo_review-0.7.0b1/web-app/.gitignore
--rw-r--r--   0        0        0     3359 2020-02-02 00:00:00.000000 repo_review-0.7.0b1/web-app/README.md
--rw-r--r--   0        0        0  1139571 2020-02-02 00:00:00.000000 repo_review-0.7.0b1/web-app/package-lock.json
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 repo_review-0.7.0b1/web-app/package.json
--rw-r--r--   0        0        0     3870 2020-02-02 00:00:00.000000 repo_review-0.7.0b1/web-app/public/favicon.ico
--rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 repo_review-0.7.0b1/web-app/public/index.html
--rw-r--r--   0        0        0     5347 2020-02-02 00:00:00.000000 repo_review-0.7.0b1/web-app/public/logo192.png
--rw-r--r--   0        0        0     9664 2020-02-02 00:00:00.000000 repo_review-0.7.0b1/web-app/public/logo512.png
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 repo_review-0.7.0b1/web-app/public/manifest.json
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 repo_review-0.7.0b1/web-app/public/robots.txt
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 repo_review-0.7.0b1/web-app/src/App.css
--rw-r--r--   0        0        0     5185 2020-02-02 00:00:00.000000 repo_review-0.7.0b1/web-app/src/App.js
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 repo_review-0.7.0b1/web-app/src/App.test.js
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 repo_review-0.7.0b1/web-app/src/index.css
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 repo_review-0.7.0b1/web-app/src/index.js
--rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 repo_review-0.7.0b1/web-app/src/logo.svg
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 repo_review-0.7.0b1/web-app/src/reportWebVitals.js
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 repo_review-0.7.0b1/web-app/src/setupTests.js
--rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 repo_review-0.7.0b1/.gitignore
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 repo_review-0.7.0b1/LICENSE
--rw-r--r--   0        0        0     3758 2020-02-02 00:00:00.000000 repo_review-0.7.0b1/README.md
--rw-r--r--   0        0        0     4290 2020-02-02 00:00:00.000000 repo_review-0.7.0b1/pyproject.toml
--rw-r--r--   0        0        0     6779 2020-02-02 00:00:00.000000 repo_review-0.7.0b1/PKG-INFO
+-rw-r--r--   0        0        0     2061 2023-06-04 00:22:47.000000 repo_review-0.7.0b2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1591 2023-06-04 00:22:47.000000 repo_review-0.7.0b2/noxfile.py
+-rw-r--r--   0        0        0      359 2023-06-04 00:22:47.000000 repo_review-0.7.0b2/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0     2324 2023-06-04 00:22:47.000000 repo_review-0.7.0b2/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      162 2023-06-04 00:22:47.000000 repo_review-0.7.0b2/.github/dependabot.yml
+-rw-r--r--   0        0        0      668 2023-06-04 00:22:47.000000 repo_review-0.7.0b2/.github/matchers/pylint.json
+-rw-r--r--   0        0        0      630 2023-06-04 00:22:47.000000 repo_review-0.7.0b2/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     1501 2023-06-04 00:22:47.000000 repo_review-0.7.0b2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0        0 2023-06-04 00:22:47.000000 repo_review-0.7.0b2/docs/.nojekyll
+-rw-r--r--   0        0        0     1778 2023-06-04 00:22:47.000000 repo_review-0.7.0b2/docs/index.html
+-rw-r--r--   0        0        0     9739 2023-06-04 00:22:47.000000 repo_review-0.7.0b2/docs/webapp.js
+-rw-r--r--   0        0        0      222 2023-06-04 00:22:47.000000 repo_review-0.7.0b2/src/repo_review/__init__.py
+-rw-r--r--   0        0        0     5329 2023-06-04 00:22:47.000000 repo_review-0.7.0b2/src/repo_review/__main__.py
+-rw-r--r--   0        0        0     1021 2023-06-04 00:22:47.000000 repo_review-0.7.0b2/src/repo_review/checks.py
+-rw-r--r--   0        0        0     1014 2023-06-04 00:22:47.000000 repo_review-0.7.0b2/src/repo_review/families.py
+-rw-r--r--   0        0        0     2004 2023-06-04 00:22:47.000000 repo_review-0.7.0b2/src/repo_review/fixtures.py
+-rw-r--r--   0        0        0     3412 2023-06-04 00:22:47.000000 repo_review-0.7.0b2/src/repo_review/ghpath.py
+-rw-r--r--   0        0        0     4241 2023-06-04 00:22:47.000000 repo_review-0.7.0b2/src/repo_review/processor.py
+-rw-r--r--   0        0        0        0 2023-06-04 00:22:47.000000 repo_review-0.7.0b2/src/repo_review/py.typed
+-rw-r--r--   0        0        0        0 2023-06-04 00:22:47.000000 repo_review-0.7.0b2/src/repo_review/_compat/__init__.py
+-rw-r--r--   0        0        0      233 2023-06-04 00:22:47.000000 repo_review-0.7.0b2/src/repo_review/_compat/tomllib.py
+-rw-r--r--   0        0        0        0 2023-06-04 00:22:47.000000 repo_review-0.7.0b2/src/repo_review/_compat/importlib/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-04 00:22:47.000000 repo_review-0.7.0b2/src/repo_review/_compat/importlib/resources/__init__.py
+-rw-r--r--   0        0        0      256 2023-06-04 00:22:47.000000 repo_review-0.7.0b2/src/repo_review/_compat/importlib/resources/abc.py
+-rw-r--r--   0        0        0     3734 2023-06-04 00:22:47.000000 repo_review-0.7.0b2/tests/test_checks.py
+-rw-r--r--   0        0        0      450 2023-06-04 00:22:47.000000 repo_review-0.7.0b2/tests/test_cmd.py
+-rw-r--r--   0        0        0     2460 2023-06-04 00:22:47.000000 repo_review-0.7.0b2/tests/test_fixtures.py
+-rw-r--r--   0        0        0      598 2023-06-04 00:22:47.000000 repo_review-0.7.0b2/tests/test_package.py
+-rw-r--r--   0        0        0     1921 2023-06-04 00:22:47.000000 repo_review-0.7.0b2/tests/test_self.py
+-rw-r--r--   0        0        0     3886 2023-06-04 00:22:47.000000 repo_review-0.7.0b2/tests/test_utilities/pyproject.py
+-rw-r--r--   0        0        0       15 2023-06-04 00:22:47.000000 repo_review-0.7.0b2/tests/test_utilities/pyproject.toml
+-rw-r--r--   0        0        0     2086 2023-06-04 00:22:47.000000 repo_review-0.7.0b2/.gitignore
+-rw-r--r--   0        0        0     1525 2023-06-04 00:22:47.000000 repo_review-0.7.0b2/LICENSE
+-rw-r--r--   0        0        0     3758 2023-06-04 00:22:47.000000 repo_review-0.7.0b2/README.md
+-rw-r--r--   0        0        0     4314 2023-06-04 00:22:47.000000 repo_review-0.7.0b2/pyproject.toml
+-rw-r--r--   0        0        0     6779 2023-06-04 00:22:47.000000 repo_review-0.7.0b2/PKG-INFO
```

### Comparing `repo_review-0.7.0b1/.pre-commit-config.yaml` & `repo_review-0.7.0b2/.pre-commit-config.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -33,16 +33,14 @@
       - id: check-case-conflict
       - id: check-merge-conflict
       - id: check-symlinks
       - id: check-yaml
       - id: debug-statements
       - id: end-of-file-fixer
       - id: mixed-line-ending
-      - id: name-tests-test
-        args: ["--pytest-test-first"]
       - id: requirements-txt-fixer
       - id: trailing-whitespace
 
   - repo: https://github.com/pre-commit/pygrep-hooks
     rev: v1.10.0
     hooks:
       - id: rst-backticks
```

### Comparing `repo_review-0.7.0b1/noxfile.py` & `repo_review-0.7.0b2/noxfile.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 nox.options.sessions = ["lint", "pylint", "tests"]
 
 
 @nox.session(reuse_venv=True)
 def run(session: nox.Session) -> None:
     """
-    Run the program
+    Run the program.
     """
 
     session.install("-e", ".[cli]")
     session.run("python", "-m", "repo_review", *session.posargs)
 
 
 @nox.session
```

### Comparing `repo_review-0.7.0b1/.github/CONTRIBUTING.md` & `repo_review-0.7.0b2/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b1/.github/matchers/pylint.json` & `repo_review-0.7.0b2/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b1/.github/workflows/ci.yml` & `repo_review-0.7.0b2/.github/workflows/ci.yml`

 * *Files 8% similar despite different names*

```diff
@@ -55,41 +55,12 @@
         run: python -m pytest -ra
         env:
           PYTHONUTF8: "1"
 
   dist:
     name: Distribution build
     runs-on: ubuntu-latest
-    needs: [pre-commit]
 
     steps:
       - uses: actions/checkout@v3
 
-      - uses: actions/setup-python@v4
-        with:
-          python-version: "3.x"
-
-      - name: Build sdist and wheel
-        run: pipx run build
-
-      - uses: actions/upload-artifact@v3
-        with:
-          path: dist
-
-      - name: Check products
-        run: pipx run twine check dist/*
-
-  publish:
-    name: Publish
-    needs: [dist]
-    environment: pypi
-    permissions:
-      id-token: write
-    runs-on: ubuntu-latest
-    if: github.event_name == 'release' && github.event.action == 'published'
-    steps:
-      - uses: actions/download-artifact@v3
-        with:
-          name: artifact
-          path: dist
-
-      - uses: pypa/gh-action-pypi-publish@release/v1
+      - uses: hynek/build-and-inspect-python-package@v1
```

### Comparing `repo_review-0.7.0b1/docs/index.html` & `repo_review-0.7.0b2/docs/index.html`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b1/docs/webapp.js` & `repo_review-0.7.0b2/docs/webapp.js`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b1/src/repo_review/__main__.py` & `repo_review-0.7.0b2/src/repo_review/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -110,34 +110,41 @@
     help="Select output format.",
 )
 @click.option(
     "--ignore",
     help="Ignore a check or checks, comma separated.",
     default="",
 )
+@click.option(
+    "--package-dir",
+    "-p",
+    help="Python package subdirectory",
+    default="",
+)
 def main(
     package: Path,
     output: Path | None,
     format: Literal["rich", "json", "html"],
     ignore: str,
+    package_dir: str,
 ) -> None:
     """
-    Pass in a local Path or gh:org/repo@branch[:root].
+    Pass in a local Path or gh:org/repo@branch.
     """
     ignore_list = [x.strip() for x in ignore.split(",")]
 
     if str(package).startswith("gh:"):
         _, org_repo_branch, *p = str(package).split(":", maxsplit=2)
         org_repo, branch = org_repo_branch.split("@", maxsplit=1)
         ghpackage = GHPath(repo=org_repo, branch=branch, path=p[0] if p else "")
         if format == "rich":
             rich.print(f"[bold]Processing [blue]{package}[/blue] from GitHub\n")
-        families, processed = process(ghpackage, ignore=ignore_list)
+        families, processed = process(ghpackage, ignore=ignore_list, subdir=package_dir)
     else:
-        families, processed = process(package, ignore=ignore_list)
+        families, processed = process(package, ignore=ignore_list, subdir=package_dir)
 
     if format == "rich":
         rich_printer(families, processed, output=output)
     elif format == "json":
         j = json.dumps(
             {"families": families, "checks": as_simple_dict(processed)}, indent=2
         )
```

### Comparing `repo_review-0.7.0b1/src/repo_review/checks.py` & `repo_review-0.7.0b2/src/repo_review/checks.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from __future__ import annotations
 
 import importlib.metadata
 from collections.abc import Mapping, Set
-from typing import Any, ClassVar, Protocol
+from typing import Any, Protocol
 
 from .fixtures import apply_fixtures
 
 __all__ = ["Check", "collect_checks", "is_allowed"]
 
 
 class Check(Protocol):
-    family: ClassVar[str]
-    requires: ClassVar[Set[str]] = frozenset()
+    family: str
+    requires: Set[str] = frozenset()
+    url: str = ""
 
-    def check(self) -> bool | None:
+    def check(self) -> bool | None | str:
         ...
 
 
 def collect_checks(fixtures: Mapping[str, Any]) -> dict[str, Check]:
     check_functions = (
         ep.load() for ep in importlib.metadata.entry_points(group="repo_review.checks")
     )
```

### Comparing `repo_review-0.7.0b1/src/repo_review/families.py` & `repo_review-0.7.0b2/src/repo_review/families.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b1/src/repo_review/ghpath.py` & `repo_review-0.7.0b2/src/repo_review/ghpath.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b1/src/repo_review/processor.py` & `repo_review-0.7.0b2/src/repo_review/processor.py`

 * *Files 15% similar despite different names*

```diff
@@ -25,49 +25,59 @@
 
 # Helper to get the type in the JSON style returns
 class ResultDict(typing.TypedDict):
     family: str
     description: str
     result: bool | None
     err_msg: str
+    url: str
 
 
 @dataclasses.dataclass(frozen=True, kw_only=True)
 class Result:
     family: str
     name: str
     description: str
     result: bool | None
     err_msg: str = ""
+    url: str = ""
 
     def err_markdown(self) -> str:
         result: str = md.render(self.err_msg).strip()
         return result.removeprefix("<p>").removesuffix("</p>").strip()
 
 
 class ProcessReturn(typing.NamedTuple):
     families: dict[str, Family]
     results: list[Result]
 
 
-def process(package: Traversable, *, ignore: Sequence[str] = ()) -> ProcessReturn:
+def process(
+    root: Traversable, *, ignore: Sequence[str] = (), subdir: str = ""
+) -> ProcessReturn:
     """
     Process the package and return a dictionary of results.
 
     Parameters
     ----------
-    package: Traversable | Path
-        The Path(like) package to process
+    root: Traversable | Path
+        The Path(like) to the repository to process
 
     ignore: Sequence[str]
         A list of checks to ignore
+
+    subidr: str
+        The path to the package in the subdirectory, if not at the root of the repository.
     """
+
+    package = root.joinpath(subdir) if subdir else root
+
     # Collect the fixtures
     fixture_functions = collect_fixtures()
-    fixtures = compute_fixtures(package, fixture_functions)
+    fixtures = compute_fixtures(root, package, fixture_functions)
 
     # Collect the checks
     checks = collect_checks(fixtures)
 
     # Collect families.
     families = collect_families()
 
@@ -76,47 +86,55 @@
         if name not in families:
             families[name] = Family()
 
     # Collect our own config
     config = pyproject(package).get("tool", {}).get("repo-review", {})
     skip_checks = set(ignore) | set(config.get("ignore", ()))
 
+    # Make list of filtered checks to run
     tasks: dict[str, Check] = {
         n: r for n, r in checks.items() if is_allowed(skip_checks, n)
     }
+    # Make a graph of the check's interdependencies
     graph: dict[str, set[str]] = {
         n: getattr(t, "requires", set()) for n, t in tasks.items()
     }
-    completed: dict[str, bool | None] = {}
+    # Keep track of which checks have been completed
+    completed: dict[str, str | None] = {}
 
-    # Run all the checks in topological order
+    # Run all the checks in topological order based on their dependencies
     ts = graphlib.TopologicalSorter(graph)
     for name in ts.static_order():
-        if all(completed.get(n, False) for n in graph[name]):
-            completed[name] = apply_fixtures(fixtures, tasks[name].check)
+        if all(completed.get(n, "") == "" for n in graph[name]):  # noqa: PLC1901
+            result = apply_fixtures(fixtures, tasks[name].check)
+            if isinstance(result, bool):
+                completed[name] = "" if result else tasks[name].check.__doc__
+            else:
+                completed[name] = result
         else:
             completed[name] = None
 
     # Collect the results
     result_list = []
     for task_name, check in sorted(
         tasks.items(),
         key=lambda x: (families[x[1].family].get("order", 0), x[1].family, x[0]),
     ):
-        result = completed[task_name]
+        result = None if completed[task_name] is None else not completed[task_name]
         doc = check.__doc__ or ""
-        err_msg = check.check.__doc__ or ""
+        err_msg = completed[task_name] or ""
 
         result_list.append(
             Result(
                 family=check.family,
                 name=task_name,
                 description=doc,
                 result=result,
                 err_msg=textwrap.dedent(err_msg.format(cls=check)),
+                url=getattr(check, "url", ""),
             )
         )
 
     return ProcessReturn(families, result_list)
 
 
 def as_simple_dict(results: list[Result]) -> dict[str, ResultDict]:
```

### Comparing `repo_review-0.7.0b1/tests/test_fixtures.py` & `repo_review-0.7.0b2/tests/test_fixtures.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 from types import ModuleType
 
 import pytest
 
 from repo_review._compat.importlib.resources.abc import Traversable
 from repo_review.checks import collect_checks
-from repo_review.fixtures import apply_fixtures, compute_fixtures, package
+from repo_review.fixtures import apply_fixtures, compute_fixtures
 
 
 class D100:
     "Was passed correctly"
     family = "pyproject"
 
     @staticmethod
@@ -50,36 +50,38 @@
 
 def get_checks(some_bool: bool) -> dict[str, type]:
     return {"D100": D100, "D200": D200} if some_bool else {"D100": D100}
 
 
 def test_process_fixtures() -> None:
     fixtures = compute_fixtures(
-        Path("."), {"simple": simple, "nothing": nothing, "not_simple": not_simple}
+        Path("."),
+        Path("."),
+        {"simple": simple, "nothing": nothing, "not_simple": not_simple},
     )
 
     assert apply_fixtures(fixtures, nothing) == 42
     assert apply_fixtures(fixtures, simple) == "."
     assert apply_fixtures(fixtures, not_simple) == ". ."
 
 
 def test_process_fixtures_with_package() -> None:
     fixtures = compute_fixtures(
         Path("."),
+        Path("."),
         {
             "simple": simple,
             "nothing": nothing,
             "not_simple": not_simple,
-            "package": package,
         },
     )
 
     assert apply_fixtures(fixtures, nothing) == 42
     assert apply_fixtures(fixtures, simple) == "."
-    assert apply_fixtures(fixtures, package) == Path(".")
+    assert apply_fixtures(fixtures, lambda package: package) == Path(".")  # type: ignore[no-any-return]
     assert apply_fixtures(fixtures, not_simple) == ". ."
 
 
 @pytest.mark.parametrize("some_bool", [True, False])
 def test_process_checks(monkeypatch: pytest.MonkeyPatch, some_bool: bool) -> None:
     ep = importlib.metadata.EntryPoint(name="x", group="y", value="test_module:f")
     sys.modules["test_module"] = ModuleType("test_module")
```

### Comparing `repo_review-0.7.0b1/tests/test_package.py` & `repo_review-0.7.0b2/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b1/.gitignore` & `repo_review-0.7.0b2/.gitignore`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b1/LICENSE` & `repo_review-0.7.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b1/README.md` & `repo_review-0.7.0b2/README.md`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b1/pyproject.toml` & `repo_review-0.7.0b2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -55,30 +55,30 @@
 webpage = "https://scientific-python.github.io/repo-review"
 
 [project.scripts]
 repo-review = "repo_review.__main__:main"
 
 [project.entry-points."repo_review.fixtures"]
 pyproject = "repo_review.fixtures:pyproject"
-package = "repo_review.fixtures:package"
 
 [tool.hatch]
 version.path = "src/repo_review/__init__.py"
 
 
 [tool.pytest.ini_options]
 minversion = "7.0"
-addopts = ["-ra", "--strict-markers", "--strict-config"]
+addopts = ["-ra", "--strict-markers", "--strict-config", "--import-mode=importlib"]
 xfail_strict = true
 log_cli_level = "INFO"
 filterwarnings = [
   'error',
   'ignore:(ast.Str|Attribute s|ast.NameConstant|ast.Num) is deprecated:DeprecationWarning:_pytest',
 ]
 testpaths = ["tests"]
+pythonpath = ["tests/test_utilities"]
 
 
 [tool.mypy]
 files = ["src", "web", "tests"]
 python_version = "3.10"
 warn_unused_configs = true
 strict = true
```

### Comparing `repo_review-0.7.0b1/PKG-INFO` & `repo_review-0.7.0b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repo_review
-Version: 0.7.0b1
+Version: 0.7.0b2
 Summary: Review repos for compliance to the Scikit-HEP developer guidelines
 Project-URL: homepage, https://github.com/scientific-python/repo-review
 Project-URL: webpage, https://scientific-python.github.io/repo-review
 Author-email: Henry Schreiner <henryfs@princeton.edu>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, Henry Schreiner.
```

