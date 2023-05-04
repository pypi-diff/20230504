# Comparing `tmp/buckaroo-0.2.7.tar.gz` & `tmp/buckaroo-0.2.8.tar.gz`

## Comparing `buckaroo-0.2.7.tar` & `buckaroo-0.2.8.tar`

### file list

```diff
@@ -1,75 +1,76 @@
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 buckaroo-0.2.7/.coveragerc
--rw-r--r--   0        0        0     7520 2020-02-02 00:00:00.000000 buckaroo-0.2.7/RELEASE.md
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 buckaroo-0.2.7/babel.config.js
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 buckaroo-0.2.7/buckaroo.json
--rwxr-xr-x   0        0        0      232 2020-02-02 00:00:00.000000 buckaroo-0.2.7/full_build.sh
--rw-r--r--   0        0        0     4419 2020-02-02 00:00:00.000000 buckaroo-0.2.7/introduction.ipynb
--rw-r--r--   0        0        0     4520 2020-02-02 00:00:00.000000 buckaroo-0.2.7/package.json
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 buckaroo-0.2.7/setup.py
--rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 buckaroo-0.2.7/tryit.ipynb
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 buckaroo-0.2.7/tsconfig.json
--rw-r--r--   0        0        0     2837 2020-02-02 00:00:00.000000 buckaroo-0.2.7/webpack.config.js
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 buckaroo-0.2.7/webpack.lab.config.js
--rw-r--r--   0        0        0   321074 2020-02-02 00:00:00.000000 buckaroo-0.2.7/yarn.lock
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 buckaroo-0.2.7/buckaroo/__init__.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 buckaroo-0.2.7/buckaroo/_frontend.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 buckaroo-0.2.7/buckaroo/_version.py
--rw-r--r--   0        0        0     5065 2020-02-02 00:00:00.000000 buckaroo-0.2.7/buckaroo/all_transforms.py
--rw-r--r--   0        0        0     4518 2020-02-02 00:00:00.000000 buckaroo-0.2.7/buckaroo/buckaroo_widget.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 buckaroo-0.2.7/buckaroo/channeldata.json
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 buckaroo-0.2.7/buckaroo/configure_utils.py
--rw-r--r--   0        0        0     5608 2020-02-02 00:00:00.000000 buckaroo-0.2.7/buckaroo/dcf_transform.py
--rw-r--r--   0        0        0     6535 2020-02-02 00:00:00.000000 buckaroo-0.2.7/buckaroo/df_methods.py
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 buckaroo-0.2.7/buckaroo/index.html
--rw-r--r--   0        0        0    17284 2020-02-02 00:00:00.000000 buckaroo-0.2.7/buckaroo/lispy.py
--rw-r--r--   0        0        0     3683 2020-02-02 00:00:00.000000 buckaroo-0.2.7/buckaroo/summary_stats.py
--rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 buckaroo-0.2.7/buckaroo/views.py
--rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 buckaroo-0.2.7/buckaroo/labextension/package.json
--rw-r--r--   0        0        0  1241256 2020-02-02 00:00:00.000000 buckaroo-0.2.7/buckaroo/labextension/static/116.b6e5adfccd7c520a720a.js
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 buckaroo-0.2.7/buckaroo/labextension/static/116.b6e5adfccd7c520a720a.js.LICENSE.txt
--rw-r--r--   0        0        0   373838 2020-02-02 00:00:00.000000 buckaroo-0.2.7/buckaroo/labextension/static/250.b55e2550464d9477eb95.js
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 buckaroo-0.2.7/buckaroo/labextension/static/250.b55e2550464d9477eb95.js.LICENSE.txt
--rw-r--r--   0        0        0    10250 2020-02-02 00:00:00.000000 buckaroo-0.2.7/buckaroo/labextension/static/480.e809fc8a18bc53e804a1.js
--rw-r--r--   0        0        0    70484 2020-02-02 00:00:00.000000 buckaroo-0.2.7/buckaroo/labextension/static/486.f08778dfb765d893ceaf.js
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 buckaroo-0.2.7/buckaroo/labextension/static/486.f08778dfb765d893ceaf.js.LICENSE.txt
--rw-r--r--   0        0        0     9717 2020-02-02 00:00:00.000000 buckaroo-0.2.7/buckaroo/labextension/static/568.9a4b0a85049c75a13a73.js
--rw-r--r--   0        0        0     7384 2020-02-02 00:00:00.000000 buckaroo-0.2.7/buckaroo/labextension/static/remoteEntry.d4606edd7ebd1ec0dcc6.js
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 buckaroo-0.2.7/buckaroo/labextension/static/style.js
--rw-r--r--   0        0        0    12889 2020-02-02 00:00:00.000000 buckaroo-0.2.7/buckaroo/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 buckaroo-0.2.7/buckaroo/nbextension/extension.js
--rw-r--r--   0        0        0  1696168 2020-02-02 00:00:00.000000 buckaroo-0.2.7/buckaroo/nbextension/index.js
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 buckaroo-0.2.7/buckaroo/nbextension/index.js.LICENSE.txt
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 buckaroo-0.2.7/buckaroo/noarch/current_repodata.json
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 buckaroo-0.2.7/buckaroo/noarch/current_repodata.json.bz2
--rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 buckaroo-0.2.7/buckaroo/noarch/index.html
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 buckaroo-0.2.7/buckaroo/noarch/repodata.json
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 buckaroo-0.2.7/buckaroo/noarch/repodata.json.bz2
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 buckaroo-0.2.7/buckaroo/noarch/repodata_from_packages.json
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 buckaroo-0.2.7/buckaroo/noarch/repodata_from_packages.json.bz2
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 buckaroo-0.2.7/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 buckaroo-0.2.7/docs/make.bat
--rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 buckaroo-0.2.7/docs/source/FAQ.rst
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 buckaroo-0.2.7/docs/source/conf.py
--rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 buckaroo-0.2.7/docs/source/contributing.rst
--rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 buckaroo-0.2.7/docs/source/index.rst
--rwxr-xr-x   0        0        0      268 2020-02-02 00:00:00.000000 buckaroo-0.2.7/docs/source/install.rst
--rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 buckaroo-0.2.7/docs/source/using.rst
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 buckaroo-0.2.7/docs/source/_static/embed-bundle.js.LICENSE.txt
--rw-r--r--   0        0        0     3054 2020-02-02 00:00:00.000000 buckaroo-0.2.7/js/dcefwidget.ts
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 buckaroo-0.2.7/js/extension.ts
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 buckaroo-0.2.7/js/index.ts
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 buckaroo-0.2.7/js/plugin.ts
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 buckaroo-0.2.7/js/version.ts
--rw-r--r--   0        0        0  1335815 2020-02-02 00:00:00.000000 buckaroo-0.2.7/static/images/dcf-jupyter.png
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 buckaroo-0.2.7/style/widget.css
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 buckaroo-0.2.7/style/icons/arrow-down-short-dark.svg
--rwxr-xr-x   0        0        0      416 2020-02-02 00:00:00.000000 buckaroo-0.2.7/style/icons/arrow-down-short.svg
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 buckaroo-0.2.7/style/icons/arrow-up-short-dark.svg
--rwxr-xr-x   0        0        0      400 2020-02-02 00:00:00.000000 buckaroo-0.2.7/style/icons/arrow-up-short.svg
--rwxr-xr-x   0        0        0      349 2020-02-02 00:00:00.000000 buckaroo-0.2.7/style/icons/filter-dark.svg
--rwxr-xr-x   0        0        0      349 2020-02-02 00:00:00.000000 buckaroo-0.2.7/style/icons/filter.svg
--rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 buckaroo-0.2.7/.gitignore
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 buckaroo-0.2.7/LICENSE.txt
--rw-r--r--   0        0        0     8870 2020-02-02 00:00:00.000000 buckaroo-0.2.7/README.md
--rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 buckaroo-0.2.7/pyproject.toml
--rw-r--r--   0        0        0    11646 2020-02-02 00:00:00.000000 buckaroo-0.2.7/PKG-INFO
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 buckaroo-0.2.8/.#README.md -> paddy@Paddys-MacBook-Air.local.752
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 buckaroo-0.2.8/.coveragerc
+-rw-r--r--   0        0        0     7520 2020-02-02 00:00:00.000000 buckaroo-0.2.8/RELEASE.md
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 buckaroo-0.2.8/babel.config.js
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 buckaroo-0.2.8/buckaroo.json
+-rwxr-xr-x   0        0        0      232 2020-02-02 00:00:00.000000 buckaroo-0.2.8/full_build.sh
+-rw-r--r--   0        0        0     4419 2020-02-02 00:00:00.000000 buckaroo-0.2.8/introduction.ipynb
+-rw-r--r--   0        0        0     4520 2020-02-02 00:00:00.000000 buckaroo-0.2.8/package.json
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 buckaroo-0.2.8/setup.py
+-rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 buckaroo-0.2.8/tryit.ipynb
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 buckaroo-0.2.8/tsconfig.json
+-rw-r--r--   0        0        0     2837 2020-02-02 00:00:00.000000 buckaroo-0.2.8/webpack.config.js
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 buckaroo-0.2.8/webpack.lab.config.js
+-rw-r--r--   0        0        0   321074 2020-02-02 00:00:00.000000 buckaroo-0.2.8/yarn.lock
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 buckaroo-0.2.8/buckaroo/__init__.py
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 buckaroo-0.2.8/buckaroo/_frontend.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 buckaroo-0.2.8/buckaroo/_version.py
+-rw-r--r--   0        0        0     5065 2020-02-02 00:00:00.000000 buckaroo-0.2.8/buckaroo/all_transforms.py
+-rw-r--r--   0        0        0     4518 2020-02-02 00:00:00.000000 buckaroo-0.2.8/buckaroo/buckaroo_widget.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 buckaroo-0.2.8/buckaroo/channeldata.json
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 buckaroo-0.2.8/buckaroo/configure_utils.py
+-rw-r--r--   0        0        0     5608 2020-02-02 00:00:00.000000 buckaroo-0.2.8/buckaroo/dcf_transform.py
+-rw-r--r--   0        0        0     6535 2020-02-02 00:00:00.000000 buckaroo-0.2.8/buckaroo/df_methods.py
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 buckaroo-0.2.8/buckaroo/index.html
+-rw-r--r--   0        0        0    17284 2020-02-02 00:00:00.000000 buckaroo-0.2.8/buckaroo/lispy.py
+-rw-r--r--   0        0        0     3683 2020-02-02 00:00:00.000000 buckaroo-0.2.8/buckaroo/summary_stats.py
+-rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 buckaroo-0.2.8/buckaroo/views.py
+-rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 buckaroo-0.2.8/buckaroo/labextension/package.json
+-rw-r--r--   0        0        0  1241256 2020-02-02 00:00:00.000000 buckaroo-0.2.8/buckaroo/labextension/static/116.b6e5adfccd7c520a720a.js
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 buckaroo-0.2.8/buckaroo/labextension/static/116.b6e5adfccd7c520a720a.js.LICENSE.txt
+-rw-r--r--   0        0        0   373838 2020-02-02 00:00:00.000000 buckaroo-0.2.8/buckaroo/labextension/static/250.b55e2550464d9477eb95.js
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 buckaroo-0.2.8/buckaroo/labextension/static/250.b55e2550464d9477eb95.js.LICENSE.txt
+-rw-r--r--   0        0        0    10250 2020-02-02 00:00:00.000000 buckaroo-0.2.8/buckaroo/labextension/static/480.e809fc8a18bc53e804a1.js
+-rw-r--r--   0        0        0    70484 2020-02-02 00:00:00.000000 buckaroo-0.2.8/buckaroo/labextension/static/486.f08778dfb765d893ceaf.js
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 buckaroo-0.2.8/buckaroo/labextension/static/486.f08778dfb765d893ceaf.js.LICENSE.txt
+-rw-r--r--   0        0        0     9717 2020-02-02 00:00:00.000000 buckaroo-0.2.8/buckaroo/labextension/static/568.9a4b0a85049c75a13a73.js
+-rw-r--r--   0        0        0     7384 2020-02-02 00:00:00.000000 buckaroo-0.2.8/buckaroo/labextension/static/remoteEntry.d4606edd7ebd1ec0dcc6.js
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 buckaroo-0.2.8/buckaroo/labextension/static/style.js
+-rw-r--r--   0        0        0    12889 2020-02-02 00:00:00.000000 buckaroo-0.2.8/buckaroo/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 buckaroo-0.2.8/buckaroo/nbextension/extension.js
+-rw-r--r--   0        0        0  1696168 2020-02-02 00:00:00.000000 buckaroo-0.2.8/buckaroo/nbextension/index.js
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 buckaroo-0.2.8/buckaroo/nbextension/index.js.LICENSE.txt
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 buckaroo-0.2.8/buckaroo/noarch/current_repodata.json
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 buckaroo-0.2.8/buckaroo/noarch/current_repodata.json.bz2
+-rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 buckaroo-0.2.8/buckaroo/noarch/index.html
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 buckaroo-0.2.8/buckaroo/noarch/repodata.json
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 buckaroo-0.2.8/buckaroo/noarch/repodata.json.bz2
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 buckaroo-0.2.8/buckaroo/noarch/repodata_from_packages.json
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 buckaroo-0.2.8/buckaroo/noarch/repodata_from_packages.json.bz2
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 buckaroo-0.2.8/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 buckaroo-0.2.8/docs/make.bat
+-rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 buckaroo-0.2.8/docs/source/FAQ.rst
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 buckaroo-0.2.8/docs/source/conf.py
+-rw-r--r--   0        0        0     4096 2020-02-02 00:00:00.000000 buckaroo-0.2.8/docs/source/contributing.rst
+-rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 buckaroo-0.2.8/docs/source/index.rst
+-rwxr-xr-x   0        0        0      289 2020-02-02 00:00:00.000000 buckaroo-0.2.8/docs/source/install.rst
+-rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 buckaroo-0.2.8/docs/source/using.rst
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 buckaroo-0.2.8/docs/source/_static/embed-bundle.js.LICENSE.txt
+-rw-r--r--   0        0        0     3054 2020-02-02 00:00:00.000000 buckaroo-0.2.8/js/dcefwidget.ts
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 buckaroo-0.2.8/js/extension.ts
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 buckaroo-0.2.8/js/index.ts
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 buckaroo-0.2.8/js/plugin.ts
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 buckaroo-0.2.8/js/version.ts
+-rw-r--r--   0        0        0  1335815 2020-02-02 00:00:00.000000 buckaroo-0.2.8/static/images/dcf-jupyter.png
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 buckaroo-0.2.8/style/widget.css
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 buckaroo-0.2.8/style/icons/arrow-down-short-dark.svg
+-rwxr-xr-x   0        0        0      416 2020-02-02 00:00:00.000000 buckaroo-0.2.8/style/icons/arrow-down-short.svg
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 buckaroo-0.2.8/style/icons/arrow-up-short-dark.svg
+-rwxr-xr-x   0        0        0      400 2020-02-02 00:00:00.000000 buckaroo-0.2.8/style/icons/arrow-up-short.svg
+-rwxr-xr-x   0        0        0      349 2020-02-02 00:00:00.000000 buckaroo-0.2.8/style/icons/filter-dark.svg
+-rwxr-xr-x   0        0        0      349 2020-02-02 00:00:00.000000 buckaroo-0.2.8/style/icons/filter.svg
+-rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 buckaroo-0.2.8/.gitignore
+-rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 buckaroo-0.2.8/LICENSE.txt
+-rw-r--r--   0        0        0     8899 2020-02-02 00:00:00.000000 buckaroo-0.2.8/README.md
+-rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 buckaroo-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0    11684 2020-02-02 00:00:00.000000 buckaroo-0.2.8/PKG-INFO
```

