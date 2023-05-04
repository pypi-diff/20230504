# Comparing `tmp/aqainterpreter-0.0.7.tar.gz` & `tmp/aqainterpreter-0.0.8.tar.gz`

## Comparing `aqainterpreter-0.0.7.tar` & `aqainterpreter-0.0.8.tar`

### file list

```diff
@@ -1,84 +1,93 @@
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/README.md
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/input.txt
--rwxr-xr-x   0        0        0     1013 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/setup.sh
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/.vscode/extentions.json
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/.vscode/launch.json
--rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/.vscode/settings.json
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/AQAInterpreter/__init__.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/AQAInterpreter/__main__.py
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/AQAInterpreter/environment.py
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/AQAInterpreter/errors.py
--rw-r--r--   0        0        0     3584 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/AQAInterpreter/interpreter.py
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/AQAInterpreter/main.py
--rw-r--r--   0        0        0     8915 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/AQAInterpreter/parser.py
--rw-r--r--   0        0        0     6837 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/AQAInterpreter/scanner.py
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/AQAInterpreter/test_.py
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/AQAInterpreter/tokens.py
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/add_code.py
--rw-r--r--   0        0        0     3943 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/aqa.xml
--rwxr-xr-x   0        0        0      601 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/compile_report.sh
--rwxr-xr-x   0        0        0      379 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/compile_report_no_font.sh
--rw-r--r--   0        0        0     4284 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/notes.md
--rw-r--r--   0        0        0    44260 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/report.md
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/watch.py
--rw-r--r--   0        0        0    39279 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/classes.svg
--rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/comparison.svg
--rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/compiler.svg
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/declaration.svg
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/declarations.svg
--rw-r--r--   0        0        0     2660 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/end.svg
--rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/equality.svg
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/expression.svg
--rw-r--r--   0        0        0     3549 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/factor.svg
--rw-r--r--   0        0        0     3696 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/for.svg
--rw-r--r--   0        0        0     4561 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/if.svg
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/logic_and.svg
--rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/logic_or.svg
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/mermaid_config.json
--rw-r--r--   0        0        0    21859 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/packages.svg
--rw-r--r--   0        0        0     7137 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/parser.svg
--rw-r--r--   0        0        0     5298 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/primary.svg
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/print.svg
--rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/program.svg
--rw-r--r--   0        0        0     7157 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/scanner.svg
--rw-r--r--   0        0        0   234850 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/screenshot1.png
--rw-r--r--   0        0        0    67423 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/screenshot2.png
--rw-r--r--   0        0        0    76110 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/screenshot3.png
--rw-r--r--   0        0        0     2824 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/statement.svg
--rw-r--r--   0        0        0     7362 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/symbol_table.svg
--rw-r--r--   0        0        0    28131 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/syntax_tree.svg
--rw-r--r--   0        0        0    27813 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/syntax_tree_edit.svg
--rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/term.svg
--rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/unary.svg
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/variable_declaration.svg
--rw-r--r--   0        0        0     3138 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/while.svg
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/input/classes.mmd
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/input/comparison.pikchr
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/input/compiler.pikchr
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/input/declaration.pikchr
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/input/declarations.pikchr
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/input/end.pikchr
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/input/equality.pikchr
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/input/expression.pikchr
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/input/factor.pikchr
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/input/for.pikchr
--rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/input/if.pikchr
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/input/logic_and.pikchr
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/input/logic_or.pikchr
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/input/packages.mmd
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/input/parser.mmd
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/input/primary.pikchr
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/input/print.pikchr
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/input/program.pikchr
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/input/scanner.mmd
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/input/statement.pikchr
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/input/symbol_table.mmd
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/input/syntax_tree.mmd
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/input/term.pikchr
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/input/unary.pikchr
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/input/variable_declaration.pikchr
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/report/assets/input/while.pikchr
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/.gitignore
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/LICENSE
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 aqainterpreter-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/README.md
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/input.txt
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/ouput.svg
+-rwxr-xr-x   0        0        0      956 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/setup.sh
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/todo.md
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/.vscode/extentions.json
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/.vscode/launch.json
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/.vscode/settings.json
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/AQAInterpreter/__init__.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/AQAInterpreter/__main__.py
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/AQAInterpreter/environment.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/AQAInterpreter/errors.py
+-rw-r--r--   0        0        0     3584 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/AQAInterpreter/interpreter.py
+-rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/AQAInterpreter/main.py
+-rw-r--r--   0        0        0     8937 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/AQAInterpreter/parser.py
+-rw-r--r--   0        0        0     6926 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/AQAInterpreter/scanner.py
+-rw-r--r--   0        0        0     2877 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/AQAInterpreter/test_.py
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/AQAInterpreter/tokens.py
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/add_code.py
+-rw-r--r--   0        0        0     3943 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/aqa.xml
+-rwxr-xr-x   0        0        0      593 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/compile_report.sh
+-rwxr-xr-x   0        0        0      385 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/compile_report_no_font.sh
+-rw-r--r--   0        0        0     4284 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/notes.md
+-rw-r--r--   0        0        0    50849 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/report.md
+-rw-r--r--   0        0        0   393766 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/classes.png
+-rw-r--r--   0        0        0    39279 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/classes.svg
+-rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/comparison.svg
+-rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/compiler.svg
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/declaration.svg
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/declarations.svg
+-rw-r--r--   0        0        0     2660 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/end.svg
+-rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/equality.svg
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/expression.svg
+-rw-r--r--   0        0        0     3549 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/factor.svg
+-rw-r--r--   0        0        0     3696 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/for.svg
+-rw-r--r--   0        0        0     4561 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/if.svg
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/logic_and.svg
+-rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/logic_or.svg
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/mermaid_config.json
+-rw-r--r--   0        0        0    21859 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/packages.svg
+-rw-r--r--   0        0        0     7137 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/parser.svg
+-rw-r--r--   0        0        0     5298 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/primary.svg
+-rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/print.svg
+-rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/program.svg
+-rw-r--r--   0        0        0   116550 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/pytest.png
+-rw-r--r--   0        0        0     7157 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/scanner.svg
+-rw-r--r--   0        0        0   234850 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/screenshot1.png
+-rw-r--r--   0        0        0    67423 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/screenshot2.png
+-rw-r--r--   0        0        0    76110 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/screenshot3.png
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/server.svg
+-rw-r--r--   0        0        0     2824 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/statement.svg
+-rw-r--r--   0        0        0     7362 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/symbol_table.svg
+-rw-r--r--   0        0        0    28131 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/syntax_tree.svg
+-rw-r--r--   0        0        0    27813 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/syntax_tree_edit.svg
+-rw-r--r--   0        0        0   214266 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/table_a.png
+-rw-r--r--   0        0        0   144629 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/table_b.png
+-rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/term.svg
+-rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/unary.svg
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/variable_declaration.svg
+-rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/website.svg
+-rw-r--r--   0        0        0     3138 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/while.svg
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/input/classes.mmd
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/input/comparison.pikchr
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/input/compiler.pikchr
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/input/declaration.pikchr
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/input/declarations.pikchr
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/input/end.pikchr
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/input/equality.pikchr
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/input/expression.pikchr
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/input/factor.pikchr
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/input/for.pikchr
+-rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/input/if.pikchr
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/input/logic_and.pikchr
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/input/logic_or.pikchr
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/input/packages.mmd
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/input/parser.mmd
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/input/primary.pikchr
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/input/print.pikchr
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/input/program.pikchr
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/input/scanner.mmd
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/input/server.pikchr
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/input/statement.pikchr
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/input/symbol_table.mmd
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/input/syntax_tree.mmd
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/input/term.pikchr
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/input/unary.pikchr
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/input/variable_declaration.pikchr
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/input/website.pikchr
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/report/assets/input/while.pikchr
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/LICENSE
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 aqainterpreter-0.0.8/PKG-INFO
```

### Comparing `aqainterpreter-0.0.7/README.md` & `aqainterpreter-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.7/setup.sh` & `aqainterpreter-0.0.8/setup.sh`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 #!/bin/bash
 
 # # ubuntu
 # sudo apt update && sudo apt upgrade -y
-# sudo apt install hatch pandoc texlive-xetex fonts-firacode yarnpkg fossil -y 
+# sudo apt install hatch pandoc texlive-xetex fonts-firacode yarnpkg fossil entr -y 
 
 # # fedora
-# sudo dnf install 'dnf-command(copr)'
-# sudo dnf copr enable adrienverge/some-nice-fonts -y
-# sudo dnf install hatch pandoc texlive-xetex fira-code-fonts some-nice-fonts yarnpkg librsvg2-tools texlive-scheme-medium fossil -y
+# sudo dnf install hatch pandoc texlive-xetex fira-code-fonts yarnpkg librsvg2-tools texlive-scheme-medium fossil entr -y
 
 
 # cd report
 # mkdir mermaid
 # cd mermaid
 # cd report
 # mkdir mermaid
@@ -26,12 +24,13 @@
 # # auto generate packages.mmd and classes.md
 # pyreverse ./AQAInterpreter/ -o mmd
 
 # # setup project
 # hatch shell
 
 # # publish to pypi
