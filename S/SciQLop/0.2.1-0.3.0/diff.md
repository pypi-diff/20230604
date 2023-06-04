# Comparing `tmp/SciQLop-0.2.1.tar.gz` & `tmp/sciqlop-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SciQLop-0.2.1.tar", last modified: Tue Apr 25 07:43:55 2023, max compression
+gzip compressed data, was "sciqlop-0.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `SciQLop-0.2.1.tar` & `sciqlop-0.3.0.tar`

### file list

```diff
@@ -1,90 +1,91 @@
--rw-r--r--   0        0        0    35147 2023-04-25 07:43:34.629640 SciQLop-0.2.1/COPYING
--rw-r--r--   0        0        0     1859 2023-04-25 07:43:34.629640 SciQLop-0.2.1/README.md
--rw-r--r--   0        0        0       23 2023-04-25 07:43:34.629640 SciQLop-0.2.1/SciQLop/__init__.py
--rw-r--r--   0        0        0     1276 2023-04-25 07:43:34.629640 SciQLop-0.2.1/SciQLop/app.py
--rw-r--r--   0        0        0     1433 2023-04-25 07:43:34.633640 SciQLop-0.2.1/SciQLop/backend/__init__.py
--rw-r--r--   0        0        0      532 2023-04-25 07:43:34.633640 SciQLop-0.2.1/SciQLop/backend/enums.py
--rw-r--r--   0        0        0      831 2023-04-25 07:43:34.633640 SciQLop-0.2.1/SciQLop/backend/logging/__init__.py
--rw-r--r--   0        0        0      172 2023-04-25 07:43:34.633640 SciQLop-0.2.1/SciQLop/backend/models.py
--rw-r--r--   0        0        0        1 2023-04-25 07:43:34.633640 SciQLop-0.2.1/SciQLop/backend/pipelines_model/__init__.py
--rw-r--r--   0        0        0     5202 2023-04-25 07:43:34.633640 SciQLop-0.2.1/SciQLop/backend/pipelines_model/auto_register.py
--rw-r--r--   0        0        0      128 2023-04-25 07:43:34.633640 SciQLop-0.2.1/SciQLop/backend/pipelines_model/base/__init__.py
--rw-r--r--   0        0        0     6856 2023-04-25 07:43:34.633640 SciQLop-0.2.1/SciQLop/backend/pipelines_model/base/model.py
--rw-r--r--   0        0        0     2925 2023-04-25 07:43:34.633640 SciQLop-0.2.1/SciQLop/backend/pipelines_model/base/pipeline_node.py
--rw-r--r--   0        0        0     5349 2023-04-25 07:43:34.633640 SciQLop-0.2.1/SciQLop/backend/pipelines_model/data_pipeline.py
--rw-r--r--   0        0        0      718 2023-04-25 07:43:34.633640 SciQLop-0.2.1/SciQLop/backend/pipelines_model/data_provider.py
--rw-r--r--   0        0        0     3820 2023-04-25 07:43:34.633640 SciQLop-0.2.1/SciQLop/backend/pipelines_model/graph.py
--rw-r--r--   0        0        0        0 2023-04-25 07:43:34.633640 SciQLop-0.2.1/SciQLop/backend/products_model/__init__.py
--rw-r--r--   0        0        0     6549 2023-04-25 07:43:34.633640 SciQLop-0.2.1/SciQLop/backend/products_model/model.py
--rw-r--r--   0        0        0     3195 2023-04-25 07:43:34.633640 SciQLop-0.2.1/SciQLop/backend/products_model/product_node.py
--rw-r--r--   0        0        0        0 2023-04-25 07:43:34.633640 SciQLop-0.2.1/SciQLop/backend/resampling/__init__.py
--rw-r--r--   0        0        0     1069 2023-04-25 07:43:34.633640 SciQLop-0.2.1/SciQLop/backend/resampling/spectro_regrid.py
--rw-r--r--   0        0        0      186 2023-04-25 07:43:34.633640 SciQLop-0.2.1/SciQLop/backend/unique_names.py
--rw-r--r--   0        0        0     1645 2023-04-25 07:43:34.633640 SciQLop-0.2.1/SciQLop/mime/__init__.py
--rw-r--r--   0        0        0      120 2023-04-25 07:43:34.633640 SciQLop-0.2.1/SciQLop/mime/types.py
--rw-r--r--   0        0        0     2279 2023-04-25 07:43:34.633640 SciQLop-0.2.1/SciQLop/plugins/__init__.py
--rw-r--r--   0        0        0      181 2023-04-25 07:43:34.633640 SciQLop-0.2.1/SciQLop/plugins/catalogs/__init__.py
--rw-r--r--   0        0        0     1555 2023-04-25 07:43:34.633640 SciQLop-0.2.1/SciQLop/plugins/catalogs/catalogs.py
--rw-r--r--   0        0        0     4035 2023-04-25 07:43:34.633640 SciQLop-0.2.1/SciQLop/plugins/catalogs/lightweight_manager/__init__.py
--rw-r--r--   0        0        0     2379 2023-04-25 07:43:34.633640 SciQLop-0.2.1/SciQLop/plugins/catalogs/lightweight_manager/catalog_selector.py
--rw-r--r--   0        0        0     1706 2023-04-25 07:43:34.633640 SciQLop-0.2.1/SciQLop/plugins/catalogs/lightweight_manager/event_selector.py
--rw-r--r--   0        0        0     3906 2023-04-25 07:43:34.633640 SciQLop-0.2.1/SciQLop/plugins/speasy.py
--rw-r--r--   0        0        0     1419 2023-04-25 07:43:34.633640 SciQLop-0.2.1/SciQLop/plugins/test_plugin.py
--rw-r--r--   0        0        0   552261 2023-04-25 07:43:34.637641 SciQLop-0.2.1/SciQLop/resources/__init__.py
--rw-r--r--   0        0        0   118794 2023-04-25 07:43:34.637641 SciQLop-0.2.1/SciQLop/resources/icons/SciQLop.png
--rw-r--r--   0        0        0     3191 2023-04-25 07:43:34.637641 SciQLop-0.2.1/SciQLop/resources/icons/Simple_icon_time.svg
--rw-r--r--   0        0        0     1956 2023-04-25 07:43:34.637641 SciQLop-0.2.1/SciQLop/resources/icons/add.png
--rw-r--r--   0        0        0     2001 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/resources/icons/allEvents.png
--rw-r--r--   0        0        0      615 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/resources/icons/catalogue.png
--rw-r--r--   0        0        0     1003 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/resources/icons/chart.png
--rw-r--r--   0        0        0     1047 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/resources/icons/cursor.png
--rw-r--r--   0        0        0     2150 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/resources/icons/dataSourceComponent.png
--rw-r--r--   0        0        0      882 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/resources/icons/dataSourceNode.png
--rw-r--r--   0        0        0     1213 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/resources/icons/dataSourceProduct.png
--rw-r--r--   0        0        0     4821 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/resources/icons/dataSourceRoot.png
--rw-r--r--   0        0        0      788 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/resources/icons/database.png
--rw-r--r--   0        0        0      834 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/resources/icons/delete.png
--rwxr-xr-x   0        0        0     1266 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/resources/icons/discard.png
--rw-r--r--   0        0        0     1231 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/resources/icons/down.png
--rw-r--r--   0        0        0     1731 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/resources/icons/drag.png
--rw-r--r--   0        0        0     4413 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/resources/icons/next.png
--rwxr-xr-x   0        0        0     1450 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/resources/icons/openInspector.png
--rw-r--r--   0        0        0     2319 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/resources/icons/plot.png
--rw-r--r--   0        0        0     2114 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/resources/icons/pointer.png
--rw-r--r--   0        0        0     4377 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/resources/icons/previous.png
--rw-r--r--   0        0        0     4841 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/resources/icons/rectangle.png
--rw-r--r--   0        0        0     1916 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/resources/icons/remove.png
--rw-r--r--   0        0        0    10041 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/resources/icons/satellite.svg
--rw-r--r--   0        0        0     1334 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/resources/icons/save.png
--rw-r--r--   0        0        0    85300 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/resources/icons/sciqlop2PNG_1024.png
--rw-r--r--   0        0        0     3714 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/resources/icons/time.png
--rw-r--r--   0        0        0     1084 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/resources/icons/trash.png
--rw-r--r--   0        0        0     2234 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/resources/icons/unplot.png
--rw-r--r--   0        0        0     1197 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/resources/icons/up.png
--rw-r--r--   0        0        0     4056 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/resources/icons/zoom.png
--rw-r--r--   0        0        0     1249 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/resources/resources.qrc
--rw-r--r--   0        0        0        0 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/widgets/__init__.py
--rw-r--r--   0        0        0     3758 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/widgets/central_widget.py
--rw-r--r--   0        0        0       31 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/widgets/common/__init__.py
--rw-r--r--   0        0        0     1005 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/widgets/common/tree_view.py
--rw-r--r--   0        0        0     2499 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/widgets/console.py
--rw-r--r--   0        0        0     3102 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/widgets/datetime_range.py
--rw-r--r--   0        0        0      157 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/widgets/drag_and_drop/__init__.py
--rw-r--r--   0        0        0      282 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/widgets/drag_and_drop/drop_handler.py
--rw-r--r--   0        0        0     2450 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/widgets/drag_and_drop/helper.py
--rw-r--r--   0        0        0     3120 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/widgets/drag_and_drop/place_holder_manager.py
--rw-r--r--   0        0        0     1134 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/widgets/drag_and_drop/placeholder.py
--rw-r--r--   0        0        0     4651 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/widgets/mainwindow.py
--rw-r--r--   0        0        0       39 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/widgets/pipelines/__init__.py
--rw-r--r--   0        0        0     2085 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/widgets/pipelines/pipeline_tree.py
--rw-r--r--   0        0        0        0 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/widgets/plots/__init__.py
--rw-r--r--   0        0        0     3451 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/widgets/plots/colormap_graph.py
--rw-r--r--   0        0        0     1719 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/widgets/plots/line_graph.py
--rw-r--r--   0        0        0    10327 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/widgets/plots/time_series_plot.py
--rw-r--r--   0        0        0     1556 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/widgets/plots/time_span.py
--rw-r--r--   0        0        0     1050 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/widgets/plots/time_span_controller.py
--rw-r--r--   0        0        0     7663 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/widgets/plots/time_sync_panel.py
--rw-r--r--   0        0        0       39 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/widgets/products_tree/__init__.py
--rw-r--r--   0        0        0     1378 2023-04-25 07:43:34.641641 SciQLop-0.2.1/SciQLop/widgets/products_tree/products_tree.py
--rw-r--r--   0        0        0     1364 2023-04-25 07:43:34.645641 SciQLop-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     3039 1970-01-01 00:00:00.000000 SciQLop-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    35147 2023-06-04 21:19:52.159462 sciqlop-0.3.0/COPYING
+-rw-r--r--   0        0        0     4594 2023-06-04 21:19:52.159462 sciqlop-0.3.0/README.md
+-rw-r--r--   0        0        0       23 2023-06-04 21:19:52.159462 sciqlop-0.3.0/SciQLop/__init__.py
+-rw-r--r--   0        0        0     1276 2023-06-04 21:19:52.159462 sciqlop-0.3.0/SciQLop/app.py
+-rw-r--r--   0        0        0     1433 2023-06-04 21:19:52.159462 sciqlop-0.3.0/SciQLop/backend/__init__.py
+-rw-r--r--   0        0        0      532 2023-06-04 21:19:52.159462 sciqlop-0.3.0/SciQLop/backend/enums.py
+-rw-r--r--   0        0        0      831 2023-06-04 21:19:52.159462 sciqlop-0.3.0/SciQLop/backend/logging/__init__.py
+-rw-r--r--   0        0        0      172 2023-06-04 21:19:52.159462 sciqlop-0.3.0/SciQLop/backend/models.py
+-rw-r--r--   0        0        0        1 2023-06-04 21:19:52.159462 sciqlop-0.3.0/SciQLop/backend/pipelines_model/__init__.py
+-rw-r--r--   0        0        0     5204 2023-06-04 21:19:52.159462 sciqlop-0.3.0/SciQLop/backend/pipelines_model/auto_register.py
+-rw-r--r--   0        0        0      128 2023-06-04 21:19:52.159462 sciqlop-0.3.0/SciQLop/backend/pipelines_model/base/__init__.py
+-rw-r--r--   0        0        0     6856 2023-06-04 21:19:52.159462 sciqlop-0.3.0/SciQLop/backend/pipelines_model/base/model.py
+-rw-r--r--   0        0        0     2925 2023-06-04 21:19:52.159462 sciqlop-0.3.0/SciQLop/backend/pipelines_model/base/pipeline_node.py
+-rw-r--r--   0        0        0     5352 2023-06-04 21:19:52.159462 sciqlop-0.3.0/SciQLop/backend/pipelines_model/data_pipeline.py
+-rw-r--r--   0        0        0      718 2023-06-04 21:19:52.159462 sciqlop-0.3.0/SciQLop/backend/pipelines_model/data_provider.py
+-rw-r--r--   0        0        0     3310 2023-06-04 21:19:52.159462 sciqlop-0.3.0/SciQLop/backend/pipelines_model/easy_provider.py
+-rw-r--r--   0        0        0     3820 2023-06-04 21:19:52.159462 sciqlop-0.3.0/SciQLop/backend/pipelines_model/graph.py
+-rw-r--r--   0        0        0        0 2023-06-04 21:19:52.159462 sciqlop-0.3.0/SciQLop/backend/products_model/__init__.py
+-rw-r--r--   0        0        0     6549 2023-06-04 21:19:52.159462 sciqlop-0.3.0/SciQLop/backend/products_model/model.py
+-rw-r--r--   0        0        0     3195 2023-06-04 21:19:52.159462 sciqlop-0.3.0/SciQLop/backend/products_model/product_node.py
+-rw-r--r--   0        0        0        0 2023-06-04 21:19:52.159462 sciqlop-0.3.0/SciQLop/backend/resampling/__init__.py
+-rw-r--r--   0        0        0     1365 2023-06-04 21:19:52.159462 sciqlop-0.3.0/SciQLop/backend/resampling/spectro_regrid.py
+-rw-r--r--   0        0        0      186 2023-06-04 21:19:52.159462 sciqlop-0.3.0/SciQLop/backend/unique_names.py
+-rw-r--r--   0        0        0     1645 2023-06-04 21:19:52.159462 sciqlop-0.3.0/SciQLop/mime/__init__.py
+-rw-r--r--   0        0        0      120 2023-06-04 21:19:52.159462 sciqlop-0.3.0/SciQLop/mime/types.py
+-rw-r--r--   0        0        0     2279 2023-06-04 21:19:52.159462 sciqlop-0.3.0/SciQLop/plugins/__init__.py
+-rw-r--r--   0        0        0      181 2023-06-04 21:19:52.159462 sciqlop-0.3.0/SciQLop/plugins/catalogs/__init__.py
+-rw-r--r--   0        0        0     1555 2023-06-04 21:19:52.159462 sciqlop-0.3.0/SciQLop/plugins/catalogs/catalogs.py
+-rw-r--r--   0        0        0     4306 2023-06-04 21:19:52.159462 sciqlop-0.3.0/SciQLop/plugins/catalogs/lightweight_manager/__init__.py
+-rw-r--r--   0        0        0     2379 2023-06-04 21:19:52.159462 sciqlop-0.3.0/SciQLop/plugins/catalogs/lightweight_manager/catalog_selector.py
+-rw-r--r--   0        0        0     1728 2023-06-04 21:19:52.159462 sciqlop-0.3.0/SciQLop/plugins/catalogs/lightweight_manager/event_selector.py
+-rw-r--r--   0        0        0     3906 2023-06-04 21:19:52.159462 sciqlop-0.3.0/SciQLop/plugins/speasy.py
+-rw-r--r--   0        0        0     1419 2023-06-04 21:19:52.159462 sciqlop-0.3.0/SciQLop/plugins/test_plugin.py
+-rw-r--r--   0        0        0   552261 2023-06-04 21:19:52.163462 sciqlop-0.3.0/SciQLop/resources/__init__.py
+-rw-r--r--   0        0        0   118794 2023-06-04 21:19:52.163462 sciqlop-0.3.0/SciQLop/resources/icons/SciQLop.png
+-rw-r--r--   0        0        0     3191 2023-06-04 21:19:52.163462 sciqlop-0.3.0/SciQLop/resources/icons/Simple_icon_time.svg
+-rw-r--r--   0        0        0     1956 2023-06-04 21:19:52.163462 sciqlop-0.3.0/SciQLop/resources/icons/add.png
+-rw-r--r--   0        0        0     2001 2023-06-04 21:19:52.163462 sciqlop-0.3.0/SciQLop/resources/icons/allEvents.png
+-rw-r--r--   0        0        0      615 2023-06-04 21:19:52.163462 sciqlop-0.3.0/SciQLop/resources/icons/catalogue.png
+-rw-r--r--   0        0        0     1003 2023-06-04 21:19:52.163462 sciqlop-0.3.0/SciQLop/resources/icons/chart.png
+-rw-r--r--   0        0        0     1047 2023-06-04 21:19:52.163462 sciqlop-0.3.0/SciQLop/resources/icons/cursor.png
+-rw-r--r--   0        0        0     2150 2023-06-04 21:19:52.163462 sciqlop-0.3.0/SciQLop/resources/icons/dataSourceComponent.png
+-rw-r--r--   0        0        0      882 2023-06-04 21:19:52.163462 sciqlop-0.3.0/SciQLop/resources/icons/dataSourceNode.png
+-rw-r--r--   0        0        0     1213 2023-06-04 21:19:52.163462 sciqlop-0.3.0/SciQLop/resources/icons/dataSourceProduct.png
+-rw-r--r--   0        0        0     4821 2023-06-04 21:19:52.163462 sciqlop-0.3.0/SciQLop/resources/icons/dataSourceRoot.png
+-rw-r--r--   0        0        0      788 2023-06-04 21:19:52.163462 sciqlop-0.3.0/SciQLop/resources/icons/database.png
+-rw-r--r--   0        0        0      834 2023-06-04 21:19:52.163462 sciqlop-0.3.0/SciQLop/resources/icons/delete.png
+-rwxr-xr-x   0        0        0     1266 2023-06-04 21:19:52.163462 sciqlop-0.3.0/SciQLop/resources/icons/discard.png
+-rw-r--r--   0        0        0     1231 2023-06-04 21:19:52.163462 sciqlop-0.3.0/SciQLop/resources/icons/down.png
+-rw-r--r--   0        0        0     1731 2023-06-04 21:19:52.163462 sciqlop-0.3.0/SciQLop/resources/icons/drag.png
+-rw-r--r--   0        0        0     4413 2023-06-04 21:19:52.163462 sciqlop-0.3.0/SciQLop/resources/icons/next.png
+-rwxr-xr-x   0        0        0     1450 2023-06-04 21:19:52.163462 sciqlop-0.3.0/SciQLop/resources/icons/openInspector.png
+-rw-r--r--   0        0        0     2319 2023-06-04 21:19:52.163462 sciqlop-0.3.0/SciQLop/resources/icons/plot.png
+-rw-r--r--   0        0        0     2114 2023-06-04 21:19:52.163462 sciqlop-0.3.0/SciQLop/resources/icons/pointer.png
+-rw-r--r--   0        0        0     4377 2023-06-04 21:19:52.163462 sciqlop-0.3.0/SciQLop/resources/icons/previous.png
+-rw-r--r--   0        0        0     4841 2023-06-04 21:19:52.163462 sciqlop-0.3.0/SciQLop/resources/icons/rectangle.png
+-rw-r--r--   0        0        0     1916 2023-06-04 21:19:52.163462 sciqlop-0.3.0/SciQLop/resources/icons/remove.png
+-rw-r--r--   0        0        0    10041 2023-06-04 21:19:52.163462 sciqlop-0.3.0/SciQLop/resources/icons/satellite.svg
+-rw-r--r--   0        0        0     1334 2023-06-04 21:19:52.163462 sciqlop-0.3.0/SciQLop/resources/icons/save.png
+-rw-r--r--   0        0        0    85300 2023-06-04 21:19:52.163462 sciqlop-0.3.0/SciQLop/resources/icons/sciqlop2PNG_1024.png
+-rw-r--r--   0        0        0     3714 2023-06-04 21:19:52.163462 sciqlop-0.3.0/SciQLop/resources/icons/time.png
+-rw-r--r--   0        0        0     1084 2023-06-04 21:19:52.163462 sciqlop-0.3.0/SciQLop/resources/icons/trash.png
+-rw-r--r--   0        0        0     2234 2023-06-04 21:19:52.163462 sciqlop-0.3.0/SciQLop/resources/icons/unplot.png
+-rw-r--r--   0        0        0     1197 2023-06-04 21:19:52.163462 sciqlop-0.3.0/SciQLop/resources/icons/up.png
+-rw-r--r--   0        0        0     4056 2023-06-04 21:19:52.163462 sciqlop-0.3.0/SciQLop/resources/icons/zoom.png
+-rw-r--r--   0        0        0     1249 2023-06-04 21:19:52.163462 sciqlop-0.3.0/SciQLop/resources/resources.qrc
+-rw-r--r--   0        0        0        0 2023-06-04 21:19:52.163462 sciqlop-0.3.0/SciQLop/widgets/__init__.py
+-rw-r--r--   0        0        0     3758 2023-06-04 21:19:52.163462 sciqlop-0.3.0/SciQLop/widgets/central_widget.py
+-rw-r--r--   0        0        0       31 2023-06-04 21:19:52.167462 sciqlop-0.3.0/SciQLop/widgets/common/__init__.py
+-rw-r--r--   0        0        0     1005 2023-06-04 21:19:52.167462 sciqlop-0.3.0/SciQLop/widgets/common/tree_view.py
+-rw-r--r--   0        0        0     2499 2023-06-04 21:19:52.167462 sciqlop-0.3.0/SciQLop/widgets/console.py
+-rw-r--r--   0        0        0     3102 2023-06-04 21:19:52.167462 sciqlop-0.3.0/SciQLop/widgets/datetime_range.py
+-rw-r--r--   0        0        0      157 2023-06-04 21:19:52.167462 sciqlop-0.3.0/SciQLop/widgets/drag_and_drop/__init__.py
+-rw-r--r--   0        0        0      282 2023-06-04 21:19:52.167462 sciqlop-0.3.0/SciQLop/widgets/drag_and_drop/drop_handler.py
+-rw-r--r--   0        0        0     2450 2023-06-04 21:19:52.167462 sciqlop-0.3.0/SciQLop/widgets/drag_and_drop/helper.py
+-rw-r--r--   0        0        0     3120 2023-06-04 21:19:52.167462 sciqlop-0.3.0/SciQLop/widgets/drag_and_drop/place_holder_manager.py
+-rw-r--r--   0        0        0     1134 2023-06-04 21:19:52.167462 sciqlop-0.3.0/SciQLop/widgets/drag_and_drop/placeholder.py
+-rw-r--r--   0        0        0     4814 2023-06-04 21:19:52.167462 sciqlop-0.3.0/SciQLop/widgets/mainwindow.py
+-rw-r--r--   0        0        0       39 2023-06-04 21:19:52.167462 sciqlop-0.3.0/SciQLop/widgets/pipelines/__init__.py
+-rw-r--r--   0        0        0     2085 2023-06-04 21:19:52.167462 sciqlop-0.3.0/SciQLop/widgets/pipelines/pipeline_tree.py
+-rw-r--r--   0        0        0        0 2023-06-04 21:19:52.167462 sciqlop-0.3.0/SciQLop/widgets/plots/__init__.py
+-rw-r--r--   0        0        0     3451 2023-06-04 21:19:52.167462 sciqlop-0.3.0/SciQLop/widgets/plots/colormap_graph.py
+-rw-r--r--   0        0        0     1720 2023-06-04 21:19:52.167462 sciqlop-0.3.0/SciQLop/widgets/plots/line_graph.py
+-rw-r--r--   0        0        0    10433 2023-06-04 21:19:52.167462 sciqlop-0.3.0/SciQLop/widgets/plots/time_series_plot.py
+-rw-r--r--   0        0        0     1556 2023-06-04 21:19:52.167462 sciqlop-0.3.0/SciQLop/widgets/plots/time_span.py
+-rw-r--r--   0        0        0     1050 2023-06-04 21:19:52.167462 sciqlop-0.3.0/SciQLop/widgets/plots/time_span_controller.py
+-rw-r--r--   0        0        0     7665 2023-06-04 21:19:52.167462 sciqlop-0.3.0/SciQLop/widgets/plots/time_sync_panel.py
+-rw-r--r--   0        0        0       39 2023-06-04 21:19:52.167462 sciqlop-0.3.0/SciQLop/widgets/products_tree/__init__.py
+-rw-r--r--   0        0        0     1378 2023-06-04 21:19:52.167462 sciqlop-0.3.0/SciQLop/widgets/products_tree/products_tree.py
+-rw-r--r--   0        0        0     1371 2023-06-04 21:19:52.171462 sciqlop-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5781 1970-01-01 00:00:00.000000 sciqlop-0.3.0/PKG-INFO
```

