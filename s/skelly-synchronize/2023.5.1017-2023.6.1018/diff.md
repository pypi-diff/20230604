# Comparing `tmp/skelly_synchronize-2023.5.1017.tar.gz` & `tmp/skelly_synchronize-2023.6.1018.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skelly_synchronize-2023.5.1017.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "skelly_synchronize-2023.6.1018.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `skelly_synchronize-2023.5.1017.tar` & `skelly_synchronize-2023.6.1018.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0       65 2023-05-24 17:56:05.918732 skelly_synchronize-2023.5.1017/.gitattributes
--rw-r--r--   0        0        0      146 2023-05-24 17:56:05.918732 skelly_synchronize-2023.5.1017/.github/workflows/lint-with-black.yml
--rw-r--r--   0        0        0     1087 2023-05-24 17:56:05.918732 skelly_synchronize-2023.5.1017/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml
--rw-r--r--   0        0        0     1025 2023-05-24 17:56:05.918732 skelly_synchronize-2023.5.1017/.github/workflows/python-testing.yml
--rw-r--r--   0        0        0     2783 2023-05-24 17:56:05.918732 skelly_synchronize-2023.5.1017/.gitignore
--rw-r--r--   0        0        0    34523 2023-05-24 17:56:05.918732 skelly_synchronize-2023.5.1017/LICENSE
--rw-r--r--   0        0        0     3030 2023-05-24 17:56:05.918732 skelly_synchronize-2023.5.1017/README.md
--rw-r--r--   0        0        0     1639 2023-05-24 17:56:05.918732 skelly_synchronize-2023.5.1017/pyproject.toml
--rw-r--r--   0        0        0      150 2023-05-24 17:56:05.918732 skelly_synchronize-2023.5.1017/requirements.txt
--rw-r--r--   0        0        0       50 2023-05-24 17:56:05.918732 skelly_synchronize-2023.5.1017/setup.py
--rw-r--r--   0        0        0     1056 2023-05-24 17:56:05.918732 skelly_synchronize-2023.5.1017/skelly_synchronize/__init__.py
--rw-r--r--   0        0        0      333 2023-05-24 17:56:05.918732 skelly_synchronize-2023.5.1017/skelly_synchronize/__main__.py
--rw-r--r--   0        0        0     2192 2023-05-24 17:56:05.918732 skelly_synchronize-2023.5.1017/skelly_synchronize/core_processes/audio_utilities.py
--rw-r--r--   0        0        0     2758 2023-05-24 17:56:05.918732 skelly_synchronize-2023.5.1017/skelly_synchronize/core_processes/correlation_functions.py
--rw-r--r--   0        0        0      616 2023-05-24 17:56:05.922732 skelly_synchronize-2023.5.1017/skelly_synchronize/core_processes/debugging/debug_output.py
--rw-r--r--   0        0        0     2697 2023-05-24 17:56:05.922732 skelly_synchronize-2023.5.1017/skelly_synchronize/core_processes/debugging/debug_plots.py
--rw-r--r--   0        0        0     1557 2023-05-24 17:56:05.922732 skelly_synchronize-2023.5.1017/skelly_synchronize/core_processes/video_functions/deffcode_functions.py
--rw-r--r--   0        0        0     2699 2023-05-24 17:56:05.922732 skelly_synchronize-2023.5.1017/skelly_synchronize/core_processes/video_functions/ffmpeg_functions.py
--rw-r--r--   0        0        0     4510 2023-05-24 17:56:05.922732 skelly_synchronize-2023.5.1017/skelly_synchronize/core_processes/video_functions/video_utilities.py
--rw-r--r--   0        0        0     1873 2023-05-24 17:56:05.922732 skelly_synchronize-2023.5.1017/skelly_synchronize/gui/skelly_synchronize_gui.py
--rw-r--r--   0        0        0      420 2023-05-24 17:56:05.922732 skelly_synchronize-2023.5.1017/skelly_synchronize/gui/widgets/run_button_widget.py
--rw-r--r--   0        0        0     4989 2023-05-24 17:56:05.922732 skelly_synchronize-2023.5.1017/skelly_synchronize/skelly_synchronize.py
--rw-r--r--   0        0        0        0 2023-05-24 17:56:05.922732 skelly_synchronize-2023.5.1017/skelly_synchronize/system/__init__.py
--rw-r--r--   0        0        0     1479 2023-05-24 17:56:05.922732 skelly_synchronize-2023.5.1017/skelly_synchronize/system/default_paths.py
--rw-r--r--   0        0        0     1402 2023-05-24 17:56:05.922732 skelly_synchronize-2023.5.1017/skelly_synchronize/system/logging_configuration.py
--rw-r--r--   0        0        0      555 2023-05-24 17:56:05.922732 skelly_synchronize-2023.5.1017/skelly_synchronize/system/paths_and_file_names.py
--rw-r--r--   0        0        0     1085 2023-05-24 17:56:05.922732 skelly_synchronize-2023.5.1017/skelly_synchronize/tests/conftest.py
--rw-r--r--   0        0        0      656 2023-05-24 17:56:05.922732 skelly_synchronize-2023.5.1017/skelly_synchronize/tests/test_normalize_lag_dict.py
--rw-r--r--   0        0        0      847 2023-05-24 17:56:05.922732 skelly_synchronize-2023.5.1017/skelly_synchronize/tests/test_trim_single_video_deffcode.py
--rw-r--r--   0        0        0      577 2023-05-24 17:56:05.922732 skelly_synchronize-2023.5.1017/skelly_synchronize/tests/utilities/check_list_values_are_equal.py
--rw-r--r--   0        0        0      262 2023-05-24 17:56:05.922732 skelly_synchronize-2023.5.1017/skelly_synchronize/tests/utilities/find_frame_count_of_video.py
--rw-r--r--   0        0        0     1263 2023-05-24 17:56:05.922732 skelly_synchronize-2023.5.1017/skelly_synchronize/tests/utilities/get_number_of_frames_of_videos_in_a_folder.py
--rw-r--r--   0        0        0     1061 2023-05-24 17:56:05.922732 skelly_synchronize-2023.5.1017/skelly_synchronize/tests/utilities/load_sample_data.py
--rw-r--r--   0        0        0     2048 2023-05-24 17:56:05.922732 skelly_synchronize-2023.5.1017/skelly_synchronize/utils/check_if_video_has_reversed_metadata.py
--rw-r--r--   0        0        0     1340 2023-05-24 17:56:05.922732 skelly_synchronize-2023.5.1017/skelly_synchronize/utils/get_video_files.py
--rw-r--r--   0        0        0     1103 2023-05-24 17:56:05.922732 skelly_synchronize-2023.5.1017/skelly_synchronize/utils/path_handling_utilities.py
--rw-r--r--   0        0        0     3961 1970-01-01 00:00:00.000000 skelly_synchronize-2023.5.1017/PKG-INFO
+-rw-r--r--   0        0        0       65 2023-06-03 23:33:27.086966 skelly_synchronize-2023.6.1018/.gitattributes
+-rw-r--r--   0        0        0      146 2023-06-03 23:33:27.086966 skelly_synchronize-2023.6.1018/.github/workflows/lint-with-black.yml
+-rw-r--r--   0        0        0     1087 2023-06-03 23:33:27.086966 skelly_synchronize-2023.6.1018/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml
+-rw-r--r--   0        0        0     1025 2023-06-03 23:33:27.086966 skelly_synchronize-2023.6.1018/.github/workflows/python-testing.yml
+-rw-r--r--   0        0        0     2783 2023-06-03 23:33:27.086966 skelly_synchronize-2023.6.1018/.gitignore
+-rw-r--r--   0        0        0    34523 2023-06-03 23:33:27.086966 skelly_synchronize-2023.6.1018/LICENSE
+-rw-r--r--   0        0        0     3030 2023-06-03 23:33:27.086966 skelly_synchronize-2023.6.1018/README.md
+-rw-r--r--   0        0        0     1639 2023-06-03 23:33:27.086966 skelly_synchronize-2023.6.1018/pyproject.toml
+-rw-r--r--   0        0        0      150 2023-06-03 23:33:27.086966 skelly_synchronize-2023.6.1018/requirements.txt
+-rw-r--r--   0        0        0       50 2023-06-03 23:33:27.086966 skelly_synchronize-2023.6.1018/setup.py
+-rw-r--r--   0        0        0     1056 2023-06-03 23:33:27.086966 skelly_synchronize-2023.6.1018/skelly_synchronize/__init__.py
+-rw-r--r--   0        0        0      333 2023-06-03 23:33:27.086966 skelly_synchronize-2023.6.1018/skelly_synchronize/__main__.py
+-rw-r--r--   0        0        0     3401 2023-06-03 23:33:27.086966 skelly_synchronize-2023.6.1018/skelly_synchronize/core_processes/audio_utilities.py
+-rw-r--r--   0        0        0     2758 2023-06-03 23:33:27.086966 skelly_synchronize-2023.6.1018/skelly_synchronize/core_processes/correlation_functions.py
+-rw-r--r--   0        0        0      616 2023-06-03 23:33:27.086966 skelly_synchronize-2023.6.1018/skelly_synchronize/core_processes/debugging/debug_output.py
+-rw-r--r--   0        0        0     2136 2023-06-03 23:33:27.086966 skelly_synchronize-2023.6.1018/skelly_synchronize/core_processes/debugging/debug_plots.py
+-rw-r--r--   0        0        0     1557 2023-06-03 23:33:27.086966 skelly_synchronize-2023.6.1018/skelly_synchronize/core_processes/video_functions/deffcode_functions.py
+-rw-r--r--   0        0        0     3438 2023-06-03 23:33:27.086966 skelly_synchronize-2023.6.1018/skelly_synchronize/core_processes/video_functions/ffmpeg_functions.py
+-rw-r--r--   0        0        0     5993 2023-06-03 23:33:27.086966 skelly_synchronize-2023.6.1018/skelly_synchronize/core_processes/video_functions/video_utilities.py
+-rw-r--r--   0        0        0     1873 2023-06-03 23:33:27.086966 skelly_synchronize-2023.6.1018/skelly_synchronize/gui/skelly_synchronize_gui.py
+-rw-r--r--   0        0        0      420 2023-06-03 23:33:27.086966 skelly_synchronize-2023.6.1018/skelly_synchronize/gui/widgets/run_button_widget.py
+-rw-r--r--   0        0        0     5326 2023-06-03 23:33:27.086966 skelly_synchronize-2023.6.1018/skelly_synchronize/skelly_synchronize.py
+-rw-r--r--   0        0        0        0 2023-06-03 23:33:27.086966 skelly_synchronize-2023.6.1018/skelly_synchronize/system/__init__.py
+-rw-r--r--   0        0        0     1479 2023-06-03 23:33:27.086966 skelly_synchronize-2023.6.1018/skelly_synchronize/system/default_paths.py
+-rw-r--r--   0        0        0     1402 2023-06-03 23:33:27.086966 skelly_synchronize-2023.6.1018/skelly_synchronize/system/logging_configuration.py
+-rw-r--r--   0        0        0      599 2023-06-03 23:33:27.086966 skelly_synchronize-2023.6.1018/skelly_synchronize/system/paths_and_file_names.py
+-rw-r--r--   0        0        0     1085 2023-06-03 23:33:27.086966 skelly_synchronize-2023.6.1018/skelly_synchronize/tests/conftest.py
+-rw-r--r--   0        0        0      656 2023-06-03 23:33:27.086966 skelly_synchronize-2023.6.1018/skelly_synchronize/tests/test_normalize_lag_dict.py
+-rw-r--r--   0        0        0      847 2023-06-03 23:33:27.086966 skelly_synchronize-2023.6.1018/skelly_synchronize/tests/test_trim_single_video_deffcode.py
+-rw-r--r--   0        0        0      577 2023-06-03 23:33:27.086966 skelly_synchronize-2023.6.1018/skelly_synchronize/tests/utilities/check_list_values_are_equal.py
+-rw-r--r--   0        0        0      262 2023-06-03 23:33:27.086966 skelly_synchronize-2023.6.1018/skelly_synchronize/tests/utilities/find_frame_count_of_video.py
+-rw-r--r--   0        0        0     1263 2023-06-03 23:33:27.086966 skelly_synchronize-2023.6.1018/skelly_synchronize/tests/utilities/get_number_of_frames_of_videos_in_a_folder.py
+-rw-r--r--   0        0        0     1061 2023-06-03 23:33:27.086966 skelly_synchronize-2023.6.1018/skelly_synchronize/tests/utilities/load_sample_data.py
+-rw-r--r--   0        0        0     2048 2023-06-03 23:33:27.086966 skelly_synchronize-2023.6.1018/skelly_synchronize/utils/check_if_video_has_reversed_metadata.py
+-rw-r--r--   0        0        0     1348 2023-06-03 23:33:27.086966 skelly_synchronize-2023.6.1018/skelly_synchronize/utils/get_video_files.py
+-rw-r--r--   0        0        0     1103 2023-06-03 23:33:27.086966 skelly_synchronize-2023.6.1018/skelly_synchronize/utils/path_handling_utilities.py
+-rw-r--r--   0        0        0     3961 1970-01-01 00:00:00.000000 skelly_synchronize-2023.6.1018/PKG-INFO
```

### Comparing `skelly_synchronize-2023.5.1017/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml` & `skelly_synchronize-2023.6.1018/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1017/.github/workflows/python-testing.yml` & `skelly_synchronize-2023.6.1018/.github/workflows/python-testing.yml`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1017/.gitignore` & `skelly_synchronize-2023.6.1018/.gitignore`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1017/LICENSE` & `skelly_synchronize-2023.6.1018/LICENSE`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1017/README.md` & `skelly_synchronize-2023.6.1018/README.md`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1017/pyproject.toml` & `skelly_synchronize-2023.6.1018/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [tool.bumpver] #bump the version by entering `bumpver update` in the terminal
-current_version = "v2023.05.1017"
+current_version = "v2023.06.1018"
 version_pattern = "vYYYY.0M.BUILD[-TAG]"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `skelly_synchronize-2023.5.1017/skelly_synchronize/__init__.py` & `skelly_synchronize-2023.6.1018/skelly_synchronize/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Top-level package for basic_template_repo."""
 
 __package_name__ = "skelly_synchronize"
-__version__ = "v2023.05.1017"
+__version__ = "v2023.06.1018"
 
 __author__ = """Philip Queen"""
 __email__ = "info@freemocap.org"
 __repo_owner_github_user_name__ = "freemocap"
 __repo_url__ = (
     f"https://github.com/{__repo_owner_github_user_name__}/{__package_name__}/"
 )
```

