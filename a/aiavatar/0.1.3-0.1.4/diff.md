# Comparing `tmp/aiavatar-0.1.3-py3-none-any.whl.zip` & `tmp/aiavatar-0.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 19376 bytes, number of entries: 20
+Zip file size: 19644 bytes, number of entries: 20
 -rw-r--r--  2.0 unx      351 b- defN 23-May-27 12:45 aiavatar/__init__.py
--rw-r--r--  2.0 unx     3407 b- defN 23-May-27 09:17 aiavatar/avatar.py
--rw-r--r--  2.0 unx     5501 b- defN 23-Jun-03 08:34 aiavatar/bot.py
+-rw-r--r--  2.0 unx     3407 b- defN 23-Jun-04 12:15 aiavatar/avatar.py
+-rw-r--r--  2.0 unx     5621 b- defN 23-Jun-04 16:36 aiavatar/bot.py
 -rw-r--r--  2.0 unx      284 b- defN 23-May-27 03:16 aiavatar/animation/__init__.py
 -rw-r--r--  2.0 unx       31 b- defN 23-May-27 03:48 aiavatar/device/__init__.py
 -rw-r--r--  2.0 unx     2535 b- defN 23-Jun-03 02:13 aiavatar/device/audio.py
--rw-r--r--  2.0 unx      888 b- defN 23-May-27 09:19 aiavatar/face/__init__.py
--rw-r--r--  2.0 unx     1709 b- defN 23-Jun-03 08:21 aiavatar/face/vrchat.py
+-rw-r--r--  2.0 unx     1650 b- defN 23-Jun-04 16:30 aiavatar/face/__init__.py
+-rw-r--r--  2.0 unx     1556 b- defN 23-Jun-04 16:30 aiavatar/face/vrchat.py
 -rw-r--r--  2.0 unx     6210 b- defN 23-Jun-03 02:23 aiavatar/listeners/__init__.py
 -rw-r--r--  2.0 unx      788 b- defN 23-May-24 12:01 aiavatar/listeners/voicerequest.py
 -rw-r--r--  2.0 unx     1007 b- defN 23-Jun-03 02:44 aiavatar/listeners/wakeword.py
 -rw-r--r--  2.0 unx      178 b- defN 23-May-27 08:55 aiavatar/processors/__init__.py
 -rw-r--r--  2.0 unx     2151 b- defN 23-May-27 08:42 aiavatar/processors/chatgpt.py
 -rw-r--r--  2.0 unx      275 b- defN 23-May-27 08:54 aiavatar/speech/__init__.py
 -rw-r--r--  2.0 unx     2794 b- defN 23-Jun-02 14:22 aiavatar/speech/voicevox.py
--rw-r--r--  2.0 unx    11324 b- defN 23-Jun-03 08:36 aiavatar-0.1.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     7901 b- defN 23-Jun-03 08:36 aiavatar-0.1.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-03 08:36 aiavatar-0.1.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Jun-03 08:36 aiavatar-0.1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1629 b- defN 23-Jun-03 08:36 aiavatar-0.1.3.dist-info/RECORD
-20 files, 49064 bytes uncompressed, 16724 bytes compressed:  65.9%
+-rw-r--r--  2.0 unx    11324 b- defN 23-Jun-04 16:45 aiavatar-0.1.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     8081 b- defN 23-Jun-04 16:45 aiavatar-0.1.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-04 16:45 aiavatar-0.1.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Jun-04 16:45 aiavatar-0.1.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1630 b- defN 23-Jun-04 16:45 aiavatar-0.1.4.dist-info/RECORD
+20 files, 49974 bytes uncompressed, 16992 bytes compressed:  66.0%
```

## zipnote {}

```diff
@@ -39,23 +39,23 @@
 
 Filename: aiavatar/speech/__init__.py
 Comment: 
 
 Filename: aiavatar/speech/voicevox.py
 Comment: 
 
-Filename: aiavatar-0.1.3.dist-info/LICENSE
+Filename: aiavatar-0.1.4.dist-info/LICENSE
 Comment: 
 
-Filename: aiavatar-0.1.3.dist-info/METADATA
+Filename: aiavatar-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: aiavatar-0.1.3.dist-info/WHEEL
+Filename: aiavatar-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: aiavatar-0.1.3.dist-info/top_level.txt
+Filename: aiavatar-0.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: aiavatar-0.1.3.dist-info/RECORD
+Filename: aiavatar-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aiavatar/bot.py

