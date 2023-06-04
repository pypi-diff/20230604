# Comparing `tmp/printbuddies-1.2.0.tar.gz` & `tmp/printbuddies-1.3.0.tar.gz`

## Comparing `printbuddies-1.2.0.tar` & `printbuddies-1.3.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 printbuddies-1.2.0/CHANGELOG.md
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 printbuddies-1.2.0/docs/index.html
--rw-r--r--   0        0        0    34315 2020-02-02 00:00:00.000000 printbuddies-1.2.0/docs/printbuddies.html
--rw-r--r--   0        0        0    34442 2020-02-02 00:00:00.000000 printbuddies-1.2.0/docs/search.js
--rw-r--r--   0        0        0   200796 2020-02-02 00:00:00.000000 printbuddies-1.2.0/docs/printbuddies/printbuddies.html
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 printbuddies-1.2.0/src/printbuddies/__init__.py
--rw-r--r--   0        0        0     9406 2020-02-02 00:00:00.000000 printbuddies-1.2.0/src/printbuddies/printbuddies.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 printbuddies-1.2.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 printbuddies-1.2.0/LICENSE.txt
--rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 printbuddies-1.2.0/README.md
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 printbuddies-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     3317 2020-02-02 00:00:00.000000 printbuddies-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 printbuddies-1.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 printbuddies-1.3.0/docs/index.html
+-rw-r--r--   0        0        0    34315 2020-02-02 00:00:00.000000 printbuddies-1.3.0/docs/printbuddies.html
+-rw-r--r--   0        0        0    34898 2020-02-02 00:00:00.000000 printbuddies-1.3.0/docs/search.js
+-rw-r--r--   0        0        0   214063 2020-02-02 00:00:00.000000 printbuddies-1.3.0/docs/printbuddies/printbuddies.html
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 printbuddies-1.3.0/src/printbuddies/__init__.py
+-rw-r--r--   0        0        0    10167 2020-02-02 00:00:00.000000 printbuddies-1.3.0/src/printbuddies/printbuddies.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 printbuddies-1.3.0/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 printbuddies-1.3.0/LICENSE.txt
+-rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 printbuddies-1.3.0/README.md
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 printbuddies-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3317 2020-02-02 00:00:00.000000 printbuddies-1.3.0/PKG-INFO
```

### Comparing `printbuddies-1.2.0/docs/printbuddies.html` & `printbuddies-1.3.0/docs/printbuddies.html`

 * *Files identical despite different names*

### Comparing `printbuddies-1.2.0/docs/search.js` & `printbuddies-1.3.0/docs/search.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -762,22 +762,22 @@
         "signature": "<span class=\"signature pdoc-code multiline\">(<span class=\"param\">\t<span class=\"bp\">self</span>,</span><span class=\"param\">\t<span class=\"n\">prefix</span><span class=\"p\">:</span> <span class=\"nb\">str</span> <span class=\"o\">=</span> <span class=\"s1\">&#39;&#39;</span>,</span><span class=\"param\">\t<span class=\"n\">suffix</span><span class=\"p\">:</span> <span class=\"nb\">str</span> <span class=\"o\">=</span> <span class=\"s1\">&#39;&#39;</span>,</span><span class=\"param\">\t<span class=\"n\">counter_override</span><span class=\"p\">:</span> <span class=\"nb\">float</span> <span class=\"o\">|</span> <span class=\"kc\">None</span> <span class=\"o\">=</span> <span class=\"kc\">None</span>,</span><span class=\"param\">\t<span class=\"n\">total_override</span><span class=\"p\">:</span> <span class=\"nb\">float</span> <span class=\"o\">|</span> <span class=\"kc\">None</span> <span class=\"o\">=</span> <span class=\"kc\">None</span>,</span><span class=\"param\">\t<span class=\"n\">return_object</span><span class=\"p\">:</span> <span class=\"n\">typing</span><span class=\"o\">.</span><span class=\"n\">Any</span> <span class=\"o\">|</span> <span class=\"kc\">None</span> <span class=\"o\">=</span> <span class=\"kc\">None</span></span><span class=\"return-annotation\">) -> <span class=\"n\">Any</span>:</span></span>",
         "funcdef": "def"
     }, {
         "fullname": "printbuddies.printbuddies.Spinner",
         "modulename": "printbuddies.printbuddies",
         "qualname": "Spinner",
         "kind": "class",
-        "doc": "<p>Prints one of a sequence of characters in order everytime display() is called.\nThe display function writes the new character to the same line, overwriting the previous character.\nThe sequence will be cycled through indefinitely.\nIf used as a context manager, the last printed character will be cleared upon exiting.</p>\n"
+        "doc": "<p>Prints one of a sequence of characters in order everytime display() is called.</p>\n\n<p>The display function writes the new character to the same line, overwriting the previous character.</p>\n\n<p>The sequence will be cycled through indefinitely.</p>\n\n<p>If used as a context manager, the last printed character will be cleared upon exiting.</p>\n"
     }, {
         "fullname": "printbuddies.printbuddies.Spinner.__init__",
         "modulename": "printbuddies.printbuddies",
         "qualname": "Spinner.__init__",
         "kind": "function",
-        "doc": "<h6 id=\"parameters\">Parameters</h6>\n\n<ul>\n<li><strong>sequence</strong>:  Override the built in spin sequence.</li>\n</ul>\n",
-        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">sequence</span><span class=\"p\">:</span> <span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"n\">typing</span><span class=\"o\">.</span><span class=\"n\">Any</span><span class=\"p\">]</span> <span class=\"o\">|</span> <span class=\"kc\">None</span> <span class=\"o\">=</span> <span class=\"kc\">None</span></span>)</span>"
+        "doc": "<h6 id=\"parameters\">Parameters</h6>\n\n<ul>\n<li><p><strong>sequence</strong>:  Override the built in spin sequence.</p></li>\n<li><p><strong>width</strong>:  The fractional amount of the terminal for characters to move across.</p></li>\n</ul>\n",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">sequence</span><span class=\"p\">:</span> <span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">]</span> <span class=\"o\">=</span> <span class=\"p\">[</span><span class=\"s1\">&#39;/&#39;</span><span class=\"p\">,</span> <span class=\"s1\">&#39;-&#39;</span><span class=\"p\">,</span> <span class=\"s1\">&#39;</span><span class=\"se\">\\\\</span><span class=\"s1\">&#39;</span><span class=\"p\">]</span>, </span><span class=\"param\"><span class=\"n\">width_ratio</span><span class=\"p\">:</span> <span class=\"nb\">float</span> <span class=\"o\">=</span> <span class=\"mf\">0.25</span></span>)</span>"
     }, {
         "fullname": "printbuddies.printbuddies.Spinner.display",
         "modulename": "printbuddies.printbuddies",
         "qualname": "Spinner.display",
         "kind": "function",
         "doc": "<p>Print the next character in the sequence.</p>\n",
         "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span></span><span class=\"return-annotation\">):</span></span>",
```

### Comparing `printbuddies-1.2.0/docs/printbuddies/printbuddies.html` & `printbuddies-1.3.0/docs/printbuddies/printbuddies.html`

 * *Files 2% similar despite different names*

```diff
@@ -311,52 +311,77 @@
 </span><span id="L-216"><a href="#L-216"><span class="linenos">216</span></a>                    <span class="nb">print</span><span class="p">()</span>
 </span><span id="L-217"><a href="#L-217"><span class="linenos">217</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">+=</span> <span class="mi">1</span>
 </span><span id="L-218"><a href="#L-218"><span class="linenos">218</span></a>        <span class="k">return</span> <span class="n">return_object</span>
 </span><span id="L-219"><a href="#L-219"><span class="linenos">219</span></a>
 </span><span id="L-220"><a href="#L-220"><span class="linenos">220</span></a>
 </span><span id="L-221"><a href="#L-221"><span class="linenos">221</span></a><span class="k">class</span> <span class="nc">Spinner</span><span class="p">:</span>
 </span><span id="L-222"><a href="#L-222"><span class="linenos">222</span></a>    <span class="sd">&quot;&quot;&quot;Prints one of a sequence of characters in order everytime display() is called.</span>
-</span><span id="L-223"><a href="#L-223"><span class="linenos">223</span></a><span class="sd">    The display function writes the new character to the same line, overwriting the previous character.</span>
-</span><span id="L-224"><a href="#L-224"><span class="linenos">224</span></a><span class="sd">    The sequence will be cycled through indefinitely.</span>
-</span><span id="L-225"><a href="#L-225"><span class="linenos">225</span></a><span class="sd">    If used as a context manager, the last printed character will be cleared upon exiting.&quot;&quot;&quot;</span>
-</span><span id="L-226"><a href="#L-226"><span class="linenos">226</span></a>
-</span><span id="L-227"><a href="#L-227"><span class="linenos">227</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">sequence</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">Any</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
-</span><span id="L-228"><a href="#L-228"><span class="linenos">228</span></a>        <span class="sd">&quot;&quot;&quot;</span>
-</span><span id="L-229"><a href="#L-229"><span class="linenos">229</span></a><span class="sd">        :param sequence: Override the built in spin sequence.&quot;&quot;&quot;</span>
-</span><span id="L-230"><a href="#L-230"><span class="linenos">230</span></a>        <span class="k">if</span> <span class="n">sequence</span><span class="p">:</span>
-</span><span id="L-231"><a href="#L-231"><span class="linenos">231</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">sequence</span> <span class="o">=</span> <span class="n">sequence</span>
-</span><span id="L-232"><a href="#L-232"><span class="linenos">232</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="L-233"><a href="#L-233"><span class="linenos">233</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">sequence</span> <span class="o">=</span> <span class="p">[</span><span class="s2">&quot;/&quot;</span><span class="p">,</span> <span class="s2">&quot;-&quot;</span><span class="p">,</span> <span class="s2">&quot;</span><span class="se">\\</span><span class="s2">&quot;</span><span class="p">]</span>
-</span><span id="L-234"><a href="#L-234"><span class="linenos">234</span></a>
-</span><span id="L-235"><a href="#L-235"><span class="linenos">235</span></a>    <span class="k">def</span> <span class="fm">__enter__</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="L-236"><a href="#L-236"><span class="linenos">236</span></a>        <span class="k">return</span> <span class="bp">self</span>
-</span><span id="L-237"><a href="#L-237"><span class="linenos">237</span></a>
-</span><span id="L-238"><a href="#L-238"><span class="linenos">238</span></a>    <span class="k">def</span> <span class="fm">__exit__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="o">*</span><span class="n">args</span><span class="p">,</span> <span class="o">**</span><span class="n">kwargs</span><span class="p">):</span>
-</span><span id="L-239"><a href="#L-239"><span class="linenos">239</span></a>        <span class="n">clear</span><span class="p">()</span>
-</span><span id="L-240"><a href="#L-240"><span class="linenos">240</span></a>
-</span><span id="L-241"><a href="#L-241"><span class="linenos">241</span></a>    <span class="nd">@property</span>
-</span><span id="L-242"><a href="#L-242"><span class="linenos">242</span></a>    <span class="k">def</span> <span class="nf">sequence</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">Any</span><span class="p">]:</span>
-</span><span id="L-243"><a href="#L-243"><span class="linenos">243</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_sequence</span>
+</span><span id="L-223"><a href="#L-223"><span class="linenos">223</span></a>
+</span><span id="L-224"><a href="#L-224"><span class="linenos">224</span></a><span class="sd">    The display function writes the new character to the same line, overwriting the previous character.</span>
+</span><span id="L-225"><a href="#L-225"><span class="linenos">225</span></a>
+</span><span id="L-226"><a href="#L-226"><span class="linenos">226</span></a><span class="sd">    The sequence will be cycled through indefinitely.</span>
+</span><span id="L-227"><a href="#L-227"><span class="linenos">227</span></a>
+</span><span id="L-228"><a href="#L-228"><span class="linenos">228</span></a><span class="sd">    If used as a context manager, the last printed character will be cleared upon exiting.</span>
+</span><span id="L-229"><a href="#L-229"><span class="linenos">229</span></a><span class="sd">    &quot;&quot;&quot;</span>
+</span><span id="L-230"><a href="#L-230"><span class="linenos">230</span></a>
+</span><span id="L-231"><a href="#L-231"><span class="linenos">231</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span>
+</span><span id="L-232"><a href="#L-232"><span class="linenos">232</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">sequence</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">=</span> <span class="p">[</span><span class="s2">&quot;/&quot;</span><span class="p">,</span> <span class="s2">&quot;-&quot;</span><span class="p">,</span> <span class="s2">&quot;</span><span class="se">\\</span><span class="s2">&quot;</span><span class="p">],</span> <span class="n">width_ratio</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="mf">0.25</span>
+</span><span id="L-233"><a href="#L-233"><span class="linenos">233</span></a>    <span class="p">):</span>
+</span><span id="L-234"><a href="#L-234"><span class="linenos">234</span></a>        <span class="sd">&quot;&quot;&quot;</span>
+</span><span id="L-235"><a href="#L-235"><span class="linenos">235</span></a><span class="sd">        :param sequence: Override the built in spin sequence.</span>
+</span><span id="L-236"><a href="#L-236"><span class="linenos">236</span></a>
+</span><span id="L-237"><a href="#L-237"><span class="linenos">237</span></a><span class="sd">        :param width: The fractional amount of the terminal for characters to move across.&quot;&quot;&quot;</span>
+</span><span id="L-238"><a href="#L-238"><span class="linenos">238</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_base_sequence</span> <span class="o">=</span> <span class="n">sequence</span>
+</span><span id="L-239"><a href="#L-239"><span class="linenos">239</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">width_ratio</span> <span class="o">=</span> <span class="n">width_ratio</span>
+</span><span id="L-240"><a href="#L-240"><span class="linenos">240</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">sequence</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_base_sequence</span>
+</span><span id="L-241"><a href="#L-241"><span class="linenos">241</span></a>
+</span><span id="L-242"><a href="#L-242"><span class="linenos">242</span></a>    <span class="k">def</span> <span class="fm">__enter__</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="L-243"><a href="#L-243"><span class="linenos">243</span></a>        <span class="k">return</span> <span class="bp">self</span>
 </span><span id="L-244"><a href="#L-244"><span class="linenos">244</span></a>
