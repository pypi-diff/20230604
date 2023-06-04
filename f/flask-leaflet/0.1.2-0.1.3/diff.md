# Comparing `tmp/flask_leaflet-0.1.2.tar.gz` & `tmp/flask_leaflet-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_leaflet-0.1.2.tar", last modified: Thu May 18 06:46:54 2023, max compression
+gzip compressed data, was "flask_leaflet-0.1.3.tar", last modified: Sun Jun  4 06:48:05 2023, max compression
```

## Comparing `flask_leaflet-0.1.2.tar` & `flask_leaflet-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,15 @@
--rwxr-xr-x   0        0        0     4478 2023-05-18 06:24:55.459001 flask_leaflet-0.1.2/README.md
--rwxr-xr-x   0        0        0     2677 2023-05-18 06:39:38.258949 flask_leaflet-0.1.2/flask_leaflet/__init__.py
--rwxr-xr-x   0        0        0     1593 2023-05-14 08:31:30.463333 flask_leaflet-0.1.2/flask_leaflet/basic_types.py
--rwxr-xr-x   0        0        0        0 2023-05-11 15:07:50.000000 flask_leaflet-0.1.2/flask_leaflet/layers/__init__.py
--rwxr-xr-x   0        0        0     1018 2023-05-18 04:18:13.595361 flask_leaflet-0.1.2/flask_leaflet/layers/base.py
--rwxr-xr-x   0        0        0     5030 2023-05-18 04:33:07.698015 flask_leaflet-0.1.2/flask_leaflet/layers/paths.py
--rwxr-xr-x   0        0        0     9359 2023-05-15 05:42:11.854584 flask_leaflet-0.1.2/flask_leaflet/layers/raster.py
--rwxr-xr-x   0        0        0     8981 2023-05-15 06:37:46.212225 flask_leaflet-0.1.2/flask_leaflet/layers/ui.py
--rwxr-xr-x   0        0        0     2551 2023-05-18 06:27:35.626652 flask_leaflet-0.1.2/flask_leaflet/map.py
--rwxr-xr-x   0        0        0     2169 2023-05-15 06:17:34.702685 flask_leaflet-0.1.2/flask_leaflet/mixins.py
--rwxr-xr-x   0        0        0     1466 2023-05-14 03:46:14.846425 flask_leaflet-0.1.2/flask_leaflet/static/images/marker-icon.png
--rwxr-xr-x   0        0        0      618 2023-05-14 03:46:19.848035 flask_leaflet-0.1.2/flask_leaflet/static/images/marker-shadow.png
--rwxr-xr-x   0        0        0     1321 2023-05-14 07:53:24.704663 flask_leaflet-0.1.2/flask_leaflet/templates/dict_as_json.jinja
--rwxr-xr-x   0        0        0      518 2023-05-15 06:24:24.745973 flask_leaflet-0.1.2/flask_leaflet/templates/factory.html
--rwxr-xr-x   0        0        0      981 2023-05-18 06:39:27.827607 flask_leaflet-0.1.2/flask_leaflet/templates/load.html
--rwxr-xr-x   0        0        0      517 2023-05-18 06:46:02.709535 flask_leaflet-0.1.2/flask_leaflet/templates/map.html
--rwxr-xr-x   0        0        0      366 2023-05-18 06:46:54.377132 flask_leaflet-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     4705 1970-01-01 00:00:00.000000 flask_leaflet-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     4627 2023-06-04 06:47:53.616061 flask_leaflet-0.1.3/README.md
+-rw-r--r--   0        0        0     2925 2023-06-04 06:47:53.616061 flask_leaflet-0.1.3/flask_leaflet/__init__.py
+-rw-r--r--   0        0        0     4916 2023-06-04 06:47:53.616061 flask_leaflet-0.1.3/flask_leaflet/basic_types.py
+-rw-r--r--   0        0        0        0 2023-06-04 06:47:53.616061 flask_leaflet-0.1.3/flask_leaflet/layers/__init__.py
+-rw-r--r--   0        0        0     2340 2023-06-04 06:47:53.620061 flask_leaflet-0.1.3/flask_leaflet/layers/base.py
+-rw-r--r--   0        0        0     5024 2023-06-04 06:47:53.620061 flask_leaflet-0.1.3/flask_leaflet/layers/paths.py
+-rw-r--r--   0        0        0     9254 2023-06-04 06:47:53.620061 flask_leaflet-0.1.3/flask_leaflet/layers/raster.py
+-rw-r--r--   0        0        0    11061 2023-06-04 06:47:53.620061 flask_leaflet-0.1.3/flask_leaflet/layers/ui.py
+-rw-r--r--   0        0        0     3496 2023-06-04 06:47:53.620061 flask_leaflet-0.1.3/flask_leaflet/map.py
+-rw-r--r--   0        0        0     4118 2023-06-04 06:47:53.620061 flask_leaflet-0.1.3/flask_leaflet/mixins.py
+-rw-r--r--   0        0        0     1466 2023-06-04 06:47:53.620061 flask_leaflet-0.1.3/flask_leaflet/static/images/marker-icon.png
+-rw-r--r--   0        0        0      618 2023-06-04 06:47:53.620061 flask_leaflet-0.1.3/flask_leaflet/static/images/marker-shadow.png
+-rw-r--r--   0        0        0      976 2023-06-04 06:47:53.620061 flask_leaflet-0.1.3/flask_leaflet/templates/load.html
+-rw-r--r--   0        0        0      366 2023-06-04 06:48:05.648176 flask_leaflet-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     4854 1970-01-01 00:00:00.000000 flask_leaflet-0.1.3/PKG-INFO
```

### Comparing `flask_leaflet-0.1.2/README.md` & `flask_leaflet-0.1.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -37,26 +37,25 @@
 
 Once installed Flask-Leaflet is easy to use. Let's walk through setting up a basic application. Also please note that this is a very basic guide: we will be taking shortcuts here that you should never take in a real application.
 
 To begin we'll set up a Flask app:
 
 ```python
 from flask import Flask
-
 from flask_leaflet import Leaflet
 
 app = Flask(__name__)
 
 leaflet = Leaflet()
 leaflet.init_app(app)
 ```
 
 ### Load resources
 
