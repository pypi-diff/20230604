# Comparing `tmp/rico-0.1.0.tar.gz` & `tmp/rico-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rico-0.1.0.tar", last modified: Sat Jun  3 18:31:56 2023, max compression
+gzip compressed data, was "rico-0.2.0.tar", last modified: Sun Jun  4 14:23:14 2023, max compression
```

## Comparing `rico-0.1.0.tar` & `rico-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1070 2023-06-03 18:30:57.625474 rico-0.1.0/LICENSE
--rw-r--r--   0        0        0      706 2023-06-03 18:30:57.625474 rico-0.1.0/README.md
--rw-r--r--   0        0        0     2870 2023-06-03 18:31:56.350493 rico-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      585 2023-06-03 18:30:57.625474 rico-0.1.0/src/rico/__init__.py
--rw-r--r--   0        0        0     4384 2023-06-03 18:30:57.625474 rico-0.1.0/src/rico/_config.py
--rw-r--r--   0        0        0     5751 2023-06-03 18:30:57.625474 rico-0.1.0/src/rico/_container.py
--rw-r--r--   0        0        0    14615 2023-06-03 18:30:57.625474 rico-0.1.0/src/rico/_content.py
--rw-r--r--   0        0        0     7012 2023-06-03 18:30:57.625474 rico-0.1.0/src/rico/_html.py
--rw-r--r--   0        0        0      340 2023-06-03 18:30:57.625474 rico-0.1.0/src/rico/_version.py
--rw-r--r--   0        0        0       18 2023-06-03 18:30:57.625474 rico-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     1476 2023-06-03 18:30:57.625474 rico-0.1.0/tests/test__config.py
--rw-r--r--   0        0        0    10237 2023-06-03 18:30:57.625474 rico-0.1.0/tests/test__container.py
--rw-r--r--   0        0        0    17190 2023-06-03 18:30:57.625474 rico-0.1.0/tests/test__content.py
--rw-r--r--   0        0        0     9491 2023-06-03 18:30:57.625474 rico-0.1.0/tests/test__html.py
--rw-r--r--   0        0        0      730 2023-06-03 18:30:57.625474 rico-0.1.0/tests/test__version.py
--rw-r--r--   0        0        0     2189 1970-01-01 00:00:00.000000 rico-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-04 14:22:49.892705 rico-0.2.0/LICENSE
+-rw-r--r--   0        0        0      706 2023-06-04 14:22:49.892705 rico-0.2.0/README.md
+-rw-r--r--   0        0        0     2870 2023-06-04 14:23:14.717679 rico-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      491 2023-06-04 14:22:49.892705 rico-0.2.0/src/rico/__init__.py
+-rw-r--r--   0        0        0     5483 2023-06-04 14:22:49.892705 rico-0.2.0/src/rico/_config.py
+-rw-r--r--   0        0        0     5605 2023-06-04 14:22:49.892705 rico-0.2.0/src/rico/_container.py
+-rw-r--r--   0        0        0    14768 2023-06-04 14:22:49.892705 rico-0.2.0/src/rico/_content.py
+-rw-r--r--   0        0        0     7015 2023-06-04 14:22:49.892705 rico-0.2.0/src/rico/_html.py
+-rw-r--r--   0        0        0      340 2023-06-04 14:22:49.892705 rico-0.2.0/src/rico/_version.py
+-rw-r--r--   0        0        0       18 2023-06-04 14:22:49.892705 rico-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     1476 2023-06-04 14:22:49.892705 rico-0.2.0/tests/test__config.py
+-rw-r--r--   0        0        0    10247 2023-06-04 14:22:49.892705 rico-0.2.0/tests/test__container.py
+-rw-r--r--   0        0        0    17232 2023-06-04 14:22:49.896705 rico-0.2.0/tests/test__content.py
+-rw-r--r--   0        0        0     9501 2023-06-04 14:22:49.896705 rico-0.2.0/tests/test__html.py
+-rw-r--r--   0        0        0      730 2023-06-04 14:22:49.896705 rico-0.2.0/tests/test__version.py
+-rw-r--r--   0        0        0     2189 1970-01-01 00:00:00.000000 rico-0.2.0/PKG-INFO
```

### Comparing `rico-0.1.0/LICENSE` & `rico-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rico-0.1.0/README.md` & `rico-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `rico-0.1.0/pyproject.toml` & `rico-0.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Visualization",
     "Topic :: Text Processing",
     "Topic :: Text Processing :: Markup",
     "Topic :: Text Processing :: Markup :: HTML",
     "Topic :: Text Processing :: Markup :: Markdown",
 ]
-version = "0.1.0"
+version = "0.2.0"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 source = "https://github.com/e10v/rico"
 "release notes" = "https://github.com/e10v/rico/releases"
```

### Comparing `rico-0.1.0/src/rico/_config.py` & `rico-0.2.0/src/rico/_config.py`

 * *Files 24% similar despite different names*

