# Comparing `tmp/entangled_cli-2.0.0b1.tar.gz` & `tmp/entangled_cli-2.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "entangled_cli-2.0.0b1.tar", max compression
+gzip compressed data, was "entangled_cli-2.0.0b2.tar", max compression
```

## Comparing `entangled_cli-2.0.0b1.tar` & `entangled_cli-2.0.0b2.tar`

### file list

```diff
@@ -1,34 +1,33 @@
--rw-r--r--   0        0        0    11357 2023-05-24 06:31:52.897137 entangled_cli-2.0.0b1/LICENSE
--rw-r--r--   0        0        0     3636 2023-05-24 06:31:52.897137 entangled_cli-2.0.0b1/README.md
--rw-r--r--   0        0        0        1 2023-05-24 06:31:52.897137 entangled_cli-2.0.0b1/entangled/__init__.py
--rw-r--r--   0        0        0     2306 2023-05-24 06:31:52.897137 entangled_cli-2.0.0b1/entangled/code_reader.py
--rw-r--r--   0        0        0      152 2023-05-24 06:31:52.897137 entangled_cli-2.0.0b1/entangled/commands/__init__.py
--rw-r--r--   0        0        0        0 2023-05-24 06:31:52.897137 entangled_cli-2.0.0b1/entangled/commands/init.py
--rw-r--r--   0        0        0     2003 2023-05-24 06:31:52.897137 entangled_cli-2.0.0b1/entangled/commands/stitch.py
--rw-r--r--   0        0        0     1184 2023-05-24 06:31:52.897137 entangled_cli-2.0.0b1/entangled/commands/sync.py
--rw-r--r--   0        0        0     1737 2023-05-24 06:31:52.897137 entangled_cli-2.0.0b1/entangled/commands/tangle.py
--rw-r--r--   0        0        0     1692 2023-05-24 06:31:52.897137 entangled_cli-2.0.0b1/entangled/commands/watch.py
--rw-r--r--   0        0        0     2586 2023-05-24 06:31:52.897137 entangled_cli-2.0.0b1/entangled/config/__init__.py
--rw-r--r--   0        0        0     1402 2023-05-24 06:31:52.897137 entangled_cli-2.0.0b1/entangled/config/language.py
--rw-r--r--   0        0        0      606 2023-05-24 06:31:52.897137 entangled_cli-2.0.0b1/entangled/config/version.py
--rw-r--r--   0        0        0     1775 2023-05-24 06:31:52.897137 entangled_cli-2.0.0b1/entangled/construct.py
--rw-r--r--   0        0        0        1 2023-05-24 06:31:52.897137 entangled_cli-2.0.0b1/entangled/data/defaults.toml
--rw-r--r--   0        0        0     3819 2023-05-24 06:31:52.897137 entangled_cli-2.0.0b1/entangled/document.py
--rw-r--r--   0        0        0        0 2023-05-24 06:31:52.897137 entangled_cli-2.0.0b1/entangled/errors/__init__.py
--rw-r--r--   0        0        0      561 2023-05-24 06:31:52.897137 entangled_cli-2.0.0b1/entangled/errors/internal.py
--rw-r--r--   0        0        0      736 2023-05-24 06:31:52.897137 entangled_cli-2.0.0b1/entangled/errors/user.py
--rw-r--r--   0        0        0     5189 2023-05-24 06:31:52.897137 entangled_cli-2.0.0b1/entangled/filedb.py
--rw-r--r--   0        0        0      652 2023-05-24 06:31:52.897137 entangled_cli-2.0.0b1/entangled/hooks/__init__.py
--rw-r--r--   0        0        0      653 2023-05-24 06:31:52.897137 entangled_cli-2.0.0b1/entangled/hooks/base.py
--rw-r--r--   0        0        0     1494 2023-05-24 06:31:52.901138 entangled_cli-2.0.0b1/entangled/hooks/build.py
--rw-r--r--   0        0        0     1744 2023-05-24 06:31:52.901138 entangled_cli-2.0.0b1/entangled/main.py
--rw-r--r--   0        0        0     4630 2023-05-24 06:31:52.901138 entangled_cli-2.0.0b1/entangled/markdown_reader.py
--rw-r--r--   0        0        0     5450 2023-05-24 06:31:52.901138 entangled_cli-2.0.0b1/entangled/parsing.py
--rw-r--r--   0        0        0     2449 2023-05-24 06:31:52.901138 entangled_cli-2.0.0b1/entangled/properties.py
--rw-r--r--   0        0        0        0 2023-05-24 06:31:52.901138 entangled_cli-2.0.0b1/entangled/py.typed
--rw-r--r--   0        0        0     1697 2023-05-24 06:31:52.901138 entangled_cli-2.0.0b1/entangled/tangle.py
--rw-r--r--   0        0        0     5470 2023-05-24 06:31:52.901138 entangled_cli-2.0.0b1/entangled/transaction.py
--rw-r--r--   0        0        0      834 2023-05-24 06:31:52.901138 entangled_cli-2.0.0b1/entangled/utility.py
--rw-r--r--   0        0        0       85 2023-05-24 06:31:52.901138 entangled_cli-2.0.0b1/entangled/version.py
--rw-r--r--   0        0        0     1169 2023-05-24 06:31:52.901138 entangled_cli-2.0.0b1/pyproject.toml
--rw-r--r--   0        0        0     4300 1970-01-01 00:00:00.000000 entangled_cli-2.0.0b1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-04 21:46:15.987765 entangled_cli-2.0.0b2/LICENSE
+-rw-r--r--   0        0        0    11707 2023-06-04 21:46:15.987765 entangled_cli-2.0.0b2/README.md
+-rw-r--r--   0        0        0        1 2023-06-04 21:46:15.987765 entangled_cli-2.0.0b2/entangled/__init__.py
+-rw-r--r--   0        0        0     2158 2023-06-04 21:46:15.987765 entangled_cli-2.0.0b2/entangled/code_reader.py
+-rw-r--r--   0        0        0      152 2023-06-04 21:46:15.987765 entangled_cli-2.0.0b2/entangled/commands/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-04 21:46:15.987765 entangled_cli-2.0.0b2/entangled/commands/init.py
+-rw-r--r--   0        0        0     1987 2023-06-04 21:46:15.987765 entangled_cli-2.0.0b2/entangled/commands/stitch.py
+-rw-r--r--   0        0        0     1184 2023-06-04 21:46:15.987765 entangled_cli-2.0.0b2/entangled/commands/sync.py
+-rw-r--r--   0        0        0     1809 2023-06-04 21:46:15.987765 entangled_cli-2.0.0b2/entangled/commands/tangle.py
+-rw-r--r--   0        0        0     1673 2023-06-04 21:46:15.987765 entangled_cli-2.0.0b2/entangled/commands/watch.py
+-rw-r--r--   0        0        0     3401 2023-06-04 21:46:15.987765 entangled_cli-2.0.0b2/entangled/config/__init__.py
+-rw-r--r--   0        0        0     1471 2023-06-04 21:46:15.987765 entangled_cli-2.0.0b2/entangled/config/language.py
+-rw-r--r--   0        0        0      606 2023-06-04 21:46:15.987765 entangled_cli-2.0.0b2/entangled/config/version.py
+-rw-r--r--   0        0        0     1769 2023-06-04 21:46:15.991765 entangled_cli-2.0.0b2/entangled/construct.py
+-rw-r--r--   0        0        0     2235 2023-06-04 21:46:15.991765 entangled_cli-2.0.0b2/entangled/document.py
+-rw-r--r--   0        0        0        0 2023-06-04 21:46:15.991765 entangled_cli-2.0.0b2/entangled/errors/__init__.py
+-rw-r--r--   0        0        0      574 2023-06-04 21:46:15.991765 entangled_cli-2.0.0b2/entangled/errors/internal.py
+-rw-r--r--   0        0        0      927 2023-06-04 21:46:15.991765 entangled_cli-2.0.0b2/entangled/errors/user.py
+-rw-r--r--   0        0        0     5189 2023-06-04 21:46:15.991765 entangled_cli-2.0.0b2/entangled/filedb.py
+-rw-r--r--   0        0        0      646 2023-06-04 21:46:15.991765 entangled_cli-2.0.0b2/entangled/hooks/__init__.py
+-rw-r--r--   0        0        0      637 2023-06-04 21:46:15.991765 entangled_cli-2.0.0b2/entangled/hooks/base.py
+-rw-r--r--   0        0        0     2325 2023-06-04 21:46:15.991765 entangled_cli-2.0.0b2/entangled/hooks/build.py
+-rw-r--r--   0        0        0     1954 2023-06-04 21:46:15.991765 entangled_cli-2.0.0b2/entangled/main.py
+-rw-r--r--   0        0        0     4724 2023-06-04 21:46:15.991765 entangled_cli-2.0.0b2/entangled/markdown_reader.py
+-rw-r--r--   0        0        0     5451 2023-06-04 21:46:15.991765 entangled_cli-2.0.0b2/entangled/parsing.py
+-rw-r--r--   0        0        0     2486 2023-06-04 21:46:15.991765 entangled_cli-2.0.0b2/entangled/properties.py
+-rw-r--r--   0        0        0        0 2023-06-04 21:46:15.991765 entangled_cli-2.0.0b2/entangled/py.typed
+-rw-r--r--   0        0        0     3366 2023-06-04 21:46:15.991765 entangled_cli-2.0.0b2/entangled/tangle.py
+-rw-r--r--   0        0        0     5470 2023-06-04 21:46:15.991765 entangled_cli-2.0.0b2/entangled/transaction.py
+-rw-r--r--   0        0        0      832 2023-06-04 21:46:15.991765 entangled_cli-2.0.0b2/entangled/utility.py
+-rw-r--r--   0        0        0       85 2023-06-04 21:46:15.991765 entangled_cli-2.0.0b2/entangled/version.py
+-rw-r--r--   0        0        0     1197 2023-06-04 21:46:15.991765 entangled_cli-2.0.0b2/pyproject.toml
+-rw-r--r--   0        0        0    12449 1970-01-01 00:00:00.000000 entangled_cli-2.0.0b2/PKG-INFO
```

### Comparing `entangled_cli-2.0.0b1/LICENSE` & `entangled_cli-2.0.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `entangled_cli-2.0.0b1/entangled/code_reader.py` & `entangled_cli-2.0.0b2/entangled/code_reader.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,23 +5,14 @@
 import re
 
 from .document import ReferenceId, TextLocation, ReferenceMap
 from .errors.user import IndentationError
 
 
 @dataclass
-class StitchError(Exception):
-    path: Path
-    msg: str
-
-    def __str__(self):
-        return f"indentation error in `{self.path}`"
-
-
-@dataclass
 class Frame:
     ref: ReferenceId
     indent: str
     content: list[str] = field(default_factory=list)
 
 
 class CodeReader(mawk.RuleSet):
```

