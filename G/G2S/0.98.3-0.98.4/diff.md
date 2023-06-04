# Comparing `tmp/G2S-0.98.3-cp39-cp39-win_amd64.whl.zip` & `tmp/G2S-0.98.4-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 323639 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat   516096 b- defN 22-May-21 22:16 G2S-0.98.3.data/data/lib/site-packages/g2s/libzmq-v143-mt-4_3_5.dll
--rw-rw-rw-  2.0 fat      408 b- defN 22-May-21 22:12 g2s/__init__.py
--rw-rw-rw-  2.0 fat   193024 b- defN 22-May-21 22:18 g2s/g2s.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat      884 b- defN 22-May-21 22:18 G2S-0.98.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 22-May-21 22:18 G2S-0.98.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        4 b- defN 22-May-21 22:18 G2S-0.98.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      567 b- defN 22-May-21 22:18 G2S-0.98.3.dist-info/RECORD
-7 files, 711083 bytes uncompressed, 322637 bytes compressed:  54.6%
+Zip file size: 323645 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat   516096 b- defN 22-May-22 18:18 G2S-0.98.4.data/data/lib/site-packages/g2s/libzmq-v143-mt-4_3_5.dll
+-rw-rw-rw-  2.0 fat      408 b- defN 22-May-22 18:16 g2s/__init__.py
+-rw-rw-rw-  2.0 fat   193024 b- defN 22-May-22 18:21 g2s/g2s.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat      884 b- defN 22-May-22 18:21 G2S-0.98.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 22-May-22 18:21 G2S-0.98.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        4 b- defN 22-May-22 18:21 G2S-0.98.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      567 b- defN 22-May-22 18:21 G2S-0.98.4.dist-info/RECORD
+7 files, 711083 bytes uncompressed, 322643 bytes compressed:  54.6%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
-Filename: G2S-0.98.3.data/data/lib/site-packages/g2s/libzmq-v143-mt-4_3_5.dll
+Filename: G2S-0.98.4.data/data/lib/site-packages/g2s/libzmq-v143-mt-4_3_5.dll
 Comment: 
 
 Filename: g2s/__init__.py
 Comment: 
 
 Filename: g2s/g2s.cp39-win_amd64.pyd
 Comment: 
 
-Filename: G2S-0.98.3.dist-info/METADATA
+Filename: G2S-0.98.4.dist-info/METADATA
 Comment: 
 
-Filename: G2S-0.98.3.dist-info/WHEEL
+Filename: G2S-0.98.4.dist-info/WHEEL
 Comment: 
 
-Filename: G2S-0.98.3.dist-info/top_level.txt
+Filename: G2S-0.98.4.dist-info/top_level.txt
 Comment: 
 
-Filename: G2S-0.98.3.dist-info/RECORD
+Filename: G2S-0.98.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `G2S-0.98.3.data/data/lib/site-packages/g2s/libzmq-v143-mt-4_3_5.dll` & `G2S-0.98.4.data/data/lib/site-packages/g2s/libzmq-v143-mt-4_3_5.dll`

 * *Files 0% similar despite different names*

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018005c638
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sat May 21 22:16:22 2022
+Time/Date		Sun May 22 18:18:58 2022
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	32
 SizeOfCode		000000000005dc00
 SizeOfInitializedData	0000000000020600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000005c638
@@ -132729,15 +132729,15 @@
    180067daa:	add    $0x180,%eax
    180067daf:	add    %bl,(%rax)
    180067db1:	testb  $0x0,0x180(%rip)        # 0x180067f38
    180067db8:	and    %dh,%dh
    180067dba:	add    $0x180,%eax
    180067dbf:	add    %al,(%rax)
    180067dc1:	add    %al,(%rax)
-   180067dc3:	add    %dh,0x628964(%rsi)
+   180067dc3:	add    %dl,0x628a7e(%rdx)
    180067dc9:	add    %al,(%rax)
    180067dcb:	add    %cl,-0x20000000(%rip)        # 0x160067dd1
    180067dd1:	add    (%rax),%al
    180067dd3:	add    %bl,(%rbx,%rdx,8)
    180067dd6:	(bad)
    180067dd7:	add    %bl,(%rbx,%rax,8)
    180067dda:	(bad)
```

## Comparing `G2S-0.98.3.dist-info/METADATA` & `G2S-0.98.4.dist-info/METADATA`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: G2S
-Version: 0.98.3
+Version: 0.98.4
 Summary: G2S interface
 Home-page: https://github.com/GAIA-UNIL/G2S
 Author: Mathieu Gravey
 Author-email: g2s@mgravey.com
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

## Comparing `G2S-0.98.3.dist-info/RECORD` & `G2S-0.98.4.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-G2S-0.98.3.data/data/lib/site-packages/g2s/libzmq-v143-mt-4_3_5.dll,sha256=hxj9wcam_0doQY3Zzrcl649C3SnGSk4J8-l0zqELgSo,516096
+G2S-0.98.4.data/data/lib/site-packages/g2s/libzmq-v143-mt-4_3_5.dll,sha256=fUOlNyYnqZHP98Oh7Lo6IcQe08hdU1L5eYGsZFa0Qmk,516096
 g2s/__init__.py,sha256=iMRYaPEvxKlXgnSCv6hqIsf152af3LwDt8KcNQ6igv8,408
-g2s/g2s.cp39-win_amd64.pyd,sha256=S8YR5_o2yce4d0R2PxqQ9FIwPHE-xDcq8JRAY-ffj0g,193024
-G2S-0.98.3.dist-info/METADATA,sha256=3HDO4dYazLR8ZS2Vt44G6ztg1lt01bMtcf2LM6BUTG8,884
-G2S-0.98.3.dist-info/WHEEL,sha256=fVcVlLzi8CGi_Ul8vjMdn8gER25dn5GBg9E6k9z41-Y,100
-G2S-0.98.3.dist-info/top_level.txt,sha256=wMPe9gVwac8XL9aTGXp3V3Sc-UbgQKQ1kH6WmAhGBME,4
-G2S-0.98.3.dist-info/RECORD,,
+g2s/g2s.cp39-win_amd64.pyd,sha256=9p5VI5LsO3vWtaxi3WlWYo7RL68vQUgvAeSdEn72XMI,193024
+G2S-0.98.4.dist-info/METADATA,sha256=hz5KcO1Js5X3rMY46YIP744AUPTVrjHXkT7P09u9gys,884
+G2S-0.98.4.dist-info/WHEEL,sha256=fVcVlLzi8CGi_Ul8vjMdn8gER25dn5GBg9E6k9z41-Y,100
+G2S-0.98.4.dist-info/top_level.txt,sha256=wMPe9gVwac8XL9aTGXp3V3Sc-UbgQKQ1kH6WmAhGBME,4
+G2S-0.98.4.dist-info/RECORD,,
```