```diff
@@ -47,23 +47,27 @@
     .dataframe th {
         font-weight: bold;
     }
 """)
 
 
 _global_config = {
+    "bootstrap_css": BOOTSTRAP_CSS,
+    "bootstrap_js": BOOTSTRAP_JS,
+    "dataframe_style": DATAFRAME_STYLE,
+    "image_format": "svg",
     "indent_html": False,
     "indent_space": "  ",
-    "strip_html": False,
-    "image_format": "svg",
     "inline_scripts": False,
     "inline_styles": False,
-    "bootstrap_css": BOOTSTRAP_CSS,
-    "bootstrap_js": "",
-    "dataframe_style": DATAFRAME_STYLE,
+    "meta_charset": "utf-8",
+    "meta_viewport": "width=device-width, initial-scale=1",
+    "strip_html": False,
+    "text_mono": False,
+    "text_wrap": False,
 }
 
 
 def get_config(param: str | None = None) -> Any:
     """Get global configuration.
 
     Args:
@@ -75,72 +79,92 @@
     config = _global_config.copy()
     if param is not None:
         return config[param]
     return config
 
 
 def set_config(
+    bootstrap_css: str | None = None,
+    bootstrap_js: str | None = None,
+    dataframe_style: str | None = None,
+    image_format: Literal["svg", "png"] | None = None,
     indent_html: bool | None = None,
     indent_space: str | None = None,
-    strip_html: bool | None = None,
-    image_format: Literal["svg", "png"] | None = None,
     inline_scripts: bool | None = None,
     inline_styles: bool | None = None,
-    bootstrap_css: str | None = None,
-    bootstrap_js: str | None = None,
-    dataframe_style: str | None = None,
+    meta_charset: str | None = None,
+    meta_viewport: str | None = None,
+    strip_html: bool | None = None,
+    text_mono: bool | None = None,
+    text_wrap: bool | None = None,
 ) -> None:
     """Set global configuration.
 
     Args:
-        indent_html: Indent HTML elements in serialization methods.
-        indent_space: Default indent space.
-        strip_html: Strip HTML elements in serialization methods.
-        image_format: Default chart image format.
-        inline_scripts: If True then scripts are loaded inline.
-        inline_styles: If True then styles are loaded inline.
         bootstrap_css: A link to a bootstrap css file.
             If empty then bootstrap css is not loaded.
         bootstrap_js: A link to a bootstrap javascript file.
             If empty then bootstrap javascript is not loaded.
         dataframe_style: A dataframe table stylesheet.
             If empty then it's not used.
+        image_format: Default chart image format.
+        indent_html: Indent HTML elements in serialization methods.
+        indent_space: Default indent space.
+        inline_scripts: If True then scripts are loaded inline.
+        inline_styles: If True then styles are loaded inline.
+        meta_charset: An HTML document charset.
+            If empty then it's not used.
+        meta_viewport: An HTML document viewport property.
+            If empty then it's not used.
+        strip_html: Strip HTML elements in serialization methods.
+        text_mono: Default value for the `mono` arg of the Text class.
+        text_wrap: Default value for the `wrap` arg of the Text class.
     """
     for param, value in locals().items():
         if value is not None:
             _global_config[param] = value
 
 
 @contextlib.contextmanager
 def config_context(
+    bootstrap_css: str | None = None,
+    bootstrap_js: str | None = None,
+    dataframe_style: str | None = None,
+    image_format: Literal["svg", "png"] | None = None,
     indent_html: bool | None = None,
     indent_space: str | None = None,
-    strip_html: bool | None = None,
-    image_format: Literal["svg", "png"] | None = None,
     inline_scripts: bool | None = None,
     inline_styles: bool | None = None,
-    bootstrap_css: str | None = None,
-    bootstrap_js: str | None = None,
-    dataframe_style: str | None = None,
+    meta_charset: str | None = None,
+    meta_viewport: str | None = None,
+    strip_html: bool | None = None,
+    text_mono: bool | None = None,
+    text_wrap: bool | None = None,
 ) -> Generator[None, Any, None]:
     """Context manager for configuration.
 
     Args:
-        indent_html: Indent HTML elements in serialization methods.
-        indent_space: Default indent space.
-        strip_html: Strip HTML elements in serialization methods.
-        image_format: Default chart image format.
-        inline_scripts: If True then scripts are loaded inline.
-        inline_styles: If True then styles are loaded inline.
         bootstrap_css: A link to a bootstrap css file.
             If empty then bootstrap css is not loaded.
         bootstrap_js: A link to a bootstrap javascript file.
             If empty then bootstrap javascript is not loaded.
         dataframe_style: A dataframe table stylesheet.
             If empty then it's not used.
+        image_format: Default chart image format.
+        indent_html: Indent HTML elements in serialization methods.
+        indent_space: Default indent space.
+        inline_scripts: If True then scripts are loaded inline.
+        inline_styles: If True then styles are loaded inline.
+        meta_charset: An HTML document charset.
+            If empty then it's not used.
+        meta_viewport: An HTML document viewport property.
+            If empty then it's not used.
+        strip_html: Strip HTML elements in serialization methods.
+        text_mono: Default value for the `mono` arg of the Text class.
+        text_wrap: Default value for the `wrap` arg of the Text class.
     """
     new_config = locals()
     old_config = get_config()
     set_config(**new_config)
 
     try:
         yield
```

### Comparing `rico-0.1.0/src/rico/_container.py` & `rico-0.2.0/src/rico/_container.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import rico._config
 import rico._content
 import rico._html
 
 
 if TYPE_CHECKING:
     from collections.abc import Callable, Iterable
