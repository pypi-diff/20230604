# Comparing `tmp/metapensiero.sphinx.patchdb-4.0.dev4.tar.gz` & `tmp/metapensiero.sphinx.patchdb-4.0.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metapensiero.sphinx.patchdb-4.0.dev4.tar", last modified: Sun Apr 30 15:01:29 2023, max compression
+gzip compressed data, was "metapensiero.sphinx.patchdb-4.0.dev5.tar", last modified: Sun Jun  4 15:33:19 2023, max compression
```

## Comparing `metapensiero.sphinx.patchdb-4.0.dev4.tar` & `metapensiero.sphinx.patchdb-4.0.dev5.tar`

### file list

```diff
@@ -1,42 +1,44 @@
--rw-r--r--   0        0        0     3506 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/CHANGES.rst
--rw-r--r--   0        0        0      609 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/Makefile
--rw-r--r--   0        0        0    10656 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/OLDERCHANGES.rst
--rw-r--r--   0        0        0    30372 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/README.rst
--rw-r--r--   0        0        0     1534 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/flake.lock
--rw-r--r--   0        0        0     4144 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/flake.nix
--rw-r--r--   0        0        0     1751 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/pyproject.toml
--rw-r--r--   0        0        0      697 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/src/metapensiero/sphinx/patchdb/__init__.py
--rw-r--r--   0        0        0     7174 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/src/metapensiero/sphinx/patchdb/contexts/__init__.py
--rw-r--r--   0        0        0     3545 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/src/metapensiero/sphinx/patchdb/contexts/firebird.py
--rw-r--r--   0        0        0     4692 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/src/metapensiero/sphinx/patchdb/contexts/mysql.py
--rw-r--r--   0        0        0     4289 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/src/metapensiero/sphinx/patchdb/contexts/postgres.py
--rw-r--r--   0        0        0     1505 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/src/metapensiero/sphinx/patchdb/contexts/python.py
--rw-r--r--   0        0        0    17886 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/src/metapensiero/sphinx/patchdb/contexts/sql.py
--rw-r--r--   0        0        0     3858 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/src/metapensiero/sphinx/patchdb/contexts/sqlite.py
--rw-r--r--   0        0        0     1546 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/src/metapensiero/sphinx/patchdb/locale/__init__.py
--rw-r--r--   0        0        0    12981 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/src/metapensiero/sphinx/patchdb/locale/it/LC_MESSAGES/metapensiero-sphinx-patchdb.po
--rw-r--r--   0        0        0      285 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/src/metapensiero/sphinx/patchdb/locale/mapping.cfg
--rw-r--r--   0        0        0     8864 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/src/metapensiero/sphinx/patchdb/locale/metapensiero-sphinx-patchdb.pot
--rw-r--r--   0        0        0    13600 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/src/metapensiero/sphinx/patchdb/manager.py
--rw-r--r--   0        0        0    14938 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/src/metapensiero/sphinx/patchdb/patch.py
--rw-r--r--   0        0        0     8782 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/src/metapensiero/sphinx/patchdb/pup.py
--rw-r--r--   0        0        0    24367 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/src/metapensiero/sphinx/patchdb/script.py
--rw-r--r--   0        0        0     7257 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/src/metapensiero/sphinx/patchdb/states.py
--rw-r--r--   0        0        0     8030 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/tests/fixtures.py
--rwxr-xr-x   0        0        0     1633 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/tests/postgresql
--rw-r--r--   0        0        0     7111 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/tests/test_bad.py
--rw-r--r--   0        0        0     4424 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/tests/test_drops.py
--rw-r--r--   0        0        0     1182 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/tests/test_external_file.py
--rw-r--r--   0        0        0     4182 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/tests/test_helpers.py
--rw-r--r--   0        0        0     4577 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/tests/test_manager.py
--rw-r--r--   0        0        0     2284 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/tests/test_modular.py
--rw-r--r--   0        0        0     3537 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/tests/test_patch.py
--rw-r--r--   0        0        0     2766 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/tests/test_python.py
--rw-r--r--   0        0        0     7007 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/tests/test_revisions.py
--rw-r--r--   0        0        0     4632 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/tests/test_sql.py
--rw-r--r--   0        0        0     2291 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/tests/test_sql_fb.py
--rw-r--r--   0        0        0     4328 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/tests/test_sql_ms.py
--rw-r--r--   0        0        0     7631 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/tests/test_sql_pg.py
--rw-r--r--   0        0        0     2835 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/tests/test_states.py
--rw-r--r--   0        0        0     2094 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/tests/test_variables.py
--rw-r--r--   0        0        0    31467 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev4/PKG-INFO
+-rw-r--r--   0        0        0     3725 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/CHANGES.rst
+-rw-r--r--   0        0        0      609 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/Makefile
+-rw-r--r--   0        0        0    10656 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/OLDERCHANGES.rst
+-rw-r--r--   0        0        0    30372 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/README.rst
+-rw-r--r--   0        0        0     2006 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/flake.lock
+-rw-r--r--   0        0        0     3373 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/flake.nix
+-rw-r--r--   0        0        0     1738 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/pyproject.toml
+-rw-r--r--   0        0        0      697 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/src/metapensiero/sphinx/patchdb/__init__.py
+-rw-r--r--   0        0        0     7496 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/src/metapensiero/sphinx/patchdb/contexts/__init__.py
+-rw-r--r--   0        0        0     3545 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/src/metapensiero/sphinx/patchdb/contexts/firebird.py
+-rw-r--r--   0        0        0     4692 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/src/metapensiero/sphinx/patchdb/contexts/mysql.py
+-rw-r--r--   0        0        0     4289 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/src/metapensiero/sphinx/patchdb/contexts/postgres.py
+-rw-r--r--   0        0        0     1505 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/src/metapensiero/sphinx/patchdb/contexts/python.py
+-rw-r--r--   0        0        0    17886 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/src/metapensiero/sphinx/patchdb/contexts/sql.py
+-rw-r--r--   0        0        0     3858 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/src/metapensiero/sphinx/patchdb/contexts/sqlite.py
+-rw-r--r--   0        0        0     1546 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/src/metapensiero/sphinx/patchdb/locale/__init__.py
+-rw-r--r--   0        0        0    13004 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/src/metapensiero/sphinx/patchdb/locale/it/LC_MESSAGES/metapensiero-sphinx-patchdb.po
+-rw-r--r--   0        0        0      285 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/src/metapensiero/sphinx/patchdb/locale/mapping.cfg
+-rw-r--r--   0        0        0     8858 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/src/metapensiero/sphinx/patchdb/locale/metapensiero-sphinx-patchdb.pot
+-rw-r--r--   0        0        0     4730 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/src/metapensiero/sphinx/patchdb/manager.py
+-rw-r--r--   0        0        0    14938 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/src/metapensiero/sphinx/patchdb/patch.py
+-rw-r--r--   0        0        0     6155 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/src/metapensiero/sphinx/patchdb/planner.py
+-rw-r--r--   0        0        0     9175 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/src/metapensiero/sphinx/patchdb/pup.py
+-rw-r--r--   0        0        0    24368 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/src/metapensiero/sphinx/patchdb/script.py
+-rw-r--r--   0        0        0     7312 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/src/metapensiero/sphinx/patchdb/states.py
+-rw-r--r--   0        0        0     8148 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/tests/fixtures.py
+-rwxr-xr-x   0        0        0     1633 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/tests/postgresql
+-rw-r--r--   0        0        0     7111 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/tests/test_bad.py
+-rw-r--r--   0        0        0     4424 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/tests/test_drops.py
+-rw-r--r--   0        0        0     1182 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/tests/test_external_file.py
+-rw-r--r--   0        0        0     3557 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/tests/test_helpers.py
+-rw-r--r--   0        0        0     1862 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/tests/test_manager.py
+-rw-r--r--   0        0        0     2284 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/tests/test_modular.py
+-rw-r--r--   0        0        0     3531 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/tests/test_patch.py
+-rw-r--r--   0        0        0     6685 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/tests/test_planner.py
+-rw-r--r--   0        0        0     2766 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/tests/test_python.py
+-rw-r--r--   0        0        0     7007 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/tests/test_revisions.py
+-rw-r--r--   0        0        0     4632 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/tests/test_sql.py
+-rw-r--r--   0        0        0     2291 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/tests/test_sql_fb.py
+-rw-r--r--   0        0        0     4328 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/tests/test_sql_ms.py
+-rw-r--r--   0        0        0     7639 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/tests/test_sql_pg.py
+-rw-r--r--   0        0        0     2835 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/tests/test_states.py
+-rw-r--r--   0        0        0     2094 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/tests/test_variables.py
+-rw-r--r--   0        0        0    31467 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev5/PKG-INFO
```

### Comparing `metapensiero.sphinx.patchdb-4.0.dev4/CHANGES.rst` & `metapensiero.sphinx.patchdb-4.0.dev5/CHANGES.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,22 @@
 Changes\ [#]_
 -------------
 
+4.0.dev5 (2023-06-04)
+~~~~~~~~~~~~~~~~~~~~~
+
+* Reimplement the logic used to determine the correct application ordering of the patches,
+  leveraging more dependencies constraints to avoid the old "postponing" strategy
+
+
 4.0.dev4 (2023-04-30)
 ~~~~~~~~~~~~~~~~~~~~~
 
 * Make ``--backups-dir`` an *opt-in* option, perform a pre-backup only when a directory is
-  specified (and different from ``None``, for backward compatibility).
+  specified (and different from ``None``, for backward compatibility)
 
 * Introduce a variant of pinned dependency, ``patchid@*``, to denote the *currently applied*
   revision of the patch or the highest available, if not already applied
 
 * Drop Python 3.9
```

### Comparing `metapensiero.sphinx.patchdb-4.0.dev4/Makefile` & `metapensiero.sphinx.patchdb-4.0.dev5/Makefile`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev4/OLDERCHANGES.rst` & `metapensiero.sphinx.patchdb-4.0.dev5/OLDERCHANGES.rst`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev4/README.rst` & `metapensiero.sphinx.patchdb-4.0.dev5/README.rst`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev4/flake.lock` & `metapensiero.sphinx.patchdb-4.0.dev5/flake.lock`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.959375%*

 * *Differences: {"'nodes'": "{'flake-utils': {'locked': {'lastModified': 1685518550, 'narHash': "*

 * *            "'sha256-o2d0KcvaXzTrPRIo0kOLV0/QXHhDQ5DTi+OxcjO8xqY=', 'rev': "*

 * *            "'a1720a10a6cfe8234c0e93907ffe81be440f4cef'}, 'inputs': OrderedDict([('systems', "*

 * *            "'systems')])}, 'nixpkgs': {'locked': {'lastModified': 1685888050, 'narHash': "*

 * *            "'sha256-bs9t6zHktV+HvmThR6ENgNllbk1L0oGQ0e1LuVSPQT4=', 'rev': "*

 * *            "'7a9b483dd8600970d49480b73d37b202da46b21f'}}, 'systems': OrderedDict([('lock […]*

```diff
@@ -1,16 +1,19 @@
 {
     "nodes": {
         "flake-utils": {
+            "inputs": {
+                "systems": "systems"
+            },
             "locked": {
-                "lastModified": 1680946745,
-                "narHash": "sha256-KqGlwg9UTDsFBZZB8wzXgMnc8XQm95LtSbFvBsnqkPI=",
+                "lastModified": 1685518550,
+                "narHash": "sha256-o2d0KcvaXzTrPRIo0kOLV0/QXHhDQ5DTi+OxcjO8xqY=",
                 "owner": "numtide",
                 "repo": "flake-utils",
-                "rev": "946da791763db1c306b86a8bd3828bf5814a1247",
+                "rev": "a1720a10a6cfe8234c0e93907ffe81be440f4cef",
                 "type": "github"
             },
             "original": {
                 "owner": "numtide",
                 "repo": "flake-utils",
                 "type": "github"
             }
@@ -33,31 +36,46 @@
                 "owner": "hercules-ci",
                 "repo": "gitignore.nix",
                 "type": "github"
             }
         },
         "nixpkgs": {
             "locked": {
-                "lastModified": 1680975136,
-                "narHash": "sha256-mVXWfWWFV/8aD+Wdsa+UPNXPjrrkfVyg4/FItBcQhPY=",
+                "lastModified": 1685888050,
+                "narHash": "sha256-bs9t6zHktV+HvmThR6ENgNllbk1L0oGQ0e1LuVSPQT4=",
                 "owner": "NixOS",
                 "repo": "nixpkgs",
-                "rev": "7f3f7ec38154b9f4eb551a67bfe4214db43d4200",
+                "rev": "7a9b483dd8600970d49480b73d37b202da46b21f",
                 "type": "github"
             },
             "original": {
                 "owner": "NixOS",
                 "repo": "nixpkgs",
                 "type": "github"
             }
         },
         "root": {
             "inputs": {
                 "flake-utils": "flake-utils",
                 "gitignore": "gitignore",
                 "nixpkgs": "nixpkgs"
             }
+        },
+        "systems": {
+            "locked": {
+                "lastModified": 1681028828,
+                "narHash": "sha256-Vy1rq5AaRuLzOxct8nz4T6wlgyUR7zLU309k9mBC768=",
+                "owner": "nix-systems",
+                "repo": "default",
+                "rev": "da67096a3b9bf56a91d16901293e51ba5b49a27e",
+                "type": "github"
+            },
+            "original": {
+                "owner": "nix-systems",
+                "repo": "default",
+                "type": "github"
+            }
         }
     },
     "root": "root",
     "version": 7
 }
```

### Comparing `metapensiero.sphinx.patchdb-4.0.dev4/flake.nix` & `metapensiero.sphinx.patchdb-4.0.dev5/flake.nix`

 * *Files 17% similar despite different names*

```diff
@@ -18,74 +18,53 @@
       inputs.nixpkgs.follows = "nixpkgs";
     };
   };
 
   outputs = { self, nixpkgs, flake-utils, gitignore }:
     flake-utils.lib.eachDefaultSystem (system:
       let
+        inherit (builtins) fromTOML readFile;
         pkgs = import nixpkgs { inherit system; };
         inherit (pkgs.lib) flip zipLists;
         inherit (gitignore.lib) gitignoreFilterWith;
 
+        pinfo = (fromTOML (readFile ./pyproject.toml)).project;
+
         getSource = name: path: pkgs.lib.cleanSourceWith {
           name = name;
           src = path;
           filter = gitignoreFilterWith { basePath = path; };
         };
 
         # List of supported Python versions, see also Makefile
         snakes = flip map [ "310" "311"]
           (ver: rec { name = "python${ver}"; value = builtins.getAttr name pkgs;});
 
-        mkPatchDBPkg = python:
-          let
-            # Current nixpkgs carries sqlparse 0.4.3
-            sqlparse' = python.pkgs.sqlparse.overridePythonAttrs (old: rec {
-              version = "0.4.4";
-              src = python.pkgs.fetchPypi {
-                pname = "sqlparse";
-                inherit version;
-                hash = "sha256-1EYYPoS4NJ+jBh8P5/BsqUumW0JpRv/r5uPoKVMyQgw=";
-              };
-              format = "pyproject";
-              buildInputs = [ python.pkgs.flitBuildHook ];
-            });
-          in
-            python.pkgs.buildPythonPackage rec {
-              name = "patchdb";
-              src = getSource "patchdb" ./.;
-              propagatedBuildInputs = [
-                sqlparse'
-              ] ++ (with python.pkgs; [
-                enlighten
-              ]);
-              format = "pyproject";
-              nativeBuildInputs = [ python.pkgs.pdm-pep517 ];
-              doCheck = false;
-            };
+        mkPatchDBPkg = python: python.pkgs.buildPythonPackage {
+          name = pinfo.name;
+          version = pinfo.version;
+
+          src = getSource "patchdb" ./.;
+          propagatedBuildInputs = (with python.pkgs; [
+            enlighten
+            sqlparse
+          ]);
+          format = "pyproject";
+          nativeBuildInputs = (with python.pkgs; [
+            pdm-pep517
+          ]);
+          doCheck = false;
+        };
 
         patchDBPkgs = flip map snakes
           (py: {
             name = "patchdb-${py.name}";
             value = mkPatchDBPkg py.value;
           });
 
-        patchDBApps = flip map (zipLists snakes patchDBPkgs)
-          (combo:
-            let
-              python = combo.fst.value;
-              name = combo.snd.name;
-              patchdb = combo.snd.value;
-            in {
-              inherit name;
-              value = {
-                type = "app";
-                program = "${python.pkgs.toPythonApplication patchdb}/bin/patchdb";};
-            });
-
         mkTestShell = python:
           let
             patchdb = mkPatchDBPkg python;
           in
             pkgs.mkShell {
               name = "Test Python ${python.version}";
               packages = [
@@ -98,14 +77,18 @@
               ]) ++ (with python.pkgs; [
                 docutils
                 psycopg
                 pytest
                 sphinx
               ]);
 
+            shellHook = ''
+               export PYTHONPATH="$(pwd)/src''${PYTHONPATH:+:}$PYTHONPATH"
+             '';
+
               LANG="C";
             };
 
         testShells = flip map snakes
           (py: {
             name = "test-${py.name}";
             value = mkTestShell py.value;
@@ -122,20 +105,18 @@
               postgresql_15
               python3
               twine
               yq-go
             ] ++ (with pkgs.python3Packages; [
               babel
               build
-              tomli
             ]);
 
             shellHook = ''
                export PYTHONPATH="$(pwd)/src''${PYTHONPATH:+:}$PYTHONPATH"
              '';
           };
         } // builtins.listToAttrs testShells;
 
-        packages = builtins.listToAttrs patchDBPkgs;
-        apps = builtins.listToAttrs patchDBApps;
+        packages = (builtins.listToAttrs patchDBPkgs);
       });
 }
```

### Comparing `metapensiero.sphinx.patchdb-4.0.dev4/pyproject.toml` & `metapensiero.sphinx.patchdb-4.0.dev5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "metapensiero.sphinx.patchdb"
 description = "Extract scripts from a reST document and apply them in order."
-version = "4.0.dev4"
+version = "4.0.dev5"
 authors = [
     { name = "Lele Gaifax", email = "lele@metapensiero.it" },
 ]
 readme = "README.rst"
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
@@ -37,15 +37,14 @@
 [project.optional-dependencies]
 dev = [
     "babel",
     "build",
     "bump2version",
     "pygments",
     "sphinx",
-    "tomli",
     "twine",
 ]
 
 [project.scripts]
 patchdb = "metapensiero.sphinx.patchdb.pup:main"
 patchdb-states = "metapensiero.sphinx.patchdb.states:main"
```

### Comparing `metapensiero.sphinx.patchdb-4.0.dev4/src/metapensiero/sphinx/patchdb/__init__.py` & `metapensiero.sphinx.patchdb-4.0.dev5/src/metapensiero/sphinx/patchdb/__init__.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev4/src/metapensiero/sphinx/patchdb/contexts/__init__.py` & `metapensiero.sphinx.patchdb-4.0.dev5/src/metapensiero/sphinx/patchdb/contexts/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 # :Project:   PatchDB -- Script execution contexts
 # :Created:   Wed Nov  5 17:32:16 2003
 # :Author:    Lele Gaifax <lele@metapensiero.it>
 # :License:   GNU General Public License version 3 or later
-# :Copyright: © 2003, 2014, 2016, 2017, 2019, 2021 Lele Gaifax
+# :Copyright: © 2003, 2014, 2016, 2017, 2019, 2021, 2023 Lele Gaifax
 #
 
 import logging
 import os
 import re
 
 from ..locale import gettext as _
@@ -61,46 +61,40 @@
             else:
                 logger.info("Executing %s %s", patch.language, patch)
                 ctx.apply(patch, options, patch_manager)
         else:
             raise ExecutionError("Not able to execute %s %s" %
                                  (patch.language, patch))
 
-    def __init__(self, current_state=None):
-        """
-        Insert this context instance in the registry.
-        """
-
-        if self.language_name:
-            registry = self.execution_contexts_registry
-            assert self.language_name not in registry
-            registry[self.language_name] = self
+    def __init__(self):
         self.assertions = {}
-        if current_state is not None:
-            self._testing_state = current_state
 
-    def __getitem__(self, patchid):
+    def register(self):
         """
-        Dummy implementation, used by doctests.
+        Insert this context instance in the registry.
         """
 
-        try:
-            return self._testing_state.get(patchid)
-        except AttributeError:
-            pass
+        assert self.language_name
+        registry = self.execution_contexts_registry
+        assert self.language_name not in registry
+        registry[self.language_name] = self
+
+    def __enter__(self):
+        self.register()
+        return self
+
+    def unregister(self):
+        assert self.language_name
+        registry = self.execution_contexts_registry
+        assert self.language_name in registry
+        assert registry[self.language_name] is self
+        del registry[self.language_name]
 
-    def __setitem__(self, patchid, revision):
-        """
-        Dummy implementation, used by doctests.
-        """
-
-        try:
-            self._testing_state[patchid] = revision
-        except AttributeError:
-            pass
+    def __exit__(self, exc_type, exc_value, traceback):
+        self.unregister()
 
     def addAssertions(self, assertions):
         """
         Add given `assertions` to the set of assertions managed by the context.
         """
 
         for assertion in assertions:
@@ -211,10 +205,26 @@
                             charset=args.charset, driver=args.driver)
 
     if args.sqlite:
         from .sqlite import SQLiteContext
         return SQLiteContext(database=args.sqlite)
 
 
+class DummyExecutionContext(ExecutionContext):
+    def __init__(self, current_state=None):
+        super().__init__()
+        self.current_state = {} if current_state is None else current_state
+
+    @property
+    def patches(self):
+        return self.current_state
+
+    def __getitem__(self, patchid):
+        return self.current_state.get(patchid)
+
+    def __setitem__(self, patchid, revision):
+        self.current_state[patchid] = revision
+
+
 # Register the context for Python, always available
 from .python import PythonContext
-PythonContext()
+PythonContext().register()
```

### Comparing `metapensiero.sphinx.patchdb-4.0.dev4/src/metapensiero/sphinx/patchdb/contexts/firebird.py` & `metapensiero.sphinx.patchdb-4.0.dev5/src/metapensiero/sphinx/patchdb/contexts/firebird.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev4/src/metapensiero/sphinx/patchdb/contexts/mysql.py` & `metapensiero.sphinx.patchdb-4.0.dev5/src/metapensiero/sphinx/patchdb/contexts/mysql.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev4/src/metapensiero/sphinx/patchdb/contexts/postgres.py` & `metapensiero.sphinx.patchdb-4.0.dev5/src/metapensiero/sphinx/patchdb/contexts/postgres.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev4/src/metapensiero/sphinx/patchdb/contexts/python.py` & `metapensiero.sphinx.patchdb-4.0.dev5/src/metapensiero/sphinx/patchdb/contexts/python.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev4/src/metapensiero/sphinx/patchdb/contexts/sql.py` & `metapensiero.sphinx.patchdb-4.0.dev5/src/metapensiero/sphinx/patchdb/contexts/sql.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev4/src/metapensiero/sphinx/patchdb/contexts/sqlite.py` & `metapensiero.sphinx.patchdb-4.0.dev5/src/metapensiero/sphinx/patchdb/contexts/sqlite.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev4/src/metapensiero/sphinx/patchdb/locale/__init__.py` & `metapensiero.sphinx.patchdb-4.0.dev5/src/metapensiero/sphinx/patchdb/locale/__init__.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev4/src/metapensiero/sphinx/patchdb/locale/it/LC_MESSAGES/metapensiero-sphinx-patchdb.po` & `metapensiero.sphinx.patchdb-4.0.dev5/src/metapensiero/sphinx/patchdb/locale/it/LC_MESSAGES/metapensiero-sphinx-patchdb.po`

 * *Files 1% similar despite different names*

```diff
@@ -2,29 +2,28 @@
 # Copyright (C) 2016, 2017, 2019, 2021, 2022, 2023 Lele Gaifax
 # This file is distributed under the same license as the
 # metapensiero.sphinx.patchdb project.
 # Lele Gaifax <lele@metapensiero.it>, 2016.
 #
 msgid ""
 msgstr ""
-"Project-Id-Version: metapensiero.sphinx.patchdb 4.0.dev4\n"
+"Project-Id-Version: metapensiero.sphinx.patchdb 4.0.dev5\n"
 "Report-Msgid-Bugs-To: lele@metapensiero.it\n"
-"POT-Creation-Date: 2023-04-30 16:25+0200\n"
-"PO-Revision-Date: 2023-04-30 16:28+0200\n"
+"POT-Creation-Date: 2023-06-04 17:23+0200\n"
+"PO-Revision-Date: 2023-06-04 17:26+0200\n"
 "Last-Translator: Lele Gaifax <lele@metapensiero.it>\n"
 "Language: it\n"
 "Language-Team: it <lele@metapensiero.it>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
-#: src/metapensiero/sphinx/patchdb/pup.py:65
-#: src/metapensiero/sphinx/patchdb/pup.py:88
+#: src/metapensiero/sphinx/patchdb/pup.py:54
 #, python-format
 msgid ""
 "\n"
 "Error: %s"
 msgstr ""
 "\n"
 "Errore: %s"
@@ -41,19 +40,19 @@
 msgid " (revision %(revno)d)"
 msgstr " (revisione %(revno)d)"
 
 #: src/metapensiero/sphinx/patchdb/script.py:496
 msgid "After any other script"
 msgstr "Dopo tutti gli altri script"
 
-#: src/metapensiero/sphinx/patchdb/pup.py:162
+#: src/metapensiero/sphinx/patchdb/pup.py:164
 msgid "Assume missing patches are already applied, do not re-execute them."
 msgstr "Assumi che gli script mancanti siano già stati applicati, non rieseguirli."
 
-#: src/metapensiero/sphinx/patchdb/pup.py:175
+#: src/metapensiero/sphinx/patchdb/pup.py:177
 msgid "Be quiet, emit only error messages."
 msgstr "Emetti solo messaggi di errore."
 
 #: src/metapensiero/sphinx/patchdb/script.py:494
 msgid "Before any other script"
 msgstr "Prima di qualsiasi altro script"
 
@@ -65,19 +64,19 @@
 msgid "Condition"
 msgstr "Condizione"
 
 #: src/metapensiero/sphinx/patchdb/script.py:478
 msgid "Conditions"
 msgstr "Condizioni"
 
-#: src/metapensiero/sphinx/patchdb/pup.py:130
+#: src/metapensiero/sphinx/patchdb/pup.py:132
 msgid "Database script applier"
 msgstr "Database script applier"
 
-#: src/metapensiero/sphinx/patchdb/pup.py:169
+#: src/metapensiero/sphinx/patchdb/pup.py:171
 msgid ""
 "Define an arbitrary variable usable as “{{VARNAME}}” within a script. VAR"
 " must be something like “varname=value”. This option may be given "
 "multiple times."
 msgstr ""
 "Definisce una variabile arbitraria usabile come “{{VARNAME}}” in uno "
 "script. VAR deve essere qualche cosa nella forma “nomevariabile=valore”. "
@@ -87,49 +86,50 @@
 msgid "Depends on"
 msgstr "Dipende da"
 
 #: src/metapensiero/sphinx/patchdb/script.py:468
 msgid "Direct dependants"
 msgstr "Dipendenze dirette"
 
-#: src/metapensiero/sphinx/patchdb/pup.py:173
+#: src/metapensiero/sphinx/patchdb/pup.py:175
 msgid "Don't apply patches, just list them."
 msgstr "Non applicare gli script, elencali solamente."
 
-#: src/metapensiero/sphinx/patchdb/pup.py:82
+#: src/metapensiero/sphinx/patchdb/pup.py:48
 #, python-format
 msgid "Done, applied %d script"
 msgid_plural "Done, applied %d scripts"
 msgstr[0] "Fatto, applicato %d script"
 msgstr[1] "Fatto, applicati %d script"
 
-#: src/metapensiero/sphinx/patchdb/pup.py:157
+#: src/metapensiero/sphinx/patchdb/pup.py:159
 msgid "Driver to access MySQL, defaults to “pymysql”."
 msgstr "Driver per accedere a MySQL, di default “pymysql”."
 
 #: src/metapensiero/sphinx/patchdb/script.py:465
 msgid "Drops"
 msgstr "Elimina"
 
-#: src/metapensiero/sphinx/patchdb/pup.py:177
+#: src/metapensiero/sphinx/patchdb/pup.py:179
 msgid "Emit debug messages."
 msgstr "Emetti i messaggi di debug."
 
-#: src/metapensiero/sphinx/patchdb/pup.py:155
+#: src/metapensiero/sphinx/patchdb/pup.py:157
 msgid "Encoding used by the MySQL driver, defaults to “utf8mb4”."
 msgstr "Codifica usata dal driver MySQL, di default “utf8mb4”."
 
-#: src/metapensiero/sphinx/patchdb/pup.py:45
+#: src/metapensiero/sphinx/patchdb/pup.py:116
 #, python-format
 msgid "Error: %s"
 msgstr "Errore: %s"
 
-#: src/metapensiero/sphinx/patchdb/pup.py:94
-msgid "Error: circular dependencies among scripts"
-msgstr "Errore: dipendenze cicliche tra gli script"
+#: src/metapensiero/sphinx/patchdb/pup.py:61
+#, python-format
+msgid "Error: could not apply %d scripts due to circular dependencies"
+msgstr "Errore: impossibile applicare %d script a causa di dipendenze circolari"
 
 #: src/metapensiero/sphinx/patchdb/script.py:492
 msgid "Execute always"
 msgstr "Applicato ogni volta"
 
 #: src/metapensiero/sphinx/patchdb/script.py:233
 msgid "File insertion disabled"
@@ -139,78 +139,78 @@
 msgid ""
 "Go on with the next script, skipping any succeding statements of the "
 "failing script"
 msgstr ""
 "Continua con il prossimo script, saltando le istruzioni successive a "
 "quella che ha generato l'errore"
 
-#: src/metapensiero/sphinx/patchdb/pup.py:151
+#: src/metapensiero/sphinx/patchdb/pup.py:153
 msgid "Host name where MySQL server runs, defaults to “localhost”."
 msgstr "Nome dell'host del server MySQL, di default “localhost”."
 
 #: src/metapensiero/sphinx/patchdb/script.py:510
 msgid ""
 "Ignore the error and keeps going with the remaining statements in the "
 "script"
 msgstr "Ignora gli errore e prosegui con le istruzioni successive dello script"
 
-#: src/metapensiero/sphinx/patchdb/pup.py:165
+#: src/metapensiero/sphinx/patchdb/pup.py:167
 msgid ""
 "Introduce an arbitrary assertion usable as a pre-condition by the "
 "scripts. NAME may be a simple string or something like “production=true”."
 " This option may be given multiple times."
 msgstr ""
 "Introduce una affermazione arbitraria usabile come precondizione in uno "
 "script. NAME può essere una semplice stringa oppure nella forma "
 "“produzione=true”. Questa opzione può essere specificata più di una "
 "volta."
 
-#: src/metapensiero/sphinx/patchdb/pup.py:59
+#: src/metapensiero/sphinx/patchdb/pup.py:109
 #, python-format
 msgid "Invalid variable: %s"
 msgstr "Variabile non valida: %s"
 
 #: src/metapensiero/sphinx/patchdb/script.py:202
 #, python-format
 msgid "Missing mandatory ID for the directive \"%s\"."
 msgstr "La direttiva \"%s\" richiede un ID."
 
-#: src/metapensiero/sphinx/patchdb/pup.py:133
+#: src/metapensiero/sphinx/patchdb/pup.py:135
 msgid ""
 "One or more archives containing collected scripts. May be either plain "
 "file names or package relative paths like “package.name:some/file”."
 msgstr ""
 "Uno o più archivi contenenti degli script. Si possono specificare sia "
 "nomi di file piuttosto che percorsi relativi tipo "
 "“nome.pacchetto:qualche/file”."
 
-#: src/metapensiero/sphinx/patchdb/pup.py:149
+#: src/metapensiero/sphinx/patchdb/pup.py:151
 msgid "Password"
 msgstr "Password"
 
 # | msgid "" "Perform a backup of the database in directory DIR (by default "
 # | "“%(default)s”) before doing anything. Specify “None” to disable backups."
-#: src/metapensiero/sphinx/patchdb/pup.py:179
+#: src/metapensiero/sphinx/patchdb/pup.py:181
 msgid ""
 "Perform a backup of the database in directory DIR before doing anything, "
 "that by default (or by specifying “None”) does not happen."
 msgstr ""
-"Esegui un backup del database nella directory DIR prima di fare qualsiasi "
-"cosa, che di norma (oppure quando viene specificato “None”) non viene "
+"Esegui un backup del database nella directory DIR prima di fare qualsiasi"
+" cosa, che di norma (oppure quando viene specificato “None”) non viene "
 "effettuato."
 
-#: src/metapensiero/sphinx/patchdb/pup.py:153
+#: src/metapensiero/sphinx/patchdb/pup.py:155
 msgid "Port number used by the MySQL server, defaults to “3306”."
 msgstr "Porta usata dal server MySQL, di default “3306”. "
 
 #: src/metapensiero/sphinx/patchdb/script.py:463
 msgid "Preceeds"
 msgstr "Precede"
 
-#: src/metapensiero/sphinx/patchdb/script.py:654
+#: src/metapensiero/sphinx/patchdb/script.py:653
 #, python-format
 msgid "Reference to an unknown script: %(scriptid)r"
 msgstr "Riferimento a uno script sconosciuto: %(scriptid)r"
 
 #: src/metapensiero/sphinx/patchdb/script.py:219
 #, python-format
 msgid ""
@@ -293,35 +293,35 @@
 msgid "Script index"
 msgstr "Indice degli script"
 
 #: src/metapensiero/sphinx/patchdb/script.py:366
 msgid "Scripts"
 msgstr "Script"
 
-#: src/metapensiero/sphinx/patchdb/pup.py:141
+#: src/metapensiero/sphinx/patchdb/pup.py:143
 msgid "Select the Firebird context."
 msgstr "Seleziona il contesto Firebird."
 
-#: src/metapensiero/sphinx/patchdb/pup.py:145
+#: src/metapensiero/sphinx/patchdb/pup.py:147
 msgid "Select the MySQL context."
 msgstr "Seleziona il contesto MySQL."
 
-#: src/metapensiero/sphinx/patchdb/pup.py:138
+#: src/metapensiero/sphinx/patchdb/pup.py:140
 msgid ""
 "Select the PostgreSQL context. DSN is a string of the kind "
 "“host=localhost dbname=mydb user=myself password=ouch”."
 msgstr ""
 "Seleziona il contesto PostgreSQL. DSN è una stringa nel formato "
 "“host=localhost dbname=miodb user=iostesso password=blabla”."
 
-#: src/metapensiero/sphinx/patchdb/pup.py:143
+#: src/metapensiero/sphinx/patchdb/pup.py:145
 msgid "Select the SQLite context."
 msgstr "Seleziona il contesto SQLite."
 
-#: src/metapensiero/sphinx/patchdb/pup.py:160
+#: src/metapensiero/sphinx/patchdb/pup.py:162
 msgid "Specify where to write the execution log."
 msgstr "Specifica dove scrivere il log dell'esecuzione."
 
 #: src/metapensiero/sphinx/patchdb/script.py:577
 #, python-format
 msgid ""
 "The %(scriptid)s (defined in %(docname)s at line %(lineno)s) brings an "
@@ -355,28 +355,28 @@
 msgid ""
 "The %(scriptid)s (defined in %(docname)s at line %(lineno)s) references "
 "an unknown script \"%(other)s\""
 msgstr ""
 "Lo %(scriptid)s (definito in %(docname)s alla riga %(lineno)s) referenzia"
 " uno script sconosciuto \"%(other)s\""
 
-#: src/metapensiero/sphinx/patchdb/pup.py:74
+#: src/metapensiero/sphinx/patchdb/pup.py:40
 msgid "Upgrading:"
 msgstr "Aggiornamento:"
 
-#: src/metapensiero/sphinx/patchdb/pup.py:147
+#: src/metapensiero/sphinx/patchdb/pup.py:149
 msgid "Username to log into the database."
 msgstr "Nome utente per accedere al database."
 
-#: src/metapensiero/sphinx/patchdb/contexts/__init__.py:192
+#: src/metapensiero/sphinx/patchdb/contexts/__init__.py:186
 #, python-format
 msgid "Would apply %s"
 msgstr "Applicherei %s"
 
-#: src/metapensiero/sphinx/patchdb/pup.py:35
+#: src/metapensiero/sphinx/patchdb/pup.py:91
 msgid ""
 "You must select exactly one database with either “--postgresql”, "
 "“--firebird”, “--mysql” or “--sqlite”!"
 msgstr ""
 "Devi selezionare un database con “--postgresql”, “--firebird”, “--mysql” "
 "o “--sqlite”!"
```

### Comparing `metapensiero.sphinx.patchdb-4.0.dev4/src/metapensiero/sphinx/patchdb/locale/metapensiero-sphinx-patchdb.pot` & `metapensiero.sphinx.patchdb-4.0.dev5/src/metapensiero/sphinx/patchdb/locale/metapensiero-sphinx-patchdb.pot`

 * *Files 2% similar despite different names*

```diff
@@ -3,27 +3,26 @@
 # This file is distributed under the same license as the
 # metapensiero.sphinx.patchdb project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2023.
 #
 #, fuzzy
 msgid ""
 msgstr ""
-"Project-Id-Version: metapensiero.sphinx.patchdb 4.0.dev4\n"
+"Project-Id-Version: metapensiero.sphinx.patchdb 4.0.dev5\n"
 "Report-Msgid-Bugs-To: lele@metapensiero.it\n"
-"POT-Creation-Date: 2023-04-30 16:25+0200\n"
+"POT-Creation-Date: 2023-06-04 17:23+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
-#: src/metapensiero/sphinx/patchdb/pup.py:65
-#: src/metapensiero/sphinx/patchdb/pup.py:88
+#: src/metapensiero/sphinx/patchdb/pup.py:54
 #, python-format
 msgid ""
 "\n"
 "Error: %s"
 msgstr ""
 
 #: src/metapensiero/sphinx/patchdb/script.py:422
@@ -38,19 +37,19 @@
 msgid " (revision %(revno)d)"
 msgstr ""
 
 #: src/metapensiero/sphinx/patchdb/script.py:496
 msgid "After any other script"
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/pup.py:162
+#: src/metapensiero/sphinx/patchdb/pup.py:164
 msgid "Assume missing patches are already applied, do not re-execute them."
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/pup.py:175
+#: src/metapensiero/sphinx/patchdb/pup.py:177
 msgid "Be quiet, emit only error messages."
 msgstr ""
 
 #: src/metapensiero/sphinx/patchdb/script.py:494
 msgid "Before any other script"
 msgstr ""
 
@@ -62,67 +61,68 @@
 msgid "Condition"
 msgstr ""
 
 #: src/metapensiero/sphinx/patchdb/script.py:478
 msgid "Conditions"
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/pup.py:130
+#: src/metapensiero/sphinx/patchdb/pup.py:132
 msgid "Database script applier"
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/pup.py:169
+#: src/metapensiero/sphinx/patchdb/pup.py:171
 msgid ""
 "Define an arbitrary variable usable as “{{VARNAME}}” within a script. VAR"
 " must be something like “varname=value”. This option may be given "
 "multiple times."
 msgstr ""
 
 #: src/metapensiero/sphinx/patchdb/script.py:462
 msgid "Depends on"
 msgstr ""
 
 #: src/metapensiero/sphinx/patchdb/script.py:468
 msgid "Direct dependants"
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/pup.py:173
+#: src/metapensiero/sphinx/patchdb/pup.py:175
 msgid "Don't apply patches, just list them."
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/pup.py:82
+#: src/metapensiero/sphinx/patchdb/pup.py:48
 #, python-format
 msgid "Done, applied %d script"
 msgid_plural "Done, applied %d scripts"
 msgstr[0] ""
 msgstr[1] ""
 
-#: src/metapensiero/sphinx/patchdb/pup.py:157
+#: src/metapensiero/sphinx/patchdb/pup.py:159
 msgid "Driver to access MySQL, defaults to “pymysql”."
 msgstr ""
 
 #: src/metapensiero/sphinx/patchdb/script.py:465
 msgid "Drops"
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/pup.py:177
+#: src/metapensiero/sphinx/patchdb/pup.py:179
 msgid "Emit debug messages."
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/pup.py:155
+#: src/metapensiero/sphinx/patchdb/pup.py:157
 msgid "Encoding used by the MySQL driver, defaults to “utf8mb4”."
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/pup.py:45
+#: src/metapensiero/sphinx/patchdb/pup.py:116
 #, python-format
 msgid "Error: %s"
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/pup.py:94
-msgid "Error: circular dependencies among scripts"
+#: src/metapensiero/sphinx/patchdb/pup.py:61
+#, python-format
+msgid "Error: could not apply %d scripts due to circular dependencies"
 msgstr ""
 
 #: src/metapensiero/sphinx/patchdb/script.py:492
 msgid "Execute always"
 msgstr ""
 
 #: src/metapensiero/sphinx/patchdb/script.py:233
@@ -131,66 +131,66 @@
 
 #: src/metapensiero/sphinx/patchdb/script.py:506
 msgid ""
 "Go on with the next script, skipping any succeding statements of the "
 "failing script"
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/pup.py:151
+#: src/metapensiero/sphinx/patchdb/pup.py:153
 msgid "Host name where MySQL server runs, defaults to “localhost”."
 msgstr ""
 
 #: src/metapensiero/sphinx/patchdb/script.py:510
 msgid ""
 "Ignore the error and keeps going with the remaining statements in the "
 "script"
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/pup.py:165
+#: src/metapensiero/sphinx/patchdb/pup.py:167
 msgid ""
 "Introduce an arbitrary assertion usable as a pre-condition by the "
 "scripts. NAME may be a simple string or something like “production=true”."
 " This option may be given multiple times."
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/pup.py:59
+#: src/metapensiero/sphinx/patchdb/pup.py:109
 #, python-format
 msgid "Invalid variable: %s"
 msgstr ""
 
 #: src/metapensiero/sphinx/patchdb/script.py:202
 #, python-format
 msgid "Missing mandatory ID for the directive \"%s\"."
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/pup.py:133
+#: src/metapensiero/sphinx/patchdb/pup.py:135
 msgid ""
 "One or more archives containing collected scripts. May be either plain "
 "file names or package relative paths like “package.name:some/file”."
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/pup.py:149
+#: src/metapensiero/sphinx/patchdb/pup.py:151
 msgid "Password"
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/pup.py:179
+#: src/metapensiero/sphinx/patchdb/pup.py:181
 msgid ""
 "Perform a backup of the database in directory DIR before doing anything, "
 "that by default (or by specifying “None”) does not happen."
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/pup.py:153
+#: src/metapensiero/sphinx/patchdb/pup.py:155
 msgid "Port number used by the MySQL server, defaults to “3306”."
 msgstr ""
 
 #: src/metapensiero/sphinx/patchdb/script.py:463
 msgid "Preceeds"
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/script.py:654
+#: src/metapensiero/sphinx/patchdb/script.py:653
 #, python-format
 msgid "Reference to an unknown script: %(scriptid)r"
 msgstr ""
 
 #: src/metapensiero/sphinx/patchdb/script.py:219
 #, python-format
 msgid ""
@@ -256,33 +256,33 @@
 msgid "Script index"
 msgstr ""
 
 #: src/metapensiero/sphinx/patchdb/script.py:366
 msgid "Scripts"
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/pup.py:141
+#: src/metapensiero/sphinx/patchdb/pup.py:143
 msgid "Select the Firebird context."
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/pup.py:145
+#: src/metapensiero/sphinx/patchdb/pup.py:147
 msgid "Select the MySQL context."
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/pup.py:138
+#: src/metapensiero/sphinx/patchdb/pup.py:140
 msgid ""
 "Select the PostgreSQL context. DSN is a string of the kind "
 "“host=localhost dbname=mydb user=myself password=ouch”."
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/pup.py:143
+#: src/metapensiero/sphinx/patchdb/pup.py:145
 msgid "Select the SQLite context."
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/pup.py:160
+#: src/metapensiero/sphinx/patchdb/pup.py:162
 msgid "Specify where to write the execution log."
 msgstr ""
 
 #: src/metapensiero/sphinx/patchdb/script.py:577
 #, python-format
 msgid ""
 "The %(scriptid)s (defined in %(docname)s at line %(lineno)s) brings an "
@@ -307,26 +307,26 @@
 #: src/metapensiero/sphinx/patchdb/script.py:471
 #, python-format
 msgid ""
 "The %(scriptid)s (defined in %(docname)s at line %(lineno)s) references "
 "an unknown script \"%(other)s\""
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/pup.py:74
+#: src/metapensiero/sphinx/patchdb/pup.py:40
 msgid "Upgrading:"
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/pup.py:147
+#: src/metapensiero/sphinx/patchdb/pup.py:149
 msgid "Username to log into the database."
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/contexts/__init__.py:192
+#: src/metapensiero/sphinx/patchdb/contexts/__init__.py:186
 #, python-format
 msgid "Would apply %s"
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/pup.py:35
+#: src/metapensiero/sphinx/patchdb/pup.py:91
 msgid ""
 "You must select exactly one database with either “--postgresql”, "
 "“--firebird”, “--mysql” or “--sqlite”!"
 msgstr ""
```

### Comparing `metapensiero.sphinx.patchdb-4.0.dev4/src/metapensiero/sphinx/patchdb/manager.py` & `metapensiero.sphinx.patchdb-4.0.dev5/src/metapensiero/sphinx/patchdb/patch.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,369 +1,419 @@
 # -*- coding: utf-8 -*-
-# :Project:   PatchDB -- Script&Patch Manager
-# :Created:   ven 14 ago 2009 13:09:28 CEST
-# :Author:    Lele Gaifax <lele@nautilus.homeip.net>
+# :Project:   PatchDB -- Patch object
+# :Created:   Fri Oct  3 01:13:20 2003
+# :Author:    Lele Gaifax <lele@metapensiero.it>
 # :License:   GNU General Public License version 3 or later
-# :Copyright: © 2009, 2010, 2012-2018, 2021, 2023 Lele Gaifax
+# :Copyright: © 2003, 2009, 2010, 2012-2017, 2019, 2021, 2023 Lele Gaifax
 #
 
 from collections import defaultdict
-import json
+from graphlib import TopologicalSorter
 import logging
-import pickle
-from os.path import dirname, exists, relpath
-
-from .patch import DependencyError, sort_by_constraints
 
 
 logger = logging.getLogger(__name__)
 # logger.setLevel(logging.DEBUG)
 
-
-class DuplicatedScriptError(Exception):
-    "Indicates that a script is not unique."
+MAX_PATCHID_LEN = 100
 
 
-class Missing3rdPartyModule(Exception):
-    "Indicates that a 3rd party module is missing"
+class DependencyError(Exception):
+    "Indicate some problem with the dependencies."
 
 
-class _MissingPatchesIterator:
-    def __init__(self, manager, context, always_first, missing, always_last):
-        self.manager = manager
-        self.context = context
-        self.always_first = always_first
-        self.missing = missing
-        self.always_last = always_last
-
-    def __len__(self):
-        return len(self.always_first) + len(self.missing) + len(self.always_last)
-
-    def __iter__(self):
-        context = self.context
-        precedences = self.manager.precedences
-        always_first = self.always_first
-        missing = self.missing
-        always_last = self.always_last
-        migrations = {p for p in missing if p.is_migration}
-
-        if always_first:
-            logger.info("Applying execute-always-first patches...")
-            for patch in sort_by_constraints(always_first, self.manager):
-                yield patch
-
-        logger.info("Applying missing patches...")
-        while missing:
-            # Get rid of already applied scripts
-
-            applied = set()
-            for patch in missing:
-                if patch.revision == context[patch.patchid]:
-                    logger.debug("Skipping %s, already applied", patch)
-                    yield None
-                    applied.add(patch)
-
-            if applied:
-                missing -= applied
-                continue
+def compute_checksum(language, script, depends, preceeds, brings, drops, conditions,
+                     onerror, revision, mimetype):
+    """Compute a checksum from the script and its metadata.
 
-            # Try to apply migration scripts as early as possible
+    This is mainly needed to avoid repeated beautification of the same script.
+    """
 
-            pending_migrations = {}
-            patches = []
-            for patch in migrations:
-                # Postpone execution if other scripts preceed this ones
-
-                precs = precedences.get((patch.patchid, patch.revision))
-                if precs is not None:
-                    skip = False
-                    for ppatch in precs:
-                        current = context[ppatch.patchid]
-                        if current is None or current < ppatch.revision:
-                            logger.debug("Postponing %s, must follow %s which is"
-                                         " currently at %s", patch, ppatch, current)
-                            skip = True
-                            break
-                    if skip:
-                        continue
-
-                # Take note about what this migration is bringing, so that we can postpone the
-                # execution of those patches, giving an higher priority to the migration itself
-
-                for depid, deprev in patch.brings:
-                    pending_migrations[(depid, deprev)] = patch
-
-                # Consider patch dependencies: postpone execution if they are not yet met, skip
-                # it if we are beyond the requested revisions
-
-                for depid, deprev in patch.depends:
-                    current = context[depid]
-                    if current is None or current < deprev:
-                        logger.debug("Postponing %s, depends on '%s@%s' but it's at %s",
-                                     patch, depid, deprev, current)
-                        break
-                    elif current is not None and current > deprev:
-                        logger.debug("Skipping %s, depends on '%s@%s' but it's already at %s",
-                                     patch, depid, deprev, current)
-                        yield None
-                        applied.add(patch)
-                        break
-                else:
-                    # Skip migration script when what it brings is already there
+    from hashlib import md5
 
-                    for depid, deprev in patch.brings:
-                        current = context[depid]
-                        if current is not None and current >= deprev:
-                            logger.debug("Skipping %s, brings '%s@%s' but it's already at %s",
-                                         patch, depid, deprev, current)
-                            yield None
-                            applied.add(patch)
-                            break
-                    else:
-                        patches.append(patch)
-            if patches:
-                for patch in sort_by_constraints(patches, self.manager):
-                    yield patch
-                    applied.add(patch)
-
-            if applied:
-                missing -= applied
-                migrations -= applied
-                continue
+    return md5(b'#'.join((language.encode('ascii', 'ignore'),
+                          script.encode('ascii', 'ignore'),
+                          repr(depends).encode('ascii', 'ignore'),
+                          repr(preceeds).encode('ascii', 'ignore'),
+                          repr(brings).encode('ascii', 'ignore'),
+                          repr(drops).encode('ascii', 'ignore'),
+                          repr(conditions).encode('ascii', 'ignore'),
+                          repr(revision).encode('ascii', 'ignore'),
+                          repr(mimetype).encode('ascii', 'ignore')))).digest()
 
-            # Normal scripts
 
-            patches = []
-            for patch in missing:
-                precs = precedences.get((patch.patchid, patch.revision))
-                if precs is not None:
-                    skip = False
-                    for ppatch in precs:
-                        current = context[ppatch.patchid]
-                        if current is None or current < ppatch.revision:
-                            logger.debug("Postponing %s, must follow %s which is"
-                                         " currently at %s", patch, ppatch, current)
-                            skip = True
-                            break
-                    if skip:
-                        continue
-
-                if (patch.patchid, patch.revision) in pending_migrations:
-                    logger.debug("Postponing %s, will be brough by %s",
-                                 patch, pending_migrations[(patch.patchid, patch.revision)])
-                    continue
+class Patch:
+    """
+    Represent a single `patch`, that is some kind of arbitrary script
+    written in some language, curried with some metadata.
+    """
 
-                for depid, deprev in patch.depends:
-                    current = context[depid]
-                    if current is None or current < deprev:
-                        logger.debug("Postponing %s, depends on '%s@%s' but it's at %s",
-                                     patch, depid, deprev, current)
-                        break
-                    elif current is not None and current > deprev:
-                        logger.debug("Skipping %s, depends on '%s@%s' but it's already at %s",
-                                     patch, depid, deprev, current)
-                        yield None
-                        applied.add(patch)
-                        break
-                else:
-                    patches.append(patch)
-            if patches:
-                for patch in sort_by_constraints(patches, self.manager):
-                    yield patch
-                    applied.add(patch)
-
-            if not applied:
-                if all(p.is_migration for p in missing):
-                    for patch in missing:
-                        yield None
-                    break
-                else:
-                    logger.critical('Could not apply %d scripts', len(missing))
+    def __init__(self, patchid, description, script, language, revision,
+                 depends, preceeds, brings, drops, conditions, onerror='abort',
+                 mimetype=None, always=False, autocommit=False,
+                 source=None, line=None):
+        self.patchid = patchid
+        """The unique ID of this patch"""
 
-                    # This will raise a CircularDependencyError, if the problem is due to
-                    # dependency cycles.
+        self.description = description
+        """The description of the script"""
 
-                    sort_by_constraints(missing, self.manager)
+        self.script = script
+        """The script itself, possibly empty for placeholders"""
 
-                    # If that's not the case, list the remaining scripts for debug
+        self.language = language
+        "The language of the script, currently either 'sql' or 'python'"
 
-                    for patch in missing:
-                        logger.warning('- %s', patch)
-                    raise DependencyError('Could not apply %d scripts, probably due to'
-                                          ' non-meetable dependencies' % len(missing))
+        self.revision = revision
+        """The revision of the script"""
 
-            missing -= applied
+        self.depends = depends
+        "List of tuples (ID,rev) of the patches this one depends on"
 
-        if always_last:
-            logger.info("Applying execute-always-last patches...")
-            for patch in sort_by_constraints(always_last, self.manager):
-                yield patch
+        self.preceeds = preceeds
+        "List of tuples (ID,rev) of the patches that depend on this one"
 
+        self.brings = brings
+        "List of tuples (ID,rev) of the patches this one updates"
 
-class PatchManager:
-    """
-    An instance of this class collects a set of patches and acts as
-    a dictionary. It's able to serialize the patches taking into
-    account the dependencies.
-    """
+        self.drops = drops
+        "List of tuples (ID,None) of the patches this one drops"
 
-    def __init__(self):
-        self.db = {}
-        self.precedences = defaultdict(set)
+        self.conditions = conditions
+        "List of *conditions* that must be verified before patch application"
 
-    def __getitem__(self, patchid):
+        self.onerror = onerror
         """
-        Return the patch given its `patchid`, or ``None`` if it does not exist.
+        Behaviour on errors: 'abort' means just that, 'skip' to jump to the
+        next patch, 'ignore' to ignore the error considering the patch as fully
+        applied
         """
-        return self.db.get(patchid)
 
-    def __setitem__(self, patchid, patch):
-        """
-        Register the given `patch` identified by `patchid`.
-        """
-        self.db[patchid] = patch
+        self.mimetype = mimetype
+        "Optional mime type, to select a more specific Pygments beautifier."
+
+        self.always = always
+        "Whether the patch shall be executed always at each run, rather than only once."
+
+        self.autocommit = autocommit
+        "Whether the patch shall be executed in autocommit mode."
+
+        self.checksum = compute_checksum(language, script, depends, preceeds, brings, drops,
+                                         conditions, onerror, revision, mimetype)
+        "Checksum of the script, to track changes"
+
+        self.source = source
+        "The source file that defined this script."
+
+        self.line = line
+        "The line number where the script is defined."
+
+    def __str__(self):
+        "Return a description of the patch, for logging purposes."
+
+        kind = 'placeholder ' if self.is_placeholder else ''
+        if self.is_migration:
+            kind += 'patch'
+        else:
+            kind += 'script'
+        return '%s "%s@%d"' % (kind, self.patchid, self.revision)
+
+    def __repr__(self):
+        return '<%s>' % self
+
+    def __hash__(self):
+        return hash((self.patchid, self.revision))
+
+    def __eq__(self, other):
+        return (isinstance(other, Patch)
+                and self.patchid == other.patchid
+                and self.revision == other.revision)
+
+    def __lt__(self, other):
+        return (self.patchid, self.revision) < (other.patchid, other.revision)
+
+    @property
+    def as_dict(self):
+        res = dict(
+            ID=self.patchid,
+            language=self.language,
+            revision=self.revision,
+            script=self.script,
+            source=self.source,
+            line=self.line,
+        )
+        if self.patchid != self.description:
+            res['description'] = self.description
+
+        def rr(d):
+            if d[1]:
+                return '%s@%s' % d
+            else:
+                return d[0]
 
-    def __iadd__(self, patch):
-        self.db[patch.patchid] = patch
-        return self
+        if self.always:
+            res['always'] = self.always
+        if self.depends:
+            res['depends'] = [rr(d) for d in self.depends]
+        if self.preceeds:
+            res['preceeds'] = [rr(p) for p in self.preceeds]
+        if self.brings:
+            res['brings'] = [rr(b) for b in self.brings]
+        if self.drops:
+            res['drops'] = [rr(d) for d in self.drops]
+        if self.conditions:
+            res['conditions'] = [c for c in self.conditions]
+        if self.onerror != 'abort':
+            res['onerror'] = self.onerror
+        if self.autocommit:
+            res['autocommit'] = self.autocommit
+
+        return res
+
+    @property
+    def is_migration(self):
+        return bool(self.brings or self.drops)
+
+    @property
+    def is_placeholder(self):
+        return not self.script
 
-    def neededPatches(self, context):
+    def adjustUnspecifiedRevisions(self, pm, context):
         """
-        Return an iterator over *applicable* patches, in the
-        right order to satisfy their inter-dependencies.
+        Replace the non-specified revision numbers with the current known version of the patch.
+
+        Perform also some sanity checks: all `depends`, `brings` and `preceeds` must exist at
+        this point.
         """
 
-        missing = set()
-        always_first = set()
-        always_last = set()
-        precedences = self.precedences
-
-        logger.debug("Collecting and ordering patches...")
-        for pid, patch in self.db.items():
-            patch.adjustUnspecifiedRevisions(self, context)
-
-            applicable, reason = patch.isApplicable(context)
-            if applicable:
-                for preceed in patch.preceeds:
-                    precedences[preceed].add(patch)
-
-                if patch.always:
-                    if patch.always == 'first':
-                        always_first.add(patch)
-                    else:
-                        always_last.add(patch)
+        for i, (pid, rev) in enumerate(self.depends):
+            p = pm[pid]
+            if p is None:
+                if self.is_migration:
+                    logger.debug('%s (defined in %s at line %s)'
+                                 ' depends on "%s@%s",'
+                                 ' which does not exist: applying anyway',
+                                 self, self.source, self.line, pid, rev)
+                    continue
+                raise DependencyError('%s (defined in %s at line %s)'
+                                      ' depends on "%s@%s",'
+                                      ' which does not exist.'
+                                      % (self, self.source, self.line, pid, rev))
+            if rev is None:
+                self.depends[i] = (pid, p.revision)
+            elif rev == '*':
+                current_rev = context[pid]
+                if current_rev is None:
+                    self.depends[i] = (pid, p.revision)
                 else:
-                    missing.add(patch)
-            else:
-                logger.debug("Ignoring %s: %s", patch, reason)
+                    self.depends[i] = (pid, current_rev)
 
-        return _MissingPatchesIterator(self, context, always_first, missing, always_last)
+        for i, (pid, rev) in enumerate(self.brings):
+            p = pm[pid]
+            if p is None:
+                logger.debug('%s (defined in %s at line %s)'
+                             ' brings to "%s@%s",'
+                             ' which does not exist: applying anyway'
+                             % (self, self.source, self.line, pid, rev))
+                continue
+            if rev is None:
+                self.brings[i] = (pid, p.revision)
 
+        for i, (pid, rev) in enumerate(self.preceeds):
+            p = pm[pid]
+            if p is None:
+                if self.is_migration:
+                    logger.debug('%s (defined in %s at line %s) preceeds "%s@%s",'
+                                 ' which does not exist: applying anyway'
+                                 % (self, self.source, self.line, pid, rev))
+                else:
+                    raise DependencyError('%s (defined in %s at line %s) preceeds "%s@%s",'
+                                          ' which does not exist.'
+                                          % (self, self.source, self.line, pid, rev))
+            if rev is None:
+                self.preceeds[i] = (pid, pm[pid].revision)
+
+    def beautify(self):
+        "Compute a beautified and highlighted HTML version of the script."
+
+        from pygments import highlight
+        from pygments.lexers import get_lexer_by_name, get_lexer_for_mimetype
+        from pygments.formatters import get_formatter_by_name
 
-class PersistentPatchManager(PatchManager):
-    """
-    Patch manager that uses a Pickle/JSON file as its persistent storage.
-    """
+        logger.debug("HTMLifying %s", self)
 
-    def __init__(self, storage_path=None):
-        super().__init__()
-        if isinstance(storage_path, str):
-            self.storages = [storage_path]
+        if self.mimetype:
+            lexer = get_lexer_for_mimetype(self.mimetype, encoding="utf-8")
         else:
-            self.storages = storage_path
+            lexer = get_lexer_by_name(self.language, encoding="utf-8")
+        formatter = get_formatter_by_name('html', linenos="inline",
+                                          # produce Unicode
+                                          encoding=None)
+        return highlight(self.script, lexer, formatter)
 
-    def _checkMissingRevisionsBump(self):
-        old_db = self._load()
-        if not old_db:
-            return
-
-        for patch in self.db.values():
-            old = old_db.get(patch.patchid)
-            if old is not None:
-                if old.revision == patch.revision and old.script != patch.script:
-                    logger.warning("The %s has been modified, but the revision did not", patch)
-
-    def save(self):
-        self._checkMissingRevisionsBump()
-
-        storage_path = self.storages[0]
-        if storage_path is None:
-            return
-
-        logger.debug("Writing patches to %s", storage_path)
-        if storage_path.endswith('.json'):
-            storage = open(storage_path, 'w', encoding='utf-8')
-
-            # Order patches by id, both for easier lookup and to
-            # avoid VCs stress
-
-            asdicts = [self.db[sid].as_dict for sid in sorted(self.db)]
-            spdir = dirname(storage_path)
-            for script in asdicts:
-                if script.get('source'):
-                    script['source'] = relpath(script['source'], spdir)
+    def verifyConditions(self, context):
+        """
+        Verify pre-conditions, returning False if even only one isn't satisfied.
+        """
 
-            with open(storage_path, 'w', encoding='utf-8') as storage:
-                json.dump(asdicts, storage, sort_keys=True, indent=1)
-        else:
-            with open(storage_path, 'wb') as storage:
-                pickle.dump(list(self.db.values()), storage)
+        if self.conditions is None:
+            return True
 
-        logger.debug("Done writing patches")
+        for c in self.conditions:
+            if not context.verifyCondition(c):
+                return False
 
-    def _load(self):
-        db = {}
-        loaded_from = {}
-        for storage_path in self.storages:
-            if not exists(storage_path):
-                logger.debug("Storage %s does not exist, skipping", storage_path)
-                continue
+        return True
 
-            logger.debug("Reading patches from %s", storage_path)
-            if storage_path.endswith('.json'):
-                from .patch import make_patch
-
-                with open(storage_path, encoding='utf-8') as storage:
-                    patches = [make_patch(d['ID'], d['script'], d)
-                               for d in json.load(storage)]
-            else:
-                with open(storage_path, 'rb') as storage:
-                    patches = pickle.load(storage)
+    def isApplicable(self, context):
+        if self.is_migration and not context.patches:
+            return False, "database is empty, migrations are useless"
+
+        if not self.always and self.revision == context[self.patchid]:
+            return False, "already applied"
+
+        lang_context = context.forLanguage(self.language)
+        if lang_context is None:
+            logger.warning('No language context for %r', self.language)
+            assert self.language == 'test'
+            return True, None
 
-            for patch in patches:
-                if patch.patchid in db:
-                    existing = db[patch.patchid]
-                    if not patch.script:
-                        existing.depends.extend(patch.depends)
-                        existing.preceeds.extend(patch.preceeds)
-                    elif not existing.script:
-                        db[patch.patchid] = patch
-                    else:
-                        logger.critical("Duplicated %s: present in %s and %s",
-                                        patch, loaded_from[patch.patchid], storage_path)
-                        raise DuplicatedScriptError("%s already loaded!" % patch)
+        if not self.verifyConditions(lang_context):
+            return False, "does not satisfy the conditions"
+
+        return lang_context.isApplicable(self)
+
+
+def parse_deps(deps, allow_star=False):
+    """Parse textual dependencies.
+
+    `deps` is the textual representation of the dependencies specified in the ``depends``,
+    ``brings``, ``drops`` and ``preceeds`` fields. `allow_star` indicates whether the form
+    ``patchid@*`` is allowed.
+
+    `deps` may contain something like ``patchid@10``, to specify the revision 10 of the given
+    patch. When the revision is not specified it's set to None, and later adjusted to be the
+    current revision of the patch.
+
+    Multiple dependencies may be separated by a comma.
+
+    """
+
+    result = []
+
+    if deps:
+        if isinstance(deps, str):
+            deps = deps.split(',')
+        for dep in deps:
+            dep = dep.strip()
+            if not dep:
+                raise ValueError("empty patch ID, spurious comma?")
+            if '@' in dep:
+                depid, deprev = dep.split('@')
+                if deprev == '*':
+                    if not allow_star:
+                        raise ValueError("invalid revision: %r" % dep)
                 else:
-                    db[patch.patchid] = patch
-                loaded_from[patch.patchid] = storage_path
+                    deprev = int(deprev)
+                    if deprev < 1:
+                        raise ValueError("invalid revision: %r" % dep)
+            else:
+                depid = dep
+                deprev = None
 
-        logger.debug("Done reading patches")
-        return db
+            result.append((depid.lower(), deprev))
 
-    def load(self):
-        self.db = self._load()
+    # For purely aesthetic reasons, order dependencies alphabetically
+    result.sort()
 
+    return result
 
-__manager = None
 
+def make_patch(patchid, script, options, description=None):
+    """Create a new Patch instance given its description.
+
+    :param patchid: the unique id of the patch
+    :param script: the text of the script
+    :param options: a dictionary with all the options
+    :param description: optional, original title of the script
+    :rtype: a :py:class:`metapensiero.sphinx.patch.Patch` instance
+    """
+
+    description = options.get('description', description or patchid)
+    language = options.get('language', 'sql')
+    revision = int(options.get('revision', 1))
+    if revision < 1:
+        raise ValueError("Invalid revision, must be greater than 0")
+
+    try:
+        depends = parse_deps(options.get('depends', ''), allow_star=True)
+    except ValueError as e:
+        raise ValueError("Error in script's depends option: %s" % str(e))
+
+    try:
+        preceeds = parse_deps(options.get('preceeds', ''))
+    except ValueError as e:
+        raise ValueError("Error in script's preceeds option: %s" % str(e))
+
+    try:
+        brings = parse_deps(options.get('brings', ''))
+    except ValueError as e:
+        raise ValueError("Error in script's brings option: %s" % str(e))
+    if not script and brings:
+        raise ValueError("Placeholder script cannot bring anything")
+
+    try:
+        drops = parse_deps(options.get('drops', ''))
+    except ValueError as e:
+        raise ValueError("Error in script's drops option: %s" % str(e))
+    else:
+        for depid, deprev in drops:
+            if deprev is not None:
+                raise ValueError("Error in script's drops option:"
+                                 " dependency %r carries a revision"
+                                 % depid)
+
+    conditions = options.get('conditions', None)
+    onerror = options.get('onerror', 'abort')
+    mimetype = options.get('mimetype', None)
+    always = options.get('always', False)
+    autocommit = 'autocommit' in options
+
+    if conditions:
+        if isinstance(conditions, str):
+            conditions = [c.strip() for c in conditions.split(',')]
+    else:
+        conditions = []
+
+    if mimetype is None:
+        if language == 'python':
+            mimetype = 'application/x-python'
+        elif language == 'sql':
+            mimetype = 'text/x-sql'
+
+    return Patch(patchid, description, script, language, revision,
+                 depends, preceeds, brings, drops, conditions, onerror, mimetype,
+                 always, autocommit, options.get('source'), options.get('line'))
+
+
+def sort_by_constraints(patches, manager):
+    "Reorder given `patches` taking into account their dependencies."
+
+    constraints = defaultdict(set)
+    for patch in patches:
+        if patch.is_placeholder:
+            # This is a "placeholder" patch and it has not been applied yet
+            logger.critical("%s has not been applied yet", patch)
+            raise DependencyError('%s has not been applied yet' % patch)
+        for otherid, otherrev in patch.depends:
+            other = manager[otherid]
+            if other in patches:
+                constraints[patch].add(other)
+        for otherid, otherrev in patch.preceeds:
+            other = manager[otherid]
+            if other in patches:
+                constraints[other].add(patch)
 
-def patch_manager(storage_path, overwrite=False, autosave=False):
-    global __manager
+    if constraints:
+        patches = tuple(TopologicalSorter(constraints).static_order())
 
-    if not __manager:
-        __manager = PersistentPatchManager(storage_path)
-        if storage_path is not None:  # used by doctests
-            if not overwrite:
-                __manager.load()
-            if autosave:
-                import atexit
-                atexit.register(__manager.save)
-    return __manager
+    return patches
```

### Comparing `metapensiero.sphinx.patchdb-4.0.dev4/src/metapensiero/sphinx/patchdb/pup.py` & `metapensiero.sphinx.patchdb-4.0.dev5/src/metapensiero/sphinx/patchdb/pup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,117 +8,119 @@
 
 from graphlib import CycleError
 from os.path import isabs
 import sys
 
 import enlighten
 
-from .contexts import ExecutionContext, ExecutionError, get_context_from_args
+from .contexts import ExecutionError, get_context_from_args
 from .locale import gettext as _, ngettext, setup as setup_i18n
+from .manager import DuplicatedScriptError, Missing3rdPartyModule, PersistentPatchManager
 from .patch import DependencyError
-from .manager import DuplicatedScriptError, Missing3rdPartyModule, patch_manager
+from .planner import ExecutionPlanner
 
 
 OK, SOFTWARE, DATAERR, CONFIG, USAGE = 0, 1, 2, 3, 128
 
 
 def path_spec(ps):
     if isabs(ps) or ':' not in ps:
         return ps
     pkgname, subpath = ps.split(':', 1)
     from importlib.resources import path
     return path(pkgname, subpath)
 
 
+def apply_missing_patches(manager, context, options, progress):
+    with context:
+        try:
+            count = 0
+            patches = ExecutionPlanner(manager, context)
+            npatches = len(patches)
+            if npatches > 0:
+                with progress.counter(total=npatches, desc=_('Upgrading:'), unit='script') as pbar:
+                    for p in patches:
+                        if p is not None:
+                            count += 1
+                            context.execute(p, options, manager)
+                        pbar.update()
+            if not options.dry_run and not options.quiet:
+                print()
+                print(ngettext("Done, applied %d script",
+                               "Done, applied %d scripts",
+                               count) % count)
+            return OK
+        except (DependencyError, ExecutionError) as e:
+            write = sys.stderr.write
+            write(_("\nError: %s") % e)
+            write('\n')
+            return DATAERR
+        except CycleError as e:
+            cycle = e.args[1]
+            write = sys.stderr.write
+            unapplied = set(cycle)
+            errmsg = _("Error: could not apply %d scripts due to circular dependencies") % len(unapplied)
+            write("\n%s\n\n" % errmsg)
+            write('digraph cycle {\n')
+            seen = set()
+            for script in cycle:
+                sid = script.patchid.replace('"', r'\"')
+                srev = script.revision
+                if script.depends:
+                    for did, drev in script.depends:
+                        did = did.replace('"', r'\"')
+                        fid = f'{sid}@{srev}'
+                        tid = f'{did}@{drev}'
+                        if (fid, tid) not in seen:
+                            write(f'  "{fid}" -> "{tid}";\n')
+                            seen.add((fid, tid))
+                if script.preceeds:
+                    for did, drev in script.preceeds:
+                        did = did.replace('"', r'\"')
+                        fid = f'{did}@{drev}'
+                        tid = f'{sid}@{srev}'
+                        if (fid, tid) not in seen:
+                            write(f'  "{fid}" -> "{tid}";\n')
+                            seen.add((fid, tid))
+            write('}\n')
+            return DATAERR
+
+
 def workhorse(args, progress):
-    sqlctx = get_context_from_args(args)
-    if sqlctx is None:
+    context = get_context_from_args(args)
+    if context is None:
         print(_("You must select exactly one database with either “--postgresql”,"
                 " “--firebird”, “--mysql” or “--sqlite”!"))
         return USAGE
 
     if args.backups_dir and args.backups_dir != 'None' and not args.dry_run:
-        sqlctx.backup(args.backups_dir)
-
-    try:
-        pm = patch_manager(args.storage)
-    except (DuplicatedScriptError, Missing3rdPartyModule) as e:
-        print(_("Error: %s") % e)
-        return DATAERR
+        context.backup(args.backups_dir)
 
     if args.assertions:
         try:
-            sqlctx.addAssertions(args.assertions)
+            context.addAssertions(args.assertions)
         except ValueError as e:
             print("Invalid assertion: %s" % e)
             return CONFIG
 
     if args.variables:
         try:
-            sqlctx.addVariables(args.variables)
+            context.addVariables(args.variables)
         except ValueError as e:
             print(_("Invalid variable: %s") % e)
             return CONFIG
 
     try:
-        patches = pm.neededPatches(sqlctx)
-    except DependencyError as e:
-        print(_("\nError: %s") % e)
+        pm = PersistentPatchManager(args.storage)
+        pm.load()
+    except (DuplicatedScriptError, Missing3rdPartyModule) as e:
+        print(_("Error: %s") % e)
         return DATAERR
 
-    execute = ExecutionContext.execute
-
-    try:
-        count = 0
-        npatches = len(patches)
-        if npatches > 0:
-            with progress.counter(total=npatches, desc=_('Upgrading:'), unit='script') as pbar:
-                for p in patches:
-                    if p is not None:
-                        count += 1
-                        execute(p, args, pm)
-                    pbar.update()
-        if not args.dry_run and not args.quiet:
-            print()
-            print(ngettext("Done, applied %d script",
-                           "Done, applied %d scripts",
-                           count) % count)
-        return OK
-    except (DependencyError, ExecutionError) as e:
-        write = sys.stderr.write
-        write(_("\nError: %s") % e)
-        write('\n')
-        return DATAERR
-    except CycleError as e:
-        cycle = e.args[1]
-        write = sys.stderr.write
-        write("\n%s\n\n" % _("Error: circular dependencies among scripts"))
-        write('digraph cycle {\n')
-        seen = set()
-        for script in cycle:
-            sid = script.patchid.replace('"', r'\"')
-            srev = script.revision
-            if script.depends:
-                for did, drev in script.depends:
-                    did = did.replace('"', r'\"')
-                    fid = f'{sid}@{srev}'
-                    tid = f'{did}@{drev}'
-                    if (fid, tid) not in seen:
-                        write(f'  "{fid}" -> "{tid}";\n')
-                        seen.add((fid, tid))
-            if script.preceeds:
-                for did, drev in script.preceeds:
-                    did = did.replace('"', r'\"')
-                    fid = f'{did}@{drev}'
-                    tid = f'{sid}@{srev}'
-                    if (fid, tid) not in seen:
-                        write(f'  "{fid}" -> "{tid}";\n')
-                        seen.add((fid, tid))
-        write('}\n')
-        return DATAERR
+    return apply_missing_patches(pm, context, args, progress)
 
 
 def main():
     import locale
     import logging
     from argparse import ArgumentParser
     from importlib import metadata
```

### Comparing `metapensiero.sphinx.patchdb-4.0.dev4/src/metapensiero/sphinx/patchdb/script.py` & `metapensiero.sphinx.patchdb-4.0.dev5/src/metapensiero/sphinx/patchdb/script.py`

 * *Files 0% similar despite different names*

```diff
@@ -545,15 +545,15 @@
 
     app.patchdb_dump_scripts = True
 
 
 def dump_scripts_collection(app, env):
     "Dump the collected scripts into a new pickle archive."
 
-    from .manager import patch_manager
+    from .manager import PersistentPatchManager
 
     scripts = env.domaindata['patchdb']['scripts']
     if not scripts or not app.config.patchdb_storage:
         return
 
     # Better safe than sorry: check dependencies and report anomalies
     for sid in scripts:
@@ -587,16 +587,15 @@
                               ' still at revision %(currev)s')
                             % dict(scriptid=patch, docname=patch.source, lineno=patch.line,
                                    other=pid, newrev=rev, currev=currev))
 
     if not getattr(app, 'patchdb_dump_scripts', False):
         return
 