```diff
@@ -17,14 +17,15 @@
 class AIAvatar:
     def __init__(
         self,
         google_api_key: str,
         openai_api_key: str,
         voicevox_url: str,
         voicevox_speaker_id: int=46,
+        volume_threshold: int=3000,
         start_voice: str="どうしたの",
         system_message_content: str=None,
         animation_controller: AnimationController=None,
         face_controller: FaceController=None,
         avatar_request_parser: Callable=None,
         input_device: int=-1,
         output_device: int=-1
@@ -33,14 +34,15 @@
         self.logger = getLogger(__name__)
         self.logger.addHandler(NullHandler())
 
         self.google_api_key = google_api_key
         self.openai_api_key = openai_api_key
         self.voicevox_url = voicevox_url
         self.voicevox_speaker_id = voicevox_speaker_id
+        self.volume_threshold = volume_threshold
 
         # Audio Devices
         if isinstance(input_device, int):
             if input_device < 0:
                 input_device_info = AudioDevice.get_default_input_device_info()
                 input_device = input_device_info["index"]
             else:
@@ -69,15 +71,15 @@
         self.output_device = output_device
         self.logger.info(f"Output device: [{output_device}] {output_device_info['name']}")
 
         # Processor
         self.chat_processor = ChatGPTProcessor(self.openai_api_key, system_message_content=system_message_content)
 
         # Listeners
-        self.request_listener = VoiceRequestListener(self.google_api_key, device_index=self.input_device)
+        self.request_listener = VoiceRequestListener(self.google_api_key, volume_threshold=volume_threshold, device_index=self.input_device)
 
         # Avatar
         speech_controller = VoicevoxSpeechController(self.voicevox_url, self.voicevox_speaker_id, device_index=self.output_device)
         animation_controller = animation_controller or AnimationControllerDummy()
         face_controller = face_controller or FaceControllerDummy()
         self.avatar_controller = AvatarController(speech_controller, animation_controller, face_controller, avatar_request_parser)
```

## aiavatar/face/__init__.py

```diff
@@ -1,29 +1,58 @@
 from abc import ABC, abstractmethod
-import asyncio
 from logging import getLogger, NullHandler
-from time import time
+from threading import Thread
+from time import time, sleep
 
 class FaceController(ABC):
     @abstractmethod
     async def set_face(self, name: str, duration: float):
         pass
 
-class FaceControllerDummy(FaceController):
-    def __init__(self) -> None:
+    @abstractmethod
+    def reset(self):
+        pass
+
+
+class FaceControllerBase(FaceController):
+    def __init__(self, verbose: bool=False):
         self.logger = getLogger(__name__)
         self.logger.addHandler(NullHandler())
+        self.verbose = verbose
 
         self.faces = {
             "neutral": "('_')",
             "joy": "(^o^)",
             "angry": "(#｀Д´)",
             "sorrow": "(; ;)",
             "fun": "(*^_^*)",
         }
 
+        self.reset_at = None
+        self.reset_thread = Thread(target=self.reset_worker, daemon=True)
+        self.reset_thread.start()
+
+    def reset_worker(self):
+        while True:
+            if self.reset_at and time() >= self.reset_at:
+                if self.verbose:
+                    self.logger.info(f"Time to reset: {self.reset_at}")
+                self.reset()
+                self.reset_at = None
+
+            sleep(0.1)
+
+    def subscribe_reset(self, reset_at: float):
+        self.reset_at = reset_at
+        if self.verbose:
+            self.logger.info(f"Reset subscribed at {self.reset_at}")
+
     async def set_face(self, name: str, duration: float):
-        start_at = time()
+        self.subscribe_reset(time() + duration)
         self.logger.info(f"face: {self.faces[name]} ({name})")
-        while time() - start_at <= duration:
-            await asyncio.sleep(0.1)
-        self.logger.info(f"face: {self.faces['neutral']} (neutral)")
+
+    def reset(self):
+        self.logger.info(f"Reset face: {self.faces['neutral']} (neutral)")
+
+
+class FaceControllerDummy(FaceControllerBase):
+    pass
```

## aiavatar/face/vrchat.py

