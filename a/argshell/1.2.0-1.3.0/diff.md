# Comparing `tmp/argshell-1.2.0.tar.gz` & `tmp/argshell-1.3.0.tar.gz`

## Comparing `argshell-1.2.0.tar` & `argshell-1.3.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 argshell-1.2.0/CHANGELOG.md
--rw-r--r--   0        0        0    34238 2020-02-02 00:00:00.000000 argshell-1.2.0/docs/argshell.html
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 argshell-1.2.0/docs/index.html
--rw-r--r--   0        0        0    38481 2020-02-02 00:00:00.000000 argshell-1.2.0/docs/search.js
--rw-r--r--   0        0        0   210283 2020-02-02 00:00:00.000000 argshell-1.2.0/docs/argshell/argshell.html
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 argshell-1.2.0/src/argshell/__init__.py
--rw-r--r--   0        0        0    10789 2020-02-02 00:00:00.000000 argshell-1.2.0/src/argshell/argshell.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 argshell-1.2.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 argshell-1.2.0/LICENSE.txt
--rw-r--r--   0        0        0     6051 2020-02-02 00:00:00.000000 argshell-1.2.0/README.md
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 argshell-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     6550 2020-02-02 00:00:00.000000 argshell-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 argshell-1.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0    34238 2020-02-02 00:00:00.000000 argshell-1.3.0/docs/argshell.html
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 argshell-1.3.0/docs/index.html
+-rw-r--r--   0        0        0    38989 2020-02-02 00:00:00.000000 argshell-1.3.0/docs/search.js
+-rw-r--r--   0        0        0   212638 2020-02-02 00:00:00.000000 argshell-1.3.0/docs/argshell/argshell.html
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 argshell-1.3.0/src/argshell/__init__.py
+-rw-r--r--   0        0        0    10830 2020-02-02 00:00:00.000000 argshell-1.3.0/src/argshell/argshell.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 argshell-1.3.0/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 argshell-1.3.0/LICENSE.txt
+-rw-r--r--   0        0        0     6051 2020-02-02 00:00:00.000000 argshell-1.3.0/README.md
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 argshell-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6550 2020-02-02 00:00:00.000000 argshell-1.3.0/PKG-INFO
```

### Comparing `argshell-1.2.0/CHANGELOG.md` & `argshell-1.3.0/CHANGELOG.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,27 @@
 # Changelog
 
-## 1.0.0 (2023-04-27)
+## 1.2.0 (2023-05-02)
+
+#### New Features
+
+* add do_sys command to built in commands
+
+
+## v1.1.0 (2023-04-27)
 
 #### Fixes
 
 * fix double printing parser help for parsers with positional args
 #### Performance improvements
 
 * override cmdloop so shell doesn't exit on exception
+#### Others
+
+* build v1.1.0
 
 
 ## v1.0.0 (2023-04-23)
 
 #### New Features
 
 * print parser help and block decorated function execution on parser error
@@ -26,14 +36,15 @@
 * better type checker appeasement
 #### Docs
 
 * write readme
 * update docstrings
 #### Others
 
+* test build
 * build v1.0.0
 * update with_parser doc string
 
 
 ## v0.0.0 (2023-04-20)
 
 #### Others