### Comparing `skelly_synchronize-2023.5.1017/skelly_synchronize/core_processes/audio_utilities.py` & `skelly_synchronize-2023.6.1018/skelly_synchronize/core_processes/audio_utilities.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import logging
-from pathlib import Path
 import librosa
+import soundfile as sf
+from pathlib import Path
 import numpy as np
 from typing import Dict
 
 from skelly_synchronize.core_processes.video_functions.ffmpeg_functions import (
     extract_audio_from_video_ffmpeg,
 )
+from skelly_synchronize.system.paths_and_file_names import TRIMMED_AUDIO_FOLDER_NAME
 
 
 def get_audio_sample_rates(audio_signal_dict: Dict[str, float]) -> list:
     """Get the sample rates of each audio file and return them in a list"""
     audio_sample_rate_list = [
         single_audio_dict["sample rate"]
         for single_audio_dict in audio_signal_dict.values()
@@ -52,7 +54,36 @@
             "audio file": audio_signal,
             "sample rate": sample_rate,
             "camera name": video_dict["camera name"],
             "audio duration": audio_duration,
         }
 
     return audio_signal_dict
+
+
+def trim_audio_files(
+    audio_folder_path: Path, lag_dictionary: dict, synced_video_length: float
+):
+    logging.info("Trimming audio files to match synchronized video length")
+
+    trimmed_audio_folder_path = Path(audio_folder_path) / TRIMMED_AUDIO_FOLDER_NAME
+    trimmed_audio_folder_path.mkdir(parents=True, exist_ok=True)
+
+    for audio_filepath in audio_folder_path.glob("*.wav"):
+        audio_signal, sr = librosa.load(path=audio_filepath, sr=None)
+        lag = lag_dictionary[audio_filepath.stem]
+
+        lag_in_samples = int(float(lag) * sr)
+        synched_video_length_in_samples = int(synced_video_length * sr)
+
+        shortened_audio_signal = audio_signal[lag_in_samples:]
+        shortened_audio_signal = shortened_audio_signal[
+            :synched_video_length_in_samples
+        ]
+
+        audio_filename = str(audio_filepath.stem) + ".wav"
+
+        logging.info(f"Saving audio {audio_filename}")
+        output_path = trimmed_audio_folder_path / audio_filename
+        sf.write(output_path, shortened_audio_signal, sr, subtype="PCM_24")
+
+    return trimmed_audio_folder_path
```

### Comparing `skelly_synchronize-2023.5.1017/skelly_synchronize/core_processes/correlation_functions.py` & `skelly_synchronize-2023.6.1018/skelly_synchronize/core_processes/correlation_functions.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1017/skelly_synchronize/core_processes/debugging/debug_output.py` & `skelly_synchronize-2023.6.1018/skelly_synchronize/core_processes/debugging/debug_output.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1017/skelly_synchronize/core_processes/video_functions/deffcode_functions.py` & `skelly_synchronize-2023.6.1018/skelly_synchronize/core_processes/video_functions/deffcode_functions.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1017/skelly_synchronize/core_processes/video_functions/ffmpeg_functions.py` & `skelly_synchronize-2023.6.1018/skelly_synchronize/core_processes/video_functions/ffmpeg_functions.py`

 * *Files 9% similar despite different names*

```diff
@@ -92,7 +92,35 @@
             f"{desired_duration}",
             "-y",
             f"{output_video_pathstring}",
         ],
         stdout=subprocess.PIPE,
         stderr=subprocess.STDOUT,
     )
