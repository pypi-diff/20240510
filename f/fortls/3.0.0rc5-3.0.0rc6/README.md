# Comparing `tmp/fortls-3.0.0rc5.tar.gz` & `tmp/fortls-3.0.0rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fortls-3.0.0rc5.tar", last modified: Wed May  8 07:54:28 2024, max compression
+gzip compressed data, was "fortls-3.0.0rc6.tar", last modified: Fri May 10 13:31:50 2024, max compression
```

## Comparing `fortls-3.0.0rc5.tar` & `fortls-3.0.0rc6.tar`

### file list

```diff
@@ -1,259 +1,259 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:54:28.663565 fortls-3.0.0rc5/
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:54:28.619565 fortls-3.0.0rc5/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:54:28.619565 fortls-3.0.0rc5/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:54:28.619565 fortls-3.0.0rc5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/.github/workflows/docs_preview.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/.github/workflows/update-intrinsics.yml
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    41497 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     5228 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12545 2024-05-08 07:54:28.663565 fortls-3.0.0rc5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10177 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:54:28.623565 fortls-3.0.0rc5/assets/
--rw-r--r--   0 runner    (1001) docker     (127)    19126 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/assets/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/assets/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:54:28.623565 fortls-3.0.0rc5/assets/animations/
--rw-r--r--   0 runner    (1001) docker     (127)  1647490 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/assets/animations/intro-demo.gif
--rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/assets/f.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4236 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/assets/icon.svg
--rw-r--r--   0 runner    (1001) docker     (127)    19148 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/assets/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    11737 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/assets/logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)    15257 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/assets/logo2-animated.svg
--rw-r--r--   0 runner    (1001) docker     (127)    78094 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/assets/logos.workspace.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:54:28.635565 fortls-3.0.0rc5/assets/lsp/
--rw-r--r--   0 runner    (1001) docker     (127)   791746 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/assets/lsp/completion-ani.gif
--rw-r--r--   0 runner    (1001) docker     (127)   450880 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/assets/lsp/completion-ani.mp4
--rw-r--r--   0 runner    (1001) docker     (127)    36257 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/assets/lsp/completion.png
--rw-r--r--   0 runner    (1001) docker     (127)   597393 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/assets/lsp/definition-goto.gif
--rw-r--r--   0 runner    (1001) docker     (127)   335329 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/assets/lsp/definition-goto.mp4
--rw-r--r--   0 runner    (1001) docker     (127)    54649 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/assets/lsp/definition-peek.png
--rw-r--r--   0 runner    (1001) docker     (127)    49007 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/assets/lsp/diagnostics1.png
--rw-r--r--   0 runner    (1001) docker     (127)    43464 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/assets/lsp/doc-highlight.png
--rw-r--r--   0 runner    (1001) docker     (127)    30439 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/assets/lsp/hover.png
--rw-r--r--   0 runner    (1001) docker     (127)    46449 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/assets/lsp/hover2.png
--rw-r--r--   0 runner    (1001) docker     (127)    65080 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/assets/lsp/references-peek.png
--rw-r--r--   0 runner    (1001) docker     (127)   703611 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/assets/lsp/rename.gif
--rw-r--r--   0 runner    (1001) docker     (127)   355841 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/assets/lsp/rename.mp4
--rw-r--r--   0 runner    (1001) docker     (127)   304764 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/assets/lsp/rename2.gif
--rw-r--r--   0 runner    (1001) docker     (127)   151579 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/assets/lsp/rename2.mp4
--rw-r--r--   0 runner    (1001) docker     (127)   628798 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/assets/lsp/sig-help.gif
--rw-r--r--   0 runner    (1001) docker     (127)   418094 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/assets/lsp/sig-help.mp4
--rw-r--r--   0 runner    (1001) docker     (127)    50499 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/assets/lsp/symbols-crop.png
--rw-r--r--   0 runner    (1001) docker     (127)     8288 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/assets/lsp/symbols-doc.png
--rw-r--r--   0 runner    (1001) docker     (127)    25726 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/assets/lsp/symbols-workspace.png
--rw-r--r--   0 runner    (1001) docker     (127)    54934 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/assets/lsp/symbols.png
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/assets/symbol-class.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:54:28.635565 fortls-3.0.0rc5/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/docs/contact.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7767 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/docs/editor_integration.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/docs/features.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4916 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/docs/fortls.parsers.internal.rst
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/docs/fortls.parsers.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/docs/fortls.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:54:28.635565 fortls-3.0.0rc5/docs/html_extra/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/docs/html_extra/CNAME
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/docs/html_extra/google3e426562ce42e98f.html
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/docs/html_extra/robots.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7412 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/docs/options.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/docs/quickstart.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:54:28.639565 fortls-3.0.0rc5/fortls/
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-08 07:54:28.000000 fortls-3.0.0rc5/fortls/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    18046 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)     6444 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/fortls.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/ftypes.py
--rw-r--r--   0 runner    (1001) docker     (127)    18017 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/helper_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13054 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/json_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     7344 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/jsonrpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    74006 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/langserver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:54:28.639565 fortls-3.0.0rc5/fortls/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/parsers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:54:28.647565 fortls-3.0.0rc5/fortls/parsers/internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/parsers/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/parsers/internal/associate.py
--rw-r--r--   0 runner    (1001) docker     (127)    12267 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/parsers/internal/ast.py
--rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/parsers/internal/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/parsers/internal/block.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/parsers/internal/diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/parsers/internal/do.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/parsers/internal/enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/parsers/internal/function.py
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/parsers/internal/if_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/parsers/internal/imports.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/parsers/internal/include.py
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/parsers/internal/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    72890 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/parsers/internal/intrinsic.modules.json
--rw-r--r--   0 runner    (1001) docker     (127)    44156 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/parsers/internal/intrinsic.procedures.json
--rw-r--r--   0 runner    (1001) docker     (127)   630782 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/parsers/internal/intrinsic.procedures.markdown.json
--rw-r--r--   0 runner    (1001) docker     (127)    10093 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/parsers/internal/intrinsics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/parsers/internal/keywords.json
--rw-r--r--   0 runner    (1001) docker     (127)     5134 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/parsers/internal/method.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/parsers/internal/module.py
--rw-r--r--   0 runner    (1001) docker     (127)    86115 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/parsers/internal/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/parsers/internal/program.py
--rw-r--r--   0 runner    (1001) docker     (127)     9597 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/parsers/internal/scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/parsers/internal/select.py
--rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/parsers/internal/statements.json
--rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/parsers/internal/submodule.py
--rw-r--r--   0 runner    (1001) docker     (127)     9739 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/parsers/internal/subroutine.py
--rw-r--r--   0 runner    (1001) docker     (127)     6532 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/parsers/internal/type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/parsers/internal/use.py
--rw-r--r--   0 runner    (1001) docker     (127)    10927 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/parsers/internal/utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     8898 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/parsers/internal/variable.py
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/parsers/internal/where.py
--rw-r--r--   0 runner    (1001) docker     (127)     8954 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/regex_patterns.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/fortls/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:54:28.659565 fortls-3.0.0rc5/fortls.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12545 2024-05-08 07:54:28.000000 fortls-3.0.0rc5/fortls.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7058 2024-05-08 07:54:28.000000 fortls-3.0.0rc5/fortls.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 07:54:28.000000 fortls-3.0.0rc5/fortls.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-08 07:54:28.000000 fortls-3.0.0rc5/fortls.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-08 07:54:28.000000 fortls-3.0.0rc5/fortls.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-08 07:54:28.000000 fortls-3.0.0rc5/fortls.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:54:28.647565 fortls-3.0.0rc5/licenses/
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/licenses/fortran-language-server-license.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-08 07:54:28.663565 fortls-3.0.0rc5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:54:28.647565 fortls-3.0.0rc5/test/
--rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/setup_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     5884 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_preproc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_preproc_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_regex_patterns.py
--rw-r--r--   0 runner    (1001) docker     (127)     7451 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_server.py
--rw-r--r--   0 runner    (1001) docker     (127)    15917 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_server_completion.py
--rw-r--r--   0 runner    (1001) docker     (127)     8486 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_server_definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)    15743 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_server_diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (127)    11628 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_server_documentation.py
--rw-r--r--   0 runner    (1001) docker     (127)    26297 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_server_hover.py
--rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_server_implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_server_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_server_references.py
--rw-r--r--   0 runner    (1001) docker     (127)     7861 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_server_rename.py
--rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_server_signature_help.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:54:28.651565 fortls-3.0.0rc5/test/test_source/
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/.fortls
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:54:28.651565 fortls-3.0.0rc5/test/test_source/completion/
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/completion/test_vis_mod_completion.f90
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/completion/use_only_interface.f90
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:54:28.651565 fortls-3.0.0rc5/test/test_source/diag/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/diag/conf_long_lines.json
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/diag/test_contains.f90
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/diag/test_critical.f90
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/diag/test_enum.f90
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/diag/test_external.f90
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/diag/test_forall.f90
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/diag/test_function.f90
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/diag/test_function_arg_list.f90
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/diag/test_implicit_none.f90
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/diag/test_import.f90
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/diag/test_lines.f90
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/diag/test_scope_end_name_var.f90
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/diag/test_scope_overreach.f90
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/diag/test_semicolon.f90
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/diag/test_use_ordering.f90
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/diag/test_var_shadowing_keyword_arg.f90
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/diag/test_variable.f90
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/diag/test_visibility.f90
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/diag/test_where.f90
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:54:28.655565 fortls-3.0.0rc5/test/test_source/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/docs/test_doxygen.f90
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/docs/test_ford.f90
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/docs/test_module_and_type_doc.f90
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:54:28.615565 fortls-3.0.0rc5/test/test_source/excldir/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:54:28.655565 fortls-3.0.0rc5/test/test_source/excldir/sub1/
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/excldir/sub1/tmp.f90
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:54:28.655565 fortls-3.0.0rc5/test/test_source/excldir/sub2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/excldir/sub2/fake2.f90
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/f90_config.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:54:28.655565 fortls-3.0.0rc5/test/test_source/hover/
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/hover/associate_block.f90
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/hover/associate_block_2.f90
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/hover/functions.f90
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/hover/intent.f90
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/hover/parameters.f90
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/hover/pointers.f90
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/hover/recursive.f90
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/hover/spaced_keywords.f90
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/hover/types.f90
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:54:28.655565 fortls-3.0.0rc5/test/test_source/imp/
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/imp/import.f90
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/imp/submodule.f90
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:54:28.655565 fortls-3.0.0rc5/test/test_source/include/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/include/empty.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:54:28.655565 fortls-3.0.0rc5/test/test_source/parse/
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/parse/line_continuations.f90
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/parse/submodule.f90
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/parse/test_incomplete_dims.f90
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/parse/test_kinds_and_dims.f90
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:54:28.659565 fortls-3.0.0rc5/test/test_source/pp/
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/pp/.fortls
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/pp/.pp_conf.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:54:28.659565 fortls-3.0.0rc5/test/test_source/pp/include/
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/pp/include/petscerror.h
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/pp/include/petscpc.h
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/pp/preproc.F90
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/pp/preproc_elif.F90
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/pp/preproc_elif_elif_skip.F90
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/pp/preproc_else.F90
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/pp/preproc_if_elif_else.F90
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/pp/preproc_if_elif_skip.F90
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/pp/preproc_keywords.F90
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:54:28.659565 fortls-3.0.0rc5/test/test_source/rename/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/rename/test_rename_imp_type_bound_proc.f90
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/rename/test_rename_intrinsic.f90
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/rename/test_rename_nested.f90
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:54:28.659565 fortls-3.0.0rc5/test/test_source/signature/
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/signature/help.f90
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/signature/nested_sigs.f90
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:54:28.659565 fortls-3.0.0rc5/test/test_source/subdir/
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/subdir/test_abstract.f90
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/subdir/test_fixed.f
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/subdir/test_free.f90
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/subdir/test_generic.f90
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/subdir/test_inc2.f90
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/subdir/test_inherit.f90
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/subdir/test_rename.F90
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/subdir/test_select.f90
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/subdir/test_submod.F90
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/subdir/test_vis.f90
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/test.f90
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/test_block.f08
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/test_diagnostic_int.f90
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/test_import.f90
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/test_inc.f90
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/test_nonintrinsic.f90
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/test_prog.f08
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/test_submodule.f90
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:54:28.659565 fortls-3.0.0rc5/test/test_source/use/
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/use/use.f90
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:54:28.659565 fortls-3.0.0rc5/test/test_source/vis/
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/vis/private.f90
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-08 07:54:22.000000 fortls-3.0.0rc5/test/test_source/wrong_syntax.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:50.849576 fortls-3.0.0rc6/
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:50.805577 fortls-3.0.0rc6/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:50.805577 fortls-3.0.0rc6/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:50.805577 fortls-3.0.0rc6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/.github/workflows/docs_preview.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/.github/workflows/update-intrinsics.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    41497 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     5228 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12638 2024-05-10 13:31:50.849576 fortls-3.0.0rc6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10270 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:50.809577 fortls-3.0.0rc6/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    19126 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/assets/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/assets/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:50.809577 fortls-3.0.0rc6/assets/animations/
+-rw-r--r--   0 runner    (1001) docker     (127)  1647490 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/assets/animations/intro-demo.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/assets/f.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4236 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/assets/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    19148 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/assets/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11737 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/assets/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    15257 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/assets/logo2-animated.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    78094 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/assets/logos.workspace.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:50.821576 fortls-3.0.0rc6/assets/lsp/
+-rw-r--r--   0 runner    (1001) docker     (127)   791746 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/assets/lsp/completion-ani.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   450880 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/assets/lsp/completion-ani.mp4
+-rw-r--r--   0 runner    (1001) docker     (127)    36257 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/assets/lsp/completion.png
+-rw-r--r--   0 runner    (1001) docker     (127)   597393 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/assets/lsp/definition-goto.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   335329 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/assets/lsp/definition-goto.mp4
+-rw-r--r--   0 runner    (1001) docker     (127)    54649 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/assets/lsp/definition-peek.png
+-rw-r--r--   0 runner    (1001) docker     (127)    49007 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/assets/lsp/diagnostics1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    43464 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/assets/lsp/doc-highlight.png
+-rw-r--r--   0 runner    (1001) docker     (127)    30439 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/assets/lsp/hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)    46449 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/assets/lsp/hover2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    65080 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/assets/lsp/references-peek.png
+-rw-r--r--   0 runner    (1001) docker     (127)   703611 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/assets/lsp/rename.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   355841 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/assets/lsp/rename.mp4
+-rw-r--r--   0 runner    (1001) docker     (127)   304764 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/assets/lsp/rename2.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   151579 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/assets/lsp/rename2.mp4
+-rw-r--r--   0 runner    (1001) docker     (127)   628798 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/assets/lsp/sig-help.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   418094 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/assets/lsp/sig-help.mp4
+-rw-r--r--   0 runner    (1001) docker     (127)    50499 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/assets/lsp/symbols-crop.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8288 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/assets/lsp/symbols-doc.png
+-rw-r--r--   0 runner    (1001) docker     (127)    25726 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/assets/lsp/symbols-workspace.png
+-rw-r--r--   0 runner    (1001) docker     (127)    54934 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/assets/lsp/symbols.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/assets/symbol-class.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:50.821576 fortls-3.0.0rc6/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/docs/contact.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7767 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/docs/editor_integration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/docs/features.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4916 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/docs/fortls.parsers.internal.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/docs/fortls.parsers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/docs/fortls.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:50.825576 fortls-3.0.0rc6/docs/html_extra/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/docs/html_extra/CNAME
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/docs/html_extra/google3e426562ce42e98f.html
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/docs/html_extra/robots.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7412 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/docs/options.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/docs/quickstart.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:50.825576 fortls-3.0.0rc6/fortls/
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-10 13:31:50.000000 fortls-3.0.0rc6/fortls/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18046 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6444 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/fortls.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/ftypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18017 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/helper_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13054 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/json_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7344 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/jsonrpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74006 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/langserver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:50.829576 fortls-3.0.0rc6/fortls/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/parsers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:50.833576 fortls-3.0.0rc6/fortls/parsers/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/parsers/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/parsers/internal/associate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12267 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/parsers/internal/ast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/parsers/internal/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/parsers/internal/block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/parsers/internal/diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/parsers/internal/do.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/parsers/internal/enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/parsers/internal/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/parsers/internal/if_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/parsers/internal/imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/parsers/internal/include.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/parsers/internal/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72890 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/parsers/internal/intrinsic.modules.json
+-rw-r--r--   0 runner    (1001) docker     (127)    44156 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/parsers/internal/intrinsic.procedures.json
+-rw-r--r--   0 runner    (1001) docker     (127)   630782 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/parsers/internal/intrinsic.procedures.markdown.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10093 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/parsers/internal/intrinsics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/parsers/internal/keywords.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5134 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/parsers/internal/method.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/parsers/internal/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86115 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/parsers/internal/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/parsers/internal/program.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9597 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/parsers/internal/scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/parsers/internal/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/parsers/internal/statements.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/parsers/internal/submodule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9739 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/parsers/internal/subroutine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6532 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/parsers/internal/type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/parsers/internal/use.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10927 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/parsers/internal/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8898 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/parsers/internal/variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/parsers/internal/where.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8954 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/regex_patterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:50.849576 fortls-3.0.0rc6/fortls.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12638 2024-05-10 13:31:50.000000 fortls-3.0.0rc6/fortls.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7058 2024-05-10 13:31:50.000000 fortls-3.0.0rc6/fortls.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 13:31:50.000000 fortls-3.0.0rc6/fortls.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-10 13:31:50.000000 fortls-3.0.0rc6/fortls.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-10 13:31:50.000000 fortls-3.0.0rc6/fortls.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-10 13:31:50.000000 fortls-3.0.0rc6/fortls.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:50.833576 fortls-3.0.0rc6/licenses/
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/licenses/fortran-language-server-license.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-10 13:31:50.849576 fortls-3.0.0rc6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:50.837576 fortls-3.0.0rc6/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/setup_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5884 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_preproc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_preproc_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_regex_patterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7451 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15917 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_server_completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8486 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_server_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15743 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_server_diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11628 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_server_documentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26297 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_server_hover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_server_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_server_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_server_references.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7861 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_server_rename.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_server_signature_help.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:50.837576 fortls-3.0.0rc6/test/test_source/
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/.fortls
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:50.837576 fortls-3.0.0rc6/test/test_source/completion/
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/completion/test_vis_mod_completion.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/completion/use_only_interface.f90
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:50.841576 fortls-3.0.0rc6/test/test_source/diag/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/diag/conf_long_lines.json
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/diag/test_contains.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/diag/test_critical.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/diag/test_enum.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/diag/test_external.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/diag/test_forall.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/diag/test_function.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/diag/test_function_arg_list.f90
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/diag/test_implicit_none.f90
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/diag/test_import.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/diag/test_lines.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/diag/test_scope_end_name_var.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/diag/test_scope_overreach.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/diag/test_semicolon.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/diag/test_use_ordering.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/diag/test_var_shadowing_keyword_arg.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/diag/test_variable.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/diag/test_visibility.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/diag/test_where.f90
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:50.841576 fortls-3.0.0rc6/test/test_source/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/docs/test_doxygen.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/docs/test_ford.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/docs/test_module_and_type_doc.f90
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:50.801577 fortls-3.0.0rc6/test/test_source/excldir/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:50.841576 fortls-3.0.0rc6/test/test_source/excldir/sub1/
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/excldir/sub1/tmp.f90
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:50.841576 fortls-3.0.0rc6/test/test_source/excldir/sub2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/excldir/sub2/fake2.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/f90_config.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:50.845576 fortls-3.0.0rc6/test/test_source/hover/
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/hover/associate_block.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/hover/associate_block_2.f90
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/hover/functions.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/hover/intent.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/hover/parameters.f90
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/hover/pointers.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/hover/recursive.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/hover/spaced_keywords.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/hover/types.f90
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:50.845576 fortls-3.0.0rc6/test/test_source/imp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/imp/import.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/imp/submodule.f90
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:50.845576 fortls-3.0.0rc6/test/test_source/include/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/include/empty.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:50.845576 fortls-3.0.0rc6/test/test_source/parse/
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/parse/line_continuations.f90
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/parse/submodule.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/parse/test_incomplete_dims.f90
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/parse/test_kinds_and_dims.f90
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:50.845576 fortls-3.0.0rc6/test/test_source/pp/
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/pp/.fortls
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/pp/.pp_conf.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:50.845576 fortls-3.0.0rc6/test/test_source/pp/include/
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/pp/include/petscerror.h
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/pp/include/petscpc.h
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/pp/preproc.F90
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/pp/preproc_elif.F90
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/pp/preproc_elif_elif_skip.F90
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/pp/preproc_else.F90
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/pp/preproc_if_elif_else.F90
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/pp/preproc_if_elif_skip.F90
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/pp/preproc_keywords.F90
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:50.845576 fortls-3.0.0rc6/test/test_source/rename/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/rename/test_rename_imp_type_bound_proc.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/rename/test_rename_intrinsic.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/rename/test_rename_nested.f90
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:50.845576 fortls-3.0.0rc6/test/test_source/signature/
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/signature/help.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/signature/nested_sigs.f90
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:50.849576 fortls-3.0.0rc6/test/test_source/subdir/
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/subdir/test_abstract.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/subdir/test_fixed.f
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/subdir/test_free.f90
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/subdir/test_generic.f90
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/subdir/test_inc2.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/subdir/test_inherit.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/subdir/test_rename.F90
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/subdir/test_select.f90
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/subdir/test_submod.F90
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/subdir/test_vis.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/test.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/test_block.f08
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/test_diagnostic_int.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/test_import.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/test_inc.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/test_nonintrinsic.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/test_prog.f08
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/test_submodule.f90
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:50.849576 fortls-3.0.0rc6/test/test_source/use/
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/use/use.f90
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:50.849576 fortls-3.0.0rc6/test/test_source/vis/
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/vis/private.f90
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/wrong_syntax.json
```

### Comparing `fortls-3.0.0rc5/.github/FUNDING.yml` & `fortls-3.0.0rc6/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/.github/ISSUE_TEMPLATE/bug_report.md` & `fortls-3.0.0rc6/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/.github/ISSUE_TEMPLATE/feature_request.md` & `fortls-3.0.0rc6/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/.github/workflows/codeql-analysis.yml` & `fortls-3.0.0rc6/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/.github/workflows/docs_preview.yml` & `fortls-3.0.0rc6/.github/workflows/docs_preview.yml`

 * *Files 12% similar despite different names*

```diff
@@ -19,16 +19,20 @@
 concurrency: preview-${{github.ref}}
 
 jobs:
   deploy-preview:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v4