-</span><span id="L-245"><a href="#L-245"><span class="linenos">245</span></a>    <span class="nd">@sequence</span><span class="o">.</span><span class="n">setter</span>
-</span><span id="L-246"><a href="#L-246"><span class="linenos">246</span></a>    <span class="k">def</span> <span class="nf">sequence</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">character_list</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">Any</span><span class="p">]):</span>
-</span><span id="L-247"><a href="#L-247"><span class="linenos">247</span></a>        <span class="c1"># Buffer each element with a leading space</span>
-</span><span id="L-248"><a href="#L-248"><span class="linenos">248</span></a>        <span class="c1"># so that the character isn&#39;t obscured by the cursor</span>
-</span><span id="L-249"><a href="#L-249"><span class="linenos">249</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_sequence</span> <span class="o">=</span> <span class="p">[</span><span class="s2">&quot; &quot;</span> <span class="o">+</span> <span class="nb">str</span><span class="p">(</span><span class="n">ch</span><span class="p">)</span> <span class="k">for</span> <span class="n">ch</span> <span class="ow">in</span> <span class="n">character_list</span><span class="p">]</span>
-</span><span id="L-250"><a href="#L-250"><span class="linenos">250</span></a>
-</span><span id="L-251"><a href="#L-251"><span class="linenos">251</span></a>    <span class="k">def</span> <span class="nf">_get_next</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="L-252"><a href="#L-252"><span class="linenos">252</span></a>        <span class="sd">&quot;&quot;&quot;Pop the first element of self._sequence,</span>
-</span><span id="L-253"><a href="#L-253"><span class="linenos">253</span></a><span class="sd">        append it to the end, and return the element.&quot;&quot;&quot;</span>
-</span><span id="L-254"><a href="#L-254"><span class="linenos">254</span></a>        <span class="n">ch</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">sequence</span><span class="o">.</span><span class="n">pop</span><span class="p">(</span><span class="mi">0</span><span class="p">)</span>
-</span><span id="L-255"><a href="#L-255"><span class="linenos">255</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">sequence</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">ch</span><span class="p">)</span>
-</span><span id="L-256"><a href="#L-256"><span class="linenos">256</span></a>        <span class="k">return</span> <span class="n">ch</span>
-</span><span id="L-257"><a href="#L-257"><span class="linenos">257</span></a>
-</span><span id="L-258"><a href="#L-258"><span class="linenos">258</span></a>    <span class="k">def</span> <span class="nf">display</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="L-259"><a href="#L-259"><span class="linenos">259</span></a>        <span class="sd">&quot;&quot;&quot;Print the next character in the sequence.&quot;&quot;&quot;</span>
-</span><span id="L-260"><a href="#L-260"><span class="linenos">260</span></a>        <span class="n">print_in_place</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_get_next</span><span class="p">())</span>
+</span><span id="L-245"><a href="#L-245"><span class="linenos">245</span></a>    <span class="k">def</span> <span class="fm">__exit__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="o">*</span><span class="n">args</span><span class="p">,</span> <span class="o">**</span><span class="n">kwargs</span><span class="p">):</span>
+</span><span id="L-246"><a href="#L-246"><span class="linenos">246</span></a>        <span class="n">clear</span><span class="p">()</span>
+</span><span id="L-247"><a href="#L-247"><span class="linenos">247</span></a>
+</span><span id="L-248"><a href="#L-248"><span class="linenos">248</span></a>    <span class="nd">@property</span>
+</span><span id="L-249"><a href="#L-249"><span class="linenos">249</span></a>    <span class="k">def</span> <span class="nf">width_ratio</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">float</span><span class="p">:</span>
+</span><span id="L-250"><a href="#L-250"><span class="linenos">250</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_width_ratio</span>
+</span><span id="L-251"><a href="#L-251"><span class="linenos">251</span></a>
+</span><span id="L-252"><a href="#L-252"><span class="linenos">252</span></a>    <span class="nd">@width_ratio</span><span class="o">.</span><span class="n">setter</span>
+</span><span id="L-253"><a href="#L-253"><span class="linenos">253</span></a>    <span class="k">def</span> <span class="nf">width_ratio</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">ratio</span><span class="p">:</span> <span class="nb">float</span><span class="p">):</span>
+</span><span id="L-254"><a href="#L-254"><span class="linenos">254</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_width_ratio</span> <span class="o">=</span> <span class="n">ratio</span>
+</span><span id="L-255"><a href="#L-255"><span class="linenos">255</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_update_width</span><span class="p">()</span>
+</span><span id="L-256"><a href="#L-256"><span class="linenos">256</span></a>
+</span><span id="L-257"><a href="#L-257"><span class="linenos">257</span></a>    <span class="k">def</span> <span class="nf">_update_width</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="L-258"><a href="#L-258"><span class="linenos">258</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_current_terminal_width</span> <span class="o">=</span> <span class="n">get_terminal_size</span><span class="p">()</span><span class="o">.</span><span class="n">columns</span>
+</span><span id="L-259"><a href="#L-259"><span class="linenos">259</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_width</span> <span class="o">=</span> <span class="nb">int</span><span class="p">((</span><span class="bp">self</span><span class="o">.</span><span class="n">_current_terminal_width</span> <span class="o">-</span> <span class="mi">1</span><span class="p">)</span> <span class="o">*</span> <span class="bp">self</span><span class="o">.</span><span class="n">width_ratio</span><span class="p">)</span>
+</span><span id="L-260"><a href="#L-260"><span class="linenos">260</span></a>
+</span><span id="L-261"><a href="#L-261"><span class="linenos">261</span></a>    <span class="nd">@property</span>
+</span><span id="L-262"><a href="#L-262"><span class="linenos">262</span></a>    <span class="k">def</span> <span class="nf">sequence</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">Any</span><span class="p">]:</span>
+</span><span id="L-263"><a href="#L-263"><span class="linenos">263</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_sequence</span>
+</span><span id="L-264"><a href="#L-264"><span class="linenos">264</span></a>
+</span><span id="L-265"><a href="#L-265"><span class="linenos">265</span></a>    <span class="nd">@sequence</span><span class="o">.</span><span class="n">setter</span>
+</span><span id="L-266"><a href="#L-266"><span class="linenos">266</span></a>    <span class="k">def</span> <span class="nf">sequence</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">character_list</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">Any</span><span class="p">]):</span>
+</span><span id="L-267"><a href="#L-267"><span class="linenos">267</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_sequence</span> <span class="o">=</span> <span class="p">[</span>
+</span><span id="L-268"><a href="#L-268"><span class="linenos">268</span></a>            <span class="n">ch</span><span class="o">.</span><span class="n">rjust</span><span class="p">(</span><span class="n">i</span> <span class="o">+</span> <span class="n">j</span><span class="p">)</span>
+</span><span id="L-269"><a href="#L-269"><span class="linenos">269</span></a>            <span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="mi">1</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">_width</span><span class="p">,</span> <span class="nb">len</span><span class="p">(</span><span class="n">character_list</span><span class="p">))</span>
+</span><span id="L-270"><a href="#L-270"><span class="linenos">270</span></a>            <span class="k">for</span> <span class="n">j</span><span class="p">,</span> <span class="n">ch</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">character_list</span><span class="p">)</span>
+</span><span id="L-271"><a href="#L-271"><span class="linenos">271</span></a>        <span class="p">]</span>
+</span><span id="L-272"><a href="#L-272"><span class="linenos">272</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_sequence</span> <span class="o">+=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_sequence</span><span class="p">[::</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span>
+</span><span id="L-273"><a href="#L-273"><span class="linenos">273</span></a>
+</span><span id="L-274"><a href="#L-274"><span class="linenos">274</span></a>    <span class="k">def</span> <span class="nf">_get_next</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="L-275"><a href="#L-275"><span class="linenos">275</span></a>        <span class="sd">&quot;&quot;&quot;Pop the first element of self._sequence, append it to the end, and return the element.&quot;&quot;&quot;</span>
+</span><span id="L-276"><a href="#L-276"><span class="linenos">276</span></a>        <span class="n">ch</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">sequence</span><span class="o">.</span><span class="n">pop</span><span class="p">(</span><span class="mi">0</span><span class="p">)</span>
+</span><span id="L-277"><a href="#L-277"><span class="linenos">277</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">sequence</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">ch</span><span class="p">)</span>
+</span><span id="L-278"><a href="#L-278"><span class="linenos">278</span></a>        <span class="k">return</span> <span class="n">ch</span>
+</span><span id="L-279"><a href="#L-279"><span class="linenos">279</span></a>
+</span><span id="L-280"><a href="#L-280"><span class="linenos">280</span></a>    <span class="k">def</span> <span class="nf">display</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="L-281"><a href="#L-281"><span class="linenos">281</span></a>        <span class="sd">&quot;&quot;&quot;Print the next character in the sequence.&quot;&quot;&quot;</span>
+</span><span id="L-282"><a href="#L-282"><span class="linenos">282</span></a>        <span class="k">if</span> <span class="n">get_terminal_size</span><span class="p">()</span><span class="o">.</span><span class="n">columns</span> <span class="o">!=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_current_terminal_width</span><span class="p">:</span>
+</span><span id="L-283"><a href="#L-283"><span class="linenos">283</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">_update_width</span><span class="p">()</span>
+</span><span id="L-284"><a href="#L-284"><span class="linenos">284</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">sequence</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_base_sequence</span>
+</span><span id="L-285"><a href="#L-285"><span class="linenos">285</span></a>        <span class="n">print_in_place</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_get_next</span><span class="p">())</span>
 </span></pre></div>
 
 
             </section>
                 <section id="clear">
                             <input id="clear-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -942,86 +967,118 @@
 
                 <label class="view-source-button" for="Spinner-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Spinner"></a>
             <div class="pdoc-code codehilite"><pre><span></span><span id="Spinner-222"><a href="#Spinner-222"><span class="linenos">222</span></a><span class="k">class</span> <span class="nc">Spinner</span><span class="p">:</span>
 </span><span id="Spinner-223"><a href="#Spinner-223"><span class="linenos">223</span></a>    <span class="sd">&quot;&quot;&quot;Prints one of a sequence of characters in order everytime display() is called.</span>