-    mgr = patch_manager(app.config.patchdb_storage, overwrite=True)
-
+    mgr = PersistentPatchManager(app.config.patchdb_storage)
     for sid in scripts:
         mgr[sid] = scripts[sid]['patch']
     mgr.save()
 
 
 def purge_doc(app, env, docname):
     "Remove references to scripts defined in purged document."
```

### Comparing `metapensiero.sphinx.patchdb-4.0.dev4/src/metapensiero/sphinx/patchdb/states.py` & `metapensiero.sphinx.patchdb-4.0.dev5/src/metapensiero/sphinx/patchdb/states.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 # :Project:   PatchDB -- States management
 # :Created:   ven 15 apr 2016 09:39:08 CEST
 # :Author:    Lele Gaifax <lele@metapensiero.it>
 # :License:   GNU General Public License version 3 or later
-# :Copyright: © 2016, 2017, 2021 Lele Gaifax
+# :Copyright: © 2016, 2017, 2021, 2023 Lele Gaifax
 #
 
 from collections import deque, namedtuple
 from os import remove, stat
 from os.path import exists, join
 from tempfile import gettempdir
 from time import localtime, strftime
@@ -115,23 +115,24 @@
         return USAGE
 
     bck = join(args.backups_dir, args.state)
     if not exists(bck):
         print("State %s does not have a backup, sorry!" % args.state)
         return UNAVAILABLE
 
