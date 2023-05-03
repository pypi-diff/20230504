# Comparing `tmp/rumex-0.4.0.tar.gz` & `tmp/rumex-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rumex-0.4.0.tar", max compression
+gzip compressed data, was "rumex-0.5.0.tar", max compression
```

## Comparing `rumex-0.4.0.tar` & `rumex-0.5.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0     1211 2022-10-01 01:54:46.296415 rumex-0.4.0/LICENSE
--rw-r--r--   0        0        0     1520 2023-04-23 22:18:05.688768 rumex-0.4.0/README.rst
--rw-r--r--   0        0        0      916 2023-04-29 00:59:13.547098 rumex-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      133 2023-04-29 00:59:13.547098 rumex-0.4.0/rumex/__init__.py
--rw-r--r--   0        0        0        0 2022-10-01 01:54:46.296415 rumex-0.4.0/rumex/parsing/__init__.py
--rw-r--r--   0        0        0     3271 2023-04-29 00:56:28.948481 rumex-0.4.0/rumex/parsing/builder.py
--rw-r--r--   0        0        0      947 2023-04-29 00:56:28.948481 rumex-0.4.0/rumex/parsing/core.py
--rw-r--r--   0        0        0     8365 2023-04-29 00:56:28.948481 rumex-0.4.0/rumex/parsing/parser.py
--rw-r--r--   0        0        0      990 2023-04-04 00:34:13.843051 rumex-0.4.0/rumex/parsing/table.py
--rw-r--r--   0        0        0     2642 2023-04-29 00:56:28.948481 rumex-0.4.0/rumex/parsing/tokenizer.py
--rw-r--r--   0        0        0    11047 2023-04-29 00:56:28.948481 rumex-0.4.0/rumex/runner.py
--rw-r--r--   0        0        0     1423 2023-04-23 21:55:25.650645 rumex-0.4.0/rumex/tests/__init__.py
--rw-r--r--   0        0        0     4206 2023-04-23 21:55:25.650645 rumex-0.4.0/rumex/tests/test_data.py
--rw-r--r--   0        0        0      810 2023-04-04 00:34:13.843051 rumex-0.4.0/rumex/tests/test_error_reporting.py
--rw-r--r--   0        0        0     5554 2023-04-24 20:26:14.685112 rumex-0.4.0/rumex/tests/test_no_execution_cases.py
--rw-r--r--   0        0        0     6710 2023-04-29 00:56:28.948481 rumex-0.4.0/rumex/tests/test_simple_execution.py
--rw-r--r--   0        0        0      894 2023-02-16 02:20:09.255404 rumex-0.4.0/rumex/utils.py
--rw-r--r--   0        0        0     1851 1970-01-01 00:00:00.000000 rumex-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1211 2022-10-01 01:54:46.296415 rumex-0.5.0/LICENSE
+-rw-r--r--   0        0        0     1520 2023-04-23 22:18:05.688768 rumex-0.5.0/README.rst
+-rw-r--r--   0        0        0      916 2023-05-03 23:39:13.199906 rumex-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      133 2023-05-03 23:39:13.199906 rumex-0.5.0/rumex/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-01 01:54:46.296415 rumex-0.5.0/rumex/parsing/__init__.py
+-rw-r--r--   0        0        0     3493 2023-05-03 23:39:13.199906 rumex-0.5.0/rumex/parsing/builder.py
+-rw-r--r--   0        0        0     1032 2023-05-03 23:39:13.199906 rumex-0.5.0/rumex/parsing/core.py
+-rw-r--r--   0        0        0     8906 2023-05-03 23:39:13.199906 rumex-0.5.0/rumex/parsing/parser.py
+-rw-r--r--   0        0        0      990 2023-05-02 00:37:46.737147 rumex-0.5.0/rumex/parsing/table.py
+-rw-r--r--   0        0        0     2797 2023-05-03 23:39:13.199906 rumex-0.5.0/rumex/parsing/tokenizer.py
+-rw-r--r--   0        0        0    13747 2023-05-03 23:39:13.199906 rumex-0.5.0/rumex/runner.py
+-rw-r--r--   0        0        0     1423 2023-04-23 21:55:25.650645 rumex-0.5.0/rumex/tests/__init__.py
+-rw-r--r--   0        0        0     4206 2023-04-23 21:55:25.650645 rumex-0.5.0/rumex/tests/test_data.py
+-rw-r--r--   0        0        0      810 2023-04-04 00:34:13.843051 rumex-0.5.0/rumex/tests/test_error_reporting.py
+-rw-r--r--   0        0        0     2749 2023-05-03 23:39:13.199906 rumex-0.5.0/rumex/tests/test_execution.py
+-rw-r--r--   0        0        0     5554 2023-04-24 20:26:14.685112 rumex-0.5.0/rumex/tests/test_no_execution_cases.py
+-rw-r--r--   0        0        0     6717 2023-05-03 23:39:13.199906 rumex-0.5.0/rumex/tests/test_simple_execution.py
+-rw-r--r--   0        0        0      894 2023-02-16 02:20:09.255404 rumex-0.5.0/rumex/utils.py
+-rw-r--r--   0        0        0     1851 1970-01-01 00:00:00.000000 rumex-0.5.0/PKG-INFO
```

### Comparing `rumex-0.4.0/LICENSE` & `rumex-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rumex-0.4.0/README.rst` & `rumex-0.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `rumex-0.4.0/pyproject.toml` & `rumex-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rumex"
-version = "0.4.0"
+version = "0.5.0"
 
 description = ""
 authors = ["uigctaw <uigctaw@metadata.social>"]
 readme = "README.rst"
 
 
 [tool.poetry.dependencies]
```