-Once the extension is set up, this will make available the `leaflet` object into the templates context so you could load the javascript package easily, like this.
+Once the extension is set up, this will make available the `leaflet` object into the templates context so you could load the javascript and css package easily, like this.
 
 ```html
 <head>
   {{ leaflet.load() }}
 </head>
 ```
 
@@ -74,20 +73,21 @@
     # Using snake_case for the options.
     my_map = Map('my-map', center=[-41.139416, -73.025431], zoom=16)
     return render('my_map.html', my_map=my_map)
 ```
 
 ### Rendering the map
 
-Now that we have a Map instance we can render it in a template. **IMPORTANT:** The map container **Must have a Height** given by a class added on the `class_` arguments.
+Now that we have a Map instance we can render it in a template. **IMPORTANT:** The map container **Must have a Height** given the special `class_` argument. Also you got access to `nonce_` in case you need to add a nonce token to the script tag.
+in the next example we use `tailwindcss` class for a 200px height
 
 ```html
 <head>
   <!-- You can add custom options at this instance that will overwrite any defaults coming from the view. Note that using class_='h-200px' we stablish a minimum height otherwise the map wouldnt be visible. -->
-  {{ leaflet.render_map(my_map, class_='h-[200px]' zoom=10) }}
+  {{ leaflet.render_map(my_map, class_='h-[200px]', zoom=10) }}
 </head>
 ```
 
 ### What about RasterLayers
 
 If you need to use a RasterTile style for every map you could stablish in your configuration the url_template and options for the default raster. Doing this will automatically be seted up for every map rendered.
 
@@ -102,36 +102,36 @@
 or
 
 ```python
 from flask_leaflet.layers.raster import TileLayer
 # ...
 my_map = Map('my-map', center=[-41.139416, -73.025431], zoom=16)
 tile_layer = TileLayer(r"https://server.arcgisonline.com/ArcGIS/rest/services/World_Imagery/MapServer/tile/{z}/{y}/{x}", max_zoom=15, min_zoom=10)
-my_map.add_layers(tile_layer)
+my_map.layers.append(tile_layer)
 ```
 
 ### What about Markers and Polys
 
 If you want to add a marker to your map, you could do it like so.
 
 ```python
 # ...
 my_map = Map('my-map', center=[-41.139416, -73.025431], zoom=16)
 my_marker = my_map.new_marker([-41.139416, -73.025431], opacity=0.8)
 
 # if you want to add a tooltip to your marker
-my_marker.bind_tooltip('This is a tooltip')
+my_marker.new_tooltip('My Marker Tooltip')
 
 # To add a popup associated with the marker
-my_marker.bind_popup('<b>This is the popup content</b>')
+my_marker.new_popup('<b>This is the popup content</b>')
 
 # Adding Polys
 circle = my_map.new_circle([-41.139416, -73.025431], radius=15)
 # You can add popups and tooltips as well
-circle.bind_tooltip('This is a circle tooltip')
+circle.new_tooltip('This is a circle tooltip')
 
 rectangle = my_map.new_rectangle([[-41.139416, -73.025431],[-41.139446, -73.025451]])
-rectangle.bind_popup('This is a rectangle popup')
+rectangle.new_popup('This is a rectangle popup')
 
 ```
 
 I will be adding more functionallity in the future to extend the capabilities and customization options.
```

### Comparing `flask_leaflet-0.1.2/flask_leaflet/__init__.py` & `flask_leaflet-0.1.3/flask_leaflet/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,24 @@
-from typing import Optional, Callable, Any
+from typing import Optional
 
 from flask import Flask, Blueprint, Markup, render_template
 from .map import Map
 from .layers.raster import TileLayer
-from .layers.ui import Marker, Tooltip, Popup
+from .layers.ui import Marker
 
-__all__ = ("Leaflet", "Map", "Marker", "Tooltip", "Popup")
+__all__ = ("Leaflet", "Map", "Marker")
 
 
 class Leaflet:
     app: Optional[Flask]
     css_local_path: Optional[str] = None
     js_local_path: Optional[str] = None
 
     config: Optional[dict] = None