### Comparing `SciQLop-0.2.1/COPYING` & `sciqlop-0.3.0/COPYING`

 * *Files identical despite different names*

### Comparing `SciQLop-0.2.1/SciQLop/app.py` & `sciqlop-0.3.0/SciQLop/app.py`

 * *Files identical despite different names*

### Comparing `SciQLop-0.2.1/SciQLop/backend/__init__.py` & `sciqlop-0.3.0/SciQLop/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `SciQLop-0.2.1/SciQLop/backend/enums.py` & `sciqlop-0.3.0/SciQLop/backend/enums.py`

 * *Files identical despite different names*

### Comparing `SciQLop-0.2.1/SciQLop/backend/logging/__init__.py` & `sciqlop-0.3.0/SciQLop/backend/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `SciQLop-0.2.1/SciQLop/backend/pipelines_model/auto_register.py` & `sciqlop-0.3.0/SciQLop/backend/pipelines_model/auto_register.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,15 @@
                 return n
 
     def _update_wrapped_object(self):
         if self._wrapped_object is not None:
             if hasattr(self._wrapped_object, 'model_please_delete_me'):
                 self._wrapped_object.model_please_delete_me.connect(self.delete_node)
             self._wrapped_class_name = self._wrapped_object.__class__.__name__
-            log.info(f"Setting wrapped object {self._wrapped_class_name}:{self._wrapped_object}")
+            log.debug(f"Setting wrapped object {self._wrapped_class_name}:{self._wrapped_object}")
             self._wrapped_object.destroyed.connect(self._wrapped_object_deleted)
 
     @property
     def wrapped_object(self):
         return self._wrapped_object
 
     @wrapped_object.setter
