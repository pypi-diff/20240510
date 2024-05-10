# Comparing `tmp/llmstudio-0.3.4a1.tar.gz` & `tmp/llmstudio-0.3.4a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmstudio-0.3.4a1.tar", max compression
+gzip compressed data, was "llmstudio-0.3.4a2.tar", max compression
```

## Comparing `llmstudio-0.3.4a1.tar` & `llmstudio-0.3.4a2.tar`

### file list

```diff
@@ -1,137 +1,137 @@
--rw-r--r--   0        0        0    16725 2024-04-12 13:53:28.367324 llmstudio-0.3.4a1/LICENSE
--rw-r--r--   0        0        0     4185 2024-04-12 13:53:28.367324 llmstudio-0.3.4a1/README.md
--rw-r--r--   0        0        0       30 2024-04-12 13:53:28.367324 llmstudio-0.3.4a1/llmstudio/__init__.py
--rw-r--r--   0        0        0     2509 2024-04-12 13:53:28.367324 llmstudio-0.3.4a1/llmstudio/cli.py
--rw-r--r--   0        0        0       56 2024-04-12 13:53:28.367324 llmstudio-0.3.4a1/llmstudio/client.py
--rw-r--r--   0        0        0     1573 2024-04-12 13:53:28.367324 llmstudio-0.3.4a1/llmstudio/config.py
--rw-r--r--   0        0        0     6177 2024-04-12 13:53:28.367324 llmstudio-0.3.4a1/llmstudio/engine/__init__.py
--rw-r--r--   0        0        0     5623 2024-04-12 13:53:28.367324 llmstudio-0.3.4a1/llmstudio/engine/config.yaml
--rw-r--r--   0        0        0      314 2024-04-12 13:53:28.367324 llmstudio-0.3.4a1/llmstudio/engine/providers/__init__.py
--rw-r--r--   0        0        0     3434 2024-04-12 13:53:28.367324 llmstudio-0.3.4a1/llmstudio/engine/providers/anthropic.py
--rw-r--r--   0        0        0     2569 2024-04-12 13:53:28.367324 llmstudio-0.3.4a1/llmstudio/engine/providers/azure.py
--rw-r--r--   0        0        0     3227 2024-04-12 13:53:28.367324 llmstudio-0.3.4a1/llmstudio/engine/providers/ollama.py
--rw-r--r--   0        0        0     2194 2024-04-12 13:53:28.367324 llmstudio-0.3.4a1/llmstudio/engine/providers/openai.py
--rw-r--r--   0        0        0    13776 2024-04-12 13:53:28.367324 llmstudio-0.3.4a1/llmstudio/engine/providers/provider.py
--rw-r--r--   0        0        0     3844 2024-04-12 13:53:28.367324 llmstudio-0.3.4a1/llmstudio/llm/__init__.py
--rw-r--r--   0        0        0     2114 2024-04-12 13:53:28.367324 llmstudio-0.3.4a1/llmstudio/llm/langchain.py
--rw-r--r--   0        0        0        0 2024-04-12 13:53:28.367324 llmstudio-0.3.4a1/llmstudio/tests/__init__.py
--rw-r--r--   0        0        0     1165 2024-04-12 13:53:28.367324 llmstudio-0.3.4a1/llmstudio/tests/conftest.py
--rw-r--r--   0        0        0     3007 2024-04-12 13:53:28.367324 llmstudio-0.3.4a1/llmstudio/tests/engine/test_engine.py
--rw-r--r--   0        0        0     3926 2024-04-12 13:53:28.367324 llmstudio-0.3.4a1/llmstudio/tests/engine/test_providers.py
--rw-r--r--   0        0        0     1800 2024-04-12 13:53:28.367324 llmstudio-0.3.4a1/llmstudio/tracking/__init__.py
--rw-r--r--   0        0        0      575 2024-04-12 13:53:28.367324 llmstudio-0.3.4a1/llmstudio/tracking/database.py
--rw-r--r--   0        0        0        0 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/tracking/logs/__init__.py
--rw-r--r--   0        0        0      797 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/tracking/logs/crud.py
--rw-r--r--   0        0        0     1513 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/tracking/logs/endpoints.py
--rw-r--r--   0        0        0      578 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/tracking/logs/models.py
--rw-r--r--   0        0        0      834 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/tracking/logs/schemas.py
--rw-r--r--   0        0        0        0 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/tracking/session/__init__.py
--rw-r--r--   0        0        0     1339 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/tracking/session/crud.py
--rw-r--r--   0        0        0     1438 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/tracking/session/endpoints.py
--rw-r--r--   0        0        0      554 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/tracking/session/models.py
--rw-r--r--   0        0        0      409 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/tracking/session/schemas.py
--rw-r--r--   0        0        0     1459 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/tracking/tracker.py
--rw-r--r--   0        0        0       40 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/.eslintrc.json
--rw-r--r--   0        0        0      391 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/.gitignore
--rw-r--r--   0        0        0      157 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/.prettierrc.json
--rw-r--r--   0        0        0      601 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/__init__.py
--rw-r--r--   0        0        0      327 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/components.json
--rw-r--r--   0        0        0       98 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/global.d.ts
--rw-r--r--   0        0        0       94 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/next.config.js
--rw-r--r--   0        0        0   154026 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/package-lock.json
--rw-r--r--   0        0        0     2697 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/package.json
--rw-r--r--   0        0        0       82 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/postcss.config.js
--rw-r--r--   0        0        0    34679 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/public/logo.json
--rw-r--r--   0        0        0     1026 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/public/svg/ai.svg
--rw-r--r--   0        0        0      212 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/public/svg/arrow.svg
--rw-r--r--   0        0        0      617 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/public/svg/compare.svg
--rw-r--r--   0        0        0      872 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/public/svg/home.svg
--rw-r--r--   0        0        0      482 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/public/svg/load.svg
--rw-r--r--   0        0        0     2894 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/public/svg/magic.svg
--rw-r--r--   0        0        0      535 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/public/svg/play.svg
--rw-r--r--   0        0        0     4669 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/public/svg/playground.svg
--rw-r--r--   0        0        0      526 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/public/svg/plus.svg
--rw-r--r--   0        0        0     1243 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/public/svg/settings.svg
--rw-r--r--   0        0        0     1803 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/public/svg/sparkles.svg
--rw-r--r--   0        0        0      118 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/compare/page.tsx
--rw-r--r--   0        0        0      992 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/dashboard/hooks/useDashboardFetch.tsx
--rw-r--r--   0        0        0     3719 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/dashboard/page.tsx
--rw-r--r--   0        0        0     2200 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/components/DataTable/ColumnHeader.tsx
--rw-r--r--   0        0        0     3847 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/components/DataTable/DataTable.tsx
--rw-r--r--   0        0        0     4986 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/components/DataTable/FacetedFilter.tsx
--rw-r--r--   0        0        0     3301 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/components/DataTable/Pagination.tsx
--rw-r--r--   0        0        0     1635 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/components/DataTable/RowActions.tsx
--rw-r--r--   0        0        0     1333 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/components/DataTable/Toolbar.tsx
--rw-r--r--   0        0        0     1942 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/components/DataTable/UserNav.tsx
--rw-r--r--   0        0        0     1671 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/components/DataTable/ViewOptions.tsx
--rw-r--r--   0        0        0     7206 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/components/DataTable/columns.tsx
--rw-r--r--   0        0        0     1982 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/components/Input.tsx
--rw-r--r--   0        0        0     1539 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/components/LogSheet.tsx
--rw-r--r--   0        0        0      639 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/components/ModelItem.tsx
--rw-r--r--   0        0        0     2561 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/components/ModelSelector.tsx
--rw-r--r--   0        0        0     1131 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/components/Output.tsx
--rw-r--r--   0        0        0     2777 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/components/Parameters.tsx
--rw-r--r--   0        0        0      266 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/components/index.tsx
--rw-r--r--   0        0        0     1239 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/hooks/useChat.tsx
--rw-r--r--   0        0        0     1013 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/hooks/useExport.tsx
--rw-r--r--   0        0        0      654 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/hooks/useLogsFetch.tsx
--rw-r--r--   0        0        0      957 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/hooks/useModelFetch.tsx
--rw-r--r--   0        0        0     1092 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/hooks/useParameterFetch.tsx
--rw-r--r--   0        0        0      707 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/page.tsx
--rw-r--r--   0        0        0     1917 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/store.tsx
--rw-r--r--   0        0        0    15406 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/app/favicon.ico
--rw-r--r--   0        0        0     1567 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/app/globals.css
--rw-r--r--   0        0        0      858 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/app/layout.tsx
--rw-r--r--   0        0        0      223 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/app/page.tsx
--rw-r--r--   0        0        0     1721 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/components/CodeBlock/index.tsx
--rw-r--r--   0        0        0     2840 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/components/CopyButton/index.tsx
--rw-r--r--   0        0        0     1507 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/components/Header/index.tsx
--rw-r--r--   0        0        0     6315 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/components/Markdown/index.tsx
--rw-r--r--   0        0        0      871 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/components/Theme/index.tsx
--rw-r--r--   0        0        0      323 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/components/Toaster/index.tsx
--rw-r--r--   0        0        0      332 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/components/theme-provider.tsx
--rw-r--r--   0        0        0     1991 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/accordion.tsx
--rw-r--r--   0        0        0     4455 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/alert-dialog.tsx
--rw-r--r--   0        0        0     1584 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/alert.tsx
--rw-r--r--   0        0        0      154 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/aspect-ratio.tsx
--rw-r--r--   0        0        0     1419 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/avatar.tsx
--rw-r--r--   0        0        0     1128 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/badge.tsx
--rw-r--r--   0        0        0     1835 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/button.tsx
--rw-r--r--   0        0        0     2623 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/calendar.tsx
--rw-r--r--   0        0        0     1877 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/card.tsx
--rw-r--r--   0        0        0     1070 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/checkbox.tsx
--rw-r--r--   0        0        0      329 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/collapsible.tsx
--rw-r--r--   0        0        0     4867 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/command.tsx
--rw-r--r--   0        0        0     7260 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/context-menu.tsx
--rw-r--r--   0        0        0     3870 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/dialog.tsx
--rw-r--r--   0        0        0     7309 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/dropdown-menu.tsx
--rw-r--r--   0        0        0     4085 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/form.tsx
--rw-r--r--   0        0        0     1198 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/hover-card.tsx
--rw-r--r--   0        0        0      824 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/input.tsx
--rw-r--r--   0        0        0      724 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/label.tsx
--rw-r--r--   0        0        0     7988 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/menubar.tsx
--rw-r--r--   0        0        0     5046 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/navigation-menu.tsx
--rw-r--r--   0        0        0     1244 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/popover.tsx
--rw-r--r--   0        0        0      791 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/progress.tsx
--rw-r--r--   0        0        0     1481 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/radio-group.tsx
--rw-r--r--   0        0        0     1656 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/scroll-area.tsx
--rw-r--r--   0        0        0     5629 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/select.tsx
--rw-r--r--   0        0        0      770 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/separator.tsx
--rw-r--r--   0        0        0     4302 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/sheet.tsx
--rw-r--r--   0        0        0      261 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/skeleton.tsx
--rw-r--r--   0        0        0     1091 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/slider.tsx
--rw-r--r--   0        0        0     1153 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/switch.tsx
--rw-r--r--   0        0        0     2765 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/table.tsx
--rw-r--r--   0        0        0     1897 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/tabs.tsx
--rw-r--r--   0        0        0      772 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/textarea.tsx
--rw-r--r--   0        0        0     4845 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/toast.tsx
--rw-r--r--   0        0        0      794 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/toaster.tsx
--rw-r--r--   0        0        0     1748 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/toggle-group.tsx
--rw-r--r--   0        0        0     1449 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/toggle.tsx
--rw-r--r--   0        0        0     1159 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/tooltip.tsx
--rw-r--r--   0        0        0     3934 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/use-toast.ts
--rw-r--r--   0        0        0     1802 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/lib/utils.ts
--rw-r--r--   0        0        0     6560 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/tailwind.config.js
--rw-r--r--   0        0        0      694 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/tsconfig.json
--rw-r--r--   0        0        0     1075 2024-04-12 13:53:41.399306 llmstudio-0.3.4a1/pyproject.toml
--rw-r--r--   0        0        0     5550 1970-01-01 00:00:00.000000 llmstudio-0.3.4a1/PKG-INFO
+-rw-r--r--   0        0        0    16725 2024-04-23 16:08:49.429131 llmstudio-0.3.4a2/LICENSE
+-rw-r--r--   0        0        0     4185 2024-04-23 16:08:49.429131 llmstudio-0.3.4a2/README.md
+-rw-r--r--   0        0        0       30 2024-04-23 16:08:49.429131 llmstudio-0.3.4a2/llmstudio/__init__.py
+-rw-r--r--   0        0        0     2509 2024-04-23 16:08:49.429131 llmstudio-0.3.4a2/llmstudio/cli.py
+-rw-r--r--   0        0        0       56 2024-04-23 16:08:49.429131 llmstudio-0.3.4a2/llmstudio/client.py
+-rw-r--r--   0        0        0     1573 2024-04-23 16:08:49.429131 llmstudio-0.3.4a2/llmstudio/config.py
+-rw-r--r--   0        0        0     6177 2024-04-23 16:08:49.429131 llmstudio-0.3.4a2/llmstudio/engine/__init__.py
+-rw-r--r--   0        0        0     5623 2024-04-23 16:08:49.429131 llmstudio-0.3.4a2/llmstudio/engine/config.yaml
+-rw-r--r--   0        0        0      314 2024-04-23 16:08:49.429131 llmstudio-0.3.4a2/llmstudio/engine/providers/__init__.py
+-rw-r--r--   0        0        0     3434 2024-04-23 16:08:49.429131 llmstudio-0.3.4a2/llmstudio/engine/providers/anthropic.py
+-rw-r--r--   0        0        0     2569 2024-04-23 16:08:49.429131 llmstudio-0.3.4a2/llmstudio/engine/providers/azure.py
+-rw-r--r--   0        0        0     3227 2024-04-23 16:08:49.433131 llmstudio-0.3.4a2/llmstudio/engine/providers/ollama.py
+-rw-r--r--   0        0        0     2194 2024-04-23 16:08:49.433131 llmstudio-0.3.4a2/llmstudio/engine/providers/openai.py
+-rw-r--r--   0        0        0    13951 2024-04-23 16:08:49.433131 llmstudio-0.3.4a2/llmstudio/engine/providers/provider.py
+-rw-r--r--   0        0        0     3844 2024-04-23 16:08:49.433131 llmstudio-0.3.4a2/llmstudio/llm/__init__.py
+-rw-r--r--   0        0        0     2114 2024-04-23 16:08:49.433131 llmstudio-0.3.4a2/llmstudio/llm/langchain.py
+-rw-r--r--   0        0        0        0 2024-04-23 16:08:49.433131 llmstudio-0.3.4a2/llmstudio/tests/__init__.py
+-rw-r--r--   0        0        0     1165 2024-04-23 16:08:49.433131 llmstudio-0.3.4a2/llmstudio/tests/conftest.py
+-rw-r--r--   0        0        0     3007 2024-04-23 16:08:49.433131 llmstudio-0.3.4a2/llmstudio/tests/engine/test_engine.py
+-rw-r--r--   0        0        0     3926 2024-04-23 16:08:49.433131 llmstudio-0.3.4a2/llmstudio/tests/engine/test_providers.py
+-rw-r--r--   0        0        0     1800 2024-04-23 16:08:49.433131 llmstudio-0.3.4a2/llmstudio/tracking/__init__.py
+-rw-r--r--   0        0        0      575 2024-04-23 16:08:49.433131 llmstudio-0.3.4a2/llmstudio/tracking/database.py
+-rw-r--r--   0        0        0        0 2024-04-23 16:08:49.433131 llmstudio-0.3.4a2/llmstudio/tracking/logs/__init__.py
+-rw-r--r--   0        0        0      797 2024-04-23 16:08:49.433131 llmstudio-0.3.4a2/llmstudio/tracking/logs/crud.py
+-rw-r--r--   0        0        0     1513 2024-04-23 16:08:49.433131 llmstudio-0.3.4a2/llmstudio/tracking/logs/endpoints.py
+-rw-r--r--   0        0        0      578 2024-04-23 16:08:49.433131 llmstudio-0.3.4a2/llmstudio/tracking/logs/models.py
+-rw-r--r--   0        0        0      834 2024-04-23 16:08:49.433131 llmstudio-0.3.4a2/llmstudio/tracking/logs/schemas.py
+-rw-r--r--   0        0        0        0 2024-04-23 16:08:49.433131 llmstudio-0.3.4a2/llmstudio/tracking/session/__init__.py
+-rw-r--r--   0        0        0     1339 2024-04-23 16:08:49.433131 llmstudio-0.3.4a2/llmstudio/tracking/session/crud.py
+-rw-r--r--   0        0        0     1438 2024-04-23 16:08:49.433131 llmstudio-0.3.4a2/llmstudio/tracking/session/endpoints.py
+-rw-r--r--   0        0        0      554 2024-04-23 16:08:49.433131 llmstudio-0.3.4a2/llmstudio/tracking/session/models.py
+-rw-r--r--   0        0        0      409 2024-04-23 16:08:49.433131 llmstudio-0.3.4a2/llmstudio/tracking/session/schemas.py
+-rw-r--r--   0        0        0     1459 2024-04-23 16:08:49.433131 llmstudio-0.3.4a2/llmstudio/tracking/tracker.py
+-rw-r--r--   0        0        0       40 2024-04-23 16:08:49.433131 llmstudio-0.3.4a2/llmstudio/ui/.eslintrc.json
+-rw-r--r--   0        0        0      391 2024-04-23 16:08:49.433131 llmstudio-0.3.4a2/llmstudio/ui/.gitignore
+-rw-r--r--   0        0        0      157 2024-04-23 16:08:49.433131 llmstudio-0.3.4a2/llmstudio/ui/.prettierrc.json
+-rw-r--r--   0        0        0      601 2024-04-23 16:08:49.433131 llmstudio-0.3.4a2/llmstudio/ui/__init__.py
+-rw-r--r--   0        0        0      327 2024-04-23 16:08:49.433131 llmstudio-0.3.4a2/llmstudio/ui/components.json
+-rw-r--r--   0        0        0       98 2024-04-23 16:08:49.433131 llmstudio-0.3.4a2/llmstudio/ui/global.d.ts
+-rw-r--r--   0        0        0       94 2024-04-23 16:08:49.433131 llmstudio-0.3.4a2/llmstudio/ui/next.config.js
+-rw-r--r--   0        0        0   154026 2024-04-23 16:08:49.433131 llmstudio-0.3.4a2/llmstudio/ui/package-lock.json
+-rw-r--r--   0        0        0     2697 2024-04-23 16:08:49.433131 llmstudio-0.3.4a2/llmstudio/ui/package.json
+-rw-r--r--   0        0        0       82 2024-04-23 16:08:49.433131 llmstudio-0.3.4a2/llmstudio/ui/postcss.config.js
+-rw-r--r--   0        0        0    34679 2024-04-23 16:08:49.433131 llmstudio-0.3.4a2/llmstudio/ui/public/logo.json
+-rw-r--r--   0        0        0     1026 2024-04-23 16:08:49.433131 llmstudio-0.3.4a2/llmstudio/ui/public/svg/ai.svg
+-rw-r--r--   0        0        0      212 2024-04-23 16:08:49.433131 llmstudio-0.3.4a2/llmstudio/ui/public/svg/arrow.svg
+-rw-r--r--   0        0        0      617 2024-04-23 16:08:49.433131 llmstudio-0.3.4a2/llmstudio/ui/public/svg/compare.svg
+-rw-r--r--   0        0        0      872 2024-04-23 16:08:49.433131 llmstudio-0.3.4a2/llmstudio/ui/public/svg/home.svg
+-rw-r--r--   0        0        0      482 2024-04-23 16:08:49.433131 llmstudio-0.3.4a2/llmstudio/ui/public/svg/load.svg
+-rw-r--r--   0        0        0     2894 2024-04-23 16:08:49.433131 llmstudio-0.3.4a2/llmstudio/ui/public/svg/magic.svg
+-rw-r--r--   0        0        0      535 2024-04-23 16:08:49.433131 llmstudio-0.3.4a2/llmstudio/ui/public/svg/play.svg
+-rw-r--r--   0        0        0     4669 2024-04-23 16:08:49.433131 llmstudio-0.3.4a2/llmstudio/ui/public/svg/playground.svg
+-rw-r--r--   0        0        0      526 2024-04-23 16:08:49.433131 llmstudio-0.3.4a2/llmstudio/ui/public/svg/plus.svg
+-rw-r--r--   0        0        0     1243 2024-04-23 16:08:49.433131 llmstudio-0.3.4a2/llmstudio/ui/public/svg/settings.svg
+-rw-r--r--   0        0        0     1803 2024-04-23 16:08:49.433131 llmstudio-0.3.4a2/llmstudio/ui/public/svg/sparkles.svg
+-rw-r--r--   0        0        0      118 2024-04-23 16:08:49.433131 llmstudio-0.3.4a2/llmstudio/ui/src/app/(llm)/compare/page.tsx
+-rw-r--r--   0        0        0      992 2024-04-23 16:08:49.433131 llmstudio-0.3.4a2/llmstudio/ui/src/app/(llm)/dashboard/hooks/useDashboardFetch.tsx
+-rw-r--r--   0        0        0     3719 2024-04-23 16:08:49.433131 llmstudio-0.3.4a2/llmstudio/ui/src/app/(llm)/dashboard/page.tsx
+-rw-r--r--   0        0        0     2200 2024-04-23 16:08:49.433131 llmstudio-0.3.4a2/llmstudio/ui/src/app/(llm)/playground/components/DataTable/ColumnHeader.tsx
+-rw-r--r--   0        0        0     3847 2024-04-23 16:08:49.433131 llmstudio-0.3.4a2/llmstudio/ui/src/app/(llm)/playground/components/DataTable/DataTable.tsx
+-rw-r--r--   0        0        0     4986 2024-04-23 16:08:49.433131 llmstudio-0.3.4a2/llmstudio/ui/src/app/(llm)/playground/components/DataTable/FacetedFilter.tsx
+-rw-r--r--   0        0        0     3301 2024-04-23 16:08:49.433131 llmstudio-0.3.4a2/llmstudio/ui/src/app/(llm)/playground/components/DataTable/Pagination.tsx
+-rw-r--r--   0        0        0     1635 2024-04-23 16:08:49.433131 llmstudio-0.3.4a2/llmstudio/ui/src/app/(llm)/playground/components/DataTable/RowActions.tsx
+-rw-r--r--   0        0        0     1333 2024-04-23 16:08:49.433131 llmstudio-0.3.4a2/llmstudio/ui/src/app/(llm)/playground/components/DataTable/Toolbar.tsx
+-rw-r--r--   0        0        0     1942 2024-04-23 16:08:49.433131 llmstudio-0.3.4a2/llmstudio/ui/src/app/(llm)/playground/components/DataTable/UserNav.tsx
+-rw-r--r--   0        0        0     1671 2024-04-23 16:08:49.433131 llmstudio-0.3.4a2/llmstudio/ui/src/app/(llm)/playground/components/DataTable/ViewOptions.tsx
+-rw-r--r--   0        0        0     7206 2024-04-23 16:08:49.433131 llmstudio-0.3.4a2/llmstudio/ui/src/app/(llm)/playground/components/DataTable/columns.tsx
+-rw-r--r--   0        0        0     1982 2024-04-23 16:08:49.433131 llmstudio-0.3.4a2/llmstudio/ui/src/app/(llm)/playground/components/Input.tsx
+-rw-r--r--   0        0        0     1539 2024-04-23 16:08:49.433131 llmstudio-0.3.4a2/llmstudio/ui/src/app/(llm)/playground/components/LogSheet.tsx
+-rw-r--r--   0        0        0      639 2024-04-23 16:08:49.433131 llmstudio-0.3.4a2/llmstudio/ui/src/app/(llm)/playground/components/ModelItem.tsx
+-rw-r--r--   0        0        0     2561 2024-04-23 16:08:49.433131 llmstudio-0.3.4a2/llmstudio/ui/src/app/(llm)/playground/components/ModelSelector.tsx
+-rw-r--r--   0        0        0     1131 2024-04-23 16:08:49.433131 llmstudio-0.3.4a2/llmstudio/ui/src/app/(llm)/playground/components/Output.tsx
+-rw-r--r--   0        0        0     2777 2024-04-23 16:08:49.433131 llmstudio-0.3.4a2/llmstudio/ui/src/app/(llm)/playground/components/Parameters.tsx
+-rw-r--r--   0        0        0      266 2024-04-23 16:08:49.433131 llmstudio-0.3.4a2/llmstudio/ui/src/app/(llm)/playground/components/index.tsx
+-rw-r--r--   0        0        0     1239 2024-04-23 16:08:49.433131 llmstudio-0.3.4a2/llmstudio/ui/src/app/(llm)/playground/hooks/useChat.tsx
+-rw-r--r--   0        0        0     1013 2024-04-23 16:08:49.433131 llmstudio-0.3.4a2/llmstudio/ui/src/app/(llm)/playground/hooks/useExport.tsx
+-rw-r--r--   0        0        0      654 2024-04-23 16:08:49.433131 llmstudio-0.3.4a2/llmstudio/ui/src/app/(llm)/playground/hooks/useLogsFetch.tsx
+-rw-r--r--   0        0        0      957 2024-04-23 16:08:49.433131 llmstudio-0.3.4a2/llmstudio/ui/src/app/(llm)/playground/hooks/useModelFetch.tsx
+-rw-r--r--   0        0        0     1092 2024-04-23 16:08:49.433131 llmstudio-0.3.4a2/llmstudio/ui/src/app/(llm)/playground/hooks/useParameterFetch.tsx
+-rw-r--r--   0        0        0      707 2024-04-23 16:08:49.433131 llmstudio-0.3.4a2/llmstudio/ui/src/app/(llm)/playground/page.tsx
+-rw-r--r--   0        0        0     1917 2024-04-23 16:08:49.433131 llmstudio-0.3.4a2/llmstudio/ui/src/app/(llm)/playground/store.tsx
+-rw-r--r--   0        0        0    15406 2024-04-23 16:08:49.433131 llmstudio-0.3.4a2/llmstudio/ui/src/app/favicon.ico
+-rw-r--r--   0        0        0     1567 2024-04-23 16:08:49.433131 llmstudio-0.3.4a2/llmstudio/ui/src/app/globals.css
+-rw-r--r--   0        0        0      858 2024-04-23 16:08:49.433131 llmstudio-0.3.4a2/llmstudio/ui/src/app/layout.tsx
+-rw-r--r--   0        0        0      223 2024-04-23 16:08:49.433131 llmstudio-0.3.4a2/llmstudio/ui/src/app/page.tsx
+-rw-r--r--   0        0        0     1721 2024-04-23 16:08:49.433131 llmstudio-0.3.4a2/llmstudio/ui/src/components/CodeBlock/index.tsx
+-rw-r--r--   0        0        0     2840 2024-04-23 16:08:49.437131 llmstudio-0.3.4a2/llmstudio/ui/src/components/CopyButton/index.tsx
+-rw-r--r--   0        0        0     1507 2024-04-23 16:08:49.437131 llmstudio-0.3.4a2/llmstudio/ui/src/components/Header/index.tsx
+-rw-r--r--   0        0        0     6315 2024-04-23 16:08:49.437131 llmstudio-0.3.4a2/llmstudio/ui/src/components/Markdown/index.tsx
+-rw-r--r--   0        0        0      871 2024-04-23 16:08:49.437131 llmstudio-0.3.4a2/llmstudio/ui/src/components/Theme/index.tsx
+-rw-r--r--   0        0        0      323 2024-04-23 16:08:49.437131 llmstudio-0.3.4a2/llmstudio/ui/src/components/Toaster/index.tsx
+-rw-r--r--   0        0        0      332 2024-04-23 16:08:49.437131 llmstudio-0.3.4a2/llmstudio/ui/src/components/theme-provider.tsx
+-rw-r--r--   0        0        0     1991 2024-04-23 16:08:49.437131 llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/accordion.tsx
+-rw-r--r--   0        0        0     4455 2024-04-23 16:08:49.437131 llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/alert-dialog.tsx
+-rw-r--r--   0        0        0     1584 2024-04-23 16:08:49.437131 llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/alert.tsx
+-rw-r--r--   0        0        0      154 2024-04-23 16:08:49.437131 llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/aspect-ratio.tsx
+-rw-r--r--   0        0        0     1419 2024-04-23 16:08:49.437131 llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/avatar.tsx
+-rw-r--r--   0        0        0     1128 2024-04-23 16:08:49.437131 llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/badge.tsx
+-rw-r--r--   0        0        0     1835 2024-04-23 16:08:49.437131 llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/button.tsx
+-rw-r--r--   0        0        0     2623 2024-04-23 16:08:49.437131 llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/calendar.tsx
+-rw-r--r--   0        0        0     1877 2024-04-23 16:08:49.437131 llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/card.tsx
+-rw-r--r--   0        0        0     1070 2024-04-23 16:08:49.437131 llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/checkbox.tsx
+-rw-r--r--   0        0        0      329 2024-04-23 16:08:49.437131 llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/collapsible.tsx
+-rw-r--r--   0        0        0     4867 2024-04-23 16:08:49.437131 llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/command.tsx
+-rw-r--r--   0        0        0     7260 2024-04-23 16:08:49.437131 llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/context-menu.tsx
+-rw-r--r--   0        0        0     3870 2024-04-23 16:08:49.437131 llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/dialog.tsx
+-rw-r--r--   0        0        0     7309 2024-04-23 16:08:49.437131 llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/dropdown-menu.tsx
+-rw-r--r--   0        0        0     4085 2024-04-23 16:08:49.437131 llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/form.tsx
+-rw-r--r--   0        0        0     1198 2024-04-23 16:08:49.437131 llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/hover-card.tsx
+-rw-r--r--   0        0        0      824 2024-04-23 16:08:49.437131 llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/input.tsx
+-rw-r--r--   0        0        0      724 2024-04-23 16:08:49.437131 llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/label.tsx
+-rw-r--r--   0        0        0     7988 2024-04-23 16:08:49.437131 llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/menubar.tsx
+-rw-r--r--   0        0        0     5046 2024-04-23 16:08:49.437131 llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/navigation-menu.tsx
+-rw-r--r--   0        0        0     1244 2024-04-23 16:08:49.437131 llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/popover.tsx
+-rw-r--r--   0        0        0      791 2024-04-23 16:08:49.437131 llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/progress.tsx
+-rw-r--r--   0        0        0     1481 2024-04-23 16:08:49.437131 llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/radio-group.tsx
+-rw-r--r--   0        0        0     1656 2024-04-23 16:08:49.437131 llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/scroll-area.tsx
+-rw-r--r--   0        0        0     5629 2024-04-23 16:08:49.437131 llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/select.tsx
+-rw-r--r--   0        0        0      770 2024-04-23 16:08:49.437131 llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/separator.tsx
+-rw-r--r--   0        0        0     4302 2024-04-23 16:08:49.437131 llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/sheet.tsx
+-rw-r--r--   0        0        0      261 2024-04-23 16:08:49.437131 llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/skeleton.tsx
+-rw-r--r--   0        0        0     1091 2024-04-23 16:08:49.437131 llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/slider.tsx
+-rw-r--r--   0        0        0     1153 2024-04-23 16:08:49.437131 llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/switch.tsx
+-rw-r--r--   0        0        0     2765 2024-04-23 16:08:49.437131 llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/table.tsx
+-rw-r--r--   0        0        0     1897 2024-04-23 16:08:49.437131 llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/tabs.tsx
+-rw-r--r--   0        0        0      772 2024-04-23 16:08:49.437131 llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/textarea.tsx
+-rw-r--r--   0        0        0     4845 2024-04-23 16:08:49.437131 llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/toast.tsx
+-rw-r--r--   0        0        0      794 2024-04-23 16:08:49.437131 llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/toaster.tsx
+-rw-r--r--   0        0        0     1748 2024-04-23 16:08:49.437131 llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/toggle-group.tsx
+-rw-r--r--   0        0        0     1449 2024-04-23 16:08:49.437131 llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/toggle.tsx
+-rw-r--r--   0        0        0     1159 2024-04-23 16:08:49.437131 llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/tooltip.tsx
+-rw-r--r--   0        0        0     3934 2024-04-23 16:08:49.437131 llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/use-toast.ts
+-rw-r--r--   0        0        0     1802 2024-04-23 16:08:49.437131 llmstudio-0.3.4a2/llmstudio/ui/src/lib/utils.ts
+-rw-r--r--   0        0        0     6560 2024-04-23 16:08:49.437131 llmstudio-0.3.4a2/llmstudio/ui/tailwind.config.js
+-rw-r--r--   0        0        0      694 2024-04-23 16:08:49.437131 llmstudio-0.3.4a2/llmstudio/ui/tsconfig.json
+-rw-r--r--   0        0        0     1075 2024-04-23 16:09:04.825055 llmstudio-0.3.4a2/pyproject.toml
+-rw-r--r--   0        0        0     5550 1970-01-01 00:00:00.000000 llmstudio-0.3.4a2/PKG-INFO
```

### Comparing `llmstudio-0.3.4a1/LICENSE` & `llmstudio-0.3.4a2/LICENSE`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/README.md` & `llmstudio-0.3.4a2/README.md`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/cli.py` & `llmstudio-0.3.4a2/llmstudio/cli.py`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/config.py` & `llmstudio-0.3.4a2/llmstudio/config.py`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/engine/__init__.py` & `llmstudio-0.3.4a2/llmstudio/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/engine/config.yaml` & `llmstudio-0.3.4a2/llmstudio/engine/config.yaml`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/engine/providers/anthropic.py` & `llmstudio-0.3.4a2/llmstudio/engine/providers/anthropic.py`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/engine/providers/azure.py` & `llmstudio-0.3.4a2/llmstudio/engine/providers/azure.py`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/engine/providers/ollama.py` & `llmstudio-0.3.4a2/llmstudio/engine/providers/ollama.py`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/engine/providers/openai.py` & `llmstudio-0.3.4a2/llmstudio/engine/providers/openai.py`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/engine/providers/provider.py` & `llmstudio-0.3.4a2/llmstudio/engine/providers/provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -207,14 +207,17 @@
                 ),
                 tool_call_arguments,
             )
         elif chunks[-1].get("choices")[0].get("finish_reason") == "function_call":
             function_calls = [
                 chunk.get("choices")[0].get("delta").get("function_call")
                 for chunk in chunks[1:-1]
+                if chunk.get("choices")
+                and chunk.get("choices")[0].get("delta")
+                and chunk.get("choices")[0].get("delta").get("function_call")
             ]
 
             if isinstance(request, AzureRequest):
                 function_call_name = function_calls[0].get("name")
             elif isinstance(request, OpenAIRequest):
                 function_call_name = (
                     chunks[0]
```

