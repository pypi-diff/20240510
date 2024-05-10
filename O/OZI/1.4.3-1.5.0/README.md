# Comparing `tmp/OZI-1.4.3.tar.gz` & `tmp/OZI-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OZI-1.4.3.tar", last modified: Wed May  8 03:06:38 2024, max compression
+gzip compressed data, was "OZI-1.5.0.tar", last modified: Thu May  9 05:39:40 2024, max compression
```

## Comparing `OZI-1.4.3.tar` & `OZI-1.5.0.tar`

### file list

```diff
@@ -1,135 +1,135 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:06:38.368252 OZI-1.4.3/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:06:38.340252 OZI-1.4.3/.github/
--rw-rw-r--   0 runner    (1001) docker     (127)      102 2024-05-08 03:02:20.000000 OZI-1.4.3/.github/.markdownlint.json
--rw-rw-r--   0 runner    (1001) docker     (127)      574 2024-05-08 03:02:20.000000 OZI-1.4.3/.github/CODEOWNERS
--rw-rw-r--   0 runner    (1001) docker     (127)     3227 2024-05-08 03:02:20.000000 OZI-1.4.3/.github/CODE_OF_CONDUCT.md
--rw-rw-r--   0 runner    (1001) docker     (127)     2862 2024-05-08 03:02:20.000000 OZI-1.4.3/.github/CONTRIBUTING.md
--rw-rw-r--   0 runner    (1001) docker     (127)       85 2024-05-08 03:02:20.000000 OZI-1.4.3/.github/FUNDING.yml
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:06:38.340252 OZI-1.4.3/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 runner    (1001) docker     (127)      834 2024-05-08 03:02:20.000000 OZI-1.4.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-rw-r--   0 runner    (1001) docker     (127)      595 2024-05-08 03:02:20.000000 OZI-1.4.3/.github/ISSUE_TEMPLATE/feature_request.md
--rw-rw-r--   0 runner    (1001) docker     (127)     1696 2024-05-08 03:02:20.000000 OZI-1.4.3/.github/SECURITY.md
--rw-rw-r--   0 runner    (1001) docker     (127)      434 2024-05-08 03:02:20.000000 OZI-1.4.3/.github/dependabot.yml
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:06:38.340252 OZI-1.4.3/.github/workflows/
--rw-rw-r--   0 runner    (1001) docker     (127)     3081 2024-05-08 03:02:20.000000 OZI-1.4.3/.github/workflows/codeql.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     1091 2024-05-08 03:02:20.000000 OZI-1.4.3/.github/workflows/dependency-review.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     2900 2024-05-08 03:02:20.000000 OZI-1.4.3/.github/workflows/dev-workflow.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     5873 2024-05-08 03:02:20.000000 OZI-1.4.3/.github/workflows/dist-workflow.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     3544 2024-05-08 03:02:20.000000 OZI-1.4.3/.github/workflows/scorecard.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     3194 2024-05-08 03:02:20.000000 OZI-1.4.3/.gitignore
--rw-rw-r--   0 runner    (1001) docker     (127)   301620 2024-05-08 03:02:20.000000 OZI-1.4.3/CHANGELOG.md
--rw-rw-r--   0 runner    (1001) docker     (127)    12456 2024-05-08 03:02:20.000000 OZI-1.4.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8627 2024-05-08 03:06:38.136252 OZI-1.4.3/PKG-INFO
--rw-rw-r--   0 runner    (1001) docker     (127)     6937 2024-05-08 03:02:20.000000 OZI-1.4.3/README.rst
--rw-rw-r--   0 runner    (1001) docker     (127)    16724 2024-05-08 03:02:20.000000 OZI-1.4.3/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     7664 2024-05-08 03:02:20.000000 OZI-1.4.3/meson.options
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:06:38.364252 OZI-1.4.3/ozi/
--rw-rw-r--   0 runner    (1001) docker     (127)      502 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     3418 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/__main__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     7089 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/actions.py
--rw-rw-r--   0 runner    (1001) docker     (127)     5811 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/comment.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:06:38.348252 OZI-1.4.3/ozi/dist/
--rw-rw-r--   0 runner    (1001) docker     (127)      481 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/dist/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:06:38.348252 OZI-1.4.3/ozi/dist/semantic_release/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/dist/semantic_release/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       26 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/dist/semantic_release/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:06:38.348252 OZI-1.4.3/ozi/dist/sigstore/
--rw-rw-r--   0 runner    (1001) docker     (127)      412 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/dist/sigstore/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)        8 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/dist/sigstore/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:06:38.352252 OZI-1.4.3/ozi/fix/
--rw-rw-r--   0 runner    (1001) docker     (127)      278 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/fix/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2469 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/fix/__main__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4061 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/fix/build_definition.py
--rw-rw-r--   0 runner    (1001) docker     (127)      619 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/fix/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     6305 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/fix/missing.py
--rw-rw-r--   0 runner    (1001) docker     (127)     3612 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/fix/parser.py
--rw-rw-r--   0 runner    (1001) docker     (127)     7877 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/fix/rewrite_command.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:06:38.356252 OZI-1.4.3/ozi/lint/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:06:38.352252 OZI-1.4.3/ozi/lint/bandit/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/lint/bandit/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       12 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/lint/bandit/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:06:38.352252 OZI-1.4.3/ozi/lint/black/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/lint/black/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       14 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/lint/black/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:06:38.352252 OZI-1.4.3/ozi/lint/flake8/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/lint/flake8/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      276 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/lint/flake8/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:06:38.352252 OZI-1.4.3/ozi/lint/isort/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/lint/isort/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)        5 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/lint/isort/requirements.in
--rw-rw-r--   0 runner    (1001) docker     (127)      553 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/lint/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:06:38.352252 OZI-1.4.3/ozi/lint/mypy/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/lint/mypy/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)        4 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/lint/mypy/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:06:38.356252 OZI-1.4.3/ozi/lint/pyright/
--rw-rw-r--   0 runner    (1001) docker     (127)      799 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/lint/pyright/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       16 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/lint/pyright/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:06:38.356252 OZI-1.4.3/ozi/lint/restructuredtext-lint/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/lint/restructuredtext-lint/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       21 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/lint/restructuredtext-lint/requirements.in
--rw-rw-r--   0 runner    (1001) docker     (127)      808 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     8128 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/meson.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:06:38.356252 OZI-1.4.3/ozi/new/
--rw-rw-r--   0 runner    (1001) docker     (127)      249 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/new/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4813 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/new/__main__.py
--rw-rw-r--   0 runner    (1001) docker     (127)      567 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/new/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     6436 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/new/parser.py
--rw-rw-r--   0 runner    (1001) docker     (127)     8155 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/new/validate.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2606 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/pkg_extra.py
--rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/py.typed
--rw-rw-r--   0 runner    (1001) docker     (127)     4801 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/render.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:06:38.360252 OZI-1.4.3/ozi/scripts/
--rw-rw-r--   0 runner    (1001) docker     (127)     1494 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/scripts/core_metadata_template.py
--rw-rw-r--   0 runner    (1001) docker     (127)      771 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/scripts/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     2088 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/scripts/meson_dist_setuptools_scm.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1850 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/scripts/meson_setuptools_scm.py
--rw-rw-r--   0 runner    (1001) docker     (127)      864 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/scripts/render_requirements.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1026 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/scripts/replace_ruff_target_version.py
--rw-rw-r--   0 runner    (1001) docker     (127)      721 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/scripts/scm_version_snip.py
--rw-rw-r--   0 runner    (1001) docker     (127)      716 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/scripts/to_distribution_template.py
--rw-rw-r--   0 runner    (1001) docker     (127)      589 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/scripts/version_metadata_template.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1045 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/spdx.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:06:38.360252 OZI-1.4.3/ozi/spec/
--rw-rw-r--   0 runner    (1001) docker     (127)      459 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/spec/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4120 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/spec/_license.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1687 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/spec/_spec.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2414 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/spec/base.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6066 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/spec/ci.py
--rw-rw-r--   0 runner    (1001) docker     (127)      641 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/spec/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     4445 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/spec/pkg.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1373 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/spec/project.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6472 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/spec/python.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4572 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/spec/src.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6649 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/tap.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:06:38.364252 OZI-1.4.3/ozi/test/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:06:38.360252 OZI-1.4.3/ozi/test/coverage/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/test/coverage/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      195 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/test/coverage/requirements.in
--rw-rw-r--   0 runner    (1001) docker     (127)      454 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/test/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:06:38.364252 OZI-1.4.3/ozi/test/pytest/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/test/pytest/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      104 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/test/pytest/requirements.in
--rw-rw-r--   0 runner    (1001) docker     (127)     1990 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/trove.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:06:38.364252 OZI-1.4.3/ozi/vendor/
--rw-rw-r--   0 runner    (1001) docker     (127)       26 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/vendor/__init__.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:06:38.364252 OZI-1.4.3/ozi/vendor/email_validator/
--rw-rw-r--   0 runner    (1001) docker     (127)     4283 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/vendor/email_validator/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2181 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/vendor/email_validator/__main__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6121 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/vendor/email_validator/deliverability.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6000 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/vendor/email_validator/exceptions_types.py
--rw-rw-r--   0 runner    (1001) docker     (127)      736 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/vendor/email_validator/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/vendor/email_validator/py.typed
--rw-rw-r--   0 runner    (1001) docker     (127)     2768 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/vendor/email_validator/rfc_constants.py
--rw-rw-r--   0 runner    (1001) docker     (127)    28340 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/vendor/email_validator/syntax.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6845 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/vendor/email_validator/validate_email.py
--rw-rw-r--   0 runner    (1001) docker     (127)       28 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/vendor/email_validator/version.py
--rw-rw-r--   0 runner    (1001) docker     (127)      659 2024-05-08 03:02:20.000000 OZI-1.4.3/ozi/vendor/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)    10899 2024-05-08 03:02:20.000000 OZI-1.4.3/pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)      190 2024-05-08 03:02:20.000000 OZI-1.4.3/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:06:38.368252 OZI-1.4.3/templates/
--rw-rw-r--   0 runner    (1001) docker     (127)     1152 2024-05-08 03:02:20.000000 OZI-1.4.3/templates/CHANGELOG.md.j2
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:06:38.368252 OZI-1.4.3/tests/
--rw-rw-r--   0 runner    (1001) docker     (127)      556 2024-05-08 03:02:20.000000 OZI-1.4.3/tests/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)    11072 2024-05-08 03:02:20.000000 OZI-1.4.3/tests/test_ozi_fix.py
--rw-rw-r--   0 runner    (1001) docker     (127)    14164 2024-05-08 03:02:20.000000 OZI-1.4.3/tests/test_ozi_new.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2238 2024-05-08 03:02:20.000000 OZI-1.4.3/tests/test_tap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:39:40.739245 OZI-1.5.0/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:39:40.711245 OZI-1.5.0/.github/
+-rw-rw-r--   0 runner    (1001) docker     (127)      102 2024-05-09 05:35:30.000000 OZI-1.5.0/.github/.markdownlint.json
+-rw-rw-r--   0 runner    (1001) docker     (127)      574 2024-05-09 05:35:30.000000 OZI-1.5.0/.github/CODEOWNERS
+-rw-rw-r--   0 runner    (1001) docker     (127)     3227 2024-05-09 05:35:30.000000 OZI-1.5.0/.github/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 runner    (1001) docker     (127)     2862 2024-05-09 05:35:30.000000 OZI-1.5.0/.github/CONTRIBUTING.md
+-rw-rw-r--   0 runner    (1001) docker     (127)       85 2024-05-09 05:35:30.000000 OZI-1.5.0/.github/FUNDING.yml
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:39:40.707244 OZI-1.5.0/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 runner    (1001) docker     (127)      834 2024-05-09 05:35:30.000000 OZI-1.5.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-rw-r--   0 runner    (1001) docker     (127)      595 2024-05-09 05:35:30.000000 OZI-1.5.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-rw-r--   0 runner    (1001) docker     (127)     1696 2024-05-09 05:35:30.000000 OZI-1.5.0/.github/SECURITY.md
+-rw-rw-r--   0 runner    (1001) docker     (127)      434 2024-05-09 05:35:30.000000 OZI-1.5.0/.github/dependabot.yml
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:39:40.711245 OZI-1.5.0/.github/workflows/
+-rw-rw-r--   0 runner    (1001) docker     (127)     3081 2024-05-09 05:35:30.000000 OZI-1.5.0/.github/workflows/codeql.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     1091 2024-05-09 05:35:30.000000 OZI-1.5.0/.github/workflows/dependency-review.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     2900 2024-05-09 05:35:30.000000 OZI-1.5.0/.github/workflows/dev-workflow.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     5873 2024-05-09 05:35:30.000000 OZI-1.5.0/.github/workflows/dist-workflow.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     3544 2024-05-09 05:35:30.000000 OZI-1.5.0/.github/workflows/scorecard.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     3194 2024-05-09 05:35:30.000000 OZI-1.5.0/.gitignore
+-rw-rw-r--   0 runner    (1001) docker     (127)   302932 2024-05-09 05:35:30.000000 OZI-1.5.0/CHANGELOG.md
+-rw-rw-r--   0 runner    (1001) docker     (127)    12456 2024-05-09 05:35:30.000000 OZI-1.5.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8627 2024-05-09 05:39:40.503243 OZI-1.5.0/PKG-INFO
+-rw-rw-r--   0 runner    (1001) docker     (127)     6937 2024-05-09 05:35:30.000000 OZI-1.5.0/README.rst
+-rw-rw-r--   0 runner    (1001) docker     (127)    16724 2024-05-09 05:35:30.000000 OZI-1.5.0/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     7664 2024-05-09 05:35:30.000000 OZI-1.5.0/meson.options
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:39:40.735245 OZI-1.5.0/ozi/
+-rw-rw-r--   0 runner    (1001) docker     (127)      502 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     3418 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/__main__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     7089 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/actions.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     5811 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/comment.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:39:40.719245 OZI-1.5.0/ozi/dist/
+-rw-rw-r--   0 runner    (1001) docker     (127)      481 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/dist/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:39:40.719245 OZI-1.5.0/ozi/dist/semantic_release/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/dist/semantic_release/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       26 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/dist/semantic_release/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:39:40.719245 OZI-1.5.0/ozi/dist/sigstore/
+-rw-rw-r--   0 runner    (1001) docker     (127)      412 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/dist/sigstore/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)        8 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/dist/sigstore/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:39:40.723245 OZI-1.5.0/ozi/fix/
+-rw-rw-r--   0 runner    (1001) docker     (127)      278 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/fix/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2469 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/fix/__main__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4061 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/fix/build_definition.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      619 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/fix/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     6305 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/fix/missing.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     3612 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/fix/parser.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     7879 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/fix/rewrite_command.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:39:40.723245 OZI-1.5.0/ozi/lint/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:39:40.723245 OZI-1.5.0/ozi/lint/bandit/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/lint/bandit/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       12 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/lint/bandit/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:39:40.723245 OZI-1.5.0/ozi/lint/black/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/lint/black/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       14 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/lint/black/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:39:40.723245 OZI-1.5.0/ozi/lint/flake8/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/lint/flake8/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      276 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/lint/flake8/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:39:40.723245 OZI-1.5.0/ozi/lint/isort/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/lint/isort/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)        5 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/lint/isort/requirements.in
+-rw-rw-r--   0 runner    (1001) docker     (127)      553 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/lint/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:39:40.723245 OZI-1.5.0/ozi/lint/mypy/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/lint/mypy/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)        4 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/lint/mypy/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:39:40.723245 OZI-1.5.0/ozi/lint/pyright/
+-rw-rw-r--   0 runner    (1001) docker     (127)      799 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/lint/pyright/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       16 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/lint/pyright/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:39:40.723245 OZI-1.5.0/ozi/lint/restructuredtext-lint/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/lint/restructuredtext-lint/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       21 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/lint/restructuredtext-lint/requirements.in
+-rw-rw-r--   0 runner    (1001) docker     (127)      808 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     8128 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/meson.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:39:40.727245 OZI-1.5.0/ozi/new/
+-rw-rw-r--   0 runner    (1001) docker     (127)      249 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/new/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4813 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/new/__main__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      567 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/new/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     6733 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/new/parser.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     8155 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/new/validate.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2606 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/pkg_extra.py
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/py.typed
+-rw-rw-r--   0 runner    (1001) docker     (127)     6744 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/render.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:39:40.727245 OZI-1.5.0/ozi/scripts/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1494 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/scripts/core_metadata_template.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      771 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/scripts/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     2088 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/scripts/meson_dist_setuptools_scm.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1850 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/scripts/meson_setuptools_scm.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      864 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/scripts/render_requirements.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1026 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/scripts/replace_ruff_target_version.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      721 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/scripts/scm_version_snip.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      716 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/scripts/to_distribution_template.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      589 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/scripts/version_metadata_template.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1045 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/spdx.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:39:40.731245 OZI-1.5.0/ozi/spec/
+-rw-rw-r--   0 runner    (1001) docker     (127)      459 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/spec/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4120 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/spec/_license.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1687 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/spec/_spec.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2414 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/spec/base.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6066 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/spec/ci.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      641 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/spec/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     4445 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/spec/pkg.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1373 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/spec/project.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6472 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/spec/python.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4572 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/spec/src.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6649 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/tap.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:39:40.731245 OZI-1.5.0/ozi/test/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:39:40.731245 OZI-1.5.0/ozi/test/coverage/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/test/coverage/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      195 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/test/coverage/requirements.in
+-rw-rw-r--   0 runner    (1001) docker     (127)      454 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/test/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:39:40.731245 OZI-1.5.0/ozi/test/pytest/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/test/pytest/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      104 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/test/pytest/requirements.in
+-rw-rw-r--   0 runner    (1001) docker     (127)     1990 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/trove.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:39:40.735245 OZI-1.5.0/ozi/vendor/
+-rw-rw-r--   0 runner    (1001) docker     (127)       26 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/vendor/__init__.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:39:40.735245 OZI-1.5.0/ozi/vendor/email_validator/
+-rw-rw-r--   0 runner    (1001) docker     (127)     4283 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/vendor/email_validator/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2181 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/vendor/email_validator/__main__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6121 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/vendor/email_validator/deliverability.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6000 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/vendor/email_validator/exceptions_types.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      736 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/vendor/email_validator/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/vendor/email_validator/py.typed
+-rw-rw-r--   0 runner    (1001) docker     (127)     2768 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/vendor/email_validator/rfc_constants.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    28340 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/vendor/email_validator/syntax.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6845 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/vendor/email_validator/validate_email.py
+-rw-rw-r--   0 runner    (1001) docker     (127)       28 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/vendor/email_validator/version.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      659 2024-05-09 05:35:30.000000 OZI-1.5.0/ozi/vendor/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)    11029 2024-05-09 05:35:30.000000 OZI-1.5.0/pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)      190 2024-05-09 05:35:30.000000 OZI-1.5.0/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:39:40.739245 OZI-1.5.0/templates/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1152 2024-05-09 05:35:30.000000 OZI-1.5.0/templates/CHANGELOG.md.j2
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:39:40.739245 OZI-1.5.0/tests/
+-rw-rw-r--   0 runner    (1001) docker     (127)      556 2024-05-09 05:35:30.000000 OZI-1.5.0/tests/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)    11130 2024-05-09 05:35:30.000000 OZI-1.5.0/tests/test_ozi_fix.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    14164 2024-05-09 05:35:30.000000 OZI-1.5.0/tests/test_ozi_new.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2238 2024-05-09 05:35:30.000000 OZI-1.5.0/tests/test_tap.py
```

### Comparing `OZI-1.4.3/.github/CODEOWNERS` & `OZI-1.5.0/.github/CODEOWNERS`

 * *Files identical despite different names*

### Comparing `OZI-1.4.3/.github/CODE_OF_CONDUCT.md` & `OZI-1.5.0/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `OZI-1.4.3/.github/CONTRIBUTING.md` & `OZI-1.5.0/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `OZI-1.4.3/.github/ISSUE_TEMPLATE/bug_report.md` & `OZI-1.5.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `OZI-1.4.3/.github/ISSUE_TEMPLATE/feature_request.md` & `OZI-1.5.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `OZI-1.4.3/.github/SECURITY.md` & `OZI-1.5.0/.github/SECURITY.md`

 * *Files identical despite different names*

### Comparing `OZI-1.4.3/.github/workflows/codeql.yml` & `OZI-1.5.0/.github/workflows/codeql.yml`

 * *Files 13% similar despite different names*

```diff
@@ -52,33 +52,33 @@
             uploads.github.com:443
 
       - name: Checkout repository
         uses: actions/checkout@44c2b7a8a4ea60a981eaca3cf939b5f4305c123b # v4.1.5
 
       # Initializes the CodeQL tools for scanning.
       - name: Initialize CodeQL