@@ -135,15 +135,15 @@
         self._cleanup()
         with model.model_update_ctx():
             self.setParent(None)
         self.deleteLater()
 
     def __del__(self):
         self._cleanup()
-        log.info(f"Deleting {self._wrapped_class_name}: {id(self):08x}")
+        log.debug(f"Deleting {self._wrapped_class_name}: {id(self):08x}")
 
     def __eq__(self, other: PipelineModelItem) -> bool:
         if other is not None:
             return self.parent_node == other.parent_node and self.row == other.row
         return False
```

### Comparing `SciQLop-0.2.1/SciQLop/backend/pipelines_model/base/model.py` & `sciqlop-0.3.0/SciQLop/backend/pipelines_model/base/model.py`

 * *Files identical despite different names*

### Comparing `SciQLop-0.2.1/SciQLop/backend/pipelines_model/base/pipeline_node.py` & `sciqlop-0.3.0/SciQLop/backend/pipelines_model/base/pipeline_node.py`

 * *Files identical despite different names*

### Comparing `SciQLop-0.2.1/SciQLop/backend/pipelines_model/data_pipeline.py` & `sciqlop-0.3.0/SciQLop/backend/pipelines_model/data_pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,30 +46,30 @@
     def get_data(self, new_range: TimeRange):
         self.range_mutex.lock()
         self.next_range = new_range
         self.range_mutex.unlock()
         self._get_data_sig.emit()
 
     def __del__(self):