### Comparing `rumex-0.4.0/rumex/parsing/builder.py` & `rumex-0.5.0/rumex/parsing/builder.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,16 @@
         row = parse_table_line(line, delimiter='|')
         if self._header is None:
             self._header = row
         else:
             self._data.append(row)
 
     def get_built(self):
-        return tuple(dict(zip(self._header, row)) for row in self._data)
+        header = self._header or []
+        return tuple(dict(zip(header, row)) for row in self._data)
 
 
 class TextBlockBuilder:
 
     def __init__(self):
         self._lines = []
 
@@ -69,34 +70,38 @@
 class ScenarioBuilder:
 
     def __init__(self, name):
         self.name = name
         self._step_builders = []
         self.description = []
         self.tags = []
+        self._examples_builder = TableBuilder()
 
     @property
     def current_step_builder(self):
         return self._step_builders[-1]
 
     def new_step(self, sentence):
         self._step_builders.append(StepBuilder(sentence))
 
+    def add_example(self, line):
+        self._examples_builder.consume(line)
+
     def get_built(self):
         if self.description:
             formatted_description = textwrap.dedent(
                     '\n'.join(self.description)).strip()
         else:
             formatted_description = None
-
         return Scenario(
                 name=self.name,
                 description=formatted_description,
                 steps=[builder.get_built() for builder in self._step_builders],
                 tags=tuple(self.tags),
+                examples_data=self._examples_builder.get_built(),
         )
 
 
 class FileBuilder:
 
     def __init__(self):
         self.name = None
```

### Comparing `rumex-0.4.0/rumex/parsing/core.py` & `rumex-0.5.0/rumex/parsing/core.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,31 +22,32 @@
     text: str
 
 
 @dataclass(frozen=True, kw_only=True)
 class Step:
 
     sentence: str
-    data: type
+    data: Sequence[dict[str, str]]
 
 
 @dataclass(frozen=True, kw_only=True)
 class Scenario:
 
     name: str
-    description: str
+    description: str | None
     steps: Sequence[Step]
     tags: Sequence[str]
+    examples_data: Sequence[dict[str, str]]
 
 
 @dataclass(frozen=True, kw_only=True)
 class ParsedFile:
 
-    name: str
-    description: str
+    name: str | None
+    description: str | None
     scenarios: Sequence[Scenario]
     uri: str
 
 
 class ParserProto(Protocol):
 
     def __call__(self, input_file: InputFile, /) -> ParsedFile:
```

### Comparing `rumex-0.4.0/rumex/parsing/parser.py` & `rumex-0.5.0/rumex/parsing/parser.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     FILE_NAME = auto()
     FILE_DESCRIPTION = auto()
     SCENARIO = auto()
     SCENARIO_WO_NAME = auto()
     STEP = auto()
     BLOCK_OF_TEXT = auto()
     SCENARIO_DESCRIPTION = auto()
