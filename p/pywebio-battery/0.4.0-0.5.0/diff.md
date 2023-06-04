# Comparing `tmp/pywebio_battery-0.4.0.tar.gz` & `tmp/pywebio_battery-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywebio_battery-0.4.0.tar", last modified: Sun Dec 11 02:35:50 2022, max compression
+gzip compressed data, was "pywebio_battery-0.5.0.tar", last modified: Sun Jun  4 11:17:15 2023, max compression
```

## Comparing `pywebio_battery-0.4.0.tar` & `pywebio_battery-0.5.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 02:35:50.629999 pywebio_battery-0.4.0/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1076 2022-12-11 02:35:43.000000 pywebio_battery-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2022-12-11 02:35:50.625999 pywebio_battery-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2022-12-11 02:35:43.000000 pywebio_battery-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 02:35:50.625999 pywebio_battery-0.4.0/pywebio_battery/
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2022-12-11 02:35:43.000000 pywebio_battery-0.4.0/pywebio_battery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2022-12-11 02:35:43.000000 pywebio_battery-0.4.0/pywebio_battery/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10496 2022-12-11 02:35:43.000000 pywebio_battery-0.4.0/pywebio_battery/interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     7466 2022-12-11 02:35:43.000000 pywebio_battery-0.4.0/pywebio_battery/web.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 02:35:50.625999 pywebio_battery-0.4.0/pywebio_battery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2022-12-11 02:35:50.000000 pywebio_battery-0.4.0/pywebio_battery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      333 2022-12-11 02:35:50.000000 pywebio_battery-0.4.0/pywebio_battery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-11 02:35:50.000000 pywebio_battery-0.4.0/pywebio_battery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2022-12-11 02:35:50.000000 pywebio_battery-0.4.0/pywebio_battery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2022-12-11 02:35:50.000000 pywebio_battery-0.4.0/pywebio_battery.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-11 02:35:50.629999 pywebio_battery-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2022-12-11 02:35:43.000000 pywebio_battery-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:17:15.965080 pywebio_battery-0.5.0/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1076 2023-06-04 11:17:08.000000 pywebio_battery-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-06-04 11:17:15.965080 pywebio_battery-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-04 11:17:08.000000 pywebio_battery-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:17:15.965080 pywebio_battery-0.5.0/pywebio_battery/
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-04 11:17:08.000000 pywebio_battery-0.5.0/pywebio_battery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-04 11:17:08.000000 pywebio_battery-0.5.0/pywebio_battery/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8855 2023-06-04 11:17:08.000000 pywebio_battery-0.5.0/pywebio_battery/file_picker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13913 2023-06-04 11:17:08.000000 pywebio_battery-0.5.0/pywebio_battery/interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7466 2023-06-04 11:17:08.000000 pywebio_battery-0.5.0/pywebio_battery/web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:17:15.965080 pywebio_battery-0.5.0/pywebio_battery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-06-04 11:17:15.000000 pywebio_battery-0.5.0/pywebio_battery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-04 11:17:15.000000 pywebio_battery-0.5.0/pywebio_battery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 11:17:15.000000 pywebio_battery-0.5.0/pywebio_battery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-04 11:17:15.000000 pywebio_battery-0.5.0/pywebio_battery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-04 11:17:15.000000 pywebio_battery-0.5.0/pywebio_battery.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 11:17:15.965080 pywebio_battery-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-04 11:17:08.000000 pywebio_battery-0.5.0/setup.py
```

### Comparing `pywebio_battery-0.4.0/LICENSE` & `pywebio_battery-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pywebio_battery-0.4.0/PKG-INFO` & `pywebio_battery-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywebio_battery
-Version: 0.4.0
+Version: 0.5.0
 Summary: Utilities that help write PyWebIO apps quickly and easily.
 Home-page: https://pywebio.readthedocs.io/en/latest/battery.html
 Author: WeiminWang
 Author-email: wang0.618@qq.com
 License: MIT
 Project-URL: Documentation, https://pywebio.readthedocs.io/en/latest/battery.html
 Project-URL: Source, https://github.com/wang0618/pywebio-battery
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pywebio_battery Version: 0.4.0 Summary: Utilities
+Metadata-Version: 2.1 Name: pywebio_battery Version: 0.5.0 Summary: Utilities
 that help write PyWebIO apps quickly and easily. Home-page: https://
 pywebio.readthedocs.io/en/latest/battery.html Author: WeiminWang Author-email:
 wang0.618@qq.com License: MIT Project-URL: Documentation, https://
 pywebio.readthedocs.io/en/latest/battery.html Project-URL: Source, https://
 github.com/wang0618/pywebio-battery Platform: UNKNOWN Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