-        log.info(f"Dtor {self.__class__.__name__}: {id(self):08x}")
+        log.debug(f"Dtor {self.__class__.__name__}: {id(self):08x}")
 
 
 class _DataPipelineController(QThread):
     def __init__(self, data_callback: Callable[[SpeasyVariable], None], product: ProductNode, time_range: TimeRange):
         QThread.__init__(self)
         self.setTerminationEnabled(True)
         self.wait_condition = QWaitCondition()
         self.next_range: Optional[TimeRange] = time_range
         self.current_range: Optional[TimeRange] = None
         self._worker = _DataPipelineWorker(data_callback, product, time_range)
         self.moveToThread(self)
         self.start()
 
     def __del__(self):
-        log.info(f"Dtor {self.__class__.__name__}: {id(self):08x}")
+        log.debug(f"Dtor {self.__class__.__name__}: {id(self):08x}")
         self._worker.requestInterruption()
         self._worker.wait_condition.wakeOne()
         self._worker.wait(1000)
 
     def run(self):
         mutex = QMutex()
         while not QThread.currentThread().isInterruptionRequested():
@@ -104,15 +104,15 @@
         if self._worker_thread:
             self._worker_thread.quit()
             self._worker_thread.wait()
             self._worker_thread.deleteLater()
             self._worker_thread = None
 
     def __del__(self):
