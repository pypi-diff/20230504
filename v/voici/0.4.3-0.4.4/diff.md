# Comparing `tmp/voici-0.4.3.tar.gz` & `tmp/voici-0.4.4.tar.gz`

## Comparing `voici-0.4.3.tar` & `voici-0.4.4.tar`

### file list

```diff
@@ -1,188 +1,190 @@
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 voici-0.4.3/.eslintignore
--rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 voici-0.4.3/.eslintrc.js
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 voici-0.4.3/.prettierignore
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 voici-0.4.3/.prettierrc
--rw-r--r--   0        0        0    15487 2020-02-02 00:00:00.000000 voici-0.4.3/CHANGELOG.md
--rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 voici-0.4.3/CONTRIBUTING.md
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 voici-0.4.3/RELEASE.md
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 voici-0.4.3/environment.yml
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 voici-0.4.3/lerna.json
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 voici-0.4.3/lint-staged.config.js
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 voici-0.4.3/package.json
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 voici-0.4.3/readthedocs.yml
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 voici-0.4.3/setup.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 voici-0.4.3/tsconfig.eslint.json
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 voici-0.4.3/tsconfigbase.json
--rw-r--r--   0        0        0   537654 2020-02-02 00:00:00.000000 voici-0.4.3/yarn.lock
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 voici-0.4.3/demo/environment.yml
--rw-r--r--   0        0        0     3712 2020-02-02 00:00:00.000000 voici-0.4.3/demo/notebooks/iris.csv
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 voici-0.4.3/demo/notebooks/voici.ipynb
--rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 voici-0.4.3/demo/notebooks/widgets/bqplot.ipynb
--rw-r--r--   0        0        0     3147 2020-02-02 00:00:00.000000 voici-0.4.3/demo/notebooks/widgets/ipycanvas.ipynb
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 voici-0.4.3/docs/changelog.md
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 voici-0.4.3/docs/conf.py
--rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 voici-0.4.3/docs/configuration.md
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 voici-0.4.3/docs/contributing.md
--rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 voici-0.4.3/docs/deploy.md
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 voici-0.4.3/docs/environment.yml
--rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 voici-0.4.3/docs/index.md
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 voici-0.4.3/docs/install.md
--rw-r--r--   0        0        0     4594 2020-02-02 00:00:00.000000 voici-0.4.3/docs/voila-logo.svg
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 voici-0.4.3/scripts/bump-version.py
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 voici-0.4.3/ui-tests/package.json
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 voici-0.4.3/ui-tests/playwright.config.js
--rw-r--r--   0        0        0    14600 2020-02-02 00:00:00.000000 voici-0.4.3/ui-tests/yarn.lock
--rw-r--r--   0        0        0     4106 2020-02-02 00:00:00.000000 voici-0.4.3/ui-tests/tests/voici.test.ts
--rw-r--r--   0        0        0     5334 2020-02-02 00:00:00.000000 voici-0.4.3/ui-tests/tests/voici.test.ts-snapshots/voici-bqplot-linux.png
--rw-r--r--   0        0        0     9762 2020-02-02 00:00:00.000000 voici-0.4.3/ui-tests/tests/voici.test.ts-snapshots/voici-dark-linux.png
--rw-r--r--   0        0        0   219768 2020-02-02 00:00:00.000000 voici-0.4.3/ui-tests/tests/voici.test.ts-snapshots/voici-ipycanvas-linux.png
--rw-r--r--   0        0        0    46536 2020-02-02 00:00:00.000000 voici-0.4.3/ui-tests/tests/voici.test.ts-snapshots/voici-simple-linux.png
--rw-r--r--   0        0        0    53032 2020-02-02 00:00:00.000000 voici-0.4.3/ui-tests/tests/voici.test.ts-snapshots/voici-simple-material-linux.png
--rw-r--r--   0        0        0    13254 2020-02-02 00:00:00.000000 voici-0.4.3/ui-tests/tests/voici.test.ts-snapshots/voici-subtree-linux.png
--rw-r--r--   0        0        0    13752 2020-02-02 00:00:00.000000 voici-0.4.3/ui-tests/tests/voici.test.ts-snapshots/voici-subtree-material-linux.png
--rw-r--r--   0        0        0    11652 2020-02-02 00:00:00.000000 voici-0.4.3/ui-tests/tests/voici.test.ts-snapshots/voici-tree-linux.png
--rw-r--r--   0        0        0    12468 2020-02-02 00:00:00.000000 voici-0.4.3/ui-tests/tests/voici.test.ts-snapshots/voici-tree-material-linux.png
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 voici-0.4.3/voici/__init__.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 voici-0.4.3/voici/__main__.py
--rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 voici-0.4.3/voici/_version.py
--rw-r--r--   0        0        0     6943 2020-02-02 00:00:00.000000 voici-0.4.3/voici/addon.py
--rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 voici-0.4.3/voici/app.py
--rw-r--r--   0        0        0     5652 2020-02-02 00:00:00.000000 voici-0.4.3/voici/exporter.py
--rw-r--r--   0        0        0     6442 2020-02-02 00:00:00.000000 voici-0.4.3/voici/tree_exporter.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/index.html
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/1023.js
--rw-r--r--   0        0        0    11364 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/103.js
--rw-r--r--   0        0        0     7661 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/1053.js
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/1058.js
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/1100.js
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/1105.js
--rw-r--r--   0        0        0    23883 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/1432.js
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/1497.js
--rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/1553.js
--rw-r--r--   0        0        0     5730 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/1581.js
--rw-r--r--   0        0        0     6320 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/1667.js
--rw-r--r--   0        0        0    53409 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/1672.js
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/1672.js.LICENSE.txt
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/1732.js
--rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/1770.js
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/1890.js
--rw-r--r--   0        0        0    11366 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/1980.js
--rw-r--r--   0        0        0    24245 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/2075.js
--rw-r--r--   0        0        0     3528 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/2106.js
--rw-r--r--   0        0        0     6625 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/2230.js
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/2266.js
--rw-r--r--   0        0        0     6575 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/2322.js
--rw-r--r--   0        0        0    11365 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/2359.js
--rw-r--r--   0        0        0     8801 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/2361.js
--rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/2488.js
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/2516.js
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/2630.js
--rw-r--r--   0        0        0    11565 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/2687.js
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/275.js
--rw-r--r--   0        0        0     7073 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/2784.js
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/2784.js.LICENSE.txt
--rw-r--r--   0        0        0    11362 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/286.js
--rw-r--r--   0        0        0     9583 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/2950.js
--rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/3008.js
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/3086.js
--rw-r--r--   0        0        0     9580 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/3251.js
--rw-r--r--   0        0        0     3133 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/3256.js
--rw-r--r--   0        0        0   432937 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/330.js
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/3305.js
--rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/3312.js
--rw-r--r--   0        0        0    16166 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/3316.js
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/3316.js.LICENSE.txt
--rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/3349.js
--rw-r--r--   0        0        0   198935 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/339.js
--rw-r--r--   0        0        0     6625 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/3504.js
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/3655.js
--rw-r--r--   0        0        0    13521 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/3693.js
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/3811.js
--rw-r--r--   0        0        0   152146 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/3851.js
--rw-r--r--   0        0        0    11367 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/3922.js
--rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/4259.js
--rw-r--r--   0        0        0    16440 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/4359.js
--rw-r--r--   0        0        0     5269 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/4382.js
--rw-r--r--   0        0        0   173449 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/450.js
--rw-r--r--   0        0        0    44048 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/4530.js
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/4530.js.LICENSE.txt
--rw-r--r--   0        0        0    33749 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/4875.js
--rw-r--r--   0        0        0    11366 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/4896.js
--rw-r--r--   0        0        0    14060 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/4939.js
--rw-r--r--   0        0        0   901522 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/4963.js
--rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/4963.js.LICENSE.txt
--rw-r--r--   0        0        0   130996 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/4977.js
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/5188.js
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/5291.js
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/53.js
--rw-r--r--   0        0        0     3363 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/5403.js
--rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/5445.js
--rw-r--r--   0        0        0    10921 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/5474.js
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/5826.js
--rw-r--r--   0        0        0   104080 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/5950.js
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/5950.js.LICENSE.txt
--rw-r--r--   0        0        0   306356 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/5952.js
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/5952.js.LICENSE.txt
--rw-r--r--   0        0        0    11364 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/596.js
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/5985.js
--rw-r--r--   0        0        0    31585 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/6111.js
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/6178.js
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/6196.js
--rw-r--r--   0        0        0    14725 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/6219.js
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/6219.js.LICENSE.txt
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/6417.js
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/6527.js
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/6587.js
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/6614.js
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/6616.js
--rw-r--r--   0        0        0     5269 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/6757.js
--rw-r--r--   0        0        0     9416 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/6770.js
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/6790.js
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/6839.js
--rw-r--r--   0        0        0    10381 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/6852.js
--rw-r--r--   0        0        0     3133 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/6856.js
--rw-r--r--   0        0        0    88422 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/6914.js
--rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/6976.js
--rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/7003.js
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/7015.js
--rw-r--r--   0        0        0    31429 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/7066.js
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/709.js
--rw-r--r--   0        0        0    89502 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/74.js
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/7469.js
--rw-r--r--   0        0        0    82106 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/7560.js
--rw-r--r--   0        0        0     6320 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/7623.js
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/7695.js
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/7795.js
--rw-r--r--   0        0        0    37531 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/8085.js
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/8164.js
--rw-r--r--   0        0        0    89999 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/8291.js
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/8291.js.LICENSE.txt
--rw-r--r--   0        0        0   123750 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/8316.js
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/8316.js.LICENSE.txt
--rw-r--r--   0        0        0     6170 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/846.js
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/86.js
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/8679.js
--rw-r--r--   0        0        0     9605 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/8809.js
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/8874.js
--rw-r--r--   0        0        0    14229 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/9060.js
--rw-r--r--   0        0        0   528943 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/9112.js
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/9320.js
--rw-r--r--   0        0        0     9624 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/9339.js
--rw-r--r--   0        0        0     5730 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/9406.js
--rw-r--r--   0        0        0   135493 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/9513.js
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/9513.js.LICENSE.txt
--rw-r--r--   0        0        0   248014 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/9727.js
--rw-r--r--   0        0        0    53651 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/9757.js
--rw-r--r--   0        0        0    37027 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/9780.js
--rw-r--r--   0        0        0     7780 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/9807.js
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/9817.js
--rw-r--r--   0        0        0    84485 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/9900.js
--rw-r--r--   0        0        0    22979 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/9988.js
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/service-worker-b2fb40a.js
--rw-r--r--   0        0        0    23502 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/treepage.js
--rw-r--r--   0        0        0    24210 2020-02-02 00:00:00.000000 voici-0.4.3/voici/static/build/voici.js
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 voici-0.4.3/.gitignore
--rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 voici-0.4.3/LICENSE
--rw-r--r--   0        0        0     5395 2020-02-02 00:00:00.000000 voici-0.4.3/README.md
--rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 voici-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     8398 2020-02-02 00:00:00.000000 voici-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 voici-0.4.4/.eslintignore
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 voici-0.4.4/.eslintrc.js
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 voici-0.4.4/.prettierignore
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 voici-0.4.4/.prettierrc
+-rw-r--r--   0        0        0    16099 2020-02-02 00:00:00.000000 voici-0.4.4/CHANGELOG.md
+-rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 voici-0.4.4/CONTRIBUTING.md
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 voici-0.4.4/RELEASE.md
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 voici-0.4.4/environment.yml
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 voici-0.4.4/lerna.json
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 voici-0.4.4/lint-staged.config.js
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 voici-0.4.4/package.json
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 voici-0.4.4/readthedocs.yml
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 voici-0.4.4/setup.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 voici-0.4.4/tsconfig.eslint.json
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 voici-0.4.4/tsconfigbase.json
+-rw-r--r--   0        0        0   538332 2020-02-02 00:00:00.000000 voici-0.4.4/yarn.lock
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 voici-0.4.4/demo/environment.yml
+-rw-r--r--   0        0        0     3712 2020-02-02 00:00:00.000000 voici-0.4.4/demo/notebooks/iris.csv
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 voici-0.4.4/demo/notebooks/voici.ipynb
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 voici-0.4.4/demo/notebooks/widgets/bqplot.ipynb
+-rw-r--r--   0        0        0     3147 2020-02-02 00:00:00.000000 voici-0.4.4/demo/notebooks/widgets/ipycanvas.ipynb
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 voici-0.4.4/docs/changelog.md
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 voici-0.4.4/docs/conf.py
+-rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 voici-0.4.4/docs/configuration.md
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 voici-0.4.4/docs/contributing.md
+-rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 voici-0.4.4/docs/deploy.md
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 voici-0.4.4/docs/environment.yml
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 voici-0.4.4/docs/index.md
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 voici-0.4.4/docs/install.md
+-rw-r--r--   0        0        0     4594 2020-02-02 00:00:00.000000 voici-0.4.4/docs/voila-logo.svg
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 voici-0.4.4/scripts/bump-version.py
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 voici-0.4.4/ui-tests/package.json
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 voici-0.4.4/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0    14600 2020-02-02 00:00:00.000000 voici-0.4.4/ui-tests/yarn.lock
+-rw-r--r--   0        0        0     4106 2020-02-02 00:00:00.000000 voici-0.4.4/ui-tests/tests/voici.test.ts
+-rw-r--r--   0        0        0     5334 2020-02-02 00:00:00.000000 voici-0.4.4/ui-tests/tests/voici.test.ts-snapshots/voici-bqplot-linux.png
+-rw-r--r--   0        0        0     9762 2020-02-02 00:00:00.000000 voici-0.4.4/ui-tests/tests/voici.test.ts-snapshots/voici-dark-linux.png
+-rw-r--r--   0        0        0   219768 2020-02-02 00:00:00.000000 voici-0.4.4/ui-tests/tests/voici.test.ts-snapshots/voici-ipycanvas-linux.png
+-rw-r--r--   0        0        0    46536 2020-02-02 00:00:00.000000 voici-0.4.4/ui-tests/tests/voici.test.ts-snapshots/voici-simple-linux.png
+-rw-r--r--   0        0        0    53032 2020-02-02 00:00:00.000000 voici-0.4.4/ui-tests/tests/voici.test.ts-snapshots/voici-simple-material-linux.png
+-rw-r--r--   0        0        0    13254 2020-02-02 00:00:00.000000 voici-0.4.4/ui-tests/tests/voici.test.ts-snapshots/voici-subtree-linux.png
+-rw-r--r--   0        0        0    13752 2020-02-02 00:00:00.000000 voici-0.4.4/ui-tests/tests/voici.test.ts-snapshots/voici-subtree-material-linux.png
+-rw-r--r--   0        0        0    11652 2020-02-02 00:00:00.000000 voici-0.4.4/ui-tests/tests/voici.test.ts-snapshots/voici-tree-linux.png
+-rw-r--r--   0        0        0    12468 2020-02-02 00:00:00.000000 voici-0.4.4/ui-tests/tests/voici.test.ts-snapshots/voici-tree-material-linux.png
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 voici-0.4.4/voici/__init__.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 voici-0.4.4/voici/__main__.py
+-rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 voici-0.4.4/voici/_version.py
+-rw-r--r--   0        0        0     6943 2020-02-02 00:00:00.000000 voici-0.4.4/voici/addon.py
+-rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 voici-0.4.4/voici/app.py
+-rw-r--r--   0        0        0     5652 2020-02-02 00:00:00.000000 voici-0.4.4/voici/exporter.py
+-rw-r--r--   0        0        0     6442 2020-02-02 00:00:00.000000 voici-0.4.4/voici/tree_exporter.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/index.html
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/1023.js
+-rw-r--r--   0        0        0    11364 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/103.js
+-rw-r--r--   0        0        0     7661 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/1053.js
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/1058.js
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/1100.js
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/1105.js
+-rw-r--r--   0        0        0    23883 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/1432.js
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/1497.js
+-rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/1553.js
+-rw-r--r--   0        0        0     5730 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/1581.js
+-rw-r--r--   0        0        0     6320 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/1667.js
+-rw-r--r--   0        0        0    53409 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/1672.js
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/1672.js.LICENSE.txt
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/1732.js
+-rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/1770.js
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/1890.js
+-rw-r--r--   0        0        0    11366 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/1980.js
+-rw-r--r--   0        0        0    24245 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/2075.js
+-rw-r--r--   0        0        0     3528 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/2106.js
+-rw-r--r--   0        0        0     6625 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/2230.js
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/2266.js
+-rw-r--r--   0        0        0     6575 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/2322.js
+-rw-r--r--   0        0        0    11365 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/2359.js
+-rw-r--r--   0        0        0     8801 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/2361.js
+-rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/2488.js
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/2516.js
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/2630.js
+-rw-r--r--   0        0        0     9934 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/2687.js
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/275.js
+-rw-r--r--   0        0        0     7073 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/2784.js
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/2784.js.LICENSE.txt
+-rw-r--r--   0        0        0    11362 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/286.js
+-rw-r--r--   0        0        0     9583 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/2950.js
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/3008.js
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/3086.js
+-rw-r--r--   0        0        0     9580 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/3251.js
+-rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/3256.js
+-rw-r--r--   0        0        0   432937 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/330.js
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/3305.js
+-rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/3312.js
+-rw-r--r--   0        0        0    16166 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/3316.js
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/3316.js.LICENSE.txt
+-rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/3349.js
+-rw-r--r--   0        0        0   198935 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/339.js
+-rw-r--r--   0        0        0     6625 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/3504.js
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/3655.js
+-rw-r--r--   0        0        0    13521 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/3693.js
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/3811.js
+-rw-r--r--   0        0        0   152146 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/3851.js
+-rw-r--r--   0        0        0    11367 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/3922.js
+-rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/4259.js
+-rw-r--r--   0        0        0    16440 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/4359.js
+-rw-r--r--   0        0        0     5269 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/4382.js
+-rw-r--r--   0        0        0   171818 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/450.js
+-rw-r--r--   0        0        0    44048 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/4530.js
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/4530.js.LICENSE.txt
+-rw-r--r--   0        0        0    33749 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/4875.js
+-rw-r--r--   0        0        0    11366 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/4896.js
+-rw-r--r--   0        0        0    14060 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/4939.js
+-rw-r--r--   0        0        0   901522 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/4963.js
+-rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/4963.js.LICENSE.txt
+-rw-r--r--   0        0        0   130996 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/4977.js
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/5188.js
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/5291.js
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/53.js
+-rw-r--r--   0        0        0     3363 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/5403.js
+-rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/5445.js
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/5826.js
+-rw-r--r--   0        0        0   104080 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/5950.js
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/5950.js.LICENSE.txt
+-rw-r--r--   0        0        0   306356 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/5952.js
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/5952.js.LICENSE.txt
+-rw-r--r--   0        0        0    11364 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/596.js
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/5985.js
+-rw-r--r--   0        0        0    31585 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/6111.js
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/6178.js
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/6196.js
+-rw-r--r--   0        0        0    14742 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/6219.js
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/6219.js.LICENSE.txt
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/6417.js
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/6527.js
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/6587.js
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/6614.js
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/6616.js
+-rw-r--r--   0        0        0     5269 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/6757.js
+-rw-r--r--   0        0        0     9416 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/6770.js
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/6790.js
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/6839.js
+-rw-r--r--   0        0        0    10503 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/6852.js
+-rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/6856.js
+-rw-r--r--   0        0        0    88422 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/6914.js
+-rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/6976.js
+-rw-r--r--   0        0        0    11145 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/7002.js
+-rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/7003.js
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/7015.js
+-rw-r--r--   0        0        0    31429 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/7066.js
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/709.js
+-rw-r--r--   0        0        0    89502 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/74.js
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/7469.js
+-rw-r--r--   0        0        0    82106 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/7560.js
+-rw-r--r--   0        0        0     6320 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/7623.js
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/7695.js
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/7795.js
+-rw-r--r--   0        0        0    37531 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/8085.js
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/8102.js
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/8164.js
+-rw-r--r--   0        0        0    89999 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/8291.js
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/8291.js.LICENSE.txt
+-rw-r--r--   0        0        0   123750 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/8316.js
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/8316.js.LICENSE.txt
+-rw-r--r--   0        0        0     6170 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/846.js
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/86.js
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/8679.js
+-rw-r--r--   0        0        0     9605 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/8809.js
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/8874.js
+-rw-r--r--   0        0        0   131402 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/8921.js
+-rw-r--r--   0        0        0    14229 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/9060.js
+-rw-r--r--   0        0        0   528943 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/9112.js
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/9320.js
+-rw-r--r--   0        0        0     9624 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/9339.js
+-rw-r--r--   0        0        0     5730 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/9406.js
+-rw-r--r--   0        0        0   135493 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/9513.js
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/9513.js.LICENSE.txt
+-rw-r--r--   0        0        0   248014 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/9727.js
+-rw-r--r--   0        0        0    53651 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/9757.js
+-rw-r--r--   0        0        0    37036 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/9780.js
+-rw-r--r--   0        0        0     7780 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/9807.js
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/9817.js
+-rw-r--r--   0        0        0    84485 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/9900.js
+-rw-r--r--   0        0        0    22979 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/9988.js
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/service-worker-b2fb40a.js
+-rw-r--r--   0        0        0    24350 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/treepage.js
+-rw-r--r--   0        0        0    25262 2020-02-02 00:00:00.000000 voici-0.4.4/voici/static/build/voici.js
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 voici-0.4.4/.gitignore
+-rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 voici-0.4.4/LICENSE
+-rw-r--r--   0        0        0     5395 2020-02-02 00:00:00.000000 voici-0.4.4/README.md
+-rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 voici-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0     8398 2020-02-02 00:00:00.000000 voici-0.4.4/PKG-INFO
```