-        uses: github/codeql-action/init@d39d31e687223d841ef683f52467bd88e9b21c14 # v3.25.3
+        uses: github/codeql-action/init@ccf74c947955fd1cf117aef6a0e4e66191ef6f61 # v3.25.4
         with:
           languages: ${{ matrix.language }}
           # If you wish to specify custom queries, you can do so here or in a config file.
           # By default, queries listed here will override any specified in a config file.
           # Prefix the list here with "+" to use these queries and those in the config file.
 
       # Autobuild attempts to build any compiled languages  (C/C++, C#, or Java).
       # If this step fails, then you should remove it and run the build manually (see below)
       - name: Autobuild
-        uses: github/codeql-action/autobuild@d39d31e687223d841ef683f52467bd88e9b21c14 # v3.25.3
+        uses: github/codeql-action/autobuild@ccf74c947955fd1cf117aef6a0e4e66191ef6f61 # v3.25.4
 
       # ℹ️ Command-line programs to run using the OS shell.
       # 📚 See https://docs.github.com/en/actions/using-workflows/workflow-syntax-for-github-actions#jobsjob_idstepsrun
 
       #   If the Autobuild fails above, remove it and uncomment the following three lines.
       #   modify them (or add more) to build your code if your project, please refer to the EXAMPLE below for guidance.
 
       # - run: |
       #   echo "Run, Build Application using script"
       #   ./location_of_script_within_repo/buildscript.sh
 
       - name: Perform CodeQL Analysis