-    _nonce_callback: Optional[Callable[[], str]] = None
-    _default_tile_layer: TileLayer | None = None
+    default_tile_layer: TileLayer | None = None
 
     default_icon_marker_url: str = None
     default_icon_marker_shadow_url: str = None
 
     def __init__(self, app: Optional[Flask] = None) -> None:
         if app is not None:
             self.init_app(app)
@@ -38,22 +37,24 @@
         if not hasattr(app, "extensions"):
             app.extensions = {}
         app.extensions["leaflet"] = self
         self.app = app
 
         self.__register_blueprint(self.app)
 
+        self.csp_nonce_callback = self.app.config.get("LEAFLET_NONCE_CALLBACK")
         self.css_local_path = self.app.config.get("LEAFLET_CSS_LOCAL_PATH")
         self.js_local_path = self.app.config.get("LEAFLET_JS_LOCAL_PATH")
         self.default_icon_marker_url = app.config.get("LEAFLET_MARKER_ICON_URL")
         self.default_icon_marker_shadow_url = app.config.get(
             "LEAFLET_MARKER_ICON_SHADOW_URL"
         )
+
         if url_template := app.config.get("LEAFLET_DEFAULT_RASTER_TILE_URL_TEMPLATE"):
-            tile_options = app.config.get("LEAFLET_DEFAULT_RASTER_TILE_OPTIONS", dict())
+            tile_options = app.config.get("LEAFLET_DEFAULT_RASTER_TILE_OPTIONS")
             self.default_tile_layer = TileLayer(url_template, **tile_options)
 
         @app.context_processor
         def inject_context_variables() -> dict:
             return dict(leaflet=self)
 
     def load(self) -> Markup:
@@ -64,17 +65,21 @@
                 js_local_path=self.js_local_path,
                 css_version="1.9.3",
                 js_version="1.9.3",
             )
         )
 
     def render_map(
-        self, map: Map, options: dict[str, Any] = None, class_: str = ""
+        self, map: Map, *, class_: str = "", nonce_: str = None, **kwargs
     ) -> Markup:
-        options = options or {}
-        for key, val in options.items():
+        for key, val in kwargs.items():
             if hasattr(map, key):
                 setattr(map, key, val)
 
-        html_str = render_template("map.html", map=map, class_=class_)
-
-        return Markup(html_str)
+        if not map.has_any_raster_layer() and self.default_tile_layer is not None:
+            map.layers.append(self.default_tile_layer)
+            self.default_tile_layer.owner = map
+
+        html_string = map.__render_html__(class_)
+        nonce_tag = f" nonce={nonce_}" if nonce_ else ""
+        js_string = Markup(f"<script{nonce_tag}>{str(map.__render_js__())}</script>")
+        return html_string + js_string
```

### Comparing `flask_leaflet-0.1.2/flask_leaflet/layers/paths.py` & `flask_leaflet-0.1.3/flask_leaflet/layers/paths.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from .base import Layer
 from ..basic_types import LatLng
-from .ui import Tooltip, Popup
+from .ui import BindsUILayers
 import typing as t
+from markupsafe import Markup
 
 
-class Path(Layer):
+class Path(BindsUILayers, Layer):
+    __not_render_options__ = Layer.__not_render_options__ + ["ui_layers"]
+    
     stroke: bool = True
     color: str = "#3388ff"
     weight: int = 3
     opacity: float = 1.0
     line_cap: str = "round"
     line_join: str = "round"
     dash_array: str = None
@@ -33,14 +36,15 @@
         dash_offset: str = None,
         fill: bool = True,
         fill_color: str = color,
         fill_opacity: float = 0.2,
         fill_rule: str = "evenodd",
         bubbling_mouse_events: bool = True,
         class_name: str = None,
+        ui_layers: list[Layer] = None,
         **kwargs,
     ) -> None:
         super().__init__(**kwargs)
         self.stroke = stroke
         self.color = color
         self.weight = weight
         self.opacity = opacity
@@ -50,48 +54,38 @@
         self.dash_offset = dash_offset
         self.fill = fill
         self.fill_color = fill_color
         self.fill_opacity = fill_opacity
         self.fill_rule = fill_rule
         self.bubbling_mouse_events = bubbling_mouse_events
         self.class_name = class_name
+        self.ui_layers = ui_layers or []
 
-    def bind_tooltip(self, content: str, **kwargs) -> Tooltip:
-        tooltip = Tooltip(self.latlng, content, **kwargs)
-        self.bind(tooltip)
-        return tooltip
-
-    def bind_popup(self, content: str, **kwargs) -> Popup:
-        popup = Popup(self.latlng, content, **kwargs)
-        self.bind(popup)
-        return popup
+    def __render_html__(self, as_variable: bool = False) -> Markup:
+        string = super().__render_html__(as_variable=as_variable)
+        string = string + self.render_ui_layers(as_variable=as_variable)
+        return string
 
 
 class CircleMarker(Path):
-    __not_options__ = Path.__not_options__ + ["latlng"]
-    __factory__ = "circleMarker"
-    __bind_str__ = "addTo"
-    __call_args__ = ["latlng"]
-    __call_as_obj__ = ["latlng"]
+    __render_args__ = ["latlng"]
+    __not_render_options__ = Path.__not_render_options__ + __render_args__
 
     latlng: LatLng | list[float]
     radius: int = 10
 
     def __init__(self, latlng: LatLng | list[float], radius: int = 10, **kwargs) -> None:
         super().__init__(**kwargs)
         self.latlng = latlng if isinstance(latlng, LatLng) else LatLng(*latlng)
         self.radius = radius
 
 
 class Polyline(Path):
