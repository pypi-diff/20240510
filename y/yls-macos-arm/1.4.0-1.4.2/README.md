# Comparing `tmp/yls_macos_arm-1.4.0.tar.gz` & `tmp/yls_macos_arm-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yls_macos_arm-1.4.0.tar", max compression
+gzip compressed data, was "yls_macos_arm-1.4.2.tar", max compression
```

## Comparing `yls_macos_arm-1.4.0.tar` & `yls_macos_arm-1.4.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1082 2024-01-02 18:31:46.985619 yls_macos_arm-1.4.0/LICENSE
--rw-r--r--   0        0        0     1772 2024-01-02 18:31:46.985737 yls_macos_arm-1.4.0/LICENSE-THIRD-PARTY
--rw-r--r--   0        0        0     2025 2024-01-28 18:10:31.525444 yls_macos_arm-1.4.0/README.md
--rw-r--r--   0        0        0     2241 2024-01-28 18:15:41.778394 yls_macos_arm-1.4.0/pyproject.toml
--rw-r--r--   0        0        0       55 2024-01-28 17:10:13.231445 yls_macos_arm-1.4.0/yls/__init__.py
--rw-r--r--   0        0        0     4707 2024-01-02 18:31:47.003959 yls_macos_arm-1.4.0/yls/code_actions.py
--rw-r--r--   0        0        0     8512 2024-01-02 18:31:47.004064 yls_macos_arm-1.4.0/yls/completer.py
--rw-r--r--   0        0        0    14959 2024-01-02 18:31:47.004181 yls_macos_arm-1.4.0/yls/completion.py
--rw-r--r--   0        0        0     4381 2024-01-02 18:31:47.004292 yls_macos_arm-1.4.0/yls/debugger.py
--rw-r--r--   0        0        0     3070 2024-01-02 18:31:47.004390 yls_macos_arm-1.4.0/yls/hookspecs.py
--rw-r--r--   0        0        0     7326 2024-01-02 18:31:47.004504 yls_macos_arm-1.4.0/yls/hover.py
--rw-r--r--   0        0        0      101 2024-01-02 18:31:47.004585 yls_macos_arm-1.4.0/yls/icons.py
--rw-r--r--   0        0        0     2235 2024-01-02 18:31:47.004683 yls_macos_arm-1.4.0/yls/linting.py
--rw-r--r--   0        0        0     2953 2024-01-28 17:10:13.232314 yls_macos_arm-1.4.0/yls/plugin_manager_provider.py
--rw-r--r--   0        0        0        0 2024-01-02 18:31:47.004806 yls_macos_arm-1.4.0/yls/py.typed
--rw-r--r--   0        0        0    22752 2024-01-02 18:31:47.004974 yls_macos_arm-1.4.0/yls/server.py
--rw-r--r--   0        0        0     3682 2024-01-02 18:31:47.005435 yls_macos_arm-1.4.0/yls/strings.py
--rw-r--r--   0        0        0    27410 2024-01-02 18:31:47.005588 yls_macos_arm-1.4.0/yls/utils.py
--rw-r--r--   0        0        0       22 2024-01-02 18:31:47.005692 yls_macos_arm-1.4.0/yls/version.py
--rw-r--r--   0        0        0      566 2024-01-02 18:31:47.005794 yls_macos_arm-1.4.0/yls/yaramod_provider.py
--rw-r--r--   0        0        0     2697 1970-01-01 00:00:00.000000 yls_macos_arm-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1082 2024-01-02 18:31:46.985619 yls_macos_arm-1.4.2/LICENSE
+-rw-r--r--   0        0        0     1772 2024-01-02 18:31:46.985737 yls_macos_arm-1.4.2/LICENSE-THIRD-PARTY
+-rw-r--r--   0        0        0     2382 2024-05-10 12:07:53.154014 yls_macos_arm-1.4.2/README.md
+-rw-r--r--   0        0        0     2190 2024-05-10 12:18:00.328424 yls_macos_arm-1.4.2/pyproject.toml
+-rw-r--r--   0        0        0       55 2024-01-28 17:10:13.231445 yls_macos_arm-1.4.2/yls/__init__.py
+-rw-r--r--   0        0        0     4707 2024-01-02 18:31:47.003959 yls_macos_arm-1.4.2/yls/code_actions.py
+-rw-r--r--   0        0        0     8512 2024-01-02 18:31:47.004064 yls_macos_arm-1.4.2/yls/completer.py
+-rw-r--r--   0        0        0    14959 2024-01-02 18:31:47.004181 yls_macos_arm-1.4.2/yls/completion.py
+-rw-r--r--   0        0        0     4441 2024-05-10 12:18:00.329007 yls_macos_arm-1.4.2/yls/debugger.py
+-rw-r--r--   0        0        0     3058 2024-05-10 12:18:00.329285 yls_macos_arm-1.4.2/yls/hookspecs.py
+-rw-r--r--   0        0        0     7326 2024-01-02 18:31:47.004504 yls_macos_arm-1.4.2/yls/hover.py
+-rw-r--r--   0        0        0      101 2024-01-02 18:31:47.004585 yls_macos_arm-1.4.2/yls/icons.py
+-rw-r--r--   0        0        0     2235 2024-01-02 18:31:47.004683 yls_macos_arm-1.4.2/yls/linting.py
+-rw-r--r--   0        0        0     2953 2024-01-28 17:10:13.232314 yls_macos_arm-1.4.2/yls/plugin_manager_provider.py
+-rw-r--r--   0        0        0        0 2024-01-02 18:31:47.004806 yls_macos_arm-1.4.2/yls/py.typed
+-rw-r--r--   0        0        0    22776 2024-05-10 12:18:00.329619 yls_macos_arm-1.4.2/yls/server.py
+-rw-r--r--   0        0        0     3682 2024-01-02 18:31:47.005435 yls_macos_arm-1.4.2/yls/strings.py
+-rw-r--r--   0        0        0    27410 2024-05-10 12:18:00.330027 yls_macos_arm-1.4.2/yls/utils.py
+-rw-r--r--   0        0        0       22 2024-05-10 12:18:00.330320 yls_macos_arm-1.4.2/yls/version.py
+-rw-r--r--   0        0        0      566 2024-01-02 18:31:47.005794 yls_macos_arm-1.4.2/yls/yaramod_provider.py
+-rw-r--r--   0        0        0     3041 1970-01-01 00:00:00.000000 yls_macos_arm-1.4.2/PKG-INFO
```

### Comparing `yls_macos_arm-1.4.0/LICENSE` & `yls_macos_arm-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yls_macos_arm-1.4.0/LICENSE-THIRD-PARTY` & `yls_macos_arm-1.4.2/LICENSE-THIRD-PARTY`

 * *Files identical despite different names*

### Comparing `yls_macos_arm-1.4.0/README.md` & `yls_macos_arm-1.4.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 **This is a temporary fork of the original YLS repository (avast/yls) in order to allow an easy installation of all components on macOS ARM devices.**
 
