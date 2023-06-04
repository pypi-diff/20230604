# Comparing `tmp/previewer-0.5.0.tar.gz` & `tmp/previewer-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "previewer-0.5.0.tar", max compression
+gzip compressed data, was "previewer-0.5.1.tar", max compression
```

## Comparing `previewer-0.5.0.tar` & `previewer-0.5.1.tar`

### file list

```diff
@@ -1,23 +1,22 @@
--rw-r--r--   0        0        0    11357 2022-10-11 22:19:16.835916 previewer-0.5.0/LICENSE
--rw-r--r--   0        0        0     6294 2022-10-11 22:19:16.835916 previewer-0.5.0/README.md
--rw-r--r--   0        0        0       97 2022-10-11 22:19:16.855916 previewer-0.5.0/previewer/__init__.py
--rw-r--r--   0        0        0     2975 2022-10-11 22:19:16.855916 previewer-0.5.0/previewer/cli.py
--rw-r--r--   0        0        0      273 2022-10-11 22:19:16.855916 previewer-0.5.0/previewer/commands/__init__.py
--rw-r--r--   0        0        0     7278 2022-10-11 22:19:16.855916 previewer-0.5.0/previewer/commands/montage.py
--rw-r--r--   0        0        0     2768 2022-10-11 22:19:16.859916 previewer-0.5.0/previewer/commands/resize.py
--rw-r--r--   0        0        0     7379 2022-10-11 22:19:16.859916 previewer-0.5.0/previewer/commands/sequence.py
--rw-r--r--   0        0        0     3829 2022-10-11 22:19:16.859916 previewer-0.5.0/previewer/commands/video_thumbnailer.py
--rw-r--r--   0        0        0     1871 2022-10-11 22:19:16.859916 previewer-0.5.0/previewer/external.py
--rw-r--r--   0        0        0      210 2022-10-11 22:19:16.859916 previewer-0.5.0/previewer/logger.py
--rw-r--r--   0        0        0     1983 2022-10-11 22:19:16.859916 previewer-0.5.0/previewer/resolution.py
--rw-r--r--   0        0        0        0 2022-10-11 22:19:16.859916 previewer-0.5.0/previewer/tools/__init__.py
--rw-r--r--   0        0        0      710 2022-10-11 22:19:16.859916 previewer-0.5.0/previewer/tools/blur.py
--rw-r--r--   0        0        0     2007 2022-10-11 22:19:16.859916 previewer-0.5.0/previewer/tools/montage.py
--rw-r--r--   0        0        0     3409 2022-10-11 22:19:16.859916 previewer-0.5.0/previewer/tools/resize.py
--rw-r--r--   0        0        0     1300 2022-10-11 22:19:16.859916 previewer-0.5.0/previewer/tools/sequence.py
--rw-r--r--   0        0        0     4380 2022-10-11 22:19:16.859916 previewer-0.5.0/previewer/utils.py
--rw-r--r--   0        0        0     3644 2022-10-11 22:19:16.859916 previewer-0.5.0/previewer/video.py
--rw-r--r--   0        0        0      382 2022-10-11 22:19:16.859916 previewer-0.5.0/previewer/wand.py
--rw-r--r--   0        0        0      769 2022-10-11 22:19:16.859916 previewer-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     7285 1970-01-01 00:00:00.000000 previewer-0.5.0/setup.py
--rw-r--r--   0        0        0     7044 1970-01-01 00:00:00.000000 previewer-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-04 15:45:23.114813 previewer-0.5.1/LICENSE
+-rw-r--r--   0        0        0     6281 2023-06-04 15:45:23.114813 previewer-0.5.1/README.md
+-rw-r--r--   0        0        0      187 2023-06-04 15:45:23.134813 previewer-0.5.1/previewer/__init__.py
+-rw-r--r--   0        0        0     2176 2023-06-04 15:45:23.134813 previewer-0.5.1/previewer/cli.py
+-rw-r--r--   0        0        0      240 2023-06-04 15:45:23.134813 previewer-0.5.1/previewer/commands/__init__.py
+-rw-r--r--   0        0        0     3268 2023-06-04 15:45:23.134813 previewer-0.5.1/previewer/commands/frames.py
+-rw-r--r--   0        0        0     6618 2023-06-04 15:45:23.134813 previewer-0.5.1/previewer/commands/montage.py
+-rw-r--r--   0        0        0     2223 2023-06-04 15:45:23.134813 previewer-0.5.1/previewer/commands/resize.py
+-rw-r--r--   0        0        0     7135 2023-06-04 15:45:23.134813 previewer-0.5.1/previewer/commands/sequence.py
+-rw-r--r--   0        0        0     3250 2023-06-04 15:45:23.134813 previewer-0.5.1/previewer/commands/utils.py
+-rw-r--r--   0        0        0     1871 2023-06-04 15:45:23.134813 previewer-0.5.1/previewer/external.py
+-rw-r--r--   0        0        0      210 2023-06-04 15:45:23.134813 previewer-0.5.1/previewer/logger.py
+-rw-r--r--   0        0        0     1983 2023-06-04 15:45:23.134813 previewer-0.5.1/previewer/resolution.py
+-rw-r--r--   0        0        0        0 2023-06-04 15:45:23.134813 previewer-0.5.1/previewer/tools/__init__.py
+-rw-r--r--   0        0        0      705 2023-06-04 15:45:23.134813 previewer-0.5.1/previewer/tools/blur.py
+-rw-r--r--   0        0        0     2007 2023-06-04 15:45:23.134813 previewer-0.5.1/previewer/tools/montage.py
+-rw-r--r--   0        0        0     3845 2023-06-04 15:45:23.134813 previewer-0.5.1/previewer/tools/resizer.py
+-rw-r--r--   0        0        0     1259 2023-06-04 15:45:23.134813 previewer-0.5.1/previewer/tools/sequence.py
+-rw-r--r--   0        0        0     3404 2023-06-04 15:45:23.134813 previewer-0.5.1/previewer/utils.py
+-rw-r--r--   0        0        0     3644 2023-06-04 15:45:23.134813 previewer-0.5.1/previewer/video.py
+-rw-r--r--   0        0        0      769 2023-06-04 15:45:23.134813 previewer-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     7031 1970-01-01 00:00:00.000000 previewer-0.5.1/PKG-INFO
```

### Comparing `previewer-0.5.0/LICENSE` & `previewer-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `previewer-0.5.0/README.md` & `previewer-0.5.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 - show or hide image filenames
 - adjust the space between thumbnails
 - add a border, a shadow to thumbnails
 
 Example:
 
 ```sh