-    sqlctx.closeConnection()
+    with sqlctx:
+        sqlctx.closeConnection()
 
-    try:
-        sqlctx.restore(bck)
-    except NotImplementedError as e:
-        print("Error: %s" % e)
-        return UNAVAILABLE
-    else:
-        return OK
+        try:
+            sqlctx.restore(bck)
+        except NotImplementedError as e:
+            print("Error: %s" % e)
+            return UNAVAILABLE
+        else:
+            return OK
 
 
 def main():
     from argparse import ArgumentParser
     import locale
     import logging
```

### Comparing `metapensiero.sphinx.patchdb-4.0.dev4/tests/fixtures.py` & `metapensiero.sphinx.patchdb-4.0.dev5/tests/fixtures.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,14 +184,16 @@
         cls.create_database()
         cls.sphinx = PatchDBSphinx((cls.DB_OPTION, cls.DB_NAME) + cls.DB_OTHER_OPTIONS,
                                    cls.BACKUPS_DIR, cls.SPHINX_BUILD_OTHER_OPTIONS)
         cls.sphinx.build({filename: content for filename, content in cls.contents()})
 
     @classmethod
     def tearDownClass(cls):
+        if getenv('PATCHDB_TEST_DRD'):
+            print(f'{cls.__name__}: leaving debris in {cls.sphinx.directory}')
         cls.sphinx.remove()
 
     @classmethod
     def drop_database_if_exists(cls):
         pass
 
     @classmethod