-      - uses: sphinx-toolbox/sphinx-action@master
+      - uses: actions/setup-python@v5
         with:
-          pre-build-command: "pip install .[docs]"
-          docs-folder: "docs/"
+          python-version: "3.11"
+      - name: Build docs
+        run: |
+          pip install -e .[dev,docs]
+          make -C docs html
       - name: Deploy Preview
         uses: rossjrw/pr-preview-action@v1.4.7
         with:
           source-dir: docs/_build/html
           preview-branch: gh-pages
+          custom-url: fortls.fortran-lang.org
```

### Comparing `fortls-3.0.0rc5/.github/workflows/main.yml` & `fortls-3.0.0rc6/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/.github/workflows/python-publish.yml` & `fortls-3.0.0rc6/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/.github/workflows/update-intrinsics.yml` & `fortls-3.0.0rc6/.github/workflows/update-intrinsics.yml`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/.pre-commit-config.yaml` & `fortls-3.0.0rc6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/CHANGELOG.md` & `fortls-3.0.0rc6/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/CODE_OF_CONDUCT.md` & `fortls-3.0.0rc6/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/CONTRIBUTING.md` & `fortls-3.0.0rc6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/LICENSE` & `fortls-3.0.0rc6/LICENSE`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/PKG-INFO` & `fortls-3.0.0rc6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fortls
-Version: 3.0.0rc5
+Version: 3.0.0rc6
 Summary: fortls - Fortran Language Server
 Author-email: Giannis Nikiteas <giannis.nikiteas@gmail.com>
 License: MIT
 Project-URL: homepage, https://fortls.fortran-lang.org
 Project-URL: Documentation, https://fortls.fortran-lang.org
 Project-URL: Changes, https://github.com/fortran-lang/fortls/blob/master/CHANGELOG.md
 Project-URL: Tracker, https://github.com/fortran-lang/fortls/issues