### Comparing `entangled_cli-2.0.0b1/entangled/commands/stitch.py` & `entangled_cli-2.0.0b2/entangled/commands/stitch.py`

 * *Files 7% similar despite different names*

```diff
@@ -52,10 +52,10 @@
                 logging.debug("reading `%s`", path)
                 t.db.update(path)
                 with open(path, "r") as f:
                     CodeReader(str(path), refs).run(f.read())
 
             for path in input_file_list:
                 t.write(path, stitch_markdown(refs, content[path]), [])
-                
+
     except UserError as e:
         logging.error(str(e))
```

### Comparing `entangled_cli-2.0.0b1/entangled/commands/sync.py` & `entangled_cli-2.0.0b2/entangled/commands/sync.py`

 * *Files identical despite different names*

### Comparing `entangled_cli-2.0.0b1/entangled/commands/tangle.py` & `entangled_cli-2.0.0b2/entangled/commands/tangle.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,16 +20,18 @@
     choices=[m.name.lower() for m in AnnotationMethod],
     help="annotation method",
 )
 @argh.arg("--force", help="force overwrite on conflict")
 @argh.arg("-s", "--show", help="only show, don't act")
 def tangle(*, annotate: Optional[str] = None, force: bool = False, show: bool = False):
     """Tangle codes from Markdown"""