### Comparing `buckaroo-0.2.7/RELEASE.md` & `buckaroo-0.2.8/RELEASE.md`

 * *Files identical despite different names*

### Comparing `buckaroo-0.2.7/introduction.ipynb` & `buckaroo-0.2.8/introduction.ipynb`

 * *Files identical despite different names*

### Comparing `buckaroo-0.2.7/package.json` & `buckaroo-0.2.8/package.json`

 * *Files identical despite different names*

### Comparing `buckaroo-0.2.7/tryit.ipynb` & `buckaroo-0.2.8/tryit.ipynb`

 * *Files identical despite different names*

### Comparing `buckaroo-0.2.7/tsconfig.json` & `buckaroo-0.2.8/tsconfig.json`

 * *Files identical despite different names*

### Comparing `buckaroo-0.2.7/webpack.config.js` & `buckaroo-0.2.8/webpack.config.js`

 * *Files identical despite different names*

### Comparing `buckaroo-0.2.7/yarn.lock` & `buckaroo-0.2.8/yarn.lock`

 * *Files identical despite different names*

### Comparing `buckaroo-0.2.7/buckaroo/all_transforms.py` & `buckaroo-0.2.8/buckaroo/all_transforms.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.2.7/buckaroo/buckaroo_widget.py` & `buckaroo-0.2.8/buckaroo/buckaroo_widget.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.2.7/buckaroo/configure_utils.py` & `buckaroo-0.2.8/buckaroo/configure_utils.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.2.7/buckaroo/dcf_transform.py` & `buckaroo-0.2.8/buckaroo/dcf_transform.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.2.7/buckaroo/df_methods.py` & `buckaroo-0.2.8/buckaroo/df_methods.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.2.7/buckaroo/index.html` & `buckaroo-0.2.8/buckaroo/index.html`

 * *Files identical despite different names*