+    SCENARIO_EXAMPLES = auto()
 
 
 class StateMachine(Mapping):
     """Represents possible states of a parser.
 
     This object is a map where keys are `State` enumerals
     and values are maps where keys are `TokenKind` enumerals
@@ -102,14 +103,18 @@
     builder.current_scenario_builder.description.append(line)
 
 
 def add_step_data(builder, data):
     builder.current_scenario_builder.current_step_builder.add_step_data(data)
 
 
+def add_scenario_example(builder, data):
+    builder.current_scenario_builder.add_example(data)
+
+
 def add_text_block_line(builder, line):
     builder.current_scenario_builder.current_step_builder.add_text_block_line(
             line)
 
 
 default_state_machine = StateMachine({
     State.START: {
@@ -187,14 +192,23 @@
         TokenKind.STEP_KW: (State.STEP, new_step),
         TokenKind.DESCRIPTION: (State.STEP, add_step_data),
         TokenKind.TRIPLE_QUOTE: (State.BLOCK_OF_TEXT, no_op),
         TokenKind.BLANK_LINE: (State.STEP, no_op),
         TokenKind.SCENARIO_KW: (State.SCENARIO, new_scenario_from_name),
         TokenKind.SCENARIO_TAG: (
             State.SCENARIO_WO_NAME, new_scenario_from_tag),
+        TokenKind.EXAMPLES: (State.SCENARIO_EXAMPLES, no_op),
+    },
+
+    State.SCENARIO_EXAMPLES: {
+        TokenKind.DESCRIPTION: (State.SCENARIO_EXAMPLES, add_scenario_example),
+        TokenKind.BLANK_LINE: (State.SCENARIO_EXAMPLES, no_op),
+        TokenKind.SCENARIO_KW: (State.SCENARIO, new_scenario_from_name),
+        TokenKind.SCENARIO_TAG: (
+            State.SCENARIO_WO_NAME, new_scenario_from_tag),
     },
 
     State.BLOCK_OF_TEXT: {
             kind: (State.BLOCK_OF_TEXT, add_text_block_line)
             for kind in TokenKind if kind != TokenKind.TRIPLE_QUOTE
     } | {TokenKind.TRIPLE_QUOTE: (State.SCENARIO, no_op)},
 })
```

### Comparing `rumex-0.4.0/rumex/parsing/table.py` & `rumex-0.5.0/rumex/parsing/table.py`

 * *Files identical despite different names*

### Comparing `rumex-0.4.0/rumex/parsing/tokenizer.py` & `rumex-0.5.0/rumex/parsing/tokenizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     NAME_KW = auto()
     SCENARIO_KW = auto()
     STEP_KW = auto()
     BLANK_LINE = auto()
     DESCRIPTION = auto()
     TRIPLE_QUOTE = auto()
     SCENARIO_TAG = auto()
+    EXAMPLES = auto()
 
 
 @dataclass(frozen=True, kw_only=True)
 class Token:
     """Every line must map to a `Token`."""
 
     kind: Hashable
@@ -51,14 +52,19 @@
 
 
 def match_name(line):
     if name := match_keyword('Name', line=line):
         return TokenKind.NAME_KW, name
 
 
+def match_examples(line):
+    if re.match(r'^\s*Examples:\s*$', line):
+        return TokenKind.EXAMPLES, None
+
+
 def match_triple_quote(line):
     if line.strip() == '"""':
         return TokenKind.TRIPLE_QUOTE, None
 
 
 def match_step(line):
     stripped = line.strip()
@@ -95,14 +101,15 @@
 
 default_tokenizers = Tokenizers(
     match_triple_quote,
     match_name,
     match_scenario_tag,
     match_scenario,
     match_step,
+    match_examples,
     match_blank_line,
     match_description,
 )
 
 
 def iter_tokens(text, tokenizers=default_tokenizers):
     for i, line in enumerate(text.splitlines()):