```diff
@@ -1,17 +1,15 @@
 import asyncio
-from logging import getLogger, NullHandler
 from time import time
 from pythonosc import udp_client
-from . import FaceController
+from . import FaceControllerBase
 
-class VRChatFaceController(FaceController):
-    def __init__(self, osc_address: str="/avatar/parameters/FaceOSC", faces: dict=None, neutral_key: str="neutral", host: str="127.0.0.1", port: int=9000):
-        self.logger = getLogger(__name__)
-        self.logger.addHandler(NullHandler())
+class VRChatFaceController(FaceControllerBase):
+    def __init__(self, osc_address: str="/avatar/parameters/FaceOSC", faces: dict=None, neutral_key: str="neutral", host: str="127.0.0.1", port: int=9000, verbose: bool=False):
+        super().__init__(verbose)
 
         self.osc_address = osc_address
         self.faces = faces or {
             "neutral": 0,
             "joy": 1,
             "angry": 2,
             "sorrow": 3,
@@ -21,26 +19,26 @@
         self.neutral_key = neutral_key
         self.host = host
         self.port = port
 
         self.client = udp_client.SimpleUDPClient(self.host, self.port)
 
     async def set_face(self, name: str, duration: float):
-        start_at = time()
+        self.subscribe_reset(time() + duration)
+
         osc_value = self.faces.get(name)
         if osc_value is None:
-            print(f"Face '{name}' is not registered")
             self.logger.warning(f"Face '{name}' is not registered")
             return
 
         self.logger.info(f"face: {name} ({osc_value})")
         self.client.send_message(self.osc_address, osc_value)
-        while time() - start_at <= duration:
-            await asyncio.sleep(0.1)
-        self.logger.info(f"face: {self.neutral_key} ({self.faces[self.neutral_key]})")
+
+    def reset(self):
+        self.logger.info(f"Reset face: {self.neutral_key} ({self.faces[self.neutral_key]})")
         self.client.send_message(self.osc_address, self.faces[self.neutral_key])
 
     def test_osc(self):
         while True:
             self.set_face(input("Face name: "), 3.0)
 
 if __name__ == "__main__":
```

## Comparing `aiavatar-0.1.3.dist-info/LICENSE` & `aiavatar-0.1.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `aiavatar-0.1.3.dist-info/METADATA` & `aiavatar-0.1.4.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiavatar
-Version: 0.1.3
+Version: 0.1.4
 Summary: 🥰 Building AI-based conversational avatars lightning fast ⚡️💬
 Home-page: https://github.com/uezo/aiavatar
 Author: uezo
 Author-email: uezo@uezo.net
 Maintainer: uezo
 Maintainer-email: uezo@uezo.net
 License: Apache v2
@@ -73,26 +73,28 @@
 
 # Create AIAvatar
 app = AIAvatar(
     google_api_key=GOOGLE_API_KEY,
     openai_api_key=OPENAI_API_KEY,
     voicevox_url=VV_URL,
     voicevox_speaker_id=VV_SPEAKER,
+    # volume_threshold=2000,    # <- Set to adjust microphone sensitivity
     system_message_content=system_message_content,
 )
 
 # Create WakewordListener
 wakewords = ["こんにちは"]
 
 async def on_wakeword(text):
     logger.info(f"Wakeword: {text}")
     await app.start_chat()
 
 wakeword_listener = WakewordListener(
     api_key=GOOGLE_API_KEY,
+    volume_threshold=app.volume_threshold,
     wakewords=wakewords,
     on_wakeword=on_wakeword,
     device_index=app.input_device
 )
 
 # Start listening
 ww_thread = wakeword_listener.start()
@@ -191,14 +193,15 @@
     VoicevoxSpeechController,
     WakewordListener
 )
 
 GOOGLE_API_KEY = "YOUR_API_KEY"
 VV_URL = "http://127.0.0.1:50021"
 VV_SPEAKER = 46
+VOLUME_THRESHOLD = 3000
 INPUT_DEVICE = -1
 OUTPUT_DEVICE = -1
 
 # Configure root logger
 logger = logging.getLogger()
 logger.setLevel(logging.INFO)
 log_format = logging.Formatter("[%(levelname)s] %(asctime)s : %(message)s")
@@ -236,14 +239,15 @@
 wakewords = ["こんにちは"]
 async def on_wakeword(text):
     logger.info(f"Wakeword: {text}")
     await speaker.speak(f"{text}")
 
 wakeword_listener = WakewordListener(
     api_key=GOOGLE_API_KEY,
+    volume_threshold=VOLUME_THRESHOLD,
     wakewords=["こんにちは"],
     on_wakeword=on_wakeword,
     verbose=True,
     device_index=input_device
 )
 
 # Start listening