-    __not_options__ = Path.__not_options__ + ["latlngs"]
-    __factory__ = "polyline"
-    __bind_str__ = "addTo"
-    __call_args__ = ["latlngs"]
-    __call_as_obj__ = ["latlngs"]
+    __render_args__ = ["latlngs"]
+    __not_render_options__ = Path.__not_render_options__ + __render_args__
 
     latlngs: list[LatLng]
 
     smooth_factor: float = 1.0
     no_clip: bool = False
 
     def __init__(self, latlngs: list[LatLng] | list[list[float]], smooth_fator: float = 1.0, no_clip: bool = False, **kwargs) -> None:
@@ -112,52 +106,53 @@
 
             elif isinstance(content, LatLng):
                 out_latlngs.append(content)
 
         return out_latlngs
 
 
-class Polygon(Polyline):
-    __factory__ = "polygon"
+class Polygon(Polyline):    
 
     def __init__(self, latlngs: list[LatLng] | list[list[float]], **kwargs) -> None:
         super().__init__(latlngs, **kwargs)
 
 
 class Rectangle(Polygon):
-    __factory__ = "rectangle"
 
     def __init__(self, latlngs: list[LatLng] | list[list[float]], **kwargs) -> None:
         super().__init__(latlngs, **kwargs)
 
 
 class Circle(CircleMarker):
-    __factory__ = "circle"
 
     def __init__(self, latlng: LatLng | list[float], radius: int = 10, **kwargs) -> None:
         super().__init__(latlng, radius, **kwargs)
 
 
-class HasPathsLayers:
-    _layers: list[Layer]
+class CreatesPathLayers:
+    layers: list[Layer]
 
     def new_polyline(
         self, latlngs: list[LatLng] | list[list[float]], smooth_fator: float = 1.0, no_clip: bool = False, **kwargs
     ) -> Polyline:
         polyline = Polyline(latlngs, smooth_fator, no_clip, **kwargs)
-        self._layers.append(polyline)
+        polyline.owner = self
+        self.layers.append(polyline)
         return polyline
 
     def new_polygon(self, latlngs: list[LatLng] | list[list[float]], **kwargs) -> Polygon:
         polygon = Polygon(latlngs, **kwargs)
-        self._layers.append(polygon)
+        polygon.owner = self
+        self.layers.append(polygon)
         return polygon
 
     def new_rectangle(self, latlngs: list[LatLng] | list[list[float]], **kwargs) -> Rectangle:
         rectangle = Rectangle(latlngs, **kwargs)
-        self._layers.append(rectangle)
+        rectangle.owner = self
+        self.layers.append(rectangle)
         return rectangle
 
     def new_circle(self, latlng: LatLng | list[float], radius: int = 10, **kwargs) -> Circle:
         circle = Circle(latlng, radius, **kwargs)
-        self._layers.append(circle)
+        circle.owner = self
+        self.layers.append(circle)
         return circle
```

### Comparing `flask_leaflet-0.1.2/flask_leaflet/layers/raster.py` & `flask_leaflet-0.1.3/flask_leaflet/layers/raster.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 from .base import Layer, InteractiveLayer
 from ..basic_types import LatLngBounds, Point
 
 RASTER_LAYERS = ("TileLayer", "WMSTileLayer", "ImageOverlay", "VideoOverlay")
 
 
 class GridLayer(Layer):
-    __factory__ = "gridLayer"
-    __bind_str__ = "addTo"
-
+    
     tile_size: int | Point = 256
     opacity: float = 1.0
     update_when_idle: bool = False
     update_when_zooming: bool = True
     update_interval: int = 200
     z_index: int = 1
     bounds: LatLngBounds = None
@@ -57,18 +55,16 @@
         self.min_native_zoom = min_native_zoom
         self.no_wrap = no_wrap
         self.class_name = class_name
         self.keep_buffer = keep_buffer
 
 
 class TileLayer(GridLayer):
-    __not_options__ = GridLayer.__not_options__ + ["url_template"]
-    __factory__ = "tileLayer"
-    __bind_str__ = "addTo"
-    __call_args__ = ["url_template"]
+    __render_args__ = ["url_template"]
+    __not_render_options__ = GridLayer.__not_render_options__ + __render_args__
 
     url_template: str
     min_zoom: int = 0
     max_zoom: int = 18
     subdomains: str = "abc"
     error_tile_url: str = ""
     zoom_offset: int = 0
@@ -103,18 +99,16 @@
         self.zoom_reverse = zoom_reverse
         self.detect_retina = detect_retina
         self.cross_origin = cross_origin
         self.referrer_policy = referrer_policy
 
 
 class WMSTileLayer(TileLayer):
-    __not_options__ = TileLayer.__not_options__ + ["base_url"]
-    __factory__ = "tileLayer.wms"
-    __bind_str__ = "addTo"
-    __call_args__ = ["base_url"]
+    __render_args__ = ["base_url"]
+    __not_render_options__ = TileLayer.__not_render_options__ + __render_args__
 
     base_url: str
     layers: str = ""
     styles: str = ""
     format: str = "image/png"
     transparent: bool = False
     version: str = "1.1.1"