+
+
+def attach_audio_to_video_ffmpeg(
+    input_video_pathstring: str,
+    audio_file_pathstring: str,
+    output_video_pathstring: str,
+):
+    """Run a subprocess call to attach audio file back to the video"""
+
+    attach_audio_subprocess = subprocess.run(
+        [
+            "ffmpeg",
+            "-i",
+            f"{input_video_pathstring}",
+            "-i",
+            f"{audio_file_pathstring}",
+            "-c:v",
+            "copy",
+            "-c:a",
+            "aac",
+            f"{output_video_pathstring}",
+        ],
+        stdout=subprocess.PIPE,
+        stderr=subprocess.PIPE,
+    )
+
+    if attach_audio_subprocess.returncode != 0:
+        print(f"Error occurred: {attach_audio_subprocess.stderr.decode('utf-8')}")
```

### Comparing `skelly_synchronize-2023.5.1017/skelly_synchronize/gui/skelly_synchronize_gui.py` & `skelly_synchronize-2023.6.1018/skelly_synchronize/gui/skelly_synchronize_gui.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1017/skelly_synchronize/skelly_synchronize.py` & `skelly_synchronize-2023.6.1018/skelly_synchronize/skelly_synchronize.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from skelly_synchronize.utils.get_video_files import get_video_file_list
 from skelly_synchronize.core_processes.audio_utilities import (
     extract_audio_files,
     get_audio_sample_rates,
 )
 from skelly_synchronize.core_processes.correlation_functions import find_lags
 from skelly_synchronize.core_processes.video_functions.video_utilities import (
+    attach_audio_to_videos,
     get_fps_list,
     create_video_info_dict,
     trim_videos,
 )
 from skelly_synchronize.core_processes.debugging.debug_output import (
     remove_audio_files_from_audio_signal_dict,
     save_dictionaries_to_toml,
@@ -119,14 +120,23 @@
                 audio_signal_dictionary=audio_signal_dict
             ),
             LAG_DICTIONARY_NAME: lag_dict,
         },
         output_file_path=synchronized_video_folder_path / DEBUG_TOML_NAME,
     )
 