-    from typing import Any, Concatenate, ParamSpec
+    from typing import Any, Concatenate, Literal, ParamSpec
 
     P = ParamSpec("P")
 
 
 def _append(
     content_type: type[rico._content.ContentBase],
     init: Callable[Concatenate[Any, P], None],
@@ -75,32 +75,28 @@
         container (Element): The <div> container element.
     """
     html: ET.Element
     head: ET.Element
     body: ET.Element
     container: ET.Element
 
-    def __init__(  # noqa: C901
+    def __init__(
         self,
         *objects: Any,
         title: str | None = None,
-        charset: str | None = "utf-8",
-        viewport: str | None = "width=device-width, initial-scale=1",
-        bootstrap: bool = True,
+        bootstrap: Literal["css", "full", "none"] = "css",
         extra_styles: Iterable[rico._content.Style] = (),
         extra_scripts: Iterable[rico._content.Script] = (),
         class_: str | None = "container",
     ):
         """Create an HTML document with content from arbitrary objects.
 
         Args:
             *objects: The objects which are used to create a content.
             title: The document title.
-            charset: The document charset.
-            viewport: The document viewport property.
             bootstrap: If True then Bootstrap included to the document.
             extra_styles: Extra styles to be included to the document.
             extra_scripts: Extra scripts to be included to the document.
             class_: The container class attribute.
         """
         super().__init__(*objects, class_=class_)
         self.html = ET.Element("html")
@@ -111,48 +107,45 @@
         self.body.append(self.container)
 
         if title is not None:
             title_element = ET.Element("title")
             title_element.text = title
             self.head.append(title_element)
 
-        if charset is not None:
-            self.head.append(ET.Element("meta", charset=charset))
-
-        if viewport is not None:
+        global_config = rico._config.get_config()
+        if global_config["meta_charset"]:
+            self.head.append(ET.Element("meta", charset=global_config["meta_charset"]))
+        if global_config["meta_viewport"]:
             self.head.append(ET.Element(
                 "meta",
                 name="viewport",
-                content=viewport,
+                content=global_config["meta_viewport"],
             ))
 
         styles : list[rico._content.Style] = []
         scripts : list[rico._content.Script] = []
-        global_config = rico._config.get_config()
-
-        if bootstrap:
-            if global_config["bootstrap_css"]:
-                styles.append(rico._content.Style(src=global_config["bootstrap_css"]))
-            if global_config["bootstrap_js"]:
-                scripts.append(rico._content.Script(src=global_config["bootstrap_js"]))
 
+        if bootstrap.lower() in {"css", "full"}:
+            styles.append(rico._content.Style(src=global_config["bootstrap_css"]))
+        if bootstrap.lower() == "full":
+            scripts.append(rico._content.Script(src=global_config["bootstrap_js"]))
         if global_config["dataframe_style"]:
             styles.append(rico._content.Style(text=global_config["dataframe_style"]))
 
         styles = [*styles, *extra_styles]
         scripts = [*scripts, *extra_scripts]
 
         for style in styles:
-            self.head.append(style.style)
+            self.head.append(style.container)
 
         for script in scripts:
             if script.footer:
-                self.body.append(script.script)
+                self.body.append(script.container)
             else:
-                self.head.append(script.script)
+                self.head.append(script.container)
 
     def serialize(
         self,
         indent: bool | None = None,
         space: str | None = None,
         strip: bool | None = None,
     ) -> str:
```

### Comparing `rico-0.1.0/src/rico/_content.py` & `rico-0.2.0/src/rico/_content.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,16 +121,16 @@
     """A Text content definition.
 
     Creates a content element from a text and appends it to the container.
     """
     def __init__(
         self,
         obj: Any,
-        mono: bool = False,
-        wrap: bool = False,
+        mono: bool | None = None,
+        wrap: bool | None = None,
         class_: str | None = None,
     ):
         """Create content from a text.
 
         The default tag is <p> unless the text contains a line break.
         Then the <pre> tag is used.
 
@@ -140,14 +140,20 @@
             obj: The text. If it's not an instance of str, then it's converted to str.
             mono: If True then "font-monospace" class is assigned to the text element.
             wrap: If True then "text-wrap" class is assigned to the text element.
             class_: The container class attribute.
         """
         super().__init__(class_)
 
+        global_config = rico._config.get_config()
+        if mono is None:
+            mono = global_config["text_mono"]
+        if wrap is None:
+            wrap = global_config["text_wrap"]
+
         if not isinstance(obj, str):
             obj = str(obj)
 
         text_class = " ".join([
             cl
             for cond, cl in [(mono, "font-monospace"), (wrap, "text-wrap")]
             if cond
@@ -373,15 +379,15 @@
     """A script definition.
 
     Attributes:
         script (Element): The script element.
         footer (bool): Defines whether the script should be placed at a document footer,
             aftert all other content.
     """
-    script: ET.Element
+    container: ET.Element
     footer: bool = False
 
     def __init__(
         self,
         text: str | None = None,
         src: str | None = None,
         inline: bool | None = None,
@@ -424,26 +430,25 @@
         if src is not None:
             attrib = {"src": src, **attrib}
             if defer:
                 attrib = {"defer": True, **attrib}
         else:
             self.footer = defer
 
-        self.script = ET.Element("script", {**attrib, **extra})
-        self.script.text = text
-        self.container = self.script
+        self.container = ET.Element("script", {**attrib, **extra})
+        self.container.text = text
 
 
 class Style(ContentBase):
     """A stylesheet definition.
 
     Attributes:
         style (Element): The style element.
     """
-    style: ET.Element
+    container: ET.Element
 
     def __init__(
         self,
         text: str | None = None,
         src: str | None = None,
         inline: bool | None = None,
         attrib: dict[str, Any] = {},
@@ -483,10 +488,9 @@
             tag = "link"
             attrib = {"src": src, **attrib}
             if "rel" not in attrib:
                 attrib = {**attrib, "rel": "stylesheet"}
         else:
             tag = "style"
 
-        self.style = ET.Element(tag, {**attrib, **extra})
-        self.style.text = text
-        self.container = self.style
+        self.container = ET.Element(tag, {**attrib, **extra})
+        self.container.text = text
```

### Comparing `rico-0.1.0/src/rico/_html.py` & `rico-0.2.0/src/rico/_html.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,21 +47,21 @@
 
     def handle_endtag(self, tag: str) -> None:
         self._builder.end(tag)
 
     def handle_data(self, data: str) -> None:
         self._builder.data(data)
 
-    def close(self) -> list[ET.Element]:
+    def close(self) -> tuple[ET.Element]:
         super().close()
         self._builder.end(self._root)
-        return list(self._builder.close())
+        return tuple(self._builder.close())
 
 
-def parse_html(data: str) -> list[ET.Element]:
+def parse_html(data: str) -> tuple[ET.Element]:
     """Parse an HTML document from a string.
 
     Assign None values to boolean attributes.
 
     Ignore comments, doctype declaration and processing instructions.
     Convert attribute names to lower case, even for SVG.
```

### Comparing `rico-0.1.0/tests/test__config.py` & `rico-0.2.0/tests/test__config.py`

 * *Files identical despite different names*

### Comparing `rico-0.1.0/tests/test__container.py` & `rico-0.2.0/tests/test__container.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,39 +22,39 @@
     assert isinstance(div0, ET.Element)
     assert div0.tag == "div"
     assert div0.attrib == {"class": "row"}
     assert div0.text is None
     assert div0.tail is None
     assert len(div0) == 2
 
-    div1 = list(div0)[0]
+    div1 = tuple(div0)[0]
     assert isinstance(div1, ET.Element)
     assert div1.tag == "div"
     assert div1.attrib == {}
     assert div1.text is None
     assert div1.tail is None
     assert len(div1) == 1
 
-    p = list(div1)[0]
+    p = tuple(div1)[0]
     assert isinstance(p, ET.Element)
     assert p.tag == "p"
     assert p.attrib == {}
     assert p.text == "Hello world"
     assert p.tail is None
     assert len(p) == 0
 
-    div2 = list(div0)[1]
+    div2 = tuple(div0)[1]
     assert isinstance(div2, ET.Element)
     assert div2.tag == "div"
     assert div2.attrib == {"class": "col"}
     assert div2.text is None
     assert div2.tail is None
     assert len(div2) == 1
 
-    h1 = list(div2)[0]
+    h1 = tuple(div2)[0]
     assert isinstance(h1, ET.Element)
     assert h1.tag == "h1"
     assert h1.attrib == {}
     assert h1.text == "Header"
     assert h1.tail is None
     assert len(h1) == 0
 
@@ -138,213 +138,213 @@
     assert html.tag == "html"
     assert html.attrib == {}
     assert html.text is None
     assert html.tail is None
     assert len(html) == 2
 
     head = doc.head
-    assert head == list(html)[0]
+    assert head == tuple(html)[0]
     assert isinstance(head, ET.Element)
     assert head.tag == "head"
     assert head.attrib == {}
     assert head.text is None
     assert head.tail is None
     assert len(head) == 4
 
-    charset = list(head)[0]
+    charset = tuple(head)[0]
     assert isinstance(charset, ET.Element)
     assert charset.tag == "meta"
     assert charset.attrib == {"charset": "utf-8"}
     assert charset.text is None
     assert charset.tail is None
     assert len(charset) == 0
 
-    viewport = list(head)[1]
+    viewport = tuple(head)[1]
     assert isinstance(viewport, ET.Element)
     assert viewport.tag == "meta"
     assert viewport.attrib == {
         "name": "viewport",
         "content": "width=device-width, initial-scale=1",
     }
     assert viewport.text is None
     assert viewport.tail is None
     assert len(viewport) == 0
 
-    bootstrap_css = list(head)[2]
+    bootstrap_css = tuple(head)[2]
     assert isinstance(bootstrap_css, ET.Element)
     assert bootstrap_css.tag == "link"
     assert bootstrap_css.attrib == {
         "src": rico._config.BOOTSTRAP_CSS,
         "rel": "stylesheet",
     }
     assert bootstrap_css.text is None
     assert bootstrap_css.tail is None
     assert len(bootstrap_css) == 0
 
-    df_style = list(head)[3]
+    df_style = tuple(head)[3]
     assert isinstance(df_style, ET.Element)
     assert df_style.tag == "style"
     assert df_style.attrib == {}
     assert df_style.text == rico._config.DATAFRAME_STYLE
     assert df_style.tail is None
     assert len(df_style) == 0
 
     body = doc.body
-    assert body == list(html)[1]
+    assert body == tuple(html)[1]
     assert isinstance(body, ET.Element)
     assert body.tag == "body"
     assert body.attrib == {}
     assert body.text is None
     assert body.tail is None
     assert len(body) == 1
 
     div0 = doc.container
-    assert div0 == list(body)[0]
+    assert div0 == tuple(body)[0]
     assert isinstance(div0, ET.Element)
     assert div0.tag == "div"
     assert div0.attrib == {"class": "container"}
     assert div0.text is None
     assert div0.tail is None
     assert len(div0) == 1
 
-    div1 = list(div0)[0]
+    div1 = tuple(div0)[0]
     assert isinstance(div1, ET.Element)
     assert div1.tag == "div"
     assert div1.attrib == {}
     assert div1.text is None
     assert div1.tail is None
     assert len(div1) == 1
 
-    p = list(div1)[0]
+    p = tuple(div1)[0]
     assert isinstance(p, ET.Element)
     assert p.tag == "p"
     assert p.attrib == {}
     assert p.text == "Hello world"
     assert p.tail is None
     assert len(p) == 0
 
 
 def test_doc_init_nondefault():  # noqa: PLR0915
     extra_style = rico._content.Style(src="style.css")
     extra_script = rico._content.Script(text="alert('Hello World!');")
     extra_script.footer = True
 
     with rico._config.config_context(
-        bootstrap_js=rico._config.BOOTSTRAP_JS,
+        meta_charset="",
+        meta_viewport="",
         dataframe_style="",
     ):
         doc = rico._container.Doc(
             "Hello world",
             title="Title",
-            charset=None,
-            viewport=None,
+           bootstrap="full",
             extra_styles=(extra_style,),
             extra_scripts=(extra_script,),
             class_=None,
         )
 
     html = doc.html
     assert isinstance(html, ET.Element)
     assert html.tag == "html"
     assert html.attrib == {}
     assert html.text is None
     assert html.tail is None
     assert len(html) == 2
 
     head = doc.head
-    assert head == list(html)[0]
+    assert head == tuple(html)[0]
     assert isinstance(head, ET.Element)
     assert head.tag == "head"
     assert head.attrib == {}
     assert head.text is None
     assert head.tail is None
     assert len(head) == 4
 
-    title = list(head)[0]
+    title = tuple(head)[0]
     assert isinstance(title, ET.Element)
     assert title.tag == "title"
     assert title.attrib == {}
     assert title.text == "Title"
     assert title.tail is None
     assert len(title) == 0
 
-    bootstrap_css = list(head)[1]
+    bootstrap_css = tuple(head)[1]
     assert isinstance(bootstrap_css, ET.Element)
     assert bootstrap_css.tag == "link"
     assert bootstrap_css.attrib == {
         "src": rico._config.BOOTSTRAP_CSS,
         "rel": "stylesheet",
     }
     assert bootstrap_css.text is None
     assert bootstrap_css.tail is None
     assert len(bootstrap_css) == 0
 
-    style = list(head)[2]
-    style = extra_style.style
+    style = tuple(head)[2]
+    style = extra_style.container
     assert isinstance(style, ET.Element)
     assert style.tag == "link"
     assert style.attrib == {"src": "style.css", "rel": "stylesheet"}
     assert style.text is None
     assert style.tail is None
     assert len(style) == 0
 
-    bootstrap_js = list(head)[3]
+    bootstrap_js = tuple(head)[3]
     assert isinstance(bootstrap_js, ET.Element)
     assert bootstrap_js.tag == "script"
     assert bootstrap_js.attrib == {"src": rico._config.BOOTSTRAP_JS}
     assert bootstrap_js.text is None
     assert bootstrap_js.tail is None
     assert len(bootstrap_js) == 0
 
     body = doc.body
-    assert body == list(html)[1]
+    assert body == tuple(html)[1]
     assert isinstance(body, ET.Element)
     assert body.tag == "body"
     assert body.attrib == {}
     assert body.text is None
     assert body.tail is None
     assert len(body) == 2
 
     div0 = doc.container
-    assert div0 == list(body)[0]
+    assert div0 == tuple(body)[0]
     assert isinstance(div0, ET.Element)
     assert div0.tag == "div"
     assert div0.attrib == {}
     assert div0.text is None
     assert div0.tail is None
     assert len(div0) == 1
 
-    div1 = list(div0)[0]
+    div1 = tuple(div0)[0]
     assert isinstance(div1, ET.Element)
     assert div1.tag == "div"
     assert div1.attrib == {}
     assert div1.text is None
     assert div1.tail is None
     assert len(div1) == 1
 
-    p = list(div1)[0]
+    p = tuple(div1)[0]
     assert isinstance(p, ET.Element)
     assert p.tag == "p"
     assert p.attrib == {}
     assert p.text == "Hello world"
     assert p.tail is None
     assert len(p) == 0
 
-    script = list(body)[1]
-    assert script == extra_script.script
+    script = tuple(body)[1]
+    assert script == extra_script.container
     assert isinstance(script, ET.Element)
     assert script.tag == "script"
     assert script.attrib == {}
     assert script.text  == "alert('Hello World!');"
     assert script.tail is None
     assert len(script) == 0
 
 
 def test_doc_serialize():
     with rico._config.config_context(dataframe_style=""):
-        doc = rico._container.Doc("Hello world", bootstrap=False)
+        doc = rico._container.Doc("Hello world", bootstrap="none")
 
     assert doc.serialize() == (
         '<!doctype html>\n<html><head><meta charset="utf-8">'
         '<meta name="viewport" content="width=device-width, initial-scale=1"></head>'
         '<body><div class="container"><div><p>Hello world</p></div></div></body></html>'
     )
```

### Comparing `rico-0.1.0/tests/test__content.py` & `rico-0.2.0/tests/test__content.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,15 +112,15 @@
     assert isinstance(div, ET.Element)
     assert div.tag == "div"
     assert div.attrib == {"class": "row"}
     assert div.text is None
     assert div.tail is None
     assert len(div) == 1
 
-    p = list(div)[0]
+    p = tuple(div)[0]
     assert isinstance(p, ET.Element)
     assert p.tag == "p"
     assert p.attrib == {"class": "col", "id": "42"}
     assert p.text == "Hello"
     assert p.tail == "world"
     assert len(p) == 0
 
@@ -132,41 +132,41 @@
     assert isinstance(div, ET.Element)
     assert div.tag == "div"
     assert div.attrib == {"class": "row"}
     assert div.text is None
     assert div.tail is None
     assert len(div) == 1
 
-    p = list(div)[0]
+    p = tuple(div)[0]
     assert isinstance(p, ET.Element)
     assert p.tag == "p"
     assert p.attrib == {}
     assert p.text == "Hello world"
     assert p.tail is None
     assert len(p) == 0
 
 
 def test_text_pre_mono():
     content = rico._content.Text("Hello\nworld", mono=True)
     div = content.container
 
-    pre = list(div)[0]
+    pre = tuple(div)[0]
     assert isinstance(pre, ET.Element)
     assert pre.tag == "pre"
     assert pre.attrib == {"class": "font-monospace"}
     assert pre.text == "Hello\nworld"
     assert pre.tail is None
     assert len(pre) == 0
 
 
 def test_text_int_mono_wrap():
     content = rico._content.Text(42, mono=True, wrap=True)
     div = content.container
 
-    p = list(div)[0]
+    p = tuple(div)[0]
     assert isinstance(p, ET.Element)
     assert p.tag == "p"
     assert p.attrib == {"class": "font-monospace text-wrap"}
     assert p.text == "42"
     assert p.tail is None
     assert len(p) == 0
 
@@ -178,23 +178,23 @@
     assert isinstance(div, ET.Element)
     assert div.tag == "div"
     assert div.attrib == {"class": "row"}
     assert div.text is None
     assert div.tail is None
     assert len(div) == 1
 
-    pre = list(div)[0]
+    pre = tuple(div)[0]
     assert isinstance(pre, ET.Element)
     assert pre.tag == "pre"
     assert pre.attrib == {}
     assert pre.text is None
     assert pre.tail is None
     assert len(pre) == 1
 
-    code = list(pre)[0]
+    code = tuple(pre)[0]
     assert isinstance(code, ET.Element)
     assert code.tag == "code"
     assert code.attrib == {}
     assert code.text == "Hello world"
     assert code.tail is None
     assert len(code) == 0
 
@@ -206,15 +206,15 @@
     assert isinstance(div, ET.Element)
     assert div.tag == "div"
     assert div.attrib == {"class": "row"}
     assert div.text is None
     assert div.tail is None
     assert len(div) == 1
 
-    p = list(div)[0]
+    p = tuple(div)[0]
     assert isinstance(p, ET.Element)
     assert p.tag == "p"
     assert p.attrib == {"border": "1"}
     assert p.text == "Hello world"
     assert p.tail is None
     assert len(p) == 0
 
@@ -240,18 +240,18 @@
     )
 
     if wrap_in_div:
         df = f"<div>{df}</div>"
 
     content = rico._content.HTML(df, strip_dataframe_borders)
     if wrap_in_div:
-        div = list(content.container)[0]
-        table = list(div)[0]
+        div = tuple(content.container)[0]
+        table = tuple(div)[0]
     else:
-        table = list(content.container)[0]
+        table = tuple(content.container)[0]
 
     if border and (not dataframe or not strip_dataframe_borders):
         assert table.get("border") == "1"
     else:
         assert table.get("border", "no border") == "no border"
 
 
@@ -268,31 +268,31 @@
     assert isinstance(div, ET.Element)
     assert div.tag == "div"
     assert div.attrib == {"class": "row"}
     assert div.text is None
     assert div.tail is None
     assert len(div) == 3
 
-    h1 = list(div)[0]
+    h1 = tuple(div)[0]
     assert isinstance(h1, ET.Element)
     assert h1.tag == "h1"
     assert h1.attrib == {}
     assert h1.text == "Header 1"
     assert h1.tail == "\n"
     assert len(h1) == 0
 
-    h2 = list(div)[1]
+    h2 = tuple(div)[1]
     assert isinstance(h2, ET.Element)
     assert h2.tag == "h2"
     assert h2.attrib == {}
     assert h2.text == "Header 2"
     assert h2.tail == "\n"
     assert len(h2) == 0
 
-    p = list(div)[2]
+    p = tuple(div)[2]
     assert isinstance(p, ET.Element)
     assert p.tag == "p"
     assert p.attrib == {}
     assert p.text == "Hello world"
     assert p.tail is None
     assert len(p) == 0
 