@@ -135,22 +129,22 @@
         self.base_url = base_url
         self.layers = layers
         self.styles = styles
         self.format = format
         self.transparent = transparent
         self.version = version
         self.uppercase = uppercase
+    
+    def __factory_str__(self) -> str:
+        return "tileLayer.wms"
 
 
 class ImageOverlay(InteractiveLayer):
-    __not_options__ = InteractiveLayer.__not_options__ + ["image_url", "image_bounds"]
-    __factory__ = "imageOverlay"
-    __bind_str__ = "addTo"
-    __call_args__ = ["image_url", "image_bounds"]
-    __call_as_obj__ = ["image_bounds"]
+    __render_args__ = ["image_url", "image_bounds"]
+    __not_render_options__ = InteractiveLayer.__not_render_options__ + __render_args__
 
     image_url: str
     image_bounds: LatLngBounds
 
     opacity: float = 1.0
     alt: str = ""
     interactive: bool = False
@@ -181,19 +175,16 @@
         self.cross_origin = cross_origin
         self.error_overlay_url = error_overlay_url
         self.z_index = z_index
         self.class_name = class_name
 
 
 class VideoOverlay(ImageOverlay):
-    __not_options__ = ImageOverlay.__not_options__ + ["video", "bounds"]
-    __factory__ = "videoOverlay"
-    __bind_str__ = "addTo"
-    __call_args__ = ["video", "bounds"]
-    __call_as_obj__ = ["bounds"]
+    __render_args__ = ["video", "bounds"]
+    __not_render_options__ = ImageOverlay.__not_render_options__ + __render_args__
 
     video: str | list[str]
     bounds: LatLngBounds
 
     autoplay: bool = True
     loop: bool = True
     keep_aspect_ratio: bool = True
@@ -217,19 +208,19 @@
         self.autoplay = autoplay
         self.loop = loop
         self.keep_aspect_ratio = keep_aspect_ratio
         self.muted = muted
         self.plays_inline = plays_inline
 
 
-class HasRasterLayers:
-    _layers: list[Layer]
+class CreatesRasterLayers:
+    layers: list[Layer]
 
     def has_any_raster_layer(self) -> bool:
-        for layer in self._layers:
+        for layer in self.layers:
             if layer.__class__.__name__ in RASTER_LAYERS:
                 return True
         return False
 
     def new_tile_layer(
         self,
         url_template: str,
@@ -255,30 +246,32 @@
             tms,
             zoom_reverse,
             detect_retina,
             cross_origin,
             referrer_policy,
             **kwargs,
         )
-        self._layers.append(tile_layer)
+        tile_layer.owner = self
+        self.layers.append(tile_layer)
         return tile_layer
 
     def new_wms_tile_layer(
         self,
         base_url: str,
         layers: str,
         styles: str = "",
         format: str = "image/png",
         transparent: bool = False,
         version: str = "1.1.1",
         uppercase: bool = False,
         **kwargs,
     ) -> WMSTileLayer:
         wms_tile_layer = WMSTileLayer(base_url, layers, styles, format, transparent, version, uppercase, **kwargs)
-        self._layers.append(wms_tile_layer)
+        wms_tile_layer.owner = self
+        self.layers.append(wms_tile_layer)
         return wms_tile_layer
 
     def new_image_overlay(
         self,
         image_url: str,
         image_bounds: LatLngBounds | list[list[float]],
         opacity: float = 1.0,
@@ -289,15 +282,16 @@
         z_index: int = 1,
         class_name: str = "",
         **kwargs,
     ) -> ImageOverlay:
         image_overlay = ImageOverlay(
             image_url, image_bounds, opacity, alt, interactive, cross_origin, error_overlay_url, z_index, class_name, **kwargs
         )
-        self._layers.append(image_overlay)
+        image_overlay.owner = self
+        self.layers.append(image_overlay)
         return image_overlay
 
     def new_video_overlay(
         self,
         video: str | list[str],
         bounds: LatLngBounds | list[list[float]],
         autoplay: bool = True,
@@ -313,9 +307,10 @@
             autoplay,
             loop,
             keep_aspect_ratio,
             muted,
             plays_inline,
             **kwargs,
         )
-        self._layers.append(video_overlay)
+        video_overlay.owner = self
+        self.layers.append(video_overlay)
         return video_overlay
```

### Comparing `flask_leaflet-0.1.2/flask_leaflet/layers/ui.py` & `flask_leaflet-0.1.3/flask_leaflet/layers/ui.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,60 +1,49 @@
+import typing as t
 from ..basic_types import Icon, Point, LatLng
 from .base import Layer, InteractiveLayer
-
+from markupsafe import Markup
 
 class DivOverlay(InteractiveLayer):
-    __call_as_obj__ = ["offset"]
-    __binded_attr__ = "content"
 
     offset: Point = None
     class_name: str = ""
     pane: str = None
     content: str = ""
 
     def __init__(self, offset: Point = None, class_name: str = "", pane: str = None, content: str = "", **kwargs) -> None:
         super().__init__(pane=pane, **kwargs)
