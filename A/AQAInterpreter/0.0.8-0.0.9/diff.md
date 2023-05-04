# Comparing `tmp/aqainterpreter-0.0.8.tar.gz` & `tmp/aqainterpreter-0.0.9.tar.gz`

## Comparing `aqainterpreter-0.0.8.tar` & `aqainterpreter-0.0.9.tar`

### file list

```diff
@@ -1,93 +1,93 @@
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/README.md
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/input.txt
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/ouput.svg
--rwxr-xr-x   0        0        0      956 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/setup.sh
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/todo.md
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/.vscode/extentions.json
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/.vscode/launch.json
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/.vscode/settings.json
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/AQAInterpreter/__init__.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/AQAInterpreter/__main__.py
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/AQAInterpreter/environment.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/AQAInterpreter/errors.py
--rw-r--r--   0        0        0     3584 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/AQAInterpreter/interpreter.py
--rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/AQAInterpreter/main.py
--rw-r--r--   0        0        0     8937 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/AQAInterpreter/parser.py
--rw-r--r--   0        0        0     6926 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/AQAInterpreter/scanner.py
--rw-r--r--   0        0        0     2877 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/AQAInterpreter/test_.py
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/AQAInterpreter/tokens.py
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/add_code.py
--rw-r--r--   0        0        0     3943 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/aqa.xml
--rwxr-xr-x   0        0        0      593 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/compile_report.sh
--rwxr-xr-x   0        0        0      385 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/compile_report_no_font.sh
--rw-r--r--   0        0        0     4284 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/notes.md
--rw-r--r--   0        0        0    50849 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/report.md
--rw-r--r--   0        0        0   393766 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/classes.png
--rw-r--r--   0        0        0    39279 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/classes.svg
--rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/comparison.svg
--rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/compiler.svg
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/declaration.svg
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/declarations.svg
--rw-r--r--   0        0        0     2660 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/end.svg
--rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/equality.svg
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/expression.svg
--rw-r--r--   0        0        0     3549 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/factor.svg
--rw-r--r--   0        0        0     3696 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/for.svg
--rw-r--r--   0        0        0     4561 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/if.svg
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/logic_and.svg
--rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/logic_or.svg
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/mermaid_config.json
--rw-r--r--   0        0        0    21859 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/packages.svg
--rw-r--r--   0        0        0     7137 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/parser.svg
--rw-r--r--   0        0        0     5298 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/primary.svg
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/print.svg
--rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/program.svg
--rw-r--r--   0        0        0   116550 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/pytest.png
--rw-r--r--   0        0        0     7157 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/scanner.svg
--rw-r--r--   0        0        0   234850 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/screenshot1.png
--rw-r--r--   0        0        0    67423 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/screenshot2.png
--rw-r--r--   0        0        0    76110 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/screenshot3.png
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/server.svg
--rw-r--r--   0        0        0     2824 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/statement.svg
--rw-r--r--   0        0        0     7362 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/symbol_table.svg
--rw-r--r--   0        0        0    28131 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/syntax_tree.svg
--rw-r--r--   0        0        0    27813 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/syntax_tree_edit.svg
--rw-r--r--   0        0        0   214266 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/table_a.png
--rw-r--r--   0        0        0   144629 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/table_b.png
--rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/term.svg
--rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/unary.svg
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/variable_declaration.svg
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/website.svg
--rw-r--r--   0        0        0     3138 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/while.svg
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/input/classes.mmd
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/input/comparison.pikchr
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/input/compiler.pikchr
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/input/declaration.pikchr
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/input/declarations.pikchr
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/input/end.pikchr
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/input/equality.pikchr
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/input/expression.pikchr
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/input/factor.pikchr
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/input/for.pikchr
--rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/input/if.pikchr
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/input/logic_and.pikchr
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/input/logic_or.pikchr
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/input/packages.mmd
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/input/parser.mmd
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/input/primary.pikchr
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/input/print.pikchr
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/input/program.pikchr
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/input/scanner.mmd
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/input/server.pikchr
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/input/statement.pikchr
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/input/symbol_table.mmd
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/input/syntax_tree.mmd
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/input/term.pikchr
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/input/unary.pikchr
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/input/variable_declaration.pikchr
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/input/website.pikchr
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/input/while.pikchr
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/.gitignore
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/LICENSE
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/README.md
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/input.txt
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/ouput.svg
+-rwxr-xr-x   0        0        0      956 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/setup.sh
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/todo.md
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/.vscode/extentions.json
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/.vscode/launch.json
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/.vscode/settings.json
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/AQAInterpreter/__init__.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/AQAInterpreter/__main__.py
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/AQAInterpreter/environment.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/AQAInterpreter/errors.py
+-rw-r--r--   0        0        0     3584 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/AQAInterpreter/interpreter.py
+-rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/AQAInterpreter/main.py
+-rw-r--r--   0        0        0     9035 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/AQAInterpreter/parser.py
+-rw-r--r--   0        0        0     6926 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/AQAInterpreter/scanner.py
+-rw-r--r--   0        0        0     2877 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/AQAInterpreter/test_.py
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/AQAInterpreter/tokens.py
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/report/add_code.py
+-rw-r--r--   0        0        0     3943 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/report/aqa.xml
+-rwxr-xr-x   0        0        0      593 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/report/compile_report.sh
+-rwxr-xr-x   0        0        0      385 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/report/compile_report_no_font.sh
+-rw-r--r--   0        0        0     4284 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/report/notes.md
+-rw-r--r--   0        0        0    50849 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/report/report.md
+-rw-r--r--   0        0        0   393766 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/report/assets/classes.png
+-rw-r--r--   0        0        0    39279 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/report/assets/classes.svg
+-rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/report/assets/comparison.svg
+-rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/report/assets/compiler.svg
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/report/assets/declaration.svg
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/report/assets/declarations.svg
+-rw-r--r--   0        0        0     2660 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/report/assets/end.svg
+-rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/report/assets/equality.svg
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/report/assets/expression.svg
+-rw-r--r--   0        0        0     3549 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/report/assets/factor.svg
+-rw-r--r--   0        0        0     3696 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/report/assets/for.svg
+-rw-r--r--   0        0        0     4561 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/report/assets/if.svg
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/report/assets/logic_and.svg
+-rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/report/assets/logic_or.svg
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/report/assets/mermaid_config.json
+-rw-r--r--   0        0        0    21859 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/report/assets/packages.svg
+-rw-r--r--   0        0        0     7137 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/report/assets/parser.svg
+-rw-r--r--   0        0        0     5298 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/report/assets/primary.svg
+-rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/report/assets/print.svg
+-rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/report/assets/program.svg
+-rw-r--r--   0        0        0   116550 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/report/assets/pytest.png
+-rw-r--r--   0        0        0     7157 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/report/assets/scanner.svg
+-rw-r--r--   0        0        0   234850 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/report/assets/screenshot1.png
+-rw-r--r--   0        0        0    67423 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/report/assets/screenshot2.png
+-rw-r--r--   0        0        0    76110 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/report/assets/screenshot3.png
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/report/assets/server.svg
+-rw-r--r--   0        0        0     2824 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/report/assets/statement.svg
+-rw-r--r--   0        0        0     7362 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/report/assets/symbol_table.svg
+-rw-r--r--   0        0        0    28131 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/report/assets/syntax_tree.svg
+-rw-r--r--   0        0        0    27813 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/report/assets/syntax_tree_edit.svg
+-rw-r--r--   0        0        0   214266 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/report/assets/table_a.png
+-rw-r--r--   0        0        0   144629 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/report/assets/table_b.png
+-rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/report/assets/term.svg
+-rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/report/assets/unary.svg
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/report/assets/variable_declaration.svg
+-rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/report/assets/website.svg
+-rw-r--r--   0        0        0     3138 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/report/assets/while.svg
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/report/assets/input/classes.mmd
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/report/assets/input/comparison.pikchr
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/report/assets/input/compiler.pikchr
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/report/assets/input/declaration.pikchr
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/report/assets/input/declarations.pikchr
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/report/assets/input/end.pikchr
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/report/assets/input/equality.pikchr
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/report/assets/input/expression.pikchr
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/report/assets/input/factor.pikchr
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/report/assets/input/for.pikchr
+-rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/report/assets/input/if.pikchr
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/report/assets/input/logic_and.pikchr
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/report/assets/input/logic_or.pikchr
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/report/assets/input/packages.mmd
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/report/assets/input/parser.mmd
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/report/assets/input/primary.pikchr
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/report/assets/input/print.pikchr
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/report/assets/input/program.pikchr
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/report/assets/input/scanner.mmd
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/report/assets/input/server.pikchr
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/report/assets/input/statement.pikchr
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/report/assets/input/symbol_table.mmd
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/report/assets/input/syntax_tree.mmd
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/report/assets/input/term.pikchr
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/report/assets/input/unary.pikchr
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/report/assets/input/variable_declaration.pikchr
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/report/assets/input/website.pikchr
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/report/assets/input/while.pikchr
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/LICENSE
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 aqainterpreter-0.0.9/PKG-INFO
```