-    if annotate is not None:
-        config.annotation = AnnotationMethod[annotate.upper()]
+    if annotate is None:
+        annotation_method = config.annotation
+    else:
+        annotation_method = AnnotationMethod[annotate.upper()]
 
     input_file_list = chain.from_iterable(map(Path(".").glob, config.watch_list))
     refs = ReferenceMap()
     hooks = get_hooks()
 
     if show:
         mode = TransactionMode.SHOW
@@ -43,16 +45,16 @@
             for path in input_file_list:
                 logging.debug("reading `%s`", path)
                 t.db.update(path)
                 with open(path, "r") as f:
                     MarkdownReader(str(path), refs, hooks).run(f.read())
 
             for tgt in refs.targets:
-                result, deps = tangle_ref(refs, tgt)
+                result, deps = tangle_ref(refs, tgt, annotation_method)
                 t.write(Path(tgt), result, list(map(Path, deps)))
             t.clear_orphans()
 
         for h in hooks:
             h.post_tangle(refs)
 
     except UserError as e:
-        logging.error(str(e))
+        logging.error(str(e))
```

### Comparing `entangled_cli-2.0.0b1/entangled/commands/watch.py` & `entangled_cli-2.0.0b2/entangled/commands/watch.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from typing import Optional
 from pathlib import Path
 from itertools import chain
-import logging
 from threading import Event
 
 from watchdog.observers import Observer
 from watchdog.events import FileSystemEventHandler, FileSystemEvent
 
 from .sync import sync
 from ..config import config
@@ -33,15 +32,15 @@
 def _watch(_stop_event: Optional[Event] = None):
     """Keep a loop running, watching for changes. This interface is separated
     from the CLI one, so that it can be tested using threading instead of
     subprocess."""
 
     def stop() -> bool:
         return _stop_event is not None and _stop_event.is_set()
-    
+
     sync()
 
     event_handler = EventHandler()
     observer = Observer()
     observer.schedule(event_handler, ".", recursive=True)
     observer.start()
```

### Comparing `entangled_cli-2.0.0b1/entangled/config/__init__.py` & `entangled_cli-2.0.0b2/entangled/config/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,20 +5,23 @@
 from __future__ import annotations
 
 from typing import Optional, ClassVar, TypeVar
 from enum import Enum
 from dataclasses import dataclass, field
 from copy import copy
 from pathlib import Path
+from contextlib import contextmanager
 
 from ..construct import construct
 from .version import Version
 from .language import Language, languages
 
+import threading
 import tomllib