```

### Comparing `metapensiero.sphinx.patchdb-4.0.dev4/tests/postgresql` & `metapensiero.sphinx.patchdb-4.0.dev5/tests/postgresql`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev4/tests/test_bad.py` & `metapensiero.sphinx.patchdb-4.0.dev5/tests/test_bad.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev4/tests/test_drops.py` & `metapensiero.sphinx.patchdb-4.0.dev5/tests/test_drops.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev4/tests/test_external_file.py` & `metapensiero.sphinx.patchdb-4.0.dev5/tests/test_external_file.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev4/tests/test_helpers.py` & `metapensiero.sphinx.patchdb-4.0.dev5/tests/test_helpers.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,95 +1,85 @@
 # -*- coding: utf-8 -*-
 # :Project:   PatchDB -- Test helper functions
 # :Created:   sab 28 mag 2016 20:24:52 CEST
 # :Author:    Lele Gaifax <lele@metapensiero.it>
 # :License:   GNU General Public License version 3 or later
-# :Copyright: © 2016, 2017 Lele Gaifax
+# :Copyright: © 2016, 2017, 2023 Lele Gaifax
 #
 
-import unittest
+def test_split_script():
+    from metapensiero.sphinx.patchdb.contexts.sql import split_script
 
+    assert split_script('a\n;;\n;;\n;;\nb\n') == ['a\n', 'b\n']
+    assert split_script('a\n  ;;  \nb  \n\n;; \n c \n') == ['a\n', 'b  \n\n', ' c \n']
 
-class TestSplitScript(unittest.TestCase):
-    def test(self):
-        from metapensiero.sphinx.patchdb.contexts.sql import split_script
-
-        self.assertEqual(split_script('a\n;;\n;;\n;;\nb\n'),
-                         ['a\n', 'b\n'])
-
-        self.assertEqual(split_script('a\n  ;;  \nb  \n\n;; \n c \n'),
-                         ['a\n', 'b  \n\n', ' c \n'])
-
-
-class TestIsCreateDomain(unittest.TestCase):
-    def test(self):
-        from metapensiero.sphinx.patchdb.contexts.sql import is_create_domain
-
-        self.assertTrue(is_create_domain('Create Domain foo bar'))
-        self.assertTrue(is_create_domain('/**/ CREATE /* asd */ Domain foo bar'))
-        self.assertTrue(is_create_domain('-- foo\n\n CREATE /* asd */ Domain foo bar'))
-
-        self.assertFalse(is_create_domain('Create Table foo bar'))
-
-        statement = "Create Domain foo /* asd */ varchar(10)"
-        iscd = is_create_domain(statement)
-        name = next(iscd).value
-        definition = statement[next(iscd).pos:]
-        self.assertEqual(name, 'foo')
-        self.assertEqual(definition, 'varchar(10)')
-
-        statement = "Create Domain `foo` /* asd */ varchar(10)"
-        iscd = is_create_domain(statement)
-        name = next(iscd).value
-        definition = statement[next(iscd).pos:]
-        self.assertEqual(name, '`foo`')
-        self.assertEqual(definition, 'varchar(10)')
-
-        statement = 'Create Domain "TABLE" /* asd */ varchar(10)'
-        iscd = is_create_domain(statement)
-        name = next(iscd).value
-        definition = statement[next(iscd).pos:]
-        self.assertEqual(name, '"TABLE"')
-        self.assertEqual(definition, 'varchar(10)')
-
-
-class TestIsCreateOrAlterTable(unittest.TestCase):
-    def test(self):
-        from metapensiero.sphinx.patchdb.contexts.sql import is_create_or_alter_table
-
-        self.assertTrue(is_create_or_alter_table('Create Table foo'))
-        self.assertTrue(is_create_or_alter_table('/**/ CREATE /* asd */ Table foo'))
-        self.assertTrue(is_create_or_alter_table('-- foo\n\n CREATE /* asd */ Table foo'))
-
-        self.assertFalse(is_create_or_alter_table('Create Domain foo bar'))
-
-        from metapensiero.sphinx.patchdb.contexts.sql import replace_fake_domains
-
-        statement = "create table foo (a /* an int */ integer_t, b /* a bool */ bool_t)"
-        domains = {'integer_t': 'INTEGER', 'bool_t': 'CHAR(1)'}
-        isct = is_create_or_alter_table(statement)
-        self.assertEqual(replace_fake_domains(statement, isct, domains),
-                         "create table foo (a /* an int */ INTEGER, b /* a bool */ CHAR(1))")
-
-        statement = 'create table foo (a INTEGER_T, b "Bool_T")'
-        domains = {'integer_t': 'INTEGER', 'bool_t': 'CHAR(1)'}
-        isct = is_create_or_alter_table(statement)
-        self.assertEqual(replace_fake_domains(statement, isct, domains),
-                         'create table foo (a INTEGER, b "Bool_T")')
-
-        statement = 'CREATE TABLE t (v0 value_t, v1 VALUE_T, v2 "VALUE_T", v3 `Value_T`)'
-        domains = {'value_t': 'X', '"VALUE_T"': 'Y', '`Value_T`': 'Z'}
-        isct = is_create_or_alter_table(statement)
-        self.assertEqual(replace_fake_domains(statement, isct, domains),
-                         'CREATE TABLE t (v0 X, v1 X, v2 Y, v3 Z)')
-
-        statement = 'ALTER TABLE test ADD another value_t NOT NULL'
-        domains = {'value_t': 'X'}
-        isct = is_create_or_alter_table(statement)
-        self.assertEqual(replace_fake_domains(statement, isct, domains),
-                         'ALTER TABLE test ADD another X NOT NULL')
-
-        statement = 'ALTER TABLE t CHANGE another another value_t NULL DEFAULT NULL'
-        domains = {'value_t': 'X'}
-        isct = is_create_or_alter_table(statement)
-        self.assertEqual(replace_fake_domains(statement, isct, domains),
-                         'ALTER TABLE t CHANGE another another X NULL DEFAULT NULL')
+
+def test_is_create_domain():
+    from metapensiero.sphinx.patchdb.contexts.sql import is_create_domain
+
+    assert is_create_domain('Create Domain foo bar')
+    assert is_create_domain('/**/ CREATE /* asd */ Domain foo bar')
+    assert is_create_domain('-- foo\n\n CREATE /* asd */ Domain foo bar')
+
+    assert not is_create_domain('Create Table foo bar')
+
+    statement = "Create Domain foo /* asd */ varchar(10)"
+    iscd = is_create_domain(statement)
+    name = next(iscd).value
+    definition = statement[next(iscd).pos:]
+    assert name == 'foo'
+    assert definition == 'varchar(10)'
+
+    statement = "Create Domain `foo` /* asd */ varchar(10)"
+    iscd = is_create_domain(statement)
+    name = next(iscd).value
+    definition = statement[next(iscd).pos:]
+    assert name == '`foo`'
+    assert definition == 'varchar(10)'
+
+    statement = 'Create Domain "TABLE" /* asd */ varchar(10)'
+    iscd = is_create_domain(statement)
+    name = next(iscd).value
+    definition = statement[next(iscd).pos:]
+    assert name == '"TABLE"'
+    assert definition == 'varchar(10)'
+
+
+def test_is_create_or_alter_table():
+    from metapensiero.sphinx.patchdb.contexts.sql import is_create_or_alter_table
+    from metapensiero.sphinx.patchdb.contexts.sql import replace_fake_domains
+
+    assert is_create_or_alter_table('Create Table foo')
+    assert is_create_or_alter_table('/**/ CREATE /* asd */ Table foo')
+    assert is_create_or_alter_table('-- foo\n\n CREATE /* asd */ Table foo')
+
+    assert not is_create_or_alter_table('Create Domain foo bar')
+
+    statement = "create table foo (a /* an int */ integer_t, b /* a bool */ bool_t)"
+    domains = {'integer_t': 'INTEGER', 'bool_t': 'CHAR(1)'}
+    isct = is_create_or_alter_table(statement)
+    assert (replace_fake_domains(statement, isct, domains)
+            == "create table foo (a /* an int */ INTEGER, b /* a bool */ CHAR(1))")
+
+    statement = 'create table foo (a INTEGER_T, b "Bool_T")'
+    domains = {'integer_t': 'INTEGER', 'bool_t': 'CHAR(1)'}
+    isct = is_create_or_alter_table(statement)
+    assert (replace_fake_domains(statement, isct, domains)
+            == 'create table foo (a INTEGER, b "Bool_T")')
+
+    statement = 'CREATE TABLE t (v0 value_t, v1 VALUE_T, v2 "VALUE_T", v3 `Value_T`)'
+    domains = {'value_t': 'X', '"VALUE_T"': 'Y', '`Value_T`': 'Z'}
+    isct = is_create_or_alter_table(statement)
+    assert (replace_fake_domains(statement, isct, domains)
+            == 'CREATE TABLE t (v0 X, v1 X, v2 Y, v3 Z)')
+
+    statement = 'ALTER TABLE test ADD another value_t NOT NULL'
+    domains = {'value_t': 'X'}
+    isct = is_create_or_alter_table(statement)
+    assert (replace_fake_domains(statement, isct, domains)
+            == 'ALTER TABLE test ADD another X NOT NULL')
+
+    statement = 'ALTER TABLE t CHANGE another another value_t NULL DEFAULT NULL'
+    domains = {'value_t': 'X'}
+    isct = is_create_or_alter_table(statement)
+    assert (replace_fake_domains(statement, isct, domains)
+            == 'ALTER TABLE t CHANGE another another X NULL DEFAULT NULL')
```