@@ -64,14 +64,15 @@
 ![Conda](https://img.shields.io/conda/dn/conda-forge/fortls?label=Anaconda&style=flat-square)
 ![GitHub License](https://img.shields.io/github/license/fortran-lang/fortls?style=flat-square)
 ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/fortran-lang/fortls/main.yml?branch=master&label=CI&style=flat-square)
 ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/fortran-lang/fortls/docs.yml?branch=master&label=Docs&style=flat-square)
 ![Codecov](https://img.shields.io/codecov/c/github/fortran-lang/fortls?style=flat-square)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/psf/black)
 ![GitHub Repo stars](https://img.shields.io/github/stars/fortran-lang/fortls?color=yellow&style=flat-square)
+[![DOI](https://zenodo.org/badge/412392321.svg?style=flat-square)](https://zenodo.org/badge/latestdoi/412392321)
 
 <!-- [<img alt="https://github.com/sponsors/gnikit" src="https://img.shields.io/static/v1?style=social&label=Sponsor&message=%E2%9D%A4&logo=GitHub&color&link=%3Curl%3E" height="30" />](https://github.com/sponsors/gnikit)
 [<img alt="https://paypal.me/inikit" src="https://img.shields.io/static/v1?style=social&label=Donate&message=%E2%9D%A4&logo=Paypal&color&link=%3Curl%3E" height="30" />](https://paypal.me/inikit) -->
 
 ![alt](https://raw.githubusercontent.com/fortran-lang/fortls/master/assets/animations/intro-demo.gif)
 
 `fortls` is an implementation of the [Language Server Protocol](https://github.com/Microsoft/language-server-protocol)
@@ -116,30 +117,18 @@
   - Generate type-bound procedures and implementation templates for
     deferred procedures
 
 ### Notes/Limitations
 
 - Signature help and hover does not handle elegantly overloaded functions i.e. interfaces
 
-## Future plans
-
-`fortls` has reached a point where it is feature complete and stable enough to be used in many modern Fortran projects without any issues.
-It does however still have fundamental limitations,
-namely its ability to understand all Fortran syntax and semantics that has been used throughout the 65+ years of the language. **The good news is that we have a plan to address this issue!**
-
-We are excited to announce that we are working on creating a new Fortran Language Server
-based on the actively developed [LFortran](https://lfortran.org/) compiler 🎉.
-The new Language Server will be able to understand all Fortran syntax, be faster,
-and give more accurate autocompletion, hover and diagnostic information. That means we plan on investing any future funding on creating our new language server and ultimately creating a better user experience for everyone.
-
-<!--  Have a look at our roadmap (link) and consider contributing to our efforts (donations and contribution tasks link).  -->
+## Documentation
 
-### What about `fortls`?
-
-Not to worry, `fortls` will continue to be here. We will keep `fortls` in maintenance mode with bug fixes and new features from volunteer contributors, but otherwise we will be focusing our efforts into making the new LFortran language server a reality.
+The full documentation for `fortls` can be found at
+[fortls.fortran-lang.org](https://fortls.fortran-lang.org/).
 
 ## Installation
 
 ### PyPi
 
 ```sh
 pip install fortls
@@ -213,14 +202,31 @@
 | `textDocument/rename`            | Rename a symbol across the workspace                   |
 | `textDocument/didOpen`           | Document synchronisation upon opening                  |
 | `textDocument/didSave`           | Document synchronisation upon saving                   |
 | `textDocument/didClose`          | Document synchronisation upon closing                  |
 | `textDocument/didChange`         | Document synchronisation upon changes to the document  |
 | `textDocument/codeAction`        | **Experimental** Generate code                         |
 
+## Future plans
+
+`fortls` has reached a point where it is feature complete and stable enough to be used in many modern Fortran projects without any issues.
+It does however still have fundamental limitations,
+namely its ability to understand all Fortran syntax and semantics that has been used throughout the 65+ years of the language. **The good news is that we have a plan to address this issue!**
+
+We are excited to announce that we are working on creating a new Fortran Language Server
+based on the actively developed [LFortran](https://lfortran.org/) compiler 🎉.
+The new Language Server will be able to understand all Fortran syntax, be faster,
+and give more accurate autocompletion, hover and diagnostic information. That means we plan on investing any future funding on creating our new language server and ultimately creating a better user experience for everyone.
+
+<!--  Have a look at our roadmap (link) and consider contributing to our efforts (donations and contribution tasks link).  -->
+
+### What about `fortls`?
+
+Not to worry, `fortls` will continue to be here. We will keep `fortls` in active maintenance mode with bug fixes and new features from volunteer contributors, but otherwise we will be focusing our efforts into making the new language server using LFortran's parser a reality.
+
 ## `fortls` vs `fortran-language-server`
 
 This project was originally based on `fortran-language-server` LSP implementation, but the two projects have since diverged.
 
 `fortls` (this project) is now developed independently of the upstream `hansec/fortran-language-server` project and contains numerous new features and bug fixes
 the original `fortran-language-server` does not.
 
@@ -232,20 +238,18 @@
 change in the future.
 
 ## Acknowledgements
 
 This project would not have been possible without the original work of [@hansec](https://github.com/hansec/)
 in [`fortran-language-server`](https://github.com/hansec/fortran-language-server)
 
-<!-- ## Support
-
-If you want to support this project you can do it through
+## Support
 
-[![Alt](https://www.paypalobjects.com/webstatic/mktg/Logo/pp-logo-150px.png)](https://paypal.me/inikit)
-[!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/gnikit) -->
+You can support Fortran-lang as a whole by donating at
+[Fortran-lang - NumFOCUS](https://numfocus.org/donate-for-fortran-lang).
 
 ## Bug reports
 
 When [filing bugs](https://github.com/fortran-lang/fortls/issues/new)
 please provide example code to reproduce the observed issue.
 
 ## Security Policy
```

### Comparing `fortls-3.0.0rc5/README.md` & `fortls-3.0.0rc6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 ![Conda](https://img.shields.io/conda/dn/conda-forge/fortls?label=Anaconda&style=flat-square)
 ![GitHub License](https://img.shields.io/github/license/fortran-lang/fortls?style=flat-square)
 ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/fortran-lang/fortls/main.yml?branch=master&label=CI&style=flat-square)
 ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/fortran-lang/fortls/docs.yml?branch=master&label=Docs&style=flat-square)
 ![Codecov](https://img.shields.io/codecov/c/github/fortran-lang/fortls?style=flat-square)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/psf/black)
 ![GitHub Repo stars](https://img.shields.io/github/stars/fortran-lang/fortls?color=yellow&style=flat-square)
+[![DOI](https://zenodo.org/badge/412392321.svg?style=flat-square)](https://zenodo.org/badge/latestdoi/412392321)
 
 <!-- [<img alt="https://github.com/sponsors/gnikit" src="https://img.shields.io/static/v1?style=social&label=Sponsor&message=%E2%9D%A4&logo=GitHub&color&link=%3Curl%3E" height="30" />](https://github.com/sponsors/gnikit)
 [<img alt="https://paypal.me/inikit" src="https://img.shields.io/static/v1?style=social&label=Donate&message=%E2%9D%A4&logo=Paypal&color&link=%3Curl%3E" height="30" />](https://paypal.me/inikit) -->
 
 ![alt](https://raw.githubusercontent.com/fortran-lang/fortls/master/assets/animations/intro-demo.gif)
 
 `fortls` is an implementation of the [Language Server Protocol](https://github.com/Microsoft/language-server-protocol)
@@ -61,30 +62,18 @@
   - Generate type-bound procedures and implementation templates for
     deferred procedures
 
 ### Notes/Limitations
 
 - Signature help and hover does not handle elegantly overloaded functions i.e. interfaces
 
-## Future plans
-
-`fortls` has reached a point where it is feature complete and stable enough to be used in many modern Fortran projects without any issues.
-It does however still have fundamental limitations,
-namely its ability to understand all Fortran syntax and semantics that has been used throughout the 65+ years of the language. **The good news is that we have a plan to address this issue!**
-
-We are excited to announce that we are working on creating a new Fortran Language Server
-based on the actively developed [LFortran](https://lfortran.org/) compiler 🎉.
-The new Language Server will be able to understand all Fortran syntax, be faster,
-and give more accurate autocompletion, hover and diagnostic information. That means we plan on investing any future funding on creating our new language server and ultimately creating a better user experience for everyone.
-
-<!--  Have a look at our roadmap (link) and consider contributing to our efforts (donations and contribution tasks link).  -->
+## Documentation
 
-### What about `fortls`?
-
-Not to worry, `fortls` will continue to be here. We will keep `fortls` in maintenance mode with bug fixes and new features from volunteer contributors, but otherwise we will be focusing our efforts into making the new LFortran language server a reality.
+The full documentation for `fortls` can be found at
+[fortls.fortran-lang.org](https://fortls.fortran-lang.org/).
 
 ## Installation
 
 ### PyPi
 
 ```sh
 pip install fortls
@@ -158,14 +147,31 @@
 | `textDocument/rename`            | Rename a symbol across the workspace                   |
 | `textDocument/didOpen`           | Document synchronisation upon opening                  |
 | `textDocument/didSave`           | Document synchronisation upon saving                   |
 | `textDocument/didClose`          | Document synchronisation upon closing                  |
 | `textDocument/didChange`         | Document synchronisation upon changes to the document  |
 | `textDocument/codeAction`        | **Experimental** Generate code                         |
 
+## Future plans
+
+`fortls` has reached a point where it is feature complete and stable enough to be used in many modern Fortran projects without any issues.
+It does however still have fundamental limitations,
+namely its ability to understand all Fortran syntax and semantics that has been used throughout the 65+ years of the language. **The good news is that we have a plan to address this issue!**
+
+We are excited to announce that we are working on creating a new Fortran Language Server
+based on the actively developed [LFortran](https://lfortran.org/) compiler 🎉.
+The new Language Server will be able to understand all Fortran syntax, be faster,
+and give more accurate autocompletion, hover and diagnostic information. That means we plan on investing any future funding on creating our new language server and ultimately creating a better user experience for everyone.
+
+<!--  Have a look at our roadmap (link) and consider contributing to our efforts (donations and contribution tasks link).  -->
+
+### What about `fortls`?
+
+Not to worry, `fortls` will continue to be here. We will keep `fortls` in active maintenance mode with bug fixes and new features from volunteer contributors, but otherwise we will be focusing our efforts into making the new language server using LFortran's parser a reality.
+
 ## `fortls` vs `fortran-language-server`
 
 This project was originally based on `fortran-language-server` LSP implementation, but the two projects have since diverged.
 
 `fortls` (this project) is now developed independently of the upstream `hansec/fortran-language-server` project and contains numerous new features and bug fixes
 the original `fortran-language-server` does not.
 
@@ -177,20 +183,18 @@
 change in the future.
 
 ## Acknowledgements
 
 This project would not have been possible without the original work of [@hansec](https://github.com/hansec/)
 in [`fortran-language-server`](https://github.com/hansec/fortran-language-server)
 
-<!-- ## Support
-
-If you want to support this project you can do it through
+## Support
 
-[![Alt](https://www.paypalobjects.com/webstatic/mktg/Logo/pp-logo-150px.png)](https://paypal.me/inikit)
-[!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/gnikit) -->
+You can support Fortran-lang as a whole by donating at
+[Fortran-lang - NumFOCUS](https://numfocus.org/donate-for-fortran-lang).
 
 ## Bug reports
 
 When [filing bugs](https://github.com/fortran-lang/fortls/issues/new)
 please provide example code to reproduce the observed issue.
 
 ## Security Policy
```

### Comparing `fortls-3.0.0rc5/SECURITY.md` & `fortls-3.0.0rc6/SECURITY.md`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/assets/LICENSE` & `fortls-3.0.0rc6/assets/LICENSE`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/assets/README.md` & `fortls-3.0.0rc6/assets/README.md`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/assets/animations/intro-demo.gif` & `fortls-3.0.0rc6/assets/animations/intro-demo.gif`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/assets/f.svg` & `fortls-3.0.0rc6/assets/f.svg`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/assets/icon.svg` & `fortls-3.0.0rc6/assets/icon.svg`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/assets/logo.png` & `fortls-3.0.0rc6/assets/logo.png`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/assets/logo.svg` & `fortls-3.0.0rc6/assets/logo.svg`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/assets/logo2-animated.svg` & `fortls-3.0.0rc6/assets/logo2-animated.svg`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/assets/logos.workspace.svg` & `fortls-3.0.0rc6/assets/logos.workspace.svg`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/assets/lsp/completion-ani.gif` & `fortls-3.0.0rc6/assets/lsp/completion-ani.gif`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/assets/lsp/completion-ani.mp4` & `fortls-3.0.0rc6/assets/lsp/completion-ani.mp4`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/assets/lsp/completion.png` & `fortls-3.0.0rc6/assets/lsp/completion.png`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/assets/lsp/definition-goto.gif` & `fortls-3.0.0rc6/assets/lsp/definition-goto.gif`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/assets/lsp/definition-goto.mp4` & `fortls-3.0.0rc6/assets/lsp/definition-goto.mp4`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/assets/lsp/definition-peek.png` & `fortls-3.0.0rc6/assets/lsp/definition-peek.png`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/assets/lsp/diagnostics1.png` & `fortls-3.0.0rc6/assets/lsp/diagnostics1.png`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/assets/lsp/doc-highlight.png` & `fortls-3.0.0rc6/assets/lsp/doc-highlight.png`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/assets/lsp/hover.png` & `fortls-3.0.0rc6/assets/lsp/hover.png`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/assets/lsp/hover2.png` & `fortls-3.0.0rc6/assets/lsp/hover2.png`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/assets/lsp/references-peek.png` & `fortls-3.0.0rc6/assets/lsp/references-peek.png`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/assets/lsp/rename.gif` & `fortls-3.0.0rc6/assets/lsp/rename.gif`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/assets/lsp/rename.mp4` & `fortls-3.0.0rc6/assets/lsp/rename.mp4`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/assets/lsp/rename2.gif` & `fortls-3.0.0rc6/assets/lsp/rename2.gif`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/assets/lsp/rename2.mp4` & `fortls-3.0.0rc6/assets/lsp/rename2.mp4`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/assets/lsp/sig-help.gif` & `fortls-3.0.0rc6/assets/lsp/sig-help.gif`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/assets/lsp/sig-help.mp4` & `fortls-3.0.0rc6/assets/lsp/sig-help.mp4`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/assets/lsp/symbols-crop.png` & `fortls-3.0.0rc6/assets/lsp/symbols-crop.png`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/assets/lsp/symbols-doc.png` & `fortls-3.0.0rc6/assets/lsp/symbols-doc.png`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/assets/lsp/symbols-workspace.png` & `fortls-3.0.0rc6/assets/lsp/symbols-workspace.png`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/assets/lsp/symbols.png` & `fortls-3.0.0rc6/assets/lsp/symbols.png`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/assets/symbol-class.svg` & `fortls-3.0.0rc6/assets/symbol-class.svg`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/docs/Makefile` & `fortls-3.0.0rc6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/docs/conf.py` & `fortls-3.0.0rc6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/docs/contact.rst` & `fortls-3.0.0rc6/docs/contact.rst`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/docs/contributing.rst` & `fortls-3.0.0rc6/docs/contributing.rst`

 * *Files 14% similar despite different names*

```diff
@@ -3,24 +3,19 @@
 ======================
 
 There are a few ways you can support the ``fortls`` project.
 
 Financial Support
 ------------------
 
-.. You can support us financially by becoming a **GitHub Sponsor** or by
-.. making a **PayPal Donation**.
+You can fiscally support Fortran-lang by donating to the project, see
+`Fortran-lang - NumFOCUS`_.
 
-.. note::
-    We are in the process of restructuring our Sponsorship structure.
-    In the meantime, please get in contact with ``gnikit`` via email at
-    ``gnikit [@] duck [.] com`` or any other `Administrator of Fortran-lang`_
-    for instructions to financially back the project.
+.. _Fortran-lang - NumFOCUS: https://numfocus.org/donate-for-fortran-lang
 
-.. _Administrator of Fortran-lang: https://github.com/orgs/fortran-lang/teams/admins/members
 
 .. .. grid:: 2
 ..     :gutter: 0
 ..     :class-container: sd-text-center sd-pt-4
 ..     :class-row: sd-align-minor-center
 
 ..     .. grid-item::
```

### Comparing `fortls-3.0.0rc5/docs/editor_integration.rst` & `fortls-3.0.0rc6/docs/editor_integration.rst`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/docs/features.rst` & `fortls-3.0.0rc6/docs/features.rst`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/docs/fortls.parsers.internal.rst` & `fortls-3.0.0rc6/docs/fortls.parsers.internal.rst`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/docs/fortls.rst` & `fortls-3.0.0rc6/docs/fortls.rst`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/docs/index.rst` & `fortls-3.0.0rc6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/docs/make.bat` & `fortls-3.0.0rc6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/docs/options.rst` & `fortls-3.0.0rc6/docs/options.rst`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/docs/quickstart.rst` & `fortls-3.0.0rc6/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/fortls/__init__.py` & `fortls-3.0.0rc6/fortls/__init__.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/fortls/constants.py` & `fortls-3.0.0rc6/fortls/constants.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/fortls/debug.py` & `fortls-3.0.0rc6/fortls/debug.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/fortls/fortls.schema.json` & `fortls-3.0.0rc6/fortls/fortls.schema.json`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/fortls/ftypes.py` & `fortls-3.0.0rc6/fortls/ftypes.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/fortls/helper_functions.py` & `fortls-3.0.0rc6/fortls/helper_functions.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/fortls/interface.py` & `fortls-3.0.0rc6/fortls/interface.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/fortls/json_templates.py` & `fortls-3.0.0rc6/fortls/json_templates.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/fortls/jsonrpc.py` & `fortls-3.0.0rc6/fortls/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/fortls/langserver.py` & `fortls-3.0.0rc6/fortls/langserver.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/fortls/parsers/internal/associate.py` & `fortls-3.0.0rc6/fortls/parsers/internal/associate.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/fortls/parsers/internal/ast.py` & `fortls-3.0.0rc6/fortls/parsers/internal/ast.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/fortls/parsers/internal/base.py` & `fortls-3.0.0rc6/fortls/parsers/internal/base.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/fortls/parsers/internal/block.py` & `fortls-3.0.0rc6/fortls/parsers/internal/block.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/fortls/parsers/internal/diagnostics.py` & `fortls-3.0.0rc6/fortls/parsers/internal/diagnostics.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/fortls/parsers/internal/function.py` & `fortls-3.0.0rc6/fortls/parsers/internal/function.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/fortls/parsers/internal/imports.py` & `fortls-3.0.0rc6/fortls/parsers/internal/imports.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/fortls/parsers/internal/interface.py` & `fortls-3.0.0rc6/fortls/parsers/internal/interface.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/fortls/parsers/internal/intrinsic.modules.json` & `fortls-3.0.0rc6/fortls/parsers/internal/intrinsic.modules.json`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/fortls/parsers/internal/intrinsic.procedures.json` & `fortls-3.0.0rc6/fortls/parsers/internal/intrinsic.procedures.json`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/fortls/parsers/internal/intrinsic.procedures.markdown.json` & `fortls-3.0.0rc6/fortls/parsers/internal/intrinsic.procedures.markdown.json`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/fortls/parsers/internal/intrinsics.py` & `fortls-3.0.0rc6/fortls/parsers/internal/intrinsics.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/fortls/parsers/internal/keywords.json` & `fortls-3.0.0rc6/fortls/parsers/internal/keywords.json`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/fortls/parsers/internal/method.py` & `fortls-3.0.0rc6/fortls/parsers/internal/method.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/fortls/parsers/internal/module.py` & `fortls-3.0.0rc6/fortls/parsers/internal/module.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/fortls/parsers/internal/parser.py` & `fortls-3.0.0rc6/fortls/parsers/internal/parser.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/fortls/parsers/internal/scope.py` & `fortls-3.0.0rc6/fortls/parsers/internal/scope.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/fortls/parsers/internal/select.py` & `fortls-3.0.0rc6/fortls/parsers/internal/select.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/fortls/parsers/internal/statements.json` & `fortls-3.0.0rc6/fortls/parsers/internal/statements.json`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/fortls/parsers/internal/submodule.py` & `fortls-3.0.0rc6/fortls/parsers/internal/submodule.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/fortls/parsers/internal/subroutine.py` & `fortls-3.0.0rc6/fortls/parsers/internal/subroutine.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/fortls/parsers/internal/type.py` & `fortls-3.0.0rc6/fortls/parsers/internal/type.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/fortls/parsers/internal/use.py` & `fortls-3.0.0rc6/fortls/parsers/internal/use.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/fortls/parsers/internal/utilities.py` & `fortls-3.0.0rc6/fortls/parsers/internal/utilities.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/fortls/parsers/internal/variable.py` & `fortls-3.0.0rc6/fortls/parsers/internal/variable.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/fortls/regex_patterns.py` & `fortls-3.0.0rc6/fortls/regex_patterns.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/fortls/schema.py` & `fortls-3.0.0rc6/fortls/schema.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/fortls.egg-info/PKG-INFO` & `fortls-3.0.0rc6/fortls.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fortls
-Version: 3.0.0rc5
+Version: 3.0.0rc6
 Summary: fortls - Fortran Language Server
 Author-email: Giannis Nikiteas <giannis.nikiteas@gmail.com>
 License: MIT
 Project-URL: homepage, https://fortls.fortran-lang.org
 Project-URL: Documentation, https://fortls.fortran-lang.org
 Project-URL: Changes, https://github.com/fortran-lang/fortls/blob/master/CHANGELOG.md
 Project-URL: Tracker, https://github.com/fortran-lang/fortls/issues
@@ -64,14 +64,15 @@
 ![Conda](https://img.shields.io/conda/dn/conda-forge/fortls?label=Anaconda&style=flat-square)
 ![GitHub License](https://img.shields.io/github/license/fortran-lang/fortls?style=flat-square)
 ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/fortran-lang/fortls/main.yml?branch=master&label=CI&style=flat-square)
 ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/fortran-lang/fortls/docs.yml?branch=master&label=Docs&style=flat-square)
 ![Codecov](https://img.shields.io/codecov/c/github/fortran-lang/fortls?style=flat-square)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/psf/black)
 ![GitHub Repo stars](https://img.shields.io/github/stars/fortran-lang/fortls?color=yellow&style=flat-square)
+[![DOI](https://zenodo.org/badge/412392321.svg?style=flat-square)](https://zenodo.org/badge/latestdoi/412392321)
 
 <!-- [<img alt="https://github.com/sponsors/gnikit" src="https://img.shields.io/static/v1?style=social&label=Sponsor&message=%E2%9D%A4&logo=GitHub&color&link=%3Curl%3E" height="30" />](https://github.com/sponsors/gnikit)
 [<img alt="https://paypal.me/inikit" src="https://img.shields.io/static/v1?style=social&label=Donate&message=%E2%9D%A4&logo=Paypal&color&link=%3Curl%3E" height="30" />](https://paypal.me/inikit) -->
 
 ![alt](https://raw.githubusercontent.com/fortran-lang/fortls/master/assets/animations/intro-demo.gif)
 
 `fortls` is an implementation of the [Language Server Protocol](https://github.com/Microsoft/language-server-protocol)
@@ -116,30 +117,18 @@
   - Generate type-bound procedures and implementation templates for
     deferred procedures
 
 ### Notes/Limitations
 
 - Signature help and hover does not handle elegantly overloaded functions i.e. interfaces
 
-## Future plans
-
-`fortls` has reached a point where it is feature complete and stable enough to be used in many modern Fortran projects without any issues.
-It does however still have fundamental limitations,
-namely its ability to understand all Fortran syntax and semantics that has been used throughout the 65+ years of the language. **The good news is that we have a plan to address this issue!**
-
-We are excited to announce that we are working on creating a new Fortran Language Server
-based on the actively developed [LFortran](https://lfortran.org/) compiler 🎉.
-The new Language Server will be able to understand all Fortran syntax, be faster,
-and give more accurate autocompletion, hover and diagnostic information. That means we plan on investing any future funding on creating our new language server and ultimately creating a better user experience for everyone.
-
-<!--  Have a look at our roadmap (link) and consider contributing to our efforts (donations and contribution tasks link).  -->
+## Documentation
 
-### What about `fortls`?
-
-Not to worry, `fortls` will continue to be here. We will keep `fortls` in maintenance mode with bug fixes and new features from volunteer contributors, but otherwise we will be focusing our efforts into making the new LFortran language server a reality.
+The full documentation for `fortls` can be found at
+[fortls.fortran-lang.org](https://fortls.fortran-lang.org/).
 
 ## Installation
 
 ### PyPi
 
 ```sh
 pip install fortls
@@ -213,14 +202,31 @@
 | `textDocument/rename`            | Rename a symbol across the workspace                   |
 | `textDocument/didOpen`           | Document synchronisation upon opening                  |
 | `textDocument/didSave`           | Document synchronisation upon saving                   |
 | `textDocument/didClose`          | Document synchronisation upon closing                  |
 | `textDocument/didChange`         | Document synchronisation upon changes to the document  |
 | `textDocument/codeAction`        | **Experimental** Generate code                         |
 
+## Future plans
+
+`fortls` has reached a point where it is feature complete and stable enough to be used in many modern Fortran projects without any issues.
+It does however still have fundamental limitations,
+namely its ability to understand all Fortran syntax and semantics that has been used throughout the 65+ years of the language. **The good news is that we have a plan to address this issue!**
+
+We are excited to announce that we are working on creating a new Fortran Language Server
+based on the actively developed [LFortran](https://lfortran.org/) compiler 🎉.
+The new Language Server will be able to understand all Fortran syntax, be faster,
+and give more accurate autocompletion, hover and diagnostic information. That means we plan on investing any future funding on creating our new language server and ultimately creating a better user experience for everyone.
+
+<!--  Have a look at our roadmap (link) and consider contributing to our efforts (donations and contribution tasks link).  -->
+
+### What about `fortls`?
+
+Not to worry, `fortls` will continue to be here. We will keep `fortls` in active maintenance mode with bug fixes and new features from volunteer contributors, but otherwise we will be focusing our efforts into making the new language server using LFortran's parser a reality.
+
 ## `fortls` vs `fortran-language-server`
 
 This project was originally based on `fortran-language-server` LSP implementation, but the two projects have since diverged.
 
 `fortls` (this project) is now developed independently of the upstream `hansec/fortran-language-server` project and contains numerous new features and bug fixes
 the original `fortran-language-server` does not.
 
@@ -232,20 +238,18 @@
 change in the future.
 
 ## Acknowledgements
 
 This project would not have been possible without the original work of [@hansec](https://github.com/hansec/)
 in [`fortran-language-server`](https://github.com/hansec/fortran-language-server)
 
-<!-- ## Support
-
-If you want to support this project you can do it through
+## Support
 
-[![Alt](https://www.paypalobjects.com/webstatic/mktg/Logo/pp-logo-150px.png)](https://paypal.me/inikit)
-[!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/gnikit) -->
+You can support Fortran-lang as a whole by donating at
+[Fortran-lang - NumFOCUS](https://numfocus.org/donate-for-fortran-lang).
 
 ## Bug reports
 
 When [filing bugs](https://github.com/fortran-lang/fortls/issues/new)
 please provide example code to reproduce the observed issue.
 
 ## Security Policy
```

### Comparing `fortls-3.0.0rc5/fortls.egg-info/SOURCES.txt` & `fortls-3.0.0rc6/fortls.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/licenses/fortran-language-server-license.txt` & `fortls-3.0.0rc6/licenses/fortran-language-server-license.txt`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/pyproject.toml` & `fortls-3.0.0rc6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/test/setup_tests.py` & `fortls-3.0.0rc6/test/setup_tests.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/test/test_interface.py` & `fortls-3.0.0rc6/test/test_interface.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/test/test_parser.py` & `fortls-3.0.0rc6/test/test_parser.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/test/test_preproc.py` & `fortls-3.0.0rc6/test/test_preproc.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/test/test_preproc_parser.py` & `fortls-3.0.0rc6/test/test_preproc_parser.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/test/test_regex_patterns.py` & `fortls-3.0.0rc6/test/test_regex_patterns.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/test/test_server.py` & `fortls-3.0.0rc6/test/test_server.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/test/test_server_completion.py` & `fortls-3.0.0rc6/test/test_server_completion.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/test/test_server_definitions.py` & `fortls-3.0.0rc6/test/test_server_definitions.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/test/test_server_diagnostics.py` & `fortls-3.0.0rc6/test/test_server_diagnostics.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/test/test_server_documentation.py` & `fortls-3.0.0rc6/test/test_server_documentation.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/test/test_server_hover.py` & `fortls-3.0.0rc6/test/test_server_hover.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/test/test_server_implementation.py` & `fortls-3.0.0rc6/test/test_server_implementation.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/test/test_server_messages.py` & `fortls-3.0.0rc6/test/test_server_messages.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/test/test_server_references.py` & `fortls-3.0.0rc6/test/test_server_references.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/test/test_server_rename.py` & `fortls-3.0.0rc6/test/test_server_rename.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/test/test_server_signature_help.py` & `fortls-3.0.0rc6/test/test_server_signature_help.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/test/test_source/completion/use_only_interface.f90` & `fortls-3.0.0rc6/test/test_source/completion/use_only_interface.f90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/test/test_source/diag/test_function_arg_list.f90` & `fortls-3.0.0rc6/test/test_source/diag/test_function_arg_list.f90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/test/test_source/diag/test_scope_overreach.f90` & `fortls-3.0.0rc6/test/test_source/diag/test_scope_overreach.f90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/test/test_source/diag/test_semicolon.f90` & `fortls-3.0.0rc6/test/test_source/diag/test_semicolon.f90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/test/test_source/docs/test_doxygen.f90` & `fortls-3.0.0rc6/test/test_source/docs/test_doxygen.f90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/test/test_source/docs/test_ford.f90` & `fortls-3.0.0rc6/test/test_source/docs/test_ford.f90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/test/test_source/excldir/sub1/tmp.f90` & `fortls-3.0.0rc6/test/test_source/excldir/sub1/tmp.f90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/test/test_source/f90_config.json` & `fortls-3.0.0rc6/test/test_source/f90_config.json`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/test/test_source/hover/functions.f90` & `fortls-3.0.0rc6/test/test_source/hover/functions.f90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/test/test_source/hover/parameters.f90` & `fortls-3.0.0rc6/test/test_source/hover/parameters.f90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/test/test_source/hover/recursive.f90` & `fortls-3.0.0rc6/test/test_source/hover/recursive.f90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/test/test_source/imp/import.f90` & `fortls-3.0.0rc6/test/test_source/imp/import.f90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/test/test_source/imp/submodule.f90` & `fortls-3.0.0rc6/test/test_source/imp/submodule.f90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/test/test_source/parse/test_kinds_and_dims.f90` & `fortls-3.0.0rc6/test/test_source/parse/test_kinds_and_dims.f90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/test/test_source/pp/preproc_elif.F90` & `fortls-3.0.0rc6/test/test_source/pp/preproc_elif.F90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/test/test_source/pp/preproc_elif_elif_skip.F90` & `fortls-3.0.0rc6/test/test_source/pp/preproc_elif_elif_skip.F90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/test/test_source/pp/preproc_if_elif_else.F90` & `fortls-3.0.0rc6/test/test_source/pp/preproc_if_elif_else.F90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/test/test_source/pp/preproc_if_elif_skip.F90` & `fortls-3.0.0rc6/test/test_source/pp/preproc_if_elif_skip.F90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/test/test_source/rename/test_rename_intrinsic.f90` & `fortls-3.0.0rc6/test/test_source/rename/test_rename_intrinsic.f90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/test/test_source/signature/help.f90` & `fortls-3.0.0rc6/test/test_source/signature/help.f90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/test/test_source/subdir/test_fixed.f` & `fortls-3.0.0rc6/test/test_source/subdir/test_fixed.f`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/test/test_source/subdir/test_free.f90` & `fortls-3.0.0rc6/test/test_source/subdir/test_free.f90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/test/test_source/subdir/test_generic.f90` & `fortls-3.0.0rc6/test/test_source/subdir/test_generic.f90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/test/test_source/subdir/test_select.f90` & `fortls-3.0.0rc6/test/test_source/subdir/test_select.f90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/test/test_source/subdir/test_submod.F90` & `fortls-3.0.0rc6/test/test_source/subdir/test_submod.F90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/test/test_source/test_diagnostic_int.f90` & `fortls-3.0.0rc6/test/test_source/test_diagnostic_int.f90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc5/test/test_source/test_prog.f08` & `fortls-3.0.0rc6/test/test_source/test_prog.f08`

 * *Files identical despite different names*