+import logging
 
 
 class AnnotationMethod(Enum):
     """Annotation methods.
 
     - `STANDARD` is the default. Comments tell where a piece of code
        came from in enough detail to reconstruct the markdown if some
@@ -43,21 +46,22 @@
     end_ignore: str
 
 
 markers = Markers(
     r"^(?P<indent>\s*)```\s*{(?P<properties>[^{}]*)}\s*$",
     r"^(?P<indent>\s*)```\s*$",
     r"^\s*\~\~\~markdown\s*$",
-    r"^\s*\~\~\~\s*$"
+    r"^\s*\~\~\~\s*$",
 )
 
 
 @dataclass
-class Config:
-    """Main config class."""
+class Config(threading.local):
+    """Main config class. This class is made thread-local to make
+    it possible to test in parallel."""
 
     version: Version
     languages: list[Language] = field(default_factory=list)
     markers: Markers = field(default_factory=lambda: copy(markers))
     watch_list: list[str] = field(default_factory=lambda: ["**/*.md"])
     annotation_format: Optional[str] = None
     annotation: AnnotationMethod = AnnotationMethod.STANDARD
@@ -70,25 +74,49 @@
 
     def make_language_index(self):
         self.language_index = dict()
         for l in self.languages:
             for i in l.identifiers:
                 self.language_index[i] = l
 
-    def get_language(self, lang_name: str) -> Optional[Language]:
-        return self.language_index.get(lang_name, None)
-
 
 default = Config(Version.from_string("2.0"))
 
 
 def read_config():
     if not Path("./entangled.toml").exists():
         return default
-    with open(Path("./entangled.toml"), "rb") as f:
-        json = tomllib.load(f)
-    return construct(Config, json)
+    try:
+        with open(Path("./entangled.toml"), "rb") as f:
+            json = tomllib.load(f)
+        return construct(Config, json)
+    except ValueError as e:
+        logging.error("Could not read config: %s", e)
+        return default
+
+
+class ConfigWrapper:
+    def __init__(self, config):
+        self.config = config
+
+    def read(self):
+        self.config = read_config()
+
+    def __getattr__(self, attr):
+        return getattr(self.config, attr)
+
+    @contextmanager
+    def __call__(self, **kwargs):
+        backup = {k: getattr(self.config, k) for k in kwargs}
+        for k, v in kwargs.items():
+            setattr(self.config, k, v)
+        yield
+        for k in kwargs.keys():
+            setattr(self.config, k, backup[k])
+
+    def get_language(self, lang_name: str) -> Optional[Language]:
+        return self.config.language_index.get(lang_name, None)
 
 
-config = read_config()
+config = ConfigWrapper(read_config())
 """The `config.config` variable is changed when the `config` module is loaded.
 Config is read from `entangled.toml` file."""
```

### Comparing `entangled_cli-2.0.0b1/entangled/config/language.py` & `entangled_cli-2.0.0b2/entangled/config/language.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,22 +22,23 @@
     name: str
     identifiers: list[str]
     comment: Comment
     line_directive: Optional[str] = None
 
 
 languages = [
+    Language("Shell", ["sh", "bash", "fish", "zsh"], Comment("#")),
     Language("C", ["c", "cpp", "c++"], Comment("/*", "*/")),
     Language("Python", ["python"], Comment("#")),
     Language("Rust", ["rust"], Comment("//")),
     Language("Haskell", ["haskell"], Comment("--")),
     Language(
         "Lisp", ["scheme", "r5rs", "r6rs", "r7rs", "racket", "clojure"], Comment(";")
     ),
     Language("Julia", ["julia"], Comment("#")),
     Language("Java", ["java"], Comment("//")),
     Language("PureScritp", ["pure", "purs", "purescript"], Comment("--")),
     Language("CSS", ["css"], Comment("/*", "*/")),
     Language("Lua", ["lua"], Comment("--")),
     Language("Make", ["make", "makefile"], Comment("#")),
-    Language("Gnuplot", ["gnuplot"], Comment("#"))
+    Language("Gnuplot", ["gnuplot"], Comment("#")),
 ]
```

### Comparing `entangled_cli-2.0.0b1/entangled/config/version.py` & `entangled_cli-2.0.0b2/entangled/config/version.py`

 * *Files identical despite different names*

### Comparing `entangled_cli-2.0.0b1/entangled/construct.py` & `entangled_cli-2.0.0b2/entangled/construct.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 import typing
 import types
 
 from .parsing import Parser
 
 
 def isgeneric(annot):
-    return hasattr(annot, "__origin__") \
-        and hasattr(annot, "__args__")
+    return hasattr(annot, "__origin__") and hasattr(annot, "__args__")
 
 
 def construct(annot, json):
     """Construct an object from a given type from a JSON stream.
 
     The `annot` type should be one of: str, int, list[T], Optional[T],
     or a dataclass, and the JSON data should match exactly the given
@@ -28,25 +27,27 @@
         return json
     if isinstance(json, str) and isinstance(annot, Parser):
         result, _ = annot.read(json)
         return result
     if isgeneric(annot) and typing.get_origin(annot) is list:
         assert isinstance(json, list)
         return [construct(typing.get_args(annot)[0], item) for item in json]
-    if isgeneric(annot) and typing.get_origin(annot) is Union \
-        and typing.get_args(annot)[1] is types.NoneType:
+    if (
+        isgeneric(annot)
+        and typing.get_origin(annot) is Union
+        and typing.get_args(annot)[1] is types.NoneType
+    ):
         if json is None:
             return None
         else:
             return construct(typing.get_args(annot)[0], json)
     if is_dataclass(annot):
         assert isinstance(json, dict)
         arg_annot = typing.get_type_hints(annot)
         # assert all(k in json for k in arg_annot)
-        args = { k: construct(arg_annot[k], json[k])
-                 for k in json }
+        args = {k: construct(arg_annot[k], json[k]) for k in json}
         return annot(**args)
     if isinstance(json, str) and issubclass(annot, Enum):
         options = {opt.name.lower(): opt for opt in annot}
         assert json.lower() in options
         return options[json.lower()]
-    raise ValueError(f"Couldn't construct {annot} from {repr(json)}")
+    raise ValueError(f"Couldn't construct {annot} from {repr(json)}")
```

### Comparing `entangled_cli-2.0.0b1/entangled/document.py` & `entangled_cli-2.0.0b2/entangled/tangle.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,127 +1,128 @@
-from typing import Union, Iterable, Any
+from typing import Optional, TypeVar, Generic, Union
 from dataclasses import dataclass, field
-from collections import defaultdict
-from functools import singledispatchmethod
-from itertools import chain
+from textwrap import indent
+from contextlib import contextmanager
+from copy import copy
+
+import re
+import mawk
+
+from .document import (
+    ReferenceMap,
+    AnnotationMethod,
+    TextLocation,
+    ReferenceId,
+    CodeBlock,
+)
+from .errors.user import CyclicReference, MissingReference
+from .config import config
 
-from .config import Language, AnnotationMethod, config
-from .properties import Property, get_attribute
-from .errors.internal import InternalError
 
