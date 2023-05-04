# Comparing `tmp/trlc-1.1.1.tar.gz` & `tmp/trlc-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trlc-1.1.1.tar", last modified: Fri Apr 28 09:17:19 2023, max compression
+gzip compressed data, was "trlc-1.1.2.tar", last modified: Thu May  4 13:51:37 2023, max compression
```

## Comparing `trlc-1.1.1.tar` & `trlc-1.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-04-28 09:17:19.584583 trlc-1.1.1/
--rw-r--r--   0 florian   (1000) florian   (1000)    35149 2022-12-05 12:42:52.000000 trlc-1.1.1/LICENSE
--rw-r--r--   0 florian   (1000) florian   (1000)     2965 2023-04-28 09:17:19.584583 trlc-1.1.1/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)     1875 2023-03-01 10:58:12.000000 trlc-1.1.1/README.md
--rw-r--r--   0 florian   (1000) florian   (1000)      103 2023-04-28 09:17:19.584583 trlc-1.1.1/setup.cfg
--rw-r--r--   0 florian   (1000) florian   (1000)     2135 2023-02-21 07:05:56.000000 trlc-1.1.1/setup.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-04-28 09:17:19.584583 trlc-1.1.1/trlc/
--rw-r--r--   0 florian   (1000) florian   (1000)      815 2022-12-05 12:42:52.000000 trlc-1.1.1/trlc/__init__.py
--rw-r--r--   0 florian   (1000) florian   (1000)    96271 2023-04-28 09:15:42.000000 trlc-1.1.1/trlc/ast.py
--rw-r--r--   0 florian   (1000) florian   (1000)     7240 2023-04-12 08:39:07.000000 trlc-1.1.1/trlc/errors.py
--rw-r--r--   0 florian   (1000) florian   (1000)    15405 2023-04-28 09:15:42.000000 trlc-1.1.1/trlc/lexer.py
--rw-r--r--   0 florian   (1000) florian   (1000)     2475 2023-04-28 09:15:42.000000 trlc-1.1.1/trlc/lint.py
--rw-r--r--   0 florian   (1000) florian   (1000)     1266 2023-03-23 13:32:34.000000 trlc-1.1.1/trlc/math.py
--rw-r--r--   0 florian   (1000) florian   (1000)     3351 2023-03-23 13:32:34.000000 trlc-1.1.1/trlc/nested.py
--rw-r--r--   0 florian   (1000) florian   (1000)    58600 2023-04-28 09:15:42.000000 trlc-1.1.1/trlc/parser.py
--rw-r--r--   0 florian   (1000) florian   (1000)    16319 2023-04-28 09:15:42.000000 trlc-1.1.1/trlc/trlc.py
--rw-r--r--   0 florian   (1000) florian   (1000)     1004 2023-04-28 09:17:12.000000 trlc-1.1.1/trlc/version.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-04-28 09:17:19.584583 trlc-1.1.1/trlc.egg-info/
--rw-r--r--   0 florian   (1000) florian   (1000)     2965 2023-04-28 09:17:19.000000 trlc-1.1.1/trlc.egg-info/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)      322 2023-04-28 09:17:19.000000 trlc-1.1.1/trlc.egg-info/SOURCES.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-04-28 09:17:19.000000 trlc-1.1.1/trlc.egg-info/dependency_links.txt
--rw-r--r--   0 florian   (1000) florian   (1000)       40 2023-04-28 09:17:19.000000 trlc-1.1.1/trlc.egg-info/entry_points.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        5 2023-04-28 09:17:19.000000 trlc-1.1.1/trlc.egg-info/top_level.txt
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-04 13:51:37.084142 trlc-1.1.2/
+-rw-r--r--   0 florian   (1000) florian   (1000)    35149 2022-12-05 12:42:52.000000 trlc-1.1.2/LICENSE
+-rw-r--r--   0 florian   (1000) florian   (1000)     2965 2023-05-04 13:51:37.084142 trlc-1.1.2/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)     1875 2023-03-01 10:58:12.000000 trlc-1.1.2/README.md
+-rw-r--r--   0 florian   (1000) florian   (1000)      103 2023-05-04 13:51:37.084142 trlc-1.1.2/setup.cfg
+-rw-r--r--   0 florian   (1000) florian   (1000)     2135 2023-02-21 07:05:56.000000 trlc-1.1.2/setup.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-04 13:51:37.084142 trlc-1.1.2/trlc/
+-rw-r--r--   0 florian   (1000) florian   (1000)      815 2022-12-05 12:42:52.000000 trlc-1.1.2/trlc/__init__.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    96418 2023-05-04 13:51:21.000000 trlc-1.1.2/trlc/ast.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     7240 2023-04-12 08:39:07.000000 trlc-1.1.2/trlc/errors.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    15521 2023-05-04 13:51:21.000000 trlc-1.1.2/trlc/lexer.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     2475 2023-04-28 09:15:42.000000 trlc-1.1.2/trlc/lint.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     1266 2023-03-23 13:32:34.000000 trlc-1.1.2/trlc/math.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     3351 2023-03-23 13:32:34.000000 trlc-1.1.2/trlc/nested.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    58761 2023-05-04 13:51:21.000000 trlc-1.1.2/trlc/parser.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    16319 2023-04-28 09:15:42.000000 trlc-1.1.2/trlc/trlc.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     1004 2023-05-04 13:51:32.000000 trlc-1.1.2/trlc/version.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-04 13:51:37.084142 trlc-1.1.2/trlc.egg-info/
+-rw-r--r--   0 florian   (1000) florian   (1000)     2965 2023-05-04 13:51:37.000000 trlc-1.1.2/trlc.egg-info/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)      322 2023-05-04 13:51:37.000000 trlc-1.1.2/trlc.egg-info/SOURCES.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-05-04 13:51:37.000000 trlc-1.1.2/trlc.egg-info/dependency_links.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)       40 2023-05-04 13:51:37.000000 trlc-1.1.2/trlc.egg-info/entry_points.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        5 2023-05-04 13:51:37.000000 trlc-1.1.2/trlc.egg-info/top_level.txt
```

### Comparing `trlc-1.1.1/LICENSE` & `trlc-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `trlc-1.1.1/PKG-INFO` & `trlc-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trlc
-Version: 1.1.1
+Version: 1.1.2
 Summary: Treat Requirements Like Code
 Home-page: https://github.com/bmw-software-engineering/trlc
 Author: Bayerische Motoren Werke Aktiengesellschaft (BMW AG)
 Author-email: florian.schanda@bmw.de
 License: GNU General Public License v3
 Project-URL: Bug Tracker, https://github.com/bmw-software-engineering/trlc/issues
 Project-URL: Documentation, https://github.com/pages/bmw-software-engineering/trlc/
```

