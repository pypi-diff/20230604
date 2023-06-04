# Comparing `tmp/rescupybs-0.1.1.1-py3-none-any.whl.zip` & `tmp/rescupybs-0.1.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 9697 bytes, number of entries: 9
--rw-rw-r--  2.0 unx       29 b- defN 23-May-29 02:30 rescupybs/__init__.py
--rw-rw-r--  2.0 unx    16032 b- defN 23-May-29 02:30 rescupybs/functions.py
--rw-rw-r--  2.0 unx     7674 b- defN 23-May-29 02:30 rescupybs/plots.py
--rw-rw-r--  2.0 unx    13777 b- defN 23-May-29 02:30 rescupybs/wrapper.py
--rw-rw-r--  2.0 unx     3044 b- defN 23-May-29 02:30 rescupybs-0.1.1.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-29 02:30 rescupybs-0.1.1.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       88 b- defN 23-May-29 02:30 rescupybs-0.1.1.1.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       10 b- defN 23-May-29 02:30 rescupybs-0.1.1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      722 b- defN 23-May-29 02:30 rescupybs-0.1.1.1.dist-info/RECORD
-9 files, 41468 bytes uncompressed, 8453 bytes compressed:  79.6%
+Zip file size: 9940 bytes, number of entries: 9
+-rw-rw-r--  2.0 unx       29 b- defN 23-Jun-04 05:27 rescupybs/__init__.py
+-rw-rw-r--  2.0 unx    16032 b- defN 23-Jun-04 05:27 rescupybs/functions.py
+-rw-rw-r--  2.0 unx     9028 b- defN 23-Jun-04 05:27 rescupybs/plots.py
+-rw-rw-r--  2.0 unx    15082 b- defN 23-Jun-04 05:27 rescupybs/wrapper.py
+-rw-rw-r--  2.0 unx     3044 b- defN 23-Jun-04 05:27 rescupybs-0.1.1.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-04 05:27 rescupybs-0.1.1.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       88 b- defN 23-Jun-04 05:27 rescupybs-0.1.1.2.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       10 b- defN 23-Jun-04 05:27 rescupybs-0.1.1.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      722 b- defN 23-Jun-04 05:27 rescupybs-0.1.1.2.dist-info/RECORD
+9 files, 44127 bytes uncompressed, 8696 bytes compressed:  80.3%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: rescupybs/plots.py
 Comment: 
 
 Filename: rescupybs/wrapper.py
 Comment: 
 
-Filename: rescupybs-0.1.1.1.dist-info/METADATA
+Filename: rescupybs-0.1.1.2.dist-info/METADATA
 Comment: 
 
-Filename: rescupybs-0.1.1.1.dist-info/WHEEL
+Filename: rescupybs-0.1.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: rescupybs-0.1.1.1.dist-info/entry_points.txt
+Filename: rescupybs-0.1.1.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: rescupybs-0.1.1.1.dist-info/top_level.txt
+Filename: rescupybs-0.1.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: rescupybs-0.1.1.1.dist-info/RECORD
+Filename: rescupybs-0.1.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## rescupybs/__init__.py

```diff
@@ -1,3 +1,3 @@
 
-__version__ = "0.1.1.1"
+__version__ = "0.1.1.2"
```

## rescupybs/plots.py

