# Comparing `tmp/buckaroo-0.2.6.tar.gz` & `tmp/buckaroo-0.2.7.tar.gz`

## Comparing `buckaroo-0.2.6.tar` & `buckaroo-0.2.7.tar`

### file list

```diff
@@ -1,76 +1,75 @@
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 buckaroo-0.2.6/.coveragerc
--rw-r--r--   0        0        0     7520 2020-02-02 00:00:00.000000 buckaroo-0.2.6/RELEASE.md
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 buckaroo-0.2.6/babel.config.js
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 buckaroo-0.2.6/dcef.json
--rwxr-xr-x   0        0        0      232 2020-02-02 00:00:00.000000 buckaroo-0.2.6/full_build.sh
--rw-r--r--   0        0        0     5826 2020-02-02 00:00:00.000000 buckaroo-0.2.6/introduction.ipynb
--rw-r--r--   0        0        0     4492 2020-02-02 00:00:00.000000 buckaroo-0.2.6/package.json
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 buckaroo-0.2.6/setup.py
--rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 buckaroo-0.2.6/tryit.ipynb
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 buckaroo-0.2.6/tsconfig.json
--rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 buckaroo-0.2.6/webpack.config.js
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 buckaroo-0.2.6/webpack.lab.config.js
--rw-r--r--   0        0        0   321074 2020-02-02 00:00:00.000000 buckaroo-0.2.6/yarn.lock
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 buckaroo-0.2.6/dcef/__init__.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 buckaroo-0.2.6/dcef/_frontend.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 buckaroo-0.2.6/dcef/_version.py
--rw-r--r--   0        0        0     5049 2020-02-02 00:00:00.000000 buckaroo-0.2.6/dcef/all_transforms.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 buckaroo-0.2.6/dcef/channeldata.json
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 buckaroo-0.2.6/dcef/configure_utils.py
--rw-r--r--   0        0        0     4490 2020-02-02 00:00:00.000000 buckaroo-0.2.6/dcef/dcef_widget.py
--rw-r--r--   0        0        0     5608 2020-02-02 00:00:00.000000 buckaroo-0.2.6/dcef/dcf_transform.py
--rw-r--r--   0        0        0     6535 2020-02-02 00:00:00.000000 buckaroo-0.2.6/dcef/df_methods.py
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 buckaroo-0.2.6/dcef/index.html
--rw-r--r--   0        0        0    17284 2020-02-02 00:00:00.000000 buckaroo-0.2.6/dcef/lispy.py
--rw-r--r--   0        0        0     3683 2020-02-02 00:00:00.000000 buckaroo-0.2.6/dcef/summary_stats.py
--rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 buckaroo-0.2.6/dcef/views.py
--rw-r--r--   0        0        0     4620 2020-02-02 00:00:00.000000 buckaroo-0.2.6/dcef/labextension/package.json
--rw-r--r--   0        0        0  1241248 2020-02-02 00:00:00.000000 buckaroo-0.2.6/dcef/labextension/static/116.3a7574d1f75164e010bc.js
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 buckaroo-0.2.6/dcef/labextension/static/116.3a7574d1f75164e010bc.js.LICENSE.txt
--rw-r--r--   0        0        0   373830 2020-02-02 00:00:00.000000 buckaroo-0.2.6/dcef/labextension/static/250.c608416dcff072a71036.js
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 buckaroo-0.2.6/dcef/labextension/static/250.c608416dcff072a71036.js.LICENSE.txt
--rw-r--r--   0        0        0    10850 2020-02-02 00:00:00.000000 buckaroo-0.2.6/dcef/labextension/static/480.55b0b32536a517ae86fb.js
--rw-r--r--   0        0        0    70476 2020-02-02 00:00:00.000000 buckaroo-0.2.6/dcef/labextension/static/486.5d15e39140ce71ec7db7.js
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 buckaroo-0.2.6/dcef/labextension/static/486.5d15e39140ce71ec7db7.js.LICENSE.txt
--rw-r--r--   0        0        0    10325 2020-02-02 00:00:00.000000 buckaroo-0.2.6/dcef/labextension/static/568.be621402413454ffa400.js
--rw-r--r--   0        0        0     7359 2020-02-02 00:00:00.000000 buckaroo-0.2.6/dcef/labextension/static/remoteEntry.b7da48392a5008410871.js
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 buckaroo-0.2.6/dcef/labextension/static/style.js
--rw-r--r--   0        0        0    12889 2020-02-02 00:00:00.000000 buckaroo-0.2.6/dcef/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 buckaroo-0.2.6/dcef/nbextension/extension.js
--rw-r--r--   0        0        0  1696784 2020-02-02 00:00:00.000000 buckaroo-0.2.6/dcef/nbextension/index.js
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 buckaroo-0.2.6/dcef/nbextension/index.js.LICENSE.txt
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 buckaroo-0.2.6/dcef/noarch/current_repodata.json
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 buckaroo-0.2.6/dcef/noarch/current_repodata.json.bz2
--rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 buckaroo-0.2.6/dcef/noarch/index.html
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 buckaroo-0.2.6/dcef/noarch/repodata.json
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 buckaroo-0.2.6/dcef/noarch/repodata.json.bz2
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 buckaroo-0.2.6/dcef/noarch/repodata_from_packages.json
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 buckaroo-0.2.6/dcef/noarch/repodata_from_packages.json.bz2
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 buckaroo-0.2.6/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 buckaroo-0.2.6/docs/make.bat
--rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 buckaroo-0.2.6/docs/source/FAQ.rst
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 buckaroo-0.2.6/docs/source/conf.py
--rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 buckaroo-0.2.6/docs/source/contributing.rst
--rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 buckaroo-0.2.6/docs/source/index.rst
--rwxr-xr-x   0        0        0      268 2020-02-02 00:00:00.000000 buckaroo-0.2.6/docs/source/install.rst
--rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 buckaroo-0.2.6/docs/source/using.rst
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 buckaroo-0.2.6/docs/source/_static/embed-bundle.js.LICENSE.txt
--rw-r--r--   0        0        0     4564 2020-02-02 00:00:00.000000 buckaroo-0.2.6/js/dcefwidget.ts
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 buckaroo-0.2.6/js/extension.ts
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 buckaroo-0.2.6/js/index.ts
--rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 buckaroo-0.2.6/js/paddywidget.ts
--rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 buckaroo-0.2.6/js/plugin.ts
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 buckaroo-0.2.6/js/version.ts
--rw-r--r--   0        0        0  1335815 2020-02-02 00:00:00.000000 buckaroo-0.2.6/static/images/dcf-jupyter.png
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 buckaroo-0.2.6/style/widget.css
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 buckaroo-0.2.6/style/icons/arrow-down-short-dark.svg
--rwxr-xr-x   0        0        0      416 2020-02-02 00:00:00.000000 buckaroo-0.2.6/style/icons/arrow-down-short.svg
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 buckaroo-0.2.6/style/icons/arrow-up-short-dark.svg
--rwxr-xr-x   0        0        0      400 2020-02-02 00:00:00.000000 buckaroo-0.2.6/style/icons/arrow-up-short.svg
--rwxr-xr-x   0        0        0      349 2020-02-02 00:00:00.000000 buckaroo-0.2.6/style/icons/filter-dark.svg
--rwxr-xr-x   0        0        0      349 2020-02-02 00:00:00.000000 buckaroo-0.2.6/style/icons/filter.svg
--rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 buckaroo-0.2.6/.gitignore
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 buckaroo-0.2.6/LICENSE.txt
--rw-r--r--   0        0        0     8870 2020-02-02 00:00:00.000000 buckaroo-0.2.6/README.md
--rw-r--r--   0        0        0     3053 2020-02-02 00:00:00.000000 buckaroo-0.2.6/pyproject.toml
--rw-r--r--   0        0        0    11643 2020-02-02 00:00:00.000000 buckaroo-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 buckaroo-0.2.7/.coveragerc
+-rw-r--r--   0        0        0     7520 2020-02-02 00:00:00.000000 buckaroo-0.2.7/RELEASE.md
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 buckaroo-0.2.7/babel.config.js
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 buckaroo-0.2.7/buckaroo.json
+-rwxr-xr-x   0        0        0      232 2020-02-02 00:00:00.000000 buckaroo-0.2.7/full_build.sh
+-rw-r--r--   0        0        0     4419 2020-02-02 00:00:00.000000 buckaroo-0.2.7/introduction.ipynb
+-rw-r--r--   0        0        0     4520 2020-02-02 00:00:00.000000 buckaroo-0.2.7/package.json
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 buckaroo-0.2.7/setup.py
+-rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 buckaroo-0.2.7/tryit.ipynb
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 buckaroo-0.2.7/tsconfig.json
+-rw-r--r--   0        0        0     2837 2020-02-02 00:00:00.000000 buckaroo-0.2.7/webpack.config.js
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 buckaroo-0.2.7/webpack.lab.config.js
+-rw-r--r--   0        0        0   321074 2020-02-02 00:00:00.000000 buckaroo-0.2.7/yarn.lock
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 buckaroo-0.2.7/buckaroo/__init__.py
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 buckaroo-0.2.7/buckaroo/_frontend.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 buckaroo-0.2.7/buckaroo/_version.py
+-rw-r--r--   0        0        0     5065 2020-02-02 00:00:00.000000 buckaroo-0.2.7/buckaroo/all_transforms.py
+-rw-r--r--   0        0        0     4518 2020-02-02 00:00:00.000000 buckaroo-0.2.7/buckaroo/buckaroo_widget.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 buckaroo-0.2.7/buckaroo/channeldata.json
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 buckaroo-0.2.7/buckaroo/configure_utils.py
+-rw-r--r--   0        0        0     5608 2020-02-02 00:00:00.000000 buckaroo-0.2.7/buckaroo/dcf_transform.py
+-rw-r--r--   0        0        0     6535 2020-02-02 00:00:00.000000 buckaroo-0.2.7/buckaroo/df_methods.py
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 buckaroo-0.2.7/buckaroo/index.html
+-rw-r--r--   0        0        0    17284 2020-02-02 00:00:00.000000 buckaroo-0.2.7/buckaroo/lispy.py
+-rw-r--r--   0        0        0     3683 2020-02-02 00:00:00.000000 buckaroo-0.2.7/buckaroo/summary_stats.py
+-rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 buckaroo-0.2.7/buckaroo/views.py
+-rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 buckaroo-0.2.7/buckaroo/labextension/package.json
+-rw-r--r--   0        0        0  1241256 2020-02-02 00:00:00.000000 buckaroo-0.2.7/buckaroo/labextension/static/116.b6e5adfccd7c520a720a.js
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 buckaroo-0.2.7/buckaroo/labextension/static/116.b6e5adfccd7c520a720a.js.LICENSE.txt
+-rw-r--r--   0        0        0   373838 2020-02-02 00:00:00.000000 buckaroo-0.2.7/buckaroo/labextension/static/250.b55e2550464d9477eb95.js
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 buckaroo-0.2.7/buckaroo/labextension/static/250.b55e2550464d9477eb95.js.LICENSE.txt
+-rw-r--r--   0        0        0    10250 2020-02-02 00:00:00.000000 buckaroo-0.2.7/buckaroo/labextension/static/480.e809fc8a18bc53e804a1.js
+-rw-r--r--   0        0        0    70484 2020-02-02 00:00:00.000000 buckaroo-0.2.7/buckaroo/labextension/static/486.f08778dfb765d893ceaf.js
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 buckaroo-0.2.7/buckaroo/labextension/static/486.f08778dfb765d893ceaf.js.LICENSE.txt
+-rw-r--r--   0        0        0     9717 2020-02-02 00:00:00.000000 buckaroo-0.2.7/buckaroo/labextension/static/568.9a4b0a85049c75a13a73.js
+-rw-r--r--   0        0        0     7384 2020-02-02 00:00:00.000000 buckaroo-0.2.7/buckaroo/labextension/static/remoteEntry.d4606edd7ebd1ec0dcc6.js
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 buckaroo-0.2.7/buckaroo/labextension/static/style.js
+-rw-r--r--   0        0        0    12889 2020-02-02 00:00:00.000000 buckaroo-0.2.7/buckaroo/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 buckaroo-0.2.7/buckaroo/nbextension/extension.js
+-rw-r--r--   0        0        0  1696168 2020-02-02 00:00:00.000000 buckaroo-0.2.7/buckaroo/nbextension/index.js
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 buckaroo-0.2.7/buckaroo/nbextension/index.js.LICENSE.txt
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 buckaroo-0.2.7/buckaroo/noarch/current_repodata.json
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 buckaroo-0.2.7/buckaroo/noarch/current_repodata.json.bz2
+-rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 buckaroo-0.2.7/buckaroo/noarch/index.html
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 buckaroo-0.2.7/buckaroo/noarch/repodata.json
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 buckaroo-0.2.7/buckaroo/noarch/repodata.json.bz2
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 buckaroo-0.2.7/buckaroo/noarch/repodata_from_packages.json
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 buckaroo-0.2.7/buckaroo/noarch/repodata_from_packages.json.bz2
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 buckaroo-0.2.7/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 buckaroo-0.2.7/docs/make.bat
+-rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 buckaroo-0.2.7/docs/source/FAQ.rst
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 buckaroo-0.2.7/docs/source/conf.py
+-rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 buckaroo-0.2.7/docs/source/contributing.rst
+-rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 buckaroo-0.2.7/docs/source/index.rst
+-rwxr-xr-x   0        0        0      268 2020-02-02 00:00:00.000000 buckaroo-0.2.7/docs/source/install.rst
+-rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 buckaroo-0.2.7/docs/source/using.rst
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 buckaroo-0.2.7/docs/source/_static/embed-bundle.js.LICENSE.txt
+-rw-r--r--   0        0        0     3054 2020-02-02 00:00:00.000000 buckaroo-0.2.7/js/dcefwidget.ts
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 buckaroo-0.2.7/js/extension.ts
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 buckaroo-0.2.7/js/index.ts
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 buckaroo-0.2.7/js/plugin.ts
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 buckaroo-0.2.7/js/version.ts
+-rw-r--r--   0        0        0  1335815 2020-02-02 00:00:00.000000 buckaroo-0.2.7/static/images/dcf-jupyter.png
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 buckaroo-0.2.7/style/widget.css
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 buckaroo-0.2.7/style/icons/arrow-down-short-dark.svg
+-rwxr-xr-x   0        0        0      416 2020-02-02 00:00:00.000000 buckaroo-0.2.7/style/icons/arrow-down-short.svg
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 buckaroo-0.2.7/style/icons/arrow-up-short-dark.svg
+-rwxr-xr-x   0        0        0      400 2020-02-02 00:00:00.000000 buckaroo-0.2.7/style/icons/arrow-up-short.svg
+-rwxr-xr-x   0        0        0      349 2020-02-02 00:00:00.000000 buckaroo-0.2.7/style/icons/filter-dark.svg
+-rwxr-xr-x   0        0        0      349 2020-02-02 00:00:00.000000 buckaroo-0.2.7/style/icons/filter.svg
+-rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 buckaroo-0.2.7/.gitignore
+-rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 buckaroo-0.2.7/LICENSE.txt
+-rw-r--r--   0        0        0     8870 2020-02-02 00:00:00.000000 buckaroo-0.2.7/README.md
+-rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 buckaroo-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0    11646 2020-02-02 00:00:00.000000 buckaroo-0.2.7/PKG-INFO
```

### Comparing `buckaroo-0.2.6/RELEASE.md` & `buckaroo-0.2.7/RELEASE.md`

 * *Files identical despite different names*

### Comparing `buckaroo-0.2.6/package.json` & `buckaroo-0.2.7/package.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9078125%*

 * *Differences: {"'bugs'": "{'url': 'https://github.com/paddymul/buckaroo/issues'}",*

 * * "'homepage'": "'https://github.com/paddymul/buckaroo'",*

 * * "'jupyterlab'": "{'outputDir': './buckaroo/labextension'}",*

 * * "'name'": "'buckaroo'",*

 * * "'repository'": "{'url': 'https://github.com/paddymul/buckaroo'}",*

 * * "'scripts'": "{'clean:labextension': 'rimraf buckaroo/labextension', 'clean:nbextension': 'rimraf "*

 * *              'buckaroo/nbextension/index.*\', \'lint:fix\': "eslint \'js/**/*.{ts,tsx}\' --fix"}'}*

```diff
@@ -1,14 +1,14 @@
 {
     "author": {
         "email": "",
         "name": "Paddy Mullen"
     },
     "bugs": {
-        "url": "https://github.com/paddymul/dcef/issues"
+        "url": "https://github.com/paddymul/buckaroo/issues"
     },
     "dependencies": {
         "@jupyter-widgets/base": "^2 || ^3 || ^4 || ^6.0.0",
         "@jupyterlab/apputils": "^3.0.2",
         "lodash": "^4.17.21",
         "paddy-react-edit-list": ">=1.1.35",
         "react": "^18.0.0",
@@ -57,18 +57,18 @@
         "lib/**/*.js.map",
         "lib/**/*.ts",
         "dist/*.js",
         "dist/*.js.map",
         "dist/*.png",
         "style/**/*.*"
     ],
-    "homepage": "https://github.com/paddymul/dcef",
+    "homepage": "https://github.com/paddymul/buckaroo",
     "jupyterlab": {
         "extension": "lib/plugin",
-        "outputDir": "./dcef/labextension",
+        "outputDir": "./buckaroo/labextension",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
             },
             "@lumino/algorithm": {
                 "bundled": false,
@@ -115,34 +115,34 @@
         "jupyter",
         "jupyterlab",
         "jupyterlab-extension",
         "widgets"
     ],
     "license": "BSD-3-Clause",
     "main": "lib/index.js",
-    "name": "dcef",
+    "name": "buckaroo",
     "repository": {
         "type": "git",
-        "url": "https://github.com/paddymul/dcef"
+        "url": "https://github.com/paddymul/buckaroo"
     },
     "scripts": {
         "build": "yarn run build:lib && yarn run build:nbextension && yarn run build:labextension",
         "build:all": "yarn run build:labextension && yarn run build:nbextension && yarn run build:widget-examples",
         "build:dev": "yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev",
         "build:labextension": "jupyter labextension build .",
         "build:labextension:dev": "jupyter labextension build --development True .",
         "build:lib": "tsc",
         "build:nbextension": "webpack --mode=production --no-devtool",
         "build:widget-examples": "cd widget-examples/basic && webpack --mode=production",
         "clean": "rimraf dist && yarn run clean:lib && yarn run clean:labextension && yarn run clean:nbextension",
-        "clean:labextension": "rimraf dcef/labextension",
+        "clean:labextension": "rimraf buckaroo/labextension",
         "clean:lib": "rimraf lib",
-        "clean:nbextension": "rimraf dcef/nbextension/index.*",
+        "clean:nbextension": "rimraf buckaroo/nbextension/index.*",
         "lint": "eslint 'js/**/*.{ts,tsx}'",
-        "lint:fix": "eslint 'js/**/*.{ts,tsx} --fix'",
+        "lint:fix": "eslint 'js/**/*.{ts,tsx}' --fix",
         "prepack": "yarn run build:labextension && yarn run build:nbextension",
         "test": "jest --verbose",
         "watch": "npm-run-all -p watch:*",
         "watch:labextension": "jupyter labextension watch .",
         "watch:lib": "tsc -w",
         "watch:nbextension": "webpack --watch"
     },
```

### Comparing `buckaroo-0.2.6/tryit.ipynb` & `buckaroo-0.2.7/tryit.ipynb`

 * *Files identical despite different names*

### Comparing `buckaroo-0.2.6/tsconfig.json` & `buckaroo-0.2.7/tsconfig.json`

 * *Files identical despite different names*

### Comparing `buckaroo-0.2.6/webpack.config.js` & `buckaroo-0.2.7/webpack.config.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -61,43 +61,43 @@
      * This bundle only contains the part of the JavaScript that is run on load of
      * the notebook.
      */
     {
         entry: './js/extension.ts',
         output: {
             filename: 'index.js',
-            path: path.resolve(__dirname, 'dcef', 'nbextension'),
+            path: path.resolve(__dirname, 'buckaroo', 'nbextension'),
             libraryTarget: 'amd',
         },
         module: {
             rules: rules,
         },
         devtool: 'source-map',
         externals,
         resolve,
     },
 
     /**
-     * Embeddable dcef bundle
+     * Embeddable buckaroo bundle
      *
      * This bundle is almost identical to the notebook extension bundle. The only
      * difference is in the configuration of the webpack public path for the
      * static assets.
      *
      * The target bundle is always `dist/index.js`, which is the path required by
      * the custom widget embedder.
      */
     {
         entry: './js/index.ts',
         output: {
             filename: 'index.js',
             path: path.resolve(__dirname, 'dist'),
             libraryTarget: 'amd',
-            library: 'dcef',
-            publicPath: 'https://unpkg.com/dcef@' + version + '/dist/',
+            library: 'buckaroo',
+            publicPath: 'https://unpkg.com/buckaroo@' + version + '/dist/',
         },
         devtool: 'source-map',
         module: {
             rules: rules,
         },
         externals,
         resolve,
@@ -109,15 +109,15 @@
      * This bundle is used to embed widgets in the package documentation.
      */
     {
         entry: './js/index.ts',
         output: {
             filename: 'embed-bundle.js',
             path: path.resolve(__dirname, 'docs', 'source', '_static'),
-            library: 'dcef',
+            library: 'buckaroo',
             libraryTarget: 'amd',
         },
         module: {
             rules: rules,
         },
         devtool: 'source-map',
         externals,
```

### Comparing `buckaroo-0.2.6/yarn.lock` & `buckaroo-0.2.7/yarn.lock`

 * *Files identical despite different names*

### Comparing `buckaroo-0.2.6/dcef/all_transforms.py` & `buckaroo-0.2.7/buckaroo/all_transforms.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from .lispy import s
-from .configure_utils import configure_dcef
+from .configure_utils import configure_buckaroo
 import pandas as pd
 import numpy as np
 
 class Command(object):
     pass
     
 class FillNA(Command):
@@ -151,9 +151,9 @@
     def transform_to_py(df, col):
         return "\n".join(
             ["    old_col = df['%s']" % col,
              "    df.drop('%s', axis=1, inplace=True)" % col,
              "    df.index = old_col.values"])
 
 DefaultCommandKlsList = [DropCol, to_datetime, SafeInt, FillNA, reindex, OneHot, GroupBy]
-command_defaults, command_patterns, dcef_transform, dcef_to_py_core = configure_dcef(DefaultCommandKlsList)
+command_defaults, command_patterns, buckaroo_transform, buckaroo_to_py_core = configure_buckaroo(DefaultCommandKlsList)
```

### Comparing `buckaroo-0.2.6/dcef/configure_utils.py` & `buckaroo-0.2.7/buckaroo/configure_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 from .lispy import make_interpreter
-def configure_dcef(transforms):
+def configure_buckaroo(transforms):
     command_defaults = {}
     command_patterns = {}
 
     transform_lisp_primitives = {}
     to_py_lisp_primitives = {}
     for T in transforms:
         t = T()
         transform_name = t.command_default[0]['symbol']
         command_defaults[transform_name] = t.command_default
         command_patterns[transform_name] = t.command_pattern
         transform_lisp_primitives[transform_name] = T.transform
         to_py_lisp_primitives[transform_name] = T.transform_to_py
     
-    dcef_eval, raw_parse = make_interpreter(transform_lisp_primitives)
-    def dcef_transform(instructions, df):
+    buckaroo_eval, raw_parse = make_interpreter(transform_lisp_primitives)
+    def buckaroo_transform(instructions, df):
         df_copy = df.copy()
-        ret_val =  dcef_eval(instructions, {'df':df_copy})
+        ret_val =  buckaroo_eval(instructions, {'df':df_copy})
         #print(ret_val)
         return ret_val
 
     convert_to_python, __unused = make_interpreter(to_py_lisp_primitives)
-    def dcef_to_py(instructions):
+    def buckaroo_to_py(instructions):
         #I would prefer to implement this with a macro named something
         #like 'clean' that is implemented for the _convert_to_python
         #interpreter to return a string code block, and for the real DCF
         #interpreter as 'begin'... that way the exact same instructions
         #could be sent to either interpreter.  For now, this will do
         individual_instructions =  [x for x in map(lambda x:convert_to_python(x, {'df':5}), instructions)]
         #print("individual_instructions", individual_instructions)
         code_block =  '\n'.join(individual_instructions)
 
         return "def clean(df):\n" + code_block + "\n    return df"
-    return command_defaults, command_patterns, dcef_transform, dcef_to_py
+    return command_defaults, command_patterns, buckaroo_transform, buckaroo_to_py
```

### Comparing `buckaroo-0.2.6/dcef/dcef_widget.py` & `buckaroo-0.2.7/buckaroo/buckaroo_widget.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 """
 TODO: Add module docstring
 """
 
 from ipywidgets import DOMWidget
 from traitlets import Unicode, List, Dict, observe
 from ._frontend import module_name, module_version
-from .all_transforms import configure_dcef, DefaultCommandKlsList
+from .all_transforms import configure_buckaroo, DefaultCommandKlsList
 from .summary_stats import summarize_df
 import json
 
 
-class DCEFWidget(DOMWidget):
+class BuckarooWidget(DOMWidget):
     """TODO: Add docstring here
     """
     _model_name = Unicode('DCEFWidgetModel').tag(sync=True)
     _model_module = Unicode(module_name).tag(sync=True)
     _model_module_version = Unicode(module_version).tag(sync=True)
     _view_name = Unicode('DCEFWidgetView').tag(sync=True)
     _view_module = Unicode(module_name).tag(sync=True)
@@ -102,27 +102,27 @@
             results = {}
             if len(operations) == 1:
                 results['transformed_df'] = self.origDf
                 results['generated_py_code'] = 'no operations'
                 print('exiting early')
                 return
             
-            transformed_df = self.dcef_transform(operations, self.df)
+            transformed_df = self.buckaroo_transform(operations, self.df)
             results['transformed_df'] = json.loads(transformed_df.to_json(orient='table', indent=2))
 
-            results['generated_py_code'] = self.dcef_to_py_core(operations[1:])
+            results['generated_py_code'] = self.buckaroo_to_py_core(operations[1:])
             self.operation_results = results
             print("operations_results", results.keys())
         except Exception as e:
             print("error_setting", e)
             self.transform_error = str(e)
             raise
 
     def setup_from_command_kls_list(self):
-        command_defaults, command_patterns, self.dcef_transform, self.dcef_to_py_core = configure_dcef(
+        command_defaults, command_patterns, self.buckaroo_transform, self.buckaroo_to_py_core = configure_buckaroo(
             self.command_classes)
         self.commandConfig = dict(
             argspecs=command_patterns, defaultArgs=command_defaults)
 
 
     def add_command(self, incomingCommandKls):
         without_incoming = [x for x in self.command_classes if not x.__name__ == incomingCommandKls.__name__]
```

### Comparing `buckaroo-0.2.6/dcef/dcf_transform.py` & `buckaroo-0.2.7/buckaroo/dcf_transform.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.2.6/dcef/df_methods.py` & `buckaroo-0.2.7/buckaroo/df_methods.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.2.6/dcef/index.html` & `buckaroo-0.2.7/buckaroo/index.html`

 * *Files identical despite different names*

### Comparing `buckaroo-0.2.6/dcef/lispy.py` & `buckaroo-0.2.7/buckaroo/lispy.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.2.6/dcef/summary_stats.py` & `buckaroo-0.2.7/buckaroo/summary_stats.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.2.6/dcef/views.py` & `buckaroo-0.2.7/buckaroo/views.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.2.6/dcef/labextension/package.json` & `buckaroo-0.2.7/buckaroo/labextension/package.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9078125%*

 * *Differences: {"'bugs'": "{'url': 'https://github.com/paddymul/buckaroo/issues'}",*

 * * "'homepage'": "'https://github.com/paddymul/buckaroo'",*

 * * "'jupyterlab'": "{'outputDir': './buckaroo/labextension', '_build': {'load': "*

 * *                 "'static/remoteEntry.d4606edd7ebd1ec0dcc6.js'}}",*

 * * "'name'": "'buckaroo'",*

 * * "'repository'": "{'url': 'https://github.com/paddymul/buckaroo'}",*

 * * "'scripts'": "{'clean:labextension': 'rimraf buckaroo/labextension', 'clean:nbextension': 'rimraf "*

 * *              'buckaroo/nbextension/index.*\' […]*

```diff
@@ -1,14 +1,14 @@
 {
     "author": {
         "email": "",
         "name": "Paddy Mullen"
     },
     "bugs": {
-        "url": "https://github.com/paddymul/dcef/issues"
+        "url": "https://github.com/paddymul/buckaroo/issues"
     },
     "dependencies": {
         "@jupyter-widgets/base": "^2 || ^3 || ^4 || ^6.0.0",
         "@jupyterlab/apputils": "^3.0.2",
         "lodash": "^4.17.21",
         "paddy-react-edit-list": ">=1.1.35",
         "react": "^18.0.0",
@@ -57,22 +57,22 @@
         "lib/**/*.js.map",
         "lib/**/*.ts",
         "dist/*.js",
         "dist/*.js.map",
         "dist/*.png",
         "style/**/*.*"
     ],
-    "homepage": "https://github.com/paddymul/dcef",
+    "homepage": "https://github.com/paddymul/buckaroo",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.b7da48392a5008410871.js"
+            "load": "static/remoteEntry.d4606edd7ebd1ec0dcc6.js"
         },
         "extension": "lib/plugin",
-        "outputDir": "./dcef/labextension",
+        "outputDir": "./buckaroo/labextension",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
             },
             "@lumino/algorithm": {
                 "bundled": false,
@@ -119,34 +119,34 @@
         "jupyter",
         "jupyterlab",
         "jupyterlab-extension",
         "widgets"
     ],
     "license": "BSD-3-Clause",
     "main": "lib/index.js",
-    "name": "dcef",
+    "name": "buckaroo",
     "repository": {
         "type": "git",
-        "url": "https://github.com/paddymul/dcef"
+        "url": "https://github.com/paddymul/buckaroo"
     },
     "scripts": {
         "build": "yarn run build:lib && yarn run build:nbextension && yarn run build:labextension",
         "build:all": "yarn run build:labextension && yarn run build:nbextension && yarn run build:widget-examples",
         "build:dev": "yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev",
         "build:labextension": "jupyter labextension build .",
         "build:labextension:dev": "jupyter labextension build --development True .",
         "build:lib": "tsc",
         "build:nbextension": "webpack --mode=production --no-devtool",
         "build:widget-examples": "cd widget-examples/basic && webpack --mode=production",
         "clean": "rimraf dist && yarn run clean:lib && yarn run clean:labextension && yarn run clean:nbextension",
-        "clean:labextension": "rimraf dcef/labextension",
+        "clean:labextension": "rimraf buckaroo/labextension",
         "clean:lib": "rimraf lib",
-        "clean:nbextension": "rimraf dcef/nbextension/index.*",
+        "clean:nbextension": "rimraf buckaroo/nbextension/index.*",
         "lint": "eslint 'js/**/*.{ts,tsx}'",
-        "lint:fix": "eslint 'js/**/*.{ts,tsx} --fix'",
+        "lint:fix": "eslint 'js/**/*.{ts,tsx}' --fix",
         "prepack": "yarn run build:labextension && yarn run build:nbextension",
         "test": "jest --verbose",
         "watch": "npm-run-all -p watch:*",
         "watch:labextension": "jupyter labextension watch .",
         "watch:lib": "tsc -w",
         "watch:nbextension": "webpack --watch"
     },
```

### Comparing `buckaroo-0.2.6/dcef/labextension/static/116.3a7574d1f75164e010bc.js` & `buckaroo-0.2.7/buckaroo/labextension/static/116.b6e5adfccd7c520a720a.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,9 +1,9 @@
-/*! For license information please see 116.3a7574d1f75164e010bc.js.LICENSE.txt */
-(self.webpackChunkdcef = self.webpackChunkdcef || []).push([
+/*! For license information please see 116.b6e5adfccd7c520a720a.js.LICENSE.txt */
+(self.webpackChunkbuckaroo = self.webpackChunkbuckaroo || []).push([
     [116], {
         1731: (e, t, o) => {
             "use strict";
 
             function n(e) {
                 return null == e || "" === e ? null : e
             }
```

### Comparing `buckaroo-0.2.6/dcef/labextension/static/116.3a7574d1f75164e010bc.js.LICENSE.txt` & `buckaroo-0.2.7/buckaroo/labextension/static/116.b6e5adfccd7c520a720a.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `buckaroo-0.2.6/dcef/labextension/static/250.c608416dcff072a71036.js` & `buckaroo-0.2.7/buckaroo/labextension/static/250.b55e2550464d9477eb95.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,9 +1,9 @@
-/*! For license information please see 250.c608416dcff072a71036.js.LICENSE.txt */
-(self.webpackChunkdcef = self.webpackChunkdcef || []).push([
+/*! For license information please see 250.b55e2550464d9477eb95.js.LICENSE.txt */
+(self.webpackChunkbuckaroo = self.webpackChunkbuckaroo || []).push([
     [250], {
         7182: (n, e, a) => {
             (e = a(3645)(!1)).push([n.id, '.ag-icon {\n  font-family: var(--ag-icon-font-family);\n  font-size: var(--ag-icon-size);\n  line-height: var(--ag-icon-size);\n  font-style: normal;\n  font-weight: normal;\n  font-variant: normal;\n  text-transform: none;\n  -webkit-font-smoothing: antialiased;\n  -moz-osx-font-smoothing: grayscale;\n}\n\n.ag-icon-aggregation::before {\n  content: var(--ag-icon-font-code-aggregation, "\\f101");\n}\n\n.ag-icon-arrows::before {\n  content: var(--ag-icon-font-code-arrows, "\\f102");\n}\n\n.ag-icon-asc::before {\n  content: var(--ag-icon-font-code-asc, "\\f103");\n}\n\n.ag-icon-cancel::before {\n  content: var(--ag-icon-font-code-cancel, "\\f104");\n}\n\n.ag-icon-chart::before {\n  content: var(--ag-icon-font-code-chart, "\\f105");\n}\n\n.ag-icon-checkbox-checked::before {\n  content: var(--ag-icon-font-code-checkbox-checked, "\\f106");\n}\n\n.ag-icon-checkbox-indeterminate::before {\n  content: var(--ag-icon-font-code-checkbox-indeterminate, "\\f107");\n}\n\n.ag-icon-checkbox-unchecked::before {\n  content: var(--ag-icon-font-code-checkbox-unchecked, "\\f108");\n}\n\n.ag-icon-color-picker::before {\n  content: var(--ag-icon-font-code-color-picker, "\\f109");\n}\n\n.ag-icon-columns::before {\n  content: var(--ag-icon-font-code-columns, "\\f10a");\n}\n\n.ag-icon-contracted::before {\n  content: var(--ag-icon-font-code-contracted, "\\f10b");\n}\n\n.ag-icon-copy::before {\n  content: var(--ag-icon-font-code-copy, "\\f10c");\n}\n\n.ag-icon-cross::before {\n  content: var(--ag-icon-font-code-cross, "\\f10d");\n}\n\n.ag-icon-csv::before {\n  content: var(--ag-icon-font-code-csv, "\\f10e");\n}\n\n.ag-icon-cut::before {\n  content: var(--ag-icon-font-code-cut, "\\f10f");\n}\n\n.ag-icon-desc::before {\n  content: var(--ag-icon-font-code-desc, "\\f110");\n}\n\n.ag-icon-excel::before {\n  content: var(--ag-icon-font-code-excel, "\\f111");\n}\n\n.ag-icon-expanded::before {\n  content: var(--ag-icon-font-code-expanded, "\\f112");\n}\n\n.ag-icon-eye-slash::before {\n  content: var(--ag-icon-font-code-eye-slash, "\\f113");\n}\n\n.ag-icon-eye::before {\n  content: var(--ag-icon-font-code-eye, "\\f114");\n}\n\n.ag-icon-filter::before {\n  content: var(--ag-icon-font-code-filter, "\\f115");\n}\n\n.ag-icon-first::before {\n  content: var(--ag-icon-font-code-first, "\\f116");\n}\n\n.ag-icon-grip::before {\n  content: var(--ag-icon-font-code-grip, "\\f117");\n}\n\n.ag-icon-group::before {\n  content: var(--ag-icon-font-code-group, "\\f118");\n}\n\n.ag-icon-last::before {\n  content: var(--ag-icon-font-code-last, "\\f119");\n}\n\n.ag-icon-left::before {\n  content: var(--ag-icon-font-code-left, "\\f11a");\n}\n\n.ag-icon-linked::before {\n  content: var(--ag-icon-font-code-linked, "\\f11b");\n}\n\n.ag-icon-loading::before {\n  content: var(--ag-icon-font-code-loading, "\\f11c");\n}\n\n.ag-icon-maximize::before {\n  content: var(--ag-icon-font-code-maximize, "\\f11d");\n}\n\n.ag-icon-menu::before {\n  content: var(--ag-icon-font-code-menu, "\\f11e");\n}\n\n.ag-icon-minimize::before {\n  content: var(--ag-icon-font-code-minimize, "\\f11f");\n}\n\n.ag-icon-next::before {\n  content: var(--ag-icon-font-code-next, "\\f120");\n}\n\n.ag-icon-none::before {\n  content: var(--ag-icon-font-code-none, "\\f121");\n}\n\n.ag-icon-not-allowed::before {\n  content: var(--ag-icon-font-code-not-allowed, "\\f122");\n}\n\n.ag-icon-paste::before {\n  content: var(--ag-icon-font-code-paste, "\\f123");\n}\n\n.ag-icon-pin::before {\n  content: var(--ag-icon-font-code-pin, "\\f124");\n}\n\n.ag-icon-pivot::before {\n  content: var(--ag-icon-font-code-pivot, "\\f125");\n}\n\n.ag-icon-previous::before {\n  content: var(--ag-icon-font-code-previous, "\\f126");\n}\n\n.ag-icon-radio-button-off::before {\n  content: var(--ag-icon-font-code-radio-button-off, "\\f127");\n}\n\n.ag-icon-radio-button-on::before {\n  content: var(--ag-icon-font-code-radio-button-on, "\\f128");\n}\n\n.ag-icon-right::before {\n  content: var(--ag-icon-font-code-right, "\\f129");\n}\n\n.ag-icon-save::before {\n  content: var(--ag-icon-font-code-save, "\\f12a");\n}\n\n.ag-icon-small-down::before {\n  content: var(--ag-icon-font-code-small-down, "\\f12b");\n}\n\n.ag-icon-small-left::before {\n  content: var(--ag-icon-font-code-small-left, "\\f12c");\n}\n\n.ag-icon-small-right::before {\n  content: var(--ag-icon-font-code-small-right, "\\f12d");\n}\n\n.ag-icon-small-up::before {\n  content: var(--ag-icon-font-code-small-up, "\\f12e");\n}\n\n.ag-icon-tick::before {\n  content: var(--ag-icon-font-code-tick, "\\f12f");\n}\n\n.ag-icon-tree-closed::before {\n  content: var(--ag-icon-font-code-tree-closed, "\\f130");\n}\n\n.ag-icon-tree-indeterminate::before {\n  content: var(--ag-icon-font-code-tree-indeterminate, "\\f131");\n}\n\n.ag-icon-tree-open::before {\n  content: var(--ag-icon-font-code-tree-open, "\\f132");\n}\n\n.ag-icon-unlinked::before {\n  content: var(--ag-icon-font-code-unlinked, "\\f133");\n}\n\n.ag-icon-row-drag::before {\n  content: var(--ag-icon-font-code-grip);\n}\n\n.ag-left-arrow::before {\n  content: var(--ag-icon-font-code-left);\n}\n\n.ag-right-arrow::before {\n  content: var(--ag-icon-font-code-right);\n}\n\n[class*=ag-theme-] {\n  --ag-foreground-color: #000;\n  --ag-data-color: var(--ag-foreground-color);\n  --ag-secondary-foreground-color: var(--ag-foreground-color);\n  --ag-header-foreground-color: var(--ag-secondary-foreground-color);\n  --ag-disabled-foreground-color: rgba(0, 0, 0, 0.5);\n  --ag-background-color: #fff;\n  --ag-header-background-color: transparent;\n  --ag-tooltip-background-color: transparent;\n  --ag-subheader-background-color: transparent;\n  --ag-subheader-toolbar-background-color: transparent;\n  --ag-control-panel-background-color: transparent;\n  --ag-side-button-selected-background-color: var(--ag-control-panel-background-color);\n  --ag-selected-row-background-color: #BBB;\n  --ag-odd-row-background-color: var(--ag-background-color);\n  --ag-modal-overlay-background-color: rgba(255, 255, 255, 0.66);\n  --ag-row-hover-color: transparent;\n  --ag-column-hover-color: transparent;\n  --ag-range-selection-border-color: var(--ag-foreground-color);\n  --ag-range-selection-border-style: solid;\n  --ag-range-selection-background-color: rgba(0, 0, 0, 0.2);\n  --ag-range-selection-background-color-2: var(--ag-range-selection-background-color);\n  --ag-range-selection-background-color-3: var(--ag-range-selection-background-color);\n  --ag-range-selection-background-color-4: var(--ag-range-selection-background-color);\n  --ag-range-selection-highlight-color: var(--ag-range-selection-border-color);\n  --ag-selected-tab-underline-color: var(--ag-range-selection-border-color);\n  --ag-selected-tab-underline-width: 0;\n  --ag-selected-tab-underline-transition-speed: 0s;\n  --ag-range-selection-chart-category-background-color: rgba(0, 255, 132, 0.1);\n  --ag-range-selection-chart-background-color: rgba(0, 88, 255, 0.1);\n  --ag-header-cell-hover-background-color: transparent;\n  --ag-header-cell-moving-background-color: var(--ag-background-color);\n  --ag-value-change-value-highlight-background-color: rgba(22, 160, 133, 0.5);\n  --ag-value-change-delta-up-color: #43a047;\n  --ag-value-change-delta-down-color: #e53935;\n  --ag-chip-background-color: transparent;\n  --ag-borders: solid 1px;\n  --ag-border-color: rgba(0, 0, 0, 0.25);\n  --ag-borders-critical: var(--ag-borders);\n  --ag-borders-secondary: var(--ag-borders);\n  --ag-secondary-border-color: var(--ag-border-color);\n  --ag-row-border-style: solid;\n  --ag-row-border-color: var(--ag-secondary-border-color);\n  --ag-row-border-width: 1px;\n  --ag-cell-horizontal-border: solid transparent;\n  --ag-borders-input: var(--ag-borders-secondary);\n  --ag-input-border-color: var(--ag-secondary-border-color);\n  --ag-borders-input-invalid: solid 2px;\n  --ag-input-border-color-invalid: var(--ag-invalid-color);\n  --ag-borders-side-button: var(--ag-borders);\n  --ag-border-radius: 0px;\n  --ag-row-border-color: var(--ag-secondary-border-color);\n  --ag-header-column-separator-display: none;\n  --ag-header-column-separator-height: 100%;\n  --ag-header-column-separator-width: 1px;\n  --ag-header-column-separator-color: var(--ag-secondary-border-color);\n  --ag-header-column-resize-handle-display: none;\n  --ag-header-column-resize-handle-height: 50%;\n  --ag-header-column-resize-handle-width: 1px;\n  --ag-header-column-resize-handle-color: var(--ag-secondary-border-color);\n  --ag-invalid-color: red;\n  --ag-input-disabled-border-color: var(--ag-input-border-color);\n  --ag-input-disabled-background-color: transparent;\n  --ag-checkbox-background-color: transparent;\n  --ag-checkbox-border-radius: var(--ag-border-radius);\n  --ag-checkbox-checked-color: var(--ag-foreground-color);\n  --ag-checkbox-unchecked-color: var(--ag-foreground-color);\n  --ag-checkbox-indeterminate-color: var(--ag-checkbox-unchecked-color);\n  --ag-toggle-button-off-border-color: var(--ag-checkbox-unchecked-color);\n  --ag-toggle-button-off-background-color: var(--ag-checkbox-unchecked-color);\n  --ag-toggle-button-on-border-color: var(--ag-checkbox-checked-color);\n  --ag-toggle-button-on-background-color: var(--ag-checkbox-checked-color);\n  --ag-toggle-button-switch-background-color: var(--ag-background-color);\n  --ag-toggle-button-switch-border-color: var(--ag-toggle-button-off-border-color);\n  --ag-toggle-button-border-width: 1px;\n  --ag-toggle-button-height: var(--ag-icon-size);\n  --ag-toggle-button-width: calc(var(--ag-toggle-button-height) * 2);\n  --ag-input-focus-box-shadow: none;\n  --ag-input-focus-border-color: none;\n  --ag-minichart-selected-chart-color: var(--ag-checkbox-checked-color);\n  --ag-minichart-selected-page-color: var(--ag-checkbox-checked-color);\n  --ag-grid-size: 4px;\n  --ag-icon-size: 12px;\n  --ag-widget-container-horizontal-padding: calc(var(--ag-grid-size) * 1.5);\n  --ag-widget-container-vertical-padding: calc(var(--ag-grid-size) * 1.5);\n  --ag-widget-horizontal-spacing: calc(var(--ag-grid-size) * 2);\n  --ag-widget-vertical-spacing: var(--ag-grid-size);\n  --ag-cell-horizontal-padding: calc(var(--ag-grid-size) * 3);\n  --ag-cell-widget-spacing: var(--ag-cell-horizontal-padding);\n  --ag-row-height: calc(var(--ag-grid-size) * 6 + 1px);\n  --ag-header-height: var(--ag-row-height);\n  --ag-list-item-height: calc(var(--ag-grid-size) * 5);\n  --ag-column-select-indent-size: calc(var(--ag-grid-size) + var(--ag-icon-size));\n  --ag-set-filter-indent-size: calc(var(--ag-grid-size) + var(--ag-icon-size));\n  --ag-row-group-indent-size: calc(var(--ag-cell-widget-spacing) + var(--ag-icon-size));\n  --ag-filter-tool-panel-group-indent: 16px;\n  --ag-tab-min-width: 220px;\n  --ag-menu-min-width: 181px;\n  --ag-side-bar-panel-width: 200px;\n  --ag-font-family: "Helvetica Neue", sans-serif;\n  --ag-font-size: 14px;\n  --ag-card-radius: var(--ag-border-radius);\n  --ag-card-shadow: none;\n  --ag-popup-shadow: 5px 5px 10px rgba(0, 0, 0, 0.3);\n}\n\n.ag-root-wrapper, .ag-sticky-top, .ag-dnd-ghost {\n  background-color: var(--ag-background-color);\n}\n\n[class*=ag-theme-] {\n  -webkit-font-smoothing: antialiased;\n  font-family: var(--ag-font-family);\n  font-size: var(--ag-font-size);\n  line-height: normal;\n  color: var(--ag-foreground-color);\n}\n\nag-grid, ag-grid-angular, ag-grid-ng2, ag-grid-polymer, ag-grid-aurelia {\n  display: block;\n}\n\n.ag-hidden {\n  display: none !important;\n}\n\n.ag-invisible {\n  visibility: hidden !important;\n}\n\n.ag-no-transition {\n  transition: none !important;\n}\n\n.ag-drag-handle {\n  cursor: grab;\n}\n\n.ag-column-drop-wrapper {\n  display: flex;\n}\n\n.ag-column-drop-horizontal-half-width {\n  display: inline-block;\n  width: 50% !important;\n}\n\n.ag-unselectable {\n  -moz-user-select: none;\n  -webkit-user-select: none;\n  -ms-user-select: none;\n  user-select: none;\n}\n\n.ag-selectable {\n  -moz-user-select: text;\n  -webkit-user-select: text;\n  -ms-user-select: text;\n  user-select: text;\n}\n\n.ag-tab {\n  position: relative;\n}\n\n.ag-tab-guard {\n  position: absolute;\n  width: 0;\n  height: 0;\n  display: block;\n}\n\n.ag-select-agg-func-popup {\n  position: absolute;\n}\n\n.ag-input-wrapper, .ag-picker-field-wrapper {\n  display: flex;\n  flex: 1 1 auto;\n  align-items: center;\n  line-height: normal;\n  position: relative;\n}\n\n.ag-shake-left-to-right {\n  animation-direction: alternate;\n  animation-duration: 0.2s;\n  animation-iteration-count: infinite;\n  animation-name: ag-shake-left-to-right;\n}\n\n@keyframes ag-shake-left-to-right {\n  from {\n    padding-left: 6px;\n    padding-right: 2px;\n  }\n  to {\n    padding-left: 2px;\n    padding-right: 6px;\n  }\n}\n.ag-root-wrapper {\n  cursor: default;\n  position: relative;\n  display: flex;\n  flex-direction: column;\n  overflow: hidden;\n}\n.ag-root-wrapper.ag-layout-normal {\n  height: 100%;\n}\n\n.ag-watermark {\n  position: absolute;\n  bottom: 20px;\n  right: 25px;\n  opacity: 0.5;\n  transition: opacity 1s ease-out 3s;\n}\n.ag-watermark::before {\n  content: "";\n  background-image: url(data:image/svg+xml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0iVVRGLTgiIHN0YW5kYWxvbmU9Im5vIj8+CjwhRE9DVFlQRSBzdmcgUFVCTElDICItLy9XM0MvL0RURCBTVkcgMS4xLy9FTiIgImh0dHA6Ly93d3cudzMub3JnL0dyYXBoaWNzL1NWRy8xLjEvRFREL3N2ZzExLmR0ZCI+Cjxzdmcgd2lkdGg9IjEwMCUiIGhlaWdodD0iMTAwJSIgdmlld0JveD0iMCAwIDIzNSA0MCIgdmVyc2lvbj0iMS4xIiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHhtbG5zOnhsaW5rPSJodHRwOi8vd3d3LnczLm9yZy8xOTk5L3hsaW5rIiB4bWw6c3BhY2U9InByZXNlcnZlIiB4bWxuczpzZXJpZj0iaHR0cDovL3d3dy5zZXJpZi5jb20vIiBzdHlsZT0iZmlsbC1ydWxlOmV2ZW5vZGQ7Y2xpcC1ydWxlOmV2ZW5vZGQ7c3Ryb2tlLWxpbmVqb2luOnJvdW5kO3N0cm9rZS1taXRlcmxpbWl0OjI7Ij4KICAgIDxnIHRyYW5zZm9ybT0ibWF0cml4KDAuNjM1NzIzLDAsMCwwLjYzNTcyMywtNDkyLjkyMSwtMzIzLjYwOCkiPgogICAgICAgIDxwYXRoIGQ9Ik0xMDk5LjQsNTQ5LjRMMTA5OS40LDUzNi45TDEwNzguMSw1MzYuOUwxMDY1LjYsNTQ5LjRMMTA5OS40LDU0OS40WiIgc3R5bGU9ImZpbGw6cmdiKDI0LDI5LDMxKTtmaWxsLXJ1bGU6bm9uemVybzsiLz4KICAgICAgICA8cGF0aCBkPSJNMTEyMy40LDUxOC40TDEwOTYuNyw1MTguNEwxMDg0LjEsNTMwLjlMMTEyMy40LDUzMC45TDExMjMuNCw1MTguNFoiIHN0eWxlPSJmaWxsOnJnYigyNCwyOSwzMSk7ZmlsbC1ydWxlOm5vbnplcm87Ii8+CiAgICAgICAgPHBhdGggZD0iTTEwNTMuMiw1NjEuOUwxMDU5LjYsNTU1LjVMMTA4MS4yLDU1NS41TDEwODEuMiw1NjhMMTA1My4yLDU2OEwxMDUzLjIsNTYxLjlaIiBzdHlsZT0iZmlsbDpyZ2IoMjQsMjksMzEpO2ZpbGwtcnVsZTpub256ZXJvOyIvPgogICAgICAgIDxwYXRoIGQ9Ik0xMDU3LjksNTQzLjNMMTA3MS43LDU0My4zTDEwODQuMyw1MzAuOEwxMDU3LjksNTMwLjhMMTA1Ny45LDU0My4zWiIgc3R5bGU9ImZpbGw6cmdiKDI0LDI5LDMxKTtmaWxsLXJ1bGU6bm9uemVybzsiLz4KICAgICAgICA8cGF0aCBkPSJNMTA0Mi44LDU2MS45TDEwNTMuMiw1NjEuOUwxMDY1LjYsNTQ5LjRMMTA0Mi44LDU0OS40TDEwNDIuOCw1NjEuOVoiIHN0eWxlPSJmaWxsOnJnYigyNCwyOSwzMSk7ZmlsbC1ydWxlOm5vbnplcm87Ii8+CiAgICAgICAgPHBhdGggZD0iTTEwOTYuNyw1MTguNEwxMDkwLjMsNTI0LjhMMTA0OS41LDUyNC44TDEwNDkuNSw1MTIuM0wxMDk2LjcsNTEyLjNMMTA5Ni43LDUxOC40WiIgc3R5bGU9ImZpbGw6cmdiKDI0LDI5LDMxKTtmaWxsLXJ1bGU6bm9uemVybzsiLz4KICAgICAgICA8cGF0aCBkPSJNODI4LjYsNTU5LjdMODA5LDU1OS43TDgwNS42LDU2OC4xTDc5Nyw1NjguMUw4MTUuMSw1MjUuN0w4MjIuNiw1MjUuN0w4NDAuNyw1NjguMUw4MzIsNTY4LjFMODI4LjYsNTU5LjdaTTgyNS45LDU1M0w4MTguOCw1MzUuN0w4MTEuNyw1NTNMODI1LjksNTUzWiIgc3R5bGU9ImZpbGw6cmdiKDI0LDI5LDMxKTtmaWxsLXJ1bGU6bm9uemVybzsiLz4KICAgICAgICA8cGF0aCBkPSJNOTYwLjEsNTQxLjNDOTYyLjYsNTM3LjYgOTY4LjksNTM3LjIgOTcxLjUsNTM3LjJMOTcxLjUsNTQ0LjRDOTY4LjMsNTQ0LjQgOTY1LjEsNTQ0LjUgOTYzLjIsNTQ1LjlDOTYxLjMsNTQ3LjMgOTYwLjMsNTQ5LjIgOTYwLjMsNTUxLjVMOTYwLjMsNTY4LjFMOTUyLjUsNTY4LjFMOTUyLjUsNTM3LjJMOTYwLDUzNy4yTDk2MC4xLDU0MS4zWiIgc3R5bGU9ImZpbGw6cmdiKDI0LDI5LDMxKTtmaWxsLXJ1bGU6bm9uemVybzsiLz4KICAgICAgICA8cmVjdCB4PSI5NzUuOCIgeT0iNTM3LjIiIHdpZHRoPSI3LjgiIGhlaWdodD0iMzAuOSIgc3R5bGU9ImZpbGw6cmdiKDI0LDI5LDMxKTsiLz4KICAgICAgICA8cmVjdCB4PSI5NzUuOCIgeT0iNTIzLjQiIHdpZHRoPSI3LjgiIGhlaWdodD0iOS4yIiBzdHlsZT0iZmlsbDpyZ2IoMjQsMjksMzEpOyIvPgogICAgICAgIDxwYXRoIGQ9Ik0xMDIyLjMsNTIzLjRMMTAyMi4zLDU2OC4xTDEwMTQuOCw1NjguMUwxMDE0LjYsNTYzLjRDMTAxMy41LDU2NSAxMDEyLjEsNTY2LjMgMTAxMC40LDU2Ny4zQzEwMDguNyw1NjguMiAxMDA2LjYsNTY4LjcgMTAwNC4yLDU2OC43QzEwMDIuMSw1NjguNyAxMDAwLjEsNTY4LjMgOTk4LjQsNTY3LjZDOTk2LjYsNTY2LjggOTk1LDU2NS44IDk5My43LDU2NC40Qzk5Mi40LDU2MyA5OTEuMyw1NjEuMyA5OTAuNiw1NTkuNEM5ODkuOCw1NTcuNSA5ODkuNSw1NTUuMyA5ODkuNSw1NTIuOUM5ODkuNSw1NTAuNSA5ODkuOSw1NDguMyA5OTAuNiw1NDYuM0M5OTEuNCw1NDQuMyA5OTIuNCw1NDIuNiA5OTMuNyw1NDEuMkM5OTUsNTM5LjggOTk2LjYsNTM4LjcgOTk4LjQsNTM3LjlDMTAwMC4yLDUzNy4xIDEwMDIuMSw1MzYuNyAxMDA0LjIsNTM2LjdDMTAwNi42LDUzNi43IDEwMDguNiw1MzcuMSAxMDEwLjMsNTM4QzEwMTIsNTM4LjkgMTAxMy40LDU0MC4xIDEwMTQuNSw1NDEuOEwxMDE0LjUsNTIzLjVMMTAyMi4zLDUyMy41TDEwMjIuMyw1MjMuNFpNMTAwNS45LDU2MkMxMDA4LjUsNTYyIDEwMTAuNSw1NjEuMSAxMDEyLjEsNTU5LjRDMTAxMy43LDU1Ny43IDEwMTQuNSw1NTUuNCAxMDE0LjUsNTUyLjZDMTAxNC41LDU0OS44IDEwMTMuNyw1NDcuNiAxMDEyLjEsNTQ1LjhDMTAxMC41LDU0NC4xIDEwMDguNSw1NDMuMiAxMDA1LjksNTQzLjJDMTAwMy40LDU0My4yIDEwMDEuMyw1NDQuMSA5OTkuOCw1NDUuOEM5OTguMiw1NDcuNSA5OTcuNCw1NDkuOCA5OTcuNCw1NTIuNkM5OTcuNCw1NTUuNCA5OTguMiw1NTcuNiA5OTkuOCw1NTkuM0MxMDAxLjQsNTYxLjEgMTAwMy40LDU2MiAxMDA1LjksNTYyIiBzdHlsZT0iZmlsbDpyZ2IoMjQsMjksMzEpO2ZpbGwtcnVsZTpub256ZXJvOyIvPgogICAgICAgIDxwYXRoIGQ9Ik04ODUuOCw1NDQuMkw4NjYuNSw1NDQuMkw4NjYuNSw1NTAuOUw4NzcuNSw1NTAuOUM4NzcuMiw1NTQuMyA4NzUuOSw1NTYuOSA4NzMuNyw1NTlDODcxLjUsNTYxIDg2OC43LDU2MiA4NjUuMSw1NjJDODYzLjEsNTYyIDg2MS4yLDU2MS42IDg1OS42LDU2MC45Qzg1Ny45LDU2MC4yIDg1Ni41LDU1OS4yIDg1NS4zLDU1Ny44Qzg1NC4xLDU1Ni41IDg1My4yLDU1NC45IDg1Mi41LDU1M0M4NTEuOCw1NTEuMSA4NTEuNSw1NDkuMSA4NTEuNSw1NDYuOEM4NTEuNSw1NDQuNSA4NTEuOCw1NDIuNSA4NTIuNSw1NDAuNkM4NTMuMSw1MzguNyA4NTQuMSw1MzcuMiA4NTUuMyw1MzUuOEM4NTYuNSw1MzQuNSA4NTcuOSw1MzMuNSA4NTkuNiw1MzIuN0M4NjEuMyw1MzIgODYzLjEsNTMxLjYgODY1LjIsNTMxLjZDODY5LjQsNTMxLjYgODcyLjYsNTMyLjYgODc0LjgsNTM0LjZMODgwLDUyOS40Qzg3Ni4xLDUyNi40IDg3MS4xLDUyNC44IDg2NS4yLDUyNC44Qzg2MS45LDUyNC44IDg1OC45LDUyNS4zIDg1Ni4yLDUyNi40Qzg1My41LDUyNy41IDg1MS4yLDUyOC45IDg0OS4zLDUzMC44Qzg0Ny40LDUzMi43IDg0NS45LDUzNSA4NDQuOSw1MzcuN0M4NDMuOSw1NDAuNCA4NDMuNCw1NDMuNCA4NDMuNCw1NDYuNkM4NDMuNCw1NDkuOCA4NDMuOSw1NTIuOCA4NDUsNTU1LjVDODQ2LjEsNTU4LjIgODQ3LjUsNTYwLjUgODQ5LjQsNTYyLjRDODUxLjMsNTY0LjMgODUzLjYsNTY1LjggODU2LjMsNTY2LjhDODU5LDU2Ny45IDg2Miw1NjguNCA4NjUuMiw1NjguNEM4NjguNCw1NjguNCA4NzEuMyw1NjcuOSA4NzMuOSw1NjYuOEM4NzYuNSw1NjUuNyA4NzguNyw1NjQuMyA4ODAuNSw1NjIuNEM4ODIuMyw1NjAuNSA4ODMuNyw1NTguMiA4ODQuNyw1NTUuNUM4ODUuNyw1NTIuOCA4ODYuMiw1NDkuOCA4ODYuMiw1NDYuNkw4ODYuMiw1NDUuM0M4ODUuOSw1NDUuMSA4ODUuOCw1NDQuNiA4ODUuOCw1NDQuMiIgc3R5bGU9ImZpbGw6cmdiKDI0LDI5LDMxKTtmaWxsLXJ1bGU6bm9uemVybzsiLz4KICAgICAgICA8cGF0aCBkPSJNOTQ2LjgsNTQ0LjJMOTI3LjUsNTQ0LjJMOTI3LjUsNTUwLjlMOTM4LjUsNTUwLjlDOTM4LjIsNTU0LjMgOTM2LjksNTU2LjkgOTM0LjcsNTU5QzkzMi41LDU2MSA5MjkuNyw1NjIgOTI2LjEsNTYyQzkyNC4xLDU2MiA5MjIuMiw1NjEuNiA5MjAuNiw1NjAuOUM5MTguOSw1NjAuMiA5MTcuNSw1NTkuMiA5MTYuMyw1NTcuOEM5MTUuMSw1NTYuNSA5MTQuMiw1NTQuOSA5MTMuNSw1NTNDOTEyLjgsNTUxLjEgOTEyLjUsNTQ5LjEgOTEyLjUsNTQ2LjhDOTEyLjUsNTQ0LjUgOTEyLjgsNTQyLjUgOTEzLjUsNTQwLjZDOTE0LjEsNTM4LjcgOTE1LjEsNTM3LjIgOTE2LjMsNTM1LjhDOTE3LjUsNTM0LjUgOTE4LjksNTMzLjUgOTIwLjYsNTMyLjdDOTIyLjMsNTMyIDkyNC4xLDUzMS42IDkyNi4yLDUzMS42QzkzMC40LDUzMS42IDkzMy42LDUzMi42IDkzNS44LDUzNC42TDk0MSw1MjkuNEM5MzcuMSw1MjYuNCA5MzIuMSw1MjQuOCA5MjYuMiw1MjQuOEM5MjIuOSw1MjQuOCA5MTkuOSw1MjUuMyA5MTcuMiw1MjYuNEM5MTQuNSw1MjcuNSA5MTIuMiw1MjguOSA5MTAuMyw1MzAuOEM5MDguNCw1MzIuNyA5MDYuOSw1MzUgOTA1LjksNTM3LjdDOTA0LjksNTQwLjQgOTA0LjQsNTQzLjQgOTA0LjQsNTQ2LjZDOTA0LjQsNTQ5LjggOTA0LjksNTUyLjggOTA2LDU1NS41QzkwNy4xLDU1OC4yIDkwOC41LDU2MC41IDkxMC40LDU2Mi40QzkxMi4zLDU2NC4zIDkxNC42LDU2NS44IDkxNy4zLDU2Ni44QzkyMCw1NjcuOSA5MjMsNTY4LjQgOTI2LjIsNTY4LjRDOTI5LjQsNTY4LjQgOTMyLjMsNTY3LjkgOTM0LjksNTY2LjhDOTM3LjUsNTY1LjcgOTM5LjcsNTY0LjMgOTQxLjUsNTYyLjRDOTQzLjMsNTYwLjUgOTQ0LjcsNTU4LjIgOTQ1LjcsNTU1LjVDOTQ2LjcsNTUyLjggOTQ3LjIsNTQ5LjggOTQ3LjIsNTQ2LjZMOTQ3LjIsNTQ1LjNDOTQ2LjksNTQ1LjEgOTQ2LjgsNTQ0LjYgOTQ2LjgsNTQ0LjIiIHN0eWxlPSJmaWxsOnJnYigyNCwyOSwzMSk7ZmlsbC1ydWxlOm5vbnplcm87Ii8+CiAgICA8L2c+Cjwvc3ZnPgo=);\n  background-repeat: no-repeat;\n  background-size: 170px 40px;\n  display: block;\n  height: 40px;\n  width: 170px;\n  opacity: 0.5;\n}\n\n.ag-watermark-text {\n  opacity: 0.5;\n  font-weight: bold;\n  font-family: Impact, sans-serif;\n  font-size: 19px;\n  padding-left: 0.7rem;\n}\n\n.ag-root-wrapper-body {\n  display: flex;\n  flex-direction: row;\n}\n.ag-root-wrapper-body.ag-layout-normal {\n  flex: 1 1 auto;\n  height: 0;\n  min-height: 0;\n}\n\n.ag-root {\n  position: relative;\n  display: flex;\n  flex-direction: column;\n}\n.ag-root.ag-layout-normal, .ag-root.ag-layout-auto-height {\n  overflow: hidden;\n  flex: 1 1 auto;\n  width: 0;\n}\n.ag-root.ag-layout-normal {\n  height: 100%;\n}\n\n.ag-header-viewport,\n.ag-floating-top-viewport,\n.ag-body-viewport,\n.ag-center-cols-viewport,\n.ag-floating-bottom-viewport,\n.ag-body-horizontal-scroll-viewport,\n.ag-body-vertical-scroll-viewport,\n.ag-virtual-list-viewport,\n.ag-sticky-top-viewport {\n  position: relative;\n  height: 100%;\n  min-width: 0px;\n  overflow: hidden;\n  flex: 1 1 auto;\n}\n\n.ag-body-viewport {\n  display: flex;\n}\n.ag-body-viewport.ag-layout-normal {\n  overflow-y: auto;\n  -webkit-overflow-scrolling: touch;\n}\n\n.ag-center-cols-viewport {\n  width: 100%;\n  overflow-x: auto;\n}\n\n.ag-body-horizontal-scroll-viewport {\n  overflow-x: scroll;\n}\n\n.ag-body-vertical-scroll-viewport {\n  overflow-y: scroll;\n}\n\n.ag-virtual-list-viewport {\n  overflow: auto;\n  width: 100%;\n}\n\n.ag-header-container,\n.ag-floating-top-container,\n.ag-body-container,\n.ag-pinned-right-cols-container,\n.ag-center-cols-container,\n.ag-pinned-left-cols-container,\n.ag-floating-bottom-container,\n.ag-body-horizontal-scroll-container,\n.ag-body-vertical-scroll-container,\n.ag-full-width-container,\n.ag-floating-bottom-full-width-container,\n.ag-virtual-list-container,\n.ag-sticky-top-container {\n  position: relative;\n}\n\n.ag-header-container,\n.ag-floating-top-container,\n.ag-floating-bottom-container,\n.ag-sticky-top-container {\n  height: 100%;\n  white-space: nowrap;\n}\n\n.ag-center-cols-container {\n  display: block;\n}\n\n.ag-pinned-right-cols-container {\n  display: block;\n}\n\n.ag-body-horizontal-scroll-container {\n  height: 100%;\n}\n\n.ag-body-vertical-scroll-container {\n  width: 100%;\n}\n\n.ag-full-width-container,\n.ag-floating-top-full-width-container,\n.ag-floating-bottom-full-width-container,\n.ag-sticky-top-full-width-container {\n  position: absolute;\n  top: 0px;\n  pointer-events: none;\n}\n.ag-ltr .ag-full-width-container,\n.ag-ltr .ag-floating-top-full-width-container,\n.ag-ltr .ag-floating-bottom-full-width-container,\n.ag-ltr .ag-sticky-top-full-width-container {\n  left: 0;\n}\n.ag-rtl .ag-full-width-container,\n.ag-rtl .ag-floating-top-full-width-container,\n.ag-rtl .ag-floating-bottom-full-width-container,\n.ag-rtl .ag-sticky-top-full-width-container {\n  right: 0;\n}\n\n.ag-floating-bottom-full-width-container, .ag-floating-top-full-width-container {\n  display: inline-block;\n  overflow: hidden;\n  height: 100%;\n  width: 100%;\n}\n\n.ag-virtual-list-container {\n  overflow: hidden;\n}\n\n.ag-center-cols-clipper {\n  flex: 1 1 auto;\n  min-width: 0;\n  overflow: hidden;\n  min-height: 100%;\n  transform: translate3d(0, 0, 0);\n}\n\n.ag-body {\n  position: relative;\n  display: flex;\n  flex: 1 1 auto;\n  flex-direction: row !important;\n  min-height: 0;\n}\n\n.ag-body-clipper {\n  overflow: hidden;\n  min-width: 0px;\n  flex: 1 1 auto;\n  height: 100%;\n  transform: translate3d(0, 0, 0);\n}\n\n.ag-body-horizontal-scroll,\n.ag-body-vertical-scroll {\n  min-height: 0;\n  min-width: 0;\n  display: flex;\n  position: relative;\n}\n.ag-body-horizontal-scroll.ag-scrollbar-invisible,\n.ag-body-vertical-scroll.ag-scrollbar-invisible {\n  position: absolute;\n  bottom: 0;\n}\n.ag-body-horizontal-scroll.ag-scrollbar-invisible.ag-apple-scrollbar,\n.ag-body-vertical-scroll.ag-scrollbar-invisible.ag-apple-scrollbar {\n  opacity: 0;\n  transition: opacity 400ms;\n  visibility: hidden;\n}\n.ag-body-horizontal-scroll.ag-scrollbar-invisible.ag-apple-scrollbar.ag-scrollbar-scrolling, .ag-body-horizontal-scroll.ag-scrollbar-invisible.ag-apple-scrollbar.ag-scrollbar-active,\n.ag-body-vertical-scroll.ag-scrollbar-invisible.ag-apple-scrollbar.ag-scrollbar-scrolling,\n.ag-body-vertical-scroll.ag-scrollbar-invisible.ag-apple-scrollbar.ag-scrollbar-active {\n  visibility: visible;\n  opacity: 1;\n}\n\n.ag-body-horizontal-scroll {\n  width: 100%;\n}\n.ag-body-horizontal-scroll.ag-scrollbar-invisible {\n  left: 0;\n  right: 0;\n}\n\n.ag-body-vertical-scroll {\n  height: 100%;\n}\n.ag-body-vertical-scroll.ag-scrollbar-invisible {\n  top: 0;\n  z-index: 10;\n}\n.ag-ltr .ag-body-vertical-scroll.ag-scrollbar-invisible {\n  right: 0;\n}\n.ag-rtl .ag-body-vertical-scroll.ag-scrollbar-invisible {\n  left: 0;\n}\n\n.ag-force-vertical-scroll {\n  overflow-y: scroll !important;\n}\n\n.ag-horizontal-left-spacer, .ag-horizontal-right-spacer {\n  height: 100%;\n  min-width: 0;\n  overflow-x: scroll;\n}\n.ag-horizontal-left-spacer.ag-scroller-corner, .ag-horizontal-right-spacer.ag-scroller-corner {\n  overflow-x: hidden;\n}\n\n.ag-header, .ag-pinned-left-header, .ag-pinned-right-header {\n  display: inline-block;\n  overflow: hidden;\n  position: relative;\n}\n\n.ag-header-cell-sortable .ag-header-cell-label {\n  cursor: pointer;\n}\n\n.ag-header {\n  display: flex;\n  width: 100%;\n  white-space: nowrap;\n}\n\n.ag-pinned-left-header {\n  height: 100%;\n}\n\n.ag-pinned-right-header {\n  height: 100%;\n}\n\n.ag-header-row {\n  position: absolute;\n}\n\n.ag-header-row:not(.ag-header-row-column-group) {\n  overflow: hidden;\n}\n\n.ag-header.ag-header-allow-overflow .ag-header-row {\n  overflow: visible;\n}\n\n.ag-header-cell {\n  display: inline-flex;\n  align-items: center;\n  position: absolute;\n  height: 100%;\n  overflow: hidden;\n}\n\n.ag-header-cell.ag-header-active .ag-header-cell-menu-button {\n  opacity: 1;\n}\n\n.ag-header-cell-menu-button:not(.ag-header-menu-always-show) {\n  transition: opacity 0.2s;\n  opacity: 0;\n}\n\n.ag-header-group-cell-label, .ag-header-cell-label {\n  display: flex;\n  flex: 1 1 auto;\n  overflow: hidden;\n  align-items: center;\n  text-overflow: ellipsis;\n  align-self: stretch;\n}\n\n.ag-header-group-cell-label.ag-sticky-label {\n  position: sticky;\n  flex: none;\n}\n\n.ag-header-cell-text {\n  overflow: hidden;\n  text-overflow: ellipsis;\n}\n\n.ag-header-cell:not(.ag-header-cell-auto-height) .ag-header-cell-comp-wrapper {\n  height: 100%;\n  display: flex;\n  align-items: center;\n}\n\n.ag-header-cell-comp-wrapper {\n  width: 100%;\n  overflow: hidden;\n}\n\n.ag-header-cell-wrap-text .ag-header-cell-comp-wrapper {\n  white-space: normal;\n}\n\n.ag-right-aligned-header .ag-header-cell-label {\n  flex-direction: row-reverse;\n}\n\n.ag-header-group-text {\n  overflow: hidden;\n  text-overflow: ellipsis;\n  white-space: nowrap;\n}\n\n.ag-header-cell-resize {\n  position: absolute;\n  z-index: 2;\n  height: 100%;\n  width: 8px;\n  top: 0;\n  cursor: ew-resize;\n}\n.ag-ltr .ag-header-cell-resize {\n  right: -4px;\n}\n.ag-rtl .ag-header-cell-resize {\n  left: -4px;\n}\n\n.ag-pinned-left-header .ag-header-cell-resize {\n  right: -4px;\n}\n\n.ag-pinned-right-header .ag-header-cell-resize {\n  left: -4px;\n}\n\n.ag-header-select-all {\n  display: flex;\n}\n\n.ag-column-moving .ag-cell {\n  transition: left 0.2s;\n}\n.ag-column-moving .ag-header-cell {\n  transition: left 0.2s;\n}\n.ag-column-moving .ag-header-group-cell {\n  transition: left 0.2s, width 0.2s;\n}\n\n.ag-column-panel {\n  display: flex;\n  flex-direction: column;\n  overflow: hidden;\n  flex: 1 1 auto;\n}\n\n.ag-column-select {\n  position: relative;\n  display: flex;\n  flex-direction: column;\n  overflow: hidden;\n  flex: 3 1 0px;\n}\n\n.ag-column-select-header {\n  position: relative;\n  display: flex;\n  flex: none;\n}\n\n.ag-column-select-header-icon {\n  position: relative;\n}\n\n.ag-column-select-header-filter-wrapper {\n  flex: 1 1 auto;\n}\n\n.ag-column-select-header-filter {\n  width: 100%;\n}\n\n.ag-column-select-list {\n  flex: 1 1 0px;\n  overflow: hidden;\n}\n\n.ag-column-drop {\n  position: relative;\n  display: inline-flex;\n  align-items: center;\n  overflow: auto;\n  width: 100%;\n}\n\n.ag-column-drop-list {\n  display: flex;\n  align-items: center;\n}\n\n.ag-column-drop-cell {\n  position: relative;\n  display: flex;\n  align-items: center;\n}\n\n.ag-column-drop-cell-text {\n  overflow: hidden;\n  flex: 1 1 auto;\n  text-overflow: ellipsis;\n  white-space: nowrap;\n}\n\n.ag-column-drop-vertical {\n  display: flex;\n  flex-direction: column;\n  overflow: hidden;\n  align-items: stretch;\n  flex: 1 1 0px;\n}\n\n.ag-column-drop-vertical-title-bar {\n  display: flex;\n  align-items: center;\n  flex: none;\n}\n\n.ag-column-drop-vertical-list {\n  position: relative;\n  align-items: stretch;\n  flex-grow: 1;\n  flex-direction: column;\n  overflow-x: auto;\n}\n.ag-column-drop-vertical-list > * {\n  flex: none;\n}\n\n.ag-column-drop-empty .ag-column-drop-vertical-list {\n  overflow: hidden;\n}\n\n.ag-column-drop-vertical-empty-message {\n  display: block;\n}\n\n.ag-column-drop.ag-column-drop-horizontal {\n  white-space: nowrap;\n  overflow: hidden;\n}\n\n.ag-column-drop-cell-button {\n  cursor: pointer;\n}\n\n.ag-filter-toolpanel {\n  flex: 1 1 0px;\n  min-width: 0;\n}\n\n.ag-filter-toolpanel-header {\n  position: relative;\n}\n\n.ag-filter-toolpanel-header, .ag-filter-toolpanel-search {\n  display: flex;\n  align-items: center;\n}\n.ag-filter-toolpanel-header > *, .ag-filter-toolpanel-search > * {\n  display: flex;\n  align-items: center;\n}\n\n.ag-filter-apply-panel {\n  display: flex;\n  justify-content: flex-end;\n  overflow: hidden;\n}\n\n.ag-row-animation .ag-row {\n  transition: transform 0.4s, top 0.4s, background-color 0.1s, opacity 0.2s;\n}\n\n.ag-row-animation .ag-row.ag-after-created {\n  transition: transform 0.4s, top 0.4s, height 0.4s, background-color 0.1s, opacity 0.2s;\n}\n\n.ag-row-no-animation .ag-row {\n  transition: background-color 0.1s;\n}\n\n.ag-row {\n  white-space: nowrap;\n  width: 100%;\n}\n\n.ag-row-loading {\n  display: flex;\n  align-items: center;\n}\n\n.ag-row-position-absolute {\n  position: absolute;\n}\n\n.ag-row-position-relative {\n  position: relative;\n}\n\n.ag-full-width-row {\n  overflow: hidden;\n  pointer-events: all;\n}\n\n.ag-row-inline-editing {\n  z-index: 1;\n}\n\n.ag-row-dragging {\n  z-index: 2;\n}\n\n.ag-stub-cell {\n  display: flex;\n  align-items: center;\n}\n\n.ag-cell {\n  display: inline-block;\n  position: absolute;\n  white-space: nowrap;\n  height: 100%;\n}\n\n.ag-cell-value {\n  flex: 1 1 auto;\n}\n\n.ag-cell-value, .ag-group-value {\n  overflow: hidden;\n  text-overflow: ellipsis;\n}\n\n.ag-cell-wrap-text {\n  white-space: normal;\n  word-break: break-all;\n}\n\n.ag-cell-wrapper {\n  display: flex;\n  align-items: center;\n}\n.ag-cell-wrapper.ag-row-group {\n  align-items: flex-start;\n}\n\n.ag-sparkline-wrapper {\n  position: absolute;\n  height: 100%;\n  width: 100%;\n  left: 0;\n  top: 0;\n}\n\n.ag-full-width-row .ag-cell-wrapper.ag-row-group {\n  height: 100%;\n  align-items: center;\n}\n\n.ag-cell-inline-editing {\n  z-index: 1;\n}\n.ag-cell-inline-editing .ag-cell-wrapper,\n.ag-cell-inline-editing .ag-cell-edit-wrapper,\n.ag-cell-inline-editing .ag-cell-editor,\n.ag-cell-inline-editing .ag-cell-editor .ag-wrapper,\n.ag-cell-inline-editing .ag-cell-editor input {\n  height: 100%;\n  width: 100%;\n  line-height: normal;\n}\n\n.ag-cell .ag-icon {\n  display: inline-block;\n  vertical-align: middle;\n}\n\n.ag-set-filter-item {\n  display: flex;\n  align-items: center;\n  height: 100%;\n}\n\n.ag-set-filter-item-checkbox {\n  display: flex;\n  overflow: hidden;\n}\n\n.ag-set-filter-group-icons {\n  display: block;\n}\n.ag-set-filter-group-icons > * {\n  cursor: pointer;\n}\n\n.ag-filter-body-wrapper {\n  display: flex;\n  flex-direction: column;\n}\n\n.ag-filter-filter {\n  flex: 1 1 0px;\n}\n\n.ag-filter-condition {\n  display: flex;\n  justify-content: center;\n}\n\n.ag-floating-filter-body {\n  position: relative;\n  display: flex;\n  flex: 1 1 auto;\n  height: 100%;\n}\n\n.ag-floating-filter-full-body {\n  display: flex;\n  flex: 1 1 auto;\n  height: 100%;\n  width: 100%;\n  align-items: center;\n  overflow: hidden;\n}\n\n.ag-floating-filter-full-body > div {\n  flex: 1 1 auto;\n}\n\n.ag-floating-filter-input {\n  align-items: center;\n  display: flex;\n  width: 100%;\n}\n.ag-floating-filter-input > * {\n  flex: 1 1 auto;\n}\n\n.ag-floating-filter-button {\n  display: flex;\n  flex: none;\n}\n\n.ag-dnd-ghost {\n  position: absolute;\n  display: inline-flex;\n  align-items: center;\n  cursor: move;\n  white-space: nowrap;\n  z-index: 9999;\n}\n\n.ag-overlay {\n  height: 100%;\n  left: 0;\n  pointer-events: none;\n  position: absolute;\n  top: 0;\n  width: 100%;\n}\n\n.ag-overlay-panel {\n  display: flex;\n  height: 100%;\n  width: 100%;\n}\n\n.ag-overlay-wrapper {\n  display: flex;\n  flex: none;\n  width: 100%;\n  height: 100%;\n  align-items: center;\n  justify-content: center;\n  text-align: center;\n}\n\n.ag-overlay-loading-wrapper {\n  pointer-events: all;\n}\n\n.ag-popup-child {\n  z-index: 5;\n  top: 0;\n}\n\n.ag-popup-editor {\n  position: absolute;\n  z-index: 1;\n  -moz-user-select: none;\n  -webkit-user-select: none;\n  -ms-user-select: none;\n  user-select: none;\n}\n\n.ag-large-text-input {\n  display: block;\n}\n\n.ag-virtual-list-item {\n  position: absolute;\n  width: 100%;\n}\n\n.ag-floating-top {\n  overflow: hidden;\n  white-space: nowrap;\n  width: 100%;\n  position: relative;\n  display: flex;\n}\n\n.ag-pinned-left-floating-top {\n  display: inline-block;\n  overflow: hidden;\n  position: relative;\n  min-width: 0px;\n}\n\n.ag-pinned-right-floating-top {\n  display: inline-block;\n  overflow: hidden;\n  position: relative;\n  min-width: 0px;\n}\n\n.ag-floating-bottom {\n  overflow: hidden;\n  white-space: nowrap;\n  width: 100%;\n  position: relative;\n  display: flex;\n}\n\n.ag-pinned-left-floating-bottom {\n  display: inline-block;\n  overflow: hidden;\n  position: relative;\n  min-width: 0px;\n}\n\n.ag-pinned-right-floating-bottom {\n  display: inline-block;\n  overflow: hidden;\n  position: relative;\n  min-width: 0px;\n}\n\n.ag-sticky-top {\n  position: absolute;\n  display: flex;\n  width: 100%;\n}\n\n.ag-pinned-left-sticky-top,\n.ag-pinned-right-sticky-top {\n  position: relative;\n  height: 100%;\n  overflow: hidden;\n}\n\n.ag-sticky-top-full-width-container {\n  overflow: hidden;\n  width: 100%;\n  height: 100%;\n}\n\n.ag-dialog, .ag-panel {\n  display: flex;\n  flex-direction: column;\n  position: relative;\n  overflow: hidden;\n}\n\n.ag-panel-title-bar {\n  display: flex;\n  flex: none;\n  align-items: center;\n  cursor: default;\n}\n\n.ag-panel-title-bar-title {\n  flex: 1 1 auto;\n}\n\n.ag-panel-title-bar-buttons {\n  display: flex;\n}\n\n.ag-panel-title-bar-button {\n  cursor: pointer;\n}\n\n.ag-panel-content-wrapper {\n  display: flex;\n  flex: 1 1 auto;\n  position: relative;\n  overflow: hidden;\n}\n\n.ag-dialog {\n  position: absolute;\n}\n\n.ag-resizer {\n  position: absolute;\n  pointer-events: none;\n  z-index: 1;\n  -moz-user-select: none;\n  -webkit-user-select: none;\n  -ms-user-select: none;\n  user-select: none;\n}\n.ag-resizer.ag-resizer-topLeft {\n  top: 0;\n  left: 0;\n  height: 5px;\n  width: 5px;\n  cursor: nwse-resize;\n}\n.ag-resizer.ag-resizer-top {\n  top: 0;\n  left: 5px;\n  right: 5px;\n  height: 5px;\n  cursor: ns-resize;\n}\n.ag-resizer.ag-resizer-topRight {\n  top: 0;\n  right: 0;\n  height: 5px;\n  width: 5px;\n  cursor: nesw-resize;\n}\n.ag-resizer.ag-resizer-right {\n  top: 5px;\n  right: 0;\n  bottom: 5px;\n  width: 5px;\n  cursor: ew-resize;\n}\n.ag-resizer.ag-resizer-bottomRight {\n  bottom: 0;\n  right: 0;\n  height: 5px;\n  width: 5px;\n  cursor: nwse-resize;\n}\n.ag-resizer.ag-resizer-bottom {\n  bottom: 0;\n  left: 5px;\n  right: 5px;\n  height: 5px;\n  cursor: ns-resize;\n}\n.ag-resizer.ag-resizer-bottomLeft {\n  bottom: 0;\n  left: 0;\n  height: 5px;\n  width: 5px;\n  cursor: nesw-resize;\n}\n.ag-resizer.ag-resizer-left {\n  left: 0;\n  top: 5px;\n  bottom: 5px;\n  width: 5px;\n  cursor: ew-resize;\n}\n\n.ag-tooltip {\n  position: absolute;\n  pointer-events: none;\n  z-index: 99999;\n}\n\n.ag-tooltip-custom {\n  position: absolute;\n  pointer-events: none;\n  z-index: 99999;\n}\n\n.ag-value-slide-out {\n  margin-right: 5px;\n  opacity: 1;\n  transition: opacity 3s, margin-right 3s;\n  transition-timing-function: linear;\n}\n\n.ag-value-slide-out-end {\n  margin-right: 10px;\n  opacity: 0;\n}\n\n.ag-opacity-zero {\n  opacity: 0 !important;\n}\n\n.ag-menu {\n  max-height: 100%;\n  overflow-y: auto;\n  position: absolute;\n  -moz-user-select: none;\n  -webkit-user-select: none;\n  -ms-user-select: none;\n  user-select: none;\n}\n\n.ag-menu-column-select-wrapper {\n  height: 265px;\n  overflow: auto;\n}\n.ag-menu-column-select-wrapper .ag-column-select {\n  height: 100%;\n}\n\n.ag-menu-list {\n  display: table;\n  width: 100%;\n}\n\n.ag-menu-option, .ag-menu-separator {\n  display: table-row;\n}\n\n.ag-menu-option-part, .ag-menu-separator-part {\n  display: table-cell;\n  vertical-align: middle;\n}\n\n.ag-menu-option-text {\n  white-space: nowrap;\n}\n\n.ag-compact-menu-option {\n  width: 100%;\n  display: flex;\n  flex-wrap: nowrap;\n}\n\n.ag-compact-menu-option-text {\n  white-space: nowrap;\n  flex: 1 1 auto;\n}\n\n.ag-rich-select {\n  cursor: default;\n  outline: none;\n}\n\n.ag-rich-select-value {\n  display: flex;\n  align-items: center;\n}\n\n.ag-rich-select-value-icon {\n  flex: 1 1 auto;\n  order: 1;\n}\n.ag-ltr .ag-rich-select-value-icon {\n  text-align: right;\n}\n.ag-rtl .ag-rich-select-value-icon {\n  text-align: left;\n}\n\n.ag-rich-select-list {\n  position: relative;\n}\n\n.ag-rich-select-virtual-list-item {\n  display: flex;\n}\n\n.ag-rich-select-row {\n  display: flex;\n  flex: 1 1 auto;\n  align-items: center;\n  white-space: nowrap;\n  overflow: hidden;\n}\n\n.ag-paging-panel {\n  align-items: center;\n  display: flex;\n  justify-content: flex-end;\n}\n\n.ag-paging-page-summary-panel {\n  display: flex;\n  align-items: center;\n}\n\n.ag-paging-button {\n  position: relative;\n}\n\n.ag-disabled .ag-paging-page-summary-panel {\n  pointer-events: none;\n}\n\n.ag-tool-panel-wrapper {\n  display: flex;\n  overflow-y: auto;\n  overflow-x: hidden;\n  cursor: default;\n  -moz-user-select: none;\n  -webkit-user-select: none;\n  -ms-user-select: none;\n  user-select: none;\n}\n\n.ag-column-select-column,\n.ag-column-select-column-group,\n.ag-select-agg-func-item {\n  position: relative;\n  align-items: center;\n  display: flex;\n  flex-direction: row;\n  flex-wrap: nowrap;\n  text-overflow: ellipsis;\n  white-space: nowrap;\n  height: 100%;\n}\n.ag-column-select-column > *,\n.ag-column-select-column-group > *,\n.ag-select-agg-func-item > * {\n  flex: none;\n}\n\n.ag-column-select-checkbox {\n  display: flex;\n}\n\n.ag-tool-panel-horizontal-resize {\n  cursor: ew-resize;\n  height: 100%;\n  position: absolute;\n  top: 0;\n  width: 5px;\n  z-index: 1;\n}\n\n.ag-ltr .ag-side-bar-left .ag-tool-panel-horizontal-resize {\n  right: -3px;\n}\n.ag-rtl .ag-side-bar-left .ag-tool-panel-horizontal-resize {\n  left: -3px;\n}\n\n.ag-ltr .ag-side-bar-right .ag-tool-panel-horizontal-resize {\n  left: -3px;\n}\n.ag-rtl .ag-side-bar-right .ag-tool-panel-horizontal-resize {\n  right: -3px;\n}\n\n.ag-details-row {\n  width: 100%;\n}\n\n.ag-details-row-fixed-height {\n  height: 100%;\n}\n\n.ag-details-grid {\n  width: 100%;\n}\n\n.ag-details-grid-fixed-height {\n  height: 100%;\n}\n\n.ag-header-group-cell {\n  display: flex;\n  align-items: center;\n  height: 100%;\n  position: absolute;\n}\n\n.ag-header-group-cell-no-group.ag-header-span-height .ag-header-cell-resize {\n  display: none;\n}\n\n.ag-cell-label-container {\n  display: flex;\n  justify-content: space-between;\n  flex-direction: row-reverse;\n  align-items: center;\n  height: 100%;\n  width: 100%;\n  overflow: hidden;\n  padding: 5px 0px;\n}\n\n.ag-right-aligned-header .ag-cell-label-container {\n  flex-direction: row;\n}\n.ag-right-aligned-header .ag-header-cell-text {\n  text-align: end;\n}\n\n.ag-side-bar {\n  display: flex;\n  flex-direction: row-reverse;\n}\n\n.ag-side-bar-left {\n  order: -1;\n  flex-direction: row;\n}\n\n.ag-side-button-button {\n  position: relative;\n  display: flex;\n  flex-direction: column;\n  align-items: center;\n  justify-content: center;\n  flex-wrap: nowrap;\n  white-space: nowrap;\n  outline: none;\n  cursor: pointer;\n}\n\n.ag-side-button-label {\n  writing-mode: vertical-lr;\n}\n\n.ag-status-bar {\n  display: flex;\n  justify-content: space-between;\n  overflow: hidden;\n}\n\n.ag-status-panel {\n  display: inline-flex;\n}\n\n.ag-status-name-value {\n  white-space: nowrap;\n}\n\n.ag-status-bar-left {\n  display: inline-flex;\n}\n\n.ag-status-bar-center {\n  display: inline-flex;\n}\n\n.ag-status-bar-right {\n  display: inline-flex;\n}\n\n.ag-icon {\n  display: block;\n  speak: none;\n}\n\n.ag-group {\n  position: relative;\n  width: 100%;\n}\n\n.ag-group-title-bar {\n  display: flex;\n  align-items: center;\n}\n\n.ag-group-title {\n  display: block;\n  flex: 1 1 auto;\n  min-width: 0;\n  overflow: hidden;\n  white-space: nowrap;\n  text-overflow: ellipsis;\n}\n\n.ag-group-title-bar .ag-group-title {\n  cursor: default;\n}\n\n.ag-group-toolbar {\n  display: flex;\n  align-items: center;\n}\n\n.ag-group-container {\n  display: flex;\n}\n\n.ag-disabled .ag-group-container {\n  pointer-events: none;\n}\n\n.ag-group-container-horizontal {\n  flex-direction: row;\n  flex-wrap: wrap;\n}\n\n.ag-group-container-vertical {\n  flex-direction: column;\n}\n\n.ag-column-group-icons {\n  display: block;\n}\n.ag-column-group-icons > * {\n  cursor: pointer;\n}\n\n.ag-group-item-alignment-stretch .ag-group-item {\n  align-items: stretch;\n}\n\n.ag-group-item-alignment-start .ag-group-item {\n  align-items: flex-start;\n}\n\n.ag-group-item-alignment-end .ag-group-item {\n  align-items: flex-end;\n}\n\n.ag-toggle-button-icon {\n  transition: right 0.3s;\n  position: absolute;\n  top: -1px;\n}\n\n.ag-input-field, .ag-select {\n  display: flex;\n  flex-direction: row;\n  align-items: center;\n}\n\n.ag-input-field-input {\n  flex: 1 1 auto;\n}\n\n.ag-floating-filter-input .ag-input-field-input[type=date] {\n  width: 1px;\n}\n\n.ag-range-field {\n  display: flex;\n  align-items: center;\n}\n\n.ag-angle-select {\n  display: flex;\n  align-items: center;\n}\n\n.ag-angle-select-wrapper {\n  display: flex;\n}\n\n.ag-angle-select-parent-circle {\n  display: block;\n  position: relative;\n}\n\n.ag-angle-select-child-circle {\n  position: absolute;\n}\n\n.ag-slider-wrapper {\n  display: flex;\n}\n.ag-slider-wrapper .ag-input-field {\n  flex: 1 1 auto;\n}\n\n.ag-picker-field-display {\n  flex: 1 1 auto;\n}\n\n.ag-picker-field {\n  display: flex;\n  align-items: center;\n}\n\n.ag-picker-field-icon {\n  display: flex;\n  border: 0;\n  padding: 0;\n  margin: 0;\n  cursor: pointer;\n}\n\n.ag-picker-field-wrapper {\n  overflow: hidden;\n}\n\n.ag-label-align-right .ag-label {\n  order: 1;\n}\n.ag-label-align-right > * {\n  flex: none;\n}\n\n.ag-label-align-top {\n  flex-direction: column;\n  align-items: flex-start;\n}\n.ag-label-align-top > * {\n  align-self: stretch;\n}\n\n.ag-label-ellipsis {\n  overflow: hidden;\n  text-overflow: ellipsis;\n  white-space: nowrap;\n  flex: 1;\n}\n\n.ag-color-panel {\n  width: 100%;\n  display: flex;\n  flex-direction: column;\n  text-align: center;\n}\n\n.ag-spectrum-color {\n  flex: 1 1 auto;\n  position: relative;\n  overflow: hidden;\n  cursor: default;\n}\n\n.ag-spectrum-fill {\n  position: absolute;\n  top: 0;\n  left: 0;\n  right: 0;\n  bottom: 0;\n}\n\n.ag-spectrum-val {\n  cursor: pointer;\n}\n\n.ag-spectrum-dragger {\n  position: absolute;\n  pointer-events: none;\n  cursor: pointer;\n}\n\n.ag-spectrum-hue {\n  cursor: default;\n  background: linear-gradient(to left, #ff0000 3%, #ffff00 17%, #00ff00 33%, #00ffff 50%, #0000ff 67%, #ff00ff 83%, #ff0000 100%);\n}\n\n.ag-spectrum-alpha {\n  cursor: default;\n}\n\n.ag-spectrum-hue-background {\n  width: 100%;\n  height: 100%;\n}\n\n.ag-spectrum-alpha-background {\n  background-image: linear-gradient(to right, rgba(0, 0, 0, 0), rgb(0, 0, 0));\n  width: 100%;\n  height: 100%;\n}\n\n.ag-spectrum-tool {\n  cursor: pointer;\n}\n\n.ag-spectrum-slider {\n  position: absolute;\n  pointer-events: none;\n}\n\n.ag-recent-colors {\n  display: flex;\n}\n\n.ag-recent-color {\n  cursor: pointer;\n}\n\n.ag-ltr .ag-column-select-indent-1 {\n  padding-left: 20px;\n}\n.ag-rtl .ag-column-select-indent-1 {\n  padding-right: 20px;\n}\n\n.ag-ltr .ag-set-filter-indent-1 {\n  padding-left: 20px;\n}\n.ag-rtl .ag-set-filter-indent-1 {\n  padding-right: 20px;\n}\n\n.ag-ltr .ag-row-group-indent-1 {\n  padding-left: 20px;\n}\n.ag-rtl .ag-row-group-indent-1 {\n  padding-right: 20px;\n}\n\n.ag-ltr .ag-column-select-indent-2 {\n  padding-left: 40px;\n}\n.ag-rtl .ag-column-select-indent-2 {\n  padding-right: 40px;\n}\n\n.ag-ltr .ag-set-filter-indent-2 {\n  padding-left: 40px;\n}\n.ag-rtl .ag-set-filter-indent-2 {\n  padding-right: 40px;\n}\n\n.ag-ltr .ag-row-group-indent-2 {\n  padding-left: 40px;\n}\n.ag-rtl .ag-row-group-indent-2 {\n  padding-right: 40px;\n}\n\n.ag-ltr .ag-column-select-indent-3 {\n  padding-left: 60px;\n}\n.ag-rtl .ag-column-select-indent-3 {\n  padding-right: 60px;\n}\n\n.ag-ltr .ag-set-filter-indent-3 {\n  padding-left: 60px;\n}\n.ag-rtl .ag-set-filter-indent-3 {\n  padding-right: 60px;\n}\n\n.ag-ltr .ag-row-group-indent-3 {\n  padding-left: 60px;\n}\n.ag-rtl .ag-row-group-indent-3 {\n  padding-right: 60px;\n}\n\n.ag-ltr .ag-column-select-indent-4 {\n  padding-left: 80px;\n}\n.ag-rtl .ag-column-select-indent-4 {\n  padding-right: 80px;\n}\n\n.ag-ltr .ag-set-filter-indent-4 {\n  padding-left: 80px;\n}\n.ag-rtl .ag-set-filter-indent-4 {\n  padding-right: 80px;\n}\n\n.ag-ltr .ag-row-group-indent-4 {\n  padding-left: 80px;\n}\n.ag-rtl .ag-row-group-indent-4 {\n  padding-right: 80px;\n}\n\n.ag-ltr .ag-column-select-indent-5 {\n  padding-left: 100px;\n}\n.ag-rtl .ag-column-select-indent-5 {\n  padding-right: 100px;\n}\n\n.ag-ltr .ag-set-filter-indent-5 {\n  padding-left: 100px;\n}\n.ag-rtl .ag-set-filter-indent-5 {\n  padding-right: 100px;\n}\n\n.ag-ltr .ag-row-group-indent-5 {\n  padding-left: 100px;\n}\n.ag-rtl .ag-row-group-indent-5 {\n  padding-right: 100px;\n}\n\n.ag-ltr .ag-column-select-indent-6 {\n  padding-left: 120px;\n}\n.ag-rtl .ag-column-select-indent-6 {\n  padding-right: 120px;\n}\n\n.ag-ltr .ag-set-filter-indent-6 {\n  padding-left: 120px;\n}\n.ag-rtl .ag-set-filter-indent-6 {\n  padding-right: 120px;\n}\n\n.ag-ltr .ag-row-group-indent-6 {\n  padding-left: 120px;\n}\n.ag-rtl .ag-row-group-indent-6 {\n  padding-right: 120px;\n}\n\n.ag-ltr .ag-column-select-indent-7 {\n  padding-left: 140px;\n}\n.ag-rtl .ag-column-select-indent-7 {\n  padding-right: 140px;\n}\n\n.ag-ltr .ag-set-filter-indent-7 {\n  padding-left: 140px;\n}\n.ag-rtl .ag-set-filter-indent-7 {\n  padding-right: 140px;\n}\n\n.ag-ltr .ag-row-group-indent-7 {\n  padding-left: 140px;\n}\n.ag-rtl .ag-row-group-indent-7 {\n  padding-right: 140px;\n}\n\n.ag-ltr .ag-column-select-indent-8 {\n  padding-left: 160px;\n}\n.ag-rtl .ag-column-select-indent-8 {\n  padding-right: 160px;\n}\n\n.ag-ltr .ag-set-filter-indent-8 {\n  padding-left: 160px;\n}\n.ag-rtl .ag-set-filter-indent-8 {\n  padding-right: 160px;\n}\n\n.ag-ltr .ag-row-group-indent-8 {\n  padding-left: 160px;\n}\n.ag-rtl .ag-row-group-indent-8 {\n  padding-right: 160px;\n}\n\n.ag-ltr .ag-column-select-indent-9 {\n  padding-left: 180px;\n}\n.ag-rtl .ag-column-select-indent-9 {\n  padding-right: 180px;\n}\n\n.ag-ltr .ag-set-filter-indent-9 {\n  padding-left: 180px;\n}\n.ag-rtl .ag-set-filter-indent-9 {\n  padding-right: 180px;\n}\n\n.ag-ltr .ag-row-group-indent-9 {\n  padding-left: 180px;\n}\n.ag-rtl .ag-row-group-indent-9 {\n  padding-right: 180px;\n}\n\n.ag-ltr {\n  direction: ltr;\n}\n.ag-ltr .ag-body, .ag-ltr .ag-floating-top, .ag-ltr .ag-floating-bottom, .ag-ltr .ag-header, .ag-ltr .ag-body-viewport, .ag-ltr .ag-body-horizontal-scroll {\n  flex-direction: row;\n}\n\n.ag-rtl {\n  direction: rtl;\n}\n.ag-rtl .ag-body, .ag-rtl .ag-floating-top, .ag-rtl .ag-floating-bottom, .ag-rtl .ag-header, .ag-rtl .ag-body-viewport, .ag-rtl .ag-body-horizontal-scroll {\n  flex-direction: row-reverse;\n}\n.ag-rtl .ag-icon-contracted,\n.ag-rtl .ag-icon-expanded,\n.ag-rtl .ag-icon-tree-closed {\n  display: block;\n  transform: rotate(180deg);\n}\n\n.ag-body .ag-body-viewport {\n  -webkit-overflow-scrolling: touch;\n}\n\n.ag-layout-print.ag-body {\n  display: block;\n  height: unset;\n}\n.ag-layout-print.ag-body-clipper {\n  height: unset;\n}\n.ag-layout-print.ag-root-wrapper {\n  display: inline-flex;\n}\n.ag-layout-print .ag-center-cols-clipper {\n  min-width: 100%;\n}\n.ag-layout-print .ag-body-vertical-scroll {\n  display: none;\n}\n.ag-layout-print .ag-body-horizontal-scroll {\n  display: none;\n}\n.ag-layout-print.ag-force-vertical-scroll {\n  overflow-y: visible !important;\n}\n\n@media print {\n  .ag-root-wrapper.ag-layout-print {\n    display: table;\n  }\n  .ag-root-wrapper.ag-layout-print .ag-root-wrapper-body,\n  .ag-root-wrapper.ag-layout-print .ag-root,\n  .ag-root-wrapper.ag-layout-print .ag-body-viewport,\n  .ag-root-wrapper.ag-layout-print .ag-center-cols-container,\n  .ag-root-wrapper.ag-layout-print .ag-center-cols-viewport,\n  .ag-root-wrapper.ag-layout-print .ag-center-cols-clipper,\n  .ag-root-wrapper.ag-layout-print .ag-body-horizontal-scroll-viewport,\n  .ag-root-wrapper.ag-layout-print .ag-virtual-list-viewport {\n    height: auto !important;\n    overflow: hidden !important;\n    display: block !important;\n  }\n  .ag-root-wrapper.ag-layout-print .ag-row, .ag-root-wrapper.ag-layout-print .ag-cell {\n    break-inside: avoid;\n  }\n}\n[class^=ag-], [class^=ag-]:focus, [class^=ag-]:after, [class^=ag-]:before {\n  box-sizing: border-box;\n  outline: none;\n}\n\n[class^=ag-]::-ms-clear {\n  display: none;\n}\n\n.ag-checkbox .ag-input-wrapper,\n.ag-radio-button .ag-input-wrapper {\n  overflow: visible;\n}\n\n.ag-range-field .ag-input-wrapper {\n  height: 100%;\n}\n\n.ag-toggle-button {\n  flex: none;\n  width: unset;\n  min-width: unset;\n}\n\n.ag-ltr .ag-label-align-right .ag-label {\n  margin-left: var(--ag-grid-size);\n}\n.ag-rtl .ag-label-align-right .ag-label {\n  margin-right: var(--ag-grid-size);\n}\n\ninput[class^=ag-] {\n  margin: 0;\n  background-color: var(--ag-background-color);\n}\n\ntextarea[class^=ag-],\nselect[class^=ag-] {\n  background-color: var(--ag-background-color);\n}\n\ninput[class^=ag-]:not([type]),\ninput[class^=ag-][type=text],\ninput[class^=ag-][type=number],\ninput[class^=ag-][type=tel],\ninput[class^=ag-][type=date],\ninput[class^=ag-][type=datetime-local],\ntextarea[class^=ag-] {\n  font-size: inherit;\n  line-height: inherit;\n  color: inherit;\n  border: var(--ag-borders-input) var(--ag-input-border-color);\n}\ninput[class^=ag-]:not([type]):disabled,\ninput[class^=ag-][type=text]:disabled,\ninput[class^=ag-][type=number]:disabled,\ninput[class^=ag-][type=tel]:disabled,\ninput[class^=ag-][type=date]:disabled,\ninput[class^=ag-][type=datetime-local]:disabled,\ntextarea[class^=ag-]:disabled {\n  color: var(--ag-disabled-foreground-color);\n  background-color: var(--ag-input-disabled-background-color);\n  border-color: var(--ag-input-disabled-border-color);\n}\ninput[class^=ag-]:not([type]):focus,\ninput[class^=ag-][type=text]:focus,\ninput[class^=ag-][type=number]:focus,\ninput[class^=ag-][type=tel]:focus,\ninput[class^=ag-][type=date]:focus,\ninput[class^=ag-][type=datetime-local]:focus,\ntextarea[class^=ag-]:focus {\n  outline: none;\n  box-shadow: var(--ag-input-focus-box-shadow);\n  border-color: var(--ag-input-focus-border-color);\n}\ninput[class^=ag-]:not([type]):invalid,\ninput[class^=ag-][type=text]:invalid,\ninput[class^=ag-][type=number]:invalid,\ninput[class^=ag-][type=tel]:invalid,\ninput[class^=ag-][type=date]:invalid,\ninput[class^=ag-][type=datetime-local]:invalid,\ntextarea[class^=ag-]:invalid {\n  border: var(--ag-borders-input-invalid) var(--ag-input-border-color-invalid);\n}\n\ninput[class^=ag-][type=number] {\n  -moz-appearance: textfield;\n}\ninput[class^=ag-][type=number]::-webkit-outer-spin-button, input[class^=ag-][type=number]::-webkit-inner-spin-button {\n  -webkit-appearance: none;\n  margin: 0;\n}\n\ninput[class^=ag-][type=range] {\n  padding: 0;\n}\n\ninput[class^=ag-][type=button]:focus, button[class^=ag-]:focus {\n  box-shadow: var(--ag-input-focus-box-shadow);\n}\n\n.ag-drag-handle {\n  color: var(--ag-secondary-foreground-color);\n}\n\n.ag-list-item, .ag-virtual-list-item {\n  height: var(--ag-list-item-height);\n}\n\n.ag-keyboard-focus .ag-virtual-list-item:focus {\n  outline: none;\n}\n.ag-keyboard-focus .ag-virtual-list-item:focus::after {\n  content: "";\n  position: absolute;\n  background-color: transparent;\n  pointer-events: none;\n  top: 4px;\n  left: 4px;\n  display: block;\n  width: calc(100% - 8px);\n  height: calc(100% - 8px);\n  border: 1px solid;\n  border-color: var(--ag-input-focus-border-color);\n}\n\n.ag-select-list {\n  background-color: var(--ag-background-color);\n  overflow-y: auto;\n  overflow-x: hidden;\n}\n\n.ag-list-item {\n  display: flex;\n  align-items: center;\n  white-space: nowrap;\n  overflow: hidden;\n  text-overflow: ellipsis;\n}\n.ag-list-item.ag-active-item {\n  background-color: var(--ag-row-hover-color);\n}\n\n.ag-select-list-item {\n  padding-left: 4px;\n  padding-right: 4px;\n  cursor: default;\n  -moz-user-select: none;\n  -webkit-user-select: none;\n  -ms-user-select: none;\n  user-select: none;\n}\n.ag-select-list-item span {\n  white-space: nowrap;\n  text-overflow: ellipsis;\n  overflow: hidden;\n}\n\n.ag-select .ag-picker-field-wrapper {\n  background-color: var(--ag-background-color);\n  min-height: var(--ag-list-item-height);\n  cursor: default;\n}\n.ag-select.ag-disabled .ag-picker-field-wrapper:focus {\n  box-shadow: none;\n}\n.ag-select:not(.ag-cell-editor, .ag-label-align-top) {\n  height: var(--ag-list-item-height);\n}\n.ag-select .ag-picker-field-display {\n  margin: 4px;\n  white-space: nowrap;\n  overflow: hidden;\n  text-overflow: ellipsis;\n}\n.ag-select .ag-picker-field-icon {\n  display: flex;\n  align-items: center;\n}\n.ag-select.ag-disabled {\n  opacity: 0.5;\n}\n\n.ag-rich-select {\n  background-color: var(--ag-control-panel-background-color);\n}\n\n.ag-rich-select-list {\n  width: 100%;\n  min-width: 200px;\n  height: calc(var(--ag-row-height) * 6.5);\n}\n\n.ag-rich-select-value {\n  height: var(--ag-row-height);\n  border-bottom: var(--ag-borders-secondary) var(--ag-secondary-border-color);\n  padding-top: 0;\n  padding-bottom: 0;\n}\n.ag-ltr .ag-rich-select-value {\n  padding-left: var(--ag-cell-horizontal-padding);\n}\n.ag-rtl .ag-rich-select-value {\n  padding-right: var(--ag-cell-horizontal-padding);\n}\n.ag-ltr .ag-rich-select-value {\n  padding-right: var(--ag-grid-size);\n}\n.ag-rtl .ag-rich-select-value {\n  padding-left: var(--ag-grid-size);\n}\n\n.ag-rich-select-virtual-list-item {\n  cursor: default;\n  height: var(--ag-list-item-height);\n}\n.ag-keyboard-focus .ag-rich-select-virtual-list-item:focus::after {\n  content: none;\n}\n.ag-rich-select-virtual-list-item:hover {\n  background-color: var(--ag-row-hover-color);\n}\n\n.ag-ltr .ag-rich-select-row {\n  padding-left: var(--ag-cell-horizontal-padding);\n}\n.ag-rtl .ag-rich-select-row {\n  padding-right: var(--ag-cell-horizontal-padding);\n}\n\n.ag-rich-select-row-selected {\n  background-color: var(--ag-selected-row-background-color);\n}\n\n.ag-row-drag,\n.ag-selection-checkbox,\n.ag-group-expanded,\n.ag-group-contracted {\n  color: var(--ag-secondary-foreground-color);\n}\n.ag-ltr .ag-row-drag,\n.ag-ltr .ag-selection-checkbox,\n.ag-ltr .ag-group-expanded,\n.ag-ltr .ag-group-contracted {\n  margin-right: var(--ag-cell-widget-spacing);\n}\n.ag-rtl .ag-row-drag,\n.ag-rtl .ag-selection-checkbox,\n.ag-rtl .ag-group-expanded,\n.ag-rtl .ag-group-contracted {\n  margin-left: var(--ag-cell-widget-spacing);\n}\n\n.ag-cell-wrapper > *:not(.ag-cell-value):not(.ag-group-value) {\n  --ag-internal-calculated-line-height: var(--ag-line-height, calc(var(--ag-row-height) - var(--ag-row-border-width)));\n  --ag-internal-padded-row-height: calc(var(--ag-row-height) - var(--ag-row-border-width));\n  height: min(var(--ag-internal-calculated-line-height), var(--ag-internal-padded-row-height));\n  display: flex;\n  align-items: center;\n  flex: none;\n}\n\n.ag-group-expanded,\n.ag-group-contracted {\n  cursor: pointer;\n}\n\n.ag-group-title-bar-icon {\n  cursor: pointer;\n  flex: none;\n  color: var(--ag-secondary-foreground-color);\n}\n\n.ag-ltr .ag-group-child-count {\n  margin-left: 2px;\n}\n.ag-rtl .ag-group-child-count {\n  margin-right: 2px;\n}\n\n.ag-group-title-bar {\n  background-color: var(--ag-subheader-background-color);\n  padding: var(--ag-grid-size);\n}\n\n.ag-group-toolbar {\n  padding: var(--ag-grid-size);\n  background-color: var(--ag-subheader-toolbar-background-color);\n}\n\n.ag-disabled-group-title-bar, .ag-disabled-group-container {\n  opacity: 0.5;\n}\n\n.group-item {\n  margin: calc(var(--ag-grid-size) * 0.5) 0;\n}\n\n.ag-label {\n  white-space: nowrap;\n}\n.ag-ltr .ag-label {\n  margin-right: var(--ag-grid-size);\n}\n.ag-rtl .ag-label {\n  margin-left: var(--ag-grid-size);\n}\n\n.ag-label-align-top .ag-label {\n  margin-bottom: calc(var(--ag-grid-size) * 0.5);\n}\n\n.ag-angle-select[disabled] {\n  color: var(--ag-disabled-foreground-color);\n  pointer-events: none;\n}\n.ag-angle-select[disabled] .ag-angle-select-field {\n  opacity: 0.4;\n}\n\n.ag-ltr .ag-slider-field,\n.ag-ltr .ag-angle-select-field {\n  margin-right: calc(var(--ag-grid-size) * 2);\n}\n.ag-rtl .ag-slider-field,\n.ag-rtl .ag-angle-select-field {\n  margin-left: calc(var(--ag-grid-size) * 2);\n}\n\n.ag-angle-select-parent-circle {\n  width: 24px;\n  height: 24px;\n  border-radius: 12px;\n  border: solid 1px;\n  border-color: var(--ag-border-color);\n  background-color: var(--ag-background-color);\n}\n\n.ag-angle-select-child-circle {\n  top: 4px;\n  left: 12px;\n  width: 6px;\n  height: 6px;\n  margin-left: -3px;\n  margin-top: -4px;\n  border-radius: 3px;\n  background-color: var(--ag-secondary-foreground-color);\n}\n\n.ag-picker-field-wrapper {\n  border: 1px solid;\n  border-color: var(--ag-border-color);\n  border-radius: 5px;\n}\n.ag-picker-field-wrapper:focus {\n  box-shadow: var(--ag-input-focus-box-shadow);\n}\n\n.ag-picker-field-button {\n  background-color: var(--ag-background-color);\n  color: var(--ag-secondary-foreground-color);\n}\n\n.ag-dialog.ag-color-dialog {\n  border-radius: 5px;\n}\n\n.ag-color-picker .ag-picker-field-display {\n  height: var(--ag-icon-size);\n}\n\n.ag-color-panel {\n  padding: var(--ag-grid-size);\n}\n\n.ag-spectrum-color {\n  background-color: rgb(255, 0, 0);\n  border-radius: 2px;\n}\n\n.ag-spectrum-tools {\n  padding: 10px;\n}\n\n.ag-spectrum-sat {\n  background-image: linear-gradient(to right, white, rgba(204, 154, 129, 0));\n}\n\n.ag-spectrum-val {\n  background-image: linear-gradient(to top, black, rgba(204, 154, 129, 0));\n}\n\n.ag-spectrum-dragger {\n  border-radius: 12px;\n  height: 12px;\n  width: 12px;\n  border: 1px solid white;\n  background: black;\n  box-shadow: 0 0 2px 0px rgba(0, 0, 0, 0.24);\n}\n\n.ag-spectrum-hue-background {\n  border-radius: 2px;\n}\n\n.ag-spectrum-alpha-background {\n  border-radius: 2px;\n}\n\n.ag-spectrum-tool {\n  margin-bottom: 10px;\n  height: 11px;\n  border-radius: 2px;\n}\n\n.ag-spectrum-slider {\n  margin-top: -12px;\n  width: 13px;\n  height: 13px;\n  border-radius: 13px;\n  background-color: rgb(248, 248, 248);\n  box-shadow: 0 1px 4px 0 rgba(0, 0, 0, 0.37);\n}\n\n.ag-recent-color {\n  margin: 0 3px;\n}\n.ag-recent-color:first-child {\n  margin-left: 0;\n}\n.ag-recent-color:last-child {\n  margin-right: 0;\n}\n\n.ag-dnd-ghost {\n  border: var(--ag-borders) var(--ag-border-color);\n  background: var(--ag-background-color);\n  border-radius: var(--ag-card-radius);\n  box-shadow: var(--ag-card-shadow);\n  padding: var(--ag-grid-size);\n  overflow: hidden;\n  text-overflow: ellipsis;\n  border: var(--ag-borders-secondary) var(--ag-secondary-border-color);\n  color: var(--ag-secondary-foreground-color);\n  height: var(--ag-header-height) !important;\n  line-height: var(--ag-header-height);\n  margin: 0;\n  padding: 0 calc(var(--ag-grid-size) * 2);\n  transform: translateY(calc(var(--ag-grid-size) * 2));\n}\n\n.ag-dnd-ghost-icon {\n  margin-right: var(--ag-grid-size);\n  color: var(--ag-foreground-color);\n}\n\n.ag-popup-child:not(.ag-tooltip-custom) {\n  box-shadow: var(--ag-popup-shadow);\n}\n\n.ag-dragging-range-handle .ag-dialog,\n.ag-dragging-fill-handle .ag-dialog {\n  opacity: 0.7;\n  pointer-events: none;\n}\n\n.ag-dialog {\n  border-radius: var(--ag-border-radius);\n  border: var(--ag-borders) var(--ag-border-color);\n}\n\n.ag-panel {\n  background-color: var(--ag-background-color);\n}\n\n.ag-panel-title-bar {\n  background-color: var(--ag-header-background-color);\n  color: var(--ag-header-foreground-color);\n  height: var(--ag-header-height);\n  padding: var(--ag-grid-size) var(--ag-cell-horizontal-padding);\n  border-bottom: var(--ag-borders) var(--ag-border-color);\n}\n\n.ag-ltr .ag-panel-title-bar-button {\n  margin-left: var(--ag-grid-size);\n}\n.ag-rtl .ag-panel-title-bar-button {\n  margin-right: var(--ag-grid-size);\n}\n\n.ag-tooltip {\n  background-color: var(--ag-tooltip-background-color);\n  color: var(--ag-foreground-color);\n  padding: var(--ag-grid-size);\n  border: var(--ag-borders) var(--ag-border-color);\n  border-radius: var(--ag-card-radius);\n  transition: opacity 1s;\n  white-space: normal;\n}\n.ag-tooltip.ag-tooltip-hiding {\n  opacity: 0;\n}\n\n.ag-tooltip-custom {\n  transition: opacity 1s;\n}\n.ag-tooltip-custom.ag-tooltip-hiding {\n  opacity: 0;\n}\n\n.ag-ltr .ag-column-select-indent-1 {\n  padding-left: calc(1 * var(--ag-column-select-indent-size));\n}\n.ag-rtl .ag-column-select-indent-1 {\n  padding-right: calc(1 * var(--ag-column-select-indent-size));\n}\n\n.ag-ltr .ag-column-select-indent-2 {\n  padding-left: calc(2 * var(--ag-column-select-indent-size));\n}\n.ag-rtl .ag-column-select-indent-2 {\n  padding-right: calc(2 * var(--ag-column-select-indent-size));\n}\n\n.ag-ltr .ag-column-select-indent-3 {\n  padding-left: calc(3 * var(--ag-column-select-indent-size));\n}\n.ag-rtl .ag-column-select-indent-3 {\n  padding-right: calc(3 * var(--ag-column-select-indent-size));\n}\n\n.ag-ltr .ag-column-select-indent-4 {\n  padding-left: calc(4 * var(--ag-column-select-indent-size));\n}\n.ag-rtl .ag-column-select-indent-4 {\n  padding-right: calc(4 * var(--ag-column-select-indent-size));\n}\n\n.ag-ltr .ag-column-select-indent-5 {\n  padding-left: calc(5 * var(--ag-column-select-indent-size));\n}\n.ag-rtl .ag-column-select-indent-5 {\n  padding-right: calc(5 * var(--ag-column-select-indent-size));\n}\n\n.ag-ltr .ag-column-select-indent-6 {\n  padding-left: calc(6 * var(--ag-column-select-indent-size));\n}\n.ag-rtl .ag-column-select-indent-6 {\n  padding-right: calc(6 * var(--ag-column-select-indent-size));\n}\n\n.ag-ltr .ag-column-select-indent-7 {\n  padding-left: calc(7 * var(--ag-column-select-indent-size));\n}\n.ag-rtl .ag-column-select-indent-7 {\n  padding-right: calc(7 * var(--ag-column-select-indent-size));\n}\n\n.ag-ltr .ag-column-select-indent-8 {\n  padding-left: calc(8 * var(--ag-column-select-indent-size));\n}\n.ag-rtl .ag-column-select-indent-8 {\n  padding-right: calc(8 * var(--ag-column-select-indent-size));\n}\n\n.ag-ltr .ag-column-select-indent-9 {\n  padding-left: calc(9 * var(--ag-column-select-indent-size));\n}\n.ag-rtl .ag-column-select-indent-9 {\n  padding-right: calc(9 * var(--ag-column-select-indent-size));\n}\n\n.ag-column-select-header-icon {\n  cursor: pointer;\n}\n\n.ag-keyboard-focus .ag-column-select-header-icon:focus {\n  outline: none;\n}\n.ag-keyboard-focus .ag-column-select-header-icon:focus::after {\n  content: "";\n  position: absolute;\n  background-color: transparent;\n  pointer-events: none;\n  top: 0px;\n  left: 0px;\n  display: block;\n  width: calc(100% - 0px);\n  height: calc(100% - 0px);\n  border: 1px solid;\n  border-color: var(--ag-input-focus-border-color);\n}\n\n.ag-ltr .ag-column-group-icons:not(:last-child),\n.ag-ltr .ag-column-select-header-icon:not(:last-child),\n.ag-ltr .ag-column-select-header-checkbox:not(:last-child),\n.ag-ltr .ag-column-select-header-filter-wrapper:not(:last-child),\n.ag-ltr .ag-column-select-checkbox:not(:last-child),\n.ag-ltr .ag-column-select-column-drag-handle:not(:last-child),\n.ag-ltr .ag-column-select-column-group-drag-handle:not(:last-child),\n.ag-ltr .ag-column-select-column-label:not(:last-child) {\n  margin-right: var(--ag-widget-horizontal-spacing);\n}\n.ag-rtl .ag-column-group-icons:not(:last-child),\n.ag-rtl .ag-column-select-header-icon:not(:last-child),\n.ag-rtl .ag-column-select-header-checkbox:not(:last-child),\n.ag-rtl .ag-column-select-header-filter-wrapper:not(:last-child),\n.ag-rtl .ag-column-select-checkbox:not(:last-child),\n.ag-rtl .ag-column-select-column-drag-handle:not(:last-child),\n.ag-rtl .ag-column-select-column-group-drag-handle:not(:last-child),\n.ag-rtl .ag-column-select-column-label:not(:last-child) {\n  margin-left: var(--ag-widget-horizontal-spacing);\n}\n\n.ag-keyboard-focus .ag-column-select-virtual-list-item:focus {\n  outline: none;\n}\n.ag-keyboard-focus .ag-column-select-virtual-list-item:focus::after {\n  content: "";\n  position: absolute;\n  background-color: transparent;\n  pointer-events: none;\n  top: 1px;\n  left: 1px;\n  display: block;\n  width: calc(100% - 2px);\n  height: calc(100% - 2px);\n  border: 1px solid;\n  border-color: var(--ag-input-focus-border-color);\n}\n\n.ag-column-select-column-group:not(:last-child),\n.ag-column-select-column:not(:last-child) {\n  margin-bottom: var(--ag-widget-vertical-spacing);\n}\n\n.ag-column-select-column-readonly,\n.ag-column-select-column-group-readonly {\n  color: var(--ag-disabled-foreground-color);\n  pointer-events: none;\n}\n\n.ag-ltr .ag-column-select-add-group-indent {\n  margin-left: calc(var(--ag-icon-size) + var(--ag-grid-size) * 2);\n}\n.ag-rtl .ag-column-select-add-group-indent {\n  margin-right: calc(var(--ag-icon-size) + var(--ag-grid-size) * 2);\n}\n\n.ag-column-select-virtual-list-viewport {\n  padding: calc(var(--ag-widget-container-vertical-padding) * 0.5) 0px;\n}\n\n.ag-column-select-virtual-list-item {\n  padding: 0 var(--ag-widget-container-horizontal-padding);\n}\n\n.ag-rtl {\n  text-align: right;\n}\n\n.ag-root-wrapper {\n  border: var(--ag-borders) var(--ag-border-color);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-1 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 1);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-1 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 1);\n}\n\n.ag-ltr .ag-row-group-indent-1 {\n  padding-left: calc(1 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-1 {\n  padding-right: calc(1 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-1 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-1 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-2 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 2);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-2 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 2);\n}\n\n.ag-ltr .ag-row-group-indent-2 {\n  padding-left: calc(2 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-2 {\n  padding-right: calc(2 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-2 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-2 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-3 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 3);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-3 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 3);\n}\n\n.ag-ltr .ag-row-group-indent-3 {\n  padding-left: calc(3 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-3 {\n  padding-right: calc(3 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-3 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-3 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-4 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 4);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-4 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 4);\n}\n\n.ag-ltr .ag-row-group-indent-4 {\n  padding-left: calc(4 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-4 {\n  padding-right: calc(4 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-4 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-4 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-5 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 5);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-5 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 5);\n}\n\n.ag-ltr .ag-row-group-indent-5 {\n  padding-left: calc(5 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-5 {\n  padding-right: calc(5 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-5 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-5 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-6 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 6);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-6 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 6);\n}\n\n.ag-ltr .ag-row-group-indent-6 {\n  padding-left: calc(6 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-6 {\n  padding-right: calc(6 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-6 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-6 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-7 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 7);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-7 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 7);\n}\n\n.ag-ltr .ag-row-group-indent-7 {\n  padding-left: calc(7 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-7 {\n  padding-right: calc(7 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-7 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-7 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-8 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 8);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-8 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 8);\n}\n\n.ag-ltr .ag-row-group-indent-8 {\n  padding-left: calc(8 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-8 {\n  padding-right: calc(8 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-8 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-8 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-9 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 9);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-9 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 9);\n}\n\n.ag-ltr .ag-row-group-indent-9 {\n  padding-left: calc(9 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-9 {\n  padding-right: calc(9 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-9 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-9 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-10 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 10);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-10 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 10);\n}\n\n.ag-ltr .ag-row-group-indent-10 {\n  padding-left: calc(10 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-10 {\n  padding-right: calc(10 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-10 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-10 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-11 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 11);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-11 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 11);\n}\n\n.ag-ltr .ag-row-group-indent-11 {\n  padding-left: calc(11 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-11 {\n  padding-right: calc(11 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-11 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-11 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-12 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 12);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-12 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 12);\n}\n\n.ag-ltr .ag-row-group-indent-12 {\n  padding-left: calc(12 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-12 {\n  padding-right: calc(12 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-12 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-12 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-13 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 13);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-13 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 13);\n}\n\n.ag-ltr .ag-row-group-indent-13 {\n  padding-left: calc(13 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-13 {\n  padding-right: calc(13 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-13 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-13 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-14 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 14);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-14 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 14);\n}\n\n.ag-ltr .ag-row-group-indent-14 {\n  padding-left: calc(14 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-14 {\n  padding-right: calc(14 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-14 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-14 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-15 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 15);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-15 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 15);\n}\n\n.ag-ltr .ag-row-group-indent-15 {\n  padding-left: calc(15 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-15 {\n  padding-right: calc(15 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-15 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-15 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-16 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 16);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-16 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 16);\n}\n\n.ag-ltr .ag-row-group-indent-16 {\n  padding-left: calc(16 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-16 {\n  padding-right: calc(16 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-16 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-16 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-17 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 17);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-17 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 17);\n}\n\n.ag-ltr .ag-row-group-indent-17 {\n  padding-left: calc(17 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-17 {\n  padding-right: calc(17 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-17 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-17 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-18 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 18);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-18 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 18);\n}\n\n.ag-ltr .ag-row-group-indent-18 {\n  padding-left: calc(18 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-18 {\n  padding-right: calc(18 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-18 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-18 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-19 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 19);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-19 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 19);\n}\n\n.ag-ltr .ag-row-group-indent-19 {\n  padding-left: calc(19 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-19 {\n  padding-right: calc(19 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-19 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-19 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-20 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 20);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-20 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 20);\n}\n\n.ag-ltr .ag-row-group-indent-20 {\n  padding-left: calc(20 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-20 {\n  padding-right: calc(20 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-20 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-20 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-21 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 21);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-21 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 21);\n}\n\n.ag-ltr .ag-row-group-indent-21 {\n  padding-left: calc(21 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-21 {\n  padding-right: calc(21 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-21 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-21 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-22 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 22);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-22 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 22);\n}\n\n.ag-ltr .ag-row-group-indent-22 {\n  padding-left: calc(22 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-22 {\n  padding-right: calc(22 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-22 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-22 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-23 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 23);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-23 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 23);\n}\n\n.ag-ltr .ag-row-group-indent-23 {\n  padding-left: calc(23 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-23 {\n  padding-right: calc(23 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-23 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-23 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-24 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 24);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-24 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 24);\n}\n\n.ag-ltr .ag-row-group-indent-24 {\n  padding-left: calc(24 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-24 {\n  padding-right: calc(24 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-24 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-24 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-25 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 25);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-25 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 25);\n}\n\n.ag-ltr .ag-row-group-indent-25 {\n  padding-left: calc(25 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-25 {\n  padding-right: calc(25 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-25 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-25 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-26 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 26);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-26 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 26);\n}\n\n.ag-ltr .ag-row-group-indent-26 {\n  padding-left: calc(26 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-26 {\n  padding-right: calc(26 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-26 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-26 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-27 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 27);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-27 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 27);\n}\n\n.ag-ltr .ag-row-group-indent-27 {\n  padding-left: calc(27 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-27 {\n  padding-right: calc(27 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-27 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-27 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-28 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 28);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-28 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 28);\n}\n\n.ag-ltr .ag-row-group-indent-28 {\n  padding-left: calc(28 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-28 {\n  padding-right: calc(28 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-28 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-28 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-29 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 29);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-29 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 29);\n}\n\n.ag-ltr .ag-row-group-indent-29 {\n  padding-left: calc(29 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-29 {\n  padding-right: calc(29 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-29 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-29 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-30 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 30);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-30 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 30);\n}\n\n.ag-ltr .ag-row-group-indent-30 {\n  padding-left: calc(30 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-30 {\n  padding-right: calc(30 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-30 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-30 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-31 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 31);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-31 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 31);\n}\n\n.ag-ltr .ag-row-group-indent-31 {\n  padding-left: calc(31 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-31 {\n  padding-right: calc(31 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-31 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-31 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-32 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 32);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-32 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 32);\n}\n\n.ag-ltr .ag-row-group-indent-32 {\n  padding-left: calc(32 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-32 {\n  padding-right: calc(32 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-32 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-32 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-33 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 33);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-33 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 33);\n}\n\n.ag-ltr .ag-row-group-indent-33 {\n  padding-left: calc(33 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-33 {\n  padding-right: calc(33 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-33 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-33 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-34 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 34);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-34 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 34);\n}\n\n.ag-ltr .ag-row-group-indent-34 {\n  padding-left: calc(34 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-34 {\n  padding-right: calc(34 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-34 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-34 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-35 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 35);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-35 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 35);\n}\n\n.ag-ltr .ag-row-group-indent-35 {\n  padding-left: calc(35 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-35 {\n  padding-right: calc(35 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-35 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-35 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-36 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 36);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-36 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 36);\n}\n\n.ag-ltr .ag-row-group-indent-36 {\n  padding-left: calc(36 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-36 {\n  padding-right: calc(36 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-36 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-36 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-37 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 37);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-37 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 37);\n}\n\n.ag-ltr .ag-row-group-indent-37 {\n  padding-left: calc(37 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-37 {\n  padding-right: calc(37 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-37 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-37 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-38 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 38);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-38 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 38);\n}\n\n.ag-ltr .ag-row-group-indent-38 {\n  padding-left: calc(38 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-38 {\n  padding-right: calc(38 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-38 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-38 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-39 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 39);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-39 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 39);\n}\n\n.ag-ltr .ag-row-group-indent-39 {\n  padding-left: calc(39 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-39 {\n  padding-right: calc(39 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-39 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-39 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-40 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 40);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-40 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 40);\n}\n\n.ag-ltr .ag-row-group-indent-40 {\n  padding-left: calc(40 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-40 {\n  padding-right: calc(40 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-40 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-40 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-41 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 41);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-41 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 41);\n}\n\n.ag-ltr .ag-row-group-indent-41 {\n  padding-left: calc(41 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-41 {\n  padding-right: calc(41 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-41 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-41 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-42 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 42);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-42 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 42);\n}\n\n.ag-ltr .ag-row-group-indent-42 {\n  padding-left: calc(42 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-42 {\n  padding-right: calc(42 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-42 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-42 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-43 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 43);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-43 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 43);\n}\n\n.ag-ltr .ag-row-group-indent-43 {\n  padding-left: calc(43 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-43 {\n  padding-right: calc(43 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-43 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-43 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-44 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 44);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-44 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 44);\n}\n\n.ag-ltr .ag-row-group-indent-44 {\n  padding-left: calc(44 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-44 {\n  padding-right: calc(44 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-44 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-44 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-45 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 45);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-45 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 45);\n}\n\n.ag-ltr .ag-row-group-indent-45 {\n  padding-left: calc(45 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-45 {\n  padding-right: calc(45 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-45 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-45 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-46 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 46);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-46 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 46);\n}\n\n.ag-ltr .ag-row-group-indent-46 {\n  padding-left: calc(46 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-46 {\n  padding-right: calc(46 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-46 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-46 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-47 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 47);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-47 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 47);\n}\n\n.ag-ltr .ag-row-group-indent-47 {\n  padding-left: calc(47 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-47 {\n  padding-right: calc(47 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-47 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-47 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-48 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 48);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-48 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 48);\n}\n\n.ag-ltr .ag-row-group-indent-48 {\n  padding-left: calc(48 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-48 {\n  padding-right: calc(48 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-48 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-48 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-49 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 49);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-49 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 49);\n}\n\n.ag-ltr .ag-row-group-indent-49 {\n  padding-left: calc(49 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-49 {\n  padding-right: calc(49 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-49 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-49 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-50 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 50);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-50 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 50);\n}\n\n.ag-ltr .ag-row-group-indent-50 {\n  padding-left: calc(50 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-50 {\n  padding-right: calc(50 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-50 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-50 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-51 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 51);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-51 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 51);\n}\n\n.ag-ltr .ag-row-group-indent-51 {\n  padding-left: calc(51 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-51 {\n  padding-right: calc(51 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-51 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-51 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-52 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 52);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-52 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 52);\n}\n\n.ag-ltr .ag-row-group-indent-52 {\n  padding-left: calc(52 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-52 {\n  padding-right: calc(52 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-52 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-52 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-53 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 53);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-53 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 53);\n}\n\n.ag-ltr .ag-row-group-indent-53 {\n  padding-left: calc(53 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-53 {\n  padding-right: calc(53 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-53 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-53 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-54 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 54);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-54 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 54);\n}\n\n.ag-ltr .ag-row-group-indent-54 {\n  padding-left: calc(54 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-54 {\n  padding-right: calc(54 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-54 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-54 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-55 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 55);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-55 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 55);\n}\n\n.ag-ltr .ag-row-group-indent-55 {\n  padding-left: calc(55 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-55 {\n  padding-right: calc(55 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-55 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-55 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-56 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 56);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-56 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 56);\n}\n\n.ag-ltr .ag-row-group-indent-56 {\n  padding-left: calc(56 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-56 {\n  padding-right: calc(56 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-56 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-56 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-57 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 57);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-57 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 57);\n}\n\n.ag-ltr .ag-row-group-indent-57 {\n  padding-left: calc(57 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-57 {\n  padding-right: calc(57 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-57 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-57 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-58 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 58);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-58 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 58);\n}\n\n.ag-ltr .ag-row-group-indent-58 {\n  padding-left: calc(58 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-58 {\n  padding-right: calc(58 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-58 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-58 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-59 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 59);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-59 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 59);\n}\n\n.ag-ltr .ag-row-group-indent-59 {\n  padding-left: calc(59 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-59 {\n  padding-right: calc(59 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-59 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-59 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-60 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 60);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-60 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 60);\n}\n\n.ag-ltr .ag-row-group-indent-60 {\n  padding-left: calc(60 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-60 {\n  padding-right: calc(60 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-60 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-60 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-61 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 61);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-61 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 61);\n}\n\n.ag-ltr .ag-row-group-indent-61 {\n  padding-left: calc(61 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-61 {\n  padding-right: calc(61 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-61 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-61 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-62 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 62);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-62 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 62);\n}\n\n.ag-ltr .ag-row-group-indent-62 {\n  padding-left: calc(62 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-62 {\n  padding-right: calc(62 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-62 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-62 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-63 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 63);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-63 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 63);\n}\n\n.ag-ltr .ag-row-group-indent-63 {\n  padding-left: calc(63 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-63 {\n  padding-right: calc(63 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-63 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-63 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-64 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 64);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-64 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 64);\n}\n\n.ag-ltr .ag-row-group-indent-64 {\n  padding-left: calc(64 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-64 {\n  padding-right: calc(64 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-64 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-64 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-65 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 65);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-65 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 65);\n}\n\n.ag-ltr .ag-row-group-indent-65 {\n  padding-left: calc(65 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-65 {\n  padding-right: calc(65 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-65 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-65 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-66 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 66);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-66 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 66);\n}\n\n.ag-ltr .ag-row-group-indent-66 {\n  padding-left: calc(66 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-66 {\n  padding-right: calc(66 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-66 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-66 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-67 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 67);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-67 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 67);\n}\n\n.ag-ltr .ag-row-group-indent-67 {\n  padding-left: calc(67 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-67 {\n  padding-right: calc(67 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-67 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-67 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-68 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 68);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-68 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 68);\n}\n\n.ag-ltr .ag-row-group-indent-68 {\n  padding-left: calc(68 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-68 {\n  padding-right: calc(68 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-68 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-68 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-69 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 69);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-69 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 69);\n}\n\n.ag-ltr .ag-row-group-indent-69 {\n  padding-left: calc(69 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-69 {\n  padding-right: calc(69 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-69 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-69 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-70 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 70);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-70 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 70);\n}\n\n.ag-ltr .ag-row-group-indent-70 {\n  padding-left: calc(70 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-70 {\n  padding-right: calc(70 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-70 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-70 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-71 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 71);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-71 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 71);\n}\n\n.ag-ltr .ag-row-group-indent-71 {\n  padding-left: calc(71 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-71 {\n  padding-right: calc(71 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-71 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-71 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-72 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 72);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-72 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 72);\n}\n\n.ag-ltr .ag-row-group-indent-72 {\n  padding-left: calc(72 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-72 {\n  padding-right: calc(72 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-72 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-72 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-73 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 73);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-73 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 73);\n}\n\n.ag-ltr .ag-row-group-indent-73 {\n  padding-left: calc(73 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-73 {\n  padding-right: calc(73 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-73 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-73 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-74 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 74);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-74 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 74);\n}\n\n.ag-ltr .ag-row-group-indent-74 {\n  padding-left: calc(74 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-74 {\n  padding-right: calc(74 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-74 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-74 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-75 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 75);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-75 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 75);\n}\n\n.ag-ltr .ag-row-group-indent-75 {\n  padding-left: calc(75 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-75 {\n  padding-right: calc(75 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-75 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-75 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-76 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 76);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-76 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 76);\n}\n\n.ag-ltr .ag-row-group-indent-76 {\n  padding-left: calc(76 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-76 {\n  padding-right: calc(76 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-76 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-76 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-77 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 77);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-77 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 77);\n}\n\n.ag-ltr .ag-row-group-indent-77 {\n  padding-left: calc(77 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-77 {\n  padding-right: calc(77 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-77 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-77 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-78 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 78);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-78 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 78);\n}\n\n.ag-ltr .ag-row-group-indent-78 {\n  padding-left: calc(78 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-78 {\n  padding-right: calc(78 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-78 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-78 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-79 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 79);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-79 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 79);\n}\n\n.ag-ltr .ag-row-group-indent-79 {\n  padding-left: calc(79 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-79 {\n  padding-right: calc(79 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-79 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-79 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-80 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 80);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-80 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 80);\n}\n\n.ag-ltr .ag-row-group-indent-80 {\n  padding-left: calc(80 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-80 {\n  padding-right: calc(80 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-80 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-80 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-81 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 81);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-81 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 81);\n}\n\n.ag-ltr .ag-row-group-indent-81 {\n  padding-left: calc(81 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-81 {\n  padding-right: calc(81 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-81 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-81 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-82 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 82);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-82 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 82);\n}\n\n.ag-ltr .ag-row-group-indent-82 {\n  padding-left: calc(82 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-82 {\n  padding-right: calc(82 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-82 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-82 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-83 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 83);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-83 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 83);\n}\n\n.ag-ltr .ag-row-group-indent-83 {\n  padding-left: calc(83 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-83 {\n  padding-right: calc(83 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-83 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-83 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-84 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 84);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-84 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 84);\n}\n\n.ag-ltr .ag-row-group-indent-84 {\n  padding-left: calc(84 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-84 {\n  padding-right: calc(84 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-84 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-84 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-85 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 85);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-85 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 85);\n}\n\n.ag-ltr .ag-row-group-indent-85 {\n  padding-left: calc(85 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-85 {\n  padding-right: calc(85 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-85 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-85 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-86 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 86);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-86 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 86);\n}\n\n.ag-ltr .ag-row-group-indent-86 {\n  padding-left: calc(86 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-86 {\n  padding-right: calc(86 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-86 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-86 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-87 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 87);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-87 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 87);\n}\n\n.ag-ltr .ag-row-group-indent-87 {\n  padding-left: calc(87 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-87 {\n  padding-right: calc(87 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-87 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-87 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-88 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 88);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-88 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 88);\n}\n\n.ag-ltr .ag-row-group-indent-88 {\n  padding-left: calc(88 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-88 {\n  padding-right: calc(88 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-88 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-88 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-89 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 89);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-89 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 89);\n}\n\n.ag-ltr .ag-row-group-indent-89 {\n  padding-left: calc(89 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-89 {\n  padding-right: calc(89 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-89 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-89 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-90 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 90);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-90 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 90);\n}\n\n.ag-ltr .ag-row-group-indent-90 {\n  padding-left: calc(90 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-90 {\n  padding-right: calc(90 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-90 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-90 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-91 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 91);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-91 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 91);\n}\n\n.ag-ltr .ag-row-group-indent-91 {\n  padding-left: calc(91 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-91 {\n  padding-right: calc(91 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-91 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-91 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-92 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 92);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-92 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 92);\n}\n\n.ag-ltr .ag-row-group-indent-92 {\n  padding-left: calc(92 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-92 {\n  padding-right: calc(92 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-92 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-92 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-93 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 93);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-93 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 93);\n}\n\n.ag-ltr .ag-row-group-indent-93 {\n  padding-left: calc(93 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-93 {\n  padding-right: calc(93 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-93 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-93 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-94 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 94);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-94 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 94);\n}\n\n.ag-ltr .ag-row-group-indent-94 {\n  padding-left: calc(94 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-94 {\n  padding-right: calc(94 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-94 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-94 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-95 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 95);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-95 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 95);\n}\n\n.ag-ltr .ag-row-group-indent-95 {\n  padding-left: calc(95 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-95 {\n  padding-right: calc(95 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-95 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-95 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-96 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 96);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-96 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 96);\n}\n\n.ag-ltr .ag-row-group-indent-96 {\n  padding-left: calc(96 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-96 {\n  padding-right: calc(96 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-96 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-96 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-97 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 97);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-97 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 97);\n}\n\n.ag-ltr .ag-row-group-indent-97 {\n  padding-left: calc(97 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-97 {\n  padding-right: calc(97 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-97 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-97 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-98 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 98);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-98 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 98);\n}\n\n.ag-ltr .ag-row-group-indent-98 {\n  padding-left: calc(98 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-98 {\n  padding-right: calc(98 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-98 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-98 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row > .ag-cell-wrapper.ag-row-group-indent-99 {\n  padding-left: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 99);\n}\n.ag-rtl .ag-row > .ag-cell-wrapper.ag-row-group-indent-99 {\n  padding-right: calc(var(--ag-cell-horizontal-padding) + var(--ag-row-group-indent-size) * 99);\n}\n\n.ag-ltr .ag-row-group-indent-99 {\n  padding-left: calc(99 * var(--ag-row-group-indent-size));\n}\n.ag-rtl .ag-row-group-indent-99 {\n  padding-right: calc(99 * var(--ag-row-group-indent-size));\n}\n\n.ag-ltr .ag-row-level-99 .ag-pivot-leaf-group {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-level-99 .ag-pivot-leaf-group {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-ltr .ag-row-group-leaf-indent {\n  margin-left: var(--ag-row-group-indent-size);\n}\n.ag-rtl .ag-row-group-leaf-indent {\n  margin-right: var(--ag-row-group-indent-size);\n}\n\n.ag-value-change-delta {\n  padding-right: 2px;\n}\n\n.ag-value-change-delta-up {\n  color: var(--ag-value-change-delta-up-color);\n}\n\n.ag-value-change-delta-down {\n  color: var(--ag-value-change-delta-down-color);\n}\n\n.ag-value-change-value {\n  background-color: transparent;\n  border-radius: 1px;\n  padding-left: 1px;\n  padding-right: 1px;\n  transition: background-color 1s;\n}\n\n.ag-value-change-value-highlight {\n  background-color: var(--ag-value-change-value-highlight-background-color);\n  transition: background-color 0.1s;\n}\n\n.ag-cell-data-changed {\n  background-color: var(--ag-value-change-value-highlight-background-color) !important;\n}\n\n.ag-cell-data-changed-animation {\n  background-color: transparent;\n}\n\n.ag-cell-highlight {\n  background-color: var(--ag-range-selection-highlight-color) !important;\n}\n\n.ag-row {\n  height: var(--ag-row-height);\n  background-color: var(--ag-background-color);\n  color: var(--ag-data-color);\n  border-bottom: var(--ag-row-border-style) var(--ag-row-border-color) var(--ag-row-border-width);\n}\n\n.ag-row-highlight-above::after, .ag-row-highlight-below::after {\n  content: "";\n  position: absolute;\n  width: calc(100% - 1px);\n  height: 1px;\n  background-color: var(--ag-range-selection-border-color);\n  left: 1px;\n}\n\n.ag-row-highlight-above::after {\n  top: -1px;\n}\n\n.ag-row-highlight-above.ag-row-first::after {\n  top: 0;\n}\n\n.ag-row-highlight-below::after {\n  bottom: 0px;\n}\n\n.ag-row-odd {\n  background-color: var(--ag-odd-row-background-color);\n}\n\n.ag-body-horizontal-scroll:not(.ag-scrollbar-invisible) .ag-horizontal-left-spacer:not(.ag-scroller-corner) {\n  border-right: var(--ag-borders-critical) var(--ag-border-color);\n}\n.ag-body-horizontal-scroll:not(.ag-scrollbar-invisible) .ag-horizontal-right-spacer:not(.ag-scroller-corner) {\n  border-left: var(--ag-borders-critical) var(--ag-border-color);\n}\n\n.ag-row-selected::before {\n  content: "";\n  background-color: var(--ag-selected-row-background-color);\n  display: block;\n  position: absolute;\n  top: 0;\n  left: 0;\n  right: 0;\n  bottom: 0;\n}\n\n.ag-row-hover:not(.ag-full-width-row)::before,\n.ag-row-hover.ag-full-width-row.ag-row-group::before {\n  content: "";\n  background-color: var(--ag-row-hover-color);\n  display: block;\n  position: absolute;\n  top: 0;\n  left: 0;\n  right: 0;\n  bottom: 0;\n  pointer-events: none;\n}\n\n.ag-row-hover.ag-full-width-row.ag-row-group > * {\n  position: relative;\n}\n\n.ag-row-hover.ag-row-selected::before {\n  background-color: var(--ag-row-hover-color);\n  background-image: linear-gradient(var(--ag-selected-row-background-color), var(--ag-selected-row-background-color));\n}\n\n.ag-column-hover {\n  background-color: var(--ag-column-hover-color);\n}\n\n.ag-ltr .ag-right-aligned-cell {\n  text-align: right;\n}\n.ag-rtl .ag-right-aligned-cell {\n  text-align: left;\n}\n\n.ag-ltr .ag-right-aligned-cell .ag-cell-value,\n.ag-ltr .ag-right-aligned-cell .ag-group-value {\n  margin-left: auto;\n}\n.ag-rtl .ag-right-aligned-cell .ag-cell-value,\n.ag-rtl .ag-right-aligned-cell .ag-group-value {\n  margin-right: auto;\n}\n\n.ag-cell, .ag-full-width-row .ag-cell-wrapper.ag-row-group {\n  --ag-internal-calculated-line-height: var(--ag-line-height, calc(var(--ag-row-height) - var(--ag-row-border-width)));\n  --ag-internal-padded-row-height: calc(var(--ag-row-height) - var(--ag-row-border-width));\n  border: 1px solid transparent;\n  line-height: min(var(--ag-internal-calculated-line-height), var(--ag-internal-padded-row-height));\n  padding-left: calc(var(--ag-cell-horizontal-padding) - 1px);\n  padding-right: calc(var(--ag-cell-horizontal-padding) - 1px);\n  -webkit-font-smoothing: subpixel-antialiased;\n}\n\n.ag-row > .ag-cell-wrapper {\n  padding-left: calc(var(--ag-cell-horizontal-padding) - 1px);\n  padding-right: calc(var(--ag-cell-horizontal-padding) - 1px);\n}\n\n.ag-row-dragging {\n  cursor: move;\n  opacity: 0.5;\n}\n\n.ag-cell-inline-editing {\n  border: var(--ag-borders) var(--ag-border-color);\n  background: var(--ag-background-color);\n  border-radius: var(--ag-card-radius);\n  box-shadow: var(--ag-card-shadow);\n  padding: var(--ag-grid-size);\n  padding: 0;\n  background-color: var(--ag-control-panel-background-color);\n}\n\n.ag-popup-editor {\n  border: var(--ag-borders) var(--ag-border-color);\n  background: var(--ag-background-color);\n  border-radius: var(--ag-card-radius);\n  box-shadow: var(--ag-card-shadow);\n  padding: var(--ag-grid-size);\n  background-color: var(--ag-control-panel-background-color);\n  padding: 0;\n}\n\n.ag-large-text-input {\n  height: auto;\n  padding: var(--ag-cell-horizontal-padding);\n}\n\n.ag-rtl .ag-large-text-input textarea {\n  resize: none;\n}\n\n.ag-details-row {\n  padding: calc(var(--ag-grid-size) * 5);\n  background-color: var(--ag-background-color);\n}\n\n.ag-layout-auto-height .ag-center-cols-clipper, .ag-layout-auto-height .ag-center-cols-container, .ag-layout-print .ag-center-cols-clipper, .ag-layout-print .ag-center-cols-container {\n  min-height: 50px;\n}\n\n.ag-overlay-loading-wrapper {\n  background-color: var(--ag-modal-overlay-background-color);\n}\n\n.ag-overlay-loading-center {\n  border: var(--ag-borders) var(--ag-border-color);\n  background: var(--ag-background-color);\n  border-radius: var(--ag-card-radius);\n  box-shadow: var(--ag-card-shadow);\n  padding: var(--ag-grid-size);\n}\n\n.ag-overlay-no-rows-wrapper.ag-layout-auto-height {\n  padding-top: 30px;\n}\n\n.ag-loading {\n  display: flex;\n  height: 100%;\n  align-items: center;\n}\n.ag-ltr .ag-loading {\n  padding-left: var(--ag-cell-horizontal-padding);\n}\n.ag-rtl .ag-loading {\n  padding-right: var(--ag-cell-horizontal-padding);\n}\n\n.ag-ltr .ag-loading-icon {\n  padding-right: var(--ag-cell-widget-spacing);\n}\n.ag-rtl .ag-loading-icon {\n  padding-left: var(--ag-cell-widget-spacing);\n}\n\n.ag-icon-loading {\n  animation-name: spin;\n  animation-duration: 1000ms;\n  animation-iteration-count: infinite;\n  animation-timing-function: linear;\n}\n\n@keyframes spin {\n  from {\n    transform: rotate(0deg);\n  }\n  to {\n    transform: rotate(360deg);\n  }\n}\n.ag-floating-top {\n  border-bottom: var(--ag-borders-critical) var(--ag-border-color);\n}\n\n.ag-floating-bottom {\n  border-top: var(--ag-borders-critical) var(--ag-border-color);\n}\n\n.ag-ltr .ag-cell {\n  border-right: var(--ag-cell-horizontal-border);\n}\n.ag-rtl .ag-cell {\n  border-left: var(--ag-cell-horizontal-border);\n}\n.ag-ltr .ag-cell {\n  border-right-width: 1px;\n}\n.ag-rtl .ag-cell {\n  border-left-width: 1px;\n}\n\n.ag-cell.ag-cell-first-right-pinned:not(.ag-cell-range-left):not(.ag-cell-range-single-cell) {\n  border-left: var(--ag-borders-critical) var(--ag-border-color);\n}\n\n.ag-cell.ag-cell-last-left-pinned:not(.ag-cell-range-right):not(.ag-cell-range-single-cell) {\n  border-right: var(--ag-borders-critical) var(--ag-border-color);\n}\n\n.ag-cell-range-selected:not(.ag-cell-focus),\n.ag-body-viewport:not(.ag-has-focus) .ag-cell-range-single-cell:not(.ag-cell-inline-editing) {\n  background-color: var(--ag-range-selection-background-color);\n}\n.ag-cell-range-selected:not(.ag-cell-focus).ag-cell-range-chart,\n.ag-body-viewport:not(.ag-has-focus) .ag-cell-range-single-cell:not(.ag-cell-inline-editing).ag-cell-range-chart {\n  background-color: var(--ag-range-selection-chart-background-color) !important;\n}\n.ag-cell-range-selected:not(.ag-cell-focus).ag-cell-range-chart.ag-cell-range-chart-category,\n.ag-body-viewport:not(.ag-has-focus) .ag-cell-range-single-cell:not(.ag-cell-inline-editing).ag-cell-range-chart.ag-cell-range-chart-category {\n  background-color: var(--ag-range-selection-chart-category-background-color) !important;\n}\n\n.ag-cell-range-selected-1:not(.ag-cell-focus),\n.ag-root:not(.ag-context-menu-open) .ag-body-viewport:not(.ag-has-focus) .ag-cell-range-selected-1:not(.ag-cell-inline-editing) {\n  background-color: var(--ag-range-selection-background-color);\n}\n\n.ag-cell-range-selected-2:not(.ag-cell-focus),\n.ag-body-viewport:not(.ag-has-focus) .ag-cell-range-selected-2 {\n  background-color: var(--ag-range-selection-background-color-2);\n}\n\n.ag-cell-range-selected-3:not(.ag-cell-focus),\n.ag-body-viewport:not(.ag-has-focus) .ag-cell-range-selected-3 {\n  background-color: var(--ag-range-selection-background-color-3);\n}\n\n.ag-cell-range-selected-4:not(.ag-cell-focus),\n.ag-body-viewport:not(.ag-has-focus) .ag-cell-range-selected-4 {\n  background-color: var(--ag-range-selection-background-color-4);\n}\n\n.ag-cell.ag-cell-range-selected:not(.ag-cell-range-single-cell).ag-cell-range-top {\n  border-top-color: var(--ag-range-selection-border-color);\n  border-top-style: var(--ag-range-selection-border-style);\n}\n.ag-cell.ag-cell-range-selected:not(.ag-cell-range-single-cell).ag-cell-range-right {\n  border-right-color: var(--ag-range-selection-border-color);\n  border-right-style: var(--ag-range-selection-border-style);\n}\n.ag-cell.ag-cell-range-selected:not(.ag-cell-range-single-cell).ag-cell-range-bottom {\n  border-bottom-color: var(--ag-range-selection-border-color);\n  border-bottom-style: var(--ag-range-selection-border-style);\n}\n.ag-cell.ag-cell-range-selected:not(.ag-cell-range-single-cell).ag-cell-range-left {\n  border-left-color: var(--ag-range-selection-border-color);\n  border-left-style: var(--ag-range-selection-border-style);\n}\n\n.ag-ltr .ag-cell-focus:not(.ag-cell-range-selected):focus-within,\n.ag-ltr .ag-context-menu-open .ag-cell-focus:not(.ag-cell-range-selected),\n.ag-ltr .ag-full-width-row.ag-row-focus:focus .ag-cell-wrapper.ag-row-group,\n.ag-ltr .ag-cell-range-single-cell,\n.ag-ltr .ag-cell-range-single-cell.ag-cell-range-handle, .ag-rtl .ag-cell-focus:not(.ag-cell-range-selected):focus-within,\n.ag-rtl .ag-context-menu-open .ag-cell-focus:not(.ag-cell-range-selected),\n.ag-rtl .ag-full-width-row.ag-row-focus:focus .ag-cell-wrapper.ag-row-group,\n.ag-rtl .ag-cell-range-single-cell,\n.ag-rtl .ag-cell-range-single-cell.ag-cell-range-handle {\n  border: 1px solid;\n  border-color: var(--ag-range-selection-border-color);\n  border-style: var(--ag-range-selection-border-style);\n  outline: initial;\n}\n\n.ag-cell.ag-selection-fill-top,\n.ag-cell.ag-selection-fill-top.ag-cell-range-selected {\n  border-top: 1px dashed;\n  border-top-color: var(--ag-range-selection-border-color);\n}\n\n.ag-ltr .ag-cell.ag-selection-fill-right,\n.ag-ltr .ag-cell.ag-selection-fill-right.ag-cell-range-selected {\n  border-right: 1px dashed var(--ag-range-selection-border-color) !important;\n}\n.ag-rtl .ag-cell.ag-selection-fill-right,\n.ag-rtl .ag-cell.ag-selection-fill-right.ag-cell-range-selected {\n  border-left: 1px dashed var(--ag-range-selection-border-color) !important;\n}\n\n.ag-cell.ag-selection-fill-bottom,\n.ag-cell.ag-selection-fill-bottom.ag-cell-range-selected {\n  border-bottom: 1px dashed;\n  border-bottom-color: var(--ag-range-selection-border-color);\n}\n\n.ag-ltr .ag-cell.ag-selection-fill-left,\n.ag-ltr .ag-cell.ag-selection-fill-left.ag-cell-range-selected {\n  border-left: 1px dashed var(--ag-range-selection-border-color) !important;\n}\n.ag-rtl .ag-cell.ag-selection-fill-left,\n.ag-rtl .ag-cell.ag-selection-fill-left.ag-cell-range-selected {\n  border-right: 1px dashed var(--ag-range-selection-border-color) !important;\n}\n\n.ag-fill-handle, .ag-range-handle {\n  position: absolute;\n  width: 6px;\n  height: 6px;\n  bottom: -1px;\n  background-color: var(--ag-range-selection-border-color);\n}\n.ag-ltr .ag-fill-handle, .ag-ltr .ag-range-handle {\n  right: -1px;\n}\n.ag-rtl .ag-fill-handle, .ag-rtl .ag-range-handle {\n  left: -1px;\n}\n\n.ag-fill-handle {\n  cursor: cell;\n}\n\n.ag-range-handle {\n  cursor: nwse-resize;\n}\n\n.ag-cell-inline-editing {\n  border-color: var(--ag-input-focus-border-color) !important;\n}\n\n.ag-menu {\n  border: var(--ag-borders) var(--ag-border-color);\n  background: var(--ag-background-color);\n  border-radius: var(--ag-card-radius);\n  box-shadow: var(--ag-card-shadow);\n  padding: var(--ag-grid-size);\n  padding: 0;\n}\n\n.ag-menu-list {\n  cursor: default;\n  padding: var(--ag-grid-size) 0;\n}\n\n.ag-menu-separator {\n  height: calc(var(--ag-grid-size) * 2 + 1px);\n}\n\n.ag-menu-separator-part::after {\n  content: "";\n  display: block;\n  border-top: var(--ag-borders-critical) var(--ag-border-color);\n}\n\n.ag-menu-option-active, .ag-compact-menu-option-active {\n  background-color: var(--ag-row-hover-color);\n}\n\n.ag-menu-option-part, .ag-compact-menu-option-part {\n  line-height: var(--ag-icon-size);\n  padding: calc(var(--ag-grid-size) + 2px) 0;\n}\n\n.ag-menu-option-disabled, .ag-compact-menu-option-disabled {\n  opacity: 0.5;\n}\n\n.ag-menu-option-icon, .ag-compact-menu-option-icon {\n  width: var(--ag-icon-size);\n}\n.ag-ltr .ag-menu-option-icon, .ag-ltr .ag-compact-menu-option-icon {\n  padding-left: calc(var(--ag-grid-size) * 2);\n}\n.ag-rtl .ag-menu-option-icon, .ag-rtl .ag-compact-menu-option-icon {\n  padding-right: calc(var(--ag-grid-size) * 2);\n}\n\n.ag-menu-option-text, .ag-compact-menu-option-text {\n  padding-left: calc(var(--ag-grid-size) * 2);\n  padding-right: calc(var(--ag-grid-size) * 2);\n}\n\n.ag-ltr .ag-menu-option-shortcut, .ag-ltr .ag-compact-menu-option-shortcut {\n  padding-right: var(--ag-grid-size);\n}\n.ag-rtl .ag-menu-option-shortcut, .ag-rtl .ag-compact-menu-option-shortcut {\n  padding-left: var(--ag-grid-size);\n}\n\n.ag-menu-option-popup-pointer, .ag-compact-menu-option-popup-pointer {\n  padding-right: var(--ag-grid-size);\n}\n\n.ag-tabs {\n  min-width: var(--ag-tab-min-width);\n}\n\n.ag-tabs-header {\n  width: 100%;\n  display: flex;\n}\n\n.ag-tab {\n  border-bottom: var(--ag-selected-tab-underline-width) solid transparent;\n  transition: border-bottom var(--ag-selected-tab-underline-transition-speed);\n  display: flex;\n  flex: none;\n  align-items: center;\n  justify-content: center;\n  cursor: pointer;\n}\n\n.ag-keyboard-focus .ag-tab:focus {\n  outline: none;\n}\n.ag-keyboard-focus .ag-tab:focus::after {\n  content: "";\n  position: absolute;\n  background-color: transparent;\n  pointer-events: none;\n  top: 4px;\n  left: 4px;\n  display: block;\n  width: calc(100% - 8px);\n  height: calc(100% - 8px);\n  border: 1px solid;\n  border-color: var(--ag-input-focus-border-color);\n}\n\n.ag-tab-selected {\n  border-bottom-color: var(--ag-selected-tab-underline-color);\n}\n\n.ag-menu-header {\n  color: var(--ag-secondary-foreground-color);\n}\n\n.ag-filter-separator {\n  border-top: var(--ag-borders-critical) var(--ag-border-color);\n}\n\n.ag-filter-select .ag-picker-field-wrapper {\n  width: 0;\n}\n\n.ag-filter-condition-operator {\n  height: 17px;\n}\n\n.ag-ltr .ag-filter-condition-operator-or {\n  margin-left: calc(var(--ag-grid-size) * 2);\n}\n.ag-rtl .ag-filter-condition-operator-or {\n  margin-right: calc(var(--ag-grid-size) * 2);\n}\n\n.ag-set-filter-select-all {\n  padding-top: var(--ag-widget-container-vertical-padding);\n}\n\n.ag-set-filter-list, .ag-filter-no-matches {\n  height: calc(var(--ag-list-item-height) * 6);\n}\n\n.ag-set-filter-tree-list {\n  height: calc(var(--ag-list-item-height) * 10);\n}\n\n.ag-set-filter-filter {\n  margin-top: var(--ag-widget-container-vertical-padding);\n  margin-left: var(--ag-widget-container-horizontal-padding);\n  margin-right: var(--ag-widget-container-horizontal-padding);\n}\n\n.ag-filter-to {\n  margin-top: var(--ag-widget-vertical-spacing);\n}\n\n.ag-mini-filter {\n  margin: var(--ag-widget-container-vertical-padding) var(--ag-widget-container-horizontal-padding);\n}\n\n.ag-set-filter-item {\n  margin: 0px var(--ag-widget-container-horizontal-padding);\n}\n\n.ag-ltr .ag-set-filter-add-group-indent {\n  margin-left: calc(var(--ag-widget-container-horizontal-padding) + var(--ag-icon-size) + var(--ag-grid-size) * 2);\n}\n.ag-rtl .ag-set-filter-add-group-indent {\n  margin-right: calc(var(--ag-widget-container-horizontal-padding) + var(--ag-icon-size) + var(--ag-grid-size) * 2);\n}\n\n.ag-ltr .ag-set-filter-indent-1 {\n  padding-left: calc(1 * var(--ag-set-filter-indent-size));\n}\n.ag-rtl .ag-set-filter-indent-1 {\n  padding-right: calc(1 * var(--ag-set-filter-indent-size));\n}\n\n.ag-ltr .ag-set-filter-indent-2 {\n  padding-left: calc(2 * var(--ag-set-filter-indent-size));\n}\n.ag-rtl .ag-set-filter-indent-2 {\n  padding-right: calc(2 * var(--ag-set-filter-indent-size));\n}\n\n.ag-ltr .ag-set-filter-indent-3 {\n  padding-left: calc(3 * var(--ag-set-filter-indent-size));\n}\n.ag-rtl .ag-set-filter-indent-3 {\n  padding-right: calc(3 * var(--ag-set-filter-indent-size));\n}\n\n.ag-ltr .ag-set-filter-indent-4 {\n  padding-left: calc(4 * var(--ag-set-filter-indent-size));\n}\n.ag-rtl .ag-set-filter-indent-4 {\n  padding-right: calc(4 * var(--ag-set-filter-indent-size));\n}\n\n.ag-ltr .ag-set-filter-indent-5 {\n  padding-left: calc(5 * var(--ag-set-filter-indent-size));\n}\n.ag-rtl .ag-set-filter-indent-5 {\n  padding-right: calc(5 * var(--ag-set-filter-indent-size));\n}\n\n.ag-ltr .ag-set-filter-indent-6 {\n  padding-left: calc(6 * var(--ag-set-filter-indent-size));\n}\n.ag-rtl .ag-set-filter-indent-6 {\n  padding-right: calc(6 * var(--ag-set-filter-indent-size));\n}\n\n.ag-ltr .ag-set-filter-indent-7 {\n  padding-left: calc(7 * var(--ag-set-filter-indent-size));\n}\n.ag-rtl .ag-set-filter-indent-7 {\n  padding-right: calc(7 * var(--ag-set-filter-indent-size));\n}\n\n.ag-ltr .ag-set-filter-indent-8 {\n  padding-left: calc(8 * var(--ag-set-filter-indent-size));\n}\n.ag-rtl .ag-set-filter-indent-8 {\n  padding-right: calc(8 * var(--ag-set-filter-indent-size));\n}\n\n.ag-ltr .ag-set-filter-indent-9 {\n  padding-left: calc(9 * var(--ag-set-filter-indent-size));\n}\n.ag-rtl .ag-set-filter-indent-9 {\n  padding-right: calc(9 * var(--ag-set-filter-indent-size));\n}\n\n.ag-ltr .ag-set-filter-group-icons {\n  margin-right: var(--ag-widget-container-horizontal-padding);\n}\n.ag-rtl .ag-set-filter-group-icons {\n  margin-left: var(--ag-widget-container-horizontal-padding);\n}\n\n.ag-filter-apply-panel {\n  padding: var(--ag-widget-container-vertical-padding) var(--ag-widget-container-horizontal-padding);\n  border-top: var(--ag-borders-secondary) var(--ag-secondary-border-color);\n}\n\n.ag-filter-apply-panel-button {\n  line-height: 1.5;\n}\n.ag-ltr .ag-filter-apply-panel-button {\n  margin-left: calc(var(--ag-grid-size) * 2);\n}\n.ag-rtl .ag-filter-apply-panel-button {\n  margin-right: calc(var(--ag-grid-size) * 2);\n}\n\n.ag-simple-filter-body-wrapper {\n  padding: var(--ag-widget-container-vertical-padding) var(--ag-widget-container-horizontal-padding);\n  padding-bottom: calc(var(--ag-widget-container-vertical-padding) - var(--ag-widget-vertical-spacing));\n  overflow-y: auto;\n  min-height: calc(var(--ag-list-item-height) + var(--ag-widget-container-vertical-padding) + var(--ag-widget-vertical-spacing));\n}\n.ag-simple-filter-body-wrapper > * {\n  margin-bottom: var(--ag-widget-vertical-spacing);\n}\n.ag-simple-filter-body-wrapper .ag-resizer-wrapper {\n  margin: 0;\n}\n\n.ag-menu:not(.ag-tabs) .ag-filter .ag-simple-filter-body-wrapper,\n.ag-menu:not(.ag-tabs) .ag-filter > *:not(.ag-filter-wrapper) {\n  min-width: calc(var(--ag-menu-min-width) - 2px);\n}\n\n.ag-filter-no-matches {\n  padding: var(--ag-widget-container-vertical-padding) var(--ag-widget-container-horizontal-padding);\n}\n\n.ag-multi-filter-menu-item {\n  margin: var(--ag-grid-size) 0;\n}\n\n.ag-multi-filter-group-title-bar {\n  padding: calc(var(--ag-grid-size) * 2) var(--ag-grid-size);\n  background-color: transparent;\n}\n\n.ag-group-filter-field-select-wrapper {\n  padding: var(--ag-widget-container-vertical-padding) var(--ag-widget-container-horizontal-padding);\n  padding-bottom: calc(var(--ag-widget-container-vertical-padding) - var(--ag-widget-vertical-spacing));\n}\n.ag-group-filter-field-select-wrapper > * {\n  margin-bottom: var(--ag-widget-vertical-spacing);\n}\n\n.ag-keyboard-focus .ag-multi-filter-group-title-bar:focus {\n  outline: none;\n}\n.ag-keyboard-focus .ag-multi-filter-group-title-bar:focus::after {\n  content: "";\n  position: absolute;\n  background-color: transparent;\n  pointer-events: none;\n  top: 4px;\n  left: 4px;\n  display: block;\n  width: calc(100% - 8px);\n  height: calc(100% - 8px);\n  border: 1px solid;\n  border-color: var(--ag-input-focus-border-color);\n}\n\n.ag-side-bar {\n  position: relative;\n}\n\n.ag-tool-panel-wrapper {\n  width: var(--ag-side-bar-panel-width);\n  background-color: var(--ag-control-panel-background-color);\n}\n\n.ag-side-buttons {\n  padding-top: calc(var(--ag-grid-size) * 4);\n  width: calc(var(--ag-icon-size) + 4px);\n  position: relative;\n  color: var(--ag-foreground-color);\n  overflow: hidden;\n}\n\nbutton.ag-side-button-button {\n  color: inherit;\n  font-family: inherit;\n  font-size: inherit;\n  font-weight: inherit;\n  line-height: inherit;\n  background: transparent;\n  padding: calc(var(--ag-grid-size) * 2) 0 calc(var(--ag-grid-size) * 2) 0;\n  width: 100%;\n  margin: 0;\n  min-height: calc(var(--ag-grid-size) * 18);\n  background-position-y: center;\n  background-position-x: center;\n  background-repeat: no-repeat;\n  border: none;\n  border-top: var(--ag-borders-side-button) var(--ag-border-color);\n  border-bottom: var(--ag-borders-side-button) var(--ag-border-color);\n}\nbutton.ag-side-button-button:focus {\n  box-shadow: none;\n}\n\n.ag-keyboard-focus .ag-side-button-button:focus {\n  outline: none;\n}\n.ag-keyboard-focus .ag-side-button-button:focus::after {\n  content: "";\n  position: absolute;\n  background-color: transparent;\n  pointer-events: none;\n  top: 4px;\n  left: 4px;\n  display: block;\n  width: calc(100% - 8px);\n  height: calc(100% - 8px);\n  border: 1px solid;\n  border-color: var(--ag-input-focus-border-color);\n}\n\n.ag-selected button.ag-side-button-button {\n  background-color: var(--ag-side-button-selected-background-color);\n}\n\n.ag-side-button-icon-wrapper {\n  margin-bottom: 3px;\n}\n\n.ag-ltr .ag-side-bar-left,\n.ag-rtl .ag-side-bar-right {\n  border-right: var(--ag-borders) var(--ag-border-color);\n}\n.ag-ltr .ag-side-bar-left .ag-tool-panel-wrapper,\n.ag-rtl .ag-side-bar-right .ag-tool-panel-wrapper {\n  border-left: var(--ag-borders) var(--ag-border-color);\n}\n.ag-ltr .ag-side-bar-left .ag-side-button-button,\n.ag-rtl .ag-side-bar-right .ag-side-button-button {\n  border-right: var(--ag-selected-tab-underline-width) solid transparent;\n  transition: border-right var(--ag-selected-tab-underline-transition-speed);\n}\n.ag-ltr .ag-side-bar-left .ag-selected .ag-side-button-button,\n.ag-rtl .ag-side-bar-right .ag-selected .ag-side-button-button {\n  border-right-color: var(--ag-selected-tab-underline-color);\n}\n\n.ag-rtl .ag-side-bar-left,\n.ag-ltr .ag-side-bar-right {\n  border-left: var(--ag-borders) var(--ag-border-color);\n}\n.ag-rtl .ag-side-bar-left .ag-tool-panel-wrapper,\n.ag-ltr .ag-side-bar-right .ag-tool-panel-wrapper {\n  border-right: var(--ag-borders) var(--ag-border-color);\n}\n.ag-rtl .ag-side-bar-left .ag-side-button-button,\n.ag-ltr .ag-side-bar-right .ag-side-button-button {\n  border-left: var(--ag-selected-tab-underline-width) solid transparent;\n  transition: border-left var(--ag-selected-tab-underline-transition-speed);\n}\n.ag-rtl .ag-side-bar-left .ag-selected .ag-side-button-button,\n.ag-ltr .ag-side-bar-right .ag-selected .ag-side-button-button {\n  border-left-color: var(--ag-selected-tab-underline-color);\n}\n\n.ag-filter-toolpanel-header {\n  height: calc(var(--ag-grid-size) * 6);\n}\n\n.ag-ltr .ag-filter-toolpanel-header,\n.ag-ltr .ag-filter-toolpanel-search {\n  padding-left: var(--ag-grid-size);\n}\n.ag-rtl .ag-filter-toolpanel-header,\n.ag-rtl .ag-filter-toolpanel-search {\n  padding-right: var(--ag-grid-size);\n}\n\n.ag-keyboard-focus .ag-filter-toolpanel-header:focus {\n  outline: none;\n}\n.ag-keyboard-focus .ag-filter-toolpanel-header:focus::after {\n  content: "";\n  position: absolute;\n  background-color: transparent;\n  pointer-events: none;\n  top: 4px;\n  left: 4px;\n  display: block;\n  width: calc(100% - 8px);\n  height: calc(100% - 8px);\n  border: 1px solid;\n  border-color: var(--ag-input-focus-border-color);\n}\n\n.ag-filter-toolpanel-group.ag-has-filter > .ag-group-title-bar .ag-group-title::after {\n  font-family: var(--ag-icon-font-family);\n  font-size: var(--ag-icon-size);\n  line-height: var(--ag-icon-size);\n  font-style: normal;\n  font-weight: normal;\n  font-variant: normal;\n  text-transform: none;\n  -webkit-font-smoothing: antialiased;\n  -moz-osx-font-smoothing: grayscale;\n  content: var(--ag-icon-font-code-filter, "\\f115");\n  position: absolute;\n}\n.ag-ltr .ag-filter-toolpanel-group.ag-has-filter > .ag-group-title-bar .ag-group-title::after {\n  padding-left: var(--ag-grid-size);\n}\n.ag-rtl .ag-filter-toolpanel-group.ag-has-filter > .ag-group-title-bar .ag-group-title::after {\n  padding-right: var(--ag-grid-size);\n}\n\n.ag-filter-toolpanel-group-level-0-header {\n  height: calc(var(--ag-grid-size) * 8);\n}\n\n.ag-filter-toolpanel-group-item {\n  margin-top: calc(var(--ag-grid-size) * 0.5);\n  margin-bottom: calc(var(--ag-grid-size) * 0.5);\n}\n\n.ag-filter-toolpanel-search {\n  height: var(--ag-header-height);\n}\n\n.ag-filter-toolpanel-search-input {\n  flex-grow: 1;\n  height: calc(var(--ag-grid-size) * 4);\n}\n.ag-ltr .ag-filter-toolpanel-search-input {\n  margin-right: var(--ag-grid-size);\n}\n.ag-rtl .ag-filter-toolpanel-search-input {\n  margin-left: var(--ag-grid-size);\n}\n\n.ag-filter-toolpanel-group-level-0 {\n  border-top: var(--ag-borders-secondary) var(--ag-secondary-border-color);\n}\n\n.ag-ltr .ag-filter-toolpanel-expand,\n.ag-ltr .ag-filter-toolpanel-group-title-bar-icon {\n  margin-right: var(--ag-grid-size);\n}\n.ag-rtl .ag-filter-toolpanel-expand,\n.ag-rtl .ag-filter-toolpanel-group-title-bar-icon {\n  margin-left: var(--ag-grid-size);\n}\n\n.ag-filter-toolpanel-group-level-1 .ag-filter-toolpanel-group-level-1-header.ag-filter-toolpanel-group-title-bar {\n  background-color: transparent;\n}\n.ag-ltr .ag-filter-toolpanel-group-level-1 .ag-filter-toolpanel-group-level-2-header {\n  padding-left: calc(var(--ag-filter-tool-panel-group-indent) * 1 + var(--ag-grid-size));\n}\n.ag-rtl .ag-filter-toolpanel-group-level-1 .ag-filter-toolpanel-group-level-2-header {\n  padding-right: calc(var(--ag-filter-tool-panel-group-indent) * 1 + var(--ag-grid-size));\n}\n\n.ag-filter-toolpanel-group-level-2 .ag-filter-toolpanel-group-level-2-header.ag-filter-toolpanel-group-title-bar {\n  background-color: transparent;\n}\n.ag-ltr .ag-filter-toolpanel-group-level-2 .ag-filter-toolpanel-group-level-3-header {\n  padding-left: calc(var(--ag-filter-tool-panel-group-indent) * 2 + var(--ag-grid-size));\n}\n.ag-rtl .ag-filter-toolpanel-group-level-2 .ag-filter-toolpanel-group-level-3-header {\n  padding-right: calc(var(--ag-filter-tool-panel-group-indent) * 2 + var(--ag-grid-size));\n}\n\n.ag-filter-toolpanel-group-level-3 .ag-filter-toolpanel-group-level-3-header.ag-filter-toolpanel-group-title-bar {\n  background-color: transparent;\n}\n.ag-ltr .ag-filter-toolpanel-group-level-3 .ag-filter-toolpanel-group-level-4-header {\n  padding-left: calc(var(--ag-filter-tool-panel-group-indent) * 3 + var(--ag-grid-size));\n}\n.ag-rtl .ag-filter-toolpanel-group-level-3 .ag-filter-toolpanel-group-level-4-header {\n  padding-right: calc(var(--ag-filter-tool-panel-group-indent) * 3 + var(--ag-grid-size));\n}\n\n.ag-filter-toolpanel-group-level-4 .ag-filter-toolpanel-group-level-4-header.ag-filter-toolpanel-group-title-bar {\n  background-color: transparent;\n}\n.ag-ltr .ag-filter-toolpanel-group-level-4 .ag-filter-toolpanel-group-level-5-header {\n  padding-left: calc(var(--ag-filter-tool-panel-group-indent) * 4 + var(--ag-grid-size));\n}\n.ag-rtl .ag-filter-toolpanel-group-level-4 .ag-filter-toolpanel-group-level-5-header {\n  padding-right: calc(var(--ag-filter-tool-panel-group-indent) * 4 + var(--ag-grid-size));\n}\n\n.ag-filter-toolpanel-group-level-5 .ag-filter-toolpanel-group-level-5-header.ag-filter-toolpanel-group-title-bar {\n  background-color: transparent;\n}\n.ag-ltr .ag-filter-toolpanel-group-level-5 .ag-filter-toolpanel-group-level-6-header {\n  padding-left: calc(var(--ag-filter-tool-panel-group-indent) * 5 + var(--ag-grid-size));\n}\n.ag-rtl .ag-filter-toolpanel-group-level-5 .ag-filter-toolpanel-group-level-6-header {\n  padding-right: calc(var(--ag-filter-tool-panel-group-indent) * 5 + var(--ag-grid-size));\n}\n\n.ag-filter-toolpanel-group-level-6 .ag-filter-toolpanel-group-level-6-header.ag-filter-toolpanel-group-title-bar {\n  background-color: transparent;\n}\n.ag-ltr .ag-filter-toolpanel-group-level-6 .ag-filter-toolpanel-group-level-7-header {\n  padding-left: calc(var(--ag-filter-tool-panel-group-indent) * 6 + var(--ag-grid-size));\n}\n.ag-rtl .ag-filter-toolpanel-group-level-6 .ag-filter-toolpanel-group-level-7-header {\n  padding-right: calc(var(--ag-filter-tool-panel-group-indent) * 6 + var(--ag-grid-size));\n}\n\n.ag-filter-toolpanel-group-level-7 .ag-filter-toolpanel-group-level-7-header.ag-filter-toolpanel-group-title-bar {\n  background-color: transparent;\n}\n.ag-ltr .ag-filter-toolpanel-group-level-7 .ag-filter-toolpanel-group-level-8-header {\n  padding-left: calc(var(--ag-filter-tool-panel-group-indent) * 7 + var(--ag-grid-size));\n}\n.ag-rtl .ag-filter-toolpanel-group-level-7 .ag-filter-toolpanel-group-level-8-header {\n  padding-right: calc(var(--ag-filter-tool-panel-group-indent) * 7 + var(--ag-grid-size));\n}\n\n.ag-filter-toolpanel-group-level-8 .ag-filter-toolpanel-group-level-8-header.ag-filter-toolpanel-group-title-bar {\n  background-color: transparent;\n}\n.ag-ltr .ag-filter-toolpanel-group-level-8 .ag-filter-toolpanel-group-level-9-header {\n  padding-left: calc(var(--ag-filter-tool-panel-group-indent) * 8 + var(--ag-grid-size));\n}\n.ag-rtl .ag-filter-toolpanel-group-level-8 .ag-filter-toolpanel-group-level-9-header {\n  padding-right: calc(var(--ag-filter-tool-panel-group-indent) * 8 + var(--ag-grid-size));\n}\n\n.ag-filter-toolpanel-group-level-9 .ag-filter-toolpanel-group-level-9-header.ag-filter-toolpanel-group-title-bar {\n  background-color: transparent;\n}\n.ag-ltr .ag-filter-toolpanel-group-level-9 .ag-filter-toolpanel-group-level-10-header {\n  padding-left: calc(var(--ag-filter-tool-panel-group-indent) * 9 + var(--ag-grid-size));\n}\n.ag-rtl .ag-filter-toolpanel-group-level-9 .ag-filter-toolpanel-group-level-10-header {\n  padding-right: calc(var(--ag-filter-tool-panel-group-indent) * 9 + var(--ag-grid-size));\n}\n\n.ag-filter-toolpanel-group-level-10 .ag-filter-toolpanel-group-level-10-header.ag-filter-toolpanel-group-title-bar {\n  background-color: transparent;\n}\n.ag-ltr .ag-filter-toolpanel-group-level-10 .ag-filter-toolpanel-group-level-11-header {\n  padding-left: calc(var(--ag-filter-tool-panel-group-indent) * 10 + var(--ag-grid-size));\n}\n.ag-rtl .ag-filter-toolpanel-group-level-10 .ag-filter-toolpanel-group-level-11-header {\n  padding-right: calc(var(--ag-filter-tool-panel-group-indent) * 10 + var(--ag-grid-size));\n}\n\n.ag-filter-toolpanel-instance-header.ag-filter-toolpanel-group-level-1-header {\n  padding-left: var(--ag-grid-size);\n}\n\n.ag-filter-toolpanel-instance-filter {\n  border-bottom: var(--ag-borders) var(--ag-border-color);\n  border-top: var(--ag-borders) var(--ag-border-color);\n  margin-top: var(--ag-grid-size);\n}\n\n.ag-ltr .ag-filter-toolpanel-instance-header-icon {\n  margin-left: var(--ag-grid-size);\n}\n.ag-rtl .ag-filter-toolpanel-instance-header-icon {\n  margin-right: var(--ag-grid-size);\n}\n\n.ag-set-filter-group-icons {\n  color: var(--ag-secondary-foreground-color);\n}\n\n.ag-pivot-mode-panel {\n  min-height: var(--ag-header-height);\n  height: var(--ag-header-height);\n  display: flex;\n}\n\n.ag-pivot-mode-select {\n  display: flex;\n  align-items: center;\n}\n.ag-ltr .ag-pivot-mode-select {\n  margin-left: var(--ag-widget-container-horizontal-padding);\n}\n.ag-rtl .ag-pivot-mode-select {\n  margin-right: var(--ag-widget-container-horizontal-padding);\n}\n\n.ag-keyboard-focus .ag-column-select-header:focus {\n  outline: none;\n}\n.ag-keyboard-focus .ag-column-select-header:focus::after {\n  content: "";\n  position: absolute;\n  background-color: transparent;\n  pointer-events: none;\n  top: 4px;\n  left: 4px;\n  display: block;\n  width: calc(100% - 8px);\n  height: calc(100% - 8px);\n  border: 1px solid;\n  border-color: var(--ag-input-focus-border-color);\n}\n\n.ag-column-select-header {\n  height: var(--ag-header-height);\n  align-items: center;\n  padding: 0 var(--ag-widget-container-horizontal-padding);\n  border-bottom: var(--ag-borders-secondary) var(--ag-secondary-border-color);\n}\n\n.ag-column-panel-column-select {\n  border-bottom: var(--ag-borders-secondary) var(--ag-secondary-border-color);\n  border-top: var(--ag-borders-secondary) var(--ag-secondary-border-color);\n}\n\n.ag-column-group-icons,\n.ag-column-select-header-icon {\n  color: var(--ag-secondary-foreground-color);\n}\n\n.ag-column-select-list .ag-list-item-hovered::after {\n  content: "";\n  position: absolute;\n  left: 0;\n  right: 0;\n  height: 1px;\n  background-color: var(--ag-range-selection-border-color);\n}\n.ag-column-select-list .ag-item-highlight-top::after {\n  top: 0;\n}\n.ag-column-select-list .ag-item-highlight-bottom::after {\n  bottom: 0;\n}\n\n.ag-header {\n  background-color: var(--ag-header-background-color);\n  border-bottom: var(--ag-borders-critical) var(--ag-border-color);\n}\n\n.ag-header-row {\n  color: var(--ag-header-foreground-color);\n  height: var(--ag-header-height);\n}\n\n.ag-pinned-right-header {\n  border-left: var(--ag-borders-critical) var(--ag-border-color);\n}\n\n.ag-pinned-left-header {\n  border-right: var(--ag-borders-critical) var(--ag-border-color);\n}\n\n.ag-ltr .ag-header-cell:not(.ag-right-aligned-header) .ag-header-label-icon {\n  margin-left: var(--ag-grid-size);\n}\n.ag-rtl .ag-header-cell:not(.ag-right-aligned-header) .ag-header-label-icon {\n  margin-right: var(--ag-grid-size);\n}\n\n.ag-ltr .ag-header-cell.ag-right-aligned-header .ag-header-label-icon {\n  margin-right: var(--ag-grid-size);\n}\n.ag-rtl .ag-header-cell.ag-right-aligned-header .ag-header-label-icon {\n  margin-left: var(--ag-grid-size);\n}\n\n.ag-header-cell,\n.ag-header-group-cell {\n  padding-left: var(--ag-cell-horizontal-padding);\n  padding-right: var(--ag-cell-horizontal-padding);\n}\n.ag-header-cell.ag-header-cell-moving,\n.ag-header-group-cell.ag-header-cell-moving {\n  background-color: var(--ag-header-cell-moving-background-color);\n}\n\n.ag-ltr .ag-header-group-cell-label.ag-sticky-label {\n  left: var(--ag-cell-horizontal-padding);\n}\n.ag-rtl .ag-header-group-cell-label.ag-sticky-label {\n  right: var(--ag-cell-horizontal-padding);\n}\n\n.ag-header-cell.ag-header-span-height::after,\n.ag-header-cell.ag-header-span-height .ag-header-cell-resize::after {\n  height: calc(100% - var(--ag-grid-size) * 4);\n  top: calc(var(--ag-grid-size) * 2);\n}\n\n.ag-keyboard-focus .ag-header-cell:focus {\n  outline: none;\n}\n.ag-keyboard-focus .ag-header-cell:focus::after {\n  content: "";\n  position: absolute;\n  background-color: transparent;\n  pointer-events: none;\n  top: 4px;\n  left: 4px;\n  display: block;\n  width: calc(100% - 8px);\n  height: calc(100% - 8px);\n  border: 1px solid;\n  border-color: var(--ag-input-focus-border-color);\n}\n.ag-keyboard-focus .ag-header-group-cell:focus {\n  outline: none;\n}\n.ag-keyboard-focus .ag-header-group-cell:focus::after {\n  content: "";\n  position: absolute;\n  background-color: transparent;\n  pointer-events: none;\n  top: 4px;\n  left: 4px;\n  display: block;\n  width: calc(100% - 8px);\n  height: calc(100% - 8px);\n  border: 1px solid;\n  border-color: var(--ag-input-focus-border-color);\n}\n\n.ag-header-icon {\n  color: var(--ag-secondary-foreground-color);\n}\n\n.ag-header-expand-icon {\n  cursor: pointer;\n}\n.ag-ltr .ag-header-expand-icon {\n  padding-left: 4px;\n}\n.ag-rtl .ag-header-expand-icon {\n  padding-right: 4px;\n}\n\n.ag-header-row:not(:first-child) .ag-header-cell:not(.ag-header-span-height.ag-header-span-total),\n.ag-header-row:not(:first-child) .ag-header-group-cell.ag-header-group-cell-with-group {\n  border-top: var(--ag-borders-critical) var(--ag-border-color);\n}\n\n.ag-header-group-cell:not(.ag-column-resizing) + .ag-header-group-cell:not(.ag-column-hover):not(.ag-header-cell-moving):hover, .ag-header-group-cell:not(.ag-column-resizing) + .ag-header-group-cell:not(.ag-column-hover).ag-column-resizing,\n.ag-header-cell:not(.ag-column-resizing) + .ag-header-cell:not(.ag-column-hover):not(.ag-header-cell-moving):hover,\n.ag-header-cell:not(.ag-column-resizing) + .ag-header-cell:not(.ag-column-hover).ag-column-resizing,\n.ag-header-group-cell:first-of-type:not(.ag-header-cell-moving):hover,\n.ag-header-group-cell:first-of-type.ag-column-resizing,\n.ag-header-cell:not(.ag-column-hover):first-of-type:not(.ag-header-cell-moving):hover,\n.ag-header-cell:not(.ag-column-hover):first-of-type.ag-column-resizing {\n  background-color: var(--ag-header-cell-hover-background-color);\n}\n\n.ag-header-cell::after,\n.ag-header-group-cell::after {\n  content: "";\n  position: absolute;\n  z-index: 1;\n  display: var(--ag-header-column-separator-display);\n  width: var(--ag-header-column-separator-width);\n  height: var(--ag-header-column-separator-height);\n  top: calc(50% - var(--ag-header-column-separator-height) * 0.5);\n  background-color: var(--ag-header-column-separator-color);\n}\n.ag-ltr .ag-header-cell::after,\n.ag-ltr .ag-header-group-cell::after {\n  right: 0;\n}\n.ag-rtl .ag-header-cell::after,\n.ag-rtl .ag-header-group-cell::after {\n  left: 0;\n}\n\n.ag-header-cell-resize {\n  display: flex;\n  align-items: center;\n}\n\n.ag-header-cell-resize::after {\n  content: "";\n  position: absolute;\n  z-index: 1;\n  display: var(--ag-header-column-resize-handle-display);\n  width: var(--ag-header-column-resize-handle-width);\n  height: var(--ag-header-column-resize-handle-height);\n  top: calc(50% - var(--ag-header-column-resize-handle-height) * 0.5);\n  background-color: var(--ag-header-column-resize-handle-color);\n}\n\n.ag-header-cell.ag-header-span-height::after,\n.ag-header-cell.ag-header-span-height .ag-header-cell-resize::after {\n  height: calc(100% - var(--ag-grid-size) * 4);\n  top: calc(var(--ag-grid-size) * 2);\n}\n\n.ag-ltr .ag-header-viewport .ag-header-cell-resize::after {\n  left: calc(50% - var(--ag-header-column-resize-handle-width));\n}\n.ag-rtl .ag-header-viewport .ag-header-cell-resize::after {\n  right: calc(50% - var(--ag-header-column-resize-handle-width));\n}\n\n.ag-pinned-left-header .ag-header-cell-resize::after {\n  left: calc(50% - var(--ag-header-column-resize-handle-width));\n}\n\n.ag-pinned-right-header .ag-header-cell-resize::after {\n  left: 50%;\n}\n\n.ag-ltr .ag-header-select-all {\n  margin-right: var(--ag-cell-horizontal-padding);\n}\n.ag-rtl .ag-header-select-all {\n  margin-left: var(--ag-cell-horizontal-padding);\n}\n\n.ag-ltr .ag-floating-filter-button {\n  margin-left: calc(var(--ag-grid-size) * 3);\n}\n.ag-rtl .ag-floating-filter-button {\n  margin-right: calc(var(--ag-grid-size) * 3);\n}\n\n.ag-floating-filter-button-button {\n  color: inherit;\n  font-family: inherit;\n  font-size: inherit;\n  font-weight: inherit;\n  line-height: inherit;\n  appearance: none;\n  background: transparent;\n  border: none;\n  height: var(--ag-icon-size);\n  padding: 0;\n  width: var(--ag-icon-size);\n}\n\n.ag-filter-loading {\n  background-color: var(--ag-control-panel-background-color);\n  height: 100%;\n  padding: var(--ag-widget-container-vertical-padding) var(--ag-widget-container-horizontal-padding);\n  position: absolute;\n  width: 100%;\n  z-index: 1;\n}\n\n.ag-paging-panel {\n  border-top: 1px solid;\n  border-top-color: var(--ag-border-color);\n  color: var(--ag-secondary-foreground-color);\n  height: var(--ag-header-height);\n}\n.ag-paging-panel > * {\n  margin: 0 var(--ag-cell-horizontal-padding);\n}\n\n.ag-paging-button {\n  cursor: pointer;\n}\n\n.ag-paging-button.ag-disabled {\n  cursor: default;\n  color: var(--ag-disabled-foreground-color);\n}\n\n.ag-keyboard-focus .ag-paging-button:focus {\n  outline: none;\n}\n.ag-keyboard-focus .ag-paging-button:focus::after {\n  content: "";\n  position: absolute;\n  background-color: transparent;\n  pointer-events: none;\n  top: 0px;\n  left: 0px;\n  display: block;\n  width: calc(100% - 0px);\n  height: calc(100% - 0px);\n  border: 1px solid;\n  border-color: var(--ag-input-focus-border-color);\n}\n\n.ag-paging-button, .ag-paging-description {\n  margin: 0 var(--ag-grid-size);\n}\n\n.ag-status-bar {\n  border-top: var(--ag-borders) var(--ag-border-color);\n  color: var(--ag-disabled-foreground-color);\n  padding-right: calc(var(--ag-grid-size) * 4);\n  padding-left: calc(var(--ag-grid-size) * 4);\n  line-height: 1.5;\n}\n\n.ag-status-name-value-value {\n  color: var(--ag-foreground-color);\n}\n\n.ag-status-bar-center {\n  text-align: center;\n}\n\n.ag-status-name-value {\n  margin-left: var(--ag-grid-size);\n  margin-right: var(--ag-grid-size);\n  padding-top: calc(var(--ag-grid-size) * 2);\n  padding-bottom: calc(var(--ag-grid-size) * 2);\n}\n\n.ag-column-drop-cell {\n  background: var(--ag-chip-background-color);\n  border-radius: calc(var(--ag-grid-size) * 4);\n  height: calc(var(--ag-grid-size) * 4);\n  padding: 0 calc(var(--ag-grid-size) * 0.5);\n  border: 1px solid transparent;\n}\n\n.ag-keyboard-focus .ag-column-drop-cell:focus {\n  outline: none;\n}\n.ag-keyboard-focus .ag-column-drop-cell:focus::after {\n  content: "";\n  position: absolute;\n  background-color: transparent;\n  pointer-events: none;\n  top: 2px;\n  left: 2px;\n  display: block;\n  width: calc(100% - 4px);\n  height: calc(100% - 4px);\n  border: 1px solid;\n  border-color: var(--ag-input-focus-border-color);\n}\n\n.ag-column-drop-cell-text {\n  margin: 0 var(--ag-grid-size);\n}\n\n.ag-column-drop-cell-button {\n  min-width: calc(var(--ag-grid-size) * 4);\n  margin: 0 calc(var(--ag-grid-size) * 0.5);\n  color: var(--ag-secondary-foreground-color);\n}\n\n.ag-column-drop-cell-drag-handle {\n  margin-left: calc(var(--ag-grid-size) * 2);\n}\n\n.ag-column-drop-cell-ghost {\n  opacity: 0.5;\n}\n\n.ag-column-drop-horizontal {\n  background-color: var(--ag-control-panel-background-color);\n  color: var(--ag-secondary-foreground-color);\n  height: var(--ag-row-height);\n  border-bottom: var(--ag-borders) var(--ag-border-color);\n}\n.ag-ltr .ag-column-drop-horizontal {\n  padding-left: var(--ag-cell-horizontal-padding);\n}\n.ag-rtl .ag-column-drop-horizontal {\n  padding-right: var(--ag-cell-horizontal-padding);\n}\n\n.ag-ltr .ag-column-drop-horizontal-half-width:not(:last-child) {\n  border-right: var(--ag-borders) var(--ag-border-color);\n}\n.ag-rtl .ag-column-drop-horizontal-half-width:not(:last-child) {\n  border-left: var(--ag-borders) var(--ag-border-color);\n}\n\n.ag-column-drop-horizontal-cell-separator {\n  margin: 0 var(--ag-grid-size);\n  color: var(--ag-secondary-foreground-color);\n}\n\n.ag-column-drop-horizontal-empty-message {\n  color: var(--ag-disabled-foreground-color);\n}\n\n.ag-ltr .ag-column-drop-horizontal-icon {\n  margin-right: var(--ag-cell-horizontal-padding);\n}\n.ag-rtl .ag-column-drop-horizontal-icon {\n  margin-left: var(--ag-cell-horizontal-padding);\n}\n\n.ag-column-drop-vertical-list {\n  padding-bottom: var(--ag-grid-size);\n  padding-right: var(--ag-grid-size);\n  padding-left: var(--ag-grid-size);\n}\n\n.ag-column-drop-vertical-cell {\n  margin-top: var(--ag-grid-size);\n}\n\n.ag-column-drop-vertical {\n  min-height: 50px;\n  border-bottom: var(--ag-borders-secondary) var(--ag-secondary-border-color);\n}\n.ag-column-drop-vertical.ag-last-column-drop {\n  border-bottom: none;\n}\n\n.ag-column-drop-vertical-icon {\n  margin-left: var(--ag-grid-size);\n  margin-right: var(--ag-grid-size);\n}\n\n.ag-column-drop-vertical-empty-message {\n  position: absolute;\n  top: 0;\n  bottom: 0;\n  left: 0;\n  right: 0;\n  overflow: hidden;\n  color: var(--ag-disabled-foreground-color);\n  margin-top: var(--ag-grid-size);\n}\n\n.ag-select-agg-func-popup {\n  border: var(--ag-borders) var(--ag-border-color);\n  background: var(--ag-background-color);\n  border-radius: var(--ag-card-radius);\n  box-shadow: var(--ag-card-shadow);\n  padding: var(--ag-grid-size);\n  background: var(--ag-background-color);\n  height: calc(var(--ag-grid-size) * 5 * 3.5);\n  padding: 0;\n}\n\n.ag-select-agg-func-virtual-list-item {\n  cursor: default;\n  padding-left: calc(var(--ag-grid-size) * 2);\n}\n.ag-select-agg-func-virtual-list-item:hover {\n  background-color: var(--ag-selected-row-background-color);\n}\n\n.ag-keyboard-focus .ag-select-agg-func-virtual-list-item:focus {\n  outline: none;\n}\n.ag-keyboard-focus .ag-select-agg-func-virtual-list-item:focus::after {\n  content: "";\n  position: absolute;\n  background-color: transparent;\n  pointer-events: none;\n  top: 1px;\n  left: 1px;\n  display: block;\n  width: calc(100% - 2px);\n  height: calc(100% - 2px);\n  border: 1px solid;\n  border-color: var(--ag-input-focus-border-color);\n}\n\n.ag-sort-indicator-container {\n  display: flex;\n}\n\n.ag-ltr .ag-sort-indicator-icon {\n  padding-left: var(--ag-grid-size);\n}\n.ag-rtl .ag-sort-indicator-icon {\n  padding-right: var(--ag-grid-size);\n}\n\n.ag-chart {\n  position: relative;\n  display: flex;\n  overflow: hidden;\n  width: 100%;\n  height: 100%;\n}\n\n.ag-chart-components-wrapper {\n  position: relative;\n  display: flex;\n  flex: 1 1 auto;\n  overflow: hidden;\n}\n\n.ag-chart-title-edit {\n  position: absolute;\n  display: none;\n  top: 0;\n  left: 0;\n  text-align: center;\n}\n\n.ag-chart-title-edit.currently-editing {\n  display: inline-block;\n}\n\n.ag-chart-canvas-wrapper {\n  position: relative;\n  flex: 1 1 auto;\n  overflow: hidden;\n}\n\n.ag-charts-canvas {\n  display: block;\n}\n\n.ag-chart-menu {\n  position: absolute;\n  top: 10px;\n  width: 24px;\n  overflow: hidden;\n  display: flex;\n  flex-direction: column;\n}\n.ag-ltr .ag-chart-menu {\n  right: 20px;\n}\n.ag-rtl .ag-chart-menu {\n  left: 20px;\n}\n\n.ag-chart-docked-container {\n  position: relative;\n  width: 0;\n  min-width: 0;\n  transition: min-width 0.4s;\n}\n\n.ag-chart-menu-hidden ~ .ag-chart-docked-container {\n  max-width: 0;\n  overflow: hidden;\n}\n\n.ag-chart-tabbed-menu {\n  width: 100%;\n  height: 100%;\n  display: flex;\n  flex-direction: column;\n  overflow: hidden;\n}\n\n.ag-chart-tabbed-menu-header {\n  flex: none;\n  -moz-user-select: none;\n  -webkit-user-select: none;\n  -ms-user-select: none;\n  user-select: none;\n  cursor: default;\n}\n\n.ag-chart-tabbed-menu-body {\n  display: flex;\n  flex: 1 1 auto;\n  align-items: stretch;\n  overflow: hidden;\n}\n\n.ag-chart-tab {\n  width: 100%;\n  overflow: hidden;\n  overflow-y: auto;\n}\n\n.ag-chart-settings {\n  overflow-x: hidden;\n}\n\n.ag-chart-settings-wrapper {\n  position: relative;\n  flex-direction: column;\n  width: 100%;\n  height: 100%;\n  display: flex;\n  overflow: hidden;\n}\n\n.ag-chart-settings-nav-bar {\n  display: flex;\n  align-items: center;\n  width: 100%;\n  height: 30px;\n  padding: 0 10px;\n  -moz-user-select: none;\n  -webkit-user-select: none;\n  -ms-user-select: none;\n  user-select: none;\n}\n\n.ag-chart-settings-card-selector {\n  display: flex;\n  align-items: center;\n  justify-content: space-around;\n  flex: 1 1 auto;\n  height: 100%;\n  padding: 0 10px;\n}\n\n.ag-chart-settings-card-item {\n  cursor: pointer;\n  width: 10px;\n  height: 10px;\n  background-color: #000;\n  position: relative;\n}\n.ag-chart-settings-card-item.ag-not-selected {\n  opacity: 0.2;\n}\n.ag-chart-settings-card-item::before {\n  content: " ";\n  display: block;\n  position: absolute;\n  background-color: transparent;\n  left: 50%;\n  top: 50%;\n  margin-left: -10px;\n  margin-top: -10px;\n  width: 20px;\n  height: 20px;\n}\n\n.ag-chart-settings-prev,\n.ag-chart-settings-next {\n  position: relative;\n  flex: none;\n}\n\n.ag-chart-settings-prev-button,\n.ag-chart-settings-next-button {\n  position: absolute;\n  top: 0;\n  left: 0;\n  width: 100%;\n  height: 100%;\n  cursor: pointer;\n  opacity: 0;\n}\n\n.ag-chart-settings-mini-charts-container {\n  position: relative;\n  flex: 1 1 auto;\n  overflow-x: hidden;\n  overflow-y: auto;\n}\n\n.ag-chart-settings-mini-wrapper {\n  position: absolute;\n  top: 0;\n  left: 0;\n  display: flex;\n  flex-direction: column;\n  width: 100%;\n  min-height: 100%;\n  overflow: hidden;\n}\n.ag-chart-settings-mini-wrapper.ag-animating {\n  transition: left 0.3s;\n  transition-timing-function: ease-in-out;\n}\n\n.ag-chart-mini-thumbnail {\n  cursor: pointer;\n}\n\n.ag-chart-mini-thumbnail-canvas {\n  display: block;\n}\n\n.ag-chart-data-wrapper,\n.ag-chart-format-wrapper {\n  display: flex;\n  flex-direction: column;\n  position: relative;\n  -moz-user-select: none;\n  -webkit-user-select: none;\n  -ms-user-select: none;\n  user-select: none;\n}\n\n.ag-chart-data-wrapper {\n  height: 100%;\n  overflow-y: auto;\n}\n\n.ag-chart-data-section,\n.ag-chart-format-section {\n  display: flex;\n  margin: 0;\n}\n\n.ag-chart-empty-text {\n  display: flex;\n  top: 0;\n  width: 100%;\n  height: 100%;\n  align-items: center;\n  justify-content: center;\n}\n\n.ag-chart .ag-chart-menu {\n  display: none;\n}\n\n.ag-chart-menu-hidden:hover .ag-chart-menu {\n  display: block;\n}\n\n.ag-chart .ag-chart-tool-panel-button-enable .ag-chart-menu {\n  display: flex;\n  flex-direction: row;\n  overflow: auto;\n  top: 5px;\n  gap: calc(var(--ag-grid-size) * 3 - 8px);\n  width: auto;\n}\n.ag-ltr .ag-chart .ag-chart-tool-panel-button-enable .ag-chart-menu {\n  right: calc(var(--ag-cell-horizontal-padding) + var(--ag-grid-size) - 4px);\n  justify-content: right;\n}\n.ag-rtl .ag-chart .ag-chart-tool-panel-button-enable .ag-chart-menu {\n  left: calc(var(--ag-cell-horizontal-padding) + var(--ag-grid-size) - 4px);\n  justify-content: left;\n}\n\n.ag-chart-menu-close {\n  display: none;\n}\n\n.ag-chart-tool-panel-button-enable .ag-chart-menu-close {\n  position: absolute;\n  top: 50%;\n  transition: transform 0.33s ease-in-out;\n  padding: 0;\n  display: block;\n  cursor: pointer;\n  border: none;\n}\n.ag-ltr .ag-chart-tool-panel-button-enable .ag-chart-menu-close {\n  right: 0px;\n}\n.ag-rtl .ag-chart-tool-panel-button-enable .ag-chart-menu-close {\n  left: 0px;\n}\n.ag-chart-tool-panel-button-enable .ag-chart-menu-close .ag-icon {\n  padding: 14px 5px 14px 2px;\n}\n.ag-chart-tool-panel-button-enable .ag-chart-menu-close:before {\n  content: "";\n  position: absolute;\n  top: -40px;\n  bottom: -40px;\n}\n.ag-ltr .ag-chart-tool-panel-button-enable .ag-chart-menu-close:before {\n  right: 0px;\n}\n.ag-rtl .ag-chart-tool-panel-button-enable .ag-chart-menu-close:before {\n  left: 0px;\n}\n.ag-ltr .ag-chart-tool-panel-button-enable .ag-chart-menu-close:before {\n  left: -10px;\n}\n.ag-rtl .ag-chart-tool-panel-button-enable .ag-chart-menu-close:before {\n  right: -10px;\n}\n.ag-chart-tool-panel-button-enable .ag-icon-menu {\n  display: none;\n}\n\n.ag-ltr .ag-chart-tool-panel-button-enable .ag-chart-menu-close {\n  transform: translate(3px, -50%);\n}\n.ag-ltr .ag-chart-tool-panel-button-enable .ag-chart-menu-close:hover {\n  transform: translate(0, -50%);\n}\n.ag-ltr .ag-chart-menu-visible .ag-chart-tool-panel-button-enable .ag-chart-menu-close:hover {\n  transform: translate(5px, -50%);\n}\n\n.ag-rtl .ag-chart-tool-panel-button-enable .ag-chart-menu-close {\n  transform: translate(-3px, -50%);\n}\n.ag-rtl .ag-chart-tool-panel-button-enable .ag-chart-menu-close:hover {\n  transform: translate(0, -50%);\n}\n.ag-rtl .ag-chart-menu-visible .ag-chart-tool-panel-button-enable .ag-chart-menu-close:hover {\n  transform: translate(-5px, -50%);\n}\n\n.ag-charts-font-size-color {\n  display: flex;\n  align-self: stretch;\n  justify-content: space-between;\n}\n\n.ag-charts-data-group-item {\n  position: relative;\n}\n\n.ag-chart-menu {\n  border-radius: var(--ag-card-radius);\n  background: var(--ag-background-color);\n}\n\n.ag-chart-menu-icon {\n  opacity: 0.5;\n  line-height: 24px;\n  font-size: 24px;\n  width: 24px;\n  height: 24px;\n  margin: 2px 0;\n  cursor: pointer;\n  border-radius: var(--ag-card-radius);\n  color: var(--ag-secondary-foreground-color);\n}\n.ag-chart-menu-icon:hover {\n  opacity: 1;\n}\n\n.ag-chart-mini-thumbnail {\n  border: 1px solid var(--ag-secondary-border-color);\n  border-radius: 5px;\n  margin: 5px;\n}\n.ag-chart-mini-thumbnail:nth-last-child(3), .ag-chart-mini-thumbnail:nth-last-child(3) ~ .ag-chart-mini-thumbnail {\n  margin-left: auto;\n  margin-right: auto;\n}\n.ag-ltr .ag-chart-mini-thumbnail:first-child {\n  margin-left: 0;\n}\n.ag-rtl .ag-chart-mini-thumbnail:first-child {\n  margin-right: 0;\n}\n.ag-ltr .ag-chart-mini-thumbnail:last-child {\n  margin-right: 0;\n}\n.ag-rtl .ag-chart-mini-thumbnail:last-child {\n  margin-left: 0;\n}\n.ag-chart-mini-thumbnail.ag-selected {\n  border-color: var(--ag-minichart-selected-chart-color);\n}\n\n.ag-chart-settings-card-item {\n  background: var(--ag-foreground-color);\n  width: 8px;\n  height: 8px;\n  border-radius: 4px;\n}\n.ag-chart-settings-card-item.ag-selected {\n  background-color: var(--ag-minichart-selected-page-color);\n}\n\n.ag-chart-data-column-drag-handle {\n  margin-left: var(--ag-grid-size);\n}\n\n.ag-charts-settings-group-title-bar,\n.ag-charts-data-group-title-bar,\n.ag-charts-format-top-level-group-title-bar {\n  border-top: var(--ag-borders-secondary) var(--ag-secondary-border-color);\n}\n\n.ag-charts-settings-group-container {\n  padding: var(--ag-grid-size);\n}\n\n.ag-charts-data-group-container {\n  padding: calc(var(--ag-widget-container-vertical-padding) * 0.5) var(--ag-widget-container-horizontal-padding);\n}\n.ag-charts-data-group-container .ag-charts-data-group-item:not(.ag-charts-format-sub-level-group) {\n  height: var(--ag-list-item-height);\n}\n.ag-charts-data-group-container .ag-list-item-hovered::after {\n  content: "";\n  position: absolute;\n  left: 0;\n  right: 0;\n  height: 1px;\n  background-color: var(--ag-range-selection-border-color);\n}\n.ag-charts-data-group-container .ag-item-highlight-top::after {\n  top: 0;\n}\n.ag-charts-data-group-container .ag-item-highlight-bottom::after {\n  bottom: 0;\n}\n\n.ag-charts-format-top-level-group-container {\n  margin-left: calc(var(--ag-grid-size) * 2);\n  padding: var(--ag-grid-size);\n}\n\n.ag-charts-format-top-level-group-item {\n  margin: var(--ag-grid-size) 0;\n}\n\n.ag-charts-format-sub-level-group-container {\n  padding: var(--ag-widget-container-vertical-padding) var(--ag-widget-container-horizontal-padding);\n  padding-bottom: calc(var(--ag-widget-container-vertical-padding) - var(--ag-widget-vertical-spacing));\n}\n.ag-charts-format-sub-level-group-container > * {\n  margin-bottom: var(--ag-widget-vertical-spacing);\n}\n\n.ag-charts-group-container.ag-group-container-horizontal {\n  padding: var(--ag-grid-size);\n}\n\n.ag-chart-data-section,\n.ag-chart-format-section {\n  display: flex;\n  margin: 0;\n}\n\n.ag-chart-menu-panel {\n  background-color: var(--ag-control-panel-background-color);\n}\n.ag-ltr .ag-chart-menu-panel {\n  border-left: solid 1px var(--ag-border-color);\n}\n.ag-rtl .ag-chart-menu-panel {\n  border-right: solid 1px var(--ag-border-color);\n}\n\n.ag-date-time-list-page-title-bar {\n  display: flex;\n}\n\n.ag-date-time-list-page-title {\n  flex-grow: 1;\n  text-align: center;\n}\n\n.ag-date-time-list-page-column-labels-row,\n.ag-date-time-list-page-entries-row {\n  display: flex;\n}\n\n.ag-date-time-list-page-column-label,\n.ag-date-time-list-page-entry {\n  flex-basis: 0;\n  flex-grow: 1;\n}\n\n.ag-date-time-list-page-entry {\n  cursor: pointer;\n  text-align: center;\n}\n\n.ag-date-time-list-page-column-label {\n  text-align: center;\n}\n\n.ag-input-field-input {\n  width: 100%;\n  min-width: 0;\n}\n\n.ag-checkbox-input-wrapper {\n  font-family: var(--ag-icon-font-family);\n  font-size: var(--ag-icon-size);\n  line-height: var(--ag-icon-size);\n  font-style: normal;\n  font-weight: normal;\n  font-variant: normal;\n  text-transform: none;\n  -webkit-font-smoothing: antialiased;\n  -moz-osx-font-smoothing: grayscale;\n  width: var(--ag-icon-size);\n  height: var(--ag-icon-size);\n  background-color: var(--ag-checkbox-background-color);\n  border-radius: var(--ag-checkbox-border-radius);\n  display: inline-block;\n  vertical-align: middle;\n  flex: none;\n}\n.ag-checkbox-input-wrapper input, .ag-checkbox-input-wrapper input {\n  -webkit-appearance: none;\n  opacity: 0;\n  width: 100%;\n  height: 100%;\n}\n.ag-checkbox-input-wrapper:focus-within, .ag-checkbox-input-wrapper:active {\n  outline: none;\n  box-shadow: var(--ag-input-focus-box-shadow);\n}\n.ag-checkbox-input-wrapper.ag-disabled {\n  opacity: 0.5;\n}\n.ag-checkbox-input-wrapper::after {\n  content: var(--ag-icon-font-code-checkbox-unchecked, "\\f108");\n  color: var(--ag-checkbox-unchecked-color);\n  position: absolute;\n  top: 0;\n  left: 0;\n  pointer-events: none;\n}\n.ag-checkbox-input-wrapper.ag-checked::after {\n  content: var(--ag-icon-font-code-checkbox-checked, "\\f106");\n  color: var(--ag-checkbox-checked-color);\n  position: absolute;\n  top: 0;\n  left: 0;\n  pointer-events: none;\n}\n.ag-checkbox-input-wrapper.ag-indeterminate::after {\n  content: var(--ag-icon-font-code-checkbox-indeterminate, "\\f107");\n  color: var(--ag-checkbox-indeterminate-color);\n  position: absolute;\n  top: 0;\n  left: 0;\n  pointer-events: none;\n}\n\n.ag-toggle-button-input-wrapper {\n  box-sizing: border-box;\n  width: var(--ag-toggle-button-width);\n  height: var(--ag-toggle-button-height);\n  background-color: var(--ag-toggle-button-off-background-color);\n  border-radius: calc(var(--ag-toggle-button-height) * 0.5);\n  position: relative;\n  flex: none;\n  border: var(--ag-toggle-button-border-width) solid;\n  border-color: var(--ag-toggle-button-off-border-color);\n}\n.ag-toggle-button-input-wrapper input {\n  opacity: 0;\n  height: 100%;\n  width: 100%;\n}\n.ag-toggle-button-input-wrapper:focus-within {\n  outline: none;\n  box-shadow: var(--ag-input-focus-box-shadow);\n}\n.ag-toggle-button-input-wrapper.ag-disabled {\n  opacity: 0.5;\n}\n.ag-toggle-button-input-wrapper.ag-checked {\n  background-color: var(--ag-toggle-button-on-background-color);\n  border-color: var(--ag-toggle-button-on-border-color);\n}\n.ag-toggle-button-input-wrapper::before {\n  content: " ";\n  position: absolute;\n  top: calc(0px - var(--ag-toggle-button-border-width));\n  left: calc(0px - var(--ag-toggle-button-border-width));\n  display: block;\n  box-sizing: border-box;\n  height: var(--ag-toggle-button-height);\n  width: var(--ag-toggle-button-height);\n  background-color: var(--ag-toggle-button-switch-background-color);\n  border-radius: 100%;\n  transition: left 100ms;\n  border: var(--ag-toggle-button-border-width) solid;\n  border-color: var(--ag-toggle-button-switch-border-color);\n}\n.ag-toggle-button-input-wrapper.ag-checked::before {\n  left: calc(100% - var(--ag-toggle-button-height));\n  border-color: var(--ag-toggle-button-on-border-color);\n}\n\n.ag-radio-button-input-wrapper {\n  font-family: var(--ag-icon-font-family);\n  font-size: var(--ag-icon-size);\n  line-height: var(--ag-icon-size);\n  font-style: normal;\n  font-weight: normal;\n  font-variant: normal;\n  text-transform: none;\n  -webkit-font-smoothing: antialiased;\n  -moz-osx-font-smoothing: grayscale;\n  width: var(--ag-icon-size);\n  height: var(--ag-icon-size);\n  background-color: var(--ag-checkbox-background-color);\n  border-radius: var(--ag-checkbox-border-radius);\n  display: inline-block;\n  vertical-align: middle;\n  flex: none;\n  border-radius: var(--ag-icon-size);\n}\n.ag-radio-button-input-wrapper input, .ag-radio-button-input-wrapper input {\n  -webkit-appearance: none;\n  opacity: 0;\n  width: 100%;\n  height: 100%;\n}\n.ag-radio-button-input-wrapper:focus-within, .ag-radio-button-input-wrapper:active {\n  outline: none;\n  box-shadow: var(--ag-input-focus-box-shadow);\n}\n.ag-radio-button-input-wrapper.ag-disabled {\n  opacity: 0.5;\n}\n.ag-radio-button-input-wrapper::after {\n  content: var(--ag-icon-font-code-radio-button-off, "\\f127");\n  color: var(--ag-checkbox-unchecked-color);\n  position: absolute;\n  top: 0;\n  left: 0;\n  pointer-events: none;\n}\n.ag-radio-button-input-wrapper.ag-checked::after {\n  content: var(--ag-icon-font-code-radio-button-on, "\\f128");\n  color: var(--ag-checkbox-checked-color);\n  position: absolute;\n  top: 0;\n  left: 0;\n  pointer-events: none;\n}\n\ninput[class^=ag-][type=range] {\n  -webkit-appearance: none;\n  width: 100%;\n  height: 100%;\n  background: none;\n  overflow: visible;\n}\ninput[class^=ag-][type=range]::-webkit-slider-runnable-track {\n  margin: 0;\n  padding: 0;\n  width: 100%;\n  height: 3px;\n  background-color: var(--ag-border-color);\n  border-radius: var(--ag-border-radius);\n  border-radius: var(--ag-checkbox-border-radius);\n}\ninput[class^=ag-][type=range]::-moz-range-track {\n  margin: 0;\n  padding: 0;\n  width: 100%;\n  height: 3px;\n  background-color: var(--ag-border-color);\n  border-radius: var(--ag-border-radius);\n  border-radius: var(--ag-checkbox-border-radius);\n}\ninput[class^=ag-][type=range]::-ms-track {\n  margin: 0;\n  padding: 0;\n  width: 100%;\n  height: 3px;\n  background-color: var(--ag-border-color);\n  border-radius: var(--ag-border-radius);\n  border-radius: var(--ag-checkbox-border-radius);\n  color: transparent;\n  width: calc(100% - 2px);\n}\ninput[class^=ag-][type=range]::-webkit-slider-thumb {\n  margin: 0;\n  padding: 0;\n  -webkit-appearance: none;\n  width: var(--ag-icon-size);\n  height: var(--ag-icon-size);\n  background-color: var(--ag-background-color);\n  border: 1px solid;\n  border-color: var(--ag-checkbox-unchecked-color);\n  border-radius: var(--ag-icon-size);\n  transform: translateY(calc(var(--ag-icon-size) * -0.5 + 1.5px));\n}\ninput[class^=ag-][type=range]::-ms-thumb {\n  margin: 0;\n  padding: 0;\n  -webkit-appearance: none;\n  width: var(--ag-icon-size);\n  height: var(--ag-icon-size);\n  background-color: var(--ag-background-color);\n  border: 1px solid;\n  border-color: var(--ag-checkbox-unchecked-color);\n  border-radius: var(--ag-icon-size);\n}\ninput[class^=ag-][type=range]::-moz-ag-range-thumb {\n  margin: 0;\n  padding: 0;\n  -webkit-appearance: none;\n  width: var(--ag-icon-size);\n  height: var(--ag-icon-size);\n  background-color: var(--ag-background-color);\n  border: 1px solid;\n  border-color: var(--ag-checkbox-unchecked-color);\n  border-radius: var(--ag-icon-size);\n}\ninput[class^=ag-][type=range]:focus {\n  outline: none;\n}\ninput[class^=ag-][type=range]:focus::-webkit-slider-thumb {\n  box-shadow: var(--ag-input-focus-box-shadow);\n  border-color: var(--ag-checkbox-checked-color);\n}\ninput[class^=ag-][type=range]:focus::-ms-thumb {\n  box-shadow: var(--ag-input-focus-box-shadow);\n  border-color: var(--ag-checkbox-checked-color);\n}\ninput[class^=ag-][type=range]:focus::-moz-ag-range-thumb {\n  box-shadow: var(--ag-input-focus-box-shadow);\n  border-color: var(--ag-checkbox-checked-color);\n}\ninput[class^=ag-][type=range]:active::-webkit-slider-runnable-track {\n  background-color: var(--ag-input-focus-border-color);\n}\ninput[class^=ag-][type=range]:active::-moz-ag-range-track {\n  background-color: var(--ag-input-focus-border-color);\n}\ninput[class^=ag-][type=range]:active::-ms-track {\n  background-color: var(--ag-input-focus-border-color);\n}\ninput[class^=ag-][type=range]:disabled {\n  opacity: 0.5;\n}\n', ""]), n.exports = e
         },
         8633: (n, e, a) => {
             (e = a(3645)(!1)).push([n.id, '@font-face {\n  font-family: "agGridAlpine";\n  src: url(data:font/woff2;charset=utf-8;base64,d09GMgABAAAAABIkAAsAAAAAJkAAABHTAAEAAAAAAAAAAAAAAAAAAAAAAAAAAAAAHIkABmAAiyoKp0ygSgE2AiQDgjALgRoABCAFhEYHhRwbXyFFIbBxAJDYv7AiqieV7P96QZO4Gu9qEMLAgorXqyjcVJKxQxvbtQieEq6u3unbTP3JwOa8v9MeN5Q8Caix/+09wyXRVJ6IfU2IWoiiiWgSIp5JhMSQaX44l/dN+kSUcPER5OzkhHT7gd9m7/PN/wkLMCowCmy8M+qHlXA73abzZiEb3DVcFEavrFyzTvMyXLeieOl4CQlIYbBNxUopM8Nip4zZ0vd82bEQmAQkTsiVYMv9DdPoIJ9DCT5BRcD/P/dqmWTV4A1khZ6f04HXNve+mwJnKdEvp5wBsgWC/5ues98OENRmp4Dl3IQnoXcm1Jydm/+MzfZ0da0rjEJkDPufQ66CYNqwBz9fhdkubhpvRgCmW3MZ9WZ/0uxT+y+dsRzmrRhA3DGcOn50v6mbLFgQE4TvcWyxpK4fl3wNVrgUXkcWRp2jpdEz0efRd9H/kLC2pYAY6p8bw1GEICmaIYgthlYsNmTaHE5dVpnJdT5rWQJjpIs2p6m7ldKIo45RDyqaUsSD6yDj7q/uKinhvdMmTBLlEbCopjVbTsRV0kGei7DXN54VtteylXaUdDSPaa+Ac+UhaYEJNa52HUV2kA3cQVq+tcAxp7Qg6+K2mETrApdi6y3eLMI7dcZFkraCSQ6fzNip7qiKcLCVq+hvOa+AcXspHXiIvvxUcX3a1wHrxZzkxYFOPnjf2Xg8Ude1oja/f90i7i5lKbx40E0ta2DETVJc1dUZ9731xTff/fQfAlOFFHn4ADa/ImNPzMrDspK+zTTH3fmko4S0xESEddPEKWoamIMWga2TmJgoWgsM4TRYdzRdSNbprCHLhgWnnE8zmBjTQzBCwjSHsNniQK3NttnmW3czBzI2JyyqamyrrpUbo0ujalAu3kWxjDzTJqyQU1wXgKVTps2ZdOequYYwYi9NleshqbVeXtI50VQwtbP69rfCNLch55ioujFqKGxo4mYj7c/yesxOmNzAPsTNyMw+pNzaEJRX6LjuTpooygim0BCQROxcCPpaO1xHDSO5mK5Y5GG4Lw4iNyIfcJu9+/DD5sAAEWaUd0mjRxqHfLH+F0FXsSNWFX9FGg/mYsDpOQqsA2IgMl1cHmJQWLcOEuU9GOwfM4UZsIU/59z49b95g/V+nXThF1LJnhHE/dZ1QxxYnrlTMF9xt6IhJF+RyJoCJwPOOJecvbaewIBgpuDiQsMiomLiEpJS0jKyctRai0rKKvhFWFPX0NTS1tHV0zcwNDI2MTUzt7C00ra2sQUhwRvONbatFefI79QbbmnxpFVf//15cb7l9tcep/1MQPQxGvpYv1cOfT/YVuAAq+AgKwCHWB2HWRI4wro4yrYBx1gJOM7SwElWxilWBE6zBs6wLHCWZYBzrIULbDtwkeWBSywFXGZNXGEdXGU54Bqr4jpr48bAHr+AvkSAEAVCDAhxICSAkARCChBSgZAGhHQgZAAhEwhZQMgGQg4QcoGQB4R8IBQAoRAIRUAoBkIJEEqBUAaEciBUAKESCFVAqAZCDRBqgVAHhHogNAChEQhNQGgGQgsQWoHQBoR2IHQAoRMIXUDoBkIP1K7TC/SmDwj9AEiyyBPxCDeJ32Jq/L5SuCTQgA+9YgrDr0OwVUVexYVeyFNcwF0FuoE0V1IcHYu52gT+0kXBK4nr6el0CcZlMiPM9IKDQY100KueobGOYYxqXmE2bizVAIvs3nqFKcc2YSnyk3Q66OkY8nTCVJah4UHTi65clskzVJytzLmz0OWG+nq6ehZcVgN2CUBdufG7YapTyZhAEsBCmDTFKiHIKIpeKyIJIV1OElQuSUcvo0RIF3kpyKIZOErmSCplKmKxYhTkUoyaXolRUsvfwaJMisimqRySziJkuA5G4YBJcQYmM1KdmYYUM2dxY/X5OURfOXuuSUKTUvLpEAvZCEemZ6S/uQf1kkyysiqfJsnvzYbNx8FV9QKi9O3ylLF1OaUYAy/Yp+PoaciqKjvhIGOqrgDDdVlkUKq4irNkPegq57Eipi6rWqrHMyGppKQSWtZGLfNK70FU8OU882IMadJnkR3cThwvKld0DA9jqsHRrq4+RLltSour902A71VtvK5RTDUNekfUY1bt7WoNqRjfi6lc227klPfOTg2uHkOUXYO8wdFJ5dTYMHeMdJ7lvq1LNQw0Gq7LDq7m3YIm6XY+omzVKGDi++/FrjYexeNdwt5ZLWnrH9vFXdPkSZeWFIuLquVlRBlPESMzkDpP5coKrg4uU+0dV0zsU2unlJP7a1RXiPGinJeSBe19ozvNZNkEOtaEyqyS9jSDpjpmVw7h6hELkuYPSG6xBbgTpKbTru2qQR7Vtr63Y6pRRLleIs0iyOpsEbnSrrMmuWbTi1HRUdmL2OLyMsXjz62Qexf9l2YprqazKVG6XCaisrR9qPEmV+jlrFDVq1cCY3GRkEovXwl+GbHYL4PilZUK5dJH8W1lBBAohXBqSMhB6HqKziZICc7AaAzByf2crEsnlgETqQA2kueLAAWoywPhAIuVlpBEliUohuuZSWdXVuVQrALl8ct4Rd4KNSy9dAwh50x3FRjg6otHl45cwKC2tRbjYChuC/a1mVROBRNh1eyBjmFtHkr5EgPF4fqz4DIWA0NuMjCZ0evIPq2gIKUKZLbn3UsbKSKaJkmCEpH0DMysVEbyRHQf/XxVHlquUi0LpQeXQFFpDBnWd0l1wRqbBwGcc2OqRxTDqlHl2Bq2Lg4sBJdS/Hb/VZgS70mk+/zGIof4Ve7j7ntDCK7GYov3eJgzRQirt5t1cC2IU4IT7lX8MbtuR0uaq8E1/CErSrZracnmx9yexUXBH+W7l5dtfyroX1kJ/buMrbNE71mwW6lRcHuvBrsgUrPXE+QZryHAuK83Dzja7GToaa8xu3UKBxyhFu1xhFaprlgTOIJXAG7bNx9Svh0TAE6fwgBvnA5l8HzFV3wlrzKbVDSoS1RTo/aeqieNT83co86TR95gAusmS1J/b6/lALsa18FKLKl5ZVWFVFIgvSxS8j0JXcLNbCTmGDUaxEjQuyjIOr+CrPdPYCS+gTyzCFdPP+XcZTcSyJ0tp8H3b5+HomdemfChsI0ZbXD9VUCKUO2xrGivk03b1tZH07k08kT6JVFe0Z5h8EHX6uoL4sX/q6Op8AJ28Zq60rDikJDisNK/WtobLw4pDfsrJ33yOzXfF3QiVRNeBVhVsOSBcu0z+XN5Q4O8UQ6h361itj7ztmfxvI8t3h8HJ4zLTUs7fWrHjrR0setzL+9ab356MzZX5T+wXugerh8dGOgqL2cwoqNO17WdPnV6Knp8/IvrpIUjJIKjBXHjCwi88rwuqG5XazcytQ0Hn8Ya4Nf7hM3Y0F+fnSN4oYceOoGjmBA/bM0+7whOYkdwZCWOYicot13nxefhQXBuXlxcXsorGUos0XKdE4TM/y+t2rhemTCDuEndAtwkbiH7/2vip3NXrP5uaPoMWTRwjzH6CVk/sMz80mbezEga8Lw/get4YiNqyo90NTHsYzVHvRfE4c8F2u+vsqdpi03s3mm2hTmXZ8M+99AE/4Ld8k7tDaYxZcIe4D8K2Qq+Zn/xTFp1Grn9rDUR6X/amrAM84fjeLztp0x6Ir/w3O+hNfcEbjPekIrpmgsWzNe1c/YWmQde9DXA+k3qYIIZvOlQyErOpYXYGI8gMiCQlHQMGSg5fgAZJIwpayqqdyuwD8prEtdABgS52gykWJ7tCe4+G7yvO7hnH4q4NWY0prsWXWnk288F2nai4hAIjB+a0FQZmac3fzq36e13v6h5myfiGDs+icwT5fVdJU4YcPyYxqlpNTlNh743+cLczDyY3kQ1B3+ia8Cx55hArTZ0ZoXdfv5eHv62C1qxmHQvobrj61usMzw8Q+ILj13UVhUGVlPQnVDfbJUREZ6SVllqcCE+O8AiprRcEZKclew00hfslezhkeQVjOmXNAblxB7FRJBYnBbhlG8eUyZR8wWg5uIt/aQ732hfdUVpuUWM+pgR/1hl1Ld0x080OZ+HdbKVVUb4x92e2qSWdhoZGhAy2+aSnv3a3FUjmsoS/jS73ur58Sd4LDh8qHB0MJZzD4iHBNj02HKhtlUkF+1vDRcVKMwPI1quwUudMEwYqhUFilp3yUXyWSqUP2sNrJMNojBR67Mk7CothruzDWLjsqXAxPbF6urI5MHIc+kVtj5wspx1GswYDC8JDS3e0NKG8FRPTrOWTiMe6UR6w45FMSR6VgkvqXMDlqmC1E9dHj+WJHoeEknyogSpgrmUzML6dNb1kJKMoCuVvMMuYWNj7q8IEhuLIL/qL5g+IvJ+8fQLBF4NrxPWyetE+/WFdSDc5S4fMr18lgX4OT6jr7yhR8JC4R+bu6HaE3leH0VT5dXtSg8OFHineqWkeKV6F4RLnbbMz1s6SVNNkRZe1hsEfFA9ufgq89WJKUdw7N5TMrMkGX/i9IkjXnzBreRuQj4gJyBT/s03BpYR6erTXavvlpd+PRwltP3BxiZl119JSdJKXR1z54iMU+9qNH//rf3nS7+vZuWPuruLNphgFhYbK3j69cbfa+q/w/9Y5t9bWIAA05HaBA+PBH3UujT9kP5QG8wCzd/D5hfhobd1bxk4BJkY3HpywZhjEuRwV7aP3aEliBxC+2mtu0dSomfde59qk/eI0HbeFfC+XTIMsUnSb93UchDe0pFvFj4VpGzUgeIWkeiArLUFUe7bhjEd/nXr5kOtteJNm2Hi3ugrqjHy6tXoul+VFLrmuqhULrmuhRda2ukq1X3Vha4XOO71Kj5cWxiSJxDkhRT+lFJuPE9QGPJTris8uJWwIS5uw6chRdqn4V8X/6yZcrv42JGXsqSZUAz/rF493qxzp0XTYbeEgUL4p4udVqXgMYeeEtiQ+k/WP6mc81tj+eRJXFxEuK1tbCxoY+uK6+DehFlmdIWSVAjHj88iBzwkoetChLAsKtxmvsR9R2FOjoG4WqloF78TEz7fbsdhJe4BSdoRG4qLkpMHB4P27oPWzW/evN78B3jNGLdRnzcvKgS9NQQAABqnMk0jSSTYabMJrYTmkyqPplkCqkAPa1/HKABvXqLr0JvOcv3oz7rGQ4qKrtaZzPRqxD8ht3UfTJSX0rUMxkm37g16DV2FNloTqmhXqNAnVVf4FzUaUg5a02WzFZVBm6wJZFOaMFPRasShjG5pLYCiLJlXie5ATZvW4x19sim9+l+py4OFtD12JZyoRwY4ugqA5Bv+fUjhjE9/oQEwflXQYVi0KpjY78hJv0woYmXN2R96//v7AiGM+n53VSkGzJ0P4PfzQiM45QhEgscGA/Q3HICGuil8dQLtmC7g4AV6vMAQwNZ6HE6NgymsBRQQHUNAwBwULmMAGzoAReAg6CDwENMFHiyDHgJvFmBA/W8g46vh4Irkd0b4kuheUomE3xiGZCU7Qfwm/1FqZDKPGzYVXd0XEopVdKZbTB3Dk6o3XjibT6ZxSSmxKcI/CNr2quX5fuMR95pb4LxhBV9E5LxIioigb7jZfYPEEonJcoz/cA0V7xsjxqPWg6Tvl8KUJkBhdYzOcrRXo+CJ+oZn9i7Bcig+tSqSkHzge1H4rh8IXLPVK4jyf6dUM/OyZgu0cNsVjGqSXt/9sAUKBg4BCQXqTwSAL/Dq1/P/n5OUyebyhWKpXKnW6o1mq93p9vqD4Wg8mc7mi+VqvdkSyriQSlu243p+pVqrN5qtdqfb6w/kWsexg2CwGpn27AhPddse2IMgwLQLlxW9WK0Rfjuem6AY3V3mDJEcKkqOZBWvinIGkrKfQCeWpsREqOzfwyFTPYImFQuKbge6LLswXOs2nHEbXt1xWWEXv7q1g5VRrHaP7hB/bGqytd8OS/d8pRq13d1Vqu6EiWX3LOWh7JRqyppe91JRw2e5n9q6SOEgxxxzXHEnJw2PiKJzpZx1h5rwmFobmxJP6HaLhnPE7VK0W2pkPSiDY+ShXsiF3g433aDK1LD355neaFcq9LpTY8Sjej80NI4nipQ20THUKnRwJ3cYdGQ2cqWCSKQ4zLblgnQwPEN5LptWIJCKGJlUIOn96swaJxsUi5G3rg0A);\n  font-weight: normal;\n  font-style: normal;\n}\n.ag-theme-alpine, .ag-theme-alpine-dark {\n  --ag-alpine-active-color: #2196f3;\n  --ag-selected-row-background-color: rgba(33, 150, 243, 0.3);\n  --ag-row-hover-color: rgba(33, 150, 243, 0.1);\n  --ag-column-hover-color: rgba(33, 150, 243, 0.1);\n  --ag-input-focus-border-color: rgba(33, 150, 243, 0.4);\n  --ag-range-selection-background-color: rgba(33, 150, 243, 0.2);\n  --ag-range-selection-background-color-2: rgba(33, 150, 243, 0.36);\n  --ag-range-selection-background-color-3: rgba(33, 150, 243, 0.49);\n  --ag-range-selection-background-color-4: rgba(33, 150, 243, 0.59);\n  --ag-background-color: #fff;\n  --ag-foreground-color: #181d1f;\n  --ag-border-color: #babfc7;\n  --ag-secondary-border-color: #dde2eb;\n  --ag-header-background-color: #f8f8f8;\n  --ag-tooltip-background-color: #f8f8f8;\n  --ag-odd-row-background-color: #fcfcfc;\n  --ag-control-panel-background-color: #f8f8f8;\n  --ag-subheader-background-color: #fff;\n  --ag-invalid-color: #e02525;\n  --ag-checkbox-unchecked-color: #999;\n  --ag-checkbox-background-color: var(--ag-background-color);\n  --ag-checkbox-checked-color: var(--ag-alpine-active-color);\n  --ag-range-selection-border-color: var(--ag-alpine-active-color);\n  --ag-secondary-foreground-color: var(--ag-foreground-color);\n  --ag-input-border-color: var(--ag-border-color);\n  --ag-input-border-color-invalid: var(--ag-invalid-color);\n  --ag-input-focus-box-shadow: 0 0 2px 0.1rem var(--ag-input-focus-border-color);\n  --ag-disabled-foreground-color: rgba(24, 29, 31, 0.5);\n  --ag-chip-background-color: rgba(24, 29, 31, 0.07);\n  --ag-input-disabled-border-color: rgba(186, 191, 199, 0.3);\n  --ag-input-disabled-background-color: rgba(186, 191, 199, 0.15);\n  --ag-borders: solid 1px;\n  --ag-border-radius: 3px;\n  --ag-borders-side-button: none;\n  --ag-side-button-selected-background-color: transparent;\n  --ag-header-column-resize-handle-display: block;\n  --ag-header-column-resize-handle-width: 2px;\n  --ag-header-column-resize-handle-height: 30%;\n  --ag-grid-size: 6px;\n  --ag-icon-size: 16px;\n  --ag-row-height: calc(var(--ag-grid-size) * 7);\n  --ag-header-height: calc(var(--ag-grid-size) * 8);\n  --ag-list-item-height: calc(var(--ag-grid-size) * 4);\n  --ag-column-select-indent-size: var(--ag-icon-size);\n  --ag-set-filter-indent-size: var(--ag-icon-size);\n  --ag-cell-horizontal-padding: calc(var(--ag-grid-size) * 3);\n  --ag-cell-widget-spacing: calc(var(--ag-grid-size) * 2);\n  --ag-widget-container-vertical-padding: calc(var(--ag-grid-size) * 2);\n  --ag-widget-container-horizontal-padding: calc(var(--ag-grid-size) * 2);\n  --ag-widget-vertical-spacing: calc(var(--ag-grid-size) * 1.5);\n  --ag-toggle-button-height: 18px;\n  --ag-toggle-button-width: 28px;\n  --ag-font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Oxygen-Sans, Ubuntu, Cantarell, "Helvetica Neue", sans-serif;\n  --ag-font-size: 13px;\n  --ag-icon-font-family: agGridAlpine;\n  --ag-selected-tab-underline-color: var(--ag-alpine-active-color);\n  --ag-selected-tab-underline-width: 2px;\n  --ag-selected-tab-underline-transition-speed: 0.3s;\n  --ag-tab-min-width: 240px;\n  --ag-card-shadow: 0 1px 4px 1px rgba(186, 191, 199, 0.4);\n  --ag-popup-shadow: var(--ag-card-shadow);\n  --ag-side-bar-panel-width: 250px;\n}\n\n.ag-theme-alpine-dark {\n  --ag-background-color: #181d1f;\n  --ag-foreground-color: #fff;\n  --ag-border-color: #68686e;\n  --ag-secondary-border-color: rgba(88, 86, 82, 0.5);\n  --ag-modal-overlay-background-color: rgba(24, 29, 31, 0.66);\n  --ag-header-background-color: #222628;\n  --ag-tooltip-background-color: #222628;\n  --ag-odd-row-background-color: #222628;\n  --ag-control-panel-background-color: #222628;\n  --ag-subheader-background-color: #000;\n  --ag-input-disabled-background-color: #282c2f;\n  --ag-input-focus-box-shadow:\n      0 0 2px 0.5px rgba(255, 255, 255, 0.5),\n      0 0 4px 3px var(--ag-input-focus-border-color);\n  --ag-card-shadow: 0 1px 20px 1px black;\n  --ag-disabled-foreground-color: rgba(255, 255, 255, 0.5);\n  --ag-chip-background-color: rgba(255, 255, 255, 0.07);\n  --ag-input-disabled-border-color: rgba(104, 104, 110, 0.3);\n  --ag-input-disabled-background-color: rgba(104, 104, 110, 0.07);\n}\n\n.ag-theme-alpine .ag-filter-toolpanel-header,\n.ag-theme-alpine .ag-filter-toolpanel-search,\n.ag-theme-alpine .ag-status-bar,\n.ag-theme-alpine .ag-header-row,\n.ag-theme-alpine .ag-panel-title-bar-title,\n.ag-theme-alpine .ag-multi-filter-group-title-bar, .ag-theme-alpine-dark .ag-filter-toolpanel-header,\n.ag-theme-alpine-dark .ag-filter-toolpanel-search,\n.ag-theme-alpine-dark .ag-status-bar,\n.ag-theme-alpine-dark .ag-header-row,\n.ag-theme-alpine-dark .ag-panel-title-bar-title,\n.ag-theme-alpine-dark .ag-multi-filter-group-title-bar {\n  font-weight: 700;\n  color: var(--ag-header-foreground-color);\n}\n.ag-theme-alpine .ag-row, .ag-theme-alpine-dark .ag-row {\n  font-size: calc(var(--ag-font-size) + 1px);\n}\n.ag-theme-alpine input[class^=ag-]:not([type]),\n.ag-theme-alpine input[class^=ag-][type=text],\n.ag-theme-alpine input[class^=ag-][type=number],\n.ag-theme-alpine input[class^=ag-][type=tel],\n.ag-theme-alpine input[class^=ag-][type=date],\n.ag-theme-alpine input[class^=ag-][type=datetime-local],\n.ag-theme-alpine textarea[class^=ag-], .ag-theme-alpine-dark input[class^=ag-]:not([type]),\n.ag-theme-alpine-dark input[class^=ag-][type=text],\n.ag-theme-alpine-dark input[class^=ag-][type=number],\n.ag-theme-alpine-dark input[class^=ag-][type=tel],\n.ag-theme-alpine-dark input[class^=ag-][type=date],\n.ag-theme-alpine-dark input[class^=ag-][type=datetime-local],\n.ag-theme-alpine-dark textarea[class^=ag-] {\n  min-height: calc(var(--ag-grid-size) * 4);\n  border-radius: var(--ag-border-radius);\n}\n.ag-theme-alpine .ag-ltr input[class^=ag-]:not([type]), .ag-theme-alpine .ag-ltr input[class^=ag-][type=text], .ag-theme-alpine .ag-ltr input[class^=ag-][type=number], .ag-theme-alpine .ag-ltr input[class^=ag-][type=tel], .ag-theme-alpine .ag-ltr input[class^=ag-][type=date], .ag-theme-alpine .ag-ltr input[class^=ag-][type=datetime-local], .ag-theme-alpine .ag-ltr textarea[class^=ag-], .ag-theme-alpine-dark .ag-ltr input[class^=ag-]:not([type]), .ag-theme-alpine-dark .ag-ltr input[class^=ag-][type=text], .ag-theme-alpine-dark .ag-ltr input[class^=ag-][type=number], .ag-theme-alpine-dark .ag-ltr input[class^=ag-][type=tel], .ag-theme-alpine-dark .ag-ltr input[class^=ag-][type=date], .ag-theme-alpine-dark .ag-ltr input[class^=ag-][type=datetime-local], .ag-theme-alpine-dark .ag-ltr textarea[class^=ag-] {\n  padding-left: var(--ag-grid-size);\n}\n\n.ag-theme-alpine .ag-rtl input[class^=ag-]:not([type]), .ag-theme-alpine .ag-rtl input[class^=ag-][type=text], .ag-theme-alpine .ag-rtl input[class^=ag-][type=number], .ag-theme-alpine .ag-rtl input[class^=ag-][type=tel], .ag-theme-alpine .ag-rtl input[class^=ag-][type=date], .ag-theme-alpine .ag-rtl input[class^=ag-][type=datetime-local], .ag-theme-alpine .ag-rtl textarea[class^=ag-], .ag-theme-alpine-dark .ag-rtl input[class^=ag-]:not([type]), .ag-theme-alpine-dark .ag-rtl input[class^=ag-][type=text], .ag-theme-alpine-dark .ag-rtl input[class^=ag-][type=number], .ag-theme-alpine-dark .ag-rtl input[class^=ag-][type=tel], .ag-theme-alpine-dark .ag-rtl input[class^=ag-][type=date], .ag-theme-alpine-dark .ag-rtl input[class^=ag-][type=datetime-local], .ag-theme-alpine-dark .ag-rtl textarea[class^=ag-] {\n  padding-right: var(--ag-grid-size);\n}\n\n.ag-theme-alpine .ag-tab, .ag-theme-alpine-dark .ag-tab {\n  padding: calc(var(--ag-grid-size) * 1.5);\n  transition: color 0.4s;\n  flex: 1 1 auto;\n}\n.ag-theme-alpine .ag-tab-selected, .ag-theme-alpine-dark .ag-tab-selected {\n  color: var(--ag-alpine-active-color);\n}\n.ag-theme-alpine .ag-menu, .ag-theme-alpine-dark .ag-menu {\n  background-color: var(--ag-control-panel-background-color);\n}\n.ag-theme-alpine .ag-menu-header, .ag-theme-alpine-dark .ag-menu-header {\n  background-color: var(--ag-control-panel-background-color);\n  padding-top: 1px;\n}\n.ag-theme-alpine .ag-tabs-header, .ag-theme-alpine-dark .ag-tabs-header {\n  border-bottom: var(--ag-borders) var(--ag-border-color);\n}\n.ag-theme-alpine .ag-charts-settings-group-title-bar,\n.ag-theme-alpine .ag-charts-data-group-title-bar,\n.ag-theme-alpine .ag-charts-format-top-level-group-title-bar, .ag-theme-alpine-dark .ag-charts-settings-group-title-bar,\n.ag-theme-alpine-dark .ag-charts-data-group-title-bar,\n.ag-theme-alpine-dark .ag-charts-format-top-level-group-title-bar {\n  padding: var(--ag-grid-size) calc(var(--ag-grid-size) * 2);\n  line-height: calc(var(--ag-icon-size) + var(--ag-grid-size) - 2px);\n}\n.ag-theme-alpine .ag-chart-mini-thumbnail, .ag-theme-alpine-dark .ag-chart-mini-thumbnail {\n  background-color: var(--ag-background-color);\n}\n.ag-theme-alpine .ag-chart-settings-nav-bar, .ag-theme-alpine-dark .ag-chart-settings-nav-bar {\n  border-top: var(--ag-borders-secondary) var(--ag-secondary-border-color);\n}\n.ag-theme-alpine .ag-ltr .ag-group-title-bar-icon, .ag-theme-alpine-dark .ag-ltr .ag-group-title-bar-icon {\n  margin-right: var(--ag-grid-size);\n}\n\n.ag-theme-alpine .ag-rtl .ag-group-title-bar-icon, .ag-theme-alpine-dark .ag-rtl .ag-group-title-bar-icon {\n  margin-left: var(--ag-grid-size);\n}\n\n.ag-theme-alpine .ag-charts-format-top-level-group-toolbar, .ag-theme-alpine-dark .ag-charts-format-top-level-group-toolbar {\n  margin-top: var(--ag-grid-size);\n}\n.ag-theme-alpine .ag-ltr .ag-charts-format-top-level-group-toolbar, .ag-theme-alpine-dark .ag-ltr .ag-charts-format-top-level-group-toolbar {\n  padding-left: calc(var(--ag-icon-size) * 0.5 + var(--ag-grid-size) * 2);\n}\n\n.ag-theme-alpine .ag-rtl .ag-charts-format-top-level-group-toolbar, .ag-theme-alpine-dark .ag-rtl .ag-charts-format-top-level-group-toolbar {\n  padding-right: calc(var(--ag-icon-size) * 0.5 + var(--ag-grid-size) * 2);\n}\n\n.ag-theme-alpine .ag-charts-format-sub-level-group, .ag-theme-alpine-dark .ag-charts-format-sub-level-group {\n  border-left: dashed 1px;\n  border-left-color: var(--ag-border-color);\n  padding-left: var(--ag-grid-size);\n  margin-bottom: calc(var(--ag-grid-size) * 2);\n}\n.ag-theme-alpine .ag-charts-format-sub-level-group-title-bar, .ag-theme-alpine-dark .ag-charts-format-sub-level-group-title-bar {\n  padding-top: 0;\n  padding-bottom: 0;\n  background: none;\n  font-weight: 700;\n}\n.ag-theme-alpine .ag-charts-format-sub-level-group-container, .ag-theme-alpine-dark .ag-charts-format-sub-level-group-container {\n  padding-bottom: 0;\n}\n.ag-theme-alpine .ag-charts-format-sub-level-group-item:last-child, .ag-theme-alpine-dark .ag-charts-format-sub-level-group-item:last-child {\n  margin-bottom: 0;\n}\n.ag-theme-alpine.ag-dnd-ghost, .ag-theme-alpine-dark.ag-dnd-ghost {\n  font-size: calc(var(--ag-font-size) - 1px);\n  font-weight: 700;\n}\n.ag-theme-alpine .ag-side-buttons, .ag-theme-alpine-dark .ag-side-buttons {\n  width: calc(var(--ag-grid-size) * 5);\n}\n.ag-theme-alpine .ag-standard-button, .ag-theme-alpine-dark .ag-standard-button {\n  appearance: none;\n  -webkit-appearance: none;\n  border-radius: var(--ag-border-radius);\n  border: 1px solid;\n  border-color: var(--ag-alpine-active-color);\n  color: var(--ag-alpine-active-color);\n  background-color: var(--ag-background-color);\n  font-weight: 600;\n  padding: var(--ag-grid-size) calc(var(--ag-grid-size) * 2);\n}\n.ag-theme-alpine .ag-standard-button:hover, .ag-theme-alpine-dark .ag-standard-button:hover {\n  border-color: var(--ag-alpine-active-color);\n  background-color: var(--ag-row-hover-color);\n}\n.ag-theme-alpine .ag-standard-button:active, .ag-theme-alpine-dark .ag-standard-button:active {\n  border-color: var(--ag-alpine-active-color);\n  background-color: var(--ag-alpine-active-color);\n  color: var(--ag-background-color);\n}\n.ag-theme-alpine .ag-standard-button:disabled, .ag-theme-alpine-dark .ag-standard-button:disabled {\n  color: var(--ag-disabled-foreground-color);\n  background-color: var(--ag-input-disabled-background-color);\n  border-color: var(--ag-input-disabled-border-color);\n}\n.ag-theme-alpine .ag-column-drop-vertical, .ag-theme-alpine-dark .ag-column-drop-vertical {\n  min-height: 75px;\n}\n.ag-theme-alpine .ag-column-drop-vertical-title-bar, .ag-theme-alpine-dark .ag-column-drop-vertical-title-bar {\n  padding: calc(var(--ag-grid-size) * 2);\n  padding-bottom: 0px;\n}\n.ag-theme-alpine .ag-column-drop-vertical-empty-message, .ag-theme-alpine-dark .ag-column-drop-vertical-empty-message {\n  display: flex;\n  align-items: center;\n  border: dashed 1px;\n  border-color: var(--ag-border-color);\n  margin: calc(var(--ag-grid-size) * 2);\n  padding: calc(var(--ag-grid-size) * 2);\n}\n.ag-theme-alpine .ag-column-drop-empty-message, .ag-theme-alpine-dark .ag-column-drop-empty-message {\n  color: var(--ag-foreground-color);\n  opacity: 0.75;\n}\n.ag-theme-alpine .ag-status-bar, .ag-theme-alpine-dark .ag-status-bar {\n  font-weight: normal;\n}\n.ag-theme-alpine .ag-status-name-value-value, .ag-theme-alpine-dark .ag-status-name-value-value {\n  font-weight: 700;\n}\n.ag-theme-alpine .ag-paging-number, .ag-theme-alpine .ag-paging-row-summary-panel-number, .ag-theme-alpine-dark .ag-paging-number, .ag-theme-alpine-dark .ag-paging-row-summary-panel-number {\n  font-weight: 700;\n}\n.ag-theme-alpine .ag-column-drop-cell-button, .ag-theme-alpine-dark .ag-column-drop-cell-button {\n  opacity: 0.5;\n}\n.ag-theme-alpine .ag-column-drop-cell-button:hover, .ag-theme-alpine-dark .ag-column-drop-cell-button:hover {\n  opacity: 0.75;\n}\n.ag-theme-alpine .ag-header-cell-menu-button:hover,\n.ag-theme-alpine .ag-side-button-button:hover,\n.ag-theme-alpine .ag-tab:hover,\n.ag-theme-alpine .ag-panel-title-bar-button:hover,\n.ag-theme-alpine .ag-header-expand-icon:hover,\n.ag-theme-alpine .ag-column-group-icons:hover,\n.ag-theme-alpine .ag-set-filter-group-icons:hover,\n.ag-theme-alpine .ag-group-expanded .ag-icon:hover,\n.ag-theme-alpine .ag-group-contracted .ag-icon:hover,\n.ag-theme-alpine .ag-chart-settings-prev:hover,\n.ag-theme-alpine .ag-chart-settings-next:hover,\n.ag-theme-alpine .ag-group-title-bar-icon:hover,\n.ag-theme-alpine .ag-column-select-header-icon:hover,\n.ag-theme-alpine .ag-floating-filter-button-button:hover,\n.ag-theme-alpine .ag-filter-toolpanel-expand:hover,\n.ag-theme-alpine .ag-chart-menu-icon:hover,\n.ag-theme-alpine .ag-chart-menu-close:hover, .ag-theme-alpine-dark .ag-header-cell-menu-button:hover,\n.ag-theme-alpine-dark .ag-side-button-button:hover,\n.ag-theme-alpine-dark .ag-tab:hover,\n.ag-theme-alpine-dark .ag-panel-title-bar-button:hover,\n.ag-theme-alpine-dark .ag-header-expand-icon:hover,\n.ag-theme-alpine-dark .ag-column-group-icons:hover,\n.ag-theme-alpine-dark .ag-set-filter-group-icons:hover,\n.ag-theme-alpine-dark .ag-group-expanded .ag-icon:hover,\n.ag-theme-alpine-dark .ag-group-contracted .ag-icon:hover,\n.ag-theme-alpine-dark .ag-chart-settings-prev:hover,\n.ag-theme-alpine-dark .ag-chart-settings-next:hover,\n.ag-theme-alpine-dark .ag-group-title-bar-icon:hover,\n.ag-theme-alpine-dark .ag-column-select-header-icon:hover,\n.ag-theme-alpine-dark .ag-floating-filter-button-button:hover,\n.ag-theme-alpine-dark .ag-filter-toolpanel-expand:hover,\n.ag-theme-alpine-dark .ag-chart-menu-icon:hover,\n.ag-theme-alpine-dark .ag-chart-menu-close:hover {\n  color: var(--ag-alpine-active-color);\n}\n.ag-theme-alpine .ag-chart-menu-close, .ag-theme-alpine-dark .ag-chart-menu-close {\n  background: var(--ag-background-color);\n}\n.ag-theme-alpine .ag-chart-menu-close:hover .ag-icon, .ag-theme-alpine-dark .ag-chart-menu-close:hover .ag-icon {\n  border-color: var(--ag-alpine-active-color);\n}\n.ag-theme-alpine .ag-chart-menu-close .ag-icon, .ag-theme-alpine-dark .ag-chart-menu-close .ag-icon {\n  background: var(--ag-header-background-color);\n  border: 1px solid var(--ag-border-color);\n  border-right: none;\n}\n.ag-theme-alpine .ag-chart-settings-card-item.ag-not-selected:hover, .ag-theme-alpine-dark .ag-chart-settings-card-item.ag-not-selected:hover {\n  opacity: 0.35;\n}\n.ag-theme-alpine .ag-ltr .ag-panel-title-bar-button, .ag-theme-alpine-dark .ag-ltr .ag-panel-title-bar-button {\n  margin-left: calc(var(--ag-grid-size) * 2);\n  margin-right: var(--ag-grid-size);\n}\n\n.ag-theme-alpine .ag-rtl .ag-panel-title-bar-button, .ag-theme-alpine-dark .ag-rtl .ag-panel-title-bar-button {\n  margin-right: calc(var(--ag-grid-size) * 2);\n  margin-left: var(--ag-grid-size);\n}\n\n.ag-theme-alpine .ag-ltr .ag-filter-toolpanel-group-container, .ag-theme-alpine-dark .ag-ltr .ag-filter-toolpanel-group-container {\n  padding-left: var(--ag-grid-size);\n}\n\n.ag-theme-alpine .ag-rtl .ag-filter-toolpanel-group-container, .ag-theme-alpine-dark .ag-rtl .ag-filter-toolpanel-group-container {\n  padding-right: var(--ag-grid-size);\n}\n\n.ag-theme-alpine .ag-filter-toolpanel-instance-filter, .ag-theme-alpine-dark .ag-filter-toolpanel-instance-filter {\n  border: none;\n  background-color: var(--ag-control-panel-background-color);\n}\n.ag-theme-alpine .ag-ltr .ag-filter-toolpanel-instance-filter, .ag-theme-alpine-dark .ag-ltr .ag-filter-toolpanel-instance-filter {\n  border-left: dashed 1px;\n  border-left-color: var(--ag-border-color);\n  margin-left: calc(var(--ag-icon-size) * 0.5);\n}\n\n.ag-theme-alpine .ag-rtl .ag-filter-toolpanel-instance-filter, .ag-theme-alpine-dark .ag-rtl .ag-filter-toolpanel-instance-filter {\n  border-right: dashed 1px;\n  border-right-color: var(--ag-border-color);\n  margin-right: calc(var(--ag-icon-size) * 0.5);\n}\n\n.ag-theme-alpine .ag-set-filter-list, .ag-theme-alpine-dark .ag-set-filter-list {\n  padding-top: calc(var(--ag-grid-size) * 0.5);\n  padding-bottom: calc(var(--ag-grid-size) * 0.5);\n}\n.ag-theme-alpine .ag-layout-auto-height .ag-center-cols-clipper, .ag-theme-alpine .ag-layout-auto-height .ag-center-cols-container, .ag-theme-alpine .ag-layout-print .ag-center-cols-clipper, .ag-theme-alpine .ag-layout-print .ag-center-cols-container, .ag-theme-alpine-dark .ag-layout-auto-height .ag-center-cols-clipper, .ag-theme-alpine-dark .ag-layout-auto-height .ag-center-cols-container, .ag-theme-alpine-dark .ag-layout-print .ag-center-cols-clipper, .ag-theme-alpine-dark .ag-layout-print .ag-center-cols-container {\n  min-height: 150px;\n}\n.ag-theme-alpine .ag-overlay-no-rows-wrapper.ag-layout-auto-height, .ag-theme-alpine-dark .ag-overlay-no-rows-wrapper.ag-layout-auto-height {\n  padding-top: 60px;\n}\n.ag-theme-alpine .ag-date-time-list-page-entry-is-current, .ag-theme-alpine-dark .ag-date-time-list-page-entry-is-current {\n  background-color: var(--ag-alpine-active-color);\n}\n\n.ag-theme-alpine-dark {\n  color-scheme: dark;\n}\n', ""]), n.exports = e
         },
```

### Comparing `buckaroo-0.2.6/dcef/labextension/static/250.c608416dcff072a71036.js.LICENSE.txt` & `buckaroo-0.2.7/buckaroo/labextension/static/250.b55e2550464d9477eb95.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `buckaroo-0.2.6/dcef/labextension/static/480.55b0b32536a517ae86fb.js` & `buckaroo-0.2.7/buckaroo/labextension/static/480.e809fc8a18bc53e804a1.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-(self.webpackChunkdcef = self.webpackChunkdcef || []).push([
+(self.webpackChunkbuckaroo = self.webpackChunkbuckaroo || []).push([
     [480], {
         8399: function(e, n, t) {
             "use strict";
             var o = this && this.__createBinding || (Object.create ? function(e, n, t, o) {
                     void 0 === o && (o = t), Object.defineProperty(e, o, {
                         enumerable: !0,
                         get: function() {
@@ -27,16 +27,16 @@
                         for (var t in e) "default" !== t && Object.prototype.hasOwnProperty.call(e, t) && o(n, e, t);
                     return i(n, e), n
                 };
             Object.defineProperty(n, "__esModule", {
                 value: !0
             }), n.DCEFWidgetView = n.DCEFWidgetModel = void 0;
             const a = t(2492),
-                s = t(7049),
-                r = l(t(7294)),
+                r = t(7049),
+                s = l(t(7294)),
                 d = l(t(745)),
                 u = t(8657);
             t(9423), t(3054), t(4260), t(801);
             class c extends a.DOMWidgetModel {
                 defaults() {
                     return Object.assign(Object.assign({}, super.defaults()), {
                         _model_name: c.model_name,
@@ -49,58 +49,39 @@
                         operations: [],
                         operation_results: {},
                         dfConfig: {}
                     })
                 }
             }
             n.DCEFWidgetModel = c, c.serializers = Object.assign({}, a.DOMWidgetModel.serializers), c.model_name = "DCEFWidgetModel", c.model_module = u.MODULE_NAME, c.model_module_version = u.MODULE_VERSION, c.view_name = "ExampleView", c.view_module = u.MODULE_NAME, c.view_module_version = u.MODULE_VERSION;
-            class p extends a.DOMWidgetView {
-                constructor() {
-                    super(...arguments), this.setCommandConfig = e => console.log("default setCommandConfig"), this.setPyCode = e => console.log("default setPyCode"), this.setTransformedDf = e => console.log("default setTransformedDf")
-                }
+            class b extends a.DOMWidgetView {
                 render() {
                     this.el.classList.add("custom-widget");
-                    const e = this.model,
-                        n = this;
-                    e.on("change:commandConfig", (() => {
-                        n.setCommandConfig(e.get("commandConfig"))
-                    }), this);
-                    const t = {
-                            getOrRequester: n => (e.on("change:operation_results", (() => {
-                                const t = e.get("operation_results");
-                                console.log("about to call setOpResult with", t), n(t)
-                            }), this), n => {
-                                console.log("orRequester passed operations", n), e.set("operations", n), e.save_changes()
-                            }),
-                            exposeCommandConfigSetter: e => {
-                                n.setCommandConfig = e
-                            }
-                        },
-                        o = document.getElementsByClassName("jp-NotebookPanel-notebook")[0],
-                        i = this.el.getBoundingClientRect().y,
-                        l = o.getBoundingClientRect().y - i + 50;
-                    o.scroll(0, l);
-                    const a = d.createRoot(this.el),
-                        u = r.default.createElement((() => {
-                            const [e, n] = r.useState(0), o = () => {
+                    const e = document.getElementsByClassName("jp-NotebookPanel-notebook")[0],
+                        n = this.el.getBoundingClientRect().y,
+                        t = e.getBoundingClientRect().y - n + 50;
+                    e.scroll(0, t);
+                    const o = d.createRoot(this.el),
+                        i = s.default.createElement((() => {
+                            const [e, n] = s.useState(0), t = () => {
                                 n((e => e + 1))
                             };
-                            r.useEffect((() => {
-                                this.listenTo(this.model, "change", o)
+                            s.useEffect((() => {
+                                this.listenTo(this.model, "change", t)
                             }), []);
-                            const i = Object.assign({}, t);
-                            for (const e of Object.keys(this.model.attributes)) i[e] = this.model.get(e), i["on_" + e] = n => {
+                            const o = {};
+                            for (const e of Object.keys(this.model.attributes)) o[e] = this.model.get(e), o["on_" + e] = n => {
                                 this.model.set(e, n), this.touch()
                             };
-                            return r.default.createElement(s.WidgetDCFCell, i)
+                            return s.default.createElement(r.WidgetDCFCell, o)
                         }), {});
-                    a.render(u)
+                    o.render(i)
                 }
             }
-            n.DCEFWidgetView = p
+            n.DCEFWidgetView = b
         },
         4480: function(e, n, t) {
             "use strict";
             var o = this && this.__createBinding || (Object.create ? function(e, n, t, o) {
                     void 0 === o && (o = t), Object.defineProperty(e, o, {
                         enumerable: !0,
                         get: function() {
@@ -125,25 +106,25 @@
                         for (var t in e) "default" !== t && Object.prototype.hasOwnProperty.call(e, t) && o(n, e, t);
                     return i(n, e), n
                 };
             Object.defineProperty(n, "__esModule", {
                 value: !0
             });
             const a = t(2492),
-                s = t(3033),
-                r = t(8657),
+                r = t(3033),
+                s = t(8657),
                 d = l(t(8399)),
                 u = {
-                    id: "dcef:plugin",
+                    id: "buckaroo:plugin",
                     requires: [a.IJupyterWidgetRegistry],
-                    optional: [s.IThemeManager],
+                    optional: [r.IThemeManager],
                     activate: function(e, n, t) {
-                        console.log("dcef_widget plugin.ts after change EXTENSION_ID"), n.registerWidget({
-                            name: r.MODULE_NAME,
-                            version: r.MODULE_VERSION,
+                        console.log("buckaroo_widget plugin.ts after change EXTENSION_ID"), n.registerWidget({
+                            name: s.MODULE_NAME,
+                            version: s.MODULE_VERSION,
                             exports: Object.assign({}, d)
                         })
                     },
                     autoStart: !0
                 };
             n.default = u
         },
@@ -186,11 +167,11 @@
                 hmr: !0,
                 transform: void 0,
                 insertInto: void 0
             }), o.locals && (e.exports = o.locals)
         },
         4147: e => {
             "use strict";
-            e.exports = JSON.parse('{"name":"dcef","version":"0.2.1","description":"Fast Datagrid widget for the Jupyter Notebook and JupyterLab","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","lib/**/*.js.map","lib/**/*.ts","dist/*.js","dist/*.js.map","dist/*.png","style/**/*.*"],"homepage":"https://github.com/paddymul/dcef","bugs":{"url":"https://github.com/paddymul/dcef/issues"},"license":"BSD-3-Clause","author":{"name":"Paddy Mullen","email":""},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/paddymul/dcef"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:dev":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack --mode=production --no-devtool","build:widget-examples":"cd widget-examples/basic && webpack --mode=production","build:all":"yarn run build:labextension && yarn run build:nbextension && yarn run build:widget-examples","clean":"rimraf dist && yarn run clean:lib && yarn run clean:labextension && yarn run clean:nbextension","clean:lib":"rimraf lib","clean:labextension":"rimraf dcef/labextension","clean:nbextension":"rimraf dcef/nbextension/index.*","lint":"eslint \'js/**/*.{ts,tsx}\'","lint:fix":"eslint \'js/**/*.{ts,tsx} --fix\'","prepack":"yarn run build:labextension && yarn run build:nbextension","test":"jest --verbose","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^2 || ^3 || ^4 || ^6.0.0","@jupyterlab/apputils":"^3.0.2","paddy-react-edit-list":">=1.1.35","lodash":"^4.17.21","react-dom":"^18.0.0","react":"^18.0.0"},"devDependencies":{"@babel/cli":"^7.6.3","@babel/core":"^7.6.3","@babel/preset-env":"^7.6.3","@babel/preset-typescript":"^7.6.0","@jupyterlab/builder":"^3.0.1","@types/jest":"^27.4.1","@types/react":"^18.0.0","@types/react-dom":"^18.0.0","@types/node":"^10.11.6","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.5.0","@typescript-eslint/parser":"^3.5.0","acorn":"^6.2.0","babel-jest":"^28.1.3","babel-plugin-transform-es2015-modules-commonjs":"^6.26.2","css-loader":"^3.0.0","eslint":"^7.3.1","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","jest":"^28.1.3","lint-staged":"^10.2.11","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","rimraf":"^2.6.2","source-map-loader":"^0.2.4","style-loader":"^0.23.1","svg-url-loader":"~3.0.3","ts-jest":"^28.0.8","ts-loader":"^6.0.4","typescript":"~4.2.4","url-loader":"^4.1.0","webpack":"^5","webpack-cli":"^4.4.0"},"jupyterlab":{"extension":"lib/plugin","webpackConfig":"webpack.lab.config.js","outputDir":"./dcef/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true},"@lumino/algorithm":{"bundled":false,"singleton":true},"@lumino/commands":{"bundled":false,"singleton":true},"@lumino/coreutils":{"bundled":false,"singleton":true},"@lumino/datagrid":{"bundled":false,"singleton":true},"@lumino/default-theme":{"bundled":false,"singleton":true},"@lumino/domutils":{"bundled":false,"singleton":true},"@lumino/messaging":{"bundled":false,"singleton":true},"@lumino/virtualdom":{"bundled":false,"singleton":true},"@lumino/widgets":{"bundled":false,"singleton":true},"react":false,"react-dom":false}}}')
+            e.exports = JSON.parse('{"name":"buckaroo","version":"0.2.1","description":"Fast Datagrid widget for the Jupyter Notebook and JupyterLab","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","lib/**/*.js.map","lib/**/*.ts","dist/*.js","dist/*.js.map","dist/*.png","style/**/*.*"],"homepage":"https://github.com/paddymul/buckaroo","bugs":{"url":"https://github.com/paddymul/buckaroo/issues"},"license":"BSD-3-Clause","author":{"name":"Paddy Mullen","email":""},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/paddymul/buckaroo"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:dev":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack --mode=production --no-devtool","build:widget-examples":"cd widget-examples/basic && webpack --mode=production","build:all":"yarn run build:labextension && yarn run build:nbextension && yarn run build:widget-examples","clean":"rimraf dist && yarn run clean:lib && yarn run clean:labextension && yarn run clean:nbextension","clean:lib":"rimraf lib","clean:labextension":"rimraf buckaroo/labextension","clean:nbextension":"rimraf buckaroo/nbextension/index.*","lint":"eslint \'js/**/*.{ts,tsx}\'","lint:fix":"eslint \'js/**/*.{ts,tsx}\' --fix","prepack":"yarn run build:labextension && yarn run build:nbextension","test":"jest --verbose","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^2 || ^3 || ^4 || ^6.0.0","@jupyterlab/apputils":"^3.0.2","paddy-react-edit-list":">=1.1.35","lodash":"^4.17.21","react-dom":"^18.0.0","react":"^18.0.0"},"devDependencies":{"@babel/cli":"^7.6.3","@babel/core":"^7.6.3","@babel/preset-env":"^7.6.3","@babel/preset-typescript":"^7.6.0","@jupyterlab/builder":"^3.0.1","@types/jest":"^27.4.1","@types/react":"^18.0.0","@types/react-dom":"^18.0.0","@types/node":"^10.11.6","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.5.0","@typescript-eslint/parser":"^3.5.0","acorn":"^6.2.0","babel-jest":"^28.1.3","babel-plugin-transform-es2015-modules-commonjs":"^6.26.2","css-loader":"^3.0.0","eslint":"^7.3.1","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","jest":"^28.1.3","lint-staged":"^10.2.11","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","rimraf":"^2.6.2","source-map-loader":"^0.2.4","style-loader":"^0.23.1","svg-url-loader":"~3.0.3","ts-jest":"^28.0.8","ts-loader":"^6.0.4","typescript":"~4.2.4","url-loader":"^4.1.0","webpack":"^5","webpack-cli":"^4.4.0"},"jupyterlab":{"extension":"lib/plugin","webpackConfig":"webpack.lab.config.js","outputDir":"./buckaroo/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true},"@lumino/algorithm":{"bundled":false,"singleton":true},"@lumino/commands":{"bundled":false,"singleton":true},"@lumino/coreutils":{"bundled":false,"singleton":true},"@lumino/datagrid":{"bundled":false,"singleton":true},"@lumino/default-theme":{"bundled":false,"singleton":true},"@lumino/domutils":{"bundled":false,"singleton":true},"@lumino/messaging":{"bundled":false,"singleton":true},"@lumino/virtualdom":{"bundled":false,"singleton":true},"@lumino/widgets":{"bundled":false,"singleton":true},"react":false,"react-dom":false}}}')
         }
     }
 ]);
```

### Comparing `buckaroo-0.2.6/dcef/labextension/static/486.5d15e39140ce71ec7db7.js` & `buckaroo-0.2.7/buckaroo/labextension/static/486.f08778dfb765d893ceaf.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,9 +1,9 @@
-/*! For license information please see 486.5d15e39140ce71ec7db7.js.LICENSE.txt */
-(self.webpackChunkdcef = self.webpackChunkdcef || []).push([
+/*! For license information please see 486.f08778dfb765d893ceaf.js.LICENSE.txt */
+(self.webpackChunkbuckaroo = self.webpackChunkbuckaroo || []).push([
     [486], {
         6486: function(n, t, r) {
             var e;
             n = r.nmd(n),
                 function() {
                     var u, i = "Expected a function",
                         o = "__lodash_hash_undefined__",
```

### Comparing `buckaroo-0.2.6/dcef/labextension/static/568.be621402413454ffa400.js` & `buckaroo-0.2.7/buckaroo/labextension/static/568.9a4b0a85049c75a13a73.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-(self.webpackChunkdcef = self.webpackChunkdcef || []).push([
+(self.webpackChunkbuckaroo = self.webpackChunkbuckaroo || []).push([
     [568], {
         8399: function(e, n, t) {
             "use strict";
             var o = this && this.__createBinding || (Object.create ? function(e, n, t, o) {
                     void 0 === o && (o = t), Object.defineProperty(e, o, {
                         enumerable: !0,
                         get: function() {
@@ -27,16 +27,16 @@
                         for (var t in e) "default" !== t && Object.prototype.hasOwnProperty.call(e, t) && o(n, e, t);
                     return i(n, e), n
                 };
             Object.defineProperty(n, "__esModule", {
                 value: !0
             }), n.DCEFWidgetView = n.DCEFWidgetModel = void 0;
             const a = t(2492),
-                s = t(7049),
-                r = l(t(7294)),
+                r = t(7049),
+                s = l(t(7294)),
                 d = l(t(745)),
                 u = t(8657);
             t(9423), t(3054), t(4260), t(801);
             class c extends a.DOMWidgetModel {
                 defaults() {
                     return Object.assign(Object.assign({}, super.defaults()), {
                         _model_name: c.model_name,
@@ -49,58 +49,39 @@
                         operations: [],
                         operation_results: {},
                         dfConfig: {}
                     })
                 }
             }
             n.DCEFWidgetModel = c, c.serializers = Object.assign({}, a.DOMWidgetModel.serializers), c.model_name = "DCEFWidgetModel", c.model_module = u.MODULE_NAME, c.model_module_version = u.MODULE_VERSION, c.view_name = "ExampleView", c.view_module = u.MODULE_NAME, c.view_module_version = u.MODULE_VERSION;
-            class p extends a.DOMWidgetView {
-                constructor() {
-                    super(...arguments), this.setCommandConfig = e => console.log("default setCommandConfig"), this.setPyCode = e => console.log("default setPyCode"), this.setTransformedDf = e => console.log("default setTransformedDf")
-                }
+            class b extends a.DOMWidgetView {
                 render() {
                     this.el.classList.add("custom-widget");
-                    const e = this.model,
-                        n = this;
-                    e.on("change:commandConfig", (() => {
-                        n.setCommandConfig(e.get("commandConfig"))
-                    }), this);
-                    const t = {
-                            getOrRequester: n => (e.on("change:operation_results", (() => {
-                                const t = e.get("operation_results");
-                                console.log("about to call setOpResult with", t), n(t)
-                            }), this), n => {
-                                console.log("orRequester passed operations", n), e.set("operations", n), e.save_changes()
-                            }),
-                            exposeCommandConfigSetter: e => {
-                                n.setCommandConfig = e
-                            }
-                        },
-                        o = document.getElementsByClassName("jp-NotebookPanel-notebook")[0],
-                        i = this.el.getBoundingClientRect().y,
-                        l = o.getBoundingClientRect().y - i + 50;
-                    o.scroll(0, l);
-                    const a = d.createRoot(this.el),
-                        u = r.default.createElement((() => {
-                            const [e, n] = r.useState(0), o = () => {
+                    const e = document.getElementsByClassName("jp-NotebookPanel-notebook")[0],
+                        n = this.el.getBoundingClientRect().y,
+                        t = e.getBoundingClientRect().y - n + 50;
+                    e.scroll(0, t);
+                    const o = d.createRoot(this.el),
+                        i = s.default.createElement((() => {
+                            const [e, n] = s.useState(0), t = () => {
                                 n((e => e + 1))
                             };
-                            r.useEffect((() => {
-                                this.listenTo(this.model, "change", o)
+                            s.useEffect((() => {
+                                this.listenTo(this.model, "change", t)
                             }), []);
-                            const i = Object.assign({}, t);
-                            for (const e of Object.keys(this.model.attributes)) i[e] = this.model.get(e), i["on_" + e] = n => {
+                            const o = {};
+                            for (const e of Object.keys(this.model.attributes)) o[e] = this.model.get(e), o["on_" + e] = n => {
                                 this.model.set(e, n), this.touch()
                             };
-                            return r.default.createElement(s.WidgetDCFCell, i)
+                            return s.default.createElement(r.WidgetDCFCell, o)
                         }), {});
-                    a.render(u)
+                    o.render(i)
                 }
             }
-            n.DCEFWidgetView = p
+            n.DCEFWidgetView = b
         },
         1568: function(e, n, t) {
             "use strict";
             var o = this && this.__createBinding || (Object.create ? function(e, n, t, o) {
                     void 0 === o && (o = t), Object.defineProperty(e, o, {
                         enumerable: !0,
                         get: function() {
@@ -156,11 +137,11 @@
                 hmr: !0,
                 transform: void 0,
                 insertInto: void 0
             }), o.locals && (e.exports = o.locals)
         },
         4147: e => {
             "use strict";
-            e.exports = JSON.parse('{"name":"dcef","version":"0.2.1","description":"Fast Datagrid widget for the Jupyter Notebook and JupyterLab","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","lib/**/*.js.map","lib/**/*.ts","dist/*.js","dist/*.js.map","dist/*.png","style/**/*.*"],"homepage":"https://github.com/paddymul/dcef","bugs":{"url":"https://github.com/paddymul/dcef/issues"},"license":"BSD-3-Clause","author":{"name":"Paddy Mullen","email":""},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/paddymul/dcef"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:dev":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack --mode=production --no-devtool","build:widget-examples":"cd widget-examples/basic && webpack --mode=production","build:all":"yarn run build:labextension && yarn run build:nbextension && yarn run build:widget-examples","clean":"rimraf dist && yarn run clean:lib && yarn run clean:labextension && yarn run clean:nbextension","clean:lib":"rimraf lib","clean:labextension":"rimraf dcef/labextension","clean:nbextension":"rimraf dcef/nbextension/index.*","lint":"eslint \'js/**/*.{ts,tsx}\'","lint:fix":"eslint \'js/**/*.{ts,tsx} --fix\'","prepack":"yarn run build:labextension && yarn run build:nbextension","test":"jest --verbose","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^2 || ^3 || ^4 || ^6.0.0","@jupyterlab/apputils":"^3.0.2","paddy-react-edit-list":">=1.1.35","lodash":"^4.17.21","react-dom":"^18.0.0","react":"^18.0.0"},"devDependencies":{"@babel/cli":"^7.6.3","@babel/core":"^7.6.3","@babel/preset-env":"^7.6.3","@babel/preset-typescript":"^7.6.0","@jupyterlab/builder":"^3.0.1","@types/jest":"^27.4.1","@types/react":"^18.0.0","@types/react-dom":"^18.0.0","@types/node":"^10.11.6","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.5.0","@typescript-eslint/parser":"^3.5.0","acorn":"^6.2.0","babel-jest":"^28.1.3","babel-plugin-transform-es2015-modules-commonjs":"^6.26.2","css-loader":"^3.0.0","eslint":"^7.3.1","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","jest":"^28.1.3","lint-staged":"^10.2.11","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","rimraf":"^2.6.2","source-map-loader":"^0.2.4","style-loader":"^0.23.1","svg-url-loader":"~3.0.3","ts-jest":"^28.0.8","ts-loader":"^6.0.4","typescript":"~4.2.4","url-loader":"^4.1.0","webpack":"^5","webpack-cli":"^4.4.0"},"jupyterlab":{"extension":"lib/plugin","webpackConfig":"webpack.lab.config.js","outputDir":"./dcef/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true},"@lumino/algorithm":{"bundled":false,"singleton":true},"@lumino/commands":{"bundled":false,"singleton":true},"@lumino/coreutils":{"bundled":false,"singleton":true},"@lumino/datagrid":{"bundled":false,"singleton":true},"@lumino/default-theme":{"bundled":false,"singleton":true},"@lumino/domutils":{"bundled":false,"singleton":true},"@lumino/messaging":{"bundled":false,"singleton":true},"@lumino/virtualdom":{"bundled":false,"singleton":true},"@lumino/widgets":{"bundled":false,"singleton":true},"react":false,"react-dom":false}}}')
+            e.exports = JSON.parse('{"name":"buckaroo","version":"0.2.1","description":"Fast Datagrid widget for the Jupyter Notebook and JupyterLab","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","lib/**/*.js.map","lib/**/*.ts","dist/*.js","dist/*.js.map","dist/*.png","style/**/*.*"],"homepage":"https://github.com/paddymul/buckaroo","bugs":{"url":"https://github.com/paddymul/buckaroo/issues"},"license":"BSD-3-Clause","author":{"name":"Paddy Mullen","email":""},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/paddymul/buckaroo"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:dev":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack --mode=production --no-devtool","build:widget-examples":"cd widget-examples/basic && webpack --mode=production","build:all":"yarn run build:labextension && yarn run build:nbextension && yarn run build:widget-examples","clean":"rimraf dist && yarn run clean:lib && yarn run clean:labextension && yarn run clean:nbextension","clean:lib":"rimraf lib","clean:labextension":"rimraf buckaroo/labextension","clean:nbextension":"rimraf buckaroo/nbextension/index.*","lint":"eslint \'js/**/*.{ts,tsx}\'","lint:fix":"eslint \'js/**/*.{ts,tsx}\' --fix","prepack":"yarn run build:labextension && yarn run build:nbextension","test":"jest --verbose","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^2 || ^3 || ^4 || ^6.0.0","@jupyterlab/apputils":"^3.0.2","paddy-react-edit-list":">=1.1.35","lodash":"^4.17.21","react-dom":"^18.0.0","react":"^18.0.0"},"devDependencies":{"@babel/cli":"^7.6.3","@babel/core":"^7.6.3","@babel/preset-env":"^7.6.3","@babel/preset-typescript":"^7.6.0","@jupyterlab/builder":"^3.0.1","@types/jest":"^27.4.1","@types/react":"^18.0.0","@types/react-dom":"^18.0.0","@types/node":"^10.11.6","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.5.0","@typescript-eslint/parser":"^3.5.0","acorn":"^6.2.0","babel-jest":"^28.1.3","babel-plugin-transform-es2015-modules-commonjs":"^6.26.2","css-loader":"^3.0.0","eslint":"^7.3.1","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","jest":"^28.1.3","lint-staged":"^10.2.11","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","rimraf":"^2.6.2","source-map-loader":"^0.2.4","style-loader":"^0.23.1","svg-url-loader":"~3.0.3","ts-jest":"^28.0.8","ts-loader":"^6.0.4","typescript":"~4.2.4","url-loader":"^4.1.0","webpack":"^5","webpack-cli":"^4.4.0"},"jupyterlab":{"extension":"lib/plugin","webpackConfig":"webpack.lab.config.js","outputDir":"./buckaroo/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true},"@lumino/algorithm":{"bundled":false,"singleton":true},"@lumino/commands":{"bundled":false,"singleton":true},"@lumino/coreutils":{"bundled":false,"singleton":true},"@lumino/datagrid":{"bundled":false,"singleton":true},"@lumino/default-theme":{"bundled":false,"singleton":true},"@lumino/domutils":{"bundled":false,"singleton":true},"@lumino/messaging":{"bundled":false,"singleton":true},"@lumino/virtualdom":{"bundled":false,"singleton":true},"@lumino/widgets":{"bundled":false,"singleton":true},"react":false,"react-dom":false}}}')
         }
     }
 ]);
```

### Comparing `buckaroo-0.2.6/dcef/labextension/static/remoteEntry.b7da48392a5008410871.js` & `buckaroo-0.2.7/buckaroo/labextension/static/remoteEntry.d4606edd7ebd1ec0dcc6.js`

 * *Files 20% similar despite different names*

#### js-beautify {}

```diff
@@ -1,296 +1,296 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, a, i, l, d, f, u, s, c, p, h, v, b, m, g, y = {
-            7987: (e, r, t) => {
-                var n = {
+    var e, r, t, a, o, n, i, l, u, d, f, s, c, p, h, b, v, m, g, y = {
+            5941: (e, r, t) => {
+                var a = {
                         "./index": () => Promise.all([t.e(250), t.e(968), t.e(568)]).then((() => () => t(1568))),
                         "./extension": () => Promise.all([t.e(250), t.e(968), t.e(480)]).then((() => () => t(4480)))
                     },
-                    o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
+                    o = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
-                    a = (e, r) => {
+                    n = (e, r) => {
                         if (t.S) {
-                            var n = "default",
-                                o = t.S[n];
+                            var a = "default",
+                                o = t.S[a];
                             if (o && o !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
-                            return t.S[n] = e, t.I(n, r)
+                            return t.S[a] = e, t.I(a, r)
                         }
                     };
                 t.d(r, {
                     get: () => o,
-                    init: () => a
+                    init: () => n
                 })
             }
         },
         w = {};
 
-    function S(e) {
+    function k(e) {
         var r = w[e];
         if (void 0 !== r) return r.exports;
         var t = w[e] = {
             id: e,
             loaded: !1,
             exports: {}
         };
-        return y[e].call(t.exports, t, t.exports, S), t.loaded = !0, t.exports
+        return y[e].call(t.exports, t, t.exports, k), t.loaded = !0, t.exports
     }
-    S.m = y, S.c = w, S.d = (e, r) => {
-        for (var t in r) S.o(r, t) && !S.o(e, t) && Object.defineProperty(e, t, {
+    k.m = y, k.c = w, k.d = (e, r) => {
+        for (var t in r) k.o(r, t) && !k.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
-    }, S.f = {}, S.e = e => Promise.all(Object.keys(S.f).reduce(((r, t) => (S.f[t](e, r), r)), [])), S.u = e => e + "." + {
-        116: "3a7574d1f75164e010bc",
-        250: "c608416dcff072a71036",
-        439: "a9341020e0030adbdf79",
-        480: "55b0b32536a517ae86fb",
-        486: "5d15e39140ce71ec7db7",
-        568: "be621402413454ffa400",
-        968: "27473ef42c3b398118fa"
+    }, k.f = {}, k.e = e => Promise.all(Object.keys(k.f).reduce(((r, t) => (k.f[t](e, r), r)), [])), k.u = e => e + "." + {
+        116: "b6e5adfccd7c520a720a",
+        250: "b55e2550464d9477eb95",
+        439: "4adf3a2c49f42aafd8ca",
+        480: "e809fc8a18bc53e804a1",
+        486: "f08778dfb765d893ceaf",
+        568: "9a4b0a85049c75a13a73",
+        968: "36cdefd1b8be6c13ff71"
     } [e] + ".js?v=" + {
-        116: "3a7574d1f75164e010bc",
-        250: "c608416dcff072a71036",
-        439: "a9341020e0030adbdf79",
-        480: "55b0b32536a517ae86fb",
-        486: "5d15e39140ce71ec7db7",
-        568: "be621402413454ffa400",
-        968: "27473ef42c3b398118fa"
-    } [e], S.g = function() {
+        116: "b6e5adfccd7c520a720a",
+        250: "b55e2550464d9477eb95",
+        439: "4adf3a2c49f42aafd8ca",
+        480: "e809fc8a18bc53e804a1",
+        486: "f08778dfb765d893ceaf",
+        568: "9a4b0a85049c75a13a73",
+        968: "36cdefd1b8be6c13ff71"
+    } [e], k.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), S.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "dcef:", S.l = (t, n, o, a) => {
-        if (e[t]) e[t].push(n);
+    }(), k.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "buckaroo:", k.l = (t, a, o, n) => {
+        if (e[t]) e[t].push(a);
         else {
             var i, l;
             if (void 0 !== o)
-                for (var d = document.getElementsByTagName("script"), f = 0; f < d.length; f++) {
-                    var u = d[f];
-                    if (u.getAttribute("src") == t || u.getAttribute("data-webpack") == r + o) {
-                        i = u;
+                for (var u = document.getElementsByTagName("script"), d = 0; d < u.length; d++) {
+                    var f = u[d];
+                    if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + o) {
+                        i = f;
                         break
                     }
                 }
-            i || (l = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, S.nc && i.setAttribute("nonce", S.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
-            var s = (r, n) => {
+            i || (l = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, k.nc && i.setAttribute("nonce", k.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [a];
+            var s = (r, a) => {
                     i.onerror = i.onload = null, clearTimeout(c);
                     var o = e[t];
-                    if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(n))), r) return r(n)
+                    if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(a))), r) return r(a)
                 },
                 c = setTimeout(s.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
             i.onerror = s.bind(null, i.onerror), i.onload = s.bind(null, i.onload), l && document.head.appendChild(i)
         }
-    }, S.r = e => {
+    }, k.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
-    }, S.nmd = e => (e.paths = [], e.children || (e.children = []), e), (() => {
-        S.S = {};
+    }, k.nmd = e => (e.paths = [], e.children || (e.children = []), e), (() => {
+        k.S = {};
         var e = {},
             r = {};
-        S.I = (t, n) => {
-            n || (n = []);
+        k.I = (t, a) => {
+            a || (a = []);
             var o = r[t];
-            if (o || (o = r[t] = {}), !(n.indexOf(o) >= 0)) {
-                if (n.push(o), e[t]) return e[t];
-                S.o(S.S, t) || (S.S[t] = {});
-                var a = S.S[t],
-                    i = "dcef",
-                    l = (e, r, t, n) => {
-                        var o = a[e] = a[e] || {},
+            if (o || (o = r[t] = {}), !(a.indexOf(o) >= 0)) {
+                if (a.push(o), e[t]) return e[t];
+                k.o(k.S, t) || (k.S[t] = {});
+                var n = k.S[t],
+                    i = "buckaroo",
+                    l = (e, r, t, a) => {
+                        var o = n[e] = n[e] || {},
                             l = o[r];
-                        (!l || !l.loaded && (!n != !l.eager ? n : i > l.from)) && (o[r] = {
+                        (!l || !l.loaded && (!a != !l.eager ? a : i > l.from)) && (o[r] = {
                             get: t,
                             from: i,
-                            eager: !!n
+                            eager: !!a
                         })
                     },
-                    d = [];
-                return "default" === t && (l("dcef", "0.2.1", (() => Promise.all([S.e(250), S.e(968), S.e(568)]).then((() => () => S(1568))))), l("lodash", "4.17.21", (() => S.e(486).then((() => () => S(6486))))), l("paddy-react-edit-list", "1.1.35", (() => Promise.all([S.e(250), S.e(116), S.e(439)]).then((() => () => S(7116)))))), e[t] = d.length ? Promise.all(d).then((() => e[t] = 1)) : 1
+                    u = [];
+                return "default" === t && (l("buckaroo", "0.2.1", (() => Promise.all([k.e(250), k.e(968), k.e(568)]).then((() => () => k(1568))))), l("lodash", "4.17.21", (() => k.e(486).then((() => () => k(6486))))), l("paddy-react-edit-list", "1.1.35", (() => Promise.all([k.e(250), k.e(116), k.e(439)]).then((() => () => k(7116)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
-        S.g.importScripts && (e = S.g.location + "");
-        var r = S.g.document;
+        k.g.importScripts && (e = k.g.location + "");
+        var r = k.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
             var t = r.getElementsByTagName("script");
             if (t.length)
-                for (var n = t.length - 1; n > -1 && !e;) e = t[n--].src
+                for (var a = t.length - 1; a > -1 && !e;) e = t[a--].src
         }
         if (!e) throw new Error("Automatic publicPath is not supported in this browser");
-        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), S.p = e
+        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), k.p = e
     })(), t = e => {
         var r = e => e.split(".").map((e => +e == e ? +e : e)),
             t = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
-            n = t[1] ? r(t[1]) : [];
-        return t[2] && (n.length++, n.push.apply(n, r(t[2]))), t[3] && (n.push([]), n.push.apply(n, r(t[3]))), n
-    }, n = (e, r) => {
+            a = t[1] ? r(t[1]) : [];
+        return t[2] && (a.length++, a.push.apply(a, r(t[2]))), t[3] && (a.push([]), a.push.apply(a, r(t[3]))), a
+    }, a = (e, r) => {
         e = t(e), r = t(r);
-        for (var n = 0;;) {
-            if (n >= e.length) return n < r.length && "u" != (typeof r[n])[0];
-            var o = e[n],
-                a = (typeof o)[0];
-            if (n >= r.length) return "u" == a;
-            var i = r[n],
+        for (var a = 0;;) {
+            if (a >= e.length) return a < r.length && "u" != (typeof r[a])[0];
+            var o = e[a],
+                n = (typeof o)[0];
+            if (a >= r.length) return "u" == n;
+            var i = r[a],
                 l = (typeof i)[0];
-            if (a != l) return "o" == a && "n" == l || "s" == l || "u" == a;
-            if ("o" != a && "u" != a && o != i) return o < i;
-            n++
+            if (n != l) return "o" == n && "n" == l || "s" == l || "u" == n;
+            if ("o" != n && "u" != n && o != i) return o < i;
+            a++
         }
     }, o = e => {
         var r = e[0],
             t = "";
         if (1 === e.length) return "*";
         if (r + .5) {
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
-            for (var n = 1, a = 1; a < e.length; a++) n--, t += "u" == (typeof(l = e[a]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, l);
+            for (var a = 1, n = 1; n < e.length; n++) a--, t += "u" == (typeof(l = e[n]))[0] ? "-" : (a > 0 ? "." : "") + (a = 2, l);
             return t
         }
         var i = [];
-        for (a = 1; a < e.length; a++) {
-            var l = e[a];
-            i.push(0 === l ? "not(" + d() + ")" : 1 === l ? "(" + d() + " || " + d() + ")" : 2 === l ? i.pop() + " " + i.pop() : o(l))
+        for (n = 1; n < e.length; n++) {
+            var l = e[n];
+            i.push(0 === l ? "not(" + u() + ")" : 1 === l ? "(" + u() + " || " + u() + ")" : 2 === l ? i.pop() + " " + i.pop() : o(l))
         }
-        return d();
+        return u();
 
-        function d() {
+        function u() {
             return i.pop().replace(/^\((.+)\)$/, "$1")
         }
-    }, a = (e, r) => {
+    }, n = (e, r) => {
         if (0 in e) {
             r = t(r);
-            var n = e[0],
-                o = n < 0;
-            o && (n = -n - 1);
-            for (var i = 0, l = 1, d = !0;; l++, i++) {
-                var f, u, s = l < e.length ? (typeof e[l])[0] : "";
-                if (i >= r.length || "o" == (u = (typeof(f = r[i]))[0])) return !d || ("u" == s ? l > n && !o : "" == s != o);
-                if ("u" == u) {
-                    if (!d || "u" != s) return !1
-                } else if (d)
-                    if (s == u)
-                        if (l <= n) {
-                            if (f != e[l]) return !1
+            var a = e[0],
+                o = a < 0;
+            o && (a = -a - 1);
+            for (var i = 0, l = 1, u = !0;; l++, i++) {
+                var d, f, s = l < e.length ? (typeof e[l])[0] : "";
+                if (i >= r.length || "o" == (f = (typeof(d = r[i]))[0])) return !u || ("u" == s ? l > a && !o : "" == s != o);
+                if ("u" == f) {
+                    if (!u || "u" != s) return !1
+                } else if (u)
+                    if (s == f)
+                        if (l <= a) {
+                            if (d != e[l]) return !1
                         } else {
-                            if (o ? f > e[l] : f < e[l]) return !1;
-                            f != e[l] && (d = !1)
+                            if (o ? d > e[l] : d < e[l]) return !1;
+                            d != e[l] && (u = !1)
                         }
                 else if ("s" != s && "n" != s) {
-                    if (o || l <= n) return !1;
-                    d = !1, l--
+                    if (o || l <= a) return !1;
+                    u = !1, l--
                 } else {
-                    if (l <= n || u < s != o) return !1;
-                    d = !1
-                } else "s" != s && "n" != s && (d = !1, l--)
+                    if (l <= a || f < s != o) return !1;
+                    u = !1
+                } else "s" != s && "n" != s && (u = !1, l--)
             }
         }
         var c = [],
             p = c.pop.bind(c);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
-            c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? a(h, r) : !p())
+            c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? n(h, r) : !p())
         }
         return !!p()
     }, i = (e, r) => {
-        var t = S.S[e];
-        if (!t || !S.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
+        var t = k.S[e];
+        if (!t || !k.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, l = (e, r) => {
         var t = e[r];
-        return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, d = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", f = (e, r, t, n) => {
+        return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && a(e, r) ? r : e), 0)
+    }, u = (e, r, t, a) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(a) + ")", d = (e, r, t, a) => {
         var o = l(e, t);
-        return a(n, o) || s(d(e, t, o, n)), c(e[t][o])
-    }, u = (e, r, t) => {
+        return n(a, o) || s(u(e, t, o, a)), c(e[t][o])
+    }, f = (e, r, t) => {
         var o = e[r];
-        return (r = Object.keys(o).reduce(((e, r) => !a(t, r) || e && !n(e, r) ? e : r), 0)) && o[r]
+        return (r = Object.keys(o).reduce(((e, r) => !n(t, r) || e && !a(e, r) ? e : r), 0)) && o[r]
     }, s = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
-    }, c = e => (e.loaded = 1, e.get()), h = (p = e => function(r, t, n, o) {
-        var a = S.I(r);
-        return a && a.then ? a.then(e.bind(e, r, S.S[r], t, n, o)) : e(r, S.S[r], t, n, o)
-    })(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), v = p(((e, r, t, n, o) => {
-        var a = r && S.o(r, t) && u(r, t, n);
-        return a ? c(a) : o()
-    })), b = {}, m = {
+    }, c = e => (e.loaded = 1, e.get()), h = (p = e => function(r, t, a, o) {
+        var n = k.I(r);
+        return n && n.then ? n.then(e.bind(e, r, k.S[r], t, a, o)) : e(r, k.S[r], t, a, o)
+    })(((e, r, t, a) => (i(e, t), d(r, 0, t, a)))), b = p(((e, r, t, a, o) => {
+        var n = r && k.o(r, t) && f(r, t, a);
+        return n ? c(n) : o()
+    })), v = {}, m = {
         2492: () => h("default", "@jupyter-widgets/base", [, [1, 6, 0, 0],
             [1, 4],
             [1, 3],
             [1, 2], 1, 1, 1
         ]),
-        7049: () => v("default", "paddy-react-edit-list", [0, 1, 1, 35], (() => Promise.all([S.e(116), S.e(439)]).then((() => () => S(7116))))),
+        7049: () => b("default", "paddy-react-edit-list", [0, 1, 1, 35], (() => Promise.all([k.e(116), k.e(439)]).then((() => () => k(7116))))),
         3033: () => h("default", "@jupyterlab/apputils", [1, 3, 6, 3]),
-        4439: () => v("default", "lodash", [1, 4, 17, 21], (() => S.e(486).then((() => () => S(6486)))))
+        4439: () => b("default", "lodash", [1, 4, 17, 21], (() => k.e(486).then((() => () => k(6486)))))
     }, g = {
         439: [4439],
         480: [3033],
         968: [2492, 7049]
-    }, S.f.consumes = (e, r) => {
-        S.o(g, e) && g[e].forEach((e => {
-            if (S.o(b, e)) return r.push(b[e]);
+    }, k.f.consumes = (e, r) => {
+        k.o(g, e) && g[e].forEach((e => {
+            if (k.o(v, e)) return r.push(v[e]);
             var t = r => {
-                    b[e] = 0, S.m[e] = t => {
-                        delete S.c[e], t.exports = r()
+                    v[e] = 0, k.m[e] = t => {
+                        delete k.c[e], t.exports = r()
                     }
                 },
-                n = r => {
-                    delete b[e], S.m[e] = t => {
-                        throw delete S.c[e], r
+                a = r => {
+                    delete v[e], k.m[e] = t => {
+                        throw delete k.c[e], r
                     }
                 };
             try {
                 var o = m[e]();
-                o.then ? r.push(b[e] = o.then(t).catch(n)) : t(o)
+                o.then ? r.push(v[e] = o.then(t).catch(a)) : t(o)
             } catch (e) {
-                n(e)
+                a(e)
             }
         }))
     }, (() => {
         var e = {
-            49: 0
+            548: 0
         };
-        S.f.j = (r, t) => {
-            var n = S.o(e, r) ? e[r] : void 0;
-            if (0 !== n)
-                if (n) t.push(n[2]);
+        k.f.j = (r, t) => {
+            var a = k.o(e, r) ? e[r] : void 0;
+            if (0 !== a)
+                if (a) t.push(a[2]);
                 else if (/^(439|968)$/.test(r)) e[r] = 0;
             else {
-                var o = new Promise(((t, o) => n = e[r] = [t, o]));
-                t.push(n[2] = o);
-                var a = S.p + S.u(r),
+                var o = new Promise(((t, o) => a = e[r] = [t, o]));
+                t.push(a[2] = o);
+                var n = k.p + k.u(r),
                     i = new Error;
-                S.l(a, (t => {
-                    if (S.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
+                k.l(n, (t => {
+                    if (k.o(e, r) && (0 !== (a = e[r]) && (e[r] = void 0), a)) {
                         var o = t && ("load" === t.type ? "missing" : t.type),
-                            a = t && t.target && t.target.src;
-                        i.message = "Loading chunk " + r + " failed.\n(" + o + ": " + a + ")", i.name = "ChunkLoadError", i.type = o, i.request = a, n[1](i)
+                            n = t && t.target && t.target.src;
+                        i.message = "Loading chunk " + r + " failed.\n(" + o + ": " + n + ")", i.name = "ChunkLoadError", i.type = o, i.request = n, a[1](i)
                     }
                 }), "chunk-" + r, r)
             }
         };
         var r = (r, t) => {
-                var n, o, [a, i, l] = t,
-                    d = 0;
-                if (a.some((r => 0 !== e[r]))) {
-                    for (n in i) S.o(i, n) && (S.m[n] = i[n]);
-                    l && l(S)
+                var a, o, [n, i, l] = t,
+                    u = 0;
+                if (n.some((r => 0 !== e[r]))) {
+                    for (a in i) k.o(i, a) && (k.m[a] = i[a]);
+                    l && l(k)
                 }
-                for (r && r(t); d < a.length; d++) o = a[d], S.o(e, o) && e[o] && e[o][0](), e[o] = 0
+                for (r && r(t); u < n.length; u++) o = n[u], k.o(e, o) && e[o] && e[o][0](), e[o] = 0
             },
-            t = self.webpackChunkdcef = self.webpackChunkdcef || [];
+            t = self.webpackChunkbuckaroo = self.webpackChunkbuckaroo || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
-    })(), S.nc = void 0;
-    var P = S(7987);
-    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB).dcef = P
+    })(), k.nc = void 0;
+    var S = k(5941);
+    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB).buckaroo = S
 })();
```

### Comparing `buckaroo-0.2.6/dcef/labextension/static/third-party-licenses.json` & `buckaroo-0.2.7/buckaroo/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `buckaroo-0.2.6/dcef/nbextension/index.js` & `buckaroo-0.2.7/buckaroo/nbextension/index.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -48529,54 +48529,35 @@
                             operation_results: {},
                             dfConfig: {}
                         })
                     }
                 }
                 t.DCEFWidgetModel = p, p.serializers = Object.assign({}, a.DOMWidgetModel.serializers), p.model_name = "DCEFWidgetModel", p.model_module = c.MODULE_NAME, p.model_module_version = c.MODULE_VERSION, p.view_name = "ExampleView", p.view_module = c.MODULE_NAME, p.view_module_version = c.MODULE_VERSION;
                 class d extends a.DOMWidgetView {
-                    constructor() {
-                        super(...arguments), this.setCommandConfig = e => console.log("default setCommandConfig"), this.setPyCode = e => console.log("default setPyCode"), this.setTransformedDf = e => console.log("default setTransformedDf")
-                    }
                     render() {
                         this.el.classList.add("custom-widget");
-                        const e = this.model,
-                            t = this;
-                        e.on("change:commandConfig", (() => {
-                            t.setCommandConfig(e.get("commandConfig"))
-                        }), this);
-                        const n = {
-                                getOrRequester: t => (e.on("change:operation_results", (() => {
-                                    const n = e.get("operation_results");
-                                    console.log("about to call setOpResult with", n), t(n)
-                                }), this), t => {
-                                    console.log("orRequester passed operations", t), e.set("operations", t), e.save_changes()
-                                }),
-                                exposeCommandConfigSetter: e => {
-                                    t.setCommandConfig = e
-                                }
-                            },
-                            r = document.getElementsByClassName("jp-NotebookPanel-notebook")[0],
-                            o = this.el.getBoundingClientRect().y,
-                            i = r.getBoundingClientRect().y - o + 50;
-                        r.scroll(0, i);
-                        const a = u.createRoot(this.el),
-                            c = l.default.createElement((() => {
-                                const [e, t] = l.useState(0), r = () => {
+                        const e = document.getElementsByClassName("jp-NotebookPanel-notebook")[0],
+                            t = this.el.getBoundingClientRect().y,
+                            n = e.getBoundingClientRect().y - t + 50;
+                        e.scroll(0, n);
+                        const r = u.createRoot(this.el),
+                            o = l.default.createElement((() => {
+                                const [e, t] = l.useState(0), n = () => {
                                     t((e => e + 1))
                                 };
                                 l.useEffect((() => {
-                                    this.listenTo(this.model, "change", r)
+                                    this.listenTo(this.model, "change", n)
                                 }), []);
-                                const o = Object.assign({}, n);
-                                for (const e of Object.keys(this.model.attributes)) o[e] = this.model.get(e), o["on_" + e] = t => {
+                                const r = {};
+                                for (const e of Object.keys(this.model.attributes)) r[e] = this.model.get(e), r["on_" + e] = t => {
                                     this.model.set(e, t), this.touch()
                                 };
-                                return l.default.createElement(s.WidgetDCFCell, o)
+                                return l.default.createElement(s.WidgetDCFCell, r)
                             }), {});
-                        a.render(c)
+                        r.render(o)
                     }
                 }
                 t.DCEFWidgetView = d
             },
             5268: function(e, t, n) {
                 "use strict";
                 var r = this && this.__createBinding || (Object.create ? function(e, t, n, r) {
@@ -48625,15 +48606,15 @@
             },
             9146: t => {
                 "use strict";
                 t.exports = e
             },
             4147: e => {
                 "use strict";
-                e.exports = JSON.parse('{"name":"dcef","version":"0.2.1","description":"Fast Datagrid widget for the Jupyter Notebook and JupyterLab","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","lib/**/*.js.map","lib/**/*.ts","dist/*.js","dist/*.js.map","dist/*.png","style/**/*.*"],"homepage":"https://github.com/paddymul/dcef","bugs":{"url":"https://github.com/paddymul/dcef/issues"},"license":"BSD-3-Clause","author":{"name":"Paddy Mullen","email":""},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/paddymul/dcef"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:dev":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack --mode=production --no-devtool","build:widget-examples":"cd widget-examples/basic && webpack --mode=production","build:all":"yarn run build:labextension && yarn run build:nbextension && yarn run build:widget-examples","clean":"rimraf dist && yarn run clean:lib && yarn run clean:labextension && yarn run clean:nbextension","clean:lib":"rimraf lib","clean:labextension":"rimraf dcef/labextension","clean:nbextension":"rimraf dcef/nbextension/index.*","lint":"eslint \'js/**/*.{ts,tsx}\'","lint:fix":"eslint \'js/**/*.{ts,tsx} --fix\'","prepack":"yarn run build:labextension && yarn run build:nbextension","test":"jest --verbose","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^2 || ^3 || ^4 || ^6.0.0","@jupyterlab/apputils":"^3.0.2","paddy-react-edit-list":">=1.1.35","lodash":"^4.17.21","react-dom":"^18.0.0","react":"^18.0.0"},"devDependencies":{"@babel/cli":"^7.6.3","@babel/core":"^7.6.3","@babel/preset-env":"^7.6.3","@babel/preset-typescript":"^7.6.0","@jupyterlab/builder":"^3.0.1","@types/jest":"^27.4.1","@types/react":"^18.0.0","@types/react-dom":"^18.0.0","@types/node":"^10.11.6","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.5.0","@typescript-eslint/parser":"^3.5.0","acorn":"^6.2.0","babel-jest":"^28.1.3","babel-plugin-transform-es2015-modules-commonjs":"^6.26.2","css-loader":"^3.0.0","eslint":"^7.3.1","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","jest":"^28.1.3","lint-staged":"^10.2.11","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","rimraf":"^2.6.2","source-map-loader":"^0.2.4","style-loader":"^0.23.1","svg-url-loader":"~3.0.3","ts-jest":"^28.0.8","ts-loader":"^6.0.4","typescript":"~4.2.4","url-loader":"^4.1.0","webpack":"^5","webpack-cli":"^4.4.0"},"jupyterlab":{"extension":"lib/plugin","webpackConfig":"webpack.lab.config.js","outputDir":"./dcef/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true},"@lumino/algorithm":{"bundled":false,"singleton":true},"@lumino/commands":{"bundled":false,"singleton":true},"@lumino/coreutils":{"bundled":false,"singleton":true},"@lumino/datagrid":{"bundled":false,"singleton":true},"@lumino/default-theme":{"bundled":false,"singleton":true},"@lumino/domutils":{"bundled":false,"singleton":true},"@lumino/messaging":{"bundled":false,"singleton":true},"@lumino/virtualdom":{"bundled":false,"singleton":true},"@lumino/widgets":{"bundled":false,"singleton":true},"react":false,"react-dom":false}}}')
+                e.exports = JSON.parse('{"name":"buckaroo","version":"0.2.1","description":"Fast Datagrid widget for the Jupyter Notebook and JupyterLab","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","lib/**/*.js.map","lib/**/*.ts","dist/*.js","dist/*.js.map","dist/*.png","style/**/*.*"],"homepage":"https://github.com/paddymul/buckaroo","bugs":{"url":"https://github.com/paddymul/buckaroo/issues"},"license":"BSD-3-Clause","author":{"name":"Paddy Mullen","email":""},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/paddymul/buckaroo"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:dev":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack --mode=production --no-devtool","build:widget-examples":"cd widget-examples/basic && webpack --mode=production","build:all":"yarn run build:labextension && yarn run build:nbextension && yarn run build:widget-examples","clean":"rimraf dist && yarn run clean:lib && yarn run clean:labextension && yarn run clean:nbextension","clean:lib":"rimraf lib","clean:labextension":"rimraf buckaroo/labextension","clean:nbextension":"rimraf buckaroo/nbextension/index.*","lint":"eslint \'js/**/*.{ts,tsx}\'","lint:fix":"eslint \'js/**/*.{ts,tsx}\' --fix","prepack":"yarn run build:labextension && yarn run build:nbextension","test":"jest --verbose","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^2 || ^3 || ^4 || ^6.0.0","@jupyterlab/apputils":"^3.0.2","paddy-react-edit-list":">=1.1.35","lodash":"^4.17.21","react-dom":"^18.0.0","react":"^18.0.0"},"devDependencies":{"@babel/cli":"^7.6.3","@babel/core":"^7.6.3","@babel/preset-env":"^7.6.3","@babel/preset-typescript":"^7.6.0","@jupyterlab/builder":"^3.0.1","@types/jest":"^27.4.1","@types/react":"^18.0.0","@types/react-dom":"^18.0.0","@types/node":"^10.11.6","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.5.0","@typescript-eslint/parser":"^3.5.0","acorn":"^6.2.0","babel-jest":"^28.1.3","babel-plugin-transform-es2015-modules-commonjs":"^6.26.2","css-loader":"^3.0.0","eslint":"^7.3.1","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","jest":"^28.1.3","lint-staged":"^10.2.11","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","rimraf":"^2.6.2","source-map-loader":"^0.2.4","style-loader":"^0.23.1","svg-url-loader":"~3.0.3","ts-jest":"^28.0.8","ts-loader":"^6.0.4","typescript":"~4.2.4","url-loader":"^4.1.0","webpack":"^5","webpack-cli":"^4.4.0"},"jupyterlab":{"extension":"lib/plugin","webpackConfig":"webpack.lab.config.js","outputDir":"./buckaroo/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true},"@lumino/algorithm":{"bundled":false,"singleton":true},"@lumino/commands":{"bundled":false,"singleton":true},"@lumino/coreutils":{"bundled":false,"singleton":true},"@lumino/datagrid":{"bundled":false,"singleton":true},"@lumino/default-theme":{"bundled":false,"singleton":true},"@lumino/domutils":{"bundled":false,"singleton":true},"@lumino/messaging":{"bundled":false,"singleton":true},"@lumino/virtualdom":{"bundled":false,"singleton":true},"@lumino/widgets":{"bundled":false,"singleton":true},"react":false,"react-dom":false}}}')
             }
         },
         n = {};
 
     function r(e) {
         var o = n[e];
         if (void 0 !== o) return o.exports;
```

### Comparing `buckaroo-0.2.6/dcef/nbextension/index.js.LICENSE.txt` & `buckaroo-0.2.7/buckaroo/nbextension/index.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `buckaroo-0.2.6/dcef/noarch/index.html` & `buckaroo-0.2.7/buckaroo/noarch/index.html`

 * *Files identical despite different names*

### Comparing `buckaroo-0.2.6/docs/Makefile` & `buckaroo-0.2.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `buckaroo-0.2.6/docs/make.bat` & `buckaroo-0.2.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `buckaroo-0.2.6/docs/source/FAQ.rst` & `buckaroo-0.2.7/docs/source/FAQ.rst`

 * *Files identical despite different names*

### Comparing `buckaroo-0.2.6/docs/source/conf.py` & `buckaroo-0.2.7/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.2.6/docs/source/contributing.rst` & `buckaroo-0.2.7/docs/source/contributing.rst`

 * *Files identical despite different names*

### Comparing `buckaroo-0.2.6/docs/source/index.rst` & `buckaroo-0.2.7/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `buckaroo-0.2.6/docs/source/using.rst` & `buckaroo-0.2.7/docs/source/using.rst`

 * *Files identical despite different names*

### Comparing `buckaroo-0.2.6/docs/source/_static/embed-bundle.js.LICENSE.txt` & `buckaroo-0.2.7/docs/source/_static/embed-bundle.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `buckaroo-0.2.6/js/extension.ts` & `buckaroo-0.2.7/js/extension.ts`

 * *Files identical despite different names*

### Comparing `buckaroo-0.2.6/js/plugin.ts` & `buckaroo-0.2.7/js/plugin.ts`

 * *Files 17% similar despite different names*

```diff
@@ -5,19 +5,18 @@
 
 import { Widget } from '@lumino/widgets';
 
 import { IJupyterWidgetRegistry } from '@jupyter-widgets/base';
 
 import { IThemeManager } from '@jupyterlab/apputils';
 
-
 import { MODULE_NAME, MODULE_VERSION } from './version';
 import * as dcefwidget from './dcefwidget';
 
-const EXTENSION_ID = 'dcef:plugin';
+const EXTENSION_ID = 'buckaroo:plugin';
 
 /**
  * The datagrid plugin.
  */
 const datagridPlugin: IPlugin<Application<Widget>, void> = {
   id: EXTENSION_ID,
   requires: [IJupyterWidgetRegistry],
@@ -31,19 +30,19 @@
 
 /**
  * Activate the widget extension.
  */
 function activateWidgetExtension(
   app: Application<Widget>,
   registry: IJupyterWidgetRegistry,
-  themeManager: IThemeManager | null,
+  themeManager: IThemeManager | null
 ): void {
-    console.log("dcef_widget plugin.ts after change EXTENSION_ID")
+  console.log('buckaroo_widget plugin.ts after change EXTENSION_ID');
   // Exporting a patched DataGridView widget which handles dynamic theme changes
   registry.registerWidget({
     name: MODULE_NAME,
     version: MODULE_VERSION,
     exports: {
-	...dcefwidget
+      ...dcefwidget,
     },
   });
 }
```

### Comparing `buckaroo-0.2.6/static/images/dcf-jupyter.png` & `buckaroo-0.2.7/static/images/dcf-jupyter.png`

 * *Files identical despite different names*

### Comparing `buckaroo-0.2.6/.gitignore` & `buckaroo-0.2.7/.gitignore`

 * *Files identical despite different names*

### Comparing `buckaroo-0.2.6/LICENSE.txt` & `buckaroo-0.2.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `buckaroo-0.2.6/README.md` & `buckaroo-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `buckaroo-0.2.6/pyproject.toml` & `buckaroo-0.2.7/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -30,40 +30,40 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 dependencies = [
     "ipywidgets>=7.6.0,<9"
 ]
-version = "0.2.6"
+version = "0.2.7"
 
 [project.license]
 file = "LICENSE.txt"
 
 [project.optional-dependencies]
 test = [
     "nbval>=0.9",
     "pandas<=1.3.5",
     "pytest-cov>=3",
     "pytest>=6",
 ]
 
 [project.urls]
-Homepage = "https://github.com/bloomberg/dcef"
+Homepage = "https://github.com/paddymul/buckaroo"
 
 [tool.hatch.build]
 artifacts = [
-    "dcef/nbextension/index.*",
-    "dcef/labextension",
+    "buckaroo/nbextension/index.*",
+    "buckaroo/labextension",
 ]
 
 [tool.hatch.build.targets.wheel.shared-data]
-"dcef/nbextension" = "share/jupyter/nbextensions/dcef"
-"dcef/labextension" = "share/jupyter/labextensions/dcef"
-"dcef.json" = "etc/jupyter/nbconfig/notebook.d/dcef.json"
+"buckaroo/nbextension" = "share/jupyter/nbextensions/buckaroo"
+"buckaroo/labextension" = "share/jupyter/labextensions/buckaroo"
+"buckaroo.json" = "etc/jupyter/nbconfig/notebook.d/buckaroo.json"
 
 [tool.hatch.build.targets.sdist]
 exclude = [
     ".github",
     "examples",
     "tests",
     "ui-tests*",
@@ -77,16 +77,16 @@
     "*.ini",
     ".pre*",
     "jest*",
 ]
 
 [tool.hatch.build.hooks.jupyter-builder]
 ensured-targets = [
-    "dcef/nbextension/index.js",
-    "dcef/labextension/package.json",
+    "buckaroo/nbextension/index.js",
+    "buckaroo/labextension/package.json",
 ]
 dependencies = [
     "hatch-jupyter-builder>=0.8.1",
 ]
 build-function = "hatch_jupyter_builder.npm_builder"
 
 [tool.hatch.build.hooks.jupyter-builder.build-kwargs]
@@ -95,15 +95,15 @@
 npm = [
     "yarn",
 ]
 
 [tool.isort]
 profile = "black"
 known_first_party = [
-    "dcef",
+    "buckaroo",
     "tests",
 ]
 line_length = 80
 
 [tool.pylint.messages_control]
 disable = "C0330, C0326"
 
@@ -129,12 +129,12 @@
 tag_template = "v{new_version}"
 
 [[tool.tbump.file]]
 src = "pyproject.toml"
 version_template = "version = \"{major}.{minor}.{patch}{channel}{release}\""
 
 [[tool.tbump.file]]
-src = "dcef/_version.py"
+src = "buckaroo/_version.py"
 
 [[tool.tbump.file]]
 src = "package.json"
 version_template = "\"version\": \"{major}.{minor}.{patch}{channel}{release}\""
```

### Comparing `buckaroo-0.2.6/PKG-INFO` & `buckaroo-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: buckaroo
-Version: 0.2.6
+Version: 0.2.7
 Summary: Herder - GUI Data wrangling for pandas
-Project-URL: Homepage, https://github.com/bloomberg/dcef
+Project-URL: Homepage, https://github.com/paddymul/buckaroo
 Author: Paddy Mullen
 License: Copyright (c) 2019 Bloomberg
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