-</span><span id="Spinner-224"><a href="#Spinner-224"><span class="linenos">224</span></a><span class="sd">    The display function writes the new character to the same line, overwriting the previous character.</span>
-</span><span id="Spinner-225"><a href="#Spinner-225"><span class="linenos">225</span></a><span class="sd">    The sequence will be cycled through indefinitely.</span>
-</span><span id="Spinner-226"><a href="#Spinner-226"><span class="linenos">226</span></a><span class="sd">    If used as a context manager, the last printed character will be cleared upon exiting.&quot;&quot;&quot;</span>
-</span><span id="Spinner-227"><a href="#Spinner-227"><span class="linenos">227</span></a>
-</span><span id="Spinner-228"><a href="#Spinner-228"><span class="linenos">228</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">sequence</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">Any</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
-</span><span id="Spinner-229"><a href="#Spinner-229"><span class="linenos">229</span></a>        <span class="sd">&quot;&quot;&quot;</span>
-</span><span id="Spinner-230"><a href="#Spinner-230"><span class="linenos">230</span></a><span class="sd">        :param sequence: Override the built in spin sequence.&quot;&quot;&quot;</span>
-</span><span id="Spinner-231"><a href="#Spinner-231"><span class="linenos">231</span></a>        <span class="k">if</span> <span class="n">sequence</span><span class="p">:</span>
-</span><span id="Spinner-232"><a href="#Spinner-232"><span class="linenos">232</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">sequence</span> <span class="o">=</span> <span class="n">sequence</span>
-</span><span id="Spinner-233"><a href="#Spinner-233"><span class="linenos">233</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="Spinner-234"><a href="#Spinner-234"><span class="linenos">234</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">sequence</span> <span class="o">=</span> <span class="p">[</span><span class="s2">&quot;/&quot;</span><span class="p">,</span> <span class="s2">&quot;-&quot;</span><span class="p">,</span> <span class="s2">&quot;</span><span class="se">\\</span><span class="s2">&quot;</span><span class="p">]</span>
-</span><span id="Spinner-235"><a href="#Spinner-235"><span class="linenos">235</span></a>
-</span><span id="Spinner-236"><a href="#Spinner-236"><span class="linenos">236</span></a>    <span class="k">def</span> <span class="fm">__enter__</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="Spinner-237"><a href="#Spinner-237"><span class="linenos">237</span></a>        <span class="k">return</span> <span class="bp">self</span>
-</span><span id="Spinner-238"><a href="#Spinner-238"><span class="linenos">238</span></a>
-</span><span id="Spinner-239"><a href="#Spinner-239"><span class="linenos">239</span></a>    <span class="k">def</span> <span class="fm">__exit__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="o">*</span><span class="n">args</span><span class="p">,</span> <span class="o">**</span><span class="n">kwargs</span><span class="p">):</span>
-</span><span id="Spinner-240"><a href="#Spinner-240"><span class="linenos">240</span></a>        <span class="n">clear</span><span class="p">()</span>
-</span><span id="Spinner-241"><a href="#Spinner-241"><span class="linenos">241</span></a>
-</span><span id="Spinner-242"><a href="#Spinner-242"><span class="linenos">242</span></a>    <span class="nd">@property</span>
-</span><span id="Spinner-243"><a href="#Spinner-243"><span class="linenos">243</span></a>    <span class="k">def</span> <span class="nf">sequence</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">Any</span><span class="p">]:</span>
-</span><span id="Spinner-244"><a href="#Spinner-244"><span class="linenos">244</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_sequence</span>
+</span><span id="Spinner-224"><a href="#Spinner-224"><span class="linenos">224</span></a>
+</span><span id="Spinner-225"><a href="#Spinner-225"><span class="linenos">225</span></a><span class="sd">    The display function writes the new character to the same line, overwriting the previous character.</span>
+</span><span id="Spinner-226"><a href="#Spinner-226"><span class="linenos">226</span></a>
+</span><span id="Spinner-227"><a href="#Spinner-227"><span class="linenos">227</span></a><span class="sd">    The sequence will be cycled through indefinitely.</span>
+</span><span id="Spinner-228"><a href="#Spinner-228"><span class="linenos">228</span></a>
+</span><span id="Spinner-229"><a href="#Spinner-229"><span class="linenos">229</span></a><span class="sd">    If used as a context manager, the last printed character will be cleared upon exiting.</span>
+</span><span id="Spinner-230"><a href="#Spinner-230"><span class="linenos">230</span></a><span class="sd">    &quot;&quot;&quot;</span>
+</span><span id="Spinner-231"><a href="#Spinner-231"><span class="linenos">231</span></a>
+</span><span id="Spinner-232"><a href="#Spinner-232"><span class="linenos">232</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span>
+</span><span id="Spinner-233"><a href="#Spinner-233"><span class="linenos">233</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">sequence</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">=</span> <span class="p">[</span><span class="s2">&quot;/&quot;</span><span class="p">,</span> <span class="s2">&quot;-&quot;</span><span class="p">,</span> <span class="s2">&quot;</span><span class="se">\\</span><span class="s2">&quot;</span><span class="p">],</span> <span class="n">width_ratio</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="mf">0.25</span>
+</span><span id="Spinner-234"><a href="#Spinner-234"><span class="linenos">234</span></a>    <span class="p">):</span>
+</span><span id="Spinner-235"><a href="#Spinner-235"><span class="linenos">235</span></a>        <span class="sd">&quot;&quot;&quot;</span>
+</span><span id="Spinner-236"><a href="#Spinner-236"><span class="linenos">236</span></a><span class="sd">        :param sequence: Override the built in spin sequence.</span>
+</span><span id="Spinner-237"><a href="#Spinner-237"><span class="linenos">237</span></a>
+</span><span id="Spinner-238"><a href="#Spinner-238"><span class="linenos">238</span></a><span class="sd">        :param width: The fractional amount of the terminal for characters to move across.&quot;&quot;&quot;</span>
+</span><span id="Spinner-239"><a href="#Spinner-239"><span class="linenos">239</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_base_sequence</span> <span class="o">=</span> <span class="n">sequence</span>
+</span><span id="Spinner-240"><a href="#Spinner-240"><span class="linenos">240</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">width_ratio</span> <span class="o">=</span> <span class="n">width_ratio</span>
+</span><span id="Spinner-241"><a href="#Spinner-241"><span class="linenos">241</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">sequence</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_base_sequence</span>
+</span><span id="Spinner-242"><a href="#Spinner-242"><span class="linenos">242</span></a>
+</span><span id="Spinner-243"><a href="#Spinner-243"><span class="linenos">243</span></a>    <span class="k">def</span> <span class="fm">__enter__</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="Spinner-244"><a href="#Spinner-244"><span class="linenos">244</span></a>        <span class="k">return</span> <span class="bp">self</span>
 </span><span id="Spinner-245"><a href="#Spinner-245"><span class="linenos">245</span></a>