@@ -321,30 +321,30 @@
     assert isinstance(div, ET.Element)
     assert div.tag == "div"
     assert div.attrib == {"class": "row"}
     assert div.text is None
     assert div.tail is None
     assert len(div) == 1
 
-    svg = list(div)[0]
+    svg = tuple(div)[0]
     assert isinstance(svg, ET.Element)
     assert svg.tag == "svg"
     assert svg.attrib == {
         "xmlns": "http://www.w3.org/2000/svg",
         "xmlns:xlink": "http://www.w3.org/1999/xlink",
         "width": "16",
         "height": "16",
         "fill": "currentColor",
         "class": "bi bi-dash",
     }
     assert svg.text is None
     assert svg.tail is None
     assert len(svg) == 1
 
-    path = list(svg)[0]
+    path = tuple(svg)[0]
     assert isinstance(path, ET.Element)
     assert path.tag == "path"
     assert path.attrib == {
         "d": "M4 8a.5.5 0 0 1 .5-.5h7a.5.5 0 0 1 0 1h-7A.5.5 0 0 1 4 8z",
     }
     assert path.text is None
     assert path.tail is None
@@ -363,15 +363,15 @@
     assert isinstance(div, ET.Element)
     assert div.tag == "div"
     assert div.attrib == {}
     assert div.text is None
     assert div.tail is None
     assert len(div) == 1
 