### Comparing `voici-0.4.3/.eslintrc.js` & `voici-0.4.4/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/CHANGELOG.md` & `voici-0.4.4/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,41 @@
 # Changelog
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 0.4.4
+
+([Full Changelog](https://github.com/voila-dashboards/voici/compare/v0.4.3...a8c9f8559318c28938f1b1a75c967a66b28e1f8f))
+
+### Enhancements made
+
+- Import all lumino packages [#77](https://github.com/voila-dashboards/voici/pull/77) ([@trungleduc](https://github.com/trungleduc))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/voila-dashboards/voici/graphs/contributors?from=2023-05-03&to=2023-05-04&type=c))
+
+[@trungleduc](https://github.com/search?q=repo%3Avoila-dashboards%2Fvoici+involves%3Atrungleduc+updated%3A2023-05-03..2023-05-04&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 0.4.3
 
 ([Full Changelog](https://github.com/voila-dashboards/voici/compare/@voila-dashboards/voici@0.4.2...3e2048cfb78a2a340f3ef4e8fab179060168deb8))
 
 ### Bugs fixed
 
 - Hotfix: Fix resize event not being triggered and some CSS issues [#75](https://github.com/voila-dashboards/voici/pull/75) ([@martinRenou](https://github.com/martinRenou))
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/voila-dashboards/voici/graphs/contributors?from=2023-05-03&to=2023-05-03&type=c))
 
 [@github-actions](https://github.com/search?q=repo%3Avoila-dashboards%2Fvoici+involves%3Agithub-actions+updated%3A2023-05-03..2023-05-03&type=Issues) | [@martinRenou](https://github.com/search?q=repo%3Avoila-dashboards%2Fvoici+involves%3AmartinRenou+updated%3A2023-05-03..2023-05-03&type=Issues) | [@trungleduc](https://github.com/search?q=repo%3Avoila-dashboards%2Fvoici+involves%3Atrungleduc+updated%3A2023-05-03..2023-05-03&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 0.4.2
 
 ([Full Changelog](https://github.com/voila-dashboards/voici/compare/@voila-dashboards/voici@0.4.1...3af43dac56a9f9e26d6a2161e0b0cdbd1573949a))
 
 ### Bugs fixed
 
 - Fix outputs DOM structure [#74](https://github.com/voila-dashboards/voici/pull/74) ([@martinRenou](https://github.com/martinRenou))
```

### Comparing `voici-0.4.3/CONTRIBUTING.md` & `voici-0.4.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/RELEASE.md` & `voici-0.4.4/RELEASE.md`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/lint-staged.config.js` & `voici-0.4.4/lint-staged.config.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/package.json` & `voici-0.4.4/package.json`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/tsconfigbase.json` & `voici-0.4.4/tsconfigbase.json`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/yarn.lock` & `voici-0.4.4/yarn.lock`

 * *Files 0% similar despite different names*

```diff
@@ -2374,15 +2374,15 @@
   integrity sha512-Z06lp/yuhz8CtIir3PNTGnuk7909eXt4ukJsCzChsGuot2l5Fbs96RJ/FOHgwCedaX74CtxPjXHXoszFbUA+4A==
 
 "@lumino/algorithm@^2.0.0":
   version "2.0.0"
   resolved "https://registry.yarnpkg.com/@lumino/algorithm/-/algorithm-2.0.0.tgz#f36e4b6bf6d2b9bde66dc3162afc9a0d2ef47530"
   integrity sha512-SwM/8U1zlMWMJj00wTCThdTUit9zap2Xghuo4uUxvZ+mfog5b1UIk2j1dP8TPpzEXHCDPEb85s2/ERo1tee3Dw==
 
-"@lumino/application@^1.27.0", "@lumino/application@^1.31.4":
+"@lumino/application@^1.27.0", "@lumino/application@^1.31.3", "@lumino/application@^1.31.4":
   version "1.31.4"
   resolved "https://registry.yarnpkg.com/@lumino/application/-/application-1.31.4.tgz#b804fcc46fb77deb41aee94c48bea990f735d6b9"
   integrity sha512-dOSsDJ1tXOxC3fnSHvtDQK5RcICLEVPtO19HeCGwurb5W2ZZ55SZT2b5jZu6V/v8lGdtkNbr1RJltRpJRSRb/A==
   dependencies:
     "@lumino/commands" "^1.21.1"
     "@lumino/coreutils" "^1.12.1"
     "@lumino/widgets" "^1.37.2"
@@ -2413,14 +2413,29 @@
   integrity sha512-JLu3nTHzJk9N8ohZ85u75YxemMrmDzJdNgZztfP7F7T7mxND3YVNCkJG35a6aJ7edu1sIgCjBxOvV+hv27iYvQ==
 
 "@lumino/coreutils@^1.11.0 || ^2.0.0-alpha.6", "@lumino/coreutils@^2.1.0":
   version "2.1.0"
   resolved "https://registry.yarnpkg.com/@lumino/coreutils/-/coreutils-2.1.0.tgz#291ed11a1bd143bfd5a2f2638cfb27aefd1bd9ba"
   integrity sha512-1pF3gaTxZY6P+Tixs2rd1aj5HgFOdH3RNupgsMaq0sFmxuvuSxaYhiK5/LB9evDN8a6HqHFeS6wVhVajSOJfDQ==
 
+"@lumino/datagrid@^0.36.0":
+  version "0.36.9"
+  resolved "https://registry.yarnpkg.com/@lumino/datagrid/-/datagrid-0.36.9.tgz#f28973e148b1ca92dae54e920bb92d522f551d82"
+  integrity sha512-qXk2IuUq31xbIYIP6HCy/taydkB/6s2cFPBuuLpAtBnAGO3VNUTI+2KYrsqTZV4odnbH1i0LKoYIpIgiDKs3Qg==
+  dependencies:
+    "@lumino/algorithm" "^1.9.2"
+    "@lumino/coreutils" "^1.12.1"
+    "@lumino/disposable" "^1.10.4"
+    "@lumino/domutils" "^1.8.2"
+    "@lumino/dragdrop" "^1.14.5"
+    "@lumino/keyboard" "^1.8.2"
+    "@lumino/messaging" "^1.10.3"
+    "@lumino/signaling" "^1.11.1"
+    "@lumino/widgets" "^1.37.2"
+
 "@lumino/disposable@^1.10.0", "@lumino/disposable@^1.10.1", "@lumino/disposable@^1.10.4", "@lumino/disposable@^1.7.2":
   version "1.10.4"
   resolved "https://registry.yarnpkg.com/@lumino/disposable/-/disposable-1.10.4.tgz#73b452044fecf988d7fa73fac9451b1a7f987323"
   integrity sha512-4ZxyYcyzUS+ZeB2KAH9oAH3w0DUUceiVr+FIZHZ2TAYGWZI/85WlqJtfm0xjwEpCwLLW1TDqJrISuZu3iMmVMA==
   dependencies:
     "@lumino/algorithm" "^1.9.2"
     "@lumino/signaling" "^1.11.1"
@@ -2441,28 +2456,28 @@
   version "1.14.5"
   resolved "https://registry.yarnpkg.com/@lumino/dragdrop/-/dragdrop-1.14.5.tgz#1db76c8a01f74cb1b0428db6234e820bb58b93ba"
   integrity sha512-LC5xB82+xGF8hFyl716TMpV32OIMIMl+s3RU1PaqDkD6B7PkgiVk6NkJ4X9/GcEvl2igkvlGQt/3L7qxDAJNxw==
   dependencies:
     "@lumino/coreutils" "^1.12.1"
     "@lumino/disposable" "^1.10.4"
 
-"@lumino/keyboard@^1.8.2":
+"@lumino/keyboard@^1.8.0", "@lumino/keyboard@^1.8.2":
   version "1.8.2"
   resolved "https://registry.yarnpkg.com/@lumino/keyboard/-/keyboard-1.8.2.tgz#714dbe671f0718f516d1ec23188b31a9ccd82fb2"
   integrity sha512-Dy+XqQ1wXbcnuYtjys5A0pAqf4SpAFl9NY6owyIhXAo0Va7w3LYp3jgiP1xAaBAwMuUppiUAfrbjrysZuZ625g==
 
 "@lumino/messaging@^1.10.0", "@lumino/messaging@^1.10.1", "@lumino/messaging@^1.10.3", "@lumino/messaging@^1.7.2":
   version "1.10.3"
   resolved "https://registry.yarnpkg.com/@lumino/messaging/-/messaging-1.10.3.tgz#b6227bdfc178a8542571625ecb68063691b6af3c"
   integrity sha512-F/KOwMCdqvdEG8CYAJcBSadzp6aI7a47Fr60zAKGqZATSRRRV41q53iXU7HjFPqQqQIvdn9Z7J32rBEAyQAzww==
   dependencies:
     "@lumino/algorithm" "^1.9.2"
     "@lumino/collections" "^1.9.3"
 
-"@lumino/polling@^1.9.0":
+"@lumino/polling@^1.11.4", "@lumino/polling@^1.9.0":
   version "1.11.4"
   resolved "https://registry.yarnpkg.com/@lumino/polling/-/polling-1.11.4.tgz#ddfe47da5b41af4cfa474898542c099e445c0e6c"
   integrity sha512-yC7JLssj3mqVK6TsYj7dg4AG0rcsC42YtpoDLtz9yzO84Q5flQUfmjAPQB6oPA6wZOlISs3iasF+uO2w1ls5jg==
   dependencies:
     "@lumino/coreutils" "^1.12.1"
     "@lumino/disposable" "^1.10.4"
     "@lumino/signaling" "^1.11.1"
```

### Comparing `voici-0.4.3/demo/notebooks/iris.csv` & `voici-0.4.4/demo/notebooks/iris.csv`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/demo/notebooks/voici.ipynb` & `voici-0.4.4/demo/notebooks/voici.ipynb`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/demo/notebooks/widgets/bqplot.ipynb` & `voici-0.4.4/demo/notebooks/widgets/bqplot.ipynb`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/demo/notebooks/widgets/ipycanvas.ipynb` & `voici-0.4.4/demo/notebooks/widgets/ipycanvas.ipynb`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/docs/conf.py` & `voici-0.4.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/docs/configuration.md` & `voici-0.4.4/docs/configuration.md`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/docs/deploy.md` & `voici-0.4.4/docs/deploy.md`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/docs/index.md` & `voici-0.4.4/docs/index.md`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/docs/install.md` & `voici-0.4.4/docs/install.md`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/docs/voila-logo.svg` & `voici-0.4.4/docs/voila-logo.svg`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/scripts/bump-version.py` & `voici-0.4.4/scripts/bump-version.py`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/ui-tests/package.json` & `voici-0.4.4/ui-tests/package.json`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/ui-tests/yarn.lock` & `voici-0.4.4/ui-tests/yarn.lock`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/ui-tests/tests/voici.test.ts` & `voici-0.4.4/ui-tests/tests/voici.test.ts`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/ui-tests/tests/voici.test.ts-snapshots/voici-bqplot-linux.png` & `voici-0.4.4/ui-tests/tests/voici.test.ts-snapshots/voici-bqplot-linux.png`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/ui-tests/tests/voici.test.ts-snapshots/voici-dark-linux.png` & `voici-0.4.4/ui-tests/tests/voici.test.ts-snapshots/voici-dark-linux.png`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/ui-tests/tests/voici.test.ts-snapshots/voici-ipycanvas-linux.png` & `voici-0.4.4/ui-tests/tests/voici.test.ts-snapshots/voici-ipycanvas-linux.png`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/ui-tests/tests/voici.test.ts-snapshots/voici-simple-linux.png` & `voici-0.4.4/ui-tests/tests/voici.test.ts-snapshots/voici-simple-linux.png`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/ui-tests/tests/voici.test.ts-snapshots/voici-simple-material-linux.png` & `voici-0.4.4/ui-tests/tests/voici.test.ts-snapshots/voici-simple-material-linux.png`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/ui-tests/tests/voici.test.ts-snapshots/voici-subtree-linux.png` & `voici-0.4.4/ui-tests/tests/voici.test.ts-snapshots/voici-subtree-linux.png`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/ui-tests/tests/voici.test.ts-snapshots/voici-subtree-material-linux.png` & `voici-0.4.4/ui-tests/tests/voici.test.ts-snapshots/voici-subtree-material-linux.png`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/ui-tests/tests/voici.test.ts-snapshots/voici-tree-linux.png` & `voici-0.4.4/ui-tests/tests/voici.test.ts-snapshots/voici-tree-linux.png`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/ui-tests/tests/voici.test.ts-snapshots/voici-tree-material-linux.png` & `voici-0.4.4/ui-tests/tests/voici.test.ts-snapshots/voici-tree-material-linux.png`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/_version.py` & `voici-0.4.4/voici/_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Distributed under the terms of the Modified BSD License.
 
 import re
 
 from collections import namedtuple
 
 # Use "hatch version xx.yy.zz" to handle version changes
-__version__ = "0.4.3"
+__version__ = "0.4.4"
 
 # PEP440 version parser
 _version_regex = re.compile(
     r"""
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
```

### Comparing `voici-0.4.3/voici/addon.py` & `voici-0.4.4/voici/addon.py`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/app.py` & `voici-0.4.4/voici/app.py`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/exporter.py` & `voici-0.4.4/voici/exporter.py`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/tree_exporter.py` & `voici-0.4.4/voici/tree_exporter.py`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/1023.js` & `voici-0.4.4/voici/static/build/1023.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/103.js` & `voici-0.4.4/voici/static/build/103.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/1053.js` & `voici-0.4.4/voici/static/build/1053.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/1058.js` & `voici-0.4.4/voici/static/build/1058.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/1100.js` & `voici-0.4.4/voici/static/build/1100.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/1105.js` & `voici-0.4.4/voici/static/build/1105.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/1432.js` & `voici-0.4.4/voici/static/build/1432.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/1553.js` & `voici-0.4.4/voici/static/build/1553.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/1581.js` & `voici-0.4.4/voici/static/build/1581.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/1667.js` & `voici-0.4.4/voici/static/build/1667.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/1672.js` & `voici-0.4.4/voici/static/build/1672.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/1770.js` & `voici-0.4.4/voici/static/build/1770.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/1890.js` & `voici-0.4.4/voici/static/build/1890.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/1980.js` & `voici-0.4.4/voici/static/build/1980.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/2075.js` & `voici-0.4.4/voici/static/build/2075.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/2106.js` & `voici-0.4.4/voici/static/build/2106.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/2230.js` & `voici-0.4.4/voici/static/build/2230.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/2322.js` & `voici-0.4.4/voici/static/build/2322.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/2359.js` & `voici-0.4.4/voici/static/build/2359.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/2361.js` & `voici-0.4.4/voici/static/build/2361.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/2488.js` & `voici-0.4.4/voici/static/build/2488.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/2630.js` & `voici-0.4.4/voici/static/build/2630.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/2687.js` & `voici-0.4.4/voici/static/build/2687.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,28 +1,28 @@
 "use strict";
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
     [2687], {
         62687: (e, t, n) => {
             n.r(t), n.d(t, {
-                CommandRegistry: () => u
+                CommandRegistry: () => m
             });
-            var r, i = n(23203),
+            var i, r = n(23203),
                 o = n(92233),
                 a = n(36e3),
                 s = n(94812),
-                c = n(34938),
+                c = n(26968),
                 d = n(4947),
                 l = function() {
                     return l = Object.assign || function(e) {
-                        for (var t, n = 1, r = arguments.length; n < r; n++)
-                            for (var i in t = arguments[n]) Object.prototype.hasOwnProperty.call(t, i) && (e[i] = t[i]);
+                        for (var t, n = 1, i = arguments.length; n < i; n++)
+                            for (var r in t = arguments[n]) Object.prototype.hasOwnProperty.call(t, r) && (e[r] = t[r]);
                         return e
                     }, l.apply(this, arguments)
                 },
-                u = function() {
+                m = function() {
                     function e() {
                         this._timerID = 0, this._replaying = !1, this._keystrokes = [], this._keydownEvents = [], this._keyBindings = [], this._exactKeyMatch = null, this._commands = Object.create(null), this._commandChanged = new d.Signal(this), this._commandExecuted = new d.Signal(this), this._keyBindingChanged = new d.Signal(this)
                     }
                     return Object.defineProperty(e.prototype, "commandChanged", {
                         get: function() {
                             return this._commandChanged
                         },
@@ -49,15 +49,15 @@
                     }), e.prototype.listCommands = function() {
                         return Object.keys(this._commands)
                     }, e.prototype.hasCommand = function(e) {
                         return e in this._commands
                     }, e.prototype.addCommand = function(e, t) {
                         var n = this;
                         if (e in this._commands) throw new Error("Command '" + e + "' already registered.");
-                        return this._commands[e] = r.createCommand(t), this._commandChanged.emit({
+                        return this._commands[e] = i.createCommand(t), this._commandChanged.emit({
                             id: e,
                             type: "added"
                         }), new a.DisposableDelegate((function() {
                             delete n._commands[e], n._commandChanged.emit({
                                 id: e,
                                 type: "removed"
                             })
@@ -122,171 +122,171 @@
                         return !!n && n.isToggleable
                     }, e.prototype.isVisible = function(e, t) {
                         void 0 === t && (t = o.JSONExt.emptyObject);
                         var n = this._commands[e];
                         return !!n && n.isVisible.call(void 0, t)
                     }, e.prototype.execute = function(e, t) {
                         void 0 === t && (t = o.JSONExt.emptyObject);
-                        var n, r = this._commands[e];
-                        if (!r) return Promise.reject(new Error("Command '" + e + "' not registered."));
+                        var n, i = this._commands[e];
+                        if (!i) return Promise.reject(new Error("Command '" + e + "' not registered."));
                         try {
-                            n = r.execute.call(void 0, t)
+                            n = i.execute.call(void 0, t)
                         } catch (e) {
                             n = Promise.reject(e)
                         }
-                        var i = Promise.resolve(n);
+                        var r = Promise.resolve(n);
                         return this._commandExecuted.emit({
                             id: e,
                             args: t,
-                            result: i
-                        }), i
+                            result: r
+                        }), r
                     }, e.prototype.addKeyBinding = function(e) {
                         var t = this,
-                            n = r.createKeyBinding(e);
+                            n = i.createKeyBinding(e);
                         return this._keyBindings.push(n), this._keyBindingChanged.emit({
                             binding: n,
                             type: "added"
                         }), new a.DisposableDelegate((function() {
-                            i.ArrayExt.removeFirstOf(t._keyBindings, n), t._keyBindingChanged.emit({
+                            r.ArrayExt.removeFirstOf(t._keyBindings, n), t._keyBindingChanged.emit({
                                 binding: n,
                                 type: "removed"
                             })
                         }))
                     }, e.prototype.processKeydownEvent = function(t) {
                         if (!this._replaying && !e.isModifierKeyPressed(t)) {
                             var n = e.keystrokeForKeydownEvent(t);
                             if (!n) return this._replayKeydownEvents(), void this._clearPendingState();
                             this._keystrokes.push(n);
-                            var i = r.matchKeyBinding(this._keyBindings, this._keystrokes, t),
-                                o = i.exact,
-                                a = i.partial;
+                            var r = i.matchKeyBinding(this._keyBindings, this._keystrokes, t),
+                                o = r.exact,
+                                a = r.partial;
                             if (!o && !a) return this._replayKeydownEvents(), void this._clearPendingState();
                             if (t.preventDefault(), t.stopPropagation(), o && !a) return this._executeKeyBinding(o), void this._clearPendingState();
                             o && (this._exactKeyMatch = o), this._keydownEvents.push(t), this._startTimer()
                         }
                     }, e.prototype._startTimer = function() {
                         var e = this;
                         this._clearTimer(), this._timerID = window.setTimeout((function() {
                             e._onPendingTimeout()
-                        }), r.CHORD_TIMEOUT)
+                        }), i.CHORD_TIMEOUT)
                     }, e.prototype._clearTimer = function() {
                         0 !== this._timerID && (clearTimeout(this._timerID), this._timerID = 0)
                     }, e.prototype._replayKeydownEvents = function() {
-                        0 !== this._keydownEvents.length && (this._replaying = !0, this._keydownEvents.forEach(r.replayKeyEvent), this._replaying = !1)
+                        0 !== this._keydownEvents.length && (this._replaying = !0, this._keydownEvents.forEach(i.replayKeyEvent), this._replaying = !1)
                     }, e.prototype._executeKeyBinding = function(e) {
                         var t = e.command,
                             n = e.args;
                         if (this.hasCommand(t) && this.isEnabled(t, n)) this.execute(t, n);
                         else {
-                            var r = this.hasCommand(t) ? "enabled" : "registered",
-                                i = "Cannot execute key binding '" + e.keys.join(", ") + "':",
-                                o = "command '" + t + "' is not " + r + ".";
-                            console.warn(i + " " + o)
+                            var i = this.hasCommand(t) ? "enabled" : "registered",
+                                r = "Cannot execute key binding '" + e.keys.join(", ") + "':",
+                                o = "command '" + t + "' is not " + i + ".";
+                            console.warn(r + " " + o)
                         }
                     }, e.prototype._clearPendingState = function() {
                         this._clearTimer(), this._exactKeyMatch = null, this._keystrokes.length = 0, this._keydownEvents.length = 0
                     }, e.prototype._onPendingTimeout = function() {
                         this._timerID = 0, this._exactKeyMatch ? this._executeKeyBinding(this._exactKeyMatch) : this._replayKeydownEvents(), this._clearPendingState()
                     }, e
                 }();
             ! function(e) {
                 function t(e) {
-                    for (var t = "", n = !1, r = !1, i = !1, o = !1, a = 0, c = e.split(/\s+/); a < c.length; a++) {
+                    for (var t = "", n = !1, i = !1, r = !1, o = !1, a = 0, c = e.split(/\s+/); a < c.length; a++) {
                         var d = c[a];
-                        "Accel" === d ? s.Platform.IS_MAC ? r = !0 : i = !0 : "Alt" === d ? n = !0 : "Cmd" === d ? r = !0 : "Ctrl" === d ? i = !0 : "Shift" === d ? o = !0 : d.length > 0 && (t = d)
+                        "Accel" === d ? s.Platform.IS_MAC ? i = !0 : r = !0 : "Alt" === d ? n = !0 : "Cmd" === d ? i = !0 : "Ctrl" === d ? r = !0 : "Shift" === d ? o = !0 : d.length > 0 && (t = d)
                     }
                     return {
-                        cmd: r,
-                        ctrl: i,
+                        cmd: i,
+                        ctrl: r,
                         alt: n,
                         shift: o,
                         key: t
                     }
                 }
 
                 function n(e) {
                     var n = "",
-                        r = t(e);
-                    return r.ctrl && (n += "Ctrl "), r.alt && (n += "Alt "), r.shift && (n += "Shift "), r.cmd && s.Platform.IS_MAC && (n += "Cmd "), n + r.key
+                        i = t(e);
+                    return i.ctrl && (n += "Ctrl "), i.alt && (n += "Alt "), i.shift && (n += "Shift "), i.cmd && s.Platform.IS_MAC && (n += "Cmd "), n + i.key
                 }
                 e.parseKeystroke = t, e.normalizeKeystroke = n, e.normalizeKeys = function(e) {
                     return (s.Platform.IS_WIN ? e.winKeys || e.keys : s.Platform.IS_MAC ? e.macKeys || e.keys : e.linuxKeys || e.keys).map(n)
                 }, e.formatKeystroke = function(e) {
                     return "string" == typeof e ? n(e) : e.map(n).join(", ");
 
                     function n(e) {
                         var n = [],
-                            i = s.Platform.IS_MAC ? " " : "+",
+                            r = s.Platform.IS_MAC ? " " : "+",
                             o = t(e);
-                        return o.ctrl && n.push("Ctrl"), o.alt && n.push("Alt"), o.shift && n.push("Shift"), s.Platform.IS_MAC && o.cmd && n.push("Cmd"), n.push(o.key), n.map(r.formatKey).join(i)
+                        return o.ctrl && n.push("Ctrl"), o.alt && n.push("Alt"), o.shift && n.push("Shift"), s.Platform.IS_MAC && o.cmd && n.push("Cmd"), n.push(o.key), n.map(i.formatKey).join(r)
                     }
                 }, e.isModifierKeyPressed = function(e) {
-                    var t = (0, c.Vc)(),
+                    var t = (0, c.getKeyboardLayout)(),
                         n = t.keyForKeydownEvent(e);
                     return t.isModifierKey(n)
                 }, e.keystrokeForKeydownEvent = function(e) {
-                    var t = (0, c.Vc)(),
+                    var t = (0, c.getKeyboardLayout)(),
                         n = t.keyForKeydownEvent(e);
                     if (!n || t.isModifierKey(n)) return "";
-                    var r = [];
-                    return e.ctrlKey && r.push("Ctrl"), e.altKey && r.push("Alt"), e.shiftKey && r.push("Shift"), e.metaKey && s.Platform.IS_MAC && r.push("Cmd"), r.push(n), r.join(" ")
+                    var i = [];
+                    return e.ctrlKey && i.push("Ctrl"), e.altKey && i.push("Alt"), e.shiftKey && i.push("Shift"), e.metaKey && s.Platform.IS_MAC && i.push("Cmd"), i.push(n), i.join(" ")
                 }
-            }(u || (u = {})),
+            }(m || (m = {})),
             function(e) {
                 e.CHORD_TIMEOUT = 1e3, e.createCommand = function(e) {
                     var t, n;
-                    return e.icon && "string" != typeof e.icon ? (n = m(e.iconClass, r), t = m(e.icon, y)) : t = n = m(e.iconClass || e.icon, r), {
+                    return e.icon && "string" != typeof e.icon ? (n = y(e.iconClass, i), t = y(e.icon, u)) : t = n = y(e.iconClass || e.icon, i), {
                         execute: e.execute,
                         describedBy: l({
                             args: null
                         }, e.describedBy),
-                        label: m(e.label, r),
-                        mnemonic: m(e.mnemonic, i),
+                        label: y(e.label, i),
+                        mnemonic: y(e.mnemonic, r),
                         icon: t,
                         iconClass: n,
-                        iconLabel: m(e.iconLabel, r),
-                        caption: m(e.caption, r),
-                        usage: m(e.usage, r),
-                        className: m(e.className, r),
-                        dataset: m(e.dataset, d),
+                        iconLabel: y(e.iconLabel, i),
+                        caption: y(e.caption, i),
+                        usage: y(e.usage, i),
+                        className: y(e.className, i),
+                        dataset: y(e.dataset, d),
                         isEnabled: e.isEnabled || a,
                         isToggled: e.isToggled || c,
                         isToggleable: e.isToggleable || !!e.isToggled,
                         isVisible: e.isVisible || a
                     }
                 }, e.createKeyBinding = function(e) {
                     return {
-                        keys: u.normalizeKeys(e),
+                        keys: m.normalizeKeys(e),
                         selector: h(e),
                         command: e.command,
                         args: e.args || o.JSONExt.emptyObject
                     }
                 }, e.matchKeyBinding = function(e, t, n) {
-                    for (var r = null, i = !1, o = 1 / 0, a = 0, c = 0, d = e.length; c < d; ++c) {
+                    for (var i = null, r = !1, o = 1 / 0, a = 0, c = 0, d = e.length; c < d; ++c) {
                         var l = e[c],
-                            u = p(l.keys, t);
-                        if (0 !== u)
-                            if (2 !== u) {
-                                var y = f(l.selector, n);
-                                if (!(-1 === y || y > o)) {
-                                    var m = s.Selector.calculateSpecificity(l.selector);
-                                    (!r || y < o || m >= a) && (r = l, o = y, a = m)
+                            m = p(l.keys, t);
+                        if (0 !== m)
+                            if (2 !== m) {
+                                var u = f(l.selector, n);
+                                if (!(-1 === u || u > o)) {
+                                    var y = s.Selector.calculateSpecificity(l.selector);
+                                    (!i || u < o || y >= a) && (i = l, o = u, a = y)
                                 }
-                            } else i || -1 === f(l.selector, n) || (i = !0)
+                            } else r || -1 === f(l.selector, n) || (r = !0)
                     }
                     return {
-                        exact: r,
-                        partial: i
+                        exact: i,
+                        partial: r
                     }
                 }, e.replayKeyEvent = function(e) {
                     e.target.dispatchEvent(function(e) {
                         var t = document.createEvent("Event"),
                             n = e.bubbles || !0,
-                            r = e.cancelable || !0;
-                        return t.initEvent(e.type || "keydown", n, r), t.key = e.key || "", t.keyCode = e.keyCode || 0, t.which = e.keyCode || 0, t.ctrlKey = e.ctrlKey || !1, t.altKey = e.altKey || !1, t.shiftKey = e.shiftKey || !1, t.metaKey = e.metaKey || !1, t.view = e.view || window, t
+                            i = e.cancelable || !0;
+                        return t.initEvent(e.type || "keydown", n, i), t.key = e.key || "", t.keyCode = e.keyCode || 0, t.which = e.keyCode || 0, t.ctrlKey = e.ctrlKey || !1, t.altKey = e.altKey || !1, t.shiftKey = e.shiftKey || !1, t.metaKey = e.metaKey || !1, t.view = e.view || window, t
                     }(e))
                 }, e.formatKey = function(e) {
                     return s.Platform.IS_MAC ? t.hasOwnProperty(e) ? t[e] : e : n.hasOwnProperty(e) ? n[e] : e
                 };
                 var t = {
                         Backspace: "⌫",
                         Tab: "⇥",
@@ -312,192 +312,56 @@
                         PageDown: "Page Down",
                         ArrowLeft: "Left",
                         ArrowUp: "Up",
                         ArrowRight: "Right",
                         ArrowDown: "Down",
                         Delete: "Del"
                     },
-                    r = function() {
+                    i = function() {
                         return ""
                     },
-                    i = function() {
+                    r = function() {
                         return -1
                     },
                     a = function() {
                         return !0
                     },
                     c = function() {
                         return !1
                     },
                     d = function() {
                         return {}
                     },
-                    y = function() {};
+                    u = function() {};
 
-                function m(e, t) {
+                function y(e, t) {
                     return void 0 === e ? t : "function" == typeof e ? e : function() {
                         return e
                     }
                 }
 
                 function h(e) {
                     if (-1 !== e.selector.indexOf(",")) throw new Error("Selector cannot contain commas: " + e.selector);
                     if (!s.Selector.isValid(e.selector)) throw new Error("Invalid selector: " + e.selector);
                     return e.selector
                 }
 
                 function p(e, t) {
                     if (e.length < t.length) return 0;
-                    for (var n = 0, r = t.length; n < r; ++n)
+                    for (var n = 0, i = t.length; n < i; ++n)
                         if (e[n] !== t[n]) return 0;
                     return e.length > t.length ? 2 : 1
                 }
 
                 function f(e, t) {
-                    for (var n = t.target, r = t.currentTarget, i = 0; null !== n; n = n.parentElement, ++i) {
+                    for (var n = t.target, i = t.currentTarget, r = 0; null !== n; n = n.parentElement, ++r) {
                         if (n.hasAttribute("data-lm-suppress-shortcuts")) return -1;
                         if (n.hasAttribute("data-p-suppress-shortcuts")) return -1;
-                        if (s.Selector.matches(n, e)) return i;
-                        if (n === r) return -1
+                        if (s.Selector.matches(n, e)) return r;
+                        if (n === i) return -1
                     }
                     return -1
                 }
-            }(r || (r = {}))
-        },
-        34938: (e, t, n) => {
-            function r() {
-                return o.keyboardLayout
-            }
-            n.d(t, {
-                Vc: () => r
-            });
-            var i = function() {
-                function e(t, n, r) {
-                    void 0 === r && (r = []), this.name = t, this._codes = n, this._keys = e.extractKeys(n), this._modifierKeys = e.convertToKeySet(r)
-                }
-                return e.prototype.keys = function() {
-                    return Object.keys(this._keys)
-                }, e.prototype.isValidKey = function(e) {
-                    return e in this._keys
-                }, e.prototype.isModifierKey = function(e) {
-                    return e in this._modifierKeys
-                }, e.prototype.keyForKeydownEvent = function(e) {
-                    return this._codes[e.keyCode] || ""
-                }, e
-            }();
-            ! function(e) {
-                e.extractKeys = function(e) {
-                    var t = Object.create(null);
-                    for (var n in e) t[e[n]] = !0;
-                    return t
-                }, e.convertToKeySet = function(e) {
-                    for (var t = Object(null), n = 0, r = e.length; n < r; ++n) t[e[n]] = !0;
-                    return t
-                }
-            }(i || (i = {}));
-            var o, a = new i("en-us", {
-                8: "Backspace",
-                9: "Tab",
-                13: "Enter",
-                16: "Shift",
-                17: "Ctrl",
-                18: "Alt",
-                19: "Pause",
-                27: "Escape",
-                32: "Space",
-                33: "PageUp",
-                34: "PageDown",
-                35: "End",
-                36: "Home",
-                37: "ArrowLeft",
-                38: "ArrowUp",
-                39: "ArrowRight",
-                40: "ArrowDown",
-                45: "Insert",
-                46: "Delete",
-                48: "0",
-                49: "1",
-                50: "2",
-                51: "3",
-                52: "4",
-                53: "5",
-                54: "6",
-                55: "7",
-                56: "8",
-                57: "9",
-                59: ";",
-                61: "=",
-                65: "A",
-                66: "B",
-                67: "C",
-                68: "D",
-                69: "E",
-                70: "F",
-                71: "G",
-                72: "H",
-                73: "I",
-                74: "J",
-                75: "K",
-                76: "L",
-                77: "M",
-                78: "N",
-                79: "O",
-                80: "P",
-                81: "Q",
-                82: "R",
-                83: "S",
-                84: "T",
-                85: "U",
-                86: "V",
-                87: "W",
-                88: "X",
-                89: "Y",
-                90: "Z",
-                91: "Meta",
-                93: "ContextMenu",
-                96: "0",
-                97: "1",
-                98: "2",
-                99: "3",
-                100: "4",
-                101: "5",
-                102: "6",
-                103: "7",
-                104: "8",
-                105: "9",
-                106: "*",
-                107: "+",
-                109: "-",
-                110: ".",
-                111: "/",
-                112: "F1",
-                113: "F2",
-                114: "F3",
-                115: "F4",
-                116: "F5",
-                117: "F6",
-                118: "F7",
-                119: "F8",
-                120: "F9",
-                121: "F10",
-                122: "F11",
-                123: "F12",
-                173: "-",
-                186: ";",
-                187: "=",
-                188: ",",
-                189: "-",
-                190: ".",
-                191: "/",
-                192: "`",
-                219: "[",
-                220: "\\",
-                221: "]",
-                222: "'",
-                224: "Meta"
-            }, ["Shift", "Ctrl", "Alt", "Meta"]);
-            ! function(e) {
-                e.keyboardLayout = a
-            }(o || (o = {}))
+            }(i || (i = {}))
         }
     }
 ]);
```

### Comparing `voici-0.4.3/voici/static/build/275.js` & `voici-0.4.4/voici/static/build/275.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/2784.js` & `voici-0.4.4/voici/static/build/2784.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/286.js` & `voici-0.4.4/voici/static/build/286.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/2950.js` & `voici-0.4.4/voici/static/build/2950.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/3008.js` & `voici-0.4.4/voici/static/build/3008.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/3086.js` & `voici-0.4.4/voici/static/build/3086.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/3251.js` & `voici-0.4.4/voici/static/build/3251.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/3256.js` & `voici-0.4.4/voici/static/build/3256.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,20 +1,20 @@
 "use strict";
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
     [3256, 6856], {
         93256: (e, t, r) => {
             r.r(t), r.d(t, {
-                IServiceWorkerManager: () => l,
+                IServiceWorkerManager: () => h,
                 JupyterLiteServer: () => a,
                 Router: () => o,
-                ServiceWorkerManager: () => _,
+                ServiceWorkerManager: () => p,
                 WORKER_NAME: () => u
             });
             var i = r(2132),
-                s = r(76219),
+                s = r(8971),
                 n = r(79988);
             class o {
                 constructor() {
                     this._routes = []
                 }
                 get(e, t) {
                     this._add("GET", e, t)
@@ -62,15 +62,15 @@
                     "string" == typeof t && (t = new RegExp(t)), this._routes.push({
                         method: e,
                         pattern: t,
                         callback: r
                     })
                 }
             }
-            class a extends s.M {
+            class a extends s.Application {
                 constructor(e) {
                     var t;
                     super(e), this.name = "JupyterLite Server", this.namespace = this.name, this.version = "unknown", this._router = new o, this._serviceManager = new i.ServiceManager({
                         standby: "never",
                         serverSettings: {
                             ...i.ServerConnection.makeSettings(),
                             WebSocket: n.WebSocket,
@@ -103,20 +103,20 @@
                 registerPluginModules(e) {
                     e.forEach((e => {
                         this.registerPluginModule(e)
                     }))
                 }
             }
             var c = r(92233);
-            const h = r.p + "service-worker-b2fb40a.js",
-                l = new c.Token("@jupyterlite/server-extension:IServiceWorkerManager"),
-                u = `${h}`.split("/").slice(-1)[0];
+            const l = r.p + "service-worker-b2fb40a.js",
+                h = new c.Token("@jupyterlite/server-extension:IServiceWorkerManager"),
+                u = `${l}`.split("/").slice(-1)[0];
             var g = r(4947),
                 d = r(86086);
-            class _ {
+            class p {
                 constructor() {
                     this._registration = null, this._registrationChanged = new g.Signal(this), this._ready = new c.PromiseDelegate, this.initialize().catch(console.warn)
                 }
                 get registrationChanged() {
                     return this._registrationChanged
                 }
                 get enabled() {
```

### Comparing `voici-0.4.3/voici/static/build/330.js` & `voici-0.4.4/voici/static/build/330.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/3305.js` & `voici-0.4.4/voici/static/build/3305.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/3312.js` & `voici-0.4.4/voici/static/build/3312.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/3316.js` & `voici-0.4.4/voici/static/build/3316.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/3316.js.LICENSE.txt` & `voici-0.4.4/voici/static/build/3316.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/3349.js` & `voici-0.4.4/voici/static/build/3349.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/339.js` & `voici-0.4.4/voici/static/build/339.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1555,15 +1555,15 @@
                     if (1 === d.length) {
                         const e = d[0];
                         return console.warn("No exact match found for " + e + ", using kernel " + e + " that matches language=" + s), e
                     }
                     return c
                 }, e.populateKernelSelect = i
             }(te || (te = {}));
-            var ie = n(82361);
+            var ie = n(48157);
             const re = "toolbar-popup-opener",
                 se = "jp-Toolbar-spacer";
             class oe extends l.PanelLayout {
                 constructor() {
                     super(...arguments), this._dirty = !1
                 }
                 onFitRequest(e) {
```

### Comparing `voici-0.4.3/voici/static/build/3504.js` & `voici-0.4.4/voici/static/build/3504.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/3655.js` & `voici-0.4.4/voici/static/build/3655.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/3693.js` & `voici-0.4.4/voici/static/build/3693.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/3811.js` & `voici-0.4.4/voici/static/build/3811.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/3851.js` & `voici-0.4.4/voici/static/build/3851.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/3922.js` & `voici-0.4.4/voici/static/build/3922.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/4259.js` & `voici-0.4.4/voici/static/build/4259.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/4359.js` & `voici-0.4.4/voici/static/build/4359.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/4382.js` & `voici-0.4.4/voici/static/build/4382.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/450.js` & `voici-0.4.4/voici/static/build/450.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,146 +1,10 @@
 "use strict";
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
     [450], {
-        34938: (e, t, i) => {
-            function n() {
-                return r.keyboardLayout
-            }
-            i.d(t, {
-                Vc: () => n
-            });
-            var o = function() {
-                function e(t, i, n) {
-                    void 0 === n && (n = []), this.name = t, this._codes = i, this._keys = e.extractKeys(i), this._modifierKeys = e.convertToKeySet(n)
-                }
-                return e.prototype.keys = function() {
-                    return Object.keys(this._keys)
-                }, e.prototype.isValidKey = function(e) {
-                    return e in this._keys
-                }, e.prototype.isModifierKey = function(e) {
-                    return e in this._modifierKeys
-                }, e.prototype.keyForKeydownEvent = function(e) {
-                    return this._codes[e.keyCode] || ""
-                }, e
-            }();
-            ! function(e) {
-                e.extractKeys = function(e) {
-                    var t = Object.create(null);
-                    for (var i in e) t[e[i]] = !0;
-                    return t
-                }, e.convertToKeySet = function(e) {
-                    for (var t = Object(null), i = 0, n = e.length; i < n; ++i) t[e[i]] = !0;
-                    return t
-                }
-            }(o || (o = {}));
-            var r, s = new o("en-us", {
-                8: "Backspace",
-                9: "Tab",
-                13: "Enter",
-                16: "Shift",
-                17: "Ctrl",
-                18: "Alt",
-                19: "Pause",
-                27: "Escape",
-                32: "Space",
-                33: "PageUp",
-                34: "PageDown",
-                35: "End",
-                36: "Home",
-                37: "ArrowLeft",
-                38: "ArrowUp",
-                39: "ArrowRight",
-                40: "ArrowDown",
-                45: "Insert",
-                46: "Delete",
-                48: "0",
-                49: "1",
-                50: "2",
-                51: "3",
-                52: "4",
-                53: "5",
-                54: "6",
-                55: "7",
-                56: "8",
-                57: "9",
-                59: ";",
-                61: "=",
-                65: "A",
-                66: "B",
-                67: "C",
-                68: "D",
-                69: "E",
-                70: "F",
-                71: "G",
-                72: "H",
-                73: "I",
-                74: "J",
-                75: "K",
-                76: "L",
-                77: "M",
-                78: "N",
-                79: "O",
-                80: "P",
-                81: "Q",
-                82: "R",
-                83: "S",
-                84: "T",
-                85: "U",
-                86: "V",
-                87: "W",
-                88: "X",
-                89: "Y",
-                90: "Z",
-                91: "Meta",
-                93: "ContextMenu",
-                96: "0",
-                97: "1",
-                98: "2",
-                99: "3",
-                100: "4",
-                101: "5",
-                102: "6",
-                103: "7",
-                104: "8",
-                105: "9",
-                106: "*",
-                107: "+",
-                109: "-",
-                110: ".",
-                111: "/",
-                112: "F1",
-                113: "F2",
-                114: "F3",
-                115: "F4",
-                116: "F5",
-                117: "F6",
-                118: "F7",
-                119: "F8",
-                120: "F9",
-                121: "F10",
-                122: "F11",
-                123: "F12",
-                173: "-",
-                186: ";",
-                187: "=",
-                188: ",",
-                189: "-",
-                190: ".",
-                191: "/",
-                192: "`",
-                219: "[",
-                220: "\\",
-                221: "]",
-                222: "'",
-                224: "Meta"
-            }, ["Shift", "Ctrl", "Alt", "Meta"]);
-            ! function(e) {
-                e.keyboardLayout = s
-            }(r || (r = {}))
-        },
         90450: (e, t, i) => {
             i.r(t), i.d(t, {
                 AccordionLayout: () => P,
                 AccordionPanel: () => R,
                 BoxEngine: () => g,
                 BoxLayout: () => H,
                 BoxPanel: () => j,
@@ -155,15 +19,15 @@
                 LayoutItem: () => C,
                 Menu: () => U,
                 MenuBar: () => oe,
                 Panel: () => B,
                 PanelLayout: () => E,
                 ScrollBar: () => se,
                 SingletonLayout: () => de,
-                SplitLayout: () => I,
+                SplitLayout: () => z,
                 SplitPanel: () => k,
                 StackedLayout: () => he,
                 StackedPanel: () => ce,
                 TabBar: () => G,
                 TabPanel: () => ue,
                 Title: () => _,
                 Widget: () => M
@@ -174,15 +38,15 @@
                 s = i(24629),
                 a = i(4947),
                 d = i(3860),
                 h = i(92233),
                 c = i(1514),
                 l = i(32886),
                 u = i(36e3),
-                p = i(34938),
+                p = i(26968),
                 m = function(e, t) {
                     return m = Object.setPrototypeOf || {
                         __proto__: []
                     }
                     instanceof Array && function(e, t) {
                         e.__proto__ = t
                     } || function(e, t) {
@@ -897,15 +761,15 @@
                     name: "verticalAlignment",
                     create: function() {
                         return "top"
                     },
                     changed: t
                 })
             }(w || (w = {}));
-            var A, E = function(e) {
+            var L, E = function(e) {
                 function t() {
                     var t = null !== e && e.apply(this, arguments) || this;
                     return t._widgets = [], t
                 }
                 return f(t, e), t.prototype.dispose = function() {
                     for (; this._widgets.length > 0;) this._widgets.pop().dispose();
                     e.prototype.dispose.call(this)
@@ -946,20 +810,20 @@
                     this.parent.isAttached && r.MessageLoop.sendMessage(t, M.Msg.BeforeDetach), this.parent.node.removeChild(t.node), this.parent.isAttached && r.MessageLoop.sendMessage(t, M.Msg.AfterDetach)
                 }, t
             }(x);
             ! function(e) {
                 e.clampDimension = function(e) {
                     return Math.max(0, Math.floor(e))
                 }
-            }(A || (A = {}));
-            var L, S = A,
-                I = function(e) {
+            }(L || (L = {}));
+            var A, S = L,
+                z = function(e) {
                     function t(t) {
                         var i = e.call(this) || this;
-                        return i.widgetOffset = 0, i._fixed = 0, i._spacing = 4, i._dirty = !1, i._hasNormedSizes = !1, i._sizers = [], i._items = [], i._handles = [], i._box = null, i._alignment = "start", i._orientation = "horizontal", i.renderer = t.renderer, void 0 !== t.orientation && (i._orientation = t.orientation), void 0 !== t.alignment && (i._alignment = t.alignment), void 0 !== t.spacing && (i._spacing = A.clampDimension(t.spacing)), i
+                        return i.widgetOffset = 0, i._fixed = 0, i._spacing = 4, i._dirty = !1, i._hasNormedSizes = !1, i._sizers = [], i._items = [], i._handles = [], i._box = null, i._alignment = "start", i._orientation = "horizontal", i.renderer = t.renderer, void 0 !== t.orientation && (i._orientation = t.orientation), void 0 !== t.alignment && (i._alignment = t.alignment), void 0 !== t.spacing && (i._spacing = L.clampDimension(t.spacing)), i
                     }
                     return f(t, e), t.prototype.dispose = function() {
                         (0, n.each)(this._items, (function(e) {
                             e.dispose()
                         })), this._box = null, this._items.length = 0, this._sizers.length = 0, this._handles.length = 0, e.prototype.dispose.call(this)
                     }, Object.defineProperty(t.prototype, "orientation", {
                         get: function() {
@@ -980,36 +844,36 @@
                         enumerable: !0,
                         configurable: !0
                     }), Object.defineProperty(t.prototype, "spacing", {
                         get: function() {
                             return this._spacing
                         },
                         set: function(e) {
-                            e = A.clampDimension(e), this._spacing !== e && (this._spacing = e, this.parent && this.parent.fit())
+                            e = L.clampDimension(e), this._spacing !== e && (this._spacing = e, this.parent && this.parent.fit())
                         },
                         enumerable: !0,
                         configurable: !0
                     }), Object.defineProperty(t.prototype, "handles", {
                         get: function() {
                             return this._handles
                         },
                         enumerable: !0,
                         configurable: !0
                     }), t.prototype.absoluteSizes = function() {
                         return this._sizers.map((function(e) {
                             return e.size
                         }))
                     }, t.prototype.relativeSizes = function() {
-                        return L.normalize(this._sizers.map((function(e) {
+                        return A.normalize(this._sizers.map((function(e) {
                             return e.size
                         })))
                     }, t.prototype.setRelativeSizes = function(e, t) {
                         void 0 === t && (t = !0);
                         for (var i = this._sizers.length, n = e.slice(0, i); n.length < i;) n.push(0);
-                        for (var o = L.normalize(n), r = 0; r < i; ++r) {
+                        for (var o = A.normalize(n), r = 0; r < i; ++r) {
                             var s = this._sizers[r];
                             s.sizeHint = o[r], s.size = o[r]
                         }
                         this._hasNormedSizes = !0, t && this.parent && this.parent.update()
                     }, t.prototype.moveHandle = function(e, t) {
                         var i, n = this._handles[e];
                         if (n && !n.classList.contains("lm-mod-hidden") && 0 != (i = "horizontal" === this._orientation ? t - n.offsetLeft : t - n.offsetTop)) {
@@ -1019,17 +883,17 @@
                             }
                             g.adjust(this._sizers, e, i), this.parent && this.parent.update()
                         }
                     }, t.prototype.init = function() {
                         this.parent.dataset.orientation = this.orientation, this.parent.dataset.alignment = this.alignment, e.prototype.init.call(this)
                     }, t.prototype.attachWidget = function(e, t) {
                         var i = new C(t),
-                            o = L.createHandle(this.renderer),
-                            s = L.averageSize(this._sizers),
-                            a = L.createSizer(s);
+                            o = A.createHandle(this.renderer),
+                            s = A.averageSize(this._sizers),
+                            a = A.createSizer(s);
                         n.ArrayExt.insert(this._items, e, i), n.ArrayExt.insert(this._sizers, e, a), n.ArrayExt.insert(this._handles, e, o), this.parent.isAttached && r.MessageLoop.sendMessage(t, M.Msg.BeforeAttach), this.parent.node.appendChild(t.node), this.parent.node.appendChild(o), this.parent.isAttached && r.MessageLoop.sendMessage(t, M.Msg.AfterAttach), this.parent.fit()
                     }, t.prototype.moveWidget = function(e, t, i) {
                         n.ArrayExt.move(this._items, e, t), n.ArrayExt.move(this._sizers, e, t), n.ArrayExt.move(this._handles, e, t), this.parent.fit()
                     }, t.prototype.detachWidget = function(e, t) {
                         var i = n.ArrayExt.removeAt(this._items, e),
                             o = n.ArrayExt.removeAt(this._handles, e);
                         n.ArrayExt.removeAt(this._sizers, e), this.parent.isAttached && r.MessageLoop.sendMessage(t, M.Msg.BeforeDetach), this.parent.node.removeChild(t.node), this.parent.node.removeChild(o), this.parent.isAttached && r.MessageLoop.sendMessage(t, M.Msg.AfterDetach), i.dispose(), this.parent.fit()
@@ -1109,30 +973,30 @@
                                 u ? a += b + y : s += b + y
                             }
                         }
                     }, t
                 }(E);
             ! function(e) {
                 e.getStretch = function(e) {
-                    return L.stretchProperty.get(e)
+                    return A.stretchProperty.get(e)
                 }, e.setStretch = function(e, t) {
-                    L.stretchProperty.set(e, t)
+                    A.stretchProperty.set(e, t)
                 }
-            }(I || (I = {})),
+            }(z || (z = {})),
             function(e) {
                 e.stretchProperty = new s.AttachedProperty({
                     name: "stretch",
                     create: function() {
                         return 0
                     },
                     coerce: function(e, t) {
                         return Math.max(0, Math.floor(t))
                     },
                     changed: function(e) {
-                        e.parent && e.parent.layout instanceof I && e.parent.fit()
+                        e.parent && e.parent.layout instanceof z && e.parent.fit()
                     }
                 }), e.createSizer = function(e) {
                     var t = new b;
                     return t.sizeHint = Math.floor(e), t
                 }, e.createHandle = function(e) {
                     var t = e.createHandle();
                     return t.style.position = "absolute", t
@@ -1148,16 +1012,16 @@
                     }), 0);
                     return 0 === i ? e.map((function(e) {
                         return 1 / t
                     })) : e.map((function(e) {
                         return e / i
                     }))
                 }
-            }(L || (L = {}));
-            var z, P = function(e) {
+            }(A || (A = {}));
+            var I, P = function(e) {
                 function t(t) {
                     var i = e.call(this, v(v({}, t), {
                         orientation: t.orientation || "vertical"
                     })) || this;
                     return i._titles = [], i.titleSpace = t.titleSpace || 22, i
                 }
                 return f(t, e), Object.defineProperty(t.prototype, "titleSpace", {
@@ -1176,36 +1040,36 @@
                     enumerable: !0,
                     configurable: !0
                 }), t.prototype.dispose = function() {
                     this.isDisposed || (this._titles.length = 0, e.prototype.dispose.call(this))
                 }, t.prototype.updateTitle = function(e, t) {
                     var i = this._titles[e],
                         n = i.classList.contains("lm-mod-expanded"),
-                        o = z.createTitle(this.renderer, t.title, n);
+                        o = I.createTitle(this.renderer, t.title, n);
                     this._titles[e] = o, this.parent.node.replaceChild(o, i)
                 }, t.prototype.attachWidget = function(t, i) {
-                    var o = z.createTitle(this.renderer, i.title);
+                    var o = I.createTitle(this.renderer, i.title);
                     n.ArrayExt.insert(this._titles, t, o), this.parent.node.appendChild(o), i.node.setAttribute("role", "region"), i.node.setAttribute("aria-labelledby", o.id), e.prototype.attachWidget.call(this, t, i)
                 }, t.prototype.moveWidget = function(t, i, o) {
                     n.ArrayExt.move(this._titles, t, i), e.prototype.moveWidget.call(this, t, i, o)
                 }, t.prototype.detachWidget = function(t, i) {
                     var o = n.ArrayExt.removeAt(this._titles, t);
                     this.parent.node.removeChild(o), e.prototype.detachWidget.call(this, t, i)
                 }, t.prototype.updateItemPosition = function(t, i, n, o, r, s, a) {
                     var d = this._titles[t].style;
                     d.top = o + "px", d.left = n + "px", d.height = this.widgetOffset + "px", d.width = i ? r + "px" : s + "px", e.prototype.updateItemPosition.call(this, t, i, n, o, r, s, a)
                 }, t
-            }(I);
+            }(z);
             ! function(e) {
                 e.createTitle = function(e, t, i) {
                     void 0 === i && (i = !0);
                     var n = e.createSectionTitle(t);
                     return n.style.position = "absolute", n.setAttribute("aria-label", t.label + " Section"), n.setAttribute("aria-expanded", i ? "true" : "false"), n.setAttribute("aria-controls", t.owner.id), i && n.classList.add("lm-mod-expanded"), n
                 }
-            }(z || (z = {}));
+            }(I || (I = {}));
             var T, B = function(e) {
                 function t(t) {
                     void 0 === t && (t = {});
                     var i = e.call(this) || this;
                     return i.addClass("lm-Panel"), i.addClass("p-Panel"), i.layout = T.createLayout(t), i
                 }
                 return f(t, e), Object.defineProperty(t.prototype, "widgets", {
@@ -1352,22 +1216,22 @@
                     function e() {}
                     return e.prototype.createHandle = function() {
                         var e = document.createElement("div");
                         return e.className = "lm-SplitPanel-handle", e.classList.add("p-SplitPanel-handle"), e
                     }, e
                 }();
                 e.Renderer = t, e.defaultRenderer = new t, e.getStretch = function(e) {
-                    return I.getStretch(e)
+                    return z.getStretch(e)
                 }, e.setStretch = function(e, t) {
-                    I.setStretch(e, t)
+                    z.setStretch(e, t)
                 }
             }(k || (k = {})),
             function(e) {
                 e.createLayout = function(e) {
-                    return e.layout || new I({
+                    return e.layout || new z({
                         renderer: e.renderer || k.defaultRenderer,
                         orientation: e.orientation,
                         alignment: e.alignment,
                         spacing: e.spacing
                     })
                 }
             }(D || (D = {}));
@@ -2388,15 +2252,15 @@
                     var t = e.keyCode;
                     if (13 !== t)
                         if (27 !== t)
                             if (37 !== t)
                                 if (38 !== t)
                                     if (39 !== t)
                                         if (40 !== t) {
-                                            var i = (0, p.Vc)().keyForKeydownEvent(e);
+                                            var i = (0, p.getKeyboardLayout)().keyForKeydownEvent(e);
                                             if (i) {
                                                 var n = this._activeIndex + 1,
                                                     o = V.findMnemonic(this._items, i, n); - 1 === o.index || o.multiple ? -1 !== o.index ? this.activeIndex = o.index : -1 !== o.auto && (this.activeIndex = o.auto) : (this.activeIndex = o.index, this.triggerActiveItem())
                                             }
                                         } else this.activateNextItem();
                     else {
                         var r = this.activeItem;
@@ -4678,16 +4542,16 @@
                                     b = Math.min(v.row, d),
                                     y = Math.min(v.column, h),
                                     _ = Math.min(v.row + v.rowSpan - 1, d),
                                     M = Math.min(v.column + v.columnSpan - 1, h),
                                     x = this._columnStarts[y],
                                     w = this._rowStarts[b],
                                     C = this._columnStarts[M] + this._columnSizers[M].size - x,
-                                    A = this._rowStarts[_] + this._rowSizers[_].size - w;
-                                f.update(x, w, C, A)
+                                    L = this._rowStarts[_] + this._rowSizers[_].size - w;
+                                f.update(x, w, C, L)
                             }
                         }
                     }, t
                 }(x);
             ! function(e) {
                 e.getCellConfig = function(e) {
                     return ee.cellConfigProperty.get(e)
@@ -4857,15 +4721,15 @@
                 }, t.prototype._evtKeyDown = function(e) {
                     var t = e.keyCode;
                     if (9 !== t)
                         if (e.preventDefault(), e.stopPropagation(), 13 !== t && 32 !== t && 38 !== t && 40 !== t) {
                             if (27 === t) return this._closeChildMenu(), this.activeIndex = -1, void this.node.blur();
                             if (37 !== t)
                                 if (39 !== t) {
-                                    var i = (0, p.Vc)().keyForKeydownEvent(e);
+                                    var i = (0, p.getKeyboardLayout)().keyForKeydownEvent(e);
                                     if (i) {
                                         var n = this._activeIndex + 1,
                                             o = ne.findMnemonic(this._menus, i, n); - 1 === o.index || o.multiple ? -1 !== o.index ? this.activeIndex = o.index : -1 !== o.auto && (this.activeIndex = o.auto) : (this.activeIndex = o.index, this.openActiveMenu())
                                     }
                                 } else r = this._activeIndex, s = this._menus.length, this.activeIndex = r === s - 1 ? 0 : r + 1;
                             else {
                                 var r = this._activeIndex,
```

### Comparing `voici-0.4.3/voici/static/build/4530.js` & `voici-0.4.4/voici/static/build/4530.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/4875.js` & `voici-0.4.4/voici/static/build/4875.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/4896.js` & `voici-0.4.4/voici/static/build/4896.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/4939.js` & `voici-0.4.4/voici/static/build/4939.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/4963.js` & `voici-0.4.4/voici/static/build/4963.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/4963.js.LICENSE.txt` & `voici-0.4.4/voici/static/build/4963.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/4977.js` & `voici-0.4.4/voici/static/build/4977.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -481,15 +481,15 @@
                     }
                 }
             }(b || (b = {}));
             var w = n(48085),
                 k = n(59110),
                 S = n(24643),
                 x = n(23203),
-                O = n(82361),
+                O = n(48157),
                 M = n(42051),
                 E = n(94812),
                 D = n(97505),
                 N = n.n(D);
             class I extends o.ReactWidget {
                 constructor() {
                     super(), this.addClass("jp-Collapser")
```

### Comparing `voici-0.4.3/voici/static/build/5188.js` & `voici-0.4.4/voici/static/build/5188.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/5291.js` & `voici-0.4.4/voici/static/build/5291.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/53.js` & `voici-0.4.4/voici/static/build/53.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/5403.js` & `voici-0.4.4/voici/static/build/5403.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/5445.js` & `voici-0.4.4/voici/static/build/5445.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/5474.js` & `voici-0.4.4/voici/static/build/6852.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,13 @@
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
-    [5474], {
+    [6852, 2233], {
         27693: e => {
             e.exports = {
                 name: "@voila-dashboards/voici",
-                version: "0.4.3",
+                version: "0.4.4",
                 description: "The Voici Frontend",
                 author: "Voilà contributors",
                 license: "BSD-3-Clause",
                 main: "lib/index.js",
                 browserslist: ">0.8%, not ie 11, not op_mini all, not dead",
                 dependencies: {
                     "@jupyter-widgets/base": "^6.0.1",
@@ -38,20 +38,24 @@
                     "@jupyterlab/ui-components": "^3.0.0",
                     "@jupyterlite/contents": "^0.1.0",
                     "@jupyterlite/iframe-extension": "^0.1.0",
                     "@jupyterlite/kernel": "^0.1.0",
                     "@jupyterlite/server": "^0.1.0",
                     "@jupyterlite/server-extension": "^0.1.0",
                     "@lumino/algorithm": "^1.6.2",
+                    "@lumino/application": "^1.31.3",
                     "@lumino/commands": "^1.15.2",
                     "@lumino/coreutils": "^1.8.2",
+                    "@lumino/datagrid": "^0.36.0",
                     "@lumino/disposable": "^1.7.2",
                     "@lumino/domutils": "^1.5.2",
                     "@lumino/dragdrop": "^1.10.2",
+                    "@lumino/keyboard": "^1.8.0",
                     "@lumino/messaging": "^1.7.2",
+                    "@lumino/polling": "^1.11.4",
                     "@lumino/properties": "^1.5.2",
                     "@lumino/signaling": "^1.7.2",
                     "@lumino/virtualdom": "^1.11.2",
                     "@lumino/widgets": "^1.26.2",
                     "@voila-dashboards/voila": "^0.5.0-alpha.3",
                     react: "^17.0.1",
                     "react-dom": "^17.0.1"
@@ -93,37 +97,36 @@
                     watch: 'tsc-watch --onSuccess "webpack --mode=development"'
                 },
                 publishConfig: {
                     access: "public"
                 }
             }
         },
-        65474: (e, t, n) => {
+        46852: (e, t, n) => {
             "use strict";
-            n.r(t), n(24627);
+            n.r(t);
             var i = n(59110),
                 a = n(94456),
-                o = n(7631),
-                r = n(22312),
-                s = n(75238),
-                l = n(73198),
-                u = n(40049),
-                c = n(12299),
-                d = n(35918),
-                p = n(92233),
-                g = n(42051);
-            const m = n(27693),
-                f = "application/vnd.jupyter.widget-view+json";
-            class h extends s.JupyterFrontEnd {
+                o = n(22312),
+                r = n(75238),
+                s = n(73198),
+                l = n(40049),
+                u = n(12299),
+                c = n(35918),
+                d = n(92233),
+                p = n(42051);
+            const g = n(27693),
+                m = "application/vnd.jupyter.widget-view+json";
+            class h extends r.JupyterFrontEnd {
                 constructor(e) {
                     var t;
                     if (super(Object.assign(Object.assign({}, e), {
-                            shell: null !== (t = e.shell) && void 0 !== t ? t : new r.VoilaShell
-                        })), this.name = "Voici", this.namespace = this.name, this.version = m.version, this._widgetManagerPromise = new p.PromiseDelegate, e.mimeExtensions)
-                        for (const t of (0, s.createRendermimePlugins)(e.mimeExtensions)) this.registerPlugin(t);
+                            shell: null !== (t = e.shell) && void 0 !== t ? t : new o.VoilaShell
+                        })), this.name = "Voici", this.namespace = this.name, this.version = g.version, this._widgetManagerPromise = new d.PromiseDelegate, e.mimeExtensions)
+                        for (const t of (0, r.createRendermimePlugins)(e.mimeExtensions)) this.registerPlugin(t);
                     this._kernelspecs = e.kernelspecs, this._serviceManager = e.serviceManager
                 }
                 get widgetManagerPromise() {
                     return this._widgetManagerPromise
                 }
                 get paths() {
                     return {
@@ -171,52 +174,52 @@
                 async renderWidgets() {
                     var e, t, n;
                     const a = this._serviceManager;
                     if (!a) return void console.error("Missing service manager");
                     await a.ready;
                     const o = a.sessions;
                     await o.ready;
-                    const r = new u.NotebookModel;
+                    const r = new l.NotebookModel;
                     r.fromString(i.PageConfig.getOption("notebookSrc"));
                     let s = r.metadata.get("kernelspec");
                     s || (s = {
                         name: "python"
                     });
-                    const l = null === (t = null === (e = this._kernelspecs) || void 0 === e ? void 0 : e.specs) || void 0 === t ? void 0 : t.kernelspecs;
+                    const d = null === (t = null === (e = this._kernelspecs) || void 0 === e ? void 0 : e.specs) || void 0 === t ? void 0 : t.kernelspecs;
                     let p;
-                    if (!l) return void console.error("No kernel available");
-                    if (s.name in l) console.log(`${s.name} kernel is available!`), p = l[s.name];
+                    if (!d) return void console.error("No kernel available");
+                    if (s.name in d) console.log(`${s.name} kernel is available!`), p = d[s.name];
                     else
-                        for (const e in l)
-                            if (s.language === (null === (n = l[e]) || void 0 === n ? void 0 : n.language)) {
-                                console.log(`${s.name} kernel is not available, fallback to using ${l[e].name}`), p = l[e];
+                        for (const e in d)
+                            if (s.language === (null === (n = d[e]) || void 0 === n ? void 0 : n.language)) {
+                                console.log(`${s.name} kernel is not available, fallback to using ${d[e].name}`), p = d[e];
                                 break
                             } if (!p) return void console.error(`No kernel available for ${s.language}`);
                     const g = await o.startNew({
                             name: "",
                             path: "",
                             type: "notebook",
                             kernel: p
                         }),
-                        m = g.kernel;
-                    m ? m.connectionStatusChanged.connect((async (e, t) => {
+                        h = g.kernel;
+                    h ? h.connectionStatusChanged.connect((async (e, t) => {
                         if ("connected" === t) {
                             window.update_loading_text(0, 0, "Starting up kernel...");
-                            const e = new c.RenderMimeRegistry({
-                                    initialFactories: c.standardRendererFactories
+                            const e = new u.RenderMimeRegistry({
+                                    initialFactories: u.standardRendererFactories
                                 }),
-                                t = new d.KernelWidgetManager(m, e);
-                            if (e.removeMimeType(f), e.addFactory({
+                                t = new c.KernelWidgetManager(h, e);
+                            if (e.removeMimeType(m), e.addFactory({
                                     safe: !1,
-                                    mimeTypes: [f],
-                                    createRenderer: e => new d.WidgetRenderer(e, t)
+                                    mimeTypes: [m],
+                                    createRenderer: e => new c.WidgetRenderer(e, t)
                                 }, -10), this._widgetManagerPromise.resolve(t), !g.kernel) return;
                             await new Promise((e => setTimeout(e, 500)));
                             let n = !1;
-                            m.statusChanged.connect((async (t, i) => {
+                            h.statusChanged.connect((async (t, i) => {
                                 n || "idle" !== i || (n = !0, await b.executeCells({
                                     source: r,
                                     rendermime: e,
                                     kernel: g.kernel
                                 }))
                             }))
                         }
@@ -227,145 +230,127 @@
             ! function(e) {
                 e.executeCells = async function(e) {
                     var t, n;
                     const {
                         source: a,
                         rendermime: o,
                         kernel: r
-                    } = e, s = a.cells.length;
-                    for (let e = 0; e < s; e++) {
+                    } = e, l = a.cells.length;
+                    for (let e = 0; e < l; e++) {
                         const u = a.cells.get(e);
-                        if (window.update_loading_text(e + 1, s, null), "code" !== u.type) continue;
-                        const c = new l.OutputAreaModel({
+                        if (window.update_loading_text(e + 1, l, null), "code" !== u.type) continue;
+                        const c = new s.OutputAreaModel({
                             trusted: !0
                         });
                         let d;
-                        d = "true" === i.PageConfig.getOption("include_output_prompt") ? new l.OutputArea({
+                        d = "true" === i.PageConfig.getOption("include_output_prompt") ? new s.OutputArea({
                             model: c,
                             rendermime: o
-                        }) : new l.SimplifiedOutputArea({
+                        }) : new s.SimplifiedOutputArea({
                             model: c,
                             rendermime: o
                         }), d.future = r.requestExecute({
                             code: u.value.text
                         }), await d.future.done;
-                        const p = document.querySelector(`[cell-index="${e+1}"]`);
-                        if (p && i.PageConfig.getOption("include_output") && d.node.childNodes.length > 0) {
-                            null === (t = p.lastElementChild) || void 0 === t || t.classList.remove("jp-mod-noOutputs", "jp-mod-noInput");
+                        const g = document.querySelector(`[cell-index="${e+1}"]`);
+                        if (g && i.PageConfig.getOption("include_output") && d.node.childNodes.length > 0) {
+                            null === (t = g.lastElementChild) || void 0 === t || t.classList.remove("jp-mod-noOutputs", "jp-mod-noInput");
                             const e = document.createElement("div");
                             e.classList.add("jp-Cell-outputWrapper");
                             const i = document.createElement("div");
-                            i.classList.add("jp-Collapser", "jp-OutputCollapser", "jp-Cell-outputCollapser"), e.appendChild(i), null === (n = p.lastElementChild) || void 0 === n || n.appendChild(e), d.node.classList.add("jp-Cell-outputArea"), d.node.style.display = "flex", d.node.style.flexDirection = "column", g.Widget.attach(d, e)
+                            i.classList.add("jp-Collapser", "jp-OutputCollapser", "jp-Cell-outputCollapser"), e.appendChild(i), null === (n = g.lastElementChild) || void 0 === n || n.appendChild(e), d.node.classList.add("jp-Cell-outputArea"), d.node.style.display = "flex", d.node.style.flexDirection = "column", p.Widget.attach(d, e)
                         }
                     }
                     window.display_cells(), window.dispatchEvent(new Event("resize"))
                 }
             }(b || (b = {}));
-            var w = n(67651),
+            var f = n(67651),
                 y = n(37782);
-            const v = {
-                    id: "@voila-dashboards/voici:widget-manager",
-                    autoStart: !0,
-                    provides: w.IJupyterWidgetRegistry,
-                    activate: async e => {
-                        if (!(e instanceof h)) throw Error("The Voici Widget Manager plugin must be activated in a VoilaApp");
-                        const t = e.widgetManagerPromise;
-                        return {
-                            registerWidget: async e => {
-                                (await t.promise).register(e)
-                            }
-                        }
-                    }
-                },
-                j = {
-                    id: "@voila-dashboards/voici:theme-manager",
-                    autoStart: !0,
-                    optional: [y.IThemeManager],
-                    activate: (e, t) => {
-                        if (!t) return;
-                        const n = window.location.search,
-                            a = new URLSearchParams(n).get("theme"),
-                            o = i.PageConfig.getOption("jpThemeName");
-                        let r = a ? decodeURIComponent(a) : o;
-                        r = r || "light", "dark" !== r && "JupyterLab Dark" !== r || (r = "JupyterLab Dark"), "light" !== r && "JupyterLab Light" !== r || (r = "JupyterLab Light"), t.themeChanged.connect((() => {
-                            t.theme !== r && t.setTheme(r)
-                        }))
-                    }
-                },
-                P = [r.pathsPlugin, r.translatorPlugin, v, j];
-            async function C(e, t) {
+            f.IJupyterWidgetRegistry;
+            const w = {
+                id: "@voila-dashboards/voici:theme-manager",
+                autoStart: !0,
+                optional: [y.IThemeManager],
+                activate: (e, t) => {
+                    if (!t) return;
+                    const n = window.location.search,
+                        a = new URLSearchParams(n).get("theme"),
+                        o = i.PageConfig.getOption("jpThemeName");
+                    let r = a ? decodeURIComponent(a) : o;
+                    r = r || "light", "dark" !== r && "JupyterLab Dark" !== r || (r = "JupyterLab Dark"), "light" !== r && "JupyterLab Light" !== r || (r = "JupyterLab Light"), t.themeChanged.connect((() => {
+                        t.theme !== r && t.setTheme(r)
+                    }))
+                }
+            };
+            async function v(e, t) {
                 try {
                     return (await window._JUPYTERLAB[e].get(t))()
                 } catch (n) {
                     throw console.warn(`Failed to create module: package: ${e}; module: ${t}`), n
                 }
             }
 
-            function* k(e, t) {
+            function* P(e, t) {
                 let n;
                 n = Object.prototype.hasOwnProperty.call(e, "__esModule") ? e.default : e;
                 const a = Array.isArray(n) ? n : [n];
                 for (const e of a) i.PageConfig.Extension.isDisabled(e.id) || t.includes(e.id) || t.includes(e.id.split(":")[0]) || (yield e)
             }
-            const O = [n.e(7531).then(n.t.bind(n, 7531, 23))],
-                x = ["@jupyter-widgets/jupyterlab-manager:plugin", "@jupyter-widgets/jupyterlab-manager:saveWidgetState"];
+            o.pathsPlugin, o.translatorPlugin;
+            const j = [n.e(7531).then(n.t.bind(n, 7531, 23))],
+                C = ["@jupyter-widgets/jupyterlab-manager:plugin", "@jupyter-widgets/jupyterlab-manager:saveWidgetState"];
             window.addEventListener("load", (async function() {
-                const e = [n(9961).default.filter((e => ["@jupyterlab/apputils-extension:settings", "@jupyterlab/apputils-extension:themes"].includes(e.id))), n(4319), n(24132), n(41412), n(99661), n(59601), P],
-                    t = [n(84632), n(70851)],
-                    s = JSON.parse(i.PageConfig.getOption("federated_extensions")),
+                const e = [n(9961).default.filter((e => ["@jupyterlab/apputils-extension:settings", "@jupyterlab/apputils-extension:themes"].includes(e.id))), n(99661), n(59601), o.translatorPlugin, o.pathsPlugin, w],
+                    t = [],
+                    r = JSON.parse(i.PageConfig.getOption("federated_extensions")),
+                    s = [],
                     l = [],
                     u = [],
-                    c = [],
-                    d = [],
-                    p = await Promise.allSettled(s.map((async e => (await async function(e, t) {
+                    c = await Promise.allSettled(r.map((async e => (await async function(e, t) {
                         await
                         function(e) {
                             return new Promise(((t, n) => {
                                 const i = document.createElement("script");
                                 i.onerror = n, i.onload = t, i.async = !0, document.head.appendChild(i), i.src = e
                             }))
                         }(e), await n.I("default");
                         const i = window._JUPYTERLAB[t];
                         await i.init(n.S.default)
                     }(`${i.URLExt.join(i.PageConfig.getOption("fullLabextensionsUrl"),e.name,e.load)}`, e.name), e))));
-                Object.entries(p).forEach((([e, t]) => {
+                Object.entries(c).forEach((([e, t]) => {
                     if ("rejected" === t.status) return void console.error(t.reason);
                     const n = t.value;
-                    n.liteExtension ? d.push(C(n.name, n.extension)) : (n.extension && l.push(C(n.name, n.extension)), n.mimeExtension && u.push(C(n.name, n.mimeExtension)), n.style && c.push(C(n.name, n.style)))
-                })), (await Promise.allSettled(l)).forEach((t => {
+                    n.extension && s.push(v(n.name, n.extension)), n.mimeExtension && l.push(v(n.name, n.mimeExtension)), n.style && u.push(v(n.name, n.style))
+                })), (await Promise.allSettled(s)).forEach((t => {
                     if ("fulfilled" === t.status)
-                        for (const n of k(t.value, x)) e.push(n);
+                        for (const n of P(t.value, C)) e.push(n);
                     else console.error(t.reason)
-                })), (await Promise.allSettled(u)).forEach((e => {
+                })), (await Promise.allSettled(l)).forEach((e => {
                     if ("fulfilled" === e.status)
-                        for (const n of k(e.value, x)) t.push(n);
+                        for (const n of P(e.value, C)) t.push(n);
                     else console.error(e.reason)
-                })), (await Promise.allSettled(c)).filter((({
+                })), (await Promise.allSettled(u)).filter((({
                     status: e
                 }) => "rejected" === e)).forEach((e => {
                     console.error(e.reason)
                 }));
-                const g = [];
-                (await Promise.all(O)).forEach((e => {
-                    for (const t of k(e, x)) g.push(t)
-                })), (await Promise.allSettled(d)).forEach((e => {
-                    if ("fulfilled" === e.status)
-                        for (const t of k(e.value, x)) g.push(t);
-                    else console.error(e.reason)
+                const d = [];
+                (await Promise.all(j)).forEach((e => {
+                    for (const t of P(e, C)) d.push(t)
                 }));
-                const m = new a.JupyterLiteServer({
+                const p = new a.JupyterLiteServer({
                     shell: null
                 });
-                m.registerPluginModules(g), await m.start();
-                const f = await m.resolveRequiredService(o.IKernelSpecs),
-                    b = m.serviceManager,
-                    w = new h({
-                        serviceManager: b,
-                        kernelspecs: f,
-                        mimeExtensions: t,
-                        shell: new r.VoilaShell
+                p.registerPluginModules(d), await p.start();
+                const g = p.serviceManager,
+                    m = new h({
+                        serviceManager: g,
+                        shell: new o.VoilaShell
                     });
-                w.registerPluginModules(e), await w.start(), await w.renderWidgets(), window.jupyterapp = w
+                m.registerPluginModules(e), m.started.then((() => {
+                    const e = document.getElementById("voila-tree-main");
+                    e && (e.style.display = "unset")
+                })), m.start()
             }))
         }
     }
 ]);
```

### Comparing `voici-0.4.3/voici/static/build/5826.js` & `voici-0.4.4/voici/static/build/5826.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/5950.js` & `voici-0.4.4/voici/static/build/5950.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/5952.js` & `voici-0.4.4/voici/static/build/5952.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/596.js` & `voici-0.4.4/voici/static/build/596.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/5985.js` & `voici-0.4.4/voici/static/build/5985.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/6111.js` & `voici-0.4.4/voici/static/build/6111.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/6178.js` & `voici-0.4.4/voici/static/build/6178.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/6196.js` & `voici-0.4.4/voici/static/build/6196.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/6219.js` & `voici-0.4.4/voici/static/build/6219.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,14 +1,14 @@
 /*! For license information please see 6219.js.LICENSE.txt */
 "use strict";
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
     [6219], {
         76219: (t, e, n) => {
-            n.d(e, {
-                M: () => p
+            n.r(e), n.d(e, {
+                Application: () => d
             });
             var r, i = n(1514),
                 o = n(92233),
                 a = n(42051);
 
             function u(t, e, n, r) {
                 return new(n || (n = Promise))((function(i, o) {
@@ -362,17 +362,17 @@
                         o < u && r.push(t.slice(o, u)), u < s + 1 && r.push(n(t.slice(u, s + 1))), o = s + 1
                     }
                     return o < t.length && r.push(t.slice(o)), r
                 }, t.cmp = function(t, e) {
                     return t < e ? -1 : t > e ? 1 : 0
                 }
             }(f || (f = {}));
-            var d, p = function() {
+            var p, d = function() {
                 function t(t) {
-                    this._started = !1, this._pluginMap = d.createPluginMap(), this._serviceMap = d.createServiceMap(), this._delegate = new o.PromiseDelegate, this.commands = new i.CommandRegistry, this.contextMenu = new a.ContextMenu({
+                    this._started = !1, this._pluginMap = p.createPluginMap(), this._serviceMap = p.createServiceMap(), this._delegate = new o.PromiseDelegate, this.commands = new i.CommandRegistry, this.contextMenu = new a.ContextMenu({
                         commands: this.commands,
                         renderer: t.contextMenuRenderer
                     }), this.shell = t.shell
                 }
                 return Object.defineProperty(t.prototype, "started", {
                     get: function() {
                         return this._delegate.promise
@@ -387,16 +387,16 @@
                 }, t.prototype.isPluginActivated = function(t) {
                     var e = this._pluginMap[t];
                     return !!e && e.activated
                 }, t.prototype.listPlugins = function() {
                     return Object.keys(this._pluginMap)
                 }, t.prototype.registerPlugin = function(t) {
                     if (t.id in this._pluginMap) throw new Error("Plugin '" + t.id + "' is already registered.");
-                    var e = d.createPluginData(t);
-                    d.ensureNoCycle(e, this._pluginMap, this._serviceMap), e.provides && this._serviceMap.set(e.provides, e.id), this._pluginMap[e.id] = e
+                    var e = p.createPluginData(t);
+                    p.ensureNoCycle(e, this._pluginMap, this._serviceMap), e.provides && this._serviceMap.set(e.provides, e.id), this._pluginMap[e.id] = e
                 }, t.prototype.registerPlugins = function(t) {
                     for (var e = 0, n = t; e < n.length; e++) {
                         var r = n[e];
                         this.registerPlugin(r)
                     }
                 }, t.prototype.deregisterPlugin = function(t, e) {
                     var n = this._pluginMap[t];
@@ -426,15 +426,15 @@
                         var e, n, r, i, o, a, u, l, v, f, h = this;
                         return s(this, (function(s) {
                             switch (s.label) {
                                 case 0:
                                     if (!(e = this._pluginMap[t])) throw new ReferenceError("Plugin '" + t + "' is not registered.");
                                     if (!e.activated) return [2, []];
                                     if (!e.deactivate) throw new TypeError("Plugin '" + t + "'#deactivate() method missing");
-                                    for (n = d.findDependents(t, this._pluginMap, this._serviceMap), r = n.map((function(t) {
+                                    for (n = p.findDependents(t, this._pluginMap, this._serviceMap), r = n.map((function(t) {
                                             return h._pluginMap[t]
                                         })), i = 0, o = r; i < o.length; i++)
                                         if (!(a = o[i]).deactivate) throw new TypeError("Plugin " + a.id + "#deactivate() method missing (depends on " + t + ")");
                                     u = 0, l = r, s.label = 1;
                                 case 1:
                                     return u < l.length ? (v = l[u], f = c(v.requires, v.optional).map((function(t) {
                                         var e = h._serviceMap.get(t);
@@ -484,15 +484,15 @@
                         }))
                     }))
                 }, t.prototype.start = function(t) {
                     var e = this;
                     if (void 0 === t && (t = {}), this._started) return this._delegate.promise;
                     this._started = !0;
                     var n = t.hostID || "",
-                        r = d.collectStartupPlugins(this._pluginMap, t).map((function(t) {
+                        r = p.collectStartupPlugins(this._pluginMap, t).map((function(t) {
                             return e.activatePlugin(t).catch((function(e) {
                                 console.error("Plugin '" + t + "' failed to activate."), console.error(e)
                             }))
                         }));
                     return Promise.all(r).then((function() {
                         e.attachShell(n), e.addEventListeners(), e._delegate.resolve(void 0)
                     })), this._delegate.promise
@@ -575,15 +575,15 @@
                             }, f = 0, h = a.map((function(t) {
                                 return t[0]
                             })).reduce((function(t, e) {
                                 return -1 == t.indexOf(e) && t.push(e), t
                             }), []); f < h.length; f++) v(h[f]);
                         u = s
                     }
-                    var d = function(t) {
+                    var p = function(t) {
                             var e = [],
                                 n = new Set,
                                 r = new Map;
                             return function(t, e) {
                                 for (var n, i = l(t); void 0 !== (n = i.next());)
                                     if (!1 === (a = void 0, u = void 0, s = void 0, a = (o = n)[0], u = o[1], void((s = r.get(u)) ? s.push(a) : r.set(u, [a])))) return;
                                 var o, a, u, s
@@ -595,26 +595,26 @@
                                 if (!n.has(t)) {
                                     n.add(t);
                                     var o = r.get(t);
                                     o && o.forEach(i), e.push(t)
                                 }
                             }
                         }(a),
-                        p = function(e, n) {
+                        d = function(e, n) {
                             for (var r, i = 0, o = l(e); void 0 !== (r = o.next());)
                                 if (i++, r === t) return i - 1;
                             return -1
-                        }(d);
-                    return -1 === p ? [t] : d.slice(0, p + 1)
+                        }(p);
+                    return -1 === d ? [t] : p.slice(0, d + 1)
                 }, t.collectStartupPlugins = function(t, e) {
                     var n = new Map;
                     for (var r in t) t[r].autoStart && n.set(r, !0);
                     if (e.startPlugins)
                         for (var i = 0, o = e.startPlugins; i < o.length; i++) r = o[i], n.set(r, !0);
                     if (e.ignorePlugins)
                         for (var a = 0, u = e.ignorePlugins; a < u.length; a++) r = u[a], n.delete(r);
                     return Array.from(n.keys())
                 }
-            }(d || (d = {}))
+            }(p || (p = {}))
         }
     }
 ]);
```

### Comparing `voici-0.4.3/voici/static/build/6219.js.LICENSE.txt` & `voici-0.4.4/voici/static/build/6219.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/6527.js` & `voici-0.4.4/voici/static/build/6527.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/6614.js` & `voici-0.4.4/voici/static/build/6614.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/6616.js` & `voici-0.4.4/voici/static/build/6616.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/6757.js` & `voici-0.4.4/voici/static/build/6757.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/6770.js` & `voici-0.4.4/voici/static/build/6770.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/6790.js` & `voici-0.4.4/voici/static/build/6790.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/6839.js` & `voici-0.4.4/voici/static/build/6839.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/6852.js` & `voici-0.4.4/voici/static/build/7002.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,13 @@
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
-    [6852], {
+    [7002], {
         27693: e => {
             e.exports = {
                 name: "@voila-dashboards/voici",
-                version: "0.4.3",
+                version: "0.4.4",
                 description: "The Voici Frontend",
                 author: "Voilà contributors",
                 license: "BSD-3-Clause",
                 main: "lib/index.js",
                 browserslist: ">0.8%, not ie 11, not op_mini all, not dead",
                 dependencies: {
                     "@jupyter-widgets/base": "^6.0.1",
@@ -38,20 +38,24 @@
                     "@jupyterlab/ui-components": "^3.0.0",
                     "@jupyterlite/contents": "^0.1.0",
                     "@jupyterlite/iframe-extension": "^0.1.0",
                     "@jupyterlite/kernel": "^0.1.0",
                     "@jupyterlite/server": "^0.1.0",
                     "@jupyterlite/server-extension": "^0.1.0",
                     "@lumino/algorithm": "^1.6.2",
+                    "@lumino/application": "^1.31.3",
                     "@lumino/commands": "^1.15.2",
                     "@lumino/coreutils": "^1.8.2",
+                    "@lumino/datagrid": "^0.36.0",
                     "@lumino/disposable": "^1.7.2",
                     "@lumino/domutils": "^1.5.2",
                     "@lumino/dragdrop": "^1.10.2",
+                    "@lumino/keyboard": "^1.8.0",
                     "@lumino/messaging": "^1.7.2",
+                    "@lumino/polling": "^1.11.4",
                     "@lumino/properties": "^1.5.2",
                     "@lumino/signaling": "^1.7.2",
                     "@lumino/virtualdom": "^1.11.2",
                     "@lumino/widgets": "^1.26.2",
                     "@voila-dashboards/voila": "^0.5.0-alpha.3",
                     react: "^17.0.1",
                     "react-dom": "^17.0.1"
@@ -93,66 +97,67 @@
                     watch: 'tsc-watch --onSuccess "webpack --mode=development"'
                 },
                 publishConfig: {
                     access: "public"
                 }
             }
         },
-        46852: (e, t, n) => {
+        47002: (e, t, n) => {
             "use strict";
-            n.r(t);
-            var i = n(59110),
-                a = n(94456),
-                o = n(22312),
-                r = n(75238),
-                s = n(73198),
-                l = n(40049),
-                u = n(12299),
-                c = n(35918),
-                d = n(92233),
-                p = n(42051);
-            const g = n(27693),
-                m = "application/vnd.jupyter.widget-view+json";
-            class h extends r.JupyterFrontEnd {
+            n.r(t), n(23203), n(8971);
+            var i = n(92233),
+                a = (n(7573), n(36e3), n(94812), n(3860), n(26968), n(78695), n(48157), n(24629), n(4947), n(32886), n(42051)),
+                o = (n(24627), n(59110)),
+                r = n(7631),
+                s = n(94456),
+                l = n(22312),
+                u = n(75238),
+                c = n(73198),
+                d = n(40049),
+                p = n(12299),
+                g = n(35918);
+            const m = n(27693),
+                f = "application/vnd.jupyter.widget-view+json";
+            class h extends u.JupyterFrontEnd {
                 constructor(e) {
                     var t;
                     if (super(Object.assign(Object.assign({}, e), {
-                            shell: null !== (t = e.shell) && void 0 !== t ? t : new o.VoilaShell
-                        })), this.name = "Voici", this.namespace = this.name, this.version = g.version, this._widgetManagerPromise = new d.PromiseDelegate, e.mimeExtensions)
-                        for (const t of (0, r.createRendermimePlugins)(e.mimeExtensions)) this.registerPlugin(t);
+                            shell: null !== (t = e.shell) && void 0 !== t ? t : new l.VoilaShell
+                        })), this.name = "Voici", this.namespace = this.name, this.version = m.version, this._widgetManagerPromise = new i.PromiseDelegate, e.mimeExtensions)
+                        for (const t of (0, u.createRendermimePlugins)(e.mimeExtensions)) this.registerPlugin(t);
                     this._kernelspecs = e.kernelspecs, this._serviceManager = e.serviceManager
                 }
                 get widgetManagerPromise() {
                     return this._widgetManagerPromise
                 }
                 get paths() {
                     return {
                         urls: {
-                            base: i.PageConfig.getOption("baseUrl"),
-                            notFound: i.PageConfig.getOption("notFoundUrl"),
-                            app: i.PageConfig.getOption("appUrl"),
-                            static: i.PageConfig.getOption("staticUrl"),
-                            settings: i.PageConfig.getOption("settingsUrl"),
-                            themes: i.PageConfig.getOption("themesUrl"),
-                            doc: i.PageConfig.getOption("docUrl"),
-                            translations: i.PageConfig.getOption("translationsApiUrl"),
-                            hubHost: i.PageConfig.getOption("hubHost") || void 0,
-                            hubPrefix: i.PageConfig.getOption("hubPrefix") || void 0,
-                            hubUser: i.PageConfig.getOption("hubUser") || void 0,
-                            hubServerName: i.PageConfig.getOption("hubServerName") || void 0
+                            base: o.PageConfig.getOption("baseUrl"),
+                            notFound: o.PageConfig.getOption("notFoundUrl"),
+                            app: o.PageConfig.getOption("appUrl"),
+                            static: o.PageConfig.getOption("staticUrl"),
+                            settings: o.PageConfig.getOption("settingsUrl"),
+                            themes: o.PageConfig.getOption("themesUrl"),
+                            doc: o.PageConfig.getOption("docUrl"),
+                            translations: o.PageConfig.getOption("translationsApiUrl"),
+                            hubHost: o.PageConfig.getOption("hubHost") || void 0,
+                            hubPrefix: o.PageConfig.getOption("hubPrefix") || void 0,
+                            hubUser: o.PageConfig.getOption("hubUser") || void 0,
+                            hubServerName: o.PageConfig.getOption("hubServerName") || void 0
                         },
                         directories: {
-                            appSettings: i.PageConfig.getOption("appSettingsDir"),
-                            schemas: i.PageConfig.getOption("schemasDir"),
-                            static: i.PageConfig.getOption("staticDir"),
-                            templates: i.PageConfig.getOption("templatesDir"),
-                            themes: i.PageConfig.getOption("themesDir"),
-                            userSettings: i.PageConfig.getOption("userSettingsDir"),
-                            serverRoot: i.PageConfig.getOption("serverRoot"),
-                            workspaces: i.PageConfig.getOption("workspacesDir")
+                            appSettings: o.PageConfig.getOption("appSettingsDir"),
+                            schemas: o.PageConfig.getOption("schemasDir"),
+                            static: o.PageConfig.getOption("staticDir"),
+                            templates: o.PageConfig.getOption("templatesDir"),
+                            themes: o.PageConfig.getOption("themesDir"),
+                            userSettings: o.PageConfig.getOption("userSettingsDir"),
+                            serverRoot: o.PageConfig.getOption("serverRoot"),
+                            workspaces: o.PageConfig.getOption("workspacesDir")
                         }
                     }
                 }
                 registerPluginModule(e) {
                     let t = e.default;
                     Object.prototype.hasOwnProperty.call(e, "__esModule") || (t = e), Array.isArray(t) || (t = [t]), t.forEach((e => {
                         try {
@@ -165,188 +170,206 @@
                 registerPluginModules(e) {
                     e.forEach((e => {
                         this.registerPluginModule(e)
                     }))
                 }
                 async renderWidgets() {
                     var e, t, n;
-                    const a = this._serviceManager;
-                    if (!a) return void console.error("Missing service manager");
+                    const i = this._serviceManager;
+                    if (!i) return void console.error("Missing service manager");
+                    await i.ready;
+                    const a = i.sessions;
                     await a.ready;
-                    const o = a.sessions;
-                    await o.ready;
-                    const r = new l.NotebookModel;
-                    r.fromString(i.PageConfig.getOption("notebookSrc"));
+                    const r = new d.NotebookModel;
+                    r.fromString(o.PageConfig.getOption("notebookSrc"));
                     let s = r.metadata.get("kernelspec");
                     s || (s = {
                         name: "python"
                     });
-                    const d = null === (t = null === (e = this._kernelspecs) || void 0 === e ? void 0 : e.specs) || void 0 === t ? void 0 : t.kernelspecs;
-                    let p;
-                    if (!d) return void console.error("No kernel available");
-                    if (s.name in d) console.log(`${s.name} kernel is available!`), p = d[s.name];
+                    const l = null === (t = null === (e = this._kernelspecs) || void 0 === e ? void 0 : e.specs) || void 0 === t ? void 0 : t.kernelspecs;
+                    let u;
+                    if (!l) return void console.error("No kernel available");
+                    if (s.name in l) console.log(`${s.name} kernel is available!`), u = l[s.name];
                     else
-                        for (const e in d)
-                            if (s.language === (null === (n = d[e]) || void 0 === n ? void 0 : n.language)) {
-                                console.log(`${s.name} kernel is not available, fallback to using ${d[e].name}`), p = d[e];
+                        for (const e in l)
+                            if (s.language === (null === (n = l[e]) || void 0 === n ? void 0 : n.language)) {
+                                console.log(`${s.name} kernel is not available, fallback to using ${l[e].name}`), u = l[e];
                                 break
-                            } if (!p) return void console.error(`No kernel available for ${s.language}`);
-                    const g = await o.startNew({
+                            } if (!u) return void console.error(`No kernel available for ${s.language}`);
+                    const c = await a.startNew({
                             name: "",
                             path: "",
                             type: "notebook",
-                            kernel: p
+                            kernel: u
                         }),
-                        h = g.kernel;
-                    h ? h.connectionStatusChanged.connect((async (e, t) => {
+                        m = c.kernel;
+                    m ? m.connectionStatusChanged.connect((async (e, t) => {
                         if ("connected" === t) {
                             window.update_loading_text(0, 0, "Starting up kernel...");
-                            const e = new u.RenderMimeRegistry({
-                                    initialFactories: u.standardRendererFactories
+                            const e = new p.RenderMimeRegistry({
+                                    initialFactories: p.standardRendererFactories
                                 }),
-                                t = new c.KernelWidgetManager(h, e);
-                            if (e.removeMimeType(m), e.addFactory({
+                                t = new g.KernelWidgetManager(m, e);
+                            if (e.removeMimeType(f), e.addFactory({
                                     safe: !1,
-                                    mimeTypes: [m],
-                                    createRenderer: e => new c.WidgetRenderer(e, t)
-                                }, -10), this._widgetManagerPromise.resolve(t), !g.kernel) return;
+                                    mimeTypes: [f],
+                                    createRenderer: e => new g.WidgetRenderer(e, t)
+                                }, -10), this._widgetManagerPromise.resolve(t), !c.kernel) return;
                             await new Promise((e => setTimeout(e, 500)));
                             let n = !1;
-                            h.statusChanged.connect((async (t, i) => {
-                                n || "idle" !== i || (n = !0, await f.executeCells({
+                            m.statusChanged.connect((async (t, i) => {
+                                n || "idle" !== i || (n = !0, await b.executeCells({
                                     source: r,
                                     rendermime: e,
-                                    kernel: g.kernel
+                                    kernel: c.kernel
                                 }))
                             }))
                         }
                     })) : console.error("Can not start kernel")
                 }
             }
-            var f;
+            var b;
             ! function(e) {
                 e.executeCells = async function(e) {
                     var t, n;
                     const {
-                        source: a,
-                        rendermime: o,
-                        kernel: r
-                    } = e, l = a.cells.length;
+                        source: i,
+                        rendermime: r,
+                        kernel: s
+                    } = e, l = i.cells.length;
                     for (let e = 0; e < l; e++) {
-                        const u = a.cells.get(e);
+                        const u = i.cells.get(e);
                         if (window.update_loading_text(e + 1, l, null), "code" !== u.type) continue;
-                        const c = new s.OutputAreaModel({
+                        const d = new c.OutputAreaModel({
                             trusted: !0
                         });
-                        let d;
-                        d = "true" === i.PageConfig.getOption("include_output_prompt") ? new s.OutputArea({
-                            model: c,
-                            rendermime: o
-                        }) : new s.SimplifiedOutputArea({
-                            model: c,
-                            rendermime: o
-                        }), d.future = r.requestExecute({
+                        let p;
+                        p = "true" === o.PageConfig.getOption("include_output_prompt") ? new c.OutputArea({
+                            model: d,
+                            rendermime: r
+                        }) : new c.SimplifiedOutputArea({
+                            model: d,
+                            rendermime: r
+                        }), p.future = s.requestExecute({
                             code: u.value.text
-                        }), await d.future.done;
+                        }), await p.future.done;
                         const g = document.querySelector(`[cell-index="${e+1}"]`);
-                        if (g && i.PageConfig.getOption("include_output") && d.node.childNodes.length > 0) {
+                        if (g && o.PageConfig.getOption("include_output") && p.node.childNodes.length > 0) {
                             null === (t = g.lastElementChild) || void 0 === t || t.classList.remove("jp-mod-noOutputs", "jp-mod-noInput");
                             const e = document.createElement("div");
                             e.classList.add("jp-Cell-outputWrapper");
                             const i = document.createElement("div");
-                            i.classList.add("jp-Collapser", "jp-OutputCollapser", "jp-Cell-outputCollapser"), e.appendChild(i), null === (n = g.lastElementChild) || void 0 === n || n.appendChild(e), d.node.classList.add("jp-Cell-outputArea"), d.node.style.display = "flex", d.node.style.flexDirection = "column", p.Widget.attach(d, e)
+                            i.classList.add("jp-Collapser", "jp-OutputCollapser", "jp-Cell-outputCollapser"), e.appendChild(i), null === (n = g.lastElementChild) || void 0 === n || n.appendChild(e), p.node.classList.add("jp-Cell-outputArea"), p.node.style.display = "flex", p.node.style.flexDirection = "column", a.Widget.attach(p, e)
                         }
                     }
                     window.display_cells(), window.dispatchEvent(new Event("resize"))
                 }
-            }(f || (f = {}));
-            var b = n(67651),
+            }(b || (b = {}));
+            var w = n(67651),
                 y = n(37782);
-            b.IJupyterWidgetRegistry;
-            const w = {
-                id: "@voila-dashboards/voici:theme-manager",
-                autoStart: !0,
-                optional: [y.IThemeManager],
-                activate: (e, t) => {
-                    if (!t) return;
-                    const n = window.location.search,
-                        a = new URLSearchParams(n).get("theme"),
-                        o = i.PageConfig.getOption("jpThemeName");
-                    let r = a ? decodeURIComponent(a) : o;
-                    r = r || "light", "dark" !== r && "JupyterLab Dark" !== r || (r = "JupyterLab Dark"), "light" !== r && "JupyterLab Light" !== r || (r = "JupyterLab Light"), t.themeChanged.connect((() => {
-                        t.theme !== r && t.setTheme(r)
-                    }))
-                }
-            };
-            async function v(e, t) {
+            const v = {
+                    id: "@voila-dashboards/voici:widget-manager",
+                    autoStart: !0,
+                    provides: w.IJupyterWidgetRegistry,
+                    activate: async e => {
+                        if (!(e instanceof h)) throw Error("The Voici Widget Manager plugin must be activated in a VoilaApp");
+                        const t = e.widgetManagerPromise;
+                        return {
+                            registerWidget: async e => {
+                                (await t.promise).register(e)
+                            }
+                        }
+                    }
+                },
+                j = {
+                    id: "@voila-dashboards/voici:theme-manager",
+                    autoStart: !0,
+                    optional: [y.IThemeManager],
+                    activate: (e, t) => {
+                        if (!t) return;
+                        const n = window.location.search,
+                            i = new URLSearchParams(n).get("theme"),
+                            a = o.PageConfig.getOption("jpThemeName");
+                        let r = i ? decodeURIComponent(i) : a;
+                        r = r || "light", "dark" !== r && "JupyterLab Dark" !== r || (r = "JupyterLab Dark"), "light" !== r && "JupyterLab Light" !== r || (r = "JupyterLab Light"), t.themeChanged.connect((() => {
+                            t.theme !== r && t.setTheme(r)
+                        }))
+                    }
+                },
+                P = [l.pathsPlugin, l.translatorPlugin, v, j];
+            async function C(e, t) {
                 try {
                     return (await window._JUPYTERLAB[e].get(t))()
                 } catch (n) {
                     throw console.warn(`Failed to create module: package: ${e}; module: ${t}`), n
                 }
             }
 
-            function* P(e, t) {
+            function* k(e, t) {
                 let n;
                 n = Object.prototype.hasOwnProperty.call(e, "__esModule") ? e.default : e;
-                const a = Array.isArray(n) ? n : [n];
-                for (const e of a) i.PageConfig.Extension.isDisabled(e.id) || t.includes(e.id) || t.includes(e.id.split(":")[0]) || (yield e)
+                const i = Array.isArray(n) ? n : [n];
+                for (const e of i) o.PageConfig.Extension.isDisabled(e.id) || t.includes(e.id) || t.includes(e.id.split(":")[0]) || (yield e)
             }
-            o.pathsPlugin, o.translatorPlugin;
-            const j = [n.e(7531).then(n.t.bind(n, 7531, 23))],
-                C = ["@jupyter-widgets/jupyterlab-manager:plugin", "@jupyter-widgets/jupyterlab-manager:saveWidgetState"];
+            const O = [n.e(7531).then(n.t.bind(n, 7531, 23))],
+                x = ["@jupyter-widgets/jupyterlab-manager:plugin", "@jupyter-widgets/jupyterlab-manager:saveWidgetState"];
             window.addEventListener("load", (async function() {
-                const e = [n(9961).default.filter((e => ["@jupyterlab/apputils-extension:settings", "@jupyterlab/apputils-extension:themes"].includes(e.id))), n(99661), n(59601), o.translatorPlugin, o.pathsPlugin, w],
-                    t = [],
-                    r = JSON.parse(i.PageConfig.getOption("federated_extensions")),
-                    s = [],
-                    l = [],
+                const e = [n(9961).default.filter((e => ["@jupyterlab/apputils-extension:settings", "@jupyterlab/apputils-extension:themes"].includes(e.id))), n(4319), n(24132), n(41412), n(99661), n(59601), P],
+                    t = [n(84632), n(70851)],
+                    i = JSON.parse(o.PageConfig.getOption("federated_extensions")),
+                    a = [],
                     u = [],
-                    c = await Promise.allSettled(r.map((async e => (await async function(e, t) {
+                    c = [],
+                    d = [],
+                    p = await Promise.allSettled(i.map((async e => (await async function(e, t) {
                         await
                         function(e) {
                             return new Promise(((t, n) => {
                                 const i = document.createElement("script");
                                 i.onerror = n, i.onload = t, i.async = !0, document.head.appendChild(i), i.src = e
                             }))
                         }(e), await n.I("default");
                         const i = window._JUPYTERLAB[t];
                         await i.init(n.S.default)
-                    }(`${i.URLExt.join(i.PageConfig.getOption("fullLabextensionsUrl"),e.name,e.load)}`, e.name), e))));
-                Object.entries(c).forEach((([e, t]) => {
+                    }(`${o.URLExt.join(o.PageConfig.getOption("fullLabextensionsUrl"),e.name,e.load)}`, e.name), e))));
+                Object.entries(p).forEach((([e, t]) => {
                     if ("rejected" === t.status) return void console.error(t.reason);
                     const n = t.value;
-                    n.extension && s.push(v(n.name, n.extension)), n.mimeExtension && l.push(v(n.name, n.mimeExtension)), n.style && u.push(v(n.name, n.style))
-                })), (await Promise.allSettled(s)).forEach((t => {
+                    n.liteExtension ? d.push(C(n.name, n.extension)) : (n.extension && a.push(C(n.name, n.extension)), n.mimeExtension && u.push(C(n.name, n.mimeExtension)), n.style && c.push(C(n.name, n.style)))
+                })), (await Promise.allSettled(a)).forEach((t => {
                     if ("fulfilled" === t.status)
-                        for (const n of P(t.value, C)) e.push(n);
+                        for (const n of k(t.value, x)) e.push(n);
                     else console.error(t.reason)
-                })), (await Promise.allSettled(l)).forEach((e => {
+                })), (await Promise.allSettled(u)).forEach((e => {
                     if ("fulfilled" === e.status)
-                        for (const n of P(e.value, C)) t.push(n);
+                        for (const n of k(e.value, x)) t.push(n);
                     else console.error(e.reason)
-                })), (await Promise.allSettled(u)).filter((({
+                })), (await Promise.allSettled(c)).filter((({
                     status: e
                 }) => "rejected" === e)).forEach((e => {
                     console.error(e.reason)
                 }));
-                const d = [];
-                (await Promise.all(j)).forEach((e => {
-                    for (const t of P(e, C)) d.push(t)
+                const g = [];
+                (await Promise.all(O)).forEach((e => {
+                    for (const t of k(e, x)) g.push(t)
+                })), (await Promise.allSettled(d)).forEach((e => {
+                    if ("fulfilled" === e.status)
+                        for (const t of k(e.value, x)) g.push(t);
+                    else console.error(e.reason)
                 }));
-                const p = new a.JupyterLiteServer({
+                const m = new s.JupyterLiteServer({
                     shell: null
                 });
-                p.registerPluginModules(d), await p.start();
-                const g = p.serviceManager,
-                    m = new h({
-                        serviceManager: g,
-                        shell: new o.VoilaShell
+                m.registerPluginModules(g), await m.start();
+                const f = await m.resolveRequiredService(r.IKernelSpecs),
+                    b = m.serviceManager,
+                    w = new h({
+                        serviceManager: b,
+                        kernelspecs: f,
+                        mimeExtensions: t,
+                        shell: new l.VoilaShell
                     });
-                m.registerPluginModules(e), m.started.then((() => {
-                    const e = document.getElementById("voila-tree-main");
-                    e && (e.style.display = "unset")
-                })), m.start()
+                w.registerPluginModules(e), await w.start(), await w.renderWidgets(), window.jupyterapp = w
             }))
         }
     }
 ]);
```

### Comparing `voici-0.4.3/voici/static/build/6856.js` & `voici-0.4.4/voici/static/build/6856.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,20 +1,20 @@
 "use strict";
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
     [6856, 3256], {
         93256: (e, t, r) => {
             r.r(t), r.d(t, {
-                IServiceWorkerManager: () => l,
+                IServiceWorkerManager: () => h,
                 JupyterLiteServer: () => a,
                 Router: () => o,
-                ServiceWorkerManager: () => _,
+                ServiceWorkerManager: () => p,
                 WORKER_NAME: () => u
             });
             var i = r(2132),
-                s = r(76219),
+                s = r(8971),
                 n = r(79988);
             class o {
                 constructor() {
                     this._routes = []
                 }
                 get(e, t) {
                     this._add("GET", e, t)
@@ -62,15 +62,15 @@
                     "string" == typeof t && (t = new RegExp(t)), this._routes.push({
                         method: e,
                         pattern: t,
                         callback: r
                     })
                 }
             }
-            class a extends s.M {
+            class a extends s.Application {
                 constructor(e) {
                     var t;
                     super(e), this.name = "JupyterLite Server", this.namespace = this.name, this.version = "unknown", this._router = new o, this._serviceManager = new i.ServiceManager({
                         standby: "never",
                         serverSettings: {
                             ...i.ServerConnection.makeSettings(),
                             WebSocket: n.WebSocket,
@@ -103,20 +103,20 @@
                 registerPluginModules(e) {
                     e.forEach((e => {
                         this.registerPluginModule(e)
                     }))
                 }
             }
             var c = r(92233);
-            const h = r.p + "service-worker-b2fb40a.js",
-                l = new c.Token("@jupyterlite/server-extension:IServiceWorkerManager"),
-                u = `${h}`.split("/").slice(-1)[0];
+            const l = r.p + "service-worker-b2fb40a.js",
+                h = new c.Token("@jupyterlite/server-extension:IServiceWorkerManager"),
+                u = `${l}`.split("/").slice(-1)[0];
             var g = r(4947),
                 d = r(86086);
-            class _ {
+            class p {
                 constructor() {
                     this._registration = null, this._registrationChanged = new g.Signal(this), this._ready = new c.PromiseDelegate, this.initialize().catch(console.warn)
                 }
                 get registrationChanged() {
                     return this._registrationChanged
                 }
                 get enabled() {
```

### Comparing `voici-0.4.3/voici/static/build/6914.js` & `voici-0.4.4/voici/static/build/6914.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -568,15 +568,15 @@
                     }
                 };
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.EventManager = void 0;
             const r = s(59110),
                 o = s(92233),
-                a = s(82361),
+                a = s(48157),
                 c = s(4947),
                 l = s(22700),
                 h = "api/events";
             var d;
             t.EventManager = class {
                     constructor(e = {}) {
                         var t;
@@ -1547,15 +1547,15 @@
         },
         72810: (e, t, s) => {
             "use strict";
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.KernelManager = void 0;
             const n = s(23203),
-                i = s(82361),
+                i = s(48157),
                 r = s(4947),
                 o = s(16914),
                 a = s(92918),
                 c = s(60925),
                 l = s(82094);
             class h extends a.BaseManager {
                 constructor(e = {}) {
@@ -1969,15 +1969,15 @@
                         for (var s in e) "default" !== s && Object.prototype.hasOwnProperty.call(e, s) && n(t, e, s);
                     return i(t, e), t
                 };
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.KernelSpecManager = void 0;
             const o = s(92233),
-                a = s(82361),
+                a = s(48157),
                 c = s(4947),
                 l = r(s(47352)),
                 h = s(92918);
             class d extends h.BaseManager {
                 constructor(e = {}) {
                     var t;
                     super(e), this._isReady = !1, this._connectionFailure = new c.Signal(this), this._specs = null, this._specsChanged = new c.Signal(this), this._ready = Promise.all([this.requestSpecs()]).then((e => {})).catch((e => {})).then((() => {
@@ -2464,15 +2464,15 @@
         },
         6699: (e, t, s) => {
             "use strict";
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.SessionManager = void 0;
             const n = s(23203),
-                i = s(82361),
+                i = s(48157),
                 r = s(4947),
                 o = s(22700),
                 a = s(92918),
                 c = s(75575),
                 l = s(28351);
             class h extends a.BaseManager {
                 constructor(e) {
@@ -2901,15 +2901,15 @@
         },
         11703: (e, t, s) => {
             "use strict";
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.TerminalManager = void 0;
             const n = s(23203),
-                i = s(82361),
+                i = s(48157),
                 r = s(4947),
                 o = s(16914),
                 a = s(92918),
                 c = s(64020),
                 l = s(5478);
             class h extends a.BaseManager {
                 constructor(e = {}) {
@@ -3068,15 +3068,15 @@
         67523: (e, t, s) => {
             "use strict";
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.UserManager = void 0;
             const n = s(59110),
                 i = s(92233),
-                r = s(82361),
+                r = s(48157),
                 o = s(4947),
                 a = s(22700),
                 c = s(92918),
                 l = "@jupyterlab/services:UserManager#user";
             class h extends c.BaseManager {
                 constructor(e = {}) {
                     var t;
```

### Comparing `voici-0.4.3/voici/static/build/6976.js` & `voici-0.4.4/voici/static/build/6976.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/7003.js` & `voici-0.4.4/voici/static/build/7003.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/7015.js` & `voici-0.4.4/voici/static/build/7015.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/7066.js` & `voici-0.4.4/voici/static/build/7066.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -11,15 +11,15 @@
                 s = a(59110),
                 i = a(68930),
                 r = a(30846),
                 l = a(56956),
                 c = a(24643),
                 d = a(92233),
                 u = a(36e3),
-                p = a(82361),
+                p = a(48157),
                 m = a(70988);
             const g = "help:open",
                 h = "https://jupyterlab.readthedocs.io/en/3.6.x/privacy_policies.html";
             async function f(e, t = {}) {
                 const a = m.ServerConnection.makeSettings(),
                     n = s.URLExt.join(a.baseUrl, e);
                 let o;
```

### Comparing `voici-0.4.3/voici/static/build/709.js` & `voici-0.4.4/voici/static/build/709.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/74.js` & `voici-0.4.4/voici/static/build/74.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1411,15 +1411,15 @@
         },
         41302: (e, t, s) => {
             "use strict";
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.KernelManager = void 0;
             const n = s(23203),
-                i = s(82361),
+                i = s(48157),
                 r = s(4947),
                 o = s(80074),
                 a = s(87207),
                 c = s(86330),
                 l = s(24270);
             class h extends a.BaseManager {
                 constructor(e = {}) {
@@ -1833,15 +1833,15 @@
                         for (var s in e) "default" !== s && Object.prototype.hasOwnProperty.call(e, s) && n(t, e, s);
                     return i(t, e), t
                 };
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.KernelSpecManager = void 0;
             const o = s(92233),
-                a = s(82361),
+                a = s(48157),
                 c = s(4947),
                 l = r(s(56304)),
                 h = s(87207);
             class d extends h.BaseManager {
                 constructor(e = {}) {
                     var t;
                     super(e), this._isReady = !1, this._connectionFailure = new c.Signal(this), this._specs = null, this._specsChanged = new c.Signal(this), this._ready = Promise.all([this.requestSpecs()]).then((e => {})).catch((e => {})).then((() => {
@@ -2326,15 +2326,15 @@
         },
         66874: (e, t, s) => {
             "use strict";
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.SessionManager = void 0;
             const n = s(23203),
-                i = s(82361),
+                i = s(48157),
                 r = s(4947),
                 o = s(54244),
                 a = s(87207),
                 c = s(76749),
                 l = s(95604);
             class h extends a.BaseManager {
                 constructor(e) {
@@ -2763,15 +2763,15 @@
         },
         26683: (e, t, s) => {
             "use strict";
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.TerminalManager = void 0;
             const n = s(23203),
-                i = s(82361),
+                i = s(48157),
                 r = s(4947),
                 o = s(80074),
                 a = s(87207),
                 c = s(33165),
                 l = s(84420);
             class h extends a.BaseManager {
                 constructor(e = {}) {
```

### Comparing `voici-0.4.3/voici/static/build/7469.js` & `voici-0.4.4/voici/static/build/7469.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/7560.js` & `voici-0.4.4/voici/static/build/7560.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1411,15 +1411,15 @@
         },
         56839: (e, t, s) => {
             "use strict";
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.KernelManager = void 0;
             const n = s(23203),
-                i = s(82361),
+                i = s(48157),
                 r = s(4947),
                 o = s(17560),
                 a = s(99417),
                 c = s(46859),
                 l = s(18371);
             class h extends a.BaseManager {
                 constructor(e = {}) {
@@ -1784,15 +1784,15 @@
                         for (var s in e) "default" !== s && Object.prototype.hasOwnProperty.call(e, s) && n(t, e, s);
                     return i(t, e), t
                 };
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.KernelSpecManager = void 0;
             const o = s(92233),
-                a = s(82361),
+                a = s(48157),
                 c = s(4947),
                 l = r(s(57562)),
                 h = s(99417);
             class d extends h.BaseManager {
                 constructor(e = {}) {
                     var t;
                     super(e), this._isReady = !1, this._connectionFailure = new c.Signal(this), this._specs = null, this._specsChanged = new c.Signal(this), this._ready = Promise.all([this.requestSpecs()]).then((e => {})).catch((e => {})).then((() => {
@@ -2277,15 +2277,15 @@
         },
         36981: (e, t, s) => {
             "use strict";
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.SessionManager = void 0;
             const n = s(23203),
-                i = s(82361),
+                i = s(48157),
                 r = s(4947),
                 o = s(75381),
                 a = s(99417),
                 c = s(26984),
                 l = s(42620);
             class h extends a.BaseManager {
                 constructor(e) {
@@ -2714,15 +2714,15 @@
         },
         43497: (e, t, s) => {
             "use strict";
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.TerminalManager = void 0;
             const n = s(23203),
-                i = s(82361),
+                i = s(48157),
                 r = s(4947),
                 o = s(17560),
                 a = s(99417),
                 c = s(90238),
                 l = s(96636);
             class h extends a.BaseManager {
                 constructor(e = {}) {
```

### Comparing `voici-0.4.3/voici/static/build/7623.js` & `voici-0.4.4/voici/static/build/7623.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/7695.js` & `voici-0.4.4/voici/static/build/7695.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/7795.js` & `voici-0.4.4/voici/static/build/7795.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/8085.js` & `voici-0.4.4/voici/static/build/8085.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/8164.js` & `voici-0.4.4/voici/static/build/8164.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/8291.js` & `voici-0.4.4/voici/static/build/8291.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/8316.js` & `voici-0.4.4/voici/static/build/8316.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/8316.js.LICENSE.txt` & `voici-0.4.4/voici/static/build/8316.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/846.js` & `voici-0.4.4/voici/static/build/846.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/86.js` & `voici-0.4.4/voici/static/build/86.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/8809.js` & `voici-0.4.4/voici/static/build/8809.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/8874.js` & `voici-0.4.4/voici/static/build/8874.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/9060.js` & `voici-0.4.4/voici/static/build/9060.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/9112.js` & `voici-0.4.4/voici/static/build/9112.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -874,15 +874,15 @@
             });
             var r = n(56956),
                 i = n(37782),
                 o = n(42938),
                 a = n(23203),
                 s = n(92233),
                 l = n(36e3),
-                c = n(82361),
+                c = n(48157),
                 u = n(4947),
                 d = n(23326),
                 h = n.n(d);
             n(82017), n(91123), n(61682), n(32407), n(3519), n(79501), n(56755), n(991), n(57342), n(49469), n(60509), n(81094), n(79480), n(70722), n(45751), n(19757), n(19238), n(43602), n(25022), n(37103), n(83280), n(94521);
             var f = n(21332),
                 p = n(23463),
                 m = n(1872);
```

### Comparing `voici-0.4.3/voici/static/build/9339.js` & `voici-0.4.4/voici/static/build/9339.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/9406.js` & `voici-0.4.4/voici/static/build/9406.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/9513.js` & `voici-0.4.4/voici/static/build/9513.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/9727.js` & `voici-0.4.4/voici/static/build/9727.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/9757.js` & `voici-0.4.4/voici/static/build/9757.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/9780.js` & `voici-0.4.4/voici/static/build/9780.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -29,18 +29,18 @@
                 return (0, n.showErrorMessage)(a, {
                     message: o
                 })
             };
             var a, o, d = i(77968),
                 l = i(70988),
                 c = i(24643),
-                h = i(76219),
+                h = i(8971),
                 u = i(92233),
                 p = i(4947);
-            class g extends h.M {
+            class g extends h.Application {
                     constructor(e) {
                         super(e), this._formatChanged = new p.Signal(this), this.contextMenu = new c.ContextMenuSvg({
                             commands: this.commands,
                             renderer: e.contextMenuRenderer,
                             groupByTarget: !1,
                             sortBySelector: !1
                         });
@@ -411,15 +411,15 @@
                 e.factoryNameProperty = new f.AttachedProperty({
                     name: "factoryName",
                     create: () => {}
                 })
             }(A || (A = {}));
             var T = i(23203),
                 B = i(78695),
-                M = i(82361),
+                M = i(48157),
                 W = i(42051);
             const x = "jp-SideBar",
                 S = "jp-mod-current",
                 L = "jp-mod-active",
                 E = 900,
                 H = "jp-Activity",
                 D = new u.Token("@jupyterlab/application:ILabShell");
```

### Comparing `voici-0.4.3/voici/static/build/9807.js` & `voici-0.4.4/voici/static/build/9807.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/9900.js` & `voici-0.4.4/voici/static/build/9900.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/9988.js` & `voici-0.4.4/voici/static/build/9988.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/service-worker-b2fb40a.js` & `voici-0.4.4/voici/static/build/service-worker-b2fb40a.js`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/voici/static/build/treepage.js` & `voici-0.4.4/voici/static/build/treepage.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,13 @@
 var _JUPYTERLAB;
 (() => {
-    var e, t, l, r, a, n, o, i, u, s, m, p, h, d = {
+    var e, t, l, r, a, n, o, i, u, s, m, h, p, d = {
             60392: (e, t, l) => {
                 "use strict";
-                Promise.all([l.e(2233), l.e(2051), l.e(9110), l.e(7782), l.e(2299), l.e(3198), l.e(7651), l.e(5238), l.e(49), l.e(4456), l.e(5918), l.e(8987), l.e(6852)]).then(l.bind(l, 46852))
+                Promise.all([l.e(2051), l.e(9110), l.e(7782), l.e(2299), l.e(3198), l.e(7651), l.e(5238), l.e(49), l.e(4456), l.e(5918), l.e(8987), l.e(6852)]).then(l.bind(l, 46852))
             },
             68444: (e, t, l) => {
                 l.p = function(e) {
                     let t = Object.create(null);
                     if ("undefined" != typeof document && document) {
                         const e = document.getElementById("jupyter-config-data");
                         e && (t = JSON.parse(e.textContent || "{}"))
@@ -67,24 +67,24 @@
                     var m = u[s];
                     if (m.getAttribute("src") == e || m.getAttribute("data-webpack") == r + a) {
                         o = m;
                         break
                     }
                 }
             o || (i = !0, (o = document.createElement("script")).charset = "utf-8", o.timeout = 120, c.nc && o.setAttribute("nonce", c.nc), o.setAttribute("data-webpack", r + a), o.src = e), l[e] = [t];
-            var p = (t, r) => {
-                    o.onerror = o.onload = null, clearTimeout(h);
+            var h = (t, r) => {
+                    o.onerror = o.onload = null, clearTimeout(p);
                     var a = l[e];
                     if (delete l[e], o.parentNode && o.parentNode.removeChild(o), a && a.forEach((e => e(r))), t) return t(r)
                 },
-                h = setTimeout(p.bind(null, void 0, {
+                p = setTimeout(h.bind(null, void 0, {
                     type: "timeout",
                     target: o
                 }), 12e4);
-            o.onerror = p.bind(null, o.onerror), o.onload = p.bind(null, o.onload), i && document.head.appendChild(o)
+            o.onerror = h.bind(null, o.onerror), o.onload = h.bind(null, o.onload), i && document.head.appendChild(o)
         }
     }, c.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -106,15 +106,15 @@
                         (!i || !i.loaded && (!r != !i.eager ? r : o > i.from)) && (a[t] = {
                             get: l,
                             from: o,
                             eager: !!r
                         })
                     },
                     u = [];
-                return "default" === l && (i("@jupyter-widgets/base", "6.0.4", (() => Promise.all([c.e(8291), c.e(9900), c.e(2233), c.e(2051), c.e(8695)]).then((() => () => c(9900))))), i("@jupyter-widgets/controls", "5.0.5", (() => Promise.all([c.e(8291), c.e(3851), c.e(4947), c.e(3203), c.e(2051), c.e(8695), c.e(4812), c.e(7651), c.e(6587)]).then((() => () => c(53851))))), i("@jupyter-widgets/jupyterlab-manager", "5.0.7", (() => Promise.all([c.e(8291), c.e(1672), c.e(9727), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(4629), c.e(988), c.e(2299), c.e(8930), c.e(3198), c.e(7651), c.e(49), c.e(5320), c.e(6678), c.e(2266)]).then((() => () => c(9727))))), i("@jupyter-widgets/output", "6.0.4", (() => Promise.all([c.e(7651), c.e(1100)]).then((() => () => c(21100))))), i("@jupyterlab/application", "3.6.3", (() => Promise.all([c.e(2361), c.e(6219), c.e(9780), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(4629), c.e(9110), c.e(7782), c.e(4643), c.e(988), c.e(2299), c.e(8695), c.e(1514), c.e(7968)]).then((() => () => c(79780))))), i("@jupyterlab/apputils-extension", "3.6.3", (() => Promise.all([c.e(2361), c.e(6770), c.e(846), c.e(4939), c.e(7066), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(4629), c.e(9110), c.e(7782), c.e(4643), c.e(7505), c.e(988), c.e(1514), c.e(7968), c.e(4627), c.e(8930), c.e(5238), c.e(5320)]).then((() => () => c(97066))))), i("@jupyterlab/apputils", "3.6.3", (() => Promise.all([c.e(2361), c.e(846), c.e(1672), c.e(339), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(4629), c.e(9110), c.e(4643), c.e(7505), c.e(988), c.e(8695), c.e(1514), c.e(4812), c.e(4627), c.e(8930), c.e(1732)]).then((() => () => c(90339))))), i("@jupyterlab/coreutils", "5.5.3", (() => Promise.all([c.e(5952), c.e(286), c.e(4947), c.e(2233), c.e(6616)]).then((() => () => c(20286))))), i("@jupyterlab/coreutils", "5.5.3", (() => Promise.all([c.e(5952), c.e(2359), c.e(4947), c.e(2233), c.e(709)]).then((() => () => c(62359))))), i("@jupyterlab/coreutils", "5.5.3", (() => Promise.all([c.e(5952), c.e(53), c.e(4947), c.e(2233), c.e(6178)]).then((() => () => c(70053))))), i("@jupyterlab/coreutils", "5.5.3", (() => Promise.all([c.e(5952), c.e(3922), c.e(4947), c.e(2233), c.e(2630)]).then((() => () => c(13922))))), i("@jupyterlab/coreutils", "5.5.3", (() => Promise.all([c.e(5952), c.e(596), c.e(4947), c.e(2233), c.e(6614)]).then((() => () => c(20596))))), i("@jupyterlab/coreutils", "5.5.3", (() => Promise.all([c.e(5952), c.e(1980), c.e(4947), c.e(2233), c.e(1023)]).then((() => () => c(1980))))), i("@jupyterlab/coreutils", "5.5.3", (() => Promise.all([c.e(5952), c.e(4896), c.e(4947), c.e(2233), c.e(6790)]).then((() => () => c(4896))))), i("@jupyterlab/coreutils", "5.6.3", (() => Promise.all([c.e(5952), c.e(103), c.e(4947), c.e(2233), c.e(3086)]).then((() => () => c(60103))))), i("@jupyterlab/coreutils", "5.6.3", (() => Promise.all([c.e(5952), c.e(2950), c.e(4947), c.e(2233), c.e(1667)]).then((() => () => c(42950))))), i("@jupyterlab/coreutils", "5.6.3", (() => Promise.all([c.e(5952), c.e(3251), c.e(4947), c.e(2233), c.e(7623)]).then((() => () => c(53251))))), i("@jupyterlab/docregistry", "3.6.3", (() => Promise.all([c.e(2361), c.e(6770), c.e(4939), c.e(9112), c.e(4875), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(9110), c.e(7782), c.e(4643), c.e(7505), c.e(2299), c.e(8695), c.e(6088), c.e(1876)]).then((() => () => c(74875))))), i("@jupyterlab/json-extension", "3.6.3", (() => Promise.all([c.e(5950), c.e(2233), c.e(6956), c.e(2051), c.e(7782), c.e(4643), c.e(7505), c.e(4627)]).then((() => () => c(45950))))), i("@jupyterlab/logconsole", "3.6.3", (() => Promise.all([c.e(9339), c.e(4947), c.e(2233), c.e(6956), c.e(2051), c.e(2299), c.e(3198)]).then((() => () => c(99339))))), i("@jupyterlab/mainmenu", "3.6.3", (() => Promise.all([c.e(2233), c.e(3203), c.e(2051), c.e(4643), c.e(1581)]).then((() => () => c(21581))))), i("@jupyterlab/markdownviewer-extension", "3.6.3", (() => Promise.all([c.e(2233), c.e(6956), c.e(2051), c.e(9110), c.e(7782), c.e(2299), c.e(7968), c.e(8930), c.e(5238), c.e(4382)]).then((() => () => c(54382))))), i("@jupyterlab/mathjax2-extension", "3.6.3", (() => Promise.all([c.e(2233), c.e(9110), c.e(2299), c.e(6976)]).then((() => () => c(66976))))), i("@jupyterlab/nbformat", "3.6.3", (() => Promise.all([c.e(2233), c.e(3655)]).then((() => () => c(63655))))), i("@jupyterlab/notebook", "3.6.3", (() => Promise.all([c.e(2361), c.e(6770), c.e(4939), c.e(9112), c.e(8085), c.e(4977), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(4629), c.e(9110), c.e(7782), c.e(4643), c.e(7505), c.e(988), c.e(2299), c.e(8695), c.e(4812), c.e(7968), c.e(6088), c.e(1876), c.e(3198), c.e(9939), c.e(2886), c.e(3860)]).then((() => () => c(24977))))), i("@jupyterlab/outputarea", "3.6.3", (() => Promise.all([c.e(1432), c.e(4947), c.e(2233), c.e(3203), c.e(2051), c.e(4629), c.e(7782), c.e(988), c.e(2299), c.e(9939)]).then((() => () => c(31432))))), i("@jupyterlab/rendermime-extension", "3.6.3", (() => Promise.all([c.e(2233), c.e(6956), c.e(7782), c.e(2299), c.e(5985)]).then((() => () => c(85985))))), i("@jupyterlab/rendermime", "3.6.3", (() => Promise.all([c.e(2361), c.e(6770), c.e(4939), c.e(9112), c.e(8085), c.e(2075), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(9110), c.e(7782), c.e(4643), c.e(7505), c.e(8695), c.e(6088), c.e(1876), c.e(9939)]).then((() => () => c(82075))))), i("@jupyterlab/services", "6.5.3", (() => Promise.all([c.e(2361), c.e(846), c.e(7560), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(4629), c.e(9098), c.e(3008)]).then((() => () => c(17560))))), i("@jupyterlab/services", "6.5.3", (() => Promise.all([c.e(2361), c.e(74), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(4629), c.e(5490), c.e(9320)]).then((() => () => c(80074))))), i("@jupyterlab/services", "6.6.3", (() => Promise.all([c.e(2361), c.e(846), c.e(6914), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(4629), c.e(9110), c.e(1497)]).then((() => () => c(16914))))), i("@jupyterlab/settingregistry", "3.6.3", (() => Promise.all([c.e(6111), c.e(9513), c.e(4947), c.e(2233), c.e(6e3), c.e(1514)]).then((() => () => c(69513))))), i("@jupyterlab/theme-dark-extension", "3.6.3", (() => Promise.all([c.e(6956), c.e(7782), c.e(1058)]).then((() => () => c(21058))))), i("@jupyterlab/theme-light-extension", "3.6.3", (() => Promise.all([c.e(6956), c.e(7782), c.e(275)]).then((() => () => c(60275))))), i("@jupyterlab/translation", "3.6.3", (() => Promise.all([c.e(846), c.e(2322), c.e(4947), c.e(2233), c.e(4629), c.e(9110), c.e(988)]).then((() => () => c(29513))))), i("@jupyterlab/ui-components", "3.6.3", (() => Promise.all([c.e(6770), c.e(4963), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(9110), c.e(7505), c.e(4627), c.e(2886)]).then((() => () => c(74963))))), i("@jupyterlite/contents", "0.1.0", (() => Promise.all([c.e(9757), c.e(2233), c.e(9110)]).then((() => () => c(9757))))), i("@jupyterlite/iframe-extension", "0.1.0", (() => Promise.all([c.e(2233), c.e(2051), c.e(6527)]).then((() => () => c(26527))))), i("@jupyterlite/kernel", "0.1.0", (() => Promise.all([c.e(9988), c.e(3693), c.e(4947), c.e(2233), c.e(5820)]).then((() => () => c(83693))))), i("@jupyterlite/server-extension", "0.1.0", (() => Promise.all([c.e(6111), c.e(4530), c.e(2233), c.e(3203), c.e(4456), c.e(7631), c.e(3862)]).then((() => () => c(24530))))), i("@jupyterlite/server", "0.1.0", (() => Promise.all([c.e(6219), c.e(9988), c.e(4947), c.e(2233), c.e(2051), c.e(1514), c.e(568), c.e(3256)]).then((() => () => c(93256))))), i("@lumino/algorithm", "1.9.2", (() => c.e(9060).then((() => () => c(69060))))), i("@lumino/algorithm", "2.0.0", (() => c.e(9807).then((() => () => c(89807))))), i("@lumino/commands", "1.21.1", (() => Promise.all([c.e(2687), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(4812)]).then((() => () => c(62687))))), i("@lumino/coreutils", "1.12.1", (() => c.e(1770).then((() => () => c(71770))))), i("@lumino/coreutils", "2.1.0", (() => c.e(4259).then((() => () => c(4259))))), i("@lumino/disposable", "1.10.4", (() => Promise.all([c.e(4947), c.e(3203), c.e(2488)]).then((() => () => c(72488))))), i("@lumino/domutils", "1.8.2", (() => c.e(5403).then((() => () => c(85403))))), i("@lumino/dragdrop", "1.14.5", (() => Promise.all([c.e(8809), c.e(6e3)]).then((() => () => c(38809))))), i("@lumino/messaging", "1.10.3", (() => Promise.all([c.e(3316), c.e(3203)]).then((() => () => c(73316))))), i("@lumino/properties", "1.8.2", (() => c.e(3312).then((() => () => c(73312))))), i("@lumino/signaling", "1.11.1", (() => Promise.all([c.e(3203), c.e(4629), c.e(5445)]).then((() => () => c(75445))))), i("@lumino/signaling", "2.1.0", (() => Promise.all([c.e(6088), c.e(319), c.e(7003)]).then((() => () => c(27003))))), i("@lumino/virtualdom", "1.14.3", (() => Promise.all([c.e(1053), c.e(3203)]).then((() => () => c(1053))))), i("@lumino/widgets", "1.37.2", (() => Promise.all([c.e(450), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(4629), c.e(8695), c.e(1514), c.e(4812), c.e(2886), c.e(3860)]).then((() => () => c(90450))))), i("@voila-dashboards/voila", "0.5.0-alpha.3", (() => Promise.all([c.e(2361), c.e(846), c.e(6914), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(4629), c.e(9110), c.e(988), c.e(2299), c.e(7651), c.e(5238), c.e(5918), c.e(3504)]).then((() => () => c(17696))))), i("react-dom", "17.0.2", (() => Promise.all([c.e(8316), c.e(7505)]).then((() => () => c(28316))))), i("react", "17.0.2", (() => c.e(2784).then((() => () => c(2784)))))), e[l] = u.length ? Promise.all(u).then((() => e[l] = 1)) : 1
+                return "default" === l && (i("@jupyter-widgets/base", "6.0.4", (() => Promise.all([c.e(8291), c.e(9900), c.e(2233), c.e(2051), c.e(8695)]).then((() => () => c(9900))))), i("@jupyter-widgets/controls", "5.0.5", (() => Promise.all([c.e(8291), c.e(3851), c.e(4947), c.e(3203), c.e(2051), c.e(8695), c.e(4812), c.e(7651), c.e(6587)]).then((() => () => c(53851))))), i("@jupyter-widgets/jupyterlab-manager", "5.0.7", (() => Promise.all([c.e(8291), c.e(1672), c.e(9727), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(4629), c.e(988), c.e(2299), c.e(8930), c.e(3198), c.e(7651), c.e(49), c.e(5320), c.e(6678), c.e(2266)]).then((() => () => c(9727))))), i("@jupyter-widgets/output", "6.0.4", (() => Promise.all([c.e(7651), c.e(1100)]).then((() => () => c(21100))))), i("@jupyterlab/application", "3.6.3", (() => Promise.all([c.e(9780), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(4629), c.e(8157), c.e(9110), c.e(7782), c.e(8695), c.e(4643), c.e(988), c.e(2299), c.e(7968), c.e(8971)]).then((() => () => c(79780))))), i("@jupyterlab/apputils-extension", "3.6.3", (() => Promise.all([c.e(6770), c.e(846), c.e(4939), c.e(7066), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(4629), c.e(8157), c.e(9110), c.e(7782), c.e(4643), c.e(7505), c.e(988), c.e(1514), c.e(7968), c.e(4627), c.e(8930), c.e(5238), c.e(5320)]).then((() => () => c(97066))))), i("@jupyterlab/apputils", "3.6.3", (() => Promise.all([c.e(846), c.e(1672), c.e(339), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(4629), c.e(8157), c.e(9110), c.e(8695), c.e(4643), c.e(7505), c.e(988), c.e(4812), c.e(1514), c.e(4627), c.e(8930), c.e(1732)]).then((() => () => c(90339))))), i("@jupyterlab/coreutils", "5.5.3", (() => Promise.all([c.e(5952), c.e(286), c.e(4947), c.e(2233), c.e(6616)]).then((() => () => c(20286))))), i("@jupyterlab/coreutils", "5.5.3", (() => Promise.all([c.e(5952), c.e(2359), c.e(4947), c.e(2233), c.e(709)]).then((() => () => c(62359))))), i("@jupyterlab/coreutils", "5.5.3", (() => Promise.all([c.e(5952), c.e(53), c.e(4947), c.e(2233), c.e(6178)]).then((() => () => c(70053))))), i("@jupyterlab/coreutils", "5.5.3", (() => Promise.all([c.e(5952), c.e(3922), c.e(4947), c.e(2233), c.e(2630)]).then((() => () => c(13922))))), i("@jupyterlab/coreutils", "5.5.3", (() => Promise.all([c.e(5952), c.e(596), c.e(4947), c.e(2233), c.e(6614)]).then((() => () => c(20596))))), i("@jupyterlab/coreutils", "5.5.3", (() => Promise.all([c.e(5952), c.e(1980), c.e(4947), c.e(2233), c.e(1023)]).then((() => () => c(1980))))), i("@jupyterlab/coreutils", "5.5.3", (() => Promise.all([c.e(5952), c.e(4896), c.e(4947), c.e(2233), c.e(6790)]).then((() => () => c(4896))))), i("@jupyterlab/coreutils", "5.6.3", (() => Promise.all([c.e(5952), c.e(103), c.e(4947), c.e(2233), c.e(3086)]).then((() => () => c(60103))))), i("@jupyterlab/coreutils", "5.6.3", (() => Promise.all([c.e(5952), c.e(2950), c.e(4947), c.e(2233), c.e(1667)]).then((() => () => c(42950))))), i("@jupyterlab/coreutils", "5.6.3", (() => Promise.all([c.e(5952), c.e(3251), c.e(4947), c.e(2233), c.e(7623)]).then((() => () => c(53251))))), i("@jupyterlab/docregistry", "3.6.3", (() => Promise.all([c.e(6770), c.e(4939), c.e(9112), c.e(4875), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(8157), c.e(9110), c.e(7782), c.e(8695), c.e(4643), c.e(7505), c.e(2299), c.e(6088), c.e(1876)]).then((() => () => c(74875))))), i("@jupyterlab/json-extension", "3.6.3", (() => Promise.all([c.e(5950), c.e(2233), c.e(6956), c.e(2051), c.e(7782), c.e(4643), c.e(7505), c.e(4627)]).then((() => () => c(45950))))), i("@jupyterlab/logconsole", "3.6.3", (() => Promise.all([c.e(9339), c.e(4947), c.e(2233), c.e(6956), c.e(2051), c.e(2299), c.e(3198)]).then((() => () => c(99339))))), i("@jupyterlab/mainmenu", "3.6.3", (() => Promise.all([c.e(2233), c.e(3203), c.e(2051), c.e(4643), c.e(1581)]).then((() => () => c(21581))))), i("@jupyterlab/markdownviewer-extension", "3.6.3", (() => Promise.all([c.e(2233), c.e(6956), c.e(2051), c.e(9110), c.e(7782), c.e(2299), c.e(7968), c.e(8930), c.e(5238), c.e(4382)]).then((() => () => c(54382))))), i("@jupyterlab/mathjax2-extension", "3.6.3", (() => Promise.all([c.e(2233), c.e(9110), c.e(2299), c.e(6976)]).then((() => () => c(66976))))), i("@jupyterlab/nbformat", "3.6.3", (() => Promise.all([c.e(2233), c.e(3655)]).then((() => () => c(63655))))), i("@jupyterlab/notebook", "3.6.3", (() => Promise.all([c.e(6770), c.e(4939), c.e(9112), c.e(8085), c.e(4977), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(4629), c.e(8157), c.e(9110), c.e(7782), c.e(8695), c.e(4643), c.e(7505), c.e(988), c.e(2299), c.e(4812), c.e(7968), c.e(6088), c.e(2886), c.e(1876), c.e(3198), c.e(9939), c.e(3860)]).then((() => () => c(24977))))), i("@jupyterlab/outputarea", "3.6.3", (() => Promise.all([c.e(1432), c.e(4947), c.e(2233), c.e(3203), c.e(2051), c.e(4629), c.e(7782), c.e(988), c.e(2299), c.e(9939)]).then((() => () => c(31432))))), i("@jupyterlab/rendermime-extension", "3.6.3", (() => Promise.all([c.e(2233), c.e(6956), c.e(7782), c.e(2299), c.e(5985)]).then((() => () => c(85985))))), i("@jupyterlab/rendermime", "3.6.3", (() => Promise.all([c.e(6770), c.e(4939), c.e(9112), c.e(8085), c.e(2075), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(8157), c.e(9110), c.e(7782), c.e(8695), c.e(4643), c.e(7505), c.e(6088), c.e(1876), c.e(9939)]).then((() => () => c(82075))))), i("@jupyterlab/services", "6.5.3", (() => Promise.all([c.e(846), c.e(7560), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(4629), c.e(8157), c.e(9098), c.e(3008)]).then((() => () => c(17560))))), i("@jupyterlab/services", "6.5.3", (() => Promise.all([c.e(74), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(4629), c.e(8157), c.e(5490), c.e(9320)]).then((() => () => c(80074))))), i("@jupyterlab/services", "6.6.3", (() => Promise.all([c.e(846), c.e(6914), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(4629), c.e(8157), c.e(9110), c.e(1497)]).then((() => () => c(16914))))), i("@jupyterlab/settingregistry", "3.6.3", (() => Promise.all([c.e(6111), c.e(9513), c.e(4947), c.e(2233), c.e(6e3), c.e(1514)]).then((() => () => c(69513))))), i("@jupyterlab/theme-dark-extension", "3.6.3", (() => Promise.all([c.e(6956), c.e(7782), c.e(1058)]).then((() => () => c(21058))))), i("@jupyterlab/theme-light-extension", "3.6.3", (() => Promise.all([c.e(6956), c.e(7782), c.e(275)]).then((() => () => c(60275))))), i("@jupyterlab/translation", "3.6.3", (() => Promise.all([c.e(846), c.e(2322), c.e(4947), c.e(2233), c.e(4629), c.e(9110), c.e(988)]).then((() => () => c(29513))))), i("@jupyterlab/ui-components", "3.6.3", (() => Promise.all([c.e(6770), c.e(4963), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(9110), c.e(7505), c.e(4627), c.e(2886)]).then((() => () => c(74963))))), i("@jupyterlite/contents", "0.1.0", (() => Promise.all([c.e(9757), c.e(2233), c.e(9110)]).then((() => () => c(9757))))), i("@jupyterlite/iframe-extension", "0.1.0", (() => Promise.all([c.e(2233), c.e(2051), c.e(6527)]).then((() => () => c(26527))))), i("@jupyterlite/kernel", "0.1.0", (() => Promise.all([c.e(9988), c.e(3693), c.e(4947), c.e(2233), c.e(5820)]).then((() => () => c(83693))))), i("@jupyterlite/server-extension", "0.1.0", (() => Promise.all([c.e(6111), c.e(4530), c.e(2233), c.e(3203), c.e(4456), c.e(7631), c.e(3862)]).then((() => () => c(24530))))), i("@jupyterlite/server", "0.1.0", (() => Promise.all([c.e(9988), c.e(4947), c.e(2233), c.e(8971), c.e(568), c.e(3256)]).then((() => () => c(93256))))), i("@lumino/algorithm", "1.9.2", (() => c.e(9060).then((() => () => c(69060))))), i("@lumino/algorithm", "2.0.0", (() => c.e(9807).then((() => () => c(89807))))), i("@lumino/application", "1.31.4", (() => Promise.all([c.e(6219), c.e(2233), c.e(2051), c.e(1514)]).then((() => () => c(76219))))), i("@lumino/commands", "1.21.1", (() => Promise.all([c.e(2687), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(4812), c.e(6968)]).then((() => () => c(62687))))), i("@lumino/coreutils", "1.12.1", (() => c.e(1770).then((() => () => c(71770))))), i("@lumino/coreutils", "2.1.0", (() => c.e(4259).then((() => () => c(4259))))), i("@lumino/datagrid", "0.36.9", (() => Promise.all([c.e(8921), c.e(4947), c.e(2233), c.e(3203), c.e(2051), c.e(8695), c.e(4812), c.e(6968), c.e(3860)]).then((() => () => c(28921))))), i("@lumino/disposable", "1.10.4", (() => Promise.all([c.e(4947), c.e(3203), c.e(2488)]).then((() => () => c(72488))))), i("@lumino/domutils", "1.8.2", (() => c.e(5403).then((() => () => c(85403))))), i("@lumino/dragdrop", "1.14.5", (() => Promise.all([c.e(8809), c.e(6e3)]).then((() => () => c(38809))))), i("@lumino/keyboard", "1.8.2", (() => c.e(8102).then((() => () => c(34938))))), i("@lumino/messaging", "1.10.3", (() => Promise.all([c.e(3316), c.e(3203)]).then((() => () => c(73316))))), i("@lumino/polling", "1.11.4", (() => Promise.all([c.e(2361), c.e(4947), c.e(2233)]).then((() => () => c(82361))))), i("@lumino/properties", "1.8.2", (() => c.e(3312).then((() => () => c(73312))))), i("@lumino/signaling", "1.11.1", (() => Promise.all([c.e(3203), c.e(4629), c.e(5445)]).then((() => () => c(75445))))), i("@lumino/signaling", "2.1.0", (() => Promise.all([c.e(6088), c.e(319), c.e(7003)]).then((() => () => c(27003))))), i("@lumino/virtualdom", "1.14.3", (() => Promise.all([c.e(1053), c.e(3203)]).then((() => () => c(1053))))), i("@lumino/widgets", "1.37.2", (() => Promise.all([c.e(450), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(4629), c.e(8695), c.e(4812), c.e(1514), c.e(2886), c.e(6968), c.e(3860)]).then((() => () => c(90450))))), i("@voila-dashboards/voila", "0.5.0-alpha.3", (() => Promise.all([c.e(846), c.e(6914), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(4629), c.e(8157), c.e(9110), c.e(988), c.e(2299), c.e(7651), c.e(5238), c.e(5918), c.e(3504)]).then((() => () => c(17696))))), i("react-dom", "17.0.2", (() => Promise.all([c.e(8316), c.e(7505)]).then((() => () => c(28316))))), i("react", "17.0.2", (() => c.e(2784).then((() => () => c(2784)))))), e[l] = u.length ? Promise.all(u).then((() => e[l] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         c.g.importScripts && (e = c.g.location + "");
         var t = c.g.document;
         if (!e && t && (t.currentScript && (e = t.currentScript.src), !e)) {
@@ -144,106 +144,109 @@
     }, o = (e, t) => {
         if (0 in e) {
             t = a(t);
             var l = e[0],
                 r = l < 0;
             r && (l = -l - 1);
             for (var n = 0, i = 1, u = !0;; i++, n++) {
-                var s, m, p = i < e.length ? (typeof e[i])[0] : "";
-                if (n >= t.length || "o" == (m = (typeof(s = t[n]))[0])) return !u || ("u" == p ? i > l && !r : "" == p != r);
+                var s, m, h = i < e.length ? (typeof e[i])[0] : "";
+                if (n >= t.length || "o" == (m = (typeof(s = t[n]))[0])) return !u || ("u" == h ? i > l && !r : "" == h != r);
                 if ("u" == m) {
-                    if (!u || "u" != p) return !1
+                    if (!u || "u" != h) return !1
                 } else if (u)
-                    if (p == m)
+                    if (h == m)
                         if (i <= l) {
                             if (s != e[i]) return !1
                         } else {
                             if (r ? s > e[i] : s < e[i]) return !1;
                             s != e[i] && (u = !1)
                         }
-                else if ("s" != p && "n" != p) {
+                else if ("s" != h && "n" != h) {
                     if (r || i <= l) return !1;
                     u = !1, i--
                 } else {
-                    if (i <= l || m < p != r) return !1;
+                    if (i <= l || m < h != r) return !1;
                     u = !1
-                } else "s" != p && "n" != p && (u = !1, i--)
+                } else "s" != h && "n" != h && (u = !1, i--)
             }
         }
-        var h = [],
-            d = h.pop.bind(h);
+        var p = [],
+            d = p.pop.bind(p);
         for (n = 1; n < e.length; n++) {
             var f = e[n];
-            h.push(1 == f ? d() | d() : 2 == f ? d() & d() : f ? o(f, t) : !d())
+            p.push(1 == f ? d() | d() : 2 == f ? d() & d() : f ? o(f, t) : !d())
         }
         return !!d()
     }, i = (e, t, l) => {
         var r = e[t];
         return (t = Object.keys(r).reduce(((e, t) => !o(l, t) || e && !n(e, t) ? e : t), 0)) && r[t]
     }, u = e => (e.loaded = 1, e.get()), s = (e => function(t, l, r, a) {
         var n = c.I(t);
         return n && n.then ? n.then(e.bind(e, t, c.S[t], l, r, a)) : e(0, c.S[t], l, r, a)
     })(((e, t, l, r, a) => {
         var n = t && c.o(t, l) && i(t, l, r);
         return n ? u(n) : a()
-    })), m = {}, p = {
+    })), m = {}, h = {
         92233: () => s("default", "@lumino/coreutils", [1, 1, 8, 2], (() => c.e(1770).then((() => () => c(71770))))),
-        42051: () => s("default", "@lumino/widgets", [1, 1, 26, 2], (() => Promise.all([c.e(450), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(4629), c.e(8695), c.e(1514), c.e(4812), c.e(2886), c.e(3860)]).then((() => () => c(90450))))),
+        42051: () => s("default", "@lumino/widgets", [1, 1, 26, 2], (() => Promise.all([c.e(450), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(4629), c.e(8695), c.e(4812), c.e(1514), c.e(2886), c.e(6968), c.e(3860)]).then((() => () => c(90450))))),
         78695: () => s("default", "@lumino/messaging", [1, 1, 7, 2], (() => Promise.all([c.e(3316), c.e(3203)]).then((() => () => c(73316))))),
         4947: () => s("default", "@lumino/signaling", [1, 1, 7, 2], (() => Promise.all([c.e(3203), c.e(4629), c.e(5445)]).then((() => () => c(75445))))),
         23203: () => s("default", "@lumino/algorithm", [1, 1, 6, 2], (() => c.e(9060).then((() => () => c(69060))))),
         94812: () => s("default", "@lumino/domutils", [1, 1, 5, 2], (() => c.e(5403).then((() => () => c(85403))))),
         67651: () => s("default", "@jupyter-widgets/base", [1, 6, 0, 1], (() => Promise.all([c.e(8291), c.e(9900), c.e(2233), c.e(2051), c.e(8695)]).then((() => () => c(9900))))),
         36e3: () => s("default", "@lumino/disposable", [1, 1, 7, 2], (() => Promise.all([c.e(4947), c.e(3203), c.e(2488)]).then((() => () => c(72488))))),
         56956: () => s("default", "@jupyterlab/translation", [1, 3, 0, 0], (() => Promise.all([c.e(846), c.e(2322), c.e(4947), c.e(2233), c.e(4629), c.e(9110), c.e(988)]).then((() => () => c(29513))))),
         24629: () => s("default", "@lumino/properties", [1, 1, 5, 2], (() => c.e(3312).then((() => () => c(73312))))),
-        70988: () => s("default", "@jupyterlab/services", [1, 6, 1, 8], (() => Promise.all([c.e(2361), c.e(846), c.e(6914), c.e(3203), c.e(6e3), c.e(9110), c.e(6417)]).then((() => () => c(16914))))),
-        12299: () => s("default", "@jupyterlab/rendermime", [1, 3, 0, 0], (() => Promise.all([c.e(2361), c.e(6770), c.e(4939), c.e(9112), c.e(8085), c.e(2075), c.e(4947), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(9110), c.e(7782), c.e(4643), c.e(7505), c.e(8695), c.e(6088), c.e(1876), c.e(9939)]).then((() => () => c(82075))))),
+        70988: () => s("default", "@jupyterlab/services", [1, 6, 1, 8], (() => Promise.all([c.e(846), c.e(6914), c.e(3203), c.e(6e3), c.e(8157), c.e(9110), c.e(6417)]).then((() => () => c(16914))))),
+        12299: () => s("default", "@jupyterlab/rendermime", [1, 3, 0, 0], (() => Promise.all([c.e(6770), c.e(4939), c.e(9112), c.e(8085), c.e(2075), c.e(4947), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(8157), c.e(9110), c.e(7782), c.e(8695), c.e(4643), c.e(7505), c.e(6088), c.e(1876), c.e(9939)]).then((() => () => c(82075))))),
         68930: () => s("default", "@jupyterlab/settingregistry", [1, 3, 0, 0], (() => Promise.all([c.e(6111), c.e(9513), c.e(4947), c.e(6e3), c.e(1514)]).then((() => () => c(69513))))),
         73198: () => s("default", "@jupyterlab/outputarea", [1, 3, 0, 0], (() => Promise.all([c.e(1432), c.e(4947), c.e(3203), c.e(4629), c.e(7782), c.e(988), c.e(9939)]).then((() => () => c(31432))))),
-        40049: () => s("default", "@jupyterlab/notebook", [1, 3, 0, 0], (() => Promise.all([c.e(2361), c.e(6770), c.e(4939), c.e(9112), c.e(8085), c.e(4977), c.e(4947), c.e(3203), c.e(6e3), c.e(6956), c.e(4629), c.e(9110), c.e(7782), c.e(4643), c.e(7505), c.e(988), c.e(8695), c.e(4812), c.e(7968), c.e(6088), c.e(1876), c.e(9939), c.e(2886), c.e(3860)]).then((() => () => c(24977))))),
+        40049: () => s("default", "@jupyterlab/notebook", [1, 3, 0, 0], (() => Promise.all([c.e(6770), c.e(4939), c.e(9112), c.e(8085), c.e(4977), c.e(4947), c.e(3203), c.e(6e3), c.e(6956), c.e(4629), c.e(8157), c.e(9110), c.e(7782), c.e(8695), c.e(4643), c.e(7505), c.e(988), c.e(4812), c.e(7968), c.e(6088), c.e(2886), c.e(1876), c.e(9939), c.e(3860)]).then((() => () => c(24977))))),
         5320: () => s("default", "@jupyterlab/mainmenu", [1, 3, 0, 0], (() => Promise.all([c.e(4643), c.e(9406)]).then((() => () => c(21581))))),
         10409: () => s("default", "@jupyter-widgets/output", [1, 6, 0, 1], (() => c.e(7015).then((() => () => c(21100))))),
         70190: () => s("default", "@jupyterlab/logconsole", [1, 3, 0, 0], (() => c.e(9339).then((() => () => c(99339))))),
+        48157: () => s("default", "@lumino/polling", [1, 1, 11, 4], (() => c.e(2361).then((() => () => c(82361))))),
         59110: () => s("default", "@jupyterlab/coreutils", [1, 5, 0, 0], (() => Promise.all([c.e(5952), c.e(103), c.e(4947), c.e(6196)]).then((() => () => c(60103))))),
-        37782: () => s("default", "@jupyterlab/apputils", [1, 3, 0, 0], (() => Promise.all([c.e(2361), c.e(846), c.e(1672), c.e(339), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(4629), c.e(9110), c.e(4643), c.e(7505), c.e(988), c.e(8695), c.e(1514), c.e(4812), c.e(4627), c.e(8930), c.e(1732)]).then((() => () => c(90339))))),
+        37782: () => s("default", "@jupyterlab/apputils", [1, 3, 0, 0], (() => Promise.all([c.e(846), c.e(1672), c.e(339), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(4629), c.e(8157), c.e(9110), c.e(8695), c.e(4643), c.e(7505), c.e(988), c.e(4812), c.e(1514), c.e(4627), c.e(8930), c.e(1732)]).then((() => () => c(90339))))),
         24643: () => s("default", "@jupyterlab/ui-components", [1, 3, 0, 0], (() => Promise.all([c.e(6770), c.e(4963), c.e(4947), c.e(3203), c.e(6e3), c.e(6956), c.e(9110), c.e(7505), c.e(4627), c.e(2886)]).then((() => () => c(74963))))),
-        1514: () => s("default", "@lumino/commands", [1, 1, 15, 2], (() => Promise.all([c.e(2687), c.e(3203), c.e(6e3), c.e(4812)]).then((() => () => c(62687))))),
-        77968: () => s("default", "@jupyterlab/docregistry", [1, 3, 0, 0], (() => Promise.all([c.e(2361), c.e(6770), c.e(4939), c.e(9112), c.e(4875), c.e(4947), c.e(3203), c.e(6e3), c.e(4643), c.e(7505), c.e(2299), c.e(8695), c.e(6088), c.e(1876)]).then((() => () => c(74875))))),
+        77968: () => s("default", "@jupyterlab/docregistry", [1, 3, 0, 0], (() => Promise.all([c.e(6770), c.e(4939), c.e(9112), c.e(4875), c.e(4947), c.e(3203), c.e(6e3), c.e(8157), c.e(8695), c.e(4643), c.e(7505), c.e(2299), c.e(6088), c.e(1876)]).then((() => () => c(74875))))),
+        8971: () => s("default", "@lumino/application", [1, 1, 31, 3], (() => Promise.all([c.e(6219), c.e(2051), c.e(1514)]).then((() => () => c(76219))))),
         97505: () => s("default", "react", [1, 17, 0, 1], (() => c.e(2784).then((() => () => c(2784))))),
+        1514: () => s("default", "@lumino/commands", [1, 1, 15, 2], (() => Promise.all([c.e(2687), c.e(4947), c.e(3203), c.e(6e3), c.e(4812), c.e(6968)]).then((() => () => c(62687))))),
         24627: () => s("default", "react-dom", [1, 17, 0, 1], (() => Promise.all([c.e(8316), c.e(7505)]).then((() => () => c(28316))))),
-        75238: () => s("default", "@jupyterlab/application", [1, 3, 0, 0], (() => Promise.all([c.e(2361), c.e(6219), c.e(9780), c.e(4947), c.e(3203), c.e(6e3), c.e(6956), c.e(4629), c.e(7782), c.e(4643), c.e(988), c.e(2299), c.e(8695), c.e(1514), c.e(7968)]).then((() => () => c(79780))))),
+        75238: () => s("default", "@jupyterlab/application", [1, 3, 0, 0], (() => Promise.all([c.e(9780), c.e(4947), c.e(3203), c.e(6e3), c.e(6956), c.e(4629), c.e(8157), c.e(7782), c.e(8695), c.e(4643), c.e(988), c.e(2299), c.e(7968), c.e(8971)]).then((() => () => c(79780))))),
         56088: () => s("default", "@lumino/coreutils", [1, 1, 8, 2], (() => c.e(4259).then((() => () => c(4259))))),
         91876: () => s("default", "@lumino/signaling", [1, 1, 7, 2], (() => Promise.all([c.e(319), c.e(1553)]).then((() => () => c(27003))))),
-        49939: () => s("default", "@jupyterlab/nbformat", [1, 3, 0, 0], (() => c.e(86).then((() => () => c(63655))))),
         32886: () => s("default", "@lumino/virtualdom", [1, 1, 11, 2], (() => c.e(1053).then((() => () => c(1053))))),
-        3860: () => s("default", "@lumino/dragdrop", [1, 1, 10, 2], (() => c.e(8809).then((() => () => c(38809))))),
+        49939: () => s("default", "@jupyterlab/nbformat", [1, 3, 0, 0], (() => c.e(86).then((() => () => c(63655))))),
+        3860: () => s("default", "@lumino/dragdrop", [1, 1, 10, 2], (() => Promise.all([c.e(8809), c.e(6e3)]).then((() => () => c(38809))))),
         89098: () => s("default", "@jupyterlab/coreutils", [1, 5, 0, 0], (() => Promise.all([c.e(5952), c.e(2950), c.e(1105)]).then((() => () => c(42950))))),
         15490: () => s("default", "@jupyterlab/coreutils", [1, 5, 0, 0], (() => Promise.all([c.e(5952), c.e(3251), c.e(8164)]).then((() => () => c(53251))))),
-        34013: () => s("default", "@jupyterlab/services", [1, 6, 1, 8], (() => Promise.all([c.e(2361), c.e(846), c.e(7560), c.e(3203), c.e(6e3), c.e(4629), c.e(9098), c.e(8679)]).then((() => () => c(17560))))),
+        34013: () => s("default", "@jupyterlab/services", [1, 6, 1, 8], (() => Promise.all([c.e(846), c.e(7560), c.e(3203), c.e(6e3), c.e(4629), c.e(8157), c.e(9098), c.e(8679)]).then((() => () => c(17560))))),
         49943: () => s("default", "@jupyterlab/coreutils", [1, 5, 0, 0], (() => Promise.all([c.e(5952), c.e(286), c.e(1890)]).then((() => () => c(20286))))),
-        94456: () => s("default", "@jupyterlite/server", [2, 0, 1, 0], (() => Promise.all([c.e(6219), c.e(9988), c.e(4947), c.e(2051), c.e(1514), c.e(568), c.e(6856)]).then((() => () => c(93256))))),
+        94456: () => s("default", "@jupyterlite/server", [2, 0, 1, 0], (() => Promise.all([c.e(9988), c.e(4947), c.e(8971), c.e(568), c.e(6856)]).then((() => () => c(93256))))),
         7631: () => s("default", "@jupyterlite/kernel", [2, 0, 1, 0], (() => Promise.all([c.e(9988), c.e(3693), c.e(4947), c.e(5820)]).then((() => () => c(83693))))),
         48753: () => s("default", "@jupyterlite/contents", [2, 0, 1, 0], (() => Promise.all([c.e(9757), c.e(9110)]).then((() => () => c(9757))))),
         52329: () => s("default", "@jupyterlab/coreutils", [1, 5, 0, 0], (() => Promise.all([c.e(5952), c.e(1980), c.e(4947), c.e(5188)]).then((() => () => c(1980))))),
         52390: () => s("default", "@jupyterlab/coreutils", [1, 5, 0, 0], (() => Promise.all([c.e(5952), c.e(53), c.e(4947), c.e(7695)]).then((() => () => c(70053))))),
         70771: () => s("default", "@jupyterlab/coreutils", [1, 5, 0, 0], (() => Promise.all([c.e(5952), c.e(2359), c.e(4947), c.e(6839)]).then((() => () => c(62359))))),
         81298: () => s("default", "@jupyterlab/coreutils", [1, 5, 0, 0], (() => Promise.all([c.e(5952), c.e(596), c.e(4947), c.e(7795)]).then((() => () => c(20596))))),
         91491: () => s("default", "@jupyterlab/coreutils", [1, 5, 0, 0], (() => Promise.all([c.e(5952), c.e(4896), c.e(4947), c.e(5291)]).then((() => () => c(4896))))),
-        2132: () => s("default", "@jupyterlab/services", [1, 6, 1, 8], (() => Promise.all([c.e(2361), c.e(74), c.e(3203), c.e(6e3), c.e(4629), c.e(5490), c.e(9817)]).then((() => () => c(80074))))),
+        2132: () => s("default", "@jupyterlab/services", [1, 6, 1, 8], (() => Promise.all([c.e(74), c.e(3203), c.e(6e3), c.e(4629), c.e(8157), c.e(5490), c.e(9817)]).then((() => () => c(80074))))),
         86086: () => s("default", "@jupyterlab/coreutils", [1, 5, 0, 0], (() => Promise.all([c.e(5952), c.e(3922), c.e(8874)]).then((() => () => c(13922))))),
+        26968: () => s("default", "@lumino/keyboard", [1, 1, 8, 0], (() => c.e(8102).then((() => () => c(34938))))),
         90319: () => s("default", "@lumino/algorithm", [1, 1, 6, 2], (() => c.e(9807).then((() => () => c(89807))))),
         35918: () => s("default", "@jupyter-widgets/jupyterlab-manager", [1, 5, 0, 3], (() => Promise.all([c.e(8291), c.e(1672), c.e(9727), c.e(4947), c.e(3203), c.e(6e3), c.e(6956), c.e(4629), c.e(988), c.e(8930), c.e(3198), c.e(49), c.e(5320), c.e(6678), c.e(2516)]).then((() => () => c(9727))))),
-        9961: () => s("default", "@jupyterlab/apputils-extension", [1, 3, 4, 8], (() => Promise.all([c.e(2361), c.e(6770), c.e(846), c.e(4939), c.e(7066), c.e(4947), c.e(3203), c.e(6e3), c.e(6956), c.e(4629), c.e(4643), c.e(7505), c.e(988), c.e(1514), c.e(7968), c.e(4627), c.e(8930), c.e(5320)]).then((() => () => c(97066))))),
-        22312: () => s("default", "@voila-dashboards/voila", [2, 0, 5, 0, , "alpha", 3], (() => Promise.all([c.e(2361), c.e(846), c.e(6914), c.e(4947), c.e(3203), c.e(6e3), c.e(6956), c.e(4629), c.e(988), c.e(2230)]).then((() => () => c(17696))))),
+        9961: () => s("default", "@jupyterlab/apputils-extension", [1, 3, 4, 8], (() => Promise.all([c.e(6770), c.e(846), c.e(4939), c.e(7066), c.e(4947), c.e(3203), c.e(6e3), c.e(6956), c.e(4629), c.e(8157), c.e(4643), c.e(7505), c.e(988), c.e(1514), c.e(7968), c.e(4627), c.e(8930), c.e(5320)]).then((() => () => c(97066))))),
+        22312: () => s("default", "@voila-dashboards/voila", [2, 0, 5, 0, , "alpha", 3], (() => Promise.all([c.e(846), c.e(6914), c.e(4947), c.e(3203), c.e(6e3), c.e(6956), c.e(4629), c.e(8157), c.e(988), c.e(2230)]).then((() => () => c(17696))))),
         59601: () => s("default", "@jupyterlab/theme-dark-extension", [1, 3, 4, 8], (() => Promise.all([c.e(6956), c.e(3811)]).then((() => () => c(21058))))),
         99661: () => s("default", "@jupyterlab/theme-light-extension", [1, 3, 4, 8], (() => Promise.all([c.e(6956), c.e(7469)]).then((() => () => c(60275))))),
         17021: () => s("default", "@jupyter-widgets/controls", [1, 5, 0, 1], (() => Promise.all([c.e(3851), c.e(8695), c.e(4812)]).then((() => () => c(53851))))),
         7531: () => s("default", "@jupyterlite/server-extension", [2, 0, 1, 0], (() => Promise.all([c.e(6111), c.e(4530), c.e(3203), c.e(7631), c.e(3862)]).then((() => () => c(24530)))))
-    }, h = {
+    }, p = {
         49: [40049],
         319: [90319],
         568: [2132, 86086],
         988: [70988],
         1514: [1514],
         1876: [91876],
         2051: [42051],
@@ -265,56 +268,60 @@
         5320: [5320],
         5490: [15490],
         5820: [34013, 49943],
         5918: [35918],
         6e3: [36e3],
         6088: [56088],
         6678: [10409, 70190],
+        6852: [92233],
         6956: [56956],
+        6968: [26968],
         7505: [97505],
         7531: [7531],
         7631: [7631],
         7651: [67651],
         7782: [37782],
         7968: [77968],
+        8157: [48157],
         8695: [78695],
         8930: [68930],
+        8971: [8971],
         8987: [9961, 22312, 59601, 99661],
         9098: [89098],
         9110: [59110],
         9939: [49939]
     }, c.f.consumes = (e, t) => {
-        c.o(h, e) && h[e].forEach((e => {
+        c.o(p, e) && p[e].forEach((e => {
             if (c.o(m, e)) return t.push(m[e]);
             var l = t => {
                     m[e] = 0, c.m[e] = l => {
                         delete c.c[e], l.exports = t()
                     }
                 },
                 r = t => {
                     delete m[e], c.m[e] = l => {
                         throw delete c.c[e], t
                     }
                 };
             try {
-                var a = p[e]();
+                var a = h[e]();
                 a.then ? t.push(m[e] = a.then(l).catch(r)) : l(a)
             } catch (e) {
                 r(e)
             }
         }))
     }, (() => {
         var e = {
             9749: 0
         };
         c.f.j = (t, l) => {
             var r = c.o(e, t) ? e[t] : void 0;
             if (0 !== r)
                 if (r) l.push(r[2]);
-                else if (/^(2(051|233|299|886)|3(19(|8)|86[02]|203)|4(6(27|29|43)|456|812|863|9|947)|5((23|6|91)8|(32|49|82)0)|6(000|088|678|956)|7((53|63|65)1|505|782|968)|8(695|930|987)|9(098|110|88|939)|1514|1876)$/.test(t)) e[t] = 0;
+                else if (/^(2(051|233|299|886)|3(19(|8)|86[02]|203)|4(6(27|29|43)|456|812|863|9|947)|5((23|6|91)8|(32|49|82)0)|6((08|67|96)8|000|956)|7((53|63|65)1|505|782|968)|8(9(30|71|87)|157|695)|9(098|110|88|939)|1514|1876)$/.test(t)) e[t] = 0;
             else {
                 var a = new Promise(((l, a) => r = e[t] = [l, a]));
                 l.push(r[2] = a);
                 var n = c.p + c.u(t),
                     o = new Error;
                 c.l(n, (l => {
                     if (c.o(e, t) && (0 !== (r = e[t]) && (e[t] = void 0), r)) {
```

### Comparing `voici-0.4.3/voici/static/build/voici.js` & `voici-0.4.4/voici/static/build/voici.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,13 @@
 var _JUPYTERLAB;
 (() => {
     var e, t, l, r, a, n, o, i, u, s, m, h, p, d = {
             37559: (e, t, l) => {
                 "use strict";
-                Promise.all([l.e(2233), l.e(2051), l.e(9110), l.e(7782), l.e(2299), l.e(4627), l.e(3198), l.e(7651), l.e(5238), l.e(49), l.e(4456), l.e(7631), l.e(5918), l.e(8987), l.e(5474)]).then(l.bind(l, 65474))
+                Promise.all([l.e(4947), l.e(2233), l.e(3203), l.e(6e3), l.e(2051), l.e(4629), l.e(8157), l.e(9110), l.e(7782), l.e(8695), l.e(2299), l.e(4812), l.e(4627), l.e(2886), l.e(3198), l.e(7651), l.e(6968), l.e(3860), l.e(8971), l.e(5238), l.e(49), l.e(4456), l.e(7631), l.e(5918), l.e(8987), l.e(7002)]).then(l.bind(l, 47002))
             },
             68444: (e, t, l) => {
                 l.p = function(e) {
                     let t = Object.create(null);
                     if ("undefined" != typeof document && document) {
                         const e = document.getElementById("jupyter-config-data");
                         e && (t = JSON.parse(e.textContent || "{}"))
@@ -106,15 +106,15 @@
                         (!i || !i.loaded && (!r != !i.eager ? r : o > i.from)) && (a[t] = {
                             get: l,
                             from: o,
                             eager: !!r
                         })
                     },
                     u = [];
-                return "default" === l && (i("@jupyter-widgets/base", "6.0.4", (() => Promise.all([c.e(8291), c.e(9900), c.e(2233), c.e(2051), c.e(8695)]).then((() => () => c(9900))))), i("@jupyter-widgets/controls", "5.0.5", (() => Promise.all([c.e(8291), c.e(3851), c.e(4947), c.e(3203), c.e(2051), c.e(8695), c.e(4812), c.e(7651), c.e(6587)]).then((() => () => c(53851))))), i("@jupyter-widgets/jupyterlab-manager", "5.0.7", (() => Promise.all([c.e(8291), c.e(1672), c.e(9727), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(4629), c.e(988), c.e(2299), c.e(8930), c.e(3198), c.e(7651), c.e(49), c.e(5320), c.e(6678), c.e(2266)]).then((() => () => c(9727))))), i("@jupyter-widgets/output", "6.0.4", (() => Promise.all([c.e(7651), c.e(1100)]).then((() => () => c(21100))))), i("@jupyterlab/application", "3.6.3", (() => Promise.all([c.e(2361), c.e(6219), c.e(9780), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(4629), c.e(9110), c.e(7782), c.e(4643), c.e(988), c.e(2299), c.e(8695), c.e(1514), c.e(7968)]).then((() => () => c(79780))))), i("@jupyterlab/apputils-extension", "3.6.3", (() => Promise.all([c.e(2361), c.e(6770), c.e(846), c.e(4939), c.e(7066), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(4629), c.e(9110), c.e(7782), c.e(4643), c.e(7505), c.e(988), c.e(1514), c.e(7968), c.e(4627), c.e(8930), c.e(5238), c.e(5320)]).then((() => () => c(97066))))), i("@jupyterlab/apputils", "3.6.3", (() => Promise.all([c.e(2361), c.e(846), c.e(1672), c.e(339), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(4629), c.e(9110), c.e(4643), c.e(7505), c.e(988), c.e(8695), c.e(1514), c.e(4812), c.e(4627), c.e(8930), c.e(1732)]).then((() => () => c(90339))))), i("@jupyterlab/coreutils", "5.5.3", (() => Promise.all([c.e(5952), c.e(286), c.e(4947), c.e(2233), c.e(6616)]).then((() => () => c(20286))))), i("@jupyterlab/coreutils", "5.5.3", (() => Promise.all([c.e(5952), c.e(2359), c.e(4947), c.e(2233), c.e(709)]).then((() => () => c(62359))))), i("@jupyterlab/coreutils", "5.5.3", (() => Promise.all([c.e(5952), c.e(53), c.e(4947), c.e(2233), c.e(6178)]).then((() => () => c(70053))))), i("@jupyterlab/coreutils", "5.5.3", (() => Promise.all([c.e(5952), c.e(3922), c.e(4947), c.e(2233), c.e(2630)]).then((() => () => c(13922))))), i("@jupyterlab/coreutils", "5.5.3", (() => Promise.all([c.e(5952), c.e(596), c.e(4947), c.e(2233), c.e(6614)]).then((() => () => c(20596))))), i("@jupyterlab/coreutils", "5.5.3", (() => Promise.all([c.e(5952), c.e(1980), c.e(4947), c.e(2233), c.e(1023)]).then((() => () => c(1980))))), i("@jupyterlab/coreutils", "5.5.3", (() => Promise.all([c.e(5952), c.e(4896), c.e(4947), c.e(2233), c.e(6790)]).then((() => () => c(4896))))), i("@jupyterlab/coreutils", "5.6.3", (() => Promise.all([c.e(5952), c.e(103), c.e(4947), c.e(2233), c.e(3086)]).then((() => () => c(60103))))), i("@jupyterlab/coreutils", "5.6.3", (() => Promise.all([c.e(5952), c.e(2950), c.e(4947), c.e(2233), c.e(1667)]).then((() => () => c(42950))))), i("@jupyterlab/coreutils", "5.6.3", (() => Promise.all([c.e(5952), c.e(3251), c.e(4947), c.e(2233), c.e(7623)]).then((() => () => c(53251))))), i("@jupyterlab/docregistry", "3.6.3", (() => Promise.all([c.e(2361), c.e(6770), c.e(4939), c.e(9112), c.e(4875), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(9110), c.e(7782), c.e(4643), c.e(7505), c.e(2299), c.e(8695), c.e(6088), c.e(1876)]).then((() => () => c(74875))))), i("@jupyterlab/json-extension", "3.6.3", (() => Promise.all([c.e(5950), c.e(2233), c.e(6956), c.e(2051), c.e(7782), c.e(4643), c.e(7505), c.e(4627)]).then((() => () => c(45950))))), i("@jupyterlab/logconsole", "3.6.3", (() => Promise.all([c.e(9339), c.e(4947), c.e(2233), c.e(6956), c.e(2051), c.e(2299), c.e(3198)]).then((() => () => c(99339))))), i("@jupyterlab/mainmenu", "3.6.3", (() => Promise.all([c.e(2233), c.e(3203), c.e(2051), c.e(4643), c.e(1581)]).then((() => () => c(21581))))), i("@jupyterlab/markdownviewer-extension", "3.6.3", (() => Promise.all([c.e(2233), c.e(6956), c.e(2051), c.e(9110), c.e(7782), c.e(2299), c.e(7968), c.e(8930), c.e(5238), c.e(4382)]).then((() => () => c(54382))))), i("@jupyterlab/mathjax2-extension", "3.6.3", (() => Promise.all([c.e(2233), c.e(9110), c.e(2299), c.e(6976)]).then((() => () => c(66976))))), i("@jupyterlab/nbformat", "3.6.3", (() => Promise.all([c.e(2233), c.e(3655)]).then((() => () => c(63655))))), i("@jupyterlab/notebook", "3.6.3", (() => Promise.all([c.e(2361), c.e(6770), c.e(4939), c.e(9112), c.e(8085), c.e(4977), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(4629), c.e(9110), c.e(7782), c.e(4643), c.e(7505), c.e(988), c.e(2299), c.e(8695), c.e(4812), c.e(7968), c.e(6088), c.e(1876), c.e(3198), c.e(9939), c.e(2886), c.e(3860)]).then((() => () => c(24977))))), i("@jupyterlab/outputarea", "3.6.3", (() => Promise.all([c.e(1432), c.e(4947), c.e(2233), c.e(3203), c.e(2051), c.e(4629), c.e(7782), c.e(988), c.e(2299), c.e(9939)]).then((() => () => c(31432))))), i("@jupyterlab/rendermime-extension", "3.6.3", (() => Promise.all([c.e(2233), c.e(6956), c.e(7782), c.e(2299), c.e(5985)]).then((() => () => c(85985))))), i("@jupyterlab/rendermime", "3.6.3", (() => Promise.all([c.e(2361), c.e(6770), c.e(4939), c.e(9112), c.e(8085), c.e(2075), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(9110), c.e(7782), c.e(4643), c.e(7505), c.e(8695), c.e(6088), c.e(1876), c.e(9939)]).then((() => () => c(82075))))), i("@jupyterlab/services", "6.5.3", (() => Promise.all([c.e(2361), c.e(846), c.e(7560), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(4629), c.e(9098), c.e(3008)]).then((() => () => c(17560))))), i("@jupyterlab/services", "6.5.3", (() => Promise.all([c.e(2361), c.e(74), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(4629), c.e(5490), c.e(9320)]).then((() => () => c(80074))))), i("@jupyterlab/services", "6.6.3", (() => Promise.all([c.e(2361), c.e(846), c.e(6914), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(4629), c.e(9110), c.e(1497)]).then((() => () => c(16914))))), i("@jupyterlab/settingregistry", "3.6.3", (() => Promise.all([c.e(6111), c.e(9513), c.e(4947), c.e(2233), c.e(6e3), c.e(1514)]).then((() => () => c(69513))))), i("@jupyterlab/theme-dark-extension", "3.6.3", (() => Promise.all([c.e(6956), c.e(7782), c.e(1058)]).then((() => () => c(21058))))), i("@jupyterlab/theme-light-extension", "3.6.3", (() => Promise.all([c.e(6956), c.e(7782), c.e(275)]).then((() => () => c(60275))))), i("@jupyterlab/translation", "3.6.3", (() => Promise.all([c.e(846), c.e(2322), c.e(4947), c.e(2233), c.e(4629), c.e(9110), c.e(988)]).then((() => () => c(29513))))), i("@jupyterlab/ui-components", "3.6.3", (() => Promise.all([c.e(6770), c.e(4963), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(9110), c.e(7505), c.e(4627), c.e(2886)]).then((() => () => c(74963))))), i("@jupyterlite/contents", "0.1.0", (() => Promise.all([c.e(9757), c.e(2233), c.e(9110)]).then((() => () => c(9757))))), i("@jupyterlite/iframe-extension", "0.1.0", (() => Promise.all([c.e(2233), c.e(2051), c.e(6527)]).then((() => () => c(26527))))), i("@jupyterlite/kernel", "0.1.0", (() => Promise.all([c.e(9988), c.e(3693), c.e(4947), c.e(2233), c.e(5820)]).then((() => () => c(83693))))), i("@jupyterlite/server-extension", "0.1.0", (() => Promise.all([c.e(6111), c.e(4530), c.e(2233), c.e(3203), c.e(4456), c.e(7631), c.e(3862)]).then((() => () => c(24530))))), i("@jupyterlite/server", "0.1.0", (() => Promise.all([c.e(6219), c.e(9988), c.e(4947), c.e(2233), c.e(2051), c.e(1514), c.e(568), c.e(3256)]).then((() => () => c(93256))))), i("@lumino/algorithm", "1.9.2", (() => c.e(9060).then((() => () => c(69060))))), i("@lumino/algorithm", "2.0.0", (() => c.e(9807).then((() => () => c(89807))))), i("@lumino/commands", "1.21.1", (() => Promise.all([c.e(2687), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(4812)]).then((() => () => c(62687))))), i("@lumino/coreutils", "1.12.1", (() => c.e(1770).then((() => () => c(71770))))), i("@lumino/coreutils", "2.1.0", (() => c.e(4259).then((() => () => c(4259))))), i("@lumino/disposable", "1.10.4", (() => Promise.all([c.e(4947), c.e(3203), c.e(2488)]).then((() => () => c(72488))))), i("@lumino/domutils", "1.8.2", (() => c.e(5403).then((() => () => c(85403))))), i("@lumino/dragdrop", "1.14.5", (() => Promise.all([c.e(8809), c.e(6e3)]).then((() => () => c(38809))))), i("@lumino/messaging", "1.10.3", (() => Promise.all([c.e(3316), c.e(3203)]).then((() => () => c(73316))))), i("@lumino/properties", "1.8.2", (() => c.e(3312).then((() => () => c(73312))))), i("@lumino/signaling", "1.11.1", (() => Promise.all([c.e(3203), c.e(4629), c.e(5445)]).then((() => () => c(75445))))), i("@lumino/signaling", "2.1.0", (() => Promise.all([c.e(6088), c.e(319), c.e(7003)]).then((() => () => c(27003))))), i("@lumino/virtualdom", "1.14.3", (() => Promise.all([c.e(1053), c.e(3203)]).then((() => () => c(1053))))), i("@lumino/widgets", "1.37.2", (() => Promise.all([c.e(450), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(4629), c.e(8695), c.e(1514), c.e(4812), c.e(2886), c.e(3860)]).then((() => () => c(90450))))), i("@voila-dashboards/voila", "0.5.0-alpha.3", (() => Promise.all([c.e(2361), c.e(846), c.e(6914), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(4629), c.e(9110), c.e(988), c.e(2299), c.e(7651), c.e(5238), c.e(5918), c.e(3504)]).then((() => () => c(17696))))), i("react-dom", "17.0.2", (() => Promise.all([c.e(8316), c.e(7505)]).then((() => () => c(28316))))), i("react", "17.0.2", (() => c.e(2784).then((() => () => c(2784)))))), e[l] = u.length ? Promise.all(u).then((() => e[l] = 1)) : 1
+                return "default" === l && (i("@jupyter-widgets/base", "6.0.4", (() => Promise.all([c.e(8291), c.e(9900), c.e(2233), c.e(2051), c.e(8695)]).then((() => () => c(9900))))), i("@jupyter-widgets/controls", "5.0.5", (() => Promise.all([c.e(8291), c.e(3851), c.e(4947), c.e(3203), c.e(2051), c.e(8695), c.e(4812), c.e(7651), c.e(6587)]).then((() => () => c(53851))))), i("@jupyter-widgets/jupyterlab-manager", "5.0.7", (() => Promise.all([c.e(8291), c.e(1672), c.e(9727), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(4629), c.e(988), c.e(2299), c.e(8930), c.e(3198), c.e(7651), c.e(49), c.e(5320), c.e(6678), c.e(2266)]).then((() => () => c(9727))))), i("@jupyter-widgets/output", "6.0.4", (() => Promise.all([c.e(7651), c.e(1100)]).then((() => () => c(21100))))), i("@jupyterlab/application", "3.6.3", (() => Promise.all([c.e(9780), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(4629), c.e(8157), c.e(9110), c.e(7782), c.e(8695), c.e(4643), c.e(988), c.e(2299), c.e(7968), c.e(8971)]).then((() => () => c(79780))))), i("@jupyterlab/apputils-extension", "3.6.3", (() => Promise.all([c.e(6770), c.e(846), c.e(4939), c.e(7066), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(4629), c.e(8157), c.e(9110), c.e(7782), c.e(4643), c.e(7505), c.e(988), c.e(1514), c.e(7968), c.e(4627), c.e(8930), c.e(5238), c.e(5320)]).then((() => () => c(97066))))), i("@jupyterlab/apputils", "3.6.3", (() => Promise.all([c.e(846), c.e(1672), c.e(339), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(4629), c.e(8157), c.e(9110), c.e(8695), c.e(4643), c.e(7505), c.e(988), c.e(4812), c.e(1514), c.e(4627), c.e(8930), c.e(1732)]).then((() => () => c(90339))))), i("@jupyterlab/coreutils", "5.5.3", (() => Promise.all([c.e(5952), c.e(286), c.e(4947), c.e(2233), c.e(6616)]).then((() => () => c(20286))))), i("@jupyterlab/coreutils", "5.5.3", (() => Promise.all([c.e(5952), c.e(2359), c.e(4947), c.e(2233), c.e(709)]).then((() => () => c(62359))))), i("@jupyterlab/coreutils", "5.5.3", (() => Promise.all([c.e(5952), c.e(53), c.e(4947), c.e(2233), c.e(6178)]).then((() => () => c(70053))))), i("@jupyterlab/coreutils", "5.5.3", (() => Promise.all([c.e(5952), c.e(3922), c.e(4947), c.e(2233), c.e(2630)]).then((() => () => c(13922))))), i("@jupyterlab/coreutils", "5.5.3", (() => Promise.all([c.e(5952), c.e(596), c.e(4947), c.e(2233), c.e(6614)]).then((() => () => c(20596))))), i("@jupyterlab/coreutils", "5.5.3", (() => Promise.all([c.e(5952), c.e(1980), c.e(4947), c.e(2233), c.e(1023)]).then((() => () => c(1980))))), i("@jupyterlab/coreutils", "5.5.3", (() => Promise.all([c.e(5952), c.e(4896), c.e(4947), c.e(2233), c.e(6790)]).then((() => () => c(4896))))), i("@jupyterlab/coreutils", "5.6.3", (() => Promise.all([c.e(5952), c.e(103), c.e(4947), c.e(2233), c.e(3086)]).then((() => () => c(60103))))), i("@jupyterlab/coreutils", "5.6.3", (() => Promise.all([c.e(5952), c.e(2950), c.e(4947), c.e(2233), c.e(1667)]).then((() => () => c(42950))))), i("@jupyterlab/coreutils", "5.6.3", (() => Promise.all([c.e(5952), c.e(3251), c.e(4947), c.e(2233), c.e(7623)]).then((() => () => c(53251))))), i("@jupyterlab/docregistry", "3.6.3", (() => Promise.all([c.e(6770), c.e(4939), c.e(9112), c.e(4875), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(8157), c.e(9110), c.e(7782), c.e(8695), c.e(4643), c.e(7505), c.e(2299), c.e(6088), c.e(1876)]).then((() => () => c(74875))))), i("@jupyterlab/json-extension", "3.6.3", (() => Promise.all([c.e(5950), c.e(2233), c.e(6956), c.e(2051), c.e(7782), c.e(4643), c.e(7505), c.e(4627)]).then((() => () => c(45950))))), i("@jupyterlab/logconsole", "3.6.3", (() => Promise.all([c.e(9339), c.e(4947), c.e(2233), c.e(6956), c.e(2051), c.e(2299), c.e(3198)]).then((() => () => c(99339))))), i("@jupyterlab/mainmenu", "3.6.3", (() => Promise.all([c.e(2233), c.e(3203), c.e(2051), c.e(4643), c.e(1581)]).then((() => () => c(21581))))), i("@jupyterlab/markdownviewer-extension", "3.6.3", (() => Promise.all([c.e(2233), c.e(6956), c.e(2051), c.e(9110), c.e(7782), c.e(2299), c.e(7968), c.e(8930), c.e(5238), c.e(4382)]).then((() => () => c(54382))))), i("@jupyterlab/mathjax2-extension", "3.6.3", (() => Promise.all([c.e(2233), c.e(9110), c.e(2299), c.e(6976)]).then((() => () => c(66976))))), i("@jupyterlab/nbformat", "3.6.3", (() => Promise.all([c.e(2233), c.e(3655)]).then((() => () => c(63655))))), i("@jupyterlab/notebook", "3.6.3", (() => Promise.all([c.e(6770), c.e(4939), c.e(9112), c.e(8085), c.e(4977), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(4629), c.e(8157), c.e(9110), c.e(7782), c.e(8695), c.e(4643), c.e(7505), c.e(988), c.e(2299), c.e(4812), c.e(7968), c.e(6088), c.e(2886), c.e(1876), c.e(3198), c.e(9939), c.e(3860)]).then((() => () => c(24977))))), i("@jupyterlab/outputarea", "3.6.3", (() => Promise.all([c.e(1432), c.e(4947), c.e(2233), c.e(3203), c.e(2051), c.e(4629), c.e(7782), c.e(988), c.e(2299), c.e(9939)]).then((() => () => c(31432))))), i("@jupyterlab/rendermime-extension", "3.6.3", (() => Promise.all([c.e(2233), c.e(6956), c.e(7782), c.e(2299), c.e(5985)]).then((() => () => c(85985))))), i("@jupyterlab/rendermime", "3.6.3", (() => Promise.all([c.e(6770), c.e(4939), c.e(9112), c.e(8085), c.e(2075), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(8157), c.e(9110), c.e(7782), c.e(8695), c.e(4643), c.e(7505), c.e(6088), c.e(1876), c.e(9939)]).then((() => () => c(82075))))), i("@jupyterlab/services", "6.5.3", (() => Promise.all([c.e(846), c.e(7560), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(4629), c.e(8157), c.e(9098), c.e(3008)]).then((() => () => c(17560))))), i("@jupyterlab/services", "6.5.3", (() => Promise.all([c.e(74), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(4629), c.e(8157), c.e(5490), c.e(9320)]).then((() => () => c(80074))))), i("@jupyterlab/services", "6.6.3", (() => Promise.all([c.e(846), c.e(6914), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(4629), c.e(8157), c.e(9110), c.e(1497)]).then((() => () => c(16914))))), i("@jupyterlab/settingregistry", "3.6.3", (() => Promise.all([c.e(6111), c.e(9513), c.e(4947), c.e(2233), c.e(6e3), c.e(1514)]).then((() => () => c(69513))))), i("@jupyterlab/theme-dark-extension", "3.6.3", (() => Promise.all([c.e(6956), c.e(7782), c.e(1058)]).then((() => () => c(21058))))), i("@jupyterlab/theme-light-extension", "3.6.3", (() => Promise.all([c.e(6956), c.e(7782), c.e(275)]).then((() => () => c(60275))))), i("@jupyterlab/translation", "3.6.3", (() => Promise.all([c.e(846), c.e(2322), c.e(4947), c.e(2233), c.e(4629), c.e(9110), c.e(988)]).then((() => () => c(29513))))), i("@jupyterlab/ui-components", "3.6.3", (() => Promise.all([c.e(6770), c.e(4963), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(9110), c.e(7505), c.e(4627), c.e(2886)]).then((() => () => c(74963))))), i("@jupyterlite/contents", "0.1.0", (() => Promise.all([c.e(9757), c.e(2233), c.e(9110)]).then((() => () => c(9757))))), i("@jupyterlite/iframe-extension", "0.1.0", (() => Promise.all([c.e(2233), c.e(2051), c.e(6527)]).then((() => () => c(26527))))), i("@jupyterlite/kernel", "0.1.0", (() => Promise.all([c.e(9988), c.e(3693), c.e(4947), c.e(2233), c.e(5820)]).then((() => () => c(83693))))), i("@jupyterlite/server-extension", "0.1.0", (() => Promise.all([c.e(6111), c.e(4530), c.e(2233), c.e(3203), c.e(4456), c.e(7631), c.e(3862)]).then((() => () => c(24530))))), i("@jupyterlite/server", "0.1.0", (() => Promise.all([c.e(9988), c.e(4947), c.e(2233), c.e(8971), c.e(568), c.e(3256)]).then((() => () => c(93256))))), i("@lumino/algorithm", "1.9.2", (() => c.e(9060).then((() => () => c(69060))))), i("@lumino/algorithm", "2.0.0", (() => c.e(9807).then((() => () => c(89807))))), i("@lumino/application", "1.31.4", (() => Promise.all([c.e(6219), c.e(2233), c.e(2051), c.e(1514)]).then((() => () => c(76219))))), i("@lumino/commands", "1.21.1", (() => Promise.all([c.e(2687), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(4812), c.e(6968)]).then((() => () => c(62687))))), i("@lumino/coreutils", "1.12.1", (() => c.e(1770).then((() => () => c(71770))))), i("@lumino/coreutils", "2.1.0", (() => c.e(4259).then((() => () => c(4259))))), i("@lumino/datagrid", "0.36.9", (() => Promise.all([c.e(8921), c.e(4947), c.e(2233), c.e(3203), c.e(2051), c.e(8695), c.e(4812), c.e(6968), c.e(3860)]).then((() => () => c(28921))))), i("@lumino/disposable", "1.10.4", (() => Promise.all([c.e(4947), c.e(3203), c.e(2488)]).then((() => () => c(72488))))), i("@lumino/domutils", "1.8.2", (() => c.e(5403).then((() => () => c(85403))))), i("@lumino/dragdrop", "1.14.5", (() => Promise.all([c.e(8809), c.e(6e3)]).then((() => () => c(38809))))), i("@lumino/keyboard", "1.8.2", (() => c.e(8102).then((() => () => c(34938))))), i("@lumino/messaging", "1.10.3", (() => Promise.all([c.e(3316), c.e(3203)]).then((() => () => c(73316))))), i("@lumino/polling", "1.11.4", (() => Promise.all([c.e(2361), c.e(4947), c.e(2233)]).then((() => () => c(82361))))), i("@lumino/properties", "1.8.2", (() => c.e(3312).then((() => () => c(73312))))), i("@lumino/signaling", "1.11.1", (() => Promise.all([c.e(3203), c.e(4629), c.e(5445)]).then((() => () => c(75445))))), i("@lumino/signaling", "2.1.0", (() => Promise.all([c.e(6088), c.e(319), c.e(7003)]).then((() => () => c(27003))))), i("@lumino/virtualdom", "1.14.3", (() => Promise.all([c.e(1053), c.e(3203)]).then((() => () => c(1053))))), i("@lumino/widgets", "1.37.2", (() => Promise.all([c.e(450), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(4629), c.e(8695), c.e(4812), c.e(1514), c.e(2886), c.e(6968), c.e(3860)]).then((() => () => c(90450))))), i("@voila-dashboards/voila", "0.5.0-alpha.3", (() => Promise.all([c.e(846), c.e(6914), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(4629), c.e(8157), c.e(9110), c.e(988), c.e(2299), c.e(7651), c.e(5238), c.e(5918), c.e(3504)]).then((() => () => c(17696))))), i("react-dom", "17.0.2", (() => Promise.all([c.e(8316), c.e(7505)]).then((() => () => c(28316))))), i("react", "17.0.2", (() => c.e(2784).then((() => () => c(2784)))))), e[l] = u.length ? Promise.all(u).then((() => e[l] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         c.g.importScripts && (e = c.g.location + "");
         var t = c.g.document;
         if (!e && t && (t.currentScript && (e = t.currentScript.src), !e)) {
@@ -182,68 +182,72 @@
     }, u = e => (e.loaded = 1, e.get()), s = (e => function(t, l, r, a) {
         var n = c.I(t);
         return n && n.then ? n.then(e.bind(e, t, c.S[t], l, r, a)) : e(0, c.S[t], l, r, a)
     })(((e, t, l, r, a) => {
         var n = t && c.o(t, l) && i(t, l, r);
         return n ? u(n) : a()
     })), m = {}, h = {
+        4947: () => s("default", "@lumino/signaling", [1, 1, 7, 2], (() => Promise.all([c.e(3203), c.e(4629), c.e(5445)]).then((() => () => c(75445))))),
         92233: () => s("default", "@lumino/coreutils", [1, 1, 8, 2], (() => c.e(1770).then((() => () => c(71770))))),
-        42051: () => s("default", "@lumino/widgets", [1, 1, 26, 2], (() => Promise.all([c.e(450), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(4629), c.e(8695), c.e(1514), c.e(4812), c.e(2886), c.e(3860)]).then((() => () => c(90450))))),
+        23203: () => s("default", "@lumino/algorithm", [1, 1, 6, 2], (() => c.e(9060).then((() => () => c(69060))))),
+        36e3: () => s("default", "@lumino/disposable", [1, 1, 7, 2], (() => Promise.all([c.e(4947), c.e(3203), c.e(2488)]).then((() => () => c(72488))))),
+        42051: () => s("default", "@lumino/widgets", [1, 1, 26, 2], (() => Promise.all([c.e(450), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(4629), c.e(8695), c.e(4812), c.e(1514), c.e(2886), c.e(6968), c.e(3860)]).then((() => () => c(90450))))),
+        24629: () => s("default", "@lumino/properties", [1, 1, 5, 2], (() => c.e(3312).then((() => () => c(73312))))),
+        48157: () => s("default", "@lumino/polling", [1, 1, 11, 4], (() => c.e(2361).then((() => () => c(82361))))),
         59110: () => s("default", "@jupyterlab/coreutils", [1, 5, 0, 0], (() => Promise.all([c.e(5952), c.e(103), c.e(4947), c.e(6196)]).then((() => () => c(60103))))),
-        37782: () => s("default", "@jupyterlab/apputils", [1, 3, 0, 0], (() => Promise.all([c.e(2361), c.e(846), c.e(1672), c.e(339), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(4629), c.e(9110), c.e(4643), c.e(7505), c.e(988), c.e(8695), c.e(1514), c.e(4812), c.e(4627), c.e(8930), c.e(1732)]).then((() => () => c(90339))))),
-        12299: () => s("default", "@jupyterlab/rendermime", [1, 3, 0, 0], (() => Promise.all([c.e(2361), c.e(6770), c.e(4939), c.e(9112), c.e(8085), c.e(2075), c.e(4947), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(9110), c.e(7782), c.e(4643), c.e(7505), c.e(8695), c.e(6088), c.e(1876), c.e(9939)]).then((() => () => c(82075))))),
+        37782: () => s("default", "@jupyterlab/apputils", [1, 3, 0, 0], (() => Promise.all([c.e(846), c.e(1672), c.e(339), c.e(4947), c.e(2233), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(4629), c.e(8157), c.e(9110), c.e(8695), c.e(4643), c.e(7505), c.e(988), c.e(4812), c.e(1514), c.e(4627), c.e(8930), c.e(1732)]).then((() => () => c(90339))))),
+        78695: () => s("default", "@lumino/messaging", [1, 1, 7, 2], (() => Promise.all([c.e(3316), c.e(3203)]).then((() => () => c(73316))))),
+        12299: () => s("default", "@jupyterlab/rendermime", [1, 3, 0, 0], (() => Promise.all([c.e(6770), c.e(4939), c.e(9112), c.e(8085), c.e(2075), c.e(4947), c.e(3203), c.e(6e3), c.e(6956), c.e(2051), c.e(8157), c.e(9110), c.e(7782), c.e(8695), c.e(4643), c.e(7505), c.e(6088), c.e(1876), c.e(9939)]).then((() => () => c(82075))))),
+        94812: () => s("default", "@lumino/domutils", [1, 1, 5, 2], (() => c.e(5403).then((() => () => c(85403))))),
         24627: () => s("default", "react-dom", [1, 17, 0, 1], (() => Promise.all([c.e(8316), c.e(7505)]).then((() => () => c(28316))))),
+        32886: () => s("default", "@lumino/virtualdom", [1, 1, 11, 2], (() => c.e(1053).then((() => () => c(1053))))),
         73198: () => s("default", "@jupyterlab/outputarea", [1, 3, 0, 0], (() => Promise.all([c.e(1432), c.e(4947), c.e(3203), c.e(4629), c.e(7782), c.e(988), c.e(9939)]).then((() => () => c(31432))))),
         67651: () => s("default", "@jupyter-widgets/base", [1, 6, 0, 1], (() => Promise.all([c.e(8291), c.e(9900), c.e(2233), c.e(2051), c.e(8695)]).then((() => () => c(9900))))),
-        75238: () => s("default", "@jupyterlab/application", [1, 3, 0, 0], (() => Promise.all([c.e(2361), c.e(6219), c.e(9780), c.e(4947), c.e(3203), c.e(6e3), c.e(6956), c.e(4629), c.e(7782), c.e(4643), c.e(988), c.e(2299), c.e(8695), c.e(1514), c.e(7968)]).then((() => () => c(79780))))),
-        40049: () => s("default", "@jupyterlab/notebook", [1, 3, 0, 0], (() => Promise.all([c.e(2361), c.e(6770), c.e(4939), c.e(9112), c.e(8085), c.e(4977), c.e(4947), c.e(3203), c.e(6e3), c.e(6956), c.e(4629), c.e(9110), c.e(7782), c.e(4643), c.e(7505), c.e(988), c.e(8695), c.e(4812), c.e(7968), c.e(6088), c.e(1876), c.e(9939), c.e(2886), c.e(3860)]).then((() => () => c(24977))))),
-        94456: () => s("default", "@jupyterlite/server", [2, 0, 1, 0], (() => Promise.all([c.e(6219), c.e(9988), c.e(4947), c.e(2051), c.e(1514), c.e(568), c.e(6856)]).then((() => () => c(93256))))),
+        26968: () => s("default", "@lumino/keyboard", [1, 1, 8, 0], (() => c.e(8102).then((() => () => c(34938))))),
+        3860: () => s("default", "@lumino/dragdrop", [1, 1, 10, 2], (() => Promise.all([c.e(8809), c.e(6e3)]).then((() => () => c(38809))))),
+        8971: () => s("default", "@lumino/application", [1, 1, 31, 3], (() => Promise.all([c.e(6219), c.e(2051), c.e(1514)]).then((() => () => c(76219))))),
+        75238: () => s("default", "@jupyterlab/application", [1, 3, 0, 0], (() => Promise.all([c.e(9780), c.e(4947), c.e(3203), c.e(6e3), c.e(6956), c.e(4629), c.e(8157), c.e(7782), c.e(8695), c.e(4643), c.e(988), c.e(2299), c.e(7968), c.e(8971)]).then((() => () => c(79780))))),
+        40049: () => s("default", "@jupyterlab/notebook", [1, 3, 0, 0], (() => Promise.all([c.e(6770), c.e(4939), c.e(9112), c.e(8085), c.e(4977), c.e(4947), c.e(3203), c.e(6e3), c.e(6956), c.e(4629), c.e(8157), c.e(9110), c.e(7782), c.e(8695), c.e(4643), c.e(7505), c.e(988), c.e(4812), c.e(7968), c.e(6088), c.e(2886), c.e(1876), c.e(9939), c.e(3860)]).then((() => () => c(24977))))),
+        94456: () => s("default", "@jupyterlite/server", [2, 0, 1, 0], (() => Promise.all([c.e(9988), c.e(4947), c.e(8971), c.e(568), c.e(6856)]).then((() => () => c(93256))))),
         7631: () => s("default", "@jupyterlite/kernel", [2, 0, 1, 0], (() => Promise.all([c.e(9988), c.e(3693), c.e(4947), c.e(5820)]).then((() => () => c(83693))))),
         35918: () => s("default", "@jupyter-widgets/jupyterlab-manager", [1, 5, 0, 3], (() => Promise.all([c.e(8291), c.e(1672), c.e(9727), c.e(4947), c.e(3203), c.e(6e3), c.e(6956), c.e(4629), c.e(988), c.e(8930), c.e(3198), c.e(49), c.e(5320), c.e(6678), c.e(2516)]).then((() => () => c(9727))))),
-        9961: () => s("default", "@jupyterlab/apputils-extension", [1, 3, 4, 8], (() => Promise.all([c.e(2361), c.e(6770), c.e(846), c.e(4939), c.e(7066), c.e(4947), c.e(3203), c.e(6e3), c.e(6956), c.e(4629), c.e(4643), c.e(7505), c.e(988), c.e(1514), c.e(7968), c.e(4627), c.e(8930), c.e(5320)]).then((() => () => c(97066))))),
-        22312: () => s("default", "@voila-dashboards/voila", [2, 0, 5, 0, , "alpha", 3], (() => Promise.all([c.e(2361), c.e(846), c.e(6914), c.e(4947), c.e(3203), c.e(6e3), c.e(6956), c.e(4629), c.e(988), c.e(2230)]).then((() => () => c(17696))))),
+        9961: () => s("default", "@jupyterlab/apputils-extension", [1, 3, 4, 8], (() => Promise.all([c.e(6770), c.e(846), c.e(4939), c.e(7066), c.e(4947), c.e(3203), c.e(6e3), c.e(6956), c.e(4629), c.e(8157), c.e(4643), c.e(7505), c.e(988), c.e(1514), c.e(7968), c.e(4627), c.e(8930), c.e(5320)]).then((() => () => c(97066))))),
+        22312: () => s("default", "@voila-dashboards/voila", [2, 0, 5, 0, , "alpha", 3], (() => Promise.all([c.e(846), c.e(6914), c.e(4947), c.e(3203), c.e(6e3), c.e(6956), c.e(4629), c.e(8157), c.e(988), c.e(2230)]).then((() => () => c(17696))))),
         59601: () => s("default", "@jupyterlab/theme-dark-extension", [1, 3, 4, 8], (() => Promise.all([c.e(6956), c.e(3811)]).then((() => () => c(21058))))),
         99661: () => s("default", "@jupyterlab/theme-light-extension", [1, 3, 4, 8], (() => Promise.all([c.e(6956), c.e(7469)]).then((() => () => c(60275))))),
         4319: () => s("default", "@jupyterlab/markdownviewer-extension", [1, 3, 0, 0], (() => Promise.all([c.e(6956), c.e(7968), c.e(8930), c.e(6757)]).then((() => () => c(54382))))),
+        7573: () => s("default", "@lumino/datagrid", [2, 0, 36, 0], (() => c.e(8921).then((() => () => c(28921))))),
         24132: () => s("default", "@jupyterlab/mathjax2-extension", [1, 3, 0, 0], (() => c.e(3349).then((() => () => c(66976))))),
         41412: () => s("default", "@jupyterlab/rendermime-extension", [1, 3, 0, 0], (() => Promise.all([c.e(6956), c.e(3305)]).then((() => () => c(85985))))),
         70851: () => s("default", "@jupyterlab/json-extension", [1, 3, 0, 0], (() => Promise.all([c.e(5950), c.e(6956), c.e(4643), c.e(7505)]).then((() => () => c(45950))))),
         84632: () => s("default", "@jupyterlite/iframe-extension", [2, 0, 1, 0], (() => c.e(5826).then((() => () => c(26527))))),
-        78695: () => s("default", "@lumino/messaging", [1, 1, 7, 2], (() => Promise.all([c.e(3316), c.e(3203)]).then((() => () => c(73316))))),
-        4947: () => s("default", "@lumino/signaling", [1, 1, 7, 2], (() => Promise.all([c.e(3203), c.e(4629), c.e(5445)]).then((() => () => c(75445))))),
-        23203: () => s("default", "@lumino/algorithm", [1, 1, 6, 2], (() => c.e(9060).then((() => () => c(69060))))),
-        94812: () => s("default", "@lumino/domutils", [1, 1, 5, 2], (() => c.e(5403).then((() => () => c(85403))))),
-        36e3: () => s("default", "@lumino/disposable", [1, 1, 7, 2], (() => Promise.all([c.e(4947), c.e(3203), c.e(2488)]).then((() => () => c(72488))))),
         56956: () => s("default", "@jupyterlab/translation", [1, 3, 0, 0], (() => Promise.all([c.e(846), c.e(2322), c.e(4947), c.e(2233), c.e(4629), c.e(9110), c.e(988)]).then((() => () => c(29513))))),
-        24629: () => s("default", "@lumino/properties", [1, 1, 5, 2], (() => c.e(3312).then((() => () => c(73312))))),
-        70988: () => s("default", "@jupyterlab/services", [1, 6, 1, 8], (() => Promise.all([c.e(2361), c.e(846), c.e(6914), c.e(3203), c.e(6e3), c.e(9110), c.e(6417)]).then((() => () => c(16914))))),
+        70988: () => s("default", "@jupyterlab/services", [1, 6, 1, 8], (() => Promise.all([c.e(846), c.e(6914), c.e(3203), c.e(6e3), c.e(8157), c.e(9110), c.e(6417)]).then((() => () => c(16914))))),
         68930: () => s("default", "@jupyterlab/settingregistry", [1, 3, 0, 0], (() => Promise.all([c.e(6111), c.e(9513), c.e(4947), c.e(6e3), c.e(1514)]).then((() => () => c(69513))))),
         5320: () => s("default", "@jupyterlab/mainmenu", [1, 3, 0, 0], (() => Promise.all([c.e(4643), c.e(9406)]).then((() => () => c(21581))))),
         10409: () => s("default", "@jupyter-widgets/output", [1, 6, 0, 1], (() => c.e(7015).then((() => () => c(21100))))),
         70190: () => s("default", "@jupyterlab/logconsole", [1, 3, 0, 0], (() => c.e(9339).then((() => () => c(99339))))),
         24643: () => s("default", "@jupyterlab/ui-components", [1, 3, 0, 0], (() => Promise.all([c.e(6770), c.e(4963), c.e(4947), c.e(3203), c.e(6e3), c.e(6956), c.e(9110), c.e(7505), c.e(4627), c.e(2886)]).then((() => () => c(74963))))),
-        1514: () => s("default", "@lumino/commands", [1, 1, 15, 2], (() => Promise.all([c.e(2687), c.e(3203), c.e(6e3), c.e(4812)]).then((() => () => c(62687))))),
-        77968: () => s("default", "@jupyterlab/docregistry", [1, 3, 0, 0], (() => Promise.all([c.e(2361), c.e(6770), c.e(4939), c.e(9112), c.e(4875), c.e(4947), c.e(3203), c.e(6e3), c.e(4643), c.e(7505), c.e(2299), c.e(8695), c.e(6088), c.e(1876)]).then((() => () => c(74875))))),
+        77968: () => s("default", "@jupyterlab/docregistry", [1, 3, 0, 0], (() => Promise.all([c.e(6770), c.e(4939), c.e(9112), c.e(4875), c.e(4947), c.e(3203), c.e(6e3), c.e(8157), c.e(8695), c.e(4643), c.e(7505), c.e(2299), c.e(6088), c.e(1876)]).then((() => () => c(74875))))),
         97505: () => s("default", "react", [1, 17, 0, 1], (() => c.e(2784).then((() => () => c(2784))))),
+        1514: () => s("default", "@lumino/commands", [1, 1, 15, 2], (() => Promise.all([c.e(2687), c.e(4947), c.e(3203), c.e(6e3), c.e(4812), c.e(6968)]).then((() => () => c(62687))))),
         56088: () => s("default", "@lumino/coreutils", [1, 1, 8, 2], (() => c.e(4259).then((() => () => c(4259))))),
         91876: () => s("default", "@lumino/signaling", [1, 1, 7, 2], (() => Promise.all([c.e(319), c.e(1553)]).then((() => () => c(27003))))),
         49939: () => s("default", "@jupyterlab/nbformat", [1, 3, 0, 0], (() => c.e(86).then((() => () => c(63655))))),
-        32886: () => s("default", "@lumino/virtualdom", [1, 1, 11, 2], (() => c.e(1053).then((() => () => c(1053))))),
-        3860: () => s("default", "@lumino/dragdrop", [1, 1, 10, 2], (() => c.e(8809).then((() => () => c(38809))))),
         89098: () => s("default", "@jupyterlab/coreutils", [1, 5, 0, 0], (() => Promise.all([c.e(5952), c.e(2950), c.e(1105)]).then((() => () => c(42950))))),
         15490: () => s("default", "@jupyterlab/coreutils", [1, 5, 0, 0], (() => Promise.all([c.e(5952), c.e(3251), c.e(8164)]).then((() => () => c(53251))))),
-        34013: () => s("default", "@jupyterlab/services", [1, 6, 1, 8], (() => Promise.all([c.e(2361), c.e(846), c.e(7560), c.e(3203), c.e(6e3), c.e(4629), c.e(9098), c.e(8679)]).then((() => () => c(17560))))),
+        34013: () => s("default", "@jupyterlab/services", [1, 6, 1, 8], (() => Promise.all([c.e(846), c.e(7560), c.e(3203), c.e(6e3), c.e(4629), c.e(8157), c.e(9098), c.e(8679)]).then((() => () => c(17560))))),
         49943: () => s("default", "@jupyterlab/coreutils", [1, 5, 0, 0], (() => Promise.all([c.e(5952), c.e(286), c.e(1890)]).then((() => () => c(20286))))),
         48753: () => s("default", "@jupyterlite/contents", [2, 0, 1, 0], (() => Promise.all([c.e(9757), c.e(9110)]).then((() => () => c(9757))))),
         52329: () => s("default", "@jupyterlab/coreutils", [1, 5, 0, 0], (() => Promise.all([c.e(5952), c.e(1980), c.e(4947), c.e(5188)]).then((() => () => c(1980))))),
         52390: () => s("default", "@jupyterlab/coreutils", [1, 5, 0, 0], (() => Promise.all([c.e(5952), c.e(53), c.e(4947), c.e(7695)]).then((() => () => c(70053))))),
         70771: () => s("default", "@jupyterlab/coreutils", [1, 5, 0, 0], (() => Promise.all([c.e(5952), c.e(2359), c.e(4947), c.e(6839)]).then((() => () => c(62359))))),
         81298: () => s("default", "@jupyterlab/coreutils", [1, 5, 0, 0], (() => Promise.all([c.e(5952), c.e(596), c.e(4947), c.e(7795)]).then((() => () => c(20596))))),
         91491: () => s("default", "@jupyterlab/coreutils", [1, 5, 0, 0], (() => Promise.all([c.e(5952), c.e(4896), c.e(4947), c.e(5291)]).then((() => () => c(4896))))),
-        2132: () => s("default", "@jupyterlab/services", [1, 6, 1, 8], (() => Promise.all([c.e(2361), c.e(74), c.e(3203), c.e(6e3), c.e(4629), c.e(5490), c.e(9817)]).then((() => () => c(80074))))),
+        2132: () => s("default", "@jupyterlab/services", [1, 6, 1, 8], (() => Promise.all([c.e(74), c.e(3203), c.e(6e3), c.e(4629), c.e(8157), c.e(5490), c.e(9817)]).then((() => () => c(80074))))),
         86086: () => s("default", "@jupyterlab/coreutils", [1, 5, 0, 0], (() => Promise.all([c.e(5952), c.e(3922), c.e(8874)]).then((() => () => c(13922))))),
         90319: () => s("default", "@lumino/algorithm", [1, 1, 6, 2], (() => c.e(9807).then((() => () => c(89807))))),
         7531: () => s("default", "@jupyterlite/server-extension", [2, 0, 1, 0], (() => Promise.all([c.e(6111), c.e(4530), c.e(3203), c.e(7631), c.e(3862)]).then((() => () => c(24530))))),
         17021: () => s("default", "@jupyter-widgets/controls", [1, 5, 0, 1], (() => Promise.all([c.e(3851), c.e(8695), c.e(4812)]).then((() => () => c(53851)))))
     }, p = {
         49: [40049],
         319: [90319],
@@ -264,30 +268,33 @@
         4629: [24629],
         4643: [24643],
         4812: [94812],
         4863: [17021],
         4947: [4947],
         5238: [75238],
         5320: [5320],
-        5474: [4319, 24132, 41412, 70851, 84632],
         5490: [15490],
         5820: [34013, 49943],
         5918: [35918],
         6e3: [36e3],
         6088: [56088],
         6678: [10409, 70190],
         6956: [56956],
+        6968: [26968],
+        7002: [4319, 7573, 24132, 41412, 70851, 84632],
         7505: [97505],
         7531: [7531],
         7631: [7631],
         7651: [67651],
         7782: [37782],
         7968: [77968],
+        8157: [48157],
         8695: [78695],
         8930: [68930],
+        8971: [8971],
         8987: [9961, 22312, 59601, 99661],
         9098: [89098],
         9110: [59110],
         9939: [49939]
     }, c.f.consumes = (e, t) => {
         c.o(p, e) && p[e].forEach((e => {
             if (c.o(m, e)) return t.push(m[e]);
@@ -312,15 +319,15 @@
         var e = {
             6684: 0
         };
         c.f.j = (t, l) => {
             var r = c.o(e, t) ? e[t] : void 0;
             if (0 !== r)
                 if (r) l.push(r[2]);
-                else if (/^(2(051|233|299|886)|3(19(|8)|86[02]|203)|4(6(27|29|43)|456|812|863|9|947)|5((23|6|91)8|(32|49|82)0)|6(000|088|678|956)|7((53|63|65)1|505|782|968)|8(695|930|987)|9(098|110|88|939)|1514|1876)$/.test(t)) e[t] = 0;
+                else if (/^(2(051|233|299|886)|3(19(|8)|86[02]|203)|4(6(27|29|43)|456|812|863|9|947)|5((23|6|91)8|(32|49|82)0)|6((08|67|96)8|000|956)|7((53|63|65)1|505|782|968)|8(9(30|71|87)|157|695)|9(098|110|88|939)|1514|1876)$/.test(t)) e[t] = 0;
             else {
                 var a = new Promise(((l, a) => r = e[t] = [l, a]));
                 l.push(r[2] = a);
                 var n = c.p + c.u(t),
                     o = new Error;
                 c.l(n, (l => {
                     if (c.o(e, t) && (0 !== (r = e[t]) && (e[t] = void 0), r)) {
```

### Comparing `voici-0.4.3/LICENSE` & `voici-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/README.md` & `voici-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/pyproject.toml` & `voici-0.4.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `voici-0.4.3/PKG-INFO` & `voici-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voici
-Version: 0.4.3
+Version: 0.4.4
 Summary: Voici turns Jupyter notebooks into static web applications
 Project-URL: Homepage, https://github.com/voila-dashboards/voici
 Author: Voila Development Team
 License: BSD License
         
         Copyright (c) 2018 Voilà contributors.
         All rights reserved.
```