-</span><span id="Spinner-246"><a href="#Spinner-246"><span class="linenos">246</span></a>    <span class="nd">@sequence</span><span class="o">.</span><span class="n">setter</span>
-</span><span id="Spinner-247"><a href="#Spinner-247"><span class="linenos">247</span></a>    <span class="k">def</span> <span class="nf">sequence</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">character_list</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">Any</span><span class="p">]):</span>
-</span><span id="Spinner-248"><a href="#Spinner-248"><span class="linenos">248</span></a>        <span class="c1"># Buffer each element with a leading space</span>
-</span><span id="Spinner-249"><a href="#Spinner-249"><span class="linenos">249</span></a>        <span class="c1"># so that the character isn&#39;t obscured by the cursor</span>
-</span><span id="Spinner-250"><a href="#Spinner-250"><span class="linenos">250</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_sequence</span> <span class="o">=</span> <span class="p">[</span><span class="s2">&quot; &quot;</span> <span class="o">+</span> <span class="nb">str</span><span class="p">(</span><span class="n">ch</span><span class="p">)</span> <span class="k">for</span> <span class="n">ch</span> <span class="ow">in</span> <span class="n">character_list</span><span class="p">]</span>
-</span><span id="Spinner-251"><a href="#Spinner-251"><span class="linenos">251</span></a>
-</span><span id="Spinner-252"><a href="#Spinner-252"><span class="linenos">252</span></a>    <span class="k">def</span> <span class="nf">_get_next</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="Spinner-253"><a href="#Spinner-253"><span class="linenos">253</span></a>        <span class="sd">&quot;&quot;&quot;Pop the first element of self._sequence,</span>
-</span><span id="Spinner-254"><a href="#Spinner-254"><span class="linenos">254</span></a><span class="sd">        append it to the end, and return the element.&quot;&quot;&quot;</span>
-</span><span id="Spinner-255"><a href="#Spinner-255"><span class="linenos">255</span></a>        <span class="n">ch</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">sequence</span><span class="o">.</span><span class="n">pop</span><span class="p">(</span><span class="mi">0</span><span class="p">)</span>
-</span><span id="Spinner-256"><a href="#Spinner-256"><span class="linenos">256</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">sequence</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">ch</span><span class="p">)</span>
-</span><span id="Spinner-257"><a href="#Spinner-257"><span class="linenos">257</span></a>        <span class="k">return</span> <span class="n">ch</span>
-</span><span id="Spinner-258"><a href="#Spinner-258"><span class="linenos">258</span></a>
-</span><span id="Spinner-259"><a href="#Spinner-259"><span class="linenos">259</span></a>    <span class="k">def</span> <span class="nf">display</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="Spinner-260"><a href="#Spinner-260"><span class="linenos">260</span></a>        <span class="sd">&quot;&quot;&quot;Print the next character in the sequence.&quot;&quot;&quot;</span>
-</span><span id="Spinner-261"><a href="#Spinner-261"><span class="linenos">261</span></a>        <span class="n">print_in_place</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_get_next</span><span class="p">())</span>
+</span><span id="Spinner-246"><a href="#Spinner-246"><span class="linenos">246</span></a>    <span class="k">def</span> <span class="fm">__exit__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="o">*</span><span class="n">args</span><span class="p">,</span> <span class="o">**</span><span class="n">kwargs</span><span class="p">):</span>
+</span><span id="Spinner-247"><a href="#Spinner-247"><span class="linenos">247</span></a>        <span class="n">clear</span><span class="p">()</span>
+</span><span id="Spinner-248"><a href="#Spinner-248"><span class="linenos">248</span></a>
+</span><span id="Spinner-249"><a href="#Spinner-249"><span class="linenos">249</span></a>    <span class="nd">@property</span>
+</span><span id="Spinner-250"><a href="#Spinner-250"><span class="linenos">250</span></a>    <span class="k">def</span> <span class="nf">width_ratio</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">float</span><span class="p">:</span>
+</span><span id="Spinner-251"><a href="#Spinner-251"><span class="linenos">251</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_width_ratio</span>
+</span><span id="Spinner-252"><a href="#Spinner-252"><span class="linenos">252</span></a>
+</span><span id="Spinner-253"><a href="#Spinner-253"><span class="linenos">253</span></a>    <span class="nd">@width_ratio</span><span class="o">.</span><span class="n">setter</span>
+</span><span id="Spinner-254"><a href="#Spinner-254"><span class="linenos">254</span></a>    <span class="k">def</span> <span class="nf">width_ratio</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">ratio</span><span class="p">:</span> <span class="nb">float</span><span class="p">):</span>
+</span><span id="Spinner-255"><a href="#Spinner-255"><span class="linenos">255</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_width_ratio</span> <span class="o">=</span> <span class="n">ratio</span>
+</span><span id="Spinner-256"><a href="#Spinner-256"><span class="linenos">256</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_update_width</span><span class="p">()</span>
+</span><span id="Spinner-257"><a href="#Spinner-257"><span class="linenos">257</span></a>
+</span><span id="Spinner-258"><a href="#Spinner-258"><span class="linenos">258</span></a>    <span class="k">def</span> <span class="nf">_update_width</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="Spinner-259"><a href="#Spinner-259"><span class="linenos">259</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_current_terminal_width</span> <span class="o">=</span> <span class="n">get_terminal_size</span><span class="p">()</span><span class="o">.</span><span class="n">columns</span>
+</span><span id="Spinner-260"><a href="#Spinner-260"><span class="linenos">260</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_width</span> <span class="o">=</span> <span class="nb">int</span><span class="p">((</span><span class="bp">self</span><span class="o">.</span><span class="n">_current_terminal_width</span> <span class="o">-</span> <span class="mi">1</span><span class="p">)</span> <span class="o">*</span> <span class="bp">self</span><span class="o">.</span><span class="n">width_ratio</span><span class="p">)</span>
+</span><span id="Spinner-261"><a href="#Spinner-261"><span class="linenos">261</span></a>
+</span><span id="Spinner-262"><a href="#Spinner-262"><span class="linenos">262</span></a>    <span class="nd">@property</span>
+</span><span id="Spinner-263"><a href="#Spinner-263"><span class="linenos">263</span></a>    <span class="k">def</span> <span class="nf">sequence</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">Any</span><span class="p">]:</span>
+</span><span id="Spinner-264"><a href="#Spinner-264"><span class="linenos">264</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_sequence</span>
+</span><span id="Spinner-265"><a href="#Spinner-265"><span class="linenos">265</span></a>
+</span><span id="Spinner-266"><a href="#Spinner-266"><span class="linenos">266</span></a>    <span class="nd">@sequence</span><span class="o">.</span><span class="n">setter</span>
+</span><span id="Spinner-267"><a href="#Spinner-267"><span class="linenos">267</span></a>    <span class="k">def</span> <span class="nf">sequence</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">character_list</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">Any</span><span class="p">]):</span>
+</span><span id="Spinner-268"><a href="#Spinner-268"><span class="linenos">268</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_sequence</span> <span class="o">=</span> <span class="p">[</span>
+</span><span id="Spinner-269"><a href="#Spinner-269"><span class="linenos">269</span></a>            <span class="n">ch</span><span class="o">.</span><span class="n">rjust</span><span class="p">(</span><span class="n">i</span> <span class="o">+</span> <span class="n">j</span><span class="p">)</span>
+</span><span id="Spinner-270"><a href="#Spinner-270"><span class="linenos">270</span></a>            <span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="mi">1</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">_width</span><span class="p">,</span> <span class="nb">len</span><span class="p">(</span><span class="n">character_list</span><span class="p">))</span>
+</span><span id="Spinner-271"><a href="#Spinner-271"><span class="linenos">271</span></a>            <span class="k">for</span> <span class="n">j</span><span class="p">,</span> <span class="n">ch</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">character_list</span><span class="p">)</span>
+</span><span id="Spinner-272"><a href="#Spinner-272"><span class="linenos">272</span></a>        <span class="p">]</span>
+</span><span id="Spinner-273"><a href="#Spinner-273"><span class="linenos">273</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_sequence</span> <span class="o">+=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_sequence</span><span class="p">[::</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span>
+</span><span id="Spinner-274"><a href="#Spinner-274"><span class="linenos">274</span></a>
+</span><span id="Spinner-275"><a href="#Spinner-275"><span class="linenos">275</span></a>    <span class="k">def</span> <span class="nf">_get_next</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="Spinner-276"><a href="#Spinner-276"><span class="linenos">276</span></a>        <span class="sd">&quot;&quot;&quot;Pop the first element of self._sequence, append it to the end, and return the element.&quot;&quot;&quot;</span>
+</span><span id="Spinner-277"><a href="#Spinner-277"><span class="linenos">277</span></a>        <span class="n">ch</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">sequence</span><span class="o">.</span><span class="n">pop</span><span class="p">(</span><span class="mi">0</span><span class="p">)</span>
+</span><span id="Spinner-278"><a href="#Spinner-278"><span class="linenos">278</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">sequence</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">ch</span><span class="p">)</span>
+</span><span id="Spinner-279"><a href="#Spinner-279"><span class="linenos">279</span></a>        <span class="k">return</span> <span class="n">ch</span>
+</span><span id="Spinner-280"><a href="#Spinner-280"><span class="linenos">280</span></a>
+</span><span id="Spinner-281"><a href="#Spinner-281"><span class="linenos">281</span></a>    <span class="k">def</span> <span class="nf">display</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="Spinner-282"><a href="#Spinner-282"><span class="linenos">282</span></a>        <span class="sd">&quot;&quot;&quot;Print the next character in the sequence.&quot;&quot;&quot;</span>
+</span><span id="Spinner-283"><a href="#Spinner-283"><span class="linenos">283</span></a>        <span class="k">if</span> <span class="n">get_terminal_size</span><span class="p">()</span><span class="o">.</span><span class="n">columns</span> <span class="o">!=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_current_terminal_width</span><span class="p">:</span>
+</span><span id="Spinner-284"><a href="#Spinner-284"><span class="linenos">284</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">_update_width</span><span class="p">()</span>
+</span><span id="Spinner-285"><a href="#Spinner-285"><span class="linenos">285</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">sequence</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_base_sequence</span>
+</span><span id="Spinner-286"><a href="#Spinner-286"><span class="linenos">286</span></a>        <span class="n">print_in_place</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_get_next</span><span class="p">())</span>
 </span></pre></div>
 
 