-
-def length(iter: Iterable[Any]) -> int:
-    return sum(1 for _ in iter)
-
-
-@dataclass
-class ReferenceId:
-    name: str
-    file: str
-    ref_count: int
-
-    def __hash__(self):
-        return hash((self.name, self.file, self.ref_count))
+T = TypeVar("T")
 
 
 @dataclass
-class PlainText:
-    content: str
+class Visitor(Generic[T]):
+    _visited: dict[T, int] = field(default_factory=dict)
 
+    def in_order(self) -> list[T]:
+        return [k for k, v in sorted(self._visited.items(), key=lambda kv: kv[1])]
 
-Content = Union[PlainText, ReferenceId]
+    @contextmanager
+    def visit(self, x: T):
+        if x in self._visited:
+            raise CyclicReference(str(x), list(map(str, self.in_order())))
+        self._visited[x] = len(self._visited)
+        yield
+        del self._visited[x]
 
 
 @dataclass
-class TextLocation:
-    filename: str
-    line_number: int = 0
+class Tangler(mawk.RuleSet):
+    refs: ReferenceMap
+    ref: ReferenceId
+    init: bool
+    visited: Visitor[str]
+    deps: set[str] = field(init=False)
+    cb: CodeBlock = field(init=False)
+    location: TextLocation = field(init=False)
+
+    def __post_init__(self):
+        self.cb = self.refs[self.ref]
+        self.location = copy(self.cb.origin)
+        self.deps = set((self.cb.origin.filename,))
+
+    @mawk.always
+    def lineno(self, _):
+        self.location.line_number += 1
+
+    @mawk.on_match(r"^(?P<indent>\s*)<<(?P<refname>[\w-]+)>>\s*$")
+    def on_noweb(self, m: re.Match):
+        try:
+            result, deps = tangle_ref(self.refs, m["refname"], type(self), self.visited)
 
-    def __str__(self):
-        return f"{self.filename}:{self.line_number}"
+        except KeyError:
+            raise MissingReference(m["refname"], self.location)
 
+        self.deps.update(deps)
+        return [indent(result, m["indent"])]
 
-@dataclass
-class CodeBlock:
-    language: Language
-    properties: list[Property]
-    indent: str
-    source: str
-    origin: TextLocation
+    def run(self):
+        return super().run(self.cb.source)
 
 
 @dataclass
-class ReferenceMap:
-    map: dict[ReferenceId, CodeBlock] = field(default_factory=dict)
-    index: defaultdict[str, list[ReferenceId]] = field(
-        default_factory=lambda: defaultdict(list)
-    )
-    targets: set[str] = field(default_factory=set)
-
-    def names(self) -> Iterable[str]:
-        return self.index.keys()
-
-    def by_name(self, n: str) -> Iterable[CodeBlock]:
-        return (self.map[r] for r in self.index[n])
-
-    def new_id(self, filename: str, name: str) -> ReferenceId:
-        c = length(filter(lambda r: r.file == filename, self.index[name]))
-        return ReferenceId(name, filename, c)
-
-    def __setitem__(self, key: ReferenceId, value: CodeBlock):
-        if key in self.map:
-            raise InternalError("Duplicate key in ReferenceMap", [key])
-        self.map[key] = value
-        self.index[key.name].append(key)
-
-    @singledispatchmethod
-    def __getitem__(self, key):
-        raise NotImplementedError(f"Invalid key: {type(key)}")
-
-    @__getitem__.register
-    def _(self, key: ReferenceId) -> CodeBlock:
-        return self.map[key]
-
-    @__getitem__.register
-    def _(self, key: str) -> Iterable[CodeBlock]:
-        return self.by_name(key)
-
-    @singledispatchmethod
-    def get_decorated(self, ref):
-        raise NotImplementedError(f"Invalid key: {type(ref)}")
-
-    @get_decorated.register
-    def _(self, ref: ReferenceId, annotation=config.annotation) -> list[str]:
-        init = ref == self.index[ref.name][0]
-        count = "init" if init else str(ref.ref_count)
-        cb = self.map[ref]
-        close_comment = (
-            "" if cb.language.comment.close is None else f" {cb.language.comment.close}"
-        )
-        start = (
-            f"{cb.language.comment.open} ~/~ begin <<{ref.file}#{ref.name}>>[{count}]"
-        )
-        end = f"{cb.language.comment.open} ~/~ end{close_comment}"
-        match annotation:
-            case AnnotationMethod.STANDARD:
-                return [start + close_comment, cb.source, end]
-            case AnnotationMethod.NAKED:
-                return [cb.source]
-            case AnnotationMethod.SUPPLEMENTED:
-                if config.annotation_format is None:
-                    return [start + close_comment, cb.source, end]
-
-                supplement = config.annotation_format.format(
-                    file=cb.origin.filename, linenumber=cb.origin.line_number
-                )
-                return [
-                    start + " " + supplement + close_comment,
-                    cb.source,
-                    end,
-                ]
-        raise InternalError("End of exhaustive match reached")
-    
-    @get_decorated.register
-    def _(self, ref_name: str, annotation=config.annotation) -> Iterable[str]:
-        return chain.from_iterable(
-            self.get_decorated(ref, annotation) for ref in self.index[ref_name]
+class AnnotatedTangler(Tangler):
+    close_comment: str = field(init=False)
+
+    def __post_init__(self):
+        super().__post_init__()
+        self.close_comment = (
+            ""
+            if self.cb.language.comment.close is None
+            else f" {self.cb.language.comment.close}"
         )
+
+    def on_begin(self):
+        count = "init" if self.init else str(self.ref.ref_count)
+        return [
+            f"{self.cb.language.comment.open} ~/~ begin <<{self.ref.file}#{self.ref.name}>>[{count}]{self.close_comment}"
+        ]
+
+    def on_eof(self):
+        return [f"{self.cb.language.comment.open} ~/~ end{self.close_comment}"]
+
+
+tanglers = {
+    AnnotationMethod.NAKED: Tangler,
+    AnnotationMethod.STANDARD: AnnotatedTangler,
+    AnnotationMethod.SUPPLEMENTED: AnnotatedTangler,
+}
+
+
+def tangle_ref(
+    refs: ReferenceMap,
+    ref_name: str,
+    annotation: Union[type[Tangler], AnnotationMethod] = config.annotation,
+    _visited: Optional[Visitor[str]] = None,
+) -> tuple[str, set[str]]:
+    if ref_name not in refs:
+        raise KeyError(ref_name)
+    v = _visited or Visitor()
+
+    if isinstance(annotation, AnnotationMethod):
+        tangler = tanglers[annotation]
+    else:
+        tangler = annotation
+
+    with v.visit(ref_name):
+        init = True
+        result = []
+        deps = set()
+        for ref in refs.index[ref_name]:
+            t = tangler(refs, ref, init, v)
+            result.append(t.run())
+            deps.update(t.deps)
+            init = False
+
+    return "\n".join(result), deps
```

### Comparing `entangled_cli-2.0.0b1/entangled/errors/internal.py` & `entangled_cli-2.0.0b2/entangled/errors/internal.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,9 +12,11 @@
     def __str__(self):
         return f"Internal error: {self.msg}"
 
 
 def bug_contact():
     logging.error(
         "This error is due to an internal bug in Entangled. Please file an "
-        "issue including the above stack trace " "and example content to "
-        "reproduce the exception at https://github.com/entangled/entangled.py/.")
+        "issue including the above stack trace "
+        "and example content to "
+        "reproduce the exception at https://github.com/entangled/entangled.py/."
+    )
```

### Comparing `entangled_cli-2.0.0b1/entangled/errors/user.py` & `entangled_cli-2.0.0b2/entangled/errors/user.py`

 * *Files 22% similar despite different names*

```diff
@@ -31,7 +31,15 @@
     ref_name: str
     cycle: list[str]
 
     def __str__(self):
         cycle_str = " -> ".join(self.cycle)
         return f"Cyclic reference in <<{self.ref_name}>>: {cycle_str}"
 