### Comparing `buckaroo-0.2.7/buckaroo/lispy.py` & `buckaroo-0.2.8/buckaroo/lispy.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.2.7/buckaroo/summary_stats.py` & `buckaroo-0.2.8/buckaroo/summary_stats.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.2.7/buckaroo/views.py` & `buckaroo-0.2.8/buckaroo/views.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.2.7/buckaroo/labextension/package.json` & `buckaroo-0.2.8/buckaroo/labextension/package.json`

 * *Files identical despite different names*

### Comparing `buckaroo-0.2.7/buckaroo/labextension/static/116.b6e5adfccd7c520a720a.js` & `buckaroo-0.2.8/buckaroo/labextension/static/116.b6e5adfccd7c520a720a.js`

 * *Files identical despite different names*

### Comparing `buckaroo-0.2.7/buckaroo/labextension/static/116.b6e5adfccd7c520a720a.js.LICENSE.txt` & `buckaroo-0.2.8/buckaroo/labextension/static/116.b6e5adfccd7c520a720a.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `buckaroo-0.2.7/buckaroo/labextension/static/250.b55e2550464d9477eb95.js` & `buckaroo-0.2.8/buckaroo/labextension/static/250.b55e2550464d9477eb95.js`

 * *Files identical despite different names*

### Comparing `buckaroo-0.2.7/buckaroo/labextension/static/250.b55e2550464d9477eb95.js.LICENSE.txt` & `buckaroo-0.2.8/buckaroo/labextension/static/250.b55e2550464d9477eb95.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `buckaroo-0.2.7/buckaroo/labextension/static/480.e809fc8a18bc53e804a1.js` & `buckaroo-0.2.8/buckaroo/labextension/static/480.e809fc8a18bc53e804a1.js`

 * *Files identical despite different names*