+This repository only includes changes that allow publishing this python module under a different name - `yls-macos-arm` - as well as including `yari-py-macos-arm` as a dependency instead of the default `yari-py` module. There are no changes to the code itself.
+
+**This repository is not managed by Avast. If you have issues, please report them upstream.**
+
 # YLS
 
 ![PyPI](https://img.shields.io/pypi/v/yls?label=yls)
 ![Visual Studio Marketplace Version](https://img.shields.io/visual-studio-marketplace/v/avast-threatlabs-yara.vscode-yls?label=vscode)
 
 [Language server](https://microsoft.github.io/language-server-protocol/) for
 [YARA](https://yara.readthedocs.io/en/stable/) language.
```

### Comparing `yls_macos_arm-1.4.0/pyproject.toml` & `yls_macos_arm-1.4.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 [tool.poetry]
 name = "yls-macos-arm"
-version = "1.4.0"
+version = "1.4.2"
 description = "YARA Language Server"
 authors = ["Matej Kašťák <matej.kastak@avast.com>"]
-maintainers = [
-  "Matej Kašťák <matej.kastak@avast.com>",
-  "Nils Kuhnert <3c7@posteo.de>",
-]
+maintainers = ["Nils Kuhnert <3c7@posteo.de>"]
 readme = "README.md"
 license = "MIT"
 include = ["py.typed", "LICENSE", "LICENSE-THIRD-PARTY"]
 
 [tool.poetry.group.dev.dependencies]
-black = "^22.3.0"
 isort = "^5.10.1"
 poethepoet = "^0.13.1"
 pytest = "^7.2.2"
 pytest-asyncio = "^0.18.3"
 pytest-black = "^0.3.12"
 pytest-cov = "^3.0.0"
 pytest-mock = "^3.7.0"
 pytest-mypy = "^0.9.1"
-pytest-pylint = "0.19.0"
 pytest-yls = { path = "./pytest-yls", develop = true }
+pytest-pylint = "^0.21.0"
+black = "^24.3.0"
 
 [tool.black]
 line-length = 100
 skip-magic-trailing-comma = true
 include = '\.pyi?$'
 exclude = '''
 /(
@@ -55,19 +52,19 @@
 format = ["_isort", "_black"]
 test = "pytest -vvv --mypy --black --pylint --pylint-rcfile=pyproject.toml --cov=yls --cov-report=term-missing -l ./yls ./tests"
 
 [tool.poetry.scripts]
 yls = 'yls.server:main'
 
 [tool.poetry.dependencies]
-python = ">=3.11,<=3.12"
-pygls = "^1.1.2"
-yaramod = "^3.20.1"
-yari-py-macos-arm = "^0.2.1"
+python = ">=3.11,<3.13"
 pluggy = "^1.0.0"
+yari-py-macos-arm = "^0.2.1"
+pygls = "^1.3.0"
+yaramod = "^3.21.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
```

### Comparing `yls_macos_arm-1.4.0/yls/code_actions.py` & `yls_macos_arm-1.4.2/yls/code_actions.py`

 * *Files identical despite different names*

### Comparing `yls_macos_arm-1.4.0/yls/completer.py` & `yls_macos_arm-1.4.2/yls/completer.py`

 * *Files identical despite different names*

### Comparing `yls_macos_arm-1.4.0/yls/completion.py` & `yls_macos_arm-1.4.2/yls/completion.py`

 * *Files identical despite different names*

### Comparing `yls_macos_arm-1.4.0/yls/debugger.py` & `yls_macos_arm-1.4.2/yls/debugger.py`

 * *Files 5% similar despite different names*

```diff
@@ -101,14 +101,17 @@
 
         return res
 
     @staticmethod
     async def get_samples_dir(ls: Any) -> Path | None:
         samples_dir_config = await utils.get_config_from_editor(ls, "yls.yari.samplesDirectory")
         log.debug(f"[DEBUGGER] Got {samples_dir_config=}")
+        if not samples_dir_config:
+            return None
+
         samples_dir_path = Path(samples_dir_config).expanduser().resolve()
         log.debug(f"[DEBUGGER] Resolved {samples_dir_config=}")
 
         if not samples_dir_path.is_dir():
             log.debug("[DEBUGGER] Samples dir does not exist or is not a directory")
             return None
```

### Comparing `yls_macos_arm-1.4.0/yls/hookspecs.py` & `yls_macos_arm-1.4.2/yls/hookspecs.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,16 +34,15 @@
 hookspec = pluggy.HookspecMarker("yls")
 
 T = TypeVar("T")
 PluggyRes = Union[Awaitable[T], Callable[[], T], T]
 
 
 @hookspec(firstresult=True)
-def create_yaramod_instance() -> yaramod.Yaramod | None:
-    ...
+def create_yaramod_instance() -> yaramod.Yaramod | None: ...
 
 
 @hookspec
 def yls_lint(document: Document) -> list[Diagnostic]:  # type: ignore
     ...
 
 
@@ -51,31 +50,29 @@
 def yls_completion(params: CompletionParams, document: Document) -> list[CompletionItem]:  # type: ignore
     ...
 
 
 @hookspec(firstresult=True)
 def yls_formatting(
     ls: Any, params: DocumentFormattingParams, document: Document
-) -> list[TextEdit] | None:
-    ...
+) -> list[TextEdit] | None: ...
 
 
 @hookspec
 def yls_code_actions(ls: Any, params: CodeActionParams) -> list[Command | CodeAction]:  # type: ignore
     ...
 
 
 @hookspec
 def yls_supported_commands(ls: Any) -> list[str]:  # type: ignore
     ...
 
 
 @hookspec
-def yls_execute_command(command: str, ls: Any, params: Any) -> PluggyRes[Any | None]:
-    ...
+def yls_execute_command(command: str, ls: Any, params: Any) -> PluggyRes[Any | None]: ...
 
 
 @hookspec
 def yls_code_lens(ls: Any, params: CodeLensParams) -> list[CodeLens]:  # type: ignore
     ...
```

### Comparing `yls_macos_arm-1.4.0/yls/hover.py` & `yls_macos_arm-1.4.2/yls/hover.py`

 * *Files identical despite different names*

### Comparing `yls_macos_arm-1.4.0/yls/linting.py` & `yls_macos_arm-1.4.2/yls/linting.py`

 * *Files identical despite different names*

### Comparing `yls_macos_arm-1.4.0/yls/plugin_manager_provider.py` & `yls_macos_arm-1.4.2/yls/plugin_manager_provider.py`

 * *Files identical despite different names*

### Comparing `yls_macos_arm-1.4.0/yls/server.py` & `yls_macos_arm-1.4.2/yls/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -201,17 +201,19 @@
     utils.log_command(TEXT_DOCUMENT_HOVER)
 
     return await ls.hoverer.hover(params)
 
 
 def lint(
     ls: YaraLanguageServer,
-    params: lsp_types.DidOpenTextDocumentParams
-    | lsp_types.DidChangeTextDocumentParams
-    | lsp_types.DidSaveTextDocumentParams,
+    params: (
+        lsp_types.DidOpenTextDocumentParams
+        | lsp_types.DidChangeTextDocumentParams
+        | lsp_types.DidSaveTextDocumentParams
+    ),
 ) -> None:
     """Lint and publish diagnostics."""
     # NOTE: DiagnosticRelatedInformation can be used to show the redefinition of a rule/string
     # Represents a related message and source code location for a diagnostic. This should be
     # used to point to code locations that cause or are related to a diagnostics, e.g when
     # duplicating a symbol in a scope.
```

### Comparing `yls_macos_arm-1.4.0/yls/strings.py` & `yls_macos_arm-1.4.2/yls/strings.py`

 * *Files identical despite different names*

### Comparing `yls_macos_arm-1.4.0/yls/utils.py` & `yls_macos_arm-1.4.2/yls/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -333,128 +333,128 @@
 
     def extract(self, expr: yaramod.Expression) -> None:
         expr_range = range_from_yaramod_expression(expr)
         if position_in_range(self.position, expr_range):
             self.expr = expr
 
     # pylint: disable-next=invalid-name
-    def visit_FunctionCallExpression(self, expr: yaramod.FunctionCallExpression) -> None:  # type: ignore
-        self.extract(expr)
+    def visit_FunctionCallExpression(self, arg0: yaramod.FunctionCallExpression) -> None:  # type: ignore
+        self.extract(arg0)
 
     # pylint: disable-next=invalid-name
-    def visit_IdExpression(self, expr: yaramod.IdExpression) -> None:  # type: ignore
-        self.extract(expr)
+    def visit_IdExpression(self, arg0: yaramod.IdExpression) -> None:  # type: ignore
+        self.extract(arg0)
 
     # pylint: disable-next=invalid-name
-    def visit_StructAccessExpression(self, expr: yaramod.StructAccessExpression) -> None:  # type: ignore
-        self.extract(expr)
+    def visit_StructAccessExpression(self, arg0: yaramod.StructAccessExpression) -> None:  # type: ignore
+        self.extract(arg0)
 
     # pylint: disable-next=invalid-name
-    def visit_ArrayAccessExpression(self, expr: yaramod.ArrayAccessExpression) -> None:  # type: ignore
-        self.extract(expr)
+    def visit_ArrayAccessExpression(self, arg0: yaramod.ArrayAccessExpression) -> None:  # type: ignore
+        self.extract(arg0)
 
     # pylint: disable-next=invalid-name
-    def visit_StringExpression(self, expr: yaramod.StringExpression) -> None:  # type: ignore
-        self.extract(expr)
+    def visit_StringExpression(self, arg0: yaramod.StringExpression) -> None:  # type: ignore
+        self.extract(arg0)
 
     # pylint: disable-next=invalid-name
-    def visit_StringCountExpression(self, expr: yaramod.StringCountExpression) -> None:  # type: ignore
-        self.extract(expr)
+    def visit_StringCountExpression(self, arg0: yaramod.StringCountExpression) -> None:  # type: ignore
+        self.extract(arg0)
 
     # pylint: disable-next=invalid-name
-    def visit_StringOffsetExpression(self, expr: yaramod.StringOffsetExpression) -> None:  # type: ignore
-        self.extract(expr)
+    def visit_StringOffsetExpression(self, arg0: yaramod.StringOffsetExpression) -> None:  # type: ignore
+        self.extract(arg0)
 
     # pylint: disable-next=invalid-name
-    def visit_StringLengthExpression(self, expr: yaramod.StringLengthExpression) -> None:  # type: ignore
-        self.extract(expr)
+    def visit_StringLengthExpression(self, arg0: yaramod.StringLengthExpression) -> None:  # type: ignore
+        self.extract(arg0)
 
     # pylint: disable-next=invalid-name
-    def visit_OfExpression(self, expr: yaramod.OfExpression) -> None:  # type: ignore
-        self.extract(expr)
+    def visit_OfExpression(self, arg0: yaramod.OfExpression) -> None:  # type: ignore
+        self.extract(arg0)
 
     # pylint: disable-next=invalid-name
-    def visit_ForExpression(self, expr: yaramod.ForExpression) -> None:
-        self.extract(expr)
+    def visit_ForExpression(self, arg0: yaramod.ForExpression) -> None:
+        self.extract(arg0)
 
     # pylint: disable-next=invalid-name
-    def visit_IequalsExpression(self, expr: yaramod.IequalsExpression) -> None:  # type: ignore
-        self.extract(expr)
-        expr.left_operand.accept(self)
-        expr.right_operand.accept(self)
+    def visit_IequalsExpression(self, arg0: yaramod.IequalsExpression) -> None:  # type: ignore
+        self.extract(arg0)
+        arg0.left_operand.accept(self)
+        arg0.right_operand.accept(self)
 
     # pylint: disable-next=invalid-name
-    def visit_LtExpression(self, expr: yaramod.LtExpression) -> None:  # type: ignore
-        self.extract(expr)
-        expr.left_operand.accept(self)
-        expr.right_operand.accept(self)
+    def visit_LtExpression(self, arg0: yaramod.LtExpression) -> None:  # type: ignore
+        self.extract(arg0)
+        arg0.left_operand.accept(self)
+        arg0.right_operand.accept(self)
 
     # pylint: disable-next=invalid-name
-    def visit_GtExpression(self, expr: yaramod.GtExpression) -> None:  # type: ignore
-        self.extract(expr)
-        expr.left_operand.accept(self)
-        expr.right_operand.accept(self)
+    def visit_GtExpression(self, arg0: yaramod.GtExpression) -> None:  # type: ignore
+        self.extract(arg0)
+        arg0.left_operand.accept(self)
+        arg0.right_operand.accept(self)
 
     # pylint: disable-next=invalid-name
-    def visit_LeExpression(self, expr: yaramod.LeExpression) -> None:  # type: ignore
-        self.extract(expr)
-        expr.left_operand.accept(self)
-        expr.right_operand.accept(self)
+    def visit_LeExpression(self, arg0: yaramod.LeExpression) -> None:  # type: ignore
+        self.extract(arg0)
+        arg0.left_operand.accept(self)
+        arg0.right_operand.accept(self)
 
     # pylint: disable-next=invalid-name
-    def visit_GeExpression(self, expr: yaramod.GeExpression) -> None:  # type: ignore
-        self.extract(expr)
-        expr.left_operand.accept(self)
-        expr.right_operand.accept(self)
+    def visit_GeExpression(self, arg0: yaramod.GeExpression) -> None:  # type: ignore
+        self.extract(arg0)
+        arg0.left_operand.accept(self)
+        arg0.right_operand.accept(self)
 
     # pylint: disable-next=invalid-name
-    def visit_EqExpression(self, expr: yaramod.EqExpression) -> None:  # type: ignore
-        self.extract(expr)
-        expr.left_operand.accept(self)
-        expr.right_operand.accept(self)
+    def visit_EqExpression(self, arg0: yaramod.EqExpression) -> None:  # type: ignore
+        self.extract(arg0)
+        arg0.left_operand.accept(self)
+        arg0.right_operand.accept(self)
 
     # pylint: disable-next=invalid-name
-    def visit_NeqExpression(self, expr: yaramod.NeqExpression) -> None:  # type: ignore
-        self.extract(expr)
-        expr.left_operand.accept(self)
-        expr.right_operand.accept(self)
+    def visit_NeqExpression(self, arg0: yaramod.NeqExpression) -> None:  # type: ignore
+        self.extract(arg0)
+        arg0.left_operand.accept(self)
+        arg0.right_operand.accept(self)
 
     # pylint: disable-next=invalid-name
-    def visit_AndExpression(self, expr: yaramod.AndExpression) -> None:  # type: ignore
-        self.extract(expr)
-        expr.left_operand.accept(self)
-        expr.right_operand.accept(self)
+    def visit_AndExpression(self, arg0: yaramod.AndExpression) -> None:  # type: ignore
+        self.extract(arg0)
+        arg0.left_operand.accept(self)
+        arg0.right_operand.accept(self)
 
     # pylint: disable-next=invalid-name
-    def visit_OrExpression(self, expr: yaramod.OrExpression) -> None:  # type: ignore
-        self.extract(expr)
-        expr.left_operand.accept(self)
-        expr.right_operand.accept(self)
+    def visit_OrExpression(self, arg0: yaramod.OrExpression) -> None:  # type: ignore
+        self.extract(arg0)
+        arg0.left_operand.accept(self)
+        arg0.right_operand.accept(self)
 
     # pylint: disable-next=invalid-name
-    def visit_NotExpression(self, expr: yaramod.NotExpression) -> None:  # type: ignore
-        self.extract(expr)
-        expr.operand.accept(self)
+    def visit_NotExpression(self, arg0: yaramod.NotExpression) -> None:  # type: ignore
+        self.extract(arg0)
+        arg0.operand.accept(self)
 
     # pylint: disable-next=invalid-name
-    def visit_DefinedExpression(self, expr: yaramod.DefinedExpression) -> None:  # type: ignore
-        self.extract(expr)
-        expr.operand.accept(self)
+    def visit_DefinedExpression(self, arg0: yaramod.DefinedExpression) -> None:  # type: ignore
+        self.extract(arg0)
+        arg0.operand.accept(self)
 
     # pylint: disable-next=invalid-name
-    def visit_ContainsExpression(self, expr: yaramod.ContainsExpression) -> None:  # type: ignore
-        self.extract(expr)
-        expr.left_operand.accept(self)
-        expr.right_operand.accept(self)
+    def visit_ContainsExpression(self, arg0: yaramod.ContainsExpression) -> None:  # type: ignore
+        self.extract(arg0)
+        arg0.left_operand.accept(self)
+        arg0.right_operand.accept(self)
 
     # pylint: disable-next=invalid-name
-    def visit_MatchesExpression(self, expr: yaramod.MatchesExpression) -> None:  # type: ignore
-        self.extract(expr)
-        expr.left_operand.accept(self)
-        expr.right_operand.accept(self)
+    def visit_MatchesExpression(self, arg0: yaramod.MatchesExpression) -> None:  # type: ignore
+        self.extract(arg0)
+        arg0.left_operand.accept(self)
+        arg0.right_operand.accept(self)
 
 
 def cursor_expression(
     yfile: yaramod.YaraFile, position: lsp_types.Position
 ) -> yaramod.Expression | None:
     """Return the expression under the cursor."""
 
@@ -701,17 +701,17 @@
             last_discovered = set(self.discovered_rules)
             for rule in yara_file.rules:
                 self.last_rule = rule
                 self.observe(rule.condition)
 
         return self.discovered_rules
 
-    def visit_IdExpression(self, expr: yaramod.IdExpression) -> None:  # type: ignore
+    def visit_IdExpression(self, arg0: yaramod.IdExpression) -> None:  # type: ignore
         if self.last_rule and self.last_rule.name in self.discovered_rules:
-            self.discovered_rules.add(expr.symbol.name)
+            self.discovered_rules.add(arg0.symbol.name)
 
 
 def extract_rule_context_from_yarafile(yara_file: yaramod.YaraFile, rule: yaramod.Rule) -> str:
     """Extract specified rule, private rules and modules it is dependent on from YaraFile."""
 
     # Get rules ordered from deepest dependency to `rule` so they can be compiled.
     rule_names = RuleDependencyIdentifier().indirectly_affected(yara_file, rule.name)
```

### Comparing `yls_macos_arm-1.4.0/yls/yaramod_provider.py` & `yls_macos_arm-1.4.2/yls/yaramod_provider.py`

 * *Files identical despite different names*

### Comparing `yls_macos_arm-1.4.0/PKG-INFO` & `yls_macos_arm-1.4.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 Metadata-Version: 2.1
 Name: yls-macos-arm
-Version: 1.4.0
+Version: 1.4.2
 Summary: YARA Language Server
 License: MIT
 Author: Matej Kašťák
 Author-email: matej.kastak@avast.com
-Maintainer: Matej Kašťák
-Maintainer-email: matej.kastak@avast.com
-Requires-Python: >=3.11,<=3.12
+Maintainer: Nils Kuhnert
+Maintainer-email: 3c7@posteo.de
+Requires-Python: >=3.11,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pluggy (>=1.0.0,<2.0.0)
-Requires-Dist: pygls (>=1.1.2,<2.0.0)
-Requires-Dist: yaramod (>=3.20.1,<4.0.0)
+Requires-Dist: pygls (>=1.3.0,<2.0.0)
+Requires-Dist: yaramod (>=3.21.0,<4.0.0)
 Requires-Dist: yari-py-macos-arm (>=0.2.1,<0.3.0)
 Description-Content-Type: text/markdown
 
 **This is a temporary fork of the original YLS repository (avast/yls) in order to allow an easy installation of all components on macOS ARM devices.**
 
+This repository only includes changes that allow publishing this python module under a different name - `yls-macos-arm` - as well as including `yari-py-macos-arm` as a dependency instead of the default `yari-py` module. There are no changes to the code itself.
+
+**This repository is not managed by Avast. If you have issues, please report them upstream.**
+
 # YLS
 
 ![PyPI](https://img.shields.io/pypi/v/yls?label=yls)
 ![Visual Studio Marketplace Version](https://img.shields.io/visual-studio-marketplace/v/avast-threatlabs-yara.vscode-yls?label=vscode)
 
 [Language server](https://microsoft.github.io/language-server-protocol/) for
 [YARA](https://yara.readthedocs.io/en/stable/) language.
```