```

### Comparing `rumex-0.4.0/rumex/runner.py` & `rumex-0.5.0/rumex/runner.py`

 * *Files 14% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 @dataclass(frozen=True, kw_only=True)
 class ExecutedScenario:
 
     name: str
     description: str
     steps: Sequence[ExecutedStep]
     tags: Sequence[str]
+    example_number: int
 
 
 class PassedScenario(ExecutedScenario):
     success = True
 
 
 class SkippedScenario(PassedScenario):
@@ -64,16 +65,16 @@
 
 
 @dataclass(frozen=True, kw_only=True)
 class ExecutedFile:
 
     scenarios: tuple[ExecutedScenario, ...]
     uri: str
-    name: str
-    description: str
+    name: str | None
+    description: str | None
 
     def __new__(cls, *, scenarios, **_):
         if all(s.success for s in scenarios):
             return super().__new__(PassedFile)
         return super().__new__(FailedFile)
 
 
@@ -166,49 +167,67 @@
 def execute_scenario(
         scenario,
         *,
         context_maker,
         steps,
         skip_scenario_tag,
 ):
+    executed_scenarios = []
+    for example_num, scenario_steps in enumerate(
+            steps.iter_steps(scenario), start=1):
+
+        if skip_scenario_tag in scenario.tags:
+            cls = SkippedScenario
+            executed_steps = []
+        else:
+            cls, executed_steps = _execute_scenario(
+                    steps=scenario_steps,
+                    context_maker=context_maker,
+            )
+
+        executed_scenario = cls(
+                name=scenario.name,
+                description=scenario.description,
+                steps=tuple(executed_steps),
+                tags=scenario.tags,
+                example_number=example_num,
+        )
+        executed_scenarios.append(executed_scenario)
+    return executed_scenarios
+
+
+def _execute_scenario(*, steps, context_maker):
     executed_steps = []
-    if skip_scenario_tag in scenario.tags:
-        cls = SkippedScenario
-    else:
-        failed = False
-        context = context_maker()
-        for step_ in steps.iter_steps(scenario):
-            if isinstance(step_, MissingStep):
+    failed = False
+    context = context_maker()
+    executed: _ExecutedStep
+    for step_ in steps:
+        if isinstance(step_, MissingStep):
+            failed = True
+            executed = FailedStep(
+                exception=MatchingFunctionNotFound(step_.sentence),
+                sentence=step_.sentence,
+            )
+        elif failed:
+            executed = IgnoredStep(sentence=step_.sentence)
+        else:
+            try:
+                step_(context=context)
+            except Exception as exc:  # pylint: disable=broad-except
                 failed = True
                 executed = FailedStep(
-                    exception=MatchingFunctionNotFound(step_.sentence),
-                    sentence=step_.sentence,
+                        exception=exc,
+                        sentence=step_.sentence,
                 )
-            elif failed:
-                executed = IgnoredStep(sentence=step_.sentence)
             else:
-                try:
-                    step_(context=context)
-                except Exception as exc:  # pylint: disable=broad-except
-                    failed = True
-                    executed = FailedStep(
-                            exception=exc,
-                            sentence=step_.sentence,
-                    )
-                else:
-                    executed = PassedStep(sentence=step_.sentence)
-            executed_steps.append(executed)
-        cls = FailedScenario if failed else PassedScenario
-
-    return cls(
-            name=scenario.name,
-            description=scenario.description,
-            steps=tuple(executed_steps),
-            tags=scenario.tags,
-    )
+                executed = PassedStep(sentence=step_.sentence)
+        executed_steps.append(executed)
+    cls = FailedScenario if failed else PassedScenario
+
+    return cls, executed_steps
 
 
 def execute_file(
         parsed_file: ParsedFile,
         /,
         *,
         context_maker: Callable[[], Any] | None,
@@ -232,22 +251,23 @@
     skip_scenario_tag:
         If a scenario in the `parsed_file` contains
         this tag, the scenario will not be executed.
     """
 
     context_maker = context_maker or (lambda: None)
     executed_scenarios: list[ExecutedScenario] = []
+
     for scenario in parsed_file.scenarios:
-        executed_scenario = execute_scenario(
+        executed = execute_scenario(
                 scenario,
                 steps=steps,
                 context_maker=context_maker,
                 skip_scenario_tag=skip_scenario_tag,
         )
-        executed_scenarios.append(executed_scenario)
+        executed_scenarios.extend(executed)
 
     return ExecutedFile(
             scenarios=tuple(executed_scenarios),
             uri=parsed_file.uri,
             name=parsed_file.name,
             description=parsed_file.description,
     )
@@ -374,53 +394,117 @@
         -------
         Decorator for registering a function as a step.
         """
         return lambda fn: self._add_step_fn(fn, pattern=pattern)
 
     def _add_step_fn(self, fn, /, *, pattern):
         self._pattern_to_fn[re.compile(pattern)] = fn
+        return fn
 
     def _wrap_mapped_function(self, *, fn_spec, fn, mapped_args, data):
 
         def wrapped(context):
             kwargs = {}
             if 'data' in fn_spec.kwonlyargs:
                 kwargs['data'] = data
             if 'context' in fn_spec.kwonlyargs:
                 kwargs['context'] = context
             return fn(*mapped_args, **kwargs)
 
         return wrapped
 
-    def _prepare_step(self, step_):
-        sentence = step_.sentence
+    def _prepare_step(self, *, sentence, data):
         for pattern, fn in self._pattern_to_fn.items():
             if match_ := pattern.search(sentence):
                 args = match_.groups()
                 spec = inspect.getfullargspec(fn)
                 mapped_args = [
                     spec.annotations.get(name, lambda x: x)(value)
                     for name, value in zip(spec.args, args)
                 ]
                 return self._wrap_mapped_function(
                     fn_spec=spec,
                     fn=fn,
                     mapped_args=mapped_args,
-                    data=step_.data,
+                    data=data,
                     )
 
         return None
 
     def iter_steps(
             self,
             scenario: Scenario,
     ) -> Iterable[ExecutableStep | MissingStep]:
         """See documentation of `StepMapperProto`."""
+        for example_data in scenario.examples_data or [{}]:
+            yield self._iter_steps(scenario, example_data=example_data)
+
+    def _iter_steps(self, scenario, example_data):
         if (hook := self._hooks.run_before_scenario):
             yield ExecutableStep(sentence=hook.name, callable_=hook.fn)
         for step_ in scenario.steps:
             if (hook := self._hooks.run_before_step):
                 yield ExecutableStep(sentence=hook.name, callable_=hook.fn)
-            if (fn := self._prepare_step(step_)):
-                yield ExecutableStep(sentence=step_.sentence, callable_=fn)
+
+            sentence = self._evaluate_sentence(
+                    template=step_.sentence,
+                    example_data=example_data,
+            )
+            data = self._evaluate_step_data(
+                    template=step_.data,
+                    example_data=example_data,
+            )
+
+            callable_ = self._prepare_step(sentence=sentence, data=data)
+
+            if callable_:
+                yield ExecutableStep(
+                        sentence=sentence, callable_=callable_)
             else:
-                yield MissingStep(sentence=step_.sentence)
+                yield MissingStep(sentence=sentence)
+
+    def _evaluate_sentence(self, *, template, example_data):
+        return self._evaluate_line(
+                template=template, example_data=example_data)
+
+    def _evaluate_line(self, template: str, *, example_data) -> str:
+        pattern = re.compile(r'(?:^|[^\\])(?:\\\\)*(<(\w+)>)')
+        line = template
+        while match_ := re.search(pattern, line):
+            _, end = match_.span()
+            outer, key = match_.groups()
+            start = end - len(outer)
+            value = example_data[key]
+            line = line[:start] + value + line[end:]
+        return line
+
+    def _evaluate_step_data(self, *, template, example_data):
+        if template is None:
+            return template
+
+        if isinstance(template, str):
+            return self._evaluate_step_text(
+                    template, example_data=example_data)
+
+        return self._evaluate_step_data_table(
+                template, example_data=example_data)
+
+    def _evaluate_step_text(self, template, *, example_data):
+        return '\n'.join(
+                self._evaluate_line(line, example_data=example_data)
+                for line in template.splitlines()
+        )
+
+    def _evaluate_step_data_table(
+            self,
+            table_template: Sequence[dict[str, str]],
+            *,
+            example_data,
+    ) -> tuple[dict[str, str], ...]:
+        return tuple(
+            {
+                self._evaluate_line(key, example_data=example_data):
+                    self._evaluate_line(value, example_data=example_data)
+                for key, value in row.items()
+            }
+            for row in table_template
+        )
```