### Comparing `llmstudio-0.3.4a1/llmstudio/llm/__init__.py` & `llmstudio-0.3.4a2/llmstudio/llm/__init__.py`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/llm/langchain.py` & `llmstudio-0.3.4a2/llmstudio/llm/langchain.py`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/tests/conftest.py` & `llmstudio-0.3.4a2/llmstudio/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/tests/engine/test_engine.py` & `llmstudio-0.3.4a2/llmstudio/tests/engine/test_engine.py`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/tests/engine/test_providers.py` & `llmstudio-0.3.4a2/llmstudio/tests/engine/test_providers.py`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/tracking/__init__.py` & `llmstudio-0.3.4a2/llmstudio/tracking/__init__.py`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/tracking/database.py` & `llmstudio-0.3.4a2/llmstudio/tracking/database.py`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/tracking/logs/crud.py` & `llmstudio-0.3.4a2/llmstudio/tracking/logs/crud.py`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/tracking/logs/endpoints.py` & `llmstudio-0.3.4a2/llmstudio/tracking/logs/endpoints.py`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/tracking/logs/models.py` & `llmstudio-0.3.4a2/llmstudio/tracking/logs/models.py`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/tracking/logs/schemas.py` & `llmstudio-0.3.4a2/llmstudio/tracking/logs/schemas.py`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/tracking/session/crud.py` & `llmstudio-0.3.4a2/llmstudio/tracking/session/crud.py`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/tracking/session/endpoints.py` & `llmstudio-0.3.4a2/llmstudio/tracking/session/endpoints.py`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/tracking/session/models.py` & `llmstudio-0.3.4a2/llmstudio/tracking/session/models.py`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/tracking/tracker.py` & `llmstudio-0.3.4a2/llmstudio/tracking/tracker.py`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/__init__.py` & `llmstudio-0.3.4a2/llmstudio/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/package-lock.json` & `llmstudio-0.3.4a2/llmstudio/ui/package-lock.json`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/package.json` & `llmstudio-0.3.4a2/llmstudio/ui/package.json`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/public/logo.json` & `llmstudio-0.3.4a2/llmstudio/ui/public/logo.json`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/public/svg/ai.svg` & `llmstudio-0.3.4a2/llmstudio/ui/public/svg/ai.svg`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/public/svg/compare.svg` & `llmstudio-0.3.4a2/llmstudio/ui/public/svg/compare.svg`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/public/svg/home.svg` & `llmstudio-0.3.4a2/llmstudio/ui/public/svg/home.svg`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/public/svg/magic.svg` & `llmstudio-0.3.4a2/llmstudio/ui/public/svg/magic.svg`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/public/svg/play.svg` & `llmstudio-0.3.4a2/llmstudio/ui/public/svg/play.svg`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/public/svg/playground.svg` & `llmstudio-0.3.4a2/llmstudio/ui/public/svg/playground.svg`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/public/svg/plus.svg` & `llmstudio-0.3.4a2/llmstudio/ui/public/svg/plus.svg`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/public/svg/settings.svg` & `llmstudio-0.3.4a2/llmstudio/ui/public/svg/settings.svg`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/public/svg/sparkles.svg` & `llmstudio-0.3.4a2/llmstudio/ui/public/svg/sparkles.svg`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/dashboard/hooks/useDashboardFetch.tsx` & `llmstudio-0.3.4a2/llmstudio/ui/src/app/(llm)/dashboard/hooks/useDashboardFetch.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/dashboard/page.tsx` & `llmstudio-0.3.4a2/llmstudio/ui/src/app/(llm)/dashboard/page.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/components/DataTable/ColumnHeader.tsx` & `llmstudio-0.3.4a2/llmstudio/ui/src/app/(llm)/playground/components/DataTable/ColumnHeader.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/components/DataTable/DataTable.tsx` & `llmstudio-0.3.4a2/llmstudio/ui/src/app/(llm)/playground/components/DataTable/DataTable.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/components/DataTable/FacetedFilter.tsx` & `llmstudio-0.3.4a2/llmstudio/ui/src/app/(llm)/playground/components/DataTable/FacetedFilter.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/components/DataTable/Pagination.tsx` & `llmstudio-0.3.4a2/llmstudio/ui/src/app/(llm)/playground/components/DataTable/Pagination.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/components/DataTable/RowActions.tsx` & `llmstudio-0.3.4a2/llmstudio/ui/src/app/(llm)/playground/components/DataTable/RowActions.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/components/DataTable/Toolbar.tsx` & `llmstudio-0.3.4a2/llmstudio/ui/src/app/(llm)/playground/components/DataTable/Toolbar.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/components/DataTable/UserNav.tsx` & `llmstudio-0.3.4a2/llmstudio/ui/src/app/(llm)/playground/components/DataTable/UserNav.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/components/DataTable/ViewOptions.tsx` & `llmstudio-0.3.4a2/llmstudio/ui/src/app/(llm)/playground/components/DataTable/ViewOptions.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/components/DataTable/columns.tsx` & `llmstudio-0.3.4a2/llmstudio/ui/src/app/(llm)/playground/components/DataTable/columns.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/components/Input.tsx` & `llmstudio-0.3.4a2/llmstudio/ui/src/app/(llm)/playground/components/Input.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/components/LogSheet.tsx` & `llmstudio-0.3.4a2/llmstudio/ui/src/app/(llm)/playground/components/LogSheet.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/components/ModelItem.tsx` & `llmstudio-0.3.4a2/llmstudio/ui/src/app/(llm)/playground/components/ModelItem.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/components/ModelSelector.tsx` & `llmstudio-0.3.4a2/llmstudio/ui/src/app/(llm)/playground/components/ModelSelector.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/components/Output.tsx` & `llmstudio-0.3.4a2/llmstudio/ui/src/app/(llm)/playground/components/Output.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/components/Parameters.tsx` & `llmstudio-0.3.4a2/llmstudio/ui/src/app/(llm)/playground/components/Parameters.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/hooks/useChat.tsx` & `llmstudio-0.3.4a2/llmstudio/ui/src/app/(llm)/playground/hooks/useChat.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/hooks/useExport.tsx` & `llmstudio-0.3.4a2/llmstudio/ui/src/app/(llm)/playground/hooks/useExport.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/hooks/useLogsFetch.tsx` & `llmstudio-0.3.4a2/llmstudio/ui/src/app/(llm)/playground/hooks/useLogsFetch.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/hooks/useModelFetch.tsx` & `llmstudio-0.3.4a2/llmstudio/ui/src/app/(llm)/playground/hooks/useModelFetch.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/hooks/useParameterFetch.tsx` & `llmstudio-0.3.4a2/llmstudio/ui/src/app/(llm)/playground/hooks/useParameterFetch.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/page.tsx` & `llmstudio-0.3.4a2/llmstudio/ui/src/app/(llm)/playground/page.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/store.tsx` & `llmstudio-0.3.4a2/llmstudio/ui/src/app/(llm)/playground/store.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/src/app/favicon.ico` & `llmstudio-0.3.4a2/llmstudio/ui/src/app/favicon.ico`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/src/app/globals.css` & `llmstudio-0.3.4a2/llmstudio/ui/src/app/globals.css`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/src/app/layout.tsx` & `llmstudio-0.3.4a2/llmstudio/ui/src/app/layout.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/src/components/CodeBlock/index.tsx` & `llmstudio-0.3.4a2/llmstudio/ui/src/components/CodeBlock/index.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/src/components/CopyButton/index.tsx` & `llmstudio-0.3.4a2/llmstudio/ui/src/components/CopyButton/index.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/src/components/Header/index.tsx` & `llmstudio-0.3.4a2/llmstudio/ui/src/components/Header/index.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/src/components/Markdown/index.tsx` & `llmstudio-0.3.4a2/llmstudio/ui/src/components/Markdown/index.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/src/components/Theme/index.tsx` & `llmstudio-0.3.4a2/llmstudio/ui/src/components/Theme/index.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/accordion.tsx` & `llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/accordion.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/alert-dialog.tsx` & `llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/alert-dialog.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/alert.tsx` & `llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/alert.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/avatar.tsx` & `llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/avatar.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/badge.tsx` & `llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/badge.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/button.tsx` & `llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/button.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/calendar.tsx` & `llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/calendar.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/card.tsx` & `llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/card.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/checkbox.tsx` & `llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/checkbox.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/command.tsx` & `llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/command.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/context-menu.tsx` & `llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/context-menu.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/dialog.tsx` & `llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/dialog.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/dropdown-menu.tsx` & `llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/dropdown-menu.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/form.tsx` & `llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/form.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/hover-card.tsx` & `llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/hover-card.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/input.tsx` & `llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/input.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/label.tsx` & `llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/label.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/menubar.tsx` & `llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/menubar.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/navigation-menu.tsx` & `llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/navigation-menu.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/popover.tsx` & `llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/popover.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/progress.tsx` & `llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/progress.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/radio-group.tsx` & `llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/radio-group.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/scroll-area.tsx` & `llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/scroll-area.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/select.tsx` & `llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/select.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/separator.tsx` & `llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/separator.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/sheet.tsx` & `llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/sheet.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/slider.tsx` & `llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/slider.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/switch.tsx` & `llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/switch.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/table.tsx` & `llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/table.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/tabs.tsx` & `llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/tabs.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/textarea.tsx` & `llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/textarea.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/toast.tsx` & `llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/toast.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/toaster.tsx` & `llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/toaster.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/toggle-group.tsx` & `llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/toggle-group.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/toggle.tsx` & `llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/toggle.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/tooltip.tsx` & `llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/tooltip.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/use-toast.ts` & `llmstudio-0.3.4a2/llmstudio/ui/src/components/ui/use-toast.ts`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/src/lib/utils.ts` & `llmstudio-0.3.4a2/llmstudio/ui/src/lib/utils.ts`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/tailwind.config.js` & `llmstudio-0.3.4a2/llmstudio/ui/tailwind.config.js`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/llmstudio/ui/tsconfig.json` & `llmstudio-0.3.4a2/llmstudio/ui/tsconfig.json`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a1/pyproject.toml` & `llmstudio-0.3.4a2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "llmstudio"
-version = "0.3.4a1"
+version = "0.3.4a2"
 description = "Prompt Perfection at Your Fingertips"
 authors = ["Cláudio Lemos <claudio@tensorops.ai>"]
 license = "MIT"
 homepage = "https://llmstudio.ai/"
 repository = "https://github.com/tensoropsai/llmstudio"
 documentation = "https://docs.llmstudio.ai"
 readme = "README.md"
```

### Comparing `llmstudio-0.3.4a1/PKG-INFO` & `llmstudio-0.3.4a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmstudio
-Version: 0.3.4a1
+Version: 0.3.4a2
 Summary: Prompt Perfection at Your Fingertips
 Home-page: https://llmstudio.ai/
 License: MIT
 Keywords: ml,ai,llm,llmops,openai,langchain,chatgpt,llmstudio,tensorops
 Author: Cláudio Lemos
 Author-email: claudio@tensorops.ai
 Requires-Python: >=3.9,<4.0
```

