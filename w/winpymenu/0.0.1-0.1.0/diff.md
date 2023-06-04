# Comparing `tmp/winpymenu-0.0.1.tar.gz` & `tmp/winpymenu-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "winpymenu-0.0.1.tar", last modified: Sun Jun  4 14:04:29 2023, max compression
+gzip compressed data, was "winpymenu-0.1.0.tar", last modified: Sun Jun  4 20:07:12 2023, max compression
```

## Comparing `winpymenu-0.0.1.tar` & `winpymenu-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 14:04:29.037202 winpymenu-0.0.1/
--rw-rw-rw-   0        0        0     1091 2023-06-04 08:16:00.000000 winpymenu-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      183 2023-06-04 14:04:29.036201 winpymenu-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      499 2023-06-04 11:06:26.000000 winpymenu-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-04 14:04:29.037202 winpymenu-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      523 2023-06-04 12:55:59.000000 winpymenu-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-04 14:04:29.025685 winpymenu-0.0.1/winpymenu/
--rw-rw-rw-   0        0        0      113 2023-06-03 21:13:23.000000 winpymenu-0.0.1/winpymenu/__init__.py
--rw-rw-rw-   0        0        0      645 2023-06-03 21:06:49.000000 winpymenu-0.0.1/winpymenu/winpycolors.py
--rw-rw-rw-   0        0        0      386 2023-06-03 10:00:45.000000 winpymenu-0.0.1/winpymenu/winpymath.py
--rw-rw-rw-   0        0        0       39 2023-06-03 10:01:44.000000 winpymenu-0.0.1/winpymenu/winpymultiselectmenu.py
--rw-rw-rw-   0        0        0     4314 2023-06-04 13:20:15.000000 winpymenu-0.0.1/winpymenu/winpysimplemenu.py
--rw-rw-rw-   0        0        0     1309 2023-06-04 11:55:37.000000 winpymenu-0.0.1/winpymenu/winpyterminal.py
-drwxrwxrwx   0        0        0        0 2023-06-04 14:04:29.035192 winpymenu-0.0.1/winpymenu.egg-info/
--rw-rw-rw-   0        0        0      183 2023-06-04 14:04:28.000000 winpymenu-0.0.1/winpymenu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      318 2023-06-04 14:04:29.000000 winpymenu-0.0.1/winpymenu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 14:04:28.000000 winpymenu-0.0.1/winpymenu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-06-04 14:04:28.000000 winpymenu-0.0.1/winpymenu.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:07:12.928195 winpymenu-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-04 20:06:57.000000 winpymenu-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-04 20:07:12.924195 winpymenu-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-04 20:06:57.000000 winpymenu-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 20:07:12.928195 winpymenu-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-04 20:06:57.000000 winpymenu-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:07:12.924195 winpymenu-0.1.0/winpymenu/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-04 20:06:57.000000 winpymenu-0.1.0/winpymenu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-04 20:06:57.000000 winpymenu-0.1.0/winpymenu/winpycolors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-04 20:06:57.000000 winpymenu-0.1.0/winpymenu/winpymath.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-04 20:06:57.000000 winpymenu-0.1.0/winpymenu/winpymultiselectmenu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-06-04 20:06:57.000000 winpymenu-0.1.0/winpymenu/winpysimplemenu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-06-04 20:06:57.000000 winpymenu-0.1.0/winpymenu/winpyterminal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:07:12.924195 winpymenu-0.1.0/winpymenu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-04 20:07:12.000000 winpymenu-0.1.0/winpymenu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-04 20:07:12.000000 winpymenu-0.1.0/winpymenu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 20:07:12.000000 winpymenu-0.1.0/winpymenu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-04 20:07:12.000000 winpymenu-0.1.0/winpymenu.egg-info/top_level.txt
```

### Comparing `winpymenu-0.0.1/winpymenu/winpysimplemenu.py` & `winpymenu-0.1.0/winpymenu/winpysimplemenu.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,101 +1,101 @@
-from dataclasses import dataclass, field
-import msvcrt
-import os
-import string
-import re
-from .winpyterminal import print_lines, delete_lines, delete_all_lines, cursor_backwards, is_decodable, clear_terminal
-from .winpycolors import WinPyColors, WinPyStyles, ENDC
-from .winpymath import clamp
-
-
-@dataclass
-class WinPySimpleMenu:
-    """ Simple CLI menu for windows
-
-    Args:
-        options (list[str]): List of the options for the menu
-        default_option (int): Deafult option that will be highlihged
-        prechar (str): Prechar for the options. Defaults to "> "
-        clear_on_exit (bool): Clear console in exit of the menu. Defaults on True
-        selected_color (WinPyColors): Color of the selected option. Defaults to None
-        selected_style (WinPyStyles): Font style pf the seletect option. Defaults to None
-    
-    """
-    options:list[str]
-    default_option:int = 0
-    prechar:str = "> "
-    clear_on_exit:bool = True
-    selected_color:WinPyColors = ""
-    selected_style:WinPyStyles = WinPyStyles.UNDERLINE
-    _selected_option:int = default_option
-
-    _searching_buffer:str = ""
-
-    _terminal_last_line_size:int = os.get_terminal_size().lines
-    _terminal_last_column_size:int = os.get_terminal_size().columns
-
-    @property
-    def _pritable_options(self):
-        temp_option:str
-        temp_printable_options:list = []
-
-        available_options:list[str] = []
-        for option in self.options:
-            if re.match(re.escape(self._searching_buffer[1:]), option):
-                available_options.append(option)
-
-        for index, option in enumerate(available_options):
-            temp_option = option
-            if index == self._selected_option:
-                temp_option = self.selected_color + self.selected_style + temp_option
-            temp_option = self.prechar + temp_option + ENDC
-            temp_printable_options.append(temp_option)
-        return temp_printable_options
-    
-    @property
-    def _terminal_resized(self):
-        return os.get_terminal_size().lines != self._terminal_last_line_size or os.get_terminal_size().columns != self._terminal_last_column_size
-
-    @property
-    def _searching(self) -> bool:
-        return len(self._searching_buffer) > 0
-
-
-    def show(self):
-        clear_terminal()
-        print_lines(self._pritable_options, self._searching_buffer)
-        while True:
-            if self._terminal_resized:
-                self._terminal_last_line_size = os.get_terminal_size().lines
-                self._terminal_last_column_size = os.get_terminal_size().columns
-                clear_terminal()
-                print_lines(self._pritable_options, self._searching_buffer)
-
-            if msvcrt.kbhit():
-                key = msvcrt.getch()
-                if key == b'\xe0': # tecla especial
-                    special_key = msvcrt.getch()
-                    if special_key == b'H':
-                        self._selected_option -= 1
-                    elif special_key == b'P':
-                        self._selected_option += 1
-                    self._selected_option = clamp(self._selected_option, 0, len(self._pritable_options)-1)
-                elif key == b'\r':
-                    delete_all_lines(self._searching_buffer, self._terminal_last_line_size)
-                    return self._selected_option
-                elif key == b'/' and not self._searching:
-                    self._searching_buffer = "/"
-                elif self._searching:
-                    if key == b'\x08':
-                        char_to_remove = self._searching_buffer[-1]
-                        self._searching_buffer = self._searching_buffer[:-1]
-                        if char_to_remove.encode() == b'\t':
-                            cursor_backwards(times=6)
-                        cursor_backwards()
-
-                    elif is_decodable(key) and key.decode() in string.printable:
-                        self._searching_buffer += key.decode()
-
-                self._selected_option = clamp(self._selected_option, 0, len(self._pritable_options)-1)
-                delete_all_lines(self._searching_buffer, self._terminal_last_line_size)
-                print_lines(self._pritable_options, self._searching_buffer)
+from dataclasses import dataclass, field
+import msvcrt
+import os
+import string
+import re
+from .winpyterminal import print_lines, delete_lines, delete_all_lines, cursor_backwards, is_decodable, clear_terminal
+from .winpycolors import WinPyColors, WinPyStyles, ENDC
+from .winpymath import clamp
+
+
+@dataclass
+class WinPySimpleMenu:
+    """ Simple CLI menu for windows
+
+    Args:
+        options (list[str]): List of the options for the menu
+        default_option (int): Deafult option that will be highlihged
+        prechar (str): Prechar for the options. Defaults to "> "
+        clear_on_exit (bool): Clear console in exit of the menu. Defaults on True
+        selected_color (WinPyColors): Color of the selected option. Defaults to None
+        selected_style (WinPyStyles): Font style pf the seletect option. Defaults to None
+    
+    """
+    options:list[str]
+    default_option:int = 0
+    prechar:str = "> "
+    clear_on_exit:bool = True
+    selected_color:WinPyColors = ""
+    selected_style:WinPyStyles = WinPyStyles.UNDERLINE
+    _selected_option:int = default_option
+
+    _searching_buffer:str = ""
+
+    _terminal_last_line_size:int = os.get_terminal_size().lines
+    _terminal_last_column_size:int = os.get_terminal_size().columns
+
+    @property
+    def _pritable_options(self):
+        temp_option:str
+        temp_printable_options:list = []
+
+        available_options:list[str] = []
+        for option in self.options:
+            if re.match(re.escape(self._searching_buffer[1:]), option):
+                available_options.append(option)
+
+        for index, option in enumerate(available_options):
+            temp_option = option
+            if index == self._selected_option:
+                temp_option = self.selected_color + self.selected_style + temp_option
+            temp_option = self.prechar + temp_option + ENDC
+            temp_printable_options.append(temp_option)
+        return temp_printable_options
+    
+    @property
+    def _terminal_resized(self):
+        return os.get_terminal_size().lines != self._terminal_last_line_size or os.get_terminal_size().columns != self._terminal_last_column_size
+
+    @property
+    def _searching(self) -> bool:
+        return len(self._searching_buffer) > 0
+
+
+    def show(self):
+        clear_terminal()
+        print_lines(self._pritable_options, self._searching_buffer)
+        while True:
+            if self._terminal_resized:
+                self._terminal_last_line_size = os.get_terminal_size().lines
+                self._terminal_last_column_size = os.get_terminal_size().columns
+                clear_terminal()
+                print_lines(self._pritable_options, self._searching_buffer)
+
+            if msvcrt.kbhit():
+                key = msvcrt.getch()
+                if key == b'\xe0': # tecla especial
+                    special_key = msvcrt.getch()
+                    if special_key == b'H':
+                        self._selected_option -= 1
+                    elif special_key == b'P':
+                        self._selected_option += 1
+                    self._selected_option = clamp(self._selected_option, 0, len(self._pritable_options)-1)
+                elif key == b'\r':
+                    delete_all_lines(self._searching_buffer, self._terminal_last_line_size)
+                    return self._selected_option
+                elif key == b'/' and not self._searching:
+                    self._searching_buffer = "/"
+                elif self._searching:
+                    if key == b'\x08':
+                        char_to_remove = self._searching_buffer[-1]
+                        self._searching_buffer = self._searching_buffer[:-1]
+                        if char_to_remove.encode() == b'\t':
+                            cursor_backwards(times=6)
+                        cursor_backwards()
+
+                    elif is_decodable(key) and key.decode() in string.printable:
+                        self._searching_buffer += key.decode()
+
+                self._selected_option = clamp(self._selected_option, 0, len(self._pritable_options)-1)
+                delete_all_lines(self._searching_buffer, self._terminal_last_line_size)
+                print_lines(self._pritable_options, self._searching_buffer)
```

### Comparing `winpymenu-0.0.1/winpymenu/winpyterminal.py` & `winpymenu-0.1.0/winpymenu/winpyterminal.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-import os
-import sys
-
-CURSOR_UP_ONE = '\x1b[1A'
-ERASE_LINE = '\x1b[2K'
-
-CURSOR_BACKWARD = '\x1b[D'
-
-GET_CURSOR_POSITION = '\x1b[6n'
-
-
-
-def print_lines(lines:list[str], searching_buffer:str)->int:
-    count:int = 0
-    for line in lines:
-        print(line)
-        count += (len(line) // int(os.get_terminal_size().columns)) + 1
-
-    for i in range(count+1, os.get_terminal_size().lines):
-        print()
-    
-    print(searching_buffer, end="", flush=True)
-
-    return count
-
-def delete_lines(lines:int):
-    """ Delete a number of lines from stodut
-
-    Args:
-        lines (int): Number of lines to be deleted
-    """
-    for i in range(lines):
-        print(f"{CURSOR_UP_ONE}{ERASE_LINE}", end="")
-
-def delete_all_lines(searching_buffer:str, lines:int):
-    print(CURSOR_BACKWARD*len(searching_buffer), end="")
-
-    for index in range(0, lines+1):
-        print(f"{ERASE_LINE}", end="")
-        if index != lines:
-            print(f"{CURSOR_UP_ONE}", end="")
-
-
-def cursor_backwards(times:int=1):
-    print(CURSOR_BACKWARD*times, end="")
-
-
-def is_decodable(byte:bytes, encoding='utf-8'):
-    try:
-        byte.decode(encoding)
-        return True
-    except UnicodeDecodeError:
-        return False
-    
-
-def clear_terminal():
-    os.system("cls")
+import os
+import sys
+
+CURSOR_UP_ONE = '\x1b[1A'
+ERASE_LINE = '\x1b[2K'
+
+CURSOR_BACKWARD = '\x1b[D'
+
+GET_CURSOR_POSITION = '\x1b[6n'
+
+
+
+def print_lines(lines:list[str], searching_buffer:str)->int:
+    count:int = 0
+    for line in lines:
+        print(line)
+        count += (len(line) // int(os.get_terminal_size().columns)) + 1
+
+    for i in range(count+1, os.get_terminal_size().lines):
+        print()
+    
+    print(searching_buffer, end="", flush=True)
+
+    return count
+
+def delete_lines(lines:int):
+    """ Delete a number of lines from stodut
+
+    Args:
+        lines (int): Number of lines to be deleted
+    """
+    for i in range(lines):
+        print(f"{CURSOR_UP_ONE}{ERASE_LINE}", end="")
+
+def delete_all_lines(searching_buffer:str, lines:int):
+    print(CURSOR_BACKWARD*len(searching_buffer), end="")
+
+    for index in range(0, lines+1):
+        print(f"{ERASE_LINE}", end="")
+        if index != lines:
+            print(f"{CURSOR_UP_ONE}", end="")
+
+
+def cursor_backwards(times:int=1):
+    print(CURSOR_BACKWARD*times, end="")
+
+
+def is_decodable(byte:bytes, encoding='utf-8'):
+    try:
+        byte.decode(encoding)
+        return True
+    except UnicodeDecodeError:
+        return False
+    
+
+def clear_terminal():
+    os.system("cls")
```

