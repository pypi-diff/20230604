# Comparing `tmp/Kurdish2Image-0.0.1-py2.py3-none-any.whl.zip` & `tmp/Kurdish2Image-0.0.2-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,10 @@
-Zip file size: 2926 bytes, number of entries: 7
+Zip file size: 3535 bytes, number of entries: 8
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-04 06:43 kurdish2image/__init__.py
--rw-rw-rw-  2.0 fat     1982 b- defN 23-Jun-04 06:53 kurdish2image/kurdish2image.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-04 07:08 Kurdish2Image-0.0.1.dist-info/License.txt
--rw-rw-rw-  2.0 fat     1206 b- defN 23-Jun-04 07:08 Kurdish2Image-0.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Jun-04 07:08 Kurdish2Image-0.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       14 b- defN 23-Jun-04 07:08 Kurdish2Image-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      584 b- defN 23-Jun-04 07:08 Kurdish2Image-0.0.1.dist-info/RECORD
-7 files, 3896 bytes uncompressed, 1876 bytes compressed:  51.8%
+-rw-rw-rw-  2.0 fat     1148 b- defN 23-Jun-04 07:26 kurdish2image/kurdish2image.py
+-rw-rw-rw-  2.0 fat      115 b- defN 23-Jun-04 07:17 kurdish2image/my-test.py
+-rw-rw-rw-  2.0 fat     1085 b- defN 23-Jun-04 07:44 Kurdish2Image-0.0.2.dist-info/License.txt
+-rw-rw-rw-  2.0 fat     1244 b- defN 23-Jun-04 07:44 Kurdish2Image-0.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Jun-04 07:44 Kurdish2Image-0.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       14 b- defN 23-Jun-04 07:44 Kurdish2Image-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      667 b- defN 23-Jun-04 07:44 Kurdish2Image-0.0.2.dist-info/RECORD
+8 files, 4383 bytes uncompressed, 2361 bytes compressed:  46.1%
```

## zipnote {}

```diff
@@ -1,22 +1,25 @@
 Filename: kurdish2image/__init__.py
 Comment: 
 
 Filename: kurdish2image/kurdish2image.py
 Comment: 
 
-Filename: Kurdish2Image-0.0.1.dist-info/License.txt
+Filename: kurdish2image/my-test.py
 Comment: 
 
-Filename: Kurdish2Image-0.0.1.dist-info/METADATA
+Filename: Kurdish2Image-0.0.2.dist-info/License.txt
 Comment: 
 
-Filename: Kurdish2Image-0.0.1.dist-info/WHEEL
+Filename: Kurdish2Image-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: Kurdish2Image-0.0.1.dist-info/top_level.txt
+Filename: Kurdish2Image-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: Kurdish2Image-0.0.1.dist-info/RECORD
+Filename: Kurdish2Image-0.0.2.dist-info/top_level.txt
+Comment: 
+
+Filename: Kurdish2Image-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kurdish2image/kurdish2image.py

```diff
@@ -1,35 +1,34 @@
+from diffusers import StableDiffusionPipeline, EulerDiscreteScheduler
+import torch
+from PIL import Image
+import torchvision.transforms as transforms
+import time
+
 def k2img(prompt):
-    from diffusers import StableDiffusionPipeline, EulerDiscreteScheduler
-    import torch
-    from PIL import Image
-    import torchvision.transforms as transforms
-    #model_id = "CompVis/stable-diffusion-v1-4"
-    # Use the Euler scheduler here instead
-    #scheduler = EulerDiscreteScheduler.from_pretrained(model_id, subfolder="scheduler")
-   # pipe = StableDiffusionPipeline.from_pretrained(model_id, scheduler=scheduler, torch_dtype=torch.float16)
-   # pipe = pipe.to("cuda")
-    #prompt = "a photo of an astronaut riding a horse on mars"
-    #image = pipe(prompt).images[0]    
-   # image.save("out.png")
-   #model_id = "CompVis/stable-diffusion-v1-4"
-    #model_id ="runwayml/stable-diffusion-v1-5"
-    model_id="Falah/kurdish-fashion"
-    # Use the Euler scheduler here instead
+    model_id = "Falah/kurdish-fashion"
     scheduler = EulerDiscreteScheduler.from_pretrained(model_id, subfolder="scheduler")
     pipe = StableDiffusionPipeline.from_pretrained(model_id, scheduler=scheduler, torch_dtype=torch.float16)
     pipe = pipe.to("cuda")
-    #prompt = "full body shot center of view a smiling young female 25 years with jewelry art and with the FLOWERS IN SPRING, Christian Helfgott Brand,color decorative , ,Hyperrealistic neo - rococo solarpunk aesthetic minimal jewelry necklace, embroidery, leather, highly detailed photography art masterpiece, smooth cam de Leon eric zener dramatic pearlescent soft light, ground angle hd 8 k, sharp focus, full body, colors decorative kurdish-fashion style,American shot"
+
     image = pipe(prompt).images[0]
-    # Save the image
-    image.save("out.png")
-    #print("woman5.png")
+
+    # Generate timestamp for the filename
+    timestamp = time.strftime("%Y%m%d%H%M%S")
+
+    # Save the image with the timestamp as the filename
+    image.save(f"out_{timestamp}.png")
+    print("Image saved as out_{timestamp}.png")
+
     # Display the image
     image.show()
+
     # Upscale the image to high resolution
     upscale_transform = transforms.Resize((1920, 1080))
     upscaled_image = upscale_transform(image)
-    # Save the upscaled image
-    upscaled_image.save("out_upscale.png")
-    print("Upscaled image saved as out_upscale.png")
+
+    # Save the upscaled image with the timestamp as the filename
+    upscaled_image.save(f"out_upscale_{timestamp}.png")
+    print("Upscaled image saved as out_upscale_{timestamp}.png")
+
     # Display the upscaled image
-    upscaled_image.show()
+    upscaled_image.show()
```

## Comparing `Kurdish2Image-0.0.1.dist-info/METADATA` & `Kurdish2Image-0.0.2.dist-info/METADATA`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: Kurdish2Image
-Version: 0.0.1
-Summary: Create Images from Text Based On Stable Diffusion Model
+Version: 0.0.2
+Summary: Create Kurdish style images from Text Based On Stable Diffusion Model
 Home-page: https://github.com/falahgs/
 Author: Falahgs.G.Saleih
 Author-email: falahgs07@gmail.com
 License: MIT
 Keywords: StableDiffusion,CLIP,Transformers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -13,26 +13,28 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: License.txt
 Requires-Dist: transformers
 Requires-Dist: diffusion
 Requires-Dist: diffusers
 Requires-Dist: torch
+Requires-Dist: accelerate
 
-# Kurdish2Images
-This is a Python package for easy Create Short Story from image captions using blip models by getting image captions.
- to get some information for any artworks, portraits, any images, and convert image captions to short stories using GPT-3 models
+# Kurdish2Images Package
+This is a Python package for easily Creating beautiful stunning images from any text about Kurdish style fashion.
+ based stable diffusion model.
+ to get some images any Kurdish style and portraits, any images, in easy code line a few code line 
  
 ## Installation
 
 ```
-pip install Image2Story==0.0.6
+pip install Kurdish2Image
 
 or in colab google cloud
-!pip install Image2Story==0.0.6
+!pip install Kurdish2Image
 
 
 ```
 
 ## Tutorial
 [Colab Google Drive](https://colab.research.google.com/drive/1ZR0cfKkOHvFi7E4IchLdc2S3JP83kvEp?usp=sharing)
 ```
```