-            <div class="docstring"><p>Prints one of a sequence of characters in order everytime display() is called.
-The display function writes the new character to the same line, overwriting the previous character.
-The sequence will be cycled through indefinitely.
-If used as a context manager, the last printed character will be cleared upon exiting.</p>
+            <div class="docstring"><p>Prints one of a sequence of characters in order everytime display() is called.</p>
+
+<p>The display function writes the new character to the same line, overwriting the previous character.</p>
+
+<p>The sequence will be cycled through indefinitely.</p>
+
+<p>If used as a context manager, the last printed character will be cleared upon exiting.</p>
 </div>
 
 
                             <div id="Spinner.__init__" class="classattr">
                                         <input id="Spinner.__init__-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
-        <span class="name">Spinner</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">sequence</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">typing</span><span class="o">.</span><span class="n">Any</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span></span>)</span>
+        <span class="name">Spinner</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">sequence</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">=</span> <span class="p">[</span><span class="s1">&#39;/&#39;</span><span class="p">,</span> <span class="s1">&#39;-&#39;</span><span class="p">,</span> <span class="s1">&#39;</span><span class="se">\\</span><span class="s1">&#39;</span><span class="p">]</span>, </span><span class="param"><span class="n">width_ratio</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="mf">0.25</span></span>)</span>
 
                 <label class="view-source-button" for="Spinner.__init__-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Spinner.__init__"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Spinner.__init__-228"><a href="#Spinner.__init__-228"><span class="linenos">228</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">sequence</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">Any</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
-</span><span id="Spinner.__init__-229"><a href="#Spinner.__init__-229"><span class="linenos">229</span></a>        <span class="sd">&quot;&quot;&quot;</span>
-</span><span id="Spinner.__init__-230"><a href="#Spinner.__init__-230"><span class="linenos">230</span></a><span class="sd">        :param sequence: Override the built in spin sequence.&quot;&quot;&quot;</span>
-</span><span id="Spinner.__init__-231"><a href="#Spinner.__init__-231"><span class="linenos">231</span></a>        <span class="k">if</span> <span class="n">sequence</span><span class="p">:</span>
-</span><span id="Spinner.__init__-232"><a href="#Spinner.__init__-232"><span class="linenos">232</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">sequence</span> <span class="o">=</span> <span class="n">sequence</span>
-</span><span id="Spinner.__init__-233"><a href="#Spinner.__init__-233"><span class="linenos">233</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="Spinner.__init__-234"><a href="#Spinner.__init__-234"><span class="linenos">234</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">sequence</span> <span class="o">=</span> <span class="p">[</span><span class="s2">&quot;/&quot;</span><span class="p">,</span> <span class="s2">&quot;-&quot;</span><span class="p">,</span> <span class="s2">&quot;</span><span class="se">\\</span><span class="s2">&quot;</span><span class="p">]</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Spinner.__init__-232"><a href="#Spinner.__init__-232"><span class="linenos">232</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span>
+</span><span id="Spinner.__init__-233"><a href="#Spinner.__init__-233"><span class="linenos">233</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">sequence</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">=</span> <span class="p">[</span><span class="s2">&quot;/&quot;</span><span class="p">,</span> <span class="s2">&quot;-&quot;</span><span class="p">,</span> <span class="s2">&quot;</span><span class="se">\\</span><span class="s2">&quot;</span><span class="p">],</span> <span class="n">width_ratio</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="mf">0.25</span>
+</span><span id="Spinner.__init__-234"><a href="#Spinner.__init__-234"><span class="linenos">234</span></a>    <span class="p">):</span>
+</span><span id="Spinner.__init__-235"><a href="#Spinner.__init__-235"><span class="linenos">235</span></a>        <span class="sd">&quot;&quot;&quot;</span>
+</span><span id="Spinner.__init__-236"><a href="#Spinner.__init__-236"><span class="linenos">236</span></a><span class="sd">        :param sequence: Override the built in spin sequence.</span>
+</span><span id="Spinner.__init__-237"><a href="#Spinner.__init__-237"><span class="linenos">237</span></a>
+</span><span id="Spinner.__init__-238"><a href="#Spinner.__init__-238"><span class="linenos">238</span></a><span class="sd">        :param width: The fractional amount of the terminal for characters to move across.&quot;&quot;&quot;</span>
+</span><span id="Spinner.__init__-239"><a href="#Spinner.__init__-239"><span class="linenos">239</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_base_sequence</span> <span class="o">=</span> <span class="n">sequence</span>
+</span><span id="Spinner.__init__-240"><a href="#Spinner.__init__-240"><span class="linenos">240</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">width_ratio</span> <span class="o">=</span> <span class="n">width_ratio</span>
+</span><span id="Spinner.__init__-241"><a href="#Spinner.__init__-241"><span class="linenos">241</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">sequence</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_base_sequence</span>
 </span></pre></div>
 
 
             <div class="docstring"><h6 id="parameters">Parameters</h6>
 
 <ul>
