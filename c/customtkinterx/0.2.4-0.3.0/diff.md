# Comparing `tmp/customtkinterx-0.2.4.tar.gz` & `tmp/customtkinterx-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "customtkinterx-0.2.4.tar", max compression
+gzip compressed data, was "customtkinterx-0.3.0.tar", max compression
```

## Comparing `customtkinterx-0.2.4.tar` & `customtkinterx-0.3.0.tar`

### file list

```diff
@@ -1,36 +1,40 @@
--rw-r--r--   0        0        0      242 2023-06-02 14:05:53.035149 customtkinterx-0.2.4/customtkinterx/__base64.py
--rw-r--r--   0        0        0      971 2023-06-03 06:08:32.364752 customtkinterx-0.2.4/customtkinterx/__init__.py
--rw-r--r--   0        0        0      809 2023-06-03 06:51:26.706174 customtkinterx-0.2.4/customtkinterx/__main__.py
--rw-r--r--   0        0        0     8210 2023-06-03 06:51:26.711685 customtkinterx-0.2.4/customtkinterx/CTkCustom.py
--rw-r--r--   0        0        0     6220 2023-06-03 03:49:13.477694 customtkinterx-0.2.4/customtkinterx/CTkFluentTheme.py
--rw-r--r--   0        0        0     6286 2023-06-03 04:57:04.717519 customtkinterx-0.2.4/customtkinterx/CTkInfoBar.py
--rw-r--r--   0        0        0     1244 2023-06-02 11:00:54.754723 customtkinterx-0.2.4/customtkinterx/CTkListBox.py
--rw-r--r--   0        0        0     3180 2023-06-03 04:57:04.655526 customtkinterx-0.2.4/customtkinterx/CTkMegaMenuBar.py
--rw-r--r--   0        0        0      269 2023-05-29 10:31:31.000000 customtkinterx-0.2.4/customtkinterx/CTkMenuBar/__init__.py
--rw-r--r--   0        0        0      522 2023-06-03 04:06:01.937274 customtkinterx-0.2.4/customtkinterx/CTkMenuBar/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    16174 2023-06-03 04:13:46.399109 customtkinterx-0.2.4/customtkinterx/CTkMenuBar/__pycache__/dropdown_menu.cpython-311.pyc
--rw-r--r--   0        0        0     5239 2023-06-03 04:13:46.393587 customtkinterx-0.2.4/customtkinterx/CTkMenuBar/__pycache__/menu_bar.cpython-311.pyc
--rw-r--r--   0        0        0     9724 2023-06-03 04:13:46.396108 customtkinterx-0.2.4/customtkinterx/CTkMenuBar/__pycache__/title_menu_win.cpython-311.pyc
--rw-r--r--   0        0        0     9636 2023-06-03 04:10:48.431998 customtkinterx-0.2.4/customtkinterx/CTkMenuBar/dropdown_menu.py
--rw-r--r--   0        0        0     3300 2023-06-03 04:10:48.421486 customtkinterx-0.2.4/customtkinterx/CTkMenuBar/menu_bar.py
--rw-r--r--   0        0        0     5858 2023-06-03 04:10:48.439015 customtkinterx-0.2.4/customtkinterx/CTkMenuBar/title_menu_win.py
--rw-r--r--   0        0        0     6190 2023-06-03 04:57:53.921397 customtkinterx-0.2.4/customtkinterx/CTkMinimalTheme.py
--rw-r--r--   0        0        0      241 2023-05-31 01:43:30.000000 customtkinterx-0.2.4/customtkinterx/CTkPDFViewer/__init__.py
--rw-r--r--   0        0        0      445 2023-06-03 04:13:46.400109 customtkinterx-0.2.4/customtkinterx/CTkPDFViewer/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     6312 2023-06-03 05:49:55.800794 customtkinterx-0.2.4/customtkinterx/CTkPDFViewer/__pycache__/ctk_pdf_viewer.cpython-311.pyc
--rw-r--r--   0        0        0     3543 2023-06-03 05:14:11.938896 customtkinterx-0.2.4/customtkinterx/CTkPDFViewer/ctk_pdf_viewer.py
--rw-r--r--   0        0        0      227 2023-05-31 01:40:22.000000 customtkinterx-0.2.4/customtkinterx/CTkTable/__init__.py
--rw-r--r--   0        0        0      427 2023-06-03 04:41:34.919572 customtkinterx-0.2.4/customtkinterx/CTkTable/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    11621 2023-06-03 04:41:34.922572 customtkinterx-0.2.4/customtkinterx/CTkTable/__pycache__/ctktable.cpython-311.pyc
--rw-r--r--   0        0        0     8158 2023-06-03 04:41:34.520984 customtkinterx-0.2.4/customtkinterx/CTkTable/ctktable.py
--rw-r--r--   0        0        0      225 2023-05-08 22:30:16.000000 customtkinterx-0.2.4/customtkinterx/CTkToolTip/__init__.py
--rw-r--r--   0        0        0      426 2023-06-03 04:22:17.427710 customtkinterx-0.2.4/customtkinterx/CTkToolTip/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    10684 2023-06-03 04:26:02.400121 customtkinterx-0.2.4/customtkinterx/CTkToolTip/__pycache__/ctk_tooltip.cpython-311.pyc
--rw-r--r--   0        0        0     6942 2023-06-03 04:22:52.495987 customtkinterx-0.2.4/customtkinterx/CTkToolTip/ctk_tooltip.py
--rw-r--r--   0        0        0     5598 2023-06-02 14:38:51.493749 customtkinterx-0.2.4/customtkinterx/Fluent.json
--rw-r--r--   0        0        0     2714 2023-06-03 05:59:19.575174 customtkinterx-0.2.4/customtkinterx/LaunchMusix.py
--rw-r--r--   0        0        0     5563 2023-06-03 05:50:30.149406 customtkinterx-0.2.4/customtkinterx/Minimal.json
--rw-r--r--   0        0        0     5435 2023-06-03 06:15:30.726312 customtkinterx-0.2.4/customtkinterx/tk_dragtool.py
--rw-r--r--   0        0        0      343 2023-06-03 06:54:18.438839 customtkinterx-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     3686 2023-06-03 06:54:12.682589 customtkinterx-0.2.4/README.md
--rw-r--r--   0        0        0     4121 1970-01-01 00:00:00.000000 customtkinterx-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0      242 2023-06-02 14:05:53.035149 customtkinterx-0.3.0/customtkinterx/__base64.py
+-rw-r--r--   0        0        0      973 2023-06-04 02:18:15.777749 customtkinterx-0.3.0/customtkinterx/__init__.py
+-rw-r--r--   0        0        0      810 2023-06-04 02:18:15.797263 customtkinterx-0.3.0/customtkinterx/__main__.py
+-rw-r--r--   0        0        0     8540 2023-06-03 22:47:50.802511 customtkinterx-0.3.0/customtkinterx/CTkCustom.py
+-rw-r--r--   0        0        0     6312 2023-06-03 22:39:55.190954 customtkinterx-0.3.0/customtkinterx/CTkFluentTheme.py
+-rw-r--r--   0        0        0     6286 2023-06-03 04:57:04.717519 customtkinterx-0.3.0/customtkinterx/CTkInfoBar.py
+-rw-r--r--   0        0        0     1244 2023-06-02 11:00:54.754723 customtkinterx-0.3.0/customtkinterx/CTkListBox.py
+-rw-r--r--   0        0        0     6321 2023-06-04 02:18:15.803265 customtkinterx-0.3.0/customtkinterx/CTkMaterialTheme.py
+-rw-r--r--   0        0        0     2596 2023-06-04 02:13:08.630709 customtkinterx-0.3.0/customtkinterx/CTkMegaMenuBar.py
+-rw-r--r--   0        0        0      269 2023-05-29 10:31:31.000000 customtkinterx-0.3.0/customtkinterx/CTkMenuBar/__init__.py
+-rw-r--r--   0        0        0      522 2023-06-03 04:06:01.937274 customtkinterx-0.3.0/customtkinterx/CTkMenuBar/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    16174 2023-06-03 04:13:46.399109 customtkinterx-0.3.0/customtkinterx/CTkMenuBar/__pycache__/dropdown_menu.cpython-311.pyc
+-rw-r--r--   0        0        0     5239 2023-06-03 04:13:46.393587 customtkinterx-0.3.0/customtkinterx/CTkMenuBar/__pycache__/menu_bar.cpython-311.pyc
+-rw-r--r--   0        0        0     9724 2023-06-03 04:13:46.396108 customtkinterx-0.3.0/customtkinterx/CTkMenuBar/__pycache__/title_menu_win.cpython-311.pyc
+-rw-r--r--   0        0        0     9636 2023-06-03 04:10:48.431998 customtkinterx-0.3.0/customtkinterx/CTkMenuBar/dropdown_menu.py
+-rw-r--r--   0        0        0     3300 2023-06-03 04:10:48.421486 customtkinterx-0.3.0/customtkinterx/CTkMenuBar/menu_bar.py
+-rw-r--r--   0        0        0     5858 2023-06-03 04:10:48.439015 customtkinterx-0.3.0/customtkinterx/CTkMenuBar/title_menu_win.py
+-rw-r--r--   0        0        0     6285 2023-06-03 22:42:43.931473 customtkinterx-0.3.0/customtkinterx/CTkMinimalTheme.py
+-rw-r--r--   0        0        0     6337 2023-06-04 02:14:05.106099 customtkinterx-0.3.0/customtkinterx/CTkOffice2019Theme.py
+-rw-r--r--   0        0        0      241 2023-05-31 01:43:30.000000 customtkinterx-0.3.0/customtkinterx/CTkPDFViewer/__init__.py
+-rw-r--r--   0        0        0      445 2023-06-03 04:13:46.400109 customtkinterx-0.3.0/customtkinterx/CTkPDFViewer/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     6312 2023-06-03 05:49:55.800794 customtkinterx-0.3.0/customtkinterx/CTkPDFViewer/__pycache__/ctk_pdf_viewer.cpython-311.pyc
+-rw-r--r--   0        0        0     3543 2023-06-03 05:14:11.938896 customtkinterx-0.3.0/customtkinterx/CTkPDFViewer/ctk_pdf_viewer.py
+-rw-r--r--   0        0        0      227 2023-05-31 01:40:22.000000 customtkinterx-0.3.0/customtkinterx/CTkTable/__init__.py
+-rw-r--r--   0        0        0      427 2023-06-03 04:41:34.919572 customtkinterx-0.3.0/customtkinterx/CTkTable/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    11621 2023-06-03 04:41:34.922572 customtkinterx-0.3.0/customtkinterx/CTkTable/__pycache__/ctktable.cpython-311.pyc
+-rw-r--r--   0        0        0     8158 2023-06-03 04:41:34.520984 customtkinterx-0.3.0/customtkinterx/CTkTable/ctktable.py
+-rw-r--r--   0        0        0      225 2023-05-08 22:30:16.000000 customtkinterx-0.3.0/customtkinterx/CTkToolTip/__init__.py
+-rw-r--r--   0        0        0      426 2023-06-03 04:22:17.427710 customtkinterx-0.3.0/customtkinterx/CTkToolTip/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    10684 2023-06-03 04:26:02.400121 customtkinterx-0.3.0/customtkinterx/CTkToolTip/__pycache__/ctk_tooltip.cpython-311.pyc
+-rw-r--r--   0        0        0     6942 2023-06-03 04:22:52.495987 customtkinterx-0.3.0/customtkinterx/CTkToolTip/ctk_tooltip.py
+-rw-r--r--   0        0        0     5690 2023-06-03 22:45:30.417651 customtkinterx-0.3.0/customtkinterx/Fluent.json
+-rw-r--r--   0        0        0     2717 2023-06-03 22:53:01.926976 customtkinterx-0.3.0/customtkinterx/LaunchMusix.py
+-rw-r--r--   0        0        0     5683 2023-06-04 02:21:16.783149 customtkinterx-0.3.0/customtkinterx/Material.json
+-rw-r--r--   0        0        0     5655 2023-06-03 22:45:30.423651 customtkinterx-0.3.0/customtkinterx/Minimal.json
+-rw-r--r--   0        0        0     5683 2023-06-03 23:01:51.610936 customtkinterx-0.3.0/customtkinterx/Office2019.json
+-rw-r--r--   0        0        0     5435 2023-06-03 06:15:30.726312 customtkinterx-0.3.0/customtkinterx/tk_dragtool.py
+-rw-r--r--   0        0        0      343 2023-06-04 08:35:41.539551 customtkinterx-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3686 2023-06-03 06:54:12.682589 customtkinterx-0.3.0/README.md
+-rw-r--r--   0        0        0     4121 1970-01-01 00:00:00.000000 customtkinterx-0.3.0/PKG-INFO
```

### Comparing `customtkinterx-0.2.4/customtkinterx/__init__.py` & `customtkinterx-0.3.0/customtkinterx/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from customtkinterx.CTkCustom import CTkCustom
-from customtkinterx.CTkFluentTheme import fluent_theme, fluent_json as CTkFluentThemeJson, fluent_path as CTkFluentThemePath, use_fluent_theme as CTkFluentTheme
-from customtkinterx.CTkMinimalTheme import minimal_theme, minimal_json as CTkMinimalThemeJson, minimal_path as CTkMinimalThemePath, use_fluent_theme as CTkMinimalTheme
+from customtkinterx.CTkFluentTheme import use_fluent_theme as CTkFluentTheme
+from customtkinterx.CTkMinimalTheme import use_minimal_theme as CTkMinimalTheme
+from customtkinterx.CTkOffice2019Theme import use_office2019_theme as CTkOffice2019Theme
+from customtkinterx.CTkMaterialTheme import use_material_theme as CTkMaterialTheme
 
 from customtkinterx.CTkInfoBar import CTkInfoBar, NORMAL, CAUTION, CRITICAL
 from customtkinterx.CTkMegaMenuBar import CTkMegaMenuBar
 
 # From https://github.com/Akascape/CTkMenuBar
 from customtkinterx.CTkMenuBar import CTkMenuBar, CTkTitleMenu, CustomDropdownMenu as CTkCustomDropdownMenu
