# Comparing `tmp/Kurdish2Image-0.0.6-py2.py3-none-any.whl.zip` & `tmp/Kurdish2Image-0.0.7-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 3869 bytes, number of entries: 8
+Zip file size: 3848 bytes, number of entries: 8
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-04 06:43 kurdish2image/__init__.py
--rw-rw-rw-  2.0 fat     1148 b- defN 23-Jun-04 07:26 kurdish2image/kurdish2image.py
+-rw-rw-rw-  2.0 fat     1089 b- defN 23-Jun-04 08:54 kurdish2image/kurdish2image.py
 -rw-rw-rw-  2.0 fat      115 b- defN 23-Jun-04 07:17 kurdish2image/my-test.py
--rw-rw-rw-  2.0 fat     1085 b- defN 23-Jun-04 08:47 Kurdish2Image-0.0.6.dist-info/License.txt
--rw-rw-rw-  2.0 fat     2027 b- defN 23-Jun-04 08:47 Kurdish2Image-0.0.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Jun-04 08:47 Kurdish2Image-0.0.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       14 b- defN 23-Jun-04 08:47 Kurdish2Image-0.0.6.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      667 b- defN 23-Jun-04 08:47 Kurdish2Image-0.0.6.dist-info/RECORD
-8 files, 5166 bytes uncompressed, 2695 bytes compressed:  47.8%
+-rw-rw-rw-  2.0 fat     1085 b- defN 23-Jun-04 09:01 Kurdish2Image-0.0.7.dist-info/License.txt
+-rw-rw-rw-  2.0 fat     1976 b- defN 23-Jun-04 09:01 Kurdish2Image-0.0.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Jun-04 09:01 Kurdish2Image-0.0.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       14 b- defN 23-Jun-04 09:01 Kurdish2Image-0.0.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      667 b- defN 23-Jun-04 09:01 Kurdish2Image-0.0.7.dist-info/RECORD
+8 files, 5056 bytes uncompressed, 2674 bytes compressed:  47.1%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: kurdish2image/kurdish2image.py
 Comment: 
 
 Filename: kurdish2image/my-test.py
 Comment: 
 
-Filename: Kurdish2Image-0.0.6.dist-info/License.txt
+Filename: Kurdish2Image-0.0.7.dist-info/License.txt
 Comment: 
 
-Filename: Kurdish2Image-0.0.6.dist-info/METADATA
+Filename: Kurdish2Image-0.0.7.dist-info/METADATA
 Comment: 
 
-Filename: Kurdish2Image-0.0.6.dist-info/WHEEL
+Filename: Kurdish2Image-0.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: Kurdish2Image-0.0.6.dist-info/top_level.txt
+Filename: Kurdish2Image-0.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: Kurdish2Image-0.0.6.dist-info/RECORD
+Filename: Kurdish2Image-0.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kurdish2image/kurdish2image.py

```diff
@@ -5,30 +5,23 @@
 import time
 
 def k2img(prompt):
     model_id = "Falah/kurdish-fashion"
     scheduler = EulerDiscreteScheduler.from_pretrained(model_id, subfolder="scheduler")
     pipe = StableDiffusionPipeline.from_pretrained(model_id, scheduler=scheduler, torch_dtype=torch.float16)
     pipe = pipe.to("cuda")
-
     image = pipe(prompt).images[0]
-
     # Generate timestamp for the filename
     timestamp = time.strftime("%Y%m%d%H%M%S")
-
     # Save the image with the timestamp as the filename
     image.save(f"out_{timestamp}.png")
-    print("Image saved as out_{timestamp}.png")
-
+    print("Image saved ")
     # Display the image
     image.show()
-
     # Upscale the image to high resolution
-    upscale_transform = transforms.Resize((1920, 1080))
+    upscale_transform = transforms.Resize((1024, 1024))
     upscaled_image = upscale_transform(image)
-
     # Save the upscaled image with the timestamp as the filename
     upscaled_image.save(f"out_upscale_{timestamp}.png")
-    print("Upscaled image saved as out_upscale_{timestamp}.png")
-
+    print("Upscaled image saved ")
     # Display the upscaled image
     upscaled_image.show()
```