### Comparing `rumex-0.4.0/rumex/tests/__init__.py` & `rumex-0.5.0/rumex/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `rumex-0.4.0/rumex/tests/test_data.py` & `rumex-0.5.0/rumex/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `rumex-0.4.0/rumex/tests/test_error_reporting.py` & `rumex-0.5.0/rumex/tests/test_error_reporting.py`

 * *Files identical despite different names*

### Comparing `rumex-0.4.0/rumex/tests/test_no_execution_cases.py` & `rumex-0.5.0/rumex/tests/test_no_execution_cases.py`

 * *Files identical despite different names*

### Comparing `rumex-0.4.0/rumex/tests/test_simple_execution.py` & `rumex-0.5.0/rumex/tests/test_simple_execution.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     uri = 'test_file'
     reporter = Reporter()
 
     steps = get_step_mapper()
 
     @dataclass
     class Context:
-        value: float = None
+        value: float | None = None
 
     @steps('Given 2')
     def given_(*, context):
         context.value = 2
 
     @steps('divide it by 2')
     def when_(*, context):
```

### Comparing `rumex-0.4.0/rumex/utils.py` & `rumex-0.5.0/rumex/utils.py`

 * *Files identical despite different names*

### Comparing `rumex-0.4.0/PKG-INFO` & `rumex-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rumex
-Version: 0.4.0
+Version: 0.5.0
 Summary: 
 Author: uigctaw
 Author-email: uigctaw@metadata.social
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