+
+@dataclass
+class MissingReference(UserError):
+    ref_name: str
+    location: TextLocation
+
+    def __str__(self):
+        return f"Missing reference `{self.ref_name}` at `{self.location}`"
```

### Comparing `entangled_cli-2.0.0b1/entangled/filedb.py` & `entangled_cli-2.0.0b2/entangled/filedb.py`

 * *Files identical despite different names*

### Comparing `entangled_cli-2.0.0b1/entangled/hooks/__init__.py` & `entangled_cli-2.0.0b2/entangled/hooks/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import logging
 from .base import HookBase
 from .build import BuildHook, PrerequisitesFailed
 from ..config import config
 
 
-hooks: dict[str, type[HookBase]] = {
-    "build": BuildHook
-}
+hooks: dict[str, type[HookBase]] = {"build": BuildHook}
 
 
 def get_hooks() -> list[HookBase]:
     active_hooks = []
     for h in config.hooks:
         if h in hooks:
             try:
```

### Comparing `entangled_cli-2.0.0b1/entangled/hooks/base.py` & `entangled_cli-2.0.0b2/entangled/hooks/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 
 @dataclass
 class PrerequisitesFailed(Exception):
     msg: str
 
     def __str__(self):
         return self.msg
-    
+
 
 class HookBase:
     @staticmethod
     def check_prerequisites():
         """When prerequisites aren't met, raise PrerequisitesFailed."""
         return
-    
+
     def condition(self, props: list[Property]):
         raise NotImplementedError()
-    
+
     def on_read(self, refs: ReferenceId, code: CodeBlock):
         raise NotImplementedError()
-    
+
     def post_tangle(self, refs: ReferenceMap):
         pass
```

### Comparing `entangled_cli-2.0.0b1/entangled/main.py` & `entangled_cli-2.0.0b2/entangled/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -50,16 +50,24 @@
     import argparse
 
     try:
         parser = argparse.ArgumentParser()
         parser.add_argument(
             "-d", "--debug", action="store_true", help="enable debug messages"
         )
+        parser.add_argument(
+            "-v", "--version", action="store_true", help="show version number"
+        )
         argh.add_commands(parser, [tangle, stitch, sync, watch])
         args = parser.parse_args()
+
+        if args.version:
+            print(f"Entangled {__version__}")
+            sys.exit(0)
+
         configure(args.debug)
         argh.dispatch(parser)
     except KeyboardInterrupt:
         logging.info("Goodbye")
         sys.exit(0)
     except UserError as e:
         logging.info(str(e))
@@ -67,9 +75,8 @@
     except Exception as e:
         logging.error(str(e))
         bug_contact(e)
         sys.exit(1)
 
 
 if __name__ == "__main__":