```diff
@@ -132,23 +132,49 @@
         for i in chpts[1:-1]:
             ax1.axvline(i, linewidth=0.4, linestyle='-.', c='gray')
             ax2.axvline(i, linewidth=0.4, linestyle='-.', c='gray')
     ax1.axhline(linewidth=0.4, linestyle='-.', c='gray')
     ax2.axhline(linewidth=0.4, linestyle='-.', c='gray')
     plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
 
-def tdos(arr, ele, fig_p):
+def tdos(arr, ele, legend, fig_p):
     plt.figure(figsize=fig_p.size)
     plt.minorticks_on()
     plt.tick_params(axis='both', which='minor', color='gray')
-    plt.plot(arr, ele)
-    plt.xlim(fig_p.vertical)
-    plt.ylim(fig_p.horizontal)
-    plt.xlabel('Energy (eV)')
-    plt.ylabel('Density of states, electrons/eV')
+    color = fig_p.color or ['']
+    linestyle = fig_p.linestyle or ['-']
+    linewidth = fig_p.linewidth or [0.8]
+    if fig_p.exchange:
+        if color[0]:
+            plt.plot(arr, ele[:,0], linewidth=linewidth[0], linestyle=linestyle[0], color=color[0])
+            if fig_p.fill:
+                plt.fill_between(arr, ele[:,0], 0, color=color[0], alpha=fig_p.fill)
+        else:
+            plt.plot(arr, ele[:,0], linewidth=linewidth[0], linestyle=linestyle[0])
+            if fig_p.fill:
+                plt.fill_between(arr, ele[:,0], 0, alpha=fig_p.fill)
+        plt.tick_params(axis='y', labelsize='medium', labelcolor='dimgray')
+        plt.xlim(fig_p.vertical)
+        plt.ylim(fig_p.horizontal)
+        plt.xlabel('Energy (eV)')
+        plt.ylabel('Density of states, electrons/eV')
+    else:
+        if color[0]:
+            plt.plot(ele[:,0], arr, linewidth=linewidth[0], linestyle=linestyle[0], color=color[0])
+            if fig_p.fill:
+                plt.fill_betweenx(arr, ele[:,0], 0, color=color[0], alpha=fig_p.fill)
+        else:
+            plt.plot(ele[:,0], arr, linewidth=linewidth[0], linestyle=linestyle[0])
+            if fig_p.fill:
+                plt.fill_betweenx(arr, ele[:,0], 0, alpha=fig_p.fill)
+        plt.tick_params(axis='x', labelsize='medium', labelcolor='dimgray')
+        plt.ylim(fig_p.vertical)
+        plt.xlim(fig_p.horizontal)
+        plt.ylabel('Energy (eV)')
+        plt.xlabel('Density of states, electrons/eV')
+    L = plt.legend([], frameon=False, loc=fig_p.location, title=legend[0], title_fontproperties={'size':'medium'})
+    plt.gca().add_artist(L)
     plt.axvline(linewidth=0.4, linestyle='-.', c='gray')
     plt.axhline(linewidth=0.4, linestyle='-.', c='gray')
-#    plt.legend(p_dos, elements, frameon=False, prop={'size':'medium'}, loc=fig_p.location)
     plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
-    
-    
+
```

## rescupybs/wrapper.py

```diff
@@ -46,15 +46,16 @@
     parser.add_argument('-l', "--labels",     type=str.upper,       nargs='+', default=[], help='labels for high-symmetry points')
     parser.add_argument('-d', "--dos",        type=str,             nargs='?', default='', help="plot DOS from .json file, default: nano_dos_out.json")
     parser.add_argument('-x', "--horizontal", type=float, nargs=2,  help="Density of states, electrons/eV range")
     parser.add_argument('-a', "--exchange",   action='store_true',  help="exchange the x and y axes of DOS")
     parser.add_argument('-p', "--partial",    type=str,             nargs='+', default=[], help='the partial DOS to plot, s p d')
     parser.add_argument('-e', "--elements",   type=str,             nargs='+', default=[], help="PDOS labels")
     parser.add_argument('-W', "--wratios",    type=float,           help='width ratio for DOS subplot')
-    parser.add_argument('-z', "--fill",       type=float,           nargs='*', help='fill a shaded region between PDOS and axis, default: 0.2', default=None)
+    parser.add_argument('-z', "--fill",       type=float,           nargs='?', help='fill a shaded region between PDOS and axis, default: 0.2', default=None,
+                                                                                    const=0.2, metavar="alpha")
     parser.add_argument('-f', "--font",       type=str,             default='STIXGeneral', help="font to use")
 
     args = parser.parse_args()
 
     labels_f = [re.sub("'|‘|’", '′', re.sub('"|“|”', '″', re.sub('^GA[A-Z]+$|^G$', 'Γ', i))) for i in args.labels]
     elements = [re.sub("'|‘|’", '′', re.sub('"|“|”', '″', i)) for i in args.elements]
     if args.dos != '':
@@ -96,15 +97,16 @@
     input = [f for i in input for f in glob.glob(i)]
     input = [os.path.join(i,'nano_bs_out.json') if os.path.isdir(i) else i for i in input]
     input = [i for i in input if os.path.exists(i)]
 
     width_ratios = args.wratios or (0.3 if args.divided else 0.5)
 
     fig_p = cla_fig(output=args.output, size=args.size, vertical=args.vertical, horizontal=args.horizontal,
-                    color=color, linestyle=linestyle, linewidth=linewidth, location=args.location, dpi=args.dpi)
+                    color=color, linestyle=linestyle, linewidth=linewidth, location=args.location, dpi=args.dpi,
+                    width_ratios=width_ratios, exchange=args.exchange, fill=args.fill)
 
     len_bandfile = len(input)
 # plot Band Structure
     if len_bandfile == 1:
         if not fig_p.vertical:
             fig_p.vertical = [-5.0, 5.0]
         if input[0].lower().endswith('.json'):
@@ -189,20 +191,40 @@
         else:
             raise Exception("The input files mismatch.")
 # plot DOS
     elif len_bandfile == 0:
         if dosfiles:
             if fig_p.output == "BAND.png":
                 fig_p.output = "DOS.png"
+            legend = args.legend or [pltname]
             arr, ele = functions.tdos(dosfiles)
-            plots.tdos(arr, ele, fig_p)
+            plots.tdos(arr, ele, legend, fig_p)
         else:
             print("ERROR: No *dos_out.json file.")
     else:
-        print("Input file mismatch.")
+        if not fig_p.vertical:
+            fig_p.vertical = [-5.0, 5.0]
+        Extension = [f.rsplit('.', 1)[-1].lower() for f in input]
+        if all(x == Extension[0] for x in Extension) and Extension[0] == 'json' and all('bs' in f.split('_') for f in input):
+            eigenvalues, chpts, labels = functions.bs_json_read_all(input)
+            if labels_f:
+                labels = labels_f
+            legend = args.legend or [pltname]
+            if len(chpts) > len(labels):
+                labels = labels + [''] * (len(chpts) - len(labels))
+            elif len(chpts) < len(labels):
+                labels = labels[:len(chpts)]
+            if len(eigenvalues) == 1:
+                plots.Nispin(eigenvalues, chpts, labels, legend, fig_p)
+            elif len(eigenvalues) == 2 and not args.divided:
+                plots.Ispin(eigenvalues, chpts, labels, legend, fig_p)
+            elif len(eigenvalues) == 2 and args.divided:
+                plots.Dispin(eigenvalues, chpts, labels, legend, fig_p)
+        else:
+            print("Input file mismatch.")
 
 def surface():
     parser = argparse.ArgumentParser(description='Export the wavefunction isosurface for VESTA from rescuplus calculation result *.json and *.h5 files.',
                                      epilog='''
 Example:
 rescuiso -b 1 -k 0
 ''',
```