### Comparing `buckaroo-0.2.7/buckaroo/labextension/static/486.f08778dfb765d893ceaf.js` & `buckaroo-0.2.8/buckaroo/labextension/static/486.f08778dfb765d893ceaf.js`

 * *Files identical despite different names*

### Comparing `buckaroo-0.2.7/buckaroo/labextension/static/568.9a4b0a85049c75a13a73.js` & `buckaroo-0.2.8/buckaroo/labextension/static/568.9a4b0a85049c75a13a73.js`

 * *Files identical despite different names*

### Comparing `buckaroo-0.2.7/buckaroo/labextension/static/remoteEntry.d4606edd7ebd1ec0dcc6.js` & `buckaroo-0.2.8/buckaroo/labextension/static/remoteEntry.d4606edd7ebd1ec0dcc6.js`

 * *Files identical despite different names*

### Comparing `buckaroo-0.2.7/buckaroo/labextension/static/third-party-licenses.json` & `buckaroo-0.2.8/buckaroo/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `buckaroo-0.2.7/buckaroo/nbextension/index.js` & `buckaroo-0.2.8/buckaroo/nbextension/index.js`

 * *Files identical despite different names*

### Comparing `buckaroo-0.2.7/buckaroo/nbextension/index.js.LICENSE.txt` & `buckaroo-0.2.8/buckaroo/nbextension/index.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `buckaroo-0.2.7/buckaroo/noarch/index.html` & `buckaroo-0.2.8/buckaroo/noarch/index.html`

 * *Files identical despite different names*

### Comparing `buckaroo-0.2.7/docs/Makefile` & `buckaroo-0.2.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `buckaroo-0.2.7/docs/make.bat` & `buckaroo-0.2.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `buckaroo-0.2.7/docs/source/FAQ.rst` & `buckaroo-0.2.8/docs/source/FAQ.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-.. DCEF documentation master file, created by
+.. Buckaroo documentation master file, created by
    sphinx-quickstart on Wed Apr 19 14:07:15 2023.
    You can adapt this file completely to your liking, but it should at least
    contain the root `toctree` directive.
 
-DCEF - FAQ
+Buckaroo - FAQ
 ==========================================
 
 
 * **Why did you use LISP?**
 
   This is a problem domain that required a DSL and intermediate language.  I could have written my own or chosen an existing language.  I chose LISP because it is simple to interpret and generate, additionally it is well understood.  Yes LISP is obscure, but it is less obscure than a custom language I would write myself.  I didn't want to expose an entire progrmaming language with all the attendant security risks, I wanted a small safe strict subset of programming features that I explicitly exposed.  LISP is easier to manipulate as an AST than any language in PL history.  I am not yet using any symbolic manipulation facilities of LISP, and will probably only use them in limited ways.