-<li><strong>sequence</strong>:  Override the built in spin sequence.</li>
+<li><p><strong>sequence</strong>:  Override the built in spin sequence.</p></li>
+<li><p><strong>width</strong>:  The fractional amount of the terminal for characters to move across.</p></li>
 </ul>
 </div>
 
 
                             </div>
                             <div id="Spinner.display" class="classattr">
                                         <input id="Spinner.display-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
@@ -1030,17 +1087,20 @@
         <span class="def">def</span>
         <span class="name">display</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="Spinner.display-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Spinner.display"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Spinner.display-259"><a href="#Spinner.display-259"><span class="linenos">259</span></a>    <span class="k">def</span> <span class="nf">display</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="Spinner.display-260"><a href="#Spinner.display-260"><span class="linenos">260</span></a>        <span class="sd">&quot;&quot;&quot;Print the next character in the sequence.&quot;&quot;&quot;</span>
-</span><span id="Spinner.display-261"><a href="#Spinner.display-261"><span class="linenos">261</span></a>        <span class="n">print_in_place</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_get_next</span><span class="p">())</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Spinner.display-281"><a href="#Spinner.display-281"><span class="linenos">281</span></a>    <span class="k">def</span> <span class="nf">display</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="Spinner.display-282"><a href="#Spinner.display-282"><span class="linenos">282</span></a>        <span class="sd">&quot;&quot;&quot;Print the next character in the sequence.&quot;&quot;&quot;</span>
+</span><span id="Spinner.display-283"><a href="#Spinner.display-283"><span class="linenos">283</span></a>        <span class="k">if</span> <span class="n">get_terminal_size</span><span class="p">()</span><span class="o">.</span><span class="n">columns</span> <span class="o">!=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_current_terminal_width</span><span class="p">:</span>
+</span><span id="Spinner.display-284"><a href="#Spinner.display-284"><span class="linenos">284</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">_update_width</span><span class="p">()</span>
+</span><span id="Spinner.display-285"><a href="#Spinner.display-285"><span class="linenos">285</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">sequence</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_base_sequence</span>
+</span><span id="Spinner.display-286"><a href="#Spinner.display-286"><span class="linenos">286</span></a>        <span class="n">print_in_place</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_get_next</span><span class="p">())</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Print the next character in the sequence.</p>
 </div>