### Comparing `metapensiero.sphinx.patchdb-4.0.dev4/tests/test_modular.py` & `metapensiero.sphinx.patchdb-4.0.dev5/tests/test_modular.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev4/tests/test_patch.py` & `metapensiero.sphinx.patchdb-4.0.dev5/tests/test_patch.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 #
 
 import pytest
 import fixtures
 
 
 def test_patch():
-    from metapensiero.sphinx.patchdb.manager import patch_manager
+    from metapensiero.sphinx.patchdb.manager import PatchManager
     from metapensiero.sphinx.patchdb.patch import make_patch, parse_deps, DependencyError
 
-    pm = patch_manager(None)
+    pm = PatchManager()
     first = make_patch('first', 'script',
                        dict(revision=1, language='test',
                             depends='second',
                             preceeds='third'))
     pm['first'] = first
 
     # __str__
```

### Comparing `metapensiero.sphinx.patchdb-4.0.dev4/tests/test_python.py` & `metapensiero.sphinx.patchdb-4.0.dev5/tests/test_python.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev4/tests/test_revisions.py` & `metapensiero.sphinx.patchdb-4.0.dev5/tests/test_revisions.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev4/tests/test_sql.py` & `metapensiero.sphinx.patchdb-4.0.dev5/tests/test_sql.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev4/tests/test_sql_fb.py` & `metapensiero.sphinx.patchdb-4.0.dev5/tests/test_sql_fb.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev4/tests/test_sql_ms.py` & `metapensiero.sphinx.patchdb-4.0.dev5/tests/test_sql_ms.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev4/tests/test_sql_pg.py` & `metapensiero.sphinx.patchdb-4.0.dev5/tests/test_sql_pg.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,15 +185,15 @@
 
            alter table parents drop column children_count
         """
 
         def test_2(self):
             self.build({'test.txt': self.SECOND_REV})
             output = self.patchdb('--debug')
-            self.assertIn('Could not apply 2 scripts', output)
+            self.assertIn('could not apply 2 scripts', output.lower())
 
     class TestDependencyOnAnyRevision(TestCircularDependencyCase):
         SECOND_REV = """
         Second version
         ==============
 
         .. patchdb:script:: Parents table
```

### Comparing `metapensiero.sphinx.patchdb-4.0.dev4/tests/test_states.py` & `metapensiero.sphinx.patchdb-4.0.dev5/tests/test_states.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev4/tests/test_variables.py` & `metapensiero.sphinx.patchdb-4.0.dev5/tests/test_variables.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev4/PKG-INFO` & `metapensiero.sphinx.patchdb-4.0.dev5/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metapensiero.sphinx.patchdb
-Version: 4.0.dev4
+Version: 4.0.dev5
 Summary: Extract scripts from a reST document and apply them in order.
 License: GPL-3.0-or-later
 Author-email: Lele Gaifax <lele@metapensiero.it>
 Requires-Python: >=3.10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Framework :: Sphinx :: Extension
```