```

### Comparing `buckaroo-0.2.7/docs/source/conf.py` & `buckaroo-0.2.8/docs/source/conf.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 #
 # For the full list of built-in configuration values, see the documentation:
 # https://www.sphinx-doc.org/en/master/usage/configuration.html
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
-project = 'DCEF'
+project = 'Buckaroo'
 copyright = '2023, Paddy Mullen'
 author = 'Paddy Mullen'
-release = '0.2'
+release = '0.2.8'
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = []
 
 templates_path = ['_templates']
```

### Comparing `buckaroo-0.2.7/docs/source/contributing.rst` & `buckaroo-0.2.8/docs/source/contributing.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 .. _Contributing:
 
 ====================
-Contributing to DCEF
+Contributing to Buckaroo
 ====================
 
-DCEF is actively looking for contributors.  All forms of participation are welcome, from bug reports, to suggestions, to code contributions.
+Buckaroo is actively looking for contributors.  All forms of participation are welcome, from bug reports, to suggestions, to code contributions.
 
 
 Developing in the Jupyter Lab environment
 =========================================
 
-The easiest way to develop and contribute to DCEF is to add ``Commands``.  When I use DCEF to clean and explore a new dataset, I firt try to use the built in DCEF commands in the UI.  When I want to perform a manipulation that doesn't yet exist in DCEF, I first drop down to raw pandas/python like I would before DCEF... Then I figure out how to expose that functionality as a ``Command``.  While working with manatee data, I recognized that a column was probably date times, but a ``to_datetime``  ``Command`` didn't exist.  So I wrote one.
+The easiest way to develop and contribute to Buckaroo is to add ``Commands``.  When I use Buckaroo to clean and explore a new dataset, I firt try to use the built in Buckaroo commands in the UI.  When I want to perform a manipulation that doesn't yet exist in Buckaroo, I first drop down to raw pandas/python like I would before Buckaroo... Then I figure out how to expose that functionality as a ``Command``.  While working with manatee data, I recognized that a column was probably date times, but a ``to_datetime``  ``Command`` didn't exist.  So I wrote one.
 
 .. code-block:: python
 
     pd.to_datetime(df['REPDATE']).head()
     #outputs ->
     #0   1974-04-03 00:00:00+00:00
     #1   1974-06-27 00:00:00+00:00
@@ -35,49 +35,49 @@
         @staticmethod 
         def transform_to_py(df, col):
             return "    df['%s'] = pd.to_datetime(df['%s'])" % (col, col)
 
 
 When you use the ``add_command`` decorator, the command is instantly added to the UI of the corresponding widget.  Subsequent re-evalutations of the same cell, will replace a ``Command`` in the widget with the same name.  This allows you to iteratively develop commands.
 
-Once you have developed a ``Command`` you can either continue to use it internally as with the ``add_command`` decorator or you can open a PR and add it to the builtin commands for DCEF `all_transforms.py <https://github.com/paddymul/dcef/blob/main/dcef/all_transforms.py>`_.
+Once you have developed a ``Command`` you can either continue to use it internally as with the ``add_command`` decorator or you can open a PR and add it to the builtin commands for Buckaroo `all_transforms.py <https://github.com/paddymul/buckaroo/blob/main/buckaroo/all_transforms.py>`_.
 
 The upside of just using the @add_command decorator is that you don't have to setup a development environment.
 
 Setting up a development environment
 ====================================
 
 First, you need to fork the project. Then setup your environment:
 
 .. code-block:: bash
 
    # create a new conda environment
-   conda create -n dcef-dev jupyterlab pandas nodejs yarn pip
-   conda activate dcef-dev
+   conda create -n buckaroo-dev jupyterlab pandas nodejs yarn pip
+   conda activate buckaroo-dev
    pip install build twine
 
-   # download dcef from your GitHub fork
-   git clone https://github.com/<your-github-username>/dcef.git
+   # download buckaroo from your GitHub fork
+   git clone https://github.com/<your-github-username>/buckaroo.git
    # or start by cloning the main repo
-   git clone https://github.com/paddymul/dcef.git
+   git clone https://github.com/paddymul/buckaroo.git
 
    # install JS dependencies and build js assets
-   cd dcef
+   cd buckaroo
    yarn install
 
-   # install DCEF in editable mode
+   # install Buckaroo in editable mode
    python -m pip install -ve .
 
    #in another shell, setup the typescript watcher
-   conda activate dcef-dev
+   conda activate buckaroo-dev
    yarn build && yarn watch
    #this will build the jupyter lab extension, and recompile on any code changes
 
    #start your jupyter lab server in another shell
-   conda activate dcef-dev
+   conda activate buckaroo-dev
    jupyter lab
 
    #work on your jupyter notebook from that lab server
 
 .. note::
    Getting typescript updates from the widget into a jupyter lab notebook is a little tricky.  The following steps ensure that typescript code changes are picked up.
```

### Comparing `buckaroo-0.2.7/docs/source/index.rst` & `buckaroo-0.2.8/docs/source/index.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-.. DCEF documentation master file, created by
+.. Buckaroo documentation master file, created by
    sphinx-quickstart on Wed Apr 19 14:07:15 2023.
    You can adapt this file completely to your liking, but it should at least
    contain the root `toctree` directive.
 