### Comparing `trlc-1.1.1/README.md` & `trlc-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `trlc-1.1.1/setup.py` & `trlc-1.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `trlc-1.1.1/trlc/__init__.py` & `trlc-1.1.2/trlc/__init__.py`

 * *Files identical despite different names*

### Comparing `trlc-1.1.1/trlc/ast.py` & `trlc-1.1.2/trlc/ast.py`

 * *Files 0% similar despite different names*

```diff
@@ -523,15 +523,15 @@
 
     def evaluate(self, mh, context):
         assert isinstance(mh, Message_Handler)
         assert context is None or isinstance(context, dict)
         return Value(self.location, self.value, self.typ)
 
     def to_python_object(self):
-        return self.value
+        return float(self.value)
 
 
 class String_Literal(Literal):
     """String literals
 
     Note the value of the string does not include the quotation marks,
     and any escape sequences are fully resolved. For example::
@@ -2305,15 +2305,17 @@
 
     :attribute token: token used to separate fields of the tuple
     :type: Token
     """
     def __init__(self, token):
         super().__init__(token.location)
         assert isinstance(token, Token) and token.kind in ("IDENTIFIER",
-                                                           "AT")
+                                                           "AT",
+                                                           "COLON",
+                                                           "SEMICOLON")
         self.token = token
 
     def dump(self, indent=0):  # pragma: no cover
         self.write_indent(indent, "Separator %s" % self.token.value)
 
 
 class Enumeration_Type(Concrete_Type):
```

### Comparing `trlc-1.1.1/trlc/errors.py` & `trlc-1.1.2/trlc/errors.py`

 * *Files identical despite different names*

### Comparing `trlc-1.1.1/trlc/lexer.py` & `trlc-1.1.2/trlc/lexer.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,14 +122,16 @@
                       "BUILTIN",
                       "KEYWORD",
                       "BRA", "KET",
                       "S_BRA", "S_KET",
                       "C_BRA", "C_KET",
                       "AT",
                       "COMMA",