## Comparing `rescupybs-0.1.1.1.dist-info/METADATA` & `rescupybs-0.1.1.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rescupybs
-Version: 0.1.1.1
+Version: 0.1.1.2
 Summary: Band structure plot and wavefunction export from rescuplus *.json and *.h5 file.
 Home-page: https://github.com/lkccrr/rescupybs
 Author: kan
 Author-email: luokan@hrbeu.edu.cn
 License: MIT
 Keywords: DFT rescuplus band plot wavefunction
 Platform: Unix
```

## Comparing `rescupybs-0.1.1.1.dist-info/RECORD` & `rescupybs-0.1.1.2.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-rescupybs/__init__.py,sha256=L8ZZeqV3ZossHfeL37DRT_aUNvdxySXK8tzaxVkJAIg,29
+rescupybs/__init__.py,sha256=JotjjeZaSfNoaQGm6SDmQ4_NXSX6NZXPNFTDh0Yfe7Q,29
 rescupybs/functions.py,sha256=LOArp6CRkUeb2Ed8auX-Ko8_HrMiWPS0Cqd_iJLidXI,16032
-rescupybs/plots.py,sha256=Slev0FrsUu0NY25qw0CJ_E4fY4oOmCgOUVkKDgSTnSM,7674
-rescupybs/wrapper.py,sha256=Ppabz1R-gw8xTgDUEDhX7u5xBTGP--5fv51YJSwvzEk,13777
-rescupybs-0.1.1.1.dist-info/METADATA,sha256=aveYvCzPgLEcs34dh2R8LLWKzIYmB55FwL38Zp6_h48,3044
-rescupybs-0.1.1.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-rescupybs-0.1.1.1.dist-info/entry_points.txt,sha256=WpFczXTlVBUla6UWHKetnJ_VGriTtoTlEQ63Tvy635U,88
-rescupybs-0.1.1.1.dist-info/top_level.txt,sha256=w6nJZTS0VDiS0Ij6-ub0Pukls7j8IAjyKwWgA8JHPS4,10
-rescupybs-0.1.1.1.dist-info/RECORD,,
+rescupybs/plots.py,sha256=pZiqVtQKctDlhrhcwfdGup55mpmSppThOLsuWmRhtlc,9028
+rescupybs/wrapper.py,sha256=Yc_9vrFtgxy1xbcIHt5gjaalvM38jSgfQi1FhwlCx0w,15082
+rescupybs-0.1.1.2.dist-info/METADATA,sha256=FJaHL_lvcfSf1mTHmrpVuYlFwxBiQmA6-89GqlNPzgU,3044
+rescupybs-0.1.1.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+rescupybs-0.1.1.2.dist-info/entry_points.txt,sha256=WpFczXTlVBUla6UWHKetnJ_VGriTtoTlEQ63Tvy635U,88
+rescupybs-0.1.1.2.dist-info/top_level.txt,sha256=w6nJZTS0VDiS0Ij6-ub0Pukls7j8IAjyKwWgA8JHPS4,10
+rescupybs-0.1.1.2.dist-info/RECORD,,
```