+# # increment version in `pyproject.toml`
 # hatch build && hatch publish && rm -rf dist
 #   # go on https://pypi.org
 #   # get a token https://pypi.org/help/#apitoke
 #   # copy paste the username and token in this command
```

### Comparing `aqainterpreter-0.0.7/.vscode/launch.json` & `aqainterpreter-0.0.8/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.7/.vscode/settings.json` & `aqainterpreter-0.0.8/.vscode/settings.json`

 * *Files 14% similar despite different names*

```diff
@@ -1,55 +1,74 @@
-00000000: 7b0a 2020 2020 2f2f 2022 5b6d 6172 6b64  {.    // "[markd
-00000010: 6f77 6e5d 223a 207b 0a20 2020 202f 2f20  own]": {.    // 
-00000020: 2020 2020 2265 6469 746f 722e 666f 6e74      "editor.font
-00000030: 4661 6d69 6c79 223a 2022 6361 6c69 6272  Family": "calibr
-00000040: 692c 2043 6172 6c69 746f 220a 2020 2020  i, Carlito".    
-00000050: 2f2f 207d 2c0a 2020 2020 2263 5370 656c  // },.    "cSpel
-00000060: 6c2e 656e 6162 6c65 6422 3a20 7472 7565  l.enabled": true
-00000070: 2c0a 2020 2020 2263 5370 656c 6c2e 776f  ,.    "cSpell.wo
-00000080: 7264 7322 3a20 5b0a 2020 2020 2020 2020  rds": [.        
-00000090: 2241 5141 2773 222c 0a20 2020 2020 2020  "AQA's",.       
-000000a0: 2022 6171 6169 6e74 6572 7072 6574 6572   "aqainterpreter
-000000b0: 222c 0a20 2020 2020 2020 2022 4249 444d  ",.        "BIDM
-000000c0: 4153 222c 0a20 2020 2020 2020 2022 636f  AS",.        "co
-000000d0: 6c6f 7572 7322 2c0a 2020 2020 2020 2020  lours",.        
-000000e0: 2245 4e44 464f 5222 2c0a 2020 2020 2020  "ENDFOR",.      
-000000f0: 2020 2265 6e64 7265 636f 7264 222c 0a20    "endrecord",. 
-00000100: 2020 2020 2020 2022 656e 6473 7562 222c         "endsub",
-00000110: 0a20 2020 2020 2020 2022 454e 4453 5542  .        "ENDSUB
-00000120: 524f 5554 494e 4522 2c0a 2020 2020 2020  ROUTINE",.      
-00000130: 2020 2245 4e44 5748 494c 4522 2c0a 2020    "ENDWHILE",.  
-00000140: 2020 2020 2020 2245 4e44 5757 4849 4c45        "ENDWWHILE
-00000150: 222c 0a20 2020 2020 2020 2022 454e 464f  ",.        "ENFO
-00000160: 5222 2c0a 2020 2020 2020 2020 2247 4353  R",.        "GCS
-00000170: 4522 2c0a 2020 2020 2020 2020 2269 6e66  E",.        "inf
-00000180: 7022 2c0a 2020 2020 2020 2020 2269 6e6f  p",.        "ino
-00000190: 7469 6679 222c 0a20 2020 2020 2020 2022  tify",.        "
-000001a0: 4e61 7572 222c 0a20 2020 2020 2020 2022  Naur",.        "
-000001b0: 4e79 7374 726f 6d22 2c0a 2020 2020 2020  Nystrom",.      
-000001c0: 2020 2270 6167 6562 7265 616b 222c 0a20    "pagebreak",. 
-000001d0: 2020 2020 2020 2022 7061 6e64 6f63 222c         "pandoc",
-000001e0: 0a20 2020 2020 2020 2022 5041 5245 4e22  .        "PAREN"
-000001f0: 2c0a 2020 2020 2020 2020 2270 7970 726f  ,.        "pypro
-00000200: 6a65 6374 222c 0a20 2020 2020 2020 2022  ject",.        "
-00000210: 7079 7465 7374 222c 0a20 2020 2020 2020  pytest",.       
-00000220: 2022 5265 6563 6522 2c0a 2020 2020 2020   "Reece",.      
-00000230: 2020 2273 7461 7274 7377 6974 6822 2c0a    "startswith",.
-00000240: 2020 2020 2020 2020 2274 6578 6c69 7665          "texlive
-00000250: 222c 0a20 2020 2020 2020 2022 546f 646f  ",.        "Todo
-00000260: 7322 2c0a 2020 2020 2020 2020 2274 7261  s",.        "tra
-00000270: 6e73 7069 6c69 6e67 222c 0a20 2020 2020  nspiling",.     
-00000280: 2020 2022 756e 7465 726d 696e 6174 6564     "unterminated
-00000290: 222c 0a20 2020 2020 2020 2022 7865 6c61  ",.        "xela
-000002a0: 7465 7822 0a20 2020 205d 2c0a 2020 2020  tex".    ],.    
-000002b0: 2270 7974 686f 6e2e 6465 6661 756c 7449  "python.defaultI
-000002c0: 6e74 6572 7072 6574 6572 5061 7468 223a  nterpreterPath":
-000002d0: 2022 7e2f 2e6c 6f63 616c 2f73 6861 7265   "~/.local/share
-000002e0: 2f68 6174 6368 2f65 6e76 2f76 6972 7475  /hatch/env/virtu
-000002f0: 616c 2f61 7161 696e 7465 7270 7265 7465  al/aqainterprete
-00000300: 722f 4849 4c30 4c73 4277 2f61 7161 696e  r/HIL0LsBw/aqain
-00000310: 7465 7270 7265 7465 722f 6269 6e2f 7079  terpreter/bin/py
-00000320: 7468 6f6e 222c 0a20 2020 2022 6353 7065  thon",.    "cSpe
-00000330: 6c6c 2e65 6e61 626c 6546 696c 6574 7970  ll.enableFiletyp
-00000340: 6573 223a 205b 2221 7961 6d6c 225d 2c0a  es": ["!yaml"],.
-00000350: 2020 2020 2263 5370 656c 6c2e 6c61 6e67      "cSpell.lang
-00000360: 7561 6765 223a 2022 656e 2d47 4222 0a7d  uage": "en-GB".}
+00000000: 7b0a 2020 2020 225b 6d61 726b 646f 776e  {.    "[markdown
+00000010: 5d22 3a20 7b0a 2020 2020 2020 2020 2265  ]": {.        "e
+00000020: 6469 746f 722e 666f 6e74 4661 6d69 6c79  ditor.fontFamily
+00000030: 223a 2022 6361 6c69 6272 692c 2043 6172  ": "calibri, Car
+00000040: 6c69 746f 220a 2020 2020 7d2c 0a20 2020  lito".    },.   
+00000050: 2022 6353 7065 6c6c 2e65 6e61 626c 6564   "cSpell.enabled
+00000060: 223a 2074 7275 652c 0a20 2020 2022 6353  ": true,.    "cS
+00000070: 7065 6c6c 2e77 6f72 6473 223a 205b 0a20  pell.words": [. 
+00000080: 2020 2020 2020 2022 4151 4127 7322 2c0a         "AQA's",.
+00000090: 2020 2020 2020 2020 2261 7161 696e 7465          "aqainte
+000000a0: 7270 7265 7465 7222 2c0a 2020 2020 2020  rpreter",.      
+000000b0: 2020 2242 4944 4d41 5322 2c0a 2020 2020    "BIDMAS",.    
+000000c0: 2020 2020 2263 6c65 616e 646f 6322 2c0a      "cleandoc",.
+000000d0: 2020 2020 2020 2020 2263 6f6c 6f75 7273          "colours
+000000e0: 222c 0a20 2020 2020 2020 2022 636f 6c75  ",.        "colu
+000000f0: 6d6e 6272 6561 6b22 2c0a 2020 2020 2020  mnbreak",.      
+00000100: 2020 2264 6174 6163 6c61 7373 222c 0a20    "dataclass",. 
+00000110: 2020 2020 2020 2022 6461 7461 636c 6173         "dataclas
+00000120: 7365 7322 2c0a 2020 2020 2020 2020 2245  ses",.        "E
+00000130: 4e44 464f 5222 2c0a 2020 2020 2020 2020  NDFOR",.        
+00000140: 2265 6e64 7265 636f 7264 222c 0a20 2020  "endrecord",.   
+00000150: 2020 2020 2022 656e 6473 7562 222c 0a20       "endsub",. 
+00000160: 2020 2020 2020 2022 454e 4453 5542 524f         "ENDSUBRO
+00000170: 5554 494e 4522 2c0a 2020 2020 2020 2020  UTINE",.        
+00000180: 2245 4e44 5748 494c 4522 2c0a 2020 2020  "ENDWHILE",.    
+00000190: 2020 2020 2245 4e44 5757 4849 4c45 222c      "ENDWWHILE",
+000001a0: 0a20 2020 2020 2020 2022 454e 464f 5222  .        "ENFOR"
+000001b0: 2c0a 2020 2020 2020 2020 2266 6173 7461  ,.        "fasta
+000001c0: 7069 222c 0a20 2020 2020 2020 2022 4743  pi",.        "GC
+000001d0: 5345 222c 0a20 2020 2020 2020 2022 696e  SE",.        "in
+000001e0: 6670 222c 0a20 2020 2020 2020 2022 696e  fp",.        "in
+000001f0: 6f74 6966 7922 2c0a 2020 2020 2020 2020  otify",.        
+00000200: 226d 756c 7469 636f 6c73 222c 0a20 2020  "multicols",.   
+00000210: 2020 2020 2022 4e61 7572 222c 0a20 2020       "Naur",.   
+00000220: 2020 2020 2022 4e79 7374 726f 6d22 2c0a       "Nystrom",.
+00000230: 2020 2020 2020 2020 2270 6167 6562 7265          "pagebre
+00000240: 616b 222c 0a20 2020 2020 2020 2022 7061  ak",.        "pa
+00000250: 6e64 6f63 222c 0a20 2020 2020 2020 2022  ndoc",.        "
+00000260: 5041 5245 4e22 2c0a 2020 2020 2020 2020  PAREN",.        
+00000270: 2270 796c 696e 7422 2c0a 2020 2020 2020  "pylint",.      
+00000280: 2020 2270 7970 726f 6a65 6374 222c 0a20    "pyproject",. 
+00000290: 2020 2020 2020 2022 7079 7269 6768 7422         "pyright"
+000002a0: 2c0a 2020 2020 2020 2020 2270 7974 6573  ,.        "pytes
+000002b0: 7422 2c0a 2020 2020 2020 2020 2252 6565  t",.        "Ree
+000002c0: 6365 222c 0a20 2020 2020 2020 2022 7265  ce",.        "re
+000002d0: 7072 222c 0a20 2020 2020 2020 2022 7374  pr",.        "st
+000002e0: 6172 7473 7769 7468 222c 0a20 2020 2020  artswith",.     
+000002f0: 2020 2022 7465 786c 6976 6522 2c0a 2020     "texlive",.  
+00000300: 2020 2020 2020 2254 6f64 6f73 222c 0a20        "Todos",. 
+00000310: 2020 2020 2020 2022 7472 616e 7370 696c         "transpil
+00000320: 696e 6722 2c0a 2020 2020 2020 2020 2275  ing",.        "u
+00000330: 6e74 6572 6d69 6e61 7465 6422 2c0a 2020  nterminated",.  
+00000340: 2020 2020 2020 2278 656c 6174 6578 220a        "xelatex".
+00000350: 2020 2020 5d2c 0a20 2020 2022 7079 7468      ],.    "pyth
+00000360: 6f6e 2e64 6566 6175 6c74 496e 7465 7270  on.defaultInterp
+00000370: 7265 7465 7250 6174 6822 3a20 227e 2f2e  reterPath": "~/.
+00000380: 6c6f 6361 6c2f 7368 6172 652f 6861 7463  local/share/hatc
+00000390: 682f 656e 762f 7669 7274 7561 6c2f 6171  h/env/virtual/aq
+000003a0: 6169 6e74 6572 7072 6574 6572 2f48 494c  ainterpreter/HIL
+000003b0: 304c 7342 772f 6171 6169 6e74 6572 7072  0LsBw/aqainterpr
+000003c0: 6574 6572 2f62 696e 2f70 7974 686f 6e22  eter/bin/python"
+000003d0: 2c0a 2020 2020 2263 5370 656c 6c2e 656e  ,.    "cSpell.en
+000003e0: 6162 6c65 4669 6c65 7479 7065 7322 3a20  ableFiletypes": 
+000003f0: 5b22 2179 616d 6c22 5d2c 0a20 2020 2022  ["!yaml"],.    "
+00000400: 6353 7065 6c6c 2e6c 616e 6775 6167 6522  cSpell.language"
+00000410: 3a20 2265 6e2d 4742 222c 0a20 2020 2022  : "en-GB",.    "
+00000420: 7079 6c69 6e74 2e69 6d70 6f72 7453 7472  pylint.importStr
+00000430: 6174 6567 7922 3a20 2275 7365 4275 6e64  ategy": "useBund
+00000440: 6c65 6422 2c0a 2020 2020 2270 7974 686f  led",.    "pytho
+00000450: 6e2e 6c69 6e74 696e 672e 7079 6c69 6e74  n.linting.pylint
+00000460: 456e 6162 6c65 6422 3a20 7472 7565 2c0a  Enabled": true,.
+00000470: 2020 2020 2270 7974 686f 6e2e 6c69 6e74      "python.lint
+00000480: 696e 672e 656e 6162 6c65 6422 3a20 7472  ing.enabled": tr
+00000490: 7565 0a7d                                ue.}
```

### Comparing `aqainterpreter-0.0.7/AQAInterpreter/environment.py` & `aqainterpreter-0.0.8/AQAInterpreter/environment.py`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.7/AQAInterpreter/errors.py` & `aqainterpreter-0.0.8/AQAInterpreter/errors.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 class AQAParseError(RuntimeError):
     token: Token
     message: str
 
 
 def report(line: int, where: str, message: str) -> None:
-    print(f"[line {line}] Error {where}: {message}", file=sys.stderr)
+    print(f"[line {line}] Error '{where}': {message}", file=sys.stderr)
 
 
 def error(token: Token | int, message: str) -> None:
     if isinstance(token, Token):
         if token.type == NEWLINE:
             report(token.line, "at end of line", message)
         else:
```

