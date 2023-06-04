# Comparing `tmp/NanoRepeat-1.5.tar.gz` & `tmp/NanoRepeat-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NanoRepeat-1.5.tar", last modified: Mon May 22 06:20:17 2023, max compression
+gzip compressed data, was "NanoRepeat-1.6.tar", last modified: Sun Jun  4 11:28:52 2023, max compression
```

## Comparing `NanoRepeat-1.5.tar` & `NanoRepeat-1.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 fangli    (1002) fangli    (1002)        0 2023-05-22 06:20:17.450181 NanoRepeat-1.5/
--rw-rw-r--   0 fangli    (1002) fangli    (1002)     1097 2023-05-11 08:33:58.000000 NanoRepeat-1.5/LICENSE
--rw-rw-r--   0 fangli    (1002) fangli    (1002)    16291 2023-05-22 06:20:17.450181 NanoRepeat-1.5/PKG-INFO
--rw-rw-r--   0 fangli    (1002) fangli    (1002)    15958 2023-05-17 14:33:11.000000 NanoRepeat-1.5/README.md
--rw-rw-r--   0 fangli    (1002) fangli    (1002)       38 2023-05-22 06:20:17.450181 NanoRepeat-1.5/setup.cfg
--rw-rw-r--   0 fangli    (1002) fangli    (1002)      801 2023-05-22 01:47:21.000000 NanoRepeat-1.5/setup.py
-drwxrwxr-x   0 fangli    (1002) fangli    (1002)        0 2023-05-22 06:20:17.446181 NanoRepeat-1.5/src/
-drwxrwxr-x   0 fangli    (1002) fangli    (1002)        0 2023-05-22 06:20:17.450181 NanoRepeat-1.5/src/NanoRepeat/
--rw-rw-r--   0 fangli    (1002) fangli    (1002)      186 2023-05-11 08:33:58.000000 NanoRepeat-1.5/src/NanoRepeat/__init__.py
--rwxrwxr-x   0 fangli    (1002) fangli    (1002)    36432 2023-05-13 06:07:32.000000 NanoRepeat-1.5/src/NanoRepeat/nanoRepeat-joint.py
--rwxrwxr-x   0 fangli    (1002) fangli    (1002)    10989 2023-05-22 01:41:48.000000 NanoRepeat-1.5/src/NanoRepeat/nanoRepeat.py
--rw-rw-r--   0 fangli    (1002) fangli    (1002)    30089 2023-05-17 13:59:27.000000 NanoRepeat-1.5/src/NanoRepeat/nanoRepeat_bam.py
--rw-rw-r--   0 fangli    (1002) fangli    (1002)     3078 2023-05-13 06:08:14.000000 NanoRepeat-1.5/src/NanoRepeat/paf.py
--rw-rw-r--   0 fangli    (1002) fangli    (1002)     4446 2023-05-13 06:08:18.000000 NanoRepeat-1.5/src/NanoRepeat/repeat_region.py
--rw-rw-r--   0 fangli    (1002) fangli    (1002)    31135 2023-05-14 07:24:25.000000 NanoRepeat-1.5/src/NanoRepeat/split_alleles.py
--rw-rw-r--   0 fangli    (1002) fangli    (1002)    16195 2023-05-17 13:58:21.000000 NanoRepeat-1.5/src/NanoRepeat/tk.py
-drwxrwxr-x   0 fangli    (1002) fangli    (1002)        0 2023-05-22 06:20:17.450181 NanoRepeat-1.5/src/NanoRepeat.egg-info/
--rw-rw-r--   0 fangli    (1002) fangli    (1002)    16291 2023-05-22 06:20:17.000000 NanoRepeat-1.5/src/NanoRepeat.egg-info/PKG-INFO
--rw-rw-r--   0 fangli    (1002) fangli    (1002)      446 2023-05-22 06:20:17.000000 NanoRepeat-1.5/src/NanoRepeat.egg-info/SOURCES.txt
--rw-rw-r--   0 fangli    (1002) fangli    (1002)        1 2023-05-22 06:20:17.000000 NanoRepeat-1.5/src/NanoRepeat.egg-info/dependency_links.txt
--rw-rw-r--   0 fangli    (1002) fangli    (1002)       53 2023-05-22 06:20:17.000000 NanoRepeat-1.5/src/NanoRepeat.egg-info/requires.txt
--rw-rw-r--   0 fangli    (1002) fangli    (1002)       11 2023-05-22 06:20:17.000000 NanoRepeat-1.5/src/NanoRepeat.egg-info/top_level.txt
+drwxrwxr-x   0 fangli    (1002) fangli    (1002)        0 2023-06-04 11:28:52.334905 NanoRepeat-1.6/
+-rw-rw-r--   0 fangli    (1002) fangli    (1002)     1097 2023-05-11 08:33:58.000000 NanoRepeat-1.6/LICENSE
+-rw-rw-r--   0 fangli    (1002) fangli    (1002)    16291 2023-06-04 11:28:52.334905 NanoRepeat-1.6/PKG-INFO
+-rw-rw-r--   0 fangli    (1002) fangli    (1002)    15958 2023-05-17 14:33:11.000000 NanoRepeat-1.6/README.md
+-rw-rw-r--   0 fangli    (1002) fangli    (1002)       38 2023-06-04 11:28:52.334905 NanoRepeat-1.6/setup.cfg
+-rw-rw-r--   0 fangli    (1002) fangli    (1002)      801 2023-06-04 10:48:01.000000 NanoRepeat-1.6/setup.py
+drwxrwxr-x   0 fangli    (1002) fangli    (1002)        0 2023-06-04 11:28:52.330905 NanoRepeat-1.6/src/
+drwxrwxr-x   0 fangli    (1002) fangli    (1002)        0 2023-06-04 11:28:52.330905 NanoRepeat-1.6/src/NanoRepeat/
+-rw-rw-r--   0 fangli    (1002) fangli    (1002)      186 2023-05-11 08:33:58.000000 NanoRepeat-1.6/src/NanoRepeat/__init__.py
+-rwxrwxr-x   0 fangli    (1002) fangli    (1002)    36432 2023-05-13 06:07:32.000000 NanoRepeat-1.6/src/NanoRepeat/nanoRepeat-joint.py
+-rwxrwxr-x   0 fangli    (1002) fangli    (1002)    10989 2023-05-22 01:41:48.000000 NanoRepeat-1.6/src/NanoRepeat/nanoRepeat.py
+-rw-rw-r--   0 fangli    (1002) fangli    (1002)    32046 2023-06-04 10:45:36.000000 NanoRepeat-1.6/src/NanoRepeat/nanoRepeat_bam.py
+-rw-rw-r--   0 fangli    (1002) fangli    (1002)     3078 2023-05-13 06:08:14.000000 NanoRepeat-1.6/src/NanoRepeat/paf.py
+-rw-rw-r--   0 fangli    (1002) fangli    (1002)     4487 2023-06-03 08:25:19.000000 NanoRepeat-1.6/src/NanoRepeat/repeat_region.py
+-rw-rw-r--   0 fangli    (1002) fangli    (1002)    31135 2023-05-14 07:24:25.000000 NanoRepeat-1.6/src/NanoRepeat/split_alleles.py
+-rw-rw-r--   0 fangli    (1002) fangli    (1002)    16195 2023-05-17 13:58:21.000000 NanoRepeat-1.6/src/NanoRepeat/tk.py
+drwxrwxr-x   0 fangli    (1002) fangli    (1002)        0 2023-06-04 11:28:52.334905 NanoRepeat-1.6/src/NanoRepeat.egg-info/
+-rw-rw-r--   0 fangli    (1002) fangli    (1002)    16291 2023-06-04 11:28:52.000000 NanoRepeat-1.6/src/NanoRepeat.egg-info/PKG-INFO
+-rw-rw-r--   0 fangli    (1002) fangli    (1002)      446 2023-06-04 11:28:52.000000 NanoRepeat-1.6/src/NanoRepeat.egg-info/SOURCES.txt
+-rw-rw-r--   0 fangli    (1002) fangli    (1002)        1 2023-06-04 11:28:52.000000 NanoRepeat-1.6/src/NanoRepeat.egg-info/dependency_links.txt
+-rw-rw-r--   0 fangli    (1002) fangli    (1002)       53 2023-06-04 11:28:52.000000 NanoRepeat-1.6/src/NanoRepeat.egg-info/requires.txt
+-rw-rw-r--   0 fangli    (1002) fangli    (1002)       11 2023-06-04 11:28:52.000000 NanoRepeat-1.6/src/NanoRepeat.egg-info/top_level.txt
```

### Comparing `NanoRepeat-1.5/LICENSE` & `NanoRepeat-1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `NanoRepeat-1.5/PKG-INFO` & `NanoRepeat-1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NanoRepeat
-Version: 1.5
+Version: 1.6
 Summary: NanoRepeat: quantification of Short Tandem Repeats (STRs) from long-read sequencing data
 Home-page: https://github.com/WGLab/NanoRepeat
 Author: Li Fang, Kai Wang
 Author-email: fangli9@sysu.edu.cn
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `NanoRepeat-1.5/README.md` & `NanoRepeat-1.6/README.md`

 * *Files identical despite different names*

### Comparing `NanoRepeat-1.5/setup.py` & `NanoRepeat-1.6/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as f:
     readme = f.read()
     
 setup(
     name='NanoRepeat',
-    version='1.5',
+    version='1.6',
     description='NanoRepeat: quantification of Short Tandem Repeats (STRs) from long-read sequencing data',
     long_description = readme,
     long_description_content_type = 'text/markdown',
     url='https://github.com/WGLab/NanoRepeat',
     author='Li Fang, Kai Wang',
     author_email='fangli9@sysu.edu.cn',
     license='MIT',
```

### Comparing `NanoRepeat-1.5/src/NanoRepeat/nanoRepeat-joint.py` & `NanoRepeat-1.6/src/NanoRepeat/nanoRepeat-joint.py`

 * *Files identical despite different names*

### Comparing `NanoRepeat-1.5/src/NanoRepeat/nanoRepeat.py` & `NanoRepeat-1.6/src/NanoRepeat/nanoRepeat.py`

 * *Files identical despite different names*

### Comparing `NanoRepeat-1.5/src/NanoRepeat/nanoRepeat_bam.py` & `NanoRepeat-1.6/src/NanoRepeat/nanoRepeat_bam.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,16 +27,15 @@
 '''
 
 import os
 import string
 import sys
 import shutil
 import numpy as np
-from sklearn.mixture import GaussianMixture
-
+from multiprocessing import Process
 from typing import List
 
 from NanoRepeat import tk
 from NanoRepeat.repeat_region import *
 from NanoRepeat.paf import *
 from NanoRepeat.split_alleles import *
 
@@ -387,14 +386,15 @@
         if read_name not in repeat_region.read_dict: continue
         read_sequence = line2.strip()            
         if repeat_region.read_dict[read_name].strand == '-':
             read_sequence = tk.rev_comp(read_sequence)
         core_sequence = read_sequence[repeat_region.read_dict[read_name].core_seq_start_pos:repeat_region.read_dict[read_name].core_seq_end_pos]
         mid_sequence = read_sequence[repeat_region.read_dict[read_name].mid_seq_start_pos:repeat_region.read_dict[read_name].mid_seq_end_pos]
 
+        repeat_region.read_core_seq_dict[read_name] = core_sequence
         core_seq_fq_f.write(line1)
         core_seq_fq_f.write(core_sequence + '\n')
         core_seq_fq_f.write(line3)
         core_seq_fq_f.write('0' * len(core_sequence) + '\n')
 
 
         mid_seq_fq_f.write(line1)
@@ -437,21 +437,40 @@
     preset = tk.get_preset_for_minimap2(data_type)
     cmd = f'{minimap2} -c -t {num_cpu} {preset} -f 0.0 {round1_fasta_file} {repeat_region.core_seq_fq_file} > {round1_paf_file}'
     tk.run_system_cmd(cmd)
     round1_paf_f = open(round1_paf_file, 'r')
     lines = list(round1_paf_f)
     round1_paf_f.close()
 
+
+    round2_repeat_size_dict = dict()
+    
     for line in lines:
         col_list = line.strip().split('\t')
         paf = PAF(col_list)
+
         if paf.tstart <= len(repeat_region.left_anchor_seq) and paf.tend >= len(repeat_region.left_anchor_seq):
             read_name = paf.qname
             round2_repeat_size = float(paf.tend - len(repeat_region.left_anchor_seq))/len(repeat_region.repeat_unit_seq)
-            repeat_region.read_dict[read_name].round2_repeat_size = round2_repeat_size
+            align_score = paf.align_score
+            if read_name not in round2_repeat_size_dict:
+                round2_repeat_size_dict[read_name] = []
+            round2_repeat_size_dict[read_name].append((align_score, round2_repeat_size))
+            
+    for read_name in round2_repeat_size_dict:
+        round2_repeat_size_dict[read_name].sort(key = lambda x:x[0], reverse=True)
+        round2_repeat_size = round2_repeat_size_dict[read_name][0][1]
+        repeat_region.read_dict[read_name].round2_repeat_size = round2_repeat_size
+
+    round2_repeat_size_file = os.path.join(repeat_region.temp_out_dir, 'round2_repeat_size.txt')
+    round2_repeat_size_f = open(round2_repeat_size_file, 'w')
+    for read_name in repeat_region.read_dict:
+        round2_repeat_size_f.write(f'{read_name}\t{repeat_region.read_dict[read_name].round2_repeat_size}\n')
+    
+    round2_repeat_size_f.close()
     
     return
 
 def get_max_read_length_from_fastq(fq_file):
 
     max_read_length = 0
     fq_f = open(fq_file, 'r')
@@ -501,51 +520,82 @@
             read_paf_list.clear()
             read_paf_list.append(paf)
 
     round3_estimation_for1read(repeat_region, read_paf_list)
     
     return 
 
-def round3_estimation(minimap2:string, data_type, repeat_region:RepeatRegion, num_cpu:int):
+def round3_estimation(minimap2:string, data_type:string, repeat_region:RepeatRegion, num_cpu:int):
     
-    estimated_repeat_size_list = []
-    for read_name in repeat_region.read_dict:
-        read = repeat_region.read_dict[read_name]
-        if read.round2_repeat_size != None:
-            estimated_repeat_size_list.append(read.round2_repeat_size)
-    if len(estimated_repeat_size_list) == 0: return
-    max_template_repeat_size = int(max(estimated_repeat_size_list) * 1.5) + 1
-    min_template_repeat_size = int(min(estimated_repeat_size_list) / 2)
-
-    if min_template_repeat_size > min(estimated_repeat_size_list) - 10:
-        min_template_repeat_size = int(min(estimated_repeat_size_list) - 10)
-    if max_template_repeat_size < max(estimated_repeat_size_list) + 10:
-        max_template_repeat_size = int(max(estimated_repeat_size_list) + 10) + 1
+    round3_paf_file = os.path.join(repeat_region.temp_out_dir, 'round3.paf')
+    round3_paf_f = open(round3_paf_file, 'w')
+    round3_paf_f.close()
     
-    if min_template_repeat_size < 0: min_template_repeat_size = 0
+    procs = []
+
+    for proc_id in range(0, num_cpu):
+        proc = Process(target=round3_align_1process, args=(proc_id, num_cpu, repeat_region, data_type, minimap2))
+        procs.append(proc)
+        proc.start()
+        
+    for proc_id in range(0, num_cpu):
+        procs[proc_id].join()
+        proc_out_paf_file = os.path.join(repeat_region.temp_out_dir, f'round3_align.process{proc_id}.paf')
+        cmd = f'cat {proc_out_paf_file} >> {round3_paf_file}'
+        tk.run_system_cmd(cmd)
+        os.remove(proc_out_paf_file)
     
-    template_fasta_file  = os.path.join(repeat_region.temp_out_dir, 'round3_ref.fasta')
-    repeat_region.temp_file_list.append(template_fasta_file)
-    template_fasta_fp    = open(template_fasta_file, 'w')
-    for repeat_size in range(min_template_repeat_size, max_template_repeat_size+1):
-        template_seq = repeat_region.left_anchor_seq + repeat_region.repeat_unit_seq * repeat_size + repeat_region.right_anchor_seq
-        template_fasta_fp.write('>%s\n' % repeat_size)
-        template_fasta_fp.write('%s\n' % template_seq)
+    round3_estimation_from_paf(repeat_region, round3_paf_file)
 
-    template_fasta_fp.close()
+def round3_align_1process(proc_id:int, num_cpu:int, repeat_region:RepeatRegion, data_type:string, minimap2:string):
+    
+    read_id = -1
+    out_paf_file = os.path.join(repeat_region.temp_out_dir, f'round3_align.process{proc_id}.paf')
+    out_paf_f = open(out_paf_file, 'w')
+    out_paf_f.close()
+    
+    for read_name in repeat_region.read_dict:
+        read = repeat_region.read_dict[read_name]
+        round2_repeat_size = read.round2_repeat_size
+        if round2_repeat_size == None: continue
+        read_id += 1
+        if read_id % num_cpu != proc_id: continue
+        
+        buffer = max(15, int(round2_repeat_size * 0.05))
+        if buffer > 150: buffer = 150
+        
+        max_template_repeat_size = int(round2_repeat_size + buffer)
+        min_template_repeat_size = int(round2_repeat_size - buffer)
+        
+        if min_template_repeat_size < 0: min_template_repeat_size = 0
+        
+        template_fasta_file  = os.path.join(repeat_region.temp_out_dir, f'round3_reference.read{read_id}.fasta')
+        template_fasta_fp    = open(template_fasta_file, 'w')
+        for repeat_size in range(min_template_repeat_size, max_template_repeat_size+1):
+            template_seq = repeat_region.left_anchor_seq + repeat_region.repeat_unit_seq * repeat_size + repeat_region.right_anchor_seq
+            template_fasta_fp.write('>%s\n' % repeat_size)
+            template_fasta_fp.write('%s\n' % template_seq)
 
-    round3_paf_file = os.path.join(repeat_region.temp_out_dir, 'round3.paf')
-    repeat_region.temp_file_list.append(round3_paf_file)
+        template_fasta_fp.close()
+        
+        read_seq = repeat_region.read_core_seq_dict[read_name].strip()
+        read_fasta_file = os.path.join(repeat_region.temp_out_dir, f'round3_input.read{read_id}.fasta')
+        
+        read_fasta_f = open(read_fasta_file, 'w')
+        read_fasta_f.write(f'>{read_name}\n')
+        read_fasta_f.write(read_seq + '\n')
+        read_fasta_f.close()
+
+        preset = tk.get_preset_for_minimap2(data_type)
+        cmd = f'{minimap2} {preset} -f 0.0 -N 100 -c --eqx -t 1 {template_fasta_file} {read_fasta_file} >> {out_paf_file}'
+        tk.run_system_cmd(cmd)
 
-    preset = tk.get_preset_for_minimap2(data_type)
-    cmd = f'{minimap2} {preset} -f 0.0 -N 100 -c --eqx -t {num_cpu} {template_fasta_file} {repeat_region.core_seq_fq_file} > {round3_paf_file}'
-    tk.run_system_cmd(cmd)
+        os.remove(template_fasta_file)
+        os.remove(read_fasta_file)
 
-    round3_estimation_from_paf(repeat_region, round3_paf_file)
-    
     return
 
 def remove_noisy_reads_1d(allele_list, ploidy):
 
     tk.eprint('NOTICE: Trying to remove noisy reads')
     allele_list.sort(key = lambda allele:allele.num_reads)
     num_removed_reads = 0
```

### Comparing `NanoRepeat-1.5/src/NanoRepeat/paf.py` & `NanoRepeat-1.6/src/NanoRepeat/paf.py`

 * *Files identical despite different names*

### Comparing `NanoRepeat-1.5/src/NanoRepeat/repeat_region.py` & `NanoRepeat-1.6/src/NanoRepeat/repeat_region.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,14 +77,15 @@
         self.temp_out_dir = None
         self.final_out_dir = None
         self.out_prefix = None
 
         self.temp_file_list = []
         self.ref_has_issue = False
         self.read_dict = dict()
+        self.read_core_seq_dict = dict()
         self.buffer_len = None
         self.brute_force_repeat_count_dict = dict()
         
     
         if line != None:
             col_list = line.strip().split('\t')
             if len(col_list) < 4:
```

### Comparing `NanoRepeat-1.5/src/NanoRepeat/split_alleles.py` & `NanoRepeat-1.6/src/NanoRepeat/split_alleles.py`

 * *Files identical despite different names*

### Comparing `NanoRepeat-1.5/src/NanoRepeat/tk.py` & `NanoRepeat-1.6/src/NanoRepeat/tk.py`

 * *Files identical despite different names*

### Comparing `NanoRepeat-1.5/src/NanoRepeat.egg-info/PKG-INFO` & `NanoRepeat-1.6/src/NanoRepeat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NanoRepeat
-Version: 1.5
+Version: 1.6
 Summary: NanoRepeat: quantification of Short Tandem Repeats (STRs) from long-read sequencing data
 Home-page: https://github.com/WGLab/NanoRepeat
 Author: Li Fang, Kai Wang
 Author-email: fangli9@sysu.edu.cn
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

