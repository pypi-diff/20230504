# Comparing `tmp/module_qc_nonelec_gui-0.0.2.tar.gz` & `tmp/module_qc_nonelec_gui-0.0.3.tar.gz`

## Comparing `module_qc_nonelec_gui-0.0.2.tar` & `module_qc_nonelec_gui-0.0.3.tar`

### file list

```diff
@@ -1,87 +1,143 @@
--rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/.gitlab-ci.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/.gitmodules
--rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/MANIFEST.in
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/tbump.toml
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/docs/Makefile
--rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/docs/conf.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/docs/index.rst
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/docs/make.bat
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/__init__.py
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/__main__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/py.typed
--rw-r--r--   0        0        0    73479 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/GUI/icon/ATLAS-Logo-BW-CMYK-LGBT-simple-transparent.png
--rw-r--r--   0        0        0   523993 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/GUI/icon/ATLAS-Logo-Blue-RGB-H_0.jpg
--rw-r--r--   0        0        0     3498 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/GUI/icon/Logo-Outline-web-Blue100.png
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/GUI/registration_bare_module/README.md
--rw-r--r--   0        0        0     7370 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/GUI/registration_bare_module/bareregist_main.py
--rw-r--r--   0        0        0    56779 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/GUI/registration_bare_module/img/assembledmodule.jpg
--rw-r--r--   0        0        0    33023 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/GUI/registration_bare_module/img/baremodule.jpg
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/cli/__init__.py
--rw-r--r--   0        0        0    36371 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/cli/main.py
--rw-r--r--   0        0        0     7054 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/configuration/configuration.json
--rw-r--r--   0        0        0     7386 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/configuration/configuration_triplet_r.json
--rw-r--r--   0        0        0     7386 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/configuration/configuration_triplet_s.json
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/dbinterface/README.md
--rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/dbinterface/bin/uploader_sample.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/dbinterface/data/sample_results.txt
--rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/qc_tests/flatness/flatness.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/qc_tests/flatness/example/example.json
--rw-r--r--   0        0        0     5053 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/qc_tests/glue_info_module_flex/Glue_info.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/qc_tests/glue_info_module_flex/README.md
--rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/qc_tests/ireftrim/IrefTrim.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/qc_tests/ivcurve/README.md
--rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/qc_tests/ivcurve/Sensor_IV.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/qc_tests/ivcurve/example/example.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/qc_tests/ivcurve/example/jsonschema/tmp
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/qc_tests/ivcurve/example/jsonschema/validation_schema.json
--rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/qc_tests/mass/MASS.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/qc_tests/mass/README.md
--rw-r--r--   0        0        0    14300 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/qc_tests/metrology/metrology_main.py
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/qc_tests/metrology/example/example.json
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/qc_tests/metrology/example/practice.txt
--rw-r--r--   0        0        0     2382 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/qc_tests/orientation/Orientation.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/qc_tests/orientation/README.md
--rw-r--r--   0        0        0     7481 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/qc_tests/parylene_properties/Parylene_prop.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/qc_tests/parylene_properties/README.md
--rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/qc_tests/pullup/Pullup.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/qc_tests/sldo_vi/README.md
--rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/qc_tests/sldo_vi/SLDO_VI.py
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/qc_tests/sldo_vi/example/example.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/qc_tests/sldo_vi/example/jsonschema/tmp
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/qc_tests/sldo_vi/example/jsonschema/validation_schema.json
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/qc_tests/thermal_cycling/README.md
--rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/qc_tests/thermal_cycling/Thermal.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/qc_tests/thermal_cycling/example/practice.txt
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/qc_tests/vi/README.md
--rw-r--r--   0        0        0    10437 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/qc_tests/vi/vi_main.py
--rw-r--r--   0        0        0     4262 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/qc_tests/vi/config/VI_Config_Module.json
--rw-r--r--   0        0        0     8934 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/qc_tests/vi/config/VI_Config_Module_MODULETOPCB.json
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/qc_tests/vi/config/config_MODULE_MODULE__ASSEMBLY.json
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/qc_tests/vi/config/config_MODULE_MODULE__PARYLENE_COATING.json
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/qc_tests/vi/config/config_MODULE_MODULE__PARYLENE_MASKING.json
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/qc_tests/vi/config/config_MODULE_MODULE__PARYLENE_UNMASKING.json
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/qc_tests/vi/config/config_MODULE_MODULE__THERMAL_CYCLES.json
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/qc_tests/vi/config/config_MODULE_MODULE__WIREBONDING.json
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/qc_tests/vi/config/config_MODULE_MODULE__WIREBOND_PROTECTION.json
--rw-r--r--   0        0        0     9592 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/qc_tests/vi/config/config_PCB.json
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/qc_tests/vi/config/reference_MODULE_MODULE__ASSEMBLY.json
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/qc_tests/vi/config/reference_MODULE_MODULE__PARYLENE_COATING.json
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/qc_tests/vi/config/reference_MODULE_MODULE__PARYLENE_MASKING.json
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/qc_tests/vi/config/reference_MODULE_MODULE__PARYLENE_UNMASKING.json
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/qc_tests/vi/config/reference_MODULE_MODULE__THERMAL_CYCLES.json
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/qc_tests/vi/config/reference_MODULE_MODULE__WIREBONDING.json
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/qc_tests/vi/config/reference_MODULE_MODULE__WIREBOND_PROTECTION.json
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/qc_tests/vi/config/reference_PCB.json
--rw-r--r--   0        0        0     8131 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/qc_tests/vi/functions/auto_trim.py
--rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/qc_tests/vi/functions/cv2_func.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/qc_tests/wirebonding_info/README.md
--rw-r--r--   0        0        0     5624 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/qc_tests/wirebonding_info/Wire_info.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/qc_tests/wirebonding_info/example/practice.txt
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/tests/test_package.py
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/.gitignore
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/LICENSE
--rw-r--r--   0        0        0     5534 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/README.md
--rw-r--r--   0        0        0     5526 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     9273 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/.gitlab-ci.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/.gitmodules
+-rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/MANIFEST.in
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/tbump.toml
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/docs/Makefile
+-rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/docs/conf.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/docs/index.rst
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/docs/make.bat
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/__init__.py
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/__main__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/_version.py
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/config_modifier.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/GUI/__init__.py
+-rw-r--r--   0        0        0    10407 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/GUI/choosetest_win.py
+-rw-r--r--   0        0        0     3336 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/GUI/componentinfo_win.py
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/GUI/connectdb_win.py
+-rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/GUI/connectpd_win.py
+-rw-r--r--   0        0        0     3710 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/GUI/continue_win.py
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/GUI/inputatlsn_win.py
+-rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/GUI/selectmode_win.py
+-rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/GUI/setup_win.py
+-rw-r--r--   0        0        0    73479 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/GUI/icon/ATLAS-Logo-BW-CMYK-LGBT-simple-transparent.png
+-rw-r--r--   0        0        0   523993 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/GUI/icon/ATLAS-Logo-Blue-RGB-H_0.jpg
+-rw-r--r--   0        0        0     3498 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/GUI/icon/Logo-Outline-web-Blue100.png
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/GUI/registration_bare_module/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/GUI/registration_bare_module/__init__.py
+-rw-r--r--   0        0        0     2825 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/GUI/registration_bare_module/bareinfo_win.py
+-rw-r--r--   0        0        0     7366 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/GUI/registration_bare_module/bareregist_main.py
+-rw-r--r--   0        0        0     4776 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/GUI/registration_bare_module/bareregist_win.py
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/GUI/registration_bare_module/connectpd_win.py
+-rw-r--r--   0        0        0     7189 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/GUI/registration_bare_module/feinfo_win.py
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/GUI/registration_bare_module/initial_win.py
+-rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/GUI/registration_bare_module/sensorinfo_win.py
+-rw-r--r--   0        0        0    56779 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/GUI/registration_bare_module/img/assembledmodule.jpg
+-rw-r--r--   0        0        0    33023 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/GUI/registration_bare_module/img/baremodule.jpg
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/cli/__init__.py
+-rw-r--r--   0        0        0    37314 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/cli/main.py
+-rw-r--r--   0        0        0     6752 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/configuration/config_default.json
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/configuration/config_quad.json
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/configuration/config_triplet_r.json
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/configuration/config_triplet_s.json
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/dbinterface/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/dbinterface/__init__.py
+-rw-r--r--   0        0        0     6658 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/dbinterface/db_write.py
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/dbinterface/localdb_authenticator.py
+-rw-r--r--   0        0        0     2538 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/dbinterface/localdb_retriever.py
+-rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/dbinterface/localdb_uploader.py
+-rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/dbinterface/upload_results_sample.py
+-rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/dbinterface/bin/uploader_sample.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/dbinterface/data/sample_results.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/FLATNESS/__init__.py
+-rw-r--r--   0        0        0     4208 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/FLATNESS/confirm.py
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/FLATNESS/main.py
+-rw-r--r--   0        0        0     4722 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/FLATNESS/user_input.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/FLATNESS/example/example.json
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/IV_MEASURE/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/IV_MEASURE/__init__.py
+-rw-r--r--   0        0        0     4076 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/IV_MEASURE/confirm.py
+-rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/IV_MEASURE/main.py
+-rw-r--r--   0        0        0     5411 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/IV_MEASURE/user_input.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/IV_MEASURE/example/example.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/IV_MEASURE/example/jsonschema/tmp
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/IV_MEASURE/example/jsonschema/validation_schema.json
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/MASS_MEASUREMENT/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/MASS_MEASUREMENT/__init__.py
+-rw-r--r--   0        0        0     2533 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/MASS_MEASUREMENT/confirm.py
+-rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/MASS_MEASUREMENT/main.py
+-rw-r--r--   0        0        0     5144 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/MASS_MEASUREMENT/user_input.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/QUAD_MODULE_METROLOGY/__init__.py
+-rw-r--r--   0        0        0     9917 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/QUAD_MODULE_METROLOGY/confirm.py
+-rw-r--r--   0        0        0     4629 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/QUAD_MODULE_METROLOGY/initial_metrology.py
+-rw-r--r--   0        0        0    14217 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/QUAD_MODULE_METROLOGY/main.py
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/QUAD_MODULE_METROLOGY/example/example.json
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/QUAD_MODULE_METROLOGY/example/practice.txt
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/THERMAL_CYCLING/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/THERMAL_CYCLING/__init__.py
+-rw-r--r--   0        0        0     5672 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/THERMAL_CYCLING/confirm.py
+-rw-r--r--   0        0        0     7902 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/THERMAL_CYCLING/initial_Thermal.py
+-rw-r--r--   0        0        0     5182 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/THERMAL_CYCLING/main.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/THERMAL_CYCLING/example/practice.txt
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/__init__.py
+-rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/checklist.py
+-rw-r--r--   0        0        0    35521 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/checklist_Module.py
+-rw-r--r--   0        0        0    81382 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/checklist_PCB.py
+-rw-r--r--   0        0        0     7122 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/confirm.py
+-rw-r--r--   0        0        0    18040 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/inspection_win.py
+-rw-r--r--   0        0        0    12310 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/main.py
+-rw-r--r--   0        0        0    26703 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/shaping_win.py
+-rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/splitimg_win.py
+-rw-r--r--   0        0        0     4807 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/summary_win.py
+-rw-r--r--   0        0        0     4083 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/vi_initial_win.py
+-rw-r--r--   0        0        0     4262 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/VI_Config_Module.json
+-rw-r--r--   0        0        0     8934 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/VI_Config_Module_MODULETOPCB.json
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/config_MODULE_MODULE__ASSEMBLY.json
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/config_MODULE_MODULE__PARYLENE_COATING.json
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/config_MODULE_MODULE__PARYLENE_MASKING.json
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/config_MODULE_MODULE__PARYLENE_UNMASKING.json
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/config_MODULE_MODULE__THERMAL_CYCLES.json
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/config_MODULE_MODULE__WIREBONDING.json
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/config_MODULE_MODULE__WIREBOND_PROTECTION.json
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/config_MODULE_default.json
+-rw-r--r--   0        0        0     9592 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/config_PCB.json
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/config_PCB_PCB_RECEPTION.json
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/config_PCB_default.json
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/reference_MODULE_MODULE__ASSEMBLY.json
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/reference_MODULE_MODULE__PARYLENE_COATING.json
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/reference_MODULE_MODULE__PARYLENE_MASKING.json
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/reference_MODULE_MODULE__PARYLENE_UNMASKING.json
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/reference_MODULE_MODULE__THERMAL_CYCLES.json
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/reference_MODULE_MODULE__WIREBONDING.json
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/reference_MODULE_MODULE__WIREBOND_PROTECTION.json
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/reference_PCB.json
+-rw-r--r--   0        0        0     8131 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/functions/auto_trim.py
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/functions/cv2_func.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/WIREBOND_PULL_TEST/README.md
+-rw-r--r--   0        0        0     3651 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/WIREBOND_PULL_TEST/confirm.py
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/WIREBOND_PULL_TEST/main.py
+-rw-r--r--   0        0        0     8647 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/WIREBOND_PULL_TEST/user_input.py
+-rw-r--r--   0        0        0     5049 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/glue_info_module_flex/Glue_info.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/glue_info_module_flex/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/glue_info_module_flex/__init__.py
+-rw-r--r--   0        0        0     5610 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/glue_info_module_flex/confirm.py
+-rw-r--r--   0        0        0     8120 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/glue_info_module_flex/initial_Glue_info.py
+-rw-r--r--   0        0        0     7477 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/parylene_properties/Parylene_prop.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/parylene_properties/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/parylene_properties/__init__.py
+-rw-r--r--   0        0        0     6090 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/parylene_properties/confirm.py
+-rw-r--r--   0        0        0     9292 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/parylene_properties/initial_Parylene_prop.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/wirebonding_info/README.md
+-rw-r--r--   0        0        0     5616 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/wirebonding_info/Wire_info.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/wirebonding_info/__init__.py
+-rw-r--r--   0        0        0     5553 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/wirebonding_info/confirm.py
+-rw-r--r--   0        0        0     9613 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/wirebonding_info/initial_Wire_info.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/wirebonding_info/example/practice.txt
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/tests/test_package.py
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/LICENSE
+-rw-r--r--   0        0        0     5534 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/README.md
+-rw-r--r--   0        0        0     5526 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     9273 2020-02-02 00:00:00.000000 module_qc_nonelec_gui-0.0.3/PKG-INFO
```

