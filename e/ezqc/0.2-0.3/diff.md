# Comparing `tmp/ezqc-0.2.tar.gz` & `tmp/ezqc-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezqc-0.2.tar", last modified: Wed May 31 23:17:18 2023, max compression
+gzip compressed data, was "ezqc-0.3.tar", last modified: Sun Jun  4 06:06:13 2023, max compression
```

## Comparing `ezqc-0.2.tar` & `ezqc-0.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:17:18.258254 ezqc-0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-31 23:17:08.000000 ezqc-0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-05-31 23:17:18.258254 ezqc-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-05-31 23:17:08.000000 ezqc-0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:17:18.258254 ezqc-0.2/ezqc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 23:17:08.000000 ezqc-0.2/ezqc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-31 23:17:08.000000 ezqc-0.2/ezqc/ac8.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-31 23:17:08.000000 ezqc-0.2/ezqc/blast.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-31 23:17:08.000000 ezqc-0.2/ezqc/color_print.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-05-31 23:17:08.000000 ezqc-0.2/ezqc/ezqc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-05-31 23:17:08.000000 ezqc-0.2/ezqc/os7.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-31 23:17:08.000000 ezqc-0.2/ezqc/pbnc5.py
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-05-31 23:17:08.000000 ezqc-0.2/ezqc/pbsc3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-05-31 23:17:08.000000 ezqc-0.2/ezqc/pbsq1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-05-31 23:17:08.000000 ezqc-0.2/ezqc/psgc4.py
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-05-31 23:17:08.000000 ezqc-0.2/ezqc/psqs2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-31 23:17:08.000000 ezqc-0.2/ezqc/sld6.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:17:18.258254 ezqc-0.2/ezqc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-05-31 23:17:18.000000 ezqc-0.2/ezqc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-31 23:17:18.000000 ezqc-0.2/ezqc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 23:17:18.000000 ezqc-0.2/ezqc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-31 23:17:18.000000 ezqc-0.2/ezqc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-31 23:17:18.000000 ezqc-0.2/ezqc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-31 23:17:18.000000 ezqc-0.2/ezqc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 23:17:18.258254 ezqc-0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-31 23:17:08.000000 ezqc-0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:17:18.258254 ezqc-0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-05-31 23:17:08.000000 ezqc-0.2/tests/test_ezqc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 06:06:13.304559 ezqc-0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-04 06:06:03.000000 ezqc-0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-06-04 06:06:13.304559 ezqc-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-06-04 06:06:03.000000 ezqc-0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 06:06:13.300559 ezqc-0.3/ezqc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 06:06:03.000000 ezqc-0.3/ezqc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-06-04 06:06:03.000000 ezqc-0.3/ezqc/ac8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-04 06:06:03.000000 ezqc-0.3/ezqc/blast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-04 06:06:03.000000 ezqc-0.3/ezqc/color_print.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-06-04 06:06:03.000000 ezqc-0.3/ezqc/ezqc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-06-04 06:06:03.000000 ezqc-0.3/ezqc/os7.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-06-04 06:06:03.000000 ezqc-0.3/ezqc/pbnc5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-06-04 06:06:03.000000 ezqc-0.3/ezqc/pbsc3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-06-04 06:06:03.000000 ezqc-0.3/ezqc/pbsq1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-06-04 06:06:03.000000 ezqc-0.3/ezqc/psgc4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-06-04 06:06:03.000000 ezqc-0.3/ezqc/psqs2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-04 06:06:03.000000 ezqc-0.3/ezqc/sld6.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 06:06:13.304559 ezqc-0.3/ezqc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-06-04 06:06:13.000000 ezqc-0.3/ezqc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-04 06:06:13.000000 ezqc-0.3/ezqc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 06:06:13.000000 ezqc-0.3/ezqc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-04 06:06:13.000000 ezqc-0.3/ezqc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-04 06:06:13.000000 ezqc-0.3/ezqc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-04 06:06:13.000000 ezqc-0.3/ezqc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 06:06:13.304559 ezqc-0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-04 06:06:03.000000 ezqc-0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 06:06:13.304559 ezqc-0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-06-04 06:06:03.000000 ezqc-0.3/tests/test_ezqc.py
```

### Comparing `ezqc-0.2/LICENSE` & `ezqc-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ezqc-0.2/PKG-INFO` & `ezqc-0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: ezqc
-Version: 0.2
+Version: 0.3
 Summary: EZQC is a streamlined, terminal-based alternative to FastQC.
 Author: Tinger Shi & Sky Li
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![EZQC Main Tests](https://github.com/skysky2333/EZQC/actions/workflows/ezqc_main_test.yml/badge.svg)](https://github.com/skysky2333/EZQC/actions/workflows/ezqc_main_test.yml)
-[![PyPI](https://github.com/skysky2333/EZQC/actions/workflows/python-publish.yml/badge.svg)](https://github.com/skysky2333/EZQC/actions/workflows/python-publish.yml)
+[![PyPI](https://img.shields.io/pypi/v/ezqc?color=blue)](https://pypi.org/project/ezqc/)
+
+
 
 # EZQC: Easy Quality Control for FastQ Files
 <p align="center">
   <img src="tests/test1.gif" alt="test Gif" width="100%">
 </p>
 
 ## Table of Contents
@@ -39,19 +41,24 @@
 7. Overrepresented sequences
 8. Adapter Content
 
 ## Quick Start Guide
 
 1. Install EZQC following [Installation guide](#installation).
 2. Run the tool on a toy example using the command `ezqc tests/SRR020182.fastq` (fastq file from [IGSR](https://www.internationalgenome.org/data-portal/sample/NA18486)).
-3. The results will be displayed in the terminal, and figures as well as csv tables will be saved to a directory named `ezqc_output` in your current working directory. Note that this file is choosen intendedly to fail multiple QC tests.
+3. The results will be displayed in the terminal, and figures as well as csv tables will be saved to a directory named `ezqc_output` in your current working directory. Note that this file is choosen intentionally to fail multiple QC tests.
 
 ## Installation
 
-You can install EZQC from source using the provided `setup.py` script. Here are the steps:
+You can install EZQC using pip:
+```
+pip install ezqc
+```
+
+Alternatively, you can compile the latest version of EZQC from source using the provided `setup.py` script. Following steps:
 
 1. Clone the repository:
 
 ```
 git clone https://github.com/skysky2333/ezqc
 ```
 
@@ -60,18 +67,18 @@
 ```
 cd ezqc
 ```
 
 3. Install the package:
 
 ```
-pip3 install .
+pip install .
 ```
 
-Or install directly:
+Or
 
 ```
 python setup.py install
 ```
 
 EZQC requires Python 3.x and depends on the following packages, which will be installed automatically during setup:
 
@@ -90,14 +97,15 @@
 ```
 
 Replace `<fastq file(s)>` with the path(s) to your FastQ files. If you want to analyze multiple files, separate the file paths with spaces:
 
 ```
 ezqc file1.fastq file2.fastq file3.fastq
 ```
+Use `-o` or `--output` to set the output directory.
 
 ## Analysis Methods
 
 Here's a brief description of the analyses performed by EZQC:
 
 1. **Per Base Sequence Quality**: Checks the quality of each base call in a sequence read.
 2. **Per Sequence Quality Scores**: Provides a histogram of quality scores over all sequences.
```

### Comparing `ezqc-0.2/README.md` & `ezqc-0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 [![EZQC Main Tests](https://github.com/skysky2333/EZQC/actions/workflows/ezqc_main_test.yml/badge.svg)](https://github.com/skysky2333/EZQC/actions/workflows/ezqc_main_test.yml)
-[![PyPI](https://github.com/skysky2333/EZQC/actions/workflows/python-publish.yml/badge.svg)](https://github.com/skysky2333/EZQC/actions/workflows/python-publish.yml)
+[![PyPI](https://img.shields.io/pypi/v/ezqc?color=blue)](https://pypi.org/project/ezqc/)
+
+
 
 # EZQC: Easy Quality Control for FastQ Files
 <p align="center">
   <img src="tests/test1.gif" alt="test Gif" width="100%">
 </p>
 
 ## Table of Contents
@@ -31,19 +33,24 @@
 7. Overrepresented sequences
 8. Adapter Content
 
 ## Quick Start Guide
 
 1. Install EZQC following [Installation guide](#installation).
 2. Run the tool on a toy example using the command `ezqc tests/SRR020182.fastq` (fastq file from [IGSR](https://www.internationalgenome.org/data-portal/sample/NA18486)).
-3. The results will be displayed in the terminal, and figures as well as csv tables will be saved to a directory named `ezqc_output` in your current working directory. Note that this file is choosen intendedly to fail multiple QC tests.
+3. The results will be displayed in the terminal, and figures as well as csv tables will be saved to a directory named `ezqc_output` in your current working directory. Note that this file is choosen intentionally to fail multiple QC tests.
 
 ## Installation
 
-You can install EZQC from source using the provided `setup.py` script. Here are the steps:
+You can install EZQC using pip:
+```
+pip install ezqc
+```
+
+Alternatively, you can compile the latest version of EZQC from source using the provided `setup.py` script. Following steps:
 
 1. Clone the repository:
 
 ```
 git clone https://github.com/skysky2333/ezqc
 ```
 
@@ -52,18 +59,18 @@
 ```
 cd ezqc
 ```
 
 3. Install the package:
 
 ```
-pip3 install .
+pip install .
 ```
 
-Or install directly:
+Or
 
 ```
 python setup.py install
 ```
 
 EZQC requires Python 3.x and depends on the following packages, which will be installed automatically during setup:
 
@@ -82,14 +89,15 @@
 ```
 
 Replace `<fastq file(s)>` with the path(s) to your FastQ files. If you want to analyze multiple files, separate the file paths with spaces:
 
 ```
 ezqc file1.fastq file2.fastq file3.fastq
 ```
+Use `-o` or `--output` to set the output directory.
 
 ## Analysis Methods
 
 Here's a brief description of the analyses performed by EZQC:
 
 1. **Per Base Sequence Quality**: Checks the quality of each base call in a sequence read.
 2. **Per Sequence Quality Scores**: Provides a histogram of quality scores over all sequences.
```

### Comparing `ezqc-0.2/ezqc/ac8.py` & `ezqc-0.3/ezqc/ac8.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,50 +6,54 @@
     'Illumina Small RNA 3\' Adapter': 'TGGAATTCTCGG',
     'Illumina Small RNA 5\' Adapter': 'GATCGTCGGACT',
     'SOLiD Small RNA Adapter': 'CTGCTGTACGGCCAAGGCG'
 }
 
 def calculate_adapter_content(sequences, adapters):
 
-    counts = {name: [0]*len(seq) for name, seq in adapters.items()}
+    counts = {name: [0]*len(sequences) for name, seq in adapters.items()}
 
+    curr = 0
     for seq in sequences:
         for name, adapter in adapters.items():
-            for i in range(len(seq) - len(adapter) + 1):
-                if seq[i:i+len(adapter)] == adapter:
-                    counts[name][i] += 1
+            if len(seq) >= len(adapter):
+                for i in range(len(seq) - len(adapter) + 1):
+                    if seq[i:i+len(adapter)] == adapter:
+                        counts[name][curr] += 1
+        curr += 1
 
     percentages = {name: [count/len(sequences)*100 for count in count_list] for name, count_list in counts.items()}
 
     all_pass = True
     for name, percentage in percentages.items():
         if max(percentage) > 10:
             print_color(f'X | {name} is present in more than 10% of all reads','red')
             all_pass = False
         elif (max(percentage) > 5):
             print_color(f'- | {name} is present in more than 5% of all reads','yellow')
             all_pass = False
     if (all_pass):
         print_color(f'O | No adaptor is present in more than 5% of all reads','green')
 
-    return percentages
+    return percentages, all_pass
 
-def plot_adapter_content(adapter_percentages):
+def plot_adapter_content(adapter_percentages,sub_directory_path):
     plt.figure()
     positions = list(range(1, max(map(len, adapter_percentages.values())) + 1))
 
     for name, percentages in adapter_percentages.items():
         plt.plot(positions[:len(percentages)], percentages, label=name)
 
     plt.xlabel('Position in read (bp)')
     plt.ylabel('% Adapter')
     plt.ylim(0, 100)
     plt.title('Adapter Content')
     plt.legend()
 
     # Save and/or display the plot
-    plt.savefig("ezqc_output/adaptor_content_plot.png")
+    plt.savefig(f"{sub_directory_path}/adaptor_content_plot.png")
     #plt.show()
 
-def run_ac8(seqs):
-    adapter_percentages = calculate_adapter_content(seqs, adapters)
-    plot_adapter_content(adapter_percentages)
+def run_ac8(seqs,sub_directory_path):
+    adapter_percentages, all_pass = calculate_adapter_content(seqs, adapters)
+    plot_adapter_content(adapter_percentages,sub_directory_path)
+    return all_pass
```

### Comparing `ezqc-0.2/ezqc/ezqc.py` & `ezqc-0.3/ezqc/ezqc.py`

 * *Files 22% similar despite different names*

```diff
@@ -31,19 +31,20 @@
     '''
     
     print(logo)
 
     # Create the argparse object and define the arguments
     parser = argparse.ArgumentParser(description="EZQC FastQ Quality Analyzer")
     parser.add_argument('seqs', metavar='SEQ', nargs='+', help='input .fastq file(s)')
+    parser.add_argument('-o', '--output', default='ezqc_output', help='output directory (default: ezqc_output)')
 
     # Parse the command-line arguments 
     args = parser.parse_args()
 
-    directory_name = "ezqc_output"
+    directory_name = args.output
     # Get the current working directory
     current_directory = os.getcwd()
     # Create a path for the new directory
     new_directory_path = os.path.join(current_directory, directory_name)
 
     # Create the directory if it doesn't already exist
     if not os.path.exists(new_directory_path):
@@ -51,38 +52,52 @@
         print(f"Directory '{directory_name}' created successfully!")
     else:
         print(f"Directory '{directory_name}' already exists.")
 
     total_num = 0
     pass_num = 0
 
+
     # Process each .fastq file
     for file_path in args.seqs:
         print(f"Processing file: {file_path}")
+       
+        file_base_name = os.path.basename(file_path)
+        file_base_name = os.path.splitext(file_base_name)[0]
+        sub_directory_path = os.path.join(new_directory_path, file_base_name)
+
+        # Create the directory if it doesn't already exist
+        if not os.path.exists(sub_directory_path):
+            os.makedirs(sub_directory_path)
+            print(f"Directory '{sub_directory_path}' created successfully!")
+        else:
+            print(f"Directory '{sub_directory_path}' already exists.")
+
         total_num += 1
         headers = []
         sequences = []
         quality_strings = []
 
         with open(file_path, 'r') as fastq_file:
             for header, sequence, quality_str in parse_fastq_file(fastq_file):
                 headers.append(header)
                 sequences.append(sequence)
                 quality_strings.append(quality_str)
         # average_length_each_sequence = int(np.average([len(x) for x in quality_strings]))
 
-    results = [
-        run_pbsq1(quality_strings),
-        run_psqs2(quality_strings),
-        run_pbsc3(sequences),
-        run_psgc4(sequences),
-        run_pbnc5(sequences),
-        run_sld6(sequences),
-        run_os7(sequences),
-        run_ac8(sequences)
-    ]
+        results = [
+            run_pbsq1(quality_strings,sub_directory_path),
+            run_psqs2(quality_strings,sub_directory_path),
+            run_pbsc3(sequences,sub_directory_path),
+            run_psgc4(sequences,sub_directory_path),
+            run_pbnc5(sequences,sub_directory_path),
+            run_sld6(sequences,sub_directory_path),
+            run_os7(sequences,sub_directory_path),
+            run_ac8(sequences,sub_directory_path)
+        ]
+
     if all(results): 
         pass_num += 1
     print(f"All fastq file analyzied, {pass_num}/{total_num} passed all tests.")
 
 if __name__ == '__main__':
     main()
```

### Comparing `ezqc-0.2/ezqc/os7.py` & `ezqc-0.3/ezqc/os7.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 import collections
 import csv
 from .color_print import print_color
 
-def run_os7(dna_sequences):
+def run_os7(dna_sequences,sub_directory_path):
+    # Track only the first 100,000 sequences
+    dna_sequences = dna_sequences[:100000] if len(dna_sequences)>100000 else dna_sequences
+
+    # Truncate sequences over 75bp to 50bp for analysis
+    dna_sequences = [seq[:50] if len(seq) > 75 else seq for seq in dna_sequences]
+
     total_count = len(dna_sequences)
     
     counter = collections.Counter(dna_sequences)
     
     table = []
     
     sequences_exceeding_1_percent = 0
@@ -19,15 +25,15 @@
             sequences_exceeding_1_percent += 1
             table.append([sequence, count, percentage])
 
         elif percentage > 0.1:
             sequences_exceeding_0_1_percent += 1
             table.append([sequence, count, percentage])
 
-    with open('ezqc_output/overrepresented_sequences.csv', 'w', newline='') as f:
+    with open(f"{sub_directory_path}/overrepresented_sequences.csv", 'w', newline='') as f:
         writer = csv.writer(f)
         writer.writerow(["Sequence", "Count", "Percentage"])
         writer.writerows(table)
 
     if (sequences_exceeding_1_percent > 0):
         print_color(f"X | Overrepresented sequences NOT pass. {sequences_exceeding_1_percent} sequences representing more than 1% of the total", "red")
         return False
```

### Comparing `ezqc-0.2/ezqc/pbnc5.py` & `ezqc-0.3/ezqc/pbnc5.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         if n_content[-1] > 20:
             greater_20 += 1
         if n_content[-1] > 10:
             greater_10 += 1
 
     return n_content, greater_10, greater_20
 
-def plot_n_content(n_content):
+def plot_n_content(n_content,sub_directory_path):
     # Create the x-values for our plot (the position in the read)
     x_values = list(range(1, len(n_content)+1))
 
     # Create a new figure
     plt.figure()
 
     # Plot the 'N' content
@@ -44,20 +44,20 @@
     # Add labels and a legend
     plt.xlabel('Position in read (bp)')
     plt.ylabel('N content (%)')
     plt.ylim(0, 100)
     plt.legend()
 
     # Save and/or display the plot
-    plt.savefig("ezqc_output/per_base_N_content_plot.png")
+    plt.savefig(f"{sub_directory_path}/per_base_N_content_plot.png")
     #plt.show()
 
-def run_pbnc5(seqs):
+def run_pbnc5(seqs,sub_directory_path):
     content, greater_10, greater_20 = per_base_n_content(seqs)
-    plot_n_content(content)
+    plot_n_content(content,sub_directory_path)
     if (greater_20>0):
         print_color(f"X | Per base N content NOT pass. {greater_20} positions with greater than 20% N content", "red")
         return False
     elif (greater_10):  
         print_color(f"- | Per base N content warning. {greater_10} positions with greater than 10% N content", "yellow")
         return False
     else:
```

### Comparing `ezqc-0.2/ezqc/pbsc3.py` & `ezqc-0.3/ezqc/pbsc3.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         if abs(base_content['A'][-1] - base_content['T'][-1]) > 10 or abs(base_content['G'][-1] - base_content['C'][-1]) > 10:
             greater_10 += 1
 
     return base_content, greater_10, greater_20
 
 
 
-def plot_base_content(base_content):
+def plot_base_content(base_content,sub_directory_path):
     # Create the x-values for our plot (the position in the read)
     x_values = list(range(1, len(base_content['A'])+1))
 
     plt.figure()
 
     # Plot the base content for each base 
     for base, y_values in base_content.items():
@@ -49,22 +49,22 @@
     # Add labels and a legend
     plt.xlabel('Position in read (bp)')
     plt.ylabel('Base content (%)')
     plt.ylim(0, 100)
     plt.legend()
 
     # Save and/or display the plot
-    plt.savefig("ezqc_output/per_base_sequence_content_plot.png")
+    plt.savefig(f"{sub_directory_path}/per_base_sequence_content_plot.png")
     #plt.show()
 
-def run_pbsc3(seqs):
+def run_pbsc3(seqs,sub_directory_path):
     content, greater_10, greater_20 = per_base_sequence_content(seqs)
-    plot_base_content(content)
+    plot_base_content(content,sub_directory_path)
     if (greater_20>0):
         print_color(f"X | Per base sequence content NOT pass. {greater_20} positions with greater than 20% differences", "red")
         return False
     elif (greater_10):  
-        print_color(f"X | Per base sequence content warning. {greater_10} positions with greater than 10% differences", "yellow")
+        print_color(f"- | Per base sequence content warning. {greater_10} positions with greater than 10% differences", "yellow")
         return False
     else:
-        print_color(f"X | Per base sequence content pass. No positions with greater than 10% differences", "green")
+        print_color(f"O | Per base sequence content pass. No positions with greater than 10% differences", "green")
         return True
```

### Comparing `ezqc-0.2/ezqc/pbsq1.py` & `ezqc-0.3/ezqc/pbsq1.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     for i, qstr in enumerate(quality_strings):
         scores = phred33_to_q(qstr)
         quality_scores[i, :len(scores)] = scores
         mask[i, :len(scores)] = True
     
     return quality_scores, mask
 
-def run_pbsq1(quality_strings):
+def run_pbsq1(quality_strings,sub_directory_path):
     # Convert quality strings to quality scores 
     quality_scores, mask = calculate_quality_scores(quality_strings)
 
     # Calculate the number of reads and the maximum length of the reads
     max_read_length = quality_scores.shape[1]
 
     # Calculate average, lower quartile, and upper quartile quality scores for each base position
@@ -67,23 +67,23 @@
     plt.xlabel('Position in read (bp)')
     plt.ylabel('Quality score')
     plt.title('Per base sequence quality plot')
     plt.xticks(np.arange(1, max_read_length+1, max(1, max_read_length//15)))  # Adjust x-axis tick spacing
     plt.yticks(np.arange(0, np.max(average_quality_scores)+1, 2))
     plt.grid(True)
     plt.legend()
-    plt.savefig("ezqc_output/per_base_sequence_quality_plot.png")
+    plt.savefig(f"{sub_directory_path}/per_base_sequence_quality_plot.png")
     # plt.show()
 
     avg_score = np.average(average_quality_scores)
 
     if avg_score < threshold*0.75:
-        print_color(f"X | Per base sequence quality NOT pass. Low average quality score of {avg_score:.2f}", "green")
+        print_color(f"X | Per base sequence quality NOT pass. Low average quality score of {avg_score:.2f}", "red")
         return False
     elif np.all(average_quality_scores >= threshold):
-        print_color(f"O | Per base sequence quality pass. With high average quality score of {avg_score:.2f}", "red")
+        print_color(f"O | Per base sequence quality pass. With high average quality score of {avg_score:.2f}", "green")
         return True
     else:
         indices_above_threshold = np.where(average_quality_scores >= threshold)[0]
         start, end = find_largest_range(indices_above_threshold)
         print_color(f"- | Per base sequence quality can be improved. With high quality reads from position {start} to {end}", "yellow")
         return False
```

### Comparing `ezqc-0.2/ezqc/psgc4.py` & `ezqc-0.3/ezqc/psgc4.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     elif sum_deviation > failure_threshold:
         print_color("X | The sum of the deviations from the normal distribution represents more than 30% of the reads.","red")
         return False
     else:
         print_color("O | The sum of the deviations from the normal distribution are good","green")
         return True
 
-def run_psgc4(sequences):
+def run_psgc4(sequences,sub_directory_path):
     gc_contents = []
     # Iterate through each sequence
     for seq in sequences:
         # Compute the GC content for the current sequence
         count_gc = sum(base in "GC" for base in seq)
         gc_percent = 100 * count_gc / len(seq)
 
@@ -45,11 +45,11 @@
 
     plt.title("GC distribution over all sequences")
     plt.xlabel("Mean GC content")
     plt.ylabel("Number of sequences")
     plt.legend(loc='upper right')
     plt.grid(True)
     # Save and/or display the all the plots
-    plt.savefig("ezqc_output/per_sequence_GC_content.png")
+    plt.savefig(f"{sub_directory_path}/per_sequence_GC_content.png")
     # plt.show()
 
     return detect_warnings_failures(gc_contents,sequences)
```

### Comparing `ezqc-0.2/ezqc/psqs2.py` & `ezqc-0.3/ezqc/psqs2.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 def phred33_to_q(qual_string):
     return [ord(ch) - 33 for ch in qual_string]
 
 def mean_qual_score(qual_string):
     qual_scores = phred33_to_q(qual_string)
     return np.mean(qual_scores)
 
-def run_psqs2(quality_strings):
+def run_psqs2(quality_strings,sub_directory_path):
 # Calculate mean quality scores for each sequence
     mean_qual_scores = [mean_qual_score(qual_string) for qual_string in quality_strings]
 
     # Set up bins for the x-axis (mean sequence quality)
     bin_edges = np.arange(0, np.ceil(max(mean_qual_scores)) + 1, 1)
 
     # Calculate the frequency (counts) for each bin
@@ -28,18 +28,18 @@
     plt.xlabel("Mean Sequence Quality(Phred scores)")
     plt.ylabel("Number of Sequences")
     plt.title("Quality Scores distribution over all sequences")
     plt.xticks(bin_edges)
     plt.grid(True, linestyle='--', alpha=0.5)
 
     # Save and/or display the plot
-    plt.savefig("ezqc_output/per_sequence_quality_scores.png")
+    plt.savefig(f"{sub_directory_path}/per_sequence_quality_scores.png")
     # plt.show()
 
 
     # print(proportion_low_quality)
-    if (proportion_low_quality > 0.01):
-        print_color(f"X | Per sequence quality score NOT pass. Because proportion of low quality is {100*proportion_low_quality:.2f} %, which is more than 1%","red")
+    if (proportion_low_quality >= 0.05):
+        print_color(f"X | Per sequence quality score NOT pass. Because proportion of low quality is {100*proportion_low_quality:.2f} %, which is more than 5%","red")
         return False
     else:
-        print_color(f"O | Per sequence quality pass. Proportion of low quality is {100*proportion_low_quality:.2f} %, which is less than 1%","green")
+        print_color(f"O | Per sequence quality pass. Proportion of low quality is {100*proportion_low_quality:.2f} %, which is less than 5%","green")
         return True
```

### Comparing `ezqc-0.2/ezqc.egg-info/PKG-INFO` & `ezqc-0.3/ezqc.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: ezqc
-Version: 0.2
+Version: 0.3
 Summary: EZQC is a streamlined, terminal-based alternative to FastQC.
 Author: Tinger Shi & Sky Li
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![EZQC Main Tests](https://github.com/skysky2333/EZQC/actions/workflows/ezqc_main_test.yml/badge.svg)](https://github.com/skysky2333/EZQC/actions/workflows/ezqc_main_test.yml)
-[![PyPI](https://github.com/skysky2333/EZQC/actions/workflows/python-publish.yml/badge.svg)](https://github.com/skysky2333/EZQC/actions/workflows/python-publish.yml)
+[![PyPI](https://img.shields.io/pypi/v/ezqc?color=blue)](https://pypi.org/project/ezqc/)
+
+
 
 # EZQC: Easy Quality Control for FastQ Files
 <p align="center">
   <img src="tests/test1.gif" alt="test Gif" width="100%">
 </p>
 
 ## Table of Contents
@@ -39,19 +41,24 @@
 7. Overrepresented sequences
 8. Adapter Content
 
 ## Quick Start Guide
 
 1. Install EZQC following [Installation guide](#installation).
 2. Run the tool on a toy example using the command `ezqc tests/SRR020182.fastq` (fastq file from [IGSR](https://www.internationalgenome.org/data-portal/sample/NA18486)).
-3. The results will be displayed in the terminal, and figures as well as csv tables will be saved to a directory named `ezqc_output` in your current working directory. Note that this file is choosen intendedly to fail multiple QC tests.
+3. The results will be displayed in the terminal, and figures as well as csv tables will be saved to a directory named `ezqc_output` in your current working directory. Note that this file is choosen intentionally to fail multiple QC tests.
 
 ## Installation
 
-You can install EZQC from source using the provided `setup.py` script. Here are the steps:
+You can install EZQC using pip:
+```
+pip install ezqc
+```
+
+Alternatively, you can compile the latest version of EZQC from source using the provided `setup.py` script. Following steps:
 
 1. Clone the repository:
 
 ```
 git clone https://github.com/skysky2333/ezqc
 ```
 
@@ -60,18 +67,18 @@
 ```
 cd ezqc
 ```
 
 3. Install the package:
 
 ```
-pip3 install .
+pip install .
 ```
 
-Or install directly:
+Or
 
 ```
 python setup.py install
 ```
 
 EZQC requires Python 3.x and depends on the following packages, which will be installed automatically during setup:
 
@@ -90,14 +97,15 @@
 ```
 
 Replace `<fastq file(s)>` with the path(s) to your FastQ files. If you want to analyze multiple files, separate the file paths with spaces:
 
 ```
 ezqc file1.fastq file2.fastq file3.fastq
 ```
+Use `-o` or `--output` to set the output directory.
 
 ## Analysis Methods
 
 Here's a brief description of the analyses performed by EZQC:
 
 1. **Per Base Sequence Quality**: Checks the quality of each base call in a sequence read.
 2. **Per Sequence Quality Scores**: Provides a histogram of quality scores over all sequences.
```

### Comparing `ezqc-0.2/setup.py` & `ezqc-0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='ezqc',
-    version='0.2',
+    version='0.3',
     author='Tinger Shi & Sky Li',
     description='EZQC is a streamlined, terminal-based alternative to FastQC.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         # Add your project dependencies here
         'numpy',
```

