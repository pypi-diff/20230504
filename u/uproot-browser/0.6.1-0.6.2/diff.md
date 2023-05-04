# Comparing `tmp/uproot_browser-0.6.1.tar.gz` & `tmp/uproot_browser-0.6.2.tar.gz`

## Comparing `uproot_browser-0.6.1.tar` & `uproot_browser-0.6.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 uproot_browser-0.6.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 uproot_browser-0.6.1/noxfile.py
--rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 uproot_browser-0.6.1/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 uproot_browser-0.6.1/.github/dependabot.yml
--rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 uproot_browser-0.6.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 uproot_browser-0.6.1/docs/make_logo.py
--rw-r--r--   0        0        0    71775 2020-02-02 00:00:00.000000 uproot_browser-0.6.1/docs/_images/iterm.png
--rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 uproot_browser-0.6.1/docs/_images/uproot-browser-logo.png
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 uproot_browser-0.6.1/src/uproot_browser/__init__.py
--rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 uproot_browser-0.6.1/src/uproot_browser/__main__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 uproot_browser-0.6.1/src/uproot_browser/_version.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 uproot_browser-0.6.1/src/uproot_browser/_version.pyi
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 uproot_browser-0.6.1/src/uproot_browser/dirs.py
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 uproot_browser-0.6.1/src/uproot_browser/exceptions.py
--rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 uproot_browser-0.6.1/src/uproot_browser/plot.py
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 uproot_browser-0.6.1/src/uproot_browser/plot_mpl.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uproot_browser-0.6.1/src/uproot_browser/py.typed
--rw-r--r--   0        0        0     5650 2020-02-02 00:00:00.000000 uproot_browser-0.6.1/src/uproot_browser/tree.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uproot_browser-0.6.1/src/uproot_browser/_compat/__init__.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 uproot_browser-0.6.1/src/uproot_browser/_compat/typing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uproot_browser-0.6.1/src/uproot_browser/_compat/importlib/__init__.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 uproot_browser-0.6.1/src/uproot_browser/_compat/importlib/resources.py
--rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 uproot_browser-0.6.1/src/uproot_browser/tui/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uproot_browser-0.6.1/src/uproot_browser/tui/__init__.py
--rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 uproot_browser-0.6.1/src/uproot_browser/tui/browser.css
--rw-r--r--   0        0        0     5398 2020-02-02 00:00:00.000000 uproot_browser-0.6.1/src/uproot_browser/tui/browser.py
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 uproot_browser-0.6.1/src/uproot_browser/tui/header.py
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 uproot_browser-0.6.1/src/uproot_browser/tui/help.py
--rw-r--r--   0        0        0     3453 2020-02-02 00:00:00.000000 uproot_browser-0.6.1/src/uproot_browser/tui/left_panel.py
--rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 uproot_browser-0.6.1/src/uproot_browser/tui/right_panel.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 uproot_browser-0.6.1/tests/test_dirs.py
--rw-r--r--   0        0        0     4000 2020-02-02 00:00:00.000000 uproot_browser-0.6.1/tests/test_printouts.py
--rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 uproot_browser-0.6.1/.gitignore
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 uproot_browser-0.6.1/LICENSE
--rw-r--r--   0        0        0    10628 2020-02-02 00:00:00.000000 uproot_browser-0.6.1/README.md
--rw-r--r--   0        0        0     4035 2020-02-02 00:00:00.000000 uproot_browser-0.6.1/pyproject.toml
--rw-r--r--   0        0        0    14276 2020-02-02 00:00:00.000000 uproot_browser-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 uproot_browser-0.6.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 uproot_browser-0.6.2/noxfile.py
+-rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 uproot_browser-0.6.2/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 uproot_browser-0.6.2/.github/dependabot.yml
+-rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 uproot_browser-0.6.2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 uproot_browser-0.6.2/docs/make_logo.py
+-rw-r--r--   0        0        0    71775 2020-02-02 00:00:00.000000 uproot_browser-0.6.2/docs/_images/iterm.png
+-rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 uproot_browser-0.6.2/docs/_images/uproot-browser-logo.png
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 uproot_browser-0.6.2/src/uproot_browser/__init__.py
+-rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 uproot_browser-0.6.2/src/uproot_browser/__main__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 uproot_browser-0.6.2/src/uproot_browser/_version.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 uproot_browser-0.6.2/src/uproot_browser/_version.pyi
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 uproot_browser-0.6.2/src/uproot_browser/dirs.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 uproot_browser-0.6.2/src/uproot_browser/exceptions.py
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 uproot_browser-0.6.2/src/uproot_browser/plot.py
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 uproot_browser-0.6.2/src/uproot_browser/plot_mpl.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uproot_browser-0.6.2/src/uproot_browser/py.typed
+-rw-r--r--   0        0        0     5650 2020-02-02 00:00:00.000000 uproot_browser-0.6.2/src/uproot_browser/tree.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uproot_browser-0.6.2/src/uproot_browser/_compat/__init__.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 uproot_browser-0.6.2/src/uproot_browser/_compat/typing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uproot_browser-0.6.2/src/uproot_browser/_compat/importlib/__init__.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 uproot_browser-0.6.2/src/uproot_browser/_compat/importlib/resources.py
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 uproot_browser-0.6.2/src/uproot_browser/tui/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uproot_browser-0.6.2/src/uproot_browser/tui/__init__.py
+-rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 uproot_browser-0.6.2/src/uproot_browser/tui/browser.css
+-rw-r--r--   0        0        0     5398 2020-02-02 00:00:00.000000 uproot_browser-0.6.2/src/uproot_browser/tui/browser.py
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 uproot_browser-0.6.2/src/uproot_browser/tui/header.py
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 uproot_browser-0.6.2/src/uproot_browser/tui/help.py
+-rw-r--r--   0        0        0     3453 2020-02-02 00:00:00.000000 uproot_browser-0.6.2/src/uproot_browser/tui/left_panel.py
+-rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 uproot_browser-0.6.2/src/uproot_browser/tui/right_panel.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 uproot_browser-0.6.2/tests/test_dirs.py
+-rw-r--r--   0        0        0     4000 2020-02-02 00:00:00.000000 uproot_browser-0.6.2/tests/test_printouts.py
+-rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 uproot_browser-0.6.2/.gitignore
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 uproot_browser-0.6.2/LICENSE
+-rw-r--r--   0        0        0    10628 2020-02-02 00:00:00.000000 uproot_browser-0.6.2/README.md
+-rw-r--r--   0        0        0     4035 2020-02-02 00:00:00.000000 uproot_browser-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0    14276 2020-02-02 00:00:00.000000 uproot_browser-0.6.2/PKG-INFO
```

### Comparing `uproot_browser-0.6.1/.pre-commit-config.yaml` & `uproot_browser-0.6.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.6.1/noxfile.py` & `uproot_browser-0.6.2/noxfile.py`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.6.1/.github/CONTRIBUTING.md` & `uproot_browser-0.6.2/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.6.1/.github/workflows/ci.yml` & `uproot_browser-0.6.2/.github/workflows/ci.yml`

 * *Files 1% similar despite different names*

