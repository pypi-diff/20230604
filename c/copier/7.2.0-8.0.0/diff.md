# Comparing `tmp/copier-7.2.0.tar.gz` & `tmp/copier-8.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copier-7.2.0.tar", max compression
+gzip compressed data, was "copier-8.0.0.tar", max compression
```

## Comparing `copier-7.2.0.tar` & `copier-8.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1076 2023-04-19 17:40:07.270090 copier-7.2.0/LICENSE
--rw-r--r--   0        0        0     6143 2023-04-19 17:40:07.270090 copier-7.2.0/README.md
--rw-r--r--   0        0        0      263 2023-04-19 17:40:24.306022 copier-7.2.0/copier/__init__.py
--rw-r--r--   0        0        0      198 2023-04-19 17:40:07.270090 copier-7.2.0/copier/__main__.py
--rw-r--r--   0        0        0    11559 2023-04-19 17:40:07.270090 copier-7.2.0/copier/cli.py
--rw-r--r--   0        0        0     3413 2023-04-19 17:40:07.270090 copier-7.2.0/copier/errors.py
--rw-r--r--   0        0        0    36644 2023-04-19 17:40:07.270090 copier-7.2.0/copier/main.py
--rw-r--r--   0        0        0     2476 2023-04-19 17:40:07.270090 copier-7.2.0/copier/subproject.py
--rw-r--r--   0        0        0    16594 2023-04-19 17:40:07.270090 copier-7.2.0/copier/template.py
--rw-r--r--   0        0        0     6234 2023-04-19 17:40:07.270090 copier-7.2.0/copier/tools.py
--rw-r--r--   0        0        0     2243 2023-04-19 17:40:07.270090 copier-7.2.0/copier/types.py
--rw-r--r--   0        0        0    15733 2023-04-19 17:40:07.274091 copier-7.2.0/copier/user_data.py
--rw-r--r--   0        0        0     6730 2023-04-19 17:40:07.274091 copier-7.2.0/copier/vcs.py
--rw-r--r--   0        0        0     3459 2023-04-19 17:40:24.306022 copier-7.2.0/pyproject.toml
--rw-r--r--   0        0        0     7983 1970-01-01 00:00:00.000000 copier-7.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-06-04 15:59:42.226863 copier-8.0.0/LICENSE
+-rw-r--r--   0        0        0     6143 2023-06-04 15:59:42.226863 copier-8.0.0/README.md
+-rw-r--r--   0        0        0      189 2023-06-04 15:59:56.982921 copier-8.0.0/copier/__init__.py
+-rw-r--r--   0        0        0      198 2023-06-04 15:59:42.226863 copier-8.0.0/copier/__main__.py
+-rw-r--r--   0        0        0    11786 2023-06-04 15:59:42.226863 copier-8.0.0/copier/cli.py
+-rw-r--r--   0        0        0     3745 2023-06-04 15:59:42.226863 copier-8.0.0/copier/errors.py
+-rw-r--r--   0        0        0    38198 2023-06-04 15:59:42.226863 copier-8.0.0/copier/main.py
+-rw-r--r--   0        0        0     2476 2023-06-04 15:59:42.226863 copier-8.0.0/copier/subproject.py
+-rw-r--r--   0        0        0    16594 2023-06-04 15:59:42.226863 copier-8.0.0/copier/template.py
+-rw-r--r--   0        0        0     6234 2023-06-04 15:59:42.226863 copier-8.0.0/copier/tools.py
+-rw-r--r--   0        0        0     2243 2023-06-04 15:59:42.226863 copier-8.0.0/copier/types.py
+-rw-r--r--   0        0        0    17020 2023-06-04 15:59:42.226863 copier-8.0.0/copier/user_data.py
+-rw-r--r--   0        0        0     6730 2023-06-04 15:59:42.226863 copier-8.0.0/copier/vcs.py
+-rw-r--r--   0        0        0     3509 2023-06-04 15:59:56.978921 copier-8.0.0/pyproject.toml
+-rw-r--r--   0        0        0     7718 1970-01-01 00:00:00.000000 copier-8.0.0/PKG-INFO
```

### Comparing `copier-7.2.0/LICENSE` & `copier-8.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `copier-7.2.0/README.md` & `copier-8.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -67,27 +67,27 @@
     ```shell
     copier path/to/project/template path/to/destination
     ```
 
 -   Or in Python code, programmatically:
 
     ```python
-    from copier import run_auto
+    from copier import run_copy
 
     # Create a project from a local path
-    run_auto("path/to/project/template", "path/to/destination")
+    run_copy("path/to/project/template", "path/to/destination")
 
     # Or from a Git URL.
-    run_auto("https://github.com/copier-org/copier.git", "path/to/destination")
+    run_copy("https://github.com/copier-org/copier.git", "path/to/destination")
 
     # You can also use "gh:" as a shortcut of "https://github.com/"
-    run_auto("gh:copier-org/copier.git", "path/to/destination")
+    run_copy("gh:copier-org/copier.git", "path/to/destination")
 
     # Or "gl:" as a shortcut of "https://gitlab.com/"
-    run_auto("gl:copier-org/copier.git", "path/to/destination")
+    run_copy("gl:copier-org/copier.git", "path/to/destination")
     ```
 
 ## Basic concepts
 
 Copier is composed of these main concepts:
 
 1. **Templates**. They lay out how to generate the subproject.
```

### Comparing `copier-7.2.0/copier/cli.py` & `copier-8.0.0/copier/cli.py`

 * *Files 24% similar despite different names*