```

### Comparing `pywebio_battery-0.4.0/README.md` & `pywebio_battery-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pywebio_battery-0.4.0/pywebio_battery/__init__.py` & `pywebio_battery-0.5.0/pywebio_battery/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,26 +4,29 @@
 
 *Utilities that help write PyWebIO apps quickly and easily.*
 
 .. note::
    ``pywebio_battery`` is an extension package of PyWebIO, you must install it before using it.
    To install this package, run ``pip3 install -U pywebio-battery``
 
-Functions list
+Functions index
 -----------------
 
 
 Interaction related
 ^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 .. list-table::
 
    * - Function name
      - Description
 
+   * - `file_picker <pywebio_battery.file_picker>`
+     - Local file picker
+
    * - `confirm <pywebio_battery.confirm>`
      - Confirmation modal
 
    * - `popup_input <pywebio_battery.popup_input>`
      - Show a form in popup window
 
    * - `redirect_stdout <pywebio_battery.redirect_stdout>`
@@ -62,17 +65,14 @@
    * - `basic_auth <pywebio_battery.basic_auth>`, `custom_auth <pywebio_battery.custom_auth>`,
        `revoke_auth <pywebio_battery.revoke_auth>`
      - Authentication
 
 """
 from .interaction import *
 from .web import *
+from .file_picker import file_picker
+
+# make Sphinx can auto generate API docs for this package
 from .interaction import __all__ as interaction_all
 from .web import __all__ as web_all
 
-__all__ = interaction_all + web_all
-
-# Set default logging handler to avoid "No handler found" warnings.
-import logging
-
-logging.getLogger(__name__).addHandler(logging.NullHandler())
-del logging
+__all__ = ['file_picker'] + interaction_all + web_all
```

### Comparing `pywebio_battery-0.4.0/pywebio_battery/interaction.py` & `pywebio_battery-0.5.0/pywebio_battery/interaction.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import base64
 import html
 import io
 import subprocess
 from functools import partial
-from typing import Union, Optional, Sequence
+from typing import Union, Optional, Sequence, Mapping, Tuple, Callable, Dict
 
 from pywebio.output import *
 from pywebio.output import Output
 from pywebio.output import OutputPosition
 from pywebio.pin import *
 from pywebio.session import *
 from pywebio.utils import random_str
 
 __all__ = ['confirm', 'popup_input', 'redirect_stdout', 'run_shell', 'put_logbox', 'logbox_append', 'put_video',
-           'put_audio']
+           'put_audio', 'wait_scroll_to_bottom']
 
 
 def confirm(
         title: str,
         content: Union[str, Output, Sequence[Union[str, Output]]] = None,
         *,
         timeout: int = None
@@ -56,55 +56,90 @@
     if result:
         result = result['value']
     close_popup()
     return result
 
 
 def popup_input(
-        pins: Sequence[Output],
-        title='Please fill out the form below'
+        pins: Union[Sequence[Output], Output],
+        title='Please fill out the form below',
+        validate: Callable[[Dict], Optional[Tuple[str, str]]] = None,
+        popup_size: str = PopupSize.NORMAL,
+        cancelable: bool = False
 ) -> Optional[dict]:
     """Show a form in popup window.
 
     :param list pins: :doc:`pin </pin>` widget list. It can also contain ordinary output widgets.
     :param str title: model title.
+    :param callable validate: validation function for the form.
+        Same as ``validate`` parameter in :func:`input_group() <pywebio.input.input_group()>`
+    :param str popup_size: popup window size. See ``size`` parameter of :func:`popup() <pywebio.output.popup()>`
+    :param bool cancelable: Whether the form can be cancelled. Default is ``False``.
+        If ``cancelable=True``, a "Cancel" button will be displayed at the bottom of the form.
     :return: return the form value as dict, return ``None`` when user cancel the form.
 
     .. exportable-codeblock::
         :name: battery-popup-input
         :summary: Blocking form in the popup.
 
         from pywebio_battery import popup_input  # ..demo-only
         # ..demo-only