### Comparing `module_qc_nonelec_gui-0.0.2/.gitlab-ci.yml` & `module_qc_nonelec_gui-0.0.3/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.2/.pre-commit-config.yaml` & `module_qc_nonelec_gui-0.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.2/tbump.toml` & `module_qc_nonelec_gui-0.0.3/tbump.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 00000000: 5b76 6572 7369 6f6e 5d0a 6375 7272 656e  [version].curren
-00000010: 7420 3d20 2230 2e30 2e32 220a 0a23 2045  t = "0.0.2"..# E
+00000010: 7420 3d20 2230 2e30 2e33 220a 0a23 2045  t = "0.0.3"..# E
 00000020: 7861 6d70 6c65 206f 6620 6120 7365 6d76  xample of a semv
 00000030: 6572 2072 6567 6578 702e 0a23 204d 616b  er regexp..# Mak
 00000040: 6520 7375 7265 2074 6869 7320 6d61 7463  e sure this matc
 00000050: 6865 7320 6375 7272 656e 745f 7665 7273  hes current_vers
 00000060: 696f 6e20 6265 666f 7265 0a23 2075 7369  ion before.# usi
 00000070: 6e67 2074 6275 6d70 0a72 6567 6578 203d  ng tbump.regex =
 00000080: 2027 2727 0a20 2028 3f50 3c6d 616a 6f72   '''.  (?P<major
@@ -15,15 +15,15 @@
 000000e0: 2029 3f0a 2020 2727 270a 0a5b 6769 745d   )?.  '''..[git]
 000000f0: 0a23 2054 6865 2063 7572 7265 6e74 2076  .# The current v
 00000100: 6572 7369 6f6e 2077 696c 6c20 6765 7420  ersion will get 
 00000110: 7570 6461 7465 6420 7768 656e 2074 6275  updated when tbu
 00000120: 6d70 2069 7320 7275 6e0a 6d65 7373 6167  mp is run.messag
 00000130: 655f 7465 6d70 6c61 7465 203d 2022 4275  e_template = "Bu
 00000140: 6d70 2076 6572 7369 6f6e 3a20 302e 302e  mp version: 0.0.
-00000150: 3220 e286 9220 7b6e 6577 5f76 6572 7369  2 ... {new_versi
+00000150: 3320 e286 9220 7b6e 6577 5f76 6572 7369  3 ... {new_versi
 00000160: 6f6e 7d22 0a74 6167 5f74 656d 706c 6174  on}".tag_templat
 00000170: 6520 3d20 2276 7b6e 6577 5f76 6572 7369  e = "v{new_versi
 00000180: 6f6e 7d22 0a0a 2320 466f 7220 6561 6368  on}"..# For each
 00000190: 2066 696c 6520 746f 2070 6174 6368 2c20   file to patch, 
 000001a0: 6164 6420 6120 5b5b 6669 6c65 5d5d 2063  add a [[file]] c
 000001b0: 6f6e 6669 670a 2320 7365 6374 696f 6e20  onfig.# section 
 000001c0: 636f 6e74 6169 6e69 6e67 2074 6865 2070  containing the p
```

### Comparing `module_qc_nonelec_gui-0.0.2/docs/Makefile` & `module_qc_nonelec_gui-0.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.2/docs/conf.py` & `module_qc_nonelec_gui-0.0.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.2/docs/make.bat` & `module_qc_nonelec_gui-0.0.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/__main__.py` & `module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
 import sys
 
 import typer
 from PyQt5.QtWidgets import QApplication
 
+from module_qc_nonelec_gui import config_modifier
 from module_qc_nonelec_gui.cli import MainWindow
-from module_qc_nonelec_gui.lib import config_modifier
 
 
 def main():
     typer.echo("Launching GUI")
     app = QApplication(sys.argv[1:])
     main_window = MainWindow()
     main_window.show()
```

### Comparing `module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/GUI/icon/ATLAS-Logo-BW-CMYK-LGBT-simple-transparent.png` & `module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/GUI/icon/ATLAS-Logo-BW-CMYK-LGBT-simple-transparent.png`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/GUI/icon/ATLAS-Logo-Blue-RGB-H_0.jpg` & `module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/GUI/icon/ATLAS-Logo-Blue-RGB-H_0.jpg`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/GUI/icon/Logo-Outline-web-Blue100.png` & `module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/GUI/icon/Logo-Outline-web-Blue100.png`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/GUI/registration_bare_module/bareregist_main.py` & `module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/GUI/registration_bare_module/bareregist_main.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import logging
 import sys
 
 import itkdb
 from PyQt5.QtWidgets import QApplication, QMainWindow
 
-from module_qc_nonelec_gui.GUI.registration_bare_module.lib import (
+from module_qc_nonelec_gui.GUI.registration_bare_module import (
     bareinfo_win,
     bareregist_win,
     connectpd_win,
     feinfo_win,
     initial_win,
     sensorinfo_win,
 )
```

### Comparing `module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/GUI/registration_bare_module/img/assembledmodule.jpg` & `module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/GUI/registration_bare_module/img/assembledmodule.jpg`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/GUI/registration_bare_module/img/baremodule.jpg` & `module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/GUI/registration_bare_module/img/baremodule.jpg`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/cli/main.py` & `module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/cli/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import contextlib
 import json
 import logging
 import os
 import pprint
 import sys
 import traceback
 from datetime import date, datetime, timezone
@@ -25,26 +26,27 @@
     QPushButton,
     QScrollArea,
     QStatusBar,
     QVBoxLayout,
     QWidget,
 )
 