```

### Comparing `customtkinterx-0.2.4/customtkinterx/__main__.py` & `customtkinterx-0.3.0/customtkinterx/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from customtkinter import *
 from customtkinterx import *
 
-CTkMinimalTheme()
+CTkMaterialTheme()
 
 set_appearance_mode("dark")
 
 root = CTkCustom()
 root.title("CustomTkinterX")
 root.titlebar_title.configure(text="CustomTkinterX")
 root.create_sizegrip(True)
```

### Comparing `customtkinterx-0.2.4/customtkinterx/CTkCustom.py` & `customtkinterx-0.3.0/customtkinterx/CTkCustom.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 class CTkCustom(CTk):
     def __init__(self, title: str = "", advanced: bool = True, **kwargs):
         try:
             super().__init__(**kwargs)
         except:
             pass
         from sys import platform
-        from customtkinterx import CTkFluentThemePath
         if advanced:
             if platform == "win32":
                 if "CTkCustom" in ThemeManager.theme:
                     self.__transparent_color = ThemeManager.theme["CTkCustom"]["transparent_color"]
                 else:
                     self.__transparent_color = "#101010"
                 self.attributes("-transparentcolor", self.__transparent_color)
@@ -56,33 +55,41 @@
                                        )
         self.__frame_border.pack(fill="both", expand=True, padx=0, pady=0)
 
         self.__frame_title = CTkFrame(self.__frame_border, border_width=0, corner_radius=ThemeManager.theme["CTkFrame"]["corner_radius"]/2+2)
         self.__frame_title.pack(fill="x", side="top", padx=2, pady=2)
         self.bind_move(self.__frame_title)
 