### Comparing `aqainterpreter-0.0.7/AQAInterpreter/interpreter.py` & `aqainterpreter-0.0.8/AQAInterpreter/interpreter.py`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.7/AQAInterpreter/main.py` & `aqainterpreter-0.0.8/AQAInterpreter/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
     for statement in statements:
         statement.interpret(output)
 
     return "".join(output)
 
 
-@click.command()
+@click.command
 @click.argument("filename", required=False)
 @click.option("-c", "--cmd")
 @click.option("-d", "--debug", is_flag=True, default=False, help="Show tokens and ast")
 def main(filename: str, cmd: str, debug: bool):
     """source code can be read in from a file or a string
     if `debug` is True, tokens and ast are also printed"""
 
@@ -48,8 +48,8 @@
         while True:
             click.echo(run(input("> "), debug=debug).rstrip())
 
     click.echo(run(cmd, debug=debug).rstrip())
 
 
 if __name__ == "__main__":
-    main()
+    main()  # pylint: disable=no-value-for-parameter
```

### Comparing `aqainterpreter-0.0.7/AQAInterpreter/parser.py` & `aqainterpreter-0.0.8/AQAInterpreter/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -206,28 +206,29 @@
         return out
 
     def _if_statement(self) -> tuple[If]:
         condition = self._expression()
         then_branch: list[Stmt] = []
         else_branch: list[Stmt] = []
 
-        if self._peek().type in {THEN, COLON}:
-            self._match_token(THEN, COLON)
+        self._match_token(THEN, COLON)
 
         while not self._match_token(END):
             if self._peek().type == EOF:
                 raise self._error(self._peek(), "Expected END after IF statement")
 
             if (stmt := self._statement()) is not None:
                 then_branch.extend(stmt)
 
             if self._match_token(ELSE):
+                self._match_token(COLON)
+
                 while not self._match_token(END):
                     if self._peek().type == EOF:
-                        raise error(self._peek(), "Expected END after IF statement")
+                        raise self._error(self._peek(), "Expected END after IF statement")
                     stmt = self._statement()
                     if stmt is not None:
                         else_branch.extend(stmt)
                 break
 
         return (If(condition, then_branch, else_branch),)
 
@@ -239,34 +240,33 @@
                 return self._print_statement()
             elif self._match_token(WHILE):
                 return self._while_statement()
             elif self._match_token(FOR):
                 return self._for_statement()
             elif self._match_token(IF):
                 return self._if_statement()
-            elif self.tokens[self._current].type == EOF:
-                return
-            self._current += 1
-            return
-
+            else:
+                errors.error(self._peek(), "unexpected token")
+                self._advance()
+            
     def _var_declaration(self) -> tuple[Var]:
         name = self._consume(IDENTIFIER, "Expect variable name. ")
         initialiser = self._expression() if self._match_token(ASSIGNMENT) else None
         # consume(NEWLINE, "Expect newline after variable deceleration")
         return (Var(name, initialiser),)
 
     def _statement(self):
         try:
             for token in self.tokens[self._current :]:
                 if token.type in {PRINT, WHILE, FOR, IF, NEWLINE}:
                     return self._statement_not_var()
                 elif token.type == ASSIGNMENT:
                     return self._var_declaration()
-        except AQAParseError as e:
-            errors.error(e.token, e.message)
+        except AQAParseError as parse_error:
+            errors.error(parse_error.token, parse_error.message)
             self._synchronize()
             return None
 
     def parse(self):
         statements: list[Stmt] = []
         while not self._at_end():
             stmt = self._statement()