-        log.info(f"Dtor {self.__class__.__name__}: {id(self):08x}")
+        log.debug(f"Dtor {self.__class__.__name__}: {id(self):08x}")
         self.close()
 
     def get_data(self, new_range: TimeRange):
         if self._worker_thread:
             self._worker.get_data(new_range)
 
     def __eq__(self, other: 'PipelineModelItem') -> bool:
```

### Comparing `SciQLop-0.2.1/SciQLop/backend/pipelines_model/data_provider.py` & `sciqlop-0.3.0/SciQLop/backend/pipelines_model/data_provider.py`

 * *Files identical despite different names*

### Comparing `SciQLop-0.2.1/SciQLop/backend/pipelines_model/graph.py` & `sciqlop-0.3.0/SciQLop/backend/pipelines_model/graph.py`

 * *Files identical despite different names*

### Comparing `SciQLop-0.2.1/SciQLop/backend/products_model/model.py` & `sciqlop-0.3.0/SciQLop/backend/products_model/model.py`

 * *Files identical despite different names*

### Comparing `SciQLop-0.2.1/SciQLop/backend/products_model/product_node.py` & `sciqlop-0.3.0/SciQLop/backend/products_model/product_node.py`

 * *Files identical despite different names*

### Comparing `SciQLop-0.2.1/SciQLop/backend/resampling/spectro_regrid.py` & `sciqlop-0.3.0/SciQLop/backend/resampling/spectro_regrid.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,26 +2,33 @@
 from speasy.products import SpeasyVariable
 from scipy.interpolate import griddata
 from typing import Tuple
 
 
 def regrid(v: SpeasyVariable) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
     t: np.ndarray = v.time.astype(np.timedelta64) / np.timedelta64(1, 's')
-    new_t = np.linspace(t[0], t[-1], num=min(10000, len(t)), endpoint=False)
+    resampled_t = np.linspace(t[0], t[-1], num=min(10000, len(t)), endpoint=False)
+    values = v.values
+
     if len(v.axes) == 1:
         y = np.arange(v.values.shape[1]) * 1.
-    else:
+    elif len(v.axes[1].values.shape) == 1:
+        y = np.nan_to_num(v.axes[1].values.astype(np.float64), nan=0., copy=False)
+    elif v.axes[1].values.shape[0] == 1:
         y = np.nan_to_num(v.axes[1].values.astype(np.float64), nan=0., copy=False)
-    if len(y.shape) == 2:
+        y = y.flatten()
+    else:
+        y = v.axes[1].values.astype(np.float64)
         new_y = np.logspace(np.log10(np.nanmin(y)), np.log10(np.nanmax(y)), num=int(4 * y.shape[1]))