### Comparing `aqainterpreter-0.0.8/README.md` & `aqainterpreter-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.8/ouput.svg` & `aqainterpreter-0.0.9/ouput.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.8/setup.sh` & `aqainterpreter-0.0.9/setup.sh`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.8/.vscode/settings.json` & `aqainterpreter-0.0.9/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.8/AQAInterpreter/environment.py` & `aqainterpreter-0.0.9/AQAInterpreter/environment.py`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.8/AQAInterpreter/errors.py` & `aqainterpreter-0.0.9/AQAInterpreter/errors.py`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.8/AQAInterpreter/interpreter.py` & `aqainterpreter-0.0.9/AQAInterpreter/interpreter.py`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.8/AQAInterpreter/main.py` & `aqainterpreter-0.0.9/AQAInterpreter/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,25 +8,24 @@
 
 
 def run(source: str, debug: bool = False) -> str:
     """evaluates `source` returning a string"""
 
     source += "\n"
     if debug:
-        print(source)
+        click.echo(source)
 
     tokens = Scanner(source).scan_tokens()
     if debug:
-        pprint(tokens)
-        print()
+        click.echo(tokens)
 
     output: list[str] = []
     statements = Parser(tokens).parse()
     if debug:
-        print(statements)
+        click.echo(statements)
 
     for statement in statements:
         statement.interpret(output)
 
     return "".join(output)
 
 
