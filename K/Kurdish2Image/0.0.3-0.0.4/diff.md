# Comparing `tmp/Kurdish2Image-0.0.3-py2.py3-none-any.whl.zip` & `tmp/Kurdish2Image-0.0.4-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,7 @@
-Zip file size: 3854 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-04 06:43 kurdish2image/__init__.py
--rw-rw-rw-  2.0 fat     1148 b- defN 23-Jun-04 07:26 kurdish2image/kurdish2image.py
--rw-rw-rw-  2.0 fat      115 b- defN 23-Jun-04 07:17 kurdish2image/my-test.py
--rw-rw-rw-  2.0 fat     1085 b- defN 23-Jun-04 08:34 Kurdish2Image-0.0.3.dist-info/License.txt
--rw-rw-rw-  2.0 fat     2016 b- defN 23-Jun-04 08:34 Kurdish2Image-0.0.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Jun-04 08:34 Kurdish2Image-0.0.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       14 b- defN 23-Jun-04 08:34 Kurdish2Image-0.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      667 b- defN 23-Jun-04 08:34 Kurdish2Image-0.0.3.dist-info/RECORD
-8 files, 5155 bytes uncompressed, 2680 bytes compressed:  48.0%
+Zip file size: 2756 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat     1085 b- defN 23-Jun-04 08:36 Kurdish2Image-0.0.4.dist-info/License.txt
+-rw-rw-rw-  2.0 fat     2018 b- defN 23-Jun-04 08:36 Kurdish2Image-0.0.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Jun-04 08:36 Kurdish2Image-0.0.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        1 b- defN 23-Jun-04 08:36 Kurdish2Image-0.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      420 b- defN 23-Jun-04 08:36 Kurdish2Image-0.0.4.dist-info/RECORD
+5 files, 3634 bytes uncompressed, 1968 bytes compressed:  45.8%
```

## zipnote {}

```diff
@@ -1,25 +1,16 @@
-Filename: kurdish2image/__init__.py
+Filename: Kurdish2Image-0.0.4.dist-info/License.txt
 Comment: 
 
-Filename: kurdish2image/kurdish2image.py
+Filename: Kurdish2Image-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: kurdish2image/my-test.py
+Filename: Kurdish2Image-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: Kurdish2Image-0.0.3.dist-info/License.txt
+Filename: Kurdish2Image-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: Kurdish2Image-0.0.3.dist-info/METADATA
-Comment: 
-
-Filename: Kurdish2Image-0.0.3.dist-info/WHEEL
-Comment: 
-
-Filename: Kurdish2Image-0.0.3.dist-info/top_level.txt
-Comment: 
-
-Filename: Kurdish2Image-0.0.3.dist-info/RECORD
+Filename: Kurdish2Image-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `Kurdish2Image-0.0.3.dist-info/License.txt` & `Kurdish2Image-0.0.4.dist-info/License.txt`

 * *Files identical despite different names*

## Comparing `Kurdish2Image-0.0.3.dist-info/METADATA` & `Kurdish2Image-0.0.4.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Kurdish2Image
-Version: 0.0.3
+Version: 0.0.4
 Summary: Create Kurdish style images from Text Based On Stable Diffusion Model
 Home-page: https://github.com/falahgs/
 Author: Falahgs.G.Saleih
 Author-email: falahgs07@gmail.com
 License: MIT
 Keywords: StableDiffusion,CLIP,Transformers
 Classifier: Programming Language :: Python :: 3
@@ -37,20 +37,20 @@
 
 ## Tutorial
 [Colab Google Drive](https://colab.research.google.com/drive/18QelFQqUgfqTq-jqfGuEPRpGv9hApU8b?usp=sharing)
 ```
 u can see tutorial in colab google drive
 
 ```
-## exampl
+## example
 ```
 from kurdish2image import kurdish2image as k2i
 prompt="full body shot center of view a old woman 50 years, color decorative, Hyperrealistic neo-rococo solar punk aesthetic , embroidery, leather, highly detailed photography art masterpiece, smooth cam de Leon eric zener dramatic pearlescent soft light, ground angle hd 8 k, sharp focus, full body, colors decorative kurdish-fashion style, American shot"
 k2i.k2img(prompt)
 
 ```
-##result images out 
+## Result images out 
 
 ![](https://huggingface.co/datasets/Falah/kurdish-images/blob/main/1.png)
 ![](https://huggingface.co/datasets/Falah/kurdish-images/blob/main/3.png)
 ![](https://huggingface.co/datasets/Falah/kurdish-images/blob/main/5.png)
 ![](https://huggingface.co/datasets/Falah/kurdish-images/blob/main/7.png)
```