-        self.offset = offset or Point(0, 0)
+        self.offset = Point(*offset) if isinstance(offset, (tuple, list)) else offset
         self.class_name = class_name
         self.content = content
 
 
 class Popup(DivOverlay):
-    __not_options__ = DivOverlay.__not_options__ + ["latlng"]
-    __factory__ = "popup"
-    __bind_str__ = "openOn"
-    __call_args__ = ["latlng"]
-    __call_as_obj__ = DivOverlay.__call_as_obj__ + [
-        "latlng",
-        "auto_pan_padding_top_left",
-        "auto_pan_padding_bottom_right",
-        "auto_pan_padding",
-    ]
-
-    __binded_str__ = "bindPopup"
+    __render_args__ = ["latlng"]
+    __not_render_options__ = DivOverlay.__not_render_options__ + __render_args__
 
     latlng: LatLng
     pane: str = "popupPane"
     offset: Point = None
     max_width: int = 300
     min_width: int = 50
     max_height: int = None
     auto_pan: bool = True
     auto_pan_padding_top_left: Point = None
     auto_pan_padding_bottom_right: Point = None
-    auto_pan_padding: Point = Point(5, 5)
+    auto_pan_padding: Point = [5,5]
     keep_in_view: bool = False
     close_button: bool = True
     auto_close: bool = True
     close_on_escape_key: bool = True
     close_on_click: bool = None
 
     def __init__(
         self,
-        latlng: LatLng | list[float, float],
+        latlng: LatLng | list[float, float] = None,
         content: str = "",
         pane: str = "popupPane",
         offset: Point | list[int] = [0, 7],
         max_width: int = 300,
         min_width: int = 50,
         max_height: int = None,
         auto_pan: bool = True,
@@ -64,17 +53,16 @@
         keep_in_view: bool = False,
         close_button: bool = True,
         auto_close: bool = True,
         close_on_escape_key: bool = True,
         close_on_click: bool = None,
         **kwargs,
     ) -> None:
-        offset = Point(*offset) if isinstance(offset, (list, tuple)) else offset
         super().__init__(offset=offset, content=content, pane=pane, **kwargs)
-        self.latlng = latlng if isinstance(latlng, LatLng) else LatLng(*latlng)
+        self.latlng = LatLng(*latlng) if isinstance(latlng, (tuple, list)) else latlng
         self.max_width = max_width
         self.min_width = min_width
         self.max_height = max_height
         self.auto_pan = auto_pan
         self.auto_pan_padding_top_left = (
             Point(*auto_pan_padding_top_left) if isinstance(auto_pan_padding_top_left, (list, tuple)) else auto_pan_padding_top_left
         )
@@ -88,24 +76,21 @@
         self.close_button = close_button
         self.auto_close = auto_close
         self.close_on_escape_key = close_on_escape_key
         self.close_on_click = close_on_click
 
 
 class Tooltip(DivOverlay):
-    __not_options__ = ["id", "latlng", "map"]
-    __factory__ = "tooltip"
-    __bind_str__ = "openOn"
-    __call_args__ = ["latlng"]
-    __call_as_obj__ = ["latlng", "offset"]
-    __binded_str__ = "bindTooltip"
+
+    __render_args__ = ["latlng"]
+    __not_render_options__ = DivOverlay.__not_render_options__ + __render_args__
 
     latlng: LatLng
     pane: str = "tooltipPane"