-DCEF - Data Cleaning Exploration Framework
+Buckaroo - Data Cleaning Exploration Framework
 ==========================================
-DCEF is a tool to quickly clean and explore DataFrames with a visual UI for common cleaning operations AND emitting python code that performs the transformation. 
+Buckaroo is a tool to quickly clean and explore DataFrames with a visual UI for common cleaning operations AND emitting python code that performs the transformation. 
 
 
-We all know how awkward it is to clean data in jupyter notebooks.  Multiple cells of exploratory work, trying different transforms, looking up different transforms, adhoc functions that work in one notebook and have to be either copied/pasta-ed to the next notebook, or rewritten from scratch.  DCEF aims to massively speed up that process.
+We all know how awkward it is to clean data in jupyter notebooks.  Multiple cells of exploratory work, trying different transforms, looking up different transforms, adhoc functions that work in one notebook and have to be either copied/pasta-ed to the next notebook, or rewritten from scratch.  Buckaroo aims to massively speed up that process.
 
 .. raw:: html
 
 	 <iframe width="560" height="315" src="https://www.youtube.com/embed/Wt-pqeBBuIY" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
 
 
 
@@ -31,8 +31,8 @@
 
 Indices and tables
 ==================
 
 * :ref:`genindex`
 * :ref:`modindex`
 * :ref:`search`
-* `DCEF on github <https://github.com/paddymul/dcef>`_
+* `Buckaroo on github <https://github.com/paddymul/buckaroo>`_
```

### Comparing `buckaroo-0.2.7/docs/source/_static/embed-bundle.js.LICENSE.txt` & `buckaroo-0.2.8/docs/source/_static/embed-bundle.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `buckaroo-0.2.7/js/dcefwidget.ts` & `buckaroo-0.2.8/js/dcefwidget.ts`

 * *Files identical despite different names*

### Comparing `buckaroo-0.2.7/js/extension.ts` & `buckaroo-0.2.8/js/extension.ts`

 * *Files identical despite different names*

### Comparing `buckaroo-0.2.7/js/plugin.ts` & `buckaroo-0.2.8/js/plugin.ts`

 * *Files identical despite different names*

### Comparing `buckaroo-0.2.7/static/images/dcf-jupyter.png` & `buckaroo-0.2.8/static/images/dcf-jupyter.png`

 * *Files identical despite different names*

### Comparing `buckaroo-0.2.7/.gitignore` & `buckaroo-0.2.8/.gitignore`

 * *Files identical despite different names*

### Comparing `buckaroo-0.2.7/LICENSE.txt` & `buckaroo-0.2.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `buckaroo-0.2.7/README.md` & `buckaroo-0.2.8/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-# DCEF - Data Cleaning Exploration Framework
-We all know how awkward it is to clean data in jupyter notebooks.  Multiple cells of exploratory work, trying different transforms, looking up different transforms, adhoc functions that work in one notebook and have to be either copied/pasta-ed to the next notebook, or rewritten from scratch.  Data Cleaning Explorationg Framework  (DCEF) makes all of that better by providing a visual UI for common cleaning operations AND emitting python code that performs the transformation. Specifically, the DCEF is a tool built to interactively explore, clean, and transform pandas dataframes.
+# Buckaroo - The Data Wrangling Assistant
+We all know how awkward it is to clean data in jupyter notebooks.  Multiple cells of exploratory work, trying different transforms, looking up different transforms, adhoc functions that work in one notebook and have to be either copied/pasta-ed to the next notebook, or rewritten from scratch.  Buckaro makes all of that better by providing a visual UI for common cleaning operations AND emitting python code that performs the transformation. Specifically, the Buckaroo is a tool built to interactively explore, clean, and transform pandas dataframes.
 
-![Data Cleaning Exploration Framework Screenshot](static/images/dcf-jupyter.png)
+![Buckaroo Screenshot](static/images/dcf-jupyter.png)
 
 
 ## Installation
 
-If using JupyterLab, `dcef` requires JupyterLab version 3 or higher.
+If using JupyterLab, `buckaroo` requires JupyterLab version 3 or higher.
 
-You can install `dcef` using `pip`
+You can install `buckaroo` using `pip`
 
 Using `pip`:
 
 ```bash
-pip install dcef
+pip install buckaroo
 ```
 
 ## Documentation
 
-To get started with using DCEF, check out the full documentation:
+To get started with using Buckaroo, check out the full documentation:
 
-https://dcef.readthedocs.io/
+https://buckaroo.readthedocs.io/
 
 
-# Using DCEF
+# Using Buckaroo
 
 in a jupyter lab notebook just add the following to a cell
 
 ```python
-from dcef.dcef_widget import DCEFWidget
-DCEFWidget(df=df)  #df being the dataframe you want to explore
+from buckaroo.buckaroo_widget import BuckarooWidget
+BuckarooWidget(df=df)  #df being the dataframe you want to explore
 ``` 
-and you will see the UI for DCEF
+and you will see the UI for Buckaroo
 
 
 ## Using commands
 
-At the core DCEF commands operate on columns.  You must first click on a cell (not a header) in the top pane to select a column.
+At the core Buckaroo commands operate on columns.  You must first click on a cell (not a header) in the top pane to select a column.
 
 Next you must click on a command like `dropcol`, `fillna`, or `groupby` to create a new command
 
 After creating a new command, you will see that command in the commands list, now you must edit the details of a command.  Select the command by clicking on the bottom cell.
 
 At this point you can either delete the command by clicking the `X` button or change command parameters.
 
 ## Writing your own commands
 