-        cli()
-
+    cli()
```

### Comparing `entangled_cli-2.0.0b1/entangled/markdown_reader.py` & `entangled_cli-2.0.0b2/entangled/markdown_reader.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,24 +7,29 @@
 import logging
 
 from .config import config
 from .utility import first
 from .document import TextLocation, CodeBlock, ReferenceMap, Content, PlainText
 from .properties import read_properties, get_attribute, get_classes, get_id
 from .hooks.base import HookBase
-from .errors.user import ParseError
+from .errors.user import ParseError, IndentationError
 from . import parsing
 
 
 class MarkdownReader(mawk.RuleSet):
     """Reads a Markdown file, and splits it up into code blocks and other
     content. The contents of the code blocks get stored in `reference_map`.
     """
 
-    def __init__(self, filename: str, refs: Optional[ReferenceMap] = None, hooks: Optional[list[HookBase]] = None):
+    def __init__(
+        self,
+        filename: str,
+        refs: Optional[ReferenceMap] = None,
+        hooks: Optional[list[HookBase]] = None,
+    ):
         self.location = TextLocation(filename)
         self.reference_map = refs or ReferenceMap()
         self.content: list[Content] = []
         self.inside_codeblock: bool = False
         self.current_content: list[str] = []
         self.ignore = False
         self.hooks = hooks or []
@@ -38,15 +43,14 @@
         self.location.line_number += 1
 
     @mawk.on_match(config.markers.begin_ignore)
     def on_begin_ignore(self, _):
         self.ignore = True
         logging.debug("ignoring markdown block %s", self.location)
 
-
     @mawk.on_match(config.markers.end_ignore)
     def on_end_ignore(self, _):
         self.ignore = False
         logging.debug("end of ignore")
 
     @mawk.on_match(config.markers.open)
     def on_open_codeblock(self, m: re.Match) -> Optional[list[str]]:
@@ -68,15 +72,15 @@
 
     @mawk.on_match(config.markers.close)
     def on_close_codeblock(self, m: re.Match):
         if self.ignore:
             return
         if not self.inside_codeblock:
             return
-        
+
         if len(m["indent"]) < len(self.current_codeblock_indent):
             raise IndentationError(self.location)
 
         if m["indent"] != self.current_codeblock_indent:
             return  # treat this as code-block content
 
         # add block to reference-map
@@ -92,28 +96,31 @@
             ref = self.reference_map.new_id(
                 self.current_codeblock_location.filename, ref_name
             )
             code = CodeBlock(
                 language,
                 self.current_codeblock_properties,
                 self.current_codeblock_indent,
-                "\n".join(line.removeprefix(self.current_codeblock_indent) for line in self.current_content),
+                "\n".join(
+                    line.removeprefix(self.current_codeblock_indent)
+                    for line in self.current_content
+                ),
                 self.current_codeblock_location,
             )
             logging.debug(repr(code))
             self.reference_map[ref] = code
             if target_file is not None:
                 self.reference_map.targets.add(target_file)
             self.content.append(ref)
             self.current_content = []
 
             for h in self.hooks:
                 if h.condition(self.current_codeblock_properties):
                     h.on_read(ref, code)
-            
+
         self.current_content.append(m[0])
         self.inside_codeblock = False
         return []
 
     @mawk.always
     def add_line(self, line: str):
         self.current_content.append(line)
```

### Comparing `entangled_cli-2.0.0b1/entangled/parsing.py` & `entangled_cli-2.0.0b2/entangled/parsing.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,14 +67,15 @@
     @property
     def expected(self):
         return " | ".join(str(f) for f in self.failures)
 
 
 class Parser(Generic[T]):
     """Base class for parsers."""
+
     def read(self, inp: str) -> tuple[T, str]:
         """Read a string and return an object the remainder of the string."""
         raise NotImplementedError()
 
     def __rshift__(self, f: Callable[[T], Parser[U]]) -> Parser[U]:
         return bind(self, f)
```

### Comparing `entangled_cli-2.0.0b1/entangled/properties.py` & `entangled_cli-2.0.0b2/entangled/properties.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,24 @@
 
 from __future__ import annotations
 
 from typing import Optional, Union, ClassVar, Iterable
 from dataclasses import dataclass
 import re
 
-from .parsing import Parser, many, choice, tokenize, matching, Parsable, starmap, Failure
+from .parsing import (
+    Parser,
+    many,
+    choice,
+    tokenize,
+    matching,
+    Parsable,
+    starmap,
+    Failure,
+)
 
 
 @dataclass
 class Id(Parsable):
     value: str
     _pattern: ClassVar[Parser] = matching(r"#([a-zA-Z]\S*)")
```

### Comparing `entangled_cli-2.0.0b1/entangled/tangle.py` & `entangled_cli-2.0.0b2/entangled/document.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,59 +1,89 @@
-from typing import Optional, TypeVar, Generic
+from typing import Union, Iterable, Any
 from dataclasses import dataclass, field
-from textwrap import indent
-from contextlib import contextmanager
+from collections import defaultdict
+from functools import singledispatchmethod
+from itertools import chain
 
-import re
-import mawk
+from .config import Language, AnnotationMethod, config
+from .properties import Property, get_attribute
+from .errors.internal import InternalError
 
-from .document import ReferenceMap, AnnotationMethod
-from .errors.user import CyclicReference
-from .config import config
 
+def length(iter: Iterable[Any]) -> int:
+    return sum(1 for _ in iter)
 
-T = TypeVar("T")
+
+@dataclass
+class ReferenceId:
+    name: str
+    file: str
+    ref_count: int
+
+    def __hash__(self):
+        return hash((self.name, self.file, self.ref_count))
+
+
+@dataclass
+class PlainText:
+    content: str
+
+
+Content = Union[PlainText, ReferenceId]
 
 
 @dataclass