-        uses: github/codeql-action/analyze@d39d31e687223d841ef683f52467bd88e9b21c14 # v3.25.3
+        uses: github/codeql-action/analyze@ccf74c947955fd1cf117aef6a0e4e66191ef6f61 # v3.25.4
         with:
           category: "/language:${{matrix.language}}"
```

### Comparing `OZI-1.4.3/.github/workflows/dependency-review.yml` & `OZI-1.5.0/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `OZI-1.4.3/.github/workflows/dev-workflow.yml` & `OZI-1.5.0/.github/workflows/dev-workflow.yml`

 * *Files identical despite different names*

### Comparing `OZI-1.4.3/.github/workflows/dist-workflow.yml` & `OZI-1.5.0/.github/workflows/dist-workflow.yml`

 * *Files identical despite different names*

### Comparing `OZI-1.4.3/.github/workflows/scorecard.yml` & `OZI-1.5.0/.github/workflows/scorecard.yml`

 * *Files 8% similar despite different names*

```diff
@@ -79,10 +79,10 @@
         with:
           name: SARIF file
           path: results.sarif
           retention-days: 5
 
       # Upload the results to GitHub's code scanning dashboard.
       - name: "Upload to code-scanning"
-        uses: github/codeql-action/upload-sarif@d39d31e687223d841ef683f52467bd88e9b21c14 # v3.25.3
+        uses: github/codeql-action/upload-sarif@ccf74c947955fd1cf117aef6a0e4e66191ef6f61 # v3.25.4
         with:
           sarif_file: results.sarif
```