```

### Comparing `argshell-1.2.0/docs/argshell.html` & `argshell-1.3.0/docs/argshell.html`

 * *Files identical despite different names*

### Comparing `argshell-1.2.0/docs/search.js` & `argshell-1.3.0/docs/search.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -766,14 +766,22 @@
         "modulename": "argshell.argshell",
         "qualname": "ArgShell.cmdloop",
         "kind": "function",
         "doc": "<p>Repeatedly issue a prompt, accept input, parse an initial prefix\noff the received input, and dispatch to action methods, passing them\nthe remainder of the line as argument.</p>\n",
         "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span>, </span><span class=\"param\"><span class=\"n\">intro</span><span class=\"o\">=</span><span class=\"kc\">None</span></span><span class=\"return-annotation\">):</span></span>",
         "funcdef": "def"
     }, {
+        "fullname": "argshell.argshell.ArgShell.emptyline",
+        "modulename": "argshell.argshell",
+        "qualname": "ArgShell.emptyline",
+        "kind": "function",
+        "doc": "<p>Called when an empty line is entered in response to the prompt.</p>\n\n<p>If this method is not overridden, it repeats the last nonempty\ncommand entered.</p>\n",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span></span><span class=\"return-annotation\">):</span></span>",
+        "funcdef": "def"
+    }, {
         "fullname": "argshell.argshell.with_parser",
         "modulename": "argshell.argshell",
         "qualname": "with_parser",
         "kind": "function",
         "doc": "<p>Decorate a 'do_*' function in an argshell.ArgShell class with this function to pass an argshell.Namespace object to the decorated function instead of a string.</p>\n\n<h6 id=\"parameters\">Parameters</h6>\n\n<ul>\n<li><p><strong>parser</strong>:  A function that creates an argshell.ArgShellParser instance, adds arguments to it, and returns the parser.</p></li>\n<li><p><strong>post_parsers</strong>:  An optional list of functions to execute where each function takes an argshell.Namespace instance and returns an argshell.Namespace instance.\n'post_parser' functions are executed in the order they are supplied.</p></li>\n</ul>\n\n<div class=\"pdoc-code codehilite\">\n<pre><span></span><code><span class=\"gp\">&gt;&gt;&gt; </span><span class=\"k\">def</span> <span class=\"nf\">get_parser</span><span class=\"p\">()</span> <span class=\"o\">-&gt;</span> <span class=\"n\">argshell</span><span class=\"o\">.</span><span class=\"n\">ArgShellParser</span><span class=\"p\">:</span>\n<span class=\"gp\">&gt;&gt;&gt; </span>    <span class=\"n\">parser</span> <span class=\"o\">=</span> <span class=\"n\">argshell</span><span class=\"o\">.</span><span class=\"n\">ArgShellParser</span><span class=\"p\">()</span>\n<span class=\"gp\">&gt;&gt;&gt; </span>    <span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">add_argument</span><span class=\"p\">(</span><span class=\"s2\">&quot;names&quot;</span><span class=\"p\">,</span> <span class=\"nb\">type</span><span class=\"o\">=</span><span class=\"nb\">str</span><span class=\"p\">,</span> <span class=\"n\">nargs</span><span class=\"o\">=</span><span class=\"s2\">&quot;*&quot;</span><span class=\"p\">,</span> <span class=\"n\">help</span><span class=\"o\">=</span><span class=\"s2\">&quot;A list of first and last names to print.&quot;</span><span class=\"p\">)</span>\n<span class=\"gp\">&gt;&gt;&gt; </span>    <span class=\"n\">parser</span><span class=\"o\">.</span><span class=\"n\">add_argument</span><span class=\"p\">(</span><span class=\"s2\">&quot;-i&quot;</span><span class=\"p\">,</span> <span class=\"s2\">&quot;--initials&quot;</span><span class=\"p\">,</span> <span class=\"n\">action</span><span class=\"o\">=</span><span class=\"s2\">&quot;store_true&quot;</span><span class=\"p\">,</span> <span class=\"n\">help</span><span class=\"o\">=</span><span class=\"s2\">&quot;Print the initials instead of the full name.&quot;</span><span class=\"p\">)</span>\n<span class=\"gp\">&gt;&gt;&gt; </span>    <span class=\"k\">return</span> <span class=\"n\">parser</span>\n<span class=\"go\">&gt;&gt;&gt;</span>\n<span class=\"gp\">&gt;&gt;&gt; </span><span class=\"c1\"># Convert list of first and last names to a list of tuples</span>\n<span class=\"gp\">&gt;&gt;&gt; </span><span class=\"k\">def</span> <span class=\"nf\">names_list_to_tuples</span><span class=\"p\">(</span><span class=\"n\">args</span><span class=\"p\">:</span> <span class=\"n\">argshell</span><span class=\"o\">.</span><span class=\"n\">Namespace</span><span class=\"p\">)</span> <span class=\"o\">-&gt;</span> <span class=\"n\">argshell</span><span class=\"o\">.</span><span class=\"n\">Namespace</span><span class=\"p\">:</span>\n<span class=\"gp\">&gt;&gt;&gt; </span>    <span class=\"n\">args</span><span class=\"o\">.</span><span class=\"n\">names</span> <span class=\"o\">=</span> <span class=\"p\">[(</span><span class=\"n\">first</span><span class=\"p\">,</span> <span class=\"n\">last</span><span class=\"p\">)</span> <span class=\"k\">for</span> <span class=\"n\">first</span><span class=\"p\">,</span> <span class=\"n\">last</span> <span class=\"ow\">in</span> <span class=\"nb\">zip</span><span class=\"p\">(</span><span class=\"n\">args</span><span class=\"o\">.</span><span class=\"n\">names</span><span class=\"p\">[::</span><span class=\"mi\">2</span><span class=\"p\">],</span> <span class=\"n\">args</span><span class=\"o\">.</span><span class=\"n\">names</span><span class=\"p\">[</span><span class=\"mi\">1</span><span class=\"p\">::</span><span class=\"mi\">2</span><span class=\"p\">])]</span>\n<span class=\"gp\">&gt;&gt;&gt; </span>    <span class=\"k\">if</span> <span class=\"n\">args</span><span class=\"o\">.</span><span class=\"n\">initials</span><span class=\"p\">:</span>\n<span class=\"gp\">&gt;&gt;&gt; </span>        <span class=\"n\">args</span><span class=\"o\">.</span><span class=\"n\">names</span> <span class=\"o\">=</span> <span class=\"p\">[(</span><span class=\"n\">name</span><span class=\"p\">[</span><span class=\"mi\">0</span><span class=\"p\">][</span><span class=\"mi\">0</span><span class=\"p\">],</span> <span class=\"n\">name</span><span class=\"p\">[</span><span class=\"mi\">1</span><span class=\"p\">][</span><span class=\"mi\">0</span><span class=\"p\">])</span> <span class=\"k\">for</span> <span class=\"n\">name</span> <span class=\"ow\">in</span> <span class=\"n\">args</span><span class=\"o\">.</span><span class=\"n\">names</span><span class=\"p\">]</span>\n<span class=\"gp\">&gt;&gt;&gt; </span>    <span class=\"k\">return</span> <span class=\"n\">args</span>\n<span class=\"go\">&gt;&gt;&gt;</span>\n<span class=\"gp\">&gt;&gt;&gt; </span><span class=\"k\">def</span> <span class=\"nf\">capitalize_names</span><span class=\"p\">(</span><span class=\"n\">args</span><span class=\"p\">:</span> <span class=\"n\">argshell</span><span class=\"o\">.</span><span class=\"n\">Namespace</span><span class=\"p\">)</span> <span class=\"o\">-&gt;</span> <span class=\"n\">argshell</span><span class=\"o\">.</span><span class=\"n\">Namespace</span><span class=\"p\">:</span>\n<span class=\"gp\">&gt;&gt;&gt; </span>    <span class=\"n\">args</span><span class=\"o\">.</span><span class=\"n\">names</span> <span class=\"o\">=</span> <span class=\"p\">[</span><span class=\"n\">name</span><span class=\"o\">.</span><span class=\"n\">capitalize</span><span class=\"p\">()</span> <span class=\"k\">for</span> <span class=\"n\">name</span> <span class=\"ow\">in</span> <span class=\"n\">args</span><span class=\"o\">.</span><span class=\"n\">names</span><span class=\"p\">]</span>\n<span class=\"gp\">&gt;&gt;&gt; </span>    <span class=\"k\">return</span> <span class=\"n\">args</span>\n<span class=\"go\">&gt;&gt;&gt;</span>\n<span class=\"gp\">&gt;&gt;&gt; </span><span class=\"k\">class</span> <span class=\"nc\">NameShell</span><span class=\"p\">(</span><span class=\"n\">ArgShell</span><span class=\"p\">):</span>\n<span class=\"gp\">&gt;&gt;&gt; </span>    <span class=\"n\">intro</span> <span class=\"o\">=</span> <span class=\"s2\">&quot;Entering nameshell...&quot;</span>\n<span class=\"gp\">&gt;&gt;&gt; </span>    <span class=\"n\">prompt</span> <span class=\"o\">=</span> <span class=\"s2\">&quot;nameshell&gt;&quot;</span>\n<span class=\"go\">&gt;&gt;&gt;</span>\n<span class=\"gp\">&gt;&gt;&gt; </span>    <span class=\"nd\">@with_parser</span><span class=\"p\">(</span><span class=\"n\">get_parser</span><span class=\"p\">,</span> <span class=\"p\">[</span><span class=\"n\">capitalize_names</span><span class=\"p\">,</span> <span class=\"n\">names_list_to_tuples</span><span class=\"p\">])</span>\n<span class=\"gp\">&gt;&gt;&gt; </span>    <span class=\"k\">def</span> <span class=\"nf\">do_printnames</span><span class=\"p\">(</span><span class=\"bp\">self</span><span class=\"p\">,</span> <span class=\"n\">args</span><span class=\"p\">:</span> <span class=\"n\">argshell</span><span class=\"o\">.</span><span class=\"n\">Namespace</span><span class=\"p\">):</span>\n<span class=\"gp\">&gt;&gt;&gt; </span>        <span class=\"nb\">print</span><span class=\"p\">(</span><span class=\"o\">*</span><span class=\"p\">[</span><span class=\"sa\">f</span><span class=\"s2\">&quot;</span><span class=\"si\">{</span><span class=\"n\">name</span><span class=\"p\">[</span><span class=\"mi\">0</span><span class=\"p\">]</span><span class=\"si\">}</span><span class=\"s2\"> </span><span class=\"si\">{</span><span class=\"n\">name</span><span class=\"p\">[</span><span class=\"mi\">1</span><span class=\"p\">]</span><span class=\"si\">}</span><span class=\"s2\">&quot;</span> <span class=\"k\">for</span> <span class=\"n\">name</span> <span class=\"ow\">in</span> <span class=\"n\">args</span><span class=\"o\">.</span><span class=\"n\">names</span><span class=\"p\">],</span> <span class=\"n\">sep</span><span class=\"o\">=</span><span class=\"s2\">&quot;</span><span class=\"se\">\\n</span><span class=\"s2\">&quot;</span><span class=\"p\">)</span>\n<span class=\"go\">&gt;&gt;&gt;</span>\n<span class=\"gp\">&gt;&gt;&gt; </span><span class=\"n\">NameShell</span><span class=\"p\">()</span><span class=\"o\">.</span><span class=\"n\">cmdloop</span><span class=\"p\">()</span>\n<span class=\"gp\">&gt;&gt;&gt; </span><span class=\"n\">Entering</span> <span class=\"n\">nameshell</span><span class=\"o\">...</span>\n<span class=\"gp\">&gt;&gt;&gt; </span><span class=\"n\">nameshell</span><span class=\"o\">&gt;</span><span class=\"n\">printnames</span> <span class=\"n\">karl</span> <span class=\"n\">marx</span> <span class=\"n\">fred</span> <span class=\"n\">hampton</span> <span class=\"n\">emma</span> <span class=\"n\">goldman</span> <span class=\"n\">angela</span> <span class=\"n\">davis</span> <span class=\"n\">nestor</span> <span class=\"n\">makhno</span>\n<span class=\"gp\">&gt;&gt;&gt; </span><span class=\"n\">Karl</span> <span class=\"n\">Marx</span>\n<span class=\"gp\">&gt;&gt;&gt; </span><span class=\"n\">Fred</span> <span class=\"n\">Hampton</span>\n<span class=\"gp\">&gt;&gt;&gt; </span><span class=\"n\">Emma</span> <span class=\"n\">Goldman</span>\n<span class=\"gp\">&gt;&gt;&gt; </span><span class=\"n\">Angela</span> <span class=\"n\">Davis</span>\n<span class=\"gp\">&gt;&gt;&gt; </span><span class=\"n\">Nestor</span> <span class=\"n\">Makhno</span>\n<span class=\"gp\">&gt;&gt;&gt; </span><span class=\"n\">nameshell</span><span class=\"o\">&gt;</span><span class=\"n\">printnames</span> <span class=\"n\">karl</span> <span class=\"n\">marx</span> <span class=\"n\">fred</span> <span class=\"n\">hampton</span> <span class=\"n\">emma</span> <span class=\"n\">goldman</span> <span class=\"n\">angela</span> <span class=\"n\">davis</span> <span class=\"n\">nestor</span> <span class=\"n\">makhno</span> <span class=\"o\">-</span><span class=\"n\">i</span>\n<span class=\"gp\">&gt;&gt;&gt; </span><span class=\"n\">K</span> <span class=\"n\">M</span>\n<span class=\"gp\">&gt;&gt;&gt; </span><span class=\"n\">F</span> <span class=\"n\">H</span>\n<span class=\"gp\">&gt;&gt;&gt; </span><span class=\"n\">E</span> <span class=\"n\">G</span>\n<span class=\"gp\">&gt;&gt;&gt; </span><span class=\"n\">A</span> <span class=\"n\">D</span>\n<span class=\"gp\">&gt;&gt;&gt; </span><span class=\"n\">N</span> <span class=\"n\">M</span>\n</code></pre>\n</div>\n",
         "signature": "<span class=\"signature pdoc-code multiline\">(<span class=\"param\">\t<span class=\"n\">parser</span><span class=\"p\">:</span> <span class=\"n\">Callable</span><span class=\"p\">[</span><span class=\"o\">...</span><span class=\"p\">,</span> <span class=\"n\">argshell</span><span class=\"o\">.</span><span class=\"n\">argshell</span><span class=\"o\">.</span><span class=\"n\">ArgShellParser</span><span class=\"p\">]</span>,</span><span class=\"param\">\t<span class=\"n\">post_parsers</span><span class=\"p\">:</span> <span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"n\">typing</span><span class=\"o\">.</span><span class=\"n\">Callable</span><span class=\"p\">[[</span><span class=\"n\">argshell</span><span class=\"o\">.</span><span class=\"n\">argshell</span><span class=\"o\">.</span><span class=\"n\">Namespace</span><span class=\"p\">],</span> <span class=\"n\">argshell</span><span class=\"o\">.</span><span class=\"n\">argshell</span><span class=\"o\">.</span><span class=\"n\">Namespace</span><span class=\"p\">]]</span> <span class=\"o\">=</span> <span class=\"p\">[]</span></span><span class=\"return-annotation\">) -> <span class=\"n\">Callable</span><span class=\"p\">[[</span><span class=\"n\">Callable</span><span class=\"p\">[[</span><span class=\"n\">Any</span><span class=\"p\">,</span> <span class=\"n\">argshell</span><span class=\"o\">.</span><span class=\"n\">argshell</span><span class=\"o\">.</span><span class=\"n\">Namespace</span><span class=\"p\">],</span> <span class=\"n\">Any</span><span class=\"p\">]],</span> <span class=\"n\">Callable</span><span class=\"p\">[[</span><span class=\"n\">Any</span><span class=\"p\">,</span> <span class=\"nb\">str</span><span class=\"p\">],</span> <span class=\"n\">Any</span><span class=\"p\">]]</span>:</span></span>",
         "funcdef": "def"
```

### Comparing `argshell-1.2.0/docs/argshell/argshell.html` & `argshell-1.3.0/docs/argshell/argshell.html`

 * *Files 0% similar despite different names*

```diff
@@ -62,14 +62,17 @@
                         </li>
                         <li>
                                 <a class="function" href="#ArgShell.do_help">do_help</a>
                         </li>
                         <li>
                                 <a class="function" href="#ArgShell.cmdloop">cmdloop</a>
                         </li>
+                        <li>
+                                <a class="function" href="#ArgShell.emptyline">emptyline</a>
+                        </li>
                 </ul>
 
             </li>
             <li>
                     <a class="function" href="#with_parser">with_parser</a>
             </li>
     </ul>
@@ -271,94 +274,97 @@
 </span><span id="L-176"><a href="#L-176"><span class="linenos">176</span></a>                <span class="k">try</span><span class="p">:</span>
 </span><span id="L-177"><a href="#L-177"><span class="linenos">177</span></a>                    <span class="kn">import</span> <span class="nn">readline</span>
 </span><span id="L-178"><a href="#L-178"><span class="linenos">178</span></a>
 </span><span id="L-179"><a href="#L-179"><span class="linenos">179</span></a>                    <span class="n">readline</span><span class="o">.</span><span class="n">set_completer</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">old_completer</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
 </span><span id="L-180"><a href="#L-180"><span class="linenos">180</span></a>                <span class="k">except</span> <span class="ne">ImportError</span><span class="p">:</span>
 </span><span id="L-181"><a href="#L-181"><span class="linenos">181</span></a>                    <span class="k">pass</span>
 </span><span id="L-182"><a href="#L-182"><span class="linenos">182</span></a>
-</span><span id="L-183"><a href="#L-183"><span class="linenos">183</span></a>
-</span><span id="L-184"><a href="#L-184"><span class="linenos">184</span></a><span class="k">def</span> <span class="nf">with_parser</span><span class="p">(</span>
-</span><span id="L-185"><a href="#L-185"><span class="linenos">185</span></a>    <span class="n">parser</span><span class="p">:</span> <span class="n">Callable</span><span class="p">[</span><span class="o">...</span><span class="p">,</span> <span class="n">ArgShellParser</span><span class="p">],</span>
-</span><span id="L-186"><a href="#L-186"><span class="linenos">186</span></a>    <span class="n">post_parsers</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">Callable</span><span class="p">[[</span><span class="n">Namespace</span><span class="p">],</span> <span class="n">Namespace</span><span class="p">]]</span> <span class="o">=</span> <span class="p">[],</span>
-</span><span id="L-187"><a href="#L-187"><span class="linenos">187</span></a><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Callable</span><span class="p">[[</span><span class="n">Callable</span><span class="p">[[</span><span class="n">Any</span><span class="p">,</span> <span class="n">Namespace</span><span class="p">],</span> <span class="n">Any</span><span class="p">]],</span> <span class="n">Callable</span><span class="p">[[</span><span class="n">Any</span><span class="p">,</span> <span class="nb">str</span><span class="p">],</span> <span class="n">Any</span><span class="p">]]:</span>
-</span><span id="L-188"><a href="#L-188"><span class="linenos">188</span></a>    <span class="sd">&quot;&quot;&quot;Decorate a &#39;do_*&#39; function in an argshell.ArgShell class with this function to pass an argshell.Namespace object to the decorated function instead of a string.</span>
-</span><span id="L-189"><a href="#L-189"><span class="linenos">189</span></a>
-</span><span id="L-190"><a href="#L-190"><span class="linenos">190</span></a><span class="sd">    :param parser: A function that creates an argshell.ArgShellParser instance, adds arguments to it, and returns the parser.</span>
-</span><span id="L-191"><a href="#L-191"><span class="linenos">191</span></a>
-</span><span id="L-192"><a href="#L-192"><span class="linenos">192</span></a><span class="sd">    :param post_parsers: An optional list of functions to execute where each function takes an argshell.Namespace instance and returns an argshell.Namespace instance.</span>
-</span><span id="L-193"><a href="#L-193"><span class="linenos">193</span></a><span class="sd">        &#39;post_parser&#39; functions are executed in the order they are supplied.</span>
+</span><span id="L-183"><a href="#L-183"><span class="linenos">183</span></a>    <span class="k">def</span> <span class="nf">emptyline</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="L-184"><a href="#L-184"><span class="linenos">184</span></a>        <span class="o">...</span>
+</span><span id="L-185"><a href="#L-185"><span class="linenos">185</span></a>
+</span><span id="L-186"><a href="#L-186"><span class="linenos">186</span></a>
+</span><span id="L-187"><a href="#L-187"><span class="linenos">187</span></a><span class="k">def</span> <span class="nf">with_parser</span><span class="p">(</span>
+</span><span id="L-188"><a href="#L-188"><span class="linenos">188</span></a>    <span class="n">parser</span><span class="p">:</span> <span class="n">Callable</span><span class="p">[</span><span class="o">...</span><span class="p">,</span> <span class="n">ArgShellParser</span><span class="p">],</span>
+</span><span id="L-189"><a href="#L-189"><span class="linenos">189</span></a>    <span class="n">post_parsers</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">Callable</span><span class="p">[[</span><span class="n">Namespace</span><span class="p">],</span> <span class="n">Namespace</span><span class="p">]]</span> <span class="o">=</span> <span class="p">[],</span>
+</span><span id="L-190"><a href="#L-190"><span class="linenos">190</span></a><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Callable</span><span class="p">[[</span><span class="n">Callable</span><span class="p">[[</span><span class="n">Any</span><span class="p">,</span> <span class="n">Namespace</span><span class="p">],</span> <span class="n">Any</span><span class="p">]],</span> <span class="n">Callable</span><span class="p">[[</span><span class="n">Any</span><span class="p">,</span> <span class="nb">str</span><span class="p">],</span> <span class="n">Any</span><span class="p">]]:</span>
+</span><span id="L-191"><a href="#L-191"><span class="linenos">191</span></a>    <span class="sd">&quot;&quot;&quot;Decorate a &#39;do_*&#39; function in an argshell.ArgShell class with this function to pass an argshell.Namespace object to the decorated function instead of a string.</span>
+</span><span id="L-192"><a href="#L-192"><span class="linenos">192</span></a>
+</span><span id="L-193"><a href="#L-193"><span class="linenos">193</span></a><span class="sd">    :param parser: A function that creates an argshell.ArgShellParser instance, adds arguments to it, and returns the parser.</span>
 </span><span id="L-194"><a href="#L-194"><span class="linenos">194</span></a>
-</span><span id="L-195"><a href="#L-195"><span class="linenos">195</span></a><span class="sd">    &gt;&gt;&gt; def get_parser() -&gt; argshell.ArgShellParser:</span>
-</span><span id="L-196"><a href="#L-196"><span class="linenos">196</span></a><span class="sd">    &gt;&gt;&gt;     parser = argshell.ArgShellParser()</span>
-</span><span id="L-197"><a href="#L-197"><span class="linenos">197</span></a><span class="sd">    &gt;&gt;&gt;     parser.add_argument(&quot;names&quot;, type=str, nargs=&quot;*&quot;, help=&quot;A list of first and last names to print.&quot;)</span>
-</span><span id="L-198"><a href="#L-198"><span class="linenos">198</span></a><span class="sd">    &gt;&gt;&gt;     parser.add_argument(&quot;-i&quot;, &quot;--initials&quot;, action=&quot;store_true&quot;, help=&quot;Print the initials instead of the full name.&quot;)</span>
-</span><span id="L-199"><a href="#L-199"><span class="linenos">199</span></a><span class="sd">    &gt;&gt;&gt;     return parser</span>
-</span><span id="L-200"><a href="#L-200"><span class="linenos">200</span></a><span class="sd">    &gt;&gt;&gt;</span>
-</span><span id="L-201"><a href="#L-201"><span class="linenos">201</span></a><span class="sd">    &gt;&gt;&gt; # Convert list of first and last names to a list of tuples</span>
-</span><span id="L-202"><a href="#L-202"><span class="linenos">202</span></a><span class="sd">    &gt;&gt;&gt; def names_list_to_tuples(args: argshell.Namespace) -&gt; argshell.Namespace:</span>
-</span><span id="L-203"><a href="#L-203"><span class="linenos">203</span></a><span class="sd">    &gt;&gt;&gt;     args.names = [(first, last) for first, last in zip(args.names[::2], args.names[1::2])]</span>
-</span><span id="L-204"><a href="#L-204"><span class="linenos">204</span></a><span class="sd">    &gt;&gt;&gt;     if args.initials:</span>
-</span><span id="L-205"><a href="#L-205"><span class="linenos">205</span></a><span class="sd">    &gt;&gt;&gt;         args.names = [(name[0][0], name[1][0]) for name in args.names]</span>
-</span><span id="L-206"><a href="#L-206"><span class="linenos">206</span></a><span class="sd">    &gt;&gt;&gt;     return args</span>
-</span><span id="L-207"><a href="#L-207"><span class="linenos">207</span></a><span class="sd">    &gt;&gt;&gt;</span>
-</span><span id="L-208"><a href="#L-208"><span class="linenos">208</span></a><span class="sd">    &gt;&gt;&gt; def capitalize_names(args: argshell.Namespace) -&gt; argshell.Namespace:</span>
-</span><span id="L-209"><a href="#L-209"><span class="linenos">209</span></a><span class="sd">    &gt;&gt;&gt;     args.names = [name.capitalize() for name in args.names]</span>
-</span><span id="L-210"><a href="#L-210"><span class="linenos">210</span></a><span class="sd">    &gt;&gt;&gt;     return args</span>
-</span><span id="L-211"><a href="#L-211"><span class="linenos">211</span></a><span class="sd">    &gt;&gt;&gt;</span>
-</span><span id="L-212"><a href="#L-212"><span class="linenos">212</span></a><span class="sd">    &gt;&gt;&gt; class NameShell(ArgShell):</span>
-</span><span id="L-213"><a href="#L-213"><span class="linenos">213</span></a><span class="sd">    &gt;&gt;&gt;     intro = &quot;Entering nameshell...&quot;</span>
-</span><span id="L-214"><a href="#L-214"><span class="linenos">214</span></a><span class="sd">    &gt;&gt;&gt;     prompt = &quot;nameshell&gt;&quot;</span>
-</span><span id="L-215"><a href="#L-215"><span class="linenos">215</span></a><span class="sd">    &gt;&gt;&gt;</span>
-</span><span id="L-216"><a href="#L-216"><span class="linenos">216</span></a><span class="sd">    &gt;&gt;&gt;     @with_parser(get_parser, [capitalize_names, names_list_to_tuples])</span>
-</span><span id="L-217"><a href="#L-217"><span class="linenos">217</span></a><span class="sd">    &gt;&gt;&gt;     def do_printnames(self, args: argshell.Namespace):</span>
-</span><span id="L-218"><a href="#L-218"><span class="linenos">218</span></a><span class="sd">    &gt;&gt;&gt;         print(*[f&quot;{name[0]} {name[1]}&quot; for name in args.names], sep=&quot;\\n&quot;)</span>
-</span><span id="L-219"><a href="#L-219"><span class="linenos">219</span></a><span class="sd">    &gt;&gt;&gt;</span>
-</span><span id="L-220"><a href="#L-220"><span class="linenos">220</span></a><span class="sd">    &gt;&gt;&gt; NameShell().cmdloop()</span>
-</span><span id="L-221"><a href="#L-221"><span class="linenos">221</span></a><span class="sd">    &gt;&gt;&gt; Entering nameshell...</span>
-</span><span id="L-222"><a href="#L-222"><span class="linenos">222</span></a><span class="sd">    &gt;&gt;&gt; nameshell&gt;printnames karl marx fred hampton emma goldman angela davis nestor makhno</span>
-</span><span id="L-223"><a href="#L-223"><span class="linenos">223</span></a><span class="sd">    &gt;&gt;&gt; Karl Marx</span>
-</span><span id="L-224"><a href="#L-224"><span class="linenos">224</span></a><span class="sd">    &gt;&gt;&gt; Fred Hampton</span>
-</span><span id="L-225"><a href="#L-225"><span class="linenos">225</span></a><span class="sd">    &gt;&gt;&gt; Emma Goldman</span>
-</span><span id="L-226"><a href="#L-226"><span class="linenos">226</span></a><span class="sd">    &gt;&gt;&gt; Angela Davis</span>
-</span><span id="L-227"><a href="#L-227"><span class="linenos">227</span></a><span class="sd">    &gt;&gt;&gt; Nestor Makhno</span>
-</span><span id="L-228"><a href="#L-228"><span class="linenos">228</span></a><span class="sd">    &gt;&gt;&gt; nameshell&gt;printnames karl marx fred hampton emma goldman angela davis nestor makhno -i</span>
-</span><span id="L-229"><a href="#L-229"><span class="linenos">229</span></a><span class="sd">    &gt;&gt;&gt; K M</span>
-</span><span id="L-230"><a href="#L-230"><span class="linenos">230</span></a><span class="sd">    &gt;&gt;&gt; F H</span>
-</span><span id="L-231"><a href="#L-231"><span class="linenos">231</span></a><span class="sd">    &gt;&gt;&gt; E G</span>
-</span><span id="L-232"><a href="#L-232"><span class="linenos">232</span></a><span class="sd">    &gt;&gt;&gt; A D</span>
-</span><span id="L-233"><a href="#L-233"><span class="linenos">233</span></a><span class="sd">    &gt;&gt;&gt; N M&quot;&quot;&quot;</span>
-</span><span id="L-234"><a href="#L-234"><span class="linenos">234</span></a>
-</span><span id="L-235"><a href="#L-235"><span class="linenos">235</span></a>    <span class="k">def</span> <span class="nf">decorator</span><span class="p">(</span>
-</span><span id="L-236"><a href="#L-236"><span class="linenos">236</span></a>        <span class="n">func</span><span class="p">:</span> <span class="n">Callable</span><span class="p">[[</span><span class="n">Any</span><span class="p">,</span> <span class="n">Namespace</span><span class="p">],</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span><span class="p">]</span>
-</span><span id="L-237"><a href="#L-237"><span class="linenos">237</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Callable</span><span class="p">[[</span><span class="n">Any</span><span class="p">,</span> <span class="nb">str</span><span class="p">],</span> <span class="n">Any</span><span class="p">]:</span>
-</span><span id="L-238"><a href="#L-238"><span class="linenos">238</span></a>        <span class="nd">@wraps</span><span class="p">(</span><span class="n">func</span><span class="p">)</span>
-</span><span id="L-239"><a href="#L-239"><span class="linenos">239</span></a>        <span class="k">def</span> <span class="nf">inner</span><span class="p">(</span><span class="bp">self</span><span class="p">:</span> <span class="n">Any</span><span class="p">,</span> <span class="n">command</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Any</span><span class="p">:</span>
-</span><span id="L-240"><a href="#L-240"><span class="linenos">240</span></a>            <span class="k">try</span><span class="p">:</span>
-</span><span id="L-241"><a href="#L-241"><span class="linenos">241</span></a>                <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="p">()</span><span class="o">.</span><span class="n">parse_args</span><span class="p">(</span><span class="n">shlex</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="n">command</span><span class="p">))</span>
-</span><span id="L-242"><a href="#L-242"><span class="linenos">242</span></a>            <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="L-243"><a href="#L-243"><span class="linenos">243</span></a>                <span class="c1"># On parser error, print help and skip post_parser and func execution</span>
-</span><span id="L-244"><a href="#L-244"><span class="linenos">244</span></a>                <span class="k">if</span> <span class="s2">&quot;the following arguments are required&quot;</span> <span class="ow">not</span> <span class="ow">in</span> <span class="nb">str</span><span class="p">(</span><span class="n">e</span><span class="p">):</span>
-</span><span id="L-245"><a href="#L-245"><span class="linenos">245</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;ERROR: </span><span class="si">{</span><span class="n">e</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-246"><a href="#L-246"><span class="linenos">246</span></a>                <span class="k">if</span> <span class="s2">&quot;-h&quot;</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">command</span> <span class="ow">and</span> <span class="s2">&quot;--help&quot;</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">command</span><span class="p">:</span>
-</span><span id="L-247"><a href="#L-247"><span class="linenos">247</span></a>                    <span class="k">try</span><span class="p">:</span>
-</span><span id="L-248"><a href="#L-248"><span class="linenos">248</span></a>                        <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="p">()</span><span class="o">.</span><span class="n">parse_args</span><span class="p">([</span><span class="s2">&quot;--help&quot;</span><span class="p">])</span>
-</span><span id="L-249"><a href="#L-249"><span class="linenos">249</span></a>                    <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="L-250"><a href="#L-250"><span class="linenos">250</span></a>                        <span class="k">pass</span>
-</span><span id="L-251"><a href="#L-251"><span class="linenos">251</span></a>                <span class="k">return</span> <span class="kc">None</span>
-</span><span id="L-252"><a href="#L-252"><span class="linenos">252</span></a>            <span class="c1"># Don&#39;t execute function, only print parser help</span>
-</span><span id="L-253"><a href="#L-253"><span class="linenos">253</span></a>            <span class="k">if</span> <span class="s2">&quot;-h&quot;</span> <span class="ow">in</span> <span class="n">command</span> <span class="ow">or</span> <span class="s2">&quot;--help&quot;</span> <span class="ow">in</span> <span class="n">command</span><span class="p">:</span>
+</span><span id="L-195"><a href="#L-195"><span class="linenos">195</span></a><span class="sd">    :param post_parsers: An optional list of functions to execute where each function takes an argshell.Namespace instance and returns an argshell.Namespace instance.</span>
+</span><span id="L-196"><a href="#L-196"><span class="linenos">196</span></a><span class="sd">        &#39;post_parser&#39; functions are executed in the order they are supplied.</span>
+</span><span id="L-197"><a href="#L-197"><span class="linenos">197</span></a>
+</span><span id="L-198"><a href="#L-198"><span class="linenos">198</span></a><span class="sd">    &gt;&gt;&gt; def get_parser() -&gt; argshell.ArgShellParser:</span>
+</span><span id="L-199"><a href="#L-199"><span class="linenos">199</span></a><span class="sd">    &gt;&gt;&gt;     parser = argshell.ArgShellParser()</span>
+</span><span id="L-200"><a href="#L-200"><span class="linenos">200</span></a><span class="sd">    &gt;&gt;&gt;     parser.add_argument(&quot;names&quot;, type=str, nargs=&quot;*&quot;, help=&quot;A list of first and last names to print.&quot;)</span>
+</span><span id="L-201"><a href="#L-201"><span class="linenos">201</span></a><span class="sd">    &gt;&gt;&gt;     parser.add_argument(&quot;-i&quot;, &quot;--initials&quot;, action=&quot;store_true&quot;, help=&quot;Print the initials instead of the full name.&quot;)</span>
+</span><span id="L-202"><a href="#L-202"><span class="linenos">202</span></a><span class="sd">    &gt;&gt;&gt;     return parser</span>
+</span><span id="L-203"><a href="#L-203"><span class="linenos">203</span></a><span class="sd">    &gt;&gt;&gt;</span>
+</span><span id="L-204"><a href="#L-204"><span class="linenos">204</span></a><span class="sd">    &gt;&gt;&gt; # Convert list of first and last names to a list of tuples</span>
+</span><span id="L-205"><a href="#L-205"><span class="linenos">205</span></a><span class="sd">    &gt;&gt;&gt; def names_list_to_tuples(args: argshell.Namespace) -&gt; argshell.Namespace:</span>
+</span><span id="L-206"><a href="#L-206"><span class="linenos">206</span></a><span class="sd">    &gt;&gt;&gt;     args.names = [(first, last) for first, last in zip(args.names[::2], args.names[1::2])]</span>
+</span><span id="L-207"><a href="#L-207"><span class="linenos">207</span></a><span class="sd">    &gt;&gt;&gt;     if args.initials:</span>
+</span><span id="L-208"><a href="#L-208"><span class="linenos">208</span></a><span class="sd">    &gt;&gt;&gt;         args.names = [(name[0][0], name[1][0]) for name in args.names]</span>
+</span><span id="L-209"><a href="#L-209"><span class="linenos">209</span></a><span class="sd">    &gt;&gt;&gt;     return args</span>
+</span><span id="L-210"><a href="#L-210"><span class="linenos">210</span></a><span class="sd">    &gt;&gt;&gt;</span>
+</span><span id="L-211"><a href="#L-211"><span class="linenos">211</span></a><span class="sd">    &gt;&gt;&gt; def capitalize_names(args: argshell.Namespace) -&gt; argshell.Namespace:</span>
+</span><span id="L-212"><a href="#L-212"><span class="linenos">212</span></a><span class="sd">    &gt;&gt;&gt;     args.names = [name.capitalize() for name in args.names]</span>
+</span><span id="L-213"><a href="#L-213"><span class="linenos">213</span></a><span class="sd">    &gt;&gt;&gt;     return args</span>
+</span><span id="L-214"><a href="#L-214"><span class="linenos">214</span></a><span class="sd">    &gt;&gt;&gt;</span>
+</span><span id="L-215"><a href="#L-215"><span class="linenos">215</span></a><span class="sd">    &gt;&gt;&gt; class NameShell(ArgShell):</span>
+</span><span id="L-216"><a href="#L-216"><span class="linenos">216</span></a><span class="sd">    &gt;&gt;&gt;     intro = &quot;Entering nameshell...&quot;</span>
+</span><span id="L-217"><a href="#L-217"><span class="linenos">217</span></a><span class="sd">    &gt;&gt;&gt;     prompt = &quot;nameshell&gt;&quot;</span>
+</span><span id="L-218"><a href="#L-218"><span class="linenos">218</span></a><span class="sd">    &gt;&gt;&gt;</span>
+</span><span id="L-219"><a href="#L-219"><span class="linenos">219</span></a><span class="sd">    &gt;&gt;&gt;     @with_parser(get_parser, [capitalize_names, names_list_to_tuples])</span>
+</span><span id="L-220"><a href="#L-220"><span class="linenos">220</span></a><span class="sd">    &gt;&gt;&gt;     def do_printnames(self, args: argshell.Namespace):</span>
+</span><span id="L-221"><a href="#L-221"><span class="linenos">221</span></a><span class="sd">    &gt;&gt;&gt;         print(*[f&quot;{name[0]} {name[1]}&quot; for name in args.names], sep=&quot;\\n&quot;)</span>
+</span><span id="L-222"><a href="#L-222"><span class="linenos">222</span></a><span class="sd">    &gt;&gt;&gt;</span>
+</span><span id="L-223"><a href="#L-223"><span class="linenos">223</span></a><span class="sd">    &gt;&gt;&gt; NameShell().cmdloop()</span>
+</span><span id="L-224"><a href="#L-224"><span class="linenos">224</span></a><span class="sd">    &gt;&gt;&gt; Entering nameshell...</span>
+</span><span id="L-225"><a href="#L-225"><span class="linenos">225</span></a><span class="sd">    &gt;&gt;&gt; nameshell&gt;printnames karl marx fred hampton emma goldman angela davis nestor makhno</span>
+</span><span id="L-226"><a href="#L-226"><span class="linenos">226</span></a><span class="sd">    &gt;&gt;&gt; Karl Marx</span>
+</span><span id="L-227"><a href="#L-227"><span class="linenos">227</span></a><span class="sd">    &gt;&gt;&gt; Fred Hampton</span>
+</span><span id="L-228"><a href="#L-228"><span class="linenos">228</span></a><span class="sd">    &gt;&gt;&gt; Emma Goldman</span>
+</span><span id="L-229"><a href="#L-229"><span class="linenos">229</span></a><span class="sd">    &gt;&gt;&gt; Angela Davis</span>
+</span><span id="L-230"><a href="#L-230"><span class="linenos">230</span></a><span class="sd">    &gt;&gt;&gt; Nestor Makhno</span>
+</span><span id="L-231"><a href="#L-231"><span class="linenos">231</span></a><span class="sd">    &gt;&gt;&gt; nameshell&gt;printnames karl marx fred hampton emma goldman angela davis nestor makhno -i</span>
+</span><span id="L-232"><a href="#L-232"><span class="linenos">232</span></a><span class="sd">    &gt;&gt;&gt; K M</span>
+</span><span id="L-233"><a href="#L-233"><span class="linenos">233</span></a><span class="sd">    &gt;&gt;&gt; F H</span>
+</span><span id="L-234"><a href="#L-234"><span class="linenos">234</span></a><span class="sd">    &gt;&gt;&gt; E G</span>
+</span><span id="L-235"><a href="#L-235"><span class="linenos">235</span></a><span class="sd">    &gt;&gt;&gt; A D</span>
+</span><span id="L-236"><a href="#L-236"><span class="linenos">236</span></a><span class="sd">    &gt;&gt;&gt; N M&quot;&quot;&quot;</span>
+</span><span id="L-237"><a href="#L-237"><span class="linenos">237</span></a>
+</span><span id="L-238"><a href="#L-238"><span class="linenos">238</span></a>    <span class="k">def</span> <span class="nf">decorator</span><span class="p">(</span>
+</span><span id="L-239"><a href="#L-239"><span class="linenos">239</span></a>        <span class="n">func</span><span class="p">:</span> <span class="n">Callable</span><span class="p">[[</span><span class="n">Any</span><span class="p">,</span> <span class="n">Namespace</span><span class="p">],</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span><span class="p">]</span>
+</span><span id="L-240"><a href="#L-240"><span class="linenos">240</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Callable</span><span class="p">[[</span><span class="n">Any</span><span class="p">,</span> <span class="nb">str</span><span class="p">],</span> <span class="n">Any</span><span class="p">]:</span>
+</span><span id="L-241"><a href="#L-241"><span class="linenos">241</span></a>        <span class="nd">@wraps</span><span class="p">(</span><span class="n">func</span><span class="p">)</span>
+</span><span id="L-242"><a href="#L-242"><span class="linenos">242</span></a>        <span class="k">def</span> <span class="nf">inner</span><span class="p">(</span><span class="bp">self</span><span class="p">:</span> <span class="n">Any</span><span class="p">,</span> <span class="n">command</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Any</span><span class="p">:</span>
+</span><span id="L-243"><a href="#L-243"><span class="linenos">243</span></a>            <span class="k">try</span><span class="p">:</span>
+</span><span id="L-244"><a href="#L-244"><span class="linenos">244</span></a>                <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="p">()</span><span class="o">.</span><span class="n">parse_args</span><span class="p">(</span><span class="n">shlex</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="n">command</span><span class="p">))</span>
+</span><span id="L-245"><a href="#L-245"><span class="linenos">245</span></a>            <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="L-246"><a href="#L-246"><span class="linenos">246</span></a>                <span class="c1"># On parser error, print help and skip post_parser and func execution</span>
+</span><span id="L-247"><a href="#L-247"><span class="linenos">247</span></a>                <span class="k">if</span> <span class="s2">&quot;the following arguments are required&quot;</span> <span class="ow">not</span> <span class="ow">in</span> <span class="nb">str</span><span class="p">(</span><span class="n">e</span><span class="p">):</span>
+</span><span id="L-248"><a href="#L-248"><span class="linenos">248</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;ERROR: </span><span class="si">{</span><span class="n">e</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-249"><a href="#L-249"><span class="linenos">249</span></a>                <span class="k">if</span> <span class="s2">&quot;-h&quot;</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">command</span> <span class="ow">and</span> <span class="s2">&quot;--help&quot;</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">command</span><span class="p">:</span>
+</span><span id="L-250"><a href="#L-250"><span class="linenos">250</span></a>                    <span class="k">try</span><span class="p">:</span>
+</span><span id="L-251"><a href="#L-251"><span class="linenos">251</span></a>                        <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="p">()</span><span class="o">.</span><span class="n">parse_args</span><span class="p">([</span><span class="s2">&quot;--help&quot;</span><span class="p">])</span>
+</span><span id="L-252"><a href="#L-252"><span class="linenos">252</span></a>                    <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="L-253"><a href="#L-253"><span class="linenos">253</span></a>                        <span class="k">pass</span>
 </span><span id="L-254"><a href="#L-254"><span class="linenos">254</span></a>                <span class="k">return</span> <span class="kc">None</span>
-</span><span id="L-255"><a href="#L-255"><span class="linenos">255</span></a>            <span class="k">for</span> <span class="n">post_parser</span> <span class="ow">in</span> <span class="n">post_parsers</span><span class="p">:</span>
-</span><span id="L-256"><a href="#L-256"><span class="linenos">256</span></a>                <span class="n">args</span> <span class="o">=</span> <span class="n">post_parser</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
-</span><span id="L-257"><a href="#L-257"><span class="linenos">257</span></a>
-</span><span id="L-258"><a href="#L-258"><span class="linenos">258</span></a>            <span class="k">return</span> <span class="n">func</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">)</span>
-</span><span id="L-259"><a href="#L-259"><span class="linenos">259</span></a>
-</span><span id="L-260"><a href="#L-260"><span class="linenos">260</span></a>        <span class="k">return</span> <span class="n">inner</span>
-</span><span id="L-261"><a href="#L-261"><span class="linenos">261</span></a>
-</span><span id="L-262"><a href="#L-262"><span class="linenos">262</span></a>    <span class="k">return</span> <span class="n">decorator</span>
+</span><span id="L-255"><a href="#L-255"><span class="linenos">255</span></a>            <span class="c1"># Don&#39;t execute function, only print parser help</span>
+</span><span id="L-256"><a href="#L-256"><span class="linenos">256</span></a>            <span class="k">if</span> <span class="s2">&quot;-h&quot;</span> <span class="ow">in</span> <span class="n">command</span> <span class="ow">or</span> <span class="s2">&quot;--help&quot;</span> <span class="ow">in</span> <span class="n">command</span><span class="p">:</span>
+</span><span id="L-257"><a href="#L-257"><span class="linenos">257</span></a>                <span class="k">return</span> <span class="kc">None</span>
+</span><span id="L-258"><a href="#L-258"><span class="linenos">258</span></a>            <span class="k">for</span> <span class="n">post_parser</span> <span class="ow">in</span> <span class="n">post_parsers</span><span class="p">:</span>
+</span><span id="L-259"><a href="#L-259"><span class="linenos">259</span></a>                <span class="n">args</span> <span class="o">=</span> <span class="n">post_parser</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
+</span><span id="L-260"><a href="#L-260"><span class="linenos">260</span></a>
+</span><span id="L-261"><a href="#L-261"><span class="linenos">261</span></a>            <span class="k">return</span> <span class="n">func</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">)</span>
+</span><span id="L-262"><a href="#L-262"><span class="linenos">262</span></a>
+</span><span id="L-263"><a href="#L-263"><span class="linenos">263</span></a>        <span class="k">return</span> <span class="n">inner</span>
+</span><span id="L-264"><a href="#L-264"><span class="linenos">264</span></a>
+</span><span id="L-265"><a href="#L-265"><span class="linenos">265</span></a>    <span class="k">return</span> <span class="n">decorator</span>
 </span></pre></div>
 
 
             </section>
                 <section id="Namespace">
                             <input id="Namespace-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr class">
@@ -699,14 +705,17 @@
 </span><span id="ArgShell-176"><a href="#ArgShell-176"><span class="linenos">176</span></a>            <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">use_rawinput</span> <span class="ow">and</span> <span class="bp">self</span><span class="o">.</span><span class="n">completekey</span><span class="p">:</span>
 </span><span id="ArgShell-177"><a href="#ArgShell-177"><span class="linenos">177</span></a>                <span class="k">try</span><span class="p">:</span>
 </span><span id="ArgShell-178"><a href="#ArgShell-178"><span class="linenos">178</span></a>                    <span class="kn">import</span> <span class="nn">readline</span>
 </span><span id="ArgShell-179"><a href="#ArgShell-179"><span class="linenos">179</span></a>
 </span><span id="ArgShell-180"><a href="#ArgShell-180"><span class="linenos">180</span></a>                    <span class="n">readline</span><span class="o">.</span><span class="n">set_completer</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">old_completer</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
 </span><span id="ArgShell-181"><a href="#ArgShell-181"><span class="linenos">181</span></a>                <span class="k">except</span> <span class="ne">ImportError</span><span class="p">:</span>
 </span><span id="ArgShell-182"><a href="#ArgShell-182"><span class="linenos">182</span></a>                    <span class="k">pass</span>
+</span><span id="ArgShell-183"><a href="#ArgShell-183"><span class="linenos">183</span></a>
+</span><span id="ArgShell-184"><a href="#ArgShell-184"><span class="linenos">184</span></a>    <span class="k">def</span> <span class="nf">emptyline</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="ArgShell-185"><a href="#ArgShell-185"><span class="linenos">185</span></a>        <span class="o">...</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Subclass this to create custom ArgShells.</p>
 </div>
 
 
@@ -904,26 +913,49 @@
             <div class="docstring"><p>Repeatedly issue a prompt, accept input, parse an initial prefix
 off the received input, and dispatch to action methods, passing them
 the remainder of the line as argument.</p>
 </div>
 
 
                             </div>
+                            <div id="ArgShell.emptyline" class="classattr">
+                                        <input id="ArgShell.emptyline-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
+<div class="attr function">
+            
+        <span class="def">def</span>
+        <span class="name">emptyline</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span></span><span class="return-annotation">):</span></span>
+
+                <label class="view-source-button" for="ArgShell.emptyline-view-source"><span>View Source</span></label>
+
+    </div>
+    <a class="headerlink" href="#ArgShell.emptyline"></a>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="ArgShell.emptyline-184"><a href="#ArgShell.emptyline-184"><span class="linenos">184</span></a>    <span class="k">def</span> <span class="nf">emptyline</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="ArgShell.emptyline-185"><a href="#ArgShell.emptyline-185"><span class="linenos">185</span></a>        <span class="o">...</span>
+</span></pre></div>
+
+
+            <div class="docstring"><p>Called when an empty line is entered in response to the prompt.</p>
+
+<p>If this method is not overridden, it repeats the last nonempty
+command entered.</p>
+</div>
+
+
+                            </div>
                             <div class="inherited">
                                 <h5>Inherited Members</h5>
                                 <dl>
                                     <div><dt>cmd.Cmd</dt>
                                 <dd id="ArgShell.__init__" class="function">Cmd</dd>
                 <dd id="ArgShell.precmd" class="function">precmd</dd>
                 <dd id="ArgShell.postcmd" class="function">postcmd</dd>
                 <dd id="ArgShell.preloop" class="function">preloop</dd>
                 <dd id="ArgShell.postloop" class="function">postloop</dd>
                 <dd id="ArgShell.parseline" class="function">parseline</dd>
                 <dd id="ArgShell.onecmd" class="function">onecmd</dd>
-                <dd id="ArgShell.emptyline" class="function">emptyline</dd>
                 <dd id="ArgShell.default" class="function">default</dd>
                 <dd id="ArgShell.completedefault" class="function">completedefault</dd>
                 <dd id="ArgShell.completenames" class="function">completenames</dd>
                 <dd id="ArgShell.complete" class="function">complete</dd>
                 <dd id="ArgShell.get_names" class="function">get_names</dd>
                 <dd id="ArgShell.complete_help" class="function">complete_help</dd>
                 <dd id="ArgShell.print_topics" class="function">print_topics</dd>
@@ -940,93 +972,93 @@
         <span class="def">def</span>
         <span class="name">with_parser</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="n">parser</span><span class="p">:</span> <span class="n">Callable</span><span class="p">[</span><span class="o">...</span><span class="p">,</span> <span class="n"><a href="#ArgShellParser">argshell.argshell.ArgShellParser</a></span><span class="p">]</span>,</span><span class="param">	<span class="n">post_parsers</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">typing</span><span class="o">.</span><span class="n">Callable</span><span class="p">[[</span><span class="n"><a href="#Namespace">argshell.argshell.Namespace</a></span><span class="p">],</span> <span class="n"><a href="#Namespace">argshell.argshell.Namespace</a></span><span class="p">]]</span> <span class="o">=</span> <span class="p">[]</span></span><span class="return-annotation">) -> <span class="n">Callable</span><span class="p">[[</span><span class="n">Callable</span><span class="p">[[</span><span class="n">Any</span><span class="p">,</span> <span class="n"><a href="#Namespace">argshell.argshell.Namespace</a></span><span class="p">],</span> <span class="n">Any</span><span class="p">]],</span> <span class="n">Callable</span><span class="p">[[</span><span class="n">Any</span><span class="p">,</span> <span class="nb">str</span><span class="p">],</span> <span class="n">Any</span><span class="p">]]</span>:</span></span>
 
                 <label class="view-source-button" for="with_parser-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#with_parser"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="with_parser-185"><a href="#with_parser-185"><span class="linenos">185</span></a><span class="k">def</span> <span class="nf">with_parser</span><span class="p">(</span>
-</span><span id="with_parser-186"><a href="#with_parser-186"><span class="linenos">186</span></a>    <span class="n">parser</span><span class="p">:</span> <span class="n">Callable</span><span class="p">[</span><span class="o">...</span><span class="p">,</span> <span class="n">ArgShellParser</span><span class="p">],</span>
-</span><span id="with_parser-187"><a href="#with_parser-187"><span class="linenos">187</span></a>    <span class="n">post_parsers</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">Callable</span><span class="p">[[</span><span class="n">Namespace</span><span class="p">],</span> <span class="n">Namespace</span><span class="p">]]</span> <span class="o">=</span> <span class="p">[],</span>
-</span><span id="with_parser-188"><a href="#with_parser-188"><span class="linenos">188</span></a><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Callable</span><span class="p">[[</span><span class="n">Callable</span><span class="p">[[</span><span class="n">Any</span><span class="p">,</span> <span class="n">Namespace</span><span class="p">],</span> <span class="n">Any</span><span class="p">]],</span> <span class="n">Callable</span><span class="p">[[</span><span class="n">Any</span><span class="p">,</span> <span class="nb">str</span><span class="p">],</span> <span class="n">Any</span><span class="p">]]:</span>
-</span><span id="with_parser-189"><a href="#with_parser-189"><span class="linenos">189</span></a>    <span class="sd">&quot;&quot;&quot;Decorate a &#39;do_*&#39; function in an argshell.ArgShell class with this function to pass an argshell.Namespace object to the decorated function instead of a string.</span>
-</span><span id="with_parser-190"><a href="#with_parser-190"><span class="linenos">190</span></a>
-</span><span id="with_parser-191"><a href="#with_parser-191"><span class="linenos">191</span></a><span class="sd">    :param parser: A function that creates an argshell.ArgShellParser instance, adds arguments to it, and returns the parser.</span>
-</span><span id="with_parser-192"><a href="#with_parser-192"><span class="linenos">192</span></a>
-</span><span id="with_parser-193"><a href="#with_parser-193"><span class="linenos">193</span></a><span class="sd">    :param post_parsers: An optional list of functions to execute where each function takes an argshell.Namespace instance and returns an argshell.Namespace instance.</span>
-</span><span id="with_parser-194"><a href="#with_parser-194"><span class="linenos">194</span></a><span class="sd">        &#39;post_parser&#39; functions are executed in the order they are supplied.</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="with_parser-188"><a href="#with_parser-188"><span class="linenos">188</span></a><span class="k">def</span> <span class="nf">with_parser</span><span class="p">(</span>
+</span><span id="with_parser-189"><a href="#with_parser-189"><span class="linenos">189</span></a>    <span class="n">parser</span><span class="p">:</span> <span class="n">Callable</span><span class="p">[</span><span class="o">...</span><span class="p">,</span> <span class="n">ArgShellParser</span><span class="p">],</span>
+</span><span id="with_parser-190"><a href="#with_parser-190"><span class="linenos">190</span></a>    <span class="n">post_parsers</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">Callable</span><span class="p">[[</span><span class="n">Namespace</span><span class="p">],</span> <span class="n">Namespace</span><span class="p">]]</span> <span class="o">=</span> <span class="p">[],</span>
+</span><span id="with_parser-191"><a href="#with_parser-191"><span class="linenos">191</span></a><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Callable</span><span class="p">[[</span><span class="n">Callable</span><span class="p">[[</span><span class="n">Any</span><span class="p">,</span> <span class="n">Namespace</span><span class="p">],</span> <span class="n">Any</span><span class="p">]],</span> <span class="n">Callable</span><span class="p">[[</span><span class="n">Any</span><span class="p">,</span> <span class="nb">str</span><span class="p">],</span> <span class="n">Any</span><span class="p">]]:</span>
+</span><span id="with_parser-192"><a href="#with_parser-192"><span class="linenos">192</span></a>    <span class="sd">&quot;&quot;&quot;Decorate a &#39;do_*&#39; function in an argshell.ArgShell class with this function to pass an argshell.Namespace object to the decorated function instead of a string.</span>
+</span><span id="with_parser-193"><a href="#with_parser-193"><span class="linenos">193</span></a>
+</span><span id="with_parser-194"><a href="#with_parser-194"><span class="linenos">194</span></a><span class="sd">    :param parser: A function that creates an argshell.ArgShellParser instance, adds arguments to it, and returns the parser.</span>
 </span><span id="with_parser-195"><a href="#with_parser-195"><span class="linenos">195</span></a>
-</span><span id="with_parser-196"><a href="#with_parser-196"><span class="linenos">196</span></a><span class="sd">    &gt;&gt;&gt; def get_parser() -&gt; argshell.ArgShellParser:</span>
-</span><span id="with_parser-197"><a href="#with_parser-197"><span class="linenos">197</span></a><span class="sd">    &gt;&gt;&gt;     parser = argshell.ArgShellParser()</span>
-</span><span id="with_parser-198"><a href="#with_parser-198"><span class="linenos">198</span></a><span class="sd">    &gt;&gt;&gt;     parser.add_argument(&quot;names&quot;, type=str, nargs=&quot;*&quot;, help=&quot;A list of first and last names to print.&quot;)</span>
-</span><span id="with_parser-199"><a href="#with_parser-199"><span class="linenos">199</span></a><span class="sd">    &gt;&gt;&gt;     parser.add_argument(&quot;-i&quot;, &quot;--initials&quot;, action=&quot;store_true&quot;, help=&quot;Print the initials instead of the full name.&quot;)</span>
-</span><span id="with_parser-200"><a href="#with_parser-200"><span class="linenos">200</span></a><span class="sd">    &gt;&gt;&gt;     return parser</span>
-</span><span id="with_parser-201"><a href="#with_parser-201"><span class="linenos">201</span></a><span class="sd">    &gt;&gt;&gt;</span>
-</span><span id="with_parser-202"><a href="#with_parser-202"><span class="linenos">202</span></a><span class="sd">    &gt;&gt;&gt; # Convert list of first and last names to a list of tuples</span>
-</span><span id="with_parser-203"><a href="#with_parser-203"><span class="linenos">203</span></a><span class="sd">    &gt;&gt;&gt; def names_list_to_tuples(args: argshell.Namespace) -&gt; argshell.Namespace:</span>
-</span><span id="with_parser-204"><a href="#with_parser-204"><span class="linenos">204</span></a><span class="sd">    &gt;&gt;&gt;     args.names = [(first, last) for first, last in zip(args.names[::2], args.names[1::2])]</span>
-</span><span id="with_parser-205"><a href="#with_parser-205"><span class="linenos">205</span></a><span class="sd">    &gt;&gt;&gt;     if args.initials:</span>
-</span><span id="with_parser-206"><a href="#with_parser-206"><span class="linenos">206</span></a><span class="sd">    &gt;&gt;&gt;         args.names = [(name[0][0], name[1][0]) for name in args.names]</span>
-</span><span id="with_parser-207"><a href="#with_parser-207"><span class="linenos">207</span></a><span class="sd">    &gt;&gt;&gt;     return args</span>
-</span><span id="with_parser-208"><a href="#with_parser-208"><span class="linenos">208</span></a><span class="sd">    &gt;&gt;&gt;</span>
-</span><span id="with_parser-209"><a href="#with_parser-209"><span class="linenos">209</span></a><span class="sd">    &gt;&gt;&gt; def capitalize_names(args: argshell.Namespace) -&gt; argshell.Namespace:</span>
-</span><span id="with_parser-210"><a href="#with_parser-210"><span class="linenos">210</span></a><span class="sd">    &gt;&gt;&gt;     args.names = [name.capitalize() for name in args.names]</span>
-</span><span id="with_parser-211"><a href="#with_parser-211"><span class="linenos">211</span></a><span class="sd">    &gt;&gt;&gt;     return args</span>
-</span><span id="with_parser-212"><a href="#with_parser-212"><span class="linenos">212</span></a><span class="sd">    &gt;&gt;&gt;</span>
-</span><span id="with_parser-213"><a href="#with_parser-213"><span class="linenos">213</span></a><span class="sd">    &gt;&gt;&gt; class NameShell(ArgShell):</span>
-</span><span id="with_parser-214"><a href="#with_parser-214"><span class="linenos">214</span></a><span class="sd">    &gt;&gt;&gt;     intro = &quot;Entering nameshell...&quot;</span>
-</span><span id="with_parser-215"><a href="#with_parser-215"><span class="linenos">215</span></a><span class="sd">    &gt;&gt;&gt;     prompt = &quot;nameshell&gt;&quot;</span>
-</span><span id="with_parser-216"><a href="#with_parser-216"><span class="linenos">216</span></a><span class="sd">    &gt;&gt;&gt;</span>
-</span><span id="with_parser-217"><a href="#with_parser-217"><span class="linenos">217</span></a><span class="sd">    &gt;&gt;&gt;     @with_parser(get_parser, [capitalize_names, names_list_to_tuples])</span>
-</span><span id="with_parser-218"><a href="#with_parser-218"><span class="linenos">218</span></a><span class="sd">    &gt;&gt;&gt;     def do_printnames(self, args: argshell.Namespace):</span>
-</span><span id="with_parser-219"><a href="#with_parser-219"><span class="linenos">219</span></a><span class="sd">    &gt;&gt;&gt;         print(*[f&quot;{name[0]} {name[1]}&quot; for name in args.names], sep=&quot;\\n&quot;)</span>
-</span><span id="with_parser-220"><a href="#with_parser-220"><span class="linenos">220</span></a><span class="sd">    &gt;&gt;&gt;</span>
-</span><span id="with_parser-221"><a href="#with_parser-221"><span class="linenos">221</span></a><span class="sd">    &gt;&gt;&gt; NameShell().cmdloop()</span>
-</span><span id="with_parser-222"><a href="#with_parser-222"><span class="linenos">222</span></a><span class="sd">    &gt;&gt;&gt; Entering nameshell...</span>
-</span><span id="with_parser-223"><a href="#with_parser-223"><span class="linenos">223</span></a><span class="sd">    &gt;&gt;&gt; nameshell&gt;printnames karl marx fred hampton emma goldman angela davis nestor makhno</span>
-</span><span id="with_parser-224"><a href="#with_parser-224"><span class="linenos">224</span></a><span class="sd">    &gt;&gt;&gt; Karl Marx</span>
-</span><span id="with_parser-225"><a href="#with_parser-225"><span class="linenos">225</span></a><span class="sd">    &gt;&gt;&gt; Fred Hampton</span>
-</span><span id="with_parser-226"><a href="#with_parser-226"><span class="linenos">226</span></a><span class="sd">    &gt;&gt;&gt; Emma Goldman</span>
-</span><span id="with_parser-227"><a href="#with_parser-227"><span class="linenos">227</span></a><span class="sd">    &gt;&gt;&gt; Angela Davis</span>
-</span><span id="with_parser-228"><a href="#with_parser-228"><span class="linenos">228</span></a><span class="sd">    &gt;&gt;&gt; Nestor Makhno</span>
-</span><span id="with_parser-229"><a href="#with_parser-229"><span class="linenos">229</span></a><span class="sd">    &gt;&gt;&gt; nameshell&gt;printnames karl marx fred hampton emma goldman angela davis nestor makhno -i</span>
-</span><span id="with_parser-230"><a href="#with_parser-230"><span class="linenos">230</span></a><span class="sd">    &gt;&gt;&gt; K M</span>
-</span><span id="with_parser-231"><a href="#with_parser-231"><span class="linenos">231</span></a><span class="sd">    &gt;&gt;&gt; F H</span>
-</span><span id="with_parser-232"><a href="#with_parser-232"><span class="linenos">232</span></a><span class="sd">    &gt;&gt;&gt; E G</span>
-</span><span id="with_parser-233"><a href="#with_parser-233"><span class="linenos">233</span></a><span class="sd">    &gt;&gt;&gt; A D</span>
-</span><span id="with_parser-234"><a href="#with_parser-234"><span class="linenos">234</span></a><span class="sd">    &gt;&gt;&gt; N M&quot;&quot;&quot;</span>
-</span><span id="with_parser-235"><a href="#with_parser-235"><span class="linenos">235</span></a>
-</span><span id="with_parser-236"><a href="#with_parser-236"><span class="linenos">236</span></a>    <span class="k">def</span> <span class="nf">decorator</span><span class="p">(</span>
-</span><span id="with_parser-237"><a href="#with_parser-237"><span class="linenos">237</span></a>        <span class="n">func</span><span class="p">:</span> <span class="n">Callable</span><span class="p">[[</span><span class="n">Any</span><span class="p">,</span> <span class="n">Namespace</span><span class="p">],</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span><span class="p">]</span>
-</span><span id="with_parser-238"><a href="#with_parser-238"><span class="linenos">238</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Callable</span><span class="p">[[</span><span class="n">Any</span><span class="p">,</span> <span class="nb">str</span><span class="p">],</span> <span class="n">Any</span><span class="p">]:</span>
-</span><span id="with_parser-239"><a href="#with_parser-239"><span class="linenos">239</span></a>        <span class="nd">@wraps</span><span class="p">(</span><span class="n">func</span><span class="p">)</span>
-</span><span id="with_parser-240"><a href="#with_parser-240"><span class="linenos">240</span></a>        <span class="k">def</span> <span class="nf">inner</span><span class="p">(</span><span class="bp">self</span><span class="p">:</span> <span class="n">Any</span><span class="p">,</span> <span class="n">command</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Any</span><span class="p">:</span>
-</span><span id="with_parser-241"><a href="#with_parser-241"><span class="linenos">241</span></a>            <span class="k">try</span><span class="p">:</span>
-</span><span id="with_parser-242"><a href="#with_parser-242"><span class="linenos">242</span></a>                <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="p">()</span><span class="o">.</span><span class="n">parse_args</span><span class="p">(</span><span class="n">shlex</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="n">command</span><span class="p">))</span>
-</span><span id="with_parser-243"><a href="#with_parser-243"><span class="linenos">243</span></a>            <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="with_parser-244"><a href="#with_parser-244"><span class="linenos">244</span></a>                <span class="c1"># On parser error, print help and skip post_parser and func execution</span>
-</span><span id="with_parser-245"><a href="#with_parser-245"><span class="linenos">245</span></a>                <span class="k">if</span> <span class="s2">&quot;the following arguments are required&quot;</span> <span class="ow">not</span> <span class="ow">in</span> <span class="nb">str</span><span class="p">(</span><span class="n">e</span><span class="p">):</span>
-</span><span id="with_parser-246"><a href="#with_parser-246"><span class="linenos">246</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;ERROR: </span><span class="si">{</span><span class="n">e</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="with_parser-247"><a href="#with_parser-247"><span class="linenos">247</span></a>                <span class="k">if</span> <span class="s2">&quot;-h&quot;</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">command</span> <span class="ow">and</span> <span class="s2">&quot;--help&quot;</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">command</span><span class="p">:</span>
-</span><span id="with_parser-248"><a href="#with_parser-248"><span class="linenos">248</span></a>                    <span class="k">try</span><span class="p">:</span>
-</span><span id="with_parser-249"><a href="#with_parser-249"><span class="linenos">249</span></a>                        <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="p">()</span><span class="o">.</span><span class="n">parse_args</span><span class="p">([</span><span class="s2">&quot;--help&quot;</span><span class="p">])</span>
-</span><span id="with_parser-250"><a href="#with_parser-250"><span class="linenos">250</span></a>                    <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="with_parser-251"><a href="#with_parser-251"><span class="linenos">251</span></a>                        <span class="k">pass</span>
-</span><span id="with_parser-252"><a href="#with_parser-252"><span class="linenos">252</span></a>                <span class="k">return</span> <span class="kc">None</span>
-</span><span id="with_parser-253"><a href="#with_parser-253"><span class="linenos">253</span></a>            <span class="c1"># Don&#39;t execute function, only print parser help</span>
-</span><span id="with_parser-254"><a href="#with_parser-254"><span class="linenos">254</span></a>            <span class="k">if</span> <span class="s2">&quot;-h&quot;</span> <span class="ow">in</span> <span class="n">command</span> <span class="ow">or</span> <span class="s2">&quot;--help&quot;</span> <span class="ow">in</span> <span class="n">command</span><span class="p">:</span>
+</span><span id="with_parser-196"><a href="#with_parser-196"><span class="linenos">196</span></a><span class="sd">    :param post_parsers: An optional list of functions to execute where each function takes an argshell.Namespace instance and returns an argshell.Namespace instance.</span>
+</span><span id="with_parser-197"><a href="#with_parser-197"><span class="linenos">197</span></a><span class="sd">        &#39;post_parser&#39; functions are executed in the order they are supplied.</span>
+</span><span id="with_parser-198"><a href="#with_parser-198"><span class="linenos">198</span></a>
+</span><span id="with_parser-199"><a href="#with_parser-199"><span class="linenos">199</span></a><span class="sd">    &gt;&gt;&gt; def get_parser() -&gt; argshell.ArgShellParser:</span>
+</span><span id="with_parser-200"><a href="#with_parser-200"><span class="linenos">200</span></a><span class="sd">    &gt;&gt;&gt;     parser = argshell.ArgShellParser()</span>
+</span><span id="with_parser-201"><a href="#with_parser-201"><span class="linenos">201</span></a><span class="sd">    &gt;&gt;&gt;     parser.add_argument(&quot;names&quot;, type=str, nargs=&quot;*&quot;, help=&quot;A list of first and last names to print.&quot;)</span>
+</span><span id="with_parser-202"><a href="#with_parser-202"><span class="linenos">202</span></a><span class="sd">    &gt;&gt;&gt;     parser.add_argument(&quot;-i&quot;, &quot;--initials&quot;, action=&quot;store_true&quot;, help=&quot;Print the initials instead of the full name.&quot;)</span>
+</span><span id="with_parser-203"><a href="#with_parser-203"><span class="linenos">203</span></a><span class="sd">    &gt;&gt;&gt;     return parser</span>
+</span><span id="with_parser-204"><a href="#with_parser-204"><span class="linenos">204</span></a><span class="sd">    &gt;&gt;&gt;</span>
+</span><span id="with_parser-205"><a href="#with_parser-205"><span class="linenos">205</span></a><span class="sd">    &gt;&gt;&gt; # Convert list of first and last names to a list of tuples</span>
+</span><span id="with_parser-206"><a href="#with_parser-206"><span class="linenos">206</span></a><span class="sd">    &gt;&gt;&gt; def names_list_to_tuples(args: argshell.Namespace) -&gt; argshell.Namespace:</span>
+</span><span id="with_parser-207"><a href="#with_parser-207"><span class="linenos">207</span></a><span class="sd">    &gt;&gt;&gt;     args.names = [(first, last) for first, last in zip(args.names[::2], args.names[1::2])]</span>
+</span><span id="with_parser-208"><a href="#with_parser-208"><span class="linenos">208</span></a><span class="sd">    &gt;&gt;&gt;     if args.initials:</span>
+</span><span id="with_parser-209"><a href="#with_parser-209"><span class="linenos">209</span></a><span class="sd">    &gt;&gt;&gt;         args.names = [(name[0][0], name[1][0]) for name in args.names]</span>
+</span><span id="with_parser-210"><a href="#with_parser-210"><span class="linenos">210</span></a><span class="sd">    &gt;&gt;&gt;     return args</span>
+</span><span id="with_parser-211"><a href="#with_parser-211"><span class="linenos">211</span></a><span class="sd">    &gt;&gt;&gt;</span>
+</span><span id="with_parser-212"><a href="#with_parser-212"><span class="linenos">212</span></a><span class="sd">    &gt;&gt;&gt; def capitalize_names(args: argshell.Namespace) -&gt; argshell.Namespace:</span>
+</span><span id="with_parser-213"><a href="#with_parser-213"><span class="linenos">213</span></a><span class="sd">    &gt;&gt;&gt;     args.names = [name.capitalize() for name in args.names]</span>
+</span><span id="with_parser-214"><a href="#with_parser-214"><span class="linenos">214</span></a><span class="sd">    &gt;&gt;&gt;     return args</span>
+</span><span id="with_parser-215"><a href="#with_parser-215"><span class="linenos">215</span></a><span class="sd">    &gt;&gt;&gt;</span>
+</span><span id="with_parser-216"><a href="#with_parser-216"><span class="linenos">216</span></a><span class="sd">    &gt;&gt;&gt; class NameShell(ArgShell):</span>
+</span><span id="with_parser-217"><a href="#with_parser-217"><span class="linenos">217</span></a><span class="sd">    &gt;&gt;&gt;     intro = &quot;Entering nameshell...&quot;</span>
+</span><span id="with_parser-218"><a href="#with_parser-218"><span class="linenos">218</span></a><span class="sd">    &gt;&gt;&gt;     prompt = &quot;nameshell&gt;&quot;</span>
+</span><span id="with_parser-219"><a href="#with_parser-219"><span class="linenos">219</span></a><span class="sd">    &gt;&gt;&gt;</span>
+</span><span id="with_parser-220"><a href="#with_parser-220"><span class="linenos">220</span></a><span class="sd">    &gt;&gt;&gt;     @with_parser(get_parser, [capitalize_names, names_list_to_tuples])</span>
+</span><span id="with_parser-221"><a href="#with_parser-221"><span class="linenos">221</span></a><span class="sd">    &gt;&gt;&gt;     def do_printnames(self, args: argshell.Namespace):</span>
+</span><span id="with_parser-222"><a href="#with_parser-222"><span class="linenos">222</span></a><span class="sd">    &gt;&gt;&gt;         print(*[f&quot;{name[0]} {name[1]}&quot; for name in args.names], sep=&quot;\\n&quot;)</span>
+</span><span id="with_parser-223"><a href="#with_parser-223"><span class="linenos">223</span></a><span class="sd">    &gt;&gt;&gt;</span>
+</span><span id="with_parser-224"><a href="#with_parser-224"><span class="linenos">224</span></a><span class="sd">    &gt;&gt;&gt; NameShell().cmdloop()</span>
+</span><span id="with_parser-225"><a href="#with_parser-225"><span class="linenos">225</span></a><span class="sd">    &gt;&gt;&gt; Entering nameshell...</span>
+</span><span id="with_parser-226"><a href="#with_parser-226"><span class="linenos">226</span></a><span class="sd">    &gt;&gt;&gt; nameshell&gt;printnames karl marx fred hampton emma goldman angela davis nestor makhno</span>
+</span><span id="with_parser-227"><a href="#with_parser-227"><span class="linenos">227</span></a><span class="sd">    &gt;&gt;&gt; Karl Marx</span>
+</span><span id="with_parser-228"><a href="#with_parser-228"><span class="linenos">228</span></a><span class="sd">    &gt;&gt;&gt; Fred Hampton</span>
+</span><span id="with_parser-229"><a href="#with_parser-229"><span class="linenos">229</span></a><span class="sd">    &gt;&gt;&gt; Emma Goldman</span>
+</span><span id="with_parser-230"><a href="#with_parser-230"><span class="linenos">230</span></a><span class="sd">    &gt;&gt;&gt; Angela Davis</span>
+</span><span id="with_parser-231"><a href="#with_parser-231"><span class="linenos">231</span></a><span class="sd">    &gt;&gt;&gt; Nestor Makhno</span>
+</span><span id="with_parser-232"><a href="#with_parser-232"><span class="linenos">232</span></a><span class="sd">    &gt;&gt;&gt; nameshell&gt;printnames karl marx fred hampton emma goldman angela davis nestor makhno -i</span>
+</span><span id="with_parser-233"><a href="#with_parser-233"><span class="linenos">233</span></a><span class="sd">    &gt;&gt;&gt; K M</span>
+</span><span id="with_parser-234"><a href="#with_parser-234"><span class="linenos">234</span></a><span class="sd">    &gt;&gt;&gt; F H</span>
+</span><span id="with_parser-235"><a href="#with_parser-235"><span class="linenos">235</span></a><span class="sd">    &gt;&gt;&gt; E G</span>
+</span><span id="with_parser-236"><a href="#with_parser-236"><span class="linenos">236</span></a><span class="sd">    &gt;&gt;&gt; A D</span>
+</span><span id="with_parser-237"><a href="#with_parser-237"><span class="linenos">237</span></a><span class="sd">    &gt;&gt;&gt; N M&quot;&quot;&quot;</span>
+</span><span id="with_parser-238"><a href="#with_parser-238"><span class="linenos">238</span></a>
+</span><span id="with_parser-239"><a href="#with_parser-239"><span class="linenos">239</span></a>    <span class="k">def</span> <span class="nf">decorator</span><span class="p">(</span>
+</span><span id="with_parser-240"><a href="#with_parser-240"><span class="linenos">240</span></a>        <span class="n">func</span><span class="p">:</span> <span class="n">Callable</span><span class="p">[[</span><span class="n">Any</span><span class="p">,</span> <span class="n">Namespace</span><span class="p">],</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span><span class="p">]</span>
+</span><span id="with_parser-241"><a href="#with_parser-241"><span class="linenos">241</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Callable</span><span class="p">[[</span><span class="n">Any</span><span class="p">,</span> <span class="nb">str</span><span class="p">],</span> <span class="n">Any</span><span class="p">]:</span>
+</span><span id="with_parser-242"><a href="#with_parser-242"><span class="linenos">242</span></a>        <span class="nd">@wraps</span><span class="p">(</span><span class="n">func</span><span class="p">)</span>
+</span><span id="with_parser-243"><a href="#with_parser-243"><span class="linenos">243</span></a>        <span class="k">def</span> <span class="nf">inner</span><span class="p">(</span><span class="bp">self</span><span class="p">:</span> <span class="n">Any</span><span class="p">,</span> <span class="n">command</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Any</span><span class="p">:</span>
+</span><span id="with_parser-244"><a href="#with_parser-244"><span class="linenos">244</span></a>            <span class="k">try</span><span class="p">:</span>
+</span><span id="with_parser-245"><a href="#with_parser-245"><span class="linenos">245</span></a>                <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="p">()</span><span class="o">.</span><span class="n">parse_args</span><span class="p">(</span><span class="n">shlex</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="n">command</span><span class="p">))</span>
+</span><span id="with_parser-246"><a href="#with_parser-246"><span class="linenos">246</span></a>            <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="with_parser-247"><a href="#with_parser-247"><span class="linenos">247</span></a>                <span class="c1"># On parser error, print help and skip post_parser and func execution</span>
+</span><span id="with_parser-248"><a href="#with_parser-248"><span class="linenos">248</span></a>                <span class="k">if</span> <span class="s2">&quot;the following arguments are required&quot;</span> <span class="ow">not</span> <span class="ow">in</span> <span class="nb">str</span><span class="p">(</span><span class="n">e</span><span class="p">):</span>
+</span><span id="with_parser-249"><a href="#with_parser-249"><span class="linenos">249</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;ERROR: </span><span class="si">{</span><span class="n">e</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="with_parser-250"><a href="#with_parser-250"><span class="linenos">250</span></a>                <span class="k">if</span> <span class="s2">&quot;-h&quot;</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">command</span> <span class="ow">and</span> <span class="s2">&quot;--help&quot;</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">command</span><span class="p">:</span>
+</span><span id="with_parser-251"><a href="#with_parser-251"><span class="linenos">251</span></a>                    <span class="k">try</span><span class="p">:</span>
+</span><span id="with_parser-252"><a href="#with_parser-252"><span class="linenos">252</span></a>                        <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="p">()</span><span class="o">.</span><span class="n">parse_args</span><span class="p">([</span><span class="s2">&quot;--help&quot;</span><span class="p">])</span>
+</span><span id="with_parser-253"><a href="#with_parser-253"><span class="linenos">253</span></a>                    <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="with_parser-254"><a href="#with_parser-254"><span class="linenos">254</span></a>                        <span class="k">pass</span>
 </span><span id="with_parser-255"><a href="#with_parser-255"><span class="linenos">255</span></a>                <span class="k">return</span> <span class="kc">None</span>
-</span><span id="with_parser-256"><a href="#with_parser-256"><span class="linenos">256</span></a>            <span class="k">for</span> <span class="n">post_parser</span> <span class="ow">in</span> <span class="n">post_parsers</span><span class="p">:</span>
-</span><span id="with_parser-257"><a href="#with_parser-257"><span class="linenos">257</span></a>                <span class="n">args</span> <span class="o">=</span> <span class="n">post_parser</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
-</span><span id="with_parser-258"><a href="#with_parser-258"><span class="linenos">258</span></a>
-</span><span id="with_parser-259"><a href="#with_parser-259"><span class="linenos">259</span></a>            <span class="k">return</span> <span class="n">func</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">)</span>
-</span><span id="with_parser-260"><a href="#with_parser-260"><span class="linenos">260</span></a>
-</span><span id="with_parser-261"><a href="#with_parser-261"><span class="linenos">261</span></a>        <span class="k">return</span> <span class="n">inner</span>
-</span><span id="with_parser-262"><a href="#with_parser-262"><span class="linenos">262</span></a>
-</span><span id="with_parser-263"><a href="#with_parser-263"><span class="linenos">263</span></a>    <span class="k">return</span> <span class="n">decorator</span>
+</span><span id="with_parser-256"><a href="#with_parser-256"><span class="linenos">256</span></a>            <span class="c1"># Don&#39;t execute function, only print parser help</span>
+</span><span id="with_parser-257"><a href="#with_parser-257"><span class="linenos">257</span></a>            <span class="k">if</span> <span class="s2">&quot;-h&quot;</span> <span class="ow">in</span> <span class="n">command</span> <span class="ow">or</span> <span class="s2">&quot;--help&quot;</span> <span class="ow">in</span> <span class="n">command</span><span class="p">:</span>
+</span><span id="with_parser-258"><a href="#with_parser-258"><span class="linenos">258</span></a>                <span class="k">return</span> <span class="kc">None</span>
+</span><span id="with_parser-259"><a href="#with_parser-259"><span class="linenos">259</span></a>            <span class="k">for</span> <span class="n">post_parser</span> <span class="ow">in</span> <span class="n">post_parsers</span><span class="p">:</span>
+</span><span id="with_parser-260"><a href="#with_parser-260"><span class="linenos">260</span></a>                <span class="n">args</span> <span class="o">=</span> <span class="n">post_parser</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
+</span><span id="with_parser-261"><a href="#with_parser-261"><span class="linenos">261</span></a>
+</span><span id="with_parser-262"><a href="#with_parser-262"><span class="linenos">262</span></a>            <span class="k">return</span> <span class="n">func</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">)</span>
+</span><span id="with_parser-263"><a href="#with_parser-263"><span class="linenos">263</span></a>
+</span><span id="with_parser-264"><a href="#with_parser-264"><span class="linenos">264</span></a>        <span class="k">return</span> <span class="n">inner</span>
+</span><span id="with_parser-265"><a href="#with_parser-265"><span class="linenos">265</span></a>
+</span><span id="with_parser-266"><a href="#with_parser-266"><span class="linenos">266</span></a>    <span class="k">return</span> <span class="n">decorator</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Decorate a 'do_*' function in an argshell.ArgShell class with this function to pass an argshell.Namespace object to the decorated function instead of a string.</p>
 
 <h6 id="parameters">Parameters</h6>
```

#### html2text {}

```diff
@@ -9,14 +9,15 @@
           o error
           o parse_args
     * ArgShell
           o do_quit
           o do_sys
           o do_help
           o cmdloop
+          o emptyline
     * with_parser
 built_with_pdoc[pdoc_logo]
 
 ****** argshell.argshell ******
 ⁰ View Source
 __1import argparse
 __2import cmd
@@ -208,110 +209,113 @@
 177                    import readline
 178
 179                    readline.set_completer(self.old_completer)  # type:
 ignore
 180                except ImportError:
 181                    pass
 182
-183
-184def with_parser(
-185    parser: Callable[..., ArgShellParser],
-186    post_parsers: list[Callable[[Namespace], Namespace]] = [],
-187) -> Callable[[Callable[[Any, Namespace], Any]], Callable[[Any, str], Any]]:
-188    """Decorate a 'do_*' function in an argshell.ArgShell class with this
+183    def emptyline(self):
+184        ...
+185
+186
+187def with_parser(
+188    parser: Callable[..., ArgShellParser],
+189    post_parsers: list[Callable[[Namespace], Namespace]] = [],
+190) -> Callable[[Callable[[Any, Namespace], Any]], Callable[[Any, str], Any]]:
+191    """Decorate a 'do_*' function in an argshell.ArgShell class with this
 function to pass an argshell.Namespace object to the decorated function instead
 of a string.
-189
-190    :param parser: A function that creates an argshell.ArgShellParser
+192
+193    :param parser: A function that creates an argshell.ArgShellParser
 instance, adds arguments to it, and returns the parser.
-191
-192    :param post_parsers: An optional list of functions to execute where each
+194
+195    :param post_parsers: An optional list of functions to execute where each
 function takes an argshell.Namespace instance and returns an argshell.Namespace
 instance.
-193        'post_parser' functions are executed in the order they are supplied.
-194
-195    >>> def get_parser() -> argshell.ArgShellParser:
-196    >>>     parser = argshell.ArgShellParser()
-197    >>>     parser.add_argument("names", type=str, nargs="*", help="A list
+196        'post_parser' functions are executed in the order they are supplied.
+197
+198    >>> def get_parser() -> argshell.ArgShellParser:
+199    >>>     parser = argshell.ArgShellParser()
+200    >>>     parser.add_argument("names", type=str, nargs="*", help="A list
 of first and last names to print.")
-198    >>>     parser.add_argument("-i", "--initials", action="store_true",
+201    >>>     parser.add_argument("-i", "--initials", action="store_true",
 help="Print the initials instead of the full name.")
-199    >>>     return parser
-200    >>>
-201    >>> # Convert list of first and last names to a list of tuples
-202    >>> def names_list_to_tuples(args: argshell.Namespace) -
+202    >>>     return parser
+203    >>>
+204    >>> # Convert list of first and last names to a list of tuples
+205    >>> def names_list_to_tuples(args: argshell.Namespace) -
 > argshell.Namespace:
-203    >>>     args.names = [(first, last) for first, last in zip(args.names[::
+206    >>>     args.names = [(first, last) for first, last in zip(args.names[::
 2], args.names[1::2])]
-204    >>>     if args.initials:
-205    >>>         args.names = [(name[0][0], name[1][0]) for name in
+207    >>>     if args.initials:
+208    >>>         args.names = [(name[0][0], name[1][0]) for name in
 args.names]
-206    >>>     return args
-207    >>>
-208    >>> def capitalize_names(args: argshell.Namespace) -
+209    >>>     return args
+210    >>>
+211    >>> def capitalize_names(args: argshell.Namespace) -
 > argshell.Namespace:
-209    >>>     args.names = [name.capitalize() for name in args.names]
-210    >>>     return args
-211    >>>
-212    >>> class NameShell(ArgShell):
-213    >>>     intro = "Entering nameshell..."
-214    >>>     prompt = "nameshell>"
-215    >>>
-216    >>>     @with_parser(get_parser, [capitalize_names,
+212    >>>     args.names = [name.capitalize() for name in args.names]
+213    >>>     return args
+214    >>>
+215    >>> class NameShell(ArgShell):
+216    >>>     intro = "Entering nameshell..."
+217    >>>     prompt = "nameshell>"
+218    >>>
+219    >>>     @with_parser(get_parser, [capitalize_names,
 names_list_to_tuples])
-217    >>>     def do_printnames(self, args: argshell.Namespace):
-218    >>>         print(*[f"{name[0]} {name[1]}" for name in args.names],
+220    >>>     def do_printnames(self, args: argshell.Namespace):
+221    >>>         print(*[f"{name[0]} {name[1]}" for name in args.names],
 sep="\\n")
-219    >>>
-220    >>> NameShell().cmdloop()
-221    >>> Entering nameshell...
-222    >>> nameshell>printnames karl marx fred hampton emma goldman angela
+222    >>>
+223    >>> NameShell().cmdloop()
+224    >>> Entering nameshell...
+225    >>> nameshell>printnames karl marx fred hampton emma goldman angela
 davis nestor makhno
-223    >>> Karl Marx
-224    >>> Fred Hampton
-225    >>> Emma Goldman
-226    >>> Angela Davis
-227    >>> Nestor Makhno
-228    >>> nameshell>printnames karl marx fred hampton emma goldman angela
+226    >>> Karl Marx
+227    >>> Fred Hampton
+228    >>> Emma Goldman
+229    >>> Angela Davis
+230    >>> Nestor Makhno
+231    >>> nameshell>printnames karl marx fred hampton emma goldman angela
 davis nestor makhno -i
-229    >>> K M
-230    >>> F H
-231    >>> E G
-232    >>> A D
-233    >>> N M"""
-234
-235    def decorator(
-236        func: Callable[[Any, Namespace], Any | None]
-237    ) -> Callable[[Any, str], Any]:
-238        @wraps(func)
-239        def inner(self: Any, command: str) -> Any:
-240            try:
-241                args = parser().parse_args(shlex.split(command))
-242            except Exception as e:
-243                # On parser error, print help and skip post_parser and func
+232    >>> K M
+233    >>> F H
+234    >>> E G
+235    >>> A D
+236    >>> N M"""
+237
+238    def decorator(
+239        func: Callable[[Any, Namespace], Any | None]
+240    ) -> Callable[[Any, str], Any]:
+241        @wraps(func)
+242        def inner(self: Any, command: str) -> Any:
+243            try:
+244                args = parser().parse_args(shlex.split(command))
+245            except Exception as e:
+246                # On parser error, print help and skip post_parser and func
 execution
-244                if "the following arguments are required" not in str(e):
-245                    print(f"ERROR: {e}")
-246                if "-h" not in command and "--help" not in command:
-247                    try:
-248                        args = parser().parse_args(["--help"])
-249                    except Exception as e:
-250                        pass
-251                return None
-252            # Don't execute function, only print parser help
-253            if "-h" in command or "--help" in command:
+247                if "the following arguments are required" not in str(e):
+248                    print(f"ERROR: {e}")
+249                if "-h" not in command and "--help" not in command:
+250                    try:
+251                        args = parser().parse_args(["--help"])
+252                    except Exception as e:
+253                        pass
 254                return None
-255            for post_parser in post_parsers:
-256                args = post_parser(args)
-257
-258            return func(self, args)
-259
-260        return inner
-261
-262    return decorator
+255            # Don't execute function, only print parser help
+256            if "-h" in command or "--help" in command:
+257                return None
+258            for post_parser in post_parsers:
+259                args = post_parser(args)
+260
+261            return func(self, args)
+262
+263        return inner
+264
+265    return decorator
   ⁰
 class Namespace(argparse.Namespace): View Source
 12class Namespace(argparse.Namespace):
 13    """Simple object for storing attributes.
 14
 15    Implements equality by attribute names and values, and provides a simple
 string representation."""
@@ -528,14 +532,17 @@
 177                try:
 178                    import readline
 179
 180                    readline.set_completer(self.old_completer)  # type:
 ignore
 181                except ImportError:
 182                    pass
+183
+184    def emptyline(self):
+185        ...
 Subclass this to create custom ArgShells.
 ⁰
 def do_quit(self, command: str): View Source
 61    def do_quit(self, command: str):
 62        """Quit shell."""
 63        return True
 Quit shell.
@@ -673,116 +680,122 @@
 180                    readline.set_completer(self.old_completer)  # type:
 ignore
 181                except ImportError:
 182                    pass
 Repeatedly issue a prompt, accept input, parse an initial prefix off the
 received input, and dispatch to action methods, passing them the remainder of
 the line as argument.
+⁰
+def emptyline(self): View Source
+184    def emptyline(self):
+185        ...
+Called when an empty line is entered in response to the prompt.
+If this method is not overridden, it repeats the last nonempty command entered.
 ** Inherited Members **
   ⁰
 def with_parser(
 parser: Callable[..., argshell.argshell.ArgShellParser],
 post_parsers: list[typing.Callable[[argshell.argshell.Namespace],
 argshell.argshell.Namespace]] = []) -> Callable[[Callable[[Any,
 argshell.argshell.Namespace], Any]], Callable[[Any, str], Any]]: View Source
-185def with_parser(
-186    parser: Callable[..., ArgShellParser],
-187    post_parsers: list[Callable[[Namespace], Namespace]] = [],
-188) -> Callable[[Callable[[Any, Namespace], Any]], Callable[[Any, str], Any]]:
-189    """Decorate a 'do_*' function in an argshell.ArgShell class with this
+188def with_parser(
+189    parser: Callable[..., ArgShellParser],
+190    post_parsers: list[Callable[[Namespace], Namespace]] = [],
+191) -> Callable[[Callable[[Any, Namespace], Any]], Callable[[Any, str], Any]]:
+192    """Decorate a 'do_*' function in an argshell.ArgShell class with this
 function to pass an argshell.Namespace object to the decorated function instead
 of a string.
-190
-191    :param parser: A function that creates an argshell.ArgShellParser
+193
+194    :param parser: A function that creates an argshell.ArgShellParser
 instance, adds arguments to it, and returns the parser.
-192
-193    :param post_parsers: An optional list of functions to execute where each
+195
+196    :param post_parsers: An optional list of functions to execute where each
 function takes an argshell.Namespace instance and returns an argshell.Namespace
 instance.
-194        'post_parser' functions are executed in the order they are supplied.
-195
-196    >>> def get_parser() -> argshell.ArgShellParser:
-197    >>>     parser = argshell.ArgShellParser()
-198    >>>     parser.add_argument("names", type=str, nargs="*", help="A list
+197        'post_parser' functions are executed in the order they are supplied.
+198
+199    >>> def get_parser() -> argshell.ArgShellParser:
+200    >>>     parser = argshell.ArgShellParser()
+201    >>>     parser.add_argument("names", type=str, nargs="*", help="A list
 of first and last names to print.")
-199    >>>     parser.add_argument("-i", "--initials", action="store_true",
+202    >>>     parser.add_argument("-i", "--initials", action="store_true",
 help="Print the initials instead of the full name.")
-200    >>>     return parser
-201    >>>
-202    >>> # Convert list of first and last names to a list of tuples
-203    >>> def names_list_to_tuples(args: argshell.Namespace) -
+203    >>>     return parser
+204    >>>
+205    >>> # Convert list of first and last names to a list of tuples
+206    >>> def names_list_to_tuples(args: argshell.Namespace) -
 > argshell.Namespace:
-204    >>>     args.names = [(first, last) for first, last in zip(args.names[::
+207    >>>     args.names = [(first, last) for first, last in zip(args.names[::
 2], args.names[1::2])]
-205    >>>     if args.initials:
-206    >>>         args.names = [(name[0][0], name[1][0]) for name in
+208    >>>     if args.initials:
+209    >>>         args.names = [(name[0][0], name[1][0]) for name in
 args.names]
-207    >>>     return args
-208    >>>
-209    >>> def capitalize_names(args: argshell.Namespace) -
+210    >>>     return args
+211    >>>
+212    >>> def capitalize_names(args: argshell.Namespace) -
 > argshell.Namespace:
-210    >>>     args.names = [name.capitalize() for name in args.names]
-211    >>>     return args
-212    >>>
-213    >>> class NameShell(ArgShell):
-214    >>>     intro = "Entering nameshell..."
-215    >>>     prompt = "nameshell>"
-216    >>>
-217    >>>     @with_parser(get_parser, [capitalize_names,
+213    >>>     args.names = [name.capitalize() for name in args.names]
+214    >>>     return args
+215    >>>
+216    >>> class NameShell(ArgShell):
+217    >>>     intro = "Entering nameshell..."
+218    >>>     prompt = "nameshell>"
+219    >>>
+220    >>>     @with_parser(get_parser, [capitalize_names,
 names_list_to_tuples])
-218    >>>     def do_printnames(self, args: argshell.Namespace):
-219    >>>         print(*[f"{name[0]} {name[1]}" for name in args.names],
+221    >>>     def do_printnames(self, args: argshell.Namespace):
+222    >>>         print(*[f"{name[0]} {name[1]}" for name in args.names],
 sep="\\n")
-220    >>>
-221    >>> NameShell().cmdloop()
-222    >>> Entering nameshell...
-223    >>> nameshell>printnames karl marx fred hampton emma goldman angela
+223    >>>
+224    >>> NameShell().cmdloop()
+225    >>> Entering nameshell...
+226    >>> nameshell>printnames karl marx fred hampton emma goldman angela
 davis nestor makhno
-224    >>> Karl Marx
-225    >>> Fred Hampton
-226    >>> Emma Goldman
-227    >>> Angela Davis
-228    >>> Nestor Makhno
-229    >>> nameshell>printnames karl marx fred hampton emma goldman angela
+227    >>> Karl Marx
+228    >>> Fred Hampton
+229    >>> Emma Goldman
+230    >>> Angela Davis
+231    >>> Nestor Makhno
+232    >>> nameshell>printnames karl marx fred hampton emma goldman angela
 davis nestor makhno -i
-230    >>> K M
-231    >>> F H
-232    >>> E G
-233    >>> A D
-234    >>> N M"""
-235
-236    def decorator(
-237        func: Callable[[Any, Namespace], Any | None]
-238    ) -> Callable[[Any, str], Any]:
-239        @wraps(func)
-240        def inner(self: Any, command: str) -> Any:
-241            try:
-242                args = parser().parse_args(shlex.split(command))
-243            except Exception as e:
-244                # On parser error, print help and skip post_parser and func
+233    >>> K M
+234    >>> F H
+235    >>> E G
+236    >>> A D
+237    >>> N M"""
+238
+239    def decorator(
+240        func: Callable[[Any, Namespace], Any | None]
+241    ) -> Callable[[Any, str], Any]:
+242        @wraps(func)
+243        def inner(self: Any, command: str) -> Any:
+244            try:
+245                args = parser().parse_args(shlex.split(command))
+246            except Exception as e:
+247                # On parser error, print help and skip post_parser and func
 execution
-245                if "the following arguments are required" not in str(e):
-246                    print(f"ERROR: {e}")
-247                if "-h" not in command and "--help" not in command:
-248                    try:
-249                        args = parser().parse_args(["--help"])
-250                    except Exception as e:
-251                        pass
-252                return None
-253            # Don't execute function, only print parser help
-254            if "-h" in command or "--help" in command:
+248                if "the following arguments are required" not in str(e):
+249                    print(f"ERROR: {e}")
+250                if "-h" not in command and "--help" not in command:
+251                    try:
+252                        args = parser().parse_args(["--help"])
+253                    except Exception as e:
+254                        pass
 255                return None
-256            for post_parser in post_parsers:
-257                args = post_parser(args)
-258
-259            return func(self, args)
-260
-261        return inner
-262
-263    return decorator
+256            # Don't execute function, only print parser help
+257            if "-h" in command or "--help" in command:
+258                return None
+259            for post_parser in post_parsers:
+260                args = post_parser(args)
+261
+262            return func(self, args)
+263
+264        return inner
+265
+266    return decorator
 Decorate a 'do_*' function in an argshell.ArgShell class with this function to
 pass an argshell.Namespace object to the decorated function instead of a
 string.
 * Parameters *
     * parser: A function that creates an argshell.ArgShellParser instance, adds
       arguments to it, and returns the parser.
     * post_parsers: An optional list of functions to execute where each
```

### Comparing `argshell-1.2.0/src/argshell/argshell.py` & `argshell-1.3.0/src/argshell/argshell.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,14 +176,17 @@
                 try:
                     import readline
 
                     readline.set_completer(self.old_completer)  # type: ignore
                 except ImportError:
                     pass
 
+    def emptyline(self):
+        ...
+
 
 def with_parser(
     parser: Callable[..., ArgShellParser],
     post_parsers: list[Callable[[Namespace], Namespace]] = [],
 ) -> Callable[[Callable[[Any, Namespace], Any]], Callable[[Any, str], Any]]:
     """Decorate a 'do_*' function in an argshell.ArgShell class with this function to pass an argshell.Namespace object to the decorated function instead of a string.
```

### Comparing `argshell-1.2.0/LICENSE.txt` & `argshell-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `argshell-1.2.0/README.md` & `argshell-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `argshell-1.2.0/pyproject.toml` & `argshell-1.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 00000040: 6c69 6e67 2e62 7569 6c64 220d 0a0d 0a5b  ling.build"....[
 00000050: 7072 6f6a 6563 745d 0d0a 6e61 6d65 203d  project]..name =
 00000060: 2022 6172 6773 6865 6c6c 220d 0a64 6573   "argshell"..des
 00000070: 6372 6970 7469 6f6e 203d 2022 496e 7465  cription = "Inte
 00000080: 6772 6174 6573 2074 6865 2061 7267 7061  grates the argpa
 00000090: 7273 6520 616e 6420 636d 6420 6d6f 6475  rse and cmd modu
 000000a0: 6c65 732e 220d 0a76 6572 7369 6f6e 203d  les."..version =
-000000b0: 2022 312e 322e 3022 0d0a 7265 7175 6972   "1.2.0"..requir
+000000b0: 2022 312e 332e 3022 0d0a 7265 7175 6972   "1.3.0"..requir
 000000c0: 6573 2d70 7974 686f 6e20 3d20 223e 3d33  es-python = ">=3
 000000d0: 2e31 3022 0d0a 6465 7065 6e64 656e 6369  .10"..dependenci
 000000e0: 6573 203d 205b 2270 7974 6573 7422 5d0d  es = ["pytest"].
 000000f0: 0a72 6561 646d 6520 3d20 2252 4541 444d  .readme = "READM
 00000100: 452e 6d64 220d 0a6b 6579 776f 7264 7320  E.md"..keywords 
 00000110: 3d20 5b22 6172 6770 6172 7365 222c 2022  = ["argparse", "
 00000120: 636d 6422 2c20 2273 6865 6c6c 222c 2022  cmd", "shell", "
```

### Comparing `argshell-1.2.0/PKG-INFO` & `argshell-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argshell
-Version: 1.2.0
+Version: 1.3.0
 Summary: Integrates the argparse and cmd modules.
 Project-URL: Homepage, https://github.com/matt-manes/argshell
 Project-URL: Documentation, https://github.com/matt-manes/argshell/tree/main/docs
 Project-URL: Source code, https://github.com/matt-manes/argshell/tree/main/src/argshell
 Author-email: Matt Manes <mattmanes@pm.me>
 License-File: LICENSE.txt
 Keywords: argparse,cmd,commandline,shell,terminal
```