-    offset: Point = Point(0, 0)
+    offset: Point = [0,0]
     direction: str = "auto"
     permanent: bool = False
     opacity: float = 0.9
 
     def __init__(
         self,
         latlng: list[float, float] | LatLng,
@@ -121,20 +106,88 @@
         super().__init__(content=content, pane=pane, offset=offset, **kwargs)
         self.latlng = latlng if isinstance(latlng, LatLng) else LatLng(*latlng)
         self.direction = direction
         self.permanent = permanent
         self.opacity = opacity
 
 
-class Marker(Layer):
-    __not_options__ = Layer.__not_options__ + ["latlng"]
-    __factory__ = "marker"
-    __bind_str__ = "addTo"
-    __call_args__ = ["latlng"]
-    __call_as_obj__ = ["latlng"]
+class BindsUILayers:
+    latlng: LatLng | None
+    var_name: str
+    ui_layers: list[Tooltip, Popup]
+
+    def add_ui_layer(self, ui_layer: Tooltip | Popup) -> None:
+        self.ui_layers.append(ui_layer)
+
+    def new_tooltip(self, content: str = "",
+        pane: str = "tooltipPane",
+        offset: Point = [0, 0],
+        direction: str = "auto",
+        permanent: bool = False,
+        opacity: float = 0.9,
+        **kwargs) -> Tooltip:
+        tooltip = Tooltip(self.latlng, content, pane, offset, direction, permanent, opacity, **kwargs)
+        self.add_ui_layer(tooltip)
+        return tooltip
+
+    def new_popup(self, content: str = "",
+        pane: str = "popupPane",
+        offset: Point | list[int] = [0, 7],
+        max_width: int = 300,
+        min_width: int = 50,
+        max_height: int = None,
+        auto_pan: bool = True,
+        auto_pan_padding_top_left: Point | list[int] = None,
+        auto_pan_padding_bottom_right: Point | list[int] = None,
+        auto_pan_padding: Point | list[int] = [5, 5],
+        keep_in_view: bool = False,
+        close_button: bool = True,
+        auto_close: bool = True,
+        close_on_escape_key: bool = True,
+        close_on_click: bool = None,
+        **kwargs) -> Popup:
+
+        popup = Popup(self.latlng or None,
+                     content,
+                     pane,
+                     offset,
+                     max_width,
+                     min_width,
+                     max_height,
+                     auto_pan,
+                     auto_pan_padding_top_left,
+                     auto_pan_padding_bottom_right,
+                     auto_pan_padding,
+                     keep_in_view,
+                     close_button,
+                     auto_close,
+                     close_on_escape_key,
+                     close_on_click,
+                     **kwargs)
+        self.add_ui_layer(popup)
+        return popup
+
+
+    def render_ui_layers(self, as_variable: bool = False) -> str:
+        string = ""
+        if as_variable:
+            for ui_layer in self.ui_layers:
+                string = ui_layer.__render_html__(as_variable)
+                
+                string = Markup(f"{string}{self.var_name}.bind{ui_layer.__class__.__name__}({ui_layer.var_name});")
+        else:
+            for ui_layer in self.ui_layers:
+                string += f".bind{ui_layer.__class__.__name__}({ui_layer.__render_html__()})"
+        print(string)
+        return string
+
+
+class Marker(BindsUILayers, Layer):
+    __render_args__ = ["latlng"]
+    __not_render_options__ = Layer.__not_render_options__ + __render_args__ + ["ui_layers"]
 
     latlng: LatLng
     icon: Icon = None
     keyboard: bool = True
     title: str = ""
     alt: str = "Marker"
     z_index_offset: int = 0
@@ -157,14 +210,15 @@
         opacity: float = 1.0,
         rise_on_hover: bool = False,
         rise_offset: int = 250,
         pane: str = "markerPane",
         shadow_pane: str = "shadowPane",
         bubbling_mouse_events: bool = False,
         auto_pan_on_focus: bool = True,
+        ui_layers: list[Layer] = None,
         **kwargs,
     ) -> None:
         super().__init__(**kwargs)
         self.latlng = latlng if isinstance(latlng, LatLng) else LatLng(*latlng)
         self.icon = icon or r"%leaflet_default_icon"
         self.keyboard = keyboard
         self.title = title
@@ -173,28 +227,24 @@
         self.opacity = opacity
         self.rise_on_hover = rise_on_hover
         self.rise_offset = rise_offset
         self.pane = pane
         self.shadow_pane = shadow_pane
         self.bubbling_mouse_events = bubbling_mouse_events
         self.auto_pan_on_focus = auto_pan_on_focus
+        self.ui_layers = ui_layers or []
 
-    def bind_tooltip(self, content: str, **kwargs) -> Tooltip:
-        tooltip = Tooltip(self.latlng, content, **kwargs)
-        self.bind(tooltip)
-        return tooltip
-
-    def bind_popup(self, content: str, **kwargs) -> Popup:
-        popup = Popup(self.latlng, content, **kwargs)
-        self.bind(popup)
-        return popup
+    def __render_html__(self, as_variable: bool = False) -> Markup:
+        string = super().__render_html__(as_variable=as_variable)
+        string = string + self.render_ui_layers(as_variable=as_variable)
+        return string
 
 
-class HasUILayers:
-    _layers: list[Layer]
+class CreatesUILayers:
+    layers: list[Layer]
 
     def new_marker(
         self,
         latlng: list[float, float] | LatLng,
         icon: Icon = None,
         keyboard: bool = True,
         title: str = "",
@@ -221,30 +271,32 @@
             rise_offset,
             pane,
             shadow_pane,
             bubbling_mouse_events,
             auto_pan_on_focus,
             **kwargs,
         )
-        self._layers.append(marker)
+        self.layers.append(marker)
+        marker.owner = self
         return marker
 
     def new_tooltip(
         self,
         latlng: list[float, float] | LatLng,
         content: str = "",
         pane: str = "tooltipPane",
         offset: Point = [0, 0],
         direction: str = "auto",
         permanent: bool = False,
         opacity: float = 0.9,
         **kwargs,
     ) -> Tooltip:
         tooltip = Tooltip(latlng, content, pane, offset, direction, permanent, opacity, **kwargs)
-        self._layers.append(tooltip)
+        self.layers.append(tooltip)
+        tooltip.owner = self
         return tooltip
 
     def new_popup(
         self,
         latlng: LatLng | list[float, float],
         content: str = "",
         pane: str = "popupPane",
@@ -278,9 +330,10 @@
             keep_in_view,
             close_button,
             auto_close,
             close_on_escape_key,
             close_on_click,
             **kwargs,
         )
-        self._layers.append(popup)
+        self.layers.append(popup)
+        popup.owner = self
         return popup