```diff
@@ -90,8 +90,8 @@
 
     steps:
     - uses: actions/download-artifact@v3
       with:
         path: dist
         name: artifact
 
-    - uses: pypa/gh-action-pypi-publish@v1.8.5
+    - uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `uproot_browser-0.6.1/docs/make_logo.py` & `uproot_browser-0.6.2/docs/make_logo.py`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.6.1/docs/_images/iterm.png` & `uproot_browser-0.6.2/docs/_images/iterm.png`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.6.1/docs/_images/uproot-browser-logo.png` & `uproot_browser-0.6.2/docs/_images/uproot-browser-logo.png`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.6.1/src/uproot_browser/__main__.py` & `uproot_browser-0.6.2/src/uproot_browser/__main__.py`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.6.1/src/uproot_browser/dirs.py` & `uproot_browser-0.6.2/src/uproot_browser/dirs.py`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.6.1/src/uproot_browser/plot.py` & `uproot_browser-0.6.2/src/uproot_browser/plot.py`

 * *Files 8% similar despite different names*

```diff
@@ -60,21 +60,23 @@
     finite = values[np.isfinite(values)]
     if len(finite) < 1:
         msg = f"Branch {tree.name} is empty."
         raise EmptyTreeError(msg)
     histogram: hist.Hist = hist.numpy.histogram(finite, bins=100, histogram=hist.Hist)
     plt.bar(histogram.axes[0].centers, histogram.values().astype(float))
     plt.ylim(lower=0)
+    plt.xticks(np.linspace(histogram.axes[0][0][0], histogram.axes[0][-1][-1], 5))
     plt.xlabel(histogram.axes[0].name)
     plt.title(make_hist_title(tree, histogram))
 
 
 @plot.register
 def plot_hist(tree: uproot.behaviors.TH1.Histogram) -> None:
     """
     Plot a 1-D Histogram.
     """
     histogram = hist.Hist(tree.to_hist())
     plt.bar(histogram.axes[0].centers, histogram.values().astype(float))
     plt.ylim(lower=0)
+    plt.xticks(np.linspace(histogram.axes[0][0][0], histogram.axes[0][-1][-1], 5))
     plt.xlabel(histogram.axes[0].name)
     plt.title(make_hist_title(tree, histogram))
```