-        self.__label_title = CTkLabel(self.__frame_title, text=title)
-        self.__label_title.pack(side="left", anchor="w", padx=10, pady=5)
-        self.bind_move(self.__label_title)
-
         self.title(title)
 
         self.maximized = False
 
+        if "CTkCustom" in ThemeManager.theme:
+            self.__frame_title._fg_color = ThemeManager.theme["CTkCustom"]["titlebar_color"]
+            self.__frame_title._draw()
+
+        self.__label_title = CTkLabel(self.__frame_title, text=title)
+        self.__label_title.pack(side="left", anchor="w", padx=10, pady=5)
+        self.bind_move(self.__label_title)
+
         self.__button_close = CTkButton(self.__frame_title, text="✕", width=30, height=30,
                                         command=lambda: self.destroy())
         self.__button_close.pack(side="right", anchor="e", padx=5, pady=5)
 
         self.__button_minimize = CTkButton(self.__frame_title, text="–", width=30, height=30,
                                            command=lambda: self.minimize())
         from sys import platform
         if platform == "win32":
             self.__button_minimize.pack(side="right", anchor="e", padx=5, pady=5)
 
         if "CTkCustom" in ThemeManager.theme:
+
+            self.__label_title._text_color = ThemeManager.theme["CTkCustom"]["title_color"]
+            self.__label_title._draw()
+
             self.__button_close._text_color = ThemeManager.theme["CTkCustom"]["closebutton_text_color"]
             self.__button_close._fg_color = ThemeManager.theme["CTkCustom"]["closebutton_color"]
             self.__button_close._hover_color = ThemeManager.theme["CTkCustom"]["closebutton_hover_color"]
             self.__button_close._draw()
 
             self.__button_minimize._text_color = ThemeManager.theme["CTkCustom"]["minimizebutton_text_color"]
             self.__button_minimize._fg_color = ThemeManager.theme["CTkCustom"]["minimizebutton_color"]
