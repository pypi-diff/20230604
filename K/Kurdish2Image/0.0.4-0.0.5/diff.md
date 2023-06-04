# Comparing `tmp/Kurdish2Image-0.0.4-py2.py3-none-any.whl.zip` & `tmp/Kurdish2Image-0.0.5-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,10 @@
-Zip file size: 2756 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat     1085 b- defN 23-Jun-04 08:36 Kurdish2Image-0.0.4.dist-info/License.txt
--rw-rw-rw-  2.0 fat     2018 b- defN 23-Jun-04 08:36 Kurdish2Image-0.0.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Jun-04 08:36 Kurdish2Image-0.0.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        1 b- defN 23-Jun-04 08:36 Kurdish2Image-0.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      420 b- defN 23-Jun-04 08:36 Kurdish2Image-0.0.4.dist-info/RECORD
-5 files, 3634 bytes uncompressed, 1968 bytes compressed:  45.8%
+Zip file size: 3865 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-04 06:43 kurdish2image/__init__.py
+-rw-rw-rw-  2.0 fat     1148 b- defN 23-Jun-04 07:26 kurdish2image/kurdish2image.py
+-rw-rw-rw-  2.0 fat      115 b- defN 23-Jun-04 07:17 kurdish2image/my-test.py
+-rw-rw-rw-  2.0 fat     1085 b- defN 23-Jun-04 08:42 Kurdish2Image-0.0.5.dist-info/License.txt
+-rw-rw-rw-  2.0 fat     2024 b- defN 23-Jun-04 08:42 Kurdish2Image-0.0.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Jun-04 08:42 Kurdish2Image-0.0.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       14 b- defN 23-Jun-04 08:42 Kurdish2Image-0.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      667 b- defN 23-Jun-04 08:42 Kurdish2Image-0.0.5.dist-info/RECORD
+8 files, 5163 bytes uncompressed, 2691 bytes compressed:  47.9%
```

## zipnote {}

```diff
@@ -1,16 +1,25 @@
-Filename: Kurdish2Image-0.0.4.dist-info/License.txt
+Filename: kurdish2image/__init__.py
 Comment: 
 
-Filename: Kurdish2Image-0.0.4.dist-info/METADATA
+Filename: kurdish2image/kurdish2image.py
 Comment: 
 
-Filename: Kurdish2Image-0.0.4.dist-info/WHEEL
+Filename: kurdish2image/my-test.py
 Comment: 
 
-Filename: Kurdish2Image-0.0.4.dist-info/top_level.txt
+Filename: Kurdish2Image-0.0.5.dist-info/License.txt
 Comment: 
 
-Filename: Kurdish2Image-0.0.4.dist-info/RECORD
+Filename: Kurdish2Image-0.0.5.dist-info/METADATA
+Comment: 
+
+Filename: Kurdish2Image-0.0.5.dist-info/WHEEL
+Comment: 
+
+Filename: Kurdish2Image-0.0.5.dist-info/top_level.txt
+Comment: 
+
+Filename: Kurdish2Image-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `Kurdish2Image-0.0.4.dist-info/License.txt` & `Kurdish2Image-0.0.5.dist-info/License.txt`

 * *Files identical despite different names*

## Comparing `Kurdish2Image-0.0.4.dist-info/METADATA` & `Kurdish2Image-0.0.5.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Kurdish2Image
-Version: 0.0.4
+Version: 0.0.5
 Summary: Create Kurdish style images from Text Based On Stable Diffusion Model
 Home-page: https://github.com/falahgs/
 Author: Falahgs.G.Saleih
 Author-email: falahgs07@gmail.com
 License: MIT
 Keywords: StableDiffusion,CLIP,Transformers
 Classifier: Programming Language :: Python :: 3
@@ -46,11 +46,12 @@
 from kurdish2image import kurdish2image as k2i
 prompt="full body shot center of view a old woman 50 years, color decorative, Hyperrealistic neo-rococo solar punk aesthetic , embroidery, leather, highly detailed photography art masterpiece, smooth cam de Leon eric zener dramatic pearlescent soft light, ground angle hd 8 k, sharp focus, full body, colors decorative kurdish-fashion style, American shot"
 k2i.k2img(prompt)
 
 ```
 ## Result images out 
 
-![](https://huggingface.co/datasets/Falah/kurdish-images/blob/main/1.png)
-![](https://huggingface.co/datasets/Falah/kurdish-images/blob/main/3.png)
-![](https://huggingface.co/datasets/Falah/kurdish-images/blob/main/5.png)
-![](https://huggingface.co/datasets/Falah/kurdish-images/blob/main/7.png)
+![1](https://huggingface.co/datasets/Falah/kurdish-images/blob/main/1.png)
+![2](https://huggingface.co/datasets/Falah/kurdish-images/blob/main/3.png)
+![3](https://huggingface.co/datasets/Falah/kurdish-images/blob/main/5.png)
+![4](https://huggingface.co/datasets/Falah/kurdish-images/blob/main/7.png)
+
```