+                      "SEMICOLON",
+                      "COLON",
                       "DOT",
                       "RANGE",
                       "ASSIGN",
                       "OPERATOR",
                       "ARROW",
                       "INTEGER",
                       "DECIMAL",
@@ -259,14 +261,16 @@
         ")" : "KET",
         "{" : "C_BRA",
         "}" : "C_KET",
         "[" : "S_BRA",
         "]" : "S_KET",
         "," : "COMMA",
         "@" : "AT",
+        ":" : "COLON",
+        ";" : "SEMICOLON",
         "/" : "OPERATOR",
         "%" : "OPERATOR",
         "+" : "OPERATOR",
         "-" : "OPERATOR",
     }
 
     def __init__(self, mh, file_name, file_content=None):
```

### Comparing `trlc-1.1.1/trlc/lint.py` & `trlc-1.1.2/trlc/lint.py`

 * *Files identical despite different names*

### Comparing `trlc-1.1.1/trlc/math.py` & `trlc-1.1.2/trlc/math.py`

 * *Files identical despite different names*

### Comparing `trlc-1.1.1/trlc/nested.py` & `trlc-1.1.2/trlc/nested.py`

 * *Files identical despite different names*

### Comparing `trlc-1.1.1/trlc/parser.py` & `trlc-1.1.2/trlc/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -405,15 +405,18 @@
             if has_separators or self.peek_kw("separator"):
                 has_separators = True
                 self.match_kw("separator")
                 if not separator_allowed:
                     self.mh.error(self.ct.location,
                                   "either all fields must be separated,"
                                   " or none")
-                if self.peek("IDENTIFIER") or self.peek("AT"):
+                if self.peek("IDENTIFIER") or \
+                   self.peek("AT") or \
+                   self.peek("COLON") or \
+                   self.peek("SEMICOLON"):
                     self.advance()
                     n_tuple.add_separator(ast.Separator(self.ct))
             else:
                 separator_allowed = False
             n_field = self.parse_tuple_field(
                 n_tuple,
                 optional_allowed  = has_separators,
@@ -1349,17 +1352,17 @@
             for n_item in typ.iter_sequence():
                 if isinstance(n_item, ast.Composite_Component):
                     if next_is_optional and n_item.optional:
                         break
                     rv.assign(n_item.name,
                               self.parse_value(n_item.n_typ))
 
-                elif n_item.token.kind == "AT":
-                    if self.peek("AT"):
-                        self.match("AT")
+                elif n_item.token.kind in ("AT", "COLON", "SEMICOLON"):
+                    if self.peek(n_item.token.kind):
+                        self.match(n_item.token.kind)
                     else:
                         next_is_optional = True
 
                 elif n_item.token.kind == "IDENTIFIER":
                     if self.peek("IDENTIFIER") and \
                        self.nt.value == n_item.token.value:
                         self.match("IDENTIFIER")
```

### Comparing `trlc-1.1.1/trlc/trlc.py` & `trlc-1.1.2/trlc/trlc.py`

 * *Files identical despite different names*

### Comparing `trlc-1.1.1/trlc/version.py` & `trlc-1.1.2/trlc/version.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,14 @@
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY
 # or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public
 # License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with TRLC. If not, see <https://www.gnu.org/licenses/>.
 
-VERSION_TUPLE = (1, 1, 1)
+VERSION_TUPLE = (1, 1, 2)
 VERSION_SUFFIX = ""
 
 TRLC_VERSION = ("%u.%u.%u" % VERSION_TUPLE) + \
     ("-%s" % VERSION_SUFFIX if VERSION_SUFFIX else "")
 
 FULL_NAME = "TRLC %s" % TRLC_VERSION
```

### Comparing `trlc-1.1.1/trlc.egg-info/PKG-INFO` & `trlc-1.1.2/trlc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trlc
-Version: 1.1.1
+Version: 1.1.2
 Summary: Treat Requirements Like Code
 Home-page: https://github.com/bmw-software-engineering/trlc
 Author: Bayerische Motoren Werke Aktiengesellschaft (BMW AG)
 Author-email: florian.schanda@bmw.de
 License: GNU General Public License v3
 Project-URL: Bug Tracker, https://github.com/bmw-software-engineering/trlc/issues
 Project-URL: Documentation, https://github.com/pages/bmw-software-engineering/trlc/
```