@@ -131,15 +138,19 @@
         self.sg_height = self.winfo_height()
 
     def _sizegrip_move(self, event: Event):
         from pyautogui import position
 
         dx = position()[0] - self.sg_cx
         dy = position()[1] - self.sg_cy
-        self.geometry(f"{self.sg_width + dx}x{self.sg_height + dy}+{self.sg_x}+{self.sg_y}")
+
+        try:
+            self.geometry(f"{self.sg_width + dx}x{self.sg_height + dy}+{self.sg_x}+{self.sg_y}")
+        except TypeError:
+            pass
 
     def create_sizegrip(self, custom: bool = False):
         from sys import platform
         if custom:
             from customtkinterx.tk_dragtool import bind_resize
             self.sizegrip = CTkButton(self.__frame_border, width=32, height=32, text="⚪")
             self.sizegrip.configure(cursor="sizing")
```

### Comparing `customtkinterx-0.2.4/customtkinterx/CTkFluentTheme.py` & `customtkinterx-0.3.0/customtkinterx/CTkFluentTheme.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 fluent_json = """
 {
   "CTkCustom": {
+    "titlebar_color": ["#ffffff", "#2c2c2c"],
+    "title_color": ["gray10", "#DCE4EE"],
+
     "transparent_color": "#101010",
 
     "closebutton_text_color": ["#000000", "#ffffff"],
     "closebutton_color": ["#ffffff", "#2c2c2c"],
     "closebutton_hover_color": ["#b40d1b", "#b40d1b"],
 
     "minimizebutton_text_color": ["#000000", "#ffffff"],
```

### Comparing `customtkinterx-0.2.4/customtkinterx/CTkInfoBar.py` & `customtkinterx-0.3.0/customtkinterx/CTkInfoBar.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.4/customtkinterx/CTkListBox.py` & `customtkinterx-0.3.0/customtkinterx/CTkListBox.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.4/customtkinterx/CTkMegaMenuBar.py` & `customtkinterx-0.3.0/customtkinterx/CTkMegaMenuBar.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from customtkinter import CTkFrame, ThemeManager, CTkLabel, CTkFont, CTkScrollableFrame, CTkButton
+from customtkinter import CTkFrame, ThemeManager, CTkLabel, CTkFont, CTkScrollableFrame, CTkButton, CTkToplevel
 from customtkinterx import CTkCustom
 
 
 class CTkMegaMenuBar(CTkFrame):
     def __init__(self, master=None, title: str = "Mega Menu", custom: CTkCustom = None, **kwargs):
         super().__init__(master, **kwargs)
 
@@ -26,64 +26,49 @@
 
     def show(self, **kwargs):
         self.pack(fill="y", side="left", padx=5, pady=5, ipadx=5, ipady=5)
         if self.__custom is not None:
             self.pack(padx=2, pady=0)
         self.pack_configure(**kwargs)
 
-    def create_menu(self, text="Menu", id: str | int = -1, **kwargs):
-        __button_menu = CTkButton(self.__scrolledframe_menus, width=30, text=text, anchor="w", **kwargs)
-        __button_menu._fg_color = self._fg_color
-        __button_menu._text_color = ThemeManager.theme["CTkLabel"]["text_color"]
-        __button_menu.pack(fill="x", side="top", padx=0, pady=5, ipadx=5, ipady=5)
-        __button_menu._draw()
-
-        if id == -1:
-
-            def generate_random_str(randomlength=16):
-                import random
-                """
-                生成一个指定长度的随机字符串
-                """
-                random_str = ''
-                base_str = 'ABCDEFGHIGKLMNOPQRSTUVWXYZabcdefghigklmnopqrstuvwxyz0123456789'
-                length = len(base_str) - 1
-                for i in range(randomlength):
-                    random_str += base_str[random.randint(0, length)]
-                return random_str
-
-            id = generate_random_str(8)
-
-        __button_menu.setvar("id", id)
-
-        self.__buttons[id] = __button_menu
-
-        return __button_menu
+    def add(self, menu):
+        menu.pack(fill="x", side="top", padx=0, pady=5, ipadx=5, ipady=5)
 
     @property
     def menus(self):
         return self.__buttons
 
     @property
     def title(self):
         return self.__label_title
 
     @property
     def menubar(self):
         return self.__scrolledframe_menus
 
 
+class CTkMegaMenu(CTkButton):
+    def __init__(self, master: CTkMegaMenuBar, text="Menu", width=30, **kwargs):
+        super().__init__(master.menubar, width=width, text=text, anchor="w", **kwargs)
+
+        self._fg_color = master._fg_color
+        self._text_color = ThemeManager.theme["CTkLabel"]["text_color"]
+        self._draw()
+
+
 if __name__ == '__main__':
-    from customtkinterx import CTkCustom, CTkMinimalTheme, CTkFluentTheme
+    from customtkinterx import CTkCustom, CTkMinimalTheme, CTkFluentTheme, CTkOffice2019Theme
 
-    CTkMinimalTheme()
+    CTkOffice2019Theme()
+    #CTkMinimalTheme()
     #CTkFluentTheme()
 
     root = CTkCustom(title="CTkMegaMenuBar")
     root.create_sizegrip()
 
     menubar = CTkMegaMenuBar(root.mainframe, custom=root)
     for menu in range(10):
-        _menu = menubar.create_menu("Menu"+str(menu))
+        _menu = CTkMegaMenu(menubar, text="Menu"+str(menu))
+        menubar.add(_menu)
     menubar.show()
 
     root.mainloop()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `customtkinterx-0.2.4/customtkinterx/CTkMenuBar/__pycache__/__init__.cpython-311.pyc` & `customtkinterx-0.3.0/customtkinterx/CTkMenuBar/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.4/customtkinterx/CTkMenuBar/__pycache__/dropdown_menu.cpython-311.pyc` & `customtkinterx-0.3.0/customtkinterx/CTkMenuBar/__pycache__/dropdown_menu.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.4/customtkinterx/CTkMenuBar/__pycache__/menu_bar.cpython-311.pyc` & `customtkinterx-0.3.0/customtkinterx/CTkMenuBar/__pycache__/menu_bar.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.4/customtkinterx/CTkMenuBar/__pycache__/title_menu_win.cpython-311.pyc` & `customtkinterx-0.3.0/customtkinterx/CTkMenuBar/__pycache__/title_menu_win.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.4/customtkinterx/CTkMenuBar/dropdown_menu.py` & `customtkinterx-0.3.0/customtkinterx/CTkMenuBar/dropdown_menu.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.4/customtkinterx/CTkMenuBar/menu_bar.py` & `customtkinterx-0.3.0/customtkinterx/CTkMenuBar/menu_bar.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.4/customtkinterx/CTkMenuBar/title_menu_win.py` & `customtkinterx-0.3.0/customtkinterx/CTkMenuBar/title_menu_win.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.4/customtkinterx/CTkMinimalTheme.py` & `customtkinterx-0.3.0/customtkinterx/CTkMinimalTheme.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 minimal_json = """
 {
   "CTkCustom": {
+    "titlebar_color": ["#f4f6f8", "#212b36"],
+    "title_color": ["gray10", "#DCE4EE"],
+
     "transparent_color": "#101010",
 
     "closebutton_text_color": ["#000000", "#ffffff"],
     "closebutton_color": ["#f4f6f8", "#212b36"],
     "closebutton_hover_color": ["#b40d1b", "#b40d1b"],
 
     "minimizebutton_text_color": ["#000000", "#ffffff"],
@@ -22,20 +25,21 @@
 
     "success_color": ["#86e8ab", "#1b806a"],
     "success_hover_color": ["#d8fbde", "#0a5554"],
     "caution_color": ["#ffd666", "#b76e00"],
     "caution_hover_color": ["#fff5cc", "#7a4100"],
     "critical_color": ["#ffac82", "#b71d18"],
     "critical_hover_color": ["#ffe9d5", "#7a0916"]
+
   },
   "CTk": {
-    "fg_color": ["#f8fafb", "#151c24"]
+    "fg_color": ["#f9fafb", "#161c24"]
   },
   "CTkToplevel": {
-    "fg_color": ["#f8fafb", "#151c24"]
+    "fg_color": ["#f9fafb", "#161c24"]
   },
   "CTkFrame": {
     "corner_radius": 10,
     "border_width": 1,
     "fg_color": ["#f9fafb", "#161c24"],
     "top_fg_color": ["#f4f6f8", "#212b36"],
     "border_color": ["#edeff1", "#212b36"]
@@ -195,13 +199,13 @@
     from customtkinter import set_default_color_theme
     _, __temp = mkstemp(suffix=".json")
     with open(__temp, "w") as __temp_file:
         __temp_file.write(minimal_json)
     return __temp
 
 
-def use_fluent_theme():
+def use_minimal_theme():
     from customtkinter import set_default_color_theme
     try:
         set_default_color_theme(minimal_path)
     except FileNotFoundError:
         set_default_color_theme(minimal_theme())
```

### Comparing `customtkinterx-0.2.4/customtkinterx/CTkPDFViewer/__pycache__/ctk_pdf_viewer.cpython-311.pyc` & `customtkinterx-0.3.0/customtkinterx/CTkPDFViewer/__pycache__/ctk_pdf_viewer.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.4/customtkinterx/CTkPDFViewer/ctk_pdf_viewer.py` & `customtkinterx-0.3.0/customtkinterx/CTkPDFViewer/ctk_pdf_viewer.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.4/customtkinterx/CTkTable/__pycache__/ctktable.cpython-311.pyc` & `customtkinterx-0.3.0/customtkinterx/CTkTable/__pycache__/ctktable.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.4/customtkinterx/CTkTable/ctktable.py` & `customtkinterx-0.3.0/customtkinterx/CTkTable/ctktable.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.4/customtkinterx/CTkToolTip/__pycache__/ctk_tooltip.cpython-311.pyc` & `customtkinterx-0.3.0/customtkinterx/CTkToolTip/__pycache__/ctk_tooltip.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.4/customtkinterx/CTkToolTip/ctk_tooltip.py` & `customtkinterx-0.3.0/customtkinterx/CTkToolTip/ctk_tooltip.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.4/customtkinterx/Fluent.json` & `customtkinterx-0.3.0/customtkinterx/Office2019.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9601426681783823%*

 * *Differences: {"'CTkButton'": "{'corner_radius': 0, 'border_width': 1, 'fg_color': ['#e5e5e5', '#3d3d3d'], "*

 * *                "'hover_color': ['#b2b2b2', '#151515'], 'text_color': {insert: [(1, '#ffffff')], "*

 * *                'delete: [0]}}',*

 * * "'CTkComboBox'": "{'corner_radius': 0, 'fg_color': ['#ffffff', '#2f2f2f'], 'border_color': "*

 * *                  "['#f3f3f3', '#949A9F']}",*

 * * "'CTkCustom'": "{'titlebar_color': ['#106ebe', '#106ebe'], 'title_color': ['#ffffff', '#ffffff']}",*

 * * "'CTkEntry'": "{'corner_radius': 0, 'fg_colo […]*

```diff
@@ -6,27 +6,27 @@
         ]
     },
     "CTkButton": {
         "border_color": [
             "#f3f3f3",
             "#949A9F"
         ],
-        "border_width": 0,
-        "corner_radius": 6,
+        "border_width": 1,
+        "corner_radius": 0,
         "fg_color": [
-            "#0067c0",
-            "#4cc2ff"
+            "#e5e5e5",
+            "#3d3d3d"
         ],
         "hover_color": [
-            "#1975c5",
-            "#48b2e9"
+            "#b2b2b2",
+            "#151515"
         ],
         "text_color": [
-            "#ffffff",
-            "#000000"
+            "#000000",
+            "#ffffff"
         ],
         "text_color_disabled": [
             "gray74",
             "gray60"
         ]
     },
     "CTkCheckbox": {
@@ -55,30 +55,30 @@
         "text_color_disabled": [
             "gray60",
             "gray45"
         ]
     },
     "CTkComboBox": {
         "border_color": [
-            "#f2f2f2",
-            "#303030"
+            "#f3f3f3",
+            "#949A9F"
         ],
         "border_width": 1,
         "button_color": [
             "#f2f2f2",
             "#565B5E"
         ],
         "button_hover_color": [
             "#f2f2f2",
             "#565B5E"
         ],
-        "corner_radius": 6,
+        "corner_radius": 0,
         "fg_color": [
-            "#F9F9FA",
-            "#343638"
+            "#ffffff",
+            "#2f2f2f"
         ],
         "text_color": [
             "gray10",
             "#ffffff"
         ],
         "text_color_disabled": [
             "gray50",
@@ -106,26 +106,34 @@
             "#cccccc",
             "#282828"
         ],
         "minimizebutton_text_color": [
             "#000000",
             "#ffffff"
         ],
+        "title_color": [
+            "#ffffff",
+            "#ffffff"
+        ],
+        "titlebar_color": [
+            "#106ebe",
+            "#106ebe"
+        ],
         "transparent_color": "#101010"
     },
     "CTkEntry": {
         "border_color": [
-            "#f2f2f2",
-            "#303030"
+            "#f3f3f3",
+            "#949A9F"
         ],
         "border_width": 1,
-        "corner_radius": 6,
+        "corner_radius": 0,
         "fg_color": [
-            "#F9F9FA",
-            "#343638"
+            "#ffffff",
+            "#2f2f2f"
         ],
         "placeholder_text_color": [
             "gray52",
             "gray62"
         ],
         "text_color": [
             "#000000",
@@ -151,15 +159,15 @@
     },
     "CTkFrame": {
         "border_color": [
             "#b0b2b2",
             "#424556"
         ],
         "border_width": 1,
-        "corner_radius": 8,
+        "corner_radius": 0,
         "fg_color": [
             "#ffffff",
             "#1c1c1c"
         ],
         "top_fg_color": [
             "#ffffff",
             "#2c2c2c"
@@ -280,24 +288,24 @@
     "CTkScrollableFrame": {
         "label_fg_color": [
             "gray78",
             "gray23"
         ]
     },
     "CTkScrollbar": {
-        "border_spacing": 4,
+        "border_spacing": 9,
         "button_color": [
             "gray55",
             "gray41"
         ],
         "button_hover_color": [
             "gray40",
             "gray53"
         ],
-        "corner_radius": 1000,
+        "corner_radius": 0,
         "fg_color": "transparent"
     },
     "CTkSegmentedButton": {
         "border_width": 2,
         "corner_radius": 6,
         "fg_color": [
             "#979DA2",
@@ -347,25 +355,25 @@
         ],
         "progress_color": [
             "gray40",
             "#AAB0B5"
         ]
     },
     "CTkSwitch": {
-        "border_width": 0.1,
+        "border_width": 1,
         "button_color": [
             "#f3f3f3",
             "#000000"
         ],
         "button_hover_color": [
             "#bfbfbf",
             "#050505"
         ],
-        "button_length": 0,
-        "corner_radius": 1000,
+        "button_length": 2,
+        "corner_radius": 8,
         "fg_color": [
             "#ededed",
             "#1d1d1d"
         ],
         "progress_color": [
             "#0067c0",
             "#4cc2ff"
@@ -377,19 +385,19 @@
         "text_color_disabled": [
             "gray60",
             "gray45"
         ]
     },
     "CTkTextbox": {
         "border_color": [
-            "#979DA2",
-            "#565B5E"
+            "#f3f3f3",
+            "#949A9F"
         ],
-        "border_width": 0,
-        "corner_radius": 6,
+        "border_width": 1,
+        "corner_radius": 0,
         "fg_color": [
             "#F9F9FA",
             "#1D1E1E"
         ],
         "scrollbar_button_color": [
             "gray55",
             "gray41"
```

### Comparing `customtkinterx-0.2.4/customtkinterx/LaunchMusix.py` & `customtkinterx-0.3.0/customtkinterx/LaunchMusix.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from tkinter import ttk
 from customtkinter import *
 from customtkinterx import *
 
 def run():
     from sys import platform
 
-    CTkMinimalTheme()
+    CTkOffice2019Theme()
 
     set_appearance_mode("system")
 
     tk_root = CTkCustom()
     tk_root.create_sizegrip()
     tk_root.wm_geometry(f"350x620")
```

### Comparing `customtkinterx-0.2.4/customtkinterx/Minimal.json` & `customtkinterx-0.3.0/customtkinterx/Minimal.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9947089947089948%*

 * *Differences: {"'CTkCustom'": "{'titlebar_color': ['#f4f6f8', '#212b36'], 'title_color': ['gray10', '#DCE4EE']}"}*

```diff
@@ -100,14 +100,22 @@
             "#dfe3e8",
             "#454f5b"
         ],
         "minimizebutton_text_color": [
             "#000000",
             "#ffffff"
         ],
+        "title_color": [
+            "gray10",
+            "#DCE4EE"
+        ],
+        "titlebar_color": [
+            "#f4f6f8",
+            "#212b36"
+        ],
         "transparent_color": "#101010"
     },
     "CTkEntry": {
         "border_color": [
             "#c4cdd5",
             "#637381"
         ],
```

### Comparing `customtkinterx-0.2.4/customtkinterx/tk_dragtool.py` & `customtkinterx-0.3.0/customtkinterx/tk_dragtool.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.4/README.md` & `customtkinterx-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.4/PKG-INFO` & `customtkinterx-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: customtkinterx
-Version: 0.2.4
+Version: 0.3.0
 Summary: extra widgets for customtkinter
 Author: XiangQinxi
 Author-email: XiangQinxi@outlook.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