```

## Comparing `aiavatar-0.1.3.dist-info/RECORD` & `aiavatar-0.1.4.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 aiavatar/__init__.py,sha256=SqrO15owXtN32q55sRbSxKqRJyOZ32gao4a-SQwJTA8,351
 aiavatar/avatar.py,sha256=ML4A_-cFggDOT4Sxb7VQMHvHD_rATxhY3Pt85ZppEKg,3407
-aiavatar/bot.py,sha256=G5vIAvW7sNhiaIjdsUoSMYLB8MhKQ2JYIQj-PGplXNo,5501
+aiavatar/bot.py,sha256=jkab04ZSwhbCy8GVwa7ms58EE_LrmipTTDRFUuI1ycc,5621
 aiavatar/animation/__init__.py,sha256=cE0zS3FgTUd0c6LcsLUnDVSTlFrCF0ZiH7-4NJxiQnU,284
 aiavatar/device/__init__.py,sha256=4DhskQxS20PcErkyF3z5-RuvXtGCQvw37jqB-yc2As8,31
 aiavatar/device/audio.py,sha256=oCqxsY3lB6ZULTA9EhausaTgKYMxrSBhKYytr2FQap0,2535
-aiavatar/face/__init__.py,sha256=nrnFS0NUhqwdW81vM2OVdQIYd2vSi7VKIEdO4ys7_Co,888
-aiavatar/face/vrchat.py,sha256=xcwUs3CWG3pX0_ODuGBytbV0SSMfekORCLh0FFuQtM4,1709
+aiavatar/face/__init__.py,sha256=FPaP8RT8UXQ_UMON7RLvg2FUotOzTFVJ1qxzVk5zBTw,1650
+aiavatar/face/vrchat.py,sha256=VOibFm5Yuof-RQGfd1Zt1tx4v-TV9Usb8aMn7rHp5HY,1556
 aiavatar/listeners/__init__.py,sha256=7EU4Ea6AdJa9soe5WtgBcJ8rsKb43M-0cmBQfUvUQXY,6210
 aiavatar/listeners/voicerequest.py,sha256=6636rbXDJ0Dw6EPD0kSsF3f46A4H0zjyY7fAMzpAvkc,788
 aiavatar/listeners/wakeword.py,sha256=UMM-1HMmEFXQpIt9C2EOuGSoxJHj1fQdrz_e9adJiGs,1007
 aiavatar/processors/__init__.py,sha256=k6qF1_UopWpaxQ89OxP7-dSVLgnrDCuuZH0Gom0JLLU,178
 aiavatar/processors/chatgpt.py,sha256=snlUw6eYS__j_PM8ab7YZmE4CcalXKQLpdO_4JQa_h0,2151
 aiavatar/speech/__init__.py,sha256=yiveD86ikoWYYVnpdi1r_6ou5bXr-SOkmnri6ry_qHI,275
 aiavatar/speech/voicevox.py,sha256=SsR-yFHb7fLYvA4M08wPw_eqiq9ZyISkeqHeiV2Epco,2794
-aiavatar-0.1.3.dist-info/LICENSE,sha256=UOZ1F5fFDe3XXvG4oNnkL1-Ecun7zpHzRxjp-XsMeAo,11324
-aiavatar-0.1.3.dist-info/METADATA,sha256=gTrc1823_rkBoSiHjBd4MgSwacTRpVNvu52NLNqgGxk,7901
-aiavatar-0.1.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-aiavatar-0.1.3.dist-info/top_level.txt,sha256=B14WVaakM_kKuOkCeI-WRP83BJ6APkOyQrn6EXxs8kg,9
-aiavatar-0.1.3.dist-info/RECORD,,
+aiavatar-0.1.4.dist-info/LICENSE,sha256=UOZ1F5fFDe3XXvG4oNnkL1-Ecun7zpHzRxjp-XsMeAo,11324
+aiavatar-0.1.4.dist-info/METADATA,sha256=QsxGgQdCSemzPf7UmTQR23FH6QLdl3gTRjmwHj7KjMA,8081
+aiavatar-0.1.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+aiavatar-0.1.4.dist-info/top_level.txt,sha256=B14WVaakM_kKuOkCeI-WRP83BJ6APkOyQrn6EXxs8kg,9
+aiavatar-0.1.4.dist-info/RECORD,,
```

