# Comparing `tmp/alluka-0.1.5.tar.gz` & `tmp/alluka-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alluka-0.1.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "alluka-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `alluka-0.1.5.tar` & `alluka-0.2.0.tar`

### file list

```diff
@@ -1,133 +1,140 @@
--rw-r--r--   0        0        0      320 2024-04-22 22:53:50.525395 alluka-0.1.5/.codeclimate.yml
--rw-r--r--   0        0        0       14 2024-04-22 22:53:50.525395 alluka-0.1.5/.gitattributes
--rw-r--r--   0        0        0       26 2024-04-22 22:53:50.525395 alluka-0.1.5/.github/CODEOWNERS
--rw-r--r--   0        0        0       45 2024-04-22 22:53:50.525395 alluka-0.1.5/.github/FUNDING.yml
--rw-r--r--   0        0        0      459 2024-04-22 22:53:50.525395 alluka-0.1.5/.github/dependabot.yml
--rw-r--r--   0        0        0      524 2024-04-22 22:53:50.525395 alluka-0.1.5/.github/pull_request_template.md
--rw-r--r--   0        0        0     1144 2024-04-22 22:53:50.525395 alluka-0.1.5/.github/workflows/freeze-for-pr.yml
--rw-r--r--   0        0        0     1034 2024-04-22 22:53:50.525395 alluka-0.1.5/.github/workflows/lint.yml
--rw-r--r--   0        0        0     1516 2024-04-22 22:53:50.525395 alluka-0.1.5/.github/workflows/pr-docs.yml
--rw-r--r--   0        0        0     1002 2024-04-22 22:53:50.525395 alluka-0.1.5/.github/workflows/publish.yml
--rw-r--r--   0        0        0     2343 2024-04-22 22:53:50.525395 alluka-0.1.5/.github/workflows/py-test.yml
--rw-r--r--   0        0        0      980 2024-04-22 22:53:50.525395 alluka-0.1.5/.github/workflows/reformat.yml
--rw-r--r--   0        0        0     1263 2024-04-22 22:53:50.525395 alluka-0.1.5/.github/workflows/release-docs.yml
--rw-r--r--   0        0        0     1039 2024-04-22 22:53:50.525395 alluka-0.1.5/.github/workflows/resync-piped.yml
--rw-r--r--   0        0        0      836 2024-04-22 22:53:50.525395 alluka-0.1.5/.github/workflows/type-check.yml
--rw-r--r--   0        0        0     1186 2024-04-22 22:53:50.525395 alluka-0.1.5/.github/workflows/update-licence.yml
--rw-r--r--   0        0        0     1221 2024-04-22 22:53:50.525395 alluka-0.1.5/.github/workflows/upgrade-locks.yml
--rw-r--r--   0        0        0     1060 2024-04-22 22:53:50.525395 alluka-0.1.5/.github/workflows/verify-locks.yml
--rw-r--r--   0        0        0      854 2024-04-22 22:53:50.525395 alluka-0.1.5/.github/workflows/verify-types.yml
--rw-r--r--   0        0        0     1748 2024-04-22 22:53:50.525395 alluka-0.1.5/.gitignore
--rw-r--r--   0        0        0       85 2024-04-22 22:53:50.525395 alluka-0.1.5/.gitmodules
--rw-r--r--   0        0        0     3409 2024-04-22 22:53:50.525395 alluka-0.1.5/CHANGELOG.md
--rw-r--r--   0        0        0     5220 2024-04-22 22:53:50.525395 alluka-0.1.5/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     6399 2024-04-22 22:53:50.525395 alluka-0.1.5/CONTRIBUTING.md
--rw-r--r--   0        0        0     1520 2024-04-22 22:53:50.525395 alluka-0.1.5/LICENSE
--rw-r--r--   0        0        0      607 2024-04-22 22:53:50.525395 alluka-0.1.5/README.md
--rw-r--r--   0        0        0     2376 2024-04-22 22:53:50.525395 alluka-0.1.5/alluka/__init__.py
--rw-r--r--   0        0        0    14896 2024-04-22 22:53:50.525395 alluka-0.1.5/alluka/_client.py
--rw-r--r--   0        0        0     2531 2024-04-22 22:53:50.525395 alluka-0.1.5/alluka/_errors.py
--rw-r--r--   0        0        0     6261 2024-04-22 22:53:50.525395 alluka-0.1.5/alluka/_self_injecting.py
--rw-r--r--   0        0        0     9605 2024-04-22 22:53:50.525395 alluka-0.1.5/alluka/_types.py
--rw-r--r--   0        0        0      167 2024-04-22 22:53:50.525395 alluka-0.1.5/alluka/_vendor/__init__.py
--rw-r--r--   0        0        0   123930 2024-04-22 22:53:50.529395 alluka-0.1.5/alluka/_vendor/inspect.py
--rw-r--r--   0        0        0    13931 2024-04-22 22:53:50.529395 alluka-0.1.5/alluka/_vendor/inspect.py.LICENSE
--rw-r--r--   0        0        0    12305 2024-04-22 22:53:50.529395 alluka-0.1.5/alluka/_vendor/inspect.pyi
--rw-r--r--   0        0        0    12657 2024-04-22 22:53:50.529395 alluka-0.1.5/alluka/_vendor/inspect.pyi.LICENSE
--rw-r--r--   0        0        0     9336 2024-04-22 22:53:50.529395 alluka-0.1.5/alluka/_visitor.py
--rw-r--r--   0        0        0    20961 2024-04-22 22:53:50.529395 alluka-0.1.5/alluka/abc.py
--rw-r--r--   0        0        0        0 2024-04-22 22:53:50.529395 alluka-0.1.5/alluka/py.typed
--rw-r--r--   0        0        0       56 2024-04-22 22:53:50.529395 alluka-0.1.5/dev-requirements/flake8.txt
--rw-r--r--   0        0        0      251 2024-04-22 22:53:50.529395 alluka-0.1.5/dev-requirements/tests.in
--rw-r--r--   0        0        0    15059 2024-04-22 22:53:50.529395 alluka-0.1.5/dev-requirements/tests.txt
--rw-r--r--   0        0        0      112 2024-04-22 22:53:50.529395 alluka-0.1.5/dev-requirements/type-checking.in
--rw-r--r--   0        0        0    32893 2024-04-22 22:53:50.529395 alluka-0.1.5/dev-requirements/type-checking.txt
--rw-r--r--   0        0        0       17 2024-04-22 22:53:50.529395 alluka-0.1.5/docs/changelog.md
--rw-r--r--   0        0        0       14 2024-04-22 22:53:50.529395 alluka-0.1.5/docs/index.md
--rw-r--r--   0        0        0       29 2024-04-22 22:53:50.529395 alluka-0.1.5/docs/reference/abc.md
--rw-r--r--   0        0        0       21 2024-04-22 22:53:50.529395 alluka-0.1.5/docs/reference/index.md
--rw-r--r--   0        0        0     5220 2024-04-22 22:53:50.529395 alluka-0.1.5/docs/usage.md
--rw-r--r--   0        0        0     1593 2024-04-22 22:53:50.529395 alluka-0.1.5/mkdocs.yml
--rw-r--r--   0        0        0     1714 2024-04-22 22:53:50.529395 alluka-0.1.5/noxfile.py
--rw-r--r--   0        0        0       50 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/.env.example
--rw-r--r--   0        0        0       14 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/.gitattributes
--rw-r--r--   0        0        0      454 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/.github/dependabot.yml
--rw-r--r--   0        0        0     3675 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/.github/workflows/docker-publish.yml
--rw-r--r--   0        0        0     1240 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/.github/workflows/freeze-for-pr.yml
--rw-r--r--   0        0        0      959 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/.github/workflows/lint.yml
--rw-r--r--   0        0        0      976 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/.github/workflows/reformat.yml
--rw-r--r--   0        0        0     1032 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/.github/workflows/resync-piped.yml
--rw-r--r--   0        0        0      832 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/.github/workflows/type-check.yml
--rw-r--r--   0        0        0     1182 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/.github/workflows/update-licence.yml
--rw-r--r--   0        0        0     1217 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/.github/workflows/upgrade-locks.yml
--rw-r--r--   0        0        0     1114 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/.github/workflows/verify-locks.yml
--rw-r--r--   0        0        0     1751 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/.gitignore
--rw-r--r--   0        0        0      404 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/Dockerfile
--rw-r--r--   0        0        0     1520 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/LICENSE
--rw-r--r--   0        0        0      138 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/README.md
--rw-r--r--   0        0        0    31151 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/bot/main.py
--rw-r--r--   0        0        0       10 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/bot/requirements-extra.txt
--rw-r--r--   0        0        0      123 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/bot/requirements.in
--rw-r--r--   0        0        0    23268 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/bot/requirements.txt
--rw-r--r--   0        0        0      933 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/dev-requirements/flake8.in
--rw-r--r--   0        0        0    20501 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/dev-requirements/flake8.txt
--rw-r--r--   0        0        0       10 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/dev-requirements/type-checking-extra.txt
--rw-r--r--   0        0        0      112 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/dev-requirements/type-checking.in
--rw-r--r--   0        0        0    33981 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/dev-requirements/type-checking.txt
--rw-r--r--   0        0        0      240 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/docker-compose.yml
--rw-r--r--   0        0        0       26 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/github/CODEOWNERS
--rw-r--r--   0        0        0       45 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/github/FUNDING.yml
--rw-r--r--   0        0        0      764 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/github/actions/clippy.yml
--rw-r--r--   0        0        0     3953 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/github/actions/docker-publish.yml
--rw-r--r--   0        0        0     1133 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/github/actions/freeze-for-pr.yml
--rw-r--r--   0        0        0     1271 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/github/actions/lint.yml
--rw-r--r--   0        0        0     1577 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/github/actions/pr-docs.yml
--rw-r--r--   0        0        0     1073 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/github/actions/publish.yml
--rw-r--r--   0        0        0     2399 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/github/actions/py-test.yml
--rw-r--r--   0        0        0     1013 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/github/actions/reformat.yml
--rw-r--r--   0        0        0     1373 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/github/actions/release-docs.yml
--rw-r--r--   0        0        0     1075 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/github/actions/resync-piped.yml
--rw-r--r--   0        0        0     1223 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/github/actions/rustfmt.yml
--rw-r--r--   0        0        0      869 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/github/actions/type-check.yml
--rw-r--r--   0        0        0     1191 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/github/actions/update-licence.yml
--rw-r--r--   0        0        0     1226 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/github/actions/upgrade-locks.yml
--rw-r--r--   0        0        0     1130 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/github/actions/verify-locks.yml
--rw-r--r--   0        0        0      887 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/github/actions/verify-types.yml
--rw-r--r--   0        0        0      550 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/github/dependabot.yml
--rw-r--r--   0        0        0      524 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/github/pull_request_template.md
--rw-r--r--   0        0        0     1713 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/noxfile.py
--rw-r--r--   0        0        0     4896 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/pyproject.toml
--rw-r--r--   0        0        0      115 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/python/base-requirements/docs.in
--rw-r--r--   0        0        0    36417 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/python/base-requirements/docs.txt
--rw-r--r--   0        0        0       31 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/python/base-requirements/flake8.in
--rw-r--r--   0        0        0     1580 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/python/base-requirements/flake8.txt
--rw-r--r--   0        0        0       32 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/python/base-requirements/freeze-locks.in
--rw-r--r--   0        0        0    48844 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/python/base-requirements/freeze-locks.txt
--rw-r--r--   0        0        0     1068 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/python/base-requirements/library-flake8.in
--rw-r--r--   0        0        0    33521 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/python/base-requirements/library-flake8.txt
--rw-r--r--   0        0        0       58 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/python/base-requirements/lint.in
--rw-r--r--   0        0        0     6314 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/python/base-requirements/lint.txt
--rw-r--r--   0        0        0       60 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/python/base-requirements/nox.in
--rw-r--r--   0        0        0    15576 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/python/base-requirements/nox.txt
--rw-r--r--   0        0        0       12 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/python/base-requirements/publish.in
--rw-r--r--   0        0        0     9861 2024-04-22 22:53:51.205402 alluka-0.1.5/piped/python/base-requirements/publish.txt
--rw-r--r--   0        0        0       78 2024-04-22 22:53:51.205402 alluka-0.1.5/piped/python/base-requirements/reformat.in
--rw-r--r--   0        0        0    18195 2024-04-22 22:53:51.205402 alluka-0.1.5/piped/python/base-requirements/reformat.txt
--rw-r--r--   0        0        0       64 2024-04-22 22:53:51.205402 alluka-0.1.5/piped/python/base-requirements/tests.in
--rw-r--r--   0        0        0     7400 2024-04-22 22:53:51.205402 alluka-0.1.5/piped/python/base-requirements/tests.txt
--rw-r--r--   0        0        0       29 2024-04-22 22:53:51.205402 alluka-0.1.5/piped/python/base-requirements/type-checking.in
--rw-r--r--   0        0        0     4051 2024-04-22 22:53:51.205402 alluka-0.1.5/piped/python/base-requirements/type-checking.txt
--rw-r--r--   0        0        0    24295 2024-04-22 22:53:51.205402 alluka-0.1.5/piped/python/noxfile.py
--rw-r--r--   0        0        0     1714 2024-04-22 22:53:51.205402 alluka-0.1.5/piped/python/noxfile.template.py
--rw-r--r--   0        0        0     4527 2024-04-22 22:53:51.205402 alluka-0.1.5/piped/python/piped_shared/__init__.py
--rw-r--r--   0        0        0        0 2024-04-22 22:53:51.205402 alluka-0.1.5/piped/python/piped_shared/py.typed
--rw-r--r--   0        0        0      334 2024-04-22 22:53:51.205402 alluka-0.1.5/piped/python/pyproject.toml
--rw-r--r--   0        0        0     6898 2024-04-22 22:53:50.529395 alluka-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1596 2024-04-22 22:53:50.529395 alluka-0.1.5/tests/__init__.py
--rw-r--r--   0        0        0    13421 2024-04-22 22:53:50.529395 alluka-0.1.5/tests/test__client.py
--rw-r--r--   0        0        0     2881 2024-04-22 22:53:50.529395 alluka-0.1.5/tests/test__self_injecting.py
--rw-r--r--   0        0        0    50719 2024-04-22 22:53:50.529395 alluka-0.1.5/tests/test_async_callback_di.py
--rw-r--r--   0        0        0    52004 2024-04-22 22:53:50.529395 alluka-0.1.5/tests/test_async_callback_di_future_annotations.py
--rw-r--r--   0        0        0    45828 2024-04-22 22:53:50.529395 alluka-0.1.5/tests/test_callback_di.py
--rw-r--r--   0        0        0    46212 2024-04-22 22:53:50.529395 alluka-0.1.5/tests/test_callback_di_future_annotations.py
--rw-r--r--   0        0        0     1912 1970-01-01 00:00:00.000000 alluka-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      320 2024-04-29 21:16:31.303313 alluka-0.2.0/.codeclimate.yml
+-rw-r--r--   0        0        0       14 2024-04-29 21:16:31.303313 alluka-0.2.0/.gitattributes
+-rw-r--r--   0        0        0       26 2024-04-29 21:16:31.303313 alluka-0.2.0/.github/CODEOWNERS
+-rw-r--r--   0        0        0       45 2024-04-29 21:16:31.303313 alluka-0.2.0/.github/FUNDING.yml
+-rw-r--r--   0        0        0      459 2024-04-29 21:16:31.303313 alluka-0.2.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      524 2024-04-29 21:16:31.303313 alluka-0.2.0/.github/pull_request_template.md
+-rw-r--r--   0        0        0     1144 2024-04-29 21:16:31.303313 alluka-0.2.0/.github/workflows/freeze-for-pr.yml
+-rw-r--r--   0        0        0     1034 2024-04-29 21:16:31.303313 alluka-0.2.0/.github/workflows/lint.yml
+-rw-r--r--   0        0        0     1516 2024-04-29 21:16:31.303313 alluka-0.2.0/.github/workflows/pr-docs.yml
+-rw-r--r--   0        0        0     1002 2024-04-29 21:16:31.303313 alluka-0.2.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     2343 2024-04-29 21:16:31.303313 alluka-0.2.0/.github/workflows/py-test.yml
+-rw-r--r--   0        0        0      980 2024-04-29 21:16:31.303313 alluka-0.2.0/.github/workflows/reformat.yml
+-rw-r--r--   0        0        0     1263 2024-04-29 21:16:31.303313 alluka-0.2.0/.github/workflows/release-docs.yml
+-rw-r--r--   0        0        0     1039 2024-04-29 21:16:31.303313 alluka-0.2.0/.github/workflows/resync-piped.yml
+-rw-r--r--   0        0        0      836 2024-04-29 21:16:31.303313 alluka-0.2.0/.github/workflows/type-check.yml
+-rw-r--r--   0        0        0     1186 2024-04-29 21:16:31.303313 alluka-0.2.0/.github/workflows/update-licence.yml
+-rw-r--r--   0        0        0     1221 2024-04-29 21:16:31.303313 alluka-0.2.0/.github/workflows/upgrade-locks.yml
+-rw-r--r--   0        0        0     1060 2024-04-29 21:16:31.303313 alluka-0.2.0/.github/workflows/verify-locks.yml
+-rw-r--r--   0        0        0      854 2024-04-29 21:16:31.303313 alluka-0.2.0/.github/workflows/verify-types.yml
+-rw-r--r--   0        0        0     1748 2024-04-29 21:16:31.303313 alluka-0.2.0/.gitignore
+-rw-r--r--   0        0        0       85 2024-04-29 21:16:31.303313 alluka-0.2.0/.gitmodules
+-rw-r--r--   0        0        0     5116 2024-04-29 21:16:31.303313 alluka-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0     5220 2024-04-29 21:16:31.303313 alluka-0.2.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     6399 2024-04-29 21:16:31.303313 alluka-0.2.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1520 2024-04-29 21:16:31.303313 alluka-0.2.0/LICENSE
+-rw-r--r--   0        0        0      607 2024-04-29 21:16:31.303313 alluka-0.2.0/README.md
+-rw-r--r--   0        0        0     2450 2024-04-29 21:16:31.303313 alluka-0.2.0/alluka/__init__.py
+-rw-r--r--   0        0        0    14212 2024-04-29 21:16:31.303313 alluka-0.2.0/alluka/_client.py
+-rw-r--r--   0        0        0     2531 2024-04-29 21:16:31.307313 alluka-0.2.0/alluka/_errors.py
+-rw-r--r--   0        0        0     5721 2024-04-29 21:16:31.307313 alluka-0.2.0/alluka/_self_injecting.py
+-rw-r--r--   0        0        0     9605 2024-04-29 21:16:31.307313 alluka-0.2.0/alluka/_types.py
+-rw-r--r--   0        0        0      167 2024-04-29 21:16:31.307313 alluka-0.2.0/alluka/_vendor/__init__.py
+-rw-r--r--   0        0        0   123930 2024-04-29 21:16:31.307313 alluka-0.2.0/alluka/_vendor/inspect.py
+-rw-r--r--   0        0        0    13931 2024-04-29 21:16:31.307313 alluka-0.2.0/alluka/_vendor/inspect.py.LICENSE
+-rw-r--r--   0        0        0    12305 2024-04-29 21:16:31.307313 alluka-0.2.0/alluka/_vendor/inspect.pyi
+-rw-r--r--   0        0        0    12657 2024-04-29 21:16:31.307313 alluka-0.2.0/alluka/_vendor/inspect.pyi.LICENSE
+-rw-r--r--   0        0        0     9336 2024-04-29 21:16:31.307313 alluka-0.2.0/alluka/_visitor.py
+-rw-r--r--   0        0        0    21842 2024-04-29 21:16:31.307313 alluka-0.2.0/alluka/abc.py
+-rw-r--r--   0        0        0     8688 2024-04-29 21:16:31.307313 alluka-0.2.0/alluka/local.py
+-rw-r--r--   0        0        0        0 2024-04-29 21:16:31.307313 alluka-0.2.0/alluka/py.typed
+-rw-r--r--   0        0        0       27 2024-04-29 21:16:31.307313 alluka-0.2.0/dev-requirements/constraints.in
+-rw-r--r--   0        0        0      484 2024-04-29 21:16:31.307313 alluka-0.2.0/dev-requirements/constraints.txt
+-rw-r--r--   0        0        0       56 2024-04-29 21:16:31.307313 alluka-0.2.0/dev-requirements/flake8.txt
+-rw-r--r--   0        0        0      251 2024-04-29 21:16:31.307313 alluka-0.2.0/dev-requirements/tests.in
+-rw-r--r--   0        0        0    15059 2024-04-29 21:16:31.307313 alluka-0.2.0/dev-requirements/tests.txt
+-rw-r--r--   0        0        0      112 2024-04-29 21:16:31.307313 alluka-0.2.0/dev-requirements/type-checking.in
+-rw-r--r--   0        0        0    32894 2024-04-29 21:16:31.307313 alluka-0.2.0/dev-requirements/type-checking.txt
+-rw-r--r--   0        0        0       17 2024-04-29 21:16:31.307313 alluka-0.2.0/docs/changelog.md
+-rw-r--r--   0        0        0       14 2024-04-29 21:16:31.307313 alluka-0.2.0/docs/index.md
+-rw-r--r--   0        0        0       29 2024-04-29 21:16:31.307313 alluka-0.2.0/docs/reference/abc.md
+-rw-r--r--   0        0        0       21 2024-04-29 21:16:31.307313 alluka-0.2.0/docs/reference/index.md
+-rw-r--r--   0        0        0       33 2024-04-29 21:16:31.307313 alluka-0.2.0/docs/reference/local.md
+-rw-r--r--   0        0        0     6929 2024-04-29 21:16:31.307313 alluka-0.2.0/docs/usage.md
+-rw-r--r--   0        0        0     4204 2024-04-29 21:16:31.307313 alluka-0.2.0/docs_src/usage.py
+-rw-r--r--   0        0        0     1714 2024-04-29 21:16:31.307313 alluka-0.2.0/mkdocs.yml
+-rw-r--r--   0        0        0     1714 2024-04-29 21:16:31.307313 alluka-0.2.0/noxfile.py
+-rw-r--r--   0        0        0       50 2024-04-29 21:16:31.735314 alluka-0.2.0/piped/.env.example
+-rw-r--r--   0        0        0       14 2024-04-29 21:16:31.735314 alluka-0.2.0/piped/.gitattributes
+-rw-r--r--   0        0        0      454 2024-04-29 21:16:31.735314 alluka-0.2.0/piped/.github/dependabot.yml
+-rw-r--r--   0        0        0     3675 2024-04-29 21:16:31.735314 alluka-0.2.0/piped/.github/workflows/docker-publish.yml
+-rw-r--r--   0        0        0     1240 2024-04-29 21:16:31.735314 alluka-0.2.0/piped/.github/workflows/freeze-for-pr.yml
+-rw-r--r--   0        0        0      959 2024-04-29 21:16:31.735314 alluka-0.2.0/piped/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      976 2024-04-29 21:16:31.735314 alluka-0.2.0/piped/.github/workflows/reformat.yml
+-rw-r--r--   0        0        0     1032 2024-04-29 21:16:31.735314 alluka-0.2.0/piped/.github/workflows/resync-piped.yml
+-rw-r--r--   0        0        0      832 2024-04-29 21:16:31.735314 alluka-0.2.0/piped/.github/workflows/type-check.yml
+-rw-r--r--   0        0        0     1182 2024-04-29 21:16:31.735314 alluka-0.2.0/piped/.github/workflows/update-licence.yml
+-rw-r--r--   0        0        0     1217 2024-04-29 21:16:31.735314 alluka-0.2.0/piped/.github/workflows/upgrade-locks.yml
+-rw-r--r--   0        0        0     1114 2024-04-29 21:16:31.735314 alluka-0.2.0/piped/.github/workflows/verify-locks.yml
+-rw-r--r--   0        0        0     1751 2024-04-29 21:16:31.735314 alluka-0.2.0/piped/.gitignore
+-rw-r--r--   0        0        0      404 2024-04-29 21:16:31.735314 alluka-0.2.0/piped/Dockerfile
+-rw-r--r--   0        0        0     1520 2024-04-29 21:16:31.735314 alluka-0.2.0/piped/LICENSE
+-rw-r--r--   0        0        0      138 2024-04-29 21:16:31.735314 alluka-0.2.0/piped/README.md
+-rw-r--r--   0        0        0    31151 2024-04-29 21:16:31.739313 alluka-0.2.0/piped/bot/main.py
+-rw-r--r--   0        0        0       10 2024-04-29 21:16:31.739313 alluka-0.2.0/piped/bot/requirements-extra.txt
+-rw-r--r--   0        0        0      123 2024-04-29 21:16:31.739313 alluka-0.2.0/piped/bot/requirements.in
+-rw-r--r--   0        0        0    23268 2024-04-29 21:16:31.739313 alluka-0.2.0/piped/bot/requirements.txt
+-rw-r--r--   0        0        0      933 2024-04-29 21:16:31.739313 alluka-0.2.0/piped/dev-requirements/flake8.in
+-rw-r--r--   0        0        0    20501 2024-04-29 21:16:31.739313 alluka-0.2.0/piped/dev-requirements/flake8.txt
+-rw-r--r--   0        0        0       10 2024-04-29 21:16:31.739313 alluka-0.2.0/piped/dev-requirements/type-checking-extra.txt
+-rw-r--r--   0        0        0      112 2024-04-29 21:16:31.739313 alluka-0.2.0/piped/dev-requirements/type-checking.in
+-rw-r--r--   0        0        0    33981 2024-04-29 21:16:31.739313 alluka-0.2.0/piped/dev-requirements/type-checking.txt
+-rw-r--r--   0        0        0      240 2024-04-29 21:16:31.739313 alluka-0.2.0/piped/docker-compose.yml
+-rw-r--r--   0        0        0       26 2024-04-29 21:16:31.739313 alluka-0.2.0/piped/github/CODEOWNERS
+-rw-r--r--   0        0        0       45 2024-04-29 21:16:31.739313 alluka-0.2.0/piped/github/FUNDING.yml
+-rw-r--r--   0        0        0      764 2024-04-29 21:16:31.739313 alluka-0.2.0/piped/github/actions/clippy.yml
+-rw-r--r--   0        0        0     3953 2024-04-29 21:16:31.739313 alluka-0.2.0/piped/github/actions/docker-publish.yml
+-rw-r--r--   0        0        0     1133 2024-04-29 21:16:31.739313 alluka-0.2.0/piped/github/actions/freeze-for-pr.yml
+-rw-r--r--   0        0        0     1271 2024-04-29 21:16:31.739313 alluka-0.2.0/piped/github/actions/lint.yml
+-rw-r--r--   0        0        0     1577 2024-04-29 21:16:31.739313 alluka-0.2.0/piped/github/actions/pr-docs.yml
+-rw-r--r--   0        0        0     1073 2024-04-29 21:16:31.739313 alluka-0.2.0/piped/github/actions/publish.yml
+-rw-r--r--   0        0        0     2399 2024-04-29 21:16:31.739313 alluka-0.2.0/piped/github/actions/py-test.yml
+-rw-r--r--   0        0        0     1013 2024-04-29 21:16:31.739313 alluka-0.2.0/piped/github/actions/reformat.yml
+-rw-r--r--   0        0        0     1373 2024-04-29 21:16:31.739313 alluka-0.2.0/piped/github/actions/release-docs.yml
+-rw-r--r--   0        0        0     1075 2024-04-29 21:16:31.739313 alluka-0.2.0/piped/github/actions/resync-piped.yml
+-rw-r--r--   0        0        0     1223 2024-04-29 21:16:31.739313 alluka-0.2.0/piped/github/actions/rustfmt.yml
+-rw-r--r--   0        0        0      869 2024-04-29 21:16:31.739313 alluka-0.2.0/piped/github/actions/type-check.yml
+-rw-r--r--   0        0        0     1191 2024-04-29 21:16:31.739313 alluka-0.2.0/piped/github/actions/update-licence.yml
+-rw-r--r--   0        0        0     1226 2024-04-29 21:16:31.739313 alluka-0.2.0/piped/github/actions/upgrade-locks.yml
+-rw-r--r--   0        0        0     1130 2024-04-29 21:16:31.739313 alluka-0.2.0/piped/github/actions/verify-locks.yml
+-rw-r--r--   0        0        0      887 2024-04-29 21:16:31.739313 alluka-0.2.0/piped/github/actions/verify-types.yml
+-rw-r--r--   0        0        0      550 2024-04-29 21:16:31.739313 alluka-0.2.0/piped/github/dependabot.yml
+-rw-r--r--   0        0        0      524 2024-04-29 21:16:31.739313 alluka-0.2.0/piped/github/pull_request_template.md
+-rw-r--r--   0        0        0     1713 2024-04-29 21:16:31.739313 alluka-0.2.0/piped/noxfile.py
+-rw-r--r--   0        0        0     4896 2024-04-29 21:16:31.739313 alluka-0.2.0/piped/pyproject.toml
+-rw-r--r--   0        0        0      115 2024-04-29 21:16:31.739313 alluka-0.2.0/piped/python/base-requirements/docs.in
+-rw-r--r--   0        0        0    36417 2024-04-29 21:16:31.739313 alluka-0.2.0/piped/python/base-requirements/docs.txt
+-rw-r--r--   0        0        0       31 2024-04-29 21:16:31.739313 alluka-0.2.0/piped/python/base-requirements/flake8.in
+-rw-r--r--   0        0        0     1580 2024-04-29 21:16:31.739313 alluka-0.2.0/piped/python/base-requirements/flake8.txt
+-rw-r--r--   0        0        0       32 2024-04-29 21:16:31.739313 alluka-0.2.0/piped/python/base-requirements/freeze-locks.in
+-rw-r--r--   0        0        0    48844 2024-04-29 21:16:31.739313 alluka-0.2.0/piped/python/base-requirements/freeze-locks.txt
+-rw-r--r--   0        0        0     1068 2024-04-29 21:16:31.739313 alluka-0.2.0/piped/python/base-requirements/library-flake8.in
+-rw-r--r--   0        0        0    33521 2024-04-29 21:16:31.739313 alluka-0.2.0/piped/python/base-requirements/library-flake8.txt
+-rw-r--r--   0        0        0       58 2024-04-29 21:16:31.739313 alluka-0.2.0/piped/python/base-requirements/lint.in
+-rw-r--r--   0        0        0     6314 2024-04-29 21:16:31.739313 alluka-0.2.0/piped/python/base-requirements/lint.txt
+-rw-r--r--   0        0        0       60 2024-04-29 21:16:31.739313 alluka-0.2.0/piped/python/base-requirements/nox.in
+-rw-r--r--   0        0        0    15576 2024-04-29 21:16:31.739313 alluka-0.2.0/piped/python/base-requirements/nox.txt
+-rw-r--r--   0        0        0       12 2024-04-29 21:16:31.739313 alluka-0.2.0/piped/python/base-requirements/publish.in
+-rw-r--r--   0        0        0     9861 2024-04-29 21:16:31.739313 alluka-0.2.0/piped/python/base-requirements/publish.txt
+-rw-r--r--   0        0        0       78 2024-04-29 21:16:31.739313 alluka-0.2.0/piped/python/base-requirements/reformat.in
+-rw-r--r--   0        0        0    18195 2024-04-29 21:16:31.739313 alluka-0.2.0/piped/python/base-requirements/reformat.txt
+-rw-r--r--   0        0        0       64 2024-04-29 21:16:31.739313 alluka-0.2.0/piped/python/base-requirements/tests.in
+-rw-r--r--   0        0        0     7400 2024-04-29 21:16:31.739313 alluka-0.2.0/piped/python/base-requirements/tests.txt
+-rw-r--r--   0        0        0       29 2024-04-29 21:16:31.739313 alluka-0.2.0/piped/python/base-requirements/type-checking.in
+-rw-r--r--   0        0        0     4051 2024-04-29 21:16:31.739313 alluka-0.2.0/piped/python/base-requirements/type-checking.txt
+-rw-r--r--   0        0        0    24295 2024-04-29 21:16:31.739313 alluka-0.2.0/piped/python/noxfile.py
+-rw-r--r--   0        0        0     1714 2024-04-29 21:16:31.739313 alluka-0.2.0/piped/python/noxfile.template.py
+-rw-r--r--   0        0        0     4527 2024-04-29 21:16:31.739313 alluka-0.2.0/piped/python/piped_shared/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 21:16:31.739313 alluka-0.2.0/piped/python/piped_shared/py.typed
+-rw-r--r--   0        0        0      334 2024-04-29 21:16:31.739313 alluka-0.2.0/piped/python/pyproject.toml
+-rw-r--r--   0        0        0     7123 2024-04-29 21:16:31.307313 alluka-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1596 2024-04-29 21:16:31.307313 alluka-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0    13589 2024-04-29 21:16:31.307313 alluka-0.2.0/tests/test__client.py
+-rw-r--r--   0        0        0     3122 2024-04-29 21:16:31.307313 alluka-0.2.0/tests/test__self_injecting.py
+-rw-r--r--   0        0        0     6215 2024-04-29 21:16:31.307313 alluka-0.2.0/tests/test_abc.py
+-rw-r--r--   0        0        0    50719 2024-04-29 21:16:31.311313 alluka-0.2.0/tests/test_async_callback_di.py
+-rw-r--r--   0        0        0    52005 2024-04-29 21:16:31.311313 alluka-0.2.0/tests/test_async_callback_di_future_annotations.py
+-rw-r--r--   0        0        0    45829 2024-04-29 21:16:31.311313 alluka-0.2.0/tests/test_callback_di.py
+-rw-r--r--   0        0        0    46212 2024-04-29 21:16:31.311313 alluka-0.2.0/tests/test_callback_di_future_annotations.py
+-rw-r--r--   0        0        0     6357 2024-04-29 21:16:31.311313 alluka-0.2.0/tests/test_local.py
+-rw-r--r--   0        0        0     1954 1970-01-01 00:00:00.000000 alluka-0.2.0/PKG-INFO
```

### Comparing `alluka-0.1.5/.github/pull_request_template.md` & `alluka-0.2.0/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `alluka-0.1.5/.github/workflows/freeze-for-pr.yml` & `alluka-0.2.0/.github/workflows/freeze-for-pr.yml`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     paths: ["piped", "pyproject.toml", "requirements.in", "dev-requirements/*.in", "!dev-requirements/constraints.in"]
 
 jobs:
   freeze-pr-dep-changes:
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f
+      - uses: actions/checkout@0ad4b8fadaa221de15dcec353f45205ec38ea70b
         with:
           submodules: "true"
 
       - name: Set up Python 3.9
         uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
         with:
           python-version: "3.9"
```

### Comparing `alluka-0.1.5/.github/workflows/lint.yml` & `alluka-0.2.0/piped/.github/workflows/lint.yml`

 * *Files 10% similar despite different names*

```diff
@@ -16,32 +16,29 @@
   workflow_dispatch:
 
 jobs:
   lint:
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f
+      - uses: actions/checkout@0ad4b8fadaa221de15dcec353f45205ec38ea70b
         with:
           submodules: "true"
 
-      - name: Set up Python 3.9
+      - name: Set up Python 3.11
         uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
         with:
-          python-version: "3.9"
+          python-version: "3.11"
 
       - name: install prerequisites
         run: |
           python -m pip install --upgrade pip wheel
-          python -m pip install -r ./piped/python/base-requirements/nox.txt
+          python -m pip install -r ./python/base-requirements/nox.txt
 
       - name: Lint markup
         run: python -m nox -s verify-markup
 
       - name: Check spelling
         run: python -m nox -s spell-check
 
       - name: Lint with flake8
         run: python -m nox -s flake8
-
-      - name: Check slotting
-        run: python -m nox -s slot-check
```

### Comparing `alluka-0.1.5/.github/workflows/pr-docs.yml` & `alluka-0.2.0/.github/workflows/pr-docs.yml`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 jobs:
   deploy-docs-preview:
     runs-on: ubuntu-latest
 
     steps:
       - name: Fetch merge branch
-        uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f
+        uses: actions/checkout@0ad4b8fadaa221de15dcec353f45205ec38ea70b
         with:
           ref: ${{ github.event.pull_request.head.sha }}
           repository: ${{ github.event.pull_request.head.repo.full_name }}
           submodules: "true"
 
       - name: Set up Python 3.9
         if: github.event.action != 'closed'
```

### Comparing `alluka-0.1.5/.github/workflows/publish.yml` & `alluka-0.2.0/.github/workflows/publish.yml`

 * *Files 14% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     name: upload release to PyPI
     runs-on: ubuntu-latest
     environment: release
     permissions:
       id-token: write
 
     steps:
-      - uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f
+      - uses: actions/checkout@0ad4b8fadaa221de15dcec353f45205ec38ea70b
         with:
           submodules: "true"
 
       - name: Set up Python 3.9
         uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
         with:
           python-version: "3.9"
```

### Comparing `alluka-0.1.5/.github/workflows/py-test.yml` & `alluka-0.2.0/.github/workflows/py-test.yml`

 * *Files 16% similar despite different names*

```diff
@@ -22,15 +22,15 @@
       matrix:
         os: [ubuntu-latest, macos-latest, windows-latest]
         python-version: ["3.9", "3.10", "3.11", "3.12"]
 
     runs-on: ${{ matrix.os }}
 
     steps:
-      - uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f
+      - uses: actions/checkout@0ad4b8fadaa221de15dcec353f45205ec38ea70b
         with:
           submodules: "true"
 
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
         with:
           python-version: ${{ matrix.python-version }}
@@ -47,15 +47,15 @@
   # TODO: Could we switch over to gather coverage from the normal test runs and combining
   # the result once https://github.com/nedbat/coveragepy/issues/1002 is fixed?
   upload-coverage:
     # needs: [test]
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f
+      - uses: actions/checkout@0ad4b8fadaa221de15dcec353f45205ec38ea70b
         with:
           submodules: "true"
 
       - name: Set up Python 3.9
         uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
         with:
           python-version: "3.9"
@@ -66,15 +66,15 @@
           python -m pip install -r ./piped/python/base-requirements/nox.txt
 
       - name: Record coverage
         run: |
           python -m nox -s test-coverage
 
       - name: Upload coverage
-        uses: paambaati/codeclimate-action@a1831d7162ea1fbc612ffe5fb3b90278b7999d59
+        uses: paambaati/codeclimate-action@b74bb25d2074a4bc16bd06fffc1b299c07b1f886
         env:
           CC_TEST_REPORTER_ID: a965935acdc9066802d7201945219784c0f24d22e8a2dff0e6529207726bc8af
         with:
           coverageLocations: .coverage.xml:coverage.py
 
       - name: Archive coverage
         uses: actions/upload-artifact@65462800fd760344b1a7b4382951275a0abb4808
```

### Comparing `alluka-0.1.5/.github/workflows/reformat.yml` & `alluka-0.2.0/piped/github/actions/reformat.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 name: Reformat PR code
 
 concurrency:
-  group: ${{ github.workflow }}-${{ github.ref }}
+  {% raw %}group: ${{ github.workflow }}-${{ github.ref }}{% endraw %}
   cancel-in-progress: true
 
 on:
   pull_request:
     branches:
       - master
 
 jobs:
   reformat:
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f
+      - uses: actions/checkout@0ad4b8fadaa221de15dcec353f45205ec38ea70b
         with:
           submodules: "true"
 
-      - name: Set up Python 3.9
+      - name: Set up Python {{ DEFAULT_PY_VER }}
         uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
         with:
-          python-version: "3.9"
+          python-version: "{{ DEFAULT_PY_VER }}"
 
       - name: install prerequisites
         run: |
           python -m pip install --upgrade pip wheel
-          python -m pip install -r ./piped/python/base-requirements/nox.txt
+          python -m pip install -r {{ NOX_DEP_PATH }}
 
       - name: Reformat
         run: python -m nox -s reformat bot-package-diff
 
       - uses: actions/upload-artifact@65462800fd760344b1a7b4382951275a0abb4808
         with:
           name: gogo.patch
```

### Comparing `alluka-0.1.5/.github/workflows/release-docs.yml` & `alluka-0.2.0/.github/workflows/release-docs.yml`

 * *Files 15% similar despite different names*

```diff
@@ -5,15 +5,15 @@
   workflow_dispatch:
 
 jobs:
   publish-docs:
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f
+      - uses: actions/checkout@0ad4b8fadaa221de15dcec353f45205ec38ea70b
         with:
           submodules: "true"
 
       - name: Set up Python 3.9
         uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
         with:
           python-version: "3.9"
```

### Comparing `alluka-0.1.5/.github/workflows/resync-piped.yml` & `alluka-0.2.0/.github/workflows/resync-piped.yml`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     paths: ["piped", "piped.toml", "pyproject.toml"]
 
 jobs:
   resync-piped:
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f
+      - uses: actions/checkout@0ad4b8fadaa221de15dcec353f45205ec38ea70b
         with:
           submodules: "true"
 
       - name: Set up Python 3.9
         uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
         with:
           python-version: "3.9"
```

### Comparing `alluka-0.1.5/.github/workflows/type-check.yml` & `alluka-0.2.0/.github/workflows/type-check.yml`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
   workflow_dispatch:
 
 jobs:
   type-check:
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f
+      - uses: actions/checkout@0ad4b8fadaa221de15dcec353f45205ec38ea70b
         with:
           submodules: "true"
 
       - name: Set up Python 3.9
         uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
         with:
           python-version: "3.9"
```

### Comparing `alluka-0.1.5/.github/workflows/update-licence.yml` & `alluka-0.2.0/.github/workflows/update-licence.yml`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   workflow_dispatch:
 
 jobs:
   update-licence:
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f
+      - uses: actions/checkout@0ad4b8fadaa221de15dcec353f45205ec38ea70b
         with:
           submodules: "true"
 
       - name: Set up Python 3.9
         uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
         with:
           python-version: "3.9"
@@ -24,15 +24,15 @@
           python -m pip install --upgrade pip wheel
           python -m pip install -r ./piped/python/base-requirements/nox.txt
 
       - name: Update licence
         run: python -m nox -s update-licence
 
       - name: Create Pull Request
-        uses: peter-evans/create-pull-request@9153d834b60caba6d51c9b9510b087acf9f33f83
+        uses: peter-evans/create-pull-request@6d6857d36972b65feb161a90e484f2984215f83e
         with:
           author: "always-on-duty[bot] <120557446+always-on-duty[bot]@users.noreply.github.com>"
           branch: task/update-licence
           commit-message: Update licence
           committer: "always-on-duty[bot] <120557446+always-on-duty[bot]@users.noreply.github.com>"
           title: Update licence
           token: ${{ secrets.ACTIONS_TOKEN || secrets.GITHUB_TOKEN }}
```

### Comparing `alluka-0.1.5/.github/workflows/upgrade-locks.yml` & `alluka-0.2.0/piped/.github/workflows/upgrade-locks.yml`

 * *Files 14% similar despite different names*

```diff
@@ -6,33 +6,33 @@
   workflow_dispatch:
 
 jobs:
   upgrade-deps:
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f
+      - uses: actions/checkout@0ad4b8fadaa221de15dcec353f45205ec38ea70b
         with:
           submodules: "true"
 
-      - name: Set up Python 3.9
+      - name: Set up Python 3.11
         uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
         with:
-          python-version: "3.9"
+          python-version: "3.11"
 
       - name: install prerequisites
         run: |
           python -m pip install --upgrade pip wheel
-          python -m pip install -r ./piped/python/base-requirements/nox.txt
+          python -m pip install -r ./python/base-requirements/nox.txt
 
       - name: Upgrade dependency locks
         run: python -m nox -s freeze-locks
 
       - name: Create Pull Request
-        uses: peter-evans/create-pull-request@9153d834b60caba6d51c9b9510b087acf9f33f83
+        uses: peter-evans/create-pull-request@6d6857d36972b65feb161a90e484f2984215f83e
         with:
           author: "always-on-duty[bot] <120557446+always-on-duty[bot]@users.noreply.github.com>"
           branch: task/upgrade-deps
           commit-message: Upgrade dependency locks
           committer: "always-on-duty[bot] <120557446+always-on-duty[bot]@users.noreply.github.com>"
           title: Upgrade dependency locks
           token: ${{ secrets.ACTIONS_TOKEN || secrets.GITHUB_TOKEN }}
```

### Comparing `alluka-0.1.5/.github/workflows/verify-locks.yml` & `alluka-0.2.0/piped/.github/workflows/verify-locks.yml`

 * *Files 11% similar despite different names*

```diff
@@ -7,30 +7,30 @@
   group: ${{ github.workflow }}-${{ github.ref }}
   cancel-in-progress: true
 
 on:
   pull_request:
     branches:
       - master
-    paths: ["dev-requirements/*.txt"]
+    paths: ["bot/requirements.txt", "dev-requirements/*.txt", "python/base-requirements/*.txt"]
 
 jobs:
   verify-pr-dep-changes:
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f
+      - uses: actions/checkout@0ad4b8fadaa221de15dcec353f45205ec38ea70b
         with:
           submodules: "true"
 
-      - name: Set up Python 3.9
+      - name: Set up Python 3.11
         uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
         with:
-          python-version: "3.9"
+          python-version: "3.11"
 
       - name: install prerequisites
         run: |
           python -m pip install --upgrade pip wheel
-          python -m pip install -r ./piped/python/base-requirements/nox.txt
+          python -m pip install -r ./python/base-requirements/nox.txt
 
       - name: Verify dependency locks
         run: python -m nox -s verify-deps
```

### Comparing `alluka-0.1.5/.github/workflows/verify-types.yml` & `alluka-0.2.0/.github/workflows/verify-types.yml`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
   workflow_dispatch:
 
 jobs:
   verify-types:
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f
+      - uses: actions/checkout@0ad4b8fadaa221de15dcec353f45205ec38ea70b
         with:
           submodules: "true"
 
       - name: Set up Python 3.9
         uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
         with:
           python-version: "3.9"
```

### Comparing `alluka-0.1.5/.gitignore` & `alluka-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `alluka-0.1.5/CODE_OF_CONDUCT.md` & `alluka-0.2.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `alluka-0.1.5/CONTRIBUTING.md` & `alluka-0.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `alluka-0.1.5/LICENSE` & `alluka-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alluka-0.1.5/README.md` & `alluka-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `alluka-0.1.5/alluka/__init__.py` & `alluka-0.2.0/alluka/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,13 +49,13 @@
 from . import abc
 from ._client import BasicContext
 from ._client import Client
 from ._client import inject
 from ._errors import AllukaError
 from ._errors import MissingDependencyError
 from ._errors import SyncOnlyError
-from ._self_injecting import AsyncSelfInjecting
-from ._self_injecting import SelfInjecting
+from ._self_injecting import AsyncSelfInjecting  # pyright: ignore[reportDeprecated]
+from ._self_injecting import SelfInjecting  # pyright: ignore[reportDeprecated]
 from ._types import Injected
 from ._types import InjectedDescriptor
 
 AsyncOnlyError = SyncOnlyError
```

### Comparing `alluka-0.1.5/alluka/_client.py` & `alluka-0.2.0/alluka/_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,44 +25,57 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 """Alluka's standard injection client implementation."""
+
+# pyright: reportOverlappingOverload=warning
+
 from __future__ import annotations
 
 __all__: list[str] = ["BasicContext", "Client", "inject"]
 
 import asyncio
+import enum
 import typing
+import warnings
 import weakref
 from collections import abc as collections
 
+import typing_extensions
+
 from . import _errors  # pyright: ignore[reportPrivateUsage]
 from . import _self_injecting  # pyright: ignore[reportPrivateUsage]
 from . import _types  # pyright: ignore[reportPrivateUsage]
 from . import _visitor
 from . import abc as alluka
 
 if typing.TYPE_CHECKING:
     from typing_extensions import Self
 
-# pyright: reportOverlappingOverload=warning
 
 _T = typing.TypeVar("_T")
 
 
 _AnyCoro = collections.Coroutine[typing.Any, typing.Any, typing.Any]
 _CallbackSigT = typing.TypeVar("_CallbackSigT", bound=alluka.CallbackSig[typing.Any])
 _DefaultT = typing.TypeVar("_DefaultT")
 _SyncCallbackSigT = typing.TypeVar("_SyncCallbackSigT", bound=collections.Callable[..., typing.Any])
 
 _TypeT = type[_T]
-_UndefinedOr = typing.Union[alluka.Undefined, _T]
+
+
+class _NoDefaultEnum(enum.Enum):
+    VALUE = object()
+
+
+_NO_VALUE: typing.Literal[_NoDefaultEnum.VALUE] = _NoDefaultEnum.VALUE
+_NoValueOr = typing.Union[_T, typing.Literal[_NoDefaultEnum.VALUE]]
 
 
 @typing.overload
 def inject(*, callback: alluka.CallbackSig[_T]) -> _T: ...
 
 
 @typing.overload
@@ -160,33 +173,37 @@
         except KeyError:
             pass
 
         # TODO: introspect_annotations=self._introspect_annotations
         descriptors = self._descriptors[callback] = _visitor.Callback(callback).accept(_visitor.ParameterVisitor())
         return descriptors
 
-    def as_async_self_injecting(self, callback: _CallbackSigT, /) -> alluka.AsyncSelfInjecting[_CallbackSigT]:
+    def make_context(self) -> alluka.Context:
         # <<inherited docstring from alluka.abc.Client>>.
-        return _self_injecting.AsyncSelfInjecting(self, callback)
+        return BasicContext(self)
 
-    def as_self_injecting(self, callback: _SyncCallbackSigT, /) -> alluka.SelfInjecting[_SyncCallbackSigT]:
+    @typing_extensions.deprecated("Use .auto_inject")
+    def as_async_self_injecting(
+        self, callback: _CallbackSigT, /
+    ) -> alluka.AsyncSelfInjecting[_CallbackSigT]:  # pyright: ignore[reportDeprecated]
         # <<inherited docstring from alluka.abc.Client>>.
-        return _self_injecting.SelfInjecting(self, callback)
+        with warnings.catch_warnings():
+            warnings.filterwarnings("ignore", category=DeprecationWarning)
 
-    @typing.overload
-    def call_with_di(
-        self, callback: collections.Callable[..., _AnyCoro], *args: typing.Any, **kwargs: typing.Any
-    ) -> typing.NoReturn: ...
-
-    @typing.overload
-    def call_with_di(self, callback: collections.Callable[..., _T], *args: typing.Any, **kwargs: typing.Any) -> _T: ...
+            return _self_injecting.AsyncSelfInjecting(self, callback)  # pyright: ignore[reportDeprecated]
 
-    def call_with_di(self, callback: collections.Callable[..., _T], *args: typing.Any, **kwargs: typing.Any) -> _T:
+    @typing_extensions.deprecated("Use .auto_inject_async")
+    def as_self_injecting(
+        self, callback: _SyncCallbackSigT, /
+    ) -> alluka.SelfInjecting[_SyncCallbackSigT]:  # pyright: ignore[reportDeprecated]
         # <<inherited docstring from alluka.abc.Client>>.
-        return BasicContext(self).call_with_di(callback, *args, **kwargs)
+        with warnings.catch_warnings():
+            warnings.filterwarnings("ignore", category=DeprecationWarning)
+
+            return _self_injecting.SelfInjecting(self, callback)  # pyright: ignore[reportDeprecated]
 
     @typing.overload
     def call_with_ctx(
         self,
         ctx: alluka.Context,
         callback: collections.Callable[..., _AnyCoro],
         *args: typing.Any,
@@ -209,18 +226,14 @@
 
         result = callback(*args, **kwargs)
         if asyncio.iscoroutine(result):
             raise _errors.SyncOnlyError
 
         return result
 
-    async def call_with_async_di(self, callback: alluka.CallbackSig[_T], *args: typing.Any, **kwargs: typing.Any) -> _T:
-        # <<inherited docstring from alluka.abc.Client>>.
-        return await BasicContext(self).call_with_async_di(callback, *args, **kwargs)
-
     async def call_with_ctx_async(
         self, ctx: alluka.Context, callback: alluka.CallbackSig[_T], *args: typing.Any, **kwargs: typing.Any
     ) -> _T:
         # <<inherited docstring from alluka.abc.Client>>.
         if descriptors := self._build_descriptors(callback):
             # Pyright currently doesn't support `is` for narrowing tuple types like this
             # This prioritises passed **kwargs over the injected dependencies.
@@ -237,24 +250,29 @@
 
     def set_type_dependency(self, type_: type[_T], value: _T, /) -> Self:
         # <<inherited docstring from alluka.abc.Client>>.
         self._type_dependencies[type_] = value
         return self
 
     @typing.overload
-    def get_type_dependency(self, type_: type[_T], /) -> _UndefinedOr[_T]: ...
+    def get_type_dependency(self, type_: type[_T], /) -> _T: ...
 
     @typing.overload
     def get_type_dependency(self, type_: type[_T], /, *, default: _DefaultT) -> typing.Union[_T, _DefaultT]: ...
 
     def get_type_dependency(
-        self, type_: type[_T], /, *, default: _UndefinedOr[_DefaultT] = alluka.UNDEFINED
-    ) -> typing.Union[_T, _DefaultT, alluka.Undefined]:
+        self, type_: type[_T], /, *, default: _NoValueOr[_DefaultT] = _NO_VALUE
+    ) -> typing.Union[_T, _DefaultT]:
         # <<inherited docstring from alluka.abc.Client>>.
-        return self._type_dependencies.get(type_, default)
+        result = self._type_dependencies.get(type_, default)
+
+        if result is _NO_VALUE:
+            raise KeyError
+
+        return result
 
     def remove_type_dependency(self, type_: type[typing.Any], /) -> Self:
         # <<inherited docstring from alluka.abc.Client>>.
         del self._type_dependencies[type_]
         return self
 
     def set_callback_override(self, callback: alluka.CallbackSig[_T], override: alluka.CallbackSig[_T], /) -> Self:
@@ -298,57 +316,51 @@
         # <<inherited docstring from alluka.abc.Context>>.
         if self._result_cache is None:
             self._result_cache = {}
 
         self._result_cache[callback] = value
 
     @typing.overload
-    def call_with_di(
-        self, callback: collections.Callable[..., _AnyCoro], *args: typing.Any, **kwargs: typing.Any
-    ) -> typing.NoReturn: ...
-
-    @typing.overload
-    def call_with_di(self, callback: collections.Callable[..., _T], *args: typing.Any, **kwargs: typing.Any) -> _T: ...
-
-    def call_with_di(self, callback: collections.Callable[..., _T], *args: typing.Any, **kwargs: typing.Any) -> _T:
-        # <<inherited docstring from alluka.abc.Context>>.
-        return self._injection_client.call_with_ctx(self, callback, *args, **kwargs)
-
-    async def call_with_async_di(self, callback: alluka.CallbackSig[_T], *args: typing.Any, **kwargs: typing.Any) -> _T:
-        # <<inherited docstring from alluka.abc.Context>>.
-        return await self._injection_client.call_with_ctx_async(self, callback, *args, **kwargs)
-
-    @typing.overload
-    def get_cached_result(self, callback: alluka.CallbackSig[_T], /) -> _UndefinedOr[_T]: ...
+    def get_cached_result(self, callback: alluka.CallbackSig[_T], /) -> _T: ...
 
     @typing.overload
     def get_cached_result(
         self, callback: alluka.CallbackSig[_T], /, *, default: _DefaultT
     ) -> typing.Union[_T, _DefaultT]: ...
 
     def get_cached_result(
-        self, callback: alluka.CallbackSig[_T], /, *, default: _UndefinedOr[_DefaultT] = alluka.UNDEFINED
-    ) -> typing.Union[_T, _DefaultT, alluka.Undefined]:
+        self, callback: alluka.CallbackSig[_T], /, *, default: _NoValueOr[_DefaultT] = _NO_VALUE
+    ) -> typing.Union[_T, _DefaultT]:
         # <<inherited docstring from alluka.abc.Context>>.
-        return self._result_cache.get(callback, default) if self._result_cache else default
+        result = self._result_cache.get(callback, default) if self._result_cache else default
+
+        if result is _NO_VALUE:
+            raise KeyError
+
+        return result
 
     @typing.overload
-    def get_type_dependency(self, type_: type[_T], /) -> _UndefinedOr[_T]: ...
+    def get_type_dependency(self, type_: type[_T], /) -> _T: ...
 
     @typing.overload
     def get_type_dependency(self, type_: type[_T], /, *, default: _DefaultT) -> typing.Union[_T, _DefaultT]: ...
 
     def get_type_dependency(
-        self, type_: type[_T], /, *, default: _UndefinedOr[_DefaultT] = alluka.UNDEFINED
-    ) -> typing.Union[_T, _DefaultT, alluka.Undefined]:
+        self, type_: type[_T], /, *, default: _NoValueOr[_DefaultT] = _NO_VALUE
+    ) -> typing.Union[_T, _DefaultT]:
         # <<inherited docstring from alluka.abc.Context>>.
         if self._special_case_types and (value := self._special_case_types.get(type_, default)) is not default:
             return typing.cast("_T", value)
 
-        return self._injection_client.get_type_dependency(type_, default=default)
+        result = self._injection_client.get_type_dependency(type_, default=default)
+
+        if result is _NO_VALUE:
+            raise KeyError
+
+        return result
 
     def _set_type_special_case(self, type_: type[_T], value: _T, /) -> Self:
         if not self._special_case_types:
             self._special_case_types = {}
 
         self._special_case_types[type_] = value
         return self
```

### Comparing `alluka-0.1.5/alluka/_errors.py` & `alluka-0.2.0/alluka/_errors.py`

 * *Files identical despite different names*

### Comparing `alluka-0.1.5/alluka/_self_injecting.py` & `alluka-0.2.0/alluka/_self_injecting.py`

 * *Files 13% similar despite different names*

```diff
@@ -24,156 +24,123 @@
 # DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+
+# pyright: reportDeprecated=none
+
 from __future__ import annotations
 
 __all__: list[str] = ["AsyncSelfInjecting", "SelfInjecting"]
 
 import typing
+import warnings
 from collections import abc as collections
 
+import typing_extensions
+
 from . import abc as alluka
 
 _CallbackSigT = typing.TypeVar("_CallbackSigT", bound=alluka.CallbackSig[typing.Any])
 _SyncCallbackT = typing.TypeVar("_SyncCallbackT", bound=collections.Callable[..., typing.Any])
 _T = typing.TypeVar("_T")
 _CoroT = collections.Coroutine[typing.Any, typing.Any, _T]
 
 
-class AsyncSelfInjecting(alluka.AsyncSelfInjecting[_CallbackSigT]):
-    """Class used to link an async function to a client to make it self-injecting.
+with warnings.catch_warnings():
+    warnings.filterwarnings("ignore", category=DeprecationWarning)
 
-    Examples
-    --------
-    ```py
-    async def callback(database: Database = alluka.inject(type=Database)) -> None:
-        await database.do_something()
-    ...
-
-    client = alluka.Client()
-    injecting_callback = alluka.AsyncSelfInjecting(callback, client)
-    await injecting_callback()
-    ```
-
-    Alternatively [alluka.abc.Client.as_async_self_injecting][] may be used:
-
-    ```py
-    client = alluka.Client()
-
-    @client.as_async_self_injecting
-    async def callback(database: Database = alluka.inject(type=Database)) -> None:
-        ...
-    ```
-    """
-
-    __slots__ = ("_callback", "_client")
-
-    def __init__(self, client: alluka.Client, callback: _CallbackSigT, /) -> None:
-        """Initialise a self injecting callback.
-
-        Parameters
-        ----------
-        client
-            The injection client to use to resolve dependencies.
-        callback : alluka.abc.CallbackSig
-            The callback to make self-injecting.
-
-            This may be sync or async.
-
-        Raises
-        ------
-        ValueError
-            If `callback` has any injected arguments which can only be passed
-            positionally.
+    @typing_extensions.deprecated("Use Client.auto_inject_async")
+    class AsyncSelfInjecting(alluka.AsyncSelfInjecting[_CallbackSigT]):
+        """Deprecated class for marking async functions as self-injecting.
+
+        Use [Client.auto_inject_async][alluka.abc.Client.auto_inject_async].
         """
-        self._callback = callback
-        self._client = client
 
-    @typing.overload
-    async def __call__(
-        self: AsyncSelfInjecting[collections.Callable[..., _CoroT[_T]]], *args: typing.Any, **kwargs: typing.Any
-    ) -> _T: ...
-
-    @typing.overload
-    async def __call__(
-        self: AsyncSelfInjecting[collections.Callable[..., _T]], *args: typing.Any, **kwargs: typing.Any
-    ) -> _T: ...
-
-    async def __call__(  # pyright: ignore[reportIncompatibleMethodOverride]
-        self: typing.Union[
-            AsyncSelfInjecting[collections.Callable[..., _T]], AsyncSelfInjecting[collections.Callable[..., _CoroT[_T]]]
-        ],
-        *args: typing.Any,
-        **kwargs: typing.Any,
-    ) -> _T:
-        # <<inherited docstring from alluka.abc.AsyncSelfInjecting>>.
-        return await self._client.call_with_async_di(self._callback, *args, **kwargs)
-
-    @property
-    def callback(self) -> _CallbackSigT:
-        # <<inherited docstring from alluka.abc.AsyncSelfInjecting>>.
-        return self._callback
-
-
-class SelfInjecting(alluka.SelfInjecting[_SyncCallbackT]):
-    """Class used to link a sync function to a client to make it self-injecting.
-
-    !!! note
-        This executes the callback synchronously and therefore will error if
-        any of the callback's dependencies are async.
-
-    Examples
-    --------
-    ```py
-    async def callback(database: Database = alluka.inject(type=Database)) -> None:
-        await database.do_something()
-    ...
-
-    client = alluka.Client()
-    injecting_callback = alluka.SelfInjecting(callback, client)
-    await injecting_callback()
-    ```
-
-    Alternatively [alluka.abc.Client.as_self_injecting][] may be used:
-
-    ```py
-    client = alluka.Client()
-
-    @client.as_self_injecting
-    async def callback(database: Database = alluka.inject(type=Database)) -> None:
-        ...
-    ```
-    """
-
-    __slots__ = ("_callback", "_client")
-
-    def __init__(self, client: alluka.Client, callback: _SyncCallbackT, /) -> None:
-        """Initialise a sync self injecting callback.
-
-        Parameters
-        ----------
-        client
-            The injection client to use to resolve dependencies.
-        callback : collections.abc.Callable
-            The callback to make self-injecting.
-
-        Raises
-        ------
-        ValueError
-            If `callback` has any injected arguments which can only be passed
-            positionally.
+        __slots__ = ("_callback", "_client")
+
+        def __init__(self, client: alluka.Client, callback: _CallbackSigT, /) -> None:
+            """Initialise a self injecting callback.
+
+            Parameters
+            ----------
+            client
+                The injection client to use to resolve dependencies.
+            callback : alluka.abc.CallbackSig
+                The callback to make self-injecting.
+
+                This may be sync or async.
+
+            Raises
+            ------
+            ValueError
+                If `callback` has any injected arguments which can only be passed
+                positionally.
+            """
+            self._callback = callback
+            self._client = client
+
+        @typing.overload
+        async def __call__(
+            self: AsyncSelfInjecting[collections.Callable[..., _CoroT[_T]]], *args: typing.Any, **kwargs: typing.Any
+        ) -> _T: ...
+
+        @typing.overload
+        async def __call__(
+            self: AsyncSelfInjecting[collections.Callable[..., _T]], *args: typing.Any, **kwargs: typing.Any
+        ) -> _T: ...
+
+        async def __call__(  # pyright: ignore[reportIncompatibleMethodOverride]
+            self: typing.Union[
+                AsyncSelfInjecting[collections.Callable[..., _T]],
+                AsyncSelfInjecting[collections.Callable[..., _CoroT[_T]]],
+            ],
+            *args: typing.Any,
+            **kwargs: typing.Any,
+        ) -> _T:
+            # <<inherited docstring from alluka.abc.AsyncSelfInjecting>>.
+            return await self._client.call_with_async_di(self._callback, *args, **kwargs)
+
+        @property
+        def callback(self) -> _CallbackSigT:
+            # <<inherited docstring from alluka.abc.AsyncSelfInjecting>>.
+            return self._callback
+
+    @typing_extensions.deprecated("Use Client.inject_async")
+    class SelfInjecting(alluka.SelfInjecting[_SyncCallbackT]):
+        """Deprecated class for marking functions as self-injecting.
+
+        Use [Client.auto_inject][alluka.abc.Client.auto_inject].
         """
-        self._callback = callback
-        self._client = client
 
-    def __call__(self: SelfInjecting[collections.Callable[..., _T]], *args: typing.Any, **kwargs: typing.Any) -> _T:
-        # <<inherited docstring from alluka.abc.SelfInjecting>>.
-        return self._client.call_with_di(self._callback, *args, **kwargs)
-
-    @property
-    def callback(self) -> _SyncCallbackT:
-        # <<inherited docstring from alluka.abc.SelfInjecting>>.
-        return self._callback
+        __slots__ = ("_callback", "_client")
+
+        def __init__(self, client: alluka.Client, callback: _SyncCallbackT, /) -> None:
+            """Initialise a sync self injecting callback.
+
+            Parameters
+            ----------
+            client
+                The injection client to use to resolve dependencies.
+            callback : collections.abc.Callable
+                The callback to make self-injecting.
+
+            Raises
+            ------
+            ValueError
+                If `callback` has any injected arguments which can only be passed
+                positionally.
+            """
+            self._callback = callback
+            self._client = client
+
+        def __call__(self: SelfInjecting[collections.Callable[..., _T]], *args: typing.Any, **kwargs: typing.Any) -> _T:
+            # <<inherited docstring from alluka.abc.SelfInjecting>>.
+            return self._client.call_with_di(self._callback, *args, **kwargs)
+
+        @property
+        def callback(self) -> _SyncCallbackT:
+            # <<inherited docstring from alluka.abc.SelfInjecting>>.
+            return self._callback
```

### Comparing `alluka-0.1.5/alluka/_types.py` & `alluka-0.2.0/alluka/_types.py`

 * *Files identical despite different names*

### Comparing `alluka-0.1.5/alluka/_vendor/inspect.py` & `alluka-0.2.0/alluka/_vendor/inspect.py`

 * *Files identical despite different names*

### Comparing `alluka-0.1.5/alluka/_vendor/inspect.py.LICENSE` & `alluka-0.2.0/alluka/_vendor/inspect.py.LICENSE`

 * *Files identical despite different names*

### Comparing `alluka-0.1.5/alluka/_vendor/inspect.pyi` & `alluka-0.2.0/alluka/_vendor/inspect.pyi`

 * *Files identical despite different names*

### Comparing `alluka-0.1.5/alluka/_vendor/inspect.pyi.LICENSE` & `alluka-0.2.0/alluka/_vendor/inspect.pyi.LICENSE`

 * *Files identical despite different names*

### Comparing `alluka-0.1.5/alluka/_visitor.py` & `alluka-0.2.0/alluka/_visitor.py`

 * *Files identical despite different names*

### Comparing `alluka-0.1.5/alluka/abc.py` & `alluka-0.2.0/alluka/abc.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,75 +25,40 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 """Alluka's abstract interfaces."""
+
+# pyright: reportOverlappingOverload=warning
+
 from __future__ import annotations
 
-__all__: list[str] = [
-    "AsyncSelfInjecting",
-    "CallbackSig",
-    "Client",
-    "Context",
-    "SelfInjecting",
-    "UNDEFINED",
-    "Undefined",
-]
+__all__: list[str] = ["AsyncSelfInjecting", "CallbackSig", "Client", "Context", "SelfInjecting"]
 
 import abc
+import functools
 import typing
 from collections import abc as collections
 
+import typing_extensions
+
 if typing.TYPE_CHECKING:
     from typing_extensions import Self
 
-# pyright: reportOverlappingOverload=warning
+    _P = typing_extensions.ParamSpec("_P")
 
 _T = typing.TypeVar("_T")
 _CoroT = collections.Coroutine[typing.Any, typing.Any, _T]
 _CallbackT = typing.TypeVar("_CallbackT", bound="CallbackSig[typing.Any]")
 _DefaultT = typing.TypeVar("_DefaultT")
 _SyncCallbackT = typing.TypeVar("_SyncCallbackT", bound=collections.Callable[..., typing.Any])
 
 
-class Undefined:
-    """Deprecated type of the [UNDEFINED][alluka.abc.UNDEFINED] constant.
-
-    !!! warning "deprecated"
-        This will be removed in `v0.2.0`.
-    """
-
-    __slots__ = ()
-    __instance: Undefined  # pyright: ignore[reportUninitializedInstanceVariable]
-
-    def __bool__(self) -> typing.Literal[False]:
-        return False
-
-    def __new__(cls) -> Undefined:
-        try:
-            return cls.__instance
-
-        except AttributeError:
-            new = super().__new__(cls)
-            assert isinstance(new, Undefined)
-            cls.__instance = new
-            return cls.__instance
-
-
-UNDEFINED: typing.Final[Undefined] = Undefined()
-"""Deprecated singleton value used to indicate that a value is undefined
-
-!!! warning "deprecated"
-    This will be removedin `v0.2.0`.
-"""
-_UndefinedOr = typing.Union[Undefined, _T]
-
-
 CallbackSig = collections.Callable[..., typing.Union[_CoroT[_T], _T]]
 """Type-hint of a injector callback.
 
 !!! note
     Dependency dependency injection is recursively supported, meaning that the
     keyword arguments for a dependency callback may also ask for dependencies
     themselves.
@@ -108,62 +73,113 @@
 
 class Client(abc.ABC):
     """Abstract interface of a dependency injection client."""
 
     __slots__ = ()
 
     @abc.abstractmethod
-    def as_async_self_injecting(self, callback: _CallbackT, /) -> AsyncSelfInjecting[_CallbackT]:
-        """Link a function to a client to make it self-injecting.
+    def make_context(self) -> Context:
+        """Create a dependency injection context.
+
+        Returns
+        -------
+        alluka.abc.Context
+            The created DI context, bound to the current client.
+        """
+
+    @abc.abstractmethod
+    @typing_extensions.deprecated("Use .auto_inject_async")
+    def as_async_self_injecting(
+        self, callback: _CallbackT, /
+    ) -> AsyncSelfInjecting[_CallbackT]:  # pyright: ignore[reportDeprecated]
+        """Deprecated callback for making async functions auto-inject.
+
+        Use [Client.auto_inject_async][alluka.abc.Client.auto_inject_async].
+        """
+
+    @abc.abstractmethod
+    @typing_extensions.deprecated("Use .auto_inject")
+    def as_self_injecting(
+        self, callback: _SyncCallbackT, /
+    ) -> SelfInjecting[_SyncCallbackT]:  # pyright: ignore[reportDeprecated]
+        """Deprecated callback for making functions auto-inject.
+
+        Use [Client.auto_inject][alluka.abc.Client.auto_inject].
+        """
+
+    def auto_inject(self, callback: collections.Callable[_P, _T], /) -> collections.Callable[_P, _T]:
+        """Wrap a function to make calls to it always inject dependencies.
+
+        Examples
+        --------
+        ```py
+        @client.auto_inject
+        def callback(dep: Injected[Type]) -> None:
+            ...
+
+        callback()  # The requested dependencies will be passed.
+        ```
 
         Parameters
         ----------
-        callback : CallbackSig
-            The callback to make self-injecting.
-
-            This may be sync or async.
+        callback
+            The callback to wrap with DI.
 
         Returns
         -------
-        AsyncSelfInjecting
-            The async self-injecting callback.
+        collections.Callable
+            The wrapped auto injecting callback.
         """
 
-    @abc.abstractmethod
-    def as_self_injecting(self, callback: _SyncCallbackT, /) -> SelfInjecting[_SyncCallbackT]:
-        """Link a sync function to a client to make it self-injecting.
+        @functools.wraps(callback)
+        def wrapped_callback(*args: _P.args, **kwargs: _P.kwargs) -> _T:
+            return self.call_with_di(callback, *args, **kwargs)
+
+        return wrapped_callback
 
-        !!! note
-            This uses sync dependency injection and therefore will lead
-            to errors if any of the callback's dependencies are async.
+    def auto_inject_async(
+        self, callback: collections.Callable[_P, _CoroT[_T]], /
+    ) -> collections.Callable[_P, _CoroT[_T]]:
+        """Wrap an async function to make calls to it always inject dependencies.
+
+        Examples
+        --------
+        ```py
+        @client.auto_inject_async
+        async def callback(dep: Injected[Type]) -> None:
+            ...
+
+        await callback()  # The requested dependencies will be passed.
+        ```
 
         Parameters
         ----------
-        callback : collections.abc.Callable
-            The callback to make self-injecting.
-
-            This must be sync.
+        callback
+            The callback to wrap with DI.
 
         Returns
         -------
-        SelfInjecting
-            The self-injecting callback.
+        collections.Callable
+            The wrapped auto injecting callback.
         """
 
+        @functools.wraps(callback)
+        def wrapped_callback(*args: _P.args, **kwargs: _P.kwargs) -> _CoroT[_T]:
+            return self.call_with_async_di(callback, *args, **kwargs)
+
+        return wrapped_callback
+
     @typing.overload
-    @abc.abstractmethod
     def call_with_di(
         self, callback: collections.Callable[..., _CoroT[typing.Any]], *args: typing.Any, **kwargs: typing.Any
     ) -> typing.NoReturn: ...
 
     @typing.overload
-    @abc.abstractmethod
     def call_with_di(self, callback: collections.Callable[..., _T], *args: typing.Any, **kwargs: typing.Any) -> _T: ...
 
-    @abc.abstractmethod
     def call_with_di(self, callback: collections.Callable[..., _T], *args: typing.Any, **kwargs: typing.Any) -> _T:
         """Call a function with sync dependency injection.
 
         Parameters
         ----------
         callback
             The callback to call.
@@ -183,14 +199,15 @@
         ------
         alluka.MissingDependencyError
             If any of the callback's required type dependencies aren't implemented
             by the client.
         alluka.SyncOnlyError
             If the callback or any of its callback dependencies are async.
         """
+        return self.make_context().call_with_di(callback, *args, **kwargs)
 
     @typing.overload
     @abc.abstractmethod
     def call_with_ctx(
         self,
         ctx: Context,
         callback: collections.Callable[..., _CoroT[typing.Any]],
@@ -235,15 +252,14 @@
         alluka.MissingDependencyError
             If any of the callback's required type dependencies aren't implemented
             by the client.
         alluka.SyncOnlyError
             If the callback or any of its callback dependencies are async.
         """
 
-    @abc.abstractmethod
     async def call_with_async_di(self, callback: CallbackSig[_T], *args: typing.Any, **kwargs: typing.Any) -> _T:
         """Call a function with async dependency injection.
 
         Parameters
         ----------
         callback
             The callback to call.
@@ -263,14 +279,15 @@
         ------
         alluka.MissingDependencyError
             If any of the callback's required type dependencies aren't implemented
             by the client.
         alluka.SyncOnlyError
             If the callback or any of its callback dependencies are async.
         """
+        return await self.make_context().call_with_async_di(callback, *args, **kwargs)
 
     @abc.abstractmethod
     async def call_with_ctx_async(
         self, ctx: Context, callback: CallbackSig[_T], *args: typing.Any, **kwargs: typing.Any
     ) -> _T:
         """Asynchronously call a function with a pre-existing DI context.
 
@@ -316,44 +333,43 @@
         -------
         Self
             The client instance to allow chaining.
         """
 
     @typing.overload
     @abc.abstractmethod
-    def get_type_dependency(self, type_: type[_T], /) -> _UndefinedOr[_T]: ...
+    def get_type_dependency(self, type_: type[_T], /) -> _T: ...
 
     @typing.overload
     @abc.abstractmethod
     def get_type_dependency(self, type_: type[_T], /, *, default: _DefaultT) -> typing.Union[_T, _DefaultT]: ...
 
     @abc.abstractmethod
-    def get_type_dependency(
-        self, type_: type[_T], /, *, default: _UndefinedOr[_DefaultT] = UNDEFINED
-    ) -> typing.Union[_T, _DefaultT, Undefined]:
+    def get_type_dependency(self, type_: type[_T], /, *, default: _DefaultT = ...) -> typing.Union[_T, _DefaultT]:
         """Get the implementation for an injected type.
 
-        !!! warning "deprecated"
-            Defaulting to [alluka.abc.UNDEFINED][] is deprecated and will be
-            replaced by a [KeyError][] raise in `v0.2.0`.
-
         Parameters
         ----------
         type_
             The associated type.
         default
             The default value to return if the type is not implemented.
 
         Returns
         -------
-        _T | _DefaultT | alluka.abc.UNDEFINED
+        _T | _DefaultT
             The resolved type if found.
 
             If the type isn't implemented then the value of `default`
-            will be returned if it is provided, else [alluka.abc.UNDEFINED][].
+            will be returned if it is provided.
+
+        Raises
+        ------
+        KeyError
+            If no dependency was found when no default was provided.
         """
 
     @abc.abstractmethod
     def remove_type_dependency(self, type_: type[typing.Any], /) -> Self:
         """Remove a type dependency.
 
         Parameters
@@ -444,24 +460,21 @@
         callback
             The callback to cache the result of.
         value
             The value to cache.
         """
 
     @typing.overload
-    @abc.abstractmethod
     def call_with_di(
         self, callback: collections.Callable[..., _CoroT[typing.Any]], *args: typing.Any, **kwargs: typing.Any
     ) -> typing.NoReturn: ...
 
     @typing.overload
-    @abc.abstractmethod
     def call_with_di(self, callback: collections.Callable[..., _T], *args: typing.Any, **kwargs: typing.Any) -> _T: ...
 
-    @abc.abstractmethod
     def call_with_di(self, callback: collections.Callable[..., _T], *args: typing.Any, **kwargs: typing.Any) -> _T:
         """Call a function with the current DI context.
 
         Parameters
         ----------
         callback
             The callback to call.
@@ -481,16 +494,16 @@
         ------
         alluka.MissingDependencyError
             If any of the callback's required type dependencies aren't implemented
             by the client.
         alluka.SyncOnlyError
             If the callback or any of its callback dependencies are async.
         """
+        return self.injection_client.call_with_ctx(self, callback, *args, **kwargs)
 
-    @abc.abstractmethod
     async def call_with_async_di(self, callback: CallbackSig[_T], *args: typing.Any, **kwargs: typing.Any) -> _T:
         """Asynchronously call a function with the current DI context.
 
         Parameters
         ----------
         callback
             The callback to call.
@@ -508,88 +521,90 @@
 
         Raises
         ------
         alluka.MissingDependencyError
             If any of the callback's required type dependencies aren't implemented
             by the client.
         """
+        return await self.injection_client.call_with_ctx_async(self, callback, *args, **kwargs)
 
     @typing.overload
     @abc.abstractmethod
-    def get_cached_result(self, callback: CallbackSig[_T], /) -> _UndefinedOr[_T]: ...
+    def get_cached_result(self, callback: CallbackSig[_T], /) -> _T: ...
 
     @typing.overload
     @abc.abstractmethod
     def get_cached_result(self, callback: CallbackSig[_T], /, *, default: _DefaultT) -> typing.Union[_T, _DefaultT]: ...
 
     @abc.abstractmethod
     def get_cached_result(
-        self, callback: CallbackSig[_T], /, *, default: _UndefinedOr[_DefaultT] = UNDEFINED
-    ) -> typing.Union[_T, _DefaultT, Undefined]:
+        self, callback: CallbackSig[_T], /, *, default: _DefaultT = ...
+    ) -> typing.Union[_T, _DefaultT]:
         """Get the cached result of a callback.
 
-        !!! warning "deprecated"
-            Defaulting to [alluka.abc.UNDEFINED][] is deprecated and will be
-            replaced by a [KeyError][] raise in `v0.2.0`.
-
         Parameters
         ----------
         callback
             The callback to get the cached result of.
         default
             The default value to return if the callback is not cached.
 
         Returns
         -------
-        _T | _DefaultT | alluka.abc.UNDEFINED
+        _T | _DefaultT
             The cached result of the callback if found.
 
             If the callback's result hasn't been cached or caching isn't
             implementing then this will return the value of `default` if it
-            is provided, else [alluka.abc.UNDEFINED][].
+            is provided.
+
+        Raises
+        ------
+        KeyError
+            If no value was found when no default was provided.
         """
 
     @typing.overload
     @abc.abstractmethod
-    def get_type_dependency(self, type_: type[_T], /) -> _UndefinedOr[_T]: ...
+    def get_type_dependency(self, type_: type[_T], /) -> _T: ...
 
     @typing.overload
     @abc.abstractmethod
     def get_type_dependency(self, type_: type[_T], /, *, default: _DefaultT) -> typing.Union[_T, _DefaultT]: ...
 
     @abc.abstractmethod
-    def get_type_dependency(
-        self, type_: type[_T], /, *, default: _UndefinedOr[_DefaultT] = UNDEFINED
-    ) -> typing.Union[_T, _DefaultT, Undefined]:
+    def get_type_dependency(self, type_: type[_T], /, *, default: _DefaultT = ...) -> typing.Union[_T, _DefaultT]:
         """Get the implementation for an injected type.
 
         Unlike [Client.get_type_dependency][alluka.abc.Client.get_type_dependency],
         this method may also return context specific implementations of a type.
 
-        !!! warning "deprecated"
-            Defaulting to [alluka.abc.UNDEFINED][] is deprecated and will be
-            replaced by a [KeyError][] raise in `v0.2.0`.
-
         Parameters
         ----------
         type_
             The associated type.
         default
             The default value to return if the type is not implemented.
 
         Returns
         -------
-        _T | _DefaultT | alluka.abc.UNDEFINED
+        _T | _DefaultT
             The resolved type if found.
 
             If the type isn't implemented then the value of `default`
-            will be returned if it is provided, else [alluka.abc.UNDEFINED][].
+            will be returned if it is provided.
+
+        Raises
+        ------
+        KeyError
+            If no dependency was found when no default was provided.
         """
 
 
+@typing_extensions.deprecated("Use Client.auto_inject_async")
 class AsyncSelfInjecting(abc.ABC, typing.Generic[_CallbackT]):
     """Interface of a class used to make an async self-injecting callback.
 
     Examples
     --------
     ```py
     client = alluka.Client()
@@ -606,27 +621,32 @@
     @abc.abstractmethod
     def callback(self) -> _CallbackT:
         """The callback this wraps."""
 
     @typing.overload
     @abc.abstractmethod
     async def __call__(
-        self: AsyncSelfInjecting[collections.Callable[..., _CoroT[_T]]], *args: typing.Any, **kwargs: typing.Any
+        self: AsyncSelfInjecting[collections.Callable[..., _CoroT[_T]]],  # pyright: ignore[reportDeprecated]
+        *args: typing.Any,
+        **kwargs: typing.Any,
     ) -> _T: ...
 
     @typing.overload
     @abc.abstractmethod
     async def __call__(
-        self: AsyncSelfInjecting[collections.Callable[..., _T]], *args: typing.Any, **kwargs: typing.Any
+        self: AsyncSelfInjecting[collections.Callable[..., _T]],  # pyright: ignore[reportDeprecated]
+        *args: typing.Any,
+        **kwargs: typing.Any,
     ) -> _T: ...
 
     @abc.abstractmethod
     async def __call__(
         self: typing.Union[
-            AsyncSelfInjecting[collections.Callable[..., _T]], AsyncSelfInjecting[collections.Callable[..., _CoroT[_T]]]
+            AsyncSelfInjecting[collections.Callable[..., _T]],  # pyright: ignore[reportDeprecated]
+            AsyncSelfInjecting[collections.Callable[..., _CoroT[_T]]],  # pyright: ignore[reportDeprecated]
         ],
         *args: typing.Any,
         **kwargs: typing.Any,
     ) -> _T:
         """Call this with the provided arguments and any injected arguments.
 
         Parameters
@@ -645,14 +665,15 @@
         ------
         alluka.MissingDependencyError
             If any of the callback's required type dependencies aren't implemented
             by the client.
         """
 
 
+@typing_extensions.deprecated("Use Client.auto_inject")
 class SelfInjecting(abc.ABC, typing.Generic[_SyncCallbackT]):
     """Interface of a class used to make a self-injecting callback.
 
     !!! note
         This executes the callback synchronously and therefore will error if
         any of the callback's dependencies are async.
 
@@ -671,15 +692,19 @@
 
     @property
     @abc.abstractmethod
     def callback(self) -> _SyncCallbackT:
         """The callback this wraps."""
 
     @abc.abstractmethod
-    def __call__(self: SelfInjecting[collections.Callable[..., _T]], *args: typing.Any, **kwargs: typing.Any) -> _T:
+    def __call__(
+        self: SelfInjecting[collections.Callable[..., _T]],  # pyright: ignore[reportDeprecated]
+        *args: typing.Any,
+        **kwargs: typing.Any,
+    ) -> _T:
         """Call this callback with the provided arguments + injected arguments.
 
         Parameters
         ----------
         *args
             Positional arguments to pass to the callback.
         **kwargs
```

### Comparing `alluka-0.1.5/dev-requirements/tests.txt` & `alluka-0.2.0/dev-requirements/tests.txt`

 * *Files 7% similar despite different names*

```diff
@@ -62,67 +62,67 @@
     --hash=sha256:ed86a35631f7bfbb28e108dd96773b9d5a6ce4811cf6ea468bb6a359b256b1e4 \
     --hash=sha256:ee07e47c12890ef248766a6e55bd38ebfb2bb8edd4142d56db91b21ea68b7627 \
     --hash=sha256:fa3a0128b152627161ce47201262d3140edb5a5c3da88d73a1b790a959126956 \
     --hash=sha256:fcc8eb6d5902bb1cf6dc4f187ee3ea80a1eba0a89aba40a5cb20a5087d961357
 colorama==0.4.6 ; python_full_version >= "3.9.0" and python_version < "3.13" and sys_platform == "win32" \
     --hash=sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44 \
     --hash=sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6
-coverage[toml]==7.4.4 ; python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:00838a35b882694afda09f85e469c96367daa3f3f2b097d846a7216993d37f4c \
-    --hash=sha256:0513b9508b93da4e1716744ef6ebc507aff016ba115ffe8ecff744d1322a7b63 \
-    --hash=sha256:09c3255458533cb76ef55da8cc49ffab9e33f083739c8bd4f58e79fecfe288f7 \
-    --hash=sha256:09ef9199ed6653989ebbcaacc9b62b514bb63ea2f90256e71fea3ed74bd8ff6f \
-    --hash=sha256:09fa497a8ab37784fbb20ab699c246053ac294d13fc7eb40ec007a5043ec91f8 \
-    --hash=sha256:0f9f50e7ef2a71e2fae92774c99170eb8304e3fdf9c8c3c7ae9bab3e7229c5cf \
-    --hash=sha256:137eb07173141545e07403cca94ab625cc1cc6bc4c1e97b6e3846270e7e1fea0 \
-    --hash=sha256:1f384c3cc76aeedce208643697fb3e8437604b512255de6d18dae3f27655a384 \
-    --hash=sha256:201bef2eea65e0e9c56343115ba3814e896afe6d36ffd37bab783261db430f76 \
-    --hash=sha256:38dd60d7bf242c4ed5b38e094baf6401faa114fc09e9e6632374388a404f98e7 \
-    --hash=sha256:3b799445b9f7ee8bf299cfaed6f5b226c0037b74886a4e11515e569b36fe310d \
-    --hash=sha256:3ea79bb50e805cd6ac058dfa3b5c8f6c040cb87fe83de10845857f5535d1db70 \
-    --hash=sha256:40209e141059b9370a2657c9b15607815359ab3ef9918f0196b6fccce8d3230f \
-    --hash=sha256:41c9c5f3de16b903b610d09650e5e27adbfa7f500302718c9ffd1c12cf9d6818 \
-    --hash=sha256:54eb8d1bf7cacfbf2a3186019bcf01d11c666bd495ed18717162f7eb1e9dd00b \
-    --hash=sha256:598825b51b81c808cb6f078dcb972f96af96b078faa47af7dfcdf282835baa8d \
-    --hash=sha256:5fc1de20b2d4a061b3df27ab9b7c7111e9a710f10dc2b84d33a4ab25065994ec \
-    --hash=sha256:623512f8ba53c422fcfb2ce68362c97945095b864cda94a92edbaf5994201083 \
-    --hash=sha256:690db6517f09336559dc0b5f55342df62370a48f5469fabf502db2c6d1cffcd2 \
-    --hash=sha256:69eb372f7e2ece89f14751fbcbe470295d73ed41ecd37ca36ed2eb47512a6ab9 \
-    --hash=sha256:73bfb9c09951125d06ee473bed216e2c3742f530fc5acc1383883125de76d9cd \
-    --hash=sha256:742a76a12aa45b44d236815d282b03cfb1de3b4323f3e4ec933acfae08e54ade \
-    --hash=sha256:7c95949560050d04d46b919301826525597f07b33beba6187d04fa64d47ac82e \
-    --hash=sha256:8130a2aa2acb8788e0b56938786c33c7c98562697bf9f4c7d6e8e5e3a0501e4a \
-    --hash=sha256:8a2b2b78c78293782fd3767d53e6474582f62443d0504b1554370bde86cc8227 \
-    --hash=sha256:8ce1415194b4a6bd0cdcc3a1dfbf58b63f910dcb7330fe15bdff542c56949f87 \
-    --hash=sha256:9ca28a302acb19b6af89e90f33ee3e1906961f94b54ea37de6737b7ca9d8827c \
-    --hash=sha256:a4cdc86d54b5da0df6d3d3a2f0b710949286094c3a6700c21e9015932b81447e \
-    --hash=sha256:aa5b1c1bfc28384f1f53b69a023d789f72b2e0ab1b3787aae16992a7ca21056c \
-    --hash=sha256:aadacf9a2f407a4688d700e4ebab33a7e2e408f2ca04dbf4aef17585389eff3e \
-    --hash=sha256:ae71e7ddb7a413dd60052e90528f2f65270aad4b509563af6d03d53e979feafd \
-    --hash=sha256:b14706df8b2de49869ae03a5ccbc211f4041750cd4a66f698df89d44f4bd30ec \
-    --hash=sha256:b1a93009cb80730c9bca5d6d4665494b725b6e8e157c1cb7f2db5b4b122ea562 \
-    --hash=sha256:b2991665420a803495e0b90a79233c1433d6ed77ef282e8e152a324bbbc5e0c8 \
-    --hash=sha256:b2c5edc4ac10a7ef6605a966c58929ec6c1bd0917fb8c15cb3363f65aa40e677 \
-    --hash=sha256:b4d33f418f46362995f1e9d4f3a35a1b6322cb959c31d88ae56b0298e1c22357 \
-    --hash=sha256:b91cbc4b195444e7e258ba27ac33769c41b94967919f10037e6355e998af255c \
-    --hash=sha256:c74880fc64d4958159fbd537a091d2a585448a8f8508bf248d72112723974cbd \
-    --hash=sha256:c901df83d097649e257e803be22592aedfd5182f07b3cc87d640bbb9afd50f49 \
-    --hash=sha256:cac99918c7bba15302a2d81f0312c08054a3359eaa1929c7e4b26ebe41e9b286 \
-    --hash=sha256:cc4f1358cb0c78edef3ed237ef2c86056206bb8d9140e73b6b89fbcfcbdd40e1 \
-    --hash=sha256:ccd341521be3d1b3daeb41960ae94a5e87abe2f46f17224ba5d6f2b8398016cf \
-    --hash=sha256:ce4b94265ca988c3f8e479e741693d143026632672e3ff924f25fab50518dd51 \
-    --hash=sha256:cf271892d13e43bc2b51e6908ec9a6a5094a4df1d8af0bfc360088ee6c684409 \
-    --hash=sha256:d5ae728ff3b5401cc320d792866987e7e7e880e6ebd24433b70a33b643bb0384 \
-    --hash=sha256:d71eec7d83298f1af3326ce0ff1d0ea83c7cb98f72b577097f9083b20bdaf05e \
-    --hash=sha256:d898fe162d26929b5960e4e138651f7427048e72c853607f2b200909794ed978 \
-    --hash=sha256:d89d7b2974cae412400e88f35d86af72208e1ede1a541954af5d944a8ba46c57 \
-    --hash=sha256:dfa8fe35a0bb90382837b238fff375de15f0dcdb9ae68ff85f7a63649c98527e \
-    --hash=sha256:e0be5efd5127542ef31f165de269f77560d6cdef525fffa446de6f7e9186cfb2 \
-    --hash=sha256:fdfafb32984684eb03c2d83e1e51f64f0906b11e64482df3c5db936ce3839d48 \
-    --hash=sha256:ff7687ca3d7028d8a5f0ebae95a6e4827c5616b31a4ee1192bdfde697db110d4
+coverage[toml]==7.5.0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
+    --hash=sha256:075299460948cd12722a970c7eae43d25d37989da682997687b34ae6b87c0ef0 \
+    --hash=sha256:07dfdd492d645eea1bd70fb1d6febdcf47db178b0d99161d8e4eed18e7f62fe7 \
+    --hash=sha256:0cbdf2cae14a06827bec50bd58e49249452d211d9caddd8bd80e35b53cb04631 \
+    --hash=sha256:2055c4fb9a6ff624253d432aa471a37202cd8f458c033d6d989be4499aed037b \
+    --hash=sha256:262fffc1f6c1a26125d5d573e1ec379285a3723363f3bd9c83923c9593a2ac25 \
+    --hash=sha256:280132aada3bc2f0fac939a5771db4fbb84f245cb35b94fae4994d4c1f80dae7 \
+    --hash=sha256:2b57780b51084d5223eee7b59f0d4911c31c16ee5aa12737c7a02455829ff067 \
+    --hash=sha256:2bd7065249703cbeb6d4ce679c734bef0ee69baa7bff9724361ada04a15b7e3b \
+    --hash=sha256:3235d7c781232e525b0761730e052388a01548bd7f67d0067a253887c6e8df46 \
+    --hash=sha256:33c020d3322662e74bc507fb11488773a96894aa82a622c35a5a28673c0c26f5 \
+    --hash=sha256:357754dcdfd811462a725e7501a9b4556388e8ecf66e79df6f4b988fa3d0b39a \
+    --hash=sha256:39793731182c4be939b4be0cdecde074b833f6171313cf53481f869937129ed3 \
+    --hash=sha256:3c2b77f295edb9fcdb6a250f83e6481c679335ca7e6e4a955e4290350f2d22a4 \
+    --hash=sha256:41327143c5b1d715f5f98a397608f90ab9ebba606ae4e6f3389c2145410c52b1 \
+    --hash=sha256:427e1e627b0963ac02d7c8730ca6d935df10280d230508c0ba059505e9233475 \
+    --hash=sha256:432949a32c3e3f820af808db1833d6d1631664d53dd3ce487aa25d574e18ad1c \
+    --hash=sha256:4ba01d9ba112b55bfa4b24808ec431197bb34f09f66f7cb4fd0258ff9d3711b1 \
+    --hash=sha256:4d0e206259b73af35c4ec1319fd04003776e11e859936658cb6ceffdeba0f5be \
+    --hash=sha256:51431d0abbed3a868e967f8257c5faf283d41ec882f58413cf295a389bb22e58 \
+    --hash=sha256:565b2e82d0968c977e0b0f7cbf25fd06d78d4856289abc79694c8edcce6eb2de \
+    --hash=sha256:6782cd6216fab5a83216cc39f13ebe30adfac2fa72688c5a4d8d180cd52e8f6a \
+    --hash=sha256:6afd2e84e7da40fe23ca588379f815fb6dbbb1b757c883935ed11647205111cb \
+    --hash=sha256:710c62b6e35a9a766b99b15cdc56d5aeda0914edae8bb467e9c355f75d14ee95 \
+    --hash=sha256:84921b10aeb2dd453247fd10de22907984eaf80901b578a5cf0bb1e279a587cb \
+    --hash=sha256:85a5dbe1ba1bf38d6c63b6d2c42132d45cbee6d9f0c51b52c59aa4afba057517 \
+    --hash=sha256:9c6384cc90e37cfb60435bbbe0488444e54b98700f727f16f64d8bfda0b84656 \
+    --hash=sha256:9dd88fce54abbdbf4c42fb1fea0e498973d07816f24c0e27a1ecaf91883ce69e \
+    --hash=sha256:a81eb64feded34f40c8986869a2f764f0fe2db58c0530d3a4afbcde50f314880 \
+    --hash=sha256:a898c11dca8f8c97b467138004a30133974aacd572818c383596f8d5b2eb04a9 \
+    --hash=sha256:a9960dd1891b2ddf13a7fe45339cd59ecee3abb6b8326d8b932d0c5da208104f \
+    --hash=sha256:a9a7ef30a1b02547c1b23fa9a5564f03c9982fc71eb2ecb7f98c96d7a0db5cf2 \
+    --hash=sha256:ad97ec0da94b378e593ef532b980c15e377df9b9608c7c6da3506953182398af \
+    --hash=sha256:adf032b6c105881f9d77fa17d9eebe0ad1f9bfb2ad25777811f97c5362aa07f2 \
+    --hash=sha256:bbfe6389c5522b99768a93d89aca52ef92310a96b99782973b9d11e80511f932 \
+    --hash=sha256:bd4bacd62aa2f1a1627352fe68885d6ee694bdaebb16038b6e680f2924a9b2cc \
+    --hash=sha256:bf0b4b8d9caa8d64df838e0f8dcf68fb570c5733b726d1494b87f3da85db3a2d \
+    --hash=sha256:c379cdd3efc0658e652a14112d51a7668f6bfca7445c5a10dee7eabecabba19d \
+    --hash=sha256:c58536f6892559e030e6924896a44098bc1290663ea12532c78cef71d0df8493 \
+    --hash=sha256:cbe6581fcff7c8e262eb574244f81f5faaea539e712a058e6707a9d272fe5b64 \
+    --hash=sha256:ced268e82af993d7801a9db2dbc1d2322e786c5dc76295d8e89473d46c6b84d4 \
+    --hash=sha256:cf3539007202ebfe03923128fedfdd245db5860a36810136ad95a564a2fdffff \
+    --hash=sha256:cf62d17310f34084c59c01e027259076479128d11e4661bb6c9acb38c5e19bb8 \
+    --hash=sha256:d0194d654e360b3e6cc9b774e83235bae6b9b2cac3be09040880bb0e8a88f4a1 \
+    --hash=sha256:d3d117890b6eee85887b1eed41eefe2e598ad6e40523d9f94c4c4b213258e4a4 \
+    --hash=sha256:db2de4e546f0ec4b2787d625e0b16b78e99c3e21bc1722b4977c0dddf11ca84e \
+    --hash=sha256:e768d870801f68c74c2b669fc909839660180c366501d4cc4b87efd6b0eee375 \
+    --hash=sha256:e7c211f25777746d468d76f11719e64acb40eed410d81c26cefac641975beb88 \
+    --hash=sha256:eed462b4541c540d63ab57b3fc69e7d8c84d5957668854ee4e408b50e92ce26a \
+    --hash=sha256:f0bfe42523893c188e9616d853c47685e1c575fe25f737adf473d0405dcfa7eb \
+    --hash=sha256:f609ebcb0242d84b7adeee2b06c11a2ddaec5464d21888b2c8255f5fd6a98ae4 \
+    --hash=sha256:fea9d3ca80bcf17edb2c08a4704259dadac196fe5e9274067e7a20511fad1743 \
+    --hash=sha256:fed7a72d54bd52f4aeb6c6e951f363903bd7d70bc1cad64dd1f087980d309ab9
 exceptiongroup==1.2.1 ; python_full_version >= "3.9.0" and python_version < "3.11" \
     --hash=sha256:5258b9ed329c5bbdd31a309f53cbfb0b155341807f6ff7606a1e801a891b29ad \
     --hash=sha256:a4785e48b045528f5bfe627b6ad554ff32def154f42372786903b7abcfe1aa16
 execnet==2.1.1 ; python_full_version >= "3.9.0" and python_version < "3.13" \
     --hash=sha256:26dee51f1b80cebd6d0ca8e74dd8745419761d3bef34163928cbebbdc4749fdc \
     --hash=sha256:5189b52c6121c24feae288166ab41b32549c7e2348652736540b9e6e7d4e72e3
 idna==3.7 ; python_full_version >= "3.9.0" and python_version < "3.13" \
@@ -151,20 +151,20 @@
     --hash=sha256:5837b58e9f6ebd335b0f8060eecce69b662415b16dc503883a02f45dfeb14857
 pytest-sugar==1.0.0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
     --hash=sha256:6422e83258f5b0c04ce7c632176c7732cab5fdb909cb39cca5c9139f81276c0a \
     --hash=sha256:70ebcd8fc5795dc457ff8b69d266a4e2e8a74ae0c3edc749381c64b5246c8dfd
 pytest-timeout==2.3.1 ; python_full_version >= "3.9.0" and python_version < "3.13" \
     --hash=sha256:12397729125c6ecbdaca01035b9e5239d4db97352320af155b3f5de1ba5165d9 \
     --hash=sha256:68188cb703edfc6a18fad98dc25a3c61e9f24d644b0b70f33af545219fc7813e
-pytest-xdist==3.5.0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:cbb36f3d67e0c478baa57fa4edc8843887e0f6cfc42d677530a36d7472b32d8a \
-    --hash=sha256:d075629c7e00b611df89f490a5063944bee7a4362a5ff11c7cc7824a03dfce24
-pytest==8.1.1 ; python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:2a8386cfc11fa9d2c50ee7b2a57e7d898ef90470a7a34c4b949ff59662bb78b7 \
-    --hash=sha256:ac978141a75948948817d360297b7aae0fcb9d6ff6bc9ec6d514b85d5a65c044
+pytest-xdist==3.6.1 ; python_full_version >= "3.9.0" and python_version < "3.13" \
+    --hash=sha256:9ed4adfb68a016610848639bb7e02c9352d5d9f03d04809919e2dafc3be4cca7 \
+    --hash=sha256:ead156a4db231eec769737f57668ef58a2084a34b2e55c4a8fa20d861107300d
+pytest==8.2.0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
+    --hash=sha256:1733f0620f6cda4095bbf0d9ff8022486e91892245bb9e7d5542c018f612f233 \
+    --hash=sha256:d507d4482197eac0ba2bae2e9babf0672eb333017bcedaa5fb1a3d42c1174b3f
 sniffio==1.3.1 ; python_full_version >= "3.9.0" and python_version < "3.13" \
     --hash=sha256:2f6da418d1f1e0fddd844478f41680e794e6051915791a034ff65e5f100525a2 \
     --hash=sha256:f4324edc670a0f49750a81b895f35c3adb843cca46f0530f79fc1babb23789dc
 sortedcontainers==2.4.0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
     --hash=sha256:25caa5a06cc30b6b83d11423433f65d1f9d76c4c6a0c90e3379eaa43b9bfdb88 \
     --hash=sha256:a163dcaede0f1c021485e957a39245190e74249897e2ae4b2aa38595db237ee0
 termcolor==2.4.0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
```

### Comparing `alluka-0.1.5/dev-requirements/type-checking.txt` & `alluka-0.2.0/piped/python/base-requirements/docs.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,159 +1,144 @@
 #
 # This file is autogenerated by pip-compile-cross-platform
 # To update, run:
 #
-#    pip-compile-cross-platform dev-requirements/type-checking.in --output-file dev-requirements/type-checking.txt --min-python-version 3.9.0,<3.13
+#    pip-compile-cross-platform python/base-requirements/docs.in --output-file python/base-requirements/docs.txt --min-python-version 3.9
 #
-annotated-types==0.6.0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:0641064de18ba7a25dee8f96403ebc39113d0cb953a01429249d5c7564666a43 \
-    --hash=sha256:563339e807e53ffd9c267e99fc6d9ea23eb8443c08f112651963e24e22f84a5d
-anyio==4.3.0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:048e05d0f6caeed70d731f3db756d35dcc1f35747c8c403364a8332c630441b8 \
-    --hash=sha256:f75253795a87df48568485fd18cdd2a3fa5c4f7c5be8e5e36637733fce06fed6
-argcomplete==3.3.0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:c168c3723482c031df3c207d4ba8fa702717ccb9fc0bfe4117166c1f537b4a54 \
-    --hash=sha256:fd03ff4a5b9e6580569d34b273f741e85cd9e072f3feeeee3eba4891c70eda62
-attrs==23.2.0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:935dc3b529c262f6cf76e50877d35a4bd3c1de194fd41f47a2b7ae8f19971f30 \
-    --hash=sha256:99b87a485a5820b23b879f04c2305b44b951b502fd64be915879d77a7e8fc6f1
-cffi==1.16.0 ; os_name == "nt" and implementation_name != "pypy" and python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:0c9ef6ff37e974b73c25eecc13952c55bceed9112be2d9d938ded8e856138bcc \
-    --hash=sha256:131fd094d1065b19540c3d72594260f118b231090295d8c34e19a7bbcf2e860a \
-    --hash=sha256:1b8ebc27c014c59692bb2664c7d13ce7a6e9a629be20e54e7271fa696ff2b417 \
-    --hash=sha256:2c56b361916f390cd758a57f2e16233eb4f64bcbeee88a4881ea90fca14dc6ab \
-    --hash=sha256:2d92b25dbf6cae33f65005baf472d2c245c050b1ce709cc4588cdcdd5495b520 \
-    --hash=sha256:31d13b0f99e0836b7ff893d37af07366ebc90b678b6664c955b54561fc36ef36 \
-    --hash=sha256:32c68ef735dbe5857c810328cb2481e24722a59a2003018885514d4c09af9743 \
-    --hash=sha256:3686dffb02459559c74dd3d81748269ffb0eb027c39a6fc99502de37d501faa8 \
-    --hash=sha256:582215a0e9adbe0e379761260553ba11c58943e4bbe9c36430c4ca6ac74b15ed \
-    --hash=sha256:5b50bf3f55561dac5438f8e70bfcdfd74543fd60df5fa5f62d94e5867deca684 \
-    --hash=sha256:5bf44d66cdf9e893637896c7faa22298baebcd18d1ddb6d2626a6e39793a1d56 \
-    --hash=sha256:6602bc8dc6f3a9e02b6c22c4fc1e47aa50f8f8e6d3f78a5e16ac33ef5fefa324 \
-    --hash=sha256:673739cb539f8cdaa07d92d02efa93c9ccf87e345b9a0b556e3ecc666718468d \
-    --hash=sha256:68678abf380b42ce21a5f2abde8efee05c114c2fdb2e9eef2efdb0257fba1235 \
-    --hash=sha256:68e7c44931cc171c54ccb702482e9fc723192e88d25a0e133edd7aff8fcd1f6e \
-    --hash=sha256:6b3d6606d369fc1da4fd8c357d026317fbb9c9b75d36dc16e90e84c26854b088 \
-    --hash=sha256:748dcd1e3d3d7cd5443ef03ce8685043294ad6bd7c02a38d1bd367cfd968e000 \
-    --hash=sha256:7651c50c8c5ef7bdb41108b7b8c5a83013bfaa8a935590c5d74627c047a583c7 \
-    --hash=sha256:7b78010e7b97fef4bee1e896df8a4bbb6712b7f05b7ef630f9d1da00f6444d2e \
-    --hash=sha256:7e61e3e4fa664a8588aa25c883eab612a188c725755afff6289454d6362b9673 \
-    --hash=sha256:80876338e19c951fdfed6198e70bc88f1c9758b94578d5a7c4c91a87af3cf31c \
-    --hash=sha256:8895613bcc094d4a1b2dbe179d88d7fb4a15cee43c052e8885783fac397d91fe \
-    --hash=sha256:88e2b3c14bdb32e440be531ade29d3c50a1a59cd4e51b1dd8b0865c54ea5d2e2 \
-    --hash=sha256:8f8e709127c6c77446a8c0a8c8bf3c8ee706a06cd44b1e827c3e6a2ee6b8c098 \
-    --hash=sha256:9cb4a35b3642fc5c005a6755a5d17c6c8b6bcb6981baf81cea8bfbc8903e8ba8 \
-    --hash=sha256:9f90389693731ff1f659e55c7d1640e2ec43ff725cc61b04b2f9c6d8d017df6a \
-    --hash=sha256:a09582f178759ee8128d9270cd1344154fd473bb77d94ce0aeb2a93ebf0feaf0 \
-    --hash=sha256:a6a14b17d7e17fa0d207ac08642c8820f84f25ce17a442fd15e27ea18d67c59b \
-    --hash=sha256:a72e8961a86d19bdb45851d8f1f08b041ea37d2bd8d4fd19903bc3083d80c896 \
-    --hash=sha256:abd808f9c129ba2beda4cfc53bde801e5bcf9d6e0f22f095e45327c038bfe68e \
-    --hash=sha256:ac0f5edd2360eea2f1daa9e26a41db02dd4b0451b48f7c318e217ee092a213e9 \
-    --hash=sha256:b29ebffcf550f9da55bec9e02ad430c992a87e5f512cd63388abb76f1036d8d2 \
-    --hash=sha256:b2ca4e77f9f47c55c194982e10f058db063937845bb2b7a86c84a6cfe0aefa8b \
-    --hash=sha256:b7be2d771cdba2942e13215c4e340bfd76398e9227ad10402a8767ab1865d2e6 \
-    --hash=sha256:b84834d0cf97e7d27dd5b7f3aca7b6e9263c56308ab9dc8aae9784abb774d404 \
-    --hash=sha256:b86851a328eedc692acf81fb05444bdf1891747c25af7529e39ddafaf68a4f3f \
-    --hash=sha256:bcb3ef43e58665bbda2fb198698fcae6776483e0c4a631aa5647806c25e02cc0 \
-    --hash=sha256:c0f31130ebc2d37cdd8e44605fb5fa7ad59049298b3f745c74fa74c62fbfcfc4 \
-    --hash=sha256:c6a164aa47843fb1b01e941d385aab7215563bb8816d80ff3a363a9f8448a8dc \
-    --hash=sha256:d8a9d3ebe49f084ad71f9269834ceccbf398253c9fac910c4fd7053ff1386936 \
-    --hash=sha256:db8e577c19c0fda0beb7e0d4e09e0ba74b1e4c092e0e40bfa12fe05b6f6d75ba \
-    --hash=sha256:dc9b18bf40cc75f66f40a7379f6a9513244fe33c0e8aa72e2d56b0196a7ef872 \
-    --hash=sha256:e09f3ff613345df5e8c3667da1d918f9149bd623cd9070c983c013792a9a62eb \
-    --hash=sha256:e4108df7fe9b707191e55f33efbcb2d81928e10cea45527879a4749cbe472614 \
-    --hash=sha256:e6024675e67af929088fda399b2094574609396b1decb609c55fa58b028a32a1 \
-    --hash=sha256:e70f54f1796669ef691ca07d046cd81a29cb4deb1e5f942003f401c0c4a2695d \
-    --hash=sha256:e715596e683d2ce000574bae5d07bd522c781a822866c20495e52520564f0969 \
-    --hash=sha256:e760191dd42581e023a68b758769e2da259b5d52e3103c6060ddc02c9edb8d7b \
-    --hash=sha256:ed86a35631f7bfbb28e108dd96773b9d5a6ce4811cf6ea468bb6a359b256b1e4 \
-    --hash=sha256:ee07e47c12890ef248766a6e55bd38ebfb2bb8edd4142d56db91b21ea68b7627 \
-    --hash=sha256:fa3a0128b152627161ce47201262d3140edb5a5c3da88d73a1b790a959126956 \
-    --hash=sha256:fcc8eb6d5902bb1cf6dc4f187ee3ea80a1eba0a89aba40a5cb20a5087d961357
-colorama==0.4.6 ; python_full_version >= "3.9.0" and python_version < "3.13" and sys_platform == "win32" \
+babel==2.14.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:6919867db036398ba21eb5c7a0f6b28ab8cbc3ae7a73a44ebe34ae74a4e7d363 \
+    --hash=sha256:efb1a25b7118e67ce3a259bed20545c29cb68be8ad2c784c83689981b7a57287
+certifi==2024.2.2 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:0569859f95fc761b18b45ef421b1290a0f65f147e92a1e5eb3e635f9a5e4e66f \
+    --hash=sha256:dc383c07b76109f368f6106eee2b593b04a011ea4d55f652c6ca24a754d1cdd1
+charset-normalizer==3.3.2 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:06435b539f889b1f6f4ac1758871aae42dc3a8c0e24ac9e60c2384973ad73027 \
+    --hash=sha256:06a81e93cd441c56a9b65d8e1d043daeb97a3d0856d177d5c90ba85acb3db087 \
+    --hash=sha256:0a55554a2fa0d408816b3b5cedf0045f4b8e1a6065aec45849de2d6f3f8e9786 \
+    --hash=sha256:0b2b64d2bb6d3fb9112bafa732def486049e63de9618b5843bcdd081d8144cd8 \
+    --hash=sha256:10955842570876604d404661fbccbc9c7e684caf432c09c715ec38fbae45ae09 \
+    --hash=sha256:122c7fa62b130ed55f8f285bfd56d5f4b4a5b503609d181f9ad85e55c89f4185 \
+    --hash=sha256:1ceae2f17a9c33cb48e3263960dc5fc8005351ee19db217e9b1bb15d28c02574 \
+    --hash=sha256:1d3193f4a680c64b4b6a9115943538edb896edc190f0b222e73761716519268e \
+    --hash=sha256:1f79682fbe303db92bc2b1136016a38a42e835d932bab5b3b1bfcfbf0640e519 \
+    --hash=sha256:2127566c664442652f024c837091890cb1942c30937add288223dc895793f898 \
+    --hash=sha256:22afcb9f253dac0696b5a4be4a1c0f8762f8239e21b99680099abd9b2b1b2269 \
+    --hash=sha256:25baf083bf6f6b341f4121c2f3c548875ee6f5339300e08be3f2b2ba1721cdd3 \
+    --hash=sha256:2e81c7b9c8979ce92ed306c249d46894776a909505d8f5a4ba55b14206e3222f \
+    --hash=sha256:3287761bc4ee9e33561a7e058c72ac0938c4f57fe49a09eae428fd88aafe7bb6 \
+    --hash=sha256:34d1c8da1e78d2e001f363791c98a272bb734000fcef47a491c1e3b0505657a8 \
+    --hash=sha256:37e55c8e51c236f95b033f6fb391d7d7970ba5fe7ff453dad675e88cf303377a \
+    --hash=sha256:3d47fa203a7bd9c5b6cee4736ee84ca03b8ef23193c0d1ca99b5089f72645c73 \
+    --hash=sha256:3e4d1f6587322d2788836a99c69062fbb091331ec940e02d12d179c1d53e25fc \
+    --hash=sha256:42cb296636fcc8b0644486d15c12376cb9fa75443e00fb25de0b8602e64c1714 \
+    --hash=sha256:45485e01ff4d3630ec0d9617310448a8702f70e9c01906b0d0118bdf9d124cf2 \
+    --hash=sha256:4a78b2b446bd7c934f5dcedc588903fb2f5eec172f3d29e52a9096a43722adfc \
+    --hash=sha256:4ab2fe47fae9e0f9dee8c04187ce5d09f48eabe611be8259444906793ab7cbce \
+    --hash=sha256:4d0d1650369165a14e14e1e47b372cfcb31d6ab44e6e33cb2d4e57265290044d \
+    --hash=sha256:549a3a73da901d5bc3ce8d24e0600d1fa85524c10287f6004fbab87672bf3e1e \
+    --hash=sha256:55086ee1064215781fff39a1af09518bc9255b50d6333f2e4c74ca09fac6a8f6 \
+    --hash=sha256:572c3763a264ba47b3cf708a44ce965d98555f618ca42c926a9c1616d8f34269 \
+    --hash=sha256:573f6eac48f4769d667c4442081b1794f52919e7edada77495aaed9236d13a96 \
+    --hash=sha256:5b4c145409bef602a690e7cfad0a15a55c13320ff7a3ad7ca59c13bb8ba4d45d \
+    --hash=sha256:6463effa3186ea09411d50efc7d85360b38d5f09b870c48e4600f63af490e56a \
+    --hash=sha256:65f6f63034100ead094b8744b3b97965785388f308a64cf8d7c34f2f2e5be0c4 \
+    --hash=sha256:663946639d296df6a2bb2aa51b60a2454ca1cb29835324c640dafb5ff2131a77 \
+    --hash=sha256:6897af51655e3691ff853668779c7bad41579facacf5fd7253b0133308cf000d \
+    --hash=sha256:68d1f8a9e9e37c1223b656399be5d6b448dea850bed7d0f87a8311f1ff3dabb0 \
+    --hash=sha256:6ac7ffc7ad6d040517be39eb591cac5ff87416c2537df6ba3cba3bae290c0fed \
+    --hash=sha256:6b3251890fff30ee142c44144871185dbe13b11bab478a88887a639655be1068 \
+    --hash=sha256:6c4caeef8fa63d06bd437cd4bdcf3ffefe6738fb1b25951440d80dc7df8c03ac \
+    --hash=sha256:6ef1d82a3af9d3eecdba2321dc1b3c238245d890843e040e41e470ffa64c3e25 \
+    --hash=sha256:753f10e867343b4511128c6ed8c82f7bec3bd026875576dfd88483c5c73b2fd8 \
+    --hash=sha256:7cd13a2e3ddeed6913a65e66e94b51d80a041145a026c27e6bb76c31a853c6ab \
+    --hash=sha256:7ed9e526742851e8d5cc9e6cf41427dfc6068d4f5a3bb03659444b4cabf6bc26 \
+    --hash=sha256:7f04c839ed0b6b98b1a7501a002144b76c18fb1c1850c8b98d458ac269e26ed2 \
+    --hash=sha256:802fe99cca7457642125a8a88a084cef28ff0cf9407060f7b93dca5aa25480db \
+    --hash=sha256:80402cd6ee291dcb72644d6eac93785fe2c8b9cb30893c1af5b8fdd753b9d40f \
+    --hash=sha256:8465322196c8b4d7ab6d1e049e4c5cb460d0394da4a27d23cc242fbf0034b6b5 \
+    --hash=sha256:86216b5cee4b06df986d214f664305142d9c76df9b6512be2738aa72a2048f99 \
+    --hash=sha256:87d1351268731db79e0f8e745d92493ee2841c974128ef629dc518b937d9194c \
+    --hash=sha256:8bdb58ff7ba23002a4c5808d608e4e6c687175724f54a5dade5fa8c67b604e4d \
+    --hash=sha256:8c622a5fe39a48f78944a87d4fb8a53ee07344641b0562c540d840748571b811 \
+    --hash=sha256:8d756e44e94489e49571086ef83b2bb8ce311e730092d2c34ca8f7d925cb20aa \
+    --hash=sha256:8f4a014bc36d3c57402e2977dada34f9c12300af536839dc38c0beab8878f38a \
+    --hash=sha256:9063e24fdb1e498ab71cb7419e24622516c4a04476b17a2dab57e8baa30d6e03 \
+    --hash=sha256:90d558489962fd4918143277a773316e56c72da56ec7aa3dc3dbbe20fdfed15b \
+    --hash=sha256:923c0c831b7cfcb071580d3f46c4baf50f174be571576556269530f4bbd79d04 \
+    --hash=sha256:95f2a5796329323b8f0512e09dbb7a1860c46a39da62ecb2324f116fa8fdc85c \
+    --hash=sha256:96b02a3dc4381e5494fad39be677abcb5e6634bf7b4fa83a6dd3112607547001 \
+    --hash=sha256:9f96df6923e21816da7e0ad3fd47dd8f94b2a5ce594e00677c0013018b813458 \
+    --hash=sha256:a10af20b82360ab00827f916a6058451b723b4e65030c5a18577c8b2de5b3389 \
+    --hash=sha256:a50aebfa173e157099939b17f18600f72f84eed3049e743b68ad15bd69b6bf99 \
+    --hash=sha256:a981a536974bbc7a512cf44ed14938cf01030a99e9b3a06dd59578882f06f985 \
+    --hash=sha256:a9a8e9031d613fd2009c182b69c7b2c1ef8239a0efb1df3f7c8da66d5dd3d537 \
+    --hash=sha256:ae5f4161f18c61806f411a13b0310bea87f987c7d2ecdbdaad0e94eb2e404238 \
+    --hash=sha256:aed38f6e4fb3f5d6bf81bfa990a07806be9d83cf7bacef998ab1a9bd660a581f \
+    --hash=sha256:b01b88d45a6fcb69667cd6d2f7a9aeb4bf53760d7fc536bf679ec94fe9f3ff3d \
+    --hash=sha256:b261ccdec7821281dade748d088bb6e9b69e6d15b30652b74cbbac25e280b796 \
+    --hash=sha256:b2b0a0c0517616b6869869f8c581d4eb2dd83a4d79e0ebcb7d373ef9956aeb0a \
+    --hash=sha256:b4a23f61ce87adf89be746c8a8974fe1c823c891d8f86eb218bb957c924bb143 \
+    --hash=sha256:bd8f7df7d12c2db9fab40bdd87a7c09b1530128315d047a086fa3ae3435cb3a8 \
+    --hash=sha256:beb58fe5cdb101e3a055192ac291b7a21e3b7ef4f67fa1d74e331a7f2124341c \
+    --hash=sha256:c002b4ffc0be611f0d9da932eb0f704fe2602a9a949d1f738e4c34c75b0863d5 \
+    --hash=sha256:c083af607d2515612056a31f0a8d9e0fcb5876b7bfc0abad3ecd275bc4ebc2d5 \
+    --hash=sha256:c180f51afb394e165eafe4ac2936a14bee3eb10debc9d9e4db8958fe36afe711 \
+    --hash=sha256:c235ebd9baae02f1b77bcea61bce332cb4331dc3617d254df3323aa01ab47bd4 \
+    --hash=sha256:cd70574b12bb8a4d2aaa0094515df2463cb429d8536cfb6c7ce983246983e5a6 \
+    --hash=sha256:d0eccceffcb53201b5bfebb52600a5fb483a20b61da9dbc885f8b103cbe7598c \
+    --hash=sha256:d965bba47ddeec8cd560687584e88cf699fd28f192ceb452d1d7ee807c5597b7 \
+    --hash=sha256:db364eca23f876da6f9e16c9da0df51aa4f104a972735574842618b8c6d999d4 \
+    --hash=sha256:ddbb2551d7e0102e7252db79ba445cdab71b26640817ab1e3e3648dad515003b \
+    --hash=sha256:deb6be0ac38ece9ba87dea880e438f25ca3eddfac8b002a2ec3d9183a454e8ae \
+    --hash=sha256:e06ed3eb3218bc64786f7db41917d4e686cc4856944f53d5bdf83a6884432e12 \
+    --hash=sha256:e27ad930a842b4c5eb8ac0016b0a54f5aebbe679340c26101df33424142c143c \
+    --hash=sha256:e537484df0d8f426ce2afb2d0f8e1c3d0b114b83f8850e5f2fbea0e797bd82ae \
+    --hash=sha256:eb00ed941194665c332bf8e078baf037d6c35d7c4f3102ea2d4f16ca94a26dc8 \
+    --hash=sha256:eb6904c354526e758fda7167b33005998fb68c46fbc10e013ca97f21ca5c8887 \
+    --hash=sha256:eb8821e09e916165e160797a6c17edda0679379a4be5c716c260e836e122f54b \
+    --hash=sha256:efcb3f6676480691518c177e3b465bcddf57cea040302f9f4e6e191af91174d4 \
+    --hash=sha256:f27273b60488abe721a075bcca6d7f3964f9f6f067c8c4c605743023d7d3944f \
+    --hash=sha256:f30c3cb33b24454a82faecaf01b19c18562b1e89558fb6c56de4d9118a032fd5 \
+    --hash=sha256:fb69256e180cb6c8a894fee62b3afebae785babc1ee98b81cdf68bbca1987f33 \
+    --hash=sha256:fd1abc0d89e30cc4e02e4064dc67fcc51bd941eb395c502aac3ec19fab46b519 \
+    --hash=sha256:ff8fa367d09b717b2a17a052544193ad76cd49979c805768879cb63d9ca50561
+click==8.1.7 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:ae74fb96c20a0277a1d615f1e4d73c8414f5a98db8b799a7931d1582f3390c28 \
+    --hash=sha256:ca9853ad459e787e2192211578cc907e7594e294c7ccc834310722b41b9ca6de
+colorama==0.4.6 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44 \
     --hash=sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6
-colorlog==6.8.2 ; python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:3e3e079a41feb5a1b64f978b5ea4f46040a94f11f0e8bbb8261e3dbbeca64d44 \
-    --hash=sha256:4dcbb62368e2800cb3c5abd348da7e53f6c362dda502ec27c560b2e58a66bd33
-coverage[toml]==7.4.4 ; python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:00838a35b882694afda09f85e469c96367daa3f3f2b097d846a7216993d37f4c \
-    --hash=sha256:0513b9508b93da4e1716744ef6ebc507aff016ba115ffe8ecff744d1322a7b63 \
-    --hash=sha256:09c3255458533cb76ef55da8cc49ffab9e33f083739c8bd4f58e79fecfe288f7 \
-    --hash=sha256:09ef9199ed6653989ebbcaacc9b62b514bb63ea2f90256e71fea3ed74bd8ff6f \
-    --hash=sha256:09fa497a8ab37784fbb20ab699c246053ac294d13fc7eb40ec007a5043ec91f8 \
-    --hash=sha256:0f9f50e7ef2a71e2fae92774c99170eb8304e3fdf9c8c3c7ae9bab3e7229c5cf \
-    --hash=sha256:137eb07173141545e07403cca94ab625cc1cc6bc4c1e97b6e3846270e7e1fea0 \
-    --hash=sha256:1f384c3cc76aeedce208643697fb3e8437604b512255de6d18dae3f27655a384 \
-    --hash=sha256:201bef2eea65e0e9c56343115ba3814e896afe6d36ffd37bab783261db430f76 \
-    --hash=sha256:38dd60d7bf242c4ed5b38e094baf6401faa114fc09e9e6632374388a404f98e7 \
-    --hash=sha256:3b799445b9f7ee8bf299cfaed6f5b226c0037b74886a4e11515e569b36fe310d \
-    --hash=sha256:3ea79bb50e805cd6ac058dfa3b5c8f6c040cb87fe83de10845857f5535d1db70 \
-    --hash=sha256:40209e141059b9370a2657c9b15607815359ab3ef9918f0196b6fccce8d3230f \
-    --hash=sha256:41c9c5f3de16b903b610d09650e5e27adbfa7f500302718c9ffd1c12cf9d6818 \
-    --hash=sha256:54eb8d1bf7cacfbf2a3186019bcf01d11c666bd495ed18717162f7eb1e9dd00b \
-    --hash=sha256:598825b51b81c808cb6f078dcb972f96af96b078faa47af7dfcdf282835baa8d \
-    --hash=sha256:5fc1de20b2d4a061b3df27ab9b7c7111e9a710f10dc2b84d33a4ab25065994ec \
-    --hash=sha256:623512f8ba53c422fcfb2ce68362c97945095b864cda94a92edbaf5994201083 \
-    --hash=sha256:690db6517f09336559dc0b5f55342df62370a48f5469fabf502db2c6d1cffcd2 \
-    --hash=sha256:69eb372f7e2ece89f14751fbcbe470295d73ed41ecd37ca36ed2eb47512a6ab9 \
-    --hash=sha256:73bfb9c09951125d06ee473bed216e2c3742f530fc5acc1383883125de76d9cd \
-    --hash=sha256:742a76a12aa45b44d236815d282b03cfb1de3b4323f3e4ec933acfae08e54ade \
-    --hash=sha256:7c95949560050d04d46b919301826525597f07b33beba6187d04fa64d47ac82e \
-    --hash=sha256:8130a2aa2acb8788e0b56938786c33c7c98562697bf9f4c7d6e8e5e3a0501e4a \
-    --hash=sha256:8a2b2b78c78293782fd3767d53e6474582f62443d0504b1554370bde86cc8227 \
-    --hash=sha256:8ce1415194b4a6bd0cdcc3a1dfbf58b63f910dcb7330fe15bdff542c56949f87 \
-    --hash=sha256:9ca28a302acb19b6af89e90f33ee3e1906961f94b54ea37de6737b7ca9d8827c \
-    --hash=sha256:a4cdc86d54b5da0df6d3d3a2f0b710949286094c3a6700c21e9015932b81447e \
-    --hash=sha256:aa5b1c1bfc28384f1f53b69a023d789f72b2e0ab1b3787aae16992a7ca21056c \
-    --hash=sha256:aadacf9a2f407a4688d700e4ebab33a7e2e408f2ca04dbf4aef17585389eff3e \
-    --hash=sha256:ae71e7ddb7a413dd60052e90528f2f65270aad4b509563af6d03d53e979feafd \
-    --hash=sha256:b14706df8b2de49869ae03a5ccbc211f4041750cd4a66f698df89d44f4bd30ec \
-    --hash=sha256:b1a93009cb80730c9bca5d6d4665494b725b6e8e157c1cb7f2db5b4b122ea562 \
-    --hash=sha256:b2991665420a803495e0b90a79233c1433d6ed77ef282e8e152a324bbbc5e0c8 \
-    --hash=sha256:b2c5edc4ac10a7ef6605a966c58929ec6c1bd0917fb8c15cb3363f65aa40e677 \
-    --hash=sha256:b4d33f418f46362995f1e9d4f3a35a1b6322cb959c31d88ae56b0298e1c22357 \
-    --hash=sha256:b91cbc4b195444e7e258ba27ac33769c41b94967919f10037e6355e998af255c \
-    --hash=sha256:c74880fc64d4958159fbd537a091d2a585448a8f8508bf248d72112723974cbd \
-    --hash=sha256:c901df83d097649e257e803be22592aedfd5182f07b3cc87d640bbb9afd50f49 \
-    --hash=sha256:cac99918c7bba15302a2d81f0312c08054a3359eaa1929c7e4b26ebe41e9b286 \
-    --hash=sha256:cc4f1358cb0c78edef3ed237ef2c86056206bb8d9140e73b6b89fbcfcbdd40e1 \
-    --hash=sha256:ccd341521be3d1b3daeb41960ae94a5e87abe2f46f17224ba5d6f2b8398016cf \
-    --hash=sha256:ce4b94265ca988c3f8e479e741693d143026632672e3ff924f25fab50518dd51 \
-    --hash=sha256:cf271892d13e43bc2b51e6908ec9a6a5094a4df1d8af0bfc360088ee6c684409 \
-    --hash=sha256:d5ae728ff3b5401cc320d792866987e7e7e880e6ebd24433b70a33b643bb0384 \
-    --hash=sha256:d71eec7d83298f1af3326ce0ff1d0ea83c7cb98f72b577097f9083b20bdaf05e \
-    --hash=sha256:d898fe162d26929b5960e4e138651f7427048e72c853607f2b200909794ed978 \
-    --hash=sha256:d89d7b2974cae412400e88f35d86af72208e1ede1a541954af5d944a8ba46c57 \
-    --hash=sha256:dfa8fe35a0bb90382837b238fff375de15f0dcdb9ae68ff85f7a63649c98527e \
-    --hash=sha256:e0be5efd5127542ef31f165de269f77560d6cdef525fffa446de6f7e9186cfb2 \
-    --hash=sha256:fdfafb32984684eb03c2d83e1e51f64f0906b11e64482df3c5db936ce3839d48 \
-    --hash=sha256:ff7687ca3d7028d8a5f0ebae95a6e4827c5616b31a4ee1192bdfde697db110d4
-distlib==0.3.8 ; python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:034db59a0b96f8ca18035f36290806a9a6e6bd9d1ff91e45a7f172eb17e51784 \
-    --hash=sha256:1530ea13e350031b6312d8580ddb6b27a104275a31106523b8f123787f494f64
-exceptiongroup==1.2.1 ; python_full_version >= "3.9.0" and python_version < "3.11" \
-    --hash=sha256:5258b9ed329c5bbdd31a309f53cbfb0b155341807f6ff7606a1e801a891b29ad \
-    --hash=sha256:a4785e48b045528f5bfe627b6ad554ff32def154f42372786903b7abcfe1aa16
-execnet==2.1.1 ; python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:26dee51f1b80cebd6d0ca8e74dd8745419761d3bef34163928cbebbdc4749fdc \
-    --hash=sha256:5189b52c6121c24feae288166ab41b32549c7e2348652736540b9e6e7d4e72e3
-filelock==3.13.4 ; python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:404e5e9253aa60ad457cae1be07c0f0ca90a63931200a47d9b6a6af84fd7b45f \
-    --hash=sha256:d13f466618bfde72bd2c18255e269f72542c6e70e7bac83a0232d6b1cc5c8cf4
-idna==3.7 ; python_full_version >= "3.9.0" and python_version < "3.13" \
+csscompressor==0.9.5 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:afa22badbcf3120a4f392e4d22f9fff485c044a1feda4a950ecc5eba9dd31a05
+ghp-import==2.1.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:8337dd7b50877f163d4c0289bc1f1c7f127550241988d568c1db512c4324a619 \
+    --hash=sha256:9c535c4c61193c2df8871222567d7fd7e5014d835f97dc7b7439069e2413d343
+griffe==0.44.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:34aee1571042f9bf00529bc715de4516fb6f482b164e90d030300601009e0223 \
+    --hash=sha256:8a4471c469ba980b87c843f1168850ce39d0c1d0c7be140dca2480f76c8e5446
+htmlmin2==0.1.13 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:75609f2a42e64f7ce57dbff28a39890363bde9e7e5885db633317efbdf8c79a2
+idna==3.7 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:028ff3aadf0609c1fd278d8ea3089299412a7a8b9bd005dd08b9f8285bcb5cfc \
     --hash=sha256:82fee1fc78add43492d3a1898bfa6d8a904cc97d8427f683ed8e798d07761aa0
-iniconfig==2.0.0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3 \
-    --hash=sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374
-jinja2==3.1.3 ; python_full_version >= "3.9.0" and python_version < "3.13" \
+importlib-metadata==7.1.0 ; python_version >= "3.9" and python_version < "3.10" \
+    --hash=sha256:30962b96c0c223483ed6cc7280e7f0199feb01a0e40cfae4d4450fc6fab1f570 \
+    --hash=sha256:b78938b926ee8d5f020fc4772d487045805a55ddbad2ecf21c6d60938dc7fcd2
+jinja2==3.1.3 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:7d6d50dd97d52cbc355597bd845fabfbac3f551e1f99619e39a35ce8c370b5fa \
     --hash=sha256:ac8bd6544d4bb2c9792bf3a159e80bba8fda7f07e81bc3aed565432d5925ba90
-markupsafe==2.1.5 ; python_full_version >= "3.9.0" and python_version < "3.13" \
+jsmin==3.0.1 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:c0959a121ef94542e807a674142606f7e90214a2b3d1eb17300244bbb5cc2bfc
+markdown-include==0.8.1 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:1d0623e0fc2757c38d35df53752768356162284259d259c486b4ab6285cdbbe3 \
+    --hash=sha256:32f0635b9cfef46997b307e2430022852529f7a5b87c0075c504283e7cc7db53
+markdown==3.6 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:48f276f4d8cfb8ce6527c8f79e2ee29708508bf4d40aa410fbc3b4ee832c850f \
+    --hash=sha256:ed4f41f6daecbeeb96e576ce414c41d2d876daa9a16cb35fa8ed8c2ddfad0224
+markupsafe==2.1.5 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:00e046b6dd71aa03a41079792f8473dc494d564611a8f89bbbd7cb93295ebdcf \
     --hash=sha256:075202fa5b72c86ad32dc7d0b56024ebdbcf2048c0ba09f1cde31bfdd57bcfff \
     --hash=sha256:0e397ac966fdf721b2c528cf028494e86172b4feba51d65f81ffd65c63798f3f \
     --hash=sha256:17b950fccb810b3293638215058e432159d2b71005c74371d784862b7e4683f3 \
     --hash=sha256:1f3fbcb7ef1f16e48246f704ab79d79da8a46891e2da03f8783a5b6fa41a9532 \
     --hash=sha256:2174c595a0d73a3080ca3257b40096db99799265e1c27cc5a610743acd86d62f \
     --hash=sha256:2b7c57a4dfc4f16f7142221afe5ba4e093e09e728ca65c51f5620c9aaeb9a617 \
@@ -206,187 +191,248 @@
     --hash=sha256:ea3d8a3d18833cf4304cd2fc9cbb1efe188ca9b5efef2bdac7adc20594a0e46b \
     --hash=sha256:ec6a563cff360b50eed26f13adc43e61bc0c04d94b8be985e6fb24b81f6dcfdf \
     --hash=sha256:f5dfb42c4604dddc8e4305050aa6deb084540643ed5804d7455b5df8fe16f5e5 \
     --hash=sha256:fa173ec60341d6bb97a89f5ea19c85c5643c1e7dedebc22f5181eb73573142c5 \
     --hash=sha256:fa9db3f79de01457b03d4f01b34cf91bc0048eb2c3846ff26f66687c2f6d16ab \
     --hash=sha256:fce659a462a1be54d2ffcacea5e3ba2d74daa74f30f5f143fe0c58636e355fdd \
     --hash=sha256:ffee1f21e5ef0d712f9033568f8344d5da8cc2869dbd08d87c84656e6a2d2f68
-mock==5.1.0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:18c694e5ae8a208cdb3d2c20a993ca1a7b0efa258c247a1e565150f477f83744 \
-    --hash=sha256:5e96aad5ccda4718e0a229ed94b2024df75cc2d55575ba5762d31f5767b8767d
-mypy-extensions==1.0.0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d \
-    --hash=sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782
-mypy==1.9.0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:0235391f1c6f6ce487b23b9dbd1327b4ec33bb93934aa986efe8a9563d9349e6 \
-    --hash=sha256:190da1ee69b427d7efa8aa0d5e5ccd67a4fb04038c380237a0d96829cb157913 \
-    --hash=sha256:2418488264eb41f69cc64a69a745fad4a8f86649af4b1041a4c64ee61fc61129 \
-    --hash=sha256:3a3c007ff3ee90f69cf0a15cbcdf0995749569b86b6d2f327af01fd1b8aee9dc \
-    --hash=sha256:3cc5da0127e6a478cddd906068496a97a7618a21ce9b54bde5bf7e539c7af974 \
-    --hash=sha256:48533cdd345c3c2e5ef48ba3b0d3880b257b423e7995dada04248725c6f77374 \
-    --hash=sha256:49c87c15aed320de9b438ae7b00c1ac91cd393c1b854c2ce538e2a72d55df150 \
-    --hash=sha256:4d3dbd346cfec7cb98e6cbb6e0f3c23618af826316188d587d1c1bc34f0ede03 \
-    --hash=sha256:571741dc4194b4f82d344b15e8837e8c5fcc462d66d076748142327626a1b6e9 \
-    --hash=sha256:587ce887f75dd9700252a3abbc9c97bbe165a4a630597845c61279cf32dfbf02 \
-    --hash=sha256:5d741d3fc7c4da608764073089e5f58ef6352bedc223ff58f2f038c2c4698a89 \
-    --hash=sha256:5e6061f44f2313b94f920e91b204ec600982961e07a17e0f6cd83371cb23f5c2 \
-    --hash=sha256:61758fabd58ce4b0720ae1e2fea5cfd4431591d6d590b197775329264f86311d \
-    --hash=sha256:653265f9a2784db65bfca694d1edd23093ce49740b2244cde583aeb134c008f3 \
-    --hash=sha256:68edad3dc7d70f2f17ae4c6c1b9471a56138ca22722487eebacfd1eb5321d612 \
-    --hash=sha256:81a10926e5473c5fc3da8abb04119a1f5811a236dc3a38d92015cb1e6ba4cb9e \
-    --hash=sha256:85ca5fcc24f0b4aeedc1d02f93707bccc04733f21d41c88334c5482219b1ccb3 \
-    --hash=sha256:a260627a570559181a9ea5de61ac6297aa5af202f06fd7ab093ce74e7181e43e \
-    --hash=sha256:aceb1db093b04db5cd390821464504111b8ec3e351eb85afd1433490163d60cd \
-    --hash=sha256:b685154e22e4e9199fc95f298661deea28aaede5ae16ccc8cbb1045e716b3e04 \
-    --hash=sha256:d357423fa57a489e8c47b7c85dfb96698caba13d66e086b412298a1a0ea3b0ed \
-    --hash=sha256:d4d5ddc13421ba3e2e082a6c2d74c2ddb3979c39b582dacd53dd5d9431237185 \
-    --hash=sha256:e49499be624dead83927e70c756970a0bc8240e9f769389cdf5714b0784ca6bf \
-    --hash=sha256:e54396d70be04b34f31d2edf3362c1edd023246c82f1730bbf8768c28db5361b \
-    --hash=sha256:f88566144752999351725ac623471661c9d1cd8caa0134ff98cceeea181789f4 \
-    --hash=sha256:f8a67616990062232ee4c3952f41c779afac41405806042a8126fe96e098419f \
-    --hash=sha256:fe28657de3bfec596bbeef01cb219833ad9d38dd5393fc649f4b366840baefe6
-nodeenv==1.8.0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:d51e0c37e64fbf47d017feac3145cdbb58836d7eee8c6f6d3b6880c5456227d2 \
-    --hash=sha256:df865724bb3c3adc86b3876fa209771517b0cfe596beff01a92700e0e8be4cec
-nox==2024.4.15 ; python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:6492236efa15a460ecb98e7b67562a28b70da006ab0be164e8821177577c0565 \
-    --hash=sha256:ecf6700199cdfa9e5ea0a41ff5e6ef4641d09508eda6edb89d9987864115817f
-outcome==1.3.0.post0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:9dcf02e65f2971b80047b377468e72a268e15c0af3cf1238e6ff14f7f91143b8 \
-    --hash=sha256:e771c5ce06d1415e356078d3bdd68523f284b4ce5419828922b6871e65eda82b
-packaging==24.0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
+mergedeep==1.3.4 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:0096d52e9dad9939c3d975a774666af186eda617e6ca84df4c94dec30004f2a8 \
+    --hash=sha256:70775750742b25c0d8f36c55aed03d24c3384d17c951b3175d898bd778ef0307
+mkdocs-autorefs==1.0.1 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:aacdfae1ab197780fb7a2dac92ad8a3d8f7ca8049a9cbe56a4218cd52e8da570 \
+    --hash=sha256:f684edf847eced40b570b57846b15f0bf57fb93ac2c510450775dcf16accb971
+mkdocs-material-extensions==1.3.1 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:10c9511cea88f568257f960358a467d12b970e1f7b2c0e5fb2bb48cab1928443 \
+    --hash=sha256:adff8b62700b25cb77b53358dad940f3ef973dd6db797907c49e3c2ef3ab4e31
+mkdocs-material==9.5.18 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:1e0e27fc9fe239f9064318acf548771a4629d5fd5dfd45444fd80a953fe21eb4 \
+    --hash=sha256:a43f470947053fa2405c33995f282d24992c752a50114f23f30da9d8d0c57e62
+mkdocs-minify-plugin==0.8.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:5fba1a3f7bd9a2142c9954a6559a57e946587b21f133165ece30ea145c66aee6 \
+    --hash=sha256:bc11b78b8120d79e817308e2b11539d790d21445eb63df831e393f76e52e753d
+mkdocs==1.5.3 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:3b3a78e736b31158d64dbb2f8ba29bd46a379d0c6e324c2246c3bc3d2189cfc1 \
+    --hash=sha256:eb7c99214dcb945313ba30426c2451b735992c73c2e10838f76d09e39ff4d0e2
+mkdocstrings-python==1.10.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:71678fac657d4d2bb301eed4e4d2d91499c095fd1f8a90fa76422a87a5693828 \
+    --hash=sha256:ba833fbd9d178a4b9d5cb2553a4df06e51dc1f51e41559a4d2398c16a6f69ecc
+mkdocstrings==0.24.3 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:5c9cf2a32958cd161d5428699b79c8b0988856b0d4a8c5baf8395fc1bf4087c3 \
+    --hash=sha256:f327b234eb8d2551a306735436e157d0a22d45f79963c60a8b585d5f7a94c1d2
+mkdocstrings[python]==0.24.3 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:5c9cf2a32958cd161d5428699b79c8b0988856b0d4a8c5baf8395fc1bf4087c3 \
+    --hash=sha256:f327b234eb8d2551a306735436e157d0a22d45f79963c60a8b585d5f7a94c1d2
+packaging==24.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:2ddfb553fdf02fb784c234c7ba6ccc288296ceabec964ad2eae3777778130bc5 \
     --hash=sha256:eb82c5e3e56209074766e6885bb04b8c38a0c015d0a30036ebe7ece34c9989e9
-platformdirs==4.2.0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
+paginate==0.5.6 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:5e6007b6a9398177a7e1648d04fdd9f8c9766a1a945bceac82f1929e8c78af2d
+pathspec==0.12.1 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:a0d503e138a4c123b27490a4f7beda6a01c6f288df0e4a8b79c7eb0dc7b4cc08 \
+    --hash=sha256:a482d51503a1ab33b1c67a6c3813a26953dbdc71c31dacaef9a838c4e29f5712
+platformdirs==4.2.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:0614df2a2f37e1a662acbd8e2b25b92ccf8632929bc6d43467e17fe89c75e068 \
     --hash=sha256:ef0cc731df711022c174543cb70a9b5bd22e5a9337c8624ef2c2ceb8ddad8768
-pluggy==1.5.0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:2cffa88e94fdc978c4c574f15f9e59b7f4201d439195c3715ca9e2486f1d0cf1 \
-    --hash=sha256:44e1ad92c8ca002de6377e165f3e0f1be63266ab4d554740532335b9d75ea669
-pycparser==2.22 ; os_name == "nt" and implementation_name != "pypy" and python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:491c8be9c040f5390f5bf44a5b07752bd07f56edf992381b05c701439eec10f6 \
-    --hash=sha256:c3702b6d3dd8c7abc1afa565d7e63d53a1d0bd86cdc24edd75470f4de499cfcc
-pydantic-core==2.18.1 ; python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:030e4f9516f9947f38179249778709a460a3adb516bf39b5eb9066fcfe43d0e6 \
-    --hash=sha256:09f03dfc0ef8c22622eaa8608caa4a1e189cfb83ce847045eca34f690895eccb \
-    --hash=sha256:12a05db5013ec0ca4a32cc6433f53faa2a014ec364031408540ba858c2172bb0 \
-    --hash=sha256:14fe73881cf8e4cbdaded8ca0aa671635b597e42447fec7060d0868b52d074e6 \
-    --hash=sha256:1a0c3e718f4e064efde68092d9d974e39572c14e56726ecfaeebbe6544521f47 \
-    --hash=sha256:1be91ad664fc9245404a789d60cba1e91c26b1454ba136d2a1bf0c2ac0c0505a \
-    --hash=sha256:201713f2f462e5c015b343e86e68bd8a530a4f76609b33d8f0ec65d2b921712a \
-    --hash=sha256:2027493cc44c23b598cfaf200936110433d9caa84e2c6cf487a83999638a96ac \
-    --hash=sha256:250ae39445cb5475e483a36b1061af1bc233de3e9ad0f4f76a71b66231b07f88 \
-    --hash=sha256:2533ad2883f001efa72f3d0e733fb846710c3af6dcdd544fe5bf14fa5fe2d7db \
-    --hash=sha256:25595ac311f20e5324d1941909b0d12933f1fd2171075fcff763e90f43e92a0d \
-    --hash=sha256:2684a94fdfd1b146ff10689c6e4e815f6a01141781c493b97342cdc5b06f4d5d \
-    --hash=sha256:27f1009dc292f3b7ca77feb3571c537276b9aad5dd4efb471ac88a8bd09024e9 \
-    --hash=sha256:2adaeea59849ec0939af5c5d476935f2bab4b7f0335b0110f0f069a41024278e \
-    --hash=sha256:2ae80f72bb7a3e397ab37b53a2b49c62cc5496412e71bc4f1277620a7ce3f52b \
-    --hash=sha256:2d5728e93d28a3c63ee513d9ffbac9c5989de8c76e049dbcb5bfe4b923a9739d \
-    --hash=sha256:2e91711e36e229978d92642bfc3546333a9127ecebb3f2761372e096395fc649 \
-    --hash=sha256:2fe0c1ce5b129455e43f941f7a46f61f3d3861e571f2905d55cdbb8b5c6f5e2c \
-    --hash=sha256:38a5024de321d672a132b1834a66eeb7931959c59964b777e8f32dbe9523f6b1 \
-    --hash=sha256:3e352f0191d99fe617371096845070dee295444979efb8f27ad941227de6ad09 \
-    --hash=sha256:48dd883db92e92519201f2b01cafa881e5f7125666141a49ffba8b9facc072b0 \
-    --hash=sha256:54764c083bbe0264f0f746cefcded6cb08fbbaaf1ad1d78fb8a4c30cff999a90 \
-    --hash=sha256:54c7375c62190a7845091f521add19b0f026bcf6ae674bdb89f296972272e86d \
-    --hash=sha256:561cf62c8a3498406495cfc49eee086ed2bb186d08bcc65812b75fda42c38294 \
-    --hash=sha256:56823a92075780582d1ffd4489a2e61d56fd3ebb4b40b713d63f96dd92d28144 \
-    --hash=sha256:582cf2cead97c9e382a7f4d3b744cf0ef1a6e815e44d3aa81af3ad98762f5a9b \
-    --hash=sha256:58aca931bef83217fca7a390e0486ae327c4af9c3e941adb75f8772f8eeb03a1 \
-    --hash=sha256:5f7973c381283783cd1043a8c8f61ea5ce7a3a58b0369f0ee0ee975eaf2f2a1b \
-    --hash=sha256:6395a4435fa26519fd96fdccb77e9d00ddae9dd6c742309bd0b5610609ad7fb2 \
-    --hash=sha256:63d7523cd95d2fde0d28dc42968ac731b5bb1e516cc56b93a50ab293f4daeaad \
-    --hash=sha256:641a018af4fe48be57a2b3d7a1f0f5dbca07c1d00951d3d7463f0ac9dac66622 \
-    --hash=sha256:667880321e916a8920ef49f5d50e7983792cf59f3b6079f3c9dac2b88a311d17 \
-    --hash=sha256:684d840d2c9ec5de9cb397fcb3f36d5ebb6fa0d94734f9886032dd796c1ead06 \
-    --hash=sha256:68717c38a68e37af87c4da20e08f3e27d7e4212e99e96c3d875fbf3f4812abfc \
-    --hash=sha256:6b7bbb97d82659ac8b37450c60ff2e9f97e4eb0f8a8a3645a5568b9334b08b50 \
-    --hash=sha256:72722ce529a76a4637a60be18bd789d8fb871e84472490ed7ddff62d5fed620d \
-    --hash=sha256:73c1bc8a86a5c9e8721a088df234265317692d0b5cd9e86e975ce3bc3db62a59 \
-    --hash=sha256:76909849d1a6bffa5a07742294f3fa1d357dc917cb1fe7b470afbc3a7579d539 \
-    --hash=sha256:76b86e24039c35280ceee6dce7e62945eb93a5175d43689ba98360ab31eebc4a \
-    --hash=sha256:7a5d83efc109ceddb99abd2c1316298ced2adb4570410defe766851a804fcd5b \
-    --hash=sha256:80e0e57cc704a52fb1b48f16d5b2c8818da087dbee6f98d9bf19546930dc64b5 \
-    --hash=sha256:85233abb44bc18d16e72dc05bf13848a36f363f83757541f1a97db2f8d58cfd9 \
-    --hash=sha256:907a4d7720abfcb1c81619863efd47c8a85d26a257a2dbebdb87c3b847df0278 \
-    --hash=sha256:9376d83d686ec62e8b19c0ac3bf8d28d8a5981d0df290196fb6ef24d8a26f0d6 \
-    --hash=sha256:94b9769ba435b598b547c762184bcfc4783d0d4c7771b04a3b45775c3589ca44 \
-    --hash=sha256:9a29726f91c6cb390b3c2338f0df5cd3e216ad7a938762d11c994bb37552edb0 \
-    --hash=sha256:9b6431559676a1079eac0f52d6d0721fb8e3c5ba43c37bc537c8c83724031feb \
-    --hash=sha256:9ece8a49696669d483d206b4474c367852c44815fca23ac4e48b72b339807f80 \
-    --hash=sha256:a139fe9f298dc097349fb4f28c8b81cc7a202dbfba66af0e14be5cfca4ef7ce5 \
-    --hash=sha256:a32204489259786a923e02990249c65b0f17235073149d0033efcebe80095570 \
-    --hash=sha256:a3982b0a32d0a88b3907e4b0dc36809fda477f0757c59a505d4e9b455f384b8b \
-    --hash=sha256:aad17e462f42ddbef5984d70c40bfc4146c322a2da79715932cd8976317054de \
-    --hash=sha256:b560b72ed4816aee52783c66854d96157fd8175631f01ef58e894cc57c84f0f6 \
-    --hash=sha256:b6b0e4912030c6f28bcb72b9ebe4989d6dc2eebcd2a9cdc35fefc38052dd4fe8 \
-    --hash=sha256:baf1c7b78cddb5af00971ad5294a4583188bda1495b13760d9f03c9483bb6203 \
-    --hash=sha256:c0295d52b012cbe0d3059b1dba99159c3be55e632aae1999ab74ae2bd86a33d7 \
-    --hash=sha256:c562b49c96906b4029b5685075fe1ebd3b5cc2601dfa0b9e16c2c09d6cbce048 \
-    --hash=sha256:c69567ddbac186e8c0aadc1f324a60a564cfe25e43ef2ce81bcc4b8c3abffbae \
-    --hash=sha256:ca71d501629d1fa50ea7fa3b08ba884fe10cefc559f5c6c8dfe9036c16e8ae89 \
-    --hash=sha256:ca976884ce34070799e4dfc6fbd68cb1d181db1eefe4a3a94798ddfb34b8867f \
-    --hash=sha256:d0491006a6ad20507aec2be72e7831a42efc93193d2402018007ff827dc62926 \
-    --hash=sha256:d074b07a10c391fc5bbdcb37b2f16f20fcd9e51e10d01652ab298c0d07908ee2 \
-    --hash=sha256:d2ce426ee691319d4767748c8e0895cfc56593d725594e415f274059bcf3cb76 \
-    --hash=sha256:d4284c621f06a72ce2cb55f74ea3150113d926a6eb78ab38340c08f770eb9b4d \
-    --hash=sha256:d5e6b7155b8197b329dc787356cfd2684c9d6a6b1a197f6bbf45f5555a98d411 \
-    --hash=sha256:d816f44a51ba5175394bc6c7879ca0bd2be560b2c9e9f3411ef3a4cbe644c2e9 \
-    --hash=sha256:dd3f79e17b56741b5177bcc36307750d50ea0698df6aa82f69c7db32d968c1c2 \
-    --hash=sha256:dd63cec4e26e790b70544ae5cc48d11b515b09e05fdd5eff12e3195f54b8a586 \
-    --hash=sha256:de9d3e8717560eb05e28739d1b35e4eac2e458553a52a301e51352a7ffc86a35 \
-    --hash=sha256:df4249b579e75094f7e9bb4bd28231acf55e308bf686b952f43100a5a0be394c \
-    --hash=sha256:e178e5b66a06ec5bf51668ec0d4ac8cfb2bdcb553b2c207d58148340efd00143 \
-    --hash=sha256:e60defc3c15defb70bb38dd605ff7e0fae5f6c9c7cbfe0ad7868582cb7e844a6 \
-    --hash=sha256:ee2794111c188548a4547eccc73a6a8527fe2af6cf25e1a4ebda2fd01cdd2e60 \
-    --hash=sha256:ee7ccc7fb7e921d767f853b47814c3048c7de536663e82fbc37f5eb0d532224b \
-    --hash=sha256:ee9cf33e7fe14243f5ca6977658eb7d1042caaa66847daacbd2117adb258b226 \
-    --hash=sha256:f0f17814c505f07806e22b28856c59ac80cee7dd0fbb152aed273e116378f519 \
-    --hash=sha256:f3202a429fe825b699c57892d4371c74cc3456d8d71b7f35d6028c96dfecad31 \
-    --hash=sha256:f7054fdc556f5421f01e39cbb767d5ec5c1139ea98c3e5b350e02e62201740c7 \
-    --hash=sha256:fd1a9edb9dd9d79fbeac1ea1f9a8dd527a6113b18d2e9bcc0d541d308dae639b
-pydantic==2.7.0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:9dee74a271705f14f9a1567671d144a851c675b072736f0a7b2608fd9e495352 \
-    --hash=sha256:b5ecdd42262ca2462e2624793551e80911a1e989f462910bb81aef974b4bb383
-pyright==1.1.359 ; python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:5582777be7eab73512277ac7da7b41e15bc0737f488629cb9babd96e0769be61 \
-    --hash=sha256:f0eab50f3dafce8a7302caeafd6a733f39901a2bf5170bb23d77fd607c8a8dbc
-pytest-cov==5.0.0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:4f0764a1219df53214206bf1feea4633c3b558a2925c8b59f144f682861ce652 \
-    --hash=sha256:5837b58e9f6ebd335b0f8060eecce69b662415b16dc503883a02f45dfeb14857
-pytest-sugar==1.0.0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:6422e83258f5b0c04ce7c632176c7732cab5fdb909cb39cca5c9139f81276c0a \
-    --hash=sha256:70ebcd8fc5795dc457ff8b69d266a4e2e8a74ae0c3edc749381c64b5246c8dfd
-pytest-timeout==2.3.1 ; python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:12397729125c6ecbdaca01035b9e5239d4db97352320af155b3f5de1ba5165d9 \
-    --hash=sha256:68188cb703edfc6a18fad98dc25a3c61e9f24d644b0b70f33af545219fc7813e
-pytest-xdist==3.5.0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:cbb36f3d67e0c478baa57fa4edc8843887e0f6cfc42d677530a36d7472b32d8a \
-    --hash=sha256:d075629c7e00b611df89f490a5063944bee7a4362a5ff11c7cc7824a03dfce24
-pytest==8.1.1 ; python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:2a8386cfc11fa9d2c50ee7b2a57e7d898ef90470a7a34c4b949ff59662bb78b7 \
-    --hash=sha256:ac978141a75948948817d360297b7aae0fcb9d6ff6bc9ec6d514b85d5a65c044
-setuptools==69.5.1 ; python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:6c1fccdac05a97e598fb0ae3bbed5904ccb317337a51139dcd51453611bbb987 \
-    --hash=sha256:c636ac361bc47580504644275c9ad802c50415c7522212252c033bd15f301f32
-sniffio==1.3.1 ; python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:2f6da418d1f1e0fddd844478f41680e794e6051915791a034ff65e5f100525a2 \
-    --hash=sha256:f4324edc670a0f49750a81b895f35c3adb843cca46f0530f79fc1babb23789dc
-sortedcontainers==2.4.0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:25caa5a06cc30b6b83d11423433f65d1f9d76c4c6a0c90e3379eaa43b9bfdb88 \
-    --hash=sha256:a163dcaede0f1c021485e957a39245190e74249897e2ae4b2aa38595db237ee0
-termcolor==2.4.0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:9297c0df9c99445c2412e832e882a7884038a25617c60cea2ad69488d4040d63 \
-    --hash=sha256:aab9e56047c8ac41ed798fa36d892a37aca6b3e9159f3e0c24bc64a9b3ac7b7a
-tomli==2.0.1 ; python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc \
-    --hash=sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f
-trio==0.25.0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:9b41f5993ad2c0e5f62d0acca320ec657fdb6b2a2c22b8c7aed6caf154475c4e \
-    --hash=sha256:e6458efe29cc543e557a91e614e2b51710eba2961669329ce9c862d50c6e8e81
-typing-extensions==4.11.0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
+pygments==2.17.2 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:b27c2826c47d0f3219f29554824c30c5e8945175d888647acd804ddd04af846c \
+    --hash=sha256:da46cec9fd2de5be3a8a784f434e4c4ab670b4ff54d605c4c2717e9d49c4c367
+pymdown-extensions==10.8 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:3539003ff0d5e219ba979d2dc961d18fcad5ac259e66c764482e8347b4c0503c \
+    --hash=sha256:91ca336caf414e1e5e0626feca86e145de9f85a3921a7bcbd32890b51738c428
+python-dateutil==2.9.0.post0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:37dd54208da7e1cd875388217d5e00ebd4179249f90fb72437e91a35459a0ad3 \
+    --hash=sha256:a8b2bc7bffae282281c8140a97d3aa9c14da0b136dfe83f850eea9a5f7470427
+pyyaml-env-tag==0.1 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:70092675bda14fdec33b31ba77e7543de9ddc88f2e5b99160396572d11525bdb \
+    --hash=sha256:af31106dec8a4d68c60207c1886031cbf839b68aa7abccdb19868200532c2069
+pyyaml==6.0.1 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:04ac92ad1925b2cff1db0cfebffb6ffc43457495c9b3c39d3fcae417d7125dc5 \
+    --hash=sha256:062582fca9fabdd2c8b54a3ef1c978d786e0f6b3a1510e0ac93ef59e0ddae2bc \
+    --hash=sha256:0d3304d8c0adc42be59c5f8a4d9e3d7379e6955ad754aa9d6ab7a398b59dd1df \
+    --hash=sha256:1635fd110e8d85d55237ab316b5b011de701ea0f29d07611174a1b42f1444741 \
+    --hash=sha256:184c5108a2aca3c5b3d3bf9395d50893a7ab82a38004c8f61c258d4428e80206 \
+    --hash=sha256:18aeb1bf9a78867dc38b259769503436b7c72f7a1f1f4c93ff9a17de54319b27 \
+    --hash=sha256:1d4c7e777c441b20e32f52bd377e0c409713e8bb1386e1099c2415f26e479595 \
+    --hash=sha256:1e2722cc9fbb45d9b87631ac70924c11d3a401b2d7f410cc0e3bbf249f2dca62 \
+    --hash=sha256:1fe35611261b29bd1de0070f0b2f47cb6ff71fa6595c077e42bd0c419fa27b98 \
+    --hash=sha256:28c119d996beec18c05208a8bd78cbe4007878c6dd15091efb73a30e90539696 \
+    --hash=sha256:326c013efe8048858a6d312ddd31d56e468118ad4cdeda36c719bf5bb6192290 \
+    --hash=sha256:40df9b996c2b73138957fe23a16a4f0ba614f4c0efce1e9406a184b6d07fa3a9 \
+    --hash=sha256:42f8152b8dbc4fe7d96729ec2b99c7097d656dc1213a3229ca5383f973a5ed6d \
+    --hash=sha256:49a183be227561de579b4a36efbb21b3eab9651dd81b1858589f796549873dd6 \
+    --hash=sha256:4fb147e7a67ef577a588a0e2c17b6db51dda102c71de36f8549b6816a96e1867 \
+    --hash=sha256:50550eb667afee136e9a77d6dc71ae76a44df8b3e51e41b77f6de2932bfe0f47 \
+    --hash=sha256:510c9deebc5c0225e8c96813043e62b680ba2f9c50a08d3724c7f28a747d1486 \
+    --hash=sha256:5773183b6446b2c99bb77e77595dd486303b4faab2b086e7b17bc6bef28865f6 \
+    --hash=sha256:596106435fa6ad000c2991a98fa58eeb8656ef2325d7e158344fb33864ed87e3 \
+    --hash=sha256:6965a7bc3cf88e5a1c3bd2e0b5c22f8d677dc88a455344035f03399034eb3007 \
+    --hash=sha256:69b023b2b4daa7548bcfbd4aa3da05b3a74b772db9e23b982788168117739938 \
+    --hash=sha256:6c22bec3fbe2524cde73d7ada88f6566758a8f7227bfbf93a408a9d86bcc12a0 \
+    --hash=sha256:704219a11b772aea0d8ecd7058d0082713c3562b4e271b849ad7dc4a5c90c13c \
+    --hash=sha256:7e07cbde391ba96ab58e532ff4803f79c4129397514e1413a7dc761ccd755735 \
+    --hash=sha256:81e0b275a9ecc9c0c0c07b4b90ba548307583c125f54d5b6946cfee6360c733d \
+    --hash=sha256:855fb52b0dc35af121542a76b9a84f8d1cd886ea97c84703eaa6d88e37a2ad28 \
+    --hash=sha256:8d4e9c88387b0f5c7d5f281e55304de64cf7f9c0021a3525bd3b1c542da3b0e4 \
+    --hash=sha256:9046c58c4395dff28dd494285c82ba00b546adfc7ef001486fbf0324bc174fba \
+    --hash=sha256:9eb6caa9a297fc2c2fb8862bc5370d0303ddba53ba97e71f08023b6cd73d16a8 \
+    --hash=sha256:a08c6f0fe150303c1c6b71ebcd7213c2858041a7e01975da3a99aed1e7a378ef \
+    --hash=sha256:a0cd17c15d3bb3fa06978b4e8958dcdc6e0174ccea823003a106c7d4d7899ac5 \
+    --hash=sha256:afd7e57eddb1a54f0f1a974bc4391af8bcce0b444685d936840f125cf046d5bd \
+    --hash=sha256:b1275ad35a5d18c62a7220633c913e1b42d44b46ee12554e5fd39c70a243d6a3 \
+    --hash=sha256:b786eecbdf8499b9ca1d697215862083bd6d2a99965554781d0d8d1ad31e13a0 \
+    --hash=sha256:ba336e390cd8e4d1739f42dfe9bb83a3cc2e80f567d8805e11b46f4a943f5515 \
+    --hash=sha256:baa90d3f661d43131ca170712d903e6295d1f7a0f595074f151c0aed377c9b9c \
+    --hash=sha256:bc1bf2925a1ecd43da378f4db9e4f799775d6367bdb94671027b73b393a7c42c \
+    --hash=sha256:bd4af7373a854424dabd882decdc5579653d7868b8fb26dc7d0e99f823aa5924 \
+    --hash=sha256:bf07ee2fef7014951eeb99f56f39c9bb4af143d8aa3c21b1677805985307da34 \
+    --hash=sha256:bfdf460b1736c775f2ba9f6a92bca30bc2095067b8a9d77876d1fad6cc3b4a43 \
+    --hash=sha256:c8098ddcc2a85b61647b2590f825f3db38891662cfc2fc776415143f599bb859 \
+    --hash=sha256:d2b04aac4d386b172d5b9692e2d2da8de7bfb6c387fa4f801fbf6fb2e6ba4673 \
+    --hash=sha256:d483d2cdf104e7c9fa60c544d92981f12ad66a457afae824d146093b8c294c54 \
+    --hash=sha256:d858aa552c999bc8a8d57426ed01e40bef403cd8ccdd0fc5f6f04a00414cac2a \
+    --hash=sha256:e7d73685e87afe9f3b36c799222440d6cf362062f78be1013661b00c5c6f678b \
+    --hash=sha256:f003ed9ad21d6a4713f0a9b5a7a0a79e08dd0f221aff4525a2be4c346ee60aab \
+    --hash=sha256:f22ac1c3cac4dbc50079e965eba2c1058622631e526bd9afd45fedd49ba781fa \
+    --hash=sha256:faca3bdcf85b2fc05d06ff3fbc1f83e1391b3e724afa3feba7d13eeab355484c \
+    --hash=sha256:fca0e3a251908a499833aa292323f32437106001d436eca0e6e7833256674585 \
+    --hash=sha256:fd1592b3fdf65fff2ad0004b5e363300ef59ced41c2e6b3a99d4089fa8c5435d \
+    --hash=sha256:fd66fc5d0da6d9815ba2cebeb4205f95818ff4b79c3ebe268e75d961704af52f
+regex==2024.4.16 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:00169caa125f35d1bca6045d65a662af0202704489fada95346cfa092ec23f39 \
+    --hash=sha256:03576e3a423d19dda13e55598f0fd507b5d660d42c51b02df4e0d97824fdcae3 \
+    --hash=sha256:03e68f44340528111067cecf12721c3df4811c67268b897fbe695c95f860ac42 \
+    --hash=sha256:0534b034fba6101611968fae8e856c1698da97ce2efb5c2b895fc8b9e23a5834 \
+    --hash=sha256:08dea89f859c3df48a440dbdcd7b7155bc675f2fa2ec8c521d02dc69e877db70 \
+    --hash=sha256:0a38d151e2cdd66d16dab550c22f9521ba79761423b87c01dae0a6e9add79c0d \
+    --hash=sha256:0c8290b44d8b0af4e77048646c10c6e3aa583c1ca67f3b5ffb6e06cf0c6f0f89 \
+    --hash=sha256:10188fe732dec829c7acca7422cdd1bf57d853c7199d5a9e96bb4d40db239c73 \
+    --hash=sha256:1210365faba7c2150451eb78ec5687871c796b0f1fa701bfd2a4a25420482d26 \
+    --hash=sha256:12f6a3f2f58bb7344751919a1876ee1b976fe08b9ffccb4bbea66f26af6017b9 \
+    --hash=sha256:159dc4e59a159cb8e4e8f8961eb1fa5d58f93cb1acd1701d8aff38d45e1a84a6 \
+    --hash=sha256:20b7a68444f536365af42a75ccecb7ab41a896a04acf58432db9e206f4e525d6 \
+    --hash=sha256:23cff1b267038501b179ccbbd74a821ac4a7192a1852d1d558e562b507d46013 \
+    --hash=sha256:2c72608e70f053643437bd2be0608f7f1c46d4022e4104d76826f0839199347a \
+    --hash=sha256:3399dd8a7495bbb2bacd59b84840eef9057826c664472e86c91d675d007137f5 \
+    --hash=sha256:34422d5a69a60b7e9a07a690094e824b66f5ddc662a5fc600d65b7c174a05f04 \
+    --hash=sha256:370c68dc5570b394cbaadff50e64d705f64debed30573e5c313c360689b6aadc \
+    --hash=sha256:3a1018e97aeb24e4f939afcd88211ace472ba566efc5bdf53fd8fd7f41fa7170 \
+    --hash=sha256:3d5ac5234fb5053850d79dd8eb1015cb0d7d9ed951fa37aa9e6249a19aa4f336 \
+    --hash=sha256:4313ab9bf6a81206c8ac28fdfcddc0435299dc88cad12cc6305fd0e78b81f9e4 \
+    --hash=sha256:445ca8d3c5a01309633a0c9db57150312a181146315693273e35d936472df912 \
+    --hash=sha256:479595a4fbe9ed8f8f72c59717e8cf222da2e4c07b6ae5b65411e6302af9708e \
+    --hash=sha256:4918fd5f8b43aa7ec031e0fef1ee02deb80b6afd49c85f0790be1dc4ce34cb50 \
+    --hash=sha256:4aba818dcc7263852aabb172ec27b71d2abca02a593b95fa79351b2774eb1d2b \
+    --hash=sha256:4e819a806420bc010489f4e741b3036071aba209f2e0989d4750b08b12a9343f \
+    --hash=sha256:4facc913e10bdba42ec0aee76d029aedda628161a7ce4116b16680a0413f658a \
+    --hash=sha256:549c3584993772e25f02d0656ac48abdda73169fe347263948cf2b1cead622f3 \
+    --hash=sha256:5c02fcd2bf45162280613d2e4a1ca3ac558ff921ae4e308ecb307650d3a6ee51 \
+    --hash=sha256:5f580c651a72b75c39e311343fe6875d6f58cf51c471a97f15a938d9fe4e0d37 \
+    --hash=sha256:62120ed0de69b3649cc68e2965376048793f466c5a6c4370fb27c16c1beac22d \
+    --hash=sha256:6295004b2dd37b0835ea5c14a33e00e8cfa3c4add4d587b77287825f3418d310 \
+    --hash=sha256:65436dce9fdc0aeeb0a0effe0839cb3d6a05f45aa45a4d9f9c60989beca78b9c \
+    --hash=sha256:684008ec44ad275832a5a152f6e764bbe1914bea10968017b6feaecdad5736e0 \
+    --hash=sha256:684e52023aec43bdf0250e843e1fdd6febbe831bd9d52da72333fa201aaa2335 \
+    --hash=sha256:6cc38067209354e16c5609b66285af17a2863a47585bcf75285cab33d4c3b8df \
+    --hash=sha256:6f2f017c5be19984fbbf55f8af6caba25e62c71293213f044da3ada7091a4455 \
+    --hash=sha256:743deffdf3b3481da32e8a96887e2aa945ec6685af1cfe2bcc292638c9ba2f48 \
+    --hash=sha256:7571f19f4a3fd00af9341c7801d1ad1967fc9c3f5e62402683047e7166b9f2b4 \
+    --hash=sha256:7731728b6568fc286d86745f27f07266de49603a6fdc4d19c87e8c247be452af \
+    --hash=sha256:785c071c982dce54d44ea0b79cd6dfafddeccdd98cfa5f7b86ef69b381b457d9 \
+    --hash=sha256:78fddb22b9ef810b63ef341c9fcf6455232d97cfe03938cbc29e2672c436670e \
+    --hash=sha256:7bb966fdd9217e53abf824f437a5a2d643a38d4fd5fd0ca711b9da683d452969 \
+    --hash=sha256:7cbc5d9e8a1781e7be17da67b92580d6ce4dcef5819c1b1b89f49d9678cc278c \
+    --hash=sha256:803b8905b52de78b173d3c1e83df0efb929621e7b7c5766c0843704d5332682f \
+    --hash=sha256:80b696e8972b81edf0af2a259e1b2a4a661f818fae22e5fa4fa1a995fb4a40fd \
+    --hash=sha256:81500ed5af2090b4a9157a59dbc89873a25c33db1bb9a8cf123837dcc9765047 \
+    --hash=sha256:89ec7f2c08937421bbbb8b48c54096fa4f88347946d4747021ad85f1b3021b3c \
+    --hash=sha256:8ba6745440b9a27336443b0c285d705ce73adb9ec90e2f2004c64d95ab5a7598 \
+    --hash=sha256:8c91e1763696c0eb66340c4df98623c2d4e77d0746b8f8f2bee2c6883fd1fe18 \
+    --hash=sha256:8d015604ee6204e76569d2f44e5a210728fa917115bef0d102f4107e622b08d5 \
+    --hash=sha256:8d1f86f3f4e2388aa3310b50694ac44daefbd1681def26b4519bd050a398dc5a \
+    --hash=sha256:8f83b6fd3dc3ba94d2b22717f9c8b8512354fd95221ac661784df2769ea9bba9 \
+    --hash=sha256:8fc6976a3395fe4d1fbeb984adaa8ec652a1e12f36b56ec8c236e5117b585427 \
+    --hash=sha256:904c883cf10a975b02ab3478bce652f0f5346a2c28d0a8521d97bb23c323cc8b \
+    --hash=sha256:911742856ce98d879acbea33fcc03c1d8dc1106234c5e7d068932c945db209c0 \
+    --hash=sha256:91797b98f5e34b6a49f54be33f72e2fb658018ae532be2f79f7c63b4ae225145 \
+    --hash=sha256:95399831a206211d6bc40224af1c635cb8790ddd5c7493e0bd03b85711076a53 \
+    --hash=sha256:956b58d692f235cfbf5b4f3abd6d99bf102f161ccfe20d2fd0904f51c72c4c66 \
+    --hash=sha256:98c1165f3809ce7774f05cb74e5408cd3aa93ee8573ae959a97a53db3ca3180d \
+    --hash=sha256:9ab40412f8cd6f615bfedea40c8bf0407d41bf83b96f6fc9ff34976d6b7037fd \
+    --hash=sha256:9df1bfef97db938469ef0a7354b2d591a2d438bc497b2c489471bec0e6baf7c4 \
+    --hash=sha256:a01fe2305e6232ef3e8f40bfc0f0f3a04def9aab514910fa4203bafbc0bb4682 \
+    --hash=sha256:a70b51f55fd954d1f194271695821dd62054d949efd6368d8be64edd37f55c86 \
+    --hash=sha256:a7ccdd1c4a3472a7533b0a7aa9ee34c9a2bef859ba86deec07aff2ad7e0c3b94 \
+    --hash=sha256:b340cccad138ecb363324aa26893963dcabb02bb25e440ebdf42e30963f1a4e0 \
+    --hash=sha256:b74586dd0b039c62416034f811d7ee62810174bb70dffcca6439f5236249eb09 \
+    --hash=sha256:b9d320b3bf82a39f248769fc7f188e00f93526cc0fe739cfa197868633d44701 \
+    --hash=sha256:ba2336d6548dee3117520545cfe44dc28a250aa091f8281d28804aa8d707d93d \
+    --hash=sha256:ba8122e3bb94ecda29a8de4cf889f600171424ea586847aa92c334772d200331 \
+    --hash=sha256:bd727ad276bb91928879f3aa6396c9a1d34e5e180dce40578421a691eeb77f47 \
+    --hash=sha256:c21fc21a4c7480479d12fd8e679b699f744f76bb05f53a1d14182b31f55aac76 \
+    --hash=sha256:c2d0e7cbb6341e830adcbfa2479fdeebbfbb328f11edd6b5675674e7a1e37730 \
+    --hash=sha256:c2ef6f7990b6e8758fe48ad08f7e2f66c8f11dc66e24093304b87cae9037bb4a \
+    --hash=sha256:c4ed75ea6892a56896d78f11006161eea52c45a14994794bcfa1654430984b22 \
+    --hash=sha256:cccc79a9be9b64c881f18305a7c715ba199e471a3973faeb7ba84172abb3f317 \
+    --hash=sha256:d0800631e565c47520aaa04ae38b96abc5196fe8b4aa9bd864445bd2b5848a7a \
+    --hash=sha256:d2da13568eff02b30fd54fccd1e042a70fe920d816616fda4bf54ec705668d81 \
+    --hash=sha256:d61ae114d2a2311f61d90c2ef1358518e8f05eafda76eaf9c772a077e0b465ec \
+    --hash=sha256:d83c2bc678453646f1a18f8db1e927a2d3f4935031b9ad8a76e56760461105dd \
+    --hash=sha256:dd5acc0a7d38fdc7a3a6fd3ad14c880819008ecb3379626e56b163165162cc46 \
+    --hash=sha256:df79012ebf6f4efb8d307b1328226aef24ca446b3ff8d0e30202d7ebcb977a8c \
+    --hash=sha256:e0a2df336d1135a0b3a67f3bbf78a75f69562c1199ed9935372b82215cddd6e2 \
+    --hash=sha256:e2f142b45c6fed48166faeb4303b4b58c9fcd827da63f4cf0a123c3480ae11fb \
+    --hash=sha256:e697e1c0238133589e00c244a8b676bc2cfc3ab4961318d902040d099fec7483 \
+    --hash=sha256:e757d475953269fbf4b441207bb7dbdd1c43180711b6208e129b637792ac0b93 \
+    --hash=sha256:e87ab229332ceb127a165612d839ab87795972102cb9830e5f12b8c9a5c1b508 \
+    --hash=sha256:ea355eb43b11764cf799dda62c658c4d2fdb16af41f59bb1ccfec517b60bcb07 \
+    --hash=sha256:ec7e0043b91115f427998febaa2beb82c82df708168b35ece3accb610b91fac1 \
+    --hash=sha256:eeaa0b5328b785abc344acc6241cffde50dc394a0644a968add75fcefe15b9d4 \
+    --hash=sha256:f2d80a6749724b37853ece57988b39c4e79d2b5fe2869a86e8aeae3bbeef9eb0 \
+    --hash=sha256:fa454d26f2e87ad661c4f0c5a5fe4cf6aab1e307d1b94f16ffdfcb089ba685c0 \
+    --hash=sha256:fb83cc090eac63c006871fd24db5e30a1f282faa46328572661c0a24a2323a08 \
+    --hash=sha256:fd80d1280d473500d8086d104962a82d77bfbf2b118053824b7be28cd5a79ea5
+requests==2.31.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f \
+    --hash=sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1
+six==1.16.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926 \
+    --hash=sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254
+typing-extensions==4.11.0 ; python_version >= "3.9" and python_version < "3.10" \
     --hash=sha256:83f085bd5ca59c80295fc2a82ab5dac679cbe02b9f33f7d83af68e241bea51b0 \
     --hash=sha256:c1f94d72897edaf4ce775bb7558d5b79d8126906a14ea5ed1635921406c0387a
-virtualenv==20.25.3 ; python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:7bb554bbdfeaacc3349fa614ea5bff6ac300fc7c335e9facf3a3bcfc703f45be \
-    --hash=sha256:8aac4332f2ea6ef519c648d0bc48a5b1d324994753519919bddbb1aff25a104e
+urllib3==2.2.1 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:450b20ec296a467077128bff42b73080516e71b56ff59a60a02bef2232c4fa9d \
+    --hash=sha256:d0570876c61ab9e520d776c38acbbb5b05a776d3f9ff98a5c8fd5162a444cf19
+watchdog==4.0.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:11e12fafb13372e18ca1bbf12d50f593e7280646687463dd47730fd4f4d5d257 \
+    --hash=sha256:2895bf0518361a9728773083908801a376743bcc37dfa252b801af8fd281b1ca \
+    --hash=sha256:39cb34b1f1afbf23e9562501673e7146777efe95da24fab5707b88f7fb11649b \
+    --hash=sha256:45cc09cc4c3b43fb10b59ef4d07318d9a3ecdbff03abd2e36e77b6dd9f9a5c85 \
+    --hash=sha256:4986db5e8880b0e6b7cd52ba36255d4793bf5cdc95bd6264806c233173b1ec0b \
+    --hash=sha256:5369136a6474678e02426bd984466343924d1df8e2fd94a9b443cb7e3aa20d19 \
+    --hash=sha256:557ba04c816d23ce98a06e70af6abaa0485f6d94994ec78a42b05d1c03dcbd50 \
+    --hash=sha256:6a4db54edea37d1058b08947c789a2354ee02972ed5d1e0dca9b0b820f4c7f92 \
+    --hash=sha256:6a80d5cae8c265842c7419c560b9961561556c4361b297b4c431903f8c33b269 \
+    --hash=sha256:6a9c71a0b02985b4b0b6d14b875a6c86ddea2fdbebd0c9a720a806a8bbffc69f \
+    --hash=sha256:6c47bdd680009b11c9ac382163e05ca43baf4127954c5f6d0250e7d772d2b80c \
+    --hash=sha256:6e949a8a94186bced05b6508faa61b7adacc911115664ccb1923b9ad1f1ccf7b \
+    --hash=sha256:73c7a935e62033bd5e8f0da33a4dcb763da2361921a69a5a95aaf6c93aa03a87 \
+    --hash=sha256:76ad8484379695f3fe46228962017a7e1337e9acadafed67eb20aabb175df98b \
+    --hash=sha256:8350d4055505412a426b6ad8c521bc7d367d1637a762c70fdd93a3a0d595990b \
+    --hash=sha256:87e9df830022488e235dd601478c15ad73a0389628588ba0b028cb74eb72fed8 \
+    --hash=sha256:8f9a542c979df62098ae9c58b19e03ad3df1c9d8c6895d96c0d51da17b243b1c \
+    --hash=sha256:8fec441f5adcf81dd240a5fe78e3d83767999771630b5ddfc5867827a34fa3d3 \
+    --hash=sha256:9a03e16e55465177d416699331b0f3564138f1807ecc5f2de9d55d8f188d08c7 \
+    --hash=sha256:ba30a896166f0fee83183cec913298151b73164160d965af2e93a20bbd2ab605 \
+    --hash=sha256:c17d98799f32e3f55f181f19dd2021d762eb38fdd381b4a748b9f5a36738e935 \
+    --hash=sha256:c522392acc5e962bcac3b22b9592493ffd06d1fc5d755954e6be9f4990de932b \
+    --hash=sha256:d0f9bd1fd919134d459d8abf954f63886745f4660ef66480b9d753a7c9d40927 \
+    --hash=sha256:d18d7f18a47de6863cd480734613502904611730f8def45fc52a5d97503e5101 \
+    --hash=sha256:d31481ccf4694a8416b681544c23bd271f5a123162ab603c7d7d2dd7dd901a07 \
+    --hash=sha256:e3e7065cbdabe6183ab82199d7a4f6b3ba0a438c5a512a68559846ccb76a78ec \
+    --hash=sha256:eed82cdf79cd7f0232e2fdc1ad05b06a5e102a43e331f7d041e5f0e0a34a51c4 \
+    --hash=sha256:f970663fa4f7e80401a7b0cbeec00fa801bf0287d93d48368fc3e6fa32716245 \
+    --hash=sha256:f9b2fdca47dc855516b2d66eef3c39f2672cbf7e7a42e7e67ad2cbfcd6ba107d
+zipp==3.18.1 ; python_version >= "3.9" and python_version < "3.10" \
+    --hash=sha256:206f5a15f2af3dbaee80769fb7dc6f249695e940acca08dfb2a4769fe61e538b \
+    --hash=sha256:2884ed22e7d8961de1c9a05142eb69a247f120291bc0206a00a7642f09b5b715
```

### Comparing `alluka-0.1.5/mkdocs.yml` & `alluka-0.2.0/mkdocs.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # mkdocs.yml
 site_name: "Alluka docs"
 repo_url: https://github.com/FasterSpeeding/Alluka
 theme:
   name: material
+  features:
+    - navigation.prune
   icon:
     admonition:
       note: octicons/tag-16
       abstract: octicons/checklist-16
       info: octicons/info-16
       tip: octicons/squirrel-16
       success: octicons/check-16
@@ -17,27 +19,30 @@
       bug: octicons/bug-16
       example: octicons/beaker-16
       quote: octicons/quote-16
   palette:
     - media: "(prefers-color-scheme: light)"
       scheme: default
       primary: pink
+      accent: pink
       toggle:
         icon: material/lightbulb
         name: Switch to dark mode
     - media: "(prefers-color-scheme: dark)"
       scheme: slate
       primary: pink
       toggle:
         icon: material/lightbulb
         name: Switch to light mode
 
 markdown_extensions:
   - admonition
   - pymdownx.details
+  - pymdownx.snippets:
+      dedent_subsections: true
   - pymdownx.superfences
   - markdown_include.include
   - toc:
       permalink: "#"
 
 plugins:
   - search
@@ -58,8 +63,9 @@
             show_signature_annotations: false
             show_source: false
             show_submodules: false
 
 watch:
   - alluka
   - CHANGELOG.md
+  - docs_src
   - README.md
```

### Comparing `alluka-0.1.5/noxfile.py` & `alluka-0.2.0/noxfile.py`

 * *Files identical despite different names*

### Comparing `alluka-0.1.5/piped/.github/workflows/docker-publish.yml` & `alluka-0.2.0/piped/.github/workflows/docker-publish.yml`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
       packages: write
       # This is used to complete the identity challenge
       # with sigstore/fulcio when running outside of PRs.
       id-token: write
 
     steps:
       - name: Checkout repository
-        uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f
+        uses: actions/checkout@0ad4b8fadaa221de15dcec353f45205ec38ea70b
 
       # Install the cosign tool except on PR
       # https://github.com/sigstore/cosign-installer
       - name: Install cosign
         if: github.event_name != 'pull_request'
         uses: sigstore/cosign-installer@59acb6260d9c0ba8f4a2f9d9b48431a222b68e20 #v3.5.0
```

### Comparing `alluka-0.1.5/piped/.github/workflows/freeze-for-pr.yml` & `alluka-0.2.0/piped/.github/workflows/freeze-for-pr.yml`

 * *Files 15% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     paths: ["piped", "pyproject.toml", "requirements.in", "bot/requirements.in", "dev-requirements/*.in", "!dev-requirements/constraints.in", "python/base-requirements/*.in", "!python/base-requirements/constraints.in"]
 
 jobs:
   freeze-pr-dep-changes:
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f
+      - uses: actions/checkout@0ad4b8fadaa221de15dcec353f45205ec38ea70b
         with:
           submodules: "true"
 
       - name: Set up Python 3.11
         uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
         with:
           python-version: "3.11"
```

### Comparing `alluka-0.1.5/piped/.github/workflows/lint.yml` & `alluka-0.2.0/piped/github/actions/verify-types.yml`

 * *Files 24% similar despite different names*

```diff
@@ -1,44 +1,38 @@
-name: Lint
+name: Verify type-completeness
 
 concurrency:
-  group: ${{ github.workflow }}-${{ github.ref }}
+  {% raw %}group: ${{ github.workflow }}-${{ github.ref }}{% endraw %}
   cancel-in-progress: true
 
 on:
   push:
     branches:
       - master
   pull_request:
     branches:
       - master
   schedule:
     - cron: "0 12 * * 6"
   workflow_dispatch:
 
 jobs:
-  lint:
+  verify-types:
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f
+      - uses: actions/checkout@0ad4b8fadaa221de15dcec353f45205ec38ea70b
         with:
           submodules: "true"
 
-      - name: Set up Python 3.11
+      - name: Set up Python {{ DEFAULT_PY_VER }}
         uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
         with:
-          python-version: "3.11"
+          python-version: "{{ DEFAULT_PY_VER }}"
 
       - name: install prerequisites
         run: |
           python -m pip install --upgrade pip wheel
-          python -m pip install -r ./python/base-requirements/nox.txt
+          python -m pip install -r {{ NOX_DEP_PATH }}
 
-      - name: Lint markup
-        run: python -m nox -s verify-markup
-
-      - name: Check spelling
-        run: python -m nox -s spell-check
-
-      - name: Lint with flake8
-        run: python -m nox -s flake8
+      - name: Run verify types
+        run: python -m nox -s verify-types
```

### Comparing `alluka-0.1.5/piped/.github/workflows/reformat.yml` & `alluka-0.2.0/piped/.github/workflows/reformat.yml`

 * *Files 14% similar despite different names*

```diff
@@ -10,15 +10,15 @@
       - master
 
 jobs:
   reformat:
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f
+      - uses: actions/checkout@0ad4b8fadaa221de15dcec353f45205ec38ea70b
         with:
           submodules: "true"
 
       - name: Set up Python 3.11
         uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
         with:
           python-version: "3.11"
```

### Comparing `alluka-0.1.5/piped/.github/workflows/resync-piped.yml` & `alluka-0.2.0/.github/workflows/reformat.yml`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,39 @@
-name: Resync piped
+name: Reformat PR code
 
 concurrency:
   group: ${{ github.workflow }}-${{ github.ref }}
   cancel-in-progress: true
 
 on:
   pull_request:
     branches:
       - master
-    paths: ["github/actions/*", "pyproject.toml"]
 
 jobs:
-  resync-piped:
+  reformat:
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f
+      - uses: actions/checkout@0ad4b8fadaa221de15dcec353f45205ec38ea70b
         with:
           submodules: "true"
 
-      - name: Set up Python 3.11
+      - name: Set up Python 3.9
         uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
         with:
-          python-version: "3.11"
+          python-version: "3.9"
 
       - name: install prerequisites
         run: |
           python -m pip install --upgrade pip wheel
-          python -m pip install -r ./python/base-requirements/nox.txt
+          python -m pip install -r ./piped/python/base-requirements/nox.txt
 
-      - name: Resync Piped
-        run: python -m nox -s copy-piped bot-package-diff
+      - name: Reformat
+        run: python -m nox -s reformat bot-package-diff
 
       - uses: actions/upload-artifact@65462800fd760344b1a7b4382951275a0abb4808
         with:
           name: gogo.patch
           path: gogo.patch
 
       - name: Check diff file
```

### Comparing `alluka-0.1.5/piped/.github/workflows/type-check.yml` & `alluka-0.2.0/piped/.github/workflows/type-check.yml`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,15 @@
   workflow_dispatch:
 
 jobs:
   type-check:
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f
+      - uses: actions/checkout@0ad4b8fadaa221de15dcec353f45205ec38ea70b
         with:
           submodules: "true"
 
       - name: Set up Python 3.11
         uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
         with:
           python-version: "3.11"
```

### Comparing `alluka-0.1.5/piped/.github/workflows/update-licence.yml` & `alluka-0.2.0/piped/.github/workflows/update-licence.yml`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   workflow_dispatch:
 
 jobs:
   update-licence:
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f
+      - uses: actions/checkout@0ad4b8fadaa221de15dcec353f45205ec38ea70b
         with:
           submodules: "true"
 
       - name: Set up Python 3.11
         uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
         with:
           python-version: "3.11"
@@ -24,15 +24,15 @@
           python -m pip install --upgrade pip wheel
           python -m pip install -r ./python/base-requirements/nox.txt
 
       - name: Update licence
         run: python -m nox -s update-licence
 
       - name: Create Pull Request
-        uses: peter-evans/create-pull-request@9153d834b60caba6d51c9b9510b087acf9f33f83
+        uses: peter-evans/create-pull-request@6d6857d36972b65feb161a90e484f2984215f83e
         with:
           author: "always-on-duty[bot] <120557446+always-on-duty[bot]@users.noreply.github.com>"
           branch: task/update-licence
           commit-message: Update licence
           committer: "always-on-duty[bot] <120557446+always-on-duty[bot]@users.noreply.github.com>"
           title: Update licence
           token: ${{ secrets.ACTIONS_TOKEN || secrets.GITHUB_TOKEN }}
```

### Comparing `alluka-0.1.5/piped/.github/workflows/upgrade-locks.yml` & `alluka-0.2.0/.github/workflows/upgrade-locks.yml`

 * *Files 14% similar despite different names*

```diff
@@ -6,33 +6,33 @@
   workflow_dispatch:
 
 jobs:
   upgrade-deps:
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f
+      - uses: actions/checkout@0ad4b8fadaa221de15dcec353f45205ec38ea70b
         with:
           submodules: "true"
 
-      - name: Set up Python 3.11
+      - name: Set up Python 3.9
         uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
         with:
-          python-version: "3.11"
+          python-version: "3.9"
 
       - name: install prerequisites
         run: |
           python -m pip install --upgrade pip wheel
-          python -m pip install -r ./python/base-requirements/nox.txt
+          python -m pip install -r ./piped/python/base-requirements/nox.txt
 
       - name: Upgrade dependency locks
         run: python -m nox -s freeze-locks
 
       - name: Create Pull Request
-        uses: peter-evans/create-pull-request@9153d834b60caba6d51c9b9510b087acf9f33f83
+        uses: peter-evans/create-pull-request@6d6857d36972b65feb161a90e484f2984215f83e
         with:
           author: "always-on-duty[bot] <120557446+always-on-duty[bot]@users.noreply.github.com>"
           branch: task/upgrade-deps
           commit-message: Upgrade dependency locks
           committer: "always-on-duty[bot] <120557446+always-on-duty[bot]@users.noreply.github.com>"
           title: Upgrade dependency locks
           token: ${{ secrets.ACTIONS_TOKEN || secrets.GITHUB_TOKEN }}
```

### Comparing `alluka-0.1.5/piped/.github/workflows/verify-locks.yml` & `alluka-0.2.0/.github/workflows/verify-locks.yml`

 * *Files 20% similar despite different names*

```diff
@@ -7,30 +7,30 @@
   group: ${{ github.workflow }}-${{ github.ref }}
   cancel-in-progress: true
 
 on:
   pull_request:
     branches:
       - master
-    paths: ["bot/requirements.txt", "dev-requirements/*.txt", "python/base-requirements/*.txt"]
+    paths: ["dev-requirements/*.txt"]
 
 jobs:
   verify-pr-dep-changes:
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f
+      - uses: actions/checkout@0ad4b8fadaa221de15dcec353f45205ec38ea70b
         with:
           submodules: "true"
 
-      - name: Set up Python 3.11
+      - name: Set up Python 3.9
         uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
         with:
-          python-version: "3.11"
+          python-version: "3.9"
 
       - name: install prerequisites
         run: |
           python -m pip install --upgrade pip wheel
-          python -m pip install -r ./python/base-requirements/nox.txt
+          python -m pip install -r ./piped/python/base-requirements/nox.txt
 
       - name: Verify dependency locks
         run: python -m nox -s verify-deps
```

### Comparing `alluka-0.1.5/piped/.gitignore` & `alluka-0.2.0/piped/.gitignore`

 * *Files identical despite different names*

### Comparing `alluka-0.1.5/piped/LICENSE` & `alluka-0.2.0/piped/LICENSE`

 * *Files identical despite different names*

### Comparing `alluka-0.1.5/piped/bot/main.py` & `alluka-0.2.0/piped/bot/main.py`

 * *Files identical despite different names*

### Comparing `alluka-0.1.5/piped/bot/requirements.txt` & `alluka-0.2.0/piped/bot/requirements.txt`

 * *Files identical despite different names*

### Comparing `alluka-0.1.5/piped/dev-requirements/flake8.in` & `alluka-0.2.0/piped/dev-requirements/flake8.in`

 * *Files identical despite different names*

### Comparing `alluka-0.1.5/piped/dev-requirements/flake8.txt` & `alluka-0.2.0/piped/dev-requirements/flake8.txt`

 * *Files identical despite different names*

### Comparing `alluka-0.1.5/piped/dev-requirements/type-checking.txt` & `alluka-0.2.0/piped/dev-requirements/type-checking.txt`

 * *Files identical despite different names*

### Comparing `alluka-0.1.5/piped/github/actions/docker-publish.yml` & `alluka-0.2.0/piped/github/actions/docker-publish.yml`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
       packages: write
       # This is used to complete the identity challenge
       # with sigstore/fulcio when running outside of PRs.
       id-token: write
 
     steps:
       - name: Checkout repository
-        uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f
+        uses: actions/checkout@0ad4b8fadaa221de15dcec353f45205ec38ea70b
 
       # Install the cosign tool except on PR
       # https://github.com/sigstore/cosign-installer
       - name: Install cosign
         if: github.event_name != 'pull_request'
         uses: sigstore/cosign-installer@59acb6260d9c0ba8f4a2f9d9b48431a222b68e20 #v3.5.0
```

### Comparing `alluka-0.1.5/piped/github/actions/freeze-for-pr.yml` & `alluka-0.2.0/piped/github/actions/freeze-for-pr.yml`

 * *Files 15% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     paths: [{{ (FILTERS + EXTEND_FILTERS) | map("quoted") | join(", ") }}]
 
 jobs:
   freeze-pr-dep-changes:
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f
+      - uses: actions/checkout@0ad4b8fadaa221de15dcec353f45205ec38ea70b
         with:
           submodules: "true"
 
       - name: Set up Python {{ DEFAULT_PY_VER }}
         uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
         with:
           python-version: "{{ DEFAULT_PY_VER }}"
```

### Comparing `alluka-0.1.5/piped/github/actions/lint.yml` & `alluka-0.2.0/piped/github/actions/lint.yml`

 * *Files 14% similar despite different names*

```diff
@@ -16,15 +16,15 @@
   workflow_dispatch:
 
 jobs:
   lint:
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f
+      - uses: actions/checkout@0ad4b8fadaa221de15dcec353f45205ec38ea70b
         with:
           submodules: "true"
 
       - name: Set up Python {{ DEFAULT_PY_VER }}
         uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
         with:
           python-version: "{{ DEFAULT_PY_VER }}"
```

### Comparing `alluka-0.1.5/piped/github/actions/pr-docs.yml` & `alluka-0.2.0/piped/github/actions/pr-docs.yml`

 * *Files 12% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 jobs:
   deploy-docs-preview:
     runs-on: ubuntu-latest
 
     steps:
       - name: Fetch merge branch
-        uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f
+        uses: actions/checkout@0ad4b8fadaa221de15dcec353f45205ec38ea70b
         with:
           {% raw %}ref: ${{ github.event.pull_request.head.sha }}{% endraw %}
           {% raw %}repository: ${{ github.event.pull_request.head.repo.full_name }}{% endraw %}
           submodules: "true"
 
       - name: Set up Python {{ DEFAULT_PY_VER }}
         if: github.event.action != 'closed'
```

### Comparing `alluka-0.1.5/piped/github/actions/publish.yml` & `alluka-0.2.0/piped/github/actions/publish.yml`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     name: upload release to PyPI
     runs-on: ubuntu-latest
     environment: release
     permissions:
       id-token: write
 
     steps:
-      - uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f
+      - uses: actions/checkout@0ad4b8fadaa221de15dcec353f45205ec38ea70b
         with:
           submodules: "true"
 
       - name: Set up Python {{ DEFAULT_PY_VER }}
         uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
         with:
           python-version: "{{ DEFAULT_PY_VER }}"
```

### Comparing `alluka-0.1.5/piped/github/actions/py-test.yml` & `alluka-0.2.0/piped/github/actions/py-test.yml`

 * *Files 10% similar despite different names*

```diff
@@ -22,15 +22,15 @@
       matrix:
         os: {{ OSES }}
         python-version: [{{ PYTHON_VERSIONS | map("quoted") | join(", ") }}]
 
     {% raw %}runs-on: ${{ matrix.os }}{% endraw %}
 
     steps:
-      - uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f
+      - uses: actions/checkout@0ad4b8fadaa221de15dcec353f45205ec38ea70b
         with:
           submodules: "true"
 
       {% raw %}- name: Set up Python ${{ matrix.python-version }}{% endraw %}
         uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
         with:
           {% raw %}python-version: ${{ matrix.python-version }}{% endraw %}
@@ -47,15 +47,15 @@
   # TODO: Could we switch over to gather coverage from the normal test runs and combining
   # the result once https://github.com/nedbat/coveragepy/issues/1002 is fixed?
   upload-coverage:
     # needs: [test]
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f
+      - uses: actions/checkout@0ad4b8fadaa221de15dcec353f45205ec38ea70b
         with:
           submodules: "true"
 
       - name: Set up Python {{ DEFAULT_PY_VER }}
         uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
         with:
           python-version: "{{ DEFAULT_PY_VER }}"
@@ -66,15 +66,15 @@
           python -m pip install -r {{ NOX_DEP_PATH }}
 
       - name: Record coverage
         run: |
           python -m nox -s test-coverage
 
       - name: Upload coverage
-        uses: paambaati/codeclimate-action@a1831d7162ea1fbc612ffe5fb3b90278b7999d59
+        uses: paambaati/codeclimate-action@b74bb25d2074a4bc16bd06fffc1b299c07b1f886
         env:
           CC_TEST_REPORTER_ID: {{ CODECLIMATE_TOKEN }}
         with:
           coverageLocations: .coverage.xml:coverage.py
 
       - name: Archive coverage
         uses: actions/upload-artifact@65462800fd760344b1a7b4382951275a0abb4808
```

### Comparing `alluka-0.1.5/piped/github/actions/reformat.yml` & `alluka-0.2.0/piped/github/actions/rustfmt.yml`

 * *Files 19% similar despite different names*

```diff
@@ -1,39 +1,44 @@
-name: Reformat PR code
+name: Run Rustfmt
 
 concurrency:
   {% raw %}group: ${{ github.workflow }}-${{ github.ref }}{% endraw %}
   cancel-in-progress: true
 
-on:
-  pull_request:
-    branches:
-      - master
+on: pull_request
 
 jobs:
-  reformat:
+  rustfmt:
     runs-on: ubuntu-latest
-
     steps:
-      - uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f
+      - uses: actions/checkout@0ad4b8fadaa221de15dcec353f45205ec38ea70b
         with:
           submodules: "true"
 
       - name: Set up Python {{ DEFAULT_PY_VER }}
         uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
         with:
           python-version: "{{ DEFAULT_PY_VER }}"
 
       - name: install prerequisites
         run: |
           python -m pip install --upgrade pip wheel
-          python -m pip install -r {{ NOX_DEP_PATH }}
+          python -m pip install -r ./piped/python/base-requirements/nox.txt
+
+      - uses: actions-rs/toolchain@16499b5e05bf2e26879000db0c1d13f7e13fa3af
+        with:
+            toolchain: nightly
+            components: rustfmt
+            override: true
 
       - name: Reformat
-        run: python -m nox -s reformat bot-package-diff
+        run: cargo +nightly fmt
+
+      - name: Package
+        run: python -m nox -s bot-package-diff
 
       - uses: actions/upload-artifact@65462800fd760344b1a7b4382951275a0abb4808
         with:
           name: gogo.patch
           path: gogo.patch
 
       - name: Check diff file
```

### Comparing `alluka-0.1.5/piped/github/actions/release-docs.yml` & `alluka-0.2.0/piped/github/actions/release-docs.yml`

 * *Files 16% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     branches: [{{ BRANCH_PUSHES | join(", ") }}]{% endif %}
 
 jobs:
   publish-docs:
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f
+      - uses: actions/checkout@0ad4b8fadaa221de15dcec353f45205ec38ea70b
         with:
           submodules: "true"
 
       - name: Set up Python {{ DEFAULT_PY_VER }}
         uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
         with:
           python-version: "{{ DEFAULT_PY_VER }}"
```

### Comparing `alluka-0.1.5/piped/github/actions/resync-piped.yml` & `alluka-0.2.0/piped/github/actions/resync-piped.yml`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     paths: [{{ FILTERS | map("quoted") | join(", ") }}]
 
 jobs:
   resync-piped:
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f
+      - uses: actions/checkout@0ad4b8fadaa221de15dcec353f45205ec38ea70b
         with:
           submodules: "true"
 
       - name: Set up Python {{ DEFAULT_PY_VER }}
         uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
         with:
           python-version: "{{ DEFAULT_PY_VER }}"
```

### Comparing `alluka-0.1.5/piped/github/actions/rustfmt.yml` & `alluka-0.2.0/piped/.github/workflows/resync-piped.yml`

 * *Files 24% similar despite different names*

```diff
@@ -1,44 +1,40 @@
-name: Run Rustfmt
+name: Resync piped
 
 concurrency:
-  {% raw %}group: ${{ github.workflow }}-${{ github.ref }}{% endraw %}
+  group: ${{ github.workflow }}-${{ github.ref }}
   cancel-in-progress: true
 
-on: pull_request
+on:
+  pull_request:
+    branches:
+      - master
+    paths: ["github/actions/*", "pyproject.toml"]
 
 jobs:
-  rustfmt:
+  resync-piped:
     runs-on: ubuntu-latest
+
     steps:
-      - uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f
+      - uses: actions/checkout@0ad4b8fadaa221de15dcec353f45205ec38ea70b
         with:
           submodules: "true"
 
-      - name: Set up Python {{ DEFAULT_PY_VER }}
+      - name: Set up Python 3.11
         uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
         with:
-          python-version: "{{ DEFAULT_PY_VER }}"
+          python-version: "3.11"
 
       - name: install prerequisites
         run: |
           python -m pip install --upgrade pip wheel
-          python -m pip install -r ./piped/python/base-requirements/nox.txt
-
-      - uses: actions-rs/toolchain@16499b5e05bf2e26879000db0c1d13f7e13fa3af
-        with:
-            toolchain: nightly
-            components: rustfmt
-            override: true
-
-      - name: Reformat
-        run: cargo +nightly fmt
+          python -m pip install -r ./python/base-requirements/nox.txt
 
-      - name: Package
-        run: python -m nox -s bot-package-diff
+      - name: Resync Piped
+        run: python -m nox -s copy-piped bot-package-diff
 
       - uses: actions/upload-artifact@65462800fd760344b1a7b4382951275a0abb4808
         with:
           name: gogo.patch
           path: gogo.patch
 
       - name: Check diff file
```

### Comparing `alluka-0.1.5/piped/github/actions/type-check.yml` & `alluka-0.2.0/piped/github/actions/type-check.yml`

 * *Files 17% similar despite different names*

```diff
@@ -16,15 +16,15 @@
   workflow_dispatch:
 
 jobs:
   type-check:
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f
+      - uses: actions/checkout@0ad4b8fadaa221de15dcec353f45205ec38ea70b
         with:
           submodules: "true"
 
       - name: Set up Python {{ DEFAULT_PY_VER }}
         uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
         with:
           python-version: "{{ DEFAULT_PY_VER }}"
```

### Comparing `alluka-0.1.5/piped/github/actions/update-licence.yml` & `alluka-0.2.0/piped/github/actions/update-licence.yml`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   workflow_dispatch:
 
 jobs:
   update-licence:
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f
+      - uses: actions/checkout@0ad4b8fadaa221de15dcec353f45205ec38ea70b
         with:
           submodules: "true"
 
       - name: Set up Python {{ DEFAULT_PY_VER }}
         uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
         with:
           python-version: "{{ DEFAULT_PY_VER }}"
@@ -24,15 +24,15 @@
           python -m pip install --upgrade pip wheel
           python -m pip install -r {{ NOX_DEP_PATH }}
 
       - name: Update licence
         run: python -m nox -s update-licence
 
       - name: Create Pull Request
-        uses: peter-evans/create-pull-request@9153d834b60caba6d51c9b9510b087acf9f33f83
+        uses: peter-evans/create-pull-request@6d6857d36972b65feb161a90e484f2984215f83e
         with:
           author: "{{ ACTION_COMMITTER_USERNAME }} <{{ ACTION_COMMITTER_EMAIL }}>"
           branch: task/update-licence
           commit-message: Update licence
           committer: "{{ ACTION_COMMITTER_USERNAME }} <{{ ACTION_COMMITTER_EMAIL }}>"
           title: Update licence
           {% raw %}token: ${{ secrets.ACTIONS_TOKEN || secrets.GITHUB_TOKEN }}{% endraw %}
```

### Comparing `alluka-0.1.5/piped/github/actions/upgrade-locks.yml` & `alluka-0.2.0/piped/github/actions/upgrade-locks.yml`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   workflow_dispatch:
 
 jobs:
   upgrade-deps:
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f
+      - uses: actions/checkout@0ad4b8fadaa221de15dcec353f45205ec38ea70b
         with:
           submodules: "true"
 
       - name: Set up Python {{ DEFAULT_PY_VER }}
         uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
         with:
           python-version: "{{ DEFAULT_PY_VER }}"
@@ -24,15 +24,15 @@
           python -m pip install --upgrade pip wheel
           python -m pip install -r {{ NOX_DEP_PATH }}
 
       - name: Upgrade dependency locks
         run: python -m nox -s freeze-locks
 
       - name: Create Pull Request
-        uses: peter-evans/create-pull-request@9153d834b60caba6d51c9b9510b087acf9f33f83
+        uses: peter-evans/create-pull-request@6d6857d36972b65feb161a90e484f2984215f83e
         with:
           author: "{{ ACTION_COMMITTER_USERNAME }} <{{ ACTION_COMMITTER_EMAIL }}>"
           branch: task/upgrade-deps
           commit-message: Upgrade dependency locks
           committer: "{{ ACTION_COMMITTER_USERNAME }} <{{ ACTION_COMMITTER_EMAIL }}>"
           title: Upgrade dependency locks
           {% raw %}token: ${{ secrets.ACTIONS_TOKEN || secrets.GITHUB_TOKEN }}{% endraw %}
```

### Comparing `alluka-0.1.5/piped/github/actions/verify-locks.yml` & `alluka-0.2.0/piped/github/actions/verify-locks.yml`

 * *Files 21% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     paths: [{{ (FILTERS + EXTEND_FILTERS) | map("quoted") | join(", ") }}]
 
 jobs:
   verify-pr-dep-changes:
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f
+      - uses: actions/checkout@0ad4b8fadaa221de15dcec353f45205ec38ea70b
         with:
           submodules: "true"
 
       - name: Set up Python {{ DEFAULT_PY_VER }}
         uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
         with:
           python-version: "{{ DEFAULT_PY_VER }}"
```

### Comparing `alluka-0.1.5/piped/github/actions/verify-types.yml` & `alluka-0.2.0/piped/github/actions/clippy.yml`

 * *Files 25% similar despite different names*

```diff
@@ -1,38 +1,31 @@
-name: Verify type-completeness
+name: Run clippy
 
 concurrency:
   {% raw %}group: ${{ github.workflow }}-${{ github.ref }}{% endraw %}
   cancel-in-progress: true
 
 on:
   push:
-    branches:
-      - master
+    branches: [ master ]
   pull_request:
-    branches:
-      - master
+    branches: [ master ]
   schedule:
     - cron: "0 12 * * 6"
   workflow_dispatch:
 
 jobs:
-  verify-types:
+  clippy:
     runs-on: ubuntu-latest
-
     steps:
-      - uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f
-        with:
-          submodules: "true"
+      - uses: actions/checkout@0ad4b8fadaa221de15dcec353f45205ec38ea70b
 
-      - name: Set up Python {{ DEFAULT_PY_VER }}
-        uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
+      - uses: actions-rs/toolchain@16499b5e05bf2e26879000db0c1d13f7e13fa3af
         with:
-          python-version: "{{ DEFAULT_PY_VER }}"
+            toolchain: nightly
+            components: clippy
+            override: true
 
-      - name: install prerequisites
-        run: |
-          python -m pip install --upgrade pip wheel
-          python -m pip install -r {{ NOX_DEP_PATH }}
-
-      - name: Run verify types
-        run: python -m nox -s verify-types
+      - uses: actions-rs/clippy-check@b5b5f21f4797c02da247df37026fcd0a5024aa4d
+        with:
+          {% raw %}token: ${{ secrets.GITHUB_TOKEN }}{% endraw %}
+          args: --all-features
```

### Comparing `alluka-0.1.5/piped/github/dependabot.yml` & `alluka-0.2.0/piped/github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `alluka-0.1.5/piped/github/pull_request_template.md` & `alluka-0.2.0/piped/github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `alluka-0.1.5/piped/noxfile.py` & `alluka-0.2.0/piped/noxfile.py`

 * *Files identical despite different names*

### Comparing `alluka-0.1.5/piped/pyproject.toml` & `alluka-0.2.0/piped/pyproject.toml`

 * *Files identical despite different names*

### Comparing `alluka-0.1.5/piped/python/base-requirements/docs.txt` & `alluka-0.2.0/piped/python/base-requirements/freeze-locks.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,75 @@
 #
 # This file is autogenerated by pip-compile-cross-platform
 # To update, run:
 #
-#    pip-compile-cross-platform python/base-requirements/docs.in --output-file python/base-requirements/docs.txt --min-python-version 3.9
+#    pip-compile-cross-platform python/base-requirements/freeze-locks.in --output-file python/base-requirements/freeze-locks.txt --min-python-version 3.9
 #
-babel==2.14.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:6919867db036398ba21eb5c7a0f6b28ab8cbc3ae7a73a44ebe34ae74a4e7d363 \
-    --hash=sha256:efb1a25b7118e67ce3a259bed20545c29cb68be8ad2c784c83689981b7a57287
+build==1.2.1 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:526263f4870c26f26c433545579475377b2b7588b6f1eac76a001e873ae3e19d \
+    --hash=sha256:75e10f767a433d9a86e50d83f418e83efc18ede923ee5ff7df93b6cb0306c5d4
+cachecontrol[filecache]==0.14.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:7db1195b41c81f8274a7bbd97c956f44e8348265a1bc7641c37dfebc39f0c938 \
+    --hash=sha256:f5bf3f0620c38db2e5122c0726bdebb0d16869de966ea6a2befe92470b740ea0
 certifi==2024.2.2 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:0569859f95fc761b18b45ef421b1290a0f65f147e92a1e5eb3e635f9a5e4e66f \
     --hash=sha256:dc383c07b76109f368f6106eee2b593b04a011ea4d55f652c6ca24a754d1cdd1
+cffi==1.16.0 ; python_version >= "3.9" and python_version < "4.0" and (sys_platform == "darwin" or sys_platform == "linux") and (sys_platform == "darwin" or platform_python_implementation != "PyPy") \
+    --hash=sha256:0c9ef6ff37e974b73c25eecc13952c55bceed9112be2d9d938ded8e856138bcc \
+    --hash=sha256:131fd094d1065b19540c3d72594260f118b231090295d8c34e19a7bbcf2e860a \
+    --hash=sha256:1b8ebc27c014c59692bb2664c7d13ce7a6e9a629be20e54e7271fa696ff2b417 \
+    --hash=sha256:2c56b361916f390cd758a57f2e16233eb4f64bcbeee88a4881ea90fca14dc6ab \
+    --hash=sha256:2d92b25dbf6cae33f65005baf472d2c245c050b1ce709cc4588cdcdd5495b520 \
+    --hash=sha256:31d13b0f99e0836b7ff893d37af07366ebc90b678b6664c955b54561fc36ef36 \
+    --hash=sha256:32c68ef735dbe5857c810328cb2481e24722a59a2003018885514d4c09af9743 \
+    --hash=sha256:3686dffb02459559c74dd3d81748269ffb0eb027c39a6fc99502de37d501faa8 \
+    --hash=sha256:582215a0e9adbe0e379761260553ba11c58943e4bbe9c36430c4ca6ac74b15ed \
+    --hash=sha256:5b50bf3f55561dac5438f8e70bfcdfd74543fd60df5fa5f62d94e5867deca684 \
+    --hash=sha256:5bf44d66cdf9e893637896c7faa22298baebcd18d1ddb6d2626a6e39793a1d56 \
+    --hash=sha256:6602bc8dc6f3a9e02b6c22c4fc1e47aa50f8f8e6d3f78a5e16ac33ef5fefa324 \
+    --hash=sha256:673739cb539f8cdaa07d92d02efa93c9ccf87e345b9a0b556e3ecc666718468d \
+    --hash=sha256:68678abf380b42ce21a5f2abde8efee05c114c2fdb2e9eef2efdb0257fba1235 \
+    --hash=sha256:68e7c44931cc171c54ccb702482e9fc723192e88d25a0e133edd7aff8fcd1f6e \
+    --hash=sha256:6b3d6606d369fc1da4fd8c357d026317fbb9c9b75d36dc16e90e84c26854b088 \
+    --hash=sha256:748dcd1e3d3d7cd5443ef03ce8685043294ad6bd7c02a38d1bd367cfd968e000 \
+    --hash=sha256:7651c50c8c5ef7bdb41108b7b8c5a83013bfaa8a935590c5d74627c047a583c7 \
+    --hash=sha256:7b78010e7b97fef4bee1e896df8a4bbb6712b7f05b7ef630f9d1da00f6444d2e \
+    --hash=sha256:7e61e3e4fa664a8588aa25c883eab612a188c725755afff6289454d6362b9673 \
+    --hash=sha256:80876338e19c951fdfed6198e70bc88f1c9758b94578d5a7c4c91a87af3cf31c \
+    --hash=sha256:8895613bcc094d4a1b2dbe179d88d7fb4a15cee43c052e8885783fac397d91fe \
+    --hash=sha256:88e2b3c14bdb32e440be531ade29d3c50a1a59cd4e51b1dd8b0865c54ea5d2e2 \
+    --hash=sha256:8f8e709127c6c77446a8c0a8c8bf3c8ee706a06cd44b1e827c3e6a2ee6b8c098 \
+    --hash=sha256:9cb4a35b3642fc5c005a6755a5d17c6c8b6bcb6981baf81cea8bfbc8903e8ba8 \
+    --hash=sha256:9f90389693731ff1f659e55c7d1640e2ec43ff725cc61b04b2f9c6d8d017df6a \
+    --hash=sha256:a09582f178759ee8128d9270cd1344154fd473bb77d94ce0aeb2a93ebf0feaf0 \
+    --hash=sha256:a6a14b17d7e17fa0d207ac08642c8820f84f25ce17a442fd15e27ea18d67c59b \
+    --hash=sha256:a72e8961a86d19bdb45851d8f1f08b041ea37d2bd8d4fd19903bc3083d80c896 \
+    --hash=sha256:abd808f9c129ba2beda4cfc53bde801e5bcf9d6e0f22f095e45327c038bfe68e \
+    --hash=sha256:ac0f5edd2360eea2f1daa9e26a41db02dd4b0451b48f7c318e217ee092a213e9 \
+    --hash=sha256:b29ebffcf550f9da55bec9e02ad430c992a87e5f512cd63388abb76f1036d8d2 \
+    --hash=sha256:b2ca4e77f9f47c55c194982e10f058db063937845bb2b7a86c84a6cfe0aefa8b \
+    --hash=sha256:b7be2d771cdba2942e13215c4e340bfd76398e9227ad10402a8767ab1865d2e6 \
+    --hash=sha256:b84834d0cf97e7d27dd5b7f3aca7b6e9263c56308ab9dc8aae9784abb774d404 \
+    --hash=sha256:b86851a328eedc692acf81fb05444bdf1891747c25af7529e39ddafaf68a4f3f \
+    --hash=sha256:bcb3ef43e58665bbda2fb198698fcae6776483e0c4a631aa5647806c25e02cc0 \
+    --hash=sha256:c0f31130ebc2d37cdd8e44605fb5fa7ad59049298b3f745c74fa74c62fbfcfc4 \
+    --hash=sha256:c6a164aa47843fb1b01e941d385aab7215563bb8816d80ff3a363a9f8448a8dc \
+    --hash=sha256:d8a9d3ebe49f084ad71f9269834ceccbf398253c9fac910c4fd7053ff1386936 \
+    --hash=sha256:db8e577c19c0fda0beb7e0d4e09e0ba74b1e4c092e0e40bfa12fe05b6f6d75ba \
+    --hash=sha256:dc9b18bf40cc75f66f40a7379f6a9513244fe33c0e8aa72e2d56b0196a7ef872 \
+    --hash=sha256:e09f3ff613345df5e8c3667da1d918f9149bd623cd9070c983c013792a9a62eb \
+    --hash=sha256:e4108df7fe9b707191e55f33efbcb2d81928e10cea45527879a4749cbe472614 \
+    --hash=sha256:e6024675e67af929088fda399b2094574609396b1decb609c55fa58b028a32a1 \
+    --hash=sha256:e70f54f1796669ef691ca07d046cd81a29cb4deb1e5f942003f401c0c4a2695d \
+    --hash=sha256:e715596e683d2ce000574bae5d07bd522c781a822866c20495e52520564f0969 \
+    --hash=sha256:e760191dd42581e023a68b758769e2da259b5d52e3103c6060ddc02c9edb8d7b \
+    --hash=sha256:ed86a35631f7bfbb28e108dd96773b9d5a6ce4811cf6ea468bb6a359b256b1e4 \
+    --hash=sha256:ee07e47c12890ef248766a6e55bd38ebfb2bb8edd4142d56db91b21ea68b7627 \
+    --hash=sha256:fa3a0128b152627161ce47201262d3140edb5a5c3da88d73a1b790a959126956 \
+    --hash=sha256:fcc8eb6d5902bb1cf6dc4f187ee3ea80a1eba0a89aba40a5cb20a5087d961357
 charset-normalizer==3.3.2 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:06435b539f889b1f6f4ac1758871aae42dc3a8c0e24ac9e60c2384973ad73027 \
     --hash=sha256:06a81e93cd441c56a9b65d8e1d043daeb97a3d0856d177d5c90ba85acb3db087 \
     --hash=sha256:0a55554a2fa0d408816b3b5cedf0045f4b8e1a6065aec45849de2d6f3f8e9786 \
     --hash=sha256:0b2b64d2bb6d3fb9112bafa732def486049e63de9618b5843bcdd081d8144cd8 \
     --hash=sha256:10955842570876604d404661fbccbc9c7e684caf432c09c715ec38fbae45ae09 \
     --hash=sha256:122c7fa62b130ed55f8f285bfd56d5f4b4a5b503609d181f9ad85e55c89f4185 \
@@ -97,342 +153,428 @@
     --hash=sha256:eb8821e09e916165e160797a6c17edda0679379a4be5c716c260e836e122f54b \
     --hash=sha256:efcb3f6676480691518c177e3b465bcddf57cea040302f9f4e6e191af91174d4 \
     --hash=sha256:f27273b60488abe721a075bcca6d7f3964f9f6f067c8c4c605743023d7d3944f \
     --hash=sha256:f30c3cb33b24454a82faecaf01b19c18562b1e89558fb6c56de4d9118a032fd5 \
     --hash=sha256:fb69256e180cb6c8a894fee62b3afebae785babc1ee98b81cdf68bbca1987f33 \
     --hash=sha256:fd1abc0d89e30cc4e02e4064dc67fcc51bd941eb395c502aac3ec19fab46b519 \
     --hash=sha256:ff8fa367d09b717b2a17a052544193ad76cd49979c805768879cb63d9ca50561
-click==8.1.7 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:ae74fb96c20a0277a1d615f1e4d73c8414f5a98db8b799a7931d1582f3390c28 \
-    --hash=sha256:ca9853ad459e787e2192211578cc907e7594e294c7ccc834310722b41b9ca6de
-colorama==0.4.6 ; python_version >= "3.9" and python_version < "4.0" \
+cleo==2.1.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:0b2c880b5d13660a7ea651001fb4acb527696c01f15c9ee650f377aa543fd523 \
+    --hash=sha256:4a31bd4dd45695a64ee3c4758f583f134267c2bc518d8ae9a29cf237d009b07e
+colorama==0.4.6 ; python_version >= "3.9" and python_version < "4.0" and os_name == "nt" \
     --hash=sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44 \
     --hash=sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6
-csscompressor==0.9.5 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:afa22badbcf3120a4f392e4d22f9fff485c044a1feda4a950ecc5eba9dd31a05
-ghp-import==2.1.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:8337dd7b50877f163d4c0289bc1f1c7f127550241988d568c1db512c4324a619 \
-    --hash=sha256:9c535c4c61193c2df8871222567d7fd7e5014d835f97dc7b7439069e2413d343
-griffe==0.44.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:34aee1571042f9bf00529bc715de4516fb6f482b164e90d030300601009e0223 \
-    --hash=sha256:8a4471c469ba980b87c843f1168850ce39d0c1d0c7be140dca2480f76c8e5446
-htmlmin2==0.1.13 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:75609f2a42e64f7ce57dbff28a39890363bde9e7e5885db633317efbdf8c79a2
+crashtest==0.4.1 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:80d7b1f316ebfbd429f648076d6275c877ba30ba48979de4191714a75266f0ce \
+    --hash=sha256:8d23eac5fa660409f57472e3851dab7ac18aba459a8d19cbbba86d3d5aecd2a5
+cryptography==42.0.5 ; python_version >= "3.9" and python_version < "4.0" and sys_platform == "linux" \
+    --hash=sha256:0270572b8bd2c833c3981724b8ee9747b3ec96f699a9665470018594301439ee \
+    --hash=sha256:111a0d8553afcf8eb02a4fea6ca4f59d48ddb34497aa8706a6cf536f1a5ec576 \
+    --hash=sha256:16a48c23a62a2f4a285699dba2e4ff2d1cff3115b9df052cdd976a18856d8e3d \
+    --hash=sha256:1b95b98b0d2af784078fa69f637135e3c317091b615cd0905f8b8a087e86fa30 \
+    --hash=sha256:1f71c10d1e88467126f0efd484bd44bca5e14c664ec2ede64c32f20875c0d413 \
+    --hash=sha256:2424ff4c4ac7f6b8177b53c17ed5d8fa74ae5955656867f5a8affaca36a27abb \
+    --hash=sha256:2bce03af1ce5a5567ab89bd90d11e7bbdff56b8af3acbbec1faded8f44cb06da \
+    --hash=sha256:329906dcc7b20ff3cad13c069a78124ed8247adcac44b10bea1130e36caae0b4 \
+    --hash=sha256:37dd623507659e08be98eec89323469e8c7b4c1407c85112634ae3dbdb926fdd \
+    --hash=sha256:3eaafe47ec0d0ffcc9349e1708be2aaea4c6dd4978d76bf6eb0cb2c13636c6fc \
+    --hash=sha256:5e6275c09d2badf57aea3afa80d975444f4be8d3bc58f7f80d2a484c6f9485c8 \
+    --hash=sha256:6fe07eec95dfd477eb9530aef5bead34fec819b3aaf6c5bd6d20565da607bfe1 \
+    --hash=sha256:7367d7b2eca6513681127ebad53b2582911d1736dc2ffc19f2c3ae49997496bc \
+    --hash=sha256:7cde5f38e614f55e28d831754e8a3bacf9ace5d1566235e39d91b35502d6936e \
+    --hash=sha256:9481ffe3cf013b71b2428b905c4f7a9a4f76ec03065b05ff499bb5682a8d9ad8 \
+    --hash=sha256:98d8dc6d012b82287f2c3d26ce1d2dd130ec200c8679b6213b3c73c08b2b7940 \
+    --hash=sha256:a011a644f6d7d03736214d38832e030d8268bcff4a41f728e6030325fea3e400 \
+    --hash=sha256:a2913c5375154b6ef2e91c10b5720ea6e21007412f6437504ffea2109b5a33d7 \
+    --hash=sha256:a30596bae9403a342c978fb47d9b0ee277699fa53bbafad14706af51fe543d16 \
+    --hash=sha256:b03c2ae5d2f0fc05f9a2c0c997e1bc18c8229f392234e8a0194f202169ccd278 \
+    --hash=sha256:b6cd2203306b63e41acdf39aa93b86fb566049aeb6dc489b70e34bcd07adca74 \
+    --hash=sha256:b7ffe927ee6531c78f81aa17e684e2ff617daeba7f189f911065b2ea2d526dec \
+    --hash=sha256:b8cac287fafc4ad485b8a9b67d0ee80c66bf3574f655d3b97ef2e1082360faf1 \
+    --hash=sha256:ba334e6e4b1d92442b75ddacc615c5476d4ad55cc29b15d590cc6b86efa487e2 \
+    --hash=sha256:ba3e4a42397c25b7ff88cdec6e2a16c2be18720f317506ee25210f6d31925f9c \
+    --hash=sha256:c41fb5e6a5fe9ebcd58ca3abfeb51dffb5d83d6775405305bfa8715b76521922 \
+    --hash=sha256:cd2030f6650c089aeb304cf093f3244d34745ce0cfcc39f20c6fbfe030102e2a \
+    --hash=sha256:cd65d75953847815962c84a4654a84850b2bb4aed3f26fadcc1c13892e1e29f6 \
+    --hash=sha256:e4985a790f921508f36f81831817cbc03b102d643b5fcb81cd33df3fa291a1a1 \
+    --hash=sha256:e807b3188f9eb0eaa7bbb579b462c5ace579f1cedb28107ce8b48a9f7ad3679e \
+    --hash=sha256:f12764b8fffc7a123f641d7d049d382b73f96a34117e0b637b80643169cec8ac \
+    --hash=sha256:f8837fe1d6ac4a8052a9a8ddab256bc006242696f03368a4009be7ee3075cdb7
+distlib==0.3.8 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:034db59a0b96f8ca18035f36290806a9a6e6bd9d1ff91e45a7f172eb17e51784 \
+    --hash=sha256:1530ea13e350031b6312d8580ddb6b27a104275a31106523b8f123787f494f64
+dulwich==0.21.7 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:0fc3078a1ba04c588fabb0969d3530efd5cd1ce2cf248eefb6baf7cbc15fc285 \
+    --hash=sha256:10893105c6566fc95bc2a67b61df7cc1e8f9126d02a1df6a8b2b82eb59db8ab9 \
+    --hash=sha256:12d61334a575474e707614f2e93d6ed4cdae9eb47214f9277076d9e5615171d3 \
+    --hash=sha256:2590e9b431efa94fc356ae33b38f5e64f1834ec3a94a6ac3a64283b206d07aa3 \
+    --hash=sha256:25c3ab8fb2e201ad2031ddd32e4c68b7c03cb34b24a5ff477b7a7dcef86372f5 \
+    --hash=sha256:274c18ec3599a92a9b67abaf110e4f181a4f779ee1aaab9e23a72e89d71b2bd9 \
+    --hash=sha256:29bb5c1d70eba155ded41ed8a62be2f72edbb3c77b08f65b89c03976292f6d1b \
+    --hash=sha256:2bc12697f0918bee324c18836053644035362bb3983dc1b210318f2fed1d7132 \
+    --hash=sha256:2e2c66888207b71cd1daa2acb06d3984a6bc13787b837397a64117aa9fc5936a \
+    --hash=sha256:404b8edeb3c3a86c47c0a498699fc064c93fa1f8bab2ffe919e8ab03eafaaad3 \
+    --hash=sha256:40dcbd29ba30ba2c5bfbab07a61a5f20095541d5ac66d813056c122244df4ac0 \
+    --hash=sha256:460b3849d5c3d3818a80743b4f7a0094c893c559f678e56a02fff570b49a644a \
+    --hash=sha256:460ba74bdb19f8d498786ae7776745875059b1178066208c0fd509792d7f7bfc \
+    --hash=sha256:4637cbd8ed1012f67e1068aaed19fcc8b649bcf3e9e26649826a303298c89b9d \
+    --hash=sha256:471305af74790827fcbafe330fc2e8bdcee4fb56ca1177c8c481b1c8f806c4a4 \
+    --hash=sha256:4a043b90958cec866b4edc6aef5fe3c2c96a664d0b357e1682a46f6c477273c4 \
+    --hash=sha256:4b09bc3a64fb70132ec14326ecbe6e0555381108caff3496898962c4136a48c6 \
+    --hash=sha256:4bc4c5366eaf26dda3fdffe160a3b515666ed27c2419f1d483da285ac1411de0 \
+    --hash=sha256:4c51058ec4c0b45dc5189225b9e0c671b96ca9713c1daf71d622c13b0ab07681 \
+    --hash=sha256:4f18f0a311fb7734b033a3101292b932158cade54b74d1c44db519e42825e5a2 \
+    --hash=sha256:61e3451bd3d3844f2dca53f131982553be4d1b1e1ebd9db701843dd76c4dba31 \
+    --hash=sha256:62bfb26bdce869cd40be443dfd93143caea7089b165d2dcc33de40f6ac9d812a \
+    --hash=sha256:675a612ce913081beb0f37b286891e795d905691dfccfb9bf73721dca6757cde \
+    --hash=sha256:6bd69921fdd813b7469a3c77bc75c1783cc1d8d72ab15a406598e5a3ba1a1503 \
+    --hash=sha256:6c589468e5c0cd84e97eb7ec209ab005a2cb69399e8c5861c3edfe38989ac3a8 \
+    --hash=sha256:6de6f8de4a453fdbae8062a6faa652255d22a3d8bce0cd6d2d6701305c75f2b3 \
+    --hash=sha256:739b191f61e1c4ce18ac7d520e7a7cbda00e182c3489552408237200ce8411ad \
+    --hash=sha256:74700e4c7d532877355743336c36f51b414d01e92ba7d304c4f8d9a5946dbc81 \
+    --hash=sha256:7836da3f4110ce684dcd53489015fb7fa94ed33c5276e3318b8b1cbcb5b71e08 \
+    --hash=sha256:7bca4b86e96d6ef18c5bc39828ea349efb5be2f9b1f6ac9863f90589bac1084d \
+    --hash=sha256:7d8ab29c660125db52106775caa1f8f7f77a69ed1fe8bc4b42bdf115731a25bf \
+    --hash=sha256:808e8b9cc0aa9ac74870b49db4f9f39a52fb61694573f84b9c0613c928d4caf8 \
+    --hash=sha256:817822f970e196e757ae01281ecbf21369383285b9f4a83496312204cf889b8c \
+    --hash=sha256:8278835e168dd097089f9e53088c7a69c6ca0841aef580d9603eafe9aea8c358 \
+    --hash=sha256:858842b30ad6486aacaa607d60bab9c9a29e7c59dc2d9cb77ae5a94053878c08 \
+    --hash=sha256:869eb7be48243e695673b07905d18b73d1054a85e1f6e298fe63ba2843bb2ca1 \
+    --hash=sha256:8869fc8ec3dda743e03d06d698ad489b3705775fe62825e00fa95aa158097fc0 \
+    --hash=sha256:8929c37986c83deb4eb500c766ee28b6670285b512402647ee02a857320e377c \
+    --hash=sha256:a0650ec77d89cb947e3e4bbd4841c96f74e52b4650830112c3057a8ca891dc2f \
+    --hash=sha256:a7b5624b02ef808cdc62dabd47eb10cd4ac15e8ac6df9e2e88b6ac6b40133673 \
+    --hash=sha256:a9e9c66833cea580c3ac12927e4b9711985d76afca98da971405d414de60e968 \
+    --hash=sha256:b0d2e4485b98695bf95350ce9d38b1bb0aaac2c34ad00a0df789aa33c934469b \
+    --hash=sha256:c01a735b9a171dcb634a97a3cec1b174cfbfa8e840156870384b633da0460f18 \
+    --hash=sha256:c3a539b4696a42fbdb7412cb7b66a4d4d332761299d3613d90a642923c7560e1 \
+    --hash=sha256:c3d1685f320907a52c40fd5890627945c51f3a5fa4bcfe10edb24fec79caadec \
+    --hash=sha256:c92e72c43c9e9e936b01a57167e0ea77d3fd2d82416edf9489faa87278a1cdf7 \
+    --hash=sha256:cc1e11be527ac06316539b57a7688bcb1b6a3e53933bc2f844397bc50734e9ae \
+    --hash=sha256:ce8db196e79c1f381469410d26fb1d8b89c6b87a4e7f00ff418c22a35121405c \
+    --hash=sha256:d05d3c781bc74e2c2a2a8f4e4e2ed693540fbe88e6ac36df81deac574a6dad99 \
+    --hash=sha256:d097e963eb6b9fa53266146471531ad9c6765bf390849230311514546ed64db2 \
+    --hash=sha256:d4a2d76c96426e791556836ef43542b639def81be4f1d6d4322cd886c115eae1 \
+    --hash=sha256:d4c0110798099bb7d36a110090f2688050703065448895c4f53ade808d889dd3 \
+    --hash=sha256:d54c9d0e845be26f65f954dff13a1cd3f2b9739820c19064257b8fd7435ab263 \
+    --hash=sha256:d5882e70b74ac3c736a42d3fdd4f5f2e6570637f59ad5d3e684760290b58f041 \
+    --hash=sha256:d62446797163317a397a10080c6397ffaaca51a7804c0120b334f8165736c56a \
+    --hash=sha256:d96ca5e0dde49376fbcb44f10eddb6c30284a87bd03bb577c59bb0a1f63903fa \
+    --hash=sha256:e0064363bd5e814359657ae32517fa8001e8573d9d040bd997908d488ab886ed \
+    --hash=sha256:e138d516baa6b5bafbe8f030eccc544d0d486d6819b82387fc0e285e62ef5261 \
+    --hash=sha256:e1957b65f96e36c301e419d7adaadcff47647c30eb072468901bb683b1000bc5 \
+    --hash=sha256:e25953c7acbbe4e19650d0225af1c0c0e6882f8bddd2056f75c1cc2b109b88ad \
+    --hash=sha256:e274cebaf345f0b1e3b70197f2651de92b652386b68020cfd3bf61bc30f6eaaa \
+    --hash=sha256:e598d743c6c0548ebcd2baf94aa9c8bfacb787ea671eeeb5828cfbd7d56b552f \
+    --hash=sha256:e84cc606b1f581733df4350ca4070e6a8b30be3662bbb81a590b177d0c996c91 \
+    --hash=sha256:ecd315847dea406a4decfa39d388a2521e4e31acde3bd9c2609c989e817c6d62 \
+    --hash=sha256:ed60d1f610ef6437586f7768254c2a93820ccbd4cfdac7d182cf2d6e615969bb \
+    --hash=sha256:f34bf9b9fa9308376263fd9ac43143c7c09da9bc75037bb75c6c2423a151b92c \
+    --hash=sha256:f6c88acb60a1f4d31bd6d13bfba465853b3df940ee4a0f2a3d6c7a0778c705b7 \
+    --hash=sha256:fa4d14767cf7a49c9231c2e52cb2a3e90d0c83f843eb6a2ca2b5d81d254cf6b9 \
+    --hash=sha256:ffc27fb063f740712e02b4d2f826aee8bbed737ed799962fef625e2ce56e2d29
+fastjsonschema==2.19.1 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:3672b47bc94178c9f23dbb654bf47440155d4db9df5f7bc47643315f9c405cd0 \
+    --hash=sha256:e3126a94bdc4623d3de4485f8d468a12f02a67921315ddc87836d6e456dc789d
+filelock==3.13.4 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:404e5e9253aa60ad457cae1be07c0f0ca90a63931200a47d9b6a6af84fd7b45f \
+    --hash=sha256:d13f466618bfde72bd2c18255e269f72542c6e70e7bac83a0232d6b1cc5c8cf4
 idna==3.7 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:028ff3aadf0609c1fd278d8ea3089299412a7a8b9bd005dd08b9f8285bcb5cfc \
     --hash=sha256:82fee1fc78add43492d3a1898bfa6d8a904cc97d8427f683ed8e798d07761aa0
-importlib-metadata==7.1.0 ; python_version >= "3.9" and python_version < "3.10" \
+importlib-metadata==7.1.0 ; python_version >= "3.9" and python_version < "3.12" \
     --hash=sha256:30962b96c0c223483ed6cc7280e7f0199feb01a0e40cfae4d4450fc6fab1f570 \
     --hash=sha256:b78938b926ee8d5f020fc4772d487045805a55ddbad2ecf21c6d60938dc7fcd2
-jinja2==3.1.3 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:7d6d50dd97d52cbc355597bd845fabfbac3f551e1f99619e39a35ce8c370b5fa \
-    --hash=sha256:ac8bd6544d4bb2c9792bf3a159e80bba8fda7f07e81bc3aed565432d5925ba90
-jsmin==3.0.1 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:c0959a121ef94542e807a674142606f7e90214a2b3d1eb17300244bbb5cc2bfc
-markdown-include==0.8.1 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:1d0623e0fc2757c38d35df53752768356162284259d259c486b4ab6285cdbbe3 \
-    --hash=sha256:32f0635b9cfef46997b307e2430022852529f7a5b87c0075c504283e7cc7db53
-markdown==3.6 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:48f276f4d8cfb8ce6527c8f79e2ee29708508bf4d40aa410fbc3b4ee832c850f \
-    --hash=sha256:ed4f41f6daecbeeb96e576ce414c41d2d876daa9a16cb35fa8ed8c2ddfad0224
-markupsafe==2.1.5 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:00e046b6dd71aa03a41079792f8473dc494d564611a8f89bbbd7cb93295ebdcf \
-    --hash=sha256:075202fa5b72c86ad32dc7d0b56024ebdbcf2048c0ba09f1cde31bfdd57bcfff \
-    --hash=sha256:0e397ac966fdf721b2c528cf028494e86172b4feba51d65f81ffd65c63798f3f \
-    --hash=sha256:17b950fccb810b3293638215058e432159d2b71005c74371d784862b7e4683f3 \
-    --hash=sha256:1f3fbcb7ef1f16e48246f704ab79d79da8a46891e2da03f8783a5b6fa41a9532 \
-    --hash=sha256:2174c595a0d73a3080ca3257b40096db99799265e1c27cc5a610743acd86d62f \
-    --hash=sha256:2b7c57a4dfc4f16f7142221afe5ba4e093e09e728ca65c51f5620c9aaeb9a617 \
-    --hash=sha256:2d2d793e36e230fd32babe143b04cec8a8b3eb8a3122d2aceb4a371e6b09b8df \
-    --hash=sha256:30b600cf0a7ac9234b2638fbc0fb6158ba5bdcdf46aeb631ead21248b9affbc4 \
-    --hash=sha256:397081c1a0bfb5124355710fe79478cdbeb39626492b15d399526ae53422b906 \
-    --hash=sha256:3a57fdd7ce31c7ff06cdfbf31dafa96cc533c21e443d57f5b1ecc6cdc668ec7f \
-    --hash=sha256:3c6b973f22eb18a789b1460b4b91bf04ae3f0c4234a0a6aa6b0a92f6f7b951d4 \
-    --hash=sha256:3e53af139f8579a6d5f7b76549125f0d94d7e630761a2111bc431fd820e163b8 \
-    --hash=sha256:4096e9de5c6fdf43fb4f04c26fb114f61ef0bf2e5604b6ee3019d51b69e8c371 \
-    --hash=sha256:4275d846e41ecefa46e2015117a9f491e57a71ddd59bbead77e904dc02b1bed2 \
-    --hash=sha256:4c31f53cdae6ecfa91a77820e8b151dba54ab528ba65dfd235c80b086d68a465 \
-    --hash=sha256:4f11aa001c540f62c6166c7726f71f7573b52c68c31f014c25cc7901deea0b52 \
-    --hash=sha256:5049256f536511ee3f7e1b3f87d1d1209d327e818e6ae1365e8653d7e3abb6a6 \
-    --hash=sha256:58c98fee265677f63a4385256a6d7683ab1832f3ddd1e66fe948d5880c21a169 \
-    --hash=sha256:598e3276b64aff0e7b3451b72e94fa3c238d452e7ddcd893c3ab324717456bad \
-    --hash=sha256:5b7b716f97b52c5a14bffdf688f971b2d5ef4029127f1ad7a513973cfd818df2 \
-    --hash=sha256:5dedb4db619ba5a2787a94d877bc8ffc0566f92a01c0ef214865e54ecc9ee5e0 \
-    --hash=sha256:619bc166c4f2de5caa5a633b8b7326fbe98e0ccbfacabd87268a2b15ff73a029 \
-    --hash=sha256:629ddd2ca402ae6dbedfceeba9c46d5f7b2a61d9749597d4307f943ef198fc1f \
-    --hash=sha256:656f7526c69fac7f600bd1f400991cc282b417d17539a1b228617081106feb4a \
-    --hash=sha256:6ec585f69cec0aa07d945b20805be741395e28ac1627333b1c5b0105962ffced \
-    --hash=sha256:72b6be590cc35924b02c78ef34b467da4ba07e4e0f0454a2c5907f473fc50ce5 \
-    --hash=sha256:7502934a33b54030eaf1194c21c692a534196063db72176b0c4028e140f8f32c \
-    --hash=sha256:7a68b554d356a91cce1236aa7682dc01df0edba8d043fd1ce607c49dd3c1edcf \
-    --hash=sha256:7b2e5a267c855eea6b4283940daa6e88a285f5f2a67f2220203786dfa59b37e9 \
-    --hash=sha256:823b65d8706e32ad2df51ed89496147a42a2a6e01c13cfb6ffb8b1e92bc910bb \
-    --hash=sha256:8590b4ae07a35970728874632fed7bd57b26b0102df2d2b233b6d9d82f6c62ad \
-    --hash=sha256:8dd717634f5a044f860435c1d8c16a270ddf0ef8588d4887037c5028b859b0c3 \
-    --hash=sha256:8dec4936e9c3100156f8a2dc89c4b88d5c435175ff03413b443469c7c8c5f4d1 \
-    --hash=sha256:97cafb1f3cbcd3fd2b6fbfb99ae11cdb14deea0736fc2b0952ee177f2b813a46 \
-    --hash=sha256:a17a92de5231666cfbe003f0e4b9b3a7ae3afb1ec2845aadc2bacc93ff85febc \
-    --hash=sha256:a549b9c31bec33820e885335b451286e2969a2d9e24879f83fe904a5ce59d70a \
-    --hash=sha256:ac07bad82163452a6884fe8fa0963fb98c2346ba78d779ec06bd7a6262132aee \
-    --hash=sha256:ae2ad8ae6ebee9d2d94b17fb62763125f3f374c25618198f40cbb8b525411900 \
-    --hash=sha256:b91c037585eba9095565a3556f611e3cbfaa42ca1e865f7b8015fe5c7336d5a5 \
-    --hash=sha256:bc1667f8b83f48511b94671e0e441401371dfd0f0a795c7daa4a3cd1dde55bea \
-    --hash=sha256:bec0a414d016ac1a18862a519e54b2fd0fc8bbfd6890376898a6c0891dd82e9f \
-    --hash=sha256:bf50cd79a75d181c9181df03572cdce0fbb75cc353bc350712073108cba98de5 \
-    --hash=sha256:bff1b4290a66b490a2f4719358c0cdcd9bafb6b8f061e45c7a2460866bf50c2e \
-    --hash=sha256:c061bb86a71b42465156a3ee7bd58c8c2ceacdbeb95d05a99893e08b8467359a \
-    --hash=sha256:c8b29db45f8fe46ad280a7294f5c3ec36dbac9491f2d1c17345be8e69cc5928f \
-    --hash=sha256:ce409136744f6521e39fd8e2a24c53fa18ad67aa5bc7c2cf83645cce5b5c4e50 \
-    --hash=sha256:d050b3361367a06d752db6ead6e7edeb0009be66bc3bae0ee9d97fb326badc2a \
-    --hash=sha256:d283d37a890ba4c1ae73ffadf8046435c76e7bc2247bbb63c00bd1a709c6544b \
-    --hash=sha256:d9fad5155d72433c921b782e58892377c44bd6252b5af2f67f16b194987338a4 \
-    --hash=sha256:daa4ee5a243f0f20d528d939d06670a298dd39b1ad5f8a72a4275124a7819eff \
-    --hash=sha256:db0b55e0f3cc0be60c1f19efdde9a637c32740486004f20d1cff53c3c0ece4d2 \
-    --hash=sha256:e61659ba32cf2cf1481e575d0462554625196a1f2fc06a1c777d3f48e8865d46 \
-    --hash=sha256:ea3d8a3d18833cf4304cd2fc9cbb1efe188ca9b5efef2bdac7adc20594a0e46b \
-    --hash=sha256:ec6a563cff360b50eed26f13adc43e61bc0c04d94b8be985e6fb24b81f6dcfdf \
-    --hash=sha256:f5dfb42c4604dddc8e4305050aa6deb084540643ed5804d7455b5df8fe16f5e5 \
-    --hash=sha256:fa173ec60341d6bb97a89f5ea19c85c5643c1e7dedebc22f5181eb73573142c5 \
-    --hash=sha256:fa9db3f79de01457b03d4f01b34cf91bc0048eb2c3846ff26f66687c2f6d16ab \
-    --hash=sha256:fce659a462a1be54d2ffcacea5e3ba2d74daa74f30f5f143fe0c58636e355fdd \
-    --hash=sha256:ffee1f21e5ef0d712f9033568f8344d5da8cc2869dbd08d87c84656e6a2d2f68
-mergedeep==1.3.4 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:0096d52e9dad9939c3d975a774666af186eda617e6ca84df4c94dec30004f2a8 \
-    --hash=sha256:70775750742b25c0d8f36c55aed03d24c3384d17c951b3175d898bd778ef0307
-mkdocs-autorefs==1.0.1 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:aacdfae1ab197780fb7a2dac92ad8a3d8f7ca8049a9cbe56a4218cd52e8da570 \
-    --hash=sha256:f684edf847eced40b570b57846b15f0bf57fb93ac2c510450775dcf16accb971
-mkdocs-material-extensions==1.3.1 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:10c9511cea88f568257f960358a467d12b970e1f7b2c0e5fb2bb48cab1928443 \
-    --hash=sha256:adff8b62700b25cb77b53358dad940f3ef973dd6db797907c49e3c2ef3ab4e31
-mkdocs-material==9.5.18 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:1e0e27fc9fe239f9064318acf548771a4629d5fd5dfd45444fd80a953fe21eb4 \
-    --hash=sha256:a43f470947053fa2405c33995f282d24992c752a50114f23f30da9d8d0c57e62
-mkdocs-minify-plugin==0.8.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:5fba1a3f7bd9a2142c9954a6559a57e946587b21f133165ece30ea145c66aee6 \
-    --hash=sha256:bc11b78b8120d79e817308e2b11539d790d21445eb63df831e393f76e52e753d
-mkdocs==1.5.3 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:3b3a78e736b31158d64dbb2f8ba29bd46a379d0c6e324c2246c3bc3d2189cfc1 \
-    --hash=sha256:eb7c99214dcb945313ba30426c2451b735992c73c2e10838f76d09e39ff4d0e2
-mkdocstrings-python==1.10.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:71678fac657d4d2bb301eed4e4d2d91499c095fd1f8a90fa76422a87a5693828 \
-    --hash=sha256:ba833fbd9d178a4b9d5cb2553a4df06e51dc1f51e41559a4d2398c16a6f69ecc
-mkdocstrings==0.24.3 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:5c9cf2a32958cd161d5428699b79c8b0988856b0d4a8c5baf8395fc1bf4087c3 \
-    --hash=sha256:f327b234eb8d2551a306735436e157d0a22d45f79963c60a8b585d5f7a94c1d2
-mkdocstrings[python]==0.24.3 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:5c9cf2a32958cd161d5428699b79c8b0988856b0d4a8c5baf8395fc1bf4087c3 \
-    --hash=sha256:f327b234eb8d2551a306735436e157d0a22d45f79963c60a8b585d5f7a94c1d2
+installer==0.7.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:05d1933f0a5ba7d8d6296bb6d5018e7c94fa473ceb10cf198a92ccea19c27b53 \
+    --hash=sha256:a26d3e3116289bb08216e0d0f7d925fcef0b0194eedfa0c944bcaaa106c4b631
+jaraco-classes==3.4.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:47a024b51d0239c0dd8c8540c6c7f484be3b8fcf0b2d85c13825780d3b3f3acd \
+    --hash=sha256:f662826b6bed8cace05e7ff873ce0f9283b5c924470fe664fff1c2f00f581790
+jeepney==0.8.0 ; python_version >= "3.9" and python_version < "4.0" and sys_platform == "linux" \
+    --hash=sha256:5efe48d255973902f6badc3ce55e2aa6c5c3b3bc642059ef3a91247bcfcc5806 \
+    --hash=sha256:c0a454ad016ca575060802ee4d590dd912e35c122fa04e70306de3d076cce755
+keyring==24.3.1 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:c3327b6ffafc0e8befbdb597cacdb4928ffe5c1212f7645f186e6d9957a898db \
+    --hash=sha256:df38a4d7419a6a60fea5cef1e45a948a3e8430dd12ad88b0f423c5c143906218
+more-itertools==10.2.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:686b06abe565edfab151cb8fd385a05651e1fdf8f0a14191e4439283421f8684 \
+    --hash=sha256:8fccb480c43d3e99a00087634c06dd02b0d50fbf088b380de5a41a015ec239e1
+msgpack==1.0.8 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:00e073efcba9ea99db5acef3959efa45b52bc67b61b00823d2a1a6944bf45982 \
+    --hash=sha256:0726c282d188e204281ebd8de31724b7d749adebc086873a59efb8cf7ae27df3 \
+    --hash=sha256:0ceea77719d45c839fd73abcb190b8390412a890df2f83fb8cf49b2a4b5c2f40 \
+    --hash=sha256:114be227f5213ef8b215c22dde19532f5da9652e56e8ce969bf0a26d7c419fee \
+    --hash=sha256:13577ec9e247f8741c84d06b9ece5f654920d8365a4b636ce0e44f15e07ec693 \
+    --hash=sha256:1876b0b653a808fcd50123b953af170c535027bf1d053b59790eebb0aeb38950 \
+    --hash=sha256:1ab0bbcd4d1f7b6991ee7c753655b481c50084294218de69365f8f1970d4c151 \
+    --hash=sha256:1cce488457370ffd1f953846f82323cb6b2ad2190987cd4d70b2713e17268d24 \
+    --hash=sha256:26ee97a8261e6e35885c2ecd2fd4a6d38252246f94a2aec23665a4e66d066305 \
+    --hash=sha256:3528807cbbb7f315bb81959d5961855e7ba52aa60a3097151cb21956fbc7502b \
+    --hash=sha256:374a8e88ddab84b9ada695d255679fb99c53513c0a51778796fcf0944d6c789c \
+    --hash=sha256:376081f471a2ef24828b83a641a02c575d6103a3ad7fd7dade5486cad10ea659 \
+    --hash=sha256:3923a1778f7e5ef31865893fdca12a8d7dc03a44b33e2a5f3295416314c09f5d \
+    --hash=sha256:4916727e31c28be8beaf11cf117d6f6f188dcc36daae4e851fee88646f5b6b18 \
+    --hash=sha256:493c5c5e44b06d6c9268ce21b302c9ca055c1fd3484c25ba41d34476c76ee746 \
+    --hash=sha256:505fe3d03856ac7d215dbe005414bc28505d26f0c128906037e66d98c4e95868 \
+    --hash=sha256:5845fdf5e5d5b78a49b826fcdc0eb2e2aa7191980e3d2cfd2a30303a74f212e2 \
+    --hash=sha256:5c330eace3dd100bdb54b5653b966de7f51c26ec4a7d4e87132d9b4f738220ba \
+    --hash=sha256:5dbf059fb4b7c240c873c1245ee112505be27497e90f7c6591261c7d3c3a8228 \
+    --hash=sha256:5e390971d082dba073c05dbd56322427d3280b7cc8b53484c9377adfbae67dc2 \
+    --hash=sha256:5fbb160554e319f7b22ecf530a80a3ff496d38e8e07ae763b9e82fadfe96f273 \
+    --hash=sha256:64d0fcd436c5683fdd7c907eeae5e2cbb5eb872fafbc03a43609d7941840995c \
+    --hash=sha256:69284049d07fce531c17404fcba2bb1df472bc2dcdac642ae71a2d079d950653 \
+    --hash=sha256:6a0e76621f6e1f908ae52860bdcb58e1ca85231a9b0545e64509c931dd34275a \
+    --hash=sha256:73ee792784d48aa338bba28063e19a27e8d989344f34aad14ea6e1b9bd83f596 \
+    --hash=sha256:74398a4cf19de42e1498368c36eed45d9528f5fd0155241e82c4082b7e16cffd \
+    --hash=sha256:7938111ed1358f536daf311be244f34df7bf3cdedb3ed883787aca97778b28d8 \
+    --hash=sha256:82d92c773fbc6942a7a8b520d22c11cfc8fd83bba86116bfcf962c2f5c2ecdaa \
+    --hash=sha256:83b5c044f3eff2a6534768ccfd50425939e7a8b5cf9a7261c385de1e20dcfc85 \
+    --hash=sha256:8db8e423192303ed77cff4dce3a4b88dbfaf43979d280181558af5e2c3c71afc \
+    --hash=sha256:9517004e21664f2b5a5fd6333b0731b9cf0817403a941b393d89a2f1dc2bd836 \
+    --hash=sha256:95c02b0e27e706e48d0e5426d1710ca78e0f0628d6e89d5b5a5b91a5f12274f3 \
+    --hash=sha256:99881222f4a8c2f641f25703963a5cefb076adffd959e0558dc9f803a52d6a58 \
+    --hash=sha256:9ee32dcb8e531adae1f1ca568822e9b3a738369b3b686d1477cbc643c4a9c128 \
+    --hash=sha256:a22e47578b30a3e199ab067a4d43d790249b3c0587d9a771921f86250c8435db \
+    --hash=sha256:b5505774ea2a73a86ea176e8a9a4a7c8bf5d521050f0f6f8426afe798689243f \
+    --hash=sha256:bd739c9251d01e0279ce729e37b39d49a08c0420d3fee7f2a4968c0576678f77 \
+    --hash=sha256:d16a786905034e7e34098634b184a7d81f91d4c3d246edc6bd7aefb2fd8ea6ad \
+    --hash=sha256:d3420522057ebab1728b21ad473aa950026d07cb09da41103f8e597dfbfaeb13 \
+    --hash=sha256:d56fd9f1f1cdc8227d7b7918f55091349741904d9520c65f0139a9755952c9e8 \
+    --hash=sha256:d661dc4785affa9d0edfdd1e59ec056a58b3dbb9f196fa43587f3ddac654ac7b \
+    --hash=sha256:dfe1f0f0ed5785c187144c46a292b8c34c1295c01da12e10ccddfc16def4448a \
+    --hash=sha256:e1dd7839443592d00e96db831eddb4111a2a81a46b028f0facd60a09ebbdd543 \
+    --hash=sha256:e2872993e209f7ed04d963e4b4fbae72d034844ec66bc4ca403329db2074377b \
+    --hash=sha256:e2f879ab92ce502a1e65fce390eab619774dda6a6ff719718069ac94084098ce \
+    --hash=sha256:e3aa7e51d738e0ec0afbed661261513b38b3014754c9459508399baf14ae0c9d \
+    --hash=sha256:e532dbd6ddfe13946de050d7474e3f5fb6ec774fbb1a188aaf469b08cf04189a \
+    --hash=sha256:e6b7842518a63a9f17107eb176320960ec095a8ee3b4420b5f688e24bf50c53c \
+    --hash=sha256:e75753aeda0ddc4c28dce4c32ba2f6ec30b1b02f6c0b14e547841ba5b24f753f \
+    --hash=sha256:eadb9f826c138e6cf3c49d6f8de88225a3c0ab181a9b4ba792e006e5292d150e \
+    --hash=sha256:ed59dd52075f8fc91da6053b12e8c89e37aa043f8986efd89e61fae69dc1b011 \
+    --hash=sha256:ef254a06bcea461e65ff0373d8a0dd1ed3aa004af48839f002a0c994a6f72d04 \
+    --hash=sha256:f3709997b228685fe53e8c433e2df9f0cdb5f4542bd5114ed17ac3c0129b0480 \
+    --hash=sha256:f51bab98d52739c50c56658cc303f190785f9a2cd97b823357e7aeae54c8f68a \
+    --hash=sha256:f9904e24646570539a8950400602d66d2b2c492b9010ea7e965025cb71d0c86d \
+    --hash=sha256:f9af38a89b6a5c04b7d18c492c8ccf2aee7048aff1ce8437c4683bb5a1df893d
 packaging==24.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:2ddfb553fdf02fb784c234c7ba6ccc288296ceabec964ad2eae3777778130bc5 \
     --hash=sha256:eb82c5e3e56209074766e6885bb04b8c38a0c015d0a30036ebe7ece34c9989e9
-paginate==0.5.6 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:5e6007b6a9398177a7e1648d04fdd9f8c9766a1a945bceac82f1929e8c78af2d
-pathspec==0.12.1 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:a0d503e138a4c123b27490a4f7beda6a01c6f288df0e4a8b79c7eb0dc7b4cc08 \
-    --hash=sha256:a482d51503a1ab33b1c67a6c3813a26953dbdc71c31dacaef9a838c4e29f5712
+pexpect==4.9.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:7236d1e080e4936be2dc3e326cec0af72acf9212a7e1d060210e70a47e253523 \
+    --hash=sha256:ee7d41123f3c9911050ea2c2dac107568dc43b2d3b0c7557a33212c398ead30f
+pip-compile-cross-platform==1.3.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:06910a8cd91bf184f93687373ce1ce099b5b35cafe3c1717dae783f78a9d2760 \
+    --hash=sha256:a0382d46c55cadf5f9fcaa63a0f80c16ce01c68f7859619f47b9fcf5d2c34c90
+pip-requirements-parser==32.0.1 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:4659bc2a667783e7a15d190f6fccf8b2486685b6dba4c19c3876314769c57526 \
+    --hash=sha256:b4fa3a7a0be38243123cf9d1f3518da10c51bdb165a2b2985566247f9155a7d3
+pkginfo==1.10.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:5df73835398d10db79f8eecd5cd86b1f6d29317589ea70796994d49399af6297 \
+    --hash=sha256:889a6da2ed7ffc58ab5b900d888ddce90bce912f2d2de1dc1c26f4cb9fe65097
 platformdirs==4.2.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:0614df2a2f37e1a662acbd8e2b25b92ccf8632929bc6d43467e17fe89c75e068 \
     --hash=sha256:ef0cc731df711022c174543cb70a9b5bd22e5a9337c8624ef2c2ceb8ddad8768
-pygments==2.17.2 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:b27c2826c47d0f3219f29554824c30c5e8945175d888647acd804ddd04af846c \
-    --hash=sha256:da46cec9fd2de5be3a8a784f434e4c4ab670b4ff54d605c4c2717e9d49c4c367
-pymdown-extensions==10.8 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:3539003ff0d5e219ba979d2dc961d18fcad5ac259e66c764482e8347b4c0503c \
-    --hash=sha256:91ca336caf414e1e5e0626feca86e145de9f85a3921a7bcbd32890b51738c428
-python-dateutil==2.9.0.post0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:37dd54208da7e1cd875388217d5e00ebd4179249f90fb72437e91a35459a0ad3 \
-    --hash=sha256:a8b2bc7bffae282281c8140a97d3aa9c14da0b136dfe83f850eea9a5f7470427
-pyyaml-env-tag==0.1 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:70092675bda14fdec33b31ba77e7543de9ddc88f2e5b99160396572d11525bdb \
-    --hash=sha256:af31106dec8a4d68c60207c1886031cbf839b68aa7abccdb19868200532c2069
-pyyaml==6.0.1 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:04ac92ad1925b2cff1db0cfebffb6ffc43457495c9b3c39d3fcae417d7125dc5 \
-    --hash=sha256:062582fca9fabdd2c8b54a3ef1c978d786e0f6b3a1510e0ac93ef59e0ddae2bc \
-    --hash=sha256:0d3304d8c0adc42be59c5f8a4d9e3d7379e6955ad754aa9d6ab7a398b59dd1df \
-    --hash=sha256:1635fd110e8d85d55237ab316b5b011de701ea0f29d07611174a1b42f1444741 \
-    --hash=sha256:184c5108a2aca3c5b3d3bf9395d50893a7ab82a38004c8f61c258d4428e80206 \
-    --hash=sha256:18aeb1bf9a78867dc38b259769503436b7c72f7a1f1f4c93ff9a17de54319b27 \
-    --hash=sha256:1d4c7e777c441b20e32f52bd377e0c409713e8bb1386e1099c2415f26e479595 \
-    --hash=sha256:1e2722cc9fbb45d9b87631ac70924c11d3a401b2d7f410cc0e3bbf249f2dca62 \
-    --hash=sha256:1fe35611261b29bd1de0070f0b2f47cb6ff71fa6595c077e42bd0c419fa27b98 \
-    --hash=sha256:28c119d996beec18c05208a8bd78cbe4007878c6dd15091efb73a30e90539696 \
-    --hash=sha256:326c013efe8048858a6d312ddd31d56e468118ad4cdeda36c719bf5bb6192290 \
-    --hash=sha256:40df9b996c2b73138957fe23a16a4f0ba614f4c0efce1e9406a184b6d07fa3a9 \
-    --hash=sha256:42f8152b8dbc4fe7d96729ec2b99c7097d656dc1213a3229ca5383f973a5ed6d \
-    --hash=sha256:49a183be227561de579b4a36efbb21b3eab9651dd81b1858589f796549873dd6 \
-    --hash=sha256:4fb147e7a67ef577a588a0e2c17b6db51dda102c71de36f8549b6816a96e1867 \
-    --hash=sha256:50550eb667afee136e9a77d6dc71ae76a44df8b3e51e41b77f6de2932bfe0f47 \
-    --hash=sha256:510c9deebc5c0225e8c96813043e62b680ba2f9c50a08d3724c7f28a747d1486 \
-    --hash=sha256:5773183b6446b2c99bb77e77595dd486303b4faab2b086e7b17bc6bef28865f6 \
-    --hash=sha256:596106435fa6ad000c2991a98fa58eeb8656ef2325d7e158344fb33864ed87e3 \
-    --hash=sha256:6965a7bc3cf88e5a1c3bd2e0b5c22f8d677dc88a455344035f03399034eb3007 \
-    --hash=sha256:69b023b2b4daa7548bcfbd4aa3da05b3a74b772db9e23b982788168117739938 \
-    --hash=sha256:6c22bec3fbe2524cde73d7ada88f6566758a8f7227bfbf93a408a9d86bcc12a0 \
-    --hash=sha256:704219a11b772aea0d8ecd7058d0082713c3562b4e271b849ad7dc4a5c90c13c \
-    --hash=sha256:7e07cbde391ba96ab58e532ff4803f79c4129397514e1413a7dc761ccd755735 \
-    --hash=sha256:81e0b275a9ecc9c0c0c07b4b90ba548307583c125f54d5b6946cfee6360c733d \
-    --hash=sha256:855fb52b0dc35af121542a76b9a84f8d1cd886ea97c84703eaa6d88e37a2ad28 \
-    --hash=sha256:8d4e9c88387b0f5c7d5f281e55304de64cf7f9c0021a3525bd3b1c542da3b0e4 \
-    --hash=sha256:9046c58c4395dff28dd494285c82ba00b546adfc7ef001486fbf0324bc174fba \
-    --hash=sha256:9eb6caa9a297fc2c2fb8862bc5370d0303ddba53ba97e71f08023b6cd73d16a8 \
-    --hash=sha256:a08c6f0fe150303c1c6b71ebcd7213c2858041a7e01975da3a99aed1e7a378ef \
-    --hash=sha256:a0cd17c15d3bb3fa06978b4e8958dcdc6e0174ccea823003a106c7d4d7899ac5 \
-    --hash=sha256:afd7e57eddb1a54f0f1a974bc4391af8bcce0b444685d936840f125cf046d5bd \
-    --hash=sha256:b1275ad35a5d18c62a7220633c913e1b42d44b46ee12554e5fd39c70a243d6a3 \
-    --hash=sha256:b786eecbdf8499b9ca1d697215862083bd6d2a99965554781d0d8d1ad31e13a0 \
-    --hash=sha256:ba336e390cd8e4d1739f42dfe9bb83a3cc2e80f567d8805e11b46f4a943f5515 \
-    --hash=sha256:baa90d3f661d43131ca170712d903e6295d1f7a0f595074f151c0aed377c9b9c \
-    --hash=sha256:bc1bf2925a1ecd43da378f4db9e4f799775d6367bdb94671027b73b393a7c42c \
-    --hash=sha256:bd4af7373a854424dabd882decdc5579653d7868b8fb26dc7d0e99f823aa5924 \
-    --hash=sha256:bf07ee2fef7014951eeb99f56f39c9bb4af143d8aa3c21b1677805985307da34 \
-    --hash=sha256:bfdf460b1736c775f2ba9f6a92bca30bc2095067b8a9d77876d1fad6cc3b4a43 \
-    --hash=sha256:c8098ddcc2a85b61647b2590f825f3db38891662cfc2fc776415143f599bb859 \
-    --hash=sha256:d2b04aac4d386b172d5b9692e2d2da8de7bfb6c387fa4f801fbf6fb2e6ba4673 \
-    --hash=sha256:d483d2cdf104e7c9fa60c544d92981f12ad66a457afae824d146093b8c294c54 \
-    --hash=sha256:d858aa552c999bc8a8d57426ed01e40bef403cd8ccdd0fc5f6f04a00414cac2a \
-    --hash=sha256:e7d73685e87afe9f3b36c799222440d6cf362062f78be1013661b00c5c6f678b \
-    --hash=sha256:f003ed9ad21d6a4713f0a9b5a7a0a79e08dd0f221aff4525a2be4c346ee60aab \
-    --hash=sha256:f22ac1c3cac4dbc50079e965eba2c1058622631e526bd9afd45fedd49ba781fa \
-    --hash=sha256:faca3bdcf85b2fc05d06ff3fbc1f83e1391b3e724afa3feba7d13eeab355484c \
-    --hash=sha256:fca0e3a251908a499833aa292323f32437106001d436eca0e6e7833256674585 \
-    --hash=sha256:fd1592b3fdf65fff2ad0004b5e363300ef59ced41c2e6b3a99d4089fa8c5435d \
-    --hash=sha256:fd66fc5d0da6d9815ba2cebeb4205f95818ff4b79c3ebe268e75d961704af52f
-regex==2024.4.16 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:00169caa125f35d1bca6045d65a662af0202704489fada95346cfa092ec23f39 \
-    --hash=sha256:03576e3a423d19dda13e55598f0fd507b5d660d42c51b02df4e0d97824fdcae3 \
-    --hash=sha256:03e68f44340528111067cecf12721c3df4811c67268b897fbe695c95f860ac42 \
-    --hash=sha256:0534b034fba6101611968fae8e856c1698da97ce2efb5c2b895fc8b9e23a5834 \
-    --hash=sha256:08dea89f859c3df48a440dbdcd7b7155bc675f2fa2ec8c521d02dc69e877db70 \
-    --hash=sha256:0a38d151e2cdd66d16dab550c22f9521ba79761423b87c01dae0a6e9add79c0d \
-    --hash=sha256:0c8290b44d8b0af4e77048646c10c6e3aa583c1ca67f3b5ffb6e06cf0c6f0f89 \
-    --hash=sha256:10188fe732dec829c7acca7422cdd1bf57d853c7199d5a9e96bb4d40db239c73 \
-    --hash=sha256:1210365faba7c2150451eb78ec5687871c796b0f1fa701bfd2a4a25420482d26 \
-    --hash=sha256:12f6a3f2f58bb7344751919a1876ee1b976fe08b9ffccb4bbea66f26af6017b9 \
-    --hash=sha256:159dc4e59a159cb8e4e8f8961eb1fa5d58f93cb1acd1701d8aff38d45e1a84a6 \
-    --hash=sha256:20b7a68444f536365af42a75ccecb7ab41a896a04acf58432db9e206f4e525d6 \
-    --hash=sha256:23cff1b267038501b179ccbbd74a821ac4a7192a1852d1d558e562b507d46013 \
-    --hash=sha256:2c72608e70f053643437bd2be0608f7f1c46d4022e4104d76826f0839199347a \
-    --hash=sha256:3399dd8a7495bbb2bacd59b84840eef9057826c664472e86c91d675d007137f5 \
-    --hash=sha256:34422d5a69a60b7e9a07a690094e824b66f5ddc662a5fc600d65b7c174a05f04 \
-    --hash=sha256:370c68dc5570b394cbaadff50e64d705f64debed30573e5c313c360689b6aadc \
-    --hash=sha256:3a1018e97aeb24e4f939afcd88211ace472ba566efc5bdf53fd8fd7f41fa7170 \
-    --hash=sha256:3d5ac5234fb5053850d79dd8eb1015cb0d7d9ed951fa37aa9e6249a19aa4f336 \
-    --hash=sha256:4313ab9bf6a81206c8ac28fdfcddc0435299dc88cad12cc6305fd0e78b81f9e4 \
-    --hash=sha256:445ca8d3c5a01309633a0c9db57150312a181146315693273e35d936472df912 \
-    --hash=sha256:479595a4fbe9ed8f8f72c59717e8cf222da2e4c07b6ae5b65411e6302af9708e \
-    --hash=sha256:4918fd5f8b43aa7ec031e0fef1ee02deb80b6afd49c85f0790be1dc4ce34cb50 \
-    --hash=sha256:4aba818dcc7263852aabb172ec27b71d2abca02a593b95fa79351b2774eb1d2b \
-    --hash=sha256:4e819a806420bc010489f4e741b3036071aba209f2e0989d4750b08b12a9343f \
-    --hash=sha256:4facc913e10bdba42ec0aee76d029aedda628161a7ce4116b16680a0413f658a \
-    --hash=sha256:549c3584993772e25f02d0656ac48abdda73169fe347263948cf2b1cead622f3 \
-    --hash=sha256:5c02fcd2bf45162280613d2e4a1ca3ac558ff921ae4e308ecb307650d3a6ee51 \
-    --hash=sha256:5f580c651a72b75c39e311343fe6875d6f58cf51c471a97f15a938d9fe4e0d37 \
-    --hash=sha256:62120ed0de69b3649cc68e2965376048793f466c5a6c4370fb27c16c1beac22d \
-    --hash=sha256:6295004b2dd37b0835ea5c14a33e00e8cfa3c4add4d587b77287825f3418d310 \
-    --hash=sha256:65436dce9fdc0aeeb0a0effe0839cb3d6a05f45aa45a4d9f9c60989beca78b9c \
-    --hash=sha256:684008ec44ad275832a5a152f6e764bbe1914bea10968017b6feaecdad5736e0 \
-    --hash=sha256:684e52023aec43bdf0250e843e1fdd6febbe831bd9d52da72333fa201aaa2335 \
-    --hash=sha256:6cc38067209354e16c5609b66285af17a2863a47585bcf75285cab33d4c3b8df \
-    --hash=sha256:6f2f017c5be19984fbbf55f8af6caba25e62c71293213f044da3ada7091a4455 \
-    --hash=sha256:743deffdf3b3481da32e8a96887e2aa945ec6685af1cfe2bcc292638c9ba2f48 \
-    --hash=sha256:7571f19f4a3fd00af9341c7801d1ad1967fc9c3f5e62402683047e7166b9f2b4 \
-    --hash=sha256:7731728b6568fc286d86745f27f07266de49603a6fdc4d19c87e8c247be452af \
-    --hash=sha256:785c071c982dce54d44ea0b79cd6dfafddeccdd98cfa5f7b86ef69b381b457d9 \
-    --hash=sha256:78fddb22b9ef810b63ef341c9fcf6455232d97cfe03938cbc29e2672c436670e \
-    --hash=sha256:7bb966fdd9217e53abf824f437a5a2d643a38d4fd5fd0ca711b9da683d452969 \
-    --hash=sha256:7cbc5d9e8a1781e7be17da67b92580d6ce4dcef5819c1b1b89f49d9678cc278c \
-    --hash=sha256:803b8905b52de78b173d3c1e83df0efb929621e7b7c5766c0843704d5332682f \
-    --hash=sha256:80b696e8972b81edf0af2a259e1b2a4a661f818fae22e5fa4fa1a995fb4a40fd \
-    --hash=sha256:81500ed5af2090b4a9157a59dbc89873a25c33db1bb9a8cf123837dcc9765047 \
-    --hash=sha256:89ec7f2c08937421bbbb8b48c54096fa4f88347946d4747021ad85f1b3021b3c \
-    --hash=sha256:8ba6745440b9a27336443b0c285d705ce73adb9ec90e2f2004c64d95ab5a7598 \
-    --hash=sha256:8c91e1763696c0eb66340c4df98623c2d4e77d0746b8f8f2bee2c6883fd1fe18 \
-    --hash=sha256:8d015604ee6204e76569d2f44e5a210728fa917115bef0d102f4107e622b08d5 \
-    --hash=sha256:8d1f86f3f4e2388aa3310b50694ac44daefbd1681def26b4519bd050a398dc5a \
-    --hash=sha256:8f83b6fd3dc3ba94d2b22717f9c8b8512354fd95221ac661784df2769ea9bba9 \
-    --hash=sha256:8fc6976a3395fe4d1fbeb984adaa8ec652a1e12f36b56ec8c236e5117b585427 \
-    --hash=sha256:904c883cf10a975b02ab3478bce652f0f5346a2c28d0a8521d97bb23c323cc8b \
-    --hash=sha256:911742856ce98d879acbea33fcc03c1d8dc1106234c5e7d068932c945db209c0 \
-    --hash=sha256:91797b98f5e34b6a49f54be33f72e2fb658018ae532be2f79f7c63b4ae225145 \
-    --hash=sha256:95399831a206211d6bc40224af1c635cb8790ddd5c7493e0bd03b85711076a53 \
-    --hash=sha256:956b58d692f235cfbf5b4f3abd6d99bf102f161ccfe20d2fd0904f51c72c4c66 \
-    --hash=sha256:98c1165f3809ce7774f05cb74e5408cd3aa93ee8573ae959a97a53db3ca3180d \
-    --hash=sha256:9ab40412f8cd6f615bfedea40c8bf0407d41bf83b96f6fc9ff34976d6b7037fd \
-    --hash=sha256:9df1bfef97db938469ef0a7354b2d591a2d438bc497b2c489471bec0e6baf7c4 \
-    --hash=sha256:a01fe2305e6232ef3e8f40bfc0f0f3a04def9aab514910fa4203bafbc0bb4682 \
-    --hash=sha256:a70b51f55fd954d1f194271695821dd62054d949efd6368d8be64edd37f55c86 \
-    --hash=sha256:a7ccdd1c4a3472a7533b0a7aa9ee34c9a2bef859ba86deec07aff2ad7e0c3b94 \
-    --hash=sha256:b340cccad138ecb363324aa26893963dcabb02bb25e440ebdf42e30963f1a4e0 \
-    --hash=sha256:b74586dd0b039c62416034f811d7ee62810174bb70dffcca6439f5236249eb09 \
-    --hash=sha256:b9d320b3bf82a39f248769fc7f188e00f93526cc0fe739cfa197868633d44701 \
-    --hash=sha256:ba2336d6548dee3117520545cfe44dc28a250aa091f8281d28804aa8d707d93d \
-    --hash=sha256:ba8122e3bb94ecda29a8de4cf889f600171424ea586847aa92c334772d200331 \
-    --hash=sha256:bd727ad276bb91928879f3aa6396c9a1d34e5e180dce40578421a691eeb77f47 \
-    --hash=sha256:c21fc21a4c7480479d12fd8e679b699f744f76bb05f53a1d14182b31f55aac76 \
-    --hash=sha256:c2d0e7cbb6341e830adcbfa2479fdeebbfbb328f11edd6b5675674e7a1e37730 \
-    --hash=sha256:c2ef6f7990b6e8758fe48ad08f7e2f66c8f11dc66e24093304b87cae9037bb4a \
-    --hash=sha256:c4ed75ea6892a56896d78f11006161eea52c45a14994794bcfa1654430984b22 \
-    --hash=sha256:cccc79a9be9b64c881f18305a7c715ba199e471a3973faeb7ba84172abb3f317 \
-    --hash=sha256:d0800631e565c47520aaa04ae38b96abc5196fe8b4aa9bd864445bd2b5848a7a \
-    --hash=sha256:d2da13568eff02b30fd54fccd1e042a70fe920d816616fda4bf54ec705668d81 \
-    --hash=sha256:d61ae114d2a2311f61d90c2ef1358518e8f05eafda76eaf9c772a077e0b465ec \
-    --hash=sha256:d83c2bc678453646f1a18f8db1e927a2d3f4935031b9ad8a76e56760461105dd \
-    --hash=sha256:dd5acc0a7d38fdc7a3a6fd3ad14c880819008ecb3379626e56b163165162cc46 \
-    --hash=sha256:df79012ebf6f4efb8d307b1328226aef24ca446b3ff8d0e30202d7ebcb977a8c \
-    --hash=sha256:e0a2df336d1135a0b3a67f3bbf78a75f69562c1199ed9935372b82215cddd6e2 \
-    --hash=sha256:e2f142b45c6fed48166faeb4303b4b58c9fcd827da63f4cf0a123c3480ae11fb \
-    --hash=sha256:e697e1c0238133589e00c244a8b676bc2cfc3ab4961318d902040d099fec7483 \
-    --hash=sha256:e757d475953269fbf4b441207bb7dbdd1c43180711b6208e129b637792ac0b93 \
-    --hash=sha256:e87ab229332ceb127a165612d839ab87795972102cb9830e5f12b8c9a5c1b508 \
-    --hash=sha256:ea355eb43b11764cf799dda62c658c4d2fdb16af41f59bb1ccfec517b60bcb07 \
-    --hash=sha256:ec7e0043b91115f427998febaa2beb82c82df708168b35ece3accb610b91fac1 \
-    --hash=sha256:eeaa0b5328b785abc344acc6241cffde50dc394a0644a968add75fcefe15b9d4 \
-    --hash=sha256:f2d80a6749724b37853ece57988b39c4e79d2b5fe2869a86e8aeae3bbeef9eb0 \
-    --hash=sha256:fa454d26f2e87ad661c4f0c5a5fe4cf6aab1e307d1b94f16ffdfcb089ba685c0 \
-    --hash=sha256:fb83cc090eac63c006871fd24db5e30a1f282faa46328572661c0a24a2323a08 \
-    --hash=sha256:fd80d1280d473500d8086d104962a82d77bfbf2b118053824b7be28cd5a79ea5
+poetry-core==1.9.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:4e0c9c6ad8cf89956f03b308736d84ea6ddb44089d16f2adc94050108ec1f5a1 \
+    --hash=sha256:fa7a4001eae8aa572ee84f35feb510b321bd652e5cf9293249d62853e1f935a2
+poetry-plugin-export==1.7.1 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:b2258e53ae0d369a73806f957ed0e726eb95c571a0ce8b1f273da686528cc1da \
+    --hash=sha256:cf62cfb6218a904290ba6db3bc1a24aa076d10f81c48c6e48b2ded430131e22e
+poetry==1.8.2 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:49cceb3838104647c3e1021f3a4f13c6053704cc18d33f849a90fe687a29cb73 \
+    --hash=sha256:b42b400d9a803af6e788a30a6f3e9998020b77860e28df20647eb10b6f414910
+ptyprocess==0.7.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:4b41f3967fce3af57cc7e94b888626c18bf37a083e3651ca8feeb66d492fef35 \
+    --hash=sha256:5c5d0a3b48ceee0b48485e0c26037c0acd7d29765ca3fbb5cb3831d347423220
+pycparser==2.22 ; python_version >= "3.9" and python_version < "4.0" and (sys_platform == "darwin" or sys_platform == "linux") and (sys_platform == "darwin" or platform_python_implementation != "PyPy") \
+    --hash=sha256:491c8be9c040f5390f5bf44a5b07752bd07f56edf992381b05c701439eec10f6 \
+    --hash=sha256:c3702b6d3dd8c7abc1afa565d7e63d53a1d0bd86cdc24edd75470f4de499cfcc
+pyparsing==3.1.2 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:a1bac0ce561155ecc3ed78ca94d3c9378656ad4c94c1270de543f621420f94ad \
+    --hash=sha256:f9db75911801ed778fe61bb643079ff86601aca99fcae6345aa67292038fb742
+pyproject-hooks==1.0.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:283c11acd6b928d2f6a7c73fa0d01cb2bdc5f07c57a2eeb6e83d5e56b97976f8 \
+    --hash=sha256:f271b298b97f5955d53fb12b72c1fb1948c22c1a6b70b315c54cedaca0264ef5
+pywin32-ctypes==0.2.2 ; python_version >= "3.9" and python_version < "4.0" and sys_platform == "win32" \
+    --hash=sha256:3426e063bdd5fd4df74a14fa3cf80a0b42845a87e1d1e81f6549f9daec593a60 \
+    --hash=sha256:bf490a1a709baf35d688fe0ecf980ed4de11d2b3e37b51e5442587a75d9957e7
+rapidfuzz==3.8.1 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:00b5ee47b387fa3805f4038362a085ec58149135dc5bc640ca315a9893a16f9e \
+    --hash=sha256:0798e32304b8009d215026bf7e1c448f1831da0a03987b7de30059a41bee92f3 \
+    --hash=sha256:07d7d4a3c49a15146d65f06e44d7545628ca0437c929684e32ef122852f44d95 \
+    --hash=sha256:14791324f0c753f5a0918df1249b91515f5ddc16281fbaa5ec48bff8fa659229 \
+    --hash=sha256:16153a97efacadbd693ccc612a3285df2f072fd07c121f30c2c135a709537075 \
+    --hash=sha256:17d79398849c1244f646425cf31d856eab9ebd67b7d6571273e53df724ca817e \
+    --hash=sha256:1905d9319a97bed29f21584ca641190dbc9218a556202b77876f1e37618d2e03 \
+    --hash=sha256:1b176f01490b48337183da5b4223005bc0c2354a4faee5118917d2fba0bedc1c \
+    --hash=sha256:1c0264d03dcee1bb975975b77c2fe041820fb4d4a25a99e3cb74ddd083d671ca \
+    --hash=sha256:1d5592b08e3cadc9e06ef3af6a9d66b6ef1bf871ed5acd7f9b1e162d78806a65 \
+    --hash=sha256:1edafc0a2737df277d3ddf401f3a73f76e246b7502762c94a3916453ae67e9b1 \
+    --hash=sha256:1ef119fc127c982053fb9ec638dcc3277f83b034b5972eb05941984b9ec4a290 \
+    --hash=sha256:2084193fd8fd346db496a2220363437eb9370a06d1d5a7a9dba00a64390c6a28 \
+    --hash=sha256:209bb712c448cdec4def6260b9f059bd4681ec61a01568f5e70e37bfe9efe830 \
+    --hash=sha256:231dc1cb63b1c8dd78c0597aa3ad3749a86a2b7e76af295dd81609522699a558 \
+    --hash=sha256:25498650e30122f4a5ad6b27c7614b4af8628c1d32b19d406410d33f77a86c80 \
+    --hash=sha256:267ff42370e031195e3020fff075420c136b69dc918ecb5542ec75c1e36af81f \
+    --hash=sha256:2a8a007fdc5cf646e48e361a39eabe725b93af7673c5ab90294e551cae72ff58 \
+    --hash=sha256:2ba0e43e9a94d256a704a674c7010e6f8ef9225edf7287cf3e7f66c9894b06cd \
+    --hash=sha256:2c6a43446f0cd8ff347b1fbb918dc0d657bebf484ddfa960ee069e422a477428 \
+    --hash=sha256:30c282612b7ebf2d7646ebebfd98dd308c582246a94d576734e4b0162f57baf4 \
+    --hash=sha256:313bdcd16e9cd5e5568b4a31d18a631f0b04cc10a3fd916e4ef75b713e6f177e \
+    --hash=sha256:392582aa784737d95255ca122ebe7dca3c774da900d100c07b53d32cd221a60e \
+    --hash=sha256:3aff3b829b0b04bdf78bd780ec9faf5f26eac3591df98c35a0ae216c925ae436 \
+    --hash=sha256:3fee62ae76e3b8b9fff8aa2ca4061575ee358927ffbdb2919a8c84a98da59f78 \
+    --hash=sha256:41219536634bd6f85419f38450ef080cfb519638125d805cf8626443e677dc61 \
+    --hash=sha256:48b6e5a337a814aec7c6dda5d6460f947c9330860615301f35b519e16dde3c77 \
+    --hash=sha256:4969fe0eb179aedacee53ca8f8f1be3c655964a6d62db30f247fee444b9c52b4 \
+    --hash=sha256:4d5cd86aca3f12e73bfc70015db7e8fc44122da03aa3761138b95112e83f66e4 \
+    --hash=sha256:50db3867864422bf6a6435ea65b9ac9de71ef52ed1e05d62f498cd430189eece \
+    --hash=sha256:58999b21d01dd353f49511a61937eac20c7a5b22eab87612063947081855d85f \
+    --hash=sha256:5f4174079dfe8ed1f13ece9bde7660f19f98ab17e0c0d002d90cc845c3a7e238 \
+    --hash=sha256:63044a7b6791a2e945dce9d812a6886e93159deb0464984eb403617ded257f08 \
+    --hash=sha256:63db612bb6da1bb9f6aa7412739f0e714b1910ec07bc675943044fe683ef192c \
+    --hash=sha256:68b185a0397aebe78bcc5d0e1efd96509d4e2f3c4a05996e5c843732f547e9ef \
+    --hash=sha256:6d4f1956fe1fc618e34ac79a6ed84fff5a6f23e41a8a476dd3e8570f0b12f02b \
+    --hash=sha256:6f34a541895627c2bc9ef7757f16f02428a08d960d33208adfb96b33338d0945 \
+    --hash=sha256:6f7641992de44ec2ca54102422be44a8e3fb75b9690ccd74fff72b9ac7fc00ee \
+    --hash=sha256:6f8b62fdccc429e6643cefffd5df9c7bca65588d06e8925b78014ad9ad983bf5 \
+    --hash=sha256:718ea99f84b16c4bdbf6a93e53552cdccefa18e12ff9a02c5041e621460e2e61 \
+    --hash=sha256:747265f39978bbaad356f5c6b6c808f0e8f5e8994875af0119b82b4700c55387 \
+    --hash=sha256:77ea62879932b32aba77ab23a9296390a67d024bf2f048dee99143be80a4ce26 \
+    --hash=sha256:78a0d2a11bb3936463609777c6d6d4984a27ebb2360b58339c699899d85db036 \
+    --hash=sha256:799f5f221d639d1c2ed8a2348d1edf5e22aa489b58b2cc99f5bf0c1917e2d0f2 \
+    --hash=sha256:81fd28389bedab28251f0535b3c034b0e63a618efc3ff1d338c81a3da723adb3 \
+    --hash=sha256:827ddf2d5d157ac3d1001b52e84c9e20366237a742946599ffc435af7fdd26d0 \
+    --hash=sha256:8b76abfec195bf1ee6f9ec56c33ba5e9615ff2d0a9530a54001ed87e5a6ced3b \
+    --hash=sha256:8c40da44ca20235cda05751d6e828b6b348e7a7c5de2922fa0f9c63f564fd675 \
+    --hash=sha256:8e02425bfc7ebed617323a674974b70eaecd8f07b64a7d16e0bf3e766b93e3c9 \
+    --hash=sha256:8e08b01dc9369941a24d7e512b0d81bf514e7d6add1b93d8aeec3c8fa08a824e \
+    --hash=sha256:90167a48de3ed7f062058826608a80242b8561d0fb0cce2c610d741624811a61 \
+    --hash=sha256:9441aca94b21f7349cdb231cd0ce9ca251b2355836e8a02bf6ccbea5b442d7a9 \
+    --hash=sha256:97c13f156f14f10667e1cfc4257069b775440ce005e896c09ce3aff21c9ae665 \
+    --hash=sha256:987cd277d27d14301019fdf61c17524f6127f5d364be5482228726049d8e0d10 \
+    --hash=sha256:9a16ef3702cecf16056c5fd66398b7ea8622ff4e3afeb00a8db3e74427e850af \
+    --hash=sha256:9ea3d2e41d8fac71cb63ee72f75bee0ed1e9c50709d4c58587f15437761c1858 \
+    --hash=sha256:a02def2eb526cc934d2125533cf2f15aa71c72ed4397afca38427ab047901e88 \
+    --hash=sha256:a0643a25937fafe8d117f2907606e9940cd1cc905c66f16ece9ab93128299994 \
+    --hash=sha256:a2ee3909f611cc5860cc8d9f92d039fd84241ce7360b49ea88e657181d2b45f6 \
+    --hash=sha256:a357aae6791118011ad3ab4f2a4aa7bd7a487e5f9981b390e9f3c2c5137ecadf \
+    --hash=sha256:aa223c73c59cc45c12eaa9c439318084003beced0447ff92b578a890288e19eb \
+    --hash=sha256:ad4dbd06c1f579eb043b2dcfc635bc6c9fb858240a70f0abd3bed84d8ac79994 \
+    --hash=sha256:b0ba20be465566264fa5580d874ccf5eabba6975dba45857e2c76e2df3359c6d \
+    --hash=sha256:b27cea618601ca5032ea98ee116ca6e0fe67be7b286bcb0b9f956d64db697472 \
+    --hash=sha256:b7b9cbc60e3eb08da6d18636c62c6eb6206cd9d0c7ad73996f7a1df3fc415b27 \
+    --hash=sha256:bb571dbd4cc93342be0ba632f0b8d7de4cbd9d959d76371d33716d2216090d41 \
+    --hash=sha256:bbc15985c5658691f637a6b97651771147744edfad2a4be56b8a06755e3932fa \
+    --hash=sha256:bc5a1ec3bd05b55d3070d557c0cdd4412272d51b4966c79aa3e9da207bd33d65 \
+    --hash=sha256:bca5acf77508d1822023a85118c2dd8d3c16abdd56d2762359a46deb14daa5e0 \
+    --hash=sha256:c04ef83c9ca3162d200df36e933b3ea0327a2626cee2e01bbe55acbc004ce261 \
+    --hash=sha256:c21d5c7cfa6078c79897e5e482a7e84ff927143d2f3fb020dd6edd27f5469574 \
+    --hash=sha256:c22b32a57ab47afb207e8fe4bd7bb58c90f9291a63723cafd4e704742166e368 \
+    --hash=sha256:c458085e067c766112f089f78ce39eab2b69ba027d7bbb11d067a0b085774367 \
+    --hash=sha256:c4dbb1ebc9a811f38da33f32ed2bb5f58b149289b89eb11e384519e9ba7ca881 \
+    --hash=sha256:c754ce1fab41b731259f100d5d46529a38aa2c9b683c92aeb7e96ef5b2898cd8 \
+    --hash=sha256:c763d99cf087e7b2c5be0cf34ae9a0e1b031f5057d2341a0a0ed782458645b7e \
+    --hash=sha256:c9597a05d08e8103ad59ebdf29e3fbffb0d0dbf3b641f102cfbeadc3a77bde51 \
+    --hash=sha256:cc4af7090a626c902c48db9b5d786c1faa0d8e141571e8a63a5350419ea575bd \
+    --hash=sha256:ceb10039e7346927cec47eaa490b34abb602b537e738ee9914bb41b8de029fbc \
+    --hash=sha256:d1a15fef1938b43468002f2d81012dbc9e7b50eb8533af202b0559c2dc7865d9 \
+    --hash=sha256:d4276c7ee061db0bac54846933b40339f60085523675f917f37de24a4b3ce0ee \
+    --hash=sha256:d48657a404fab82b2754faa813a10c5ad6aa594cb1829dca168a49438b61b4ec \
+    --hash=sha256:e3f882110f2f4894942e314451773c47e8b1b4920b5ea2b6dd2e2d4079dd3135 \
+    --hash=sha256:e4c647795c5b901091a68e210c76b769af70a33a8624ac496ac3e34d33366c0d \
+    --hash=sha256:e62bde7d5df3312acc528786ee801c472cae5078b1f1e42761c853ba7fe1072a \
+    --hash=sha256:e6ec696a268e8d730b42711537e500f7397afc06125c0e8fa9c8211386d315a5 \
+    --hash=sha256:f176867f438ff2a43e6a837930153ca78fddb3ca94e378603a1e7b860d7869bf \
+    --hash=sha256:f8af980695b866255447703bf634551e67e1a4e1c2d2d26501858d9233d886d7 \
+    --hash=sha256:f8e57f9c2367706a320b78e91f8bf9a3b03bf9069464eb7b54455fa340d03e4c \
+    --hash=sha256:f9d5d924970b07128c61c08eebee718686f4bd9838ef712a50468169520c953f
+requests-toolbelt==1.0.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:7681a0a3d047012b5bdc0ee37d7f8f07ebe76ab08caeccfc3921ce23c88d5bc6 \
+    --hash=sha256:cccfdd665f0a24fcf4726e690f65639d272bb0637b9b92dfd91a5568ccf6bd06
 requests==2.31.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f \
     --hash=sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1
-six==1.16.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926 \
-    --hash=sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254
-typing-extensions==4.11.0 ; python_version >= "3.9" and python_version < "3.10" \
-    --hash=sha256:83f085bd5ca59c80295fc2a82ab5dac679cbe02b9f33f7d83af68e241bea51b0 \
-    --hash=sha256:c1f94d72897edaf4ce775bb7558d5b79d8126906a14ea5ed1635921406c0387a
+secretstorage==3.3.3 ; python_version >= "3.9" and python_version < "4.0" and sys_platform == "linux" \
+    --hash=sha256:2403533ef369eca6d2ba81718576c5e0f564d5cca1b58f73a8b23e7d4eeebd77 \
+    --hash=sha256:f356e6628222568e3af06f2eba8df495efa13b3b63081dafd4f7d9a7b7bc9f99
+shellingham==1.5.4 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:7ecfff8f2fd72616f7481040475a65b2bf8af90a56c89140852d1120324e8686 \
+    --hash=sha256:8dbca0739d487e5bd35ab3ca4b36e11c4078f3a234bfce294b0a0291363404de
+tomli==2.0.1 ; python_version >= "3.9" and python_version < "3.11" \
+    --hash=sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc \
+    --hash=sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f
+tomlkit==0.12.4 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:5cd82d48a3dd89dee1f9d64420aa20ae65cfbd00668d6f094d7578a78efbb77b \
+    --hash=sha256:7ca1cfc12232806517a8515047ba66a19369e71edf2439d0f5824f91032b6cc3
+trove-classifiers==2024.4.10 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:49f40bb6a746b72a1cba4f8d55ee8252169cda0f70802e3fd24f04b7fb25a492 \
+    --hash=sha256:678bd6fcc5218d72e3304e27a608acc9b91e17bd00c3f3d8c968497c843ad98b
 urllib3==2.2.1 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:450b20ec296a467077128bff42b73080516e71b56ff59a60a02bef2232c4fa9d \
     --hash=sha256:d0570876c61ab9e520d776c38acbbb5b05a776d3f9ff98a5c8fd5162a444cf19
-watchdog==4.0.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:11e12fafb13372e18ca1bbf12d50f593e7280646687463dd47730fd4f4d5d257 \
-    --hash=sha256:2895bf0518361a9728773083908801a376743bcc37dfa252b801af8fd281b1ca \
-    --hash=sha256:39cb34b1f1afbf23e9562501673e7146777efe95da24fab5707b88f7fb11649b \
-    --hash=sha256:45cc09cc4c3b43fb10b59ef4d07318d9a3ecdbff03abd2e36e77b6dd9f9a5c85 \
-    --hash=sha256:4986db5e8880b0e6b7cd52ba36255d4793bf5cdc95bd6264806c233173b1ec0b \
-    --hash=sha256:5369136a6474678e02426bd984466343924d1df8e2fd94a9b443cb7e3aa20d19 \
-    --hash=sha256:557ba04c816d23ce98a06e70af6abaa0485f6d94994ec78a42b05d1c03dcbd50 \
-    --hash=sha256:6a4db54edea37d1058b08947c789a2354ee02972ed5d1e0dca9b0b820f4c7f92 \
-    --hash=sha256:6a80d5cae8c265842c7419c560b9961561556c4361b297b4c431903f8c33b269 \
-    --hash=sha256:6a9c71a0b02985b4b0b6d14b875a6c86ddea2fdbebd0c9a720a806a8bbffc69f \
-    --hash=sha256:6c47bdd680009b11c9ac382163e05ca43baf4127954c5f6d0250e7d772d2b80c \
-    --hash=sha256:6e949a8a94186bced05b6508faa61b7adacc911115664ccb1923b9ad1f1ccf7b \
-    --hash=sha256:73c7a935e62033bd5e8f0da33a4dcb763da2361921a69a5a95aaf6c93aa03a87 \
-    --hash=sha256:76ad8484379695f3fe46228962017a7e1337e9acadafed67eb20aabb175df98b \
-    --hash=sha256:8350d4055505412a426b6ad8c521bc7d367d1637a762c70fdd93a3a0d595990b \
-    --hash=sha256:87e9df830022488e235dd601478c15ad73a0389628588ba0b028cb74eb72fed8 \
-    --hash=sha256:8f9a542c979df62098ae9c58b19e03ad3df1c9d8c6895d96c0d51da17b243b1c \
-    --hash=sha256:8fec441f5adcf81dd240a5fe78e3d83767999771630b5ddfc5867827a34fa3d3 \
-    --hash=sha256:9a03e16e55465177d416699331b0f3564138f1807ecc5f2de9d55d8f188d08c7 \
-    --hash=sha256:ba30a896166f0fee83183cec913298151b73164160d965af2e93a20bbd2ab605 \
-    --hash=sha256:c17d98799f32e3f55f181f19dd2021d762eb38fdd381b4a748b9f5a36738e935 \
-    --hash=sha256:c522392acc5e962bcac3b22b9592493ffd06d1fc5d755954e6be9f4990de932b \
-    --hash=sha256:d0f9bd1fd919134d459d8abf954f63886745f4660ef66480b9d753a7c9d40927 \
-    --hash=sha256:d18d7f18a47de6863cd480734613502904611730f8def45fc52a5d97503e5101 \
-    --hash=sha256:d31481ccf4694a8416b681544c23bd271f5a123162ab603c7d7d2dd7dd901a07 \
-    --hash=sha256:e3e7065cbdabe6183ab82199d7a4f6b3ba0a438c5a512a68559846ccb76a78ec \
-    --hash=sha256:eed82cdf79cd7f0232e2fdc1ad05b06a5e102a43e331f7d041e5f0e0a34a51c4 \
-    --hash=sha256:f970663fa4f7e80401a7b0cbeec00fa801bf0287d93d48368fc3e6fa32716245 \
-    --hash=sha256:f9b2fdca47dc855516b2d66eef3c39f2672cbf7e7a42e7e67ad2cbfcd6ba107d
-zipp==3.18.1 ; python_version >= "3.9" and python_version < "3.10" \
+virtualenv==20.25.3 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:7bb554bbdfeaacc3349fa614ea5bff6ac300fc7c335e9facf3a3bcfc703f45be \
+    --hash=sha256:8aac4332f2ea6ef519c648d0bc48a5b1d324994753519919bddbb1aff25a104e
+xattr==1.1.0 ; python_version >= "3.9" and python_version < "4.0" and sys_platform == "darwin" \
+    --hash=sha256:00d2b415cf9d6a24112d019e721aa2a85652f7bbc9f3b9574b2d1cd8668eb491 \
+    --hash=sha256:0683dae7609f7280b0c89774d00b5957e6ffcb181c6019c46632b389706b77e6 \
+    --hash=sha256:08f61cbed52dc6f7c181455826a9ff1e375ad86f67dd9d5eb7663574abb32451 \
+    --hash=sha256:0a9c431b0e66516a078125e9a273251d4b8e5ba84fe644b619f2725050d688a0 \
+    --hash=sha256:0f06e0c1e4d06b4e0e49aaa1184b6f0e81c3758c2e8365597918054890763b53 \
+    --hash=sha256:1a5921ea3313cc1c57f2f53b63ea8ca9a91e48f4cc7ebec057d2447ec82c7efe \
+    --hash=sha256:23705c7079b05761ff2fa778ad17396e7599c8759401abc05b312dfb3bc99f69 \
+    --hash=sha256:24d97f0d28f63695e3344ffdabca9fcc30c33e5c8ccc198c7524361a98d526f2 \
+    --hash=sha256:27272afeba8422f2a9d27e1080a9a7b807394e88cce73db9ed8d2dde3afcfb87 \
+    --hash=sha256:46a641ac038a9f53d2f696716147ca4dbd6a01998dc9cd4bc628801bc0df7f4d \
+    --hash=sha256:47a3bdfe034b4fdb70e5941d97037405e3904accc28e10dbef6d1c9061fb6fd7 \
+    --hash=sha256:4cb70c16e7c3ae6ba0ab6c6835c8448c61d8caf43ea63b813af1f4dbe83dd156 \
+    --hash=sha256:54cb15cd94e5ef8a0ef02309f1bf973ba0e13c11e87686e983f371948cfee6af \
+    --hash=sha256:6461a43b585e5f2e049b39bcbfcb6391bfef3c5118231f1b15d10bdb89ef17fe \
+    --hash=sha256:6480589c1dac7785d1f851347a32c4a97305937bf7b488b857fe8b28a25de9e9 \
+    --hash=sha256:687e7d18611ef8d84a6ecd8f4d1ab6757500c1302f4c2046ce0aa3585e13da3f \
+    --hash=sha256:6881b120f9a4b36ccd8a28d933bc0f6e1de67218b6ce6e66874e0280fc006844 \
+    --hash=sha256:6ad47d89968c9097900607457a0c89160b4771601d813e769f68263755516065 \
+    --hash=sha256:78b377832dd0ee408f9f121a354082c6346960f7b6b1480483ed0618b1912120 \
+    --hash=sha256:793c01deaadac50926c0e1481702133260c7cb5e62116762f6fe1543d07b826f \
+    --hash=sha256:7a92aff66c43fa3e44cbeab7cbeee66266c91178a0f595e044bf3ce51485743b \
+    --hash=sha256:7e4ca0956fd11679bb2e0c0d6b9cdc0f25470cc00d8da173bb7656cc9a9cf104 \
+    --hash=sha256:83652910ef6a368b77b00825ad67815e5c92bfab551a848ca66e9981d14a7519 \
+    --hash=sha256:9013f290387f1ac90bccbb1926555ca9aef75651271098d99217284d9e010f7c \
+    --hash=sha256:918e1f83f2e8a072da2671eac710871ee5af337e9bf8554b5ce7f20cdb113186 \
+    --hash=sha256:96ca300c0acca4f0cddd2332bb860ef58e1465d376364f0e72a1823fdd58e90d \
+    --hash=sha256:9b1664edf003153ac8d1911e83a0fc60db1b1b374ee8ac943f215f93754a1102 \
+    --hash=sha256:9c5a78c7558989492c4cb7242e490ffb03482437bf782967dfff114e44242343 \
+    --hash=sha256:9d4f71b673339aeaae1f6ea9ef8ea6c9643c8cd0df5003b9a0eaa75403e2e06c \
+    --hash=sha256:9dcd5dfbcee73c7be057676ecb900cabb46c691aff4397bf48c579ffb30bb963 \
+    --hash=sha256:a20de1c47b5cd7b47da61799a3b34e11e5815d716299351f82a88627a43f9a96 \
+    --hash=sha256:afacebbc1fa519f41728f8746a92da891c7755e6745164bd0d5739face318e86 \
+    --hash=sha256:b0d73150f2f9655b4da01c2369eb33a294b7f9d56eccb089819eafdbeb99f896 \
+    --hash=sha256:b489b7916f239100956ea0b39c504f3c3a00258ba65677e4c8ba1bd0b5513446 \
+    --hash=sha256:b6ceb9efe0657a982ccb8b8a2efe96b690891779584c901d2f920784e5d20ae3 \
+    --hash=sha256:b735ac2625a4fc2c9343b19f806793db6494336338537d2911c8ee4c390dda46 \
+    --hash=sha256:caab2c2986c30f92301f12e9c50415d324412e8e6a739a52a603c3e6a54b3610 \
+    --hash=sha256:ccab735d0632fe71f7d72e72adf886f45c18b7787430467ce0070207882cfe25 \
+    --hash=sha256:cd11e917f5b89f2a0ad639d9875943806c6c9309a3dd02da5a3e8ef92db7bed9 \
+    --hash=sha256:cebcf8a303a44fbc439b68321408af7267507c0d8643229dbb107f6c132d389c \
+    --hash=sha256:d1059b2f726e2702c8bbf9bbf369acfc042202a4cc576c2dec6791234ad5e948 \
+    --hash=sha256:d1418705f253b6b6a7224b69773842cac83fcbcd12870354b6e11dd1cd54630f \
+    --hash=sha256:d44e8f955218638c9ab222eed21e9bd9ab430d296caf2176fb37abe69a714e5c \
+    --hash=sha256:d6eb7d5f281014cd44e2d847a9107491af1bf3087f5afeded75ed3e37ec87239 \
+    --hash=sha256:dab29d9288aa28e68a6f355ddfc3f0a7342b40c9012798829f3e7bd765e85c2c \
+    --hash=sha256:dba4f80b9855cc98513ddf22b7ad8551bc448c70d3147799ea4f6c0b758fb466 \
+    --hash=sha256:dc53cab265f6e8449bd683d5ee3bc5a191e6dd940736f3de1a188e6da66b0653 \
+    --hash=sha256:dd43978966de3baf4aea367c99ffa102b289d6c2ea5f3d9ce34a203dc2f2ab73 \
+    --hash=sha256:dda2684228798e937a7c29b0e1c7ef3d70e2b85390a69b42a1c61b2039ba81de \
+    --hash=sha256:ded771eaf27bb4eb3c64c0d09866460ee8801d81dc21097269cf495b3cac8657 \
+    --hash=sha256:e0c80bbf55339c93770fc294b4b6586b5bf8e85ec00a4c2d585c33dbd84b5006 \
+    --hash=sha256:e189e440bcd04ccaad0474720abee6ee64890823ec0db361fb0a4fb5e843a1bf \
+    --hash=sha256:e2255f36ebf2cb2dbf772a7437ad870836b7396e60517211834cf66ce678b595 \
+    --hash=sha256:ef2fa0f85458736178fd3dcfeb09c3cf423f0843313e25391db2cfd1acec8888 \
+    --hash=sha256:f6ad2a7bd5e6cf71d4a862413234a067cf158ca0ae94a40d4b87b98b62808498 \
+    --hash=sha256:fa6a7af7a4ada43f15ccc58b6f9adcdbff4c36ba040013d2681e589e07ae280a \
+    --hash=sha256:fecbf3b05043ed3487a28190dec3e4c4d879b2fcec0e30bafd8ec5d4b6043630 \
+    --hash=sha256:ff6223a854229055e803c2ad0c0ea9a6da50c6be30d92c198cf5f9f28819a921
+zipp==3.18.1 ; python_version >= "3.9" and python_version < "3.12" \
     --hash=sha256:206f5a15f2af3dbaee80769fb7dc6f249695e940acca08dfb2a4769fe61e538b \
     --hash=sha256:2884ed22e7d8961de1c9a05142eb69a247f120291bc0206a00a7642f09b5b715
```

### Comparing `alluka-0.1.5/piped/python/base-requirements/flake8.txt` & `alluka-0.2.0/piped/python/base-requirements/flake8.txt`

 * *Files identical despite different names*

### Comparing `alluka-0.1.5/piped/python/base-requirements/library-flake8.in` & `alluka-0.2.0/piped/python/base-requirements/library-flake8.in`

 * *Files identical despite different names*

### Comparing `alluka-0.1.5/piped/python/base-requirements/library-flake8.txt` & `alluka-0.2.0/piped/python/base-requirements/library-flake8.txt`

 * *Files identical despite different names*

### Comparing `alluka-0.1.5/piped/python/base-requirements/lint.txt` & `alluka-0.2.0/piped/python/base-requirements/lint.txt`

 * *Files identical despite different names*

### Comparing `alluka-0.1.5/piped/python/base-requirements/nox.txt` & `alluka-0.2.0/piped/python/base-requirements/nox.txt`

 * *Files identical despite different names*

### Comparing `alluka-0.1.5/piped/python/base-requirements/publish.txt` & `alluka-0.2.0/piped/python/base-requirements/publish.txt`

 * *Files identical despite different names*

### Comparing `alluka-0.1.5/piped/python/base-requirements/reformat.txt` & `alluka-0.2.0/piped/python/base-requirements/reformat.txt`

 * *Files identical despite different names*

### Comparing `alluka-0.1.5/piped/python/base-requirements/tests.txt` & `alluka-0.2.0/piped/python/base-requirements/tests.txt`

 * *Files identical despite different names*

### Comparing `alluka-0.1.5/piped/python/base-requirements/type-checking.txt` & `alluka-0.2.0/piped/python/base-requirements/type-checking.txt`

 * *Files identical despite different names*

### Comparing `alluka-0.1.5/piped/python/noxfile.py` & `alluka-0.2.0/piped/python/noxfile.py`

 * *Files identical despite different names*

### Comparing `alluka-0.1.5/piped/python/noxfile.template.py` & `alluka-0.2.0/piped/python/noxfile.template.py`

 * *Files identical despite different names*

### Comparing `alluka-0.1.5/piped/python/piped_shared/__init__.py` & `alluka-0.2.0/piped/python/piped_shared/__init__.py`

 * *Files identical despite different names*

### Comparing `alluka-0.1.5/pyproject.toml` & `alluka-0.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.3,<4,!=3.7"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "alluka"
-version = "0.1.5"
+version = "0.2.0"
 readme = "README.md"
 requires-python = ">=3.9.0,<3.13"
 license = {file = "LICENSE"}
 authors = [ {name = "Faster Speeding", email="lucina@lmbyrne.dev"} ]
 keywords = ["DI", "injection"]
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -25,15 +25,15 @@
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Utilities",
     "Typing :: Typed"
 ]
-dependencies = []
+dependencies = ["typing-extensions>=4.5, <5"]
 dynamic = ["description"]
 
 [project.urls]
 Homepage = "https://github.com/FasterSpeeding/Alluka"
 Repository = "https://github.com/FasterSpeeding/Alluka"
 Documentation = "https://alluka.cursed.solutions/"
 Changelog = "https://alluka.cursed.solutions/changelog"
@@ -102,14 +102,15 @@
     "E231",    # missing whitespace after ','
     "E701",    # Incompatible with black: E701 multiple statements on one line (colon)
     "E704",    # Incompatible with black: E704 multiple statements on one line (def)
 ]
 # Doc errors don't matter in the tests
 per-file-ignores = [
     "alluka/py.typed: D100",
+    "docs_src/*.py: ASYNC910, ASYNC911, DALL000, D100, D101, D103, E800, FA100, FA101, F841, INP001, M511, N806, TC001, TC101, VNE002",
     "noxfile.py: D100, FA101, F401, F403, INP001",
     "tests/*.py: ASYNC910, CCE002, DALL000, D100, D101, D103, D104, FA100, FA101, M511"
 ]
 
 [tool.isort]
 profile = "black"
 force_single_line = true
@@ -145,15 +146,15 @@
     "verify-types",
 ]
 extra_test_installs = ["."]
 mypy_allowed_to_fail = true
 mypy_targets = ["alluka"]
 path_ignore = "^alluka\\/_vendor\\/"
 project_name = "alluka"
-top_level_targets = ["./alluka", "./noxfile.py", "./tests"]
+top_level_targets = ["./alluka", "./docs_src", "./noxfile.py", "./tests"]
 
 [tool.piped.github_actions.freeze_for_pr]
 [tool.piped.github_actions.lint]
 [tool.piped.github_actions.pr_docs]
 [tool.piped.github_actions.publish]
 [tool.piped.github_actions.py_test]
 codeclimate_token = "a965935acdc9066802d7201945219784c0f24d22e8a2dff0e6529207726bc8af"
@@ -164,17 +165,20 @@
 [tool.piped.github_actions.resync_piped]
 [tool.piped.github_actions.type_check]
 [tool.piped.github_actions.update_licence]
 [tool.piped.github_actions.upgrade_locks]
 [tool.piped.github_actions.verify_locks]
 [tool.piped.github_actions.verify_types]
 
+[tool.pycln]
+exclude = "docs_src"
+
 [tool.pyright]
 exclude = ["alluka/_vendor"]
-include = ["alluka", "noxfile.py", "tests"]
+include = ["alluka", "docs_src", "noxfile.py", "tests"]
 
 pythonVersion = "3.9"
 typeCheckingMode = "strict"
 reportMissingModuleSource = "error"  # Is only "warning" on strict mode.
 
 # Error code which are disabled even when general strict.
 reportShadowedImports = "error"
```

### Comparing `alluka-0.1.5/tests/__init__.py` & `alluka-0.2.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `alluka-0.1.5/tests/test__client.py` & `alluka-0.2.0/tests/test__client.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,26 +25,26 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
+# pyright: reportUnknownMemberType=none
+# pyright: reportPrivateUsage=none
+# pyright: reportIncompatibleMethodOverride=none
+
 import typing
 import warnings
 
 import mock
 import pytest
 
 import alluka
 
-# pyright: reportUnknownMemberType=none
-# pyright: reportPrivateUsage=none
-# pyright: reportIncompatibleMethodOverride=none
-
 
 def test_inject():
     descriptor = alluka.inject()
 
     assert descriptor.type is None
     assert descriptor.callback is None
 
@@ -73,27 +73,29 @@
 
 
 class TestClient:
     def test_as_async_self_injecting(self):
         mock_callback = mock.Mock()
         client = alluka.Client()
 
-        result = client.as_async_self_injecting(mock_callback)
+        with pytest.warns(DeprecationWarning):
+            result = client.as_async_self_injecting(mock_callback)  # pyright: ignore[reportDeprecated]
 
-        assert isinstance(result, alluka.AsyncSelfInjecting)
+        assert isinstance(result, alluka.AsyncSelfInjecting)  # pyright: ignore[reportDeprecated]
         assert result._callback is mock_callback
         assert result._client is client
 
     def test_as_self_injecting(self):
         mock_callback = mock.Mock()
         client = alluka.Client()
 
-        result = client.as_self_injecting(mock_callback)
+        with pytest.warns(DeprecationWarning):
+            result = client.as_self_injecting(mock_callback)  # pyright: ignore[reportDeprecated]
 
-        assert isinstance(result, alluka.SelfInjecting)
+        assert isinstance(result, alluka.SelfInjecting)  # pyright: ignore[reportDeprecated]
         assert result._callback is mock_callback
         assert result._client is client
 
     def test_call_with_di(self):
         class MockType1: ...
 
         class MockType2: ...
@@ -246,21 +248,18 @@
         client = alluka.Client()
 
         with pytest.raises(alluka.MissingDependencyError):
             await client.call_with_async_di(callback)
 
     def test_set_type_dependency_when_not_found(self):
         mock_type: typing.Any = mock.Mock()
-        mock_value = mock.Mock()
         client = alluka.Client()
 
-        result = client.set_type_dependency(mock_type, mock_value)
-
-        assert result is client
-        assert client.get_type_dependency(mock_type) is mock_value
+        with pytest.raises(KeyError):
+            client.get_type_dependency(mock_type)
 
     def test_get_type_dependency_when_not_found_and_default(self):
         mock_type: typing.Any = mock.Mock()
         default = object()
         client = alluka.Client()
 
         result = client.get_type_dependency(mock_type, default=default)
@@ -271,15 +270,17 @@
         mock_type: typing.Any = mock.Mock()
         client = alluka.Client()
         client.set_type_dependency(mock_type, mock.Mock())
 
         result = client.remove_type_dependency(mock_type)
 
         assert result is client
-        assert client.get_type_dependency(mock_type) is alluka.abc.UNDEFINED
+
+        with pytest.raises(KeyError):
+            assert client.get_type_dependency(mock_type)
 
     def test_remove_type_dependency_when_not_set(self):
         mock_type: typing.Any = mock.Mock()
         client = alluka.Client()
 
         with pytest.raises(KeyError):
             client.remove_type_dependency(mock_type)
@@ -331,15 +332,16 @@
         ctx.cache_result(mock_callback, mock_result)
 
         assert ctx.get_cached_result(mock_callback) is mock_result
 
     def test_get_cached_result_when_not_found(self):
         ctx = alluka.BasicContext(alluka.Client())
 
-        assert ctx.get_cached_result(mock.Mock()) is alluka.abc.UNDEFINED
+        with pytest.raises(KeyError):
+            ctx.get_cached_result(mock.Mock())
 
     def test_get_cached_result_when_not_found_and_default(self):
         ctx = alluka.BasicContext(alluka.Client())
         default = object()
 
         assert ctx.get_cached_result(mock.Mock(), default=default) is default
```

### Comparing `alluka-0.1.5/tests/test__self_injecting.py` & `alluka-0.2.0/tests/test__self_injecting.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,50 +24,59 @@
 # DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+
+# pyright: reportDeprecated=none
+
 import mock
 import pytest
 
 import alluka
 
 
 class TestAsyncSelfInjecting:
     @pytest.mark.anyio
     async def test_call_dunder_method(self):
         mock_callback = mock.Mock()
         mock_client = mock.AsyncMock()
-        self_injecting = alluka.AsyncSelfInjecting(mock_client, mock_callback)
+
+        with pytest.warns(DeprecationWarning):
+            self_injecting = alluka.AsyncSelfInjecting(mock_client, mock_callback)
 
         result = await self_injecting()
 
         assert result is mock_client.call_with_async_di.return_value
         mock_client.call_with_async_di.assert_awaited_once_with(mock_callback)
 
     def test_callback_property(self):
         mock_callback = mock.Mock()
 
-        self_injecting = alluka.AsyncSelfInjecting(mock.Mock(), mock_callback)
+        with pytest.warns(DeprecationWarning):
+            self_injecting = alluka.AsyncSelfInjecting(mock.Mock(), mock_callback)
 
         assert self_injecting.callback is mock_callback
 
 
 class TestSelfInjecting:
     def test_call_dunder_method(self):
         mock_callback = mock.Mock()
         mock_client = mock.Mock()
-        self_injecting = alluka.SelfInjecting(mock_client, mock_callback)
+
+        with pytest.warns(DeprecationWarning):
+            self_injecting = alluka.SelfInjecting(mock_client, mock_callback)
 
         result = self_injecting()
 
         assert result is mock_client.call_with_di.return_value
         mock_client.call_with_di.assert_called_once_with(mock_callback)
 
     def test_callback_property(self):
         mock_callback = mock.Mock()
 
-        self_injecting = alluka.SelfInjecting(mock.Mock(), mock_callback)
+        with pytest.warns(DeprecationWarning):
+            self_injecting = alluka.SelfInjecting(mock.Mock(), mock_callback)
 
         assert self_injecting.callback is mock_callback
```

### Comparing `alluka-0.1.5/tests/test_async_callback_di.py` & `alluka-0.2.0/tests/test_async_callback_di.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -25,27 +25,27 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
+# pyright: reportUnknownMemberType=none
+# pyright: reportPrivateUsage=none
+# pyright: reportIncompatibleMethodOverride=none
+
 import sys
 import typing
 
 import mock
 import pytest
 
 import alluka
 from alluka._vendor import inspect
 
-# pyright: reportUnknownMemberType=none
-# pyright: reportPrivateUsage=none
-# pyright: reportIncompatibleMethodOverride=none
-
 
 class MockType(int): ...
 
 
 class MockOtherType(int): ...
```

### Comparing `alluka-0.1.5/tests/test_async_callback_di_future_annotations.py` & `alluka-0.2.0/tests/test_async_callback_di_future_annotations.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,29 +25,30 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
+# pyright: reportUnknownMemberType=none
+# pyright: reportPrivateUsage=none
+# pyright: reportIncompatibleMethodOverride=none
+
+
 from __future__ import annotations
 
 import sys
 import typing
 
 import mock
 import pytest
 
 import alluka
 from alluka._vendor import inspect
 
-# pyright: reportUnknownMemberType=none
-# pyright: reportPrivateUsage=none
-# pyright: reportIncompatibleMethodOverride=none
-
 
 class MockType(int): ...
 
 
 class MockOtherType(int): ...
```

### Comparing `alluka-0.1.5/tests/test_callback_di.py` & `alluka-0.2.0/tests/test_callback_di.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,28 +25,29 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
+# pyright: reportUnknownMemberType=none
+# pyright: reportPrivateUsage=none
+# pyright: reportIncompatibleMethodOverride=none
+
+
 import sys
 import typing
 import warnings
 
 import mock
 import pytest
 
 import alluka
 from alluka._vendor import inspect
 
-# pyright: reportUnknownMemberType=none
-# pyright: reportPrivateUsage=none
-# pyright: reportIncompatibleMethodOverride=none
-
 
 class MockType(int): ...
 
 
 class MockOtherType(int): ...
```

### Comparing `alluka-0.1.5/tests/test_callback_di_future_annotations.py` & `alluka-0.2.0/tests/test_callback_di_future_annotations.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -25,30 +25,30 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
+# pyright: reportUnknownMemberType=none
+# pyright: reportPrivateUsage=none
+# pyright: reportIncompatibleMethodOverride=none
+
 from __future__ import annotations
 
 import sys
 import typing
 import warnings
 
 import mock
 import pytest
 
 import alluka
 from alluka._vendor import inspect
 
-# pyright: reportUnknownMemberType=none
-# pyright: reportPrivateUsage=none
-# pyright: reportIncompatibleMethodOverride=none
-
 
 class MockType(int): ...
 
 
 class MockOtherType(int): ...
```

### Comparing `alluka-0.1.5/PKG-INFO` & `alluka-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alluka
-Version: 0.1.5
+Version: 0.2.0
 Summary: A type based dependency injection framework for Python 3.9+.
 Keywords: DI,injection
 Author-email: Faster Speeding <lucina@lmbyrne.dev>
 Requires-Python: >=3.9.0,<3.13
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AnyIO
@@ -19,14 +19,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
+Requires-Dist: typing-extensions>=4.5, <5
 Project-URL: Changelog, https://alluka.cursed.solutions/changelog
 Project-URL: Documentation, https://alluka.cursed.solutions/
 Project-URL: Homepage, https://github.com/FasterSpeeding/Alluka
 Project-URL: Repository, https://github.com/FasterSpeeding/Alluka
 
 # Alluka
```