-    img = list(div)[0]
+    img = tuple(div)[0]
     assert isinstance(img, ET.Element)
     assert img.tag == "img"
     assert img.attrib == {"src": f"data:image/png;base64,{encoded_image}"}
     assert img.text is None
     assert img.tail is None
     assert len(img) == 0
 
@@ -405,19 +405,19 @@
     assert div.tag == "div"
     assert div.attrib == {"class": "row"}
     assert div.text is None
     assert div.tail is None
     assert len(div) == 1
 
     if format is None:
-        svg = list(div)[0]
+        svg = tuple(div)[0]
         assert isinstance(svg, ET.Element)
         assert svg.tag == "svg"
     else:
-        img = list(div)[0]
+        img = tuple(div)[0]
         assert isinstance(img, ET.Element)
         assert img.tag == "img"
 
 
 @pytest.mark.parametrize(
     ("module", "err_chart", "chart"),
     [
@@ -448,42 +448,42 @@
     assert isinstance(div, ET.Element)
     assert div.tag == "div"
     assert div.attrib == {"class": "row"}
     assert div.text is None
     assert div.tail is None
     assert len(div) == 3
 
-    h1 = list(div)[0]
+    h1 = tuple(div)[0]
     assert isinstance(h1, ET.Element)
     assert h1.tag == "h1"
     assert h1.attrib == {}
     assert h1.text == "Hello"
     assert h1.tail is None
     assert len(h1) == 0
 
-    p = list(div)[1]
+    p = tuple(div)[1]
     assert isinstance(p, ET.Element)
     assert p.tag == "p"
     assert p.attrib == {}
     assert p.text == "world"
     assert p.tail is None
     assert len(p) == 0
 
-    svg = list(div)[2]
+    svg = tuple(div)[2]
     assert isinstance(svg, ET.Element)
     assert svg.tag == "svg"
 
 
 @pytest.mark.parametrize("defer", [True, False], ids=["defer", "not defer"])
 def test_script_text(defer: bool):
     text = "alert('Hello World!');"
     attrib = {"async": True}
     content = rico._content.Script(text=text, defer=defer, attrib=attrib)
 
-    script = content.script
+    script = content.container
     assert isinstance(script, ET.Element)
     assert script.tag == "script"
     assert script.attrib == attrib
     assert script.text == text
     assert script.tail is None
     assert len(script) == 0
 
@@ -497,15 +497,15 @@
     attrib = {"async": True}
     content = rico._content.Script(src=src, defer=defer, attrib=attrib)
 
     attrib = {"src": src, **attrib}
     if defer:
         attrib = {"defer": True, **attrib}
 
-    script = content.script
+    script = content.container
     assert isinstance(script, ET.Element)
     assert script.tag == "script"
     assert script.attrib == attrib
     assert script.text is None
     assert script.tail is None
     assert len(script) == 0
 
@@ -520,15 +520,15 @@
     attrib = {"async": True}
 
     with unittest.mock.patch("rico._content.urllib.request.urlopen") as urlopen:
         urlopen.return_value = io.BytesIO(text.encode())
         content = rico._content.Script(src=src, inline=True, defer=defer, attrib=attrib)
         urlopen.assert_called_once_with(src)
 
-    script = content.script
+    script = content.container
     assert isinstance(script, ET.Element)
     assert script.tag == "script"
     assert script.attrib == attrib
     assert script.text == text
     assert script.tail is None
     assert len(script) == 0
 
@@ -544,15 +544,15 @@
 
 
 def test_style_text():
     text = "p {color: red;}"
     attrib = {"title": "Style title"}
     content = rico._content.Style(text=text, attrib=attrib)
 
-    style = content.style
+    style = content.container
     assert isinstance(style, ET.Element)
     assert style.tag == "style"
     assert style.attrib == attrib
     assert style.text == text
     assert style.tail is None
     assert len(style) == 0
 
@@ -562,15 +562,15 @@
 def test_style_src():
     src = "style.css"
     attrib = {"crossorigin": "anonymous"}
     content = rico._content.Style(src=src, attrib=attrib)
 
     attrib = {"src": src, **attrib, "rel": "stylesheet"}
 
-    link = content.style
+    link = content.container
     assert isinstance(link, ET.Element)
     assert link.tag == "link"
     assert link.attrib == attrib
     assert link.text is None
     assert link.tail is None
     assert len(link) == 0
 
@@ -583,15 +583,15 @@
     attrib = {"title": "Style title"}
 
     with unittest.mock.patch("rico._content.urllib.request.urlopen") as urlopen:
         urlopen.return_value = io.BytesIO(text.encode())
         content = rico._content.Style(src=src, inline=True, attrib=attrib)
         urlopen.assert_called_once_with(src)
 
-    style = content.style
+    style = content.container
     assert isinstance(style, ET.Element)
     assert style.tag == "style"
     assert style.attrib == attrib
     assert style.text == text
     assert style.tail is None
     assert len(style) == 0
```

### Comparing `rico-0.1.0/tests/test__html.py` & `rico-0.2.0/tests/test__html.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,28 +4,28 @@
 import xml.etree.ElementTree as ET
 
 import pytest
 
 import rico._html
 
 
-def elem_to_string(elem: ET.Element | list[ET.Element], sep: str = "") -> str:
-    if isinstance(elem, list):
+def elem_to_string(elem: ET.Element | tuple[ET.Element], sep: str = "") -> str:
+    if isinstance(elem, tuple):
         return sep.join(elem_to_string(e) for e in elem)
     return ET.tostring(elem, encoding="unicode", method="html")
 
 
 def test_html_parser_two_elements():
     text = "<p>Hello</p><p>world</p>"
     parser = rico._html.HTMLParser()
     parser.feed(text)
     elements = parser.close()
 
     assert elem_to_string(elements) == text
-    assert isinstance(elements, list)
+    assert isinstance(elements, tuple)
     assert len(elements) == 2
 
     p0 = elements[0]
     assert isinstance(p0, ET.Element)
     assert p0.tag == "p"
     assert p0.attrib == {}
     assert p0.text == "Hello"
@@ -44,34 +44,34 @@
 def test_html_parser_nested_tags():
     text = "<div><p>Hello <strong>world</strong>!</p></div>"
     parser = rico._html.HTMLParser()
     parser.feed(text)
     elements = parser.close()
 
     assert elem_to_string(elements) == text
-    assert isinstance(elements, list)
+    assert isinstance(elements, tuple)
     assert len(elements) == 1
 
     div = elements[0]
     assert isinstance(div, ET.Element)
     assert div.tag == "div"
     assert div.attrib == {}
     assert div.text is None
     assert div.tail is None
     assert len(div) == 1
 
-    p = list(div)[0]
+    p = tuple(div)[0]
     assert isinstance(p, ET.Element)
     assert p.tag == "p"
     assert p.attrib == {}
     assert p.text == "Hello "
     assert p.tail is None
     assert len(p) == 1
 
-    strong = list(p)[0]
+    strong = tuple(p)[0]
     assert isinstance(strong, ET.Element)
     assert strong.tag == "strong"
     assert strong.attrib == {}
     assert strong.text == "world"
     assert strong.tail == "!"
     assert len(strong) == 0
 
@@ -79,15 +79,15 @@
 def test_html_parser_attributes():
     script_src = "https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha3/dist/js/bootstrap.bundle.min.js"
     text = f"<script defer src='{script_src}' crossorigin='anonymous'></script>"
     parser = rico._html.HTMLParser()
     parser.feed(text)
     elements = parser.close()
 
-    assert isinstance(elements, list)
+    assert isinstance(elements, tuple)
     assert len(elements) == 1
 
     script = elements[0]
     assert isinstance(script, ET.Element)
     assert script.tag == "script"
     assert script.attrib == {
         "defer": None,
@@ -107,15 +107,15 @@
         '<path d="M4 8a.5.5 0 0 1 .5-.5h7a.5.5 0 0 1 0 1h-7A.5.5 0 0 1 4 8z"/>'
         "</svg>"
     )
     parser = rico._html.HTMLParser()
     parser.feed(text)
     elements = parser.close()
 
-    assert isinstance(elements, list)
+    assert isinstance(elements, tuple)
     assert len(elements) == 1
 
     svg = elements[0]
     assert isinstance(svg, ET.Element)
     assert svg.tag == "svg"
     assert svg.attrib == {
         "xmlns": "http://www.w3.org/2000/svg",
@@ -125,15 +125,15 @@
         "fill": "currentColor",
         "class": "bi bi-dash",
     }
     assert svg.text is None
     assert svg.tail is None
     assert len(svg) == 1
 
-    path = list(svg)[0]
+    path = tuple(svg)[0]
     assert isinstance(path, ET.Element)
     assert path.tag == "path"
     assert path.attrib == {
         "d": "M4 8a.5.5 0 0 1 .5-.5h7a.5.5 0 0 1 0 1h-7A.5.5 0 0 1 4 8z",
     }
     assert path.text is None
     assert path.tail is None
@@ -141,15 +141,15 @@
 
 
 def test_parse_html():
     text = "<p>Hello world</p>"
     elements = rico._html.parse_html(text)
 
     assert elem_to_string(elements) == text
-    assert isinstance(elements, list)
+    assert isinstance(elements, tuple)
     assert len(elements) == 1
 
     p = elements[0]
     assert isinstance(p, ET.Element)
     assert p.tag == "p"
     assert p.attrib == {}
     assert p.text == "Hello world"
```

### Comparing `rico-0.1.0/tests/test__version.py` & `rico-0.2.0/tests/test__version.py`

 * *Files identical despite different names*

### Comparing `rico-0.1.0/PKG-INFO` & `rico-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rico
-Version: 0.1.0
+Version: 0.2.0
 Summary: Rich content to HTML as easy as Doc(df, plot).
 Author-Email: Evgeny Ivanov <ivanov.evgeny.n@gmail.com>
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