### Comparing `uproot_browser-0.6.1/src/uproot_browser/plot_mpl.py` & `uproot_browser-0.6.2/src/uproot_browser/plot_mpl.py`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.6.1/src/uproot_browser/tree.py` & `uproot_browser-0.6.2/src/uproot_browser/tree.py`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.6.1/src/uproot_browser/tui/README.md` & `uproot_browser-0.6.2/src/uproot_browser/tui/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 also use the VIM keys: `j` to move down, `k` to move up, `l` to open a folder,
 and `h` to close a folder.
 
 ## Plotting
 
 Histograms, rectangular simple data (e.g. TTree's), and jagged arrays can
 be plotted. Click on an item or press `enter` to plot. If something can't
-be plotted, you'll see a scrollable error traceback.
+be plotted, you'll see a scrollable error traceback. If you think it should
+be plottable, feel free to open an issue. 2D plots are not yet supported.
 
 ## Themes
 
 You can press `t` to toggle light and dark mode.
 
 ## Leaving
 
@@ -29,13 +30,14 @@
 You can press `esc` or `q` to exit this help screen. You can also use `tab` to
 switch between the panes in the help screen. You can use `F1` (or `?`) to access
 the help again.
 
 # Credits
 
 Uproot browser was created by Henry Schreiner and Aman Goel. It was rewritten
-by Elie Svoll and Jose Garcia to use the modern CSS-based Textaul library.
+by Elie Svoll and Jose Ayala Garcia to use the modern CSS-based Textual
+library.
 
 Uproot browser is made possible by the Scikit-HEP ecosystem, including uproot
 and awkward-array for data reading, hist and boost-histogram for computation.
 The TUI (terminal user interface) was built using the Textual library.
 Text-based plotting is provided by plotext.
```

### Comparing `uproot_browser-0.6.1/src/uproot_browser/tui/browser.css` & `uproot_browser-0.6.2/src/uproot_browser/tui/browser.css`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.6.1/src/uproot_browser/tui/browser.py` & `uproot_browser-0.6.2/src/uproot_browser/tui/browser.py`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.6.1/src/uproot_browser/tui/header.py` & `uproot_browser-0.6.2/src/uproot_browser/tui/header.py`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.6.1/src/uproot_browser/tui/help.py` & `uproot_browser-0.6.2/src/uproot_browser/tui/help.py`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.6.1/src/uproot_browser/tui/left_panel.py` & `uproot_browser-0.6.2/src/uproot_browser/tui/left_panel.py`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.6.1/src/uproot_browser/tui/right_panel.py` & `uproot_browser-0.6.2/src/uproot_browser/tui/right_panel.py`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.6.1/tests/test_printouts.py` & `uproot_browser-0.6.2/tests/test_printouts.py`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.6.1/.gitignore` & `uproot_browser-0.6.2/.gitignore`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.6.1/LICENSE` & `uproot_browser-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.6.1/README.md` & `uproot_browser-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.6.1/pyproject.toml` & `uproot_browser-0.6.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `uproot_browser-0.6.1/PKG-INFO` & `uproot_browser-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uproot_browser
-Version: 0.6.1
+Version: 0.6.2
 Summary: Tools to inspect ROOT files with uproot
 Project-URL: homepage, https://github.com/scikit-hep/uproot-browser
 Project-URL: repository, https://github.com/scikit-hep/uproot-browser
 Author-email: Henry Schreiner <henryfs@princeton.edu>
 Maintainer-email: The Scikit-HEP admins <scikit-hep-admins@googlegroups.com>
 License: BSD 3-Clause License
```