```

### Comparing `aqainterpreter-0.0.7/AQAInterpreter/scanner.py` & `aqainterpreter-0.0.8/AQAInterpreter/scanner.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,17 +186,18 @@
                     self._add(STEP)
                 elif text in {"end", "endif", "endwhile", "endfor"}:
                     self._add(END)
                 elif text in {"print", "output"}:
                     self._add(PRINT)
                 else:
                     self._add(IDENTIFIER)
-
-            case _:
-                errors.error(self._line, "Unexpected character")
+            case [character, *_]:
+                print("idk")
+                errors.report(self._line, character, "Unexpected character")
+                self._current += 1
 
     def scan_tokens(self) -> list[Token]:
         """takes in `source` and performs lexical analysis emitting tokens"""
         while self._current < len(self.source):
             self._start = self._current
             self._scan_token()
         return self._tokens + [Token(EOF, line=self._line)]
```

### Comparing `aqainterpreter-0.0.7/AQAInterpreter/tokens.py` & `aqainterpreter-0.0.8/AQAInterpreter/tokens.py`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.7/report/add_code.py` & `aqainterpreter-0.0.8/report/add_code.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,54 +1,61 @@
 """adds tree and code for technical solution in `report.md` from disk"""
 
 from pathlib import Path
 import subprocess
 import sys
 
-lst = (
+files_list = (
     (".gitignore", "text"),
     ("LICENSE", "text"),
     ("pyproject.toml", "toml"),
     ("AQAInterpreter/__init__.py", "python"),
     ("AQAInterpreter/main.py", "python"),
     ("AQAInterpreter/errors.py", "python"),
     ("AQAInterpreter/tokens.py", "python"),
     ("AQAInterpreter/scanner.py", "python"),
     ("AQAInterpreter/environment.py", "python"),
     ("AQAInterpreter/parser.py", "python"),
     ("AQAInterpreter/interpreter.py", "python"),
-    ("AQAInterpreter/test_.py", "python"),
 )
 
+tests_list = (("AQAInterpreter/test_.py", "python"),)
 
-out = (
+
+files_out = (
     "```\n"
     + subprocess.run(
-        f"tree --prune -P '{'|'.join(Path(row[0]).name for row in lst)}'",
+        f"tree --prune -P '{'|'.join(Path(row[0]).name for row in files_list)}'",
         shell=True,
         text=True,
         capture_output=True,
         check=True,
     ).stdout.rstrip()
     + "\n```"
 )
-
+tests_out = ""
 
 TEMPLATE = """
 ## {}
 ``` {{.{} .numberLines}}
 {}
 ```
 """
 
 
-for file, file_ext in lst:
-    out += TEMPLATE.format(file, file_ext, open(file, encoding="utf-8").read())
+for file, file_ext in files_list:
+    files_out += TEMPLATE.format(file, file_ext, Path(file).read_text(encoding="utf-8"))
+
+for file, file_ext in tests_list:
+    tests_out += TEMPLATE.format(file, file_ext, Path(file).read_text(encoding="utf-8"))
 
+file_path = Path(sys.argv[1])
 
-with open(sys.argv[1], encoding="utf-8") as infp:
-    content = infp.read()
+content = file_path.read_text(encoding="utf-8")
+content = content.replace("\\TECHNICAL_SOLUTION", files_out)
+content = content.replace("\\TESTS", tests_out)
 
-content = content.replace("\\TECHNICAL_SOLUTION", out)
+if len(sys.argv) == 3:
+    for char in ("│", "╭", "─", "├", "└", "∕", "≠", "≤", "≥"):
+        content = content.replace(char, "")
 
-with open(sys.argv[1], "w", encoding="utf-8") as outfile:
-    outfile.write(content)
+file_path.write_text(content, encoding="utf-8")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aqainterpreter-0.0.7/report/aqa.xml` & `aqainterpreter-0.0.8/report/aqa.xml`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.7/report/compile_report.sh` & `aqainterpreter-0.0.8/report/compile_report.sh`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 #!/bin/bash
 
-# cd report/assets/input
+cd report/assets/input
 
 # for i in *.mmd; do
 #     ~/.yarn/bin/mmdc -c ../mermaid_config.json \
 #          -i "$i" \
 #          -o "../${i%.*}.svg"
 # done
 
-# for i in *.pikchr; do
-#     fossil pikchr "$i" "../${i%.*}.svg"
-# done
+for i in *.pikchr; do
+    fossil pikchr "$i" "../${i%.*}.svg"
+done
 
-# cd ../../..
+cd ../../..
 
 cp report/report.md report/temp_report.md
 python report/add_code.py report/temp_report.md
 
 cd report
 pandoc metadata.yaml temp_report.md \
         --output=out.pdf \
@@ -25,8 +25,8 @@
         --table-of-contents \
         --number-sections
 
 
 rm temp_report.md
 cd ..
 
-xdg-open report/out.pdf
+# xdg-open report/out.pdf
```

### Comparing `aqainterpreter-0.0.7/report/notes.md` & `aqainterpreter-0.0.8/report/notes.md`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.7/report/report.md` & `aqainterpreter-0.0.8/report/report.md`

 * *Files 14% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 # AQA Pseudo-code
 array = ["a", "b", "c"]
 OUTPUT array[1]
 ```
 
 Following the spec, arrays in AQA Pseudo-code start indexing at `0` so therefore the  is `b`.  Due to the consistency of the spec, we where  able to unambiguously determine the output. 
 
-This consistency means that it would be possible to write a translator, that would take any set of pseudo-code following the AQA's style and convert it to the corresponding machine code. This blurs the lines between the pseudo-code and *real languages*. So henceforth correct AQA Pseudo-code, following the spec will just be referred to as AQA code.
+This consistency means that it would be possible to write a translator, that would take any set of pseudo-code following the AQA's style and convert it to the corresponding machine code. This blurs the lines between the pseudo-code and *real languages*.
 
 ## Justification
 
 Some people may argue that a translator for AQA code would be unnecessary and would hinder students. It is mainly used for offline on-paper examinations without a computer. So having  a tool to generate machine code would not be needed as it  may confuse students to what the purpose of pseudo-code is. Furthermore where a working algorithm is needed it would be sufficient to manually translate AQA pseudo-code to an existing high level language where a compiler or translator is already available.
 
 However I would argue that an AQA code translator would have real world uses not just as a research project. For example using this tool,  it would give students more experience and knowledge of AQA code, which would aid reading and comprehension skills. Moreover, it would mean that manually rewriting AQA code into another high level language for example python would be unheeded. And it would avoid the chances of bugs being introduced in the rewrite saving students a large amount of time.
 
@@ -109,15 +109,14 @@
 - **Compilers** first scan/tokenize the source code producing a list of tokens which are then parsed producing an intermediary format such as byte-code. This is then converted into *machine code*. For example the *clang* compiler for *C++* converts the source code to *LLVM byte-codes* which is then converted to standalone *machine code* for each system, for example *X-86*. However *Java byte-code* is distributed standalone and each system requires a *JVM* (Java Virtual Machine) installed to do the final conversion step to *machine code*.
 
 - **Interpreters** scan and parse but the source code is executed statement by statement and converted to *machine code* on the fly. Interpreters are simpler to implement but can be slower than the final output of a compiled language.
 
 - **Transpilers** scan and parse but the intermediary form is converted to another high level language where a compiler or interpreter already available. For example, the *Nim* programming language works by first transpiling to either *C*, *C++* or *Java-Script*.
 
 - Other notes: languages can be expressed with regular grammar. Tools like yacc and lex are known as compiler compilers as they create a compiler given regular grammar of the language to be built as input. However I will not be using these and I am interesting in learning how a translator works.
-- Other notes: languages can be expressed with regular grammar. Tools like yacc and lex are known as compiler compilers as they create a compiler given regular grammar of the language to be built as input. However I will not be using these and I am interesting in learning how a translator works.
 
 **Advantages and disadvantages of each approach**
 
 The advantages of a compiler is that is can optimize the resulting machine code, making the executable more efficient. However a disadvantage of machine code is that the machine code is not portable, and cannot be copied over to different systems. Furthermore,  the compilation step may take a large amount of time for complex projects, which means that errors, also will take a long time to show up. This reduces iteration speeds and can result in a worse developer experience than an interpreter where the errors show up much quicker. 
 
 Therefore I will create an interpreter as its the simplest to implement and based on my user research usability and develop experience are more important factors than performance.
 
@@ -134,27 +133,31 @@
    line = line.replace(/ mod /g, " % ")    // The bug is here
     var lin = line.trim();
     var sp = lin.indexOf(" ");
     var first = "";
     if (startswith(lin, "if")) { first = "if" }
     ...
 }
+
 ```