```

#### html2text {}

```diff
@@ -253,54 +253,83 @@
 217        self.counter += 1
 218        return return_object
 219
 220
 221class Spinner:
 222    """Prints one of a sequence of characters in order everytime display()
 is called.
-223    The display function writes the new character to the same line,
+223
+224    The display function writes the new character to the same line,
 overwriting the previous character.
-224    The sequence will be cycled through indefinitely.
-225    If used as a context manager, the last printed character will be cleared
-upon exiting."""
-226
-227    def __init__(self, sequence: list[Any] | None = None):
-228        """
-229        :param sequence: Override the built in spin sequence."""
-230        if sequence:
-231            self.sequence = sequence
-232        else:
-233            self.sequence = ["/", "-", "\\"]
-234
-235    def __enter__(self):
-236        return self
-237
-238    def __exit__(self, *args, **kwargs):
-239        clear()
-240
-241    @property
-242    def sequence(self) -> list[Any]:
-243        return self._sequence
+225
+226    The sequence will be cycled through indefinitely.
+227
+228    If used as a context manager, the last printed character will be cleared
+upon exiting.
+229    """
+230
+231    def __init__(
+232        self, sequence: list[str] = ["/", "-", "\\"], width_ratio: float =
+0.25
+233    ):
+234        """
+235        :param sequence: Override the built in spin sequence.
+236
+237        :param width: The fractional amount of the terminal for characters
+to move across."""
+238        self._base_sequence = sequence
+239        self.width_ratio = width_ratio
+240        self.sequence = self._base_sequence
+241
+242    def __enter__(self):
+243        return self
 244
-245    @sequence.setter
-246    def sequence(self, character_list: list[Any]):
-247        # Buffer each element with a leading space
-248        # so that the character isn't obscured by the cursor
-249        self._sequence = [" " + str(ch) for ch in character_list]
-250
-251    def _get_next(self) -> str:
-252        """Pop the first element of self._sequence,
-253        append it to the end, and return the element."""
-254        ch = self.sequence.pop(0)
-255        self.sequence.append(ch)
-256        return ch
-257
-258    def display(self):
-259        """Print the next character in the sequence."""
-260        print_in_place(self._get_next())
+245    def __exit__(self, *args, **kwargs):
+246        clear()
+247
+248    @property
+249    def width_ratio(self) -> float:
+250        return self._width_ratio
+251
+252    @width_ratio.setter
+253    def width_ratio(self, ratio: float):
+254        self._width_ratio = ratio
+255        self._update_width()
+256
+257    def _update_width(self):
+258        self._current_terminal_width = get_terminal_size().columns
+259        self._width = int((self._current_terminal_width - 1) *
+self.width_ratio)
+260
+261    @property
+262    def sequence(self) -> list[Any]:
+263        return self._sequence
+264
+265    @sequence.setter
+266    def sequence(self, character_list: list[Any]):
+267        self._sequence = [
+268            ch.rjust(i + j)
+269            for i in range(1, self._width, len(character_list))
+270            for j, ch in enumerate(character_list)
+271        ]
+272        self._sequence += self._sequence[::-1]
+273
+274    def _get_next(self) -> str:
+275        """Pop the first element of self._sequence, append it to the end,
+and return the element."""
+276        ch = self.sequence.pop(0)
+277        self.sequence.append(ch)
+278        return ch
+279
+280    def display(self):
+281        """Print the next character in the sequence."""
+282        if get_terminal_size().columns != self._current_terminal_width:
+283            self._update_width()
+284            self.sequence = self._base_sequence
+285        print_in_place(self._get_next())
   ⁰
 def clear(): View Source
 _9def clear():
 10    """Erase the current line from the terminal."""
 11    print(" " * (get_terminal_size().columns - 1), flush=True, end="\r")
 Erase the current line from the terminal.
   ⁰
@@ -745,69 +774,111 @@
 >>> myList
 >>> [0, 1, 4, 9, 16, 25, 36, 49, 64, 81]
   ⁰
 class Spinner: View Source
 222class Spinner:
 223    """Prints one of a sequence of characters in order everytime display()
 is called.
-224    The display function writes the new character to the same line,
+224
+225    The display function writes the new character to the same line,
 overwriting the previous character.
-225    The sequence will be cycled through indefinitely.
-226    If used as a context manager, the last printed character will be cleared
-upon exiting."""
-227
-228    def __init__(self, sequence: list[Any] | None = None):
-229        """
-230        :param sequence: Override the built in spin sequence."""
-231        if sequence:
-232            self.sequence = sequence
-233        else:
-234            self.sequence = ["/", "-", "\\"]
-235
-236    def __enter__(self):
-237        return self
-238
-239    def __exit__(self, *args, **kwargs):
-240        clear()
-241
-242    @property
-243    def sequence(self) -> list[Any]:
-244        return self._sequence
+226
+227    The sequence will be cycled through indefinitely.
+228
+229    If used as a context manager, the last printed character will be cleared
+upon exiting.
+230    """
+231
+232    def __init__(
+233        self, sequence: list[str] = ["/", "-", "\\"], width_ratio: float =
+0.25
+234    ):
+235        """
+236        :param sequence: Override the built in spin sequence.
+237
+238        :param width: The fractional amount of the terminal for characters
+to move across."""
+239        self._base_sequence = sequence
+240        self.width_ratio = width_ratio
+241        self.sequence = self._base_sequence
+242
+243    def __enter__(self):
+244        return self
 245