-$ previewer montage --size 120x120 --crop --fill --background SlateGray1 "Rick Astley - Never Gonna Give You Up (Official Music Video).mp4"
+$ previewer montage --size 120x120 --crop --background SlateGray1 "Rick Astley - Never Gonna Give You Up (Official Music Video).mp4"
 🎬 Generate montage from video ./Rick Astley - Never Gonna Give You Up (Official Music Video).mp4 using 36 thumbnails
 🍺 Montage generated ./Rick Astley - Never Gonna Give You Up (Official Music Video).jpg
 ```
 
 ![Example of montage](images/montage.jpg)
 
 # Sequence
@@ -71,23 +71,23 @@
 - adjust _fps_ (frames per seconds), _delay_ between 2 frames ...
 - when extrating frames from a video, you can either use a fixed number of frames to extract or compute it given a given _speed_
 - change geometry (width, height, crop, fit or fill) of the frames
 
 Example:
 
 ```sh
-$ previewer gif --size 320x240 --crop --fill -n 20 "Rick Astley - Never Gonna Give You Up (Official Music Video).mp4"
+$ previewer gif --size 320x240 --crop -n 20 "Rick Astley - Never Gonna Give You Up (Official Music Video).mp4"
 🎬 Generate gif from video ./Rick Astley - Never Gonna Give You Up (Official Music Video).mp4 using 20 thumbnails
 🍺 Sequence generated ./Rick Astley - Never Gonna Give You Up (Official Music Video).gif
 ```
 
 ![Example of sequence](images/sequence.gif)
 
 ```sh
-$ previewer gif --start 3 --end 4 --fps 10 --aba --size 320x240 --crop --fill "Rick Astley - Never Gonna Give You Up (Official Music Video).mp4"
+$ previewer gif --start 3:21 --duration 1 --fps 10 --aba --size 320x240 --crop "Rick Astley - Never Gonna Give You Up (Official Music Video).mp4"
 🎬 Generate gif from video ./Rick Astley - Never Gonna Give You Up (Official Music Video).mp4 using 10 thumbnails
 🍺 Sequence generated ./Rick Astley - Never Gonna Give You Up (Official Music Video).gif
 ```
 
 ![Example of sequence with A-B-A loop](images/sequence-aba.gif)
 
 # Thumbnailer
```

### Comparing `previewer-0.5.0/previewer/commands/montage.py` & `previewer-0.5.1/previewer/commands/montage.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,22 +6,17 @@
 from argparse import ONE_OR_MORE, ArgumentParser, BooleanOptionalAction, Namespace
 from datetime import timedelta
 from pathlib import Path
 from tempfile import TemporaryDirectory
 
 from ..resolution import Resolution
 from ..tools.montage import Montage
-from ..utils import (
-    auto_resize_image,
-    color_str,
-    is_video,
-    iter_images_in_folder,
-    parser_group,
-)
+from ..utils import color_str, is_video, iter_copy_tree, iter_images_in_folder
 from ..video import Position, get_video_duration, iter_video_frames
+from .utils import add_geometry_group, get_image_resizer, parser_group
 
 
 def configure(parser: ArgumentParser):
     parser.set_defaults(handler=run)
 
     ## Generated file
     with parser_group(parser, name="output file options") as group:
@@ -118,35 +113,17 @@
             "--offset",
             type=int,
             default=10,
             help="thumbnail offset (default is 10)",
         )
 
     ## Geometry
-    with parser_group(parser, name="image geometry") as group:
-        default_size = Resolution(256, 256)
-        group.add_argument(
-            "--size",
-            type=Resolution,
-            metavar="WIDTHxHEIGHT",
-            default=default_size,
-            help=f"thumbnail size (default: {default_size})",
-        )
-        group.add_argument(
-            "--crop",
-            action=BooleanOptionalAction,
-            default=False,
-            help="crop thumbnails",
-        )
-        group.add_argument(
-            "--fill",
-            action=BooleanOptionalAction,
-            default=True,
-            help="fill thumbnails",
-        )
+    add_geometry_group(
+        parser, resolution_required=False, resolution_default=Resolution(256, 256)
+    )
 
     parser.add_argument(
         "input_files",
         type=Path,
         nargs=ONE_OR_MORE,
         help="folders containing images or video files",
     )
@@ -185,54 +162,48 @@
             else:
                 print(f"🙈 {color_str(folder_or_video)} is not a folder nor a video")
 
 
 def run_folder(
     args: Namespace, montage: Montage, folder: Path, output_jpg: Path, tmp_folder: Path
 ):