## Comparing `Kurdish2Image-0.0.6.dist-info/License.txt` & `Kurdish2Image-0.0.7.dist-info/License.txt`

 * *Files identical despite different names*

## Comparing `Kurdish2Image-0.0.6.dist-info/METADATA` & `Kurdish2Image-0.0.7.dist-info/METADATA`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Kurdish2Image
-Version: 0.0.6
+Version: 0.0.7
 Summary: Create Kurdish style images from Text Based On Stable Diffusion Model
 Home-page: https://github.com/falahgs/
 Author: Falahgs.G.Saleih
 Author-email: falahgs07@gmail.com
 License: MIT
 Keywords: StableDiffusion,CLIP,Transformers
 Classifier: Programming Language :: Python :: 3
@@ -46,12 +46,12 @@
 from kurdish2image import kurdish2image as k2i
 prompt="full body shot center of view a old woman 50 years, color decorative, Hyperrealistic neo-rococo solar punk aesthetic , embroidery, leather, highly detailed photography art masterpiece, smooth cam de Leon eric zener dramatic pearlescent soft light, ground angle hd 8 k, sharp focus, full body, colors decorative kurdish-fashion style, American shot"
 k2i.k2img(prompt)
 
 ```
 ## Result images out 
 
-![1](https://huggingface.co/datasets/Falah/kurdish-images/blob/resolve/1.png)
-![2](https://huggingface.co/datasets/Falah/kurdish-images/blob/main/3.png)
-![3](https://huggingface.co/datasets/Falah/kurdish-images/blob/main/5.png)
-![4](https://huggingface.co/datasets/Falah/kurdish-images/blob/main/7.png)
+![1](https://iraqprogrammer.files.wordpress.com/2023/06/1.png)
+![2](https://iraqprogrammer.files.wordpress.com/2023/06/3.png)
+![3](https://iraqprogrammer.files.wordpress.com/2023/06/5.png)
+![4](https://iraqprogrammer.files.wordpress.com/2023/06/7.png)
```

## Comparing `Kurdish2Image-0.0.6.dist-info/RECORD` & `Kurdish2Image-0.0.7.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 kurdish2image/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-kurdish2image/kurdish2image.py,sha256=K90MoK7ASp06rOUUxEPwwITGDgLlTppEpTtgnboFbCM,1148
+kurdish2image/kurdish2image.py,sha256=JJTn8esOD6Iep6shNhBDF-Agg6t4OgWAzkI_v9sWmwk,1089
 kurdish2image/my-test.py,sha256=3GUiN5VH0R9jZI-pTx5HS3TV898d27EfG5wGdbHhtIs,115
-Kurdish2Image-0.0.6.dist-info/License.txt,sha256=YgouLRpKUVhFH3iCbDxSlpLSl236jy1t-NxTegPbT5s,1085
-Kurdish2Image-0.0.6.dist-info/METADATA,sha256=bGwiLs8fFjY3YmrxZyFRURV1YjdfUTaEIMf9cKIWSwQ,2027
-Kurdish2Image-0.0.6.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-Kurdish2Image-0.0.6.dist-info/top_level.txt,sha256=aF5ig4CIkQxbwUPtTFygYtDe9_MMJ4dCJZiSWO4hFnI,14
-Kurdish2Image-0.0.6.dist-info/RECORD,,
+Kurdish2Image-0.0.7.dist-info/License.txt,sha256=YgouLRpKUVhFH3iCbDxSlpLSl236jy1t-NxTegPbT5s,1085
+Kurdish2Image-0.0.7.dist-info/METADATA,sha256=CgD3KcgYK5qX8WhWdxYREZ193Te0Jm2Whgfqa5Q9Sus,1976
+Kurdish2Image-0.0.7.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+Kurdish2Image-0.0.7.dist-info/top_level.txt,sha256=aF5ig4CIkQxbwUPtTFygYtDe9_MMJ4dCJZiSWO4hFnI,14
+Kurdish2Image-0.0.7.dist-info/RECORD,,
```