-Builtin commands are found in [all_transforms.py](dcef/all_transforms.py)
+Builtin commands are found in [all_transforms.py](buckaroo/all_transforms.py)
 
 ### Simple example
 Here is a simple example command
 ```python
 class DropCol(Command):
     command_default = [s('dropcol'), s('df'), "col"]
     command_pattern = [None]
@@ -138,15 +138,15 @@
 These transforms emit multiple DataFrames
   * Relational extract (extract one or more columns into a second dataframe that can be joined back to a foreign key column)
   * Split on column (emit separate dataframes for each value of a categorical, no shape editting)
 * DataFrame combination
   * concat (concatenate multiple dataframes, with UI affordances to assure a similar shape)
   * join (join two dataframes on a key, with UI affordances)
 
-DCEF can only work on a single input dataframe shape at a time.  Any newly created columns are visible on output, but not available for manipulation in the same DCEF Cell.
+Buckaroo can only work on a single input dataframe shape at a time.  Any newly created columns are visible on output, but not available for manipulation in the same Buckaroo Cell.
 
 
 # Components
 * a rich table widget that is embeddable into applications and in the jupyter notebook.
 * A UI for selecting and trying transforms interactively
 * An output table widget showing the transformed dataframe
 
@@ -155,23 +155,23 @@
 
 ## Exists now
   * React frontend app
     * Displays a datatframe
 	* Simple UI for column level functions
 	* Shows generated python code
 	* Shows transformed data frame
-  * DCEF server
+  * Buckaroo server
     * Serves up dataframes for use by frontend
-	* responds to dcef commands
+	* responds to buckaroo commands
 	* shows generated python code
   * Developer User experience
-	* define DCEF commands in python onloy
-  * DCEF Intepreter
+	* define Buckaroo commands in python onloy
+  * Buckaroo Intepreter
     * Based on Peter Norvig's lispy.py, a simple syntax that is easy for the frontend to generate (no parens, just JSON arrays)
-  * DCEF core (actual transforms supported)
+  * Buckaroo core (actual transforms supported)
     * dropcol
 	* fillna
 	* one hot
 	* safe int
 	* GroupBy
 
 ## Next major features
@@ -183,15 +183,15 @@
     * Styling
 	  * Server only, some UI for DataFrame selection
     * Pre filtering concept (only operate on first 1000 rows, some sample of all rows)
 	* DataFrame joining UI
 	* Summary statistics tab for incoming dataframe
 	* Multi index columns
 	* DateTimeIndex support
-  * DCEF core
+  * Buckaroo core
 	* MakeCategorical
 	* Quantize
 	* Resample
 	* ManyColdDecoding
 	* IndexShift
 	* Computed
 	* Stack/Unstack
@@ -204,16 +204,16 @@
 
 
 ## Development installation
 
 For a development installation:
 
 ```bash
-git clone https://github.com/paddymul/dcef.git
-cd dcef
+git clone https://github.com/paddymul/buckaroo.git
+cd buckaroo
 conda install ipywidgets=8 jupyterlab
 pip install -ve .
 ```
 
 Enabling development install for Jupyter notebook:
```