### Comparing `OZI-1.4.3/.gitignore` & `OZI-1.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `OZI-1.4.3/CHANGELOG.md` & `OZI-1.5.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,43 @@
 # CHANGELOG
+## 1.5.0 (2024-05-09)
+
+### :arrow_up:
+
+* :arrow_up: Bump github/codeql-action from 3.25.3 to 3.25.4
+
+Bumps [github/codeql-action](https://github.com/github/codeql-action) from 3.25.3 to 3.25.4.
+- [Release notes](https://github.com/github/codeql-action/releases)
+- [Changelog](https://github.com/github/codeql-action/blob/main/CHANGELOG.md)
+- [Commits](https://github.com/github/codeql-action/compare/d39d31e687223d841ef683f52467bd88e9b21c14...ccf74c947955fd1cf117aef6a0e4e66191ef6f61)
+
+---
+updated-dependencies:
+- dependency-name: github/codeql-action
+  dependency-type: direct:production
+  update-type: version-update:semver-patch
+...
+
+Signed-off-by: dependabot[bot] &lt;support@github.com&gt; ([`8e83edb`](https://github.com/OZI-Project/OZI/commit/8e83edbd2c514fa57bb9cccf51730f9eebc6a6e8))
+
+### :sparkles:
+
+* :sparkles:  Add cython extensions with ``ozi-fix``
+
+Also add ``--[no-]enable-cython`` to ``ozi-new``.
+:arrow_up: blastpipe 2024.5
+
+Signed-off-by: rjdbcm &lt;ozi.project@outlook.com&gt; ([`407db9b`](https://github.com/OZI-Project/OZI/commit/407db9b1abc53b30e9aa73ab589a2e5b0056f726))
+
+### :wrench:
+
+* :wrench: add 1.5 release branch group
+
+Signed-off-by: Eden Rose, MSc &lt;ozi.project@outlook.com&gt; ([`fa09315`](https://github.com/OZI-Project/OZI/commit/fa09315597531d789b1a364e35bdb3885e20e301))
+
 ## 1.4.3 (2024-05-08)
 
 ### :arrow_up:
 
 * :arrow_up: Bump OZI-Project workflow actions
 
 * OZI-Project/checkpoint 0.1.6
```

### Comparing `OZI-1.4.3/LICENSE.txt` & `OZI-1.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.4.3/PKG-INFO` & `OZI-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: OZI
-Version: 1.4.3
+Version: 1.5.0
 Summary: Packager for Python projects using Meson.
-Download-URL: https://github.com/rjdbcm/OZI/archive/refs/tags/1.4.3.tar.gz
+Download-URL: https://github.com/rjdbcm/OZI/archive/refs/tags/1.5.0.tar.gz
 Home-page: https://oziproject.dev/
-Author: Eden Rose Duff MSc
+Author: Eden Ross Duff MSc
 Author-email: help@oziproject.dev
 License: Apache-2.0 WITH LLVM-exception
 Keywords: meson,packaging,wheel
 Project-URL: Bug Tracker, https://github.com/rjdbcm/ozi/issues
 Project-URL: Community, https://github.com/orgs/OZI-Project/discussions
-Requires-Dist: blastpipe==2024.4.3
+Requires-Dist: blastpipe==2024.5.0
 Requires-Dist: GitPython>=3
 Requires-Dist: dnspython
 Requires-Dist: idna>=2
 Requires-Dist: jinja2>=3
 Requires-Dist: meson>=1.1.0
 Requires-Dist: pyparsing~=3.1
 Requires-Dist: requests
```

### Comparing `OZI-1.4.3/README.rst` & `OZI-1.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `OZI-1.4.3/meson.build` & `OZI-1.5.0/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.4.3/meson.options` & `OZI-1.5.0/meson.options`

 * *Files identical despite different names*

### Comparing `OZI-1.4.3/ozi/__main__.py` & `OZI-1.5.0/ozi/__main__.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.3/ozi/actions.py` & `OZI-1.5.0/ozi/actions.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.3/ozi/comment.py` & `OZI-1.5.0/ozi/comment.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.3/ozi/fix/__main__.py` & `OZI-1.5.0/ozi/fix/__main__.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.3/ozi/fix/build_definition.py` & `OZI-1.5.0/ozi/fix/build_definition.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.3/ozi/fix/meson.build` & `OZI-1.5.0/ozi/fix/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.4.3/ozi/fix/missing.py` & `OZI-1.5.0/ozi/fix/missing.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.3/ozi/fix/parser.py` & `OZI-1.5.0/ozi/fix/parser.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.3/ozi/fix/rewrite_command.py` & `OZI-1.5.0/ozi/fix/rewrite_command.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from pathlib import Path
 from typing import TYPE_CHECKING
 from typing import Annotated
 from typing import Union
 from warnings import warn
 
 from ozi.render import build_child
+from ozi.render import build_file
 from ozi.render import find_user_template
 
 if TYPE_CHECKING:
     import sys
     from collections.abc import Callable
     from collections.abc import Mapping
 
@@ -110,62 +111,70 @@
             'root': self.env.get_template(METADATA.spec.python.src.template.add_root),
             'source': self.env.get_template(METADATA.spec.python.src.template.add_source),
             'test': self.env.get_template(METADATA.spec.python.src.template.add_root),
         }
 
     def _add_dunder_init(self: Self, filename: str) -> None:
         """Render a :file:`{filename}/__init__.py`."""
-        with open(
-            (
-                self.path_map.get(self.fix, partial(Path))(
-                    *filename.rstrip('/').split('/'),
-                )
-                / '__init__.py'
+        build_file(
+            self.env,
+            self.fix,
+            self.path_map.get(self.fix, partial(Path))(
+                *filename.rstrip('/').split('/'),
+            )
+            / '__init__.py',
+            find_user_template(
+                self.target,
+                filename,
+                self.fix,
             ),
-            'x',
-        ) as f:
-            f.write(
-                self.env.get_template('project.name/__init__.py.j2').render(
-                    user_template=find_user_template(
-                        self.target,
-                        filename,
-                        self.fix,
-                    ),
-                ),
+        )
+
+    def _add_files(
+        self: Self,
+        child: Path,
+        filename: str,
+        cmd_files: RewriteCommand,
+    ) -> RewriteCommand:
+        """add files to a project if they do not exist."""
+        if child.exists():  # pragma: no cover
+            pass
+        else:
+            build_file(
+                self.env,
+                self.fix,
+                child,
+                user_template=find_user_template(self.target, filename, self.fix),
             )
+        if filename.endswith('.pyx'):  # pragma: no cover
+            cmd_files.add('ext', 'files', str(Path(filename)))
+        else:
+            cmd_files.add(self.fix, 'files', str(Path(filename)))
+        return cmd_files
 
     def _add(
         self: Rewriter,
         child: Path,
         filename: str,
         cmd_files_children: tuple[RewriteCommand, RewriteCommand],
     ) -> tuple[RewriteCommand, RewriteCommand]:
         """Add items to OZI Rewriter"""
         cmd_files, cmd_children = cmd_files_children
         if self.fix not in ['source', 'test', 'root']:
             warn('Invalid fix mode nothing will be added.', RuntimeWarning, stacklevel=0)
         elif filename.endswith('/'):
-            build_child(self.env, filename, child)
-            if self.fix == 'source':
-                self._add_dunder_init(filename)
+            if child.exists():  # pragma: no cover
+                pass
+            else:
+                build_child(self.env, filename, child)
+                if self.fix == 'source':
+                    self._add_dunder_init(filename)
             cmd_children.add(self.fix, 'children', filename.rstrip('/'))
-        elif filename.endswith('.py'):
-            child.write_text(
-                self.base_templates.get(
-                    self.fix,
-                    self.base_templates.setdefault(
-                        self.fix,
-                        self.env.get_template('project.name/new_module.py.j2'),
-                    ),
-                ).render(user_template=find_user_template(self.target, filename, self.fix)),
-            )
-            cmd_files.add(self.fix, 'files', str(Path(filename)))
         else:
-            child.touch()
-            cmd_files.add(self.fix, 'files', str(Path(filename)))
+            cmd_files = self._add_files(child, filename, cmd_files)
         return cmd_files, cmd_children
 
     def __iadd__(self: Self, other: list[str]) -> Self:
         """Add a list of paths"""
         cmd_files = RewriteCommand()
         cmd_children = RewriteCommand()
 
@@ -186,16 +195,14 @@
         filename: str,
         cmd_files_children: tuple[RewriteCommand, RewriteCommand],
     ) -> tuple[RewriteCommand, RewriteCommand]:
         """Remove items from OZI Rewriter"""
         cmd_files, cmd_children = cmd_files_children
         if filename.endswith('/'):
             cmd_children.rem(self.fix, 'children', str(child / 'meson.build'))
-        elif filename.endswith('.py'):
-            cmd_files.rem(self.fix, 'files', str(Path(filename)))
         else:
             cmd_files.rem(self.fix, 'files', str(Path(filename)))
         return cmd_files, cmd_children
 
     def __isub__(self: Self, other: list[str]) -> Self:
         """Remove a list of paths"""
         cmd_files = RewriteCommand()
```

### Comparing `OZI-1.4.3/ozi/lint/meson.build` & `OZI-1.5.0/ozi/lint/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.4.3/ozi/lint/pyright/meson.build` & `OZI-1.5.0/ozi/lint/pyright/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.4.3/ozi/meson.build` & `OZI-1.5.0/ozi/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.4.3/ozi/meson.py` & `OZI-1.5.0/ozi/meson.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.3/ozi/new/__main__.py` & `OZI-1.5.0/ozi/new/__main__.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.3/ozi/new/meson.build` & `OZI-1.5.0/ozi/new/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.4.3/ozi/new/parser.py` & `OZI-1.5.0/ozi/new/parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 # ozi/new/parser.py
 # Part of the OZI Project, under the Apache License v2.0 with LLVM Exceptions.
 # See LICENSE.txt for license information.
 # SPDX-License-Identifier: Apache-2.0 WITH LLVM-exception
-"""``ozi-new`` argparse argument parser."""
+"""``ozi-new`` argparse argument parser.
+
+    .. versionchanged:: 1.5
+       Added `--[no-]enable-cython` argument. Default: `--no-enable-cython`
+
+"""
 from __future__ import annotations
 
 import argparse
 import sys
 
 from ozi.actions import CloseMatch
 from ozi.spec import METADATA
@@ -221,14 +226,20 @@
 ozi_defaults.add_argument(
     '--verify-email',
     default=False,
     action=argparse.BooleanOptionalAction,
     help='verify email domain deliverability(default: --no-verify-email)',
 )
 ozi_defaults.add_argument(
+    '--enable-cython',
+    default=False,
+    action=argparse.BooleanOptionalAction,
+    help='build extension module with Cython(default: --no-enable-cython)',
+)
+ozi_defaults.add_argument(
     '--strict',
     default=False,
     action=argparse.BooleanOptionalAction,
     help='strict mode raises warnings to errors(default: --strict)',
 )
 ozi_defaults.add_argument(
     '--allow-file',
```

### Comparing `OZI-1.4.3/ozi/new/validate.py` & `OZI-1.5.0/ozi/new/validate.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.3/ozi/pkg_extra.py` & `OZI-1.5.0/ozi/pkg_extra.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.3/ozi/render.py` & `OZI-1.5.0/ozi/render.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 # SPDX-License-Identifier: Apache-2.0 WITH LLVM-exception
 """Rendering utilities for the OZI project templates.
 """
 from __future__ import annotations
 
 from pathlib import Path
 from typing import TYPE_CHECKING
+from typing import AnyStr
+from typing import Literal
 from warnings import warn
 
 from blastpipe.ozi_templates.filter import underscorify  # pyright: ignore
 from git import InvalidGitRepositoryError
 from git import Repo
 
 if TYPE_CHECKING:
@@ -39,14 +41,75 @@
             user_template = template.read()
     else:
         TAP.diagnostic('User tempate not found', str(fp))
         user_template = None
     return user_template
 
 
+def map_to_template(
+    fix: Literal['source', 'root', 'test'] | AnyStr,
+    filename: str,
+) -> str:
+    """Map an appropriate template for an ozi-fix mode and filename.
+
+    .. versionadded:: 1.5
+
+    :param fix: ozi-fix mode setting
+    :type fix: Literal[&#39;source&#39;, &#39;root&#39;, &#39;test&#39;] | AnyStr
+    :param filename: name with file extension
+    :type filename: str
+    :return: template path
+    :rtype: str
+    """
+    match fix, filename:
+        case ['test' | 'root', f] if f.endswith('.py'):
+            x = 'tests/new_test.py.j2'
+        case ['source', f] if f.endswith('.py'):
+            x = 'project.name/new_module.py.j2'
+        case ['source', f] if f.endswith('.pyx'):  # pragma: no cover
+            x = 'project.name/new_ext.pyx.j2'
+        case ['root', f]:
+            x = f'{f}.j2'
+        case ['source', f]:
+            x = f'project.name/{f}.j2'
+        case ['test', f]:
+            x = f'tests/{f}.j2'
+        case [_, _]:  # pragma: no cover
+            x = ''
+    return x
+
+
+def build_file(
+    env: Environment,
+    fix: Literal['source', 'root', 'test'] | AnyStr,
+    path: Path,
+    user_template: str | None,
+) -> None:
+    """Render project file based on OZI templates.
+
+    .. versionadded:: 1.5
+
+    :param env: rendering environment
+    :type env: Environment
+    :param fix: ozi-fix setting
+    :type fix: Literal[&#39;source&#39;, &#39;root&#39;, &#39;test&#39;] | AnyStr
+    :param path: full path of file to be rendered
+    :type path: Path
+    :param user_template: path to a user template to extend
+    :type user_template: str | None
+    """
+    try:
+        template = env.get_template(map_to_template(fix, path.name)).render(
+            user_template=user_template,
+        )
+        path.write_text(template)
+    except LookupError as e:
+        warn(str(e), RuntimeWarning)
+
+
 def build_child(env: Environment, parent: str, child: Path) -> None:
     """Add a child directory to a parent in an existing OZI-style project.
 
     :param env: the OZI project file rendering environment
     :type env: jinja2.Environment
     :param parent: existing directory name in project
     :type parent: str
@@ -115,20 +178,26 @@
         except LookupError:  # pragma: defer to good-first-issue
             content = f'template "{filename}" failed to render.'
             warn(content, RuntimeWarning, stacklevel=0)
         with open(target / filename, 'w') as f:
             f.write(content)
 
     for filename in templates.source:
-        template = env.get_template(f'{filename}.j2')
         filename = filename.replace('project.name', underscorify(name).lower())
-        with open(target / filename, 'w') as f:
-            f.write(template.render())
+        build_file(
+            env,
+            'source',
+            target / filename,
+            find_user_template(str(target), filename, 'source'),
+        )
 
     for filename in templates.test:
-        template = env.get_template(f'{filename}.j2')
-        with open(target / filename, 'w') as f:
-            f.write(template.render())
+        build_file(
+            env,
+            'test',
+            target / filename,
+            find_user_template(str(target), filename, 'test'),
+        )
 
     template = env.get_template('project.ozi.wrap.j2')
     with open(target / 'subprojects' / 'ozi.wrap', 'w') as f:
         f.write(template.render())
```

### Comparing `OZI-1.4.3/ozi/scripts/core_metadata_template.py` & `OZI-1.5.0/ozi/scripts/core_metadata_template.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.3/ozi/scripts/meson.build` & `OZI-1.5.0/ozi/scripts/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.4.3/ozi/scripts/meson_dist_setuptools_scm.py` & `OZI-1.5.0/ozi/scripts/meson_dist_setuptools_scm.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.3/ozi/scripts/meson_setuptools_scm.py` & `OZI-1.5.0/ozi/scripts/meson_setuptools_scm.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.3/ozi/scripts/render_requirements.py` & `OZI-1.5.0/ozi/scripts/render_requirements.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.3/ozi/scripts/replace_ruff_target_version.py` & `OZI-1.5.0/ozi/scripts/replace_ruff_target_version.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.3/ozi/scripts/scm_version_snip.py` & `OZI-1.5.0/ozi/scripts/scm_version_snip.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.3/ozi/scripts/to_distribution_template.py` & `OZI-1.5.0/ozi/scripts/to_distribution_template.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.3/ozi/scripts/version_metadata_template.py` & `OZI-1.5.0/ozi/scripts/version_metadata_template.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.3/ozi/spdx.py` & `OZI-1.5.0/ozi/spdx.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.3/ozi/spec/_license.py` & `OZI-1.5.0/ozi/spec/_license.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.3/ozi/spec/_spec.py` & `OZI-1.5.0/ozi/spec/_spec.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.3/ozi/spec/base.py` & `OZI-1.5.0/ozi/spec/base.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.3/ozi/spec/ci.py` & `OZI-1.5.0/ozi/spec/ci.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.3/ozi/spec/meson.build` & `OZI-1.5.0/ozi/spec/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.4.3/ozi/spec/pkg.py` & `OZI-1.5.0/ozi/spec/pkg.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.3/ozi/spec/project.py` & `OZI-1.5.0/ozi/spec/project.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.3/ozi/spec/python.py` & `OZI-1.5.0/ozi/spec/python.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.3/ozi/spec/src.py` & `OZI-1.5.0/ozi/spec/src.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.3/ozi/tap.py` & `OZI-1.5.0/ozi/tap.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.3/ozi/trove.py` & `OZI-1.5.0/ozi/trove.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.3/ozi/vendor/email_validator/__init__.py` & `OZI-1.5.0/ozi/vendor/email_validator/__init__.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.3/ozi/vendor/email_validator/__main__.py` & `OZI-1.5.0/ozi/vendor/email_validator/__main__.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.3/ozi/vendor/email_validator/deliverability.py` & `OZI-1.5.0/ozi/vendor/email_validator/deliverability.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.3/ozi/vendor/email_validator/exceptions_types.py` & `OZI-1.5.0/ozi/vendor/email_validator/exceptions_types.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.3/ozi/vendor/email_validator/meson.build` & `OZI-1.5.0/ozi/vendor/email_validator/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.4.3/ozi/vendor/email_validator/rfc_constants.py` & `OZI-1.5.0/ozi/vendor/email_validator/rfc_constants.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.3/ozi/vendor/email_validator/syntax.py` & `OZI-1.5.0/ozi/vendor/email_validator/syntax.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.3/ozi/vendor/email_validator/validate_email.py` & `OZI-1.5.0/ozi/vendor/email_validator/validate_email.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.3/ozi/vendor/meson.build` & `OZI-1.5.0/ozi/vendor/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.4.3/pyproject.toml` & `OZI-1.5.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 version_file_template = """
 Metadata-Version: 2.1
 Name: @PROJECT_NAME@
 Version: @SCM_VERSION@
 Summary: Packager for Python projects using Meson.
 Download-URL: https://github.com/rjdbcm/OZI/archive/refs/tags/@SCM_VERSION@.tar.gz
 Home-page: https://oziproject.dev/
-Author: Eden Rose Duff MSc
+Author: Eden Ross Duff MSc
 Author-email: help@oziproject.dev
 License: @LICENSE@
 Keywords: meson,packaging,wheel
 Project-URL: Bug Tracker, https://github.com/rjdbcm/ozi/issues
 Project-URL: Community, https://github.com/orgs/OZI-Project/discussions
 @REQUIREMENTS_IN@
 Requires-External: git
@@ -149,41 +149,42 @@
 line-length = 93
 extend-exclude = ["meson-private", "scripts", "vendor"]
 # target-version = "@PYTHON_VERSION_DIST@"
 
 [tool.ruff.lint]
 ignore = [
     "A003",
-    "ARG",
     "ANN401",
-    "TRY003",
+    "ARG",
     "B028",
     "B905",
     "D1",
-    "D2",
     "D101",
+    "D2",
     "D4",
-    "FLY",
+    "EM",
     "FBT",
+    "FLY",
+    "PERF203",
     "PGH003",
     "PLR",
-    "PT001",
-    "RET",
-    "EM",
     "PLW",
+    "PT001",
     "PTH",
+    "RET",
     "RUF009",
     "RUF012",
     "RUF015",
+    "RUF200",
     "SIM",
     "T201",
     "TCH002",
     "TCH004",
+    "TRY003",
     "UP",
-    "PERF203",
 ]
 select = ["ALL"]
 
 [tool.ruff.lint.mccabe]
 max-complexity = 6
 
 [tool.ruff.format]
@@ -306,14 +307,19 @@
 prerelease = false
 
 [tool.semantic_release.branches."release/1.4"]
 match = "release/1.4"
 prerelease_token = "alpha"
 prerelease = false
 
+[tool.semantic_release.branches."release/1.5"]
+match = "release/1.5"
+prerelease_token = "alpha"
+prerelease = false
+
 [tool.semantic_release.commit_parser_options]
 major_tags = [":boom:"]
 minor_tags = [
     ":sparkles:",
 ]
 patch_tags = [
     ":adhesive_bandage:",
```

### Comparing `OZI-1.4.3/templates/CHANGELOG.md.j2` & `OZI-1.5.0/templates/CHANGELOG.md.j2`

 * *Files identical despite different names*

### Comparing `OZI-1.4.3/tests/meson.build` & `OZI-1.5.0/tests/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.4.3/tests/test_ozi_fix.py` & `OZI-1.5.0/tests/test_ozi_fix.py`

 * *Files 2% similar despite different names*

```diff
@@ -314,15 +314,15 @@
     )
     rewriter += ['foo.py']
     assert len(rewriter.commands) == 1
 
 
 @pytest.mark.parametrize('fix', ['test', 'root', 'source'])
 def test_Rewriter_bad_project__iadd__file_from_template(  # noqa: N802, DC102, RUF100
-    bad_project: pytest.FixtureRequest,
+    bad_project: pytest.FixtureRequest | pathlib.Path,
     fix: str,
 ) -> None:
     rewriter = ozi.fix.rewrite_command.Rewriter(
         target=str(bad_project),
         name='ozi_phony',
         fix=fix,
         env=env,
@@ -344,15 +344,16 @@
 ) -> None:
     rewriter = ozi.fix.rewrite_command.Rewriter(
         target=str(bad_project),
         name='ozi_phony',
         fix=fix,
         env=env,
     )
-    rewriter += ['foo']
+    with pytest.warns(RuntimeWarning):
+        rewriter += ['foo']
     assert len(rewriter.commands) == 1
 
 
 header = """.. OZI
   Classifier: License-Expression :: Apache-2.0 WITH LLVM-exception
   Classifier: License-File :: LICENSE.txt
 """
```

### Comparing `OZI-1.4.3/tests/test_ozi_new.py` & `OZI-1.5.0/tests/test_ozi_new.py`

 * *Files identical despite different names*

### Comparing `OZI-1.4.3/tests/test_tap.py` & `OZI-1.5.0/tests/test_tap.py`

 * *Files identical despite different names*