```diff
@@ -40,60 +40,46 @@
         copier update
         ```
 
 Below are the docs of each one of those.
 """
 
 import sys
-from functools import wraps
 from io import StringIO
 from pathlib import Path
 from textwrap import dedent
 from unittest.mock import patch
 
+from decorator import decorator
 from plumbum import cli, colors
 
-from .errors import UserMessageError
+from .errors import UnsafeTemplateError, UserMessageError
 from .main import Worker
 from .tools import copier_version
 from .types import AnyByStrDict, OptStr, StrSeq
 
 
-def handle_exceptions(method):
+@decorator
+def handle_exceptions(method, *args, **kwargs):
     """Handle keyboard interruption while running a method."""
-
-    @wraps(method)
-    def _wrapper(*args, **kwargs):
+    try:
         try:
-            try:
-                return method(*args, **kwargs)
-            except KeyboardInterrupt:
-                raise UserMessageError("Execution stopped by user")
-        except UserMessageError as error:
-            print(colors.red | "\n".join(error.args), file=sys.stderr)
-            return 1
-
-    return _wrapper
+            return method(*args, **kwargs)
+        except KeyboardInterrupt:
+            raise UserMessageError("Execution stopped by user")
+    except UserMessageError as error:
+        print(colors.red | "\n".join(error.args), file=sys.stderr)
+        return 1
+    except UnsafeTemplateError as error:
+        print(colors.red | "\n".join(error.args), file=sys.stderr)
+        return 2
 
 
 class CopierApp(cli.Application):
-    """The Copier CLI application.
-
-    Attributes:
-        answers_file: Set [answers_file][] option.
-        exclude: Set [exclude][] option.
-        vcs_ref: Set [vcs_ref][] option.
-        pretend: Set [pretend][] option.
-        force: Set [force][] option.
-        defaults: Set [defaults][] option.
-        overwrite: Set [overwrite][] option.
-        skip: Set [skip_if_exists][] option.
-        prereleases: Set [use_prereleases][] option.
-        quiet: Set [quiet][] option.
-    """
+    """The Copier CLI application."""
 
     DESCRIPTION = "Create a new project from a template."
     DESCRIPTION_MORE = (
         dedent(
             """\
             Docs in https://copier.readthedocs.io/
 
@@ -105,77 +91,68 @@
                 """\
                 WARNING! Use only trusted project templates, as they might
                 execute code with the same level of access as your user.\n
                 """
             )
         )
     )
-    USAGE = dedent(
-        """\
-        copier [MAIN_SWITCHES] [copy] [SUB_SWITCHES] template_src destination_path
-        copier [MAIN_SWITCHES] [update] [SUB_SWITCHES] [destination_path]
-        """
-    )
     VERSION = copier_version()
     CALL_MAIN_IF_NESTED_COMMAND = False
+
+
+class _Subcommand(cli.Application):
+    """Base class for Copier subcommands."""
+
     data: AnyByStrDict = {}
 