-246    @sequence.setter
-247    def sequence(self, character_list: list[Any]):
-248        # Buffer each element with a leading space
-249        # so that the character isn't obscured by the cursor
-250        self._sequence = [" " + str(ch) for ch in character_list]
-251
-252    def _get_next(self) -> str:
-253        """Pop the first element of self._sequence,
-254        append it to the end, and return the element."""
-255        ch = self.sequence.pop(0)
-256        self.sequence.append(ch)
-257        return ch
-258
-259    def display(self):
-260        """Print the next character in the sequence."""
-261        print_in_place(self._get_next())
+246    def __exit__(self, *args, **kwargs):
+247        clear()
+248
+249    @property
+250    def width_ratio(self) -> float:
+251        return self._width_ratio
+252
+253    @width_ratio.setter
+254    def width_ratio(self, ratio: float):
+255        self._width_ratio = ratio
+256        self._update_width()
+257
+258    def _update_width(self):
+259        self._current_terminal_width = get_terminal_size().columns
+260        self._width = int((self._current_terminal_width - 1) *
+self.width_ratio)
+261
+262    @property
+263    def sequence(self) -> list[Any]:
+264        return self._sequence
+265
+266    @sequence.setter
+267    def sequence(self, character_list: list[Any]):
+268        self._sequence = [
+269            ch.rjust(i + j)
+270            for i in range(1, self._width, len(character_list))
+271            for j, ch in enumerate(character_list)
+272        ]
+273        self._sequence += self._sequence[::-1]
+274
+275    def _get_next(self) -> str:
+276        """Pop the first element of self._sequence, append it to the end,
+and return the element."""
+277        ch = self.sequence.pop(0)
+278        self.sequence.append(ch)
+279        return ch
+280
+281    def display(self):
+282        """Print the next character in the sequence."""
+283        if get_terminal_size().columns != self._current_terminal_width:
+284            self._update_width()
+285            self.sequence = self._base_sequence
+286        print_in_place(self._get_next())
 Prints one of a sequence of characters in order everytime display() is called.
 The display function writes the new character to the same line, overwriting the
-previous character. The sequence will be cycled through indefinitely. If used
-as a context manager, the last printed character will be cleared upon exiting.
+previous character.
+The sequence will be cycled through indefinitely.
+If used as a context manager, the last printed character will be cleared upon
+exiting.
 ⁰
-Spinner(sequence: list[typing.Any] | None = None) View Source
-228    def __init__(self, sequence: list[Any] | None = None):
-229        """
-230        :param sequence: Override the built in spin sequence."""
-231        if sequence:
-232            self.sequence = sequence
-233        else:
-234            self.sequence = ["/", "-", "\\"]
+Spinner(sequence: list[str] = ['/', '-', '\\'], width_ratio: float = 0.25) View
+Source
+232    def __init__(
+233        self, sequence: list[str] = ["/", "-", "\\"], width_ratio: float =
+0.25
+234    ):
+235        """
+236        :param sequence: Override the built in spin sequence.
+237
+238        :param width: The fractional amount of the terminal for characters
+to move across."""
+239        self._base_sequence = sequence
+240        self.width_ratio = width_ratio
+241        self.sequence = self._base_sequence
 * Parameters *
     * sequence: Override the built in spin sequence.
+    * width: The fractional amount of the terminal for characters to move
+      across.
 ⁰
 def display(self): View Source
-259    def display(self):
-260        """Print the next character in the sequence."""
-261        print_in_place(self._get_next())
+281    def display(self):
+282        """Print the next character in the sequence."""
+283        if get_terminal_size().columns != self._current_terminal_width:
+284            self._update_width()
+285            self.sequence = self._base_sequence
+286        print_in_place(self._get_next())
 Print the next character in the sequence.
```

### Comparing `printbuddies-1.2.0/src/printbuddies/printbuddies.py` & `printbuddies-1.3.0/src/printbuddies/printbuddies.py`

 * *Files 3% similar despite different names*

```diff
@@ -216,45 +216,70 @@
                     print()
         self.counter += 1
         return return_object
 
 
 class Spinner:
     """Prints one of a sequence of characters in order everytime display() is called.
+
     The display function writes the new character to the same line, overwriting the previous character.
+
     The sequence will be cycled through indefinitely.
-    If used as a context manager, the last printed character will be cleared upon exiting."""
 
-    def __init__(self, sequence: list[Any] | None = None):
+    If used as a context manager, the last printed character will be cleared upon exiting.
+    """
+
+    def __init__(
+        self, sequence: list[str] = ["/", "-", "\\"], width_ratio: float = 0.25
+    ):
         """
-        :param sequence: Override the built in spin sequence."""
-        if sequence:
-            self.sequence = sequence
-        else:
-            self.sequence = ["/", "-", "\\"]
+        :param sequence: Override the built in spin sequence.
+
+        :param width: The fractional amount of the terminal for characters to move across."""
+        self._base_sequence = sequence
+        self.width_ratio = width_ratio
+        self.sequence = self._base_sequence
 
     def __enter__(self):
         return self
 
     def __exit__(self, *args, **kwargs):
         clear()
 
     @property
+    def width_ratio(self) -> float:
+        return self._width_ratio
+
+    @width_ratio.setter
+    def width_ratio(self, ratio: float):
+        self._width_ratio = ratio
+        self._update_width()
+
+    def _update_width(self):
+        self._current_terminal_width = get_terminal_size().columns
+        self._width = int((self._current_terminal_width - 1) * self.width_ratio)
+
+    @property
     def sequence(self) -> list[Any]:
         return self._sequence
 
     @sequence.setter
     def sequence(self, character_list: list[Any]):
-        # Buffer each element with a leading space
-        # so that the character isn't obscured by the cursor
-        self._sequence = [" " + str(ch) for ch in character_list]
+        self._sequence = [
+            ch.rjust(i + j)
+            for i in range(1, self._width, len(character_list))
+            for j, ch in enumerate(character_list)
+        ]
+        self._sequence += self._sequence[::-1]
 
     def _get_next(self) -> str:
-        """Pop the first element of self._sequence,
-        append it to the end, and return the element."""
+        """Pop the first element of self._sequence, append it to the end, and return the element."""
         ch = self.sequence.pop(0)
         self.sequence.append(ch)
         return ch
 
     def display(self):
         """Print the next character in the sequence."""
+        if get_terminal_size().columns != self._current_terminal_width:
+            self._update_width()
+            self.sequence = self._base_sequence
         print_in_place(self._get_next())
```

### Comparing `printbuddies-1.2.0/LICENSE.txt` & `printbuddies-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `printbuddies-1.2.0/README.md` & `printbuddies-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `printbuddies-1.2.0/pyproject.toml` & `printbuddies-1.3.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "printbuddies"
 authors = [{name="Matt Manes"}]
 description = "Handful of utilities to do printing tricks to the terminal."
-version = "1.2.0"
+version = "1.3.0"
 requires-python = ">=3.10"
 dependencies = ["noiftimer", "pytest"]
 readme = "README.md"
 keywords = [
     "terminal",
     "print",
     "printing",
```

### Comparing `printbuddies-1.2.0/PKG-INFO` & `printbuddies-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: printbuddies
-Version: 1.2.0
+Version: 1.3.0
 Summary: Handful of utilities to do printing tricks to the terminal.
 Project-URL: Homepage, https://github.com/matt-manes/printbuddies
 Project-URL: Documentation, https://github.com/matt-manes/printbuddies/tree/main/docs
 Project-URL: Source code, https://github.com/matt-manes/printbuddies/tree/main/src/printbuddies
 Author: Matt Manes
 License-File: LICENSE.txt
 Keywords: print,printing,progressbar,terminal
```