-        form = popup_input([
-            put_input("username", label="User name"),
-            put_input("password", type=PASSWORD, label="Password"),
-            put_info("If you forget your password, please contact the administrator."),
-        ], "Login")
+        def check_password(form):
+            if len(form['password']) < 6:
+                return 'password', 'password length must greater than 6'
+
+        form = popup_input(
+            [
+                put_input("username", label="Username"),
+                put_input("password", type=PASSWORD, label="Password"),
+                put_info("If you forget your password, please contact the administrator."),
+            ],
+            title="Login",
+            validate=check_password
+        )
         put_text("Login info:", form)
     """
     if not isinstance(pins, list):
         pins = [pins]
 
     pin_names = [
         p.spec['input']['name']
         for p in pins
         if 'input' in p.spec and 'name' in p.spec['input']
     ]
     action_name = 'action_' + random_str(10)
-    pins.append(put_actions(action_name, buttons=[
-        {'label': 'Submit', 'value': True},
-        {'label': 'Cancel', 'value': False, 'color': 'danger'},
-    ]))
-    popup(title=title, content=pins, closable=False)
+    action_buttons = [{'label': 'Submit', 'value': True}]
+    if cancelable:
+        action_buttons.append({'label': 'Cancel', 'value': False, 'color': 'danger'})
+    pins.append(put_actions(action_name, buttons=action_buttons))
+    popup(title=title, content=pins, closable=False, size=popup_size)
 
-    change_info = pin_wait_change(action_name)
     result = None
-    if change_info['name'] == action_name and change_info['value']:
-        result = {name: pin[name] for name in pin_names}
+    previous_invalid_field = None
+    while True:
+        change_info = pin_wait_change(action_name)
+        if change_info and change_info['name'] == action_name:
+            if not change_info['value']:  # cancel
+                break
+            result = {name: pin[name] for name in pin_names}
+            if not validate:
+                break
+            error_info = validate(result)
+            if not error_info:
+                break
+            try:
+                name, error_msg = error_info
+            except Exception:
+                raise ValueError("The `validate` function for popup_input() must "
+                                 "return `(name, error_msg)` when validation failed.") from None
+            pin_update(name, valid_status=False, invalid_feedback=error_msg)
+            if previous_invalid_field and previous_invalid_field != name:
+                pin_update(previous_invalid_field, valid_status=0)  # remove the previous invalid status
+            previous_invalid_field = name
+
     close_popup()
     return result
 
 
 def redirect_stdout(output_func=partial(put_text, inline=True)):
     """Context manager for temporarily redirecting stdout to pywebio.
 
@@ -271,7 +306,46 @@
         src = 'data:audio/wav;base64, ' + base64.b64encode(src).decode('ascii')
 
     tag_fields = ['autoplay', 'loop', 'muted']
     tags = ' '.join(t for t in tag_fields if kwargs[t])
 
     tag = r'<audio src="{src}" {tags} controls preload="metadata"><audio/>'.format(src=src, tags=tags)
     return put_html(tag, scope=scope, position=position)
+
+
+def wait_scroll_to_bottom(threshold: float = 10, timeout: float = None) -> bool:
+    """Wait until the page is scrolled to bottom.
+
+    This function is useful to achieve infinite scrolling.
+
+    :param float threshold: If the distance (in pixels) of the browser's viewport from the bottom of the page is less
+        than the threshold, it is considered to reach the bottom
+    :param float timeout: Timeout in seconds. The maximum time to wait for the page to scroll to bottom.
+        Default is None, which means no timeout.
+    :return: Return ``True`` if the page is scrolled to bottom, return ``False`` only when timeout.
+
+    Example:
+
+    .. exportable-codeblock::
+        :name: wait_scroll_to_bottom
+        :summary: `wait_scroll_to_bottom()` usage
+
+        put_text('This is long text. Scroll to bottom to continue.\n' * 100)
+        while True:
+            wait_scroll_to_bottom()
+            put_text("New generated content\n"*20)
+
+    .. versionadded:: 0.5
+    """
+    return eval_js("""
+        (function(){
+            if($(window).scrollTop() + window.innerHeight > $(document).height() - threshold) return true;
+            return new Promise(function(resolve){
+                $(window).on('scroll', function(e){
+                    if($(window).scrollTop() + window.innerHeight > $(document).height() - threshold){
+                        resolve(true);
+                    }
+                });
+                if(timeout) setTimeout(function(){ resolve(false); }, timeout*1000);
+            });
+        })();
+    """, threshold=threshold, timeout=timeout)
```

### Comparing `pywebio_battery-0.4.0/pywebio_battery/web.py` & `pywebio_battery-0.5.0/pywebio_battery/web.py`

 * *Files identical despite different names*

### Comparing `pywebio_battery-0.4.0/pywebio_battery.egg-info/PKG-INFO` & `pywebio_battery-0.5.0/pywebio_battery.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywebio-battery
-Version: 0.4.0
+Version: 0.5.0
 Summary: Utilities that help write PyWebIO apps quickly and easily.
 Home-page: https://pywebio.readthedocs.io/en/latest/battery.html
 Author: WeiminWang
 Author-email: wang0.618@qq.com
 License: MIT
 Project-URL: Documentation, https://pywebio.readthedocs.io/en/latest/battery.html
 Project-URL: Source, https://github.com/wang0618/pywebio-battery
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pywebio-battery Version: 0.4.0 Summary: Utilities
+Metadata-Version: 2.1 Name: pywebio-battery Version: 0.5.0 Summary: Utilities
 that help write PyWebIO apps quickly and easily. Home-page: https://
 pywebio.readthedocs.io/en/latest/battery.html Author: WeiminWang Author-email:
 wang0.618@qq.com License: MIT Project-URL: Documentation, https://
 pywebio.readthedocs.io/en/latest/battery.html Project-URL: Source, https://
 github.com/wang0618/pywebio-battery Platform: UNKNOWN Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
```

### Comparing `pywebio_battery-0.4.0/setup.py` & `pywebio_battery-0.5.0/setup.py`

 * *Files identical despite different names*