+    resizer = get_image_resizer(args)
     count = len(list(iter_images_in_folder(folder, recursive=args.recursive)))
     assert count > 0, "Folder does not contain any image"
     print(
         f"📷 Generate montage from folder {color_str(folder)} containing {count} images"
     )
     montage.build(
-        (
-            auto_resize_image(
-                image,
-                tmp_folder / image.name,
-                resolution=args.size,
-                crop=args.crop,
-                fill=args.fill,
+        [
+            resizer.transform_file(source, dest)
+            for source, dest in iter_copy_tree(
+                folder, tmp_folder, recursive=args.recursive, mkdirs=True
             )
-            for image in iter_images_in_folder(folder, recursive=args.recursive)
-        ),
+        ],
         output_jpg,
         filenames=args.filenames,
         title=folder.name if args.title else None,
     )
     print(f"🍺 Montage generated {color_str(output_jpg)}")
 
 
 def run_video(
     args: Namespace, montage: Montage, video: Path, output_jpg: Path, tmp_folder: Path
 ):
+    resizer = get_image_resizer(args)
     count = args.count or (args.columns * args.columns)
     print(f"🎬 Generate montage from video {color_str(video)} using {count} thumbnails")
     duration = get_video_duration(video)
     start = args.start.get_seconds(duration)
     end = args.end.get_seconds(duration)
     montage.build(
-        (
-            auto_resize_image(
-                frame,
-                tmp_folder / f"{timedelta(seconds=position)}.jpg",
-                resolution=args.size,
-                crop=args.crop,
-                fill=args.fill,
+        [
+            resizer.transform_file(
+                frame, tmp_folder / f"{timedelta(seconds=position)}.jpg"
             )
             for frame, position in iter_video_frames(video, count, start=start, end=end)
-        ),
+        ],
         output_jpg,
         filenames=args.filenames,
         title=video.name if args.title else None,
     )
     print(f"🍺 Montage generated {color_str(output_jpg)}")
```

### Comparing `previewer-0.5.0/previewer/commands/resize.py` & `previewer-0.5.1/previewer/commands/resize.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """
 command line interface
 """
 
-from argparse import ONE_OR_MORE, ArgumentParser, BooleanOptionalAction, Namespace
+from argparse import ONE_OR_MORE, ArgumentParser, Namespace
 from pathlib import Path
 
 from wand.image import Image
 
-from ..resolution import Resolution
-from ..utils import auto_resize_img, check_image, color_str, parser_group, save_img
+from ..utils import check_image, color_str, save_img
+from .utils import add_geometry_group, get_image_resizer, parser_group
 
 
 def configure(parser: ArgumentParser):
     parser.set_defaults(handler=run)
 
     ## Generated file
     with parser_group(parser, name="output file options") as group:
@@ -31,51 +31,33 @@
         group.add_argument(
             "-S",
             "--suffix",
             help="generated filename suffix",
         )
 
     ## Geometry
-    with parser_group(parser, name="image geometry") as group:
-        group.add_argument(
-            "--size",
-            type=Resolution,
-            metavar="WIDTHxHEIGHT",
-            required=True,
-            help="thumbnail size",
-        )
-        group.add_argument(
-            "--crop",
-            action=BooleanOptionalAction,
-            default=False,
-            help="crop thumbnails",
-        )
-        group.add_argument(
-            "--fill",
-            action=BooleanOptionalAction,
-            default=False,
-            help="fill thumbnails",
-        )
+    add_geometry_group(parser, resolution_required=True)
 
     parser.add_argument(
         "images",
         nargs=ONE_OR_MORE,
         type=Path,
         help="images to resize",
     )
 
 
 def run(args: Namespace):
+    resizer = get_image_resizer(args)
     for source_image in args.images:
         output_folder = args.output or source_image.parent
         print(
             f"{'Crop' if args.crop else 'Resize'} {color_str(source_image)} to {'fill' if args.fill else 'fit'} {args.size}"
         )
         with Image(filename=check_image(source_image)) as img:
-            img = auto_resize_img(img, args.size, crop=args.crop, fill=args.fill)
+            img = resizer.transform(img)
             suffix = (
                 args.suffix
                 if args.suffix is not None
                 else f" ({'crop' if args.crop else 'resize'}:{img.width}x{img.height})"
             )
             destination_image = (
                 output_folder
```

### Comparing `previewer-0.5.0/previewer/commands/sequence.py` & `previewer-0.5.1/previewer/commands/sequence.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """
 command line interface
 """
-from argparse import ONE_OR_MORE, ArgumentParser, BooleanOptionalAction, Namespace
+from argparse import ONE_OR_MORE, ArgumentParser, Namespace
 from datetime import timedelta
 from operator import itemgetter
 from pathlib import Path
 
 from ..logger import DEBUG
-from ..resolution import Resolution
-from ..tools.sequence import create_gif
-from ..utils import color_str, is_video, iter_images_in_folder, iter_img, parser_group
+from ..tools.resizer import ImageResizer
+from ..tools.sequence import create_sequence
+from ..utils import color_str, is_video, iter_images_in_folder, iter_img
 from ..video import Position, get_video_duration, iter_video_frames
-from ..wand import auto_resize_img
+from .utils import add_geometry_group, get_image_resizer, parser_group
 
 
 def configure(parser: ArgumentParser):
     parser.set_defaults(handler=run)
 
     ## Generated file
     with parser_group(parser, name="output file options") as group:
@@ -41,52 +41,39 @@
             dest="extension",
             choices=["gif", "webm", "webp", "mp4"],
             default="gif",
             help="generated file format, default is gif",
         )
 
     ## Geometry
-    with parser_group(parser, name="image geometry") as group:
-        default_size = Resolution(640, 480)
-        group.add_argument(
-            "--size",
-            type=Resolution,
-            metavar="WIDTHxHEIGHT",
-            default=default_size,
-            help=f"thumbnail size (default: {default_size})",
-        )
-        group.add_argument(
-            "--crop",
-            action=BooleanOptionalAction,
-            default=True,
-            help="crop thumbnails",
-        )
-        group.add_argument(
-            "--fill",
-            action=BooleanOptionalAction,
-            default=False,
-            help="fill thumbnails",
-        )
+    add_geometry_group(parser, resolution_required=False, crop_default=True)
 
     ## Video only
     with parser_group(parser, name="only for videos") as group:
         group.add_argument(
             "--start",
             type=Position,
             metavar="POSITION",
             default="5%",
             help="start position (default: 5%%)",
         )
-        group.add_argument(
-            "--end",
-            type=Position,
-            metavar="POSITION",
-            default="-5%",
-            help="end position (default: -5%%)",
-        )
+        with parser_group(parser, exclusive=True) as xgroup:
+            xgroup.add_argument(
+                "--end",
+                type=Position,
+                metavar="POSITION",
+                default="-5%",
+                help="end position (default: -5%%)",
+            )
+            xgroup.add_argument(
+                "--duration",
+                type=Position,
+                metavar="DURATION",
+                help="calculate --end given the length",
+            )
         with parser_group(parser, exclusive=True) as xgroup:
             xgroup.add_argument(
                 "-n",
                 "--count",
                 type=int,
                 help="number of frames to extract (default calculated given --delay/--fps)",
             )
@@ -146,65 +133,66 @@
         type=Path,
         nargs=ONE_OR_MORE,
         help="folders containing images or video files",
     )
 
 
 def run(args: Namespace):
+    resizer = get_image_resizer(args)
     for folder_or_video in args.input_files:
         output_file = (
             (args.output or Path())
             / f"{args.prefix or ''}{folder_or_video.name if folder_or_video.is_dir() else folder_or_video.stem}{args.suffix or ''}.{args.extension}"
         )
         if output_file.exists():
             print(
                 f"💡 Sequence {color_str(output_file)} already generated from {color_str(folder_or_video)}"
             )
             continue
 
         if folder_or_video.is_dir():
-            run_folder(args, folder_or_video, output_file)
+            run_folder(args, folder_or_video, output_file, resizer)
         elif is_video(folder_or_video):
-            run_video(args, folder_or_video, output_file)
+            run_video(args, folder_or_video, output_file, resizer)
         else:
             print(f"🙈 {color_str(folder_or_video)} is not a folder nor a video")
 
 
-def run_folder(args: Namespace, folder: Path, output_file: Path):
+def run_folder(args: Namespace, folder: Path, output_file: Path, resizer: ImageResizer):
     count = len(list(iter_images_in_folder(folder, recursive=args.recursive)))
     assert count > 0, "Folder does not contain any image"
 
     print(
         f"📷 Generate {args.extension} from folder {color_str(folder)} containing {count} images"
     )
-    create_gif(
-        (
-            auto_resize_img(
-                img,
-                resolution=args.size,
-                crop=args.crop,
-                fill=args.fill,
-            )
-            for img in iter_img(
+    create_sequence(
+        map(
+            resizer.transform,
+            iter_img(
                 iter_images_in_folder(
                     folder, recursive=args.recursive, shuffle=args.shuffle
                 )
-            )
+            ),
         ),
         output_file,
         delay=int(100 / args.fps if args.fps else args.delay / 10),
         aba_loop=args.aba,
+        gif_optimize=args.extension == "gif",
     )
     print(f"🍺 Sequence generated {color_str(output_file)}")
 
 
-def run_video(args: Namespace, video: Path, output_file: Path):
+def run_video(args: Namespace, video: Path, output_file: Path, resizer: ImageResizer):
     duration = get_video_duration(video)
     start = args.start.get_seconds(duration)
-    end = args.end.get_seconds(duration)
+    end = end = (
+        start + args.duration.get_seconds(duration)
+        if args.duration is not None
+        else args.end.get_seconds(duration)
+    )
     count = args.count or int(
         (end - start) * args.fps if args.fps else (end - start) * (1000 / args.delay)
     )
     if args.speed is not None:
         count = int(count / args.speed)
     DEBUG(
         "Video duration is %s, extract %d frames from %.3lf -> %.3lf, gif duration will be %s",
@@ -214,26 +202,22 @@
         end,
         timedelta(milliseconds=count * args.delay * 10),
     )
 
     print(
         f"🎬 Generate {args.extension} from video {color_str(video)} using {count} thumbnails"
     )
-    create_gif(
-        (
-            auto_resize_img(
-                img,
-                resolution=args.size,
-                crop=args.crop,
-                fill=args.fill,
-            )
-            for img in iter_img(
+    create_sequence(
+        map(
+            resizer.transform,
+            iter_img(
                 map(
                     itemgetter(0), iter_video_frames(video, count, start=start, end=end)
                 )
-            )
+            ),
         ),
         output_file,
         delay=int(100 / args.fps if args.fps else args.delay / 10),
         aba_loop=args.aba,
+        gif_optimize=args.extension == "gif",
     )
     print(f"🍺 Sequence generated {color_str(output_file)}")
```

### Comparing `previewer-0.5.0/previewer/commands/video_thumbnailer.py` & `previewer-0.5.1/previewer/commands/frames.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,15 @@
-from argparse import ONE_OR_MORE, ArgumentParser, BooleanOptionalAction, Namespace
+from argparse import ONE_OR_MORE, ArgumentParser, Namespace
 from datetime import timedelta
 from pathlib import Path
 
 from ..resolution import Resolution
-from ..utils import (
-    auto_resize_image,
-    check_empty_folder,
-    check_video,
-    color_str,
-    parser_group,
-)
+from ..utils import check_empty_folder, check_video, color_str
 from ..video import Position, get_video_duration, iter_video_frames
+from .utils import add_geometry_group, get_image_resizer, parser_group
 
 
 def configure(parser: ArgumentParser):
     parser.set_defaults(handler=run)
 
     ## Generated file
     with parser_group(parser, name="output file options") as group:
@@ -33,33 +28,15 @@
         group.add_argument(
             "-S",
             "--suffix",
             help="generated filename prefix (default frame time)",
         )
 
     ## Geometry
-    with parser_group(parser, name="image geometry") as group:
-        group.add_argument(
-            "--size",
-            type=Resolution,
-            metavar="WIDTHxHEIGHT",
-            help="thumbnail size",
-        )
-        group.add_argument(
-            "--crop",
-            action=BooleanOptionalAction,
-            default=False,
-            help="crop thumbnails",
-        )
-        group.add_argument(
-            "--fill",
-            action=BooleanOptionalAction,
-            default=False,
-            help="fill thumbnails",
-        )
+    add_geometry_group(parser)
 
     with parser_group(parser, exclusive=True) as xgroup:
         xgroup.add_argument(
             "--fps",
             type=int,
             metavar="INT",
             help="frames per second",
@@ -92,14 +69,16 @@
         nargs=ONE_OR_MORE,
         type=Path,
         help="video files",
     )
 
 
 def run(args: Namespace):
+
+    resizer = get_image_resizer(args)
     for video in args.videos:
         video = check_video(video)
         folder = (
             check_empty_folder(args.output)
             if args.output is not None
             else check_empty_folder(Path(video.stem))
         )
@@ -114,16 +93,14 @@
             position = str(timedelta(seconds=int(seconds)))
             filename = (
                 (f"{video.stem} " if args.prefix is None else args.prefix)
                 + f"{frame.stem}"
                 + (args.suffix if args.suffix is not None else f" ({position})")
             )
             destination = folder / f"{filename}{frame.suffix}"
-            auto_resize_image(
-                frame, destination, args.size, crop=args.crop, fill=args.fill
-            )
+            resizer.transform_file(frame, destination)
             index += 1
             print(
                 f"[{index}/{count}] {color_str(destination)} ({Resolution.from_image(destination)}) at position {position}"
             )
 
         print(f"🍺 {index} thumbnails extracted in {color_str(folder)}")
```

### Comparing `previewer-0.5.0/previewer/external.py` & `previewer-0.5.1/previewer/external.py`

 * *Files identical despite different names*

### Comparing `previewer-0.5.0/previewer/resolution.py` & `previewer-0.5.1/previewer/resolution.py`

 * *Files identical despite different names*

### Comparing `previewer-0.5.0/previewer/tools/blur.py` & `previewer-0.5.1/previewer/tools/blur.py`

 * *Files 19% similar despite different names*

```diff
@@ -23,11 +23,11 @@
         """
         if self.blur_sigma > 0:
             image.gaussian_blur(sigma=self.blur_sigma)
         image.level(black=self.black, white=self.white, gamma=self.gamma)
         return image
 
     def __str__(self):
-        return f"blur:{self.blur_sigma}:{self.black}:{self.white}:{self.gamma}"
+        return f"{self.blur_sigma}:{self.black}:{self.white}:{self.gamma}"
 
 
 DEFAULT_BLUR = BlurGenerator(30, 0, 1, 0.7)
```

### Comparing `previewer-0.5.0/previewer/tools/montage.py` & `previewer-0.5.1/previewer/tools/montage.py`

 * *Files identical despite different names*

### Comparing `previewer-0.5.0/previewer/tools/resize.py` & `previewer-0.5.1/previewer/tools/resizer.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 """
 Wand related manipulation functions
 """
+import shutil
 import time
 from dataclasses import dataclass
+from pathlib import Path
 
 from wand.image import GRAVITY_TYPES, Image
 
 from ..logger import DEBUG
 from ..resolution import Resolution
+from ..utils import save_img
 from .blur import DEFAULT_BLUR, BlurGenerator
 
 
 @dataclass
 class ImageResizer:
     """
     Utility class to blur an image
@@ -25,14 +28,23 @@
     crop_blur: BlurGenerator = DEFAULT_BLUR
 
     def __post_init__(self):
         assert (
             self.crop_gravity in GRAVITY_TYPES
         ), f"Invalid gravity {self.crop_gravity}, must be {GRAVITY_TYPES}"
 
+    def transform_file(self, source: Path, dest: Path) -> Path:
+        if self.resolution is None or Resolution.from_image(source) == self.resolution:
+            # fallback copy, image
+            return shutil.copy2(source, dest)
+        else:
+            with Image(filename=source) as img:
+                save_img(self.transform(img), dest)
+        return dest
+
     def transform(self, image: Image) -> Image:
         """
         Resize the given image
         """
         start = time.time()
         orig_size = Resolution.from_img(image)
         if self.resolution is None:
```

### Comparing `previewer-0.5.0/previewer/tools/sequence.py` & `previewer-0.5.1/previewer/tools/sequence.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 from typing import Iterable, Optional
 
 from wand.image import Image
 
 from ..logger import DEBUG
 
 
-def create_gif(
+def create_sequence(
     frames: Iterable[Image],
     output_file: Path,
     delay: int = 50,
-    optimize: bool = True,
+    gif_optimize: bool = True,
     aba_loop: Optional[str] = None,
 ):
     """
     Create a gif with the given images
     """
     with Image() as gif:
         queue = []
@@ -30,15 +30,15 @@
                 queue.pop(0).destroy()
                 queue.pop(-1).destroy()
             for frame in queue:
                 gif.sequence.append(frame)
                 # ba frames are reated
                 frame.destroy()
 
-        # TODO: try to use optimize_transparency/optimize_layers/coalesce for optimizations
+        # Gif only optimisation
+        if gif_optimize:
+            gif.optimize_transparency()
 
         DEBUG("set gif delay to %d", delay)
         for frame in gif.sequence:
             frame.delay = delay
-        if optimize:
-            gif.type = "optimize"
         gif.save(filename=output_file)
```

### Comparing `previewer-0.5.0/previewer/utils.py` & `previewer-0.5.1/previewer/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,17 @@
 import random
-import shutil
 import sys
-from argparse import _ActionsContainer
 from collections.abc import Iterable
-from contextlib import contextmanager
 from pathlib import Path
-from typing import Any, Generator, Iterator, Tuple
+from typing import Any, Iterator, Tuple
 
 import magic
 from colorama import Fore, Style
-
 from wand.image import Image
 
-from .resolution import Resolution
-from .wand import auto_resize_img
-
 
 def get_mime(file: Path) -> str:
     """
     Return the mime of a file
     """
     if not file.exists():
         raise FileNotFoundError(f"Cannot find file: {file}")
@@ -89,34 +82,14 @@
         if item.is_dir():
             if recursive:
                 yield from iter_images_in_folder(item, recursive=True)
         elif is_image(item):
             yield item
 
 
-def auto_resize_image(
-    source: Path,
-    destination: Path,
-    resolution: Resolution,
-    crop: bool,
-    fill: bool,
-) -> Path:
-    """
-    resize the given image
-    """
-    if resolution is not None:
-        with Image(filename=source) as img:
-            if resolution.size != img.size:
-                return save_img(
-                    auto_resize_img(img, resolution, crop=crop, fill=fill), destination
-                )
-    # fallback copy, image
-    return shutil.copy2(source, destination)
-
-
 def iter_img(images: Iterable[Path], auto_orient: bool = True) -> Iterator[Image]:
     for image in images:
         with Image(filename=image) as img:
             if auto_orient:
                 img.auto_orient()
             yield img
 
@@ -146,17 +119,7 @@
     iterator to copy folder recursively
     """
     for source_file in iter_images_in_folder(source_folder, recursive=recursive):
         destination_file = destination_folder / source_file.relative_to(source_folder)
         if mkdirs:
             destination_file.parent.mkdir(parents=True, exist_ok=True)
         yield source_file, destination_file
-
-
-@contextmanager
-def parser_group(
-    parser: _ActionsContainer, name: str = "options group", exclusive: bool = False
-) -> Generator[_ActionsContainer, None, None]:
-    if exclusive:
-        yield parser.add_mutually_exclusive_group()
-    else:
-        yield parser.add_argument_group(name)
```

### Comparing `previewer-0.5.0/previewer/video.py` & `previewer-0.5.1/previewer/video.py`

 * *Files identical despite different names*

### Comparing `previewer-0.5.0/pyproject.toml` & `previewer-0.5.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "previewer"
-version = "0.5.0"
+version = "0.5.1"
 description = "Video or Folder preview generator"
 homepage = "https://github.com/essembeh/previewer"
 authors = ["Sébastien MB <seb@essembeh.org>"]
 license = "Apache-2.0"
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: Apache Software License",
```

### Comparing `previewer-0.5.0/setup.py` & `previewer-0.5.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,154 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: previewer
+Version: 0.5.1
+Summary: Video or Folder preview generator
+Home-page: https://github.com/essembeh/previewer
+License: Apache-2.0
+Author: Sébastien MB
+Author-email: seb@essembeh.org
+Requires-Python: >=3.9,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Utilities
+Requires-Dist: Wand (>=0.6.10,<0.7.0)
+Requires-Dist: colorama (>=0.4.5,<0.5.0)
+Requires-Dist: python-magic (>=0.4.27,<0.5.0)
+Description-Content-Type: text/markdown
+
+![Github](https://img.shields.io/github/tag/essembeh/previewer.svg)
+![PyPi](https://img.shields.io/pypi/v/previewer.svg)
+![Python](https://img.shields.io/pypi/pyversions/previewer.svg)
+![CI](https://github.com/essembeh/previewer/actions/workflows/poetry.yml/badge.svg)
+
+# Previewer
+
+Command line tool to generate montages/sequences from video clips or folders containing images.
+
+_previewer_ is a collection of tools:
+
+- `previewer montage`: to generate a single image with thumbnails (a _montage_) from a folder containing images or a video
+- `previewer gif`: to generate a Gif (or mp4/webp/webm) with thumbnails from a folder containing images or a video
+- `previewer video-thumbnailer`: to extract a given number of thumbnails from a video clip
+- `previewer resize`: to change geometry (resize, crop, fit, fill) of images
+
+# Install
+
+Install dependencies
+
+```sh
+$ sudo apt update
+$ sudo apt install imagemagick ffmpeg
+```
+
+Install the latest release of _previewer_ from [PyPI](https://pypi.org/project/previewer/)
+
+```sh
+$ pip3 install previewer
+$ previewer-montage --help
+```
+
+Or install _previewer_ from the sources
+
+```sh
+$ pip3 install poetry
+$ pip3 install git+https://github.com/essembeh/previewer
+$ previewer --help
+```
+
+# Montage
+
+`previewer montage` can create _preview_ image from a folder containing images or a video.
+
+You can customize the generated image:
+
+- change the background color
+- change geometry (width, height, crop, fit or fill) of the thumbnails
+- show or hide the a title
+- show or hide image filenames
+- adjust the space between thumbnails
+- add a border, a shadow to thumbnails
+
+Example:
+
+```sh
+$ previewer montage --size 120x120 --crop --background SlateGray1 "Rick Astley - Never Gonna Give You Up (Official Music Video).mp4"
+🎬 Generate montage from video ./Rick Astley - Never Gonna Give You Up (Official Music Video).mp4 using 36 thumbnails
+🍺 Montage generated ./Rick Astley - Never Gonna Give You Up (Official Music Video).jpg
+```
+
+![Example of montage](images/montage.jpg)
+
+# Sequence
+
+`previewer gif` can generate sequences with images in a folder or extracted from a video.
+
+You can customize the sequence:
+
+- choose the format between _gif_, _mp4_, _webp_ or _webm_
+- adjust _fps_ (frames per seconds), _delay_ between 2 frames ...
+- when extrating frames from a video, you can either use a fixed number of frames to extract or compute it given a given _speed_
+- change geometry (width, height, crop, fit or fill) of the frames
+
+Example:
+
+```sh
+$ previewer gif --size 320x240 --crop -n 20 "Rick Astley - Never Gonna Give You Up (Official Music Video).mp4"
+🎬 Generate gif from video ./Rick Astley - Never Gonna Give You Up (Official Music Video).mp4 using 20 thumbnails
+🍺 Sequence generated ./Rick Astley - Never Gonna Give You Up (Official Music Video).gif
+```
+
+![Example of sequence](images/sequence.gif)
+
+```sh
+$ previewer gif --start 3:21 --duration 1 --fps 10 --aba --size 320x240 --crop "Rick Astley - Never Gonna Give You Up (Official Music Video).mp4"
+🎬 Generate gif from video ./Rick Astley - Never Gonna Give You Up (Official Music Video).mp4 using 10 thumbnails
+🍺 Sequence generated ./Rick Astley - Never Gonna Give You Up (Official Music Video).gif
+```
+
+![Example of sequence with A-B-A loop](images/sequence-aba.gif)
+
+# Thumbnailer
+
+`previewer video-thumbnailer` can extract and resize/crop frames from a video
+
+You can also:
+
+- choose the frame count to extract
+- select a start position and/or a end position in the video
+- change geometry (width, height, crop, fit or fill) of the frames
+
+Example:
+
+```sh
+$ previewer video-thumbnailer -n 20 "Rick Astley - Never Gonna Give You Up (Official Music Video).mp4"
+Extract 20 thumbnails from ./Rick Astley - Never Gonna Give You Up (Official Music Video).mp4
+  Rick Astley - Never Gonna Give You Up (Official Music Video)/frame 01 (0:00:05).jpg (1920x1080) at position 0:00:05
+  Rick Astley - Never Gonna Give You Up (Official Music Video)/frame 02 (0:00:15).jpg (1920x1080) at position 0:00:15
+  Rick Astley - Never Gonna Give You Up (Official Music Video)/frame 03 (0:00:26).jpg (1920x1080) at position 0:00:26
+  Rick Astley - Never Gonna Give You Up (Official Music Video)/frame 04 (0:00:37).jpg (1920x1080) at position 0:00:37
+  Rick Astley - Never Gonna Give You Up (Official Music Video)/frame 05 (0:00:47).jpg (1920x1080) at position 0:00:47
+  Rick Astley - Never Gonna Give You Up (Official Music Video)/frame 06 (0:00:58).jpg (1920x1080) at position 0:00:58
+  Rick Astley - Never Gonna Give You Up (Official Music Video)/frame 07 (0:01:08).jpg (1920x1080) at position 0:01:08
+  Rick Astley - Never Gonna Give You Up (Official Music Video)/frame 08 (0:01:19).jpg (1920x1080) at position 0:01:19
+  Rick Astley - Never Gonna Give You Up (Official Music Video)/frame 09 (0:01:30).jpg (1920x1080) at position 0:01:30
+  Rick Astley - Never Gonna Give You Up (Official Music Video)/frame 10 (0:01:40).jpg (1920x1080) at position 0:01:40
+  Rick Astley - Never Gonna Give You Up (Official Music Video)/frame 11 (0:01:51).jpg (1920x1080) at position 0:01:51
+  Rick Astley - Never Gonna Give You Up (Official Music Video)/frame 12 (0:02:01).jpg (1920x1080) at position 0:02:01
+  Rick Astley - Never Gonna Give You Up (Official Music Video)/frame 13 (0:02:12).jpg (1920x1080) at position 0:02:12
+  Rick Astley - Never Gonna Give You Up (Official Music Video)/frame 14 (0:02:23).jpg (1920x1080) at position 0:02:23
+  Rick Astley - Never Gonna Give You Up (Official Music Video)/frame 15 (0:02:33).jpg (1920x1080) at position 0:02:33
+  Rick Astley - Never Gonna Give You Up (Official Music Video)/frame 16 (0:02:44).jpg (1920x1080) at position 0:02:44
+  Rick Astley - Never Gonna Give You Up (Official Music Video)/frame 17 (0:02:54).jpg (1920x1080) at position 0:02:54
+  Rick Astley - Never Gonna Give You Up (Official Music Video)/frame 18 (0:03:05).jpg (1920x1080) at position 0:03:05
+  Rick Astley - Never Gonna Give You Up (Official Music Video)/frame 19 (0:03:16).jpg (1920x1080) at position 0:03:16
+  Rick Astley - Never Gonna Give You Up (Official Music Video)/frame 20 (0:03:26).jpg (1920x1080) at position 0:03:26
+🍺 20 thumbnails extracted in Rick Astley - Never Gonna Give You Up (Official Music Video)/
 
-packages = \
-['previewer', 'previewer.commands', 'previewer.tools']
+```
 
-package_data = \
-{'': ['*']}
+![Example of thumbnailer](images/frames.png)
 
-install_requires = \
-['Wand>=0.6.10,<0.7.0', 'colorama>=0.4.5,<0.5.0', 'python-magic>=0.4.27,<0.5.0']
-
-entry_points = \
-{'console_scripts': ['previewer = previewer.cli:run']}
-
-setup_kwargs = {
-    'name': 'previewer',
-    'version': '0.5.0',
-    'description': 'Video or Folder preview generator',
-    'long_description': '![Github](https://img.shields.io/github/tag/essembeh/previewer.svg)\n![PyPi](https://img.shields.io/pypi/v/previewer.svg)\n![Python](https://img.shields.io/pypi/pyversions/previewer.svg)\n![CI](https://github.com/essembeh/previewer/actions/workflows/poetry.yml/badge.svg)\n\n# Previewer\n\nCommand line tool to generate montages/sequences from video clips or folders containing images.\n\n_previewer_ is a collection of tools:\n\n- `previewer montage`: to generate a single image with thumbnails (a _montage_) from a folder containing images or a video\n- `previewer gif`: to generate a Gif (or mp4/webp/webm) with thumbnails from a folder containing images or a video\n- `previewer video-thumbnailer`: to extract a given number of thumbnails from a video clip\n- `previewer resize`: to change geometry (resize, crop, fit, fill) of images\n\n# Install\n\nInstall dependencies\n\n```sh\n$ sudo apt update\n$ sudo apt install imagemagick ffmpeg\n```\n\nInstall the latest release of _previewer_ from [PyPI](https://pypi.org/project/previewer/)\n\n```sh\n$ pip3 install previewer\n$ previewer-montage --help\n```\n\nOr install _previewer_ from the sources\n\n```sh\n$ pip3 install poetry\n$ pip3 install git+https://github.com/essembeh/previewer\n$ previewer --help\n```\n\n# Montage\n\n`previewer montage` can create _preview_ image from a folder containing images or a video.\n\nYou can customize the generated image:\n\n- change the background color\n- change geometry (width, height, crop, fit or fill) of the thumbnails\n- show or hide the a title\n- show or hide image filenames\n- adjust the space between thumbnails\n- add a border, a shadow to thumbnails\n\nExample:\n\n```sh\n$ previewer montage --size 120x120 --crop --fill --background SlateGray1 "Rick Astley - Never Gonna Give You Up (Official Music Video).mp4"\n🎬 Generate montage from video ./Rick Astley - Never Gonna Give You Up (Official Music Video).mp4 using 36 thumbnails\n🍺 Montage generated ./Rick Astley - Never Gonna Give You Up (Official Music Video).jpg\n```\n\n![Example of montage](images/montage.jpg)\n\n# Sequence\n\n`previewer gif` can generate sequences with images in a folder or extracted from a video.\n\nYou can customize the sequence:\n\n- choose the format between _gif_, _mp4_, _webp_ or _webm_\n- adjust _fps_ (frames per seconds), _delay_ between 2 frames ...\n- when extrating frames from a video, you can either use a fixed number of frames to extract or compute it given a given _speed_\n- change geometry (width, height, crop, fit or fill) of the frames\n\nExample:\n\n```sh\n$ previewer gif --size 320x240 --crop --fill -n 20 "Rick Astley - Never Gonna Give You Up (Official Music Video).mp4"\n🎬 Generate gif from video ./Rick Astley - Never Gonna Give You Up (Official Music Video).mp4 using 20 thumbnails\n🍺 Sequence generated ./Rick Astley - Never Gonna Give You Up (Official Music Video).gif\n```\n\n![Example of sequence](images/sequence.gif)\n\n```sh\n$ previewer gif --start 3 --end 4 --fps 10 --aba --size 320x240 --crop --fill "Rick Astley - Never Gonna Give You Up (Official Music Video).mp4"\n🎬 Generate gif from video ./Rick Astley - Never Gonna Give You Up (Official Music Video).mp4 using 10 thumbnails\n🍺 Sequence generated ./Rick Astley - Never Gonna Give You Up (Official Music Video).gif\n```\n\n![Example of sequence with A-B-A loop](images/sequence-aba.gif)\n\n# Thumbnailer\n\n`previewer video-thumbnailer` can extract and resize/crop frames from a video\n\nYou can also:\n\n- choose the frame count to extract\n- select a start position and/or a end position in the video\n- change geometry (width, height, crop, fit or fill) of the frames\n\nExample:\n\n```sh\n$ previewer video-thumbnailer -n 20 "Rick Astley - Never Gonna Give You Up (Official Music Video).mp4"\nExtract 20 thumbnails from ./Rick Astley - Never Gonna Give You Up (Official Music Video).mp4\n  Rick Astley - Never Gonna Give You Up (Official Music Video)/frame 01 (0:00:05).jpg (1920x1080) at position 0:00:05\n  Rick Astley - Never Gonna Give You Up (Official Music Video)/frame 02 (0:00:15).jpg (1920x1080) at position 0:00:15\n  Rick Astley - Never Gonna Give You Up (Official Music Video)/frame 03 (0:00:26).jpg (1920x1080) at position 0:00:26\n  Rick Astley - Never Gonna Give You Up (Official Music Video)/frame 04 (0:00:37).jpg (1920x1080) at position 0:00:37\n  Rick Astley - Never Gonna Give You Up (Official Music Video)/frame 05 (0:00:47).jpg (1920x1080) at position 0:00:47\n  Rick Astley - Never Gonna Give You Up (Official Music Video)/frame 06 (0:00:58).jpg (1920x1080) at position 0:00:58\n  Rick Astley - Never Gonna Give You Up (Official Music Video)/frame 07 (0:01:08).jpg (1920x1080) at position 0:01:08\n  Rick Astley - Never Gonna Give You Up (Official Music Video)/frame 08 (0:01:19).jpg (1920x1080) at position 0:01:19\n  Rick Astley - Never Gonna Give You Up (Official Music Video)/frame 09 (0:01:30).jpg (1920x1080) at position 0:01:30\n  Rick Astley - Never Gonna Give You Up (Official Music Video)/frame 10 (0:01:40).jpg (1920x1080) at position 0:01:40\n  Rick Astley - Never Gonna Give You Up (Official Music Video)/frame 11 (0:01:51).jpg (1920x1080) at position 0:01:51\n  Rick Astley - Never Gonna Give You Up (Official Music Video)/frame 12 (0:02:01).jpg (1920x1080) at position 0:02:01\n  Rick Astley - Never Gonna Give You Up (Official Music Video)/frame 13 (0:02:12).jpg (1920x1080) at position 0:02:12\n  Rick Astley - Never Gonna Give You Up (Official Music Video)/frame 14 (0:02:23).jpg (1920x1080) at position 0:02:23\n  Rick Astley - Never Gonna Give You Up (Official Music Video)/frame 15 (0:02:33).jpg (1920x1080) at position 0:02:33\n  Rick Astley - Never Gonna Give You Up (Official Music Video)/frame 16 (0:02:44).jpg (1920x1080) at position 0:02:44\n  Rick Astley - Never Gonna Give You Up (Official Music Video)/frame 17 (0:02:54).jpg (1920x1080) at position 0:02:54\n  Rick Astley - Never Gonna Give You Up (Official Music Video)/frame 18 (0:03:05).jpg (1920x1080) at position 0:03:05\n  Rick Astley - Never Gonna Give You Up (Official Music Video)/frame 19 (0:03:16).jpg (1920x1080) at position 0:03:16\n  Rick Astley - Never Gonna Give You Up (Official Music Video)/frame 20 (0:03:26).jpg (1920x1080) at position 0:03:26\n🍺 20 thumbnails extracted in Rick Astley - Never Gonna Give You Up (Official Music Video)/\n\n```\n\n![Example of thumbnailer](images/frames.png)\n',
-    'author': 'Sébastien MB',
-    'author_email': 'seb@essembeh.org',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/essembeh/previewer',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.9,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