-    answers_file: cli.SwitchAttr = cli.SwitchAttr(
+    answers_file = cli.SwitchAttr(
         ["-a", "--answers-file"],
         default=None,
         help=(
             "Update using this path (relative to `destination_path`) "
             "to find the answers file"
         ),
     )
-    exclude: cli.SwitchAttr = cli.SwitchAttr(
+    exclude = cli.SwitchAttr(
         ["-x", "--exclude"],
         str,
         list=True,
         help=(
             "A name or shell-style pattern matching files or folders "
             "that must not be copied"
         ),
     )
-    vcs_ref: cli.SwitchAttr = cli.SwitchAttr(
+    vcs_ref = cli.SwitchAttr(
         ["-r", "--vcs-ref"],
         str,
         help=(
             "Git reference to checkout in `template_src`. "
             "If you do not specify it, it will try to checkout the latest git tag, "
             "as sorted using the PEP 440 algorithm. If you want to checkout always "
             "the latest version, use `--vcs-ref=HEAD`."
         ),
     )
-    pretend: cli.Flag = cli.Flag(
-        ["-n", "--pretend"], help="Run but do not make any changes"
-    )
-    force: cli.Flag = cli.Flag(
-        ["-f", "--force"],
-        help="Same as `--defaults --overwrite`.",
-    )
-    defaults: cli.Flag = cli.Flag(
-        ["-l", "--defaults"],
-        help="Use default answers to questions, which might be null if not specified.",
-    )
-    overwrite: cli.Flag = cli.Flag(
-        ["-w", "--overwrite"],
-        help="Overwrite files that already exist, without asking.",
-    )
-    skip: cli.Flag = cli.SwitchAttr(
+    pretend = cli.Flag(["-n", "--pretend"], help="Run but do not make any changes")
+    skip = cli.SwitchAttr(
         ["-s", "--skip"],
         str,
         list=True,
         help="Skip specified files if they exist already",
     )
-    quiet: cli.Flag = cli.Flag(["-q", "--quiet"], help="Suppress status output")
-    prereleases: cli.Flag = cli.Flag(
+    quiet = cli.Flag(["-q", "--quiet"], help="Suppress status output")
+    prereleases = cli.Flag(
         ["-g", "--prereleases"],
         help="Use prereleases to compare template VCS tags.",
     )
+    unsafe = cli.Flag(
+        ["--UNSAFE"],
+        help=(
+            "Allow templates with unsafe features (Jinja extensions, migrations, tasks)"
+        ),
+    )
 
     @cli.switch(
         ["-d", "--data"],
         str,
         "VARIABLE=VALUE",
         list=True,
         help="Make VARIABLE available as VALUE when rendering the template",
@@ -201,165 +178,198 @@
             **kwargs: Arguments passed to [Worker][copier.main.Worker].
         """
         return Worker(
             data=self.data,
             dst_path=Path(dst_path),
             answers_file=self.answers_file,
             exclude=self.exclude,
-            defaults=self.force or self.defaults,
-            overwrite=self.force or self.overwrite,
             pretend=self.pretend,
             skip_if_exists=self.skip,
             quiet=self.quiet,
             src_path=src_path,
             vcs_ref=self.vcs_ref,
             use_prereleases=self.prereleases,
+            unsafe=self.unsafe,
             **kwargs,
         )
 
-    @handle_exceptions
-    def main(self, *args: str) -> int:
-        """Copier CLI app shortcuts.
-
-        This method redirects abstract CLI calls
-        (those that don't specify `copy` or `update`)
-        to [CopierCopySubApp.main][copier.cli.CopierCopySubApp.main]
-        or [CopierUpdateSubApp.main][copier.cli.CopierUpdateSubApp.main]
-        automatically.
-
-        Examples:
-            - `copier from to` → `copier copy from to`
-            - `copier from` → `copier update from`
-            - `copier` → `copier update .`
-        """
-        # Redirect to subcommand if supplied
-        if args and args[0] in self._subcommands:
-            self.nested_command = (
-                self._subcommands[args[0]].subapplication,
-                ["copier %s" % args[0]] + list(args[1:]),
-            )
-        # If using 0 or 1 args, you want to update
-        elif len(args) in {0, 1}:
-            self.nested_command = (
-                self._subcommands["update"].subapplication,
-                ["copier update"] + list(args),
-            )
-        # If using 2 args, you want to copy
-        elif len(args) == 2:
-            self.nested_command = (
-                self._subcommands["copy"].subapplication,
-                ["copier copy"] + list(args),
-            )
-        # If using more args, you're wrong
-        else:
-            self.help()
-            raise UserMessageError("Unsupported arguments")
-        return 0
-
 
 @CopierApp.subcommand("copy")
-class CopierCopySubApp(cli.Application):
+class CopierCopySubApp(_Subcommand):
     """The `copier copy` subcommand.
 
     Use this subcommand to bootstrap a new subproject from a template, or to override
     a preexisting subproject ignoring its history diff.
-
-    Attributes:
-        cleanup_on_error: Set [cleanup_on_error][] option.
     """
 
     DESCRIPTION = "Copy from a template source to a destination."
 
-    cleanup_on_error: cli.Flag = cli.Flag(
+    cleanup_on_error = cli.Flag(
         ["-C", "--no-cleanup"],
         default=True,
         help="On error, do not delete destination if it was created by Copier.",
     )
+    defaults = cli.Flag(
+        ["-l", "--defaults"],
+        help="Use default answers to questions, which might be null if not specified.",
+    )
+    force = cli.Flag(
+        ["-f", "--force"],
+        help="Same as `--defaults --overwrite`.",
+    )
+    overwrite = cli.Flag(
+        ["-w", "--overwrite"],
+        help="Overwrite files that already exist, without asking.",
+    )
 
     @handle_exceptions
     def main(self, template_src: str, destination_path: str) -> int:
         """Call [run_copy][copier.main.Worker.run_copy].
 
         Params:
             template_src:
                 Indicate where to get the template from.
 
                 This can be a git URL or a local path.
 
             destination_path:
                 Where to generate the new subproject. It must not exist or be empty.
         """
-        self.parent._worker(
+        self._worker(
             template_src,
             destination_path,
             cleanup_on_error=self.cleanup_on_error,
+            defaults=self.force or self.defaults,
+            overwrite=self.force or self.overwrite,
         ).run_copy()
         return 0
 
 
+@CopierApp.subcommand("recopy")
+class CopierRecopySubApp(_Subcommand):
+    """The `copier recopy` subcommand.
+
+    Use this subcommand to update an existing subproject from a template that
+    supports updates, ignoring any subproject evolution since the last Copier
+    execution.
+    """
+
+    DESCRIPTION = "Recopy a subproject from its original template"
+    DESCRIPTION_MORE = dedent(
+        """\
+        The copy must have a valid answers file which contains info from the
+        last Copier execution, including the source template (it must be a key
+        called `_src_path`).
+
+        This command will ignore any diff that you have generated since the
+        last `copier` execution. It will act as if it were the 1st time you
+        apply the template to the destination path. However, it will keep the
+        answers.
+
+        If you want a smarter update that respects your project evolution, use
+        `copier update` instead.
+        """
+    )
+
+    defaults = cli.Flag(
+        ["-l", "--defaults"],
+        help="Use default answers to questions, which might be null if not specified.",
+    )
+    force = cli.Flag(
+        ["-f", "--force"],
+        help="Same as `--defaults --overwrite`.",
+    )
+    overwrite = cli.Flag(
+        ["-w", "--overwrite"],
+        help="Overwrite files that already exist, without asking.",
+    )
+
+    @handle_exceptions
+    def main(self, destination_path: cli.ExistingDirectory = ".") -> int:
+        """Call [run_recopy][copier.main.Worker.run_recopy].
+
+        Parameters:
+            destination_path:
+                Only the destination path is needed to update, because the
+                `src_path` comes from [the answers file][the-copier-answersyml-file].
+
+                The subproject must exist. If not specified, the currently
+                working directory is used.
+        """
+        self._worker(
+            dst_path=destination_path,
+            defaults=self.force or self.defaults,
+            overwrite=self.force or self.overwrite,
+        ).run_recopy()
+        return 0
+
+
 @CopierApp.subcommand("update")
-class CopierUpdateSubApp(cli.Application):
+class CopierUpdateSubApp(_Subcommand):
     """The `copier update` subcommand.
 
     Use this subcommand to update an existing subproject from a template
-    that supports updates.
-
-    Attributes:
-        conflict: Set [conflict][] option.
+    that supports updates, respecting that subproject evolution since the last
+    Copier execution.
     """
 
-    DESCRIPTION = "Update a copy from its original template"
+    DESCRIPTION = "Update a subproject from its original template"
     DESCRIPTION_MORE = dedent(
         """\
         The copy must have a valid answers file which contains info
         from the last Copier execution, including the source template
         (it must be a key called `_src_path`).
 
-        If that file contains also `_commit` and `destination_path` is a git
+        If that file contains also `_commit`, and `destination_path` is a git
         repository, this command will do its best to respect the diff that you have
-        generated since the last `copier` execution. To avoid that, use `copier copy`
+        generated since the last `copier` execution. To avoid that, use `copier recopy`
         instead.
         """
     )
 
-    conflict: cli.SwitchAttr = cli.SwitchAttr(
+    conflict = cli.SwitchAttr(
         ["-o", "--conflict"],
         cli.Set("rej", "inline"),
-        default="rej",
+        default="inline",
         help=(
-            "Behavior on conflict: rej=Create .rej file, inline=inline conflict "
-            "markers (inline is still experimental)"
+            "Behavior on conflict: Create .rej files, or add inline conflict markers."
         ),
     )
-    context_lines: cli.SwitchAttr = cli.SwitchAttr(
+    context_lines = cli.SwitchAttr(
         ["-c", "--context-lines"],
         int,
-        default=1,
+        default=3,
         help=(
             "Lines of context to use for detecting conflicts. Increase for "
             "accuracy, decrease for resilience."
         ),
     )
+    defaults = cli.Flag(
+        ["-l", "-f", "--defaults"],
+        help="Use default answers to questions, which might be null if not specified.",
+    )
 
     @handle_exceptions
     def main(self, destination_path: cli.ExistingDirectory = ".") -> int:
         """Call [run_update][copier.main.Worker.run_update].
 
         Parameters:
             destination_path:
                 Only the destination path is needed to update, because the
                 `src_path` comes from [the answers file][the-copier-answersyml-file].
 
                 The subproject must exist. If not specified, the currently
                 working directory is used.
         """
-        self.parent._worker(
+        self._worker(
             dst_path=destination_path,
             conflict=self.conflict,
             context_lines=self.context_lines,
+            defaults=self.defaults,
+            overwrite=True,
         ).run_update()
         return 0
 
 
 # Add --help-all results to docs
 if __doc__:
     help_io = StringIO()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `copier-7.2.0/copier/errors.py` & `copier-8.0.0/copier/errors.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Custom exceptions used by Copier."""
 
 from pathlib import Path
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Sequence
 
 from pydantic.errors import _PathValueError
 
 from .tools import printf_exception
 from .types import PathSeq
 
 if TYPE_CHECKING:  # always false
@@ -94,14 +94,23 @@
         self, answers: "AnswersMap", last_question: "Question", template: "Template"
     ) -> None:
         self.answers = answers
         self.last_question = last_question
         self.template = template
 
 
+class UnsafeTemplateError(CopierError):
+    """Unsafe Copier template features are used without explicit consent."""
+
+    def __init__(self, features: Sequence[str]):
+        assert features
+        s = "s" if len(features) > 1 else ""
+        super().__init__(f"Template uses unsafe feature{s}: {', '.join(features)}")
+
+
 # Warnings
 class CopierWarning(Warning):
     """Base class for all other Copier warnings."""
 
 
 class UnknownCopierVersionWarning(UserWarning, CopierWarning):
     """Cannot determine installed Copier version."""
```

### Comparing `copier-7.2.0/copier/main.py` & `copier-8.0.0/copier/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,30 +7,35 @@
 from contextlib import suppress
 from dataclasses import asdict, field, replace
 from filecmp import dircmp
 from functools import partial
 from itertools import chain
 from pathlib import Path
 from shutil import rmtree
-from typing import Callable, Iterable, Mapping, Optional, Sequence, Union
+from typing import Callable, Iterable, Mapping, Optional, Sequence, Set, Union
 from unicodedata import normalize
 
 from jinja2.loaders import FileSystemLoader
 from jinja2.sandbox import SandboxedEnvironment
 from pathspec import PathSpec
 from plumbum import ProcessExecutionError, colors
 from plumbum.cli.terminal import ask
 from plumbum.cmd import git
 from plumbum.machines import local
 from pydantic import ConfigDict, Extra, PositiveInt
 from pydantic.dataclasses import dataclass
 from pydantic.json import pydantic_encoder
 from questionary import unsafe_prompt
 
-from .errors import CopierAnswersInterrupt, ExtensionNotFoundError, UserMessageError
+from .errors import (
+    CopierAnswersInterrupt,
+    ExtensionNotFoundError,
+    UnsafeTemplateError,
+    UserMessageError,
+)
 from .subproject import Subproject
 from .template import Task, Template
 from .tools import Style, TemporaryDirectory, printf, readlink
 from .types import (
     MISSING,
     AnyByStrDict,
     JSONSerializable,
@@ -58,29 +63,35 @@
         """Backport of `shutil.copytree` with `dirs_exist_ok` argument.
 
         Can be remove once python 3.7 dropped.
         """
         copy_tree(str(src), str(dst))
 
 
+# HACK https://github.com/python/mypy/issues/8520#issuecomment-772081075
+if sys.version_info >= (3, 8):
+    from typing import get_args
+else:
+    from typing_extensions import get_args
+
+
 @dataclass(config=ConfigDict(extra=Extra.forbid))
 class Worker:
     """Copier process state manager.
 
     This class represents the state of a copier work, and contains methods to
     actually produce the desired work.
 
     To use it properly, use it as a context manager and fill all dataclass fields.
 
     Then, execute one of its main methods, which are prefixed with `run_`:
 
     -   [run_copy][copier.main.Worker.run_copy] to copy a subproject.
+    -   [run_recopy][copier.main.Worker.run_recopy] to recopy a subproject.
     -   [run_update][copier.main.Worker.run_update] to update a subproject.
-    -   [run_auto][copier.main.Worker.run_auto] to let it choose whether you
-        want to copy or update the subproject.
 
     Example:
         ```python
         with Worker(
             src_path="https://github.com/copier-org/autopretty.git", "output"
         ) as worker:
             worker.run_copy()
@@ -162,14 +173,19 @@
             Lines of context to consider when solving conflicts in updates.
 
             With more lines, context resolution is more accurate, but it will
             also produce more conflicts if your subproject has evolved.
 
             With less lines, context resolution is less accurate, but it will
             respect better the evolution of your subproject.
+
+        unsafe:
+            When `True`, allow usage of unsafe templates.
+
+            See [unsafe][]
     """
 
     src_path: Optional[str] = None
     dst_path: Path = field(default=Path("."))
     answers_file: Optional[RelativePath] = None
     vcs_ref: OptStr = None
     data: AnyByStrDict = field(default_factory=dict)
@@ -178,16 +194,17 @@
     skip_if_exists: StrSeq = ()
     cleanup_on_error: bool = True
     defaults: bool = False
     user_defaults: AnyByStrDict = field(default_factory=dict)
     overwrite: bool = False
     pretend: bool = False
     quiet: bool = False
-    conflict: str = "rej"
-    context_lines: PositiveInt = 1
+    conflict: str = "inline"
+    context_lines: PositiveInt = 3
+    unsafe: bool = False
 
     def __enter__(self):
         """Allow using worker as a context manager."""
         return self
 
     def __exit__(self, type, value, traceback):
         """Clean up garbage files after worker usage ends."""
@@ -199,14 +216,35 @@
             raise value
         # otherwise clean up and let any exception bubble up
         self._cleanup()
 
     def _cleanup(self):
         self.template._cleanup()
 
+    def _check_unsafe(self, mode: Literal["copy", "update"]) -> None:
+        """Check whether a template uses unsafe features."""
+        if self.unsafe:
+            return
+        features: Set[str] = set()
+        if self.template.jinja_extensions:
+            features.add("jinja_extensions")
+        if self.template.tasks:
+            features.add("tasks")
+        if mode == "update" and self.subproject.template:
+            if self.subproject.template.jinja_extensions:
+                features.add("jinja_extensions")
+            if self.subproject.template.tasks:
+                features.add("tasks")
+            for stage in get_args(Literal["before", "after"]):
+                if self.template.migration_tasks(stage, self.subproject.template):
+                    features.add("migrations")
+                    break
+        if features:
+            raise UnsafeTemplateError(sorted(features))
+
     def _answers_to_remember(self) -> Mapping:
         """Get only answers that will be remembered in the copier answers file."""
         # All internal values must appear first
         answers: AnyByStrDict = {}
         commit = self.template.commit
         src = self.template.url
         for key, value in (("_commit", commit), ("_src_path", src)):
@@ -386,14 +424,20 @@
         for var_name, details in self.template.questions_data.items():
             question = Question(
                 answers=result,
                 jinja_env=self.jinja_env,
                 var_name=var_name,
                 **details,
             )
+            # Skip a question when the skip condition is met and remove any data
+            # from the answers map, so no answer for this question is recorded
+            # in the answers file.
+            if not question.get_when():
+                result.remove(var_name)
+                continue
             if var_name in result.init:
                 # Try to parse the answer value.
                 answer = question.parse_answer(result.init[var_name])
                 # Try to validate the answer value if the question has a
                 # validator.
                 question.validate_answer(answer)
                 # At this point, the answer value is valid. Do not ask the
@@ -409,23 +453,15 @@
                         raise ValueError(f'Question "{var_name}" is required')
                 else:
                     new_answer = unsafe_prompt(
                         [question.get_questionary_structure()], answers=result.combined
                     )[question.var_name]
             except KeyboardInterrupt as err:
                 raise CopierAnswersInterrupt(result, question, self.template) from err
-            previous_answer = result.combined.get(question.var_name)
-            # If question was skipped and it's the 1st
-            # run, you could be getting a raw templated value
-            default_answer = result.default.get(question.var_name)
-            if new_answer == default_answer:
-                new_answer = question.render_value(default_answer)
-                new_answer = question.filter_answer(new_answer)
-            if new_answer != previous_answer:
-                result.user[question.var_name] = new_answer
+            result.user[var_name] = new_answer
 
         return result
 
     @cached_property
     def answers_relpath(self) -> Path:
         """Obtain the proper relative path for the answers file.
 
@@ -595,18 +631,18 @@
             return
         if not self._render_allowed(dst_relpath, is_dir=True):
             return
         dst_abspath = Path(self.subproject.local_abspath, dst_relpath)
         if not self.pretend:
             dst_abspath.mkdir(parents=True, exist_ok=True)
         for file in src_abspath.iterdir():
-            if file.is_dir():
-                self._render_folder(file)
-            elif file.is_symlink() and self.template.preserve_symlinks:
+            if file.is_symlink() and self.template.preserve_symlinks:
                 self._render_symlink(file)
+            elif file.is_dir():
+                self._render_folder(file)
             else:
                 self._render_file(file)
 
     def _render_path(self, relpath: Path) -> Optional[Path]:
         """Render one relative path.
 
         Args:
@@ -677,36 +713,25 @@
 
         It points to the cloned template local abspath + the rendered subdir, if any.
         """
         subdir = self._render_string(self.template.subdirectory) or ""
         return self.template.local_abspath / subdir
 
     # Main operations
-    def run_auto(self) -> None:
-        """Copy or update automatically.
-
-        If `src_path` was supplied, execute
-        [run_copy][copier.main.Worker.run_copy].
-
-        Otherwise, execute [run_update][copier.main.Worker.run_update].
-        """
-        if self.src_path:
-            return self.run_copy()
-        return self.run_update()
-
     def run_copy(self) -> None:
         """Generate a subproject from zero, ignoring what was in the folder.
 
         If `dst_path` was missing, it will be
         created. Otherwise, `src_path` be rendered
         directly into it, without worrying about evolving what was there
         already.
 
         See [generating a project][generating-a-project].
         """
+        self._check_unsafe("copy")
         was_existing = self.subproject.local_abspath.exists()
         src_abspath = self.template_copy_root
         try:
             if not self.quiet:
                 # TODO Unify printing tools
                 print(
                     f"\nCopying from template version {self.template.version}",
@@ -721,19 +746,30 @@
             if not was_existing and self.cleanup_on_error:
                 rmtree(self.subproject.local_abspath)
             raise
         if not self.quiet:
             # TODO Unify printing tools
             print("")  # padding space
 
+    def run_recopy(self) -> None:
+        """Update a subproject, keeping answers but discarding evolution."""
+        if self.subproject.template is None:
+            raise UserMessageError(
+                "Cannot recopy because cannot obtain old template references "
+                f"from `{self.subproject.answers_relpath}`."
+            )
+        new_worker = replace(self, src_path=self.subproject.template.url)
+        return new_worker.run_copy()
+
     def run_update(self) -> None:
         """Update a subproject that was already generated.
 
         See [updating a project][updating-a-project].
         """
+        self._check_unsafe("update")
         # Check all you need is there
         if self.subproject.vcs != "git":
             raise UserMessageError(
                 "Updating is only supported in git-tracked subprojects."
             )
         if self.subproject.is_dirty():
             raise UserMessageError(
@@ -756,14 +792,19 @@
         if not self.template.version:
             raise UserMessageError("Cannot update: version from template not detected.")
         if self.subproject.template.version > self.template.version:
             raise UserMessageError(
                 f"Your are downgrading from {self.subproject.template.version} to {self.template.version}. "
                 "Downgrades are not supported."
             )
+        if not self.overwrite:
+            # Only git-tracked subprojects can be updated, so the user can
+            # review the diff before committing; so we can safely avoid
+            # asking for confirmation
+            raise UserMessageError("Enable overwrite to update a subproject.")
         if not self.quiet:
             # TODO Unify printing tools
             print(
                 f"Updating to template version {self.template.version}", file=sys.stderr
             )
         self._apply_update()
 
@@ -903,47 +944,46 @@
     if data is not None:
         kwargs["data"] = data
     with Worker(src_path=src_path, dst_path=Path(dst_path), **kwargs) as worker:
         worker.run_copy()
     return worker
 
 
-def run_update(
-    dst_path: StrOrPath = ".",
-    data: Optional[AnyByStrDict] = None,
-    **kwargs,
+def run_recopy(
+    dst_path: StrOrPath = ".", data: Optional[AnyByStrDict] = None, **kwargs
 ) -> Worker:
-    """Update a subproject, from its template.
+    """Update a subproject from its template, discarding subproject evolution.
 
-    This is a shortcut for [run_update][copier.main.Worker.run_update].
+    This is a shortcut for [run_recopy][copier.main.Worker.run_recopy].
 
     See [Worker][copier.main.Worker] fields to understand this function's args.
     """
     if data is not None:
         kwargs["data"] = data
     with Worker(dst_path=Path(dst_path), **kwargs) as worker:
-        worker.run_update()
+        worker.run_recopy()
     return worker
 
 
-def run_auto(
-    src_path: OptStr = None,
+def run_update(
     dst_path: StrOrPath = ".",
     data: Optional[AnyByStrDict] = None,
     **kwargs,
 ) -> Worker:
-    """Generate or update a subproject.
+    """Update a subproject, from its template.
 
-    This is a shortcut for [run_auto][copier.main.Worker.run_auto].
+    This is a shortcut for [run_update][copier.main.Worker.run_update].
 
     See [Worker][copier.main.Worker] fields to understand this function's args.
     """
-    if src_path is None:
-        return run_update(dst_path, data, **kwargs)
-    return run_copy(src_path, dst_path, data, **kwargs)
+    if data is not None:
+        kwargs["data"] = data
+    with Worker(dst_path=Path(dst_path), **kwargs) as worker:
+        worker.run_update()
+    return worker
 
 
 def _remove_old_files(prefix: Path, cmp: dircmp, rm_common: bool = False):
     """Remove files and directories only found in "old" template.
 
     This is an internal helper method used to process a comparison of 2
     directories, where the left one is considered the "old" one, and the
```

### Comparing `copier-7.2.0/copier/subproject.py` & `copier-8.0.0/copier/subproject.py`

 * *Files identical despite different names*

### Comparing `copier-7.2.0/copier/template.py` & `copier-8.0.0/copier/template.py`

 * *Files identical despite different names*

### Comparing `copier-7.2.0/copier/tools.py` & `copier-8.0.0/copier/tools.py`

 * *Files identical despite different names*

### Comparing `copier-7.2.0/copier/types.py` & `copier-8.0.0/copier/types.py`

 * *Files identical despite different names*

### Comparing `copier-7.2.0/copier/user_data.py` & `copier-8.0.0/copier/user_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     TYPE_CHECKING,
     Any,
     Callable,
     Dict,
     Mapping,
     Optional,
     Sequence,
+    Set,
     Union,
 )
 
 import yaml
 from jinja2 import UndefinedError
 from jinja2.sandbox import SandboxedEnvironment
 from prompt_toolkit.lexers import PygmentsLexer
@@ -79,17 +80,14 @@
 
 
 @dataclass
 class AnswersMap:
     """Object that gathers answers from different sources.
 
     Attributes:
-        local:
-            Local overrides to other answers.
-
         user:
             Answers provided by the user, interactively.
 
         init:
             Answers provided on init.
 
             This will hold those answers that come from `--data` in
@@ -113,42 +111,51 @@
         user_defaults:
             Default data from the user e.g. previously completed and restored data.
 
             See [copier.main.Worker][].
     """
 
     # Private
-    local: AnyByStrDict = field(default_factory=dict, init=False)
+    removed: Set[str] = field(default_factory=set, init=False)
 
     # Public
     user: AnyByStrDict = field(default_factory=dict)
     init: AnyByStrDict = field(default_factory=dict)
     metadata: AnyByStrDict = field(default_factory=dict)
     last: AnyByStrDict = field(default_factory=dict)
     user_defaults: AnyByStrDict = field(default_factory=dict)
     default: AnyByStrDict = field(default_factory=dict)
 
-    @cached_property
+    @property
     def combined(self) -> Mapping[str, Any]:
         """Answers combined from different sources, sorted by priority."""
-        return ChainMap(
-            self.local,
-            self.user,
-            self.init,
-            self.metadata,
-            self.last,
-            self.user_defaults,
-            self.default,
-            DEFAULT_DATA,
+        combined = dict(
+            ChainMap(
+                self.user,
+                self.init,
+                self.metadata,
+                self.last,
+                self.user_defaults,
+                self.default,
+                DEFAULT_DATA,
+            )
         )
+        for key in self.removed:
+            if key in combined:
+                del combined[key]
+        return combined
 
     def old_commit(self) -> OptStr:
         """Commit when the project was updated from this template the last time."""
         return self.last.get("_commit")
 
+    def remove(self, key: str) -> None:
+        """Remove an answer by key."""
+        self.removed.add(key)
+
 
 @dataclass(config=AllowArbitraryTypes)
 class Question:
     """One question asked to the user.
 
     All attributes are init kwargs.
 
@@ -198,15 +205,15 @@
             converted to boolean using a parser similar to YAML, but only for
             boolean values.
     """
 
     var_name: str
     answers: AnswersMap
     jinja_env: SandboxedEnvironment
-    choices: Union[Dict[Any, Any], Sequence[Any]] = field(default_factory=list)
+    choices: Union[Sequence[Any], Dict[Any, Any]] = field(default_factory=list)
     default: Any = MISSING
     help: str = ""
     multiline: Union[str, bool] = False
     placeholder: str = ""
     secret: bool = False
     type: str = ""
     validator: str = ""
@@ -221,30 +228,47 @@
     @pydantic_validator("type", always=True)
     def _check_type(cls, v, values):
         if v == "":
             default_type_name = type(values.get("default")).__name__
             v = default_type_name if default_type_name in CAST_STR_TO_NATIVE else "yaml"
         return v
 
+    def cast_answer(self, answer: Any) -> Any:
+        """Cast answer to expected type."""
+        type_name = self.get_type_name()
+        type_fn = CAST_STR_TO_NATIVE[type_name]
+        # Only JSON or YAML questions support `None` as an answer
+        if answer is None and type_name not in {"json", "yaml"}:
+            raise InvalidTypeError(
+                f'Invalid answer "{answer}" of type "{type(answer)}" '
+                f'to question "{self.var_name}" of type "{type_name}"'
+            )
+        try:
+            return type_fn(answer)
+        except (TypeError, AttributeError) as error:
+            # JSON or YAML failed because it wasn't a string; no need to convert
+            if type_name in {"json", "yaml"}:
+                return answer
+            raise InvalidTypeError from error
+
     def get_default(self) -> Any:
         """Get the default value for this question, casted to its expected type."""
-        cast_fn = self.get_cast_fn()
         try:
             result = self.answers.init[self.var_name]
         except KeyError:
             try:
                 result = self.answers.last[self.var_name]
             except KeyError:
                 try:
                     result = self.answers.user_defaults[self.var_name]
                 except KeyError:
                     if self.default is MISSING:
                         return MISSING
                     result = self.render_value(self.default)
-        result = cast_answer_type(result, cast_fn)
+        result = self.cast_answer(result)
         return result
 
     def get_default_rendered(self) -> Union[bool, str, Choice, None, MissingType]:
         """Get default answer rendered for the questionary lib.
 
         The questionary lib expects some specific data types, and returns
         it when the user answers. Sometimes you need to compare the response
@@ -289,23 +313,33 @@
             if isinstance(choice, (tuple, list)):
                 name, value = choice
             # If a choice is a single value
             else:
                 name = value = choice
             # The name must always be a str
             name = str(self.render_value(name))
+            # Extract the extended syntax for dict-like (dict-style or
+            # tuple-style) choices if applicable
+            disabled = ""
+            if isinstance(choice, (tuple, list)) and isinstance(value, dict):
+                if "value" not in value:
+                    raise KeyError("Property 'value' is required")
+                if "validator" in value and not isinstance(value["validator"], str):
+                    raise ValueError("Property 'validator' must be a string")
+                disabled = self.render_value(value.get("validator", ""))
+                value = value["value"]
             # The value can be templated
             value = self.render_value(value)
-            result.append(Choice(name, value))
+            c = Choice(name, value, disabled=disabled)
+            # Try to cast the value according to the question's type to raise
+            # an error in case the value is incompatible.
+            self.cast_answer(c.value)
+            result.append(c)
         return result
 
-    def filter_answer(self, answer) -> Any:
-        """Cast the answer to the desired type."""
-        return cast_answer_type(answer, self.get_cast_fn())
-
     def get_message(self) -> str:
         """Get the message that will be printed to the user."""
         if self.help:
             rendered_help = self.render_value(self.help)
             if rendered_help:
                 return force_str_end(rendered_help) + "  "
         # Otherwise, there's no help message defined.
@@ -319,20 +353,20 @@
         """Render and obtain the placeholder."""
         return self.render_value(self.placeholder)
 
     def get_questionary_structure(self) -> AnyByStrDict:
         """Get the question in a format that the questionary lib understands."""
         lexer = None
         result: AnyByStrDict = {
-            "filter": self.filter_answer,
+            "filter": self.cast_answer,
             "message": self.get_message(),
             "mouse_support": True,
             "name": self.var_name,
             "qmark": "🕵️" if self.secret else "🎤",
-            "when": self.get_when,
+            "when": lambda _: self.get_when(),
         }
         default = self.get_default_rendered()
         if default is not MISSING:
             result["default"] = default
         questionary_type = "input"
         type_name = self.get_type_name()
         if type_name == "bool":
@@ -356,24 +390,22 @@
             placeholder = self.get_placeholder()
             if placeholder:
                 result["placeholder"] = placeholder
             result["validate"] = self.validate_answer
         result.update({"type": questionary_type})
         return result
 
-    def get_cast_fn(self) -> Callable:
-        """Obtain function to cast user answer to desired type."""
-        type_name = self.get_type_name()
-        if type_name not in CAST_STR_TO_NATIVE:
-            raise InvalidTypeError("Invalid question type")
-        return CAST_STR_TO_NATIVE.get(type_name, parse_yaml_string)
-
     def get_type_name(self) -> str:
         """Render the type name and return it."""
-        return self.render_value(self.type)
+        type_name = self.render_value(self.type)
+        if type_name not in CAST_STR_TO_NATIVE:
+            raise InvalidTypeError(
+                f'Unsupported type "{type_name}" in question "{self.var_name}"'
+            )
+        return type_name
 
     def get_multiline(self) -> bool:
         """Get the value for multiline."""
         return cast_str_to_bool(self.render_value(self.multiline))
 
     def validate_answer(self, answer) -> bool:
         """Validate user answer."""
@@ -386,15 +418,15 @@
             err_msg = self.render_value(self.validator, {self.var_name: ans}).strip()
         except Exception as error:
             raise ValidationError(message=str(error)) from error
         if err_msg:
             raise ValidationError(message=err_msg)
         return True
 
-    def get_when(self, answers) -> bool:
+    def get_when(self) -> bool:
         """Get skip condition for question."""
         return cast_str_to_bool(self.render_value(self.when))
 
     def render_value(
         self, value: Any, extra_answers: Optional[AnyByStrDict] = None
     ) -> str:
         """Render a single templated value using Jinja.
@@ -411,23 +443,24 @@
         try:
             return template.render({**self.answers.combined, **(extra_answers or {})})
         except UndefinedError as error:
             raise UserMessageError(str(error)) from error
 
     def parse_answer(self, answer: Any) -> Any:
         """Parse the answer according to the question's type."""
-        cast_fn = self.get_cast_fn()
-        ans = cast_answer_type(answer, cast_fn)
-        choice_values = [
-            cast_answer_type(choice.value, cast_fn)
-            for choice in self._formatted_choices
-        ]
-        if choice_values and ans not in choice_values:
-            raise ValueError("Invalid choice")
-        return ans
+        ans = self.cast_answer(answer)
+        choices = self._formatted_choices
+        if not choices:
+            return ans
+        for choice in choices:
+            if ans == self.cast_answer(choice.value):
+                if choice.disabled:
+                    raise ValueError(f"Invalid choice: {choice.disabled}")
+                return ans
+        raise ValueError("Invalid choice")
 
 
 def parse_yaml_string(string: str) -> Any:
     """Parse a YAML string and raise a ValueError if parsing failed.
 
     This method is needed because :meth:`prompt` requires a ``ValueError``
     to repeat failed questions.
@@ -446,23 +479,14 @@
     try:
         with open(Path(dst_path) / (answers_file or ".copier-answers.yml")) as fd:
             return yaml.safe_load(fd)
     except FileNotFoundError:
         return {}
 
 
-def cast_answer_type(answer: Any, type_fn: Callable) -> Any:
-    """Cast answer to expected type."""
-    try:
-        return type_fn(answer)
-    except (TypeError, AttributeError):
-        # JSON or YAML failed because it wasn't a string; no need to convert
-        return answer
-
-
 CAST_STR_TO_NATIVE: Mapping[str, Callable] = {
     "bool": cast_str_to_bool,
     "float": float,
     "int": int,
     "json": json.loads,
     "str": str,
     "yaml": parse_yaml_string,
```

### Comparing `copier-7.2.0/copier/vcs.py` & `copier-8.0.0/copier/vcs.py`

 * *Files identical despite different names*

### Comparing `copier-7.2.0/pyproject.toml` & `copier-8.0.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "copier"
 # This version is a placeholder autoupdated by poetry-dynamic-versioning
-version = "7.2.0"
+version = "8.0.0"
 description = "A library for rendering project templates."
 license = "MIT"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
@@ -26,14 +26,15 @@
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/copier-org/copier/issues"
 
 [tool.poetry.dependencies]
 python = ">=3.7,<4.0" # HACK https://github.com/PyCQA/isort/issues/1945
 "backports.cached-property" = { version = ">=1.0.0", python = "<3.8" }
 colorama = ">=0.4.3"
+decorator = ">=5.1.1"
 dunamai = ">=1.7.0"
 funcy = ">=1.17"
 importlib-metadata = { version = ">=3.4,<7.0", python = "<3.8" }
 jinja2 = ">=3.1.1"
 jinja2-ansible-filters = ">=1.3.1"
 packaging = ">=23.0"
 pathspec = ">=0.9.0"
@@ -53,14 +54,15 @@
 pexpect = ">=4.8.0"
 poethepoet = ">=0.12.3"
 pre-commit = ">=2.17.0"
 pytest = ">=7.2.0"
 pytest-cov = ">=3.0.0"
 pytest-xdist = ">=2.5.0"
 types-backports = ">=0.1.3"
+types-decorator = ">=5.1.1"
 types-pyyaml = ">=6.0.4"
 types-psutil = "*"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
@@ -125,12 +127,12 @@
 ]
 
 [tool.commitizen]
 annotated_tag = true
 changelog_incremental = true
 tag_format = "v$version"
 update_changelog_on_bump = true
-version = "7.2.0"
+version = "8.0.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
```

### Comparing `copier-7.2.0/PKG-INFO` & `copier-8.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copier
-Version: 7.2.0
+Version: 8.0.0
 Summary: A library for rendering project templates.
 Home-page: https://github.com/copier-org/copier
 License: MIT
 Author: Ben Felder
 Author-email: ben@felder.io
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -12,22 +12,17 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: backports.cached-property (>=1.0.0) ; python_version < "3.8"
 Requires-Dist: colorama (>=0.4.3)
+Requires-Dist: decorator (>=5.1.1)
 Requires-Dist: dunamai (>=1.7.0)
 Requires-Dist: funcy (>=1.17)
 Requires-Dist: importlib-metadata (>=3.4,<7.0) ; python_version < "3.8"
 Requires-Dist: jinja2 (>=3.1.1)
 Requires-Dist: jinja2-ansible-filters (>=1.3.1)
 Requires-Dist: packaging (>=23.0)
 Requires-Dist: pathspec (>=0.9.0)
@@ -111,27 +106,27 @@
     ```shell
     copier path/to/project/template path/to/destination
     ```
 
 -   Or in Python code, programmatically:
 
     ```python
-    from copier import run_auto
+    from copier import run_copy
 
     # Create a project from a local path
-    run_auto("path/to/project/template", "path/to/destination")
+    run_copy("path/to/project/template", "path/to/destination")
 
     # Or from a Git URL.
-    run_auto("https://github.com/copier-org/copier.git", "path/to/destination")
+    run_copy("https://github.com/copier-org/copier.git", "path/to/destination")
 
     # You can also use "gh:" as a shortcut of "https://github.com/"
-    run_auto("gh:copier-org/copier.git", "path/to/destination")
+    run_copy("gh:copier-org/copier.git", "path/to/destination")
 
     # Or "gl:" as a shortcut of "https://gitlab.com/"
-    run_auto("gl:copier-org/copier.git", "path/to/destination")
+    run_copy("gl:copier-org/copier.git", "path/to/destination")
     ```
 
 ## Basic concepts
 
 Copier is composed of these main concepts:
 
 1. **Templates**. They lay out how to generate the subproject.
```

