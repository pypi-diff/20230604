# Comparing `tmp/mathbib-0.6.3.tar.gz` & `tmp/mathbib-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathbib-0.6.3.tar", max compression
+gzip compressed data, was "mathbib-0.7.0.tar", max compression
```

## Comparing `mathbib-0.6.3.tar` & `mathbib-0.7.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1070 2023-05-29 16:29:17.682650 mathbib-0.6.3/LICENSE
--rw-r--r--   0        0        0     5351 2023-05-29 16:41:55.640378 mathbib-0.6.3/README.md
--rw-r--r--   0        0        0      143 2023-05-29 16:27:47.709639 mathbib-0.6.3/mathbib/__init__.py
--rw-r--r--   0        0        0       63 2023-05-10 21:47:55.276481 mathbib-0.6.3/mathbib/__main__.py
--rw-r--r--   0        0        0     1402 2023-05-28 11:08:27.988644 mathbib-0.6.3/mathbib/bibtex.py
--rw-r--r--   0        0        0     2831 2023-05-28 15:54:03.882001 mathbib-0.6.3/mathbib/citegen.py
--rw-r--r--   0        0        0     9907 2023-06-04 06:38:05.985770 mathbib-0.6.3/mathbib/command.py
--rw-r--r--   0        0        0     2841 2023-05-28 16:33:13.843882 mathbib-0.6.3/mathbib/partition.py
--rw-r--r--   0        0        0     9459 2023-06-04 06:39:11.761721 mathbib-0.6.3/mathbib/record.py
--rw-r--r--   0        0        0     5697 2023-06-04 06:38:46.252732 mathbib-0.6.3/mathbib/remote/__init__.py
--rw-r--r--   0        0        0     3088 2023-05-28 12:38:27.635690 mathbib-0.6.3/mathbib/remote/arxiv.py
--rw-r--r--   0        0        0      923 2023-05-27 20:04:18.325197 mathbib-0.6.3/mathbib/remote/doi.py
--rw-r--r--   0        0        0      855 2023-05-28 09:33:03.953274 mathbib-0.6.3/mathbib/remote/error.py
--rw-r--r--   0        0        0     1475 2023-05-27 20:04:18.354984 mathbib-0.6.3/mathbib/remote/isbn.py
--rw-r--r--   0        0        0     1194 2023-05-27 18:35:57.528452 mathbib-0.6.3/mathbib/remote/ol.py
--rw-r--r--   0        0        0     4260 2023-06-04 06:31:57.308890 mathbib-0.6.3/mathbib/remote/utils.py
--rw-r--r--   0        0        0      597 2023-05-25 12:11:18.575783 mathbib-0.6.3/mathbib/remote/zbl.py
--rw-r--r--   0        0        0     1816 2023-05-28 12:19:04.718450 mathbib-0.6.3/mathbib/remote/zbmath.py
--rw-r--r--   0        0        0     6435 2023-06-04 06:38:50.839466 mathbib-0.6.3/mathbib/request.py
--rw-r--r--   0        0        0        0 2023-05-25 15:24:07.234292 mathbib-0.6.3/mathbib/resources/__init__.py
--rw-r--r--   0        0        0   270281 2023-05-30 19:36:41.814752 mathbib-0.6.3/mathbib/resources/journal_abbrevs.json
--rw-r--r--   0        0        0     2785 2023-06-03 20:06:26.993600 mathbib-0.6.3/mathbib/session.py
--rw-r--r--   0        0        0      705 2023-05-25 11:53:39.451875 mathbib-0.6.3/mathbib/term.py
--rw-r--r--   0        0        0      953 2023-06-04 06:39:22.667000 mathbib-0.6.3/pyproject.toml
--rw-r--r--   0        0        0     6240 1970-01-01 00:00:00.000000 mathbib-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-29 16:29:17.682650 mathbib-0.7.0/LICENSE
+-rw-r--r--   0        0        0     5341 2023-06-04 07:15:23.414124 mathbib-0.7.0/README.md
+-rw-r--r--   0        0        0      143 2023-05-29 16:27:47.709639 mathbib-0.7.0/mathbib/__init__.py
+-rw-r--r--   0        0        0       63 2023-05-10 21:47:55.276481 mathbib-0.7.0/mathbib/__main__.py
+-rw-r--r--   0        0        0     1402 2023-05-28 11:08:27.988644 mathbib-0.7.0/mathbib/bibtex.py
+-rw-r--r--   0        0        0     2831 2023-05-28 15:54:03.882001 mathbib-0.7.0/mathbib/citegen.py
+-rw-r--r--   0        0        0    10823 2023-06-04 07:21:28.332360 mathbib-0.7.0/mathbib/command.py
+-rw-r--r--   0        0        0     2841 2023-05-28 16:33:13.843882 mathbib-0.7.0/mathbib/partition.py
+-rw-r--r--   0        0        0     9441 2023-06-04 07:04:03.110810 mathbib-0.7.0/mathbib/record.py
+-rw-r--r--   0        0        0     5697 2023-06-04 06:38:46.252732 mathbib-0.7.0/mathbib/remote/__init__.py
+-rw-r--r--   0        0        0     3088 2023-05-28 12:38:27.635690 mathbib-0.7.0/mathbib/remote/arxiv.py
+-rw-r--r--   0        0        0      923 2023-05-27 20:04:18.325197 mathbib-0.7.0/mathbib/remote/doi.py
+-rw-r--r--   0        0        0      855 2023-05-28 09:33:03.953274 mathbib-0.7.0/mathbib/remote/error.py
+-rw-r--r--   0        0        0     1475 2023-05-27 20:04:18.354984 mathbib-0.7.0/mathbib/remote/isbn.py
+-rw-r--r--   0        0        0     1194 2023-05-27 18:35:57.528452 mathbib-0.7.0/mathbib/remote/ol.py
+-rw-r--r--   0        0        0     4260 2023-06-04 06:31:57.308890 mathbib-0.7.0/mathbib/remote/utils.py
+-rw-r--r--   0        0        0      597 2023-05-25 12:11:18.575783 mathbib-0.7.0/mathbib/remote/zbl.py
+-rw-r--r--   0        0        0     1816 2023-05-28 12:19:04.718450 mathbib-0.7.0/mathbib/remote/zbmath.py
+-rw-r--r--   0        0        0     6435 2023-06-04 06:38:50.839466 mathbib-0.7.0/mathbib/request.py
+-rw-r--r--   0        0        0        0 2023-05-25 15:24:07.234292 mathbib-0.7.0/mathbib/resources/__init__.py
+-rw-r--r--   0        0        0   270281 2023-05-30 19:36:41.814752 mathbib-0.7.0/mathbib/resources/journal_abbrevs.json
+-rw-r--r--   0        0        0     2785 2023-06-03 20:06:26.993600 mathbib-0.7.0/mathbib/session.py
+-rw-r--r--   0        0        0      705 2023-05-25 11:53:39.451875 mathbib-0.7.0/mathbib/term.py
+-rw-r--r--   0        0        0      953 2023-06-04 07:22:15.699317 mathbib-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     6230 1970-01-01 00:00:00.000000 mathbib-0.7.0/PKG-INFO
```

### Comparing `mathbib-0.6.3/LICENSE` & `mathbib-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mathbib-0.6.3/README.md` & `mathbib-0.7.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 ```sh
 pip install mathbib
 ```
 This installs the `mbib` command-line interface.
 The first useful subcommand is `mbib get`.
 For instance, running
 ```sh
-mbib get bibtex arxiv:1212.1873
+mbib get arxiv:1212.1873
 ```
 will retrieve the arxiv record at [https://arxiv.org/abs/1212.1873](https://arxiv.org/abs/1212.1873).
 If you check the output, you will notice that it actually returns
 ```bib
 @article{arxiv:1212.1873,
   author = {Hochman, Michael},
   eprint = {1337.28015},
@@ -28,15 +28,15 @@
   publisher = {Annals of Mathematics},
   title = {On self-similar sets with overlaps and inverse theorems for entropy},
   volume = {180},
   year = {2014}
 }
 ```
 This contains more information than what can be found on arxiv!
-In general `mbib` will attempt to search multiple locations for records to build the most updated citation possible.
+In general `mbib` will search multiple locations for records to build the most updated citation possible.
 
 Generating records from command-line arguments is nice, but a much more common use case is to generate records corresponding to a file.
 Suppose you have a file `doc.tex` containing the contents
 ```tex
 \documentclass{article}
 \usepackage{biblatex}
 \addbibresource{doc.bib}
@@ -49,15 +49,15 @@
 Simply run
 ```sh
 mbib generate doc.tex --out doc.bib
 ```
 to build the `.bib` file, and compile.
 
 Of course, it can be somewhat inconvenient to remember a large number of citation keys, especially ones that are designed to be machine-readable.
-An easy fix here is to create aliases.
+One solution is to create aliases.
 Let's define a few:
 ```sh
 mbib alias add Hoc2014 arxiv:1212.1873
 mbib alias add HocShm2012 zbl:1251.28008
 mbib alias add Shm2019 doi:10.4007/annals.2019.189.2.1
 ```
 We could now instead write our file  as
@@ -67,15 +67,15 @@
 \addbibresource{doc.bib}
 \begin{document}
 This document references an article \cite{Hoc2014}.
 It also contains more references \cite{HocShm2012, Shm2019}.
 \printbibliography
 \end{document}
 ```
-Remember to regenerate the `doc.bib` file with `mbib generate doc.tex > doc.bib` (the keys need to be updated), and the file will compile!
+Remember to regenerate the `doc.bib` file with `mbib generate doc.tex > doc.bib` (the citation keys need to be updated), and the file will compile!
 Aliases also work as command line arguments anywhere a `key:id` is expected.
 
 Suppose you have been working on the above TEX document for a while, and now you want to cite a specific theorem from the paper `Hoc2014`.
 Simply run
 ```sh
 mbib file open Hoc2014
 ```
@@ -109,15 +109,15 @@
 - `ol:` [Open Library](https://openlibrary.org/) resource identifiers.
 
 The requests to the various sources are cached in `$XDG_CACHE_HOME/mathbib`.
 In particular, the first search will be slow, but afterwards the request will resolve quickly.
 
 You can see all the information collected by MathBib by running, for instance,
 ```
-mbib get json arxiv:1212.1873
+mbib get -r json arxiv:1212.1873
 ```
 Note that MathBib also has an internal notion of record priority.
 Local modifications of records have the highest priority, and otherwise the priority is precisely as specified in the list above.
 For instance, if you run `mbib show arxiv:1212.1873`, your web browser will open a record on zbMATH.
 If you view the corresponding JSON record, you will see the `zbl:` entry has the highest priority.
```

### Comparing `mathbib-0.6.3/mathbib/bibtex.py` & `mathbib-0.7.0/mathbib/bibtex.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.6.3/mathbib/citegen.py` & `mathbib-0.7.0/mathbib/citegen.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.6.3/mathbib/command.py` & `mathbib-0.7.0/mathbib/command.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from __future__ import annotations
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
-    from typing import Iterable, Optional, Sequence
+    from typing import Iterable, Optional, Sequence, Literal
 
 from pathlib import Path
 from tomllib import loads, TOMLDecodeError
 
 import click
 
 from .citegen import generate_biblatex, get_citekeys_from_paths
 from .record import ArchiveRecord
 from .remote import AliasedKeyId, KeyIdError
 from .remote.error import RemoteAccessError
 from .session import CLISession
 from .term import TermWrite
 
 from tomli_w import dumps
+import json
 from xdg_base_dirs import xdg_data_home
 import shutil
 
 
 def keyid_callback(ctx, _, keyid_str: str) -> AliasedKeyId:
     """Construct the KeyId argument: first check if the keyid is aliased;
     otherwise, try to obtain it directly.
@@ -37,20 +38,39 @@
 def record_callback(ctx, param, keyid_str: str) -> ArchiveRecord:
     """Construct the KeyId argument: first check if the keyid is aliased;
     otherwise, try to obtain it directly.
     """
     return ArchiveRecord(keyid_callback(ctx, param, keyid_str), ctx.obj)
 
 
+def record_callback_multiple(
+    ctx, param, keyid_strs: tuple[str]
+) -> Iterable[ArchiveRecord]:
+    """Construct the KeyId argument: first check if the keyid is aliased;
+    otherwise, try to obtain it directly.
+    """
+    return (
+        ArchiveRecord(keyid_callback(ctx, param, keyid_str), ctx.obj)
+        for keyid_str in sorted(set(keyid_strs))
+    )
+
+
 keyid_argument = click.argument(
     "keyid", type=str, metavar="KEY:ID", callback=keyid_callback
 )
 record_argument = click.argument(
     "record", type=str, metavar="KEY:ID", callback=record_callback
 )
+record_argument_multiple = click.argument(
+    "records",
+    type=str,
+    nargs=-1,
+    metavar="[KEY:ID]...",
+    callback=record_callback_multiple,
+)
 texfile_argument = click.argument(
     "texfile",
     nargs=-1,
     type=click.Path(
         exists=True, file_okay=True, dir_okay=False, writable=True, path_type=Path
     ),
     metavar="TEXFILE",
@@ -113,35 +133,48 @@
     bibstr = generate_biblatex(ctx.obj, *texfile)
     if out is None:
         click.echo(bibstr, nl=False)
     else:
         out.write_text(bibstr)
 
 
-@cli.group(name="get", short_help="Retrieve records.")
-def get_group():
-    """Retrieve various record types associated with KEYI:ID records."""
-
-
-@get_group.command(name="json", short_help="Get record from KEY:ID.")
-@record_argument
-def json_cmd(record: ArchiveRecord):
-    """Generate a JSON record for KEY:ID."""
-    click.echo(record.as_json())
-
-
-@get_group.command(name="bibtex", short_help="Get bibtex from KEY:ID.")
-@record_argument
-def bibtex(record: ArchiveRecord):
-    """Generate a BibTeX record for KEY:ID."""
+@cli.command(name="get", short_help="Get record from KEY:ID.")
+@click.option(
+    "--record-type",
+    "-r",
+    "record_type",
+    type=click.Choice(["bibtex", "json"], case_sensitive=False),
+    default="bibtex",
+    help="Record type.",
+)
+@record_argument_multiple
+@click.pass_obj
+def get(
+    session: CLISession,
+    record_type: Literal["bibtex", "json"],
+    records: Iterable[ArchiveRecord],
+):
+    """Generate a record for multiple KEY:ID records. Specify the output type
+    using -r.
+
+    Input KEY:ID pairs are automatically sorted and duplicates are removed.
+
+    - BibTex records are returned as the string contents of a valid .bib file.
+    - JSON records are returned as list of dictionaries containing the associated
+    record objects.
+    """
     # TODO: option to pass multiple records
-    click.echo(record.cli_session.bibtex_handler.write_records((record,)), nl=False)
+    match record_type:
+        case "json":
+            click.echo(json.dumps([record.as_json_dict() for record in records]))
+        case "bibtex":
+            click.echo(session.bibtex_handler.write_records(records), nl=False)
 
 
-@get_group.command(name="key", short_help="Get highest priority key from KEY:ID.")
+@cli.command(name="key", short_help="Get highest priority key from KEY:ID.")
 @record_argument
 def key(record: ArchiveRecord):
     """Generate a BibTeX record for KEY:ID."""
     click.echo(record.priority_key())
 
 
 @cli.group(name="file", short_help="Access and manage files associated with records.")
```

### Comparing `mathbib-0.6.3/mathbib/partition.py` & `mathbib-0.7.0/mathbib/partition.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.6.3/mathbib/record.py` & `mathbib-0.7.0/mathbib/record.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,14 @@
         id: str
         record: dict
 
     RecordList = dict[str, RecordEntry]
 
 from itertools import chain
 import operator
-import json
 from functools import reduce
 
 from requests.exceptions import ConnectionError
 from xdg_base_dirs import xdg_data_home
 
 from .remote import KeyId, AliasedKeyId, get_remote_record, KeyIdError
 from .remote.error import NullRecordError, RemoteAccessError
@@ -143,16 +142,16 @@
         cls,
         keyid_str: str,
         session: CLISession,
         alias: Optional[str] = None,
     ):
         return cls(AliasedKeyId.from_str(keyid_str, alias=alias), session=session)
 
-    def as_json(self) -> str:
-        return json.dumps({str(k): v for k, v in self.record.resolve().items()})
+    def as_json_dict(self) -> dict:
+        return {str(k): v for k, v in self.record.resolve().items()}
 
     def as_joint_record(self) -> dict:
         records = list(reversed(self.record.resolve().values()))
         returned_record = reduce(operator.ior, records, {})
 
         # collect compound keys
         classifications = sorted(
```

### Comparing `mathbib-0.6.3/mathbib/remote/__init__.py` & `mathbib-0.7.0/mathbib/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.6.3/mathbib/remote/arxiv.py` & `mathbib-0.7.0/mathbib/remote/arxiv.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.6.3/mathbib/remote/doi.py` & `mathbib-0.7.0/mathbib/remote/doi.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.6.3/mathbib/remote/error.py` & `mathbib-0.7.0/mathbib/remote/error.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.6.3/mathbib/remote/isbn.py` & `mathbib-0.7.0/mathbib/remote/isbn.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.6.3/mathbib/remote/ol.py` & `mathbib-0.7.0/mathbib/remote/ol.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.6.3/mathbib/remote/utils.py` & `mathbib-0.7.0/mathbib/remote/utils.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.6.3/mathbib/remote/zbl.py` & `mathbib-0.7.0/mathbib/remote/zbl.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.6.3/mathbib/remote/zbmath.py` & `mathbib-0.7.0/mathbib/remote/zbmath.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.6.3/mathbib/request.py` & `mathbib-0.7.0/mathbib/request.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.6.3/mathbib/resources/journal_abbrevs.json` & `mathbib-0.7.0/mathbib/resources/journal_abbrevs.json`

 * *Files identical despite different names*

### Comparing `mathbib-0.6.3/mathbib/session.py` & `mathbib-0.7.0/mathbib/session.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.6.3/mathbib/term.py` & `mathbib-0.7.0/mathbib/term.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.6.3/pyproject.toml` & `mathbib-0.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "poetry.core.masonry.api"
 
 [virtualenv]
 in-project = true
 
 [tool.poetry]
 name = "mathbib"
-version = "0.6.3"
+version = "0.7.0"
 description = "A mathematics BibLaTeX bibliography manager."
 authors = ["Alex Rutar <alex@rutar.org>"]
 readme = "README.md"
 packages = [{include = "mathbib"}]
 license = "MIT"
 repository = "https://github.com/alexrutar/mathbib-py"
 include = ["mathbib/resources/journal_abbrevs.json"]
```

### Comparing `mathbib-0.6.3/PKG-INFO` & `mathbib-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathbib
-Version: 0.6.3
+Version: 0.7.0
 Summary: A mathematics BibLaTeX bibliography manager.
 Home-page: https://github.com/alexrutar/mathbib-py
 License: MIT
 Author: Alex Rutar
 Author-email: alex@rutar.org
 Requires-Python: >=3.11.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
@@ -32,15 +32,15 @@
 ```sh
 pip install mathbib
 ```
 This installs the `mbib` command-line interface.
 The first useful subcommand is `mbib get`.
 For instance, running
 ```sh
-mbib get bibtex arxiv:1212.1873
+mbib get arxiv:1212.1873
 ```
 will retrieve the arxiv record at [https://arxiv.org/abs/1212.1873](https://arxiv.org/abs/1212.1873).
 If you check the output, you will notice that it actually returns
 ```bib
 @article{arxiv:1212.1873,
   author = {Hochman, Michael},
   eprint = {1337.28015},
@@ -52,15 +52,15 @@
   publisher = {Annals of Mathematics},
   title = {On self-similar sets with overlaps and inverse theorems for entropy},
   volume = {180},
   year = {2014}
 }
 ```
 This contains more information than what can be found on arxiv!
-In general `mbib` will attempt to search multiple locations for records to build the most updated citation possible.
+In general `mbib` will search multiple locations for records to build the most updated citation possible.
 
 Generating records from command-line arguments is nice, but a much more common use case is to generate records corresponding to a file.
 Suppose you have a file `doc.tex` containing the contents
 ```tex
 \documentclass{article}
 \usepackage{biblatex}
 \addbibresource{doc.bib}
@@ -73,15 +73,15 @@
 Simply run
 ```sh
 mbib generate doc.tex --out doc.bib
 ```
 to build the `.bib` file, and compile.
 
 Of course, it can be somewhat inconvenient to remember a large number of citation keys, especially ones that are designed to be machine-readable.
-An easy fix here is to create aliases.
+One solution is to create aliases.
 Let's define a few:
 ```sh
 mbib alias add Hoc2014 arxiv:1212.1873
 mbib alias add HocShm2012 zbl:1251.28008
 mbib alias add Shm2019 doi:10.4007/annals.2019.189.2.1
 ```
 We could now instead write our file  as
@@ -91,15 +91,15 @@
 \addbibresource{doc.bib}
 \begin{document}
 This document references an article \cite{Hoc2014}.
 It also contains more references \cite{HocShm2012, Shm2019}.
 \printbibliography
 \end{document}
 ```
-Remember to regenerate the `doc.bib` file with `mbib generate doc.tex > doc.bib` (the keys need to be updated), and the file will compile!
+Remember to regenerate the `doc.bib` file with `mbib generate doc.tex > doc.bib` (the citation keys need to be updated), and the file will compile!
 Aliases also work as command line arguments anywhere a `key:id` is expected.
 
 Suppose you have been working on the above TEX document for a while, and now you want to cite a specific theorem from the paper `Hoc2014`.
 Simply run
 ```sh
 mbib file open Hoc2014
 ```
@@ -133,15 +133,15 @@
 - `ol:` [Open Library](https://openlibrary.org/) resource identifiers.
 
 The requests to the various sources are cached in `$XDG_CACHE_HOME/mathbib`.
 In particular, the first search will be slow, but afterwards the request will resolve quickly.
 
 You can see all the information collected by MathBib by running, for instance,
 ```
-mbib get json arxiv:1212.1873
+mbib get -r json arxiv:1212.1873
 ```
 Note that MathBib also has an internal notion of record priority.
 Local modifications of records have the highest priority, and otherwise the priority is precisely as specified in the list above.
 For instance, if you run `mbib show arxiv:1212.1873`, your web browser will open a record on zbMATH.
 If you view the corresponding JSON record, you will see the `zbl:` entry has the highest priority.
```