+    attach_audio_to_videos(
+        synchronized_video_folder_path=synchronized_video_folder_path,
+        audio_folder_path=audio_folder_path,
+        lag_dictionary=lag_dict,
+        synchronized_video_length=next(iter(synchronized_video_info_dict.values()))[
+            "video duration"
+        ],
+    )
+
     create_debug_plots(synchronized_video_folder_path=synchronized_video_folder_path)
 
     end_timer = time.time()
 
     logging.info(f"Elapsed processing time in seconds: {end_timer - start_timer}")
 
     return synchronized_video_folder_path
```

### Comparing `skelly_synchronize-2023.5.1017/skelly_synchronize/system/default_paths.py` & `skelly_synchronize-2023.6.1018/skelly_synchronize/system/default_paths.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1017/skelly_synchronize/system/logging_configuration.py` & `skelly_synchronize-2023.6.1018/skelly_synchronize/system/logging_configuration.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1017/skelly_synchronize/system/paths_and_file_names.py` & `skelly_synchronize-2023.6.1018/skelly_synchronize/system/paths_and_file_names.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # directory names
 SYNCHRONIZED_VIDEOS_FOLDER_NAME = "synchronized_videos"
 AUDIO_FILES_FOLDER_NAME = "audio_files"
+TRIMMED_AUDIO_FOLDER_NAME = "trimmed_audio"
 
 # file names
 DEBUG_TOML_NAME = "synchronization_debug.toml"
 DEBUG_PLOT_NAME = "debug_plot.png"
 
 # debug dictionary keys
 RAW_VIDEO_NAME = "Raw_video_information"