@@ -39,17 +38,19 @@
     if `debug` is True, tokens and ast are also printed"""
 
     if filename and cmd:
         raise click.UsageError("cannot specify both filename and command")
 
     if filename:
         with open(filename, encoding="utf-8") as infp:
-            cmd = infp.read()
+            click.echo(run(infp.read(), debug=debug).rstrip())
+    elif cmd:
+        click.echo(run(cmd, debug=debug).rstrip())
     else:
+        # run REPL
         while True:
             click.echo(run(input("> "), debug=debug).rstrip())
 
-    click.echo(run(cmd, debug=debug).rstrip())
 
 
 if __name__ == "__main__":
     main()  # pylint: disable=no-value-for-parameter
```

### Comparing `aqainterpreter-0.0.8/AQAInterpreter/parser.py` & `aqainterpreter-0.0.9/AQAInterpreter/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -220,15 +220,17 @@
                 then_branch.extend(stmt)
 
             if self._match_token(ELSE):
                 self._match_token(COLON)
 
                 while not self._match_token(END):
                     if self._peek().type == EOF:
-                        raise self._error(self._peek(), "Expected END after IF statement")
+                        raise self._error(
+                            self._peek(), "Expected END after IF statement"
+                        )
                     stmt = self._statement()
                     if stmt is not None:
                         else_branch.extend(stmt)
                 break
 
         return (If(condition, then_branch, else_branch),)
 
@@ -243,15 +245,15 @@
             elif self._match_token(FOR):
                 return self._for_statement()
             elif self._match_token(IF):
                 return self._if_statement()
             else:
                 errors.error(self._peek(), "unexpected token")
                 self._advance()
-            
+
     def _var_declaration(self) -> tuple[Var]:
         name = self._consume(IDENTIFIER, "Expect variable name. ")
         initialiser = self._expression() if self._match_token(ASSIGNMENT) else None
         # consume(NEWLINE, "Expect newline after variable deceleration")
         return (Var(name, initialiser),)
 
     def _statement(self):
@@ -262,14 +264,17 @@
                 elif token.type == ASSIGNMENT:
                     return self._var_declaration()
         except AQAParseError as parse_error:
             errors.error(parse_error.token, parse_error.message)
             self._synchronize()
             return None
 
+        # our program is blank
+        self._advance()
+
     def parse(self):
         statements: list[Stmt] = []
         while not self._at_end():
             stmt = self._statement()
             if stmt is not None:
                 statements.extend(stmt)
         return statements
```

### Comparing `aqainterpreter-0.0.8/AQAInterpreter/scanner.py` & `aqainterpreter-0.0.9/AQAInterpreter/scanner.py`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.8/AQAInterpreter/test_.py` & `aqainterpreter-0.0.9/AQAInterpreter/test_.py`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.8/AQAInterpreter/tokens.py` & `aqainterpreter-0.0.9/AQAInterpreter/tokens.py`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.8/report/add_code.py` & `aqainterpreter-0.0.9/report/add_code.py`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.8/report/aqa.xml` & `aqainterpreter-0.0.9/report/aqa.xml`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.8/report/compile_report.sh` & `aqainterpreter-0.0.9/report/compile_report.sh`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.8/report/notes.md` & `aqainterpreter-0.0.9/report/notes.md`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.8/report/report.md` & `aqainterpreter-0.0.9/report/report.md`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.8/report/assets/classes.png` & `aqainterpreter-0.0.9/report/assets/classes.png`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.8/report/assets/classes.svg` & `aqainterpreter-0.0.9/report/assets/classes.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.8/report/assets/comparison.svg` & `aqainterpreter-0.0.9/report/assets/comparison.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.8/report/assets/compiler.svg` & `aqainterpreter-0.0.9/report/assets/compiler.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.8/report/assets/declaration.svg` & `aqainterpreter-0.0.9/report/assets/declaration.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.8/report/assets/declarations.svg` & `aqainterpreter-0.0.9/report/assets/declarations.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.8/report/assets/end.svg` & `aqainterpreter-0.0.9/report/assets/end.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.8/report/assets/equality.svg` & `aqainterpreter-0.0.9/report/assets/equality.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.8/report/assets/expression.svg` & `aqainterpreter-0.0.9/report/assets/expression.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.8/report/assets/factor.svg` & `aqainterpreter-0.0.9/report/assets/factor.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.8/report/assets/for.svg` & `aqainterpreter-0.0.9/report/assets/for.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.8/report/assets/if.svg` & `aqainterpreter-0.0.9/report/assets/if.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.8/report/assets/logic_and.svg` & `aqainterpreter-0.0.9/report/assets/logic_and.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.8/report/assets/logic_or.svg` & `aqainterpreter-0.0.9/report/assets/logic_or.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.8/report/assets/packages.svg` & `aqainterpreter-0.0.9/report/assets/packages.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.8/report/assets/parser.svg` & `aqainterpreter-0.0.9/report/assets/parser.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.8/report/assets/primary.svg` & `aqainterpreter-0.0.9/report/assets/primary.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.8/report/assets/print.svg` & `aqainterpreter-0.0.9/report/assets/print.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.8/report/assets/program.svg` & `aqainterpreter-0.0.9/report/assets/program.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.8/report/assets/pytest.png` & `aqainterpreter-0.0.9/report/assets/pytest.png`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.8/report/assets/scanner.svg` & `aqainterpreter-0.0.9/report/assets/scanner.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.8/report/assets/screenshot1.png` & `aqainterpreter-0.0.9/report/assets/screenshot1.png`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.8/report/assets/screenshot2.png` & `aqainterpreter-0.0.9/report/assets/screenshot2.png`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.8/report/assets/screenshot3.png` & `aqainterpreter-0.0.9/report/assets/screenshot3.png`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.8/report/assets/server.svg` & `aqainterpreter-0.0.9/report/assets/server.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.8/report/assets/statement.svg` & `aqainterpreter-0.0.9/report/assets/statement.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.8/report/assets/symbol_table.svg` & `aqainterpreter-0.0.9/report/assets/symbol_table.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.8/report/assets/syntax_tree.svg` & `aqainterpreter-0.0.9/report/assets/syntax_tree.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.8/report/assets/syntax_tree_edit.svg` & `aqainterpreter-0.0.9/report/assets/syntax_tree_edit.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.8/report/assets/table_a.png` & `aqainterpreter-0.0.9/report/assets/table_a.png`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.8/report/assets/table_b.png` & `aqainterpreter-0.0.9/report/assets/table_b.png`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.8/report/assets/term.svg` & `aqainterpreter-0.0.9/report/assets/term.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.8/report/assets/unary.svg` & `aqainterpreter-0.0.9/report/assets/unary.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.8/report/assets/variable_declaration.svg` & `aqainterpreter-0.0.9/report/assets/variable_declaration.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.8/report/assets/website.svg` & `aqainterpreter-0.0.9/report/assets/website.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.8/report/assets/while.svg` & `aqainterpreter-0.0.9/report/assets/while.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.8/report/assets/input/classes.mmd` & `aqainterpreter-0.0.9/report/assets/input/classes.mmd`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.8/report/assets/input/comparison.pikchr` & `aqainterpreter-0.0.9/report/assets/input/comparison.pikchr`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.8/report/assets/input/declaration.pikchr` & `aqainterpreter-0.0.9/report/assets/input/declaration.pikchr`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.8/report/assets/input/end.pikchr` & `aqainterpreter-0.0.9/report/assets/input/end.pikchr`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.8/report/assets/input/equality.pikchr` & `aqainterpreter-0.0.9/report/assets/input/equality.pikchr`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.8/report/assets/input/factor.pikchr` & `aqainterpreter-0.0.9/report/assets/input/factor.pikchr`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.8/report/assets/input/for.pikchr` & `aqainterpreter-0.0.9/report/assets/input/for.pikchr`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.8/report/assets/input/if.pikchr` & `aqainterpreter-0.0.9/report/assets/input/if.pikchr`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.8/report/assets/input/logic_and.pikchr` & `aqainterpreter-0.0.9/report/assets/input/logic_and.pikchr`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.8/report/assets/input/logic_or.pikchr` & `aqainterpreter-0.0.9/report/assets/input/logic_or.pikchr`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.8/report/assets/input/packages.mmd` & `aqainterpreter-0.0.9/report/assets/input/packages.mmd`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.8/report/assets/input/primary.pikchr` & `aqainterpreter-0.0.9/report/assets/input/primary.pikchr`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.8/report/assets/input/statement.pikchr` & `aqainterpreter-0.0.9/report/assets/input/statement.pikchr`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.8/report/assets/input/term.pikchr` & `aqainterpreter-0.0.9/report/assets/input/term.pikchr`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.8/report/assets/input/unary.pikchr` & `aqainterpreter-0.0.9/report/assets/input/unary.pikchr`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.8/report/assets/input/while.pikchr` & `aqainterpreter-0.0.9/report/assets/input/while.pikchr`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.8/LICENSE` & `aqainterpreter-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.8/pyproject.toml` & `aqainterpreter-0.0.9/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "AQAInterpreter"
 requires-python = ">=3.10"
 license = "MIT"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name = "CyberWarrior5466", email = "asaleen898@gmail.com" },
 ]
 dependencies = ["click==8.*"]
 
 [project.urls]
 Documentation = "https://github.com/CyberWarrior5466/nea"
```