-class Visitor(Generic[T]):
-    _visited: dict[T, int] = field(default_factory=dict)
+class TextLocation:
+    filename: str
+    line_number: int = 0
 
-    def in_order(self) -> list[T]:
-        return [k for k, v in sorted(self._visited.items(), key=lambda kv: kv[1])]
-    
-    @contextmanager
-    def visit(self, x: T):
-        if x in self._visited:
-            raise CyclicReference(str(x), list(map(str, self.in_order())))
-        self._visited[x] = len(self._visited)
-        yield
-        del self._visited[x]
+    def __str__(self):
+        return f"{self.filename}:{self.line_number}"
 
 
 @dataclass
-class Tangler(mawk.RuleSet):
-    reference_map: ReferenceMap
-    visited: Visitor[str]
-    deps: set[str]
-    annotation: AnnotationMethod
-
-    @mawk.on_match(r"^(?P<indent>\s*)<<(?P<refname>[\w-]+)>>\s*$")
-    def on_noweb(self, m: re.Match):
-        result, deps = tangle_ref(self.reference_map, m["refname"], self.annotation, self.visited)
-        self.deps.update(deps)
-        return [indent(result, m["indent"])]
-
-
-def tangle_ref(
-    refs: ReferenceMap, ref_name: str, 
-    annotation: AnnotationMethod = config.annotation,
-    _visited: Optional[Visitor[str]] = None
-) -> tuple[str, set[str]]:
-    v = _visited or Visitor()
-    with v.visit(ref_name):
-        deps = set(cb.origin.filename for cb in refs.by_name(ref_name))
-        source = "\n".join(refs.get_decorated(ref_name, annotation))
-        t = Tangler(refs, v, deps, annotation)
-        result = t.run(source)
-    return result, deps
+class CodeBlock:
+    language: Language
+    properties: list[Property]
+    indent: str
+    source: str
+    origin: TextLocation
 
+
+@dataclass
+class ReferenceMap:
+    map: dict[ReferenceId, CodeBlock] = field(default_factory=dict)
+    index: defaultdict[str, list[ReferenceId]] = field(
+        default_factory=lambda: defaultdict(list)
+    )
+    targets: set[str] = field(default_factory=set)
+
+    def names(self) -> Iterable[str]:
+        return self.index.keys()
+
+    def by_name(self, n: str) -> Iterable[CodeBlock]:
+        return (self.map[r] for r in self.index[n])
+
+    def new_id(self, filename: str, name: str) -> ReferenceId:
+        c = length(filter(lambda r: r.file == filename, self.index[name]))
+        return ReferenceId(name, filename, c)
+
+    def __setitem__(self, key: ReferenceId, value: CodeBlock):
+        if key in self.map:
+            raise InternalError("Duplicate key in ReferenceMap", [key])
+        self.map[key] = value
+        self.index[key.name].append(key)
+
+    def __contains__(self, key: str) -> bool:
+        return key in self.index
+
+    @singledispatchmethod
+    def __getitem__(self, key):
+        raise NotImplementedError(f"Invalid key: {type(key)}")
+
+    @__getitem__.register
+    def _(self, key: ReferenceId) -> CodeBlock:
+        return self.map[key]
+
+    @__getitem__.register
+    def _(self, key: str) -> Iterable[CodeBlock]:
+        return self.by_name(key)
```

### Comparing `entangled_cli-2.0.0b1/entangled/transaction.py` & `entangled_cli-2.0.0b2/entangled/transaction.py`

 * *Files identical despite different names*

### Comparing `entangled_cli-2.0.0b1/entangled/utility.py` & `entangled_cli-2.0.0b2/entangled/utility.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,9 +36,7 @@
 
 
 def cat_maybes(it: Iterable[Optional[T]]) -> Iterable[T]:
     def pred(x: Optional[T]) -> TypeGuard[T]:
         return x is not None
 
     return filter(pred, it)
-
-
```

### Comparing `entangled_cli-2.0.0b1/pyproject.toml` & `entangled_cli-2.0.0b2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,41 +1,40 @@
 [tool.poetry]
 name = "entangled-cli"
-version = "2.0.0-beta-1"
+version = "2.0.0-beta-2"
 description = "Literate Programming toolbox"
 repository = "https://github.com/entangled/entangled.py"
 homepage = "https://entangled.github.io/"
 authors = ["Johan Hidding <j.hidding@esciencecenter.nl>"]
 license = "Apache 2"
 readme = "README.md"
 packages = [
     { include = "entangled" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.11"          # we need tomllib support
-mawk = "^0.1.3"           # use mawk as line parsing engine
+mawk = "^0.1.4"           # use mawk as line parsing engine
 watchdog = "^3.0.0"       # file watching
 filelock = "^3.12.0"      # file lock for json db
 argh = "^0.28.1"
-
+rich = { version = "^13.3.5", optional = true }
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 mypy = "^1.3.0"
 black = "^23.3.0"
 pytest-cov = "^4.0.0"
 mkdocs = "^1.4.3"
 mkdocs-material = "^9.1.13"
 mkdocstrings = {extras = ["python"], version = "^0.21.2"}
 twine = "^4.0.2"
 
-
-[tool.poetry.group.rich.dependencies]
-rich = "^13.3.5"
+[tool.poetry.extras]
+rich = ["rich"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 testpaths = [
```