```

### Comparing `skelly_synchronize-2023.5.1017/skelly_synchronize/tests/conftest.py` & `skelly_synchronize-2023.6.1018/skelly_synchronize/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1017/skelly_synchronize/tests/test_normalize_lag_dict.py` & `skelly_synchronize-2023.6.1018/skelly_synchronize/tests/test_normalize_lag_dict.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1017/skelly_synchronize/tests/test_trim_single_video_deffcode.py` & `skelly_synchronize-2023.6.1018/skelly_synchronize/tests/test_trim_single_video_deffcode.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1017/skelly_synchronize/tests/utilities/check_list_values_are_equal.py` & `skelly_synchronize-2023.6.1018/skelly_synchronize/tests/utilities/check_list_values_are_equal.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1017/skelly_synchronize/tests/utilities/get_number_of_frames_of_videos_in_a_folder.py` & `skelly_synchronize-2023.6.1018/skelly_synchronize/tests/utilities/get_number_of_frames_of_videos_in_a_folder.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1017/skelly_synchronize/tests/utilities/load_sample_data.py` & `skelly_synchronize-2023.6.1018/skelly_synchronize/tests/utilities/load_sample_data.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1017/skelly_synchronize/utils/check_if_video_has_reversed_metadata.py` & `skelly_synchronize-2023.6.1018/skelly_synchronize/utils/check_if_video_has_reversed_metadata.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1017/skelly_synchronize/utils/get_video_files.py` & `skelly_synchronize-2023.6.1018/skelly_synchronize/utils/get_video_files.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 from pathlib import Path
 
 
-def get_video_file_list(folder_path: Path, file_type: str) -> list:
+def get_video_file_list(folder_path: Path, file_type: str = "mp4") -> list:
     """Return a list of all video files in the base_path folder that match the given file type.
     file_type can be upper or lower case, with or without a leading period"""
 
     # create general search from file type to use in glob search, including cases for upper and lowercase file types
     file_extension_upper = "*" + file_type.upper()
     file_extension_lower = "*" + file_type.lower()
     # make list of all files with file type
```

### Comparing `skelly_synchronize-2023.5.1017/skelly_synchronize/utils/path_handling_utilities.py` & `skelly_synchronize-2023.6.1018/skelly_synchronize/utils/path_handling_utilities.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1017/PKG-INFO` & `skelly_synchronize-2023.6.1018/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skelly_synchronize
-Version: 2023.5.1017
+Version: 2023.6.1018
 Summary: Basic template of a python repository
 Keywords: basic,template,python,repository
 Author-email: skelly_synchronize <info@freemocap.org>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python
```