-from module_qc_nonelec_gui.dbinterface.lib import (
+from module_qc_nonelec_gui.dbinterface import (
     localdb_authenticator,
     localdb_retriever,
 )
-from module_qc_nonelec_gui.GUI.lib import (
+from module_qc_nonelec_gui.GUI import (
     choosetest_win,
     componentinfo_win,
     connectdb_win,
     connectpd_win,
     continue_win,
     inputatlsn_win,
     selectmode_win,
+    setup_win,
 )
 from module_qc_nonelec_gui.GUI.registration_bare_module import bareregist_main
 
 logging.basicConfig(stream=sys.stdout, level=logging.INFO)
 log = logging.getLogger(__name__)
 
 
@@ -87,25 +89,50 @@
 
         self.atlsn = ""
         self.db_user = None
         self.db_pass = None
 
         self.supportedComponentTypes = ["MODULE", "BARE_MODULE", "PCB"]
 
-        # configuration1
-        with Path(
-            self.module_qc_nonelec_gui_dir + "/configuration/configuration.json"
-        ).open() as f1:
-            self.configuration = json.load(f1)
+        self.make_statusbar()
+        self.update_statusbar(self)
 
         self.init_ui()
 
     def init_ui(self):
-        self.make_statusbar()
-        self.update_statusbar(self)
+        # configuration1
+        try:
+            log.info("loading custom json file...")
+            with Path(
+                self.module_qc_nonelec_gui_dir + "/configuration/custom.json"
+            ).open() as f:
+                self.custom_conf = json.load(f)
+
+            log.info("loaded custom json file:")
+            log.info(pprint.pformat(self.custom_conf))
+
+        except Exception as e:
+            log.error(e)
+            self.close()
+            wid = setup_win.SetupWindow(self)
+            self.update_widget(wid)
+            return
+
+        try:
+            with Path(
+                self.module_qc_nonelec_gui_dir + "/configuration/config_default.json"
+            ).open() as f1:
+                self.default_conf = json.load(f1)
+
+        except Exception as e:
+            log.error(e)
+            pass
+
+        self.config = self.default_conf
+
         if self.isSameComponent:
             self.fill_info()
 
         else:
             wid = selectmode_win.SelectmodeWindow(self)
             self.update_widget(wid)
             log.info(
@@ -227,48 +254,55 @@
 
     def get_component_info(self):
         self.component = self.localDB.component.find_one({"serialNumber": self.atlsn})
 
         componentType = self.component["componentType"]
         cptCfgFile = ""
 
+        self.fill_info()
+
         if componentType == "module":
             # triplet stave
             if any((tok in self.atlsn) for tok in ["MS", "R6", "R3"]):
                 log.exception(self.atlsn + ": triplet stave module")
-                cptCfgFile = "configuration.json"
+                cptCfgFile = "config_triplet_s.json"
 
             # triplet ring
             elif any(
                 (tok in self.atlsn) for tok in ["M0", "M5", "R7", "R8", "R4", "R5"]
             ):
                 log.info(self.atlsn + ": triplet ring module")
-                cptCfgFile = "configuration.json"
+                cptCfgFile = "config_triplet_r.json"
 
             # quad
             else:
                 log.info(self.atlsn + ": quad module")
-                cptCfgFile = "configuration.json"
+                cptCfgFile = "config_quad.json"
 
         # bare_module
         elif componentType == "bare_module":
             log.info(self.atlsn + ": bare_module")
-            cptCfgFile = "configuration.json"
+            cptCfgFile = "config_quad.json"
 
         # pcb
         elif componentType == "module_pcb":
             log.info(self.atlsn + ": pcb")
-            cptCfgFile = "configuration.json"
+            cptCfgFile = "config_quad.json"
 
         with Path(self.module_qc_nonelec_gui_dir).joinpath(
             "configuration", cptCfgFile
         ).open() as f:
-            self.configuration = json.load(f)
+            self.override_conf = json.load(f)
 
-        self.fill_info()
+        self.config = self.default_conf
+
+        for code, obj in self.override_conf[self.info_dict.get("componentType")][
+            "test"
+        ].items():
+            self.config[self.info_dict.get("componentType")]["test"][code] = obj
 
     def fill_info(self):
         try:
             self.cptTypeMap
         except Exception:
             self.cptTypeMap = {
                 "module": "MODULE",
@@ -285,19 +319,21 @@
                 {"code": self.cptTypeMap.get(self.component["componentType"])}
             )
 
             self.info_dict["component"] = self.atlsn
             self.info_dict["componentType"] = self.cptTypeMap.get(
                 self.component["componentType"]
             )
-            self.info_dict["FE_version"] = [
-                d.get("value")
-                for d in self.component["properties"]
-                if d.get("code") == "FECHIP_VERSION"
-            ][0]
+            with contextlib.suppress(Exception):
+                self.info_dict["FE_version"] = [
+                    d.get("value")
+                    for d in self.component["properties"]
+                    if d.get("code") == "FECHIP_VERSION"
+                ][0]
+
             self.info_dict["date"] = datetime.now(timezone.utc)
             self.info_dict["sys"] = {
                 "cts": datetime.now(timezone.utc),
                 "mts": datetime.now(timezone.utc),
                 "rev": 0,
             }
 
@@ -425,16 +461,16 @@
         self.start_QCupload()
 
     def receive_db_user(self, username, password):
         self.db_user = username
         self.db_pass = password
 
         self.localDB, self.localDBtools = localdb_authenticator.connectDB(
-            self.configuration["mongoDB"]["address"],
-            self.configuration["mongoDB"]["port"],
+            self.custom_conf["mongoDB"]["address"],
+            self.custom_conf["mongoDB"]["port"],
         )
 
         self.info_dict["user"] = self.db_user
         self.db_pass = None
 
         self.component_list = [
             c["serialNumber"] for c in self.localDB.component.find({})
@@ -534,17 +570,17 @@
     def receive_testtype(self, testtype):
         self.info_dict["testType"] = testtype
 
         self.call_targetGUI()
 
     def call_targetGUI(self):
         try:
-            cptType = self.info_dict["componentType"]
-            cptCfgTests = self.configuration["QC_item"][cptType]["test"]
-            testType = self.info_dict["testType"]
+            cptType = self.info_dict.get("componentType")
+            cptCfgTests = self.config.get(cptType).get("test")
+            testType = self.info_dict.get("testType")
 
             log.debug("cptType: " + cptType)
             log.debug("cptCfgTests: " + pprint.pformat(cptCfgTests))
             log.debug("testType: " + testType)
 
             self.testRunFormat = self.localDBtools.QC.tests.find_one(
                 {
@@ -572,29 +608,29 @@
             self.testRun.get("results").update(
                 {param["code"]: None for param in self.testRunFormat["parameters"]}
             )
 
             log.debug("testRunFormat: " + pprint.pformat(self.testRunFormat))
             log.debug("testRun skeleton: " + pprint.pformat(self.testRun))
 
-            test = next(filter(lambda t: t["code"] == testType, cptCfgTests))
+            test = cptCfgTests.get(testType)
 
             log.debug("identified test: " + pprint.pformat(test))
 
             testGUI_path = str(Path(self.module_qc_nonelec_gui_dir) / test["path"])
 
             log.debug("testGUI_path: " + testGUI_path)
 
             self.test_module = machinery.SourceFileLoader(
                 testType, testGUI_path
             ).load_module()
 
             try:
                 module_property_list = []
-                for property_i in self.configuration["QC_item"][cptType]["property"]:
+                for _code, property_i in self.config[cptType]["property"].items():
                     module_property_list.append(property_i["code"])
                 if self.info_dict["testType"] in module_property_list:
                     self.isProperty = True
                 else:
                     self.isProperty = False
 
                 self.test_win = self.test_module.TestWindow(self)
@@ -647,20 +683,18 @@
         log.info("==========================================================")
         log.info("confirm_result(): [results]")
         log.info(pprint.pformat(self.testRun))
         log.info("==========================================================")
 
         try:
             cptType = self.info_dict.get("componentType")
-            cptCfgTests = self.configuration.get("QC_item").get(cptType).get("test")
+            cptCfgTests = self.config.get(cptType).get("test")
             testType = self.info_dict.get("testType")
 
-            test_confirm = next(
-                filter(lambda t: t.get("code") == testType, cptCfgTests)
-            ).get("confirm_path")
+            test_confirm = cptCfgTests.get(testType).get("confirm_path")
 
             log.info(f"test_confirm = {test_confirm}")
 
             test_confirm = str(Path(self.module_qc_nonelec_gui_dir) / test_confirm)
             log.info(f"test_confirm = {test_confirm}")
 
             self.confirm_module = machinery.SourceFileLoader(
@@ -732,14 +766,16 @@
         inner.setWidget(result_wid)
 
         layout.addLayout(titlebox)
         layout.addWidget(inner)
         layout.addLayout(button_box)
         sub.setLayout(layout)
 
+        self.update_widget(result_wid)
+
     def confirm_layout_common(self, sub):
         Form_layout = QFormLayout()
         sub.add_info(Form_layout, "Serial Number :", self.info_dict["component"])
         sub.add_info(Form_layout, "Component Type :", self.info_dict["componentType"])
         sub.add_info(
             Form_layout,
             "Current Stage :",
@@ -778,24 +814,26 @@
 
     def upload_to_db(self):
         if self.isPractice:
             self.terminate_message()
         else:
             if self.isOK_to_upload:
                 try:
-                    self.output_result()
+                    self.local_save()
+
+                    host = self.custom_conf.get("localDB_web").get("address")
+                    port = self.custom_conf.get("localDB_web").get("port")
 
-                    host = self.configuration.get("localDB_web").get("address")
-                    port = self.configuration.get("localDB_web").get("port")
+                    protocol = "http" if port == 80 else "https"
 
                     log.info(
-                        f"attempting to upload TestRun to LocalDB on http://{host}:{port}/localdb/ ..."
+                        f"attempting to upload TestRun to LocalDB on {protocol}://{host}:{port}/localdb/ ..."
                     )
                     res = requests.post(
-                        f"http://{host}:{port}/localdb/qc_uploader_post",
+                        f"{protocol}://{host}:{port}/localdb/qc_uploader_post",
                         json=[[self.testRun]],
                     )
                     log.info("... posted! response = " + str(res.text))
                     out = json.loads(str(res.text))
                     log.info(pprint.pformat(out))
                     self.terminate_message(str(res.text))
 
@@ -813,15 +851,15 @@
                 QMessageBox.warning(
                     None,
                     "Warning",
                     "you can not have prepared to upload",
                     QMessageBox.Ok,
                 )
 
-    def output_result(self):
+    def local_save(self):
         try:
             file_name = (
                 "_".join(
                     [
                         self.info_dict["component"],
                         self.info_dict["currentStage"].replace("/", "__"),
                         self.info_dict["testType"],
@@ -943,18 +981,18 @@
         log.info("Finish QCHelper :" + str(self.close()))
         log.info("---------------------------------------------------------------\n")
 
     def fill_practice_testtype_dict(self):
         self.test_dict.setdefault("practice", {})
         cptType = self.info_dict["componentType"]
 
-        for i in self.configuration["QC_item"][cptType]:
+        for i in self.config[cptType]:
             for test_i in [
                 (d.get("name"), d.get("code"), d.get("path"))
-                for d in self.configuration["QC_item"][cptType][i]
+                for d in self.config[cptType][i]
                 if d.get("supported")
             ]:
                 name = test_i[0]
                 code = test_i[1]
                 if test_i[2] == "":
                     name = name + "(TBA)"
                 self.test_dict["practice"][name] = code
@@ -965,24 +1003,24 @@
 
         self.test_dict[stage] = {}
 
         for test_code in self.qcStages["stage_test"][stage]:
             try:
                 log.info(test_code)
 
-                supported_tests = self.configuration["QC_item"][cptType]["test"]
+                supported_tests = self.config[cptType]["test"]
 
-                for config_i in supported_tests:
-                    if config_i["path"] == "":
-                        name = config_i["name"] + "(TBA)"
+                for _code, testCfg in supported_tests.items():
+                    if testCfg["path"] == "":
+                        name = testCfg["name"] + "(TBA)"
                     else:
-                        name = config_i["name"]
-                    if config_i["supported"] and (test_code in config_i["ITkPDcode"]):
-                        self.test_dict[stage][name] = config_i["code"]
-                        log.info(f'--> added test {config_i["code"]}')
+                        name = testCfg["name"]
+                    if testCfg["supported"] and (test_code in testCfg["ITkPDcode"]):
+                        self.test_dict[stage][name] = testCfg["code"]
+                        log.info(f'--> added test {testCfg["code"]}')
 
             except Exception as e:
                 log.info(pprint.pformat(e))
                 log.info(traceback.format_exc())
                 pass
 
         log.info(pprint.pformat(self.test_dict))
```

### Comparing `module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/configuration/configuration.json` & `module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/configuration/config_default.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Differences: {'replace': "OrderedDict([('MODULE', OrderedDict([('test', OrderedDict([('MASS_MEASUREMENT', "*

 * *            "OrderedDict([('code', 'MASS_MEASUREMENT'), ('name', 'Mass Measurement'), ('path', "*

 * *            "'qc_tests/MASS_MEASUREMENT/main.py'), ('confirm_path', "*

 * *            "'qc_tests/MASS_MEASUREMENT/confirm.py'), ('supported', False), ('ITkPDcode', "*

 * *            "['MASS_MEASUREMENT'])])), ('GLUE_MODULE_FLEX_ATTACH', OrderedDict([('code', "*

 * *            "'GLUE_MODULE_FLEX_ATTACH'), ('name', 'Glue Information […]*

```diff
@@ -1,279 +1,257 @@
 {
-    "QC_item": {
-        "BARE_MODULE": {
-            "property": [
-                {
-                    "ITkPDcode": [
-                        "MASS_MEASUREMENT"
-                    ],
-                    "code": "MASS_MEASUREMENT",
-                    "confirm_path": "qc_tests/mass/lib/confirm.py",
-                    "name": "Mass Measurement",
-                    "path": "qc_tests/mass/MASS.py",
-                    "supported": true
-                }
-            ],
-            "test": [
-                {
-                    "ITkPDcode": [
-                        "MASS_MEASUREMENT"
-                    ],
-                    "code": "MASS_MEASUREMENT",
-                    "confirm_path": "qc_tests/mass/lib/confirm.py",
-                    "name": "Mass Measurement",
-                    "path": "qc_tests/mass/MASS.py",
-                    "supported": true
-                },
-                {
-                    "ITkPDcode": [
-                        "OPTICAL_INSPECTION"
-                    ],
-                    "code": "OPTICAL_INSPECTION",
-                    "confirm_path": "qc_tests/vi/lib/confirm.py",
-                    "name": "Optical Inspection",
-                    "path": "qc_tests/vi/vi_main.py",
-                    "supported": true
-                },
-                {
-                    "ITkPDcode": [
-                        "BARE_MODULE_METROLOGY"
-                    ],
-                    "code": "BARE_MODULE_METROLOGY",
-                    "confirm_path": "qc_tests/metrology/lib/confirm.py",
-                    "name": "Bare Module Metrology",
-                    "path": "qc_tests/metrology/metrology_main.py",
-                    "supported": true
-                },
-                {
-                    "ITkPDcode": [
-                        "SENSOR_IV"
-                    ],
-                    "code": "SENSOR_IV",
-                    "confirm_path": "qc_tests/ivcurve/lib/confirm.py",
-                    "name": "Sensor IV",
-                    "path": "qc_tests/ivcurve/Sensor_IV.py",
-                    "supported": true
-                }
-            ]
+    "BARE_MODULE": {
+        "property": {
+            "MASS_MEASUREMENT": {
+                "ITkPDcode": [
+                    "MASS_MEASUREMENT"
+                ],
+                "code": "MASS_MEASUREMENT",
+                "confirm_path": "qc_tests/mass/confirm.py",
+                "name": "Mass Measurement",
+                "path": "qc_tests/mass/MASS.py",
+                "supported": false
+            }
         },
-        "MODULE": {
-            "property": [
-                {
-                    "ITkPDcode": [
-                        "RD53A_PULL-UP_RESISTOR1",
-                        "RD53A_PULL-UP_RESISTOR2",
-                        "RD53A_PULL-UP_RESISTOR3",
-                        "RD53A_PULL-UP_RESISTOR4"
-                    ],
-                    "code": "RD53A_PULL-UP_RESISTOR",
-                    "confirm_path": "qc_tests/pullup/lib/confirm.py",
-                    "exception": {},
-                    "name": "RD53A pull-up resistor FE",
-                    "path": "qc_tests/pullup/Pullup.py",
-                    "stage": [
-                        "MODULEWIREBONDING"
-                    ],
-                    "supported": true
-                },
-                {
-                    "ITkPDcode": [
-                        "IREFTRIM_FE1",
-                        "IREFTRIM_FE2",
-                        "IREFTRIM_FE3",
-                        "IREFTRIM_FE4"
-                    ],
-                    "code": "IREFTRIM_FE",
-                    "confirm_path": "qc_tests/ireftrim/lib/confirm.py",
-                    "exception": {},
-                    "name": "IrefTrim FE",
-                    "path": "qc_tests/ireftrim/IrefTrim.py",
-                    "stage": [
-                        "MODULEWIREBONDING"
-                    ],
-                    "supported": true
-                },
-                {
-                    "ITkPDcode": [
-                        "ORIENTATION"
-                    ],
-                    "code": "ORIENTATION",
-                    "confirm_path": "qc_tests/orientation/lib/confirm.py",
-                    "exception": {
-                        "chip_quantity": [
-                            0,
-                            1,
-                            2,
-                            3
-                        ]
-                    },
-                    "name": "PCB-Bare Orientation isNormal",
-                    "path": "qc_tests/orientation/Orientation.py",
-                    "stage": [
-                        "MODULEWIREBONDING"
-                    ],
-                    "supported": true
-                },
-                {
-                    "ITkPDcode": [
-                        "FECHIP_VERSION"
-                    ],
-                    "code": "FECHIP_VERSION",
-                    "confirm_path": "",
-                    "exception": {},
-                    "name": "FE chip version",
-                    "path": "",
-                    "stage": [],
-                    "supported": false
-                }
-            ],
-            "test": [
-                {
-                    "ITkPDcode": [
-                        "MASS_MEASUREMENT",
-                        "MASS"
-                    ],
-                    "code": "MASS_MEASUREMENT",
-                    "confirm_path": "qc_tests/mass/lib/confirm.py",
-                    "name": "Mass Measurement",
-                    "path": "qc_tests/mass/MASS.py",
-                    "supported": true
-                },
-                {
-                    "ITkPDcode": [
-                        "FLATNESS"
-                    ],
-                    "code": "FLATNESS",
-                    "confirm_path": "qc_tests/flatness/lib/confirm.py",
-                    "name": "Flatness",
-                    "path": "qc_tests/flatness/flatness.py",
-                    "supported": true
-                },
-                {
-                    "ITkPDcode": [
-                        "WIREBOND"
-                    ],
-                    "code": "WIREBOND",
-                    "confirm_path": "qc_tests/wirebond_pull/lib/confirm.py",
-                    "name": "Wirebond pull tests",
-                    "path": "qc_tests/wirebond_pull/Wire_pull.py",
-                    "supported": true
-                },
-                {
-                    "ITkPDcode": [
-                        "WIREBONDING"
-                    ],
-                    "code": "WIREBONDING",
-                    "confirm_path": "qc_tests/wirebonding_info/lib/confirm.py",
-                    "name": "Wirebonding Information",
-                    "path": "qc_tests/wirebonding_info/Wire_info.py",
-                    "supported": true
-                },
-                {
-                    "ITkPDcode": [
-                        "POTTING"
-                    ],
-                    "code": "POTTING",
-                    "confirm_path": "",
-                    "name": "Glue Information Potting",
-                    "path": "",
-                    "supported": false
-                },
-                {
-                    "ITkPDcode": [
-                        "PARYLENE"
-                    ],
-                    "code": "PARYLENE",
-                    "confirm_path": "qc_tests/parylene_properties/lib/confirm.py",
-                    "name": "Parylene Properties",
-                    "path": "qc_tests/parylene_properties/Parylene_prop.py",
-                    "supported": true
-                },
-                {
-                    "ITkPDcode": [
-                        "GLUE_MODULE_FLEX_ATTACH"
-                    ],
-                    "code": "GLUE_MODULE_FLEX_ATTACH",
-                    "confirm_path": "qc_tests/glue_info_module_flex/lib/confirm.py",
-                    "name": "Glue Information Module+Flex Attach",
-                    "path": "qc_tests/glue_info_module_flex/Glue_info.py",
-                    "supported": false
-                },
-                {
-                    "ITkPDcode": [
-                        "THERMAL_CYCLING"
-                    ],
-                    "code": "THERMAL_CYCLING",
-                    "confirm_path": "qc_tests/thermal_cycling/lib/confirm.py",
-                    "name": "Thermal Cycling",
-                    "path": "qc_tests/thermal_cycling/Thermal.py",
-                    "supported": true
-                },
-                {
-                    "ITkPDcode": [
-                        "OPTICAL",
-                        "VISUAL_INSPECTION"
-                    ],
-                    "code": "VISUAL_INSPECTION",
-                    "confirm_path": "qc_tests/vi/lib/confirm.py",
-                    "name": "Visual Inspection",
-                    "path": "qc_tests/vi/vi_main.py",
-                    "supported": true
-                },
-                {
-                    "ITkPDcode": [
-                        "METROLOGY_QUAD",
-                        "QUAD_MODULE_METROLOGY"
-                    ],
-                    "code": "QUAD_MODULE_METROLOGY",
-                    "confirm_path": "qc_tests/metrology/lib/confirm.py",
-                    "name": "Metrology",
-                    "path": "qc_tests/metrology/metrology_main.py",
-                    "supported": true
-                },
-                {
-                    "ITkPDcode": [
-                        "SENSOR_IV"
-                    ],
-                    "code": "SENSOR_IV",
-                    "confirm_path": "qc_tests/ivcurve/lib/confirm.py",
-                    "name": "Sensor IV",
-                    "path": "qc_tests/ivcurve/Sensor_IV.py",
-                    "supported": true
-                },
-                {
-                    "ITkPDcode": [
-                        "WP_ENVELOPE"
-                    ],
-                    "code": "WP_ENVELOPE",
-                    "confirm_path": "./qc_tests/roof_envelope/lib/confirm.py",
-                    "name": "Wire bonding roof envelope",
-                    "path": "./qc_tests/roof_envelope/roof_envelope.py",
-                    "supported": true
-                }
-            ]
-        },
-        "PCB": {
-            "property": [],
-            "test": [
-                {
-                    "ITkPDcode": [
-                        "METROLOGY"
-                    ],
-                    "code": "METROLOGY",
-                    "confirm_path": "qc_tests/metrology/lib/confirm.py",
-                    "name": "Metrology",
-                    "path": "qc_tests/metrology/metrology_main.py",
-                    "supported": true
-                }
-            ]
+        "test": {
+            "BARE_MODULE_METROLOGY": {
+                "ITkPDcode": [
+                    "BARE_MODULE_METROLOGY"
+                ],
+                "code": "BARE_MODULE_METROLOGY",
+                "confirm_path": "qc_tests/metrology/confirm.py",
+                "name": "Bare Module Metrology",
+                "path": "qc_tests/metrology/metrology_main.py",
+                "supported": false
+            },
+            "MASS_MEASUREMENT": {
+                "ITkPDcode": [
+                    "MASS_MEASUREMENT"
+                ],
+                "code": "MASS_MEASUREMENT",
+                "confirm_path": "qc_tests/mass/confirm.py",
+                "name": "Mass Measurement",
+                "path": "qc_tests/mass/MASS.py",
+                "supported": false
+            },
+            "OPTICAL_INSPECTION": {
+                "ITkPDcode": [
+                    "OPTICAL_INSPECTION"
+                ],
+                "code": "OPTICAL_INSPECTION",
+                "confirm_path": "qc_tests/vi/confirm.py",
+                "name": "Optical Inspection",
+                "path": "qc_tests/vi/vi_main.py",
+                "supported": false
+            }
         }
     },
-    "localDB_web": {
-        "address": "127.0.0.1",
-        "port": "5010"
+    "MODULE": {
+        "property": {
+            "FECHIP_VERSION": {
+                "ITkPDcode": [
+                    "FECHIP_VERSION"
+                ],
+                "code": "FECHIP_VERSION",
+                "confirm_path": "",
+                "exception": {},
+                "name": "FE chip version",
+                "path": "",
+                "stage": [],
+                "supported": false
+            },
+            "IREFTRIM_FE": {
+                "ITkPDcode": [
+                    "IREFTRIM_FE1",
+                    "IREFTRIM_FE2",
+                    "IREFTRIM_FE3",
+                    "IREFTRIM_FE4"
+                ],
+                "code": "IREFTRIM_FE",
+                "confirm_path": "qc_tests/ireftrim/confirm.py",
+                "exception": {},
+                "name": "IrefTrim FE",
+                "path": "qc_tests/ireftrim/IrefTrim.py",
+                "stage": [
+                    "MODULEWIREBONDING"
+                ],
+                "supported": false
+            },
+            "ORIENTATION": {
+                "ITkPDcode": [
+                    "ORIENTATION"
+                ],
+                "code": "ORIENTATION",
+                "confirm_path": "qc_tests/orientation/confirm.py",
+                "exception": {
+                    "chip_quantity": [
+                        0,
+                        1,
+                        2,
+                        3
+                    ]
+                },
+                "name": "PCB-Bare Orientation isNormal",
+                "path": "qc_tests/orientation/Orientation.py",
+                "stage": [
+                    "MODULEWIREBONDING"
+                ],
+                "supported": false
+            },
+            "RD53A_PULL-UP_RESISTOR": {
+                "ITkPDcode": [
+                    "RD53A_PULL-UP_RESISTOR1",
+                    "RD53A_PULL-UP_RESISTOR2",
+                    "RD53A_PULL-UP_RESISTOR3",
+                    "RD53A_PULL-UP_RESISTOR4"
+                ],
+                "code": "RD53A_PULL-UP_RESISTOR",
+                "confirm_path": "qc_tests/pullup/confirm.py",
+                "exception": {},
+                "name": "RD53A pull-up resistor FE",
+                "path": "qc_tests/pullup/Pullup.py",
+                "stage": [
+                    "MODULEWIREBONDING"
+                ],
+                "supported": false
+            }
+        },
+        "test": {
+            "FLATNESS": {
+                "ITkPDcode": [
+                    "FLATNESS"
+                ],
+                "code": "FLATNESS",
+                "confirm_path": "qc_tests/FLATNESS/confirm.py",
+                "name": "Flatness",
+                "path": "qc_tests/FLATNESS/main.py",
+                "supported": true
+            },
+            "GLUE_MODULE_FLEX_ATTACH": {
+                "ITkPDcode": [
+                    "GLUE_MODULE_FLEX_ATTACH"
+                ],
+                "code": "GLUE_MODULE_FLEX_ATTACH",
+                "confirm_path": "qc_tests/glue_info_module_flex/confirm.py",
+                "name": "Glue Information Module+Flex Attach",
+                "path": "qc_tests/glue_info_module_flex/Glue_info.py",
+                "supported": false
+            },
+            "IV_MEASURE": {
+                "ITkPDcode": [
+                    "IV_MEASURE"
+                ],
+                "code": "IV_MEASURE",
+                "confirm_path": "qc_tests/IV_MEASURE/confirm.py",
+                "name": "IV measurement",
+                "path": "qc_tests/IV_MEASURE/main.py",
+                "supported": true
+            },
+            "MASS_MEASUREMENT": {
+                "ITkPDcode": [
+                    "MASS_MEASUREMENT"
+                ],
+                "code": "MASS_MEASUREMENT",
+                "confirm_path": "qc_tests/MASS_MEASUREMENT/confirm.py",
+                "name": "Mass Measurement",
+                "path": "qc_tests/MASS_MEASUREMENT/main.py",
+                "supported": false
+            },
+            "PARYLENE": {
+                "ITkPDcode": [
+                    "PARYLENE"
+                ],
+                "code": "PARYLENE",
+                "confirm_path": "qc_tests/parylene_properties/confirm.py",
+                "name": "Parylene Properties",
+                "path": "qc_tests/parylene_properties/Parylene_prop.py",
+                "supported": false
+            },
+            "QUAD_MODULE_METROLOGY": {
+                "ITkPDcode": [
+                    "METROLOGY_QUAD",
+                    "QUAD_MODULE_METROLOGY"
+                ],
+                "code": "QUAD_MODULE_METROLOGY",
+                "confirm_path": "qc_tests/QUAD_MODULE_METROLOGY/confirm.py",
+                "name": "Quad Module Metrology",
+                "path": "qc_tests/QUAD_MODULE_METROLOGY/main.py",
+                "supported": true
+            },
+            "THERMAL_CYCLING": {
+                "ITkPDcode": [
+                    "THERMAL_CYCLING"
+                ],
+                "code": "THERMAL_CYCLING",
+                "confirm_path": "qc_tests/THERMAL_CYCLING/confirm.py",
+                "name": "Thermal Cycling",
+                "path": "qc_tests/THERMAL_CYCLING/Thermal.py",
+                "supported": true
+            },
+            "VISUAL_INSPECTION": {
+                "ITkPDcode": [
+                    "VISUAL_INSPECTION"
+                ],
+                "code": "VISUAL_INSPECTION",
+                "confirm_path": "qc_tests/VISUAL_INSPECTION/confirm.py",
+                "name": "Visual Inspection",
+                "path": "qc_tests/VISUAL_INSPECTION/main.py",
+                "supported": true
+            },
+            "WIREBONDING": {
+                "ITkPDcode": [
+                    "WIREBONDING"
+                ],
+                "code": "WIREBONDING",
+                "confirm_path": "qc_tests/wirebonding_info/confirm.py",
+                "name": "Wirebonding Information",
+                "path": "qc_tests/wirebonding_info/Wire_info.py",
+                "supported": false
+            },
+            "WIREBOND_PULL_TEST": {
+                "ITkPDcode": [
+                    "WIREBOND_PULL_TEST"
+                ],
+                "code": "WIREBOND_PULL_TEST",
+                "confirm_path": "qc_tests/WIREBOND_PULL_TEST/confirm.py",
+                "name": "Wirebond Pull Tests",
+                "path": "qc_tests/WIREBOND_PULL_TEST/main.py",
+                "supported": true
+            },
+            "WP_ENVELOPE": {
+                "ITkPDcode": [
+                    "WP_ENVELOPE"
+                ],
+                "code": "WP_ENVELOPE",
+                "confirm_path": "./qc_tests/roof_envelope/confirm.py",
+                "name": "Wire bonding roof envelope",
+                "path": "./qc_tests/roof_envelope/roof_envelope.py",
+                "supported": false
+            }
+        }
     },
-    "mongoDB": {
-        "address": "127.0.0.1",
-        "port": "27017"
+    "PCB": {
+        "property": {},
+        "test": {
+            "METROLOGY": {
+                "ITkPDcode": [
+                    "METROLOGY"
+                ],
+                "code": "METROLOGY",
+                "confirm_path": "qc_tests/metrology/confirm.py",
+                "name": "Metrology",
+                "path": "qc_tests/metrology/metrology_main.py",
+                "supported": false
+            },
+            "VISUAL_INSPECTION": {
+                "ITkPDcode": [
+                    "VISUAL_INSPECTION"
+                ],
+                "code": "VISUAL_INSPECTION",
+                "confirm_path": "qc_tests/VISUAL_INSPECTION/confirm.py",
+                "name": "Visual Inspection",
+                "path": "qc_tests/VISUAL_INSPECTION/main.py",
+                "supported": true
+            }
+        }
     }
 }
```

### Comparing `module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/dbinterface/bin/uploader_sample.py` & `module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/dbinterface/bin/uploader_sample.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import getpass
 import logging
 import sys
 from pathlib import Path
 
 import itkdb
 
-from module_qc_nonelec_gui.dbinterface.lib.upload_results_sample import upload_results
+from module_qc_nonelec_gui.dbinterface.upload_results_sample import upload_results
 
 log = logging.getLogger(__name__)
 
 ####################################
 ## upload test results
```

### Comparing `module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/qc_tests/flatness/flatness.py` & `module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/FLATNESS/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
 import json
 import logging
+from pathlib import Path
 
-import Path
 from PyQt5.QtWidgets import QMainWindow
 
-from module_qc_nonelec_gui.qc_tests.metrology.lib import initial_flatness
+from module_qc_nonelec_gui.qc_tests.FLATNESS import user_input
 
 log = logging.getLogger(__name__)
 
 
 class TestWindow(QMainWindow):
     ############################################################################################
     def __init__(self, parent=None):
@@ -44,20 +44,16 @@
 
         self.parent.testRun["results"]["comment"] = comment
 
         self.parent.receive_result(self)
 
     ############################################################################################
     def init_ui(self):
-        self.initial_bare_wid = initial_flatness.InitialWindow(self)
-        self.update_widget(self.initial_bare_wid)
-
-    def update_widget(self, w):
-        self.setCentralWidget(w)
-        self.show()
+        self.user_input_wid = user_input.InitialWindow(self)
+        self.parent.update_widget(self.user_input_wid)
 
     def close_and_return(self):
         self.close()
         self.parent.back_from_test()
 
     def back_page(self):
         self.parent.init_ui()
```

### Comparing `module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/qc_tests/flatness/example/example.json` & `module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/FLATNESS/example/example.json`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/qc_tests/glue_info_module_flex/Glue_info.py` & `module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/glue_info_module_flex/Glue_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import logging
 
 from PyQt5.QtWidgets import QMainWindow
 
-from module_qc_nonelec_gui.qc_tests.glue_info_module_flex.lib import initial_Glue_info
+from module_qc_nonelec_gui.qc_tests.glue_info_module_flex import initial_Glue_info
 
 log = logging.getLogger(__name__)
 
 
 class TestWindow(QMainWindow):
     ############################################################################################
     def __init__(self, parent=None):
```

### Comparing `module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/qc_tests/ivcurve/Sensor_IV.py` & `module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/WIREBOND_PULL_TEST/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,71 +1,51 @@
 from __future__ import annotations
 
-import logging
-
 from PyQt5.QtWidgets import QMainWindow
 
-from module_qc_nonelec_gui.qc_tests.ivcurve.lib import initial_Sensor_IV
-
-log = logging.getLogger(__name__)
+from module_qc_nonelec_gui.qc_tests.WIREBOND_PULL_TEST import user_input
 
 
 class TestWindow(QMainWindow):
     ############################################################################################
     def __init__(self, parent=None):
         super(QMainWindow, self).__init__()
         self.parent = parent
 
-        self.setWindowTitle("Sensor I-V")
-        self.scale_window(510, 255)
+        self.setWindowTitle("Wirebond pull tests")
+        self.scale_window(340, 255)
 
-        self.result_info = {"comment": "", "filename": ""}
-
-    def receive_result(self, result, comment):
-        self.parent.testRun["results"]["Metadata"].update(result)
-        self.parent.testRun["results"]["comment"] = comment
-
-        varMap = {
-            "CURRENT_MEAN": "Current_mean",
-            "CURRENT_SIGMA": "Current_sigma",
-            "VOLTAGE": "Voltage",
-            "TIME": "Time",
-            "HUMIDITY": "Humidity",
+        self.result_info = {
+            "minimum_load": "",
+            "minimum_load_unit": "g",
+            "maximum_load": "",
+            "maximum_load_unit": "g",
+            "mean_load": "",
+            "mean_load_unit": "g",
+            "load_standard_deviation": "",
+            "load_standard_deviation_unit": "g",
+            "percentage_of_heel_breaks": "",
+            "percentage_of_heel_breaks_unit": "%",
+            "comment": "",
         }
 
-        for v1, v2 in varMap.items():
-            self.parent.testRun["results"][v1] = [
-                dataPoint.get(v2) for dataPoint in result["Sensor_IV"]
-            ]
-
-        self.return_result()
-
     ###########################################################################################
 
     def init_ui(self):
-        self.initial_wid = initial_Sensor_IV.InitialWindow(self)
-        self.update_widget(self.initial_wid)
+        self.initial_wid = user_input.InitialWindow(self)
+        self.parent.update_widget(self.initial_wid)
 
     def scale_window(self, x, y):
         self.setGeometry(0, 0, x, y)
 
-    def update_widget(self, w):
-        self.scale_window(425, 255)
-        self.setCentralWidget(w)
-        self.show()
-
     def close_and_return(self):
         self.close()
         self.parent.back_from_test()
 
     def back_page(self):
         self.parent.init_ui()
 
     def back_window(self):
         self.parent.receive_backpage()
 
-    def call_another_window(self, window):
-        self.hide()
-        window.init_ui()
-
     def return_result(self):
-        self.parent.receive_result(self)
+        self.parent.receive_result(self, self.test_result_dict)
```

### Comparing `module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/qc_tests/mass/MASS.py` & `module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/MASS_MEASUREMENT/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import logging
 
 from PyQt5.QtWidgets import QMainWindow
 
-from module_qc_nonelec_gui.qc_tests.mass.lib import initial_MASS
+from module_qc_nonelec_gui.qc_tests.MASS_MEASUREMENT import user_input
 
 log = logging.getLogger(__name__)
 
 
 class TestWindow(QMainWindow):
     ############################################################################################
     def __init__(self, parent=None):
@@ -25,15 +25,15 @@
             "mass_unit": "mg",
             "comment": "",
         }
 
     ###########################################################################################
 
     def init_ui(self):
-        self.initial_wid = initial_MASS.InitialWindow(self)
+        self.initial_wid = user_input.InitialWindow(self)
         self.parent.update_widget(self.initial_wid)
 
     def scale_window(self, x, y):
         self.setGeometry(0, 0, x, y)
 
     def close_and_return(self):
         self.close()
@@ -50,18 +50,15 @@
         window.init_ui()
 
     def receive_mass(self, mass_value, acu_value, comment):
         # Essentially only here is the hard-coded part (value mapping ).
         self.parent.testRun["results"]["MASS"] = float(mass_value)
         self.parent.testRun["results"]["property"]["SCALE_ACCURACY"] = float(acu_value)
         self.parent.testRun["results"]["comment"] = str(comment)
-        self.parent.testRun["results"]["Metadata"]["MASS_UNIT"] = self.result_info[
+        self.parent.testRun["results"]["metadata"]["MASS_UNIT"] = self.result_info[
             "mass_unit"
         ]
-        self.parent.testRun["results"]["Metadata"][
+        self.parent.testRun["results"]["metadata"][
             "SCALE_ACCURACY_UNIT"
         ] = self.result_info["Scale_accuracy_unit"]
 
-        self.return_result()
-
-    def return_result(self):
         self.parent.receive_result(self)
```

### Comparing `module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/qc_tests/metrology/metrology_main.py` & `module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/QUAD_MODULE_METROLOGY/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import json
 import logging
 from pathlib import Path
 
 from PyQt5.QtWidgets import QMainWindow
 
-from module_qc_nonelec_gui.qc_tests.metrology.lib import initial_metrology
+from module_qc_nonelec_gui.qc_tests.metrology import initial_metrology
 
 log = logging.getLogger(__name__)
 
 
 class TestWindow(QMainWindow):
     ############################################################################################
     def __init__(self, parent=None):
@@ -270,19 +270,15 @@
 
         log.info("[Test Result file] " + self.result_info["filename"])
         self.return_result()
 
     ############################################################################################
     def init_ui(self):
         self.initial_bare_wid = initial_metrology.InitialWindow(self)
-        self.update_widget(self.initial_bare_wid)
-
-    def update_widget(self, w):
-        self.setCentralWidget(w)
-        self.show()
+        self.parent.update_widget(self.initial_bare_wid)
 
     def close_and_return(self):
         self.close()
         self.parent.back_from_test()
 
     def back_page(self):
         self.parent.init_ui()
```

### Comparing `module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/qc_tests/metrology/example/example.json` & `module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/QUAD_MODULE_METROLOGY/example/example.json`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/qc_tests/parylene_properties/Parylene_prop.py` & `module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/parylene_properties/Parylene_prop.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import logging
 
 from PyQt5.QtWidgets import QMainWindow
 
-from module_qc_nonelec_gui.qc_tests.parylene_properties.lib import initial_Parylene_prop
+from module_qc_nonelec_gui.qc_tests.parylene_properties import initial_Parylene_prop
 
 log = logging.getLogger(__name__)
 
 
 class TestWindow(QMainWindow):
     ############################################################################################
     def __init__(self, parent=None):
```

### Comparing `module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/qc_tests/sldo_vi/example/jsonschema/validation_schema.json` & `module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/IV_MEASURE/example/jsonschema/validation_schema.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.625%*

 * *Differences: {"'additionalProperties'": 'True',*

 * * "'properties'": "{replace: OrderedDict([('properties', OrderedDict([('type', 'object'), "*

 * *                 "('properties', OrderedDict([('HUM', OrderedDict([('type', 'number')])), ('TEMP', "*

 * *                 "OrderedDict([('type', 'number')]))]))])), ('IV_ARRAY', OrderedDict([('type', "*

 * *                 "'object'), ('additionalProperties', True), ('required', ['voltage', 'current', "*

 * *                 "'sigma current', 'temperature', 'humidity', 'time']), ('properties', "*

 * * […]*

```diff
@@ -1,90 +1,70 @@
 {
-    "additionalProperties": false,
+    "additionalProperties": true,
     "properties": {
-        "A_step": {
-            "type": "number"
-        },
-        "Humidity": {
-            "type": "number"
-        },
-        "N_measurements_per_step": {
-            "type": "number"
-        },
-        "SLDO_VI": {
-            "items": {
-                "additionalProperties": false,
-                "maxProperties": 6,
-                "minProperties": 4,
-                "properties": {
-                    "Current": {
+        "IV_ARRAY": {
+            "additionalProperties": true,
+            "properties": {
+                "current": {
+                    "items": {
                         "type": "number"
                     },
-                    "Humidity": {
+                    "type": "array"
+                },
+                "humidity": {
+                    "items": {
                         "type": "number"
                     },
-                    "Temperature": {
+                    "type": "array"
+                },
+                "sigma current": {
+                    "items": {
                         "type": "number"
                     },
-                    "Time": {
+                    "type": "array"
+                },
+                "temperature": {
+                    "items": {
                         "type": "number"
                     },
-                    "Voltage_mean": {
+                    "type": "array"
+                },
+                "time": {
+                    "items": {
                         "type": "number"
                     },
-                    "Voltage_sigma": {
-                        "type": "number"
-                    }
+                    "type": "array"
                 },
-                "required": [
-                    "Time",
-                    "Current",
-                    "Voltage_mean",
-                    "Voltage_sigma"
-                ],
-                "type": "object"
+                "voltage": {
+                    "items": {
+                        "type": "number"
+                    },
+                    "type": "array"
+                }
             },
-            "type": "array"
-        },
-        "Step_duration": {
-            "type": "number"
-        },
-        "Temperature": {
-            "type": "number"
-        },
-        "V_Compliance": {
-            "type": "number"
+            "required": [
+                "voltage",
+                "current",
+                "sigma current",
+                "temperature",
+                "humidity",
+                "time"
+            ],
+            "type": "object"
         },
-        "unit": {
+        "properties": {
             "properties": {
-                "Current": {
-                    "type": "string"
+                "HUM": {
+                    "type": "number"
                 },
-                "Humidity": {
-                    "type": "string"
-                },
-                "Temperature": {
-                    "type": "string"
-                },
-                "Time": {
-                    "type": "string"
-                },
-                "Voltage": {
-                    "type": "string"
+                "TEMP": {
+                    "type": "number"
                 }
             },
-            "required": [
-                "Time",
-                "Voltage",
-                "Current"
-            ],
             "type": "object"
         }
     },
     "required": [
-        "A_step",
-        "N_measurements_per_step",
-        "Step_duration",
-        "V_Compliance"
+        "IV_ARRAY"
     ],
     "type": "object"
 }
```

### Comparing `module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/qc_tests/thermal_cycling/Thermal.py` & `module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/THERMAL_CYCLING/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 from PyQt5.QtWidgets import QMainWindow
 
-from module_qc_nonelec_gui.dbinterface.lib import localdb_uploader
-from module_qc_nonelec_gui.qc_tests.thermal_cycling.lib import initial_Thermal
+from module_qc_nonelec_gui.dbinterface import localdb_uploader
+from module_qc_nonelec_gui.qc_tests.thermal_cycling import initial_Thermal
 
 
 class TestWindow(QMainWindow):
     ############################################################################################
     def __init__(self, parent=None):
         super(QMainWindow, self).__init__()
         self.parent = parent
@@ -101,23 +101,15 @@
             }
         }
 
     ###########################################################################################
 
     def init_ui(self):
         self.initial_wid = initial_Thermal.InitialWindow(self)
-        self.update_widget(self.initial_wid)
-
-    def scale_window(self, x, y):
-        self.setGeometry(0, 0, x, y)
-
-    def update_widget(self, w):
-        self.scale_window(480, 360)
-        self.setCentralWidget(w)
-        self.show()
+        self.parent.update_widget(self.initial_wid)
 
     def close_and_return(self):
         self.close()
         self.parent.back_from_test()
 
     def back_page(self):
         self.parent.init_ui()
```

### Comparing `module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/qc_tests/vi/README.md` & `module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/README.md`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/qc_tests/vi/vi_main.py` & `module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/main.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,294 +1,351 @@
 from __future__ import annotations
 
 import json
 import logging
+import pprint
 import shutil
 import subprocess
 from pathlib import Path
 
 from PyQt5.QtWidgets import QFileDialog, QMainWindow, QMessageBox
 
-from module_qc_nonelec_gui.dbinterface.lib import localdb_uploader
-from module_qc_nonelec_gui.qc_tests.vi.functions.auto_trim import detect_circle
-from module_qc_nonelec_gui.qc_tests.vi.functions.cv2_func import (
-    cv2,
-    img_rotate,
-    read_img,
-    write_img,
-)
-from module_qc_nonelec_gui.qc_tests.vi.lib import (
-    auto_trimimg_win,
+from module_qc_nonelec_gui.dbinterface import localdb_uploader
+from module_qc_nonelec_gui.qc_tests.VISUAL_INSPECTION import (
     inspection_win,
-    loadimg_win,
+    shaping_win,
     splitimg_win,
     summary_win,
-    trimimg_win,
     vi_initial_win,
 )
+from module_qc_nonelec_gui.qc_tests.VISUAL_INSPECTION.functions.cv2_func import (
+    cv2,
+    img_rotate,
+    read_img,
+    write_img,
+)
 
 log = logging.getLogger(__name__)
 
 
 class TestWindow(QMainWindow):
     def __init__(self, parent=None):
         super(QMainWindow, self).__init__(parent)
         self.parent = parent
 
         self.setGeometry(0, 0, 500, 300)
 
-        temp_dir_path = "temp"
+        self.temp_dir_path = "/var/tmp/modulq-qc-nonelec-gui/vi"
         try:
-            Path(temp_dir_path).mkdir(parents=True)
+            Path(self.temp_dir_path).mkdir(parents=True)
         except FileExistsError:
-            shutil.rmtree(temp_dir_path)
-            Path(temp_dir_path).mkdir(parents=True)
+            shutil.rmtree(self.temp_dir_path)
+            Path(self.temp_dir_path).mkdir(parents=True)
 
         # window title
         self.setWindowTitle("Visual Inspection GUI")
 
         # list and dict of anomalies
         self.anomaly_dic = {}
         self.comment_dic = {}
         self.img_dic = {}
 
         # component and user information
         self.atlsn = self.parent.info_dict["component"]
         self.type_name = self.parent.info_dict["componentType"]
         # self.original_institution = self.parent.info_dict["institution"]
         # self.current_location = self.parent.info_dict["currentLocation"]
-        if self.type_name == "MODULE":
+        if self.type_name in ["MODULE", "PCB"]:
             self.stage = self.parent.info_dict["currentStage"]
             self.inspector = self.parent.db_user
         else:
             self.stage = ""
             self.inspector = ""
 
         # load configuration file
         log.info(f"type_name = {self.type_name}")
         log.info(f"stage = {self.stage}")
 
         stage_alt = self.stage.replace("/", "__")
 
-        if self.type_name == "MODULE":
+        if self.type_name in ["MODULE", "PCB"]:
+            self.json_default = str(
+                Path(__file__).parent / f"config/config_{self.type_name}_default.json"
+            )
             self.json_config = str(
                 Path(__file__).parent
                 / f"config/config_{self.type_name}_{stage_alt}.json"
             )
-            self.json_reference = str(
-                Path(__file__).parent
-                / f"config/reference_{self.type_name}_{stage_alt}.json"
-            )
-        with Path(self.json_config).open() as f:
+
+        with Path(self.json_default).open() as f:
             self.config = json.load(f)
-        with Path(self.json_reference).open() as f:
-            self.reference = json.load(f)
+        with Path(self.json_config).open() as f:
+            self.custom = json.load(f)
+
+            for key in [
+                "frontside_goldenmodule_path",
+                "backside_goldenmodule_path",
+                "ntile",
+                "nsplit",
+                "backside",
+            ]:
+                if key in self.custom:
+                    self.config[key] = self.custom[key]
+
+            if "checklist" in self.custom:
+                for side in ["front", "back"]:
+                    if side in self.custom["checklist"]:
+                        for flag in ["Yellow", "Red"]:
+                            if flag in self.custom["checklist"][side]:
+                                self.config["checklist"][side][flag] = (
+                                    self.custom["checklist"][side][flag]
+                                    + self.config["checklist"][side][flag]
+                                )
+
+        if self.config.get("backside") is True:
+            QMessageBox.warning(
+                self,
+                "Warning",
+                "Back-side inspection is required in this stage: please make sure that the photograph is already recorded at this point, otherwise you will be required to re-do the front-side inspection again!",
+            )
+
+        log.info(pprint.pformat(self.config))
 
-        # path to golden modules
-        # self.path_gm = 'qc_tests/vi/golden_module'
-        self.path_gm = str(Path(__file__).parent / self.config["goldenmodule_path"])
+        self.origImgPath = {"front": "", "back": ""}
+        self.mode = "front"
 
+        # checked page list
+        self.rev = 0
+        self.tot_page = int(self.config["ntile"])
+        self.nsplit = int(self.config["nsplit"])
+        self.page_checked = []
+        for i in range(self.tot_page):
+            self.page_checked.insert(i, False)
+
+    def init_ui(self):
         # check the presence of golden modules
+
         try:
-            with Path(self.path_gm + "/main_img.jpg").open() as f:
-                pass
+            self.path_gm = str(
+                Path(__file__).parent
+                / self.config[f"{self.mode}side_goldenmodule_path"]
+            )
+
+        except Exception:
+            QMessageBox.warning(
+                self,
+                "Warning",
+                f"{self.mode.capitalize()}-side Golden module path is undefined in the config file!",
+            )
+
+        try:
+            with (Path(self.path_gm).parent / ".version").open() as f:
+                version_info = f.read()
+
+                if version_info.find("2023-04-04") < 0:
+                    msg = "Golden module version outdated"
+                    raise Exception(msg)
+
         except Exception as e:
             log.exception("missing the golden image file: " + str(e))
 
             QMessageBox.warning(
-                None,
+                self,
                 "Warning",
                 "Golden module image bank is being downloaded...\nWait for a minute.",
             )
 
             log.info(f"Golden module not found on {self.path_gm}, deploying it...")
+
             subprocess.run(
-                "cd /tmp; rm -rf golden_module*; curl -O https://cernbox.cern.ch/remote.php/dav/public-files/FmenidYbrKAJAdW/golden_module_20230320.zip",
+                "cd /var/tmp; rm -rf golden_module*; curl -O https://cernbox.cern.ch/remote.php/dav/public-files/EAbb7RxrEqyCyrS/golden_module_20230404.zip",
                 shell=True,
             )
-            subprocess.run("cd /tmp; unzip golden_module_20230320.zip", shell=True)
+            subprocess.run("cd /var/tmp; unzip golden_module_*.zip", shell=True)
+
+            shutil.rmtree(str(Path(self.path_gm).parent))
+
             subprocess.run(
-                "mv -f /tmp/golden_module {}".format(
+                "mv -f /var/tmp/golden_module {}; rm -rf golden_module*".format(
                     str(Path(self.path_gm).parent.parent)
                 ),
                 shell=True,
             )
-            subprocess.run("rm -rf /tmp/golden_module*", shell=True)
 
             with Path(self.path_gm + "/main_img.jpg").open() as f:
                 pass
 
-        # checked page list
-        self.rev = 0
-        self.tot_page = int(self.config["ntile"])
-        self.nsplit = int(self.config["nsplit"])
-        self.page_checked = []
-        for i in range(self.tot_page):
-            self.page_checked.insert(i, False)
+            QMessageBox.warning(
+                self,
+                "Information",
+                "The latest golden module image bank was deployed.",
+            )
+
+        for index, _check in enumerate(self.page_checked):
+            self.page_checked[index] = False
+
+        self.anomaly_dic = {}
+        self.comment_dic = {}
+        self.img_dic = {}
 
         # check list
         self.checklist_dict = {}
 
-        for tile in range(36):
-            default = self.config["checklist"].get("default")
+        checklist = self.config["checklist"].get(self.mode)
 
-            if default:
-                self.checklist_dict[str(tile)] = default
-
-            if str(tile) in self.config["checklist"]:
-                self.checklist_dict[str(tile)].update(
-                    self.config["checklist"].get(str(tile))
-                )
-
-    def update_widget(self, w):
-        self.setCentralWidget(w)
-        self.show()
+        for tile in range(36):
+            if checklist:
+                self.checklist_dict[str(tile)] = checklist
 
-    def init_ui(self):
         self.initial_wid = vi_initial_win.InitialWindow(self)
-        self.update_widget(self.initial_wid)
+        self.parent.update_widget(self.initial_wid)
 
     def close_and_return(self):
         self.close()
         self.parent.back_from_test()
 
     def update_img(self, img):
-        path = f"temp/img_{self.rev}.jpg"
+        self.rev = self.rev + 1
+        path = f"{self.temp_dir_path}/img_{self.mode}_{self.rev}.jpg"
         write_img(img, path)
+        log.info(f"dumped image {path}")
         self.img_bgr, self.img_h, self.img_w, self.img_d = read_img(path)
-        self.rev = self.rev + 1
 
     def undo_img(self):
         if self.rev == 0:
             self.rev = self.rev
         else:
             self.rev = self.rev - 1
-        path = f"temp/img_{self.rev}.jpg"
+        path = f"{self.temp_dir_path}/img_{self.mode}_{self.rev}.jpg"
         self.img_bgr, self.img_h, self.img_w, self.img_d = read_img(path)
 
-    def load_img(self):
-        try:
-            self.img_bgr
-            self.load_img_wid = loadimg_win.LoadImageWindow(self)
-            self.update_widget(self.load_img_wid)
-        except AttributeError:
-            options = QFileDialog.Options()
-            inputFileName, _ = QFileDialog.getOpenFileName(
-                self,
-                "Open File",
-                "",
-                "Images (*.bmp *.dib *.pbm *.pgm *.ppm *.sr *.ras *.jpeg *.jpg *.jpe *.jp2 *.png *.tiff *.tif);;Any files (*)",
-                options=options,
-            )
-            if not inputFileName:
-                log.info("image is not chosen")
+    def load_img(self, mode="front"):
+        options = QFileDialog.Options()
+        inputFileName, _ = QFileDialog.getOpenFileName(
+            self,
+            "Open File",
+            "",
+            "Images (*.bmp *.dib *.pbm *.pgm *.ppm *.sr *.ras *.jpeg *.jpg *.jpe *.jp2 *.png *.tiff *.tif);;Any files (*)",
+            options=options,
+        )
+        if not inputFileName:
+            log.info("image is not chosen")
+        else:
+            self.statusBar().showMessage(inputFileName)
+            log.info(inputFileName)
+
+            self.img_bgr, self.img_h, self.img_w, self.img_d = read_img(inputFileName)
+
+            self.mode = mode
+
+            self.origImgPath[
+                self.mode
+            ] = f"{self.temp_dir_path}/img_{self.mode}_org.jpg"
+            write_img(self.img_bgr, self.origImgPath[self.mode])
+
+            if self.img_h > 1000 and self.img_w > 1000:
+                self.scale = 10
             else:
-                self.statusBar().showMessage(inputFileName)
-                log.info(inputFileName)
+                self.scale = 1
+            self.n_page = 0
+            log.info("OpenCV image read success.")
 
-                self.img_bgr, self.img_h, self.img_w, self.img_d = read_img(
-                    inputFileName
-                )
-                write_img(self.img_bgr, "temp/img_org.jpg")
-                if self.img_h > 1000 and self.img_w > 1000:
-                    self.scale = 10
-                else:
-                    self.scale = 1
-                self.n_page = 0
-                log.info("OpenCV image read success.")
-
-                self.rev = 0
-
-                QMessageBox.information(
-                    self,
-                    "Instruction",
-                    'Before starting inspection, proper trimming is required.\n\n * "Rotate Image" for rotation by 90 degree for each click;\n * "Trim Image" for arranging the inspection scope;\n * Once above are done, proceed to "Split Image".',
-                )
+            self.rev = 0
 
-                self.load_img_wid = loadimg_win.LoadImageWindow(self)
-                self.update_widget(self.load_img_wid)
+            self.shape_img()
 
-    def rotate_img(self):
-        # self.rotate_img_wid = rotateimg_win.RotateImageWindow(self)
-        # self.update_widget(self.rotate_img_wid)
-        img, h, w, d = img_rotate(self.img_bgr)
-        self.update_img(img)
-        self.load_img()
+    def shape_img(self):
+        log.info("shape_img()")
+        img, h, w, d = read_img(self.origImgPath.get(self.mode))
+
+        if self.mode == "front":
+            self.shape_img_wid = shaping_win.QuadFrontTrimmer(self)
+        elif self.mode == "back":
+            self.shape_img_wid = shaping_win.QuadBackTrimmer(self)
 
-    def auto_trim_img(self):
-        img, h, w, d = read_img("temp/img_org.jpg")
+        self.parent.update_widget(self.shape_img_wid)
+
+    def rotate_img(self):
         try:
-            self.circles = detect_circle(self.img_bgr)
-            self.iscircle = True
-            self.auto_trim_img_wid = auto_trimimg_win.TrimImageWindow(self)
-            self.update_widget(self.auto_trim_img_wid)
-        except Exception:
-            self.img_bgr, self.img_h, self.img_w, self.img_d = read_img(
-                "temp/img_org.jpg"
+            img, h, w, d = read_img(
+                f"{self.temp_dir_path}/img_{self.mode}_{self.rev}.jpg"
             )
-            self.trim_img()
-            self.iscircle = False
+        except Exception:
+            img, h, w, d = read_img(self.origImgPath.get(self.mode))
 
-    def trim_img(self):
-        self.trim_img_wid = trimimg_win.TrimImageWindow(self)
-        self.update_widget(self.trim_img_wid)
+        img, h, w, d = img_rotate(img)
+        self.update_img(img)
 
     def split_img(self):
         self.split_img_wid = splitimg_win.SplitImageWindow(self)
-        self.update_widget(self.split_img_wid)
+        self.parent.update_widget(self.split_img_wid)
 
     def inspection(self):
         # Guiding dialog
         self.msg_map = {
             "MODULE/ASSEMBLY": "Check carefully:\n * Glue must not reach the edge of sensor/PCB;\n * Glue does not infiltrate the pads or back-side of the sensor;\n",
             "MODULE/WIREBONDING": "Check carefully:\n * All wires match the wire bond map;\n * No shorts due to bad bonding.",
             "MODULE/PARYLENE_MASKING": "Check carefully:\n * All wires match the wire bond map;\n * No shorts due to bad bonding.",
             "MODULE/PARYLENE_COATING": "",
-            "MODULE/PARYLENE_UNMASKING": "",
+            "MODULE/PARYLENE_UNMASKING": 'Check carefully:\n * Has the parylene coating penetrated the pickup and strain relief or connector areas?\n * Are there any areas where de-lamination of the parylene layer is seen that may result in contamination of the module?\n * Is the back of the module free of parylene such that only small "witness marks" are visible on the edges of the ASICs?',
             "MODULE/WIREBOND_PROTECTION": "",
             "MODULE/THERMAL_CYCLES": "",
+            "PCB_RECEPTION": "",
+            "PCB_POPULATION": "",
+            "PCB_CUTTING": "",
+            "PCB_RECEPTION_MODULE_SITE": "",
         }
 
         if self.n_page == 0:
             QMessageBox.information(
                 self,
                 "Note",
                 "\n\n".join(
                     [
-                        self.parent.info_dict.get("currentStage"),
-                        self.msg_map.get(self.parent.info_dict.get("currentStage")),
+                        self.parent.info_dict.get("currentStage", ""),
+                        self.msg_map.get(self.parent.info_dict.get("currentStage", "")),
                         "Key-binds:\n * X: Checkout Tile\n * F: Next Page\n * B: Previous Page\n * S: Switch Target/Reference",
                     ]
                 ),
             )
 
         inspection_wid = inspection_win.InspectionWindow(self)
-        self.update_widget(inspection_wid)
+        self.parent.update_widget(inspection_wid)
 
     def make_result(self):
-        # write whole module picture
-        cv2.imwrite("temp/main_img.jpg", self.img_bgr)
-        path_target = "temp/main_img.jpg"
-        path_reference = self.path_gm + "/main_img.jpg"
+        path_target = f"{self.temp_dir_path}/main_{self.mode}_img.jpg"
+        cv2.imwrite(path_target, self.img_bgr)
 
-        path_target = str(
+        oid_target = str(
             localdb_uploader.jpeg_formatter(self.parent.localDB, path_target)
         )
-        path_reference = str(
-            localdb_uploader.jpeg_formatter(self.parent.localDB, path_reference)
-        )
+
         for page, path_jpeg in self.img_dic.items():
             self.img_dic[page] = str(
                 localdb_uploader.jpeg_formatter(self.parent.localDB, path_jpeg)
             )
 
-        self.parent.testRun["results"]["Metadata"]["defects"] = self.anomaly_dic
-        self.parent.testRun["results"]["Metadata"]["comments"] = self.comment_dic
+        self.parent.testRun["results"]["metadata"][
+            f"{self.mode}_defects"
+        ] = self.anomaly_dic
+        self.parent.testRun["results"]["metadata"][
+            f"{self.mode}_comments"
+        ] = self.comment_dic
+        self.parent.testRun["results"]["metadata"][f"{self.mode}_image"] = oid_target
+        self.parent.testRun["results"]["metadata"][
+            f"{self.mode}_defect_images"
+        ] = self.img_dic
+
+        if self.config.get("backside") is True and self.mode == "front":
+            self.mode = "back"
+            self.init_ui()
 
-        self.return_result()
+        else:
+            self.return_result()
 
-    def go_to_summary(self):
+    def go_to_summary(self, sub):
+        sub.hide()
         summary_wid = summary_win.SummaryWindow(self)
-        self.update_widget(summary_wid)
+        self.parent.update_widget(summary_wid)
 
     def return_result(self):
         self.parent.receive_result(self)
```

### Comparing `module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/qc_tests/vi/config/VI_Config_Module.json` & `module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/VI_Config_Module.json`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/qc_tests/vi/config/VI_Config_Module_MODULETOPCB.json` & `module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/VI_Config_Module_MODULETOPCB.json`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/qc_tests/vi/config/config_PCB.json` & `module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/config/config_PCB.json`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/qc_tests/vi/functions/auto_trim.py` & `module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/functions/auto_trim.py`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/qc_tests/vi/functions/cv2_func.py` & `module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/VISUAL_INSPECTION/functions/cv2_func.py`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.2/src/module_qc_nonelec_gui/qc_tests/wirebonding_info/Wire_info.py` & `module_qc_nonelec_gui-0.0.3/src/module_qc_nonelec_gui/qc_tests/wirebonding_info/Wire_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 from PyQt5.QtWidgets import QMainWindow
 
-from module_qc_nonelec_gui.dbinterface.lib import localdb_uploader
-from module_qc_nonelec_gui.qc_tests.wirebonding_info.lib import initial_Wire_info
+from module_qc_nonelec_gui.dbinterface import localdb_uploader
+from module_qc_nonelec_gui.qc_tests.wirebonding_info import initial_Wire_info
 
 
 class TestWindow(QMainWindow):
     ############################################################################################
     def __init__(self, parent=None):
         super(QMainWindow, self).__init__()
         self.parent = parent
```

### Comparing `module_qc_nonelec_gui-0.0.2/.gitignore` & `module_qc_nonelec_gui-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.2/LICENSE` & `module_qc_nonelec_gui-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.2/README.md` & `module_qc_nonelec_gui-0.0.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# module-qc-nonelec-gui 0.0.2
+# module-qc-nonelec-gui 0.0.3
 
 ## What is this
 
 This package is previously known to as "QC Helper" and it provides a GUI
 application for submitting non-electrical QC tests of ITkPix modules.
 
 It requires `python3.7` and relevant python modules. The GUI uses `PyQT5`
```

### Comparing `module_qc_nonelec_gui-0.0.2/pyproject.toml` & `module_qc_nonelec_gui-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `module_qc_nonelec_gui-0.0.2/PKG-INFO` & `module_qc_nonelec_gui-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: module-qc-nonelec-gui
-Version: 0.0.2
+Version: 0.0.3
 Summary: GUI to upload Pixel Quality Control tests to ITk Production Database
 Project-URL: Documentation, https://module-qc-nonelec-gui.readthedocs.io/
 Project-URL: Homepage, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-nonelec-gui
 Project-URL: Bug Tracker, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-nonelec-gui/-/issues
 Project-URL: Source, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-nonelec-gui
 Author-email: Hideyuki Oide <Hideyuki.Oide@cern.ch>, Minoru Hirose <Minoru.Hirose@cern.ch>, Giordon Stark <gstark@cern.ch>, Daiki Sameshima <sameshima@hepmail.phys.se.tmu.ac.jp>, Erika Oshima <ooshima@hepmail.phys.se.tmu.ac.jp>, Yuji Onishi <onishi@cern.ch>
 Maintainer-email: Giordon Stark <gstark@cern.ch>, Hideyuki Oide <Hideyuki.Oide@cern.ch>, ATLAS ITk Pixels <atlas-itk-pixel-modules@cern.ch>
@@ -60,15 +60,15 @@
 Requires-Dist: pyqt5; platform_system == 'Darwin'
 Requires-Dist: pyqt5<=5.15.3; platform_system == 'Linux'
 Requires-Dist: requests
 Requires-Dist: typer
 Requires-Dist: typing-extensions>=3.7; python_version < '3.8'
 Description-Content-Type: text/markdown
 
-# module-qc-nonelec-gui 0.0.2
+# module-qc-nonelec-gui 0.0.3
 
 ## What is this
 
 This package is previously known to as "QC Helper" and it provides a GUI
 application for submitting non-electrical QC tests of ITkPix modules.
 
 It requires `python3.7` and relevant python modules. The GUI uses `PyQT5`
```