-        values = v.values
-        values = griddata((np.repeat(t, y.shape[1]), y.ravel()), values.ravel(),
-                          (np.repeat(new_t, len(new_y)), np.tile(new_y, len(new_t))), method='nearest',
+        y = np.nan_to_num(y, nan=0., copy=False)
+
+        values = griddata((np.repeat(t, y.shape[1]), y.ravel()),
+                          values.ravel(),
+                          (np.repeat(resampled_t, len(new_y)), np.tile(new_y, len(resampled_t))),
+                          method='nearest',
                           fill_value=np.nan)
-    else:
-        new_y = y
-        values = v.values
+        y = new_y
 
     if values.dtype != np.float64:
         values = values.astype(np.float64)
 
-    return new_t, new_y, values
+    return resampled_t, y, values
```

### Comparing `SciQLop-0.2.1/SciQLop/mime/__init__.py` & `sciqlop-0.3.0/SciQLop/mime/__init__.py`

 * *Files identical despite different names*

### Comparing `SciQLop-0.2.1/SciQLop/plugins/__init__.py` & `sciqlop-0.3.0/SciQLop/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `SciQLop-0.2.1/SciQLop/plugins/catalogs/catalogs.py` & `sciqlop-0.3.0/SciQLop/plugins/catalogs/catalogs.py`

 * *Files identical despite different names*

### Comparing `SciQLop-0.2.1/SciQLop/plugins/catalogs/lightweight_manager/__init__.py` & `sciqlop-0.3.0/SciQLop/plugins/catalogs/lightweight_manager/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,15 +70,19 @@
             events += c.events
         self.event_selector.update_list(events)
         self.update_spans()
 
     @Slot()
     def event_selected(self, event):
         if self.follow_selected_event.isChecked() and self.current_panel is not None:
-            self.current_panel.time_range = TimeRange(event.start.timestamp(), event.stop.timestamp()) * 1.3
+            log.debug(f"event selected {event}, setting panel: {self.current_panel}")
+            if event.start == event.stop:
+                self.current_panel.time_range = TimeRange(event.start.timestamp() - 3600, event.stop.timestamp() + 3600)
+            else:
+                self.current_panel.time_range = TimeRange(event.start.timestamp(), event.stop.timestamp()) * 1.3
 
     def update_spans(self):
         if self.current_panel is not None:
             self._time_span_ctrlr = TimeSpanController(parent=self, plot_panel=self.current_panel)
             ro = not self.allow_edition.isChecked()
             self.spans = [
                 TimeSpan(TimeRange(event.start.timestamp(), event.stop.timestamp()), plot_panel=self.current_panel,
```

### Comparing `SciQLop-0.2.1/SciQLop/plugins/catalogs/lightweight_manager/catalog_selector.py` & `sciqlop-0.3.0/SciQLop/plugins/catalogs/lightweight_manager/catalog_selector.py`

 * *Files identical despite different names*

### Comparing `SciQLop-0.2.1/SciQLop/plugins/catalogs/lightweight_manager/event_selector.py` & `sciqlop-0.3.0/SciQLop/plugins/catalogs/lightweight_manager/event_selector.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,15 @@
             item.setData(event.uuid, Qt.UserRole)
             item.setText(f"{event.start}:{event.stop}")
             self.model.setItem(index, item)
             self._events[event.uuid] = event
 
     def _event_selected(self, selected: QItemSelection, deselected: QItemSelection):
         indexes = selected.indexes()
-        if len(indexes):
+        if len(indexes) and len(self._events):
             item = self.model.itemFromIndex(indexes[0])
             self.event_selected.emit(self._events[item.data(Qt.UserRole)])
 
     @property
     def events(self):
         return self._events.values()
```

### Comparing `SciQLop-0.2.1/SciQLop/plugins/speasy.py` & `sciqlop-0.3.0/SciQLop/plugins/speasy.py`

 * *Files identical despite different names*

### Comparing `SciQLop-0.2.1/SciQLop/plugins/test_plugin.py` & `sciqlop-0.3.0/SciQLop/plugins/test_plugin.py`

 * *Files identical despite different names*

### Comparing `SciQLop-0.2.1/SciQLop/resources/__init__.py` & `sciqlop-0.3.0/SciQLop/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `SciQLop-0.2.1/SciQLop/resources/icons/SciQLop.png` & `sciqlop-0.3.0/SciQLop/resources/icons/SciQLop.png`

 * *Files identical despite different names*

### Comparing `SciQLop-0.2.1/SciQLop/resources/icons/Simple_icon_time.svg` & `sciqlop-0.3.0/SciQLop/resources/icons/Simple_icon_time.svg`

 * *Files identical despite different names*

### Comparing `SciQLop-0.2.1/SciQLop/resources/icons/add.png` & `sciqlop-0.3.0/SciQLop/resources/icons/add.png`

 * *Files identical despite different names*

### Comparing `SciQLop-0.2.1/SciQLop/resources/icons/allEvents.png` & `sciqlop-0.3.0/SciQLop/resources/icons/allEvents.png`

 * *Files identical despite different names*

### Comparing `SciQLop-0.2.1/SciQLop/resources/icons/catalogue.png` & `sciqlop-0.3.0/SciQLop/resources/icons/catalogue.png`

 * *Files identical despite different names*

### Comparing `SciQLop-0.2.1/SciQLop/resources/icons/chart.png` & `sciqlop-0.3.0/SciQLop/resources/icons/chart.png`

 * *Files identical despite different names*

### Comparing `SciQLop-0.2.1/SciQLop/resources/icons/cursor.png` & `sciqlop-0.3.0/SciQLop/resources/icons/cursor.png`

 * *Files identical despite different names*

### Comparing `SciQLop-0.2.1/SciQLop/resources/icons/dataSourceComponent.png` & `sciqlop-0.3.0/SciQLop/resources/icons/dataSourceComponent.png`

 * *Files identical despite different names*

### Comparing `SciQLop-0.2.1/SciQLop/resources/icons/dataSourceNode.png` & `sciqlop-0.3.0/SciQLop/resources/icons/dataSourceNode.png`

 * *Files identical despite different names*

### Comparing `SciQLop-0.2.1/SciQLop/resources/icons/dataSourceProduct.png` & `sciqlop-0.3.0/SciQLop/resources/icons/dataSourceProduct.png`

 * *Files identical despite different names*

### Comparing `SciQLop-0.2.1/SciQLop/resources/icons/dataSourceRoot.png` & `sciqlop-0.3.0/SciQLop/resources/icons/dataSourceRoot.png`

 * *Files identical despite different names*

### Comparing `SciQLop-0.2.1/SciQLop/resources/icons/database.png` & `sciqlop-0.3.0/SciQLop/resources/icons/database.png`

 * *Files identical despite different names*

### Comparing `SciQLop-0.2.1/SciQLop/resources/icons/delete.png` & `sciqlop-0.3.0/SciQLop/resources/icons/delete.png`

 * *Files identical despite different names*

### Comparing `SciQLop-0.2.1/SciQLop/resources/icons/discard.png` & `sciqlop-0.3.0/SciQLop/resources/icons/discard.png`

 * *Files identical despite different names*

### Comparing `SciQLop-0.2.1/SciQLop/resources/icons/down.png` & `sciqlop-0.3.0/SciQLop/resources/icons/down.png`

 * *Files identical despite different names*

### Comparing `SciQLop-0.2.1/SciQLop/resources/icons/drag.png` & `sciqlop-0.3.0/SciQLop/resources/icons/drag.png`

 * *Files identical despite different names*

### Comparing `SciQLop-0.2.1/SciQLop/resources/icons/next.png` & `sciqlop-0.3.0/SciQLop/resources/icons/next.png`

 * *Files identical despite different names*

### Comparing `SciQLop-0.2.1/SciQLop/resources/icons/openInspector.png` & `sciqlop-0.3.0/SciQLop/resources/icons/openInspector.png`

 * *Files identical despite different names*

### Comparing `SciQLop-0.2.1/SciQLop/resources/icons/plot.png` & `sciqlop-0.3.0/SciQLop/resources/icons/plot.png`

 * *Files identical despite different names*

### Comparing `SciQLop-0.2.1/SciQLop/resources/icons/pointer.png` & `sciqlop-0.3.0/SciQLop/resources/icons/pointer.png`

 * *Files identical despite different names*

### Comparing `SciQLop-0.2.1/SciQLop/resources/icons/previous.png` & `sciqlop-0.3.0/SciQLop/resources/icons/previous.png`

 * *Files identical despite different names*

### Comparing `SciQLop-0.2.1/SciQLop/resources/icons/rectangle.png` & `sciqlop-0.3.0/SciQLop/resources/icons/rectangle.png`

 * *Files identical despite different names*

### Comparing `SciQLop-0.2.1/SciQLop/resources/icons/remove.png` & `sciqlop-0.3.0/SciQLop/resources/icons/remove.png`

 * *Files identical despite different names*

### Comparing `SciQLop-0.2.1/SciQLop/resources/icons/satellite.svg` & `sciqlop-0.3.0/SciQLop/resources/icons/satellite.svg`

 * *Files identical despite different names*

### Comparing `SciQLop-0.2.1/SciQLop/resources/icons/save.png` & `sciqlop-0.3.0/SciQLop/resources/icons/save.png`

 * *Files identical despite different names*

### Comparing `SciQLop-0.2.1/SciQLop/resources/icons/sciqlop2PNG_1024.png` & `sciqlop-0.3.0/SciQLop/resources/icons/sciqlop2PNG_1024.png`

 * *Files identical despite different names*

### Comparing `SciQLop-0.2.1/SciQLop/resources/icons/time.png` & `sciqlop-0.3.0/SciQLop/resources/icons/time.png`

 * *Files identical despite different names*

### Comparing `SciQLop-0.2.1/SciQLop/resources/icons/trash.png` & `sciqlop-0.3.0/SciQLop/resources/icons/trash.png`

 * *Files identical despite different names*

### Comparing `SciQLop-0.2.1/SciQLop/resources/icons/unplot.png` & `sciqlop-0.3.0/SciQLop/resources/icons/unplot.png`

 * *Files identical despite different names*

### Comparing `SciQLop-0.2.1/SciQLop/resources/icons/up.png` & `sciqlop-0.3.0/SciQLop/resources/icons/up.png`

 * *Files identical despite different names*

### Comparing `SciQLop-0.2.1/SciQLop/resources/icons/zoom.png` & `sciqlop-0.3.0/SciQLop/resources/icons/zoom.png`

 * *Files identical despite different names*

### Comparing `SciQLop-0.2.1/SciQLop/resources/resources.qrc` & `sciqlop-0.3.0/SciQLop/resources/resources.qrc`

 * *Files identical despite different names*

### Comparing `SciQLop-0.2.1/SciQLop/widgets/central_widget.py` & `sciqlop-0.3.0/SciQLop/widgets/central_widget.py`

 * *Files identical despite different names*

### Comparing `SciQLop-0.2.1/SciQLop/widgets/common/tree_view.py` & `sciqlop-0.3.0/SciQLop/widgets/common/tree_view.py`

 * *Files identical despite different names*

### Comparing `SciQLop-0.2.1/SciQLop/widgets/console.py` & `sciqlop-0.3.0/SciQLop/widgets/console.py`

 * *Files identical despite different names*

### Comparing `SciQLop-0.2.1/SciQLop/widgets/datetime_range.py` & `sciqlop-0.3.0/SciQLop/widgets/datetime_range.py`

 * *Files identical despite different names*

### Comparing `SciQLop-0.2.1/SciQLop/widgets/drag_and_drop/helper.py` & `sciqlop-0.3.0/SciQLop/widgets/drag_and_drop/helper.py`

 * *Files identical despite different names*

### Comparing `SciQLop-0.2.1/SciQLop/widgets/drag_and_drop/place_holder_manager.py` & `sciqlop-0.3.0/SciQLop/widgets/drag_and_drop/place_holder_manager.py`

 * *Files identical despite different names*

### Comparing `SciQLop-0.2.1/SciQLop/widgets/drag_and_drop/placeholder.py` & `sciqlop-0.3.0/SciQLop/widgets/drag_and_drop/placeholder.py`

 * *Files identical despite different names*

### Comparing `SciQLop-0.2.1/SciQLop/widgets/mainwindow.py` & `sciqlop-0.3.0/SciQLop/widgets/mainwindow.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 from datetime import datetime, timedelta
 
 import PySide6QtAds as QtAds
 from PySide6 import QtCore, QtWidgets, QtGui
 from PySide6.QtGui import QCloseEvent
 from PySide6.QtWidgets import QWidget, QSizePolicy, QMenu
 
@@ -19,14 +20,16 @@
     def __init__(self):
 
         QtWidgets.QMainWindow.__init__(self)
         self._setup_ui()
 
     def _setup_ui(self):
         QtAds.CDockManager.setAutoHideConfigFlag(QtAds.CDockManager.DefaultAutoHideConfig)
+        if "WAYLAND_DISPLAY" in os.environ:
+            QtAds.CDockManager.setConfigFlag(QtAds.CDockManager.FloatingContainerForceQWidgetTitleBar, True)
         self.dock_manager = QtAds.CDockManager(self)
         self._menubar = QtWidgets.QMenuBar(self)
         self.setMenuBar(self._menubar)
         self._menubar.setGeometry(QtCore.QRect(0, 0, 615, 23))
         self._menubar.setDefaultUp(True)
         self.viewMenu = QMenu("View")
         self._menubar.addMenu(self.viewMenu)
```

### Comparing `SciQLop-0.2.1/SciQLop/widgets/pipelines/pipeline_tree.py` & `sciqlop-0.3.0/SciQLop/widgets/pipelines/pipeline_tree.py`

 * *Files identical despite different names*

### Comparing `SciQLop-0.2.1/SciQLop/widgets/plots/colormap_graph.py` & `sciqlop-0.3.0/SciQLop/widgets/plots/colormap_graph.py`

 * *Files identical despite different names*

### Comparing `SciQLop-0.2.1/SciQLop/widgets/plots/line_graph.py` & `sciqlop-0.3.0/SciQLop/widgets/plots/line_graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,8 +38,8 @@
     def graphAt(self, index: int):
         return self.graph.graphAt(index)
 
     def close(self):
         super().close()
 
     def __del__(self):
-        log.info(f"Dtor {self.__class__.__name__}: {id(self):08x}")
+        log.debug(f"Dtor {self.__class__.__name__}: {id(self):08x}")
```

### Comparing `SciQLop-0.2.1/SciQLop/widgets/plots/time_series_plot.py` & `sciqlop-0.3.0/SciQLop/widgets/plots/time_series_plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,17 @@
 from ..drag_and_drop import DropHandler, DropHelper
 from ...backend import Product
 from ...backend import TimeRange
 from ...backend.enums import ParameterType, DataOrder
 from ...backend.unique_names import make_simple_incr_name
 from ...mime import decode_mime
 from ...mime.types import PRODUCT_LIST_MIME_TYPE, TIME_RANGE_MIME_TYPE
+from ...backend import logging
+
+log = logging.getLogger(__name__)
 
 
 def _to_qcolor(r: float, g: float, b: float):
     return QColor(int(r * 255), int(g * 255), int(b * 255))
 
 
 def _configure_plot(plot: SciQLopPlot):
@@ -58,15 +61,14 @@
 class MetaTimeSeriesPlot(type(QFrame), type(PipelineModelItem)):
     pass
 
 
 @auto_register
 class TimeSeriesPlot(QFrame, PipelineModelItem, metaclass=MetaTimeSeriesPlot):
     time_range_changed = Signal(TimeRange)
-    _time_range: TimeRange = TimeRange(0., 0.)
 
     def __init__(self, parent=None):
         QFrame.__init__(self, parent=parent)
         self.setObjectName(make_simple_incr_name(base="Plot"))
         self._plot = SciQLopPlot(self)
         self.setLayout(QVBoxLayout())
         self.layout().addWidget(self._plot)
@@ -170,15 +172,16 @@
 
     @property
     def time_range(self) -> TimeRange:
         return TimeRange.from_qcprange(self.xAxis.range())
 
     @time_range.setter
     def time_range(self, time_range: TimeRange):
-        if self._time_range != time_range:
+        if TimeRange.from_qcprange(self.xAxis.range()) != time_range:
+            log.debug(f"setting xAxis range: {time_range}")
             self.xAxis.setRange(time_range.start, time_range.stop)
             self.replot(QCustomPlot.rpQueuedReplot)
 
     def plot(self, product: Product or str):
         if type(product) is str:
             product = products.product(product)
         if product:
```

### Comparing `SciQLop-0.2.1/SciQLop/widgets/plots/time_span.py` & `sciqlop-0.3.0/SciQLop/widgets/plots/time_span.py`

 * *Files identical despite different names*

### Comparing `SciQLop-0.2.1/SciQLop/widgets/plots/time_span_controller.py` & `sciqlop-0.3.0/SciQLop/widgets/plots/time_span_controller.py`

 * *Files identical despite different names*

### Comparing `SciQLop-0.2.1/SciQLop/widgets/plots/time_sync_panel.py` & `sciqlop-0.3.0/SciQLop/widgets/plots/time_sync_panel.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
     def time_range(self) -> TimeRange:
         return self._time_range
 
     @time_range.setter
     def time_range(self, time_range: TimeRange):
         if self._time_range != time_range:
             self._time_range = time_range
-            for p in self._plot_container.plots:
+            for p in self.plots:
                 p.time_range = time_range
             self.time_range_changed.emit(time_range)
 
     @property
     def name(self):
         return self.objectName()
 
@@ -172,15 +172,15 @@
     def select(self):
         self.setStyleSheet("border: 3px dashed blue")
 
     def unselect(self):
         self.setStyleSheet("")
 
     def __del__(self):
-        print("lkdslkdf")
+        log.debug("deleting TimeSyncPanel")
 
     def __eq__(self, other: 'PipelineModelItem') -> bool:
         return self is other
 
     @property
     def icon(self) -> str:
         return ""
```

### Comparing `SciQLop-0.2.1/SciQLop/widgets/products_tree/products_tree.py` & `sciqlop-0.3.0/SciQLop/widgets/products_tree/products_tree.py`

 * *Files identical despite different names*

### Comparing `SciQLop-0.2.1/pyproject.toml` & `sciqlop-0.3.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "flit_core.buildapi"
 requires = ["flit_core"]
 
 [project]
 name = 'SciQLop'
-version = "0.2.1"
+version = "0.3.0"
 description = "An ergonomic and efficient application to browse and label in situ plasma measurements from multi-mission satellite data."
 keywords = ["machine-learning", "satellite", "plasma-physics", "nasa-data", "amda", "cdpp"]
 authors = [
     { name = "Alexis Jeandet", email = "alexis.jeandet@member.fsf.org" }
 ]
 
 maintainers = [
@@ -25,15 +25,15 @@
     "Natural Language :: English",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
-dependencies = ['numpy', 'SciQLopPlots>=0.3.2', 'speasy', 'qtconsole', 'tscat_gui>=0.2.0', 'seaborn', "scipy", "PySide6-QtAds==4.0.1.2"]
+dependencies = ['numpy', 'SciQLopPlots>=0.3.2', 'speasy', 'qtconsole==5.4.1', 'tscat_gui>=0.2.0', 'seaborn', "scipy", "PySide6-QtAds==4.0.1.2"]
 [project.urls]
 homepage = "https://github.com/SciQLop/SciQLop"
 
 [project.gui-scripts]
 sciqlop = "SciQLop.app:main"
 
 [tool.pytest.ini_options]
```