+![http://ibcomp.fis.edu/pseudocode/pcode.html](assets/screenshot1.png){width=85% align=centre}
 
-![Website 1](assets/screenshot1.png){width=85% align=centre}
+\pagebreak
 
 Another solution, also for IB 'pseudo-code' is written by [Dep Jain](https://pseudocode.deepjain.com/). It is much more complicated and includes syntax highlighting and auto-completions powered by an open source project code editor called [ace](https://github.com/ajaxorg/ace). It defaults to dark mode which makes the website easier on the eyes. It has large buttons on the top and also has the ability to save and load files from the users cookies similar to the previous program. However the web page makes a *HTTP* request to a server to translate the code, making it closed source and also slower than the previous solution.
 
-![Website 2](assets/screenshot2.png){width=85% align=centre}
+![(https://pseudocode.deepjain.com/)](assets/screenshot2.png){width=70% align=centre}
+
+\pagebreak  <!-- this page break is so image goes on page    -->
 
 Both programs are website, making it convenient as the user does not have to download any language tools. Website are also portable and can be accessed on any computer with an internet connection. Therefore I would consider developing a simple online IDE as well, second to a programmed solution.
 
 Another disadvantage is that both solutions are limited to the IB computer science syllabus and not AQA's. Focusing my project on AQA's 'pseudo-code' will make my project unique. My solution should also be open source like the first example allowing the user to view the source code to better understand how their code was interpreted.
 
-## Project Requirements
+## Project requirements
 
 1. Create a tree-walk interpreter for all the features in AQA's 'pseudo-code' command set including but not limited to: 
    
    - `REPEAT`, `WHILE`, `FOR`, `IF`, `RECORD`, `SUBROUTINE` constructs
    
    - `INPUT`, `OUTPUT`, `LEN`, `POSITION`, `SUBSTRING`, `RANDOM_INT` functions
    
@@ -168,41 +171,202 @@
 
 2. Additionally I would like to make keywords case insensitive giving the use the ability to style code to his preference.
 
 3. The program should accept a large range of input. For example the 'pseudo-code' command set uses the unicode multiply sign `(×)` whereas most programming languages use an `(*)` as it can be typed on a traditional keyboard. My program should accept both of these symbols, making it adaptable. A table of these special symbols is show below.
    
    | Traditional | Unicode |
    | :---------: | :-----: |
-   |      *      |   ×     |
-   |      /      |   ÷     |
+   |      *      |    ×    |
+   |      /      |    ÷    |
    |     !=      |  `!=`   |
    |     <=      |  `<=`   |
    |     >=      |  `>=`   |
-   |     <-      |  `←`    |
+   |     <-      |   `←`   |
 
 4. Robust error handling, informing the user of what line syntax errors have occurred.
 
 5. Create on online IDE for users to quickly try out the language without having to install any extra language tools their local machine.
 
 6. Add syntax highlighting to highlight keywords and constructs, following the colours of the atom text editor, as it was my clients preference. 
 
+\pagebreak
+
 # Documented design
 
-## Language Choice
+## Language choice
 
 To translate 'pseudo-code' I am going ot build a *tree-walk* interpreter. The rough structure of my implementation is based on a book called *Crafting Interpreters* (ISBN 9780990582939) by *Robert Nystrom* which is written in *Java*. I have decided to use *Python* instead as it has a simple and readable syntax and is dynamically typed. This means I can re-use *python's* base types, which support string concatenation and integers of arbitrary precision meaning that integers will never overflow. *Python's* slower performance is not an issue as having a robust solution is higher priority and python is widely understood and is a popular language. Python is also multi-paradigm and supports OOP programming which is the main language feature I will use to structure my code. I also intend to use modules and split my code across multiple files to separate concerns.
 
+## Addressing redundancy
+
+Python has a number of language features and libraries to help write more concise code. Including dataclasses, pattern matching, and creating terminal user interfaces with the click library.
+
+### Using dataclass
+
+Dataclasses reduces a large amount of boiler plate normally required when working with classes. Here we use the builtin `@dataclass` decorator automatically creating an  `__init__` and `__repr__` method for us. Moreover, we can use the dot notation `instance.attribute` instead of having to define a separate getter and setter method for `attribute`. Our class definition goes from 15 lines to just 3.
+
+\Begin{multicols}{2}
+``` {.python .numberLines}
+from typing import Any
+
+
+class Example:
+    def __init__(self, attribute: Any):
+        self.attribute = attribute
+
+    def get_attribute(self):
+        return self.attribute
+
+    def set_attribute(
+        self, attribute: Any
+    ):
+        self.attribute = attribute
+
+    def __str__(self):
+        attribute = repr(self.attribute)
+        return f"Example({attribute})"
+
+
+instance = Example("foo")
+
+# prints `Example('foo')`
+print(instance)
+
+# prints `bar`
+instance.set_attribute("bar")
+print(instance.get_attribute())
+```
+
+\columnbreak
+
+
+``` {.python .numberLines}
+from dataclasses import dataclass
+
+
+@dataclass
+class Example:
+    attribute: Any
+
+
+instance = Example("foo")
+
+# prints `Example(instance='foo')`
+print(instance)
+
+# prints `bar`
+instance.attribute = "bar"
+print(instance.attribute)
+```
+\End{multicols}
+
+
+### Using match statement
+
+Python's match statement was introduced in 3.10. Using an `if` statement we have to manually check that the `tokens` list contains at least two characters otherwise accessing `tokens[0]` would raise and index error. Using a `match` statement, we don't have to worry about this. The `match` example also contains a wildcard `(*)` capturing any remaining characters, and storing them in a variable. The underscore denotes an unused variable.
+
+\Begin{multicols}{2}
+``` {.python .numberLines}
+tokens = list(input())
+
+if (
+    len(tokens) >= 2
+    and tokens[0] == "<"
+    and tokens[1] == "-"
+):
+    print("assignment")
+
+```
+\columnbreak
+
+``` {.python .numberLines}
+tokens = list(input())
+
+match tokens:
+    case ["<", "-", *_]:
+        print("assignment")
+
+    case _: pass
+```
+\End{multicols}
+
+### Using the click library
+
+Writing a program to take in command line arguments can be a chore. A manual approach like the first example doesn't scale well if there are lots of options. However, using a library like click allows for much more concise code, automatically creating a `--help` method from the function docstring and providing error handling on incorrect usage.
+
+``` {.python .numberLines}
+import inspect
+import sys
+
+
+match sys.argv: # pyright: reportMatchNotExhaustive=false
+    case [script_name, *other_args] if "--help" in other_args:
+        print(inspect.cleandoc(f"""
+            Usage: {script_name} [OPTIONS] [NAME]
+
+            Prints "Hello, NAME!", or simply "Hello, World!" if a name is not specified.
+
+            Options:
+            --help  Show this message and exit.
+        """))
+
+    case [script_name, name, *_]:
+        print(f"Hello, {name}!")
+
+    case [script_name]:
+        print("Hello, World!")
+
+    case [script_name]:
+        print(inspect.cleandoc(f"""
+            Usage: {script_name} [OPTIONS] [NAME]
+            Try '{script_name} --help' for help.
+
+            Argument error
+        """))
+
+        sys.exit(2)
+```
+
+``` {.python .numberLines}
+import click
+
+@click.command
+@click.argument("name", required=False, default="World")
+def hello(name: str = "world"):
+    """Prints "Hello, NAME!", or simply "Hello, World!" if a name is not specified."""
+    click.echo(f"Hello, {name}!")
+
+hello() # pylint: disable=no-value-for-parameter
+```
+\
+
+```bash
+$ python main.py --help
+Usage: main.py [OPTIONS] [NAME]
+
+  Prints "Hello, NAME!", or simply "Hello, World!" if a name is not specified.
+
+Options:
+  --help  Show this message and exit.
+
+$ python main.py Ali
+Hello, Ali!
+
+$ python main.py
+Hello, World!
+```
+
 ## High level system overview
 
+**Scanning**
+
 Converting 'pseudo-code' to *machine code* is comprised of several stages. After the user's source code is read in from a file or *stdin* it is stored in a variable of type string and resides in memory. The first main stage is known as scanning of tokenizing where the alphabet of characters are grouped together to form tokens that represent the grammar and punctuation of the language.
 
 During this stage lexical analysis is performed to group the right amount of characters into the right token. Some tokens are made up of single characters such as  (+) and (-). Whereas other tokens are made up of a set number of characters  such as FOR and IF.
 
-STRING and  NUMBER literals are made up of a variable number of characters and need to be handled correctly. If the number 3 is found inside of a string, it should be treated as part of the STRING literal and not its own NUMBER literal. Therefore our scanner program will need to treat the same character differently depending on its state such as whether it has seen an opening `"` or `'`. The NUMBER literals include floats so the scanner should also handle decimal points correctly.
-
 **Source code**
 
 ``` {.aqa .numberLines}
    IDENTIFIER `i`
          |  ╭───── ASSIGNMENT token
          ↓  ↓
          i <- 1
@@ -212,14 +376,16 @@
              ELSE                              ←─ ELSE token
                  OUTPUT i                      ←─ IDENTIFIER token
              ENDIF                             ←─ ENDIF token
              i <- i + 1
          ENDWHILE                              ←─ ENDWHILE token
 ```
 
+STRING and NUMBER literals are made up of a variable number of characters and need to be handled correctly. If the number 3 is found inside of a string, it should be treated as part of the STRING literal and not its own NUMBER literal. Therefore our scanner program will need to treat the same character differently depending on its state such as whether it has seen an opening `"` or `'`. This makes an OOP model a suitable paradigm for implementing a scanner. The NUMBER literals include floats so the scanner should also handle decimal points correctly.
+
 **Table of tokens**
 
 | Token      |         Value         |
 | :--------- | :-------------------: |
 | IDENTIFIER |          'i'          |
 | ASSIGNMENT |                       |
 | NUMBER     |           1           |
@@ -242,42 +408,43 @@
 | IDENTIFIER |          'i'          |
 | ADD        |                       |
 | NUMBER     |           1           |
 | END        |                       |
 | EOF        |                       |
 
 
-**Abstract Syntax Tree**
-
-Looking in the table, the scanner has produced 18 separate tokens including an EOF (End Of File) token. The variable `i` also given a special  IDENTIFIER token. We can use a hashmap  data structure to store the value of `i` as it is incremented at the end of the for loop, so that it is printed correctly on the fifth line.
+Looking in the table, the scanner has produced 18 separate tokens including an EOF (End Of File) token. The variable `i` also given a special IDENTIFIER token. This table is all that is needed for the next stage, parsing.
 
 **Parsing**
 
 The next step is parsing, where we convert the alphabet of tokens into expressions.  This will be modelled using an as an Abstract Syntax Tree (AST). This nesting of the nodes inside a tree allows us to represent the nesting or or `FOR` and `IF` blocks. As well as correctly defining the order of operations of expressions following BIDMAS.
 
 To do this the parser could use two possible methods to recognize the start and end of out `FOR` and `IF` blocks. Method 1 involves counting indentation levels which would require our scanner to emit INDENT tokens matching tab character or spaces. This can be complicated and erroneous where the user inconsistently mixes tabs and spaces. However, it would make the use of `ENFOR` and `ENDIF` keywords optional. 
-To do this the parser could use two possible methods to recognize the start and end of out `FOR` and `IF` blocks. Method 1 involves counting indentation levels which would require our scanner to emit INDENT tokens matching tab character or spaces. This can be complicated and erroneous where the user inconsistently mixes tabs and spaces. However, it would make the use of `ENFOR` and `ENDIF` keywords optional. 
 
-The second method is completely ignoring the indentation and only looking at the `ENDFOR` and `ENDIF` to determine the end of our `FOR` and `IF` blocks. This is simpler and less error-prone as it makes leading spaces or tab optional, but the user can still include them for readability. Therefore, this is the design i'll chose to use.
+The second method is completely ignoring the indentation and only looking at the `ENDFOR` and `ENDIF` to determine the end of our `FOR` and `IF` blocks. This is simpler and a lot easier to implement as we can make leading spaces and tabs insignificant, but the user can still include them for readability. Therefore, this is the design i'll chose to use.
 
 That aside, after parsing our AST looks like this:
 
 ![](assets/syntax_tree_edit.svg)
 
+**syntax tree**
+
 During this stage the parser performs syntactic analysis, mapping tokens to `WHILE` and `IF` The parser sees a `WHILE` token so it knows what follows has to be a condition. Every statement thereafter is nested inside of the `WHILE` block until the parser sees the `ENDWHILE` token, A Tree data structure to represent the order of operations. The final stage is interpreting this tree.
 
-The tree is interpreted from the leaves to the root. The source doe is made up of two statements. The first is the variable declaration `i <- 1` and the next is the `WHILE` loop. The while loop is then made of the condition `i <= 5` and two statements. The two statements are the `IF` statement and another assignment `i <- i + 1`. The `IF` statement also consists of a condition `i = 3`, only a single `=` and not a double `==`. This is because an `<-` is used as the assignment operator, and so the comparison operator hence is a single equal sign, compared to other languages. The `IF` statement has a then and else branch each consisting of a single `OUTPUT` statement. Each construct like the `WHILE` and the `IF` can nest any amount of statements.
+The tree is interpreted from the leaves to the root. The source node is made up of two statements. The first is the variable declaration `i <- 1` and the next is the `WHILE` loop. The while loop is then made of the condition `i <= 5` and two statements. The two statements are the `IF` statement and another assignment `i <- i + 1`. The `IF` statement also consists of a condition `i = 3`, only a single `=` and not a double `==`. This is because an `<-` is used as the assignment operator, and so the comparison operator hence is a single equal sign, compared to other languages. The `IF` statement has a then and else branch each consisting of a single `OUTPUT` statement. Each construct like the `WHILE` and the `IF` can nest any amount of statements.
 
 A symbol table is used to keep track of the `i` variable as its value changes throughout the program. From here instead of traversing the tree and emitting byte code, we'll take a simpler but less efficient approach and run the python equivalent for each statement. So the `OUTPUT` is then mapped to the python `print()` statement.
 
-## Language syntax
+## Language grammar
+
+Backus-naur (BNF) is useful notation for describing the grammar of languages. BNF is a series of rules, consisting of a head and a body making up a production. The head is on the LHS of the `'::='` and the body is on RHS of the `'::='`. A rule can either be *terminal* or *non-terminal*. A *terminal* production matches string literals, number literals or tokens. A *non-terminal* production matches other rules.
 
-Backus-naur (BNF) is useful notation for describing the grammar of languages. BNF is a series of rules, consisting of a head and a body making up a production. The head is on the LHS of the `'::='` and the body is on RHS of the `'::='`. A rule can either be *terminal* or *non-terminal*. A *terminal* production matches string literals, number literals or tokens. A *non-terminal* production matches other rules. Note: keywords are case insensitive so `PRINT` or `print` or any other casing is perfectly valid. Although this gives the user less options for valid variable names, this gives the language more flexibility in the valid source code it accepts. Each BNF statement will be accompanied by a syntax diagram, for a clearer explanation.
+Note: keywords are case insensitive so `PRINT` or `print` or any other casing is perfectly valid. Although this gives the user less options for valid variable names, this gives the language more flexibility in the valid source code it accepts. Each BNF statement will be accompanied by a syntax diagram also known as a railroad diagram, for a clearer explanation.
 
-Moreover the meta-characters `(*)`,  `(?)` and `(|)` will be used. The `(*)` means zero or more, the `(?)` means zero or one and the `(|)` means or.
+The meta-characters `(*)`,  `(?)` and `(|)` are used. The `(*)` means zero or more, the `(?)` means zero or one and the `(|)` means or.
 
 `<program> ::= <declarations> "EOF"`
 
 ![](assets/program.svg)
 
 `<declarations> ::= <declaration>*`
 
@@ -347,16 +514,30 @@
 
 ![](assets/unary.svg)
 
 `<primary> ::=   INTEGER | REAL | STRING | None | True | False | "(" <expression> ")"`
 
 ![](assets/primary.svg)
 
+\pagebreak
+
+## User interface
+
+My program will have two user interfaces: a command line interface as well as a web based ide. The web based ide will need to have an editor and output windows with three buttons. One to run the code, one to server as a link to documentation and another button to toggle between a light and dark theme.
+
+### Online IDE
+
+![prototype of online ide ](assets/website.svg)
+
+The fronted for my online ide will be build in plain html and css. For the backend i'll use fastapi for its type safety. The way it will work is whe  the user enters in code and clicks the 'Run' button, the frontend will send a http `GET` request to the fastapi server, with the body or the request containing the code the user entered in. When the fastapi server receives this response, it will evaluate the AQA pseudo-code and return a response consisted of the output of the code. This output is then displayed in the output window.
 
-## User Interface
+![GET response](assets/server.svg)
+
+
+### CLI interface
 
 My program will have a basic command line interface. It should let the user pick from running the program via the Read Eval Print Loop (REPl), passing in the program as a string, or reading in the program as a file. The program should also display a helpful message when the program is called with the `---help` flag. Below shows a draft of what this might look like.
 
 ``` {.bash .numberLines}
 # display help message
 $ python aqainterpreter.py --help
 Usage: aqainterpreter.py [OPTIONS] [FILENAME]
@@ -382,34 +563,54 @@
 $ python aqainterpreter.py input.txt
 Hi!
 
 # program passed in as a string
 $ python aqainterpreter.py --cmd "OUTPUT 'Hi!'"
 Hi!
 ```
+\pagebreak
 
-# Technical Solution
+## Class, hierarchy diagrams
+
+Below I have produces a class diagram as well a hierarchy chart showing the rough structure of my project.  The code for my project is also available on a public github repo at  [https://github.com/CyberWarrior5466/nea](https://github.com/CyberWarrior5466/nea).
 
 **module hierarchy**
 
-![](assets/packages.svg){ width=30% }
+![Hierarchy diagram](assets/packages.svg){ width=30% }
 
 **Class diagrams**
 
-![](assets/scanner.svg){ width=30% }
-![](assets/parser.svg){ width=20% }
-![](assets/symbol_table.svg){ width=30% }
+![Scanner](assets/scanner.svg){ width=30% }
+![Parser](assets/parser.svg){ width=20% }
+![Symbol Table](assets/symbol_table.svg){ width=30% }
+
+![Class diagram](assets/classes.png)
+
+\pagebreak
+# Technical Solution
+
+## Grade A/B algorithms used
+
+![Table A](assets/table_a.png)
+
+My program uses a number of complex data structures and algorithms involved in translating pseudo-code. A hash table is used in the `SymbolTable` class in the `environment.py` file. which  is used to keep track of variables as the change throughout the execution of an AQA pseudo-code program.
+
+My program uses complex OOP; In `interpreter.py` each class inherits from either the `Expr` of `Stmt` interface. Each class has a `.interpret()` method and the `If` and `While` class call `.interpret()` on their children, which is an example of polymorphism. These classes are instantiated in the `parser.py` file.
 
-![](assets/classes.svg)
+The list operations `.append()` is used on line 17  in `scanner.py`. And the `.extent()` method is used on line 274 in `parse.py`. Complex pattern matching occurs in the `_scan_token()` method on line 48 in `scanner.py` using pythons match statement as described in [addressing redundancy section](#using-match-statement).
 
-## project structure
+![Table B](assets/table_b.png)
+
+AQA pseudo-code is read in from a text file in line 45 and 46 in `main.py`
+
+## Project structure
 
 \TECHNICAL_SOLUTION
 
-## syntax highlighting
+## Syntax highlighting
 
 Another one my clients needs was to produce syntax highlighting for the vscode editor. Due to time limitations, I instead prioritised the syntax highlighting of the code snippets in this document. This document was produced in pandoc which accepts KDE-style XML syntax definition files so I wrote one AQA pseudo-code. Unfortunately I couldn't get comments to work which is why AQA pseudo-code comments appear black in this documents whereas they appear green in python snippets. The XML file below contains regular expressions and is a lot more of a declarative style compared to the tokenizer and parse I wrote in python. In fact its only 114 lines compared to my scanner which is 203.
 
 **aqa.xml**
 ``` {.xml .numberLines}
 <?xml version="1.0" encoding="UTF-8"?>
 <!DOCTYPE language>
@@ -536,158 +737,30 @@
         --pdf-engine=xelatex \
         --table-of-contents \
         --number-sections
 ```
 
 `metedata.yaml` describes extra information such as the headers and footers used in this document. And `aqa.xml` is the KDE style XML file previously.
 
+\pagebreak
 # Testing
 
-To perform quality assurance on my project, I created several unit tests inside of the `test_.py` file. These tests where run using pythons `pytest` library. The `pytest` library automatically runs all functions and files prefixed with `test_` hence the strange name `test_.py`. Here is a more detailed snippet of all the code samples that where used as testing. However as the set of string matched by a context free grammar is infinite, it is impossible to test every pseudo-code input that can be run by my program. Therefore my testing covers the main language features I managed to implement and a couple extra pseudo-code programs that make use of multiple language features at once.
-
-## testing expressions
+To perform quality assurance on my project, I created several unit tests inside of the `test_.py` file. These tests where run using python's `pytest` library. The `pytest` library automatically runs all functions and files prefixed with `test_` hence the strange name `test_.py`. As the set of string matched by a context free grammar is infinite, it is impossible to test every possible pseudo-code combination. Therefore my testing covers the main language features I managed to implement and a couple extra pseudo-code programs that make use of multiple language features at once.
 
-``` {.aqa .numberLines}
-OUTPUT 1 + 1  # 2
-OUTPUT 1 - 1  # 0
-OUTPUT -1     # -1
-OUTPUT 2 * 1  # 2
-OUTPUT 2 × 1  # 2
-OUTPUT 2 / 1  # 2.0
-OUTPUT 2 ÷ 1  # 2.0
-
-OUTPUT "hi" + "÷"  # "hi÷"
-OUTPUT "a" * 3     # "aaa"
-
-OUTPUT 1 > 0    # True
-OUTPUT 1 ≥ 0    # True
-OUTPUT 1 >= 1   # True
-OUTPUT 1 < 0    # False
-OUTPUT 1 ≤ 0    # False
-OUTPUT 1 <= 1   # True
-```
+\TESTS
 
-## testing comments
-``` {.aqa .numberLines}
-# a comments
-```
+Here is a screenshot showing all the tests passing inside of pytest.
 
-## testing assignment
-``` {.aqa .numberLines}
-a <- 0
-a <- a + 1
-OUTPUT a   # 1
-```
-
-## testing assignment
-``` {.aqa .numberLines}
-IF True
-   OUTPUT "yes"
-ENDIF  # yes
-
-IF False
-   OUTPUT "yes"
-ENDIF  # "yes"
-
-IF True
-   IF True
-      OUTPUT "yes"
-   ENDIF
-ENDIF  # "yes"
-```
-
-## testing while loops
-``` {.aqa .numberLines}
-a <- 1
-WHILE a <= 3 DO
-   OUTPUT a
-   a <- a + 1
-ENDWHILE  # 1, 2, 3
-
-# fibonacci sequence
-a <- 1
-b <- 1
-c <- 2
-count <- 0
-WHILE count != 2
-    OUTPUT a
-    a <- b + c
-    OUTPUT b
-    b <- c + a
-    OUTPUT c
-    c <- a + b
-    count <- count + 1
-ENDWHILE  # 1, 1, 2, 3, 5, 8 
-```
-
-## testing for loops
-``` {.aqa .numberLines}
-FOR a <- 1 TO 1
-   OUTPUT a
-ENDFOR # 1
-
-FOR a <- 1 TO 1 STEP 1
-   OUTPUT a
-ENDFOR # 1
-
-FOR a <- 1 TO 1 STEP -1
-   OUTPUT a
-ENDFOR # 1
-
-FOR a <- 1 TO 3
-   OUTPUT a
-ENDFOR # 1, 2, 3
-
-FOR a <- 1 TO 3 STEP 1
-   OUTPUT a
-ENDFOR # 1, 2, 3
-
-FOR a <- 3 TO 1
-   OUTPUT a
-ENDFOR # 3, 2, 1
-
-FOR a <- 3 TO 1 STEP -1
-   OUTPUT a
-ENDFOR # 3, 2, 1
-
-FOR a <- 1 TO 5 STEP 2
-   OUTPUT a
-ENDFOR # 1, 3, 5
-
-FOR a <- 5 TO 1 STEP -2
-   OUTPUT a
-ENDFOR # 5, 3, 1
-
-FOR a <- 1 TO 2
-   FOR b <- 1 TO 2
-       OUTPUT a
-       OUTPUT b
-       OUTPUT ''
-   ENDFOR
-ENDFOR  # 1,1  1,2  2,1  2,2
-
-FOR a <- 1 TO 12
-    FOR b <- 1 TO 12
-        OUTPUT a + " × " + b + " = " + (a * b)
-    END
-END
-# 1 × 1 = 1
-# 1 × 2 = 2
-# 1 × 3 = 3
-# 1 × 4 = 4
-# 1 × 5 = 5
-# 1 × 6 = 6
-# ... all the times tables up to 12 × 12
-```
+![Pytest output](assets/pytest.png)
 
 ## Tokens and AST
 
-Here are the tokens and the ast generated by my program for a couple of the tests as showing them all would be too long.
+My program has an optional `--debug`. When this flag is passed the list of tokens and the Abstract Syntax Tree is also printed in addition to the normal output of the program. Showing the tokens list and AST for every one of my units tests would be tedious, so below is a sample of three programs.
 
-### program 1
+### Example program 1
 
 ``` {.aqa .numberLines}
 OUTPUT 1 + 2 * 3
 ```
 
 **tokens**
 ``` {.python .numberLines}
@@ -713,15 +786,15 @@
                 right=Literal(value=3),
             ),
         )
     )
 ]
 ```
 
-### program 2
+### Example program 2
 
 ``` {.aqa .numberLines}
 IF True
    IF True
       OUTPUT "yes"
    ENDIF
 ENDIF
@@ -753,15 +826,15 @@
             )
         ],
         else_branch=[],
     )
 ]
 ```
 
-### program 3
+### Example program 3
 
 ``` {.aqa .numberLines}
 FOR a <- 1 TO 12
     FOR b <- 1 TO 12
         OUTPUT a + " × " + b + " = " + (a * b)
     END
 END
@@ -886,18 +959,67 @@
                 ),
             ),
         ],
     ),
 ]
 ```
 
+\pagebreak
 
 # Evaluation
 
-My program achieves a large number of my project requirements so I consider it a success. The first objective was partially met. I implemented `WHILE`, `FOR` and `IF` statements but missed out on `REPEAT`, `RECORD` and `SUBROUTINE` statements. I also didn't implement any of the functions including the call stack but i did have all the data types. Another thing that is missing where constants and arrays.
+
+## [Project Requirements](#project-requirements)
+
+**The requirements for this project are repeated again here so you do not have to flick back to the analysis section.**
+
+1. Create a tree-walk interpreter for all the features in AQA's 'pseudo-code' command set including but not limited to: 
+   
+   - `REPEAT`, `WHILE`, `FOR`, `IF`, `RECORD`, `SUBROUTINE` constructs
+   
+   - `INPUT`, `OUTPUT`, `LEN`, `POSITION`, `SUBSTRING`, `RANDOM_INT` functions
+   
+   - `STRING`, `INT`, `REAL`, `BOOL` types
+   
+   - `INPUT`, `OUTPUT` operations
+   
+   - variables, constants and arrays
+   
+   If it is not possible to implement all of these features, the the language should at least be Turing complete. For a language to be considered Turing complete it needs at lease arithmetic operations, control flow (`WHILE` / `REPEAT` loops), and access to arbitrary memory (arrays)
+
+2. Additionally I would like to make keywords case insensitive giving the use the ability to style code to his preference.
+
+3. The program should accept a large range of input. For example the 'pseudo-code' command set uses the unicode multiply sign `(×)` whereas most programming languages use an `(*)` as it can be typed on a traditional keyboard. My program should accept both of these symbols, making it adaptable. A table of these special symbols is show below.
+   
+   | Traditional | Unicode |
+   | :---------: | :-----: |
+   |      *      |    ×    |
+   |      /      |    ÷    |
+   |     !=      |  `!=`   |
+   |     <=      |  `<=`   |
+   |     >=      |  `>=`   |
+   |     <-      |   `←`   |
+
+4. Robust error handling, informing the user of what line syntax errors have occurred.
+
+5. Create on online IDE for users to quickly try out the language without having to install any extra language tools their local machine.
+
+6. Add syntax highlighting to highlight keywords and constructs, following the colours of the atom text editor, as it was my clients preference. 
+
+----
+
+## Assessing whether the requirements where met
+
+My program achieves a large number of my project requirements so overall I consider it a success. 
+
+1. The first objective was partially met. I implemented `WHILE`, `FOR` and `IF` statements but missed out on `REPEAT`, `RECORD` and `SUBROUTINE` statements. A `REPEAT` loop is just syntactic sugar for a `WHILE` loop where the condition is evaluated at the end instead of at the start, so i would argue this objective was not paramount. 
+   
+   No `SUBROUTINE` or function logic was implemented which would of required the use of requires using a call stack. None of the functions where implemented which would of additionally required implementing a call stack. All of the data types where implemented being based of python's builting types.
+   
+   variables 
 Since I din't implement arrays, my solution wasn't turning complete, but it did feature control flow so at least we where half way there.
 
 My project was expressive enough to write some novel programs such a fibonacci sequence and display the times tables. And I successfully implemented a scanner, parser and a tree-walk interpreter.
 
 Objective two and three where met fully. My program has case insensitive keywords due to the `.lower()` in `self.source[self._start : self._current].lower()` in `scanner.py` on line 160. The capitalisation of all the keywords in this documents was purely stylistic. Objective three was also fully met, due to more effort in `scanner.py`. Infant there aren't any other languages that support special symbols like `<-`, `<=`, `!=`, `÷` unless you use a special font with ligatures. The support of these symbols means my projects is more suitable for the source code to be printed.
 
 Objective 4 was also met. My program shows helpful error messages. For example if the user entered:
@@ -969,8 +1091,7 @@
 </html>
 ```
 
 ![](assets/screenshot3.png)
 
 
 Objective 6 was also met as you can have no doubt seen the syntax highlighting for AQA code snippets many times in this document. The code for which is also explained in the technical solution.
-
```

### Comparing `aqainterpreter-0.0.7/report/assets/classes.svg` & `aqainterpreter-0.0.8/report/assets/classes.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.7/report/assets/comparison.svg` & `aqainterpreter-0.0.8/report/assets/comparison.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.7/report/assets/compiler.svg` & `aqainterpreter-0.0.8/report/assets/compiler.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.7/report/assets/declaration.svg` & `aqainterpreter-0.0.8/report/assets/declaration.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.7/report/assets/declarations.svg` & `aqainterpreter-0.0.8/report/assets/declarations.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.7/report/assets/end.svg` & `aqainterpreter-0.0.8/report/assets/end.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.7/report/assets/equality.svg` & `aqainterpreter-0.0.8/report/assets/equality.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.7/report/assets/expression.svg` & `aqainterpreter-0.0.8/report/assets/expression.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.7/report/assets/factor.svg` & `aqainterpreter-0.0.8/report/assets/factor.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.7/report/assets/for.svg` & `aqainterpreter-0.0.8/report/assets/for.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.7/report/assets/if.svg` & `aqainterpreter-0.0.8/report/assets/if.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.7/report/assets/logic_and.svg` & `aqainterpreter-0.0.8/report/assets/logic_and.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.7/report/assets/logic_or.svg` & `aqainterpreter-0.0.8/report/assets/logic_or.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.7/report/assets/packages.svg` & `aqainterpreter-0.0.8/report/assets/packages.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.7/report/assets/parser.svg` & `aqainterpreter-0.0.8/report/assets/parser.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.7/report/assets/primary.svg` & `aqainterpreter-0.0.8/report/assets/primary.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.7/report/assets/print.svg` & `aqainterpreter-0.0.8/report/assets/print.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.7/report/assets/program.svg` & `aqainterpreter-0.0.8/report/assets/program.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.7/report/assets/scanner.svg` & `aqainterpreter-0.0.8/report/assets/scanner.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.7/report/assets/screenshot1.png` & `aqainterpreter-0.0.8/report/assets/screenshot1.png`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.7/report/assets/screenshot2.png` & `aqainterpreter-0.0.8/report/assets/screenshot2.png`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.7/report/assets/screenshot3.png` & `aqainterpreter-0.0.8/report/assets/screenshot3.png`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.7/report/assets/statement.svg` & `aqainterpreter-0.0.8/report/assets/statement.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.7/report/assets/symbol_table.svg` & `aqainterpreter-0.0.8/report/assets/symbol_table.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.7/report/assets/syntax_tree.svg` & `aqainterpreter-0.0.8/report/assets/syntax_tree.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.7/report/assets/syntax_tree_edit.svg` & `aqainterpreter-0.0.8/report/assets/syntax_tree_edit.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.7/report/assets/term.svg` & `aqainterpreter-0.0.8/report/assets/term.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.7/report/assets/unary.svg` & `aqainterpreter-0.0.8/report/assets/unary.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.7/report/assets/variable_declaration.svg` & `aqainterpreter-0.0.8/report/assets/variable_declaration.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.7/report/assets/while.svg` & `aqainterpreter-0.0.8/report/assets/while.svg`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.7/report/assets/input/classes.mmd` & `aqainterpreter-0.0.8/report/assets/input/classes.mmd`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.7/report/assets/input/comparison.pikchr` & `aqainterpreter-0.0.8/report/assets/input/comparison.pikchr`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.7/report/assets/input/declaration.pikchr` & `aqainterpreter-0.0.8/report/assets/input/declaration.pikchr`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.7/report/assets/input/end.pikchr` & `aqainterpreter-0.0.8/report/assets/input/end.pikchr`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.7/report/assets/input/equality.pikchr` & `aqainterpreter-0.0.8/report/assets/input/equality.pikchr`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.7/report/assets/input/factor.pikchr` & `aqainterpreter-0.0.8/report/assets/input/factor.pikchr`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.7/report/assets/input/for.pikchr` & `aqainterpreter-0.0.8/report/assets/input/for.pikchr`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.7/report/assets/input/if.pikchr` & `aqainterpreter-0.0.8/report/assets/input/if.pikchr`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.7/report/assets/input/logic_and.pikchr` & `aqainterpreter-0.0.8/report/assets/input/logic_and.pikchr`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.7/report/assets/input/logic_or.pikchr` & `aqainterpreter-0.0.8/report/assets/input/logic_or.pikchr`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.7/report/assets/input/packages.mmd` & `aqainterpreter-0.0.8/report/assets/input/packages.mmd`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.7/report/assets/input/primary.pikchr` & `aqainterpreter-0.0.8/report/assets/input/primary.pikchr`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.7/report/assets/input/statement.pikchr` & `aqainterpreter-0.0.8/report/assets/input/statement.pikchr`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.7/report/assets/input/term.pikchr` & `aqainterpreter-0.0.8/report/assets/input/term.pikchr`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.7/report/assets/input/unary.pikchr` & `aqainterpreter-0.0.8/report/assets/input/unary.pikchr`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.7/report/assets/input/while.pikchr` & `aqainterpreter-0.0.8/report/assets/input/while.pikchr`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.7/LICENSE` & `aqainterpreter-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `aqainterpreter-0.0.7/pyproject.toml` & `aqainterpreter-0.0.8/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "AQAInterpreter"
 requires-python = ">=3.10"
 license = "MIT"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name = "CyberWarrior5466", email = "asaleen898@gmail.com" },
 ]
 dependencies = ["click==8.*"]
 
 [project.urls]
 Documentation = "https://github.com/CyberWarrior5466/nea"
 Issues = "https://github.com/CyberWarrior5466/nea/issues"
 Source = "https://github.com/CyberWarrior5466/nea"
 
 
 [tool.hatch.envs.default]
-dependencies = ["black", "inotify", "pytest"]
+dependencies = ["pytest"]
```