### Comparing `buckaroo-0.2.7/pyproject.toml` & `buckaroo-0.2.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,24 +3,25 @@
     "hatchling",
     "jupyterlab~=3.0",
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "buckaroo"
-description = "Herder - GUI Data wrangling for pandas"
+description = "Buckaroo - GUI Data wrangling for pandas"
 readme = "README.md"
 requires-python = ">=3.7"
 authors = [
     { name = "Paddy Mullen" },
 ]
 keywords = [
     "IPython",
     "Jupyter",
     "Widgets",
+    "pandas",
 ]
 classifiers = [
     "Framework :: Jupyter",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python",
@@ -30,15 +31,15 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 dependencies = [
     "ipywidgets>=7.6.0,<9"
 ]
-version = "0.2.7"
+version = "0.2.8"
 
 [project.license]
 file = "LICENSE.txt"
 
 [project.optional-dependencies]
 test = [
     "nbval>=0.9",
```

### Comparing `buckaroo-0.2.7/PKG-INFO` & `buckaroo-0.2.8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: buckaroo
-Version: 0.2.7
-Summary: Herder - GUI Data wrangling for pandas
+Version: 0.2.8
+Summary: Buckaroo - GUI Data wrangling for pandas
 Project-URL: Homepage, https://github.com/paddymul/buckaroo
 Author: Paddy Mullen
 License: Copyright (c) 2019 Bloomberg
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
@@ -28,15 +28,15 @@
         FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
         DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
         SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
         CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 License-File: LICENSE.txt
-Keywords: IPython,Jupyter,Widgets
+Keywords: IPython,Jupyter,Widgets,pandas
 Classifier: Framework :: Jupyter
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -49,63 +49,63 @@
 Provides-Extra: test
 Requires-Dist: nbval>=0.9; extra == 'test'
 Requires-Dist: pandas<=1.3.5; extra == 'test'
 Requires-Dist: pytest-cov>=3; extra == 'test'
 Requires-Dist: pytest>=6; extra == 'test'
 Description-Content-Type: text/markdown
 
-# DCEF - Data Cleaning Exploration Framework
-We all know how awkward it is to clean data in jupyter notebooks.  Multiple cells of exploratory work, trying different transforms, looking up different transforms, adhoc functions that work in one notebook and have to be either copied/pasta-ed to the next notebook, or rewritten from scratch.  Data Cleaning Explorationg Framework  (DCEF) makes all of that better by providing a visual UI for common cleaning operations AND emitting python code that performs the transformation. Specifically, the DCEF is a tool built to interactively explore, clean, and transform pandas dataframes.
+# Buckaroo - The Data Wrangling Assistant
+We all know how awkward it is to clean data in jupyter notebooks.  Multiple cells of exploratory work, trying different transforms, looking up different transforms, adhoc functions that work in one notebook and have to be either copied/pasta-ed to the next notebook, or rewritten from scratch.  Buckaro makes all of that better by providing a visual UI for common cleaning operations AND emitting python code that performs the transformation. Specifically, the Buckaroo is a tool built to interactively explore, clean, and transform pandas dataframes.
 
-![Data Cleaning Exploration Framework Screenshot](static/images/dcf-jupyter.png)
+![Buckaroo Screenshot](static/images/dcf-jupyter.png)
 
 
 ## Installation
 
-If using JupyterLab, `dcef` requires JupyterLab version 3 or higher.
+If using JupyterLab, `buckaroo` requires JupyterLab version 3 or higher.
 
-You can install `dcef` using `pip`
+You can install `buckaroo` using `pip`
 
 Using `pip`:
 
 ```bash
-pip install dcef
+pip install buckaroo
 ```
 
 ## Documentation
 
-To get started with using DCEF, check out the full documentation:
+To get started with using Buckaroo, check out the full documentation:
 
-https://dcef.readthedocs.io/
+https://buckaroo.readthedocs.io/
 
 
-# Using DCEF
+# Using Buckaroo
 
 in a jupyter lab notebook just add the following to a cell
 
 ```python
-from dcef.dcef_widget import DCEFWidget
-DCEFWidget(df=df)  #df being the dataframe you want to explore
+from buckaroo.buckaroo_widget import BuckarooWidget
+BuckarooWidget(df=df)  #df being the dataframe you want to explore
 ``` 
-and you will see the UI for DCEF
+and you will see the UI for Buckaroo
 
 
 ## Using commands
 
-At the core DCEF commands operate on columns.  You must first click on a cell (not a header) in the top pane to select a column.
+At the core Buckaroo commands operate on columns.  You must first click on a cell (not a header) in the top pane to select a column.
 
 Next you must click on a command like `dropcol`, `fillna`, or `groupby` to create a new command
 
 After creating a new command, you will see that command in the commands list, now you must edit the details of a command.  Select the command by clicking on the bottom cell.
 
 At this point you can either delete the command by clicking the `X` button or change command parameters.
 
 ## Writing your own commands
 
-Builtin commands are found in [all_transforms.py](dcef/all_transforms.py)
+Builtin commands are found in [all_transforms.py](buckaroo/all_transforms.py)
 
 ### Simple example
 Here is a simple example command
 ```python
 class DropCol(Command):
     command_default = [s('dropcol'), s('df'), "col"]
     command_pattern = [None]
@@ -193,15 +193,15 @@
 These transforms emit multiple DataFrames
   * Relational extract (extract one or more columns into a second dataframe that can be joined back to a foreign key column)
   * Split on column (emit separate dataframes for each value of a categorical, no shape editting)
 * DataFrame combination
   * concat (concatenate multiple dataframes, with UI affordances to assure a similar shape)
   * join (join two dataframes on a key, with UI affordances)
 
-DCEF can only work on a single input dataframe shape at a time.  Any newly created columns are visible on output, but not available for manipulation in the same DCEF Cell.
+Buckaroo can only work on a single input dataframe shape at a time.  Any newly created columns are visible on output, but not available for manipulation in the same Buckaroo Cell.
 
 
 # Components
 * a rich table widget that is embeddable into applications and in the jupyter notebook.
 * A UI for selecting and trying transforms interactively
 * An output table widget showing the transformed dataframe
 
@@ -210,23 +210,23 @@
 
 ## Exists now
   * React frontend app
     * Displays a datatframe
 	* Simple UI for column level functions
 	* Shows generated python code
 	* Shows transformed data frame
-  * DCEF server
+  * Buckaroo server
     * Serves up dataframes for use by frontend
-	* responds to dcef commands
+	* responds to buckaroo commands
 	* shows generated python code
   * Developer User experience
-	* define DCEF commands in python onloy
-  * DCEF Intepreter
+	* define Buckaroo commands in python onloy
+  * Buckaroo Intepreter
     * Based on Peter Norvig's lispy.py, a simple syntax that is easy for the frontend to generate (no parens, just JSON arrays)
-  * DCEF core (actual transforms supported)
+  * Buckaroo core (actual transforms supported)
     * dropcol
 	* fillna
 	* one hot
 	* safe int
 	* GroupBy
 
 ## Next major features
@@ -238,15 +238,15 @@
     * Styling
 	  * Server only, some UI for DataFrame selection
     * Pre filtering concept (only operate on first 1000 rows, some sample of all rows)
 	* DataFrame joining UI
 	* Summary statistics tab for incoming dataframe
 	* Multi index columns
 	* DateTimeIndex support
-  * DCEF core
+  * Buckaroo core
 	* MakeCategorical
 	* Quantize
 	* Resample
 	* ManyColdDecoding
 	* IndexShift
 	* Computed
 	* Stack/Unstack
@@ -259,16 +259,16 @@
 
 
 ## Development installation
 
 For a development installation:
 
 ```bash
-git clone https://github.com/paddymul/dcef.git
-cd dcef
+git clone https://github.com/paddymul/buckaroo.git
+cd buckaroo
 conda install ipywidgets=8 jupyterlab
 pip install -ve .
 ```
 
 Enabling development install for Jupyter notebook:
```