```

### Comparing `flask_leaflet-0.1.2/flask_leaflet/static/images/marker-icon.png` & `flask_leaflet-0.1.3/flask_leaflet/static/images/marker-icon.png`

 * *Files identical despite different names*

### Comparing `flask_leaflet-0.1.2/flask_leaflet/static/images/marker-shadow.png` & `flask_leaflet-0.1.3/flask_leaflet/static/images/marker-shadow.png`

 * *Files identical despite different names*

### Comparing `flask_leaflet-0.1.2/flask_leaflet/templates/load.html` & `flask_leaflet-0.1.3/flask_leaflet/templates/load.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 {% if css_local_path %}
-<link rel="stylesheet" href="{{ url_for('static', filename=css_local_path) }}"
-     crossorigin=""/>
+<link rel="stylesheet" href="{{ url_for('static', filename=css_local_path) }}" crossorigin=""/>
 {% else %}
 <link rel="stylesheet" href="https://unpkg.com/leaflet@{{ css_version }}/dist/leaflet.css">
 {% endif %}
 {% if js_local_path %}
 <script src="{{ url_for('static', filename=js_local_path) }}"></script>
 {% else %}
 <script nonce={{ csp_nonce() if csp_nonce else "" }} src="https://unpkg.com/leaflet@{{ js_version }}/dist/leaflet.js"
```

### Comparing `flask_leaflet-0.1.2/PKG-INFO` & `flask_leaflet-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-leaflet
-Version: 0.1.2
+Version: 0.1.3
 Author-Email: Sebastian Salinas <seba.salinas.delrio@gmail.com>
 License: MIT
 Requires-Python: >=3.11
 Requires-Dist: flask>=2.3.2
 Description-Content-Type: text/markdown
 
 # Flask-Leaflet
@@ -46,26 +46,25 @@
 
 Once installed Flask-Leaflet is easy to use. Let's walk through setting up a basic application. Also please note that this is a very basic guide: we will be taking shortcuts here that you should never take in a real application.
 
 To begin we'll set up a Flask app:
 
 ```python
 from flask import Flask
-
 from flask_leaflet import Leaflet
 
 app = Flask(__name__)
 
 leaflet = Leaflet()
 leaflet.init_app(app)
 ```
 
 ### Load resources
 
-Once the extension is set up, this will make available the `leaflet` object into the templates context so you could load the javascript package easily, like this.
+Once the extension is set up, this will make available the `leaflet` object into the templates context so you could load the javascript and css package easily, like this.
 
 ```html
 <head>
   {{ leaflet.load() }}
 </head>
 ```
 
@@ -83,20 +82,21 @@
     # Using snake_case for the options.
     my_map = Map('my-map', center=[-41.139416, -73.025431], zoom=16)
     return render('my_map.html', my_map=my_map)
 ```
 
 ### Rendering the map
 
-Now that we have a Map instance we can render it in a template. **IMPORTANT:** The map container **Must have a Height** given by a class added on the `class_` arguments.
+Now that we have a Map instance we can render it in a template. **IMPORTANT:** The map container **Must have a Height** given the special `class_` argument. Also you got access to `nonce_` in case you need to add a nonce token to the script tag.
+in the next example we use `tailwindcss` class for a 200px height
 
 ```html
 <head>
   <!-- You can add custom options at this instance that will overwrite any defaults coming from the view. Note that using class_='h-200px' we stablish a minimum height otherwise the map wouldnt be visible. -->
-  {{ leaflet.render_map(my_map, class_='h-[200px]' zoom=10) }}
+  {{ leaflet.render_map(my_map, class_='h-[200px]', zoom=10) }}
 </head>
 ```
 
 ### What about RasterLayers
 
 If you need to use a RasterTile style for every map you could stablish in your configuration the url_template and options for the default raster. Doing this will automatically be seted up for every map rendered.
 
@@ -111,36 +111,36 @@
 or
 
 ```python
 from flask_leaflet.layers.raster import TileLayer
 # ...
 my_map = Map('my-map', center=[-41.139416, -73.025431], zoom=16)
 tile_layer = TileLayer(r"https://server.arcgisonline.com/ArcGIS/rest/services/World_Imagery/MapServer/tile/{z}/{y}/{x}", max_zoom=15, min_zoom=10)
-my_map.add_layers(tile_layer)
+my_map.layers.append(tile_layer)
 ```
 
 ### What about Markers and Polys
 
 If you want to add a marker to your map, you could do it like so.
 
 ```python
 # ...
 my_map = Map('my-map', center=[-41.139416, -73.025431], zoom=16)
 my_marker = my_map.new_marker([-41.139416, -73.025431], opacity=0.8)
 
 # if you want to add a tooltip to your marker
-my_marker.bind_tooltip('This is a tooltip')
+my_marker.new_tooltip('My Marker Tooltip')
 
 # To add a popup associated with the marker
-my_marker.bind_popup('<b>This is the popup content</b>')
+my_marker.new_popup('<b>This is the popup content</b>')
 
 # Adding Polys
 circle = my_map.new_circle([-41.139416, -73.025431], radius=15)
 # You can add popups and tooltips as well
-circle.bind_tooltip('This is a circle tooltip')
+circle.new_tooltip('This is a circle tooltip')
 
 rectangle = my_map.new_rectangle([[-41.139416, -73.025431],[-41.139446, -73.025451]])
-rectangle.bind_popup('This is a rectangle popup')
+rectangle.new_popup('This is a rectangle popup')
 
 ```
 
 I will be adding more functionallity in the future to extend the capabilities and customization options.
```

