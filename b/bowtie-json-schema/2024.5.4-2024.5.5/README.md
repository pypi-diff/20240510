# Comparing `tmp/bowtie_json_schema-2024.5.4.tar.gz` & `tmp/bowtie_json_schema-2024.5.5.tar.gz`

## Comparing `bowtie_json_schema-2024.5.4.tar` & `bowtie_json_schema-2024.5.5.tar`

### file list

```diff
@@ -1,253 +1,261 @@
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/.gitpod.Dockerfile
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/.gitpod.yml
--rw-r--r--   0        0        0     3928 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/.prettierrc.json
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/.readthedocs.yaml
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/CONTRIBUTING.rst
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/action.yml
--rw-r--r--   0        0        0    12706 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/noxfile.py
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/requirements.txt
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/test-requirements.in
--rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/test-requirements.txt
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/.devcontainer/devcontainer.json
--rwxr-xr-x   0        0        0     2229 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/.pre-commit-hooks/check-dependabot
--rwxr-xr-x   0        0        0     1267 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/.pre-commit-hooks/check-lintsonschema-schema
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/bowtie/__init__.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/bowtie/__main__.py
--rw-r--r--   0        0        0    48740 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/bowtie/_cli.py
--rw-r--r--   0        0        0    12066 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/bowtie/_commands.py
--rw-r--r--   0        0        0    10478 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/bowtie/_containers.py
--rw-r--r--   0        0        0    22876 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/bowtie/_core.py
--rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/bowtie/_registry.py
--rw-r--r--   0        0        0    11625 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/bowtie/_report.py
--rw-r--r--   0        0        0     7661 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/bowtie/_suite.py
--rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/bowtie/exceptions.py
--rw-r--r--   0        0        0     9707 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/bowtie/hypothesis.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/bowtie/py.typed
--rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/bowtie/schemas/report.json
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/bowtie/schemas/cli/info.json
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/bowtie/schemas/cli/smoke.json
--rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/bowtie/schemas/cli/summary.json
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/bowtie/schemas/io/v1.json
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/bowtie/schemas/io/commands/dialect.json
--rw-r--r--   0        0        0     3796 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/bowtie/schemas/io/commands/run.json
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/bowtie/schemas/io/commands/start.json
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/bowtie/schemas/io/commands/stop.json
--rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/bowtie/schemas/models/dialect.json
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/bowtie/schemas/models/group.json
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/bowtie/schemas/models/implementation-id.json
--rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/bowtie/schemas/models/implementation.json
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/bowtie/schemas/models/registry.json
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/bowtie/schemas/models/test.json
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/data/dialects.json
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/docs/Makefile
--rw-r--r--   0        0        0     8277 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/docs/cli.rst
--rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/docs/conf.py
--rw-r--r--   0        0        0     8235 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/docs/contributing.rst
--rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/docs/github-actions.rst
--rw-r--r--   0        0        0    36467 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/docs/implementers.rst
--rw-r--r--   0        0        0     3256 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/docs/index.rst
--rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/docs/motd.txt
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/docs/requirements.in
--rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/docs/requirements.txt
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/docs/spelling-wordlist.txt
--rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/docs/_static/bowtie_diagram_dark.svg
--rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/docs/_static/bowtie_diagram_light.svg
--rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/docs/_static/logo.svg
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/index.html
--rw-r--r--   0        0        0     2541 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/package.json
--rw-r--r--   0        0        0   163423 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/pnpm-lock.yaml
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/tsconfig.json
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/vite.config.ts
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/public/favicon.svg
--rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/DialectReportView.tsx
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/MainContainer.tsx
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/ReportDataHandler.tsx
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/global.css
--rw-r--r--   0        0        0     3366 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/index.tsx
--rw-r--r--   0        0        0     2451 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/assets/landscape-logo.svg
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/components/CopyToClipboard.tsx
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/components/FilterSection.css
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/components/FilterSection.tsx
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/components/LoadingAnimation.tsx
--rw-r--r--   0        0        0     5644 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/components/NavBar.tsx
--rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/components/OtherImplementations.tsx
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/components/BowtieInfo/BowtieInfoSection.tsx
--rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/components/Cases/CaseItem.tsx
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/components/Cases/CaseResultSvg.test.tsx
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/components/Cases/CaseResultSvg.tsx
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/components/Cases/CasesSection.tsx
--rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/components/Cases/SchemaDisplay.tsx
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/components/DragAndDrop/DragAndDrop.css
--rw-r--r--   0        0        0     4907 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/components/DragAndDrop/DragAndDrop.tsx
--rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/components/ImplementationReportView/DialectCompliance.tsx
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/components/ImplementationReportView/EmbedBadges.css
--rw-r--r--   0        0        0     6071 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/components/ImplementationReportView/EmbedBadges.tsx
--rw-r--r--   0        0        0     4815 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/components/ImplementationReportView/ImplementationReportView.tsx
--rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/components/Modals/DetailsButtonModal.tsx
--rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/components/RunInfo/RunInfoSection.tsx
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/components/Summary/ImplementationRow.css
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/components/Summary/ImplementationRow.tsx
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/components/Summary/SummarySection.tsx
--rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/components/Summary/SummaryTable.tsx
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/context/BowtieVersionContext.tsx
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/context/ThemeContext.tsx
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/data/Badge.test.ts
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/data/Badge.ts
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/data/Dialect.test.ts
--rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/data/Dialect.ts
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/data/Site.test.ts
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/data/Site.ts
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/data/mapLanguage.ts
--rw-r--r--   0        0        0     8855 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/data/parseReportData.test.ts
--rw-r--r--   0        0        0     9164 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/data/parseReportData.ts
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/frontend/src/hooks/useSearchParams.ts
--rw-r--r--   0        0        0    21214 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/.java-implementations-pmd-ruleset.xml
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/clojure-json-schema/Dockerfile
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/clojure-json-schema/project.clj
--rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/clojure-json-schema/src/bowtie_json_schema/core.clj
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/cpp-valijson/.dockerignore
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/cpp-valijson/.gitignore
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/cpp-valijson/Dockerfile
--rw-r--r--   0        0        0     5406 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/cpp-valijson/bowtie_valijson.cpp
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/cpp-valijson/compile_flags.txt
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/dotnet-jsonschema-net/.clang-format
--rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/dotnet-jsonschema-net/.gitignore
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/dotnet-jsonschema-net/Dockerfile
--rw-r--r--   0        0        0     7123 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/dotnet-jsonschema-net/Program.cs
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/dotnet-jsonschema-net/bowtie_json_everything.csproj
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/dotnet-jsonschema-net/Properties/launchSettings.json
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/go-gojsonschema/Dockerfile
--rw-r--r--   0        0        0     4681 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/go-gojsonschema/bowtie_gojsonschema.go
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/go-gojsonschema/go.mod
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/go-gojsonschema/go.sum
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/go-jsonschema/Dockerfile
--rw-r--r--   0        0        0     4958 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/go-jsonschema/bowtie_jsonschema.go
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/go-jsonschema/go.mod
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/go-jsonschema/go.sum
--rw-r--r--   0        0        0     8804 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/java-json-schema/BowtieJsonSchema.java
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/java-json-schema/Dockerfile
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/java-json-schema/build.gradle
--rw-r--r--   0        0        0     9453 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/java-json-schema-validator/BowtieJsonSchemaValidator.java
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/java-json-schema-validator/Dockerfile
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/java-json-schema-validator/build.gradle
--rw-r--r--   0        0        0     7844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/java-jsonschemafriend/BowtieJsonSchemaFriend.java
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/java-jsonschemafriend/Dockerfile
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/java-jsonschemafriend/build.gradle
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/java-openapiprocessor/.dockerignore
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/java-openapiprocessor/.editorconfig
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/java-openapiprocessor/Dockerfile
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/java-openapiprocessor/build.gradle.kts
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/java-openapiprocessor/gradle.properties
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/java-openapiprocessor/justfile
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/java-openapiprocessor/settings.gradle.kts
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/java-openapiprocessor/gradle/libs.versions.toml
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/java-openapiprocessor/src/main/kotlin/Main.kt
--rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/java-openapiprocessor/src/main/kotlin/Runner.kt
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/java-openapiprocessor/src/main/kotlin/Support.kt
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/java-openapiprocessor/src/main/kotlin/commands/Configuration.kt
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/java-openapiprocessor/src/main/kotlin/commands/Dialect.kt
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/java-openapiprocessor/src/main/kotlin/commands/Request.kt
--rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/java-openapiprocessor/src/main/kotlin/commands/RunCmd.kt
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/java-openapiprocessor/src/main/kotlin/commands/StartCmd.kt
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/java-openapiprocessor/src/main/kotlin/commands/StopCmd.kt
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/js-ajv/Dockerfile
--rw-r--r--   0        0        0     2990 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/js-ajv/bowtie_ajv.js
--rw-r--r--   0        0        0     4870 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/js-ajv/package-lock.json
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/js-ajv/package.json
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/js-hyperjump/Dockerfile
--rw-r--r--   0        0        0     5711 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/js-hyperjump/bowtie_hyperjump.js
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/js-hyperjump/package.json
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/js-json-schema/Dockerfile
--rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/js-json-schema/bowtie_json_schema.js
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/js-json-schema/package.json
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/js-jsonschema/Dockerfile
--rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/js-jsonschema/bowtie_jsonschema.js
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/js-jsonschema/package.json
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/kotlin-kmp-json-schema-validator/.gitignore
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/kotlin-kmp-json-schema-validator/Dockerfile
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/kotlin-kmp-json-schema-validator/build.gradle.kts
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/kotlin-kmp-json-schema-validator/settings.gradle.kts
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/kotlin-kmp-json-schema-validator/gradle/libs.versions.toml
--rw-r--r--   0        0        0     7879 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/BowtieSampsonSchemaValidatorLauncher.kt
--rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Commands.kt
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Responses.kt
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/TestFilters.kt
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/lua-jsonschema/Dockerfile
--rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/lua-jsonschema/bowtie_jsonschema.lua
--rw-r--r--   0        0        0     9638 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/lua-jsonschema/json.lua
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/lua-jsonschema/stylua.toml
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/php-opis-json-schema/Dockerfile
--rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/php-opis-json-schema/bowtieJsonSchema.php
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/php-opis-json-schema/composer.json
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/python-fastjsonschema/Dockerfile
--rwxr-xr-x   0        0        0     2980 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/python-fastjsonschema/bowtie_fastjsonschema.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/python-jschon/Dockerfile
--rwxr-xr-x   0        0        0     3844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/python-jschon/bowtie_jschon.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/python-jsonschema/Dockerfile
--rwxr-xr-x   0        0        0     3409 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/python-jsonschema/bowtie_jsonschema.py
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/ruby-json_schemer/.rubocop.yml
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/ruby-json_schemer/Dockerfile
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/ruby-json_schemer/Gemfile
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/ruby-json_schemer/Gemfile.lock
--rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/ruby-json_schemer/bowtie_json_schemer.rb
--rw-r--r--   0        0        0    13200 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/rust-boon/Cargo.lock
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/rust-boon/Cargo.toml
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/rust-boon/Dockerfile
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/rust-boon/build.rs
--rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/rust-boon/src/main.rs
--rw-r--r--   0        0        0    39774 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/rust-jsonschema/Cargo.lock
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/rust-jsonschema/Cargo.toml
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/rust-jsonschema/Dockerfile
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/rust-jsonschema/build.rs
--rw-r--r--   0        0        0     5169 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/rust-jsonschema/src/main.rs
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/scala-mjs-validator/Dockerfile
--rw-r--r--   0        0        0     6835 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/scala-mjs-validator/Harness.scala
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/scala-mjs-validator/build.sbt
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/scala-mjs-validator/project/build.properties
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/scala-mjs-validator/project/plugins.sbt
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/scala-rc-circe-json-validator/Dockerfile
--rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/scala-rc-circe-json-validator/Harness.scala
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/scala-rc-circe-json-validator/build.sbt
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/scala-rc-circe-json-validator/project/build.properties
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/scala-rc-circe-json-validator/project/plugins.sbt
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/ts-vscode-json-languageservice/Dockerfile
--rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/ts-vscode-json-languageservice/bowtie_jsonls.ts
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/ts-vscode-json-languageservice/package.json
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/implementations/ts-vscode-json-languageservice/tsconfig.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/tests/__init__.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/tests/conftest.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/tests/test_cli.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/tests/test_dialect.py
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/tests/test_github.py
--rw-r--r--   0        0        0     3914 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/tests/test_hypothesis.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/tests/test_implementation.py
--rw-r--r--   0        0        0    64845 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/tests/test_integration.py
--rw-r--r--   0        0        0    10149 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/tests/test_report.py
--rw-r--r--   0        0        0     4005 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/tests/test_schemas.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/tests/fauxmplementations/envsonschema/Dockerfile
--rwxr-xr-x   0        0        0     6837 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/tests/fauxmplementations/envsonschema/envsonschema
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/tests/fauxmplementations/lintsonschema/Dockerfile
--rwxr-xr-x   0        0        0     3357 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/tests/fauxmplementations/lintsonschema/lintsonschema
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/tests/fauxmplementations/lintsonschema/schemas/.gitattributes
--rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/tests/fauxmplementations/lintsonschema/schemas/report.json
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/tests/fauxmplementations/lintsonschema/schemas/cli/info.json
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/tests/fauxmplementations/lintsonschema/schemas/cli/smoke.json
--rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/tests/fauxmplementations/lintsonschema/schemas/cli/summary.json
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/tests/fauxmplementations/lintsonschema/schemas/io/v1.json
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/tests/fauxmplementations/lintsonschema/schemas/io/commands/dialect.json
--rw-r--r--   0        0        0     3796 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/tests/fauxmplementations/lintsonschema/schemas/io/commands/run.json
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/tests/fauxmplementations/lintsonschema/schemas/io/commands/start.json
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/tests/fauxmplementations/lintsonschema/schemas/io/commands/stop.json
--rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/tests/fauxmplementations/lintsonschema/schemas/models/dialect.json
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/tests/fauxmplementations/lintsonschema/schemas/models/group.json
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/tests/fauxmplementations/lintsonschema/schemas/models/implementation-id.json
--rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/tests/fauxmplementations/lintsonschema/schemas/models/implementation.json
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/tests/fauxmplementations/lintsonschema/schemas/models/registry.json
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/tests/fauxmplementations/lintsonschema/schemas/models/test.json
--rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/.gitignore
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/LICENSE
--rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/README.rst
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/hatch_build.py
--rw-r--r--   0        0        0     5379 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/pyproject.toml
--rw-r--r--   0        0        0     3652 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.4/PKG-INFO
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/.gitpod.Dockerfile
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/.gitpod.yml
+-rw-r--r--   0        0        0     3928 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/.prettierrc.json
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/.readthedocs.yaml
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/CONTRIBUTING.rst
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/action.yml
+-rw-r--r--   0        0        0    12706 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/noxfile.py
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/requirements.txt
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/test-requirements.in
+-rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/test-requirements.txt
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/.devcontainer/devcontainer.json
+-rwxr-xr-x   0        0        0     2229 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/.pre-commit-hooks/check-dependabot
+-rwxr-xr-x   0        0        0     1267 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/.pre-commit-hooks/check-lintsonschema-schema
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/bowtie/__init__.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/bowtie/__main__.py
+-rw-r--r--   0        0        0    48283 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/bowtie/_cli.py
+-rw-r--r--   0        0        0    12066 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/bowtie/_commands.py
+-rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/bowtie/_connectables.py
+-rw-r--r--   0        0        0    11145 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/bowtie/_containers.py
+-rw-r--r--   0        0        0    22876 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/bowtie/_core.py
+-rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/bowtie/_registry.py
+-rw-r--r--   0        0        0    11625 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/bowtie/_report.py
+-rw-r--r--   0        0        0     7661 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/bowtie/_suite.py
+-rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/bowtie/exceptions.py
+-rw-r--r--   0        0        0     9707 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/bowtie/hypothesis.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/bowtie/py.typed
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/bowtie/schemas/connectables.json
+-rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/bowtie/schemas/report.json
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/bowtie/schemas/cli/info.json
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/bowtie/schemas/cli/smoke.json
+-rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/bowtie/schemas/cli/summary.json
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/bowtie/schemas/io/v1.json
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/bowtie/schemas/io/commands/dialect.json
+-rw-r--r--   0        0        0     3796 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/bowtie/schemas/io/commands/run.json
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/bowtie/schemas/io/commands/start.json
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/bowtie/schemas/io/commands/stop.json
+-rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/bowtie/schemas/models/dialect.json
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/bowtie/schemas/models/group.json
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/bowtie/schemas/models/implementation-id.json
+-rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/bowtie/schemas/models/implementation.json
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/bowtie/schemas/models/registry.json
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/bowtie/schemas/models/test.json
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/data/dialects.json
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/docs/Makefile
+-rw-r--r--   0        0        0     8253 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/docs/cli.rst
+-rw-r--r--   0        0        0     4100 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/docs/conf.py
+-rw-r--r--   0        0        0     8235 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/docs/contributing.rst
+-rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/docs/github-actions.rst
+-rw-r--r--   0        0        0    36467 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/docs/implementers.rst
+-rw-r--r--   0        0        0     3256 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/docs/index.rst
+-rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/docs/motd.txt
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/docs/requirements.in
+-rw-r--r--   0        0        0     3713 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/docs/requirements.txt
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/docs/spelling-wordlist.txt
+-rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/docs/_static/bowtie_diagram_dark.svg
+-rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/docs/_static/bowtie_diagram_light.svg
+-rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/docs/_static/logo.svg
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/index.html
+-rw-r--r--   0        0        0     2541 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/package.json
+-rw-r--r--   0        0        0   163423 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/pnpm-lock.yaml
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/tsconfig.json
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/vite.config.ts
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/public/favicon.svg
+-rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/DialectReportView.tsx
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/MainContainer.tsx
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/ReportDataHandler.tsx
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/global.css
+-rw-r--r--   0        0        0     3366 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/index.tsx
+-rw-r--r--   0        0        0     2451 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/assets/landscape-logo.svg
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/components/CopyToClipboard.tsx
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/components/FilterSection.css
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/components/FilterSection.tsx
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/components/LoadingAnimation.tsx
+-rw-r--r--   0        0        0     5644 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/components/NavBar.tsx
+-rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/components/OtherImplementations.tsx
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/components/BowtieInfo/BowtieInfoSection.tsx
+-rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/components/Cases/CaseItem.tsx
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/components/Cases/CaseResultSvg.test.tsx
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/components/Cases/CaseResultSvg.tsx
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/components/Cases/CasesSection.tsx
+-rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/components/Cases/SchemaDisplay.tsx
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/components/DragAndDrop/DragAndDrop.css
+-rw-r--r--   0        0        0     4907 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/components/DragAndDrop/DragAndDrop.tsx
+-rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/components/ImplementationReportView/DialectCompliance.tsx
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/components/ImplementationReportView/EmbedBadges.css
+-rw-r--r--   0        0        0     6071 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/components/ImplementationReportView/EmbedBadges.tsx
+-rw-r--r--   0        0        0     4815 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/components/ImplementationReportView/ImplementationReportView.tsx
+-rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/components/Modals/DetailsButtonModal.tsx
+-rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/components/RunInfo/RunInfoSection.tsx
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/components/Summary/ImplementationRow.css
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/components/Summary/ImplementationRow.tsx
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/components/Summary/SummarySection.tsx
+-rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/components/Summary/SummaryTable.tsx
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/context/BowtieVersionContext.tsx
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/context/ThemeContext.tsx
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/data/Badge.test.ts
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/data/Badge.ts
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/data/Dialect.test.ts
+-rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/data/Dialect.ts
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/data/Site.test.ts
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/data/Site.ts
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/data/mapLanguage.ts
+-rw-r--r--   0        0        0     8855 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/data/parseReportData.test.ts
+-rw-r--r--   0        0        0     9164 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/data/parseReportData.ts
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/hooks/useSearchParams.ts
+-rw-r--r--   0        0        0    21214 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/.java-implementations-pmd-ruleset.xml
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/clojure-json-schema/Dockerfile
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/clojure-json-schema/project.clj
+-rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/clojure-json-schema/src/bowtie_json_schema/core.clj
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/cpp-valijson/.dockerignore
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/cpp-valijson/.gitignore
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/cpp-valijson/Dockerfile
+-rw-r--r--   0        0        0     5406 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/cpp-valijson/bowtie_valijson.cpp
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/cpp-valijson/compile_flags.txt
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/dotnet-jsonschema-net/.clang-format
+-rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/dotnet-jsonschema-net/.gitignore
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/dotnet-jsonschema-net/Dockerfile
+-rw-r--r--   0        0        0     7121 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/dotnet-jsonschema-net/Program.cs
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/dotnet-jsonschema-net/bowtie_json_everything.csproj
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/dotnet-jsonschema-net/Properties/launchSettings.json
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/go-gojsonschema/Dockerfile
+-rw-r--r--   0        0        0     4681 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/go-gojsonschema/bowtie_gojsonschema.go
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/go-gojsonschema/go.mod
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/go-gojsonschema/go.sum
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/go-jsonschema/Dockerfile
+-rw-r--r--   0        0        0     4958 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/go-jsonschema/bowtie_jsonschema.go
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/go-jsonschema/go.mod
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/go-jsonschema/go.sum
+-rw-r--r--   0        0        0     8804 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/java-json-schema/BowtieJsonSchema.java
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/java-json-schema/Dockerfile
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/java-json-schema/build.gradle
+-rw-r--r--   0        0        0     7843 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/java-json-tools-json-schema-validator/BowtieJsonSchemaValidator.java
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/java-json-tools-json-schema-validator/Dockerfile
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/java-json-tools-json-schema-validator/build.gradle
+-rw-r--r--   0        0        0     7844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/java-jsonschemafriend/BowtieJsonSchemaFriend.java
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/java-jsonschemafriend/Dockerfile
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/java-jsonschemafriend/build.gradle
+-rw-r--r--   0        0        0     9453 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/java-networknt-json-schema-validator/BowtieJsonSchemaValidator.java
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/java-networknt-json-schema-validator/Dockerfile
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/java-networknt-json-schema-validator/build.gradle
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/java-openapiprocessor/.dockerignore
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/java-openapiprocessor/.editorconfig
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/java-openapiprocessor/Dockerfile
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/java-openapiprocessor/build.gradle.kts
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/java-openapiprocessor/gradle.properties
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/java-openapiprocessor/justfile
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/java-openapiprocessor/settings.gradle.kts
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/java-openapiprocessor/gradle/libs.versions.toml
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/java-openapiprocessor/src/main/kotlin/Main.kt
+-rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/java-openapiprocessor/src/main/kotlin/Runner.kt
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/java-openapiprocessor/src/main/kotlin/Support.kt
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/java-openapiprocessor/src/main/kotlin/commands/Configuration.kt
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/java-openapiprocessor/src/main/kotlin/commands/Dialect.kt
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/java-openapiprocessor/src/main/kotlin/commands/Request.kt
+-rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/java-openapiprocessor/src/main/kotlin/commands/RunCmd.kt
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/java-openapiprocessor/src/main/kotlin/commands/StartCmd.kt
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/java-openapiprocessor/src/main/kotlin/commands/StopCmd.kt
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/js-ajv/Dockerfile
+-rw-r--r--   0        0        0     2990 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/js-ajv/bowtie_ajv.js
+-rw-r--r--   0        0        0     4870 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/js-ajv/package-lock.json
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/js-ajv/package.json
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/js-hyperjump/Dockerfile
+-rw-r--r--   0        0        0     5711 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/js-hyperjump/bowtie_hyperjump.js
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/js-hyperjump/package.json
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/js-json-schema/Dockerfile
+-rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/js-json-schema/bowtie_json_schema.js
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/js-json-schema/package.json
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/js-jsonschema/Dockerfile
+-rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/js-jsonschema/bowtie_jsonschema.js
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/js-jsonschema/package.json
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/kotlin-kmp-json-schema-validator/.gitignore
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/kotlin-kmp-json-schema-validator/Dockerfile
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/kotlin-kmp-json-schema-validator/build.gradle.kts
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/kotlin-kmp-json-schema-validator/settings.gradle.kts
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/kotlin-kmp-json-schema-validator/gradle/libs.versions.toml
+-rw-r--r--   0        0        0     7879 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/BowtieSampsonSchemaValidatorLauncher.kt
+-rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Commands.kt
+-rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Responses.kt
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/TestFilters.kt
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/lua-jsonschema/Dockerfile
+-rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/lua-jsonschema/bowtie_jsonschema.lua
+-rw-r--r--   0        0        0     9638 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/lua-jsonschema/json.lua
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/lua-jsonschema/stylua.toml
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/php-opis-json-schema/Dockerfile
+-rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/php-opis-json-schema/bowtieJsonSchema.php
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/php-opis-json-schema/composer.json
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/python-fastjsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     2980 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/python-fastjsonschema/bowtie_fastjsonschema.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/python-jschon/Dockerfile
+-rwxr-xr-x   0        0        0     3844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/python-jschon/bowtie_jschon.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/python-jsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     3409 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/python-jsonschema/bowtie_jsonschema.py
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/ruby-json_schemer/.rubocop.yml
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/ruby-json_schemer/Dockerfile
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/ruby-json_schemer/Gemfile
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/ruby-json_schemer/Gemfile.lock
+-rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/ruby-json_schemer/bowtie_json_schemer.rb
+-rw-r--r--   0        0        0    13200 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/rust-boon/Cargo.lock
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/rust-boon/Cargo.toml
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/rust-boon/Dockerfile
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/rust-boon/build.rs
+-rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/rust-boon/src/main.rs
+-rw-r--r--   0        0        0    38883 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/rust-jsonschema/Cargo.lock
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/rust-jsonschema/Cargo.toml
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/rust-jsonschema/Dockerfile
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/rust-jsonschema/build.rs
+-rw-r--r--   0        0        0     5169 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/rust-jsonschema/src/main.rs
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/scala-mjs-validator/Dockerfile
+-rw-r--r--   0        0        0     6835 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/scala-mjs-validator/Harness.scala
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/scala-mjs-validator/build.sbt
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/scala-mjs-validator/project/build.properties
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/scala-mjs-validator/project/plugins.sbt
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/scala-rc-circe-json-validator/Dockerfile
+-rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/scala-rc-circe-json-validator/Harness.scala
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/scala-rc-circe-json-validator/build.sbt
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/scala-rc-circe-json-validator/project/build.properties
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/scala-rc-circe-json-validator/project/plugins.sbt
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/ts-vscode-json-languageservice/Dockerfile
+-rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/ts-vscode-json-languageservice/bowtie_jsonls.ts
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/ts-vscode-json-languageservice/package.json
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/ts-vscode-json-languageservice/tsconfig.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/tests/__init__.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/tests/conftest.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/tests/test_cli.py
+-rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/tests/test_connectables.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/tests/test_dialect.py
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/tests/test_github.py
+-rw-r--r--   0        0        0     3914 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/tests/test_hypothesis.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/tests/test_implementation.py
+-rw-r--r--   0        0        0    65160 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/tests/test_integration.py
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/tests/test_registry.py
+-rw-r--r--   0        0        0    10149 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/tests/test_report.py
+-rw-r--r--   0        0        0     4005 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/tests/test_schemas.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/tests/fauxmplementations/envsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     6837 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/tests/fauxmplementations/envsonschema/envsonschema
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/tests/fauxmplementations/lintsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     3357 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/tests/fauxmplementations/lintsonschema/lintsonschema
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/tests/fauxmplementations/lintsonschema/schemas/.gitattributes
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/tests/fauxmplementations/lintsonschema/schemas/connectables.json
+-rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/tests/fauxmplementations/lintsonschema/schemas/report.json
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/tests/fauxmplementations/lintsonschema/schemas/cli/info.json
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/tests/fauxmplementations/lintsonschema/schemas/cli/smoke.json
+-rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/tests/fauxmplementations/lintsonschema/schemas/cli/summary.json
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/tests/fauxmplementations/lintsonschema/schemas/io/v1.json
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/tests/fauxmplementations/lintsonschema/schemas/io/commands/dialect.json
+-rw-r--r--   0        0        0     3796 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/tests/fauxmplementations/lintsonschema/schemas/io/commands/run.json
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/tests/fauxmplementations/lintsonschema/schemas/io/commands/start.json
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/tests/fauxmplementations/lintsonschema/schemas/io/commands/stop.json
+-rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/tests/fauxmplementations/lintsonschema/schemas/models/dialect.json
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/tests/fauxmplementations/lintsonschema/schemas/models/group.json
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/tests/fauxmplementations/lintsonschema/schemas/models/implementation-id.json
+-rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/tests/fauxmplementations/lintsonschema/schemas/models/implementation.json
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/tests/fauxmplementations/lintsonschema/schemas/models/registry.json
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/tests/fauxmplementations/lintsonschema/schemas/models/test.json
+-rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/.gitignore
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/LICENSE
+-rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/README.rst
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/hatch_build.py
+-rw-r--r--   0        0        0     5379 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/pyproject.toml
+-rw-r--r--   0        0        0     3652 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/PKG-INFO
```

### Comparing `bowtie_json_schema-2024.5.4/.gitpod.yml` & `bowtie_json_schema-2024.5.5/.gitpod.yml`

 * *Files 13% similar despite different names*

```diff
@@ -11,11 +11,11 @@
   - name: Populate MOTD with documentation
     init: sudo chown -R gitpod:gitpod /etc/motd && cp /workspace/bowtie/docs/motd.txt /etc/motd
 
   - name: Install Bowtie
     init: python3 -m pip install -r requirements.txt -e . && pyenv rehash
 
   - name: Pull Bowtie Images
-    init: for each in $(ls implementations); do docker pull ghcr.io/bowtie-json-schema/$each; done
+    init: for each in $(bowtie filter-implementations); do docker pull ghcr.io/bowtie-json-schema/$each; done
 
   - name: Open Bowtie Documentation by default in web-ui
     init: gp open /workspace/bowtie/docs/motd.txt
```

### Comparing `bowtie_json_schema-2024.5.4/.pre-commit-config.yaml` & `bowtie_json_schema-2024.5.5/.pre-commit-config.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
       - id: check-yaml
       - id: debug-statements
       - id: end-of-file-fixer
       - id: mixed-line-ending
         args: [--fix, lf]
       - id: trailing-whitespace
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: "v0.4.2"
+    rev: "v0.4.3"
     hooks:
       - id: ruff
         args: [--fix, --exit-non-zero-on-fix]
   - repo: https://github.com/python-jsonschema/check-jsonschema
     rev: 0.28.2
     hooks:
       - name: ensure bowtie's own schemas are valid
```

### Comparing `bowtie_json_schema-2024.5.4/CONTRIBUTING.rst` & `bowtie_json_schema-2024.5.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/action.yml` & `bowtie_json_schema-2024.5.5/action.yml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/noxfile.py` & `bowtie_json_schema-2024.5.5/noxfile.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/requirements.txt` & `bowtie_json_schema-2024.5.5/requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     # via requests
 cffi==1.16.0
     # via cryptography
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via rich-click
-cryptography==42.0.5
+cryptography==42.0.7
     # via pyjwt
 diagnostic==2.1.0
 docutils==0.21.2
     # via diagnostic
 frozenlist==1.4.1
     # via
     #   aiohttp
@@ -44,36 +44,36 @@
     # via markdown-it-py
 multidict==6.0.5
     # via
     #   aiohttp
     #   yarl
 pycparser==2.22
     # via cffi
-pygments==2.17.2
+pygments==2.18.0
     # via
     #   jsonschema-lexer
     #   rich
 pyjwt==2.8.0
     # via github3-py
 python-dateutil==2.9.0.post0
     # via github3-py
-referencing==0.35.0
+referencing==0.35.1
     # via
     #   jsonschema
     #   jsonschema-specifications
     #   referencing-loaders
 referencing-loaders==2024.5.2
 requests==2.31.0
     # via github3-py
 rich==13.7.1
     # via
     #   diagnostic
     #   rich-click
 rich-click==1.8.0
-rpds-py==0.18.0
+rpds-py==0.18.1
     # via
     #   jsonschema
     #   referencing
 six==1.16.0
     # via python-dateutil
 structlog==24.1.0
 typing-extensions==4.11.0
```

### Comparing `bowtie_json_schema-2024.5.4/test-requirements.txt` & `bowtie_json_schema-2024.5.5/test-requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -18,27 +18,27 @@
     # via requests
 cffi==1.16.0
     # via cryptography
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via rich-click
-cryptography==42.0.5
+cryptography==42.0.7
     # via pyjwt
 diagnostic==2.1.0
     # via bowtie-json-schema
 docutils==0.21.2
     # via diagnostic
 frozenlist==1.4.1
     # via
     #   aiohttp
     #   aiosignal
 github3-py==4.0.1
     # via bowtie-json-schema
-hypothesis==6.100.2
+hypothesis==6.100.5
 icdiff==2.0.7
     # via pytest-icdiff
 idna==3.7
     # via
     #   requests
     #   yarl
 iniconfig==2.0.0
@@ -66,29 +66,29 @@
     # via pytest
 pprintpp==0.4.0
     # via pytest-icdiff
 ptyprocess==0.7.0
     # via pexpect
 pycparser==2.22
     # via cffi
-pygments==2.17.2
+pygments==2.18.0
     # via
     #   jsonschema-lexer
     #   rich
 pyjwt==2.8.0
     # via github3-py
 pytest==8.2.0
     # via
     #   pytest-asyncio
     #   pytest-icdiff
 pytest-asyncio==0.21.2
 pytest-icdiff==0.9
 python-dateutil==2.9.0.post0
     # via github3-py
-referencing==0.35.0
+referencing==0.35.1
     # via
     #   bowtie-json-schema
     #   jsonschema
     #   jsonschema-specifications
     #   referencing-loaders
 referencing-loaders==2024.5.2
     # via bowtie-json-schema
@@ -97,15 +97,15 @@
 rich==13.7.1
     # via
     #   bowtie-json-schema
     #   diagnostic
     #   rich-click
 rich-click==1.8.0
     # via bowtie-json-schema
-rpds-py==0.18.0
+rpds-py==0.18.1
     # via
     #   bowtie-json-schema
     #   jsonschema
     #   referencing
 six==1.16.0
     # via python-dateutil
 sortedcontainers==2.4.0
```

### Comparing `bowtie_json_schema-2024.5.4/.pre-commit-hooks/check-dependabot` & `bowtie_json_schema-2024.5.5/.pre-commit-hooks/check-dependabot`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/.pre-commit-hooks/check-lintsonschema-schema` & `bowtie_json_schema-2024.5.5/.pre-commit-hooks/check-lintsonschema-schema`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/bowtie/_cli.py` & `bowtie_json_schema-2024.5.5/bowtie/_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from typing import TYPE_CHECKING, Literal, ParamSpec, Protocol
 import asyncio
 import json
 import logging
 import os
 import sys
 
-from aiodocker import Docker
 from attrs import asdict
 from click.shell_completion import CompletionItem
 from diagnostic import DiagnosticError
 from jsonschema_lexer import JSONSchemaLexer
 from pygments.lexers.data import (  # type: ignore[reportMissingTypeStubs]
     JsonLexer,
 )
@@ -28,15 +27,15 @@
 from rich.text import Text
 from rich_click.utils import CommandGroupDict, OptionGroupDict
 from url import URL, RelativeURLWithoutBase
 import rich_click as click
 import structlog
 import structlog.typing
 
-from bowtie import _containers, _report, _suite
+from bowtie import _connectables, _report, _suite
 from bowtie._commands import SeqCase, Unsuccessful
 from bowtie._core import (
     Dialect,
     Example,
     Implementation,
     NoSuchImplementation,
     StartupFailed,
@@ -60,23 +59,22 @@
     from click.decorators import FC
     from referencing.jsonschema import Schema, SchemaResource
 
     from bowtie._commands import AnyTestResult, ImplementationId
     from bowtie._core import DialectRunner, ImplementationInfo, MakeValidator
 
 
-# Windows fallbacks...
-_EX_CONFIG = getattr(os, "EX_CONFIG", 1)
-_EX_DATAERR = getattr(os, "EX_DATAERR", 1)
-_EX_NOINPUT = getattr(os, "EX_NOINPUT", 1)
+class _EX:
+    def __getattr__(self, attr: str) -> int:
+        return getattr(os, f"EX_{attr}", 1)  # Windows fallbacks...
 
-STDERR = console.Console(stderr=True)
 
+EX = _EX()
 
-IMAGE_REPOSITORY = "ghcr.io/bowtie-json-schema"
+STDERR = console.Console(stderr=True)
 
 
 # rich-click's CommandGroupDict seems to be missing some covariance, as using a
 # regular dict here makes pyright complain.
 _COMMAND_GROUPS = dict(
     bowtie=[
         CommandGroupDict(
@@ -225,15 +223,18 @@
 
     return run
 
 
 class ImplementationSubcommand(Protocol):
     def __call__(
         self,
-        start: Callable[[], AsyncIterator[Implementation]],
+        start: Callable[
+            [],
+            AsyncIterator[tuple[ImplementationId, Implementation]],
+        ],
         **kwargs: Any,
     ) -> Awaitable[int | None]: ...
 
 
 SILENT = _report.Reporter(write=lambda **_: None)  # type: ignore[reportUnknownArgumentType])
 
 
@@ -246,69 +247,79 @@
 
     Runs the wrapped function with only the successfully started
     implementations.
     """
 
     def wrapper(fn: ImplementationSubcommand):
         async def run(
-            image_names: Iterable[str],
+            connectables: Iterable[_connectables.Connectable],
             read_timeout_sec: float,
             make_validator: MakeValidator = make_validator,
             **kw: Any,
         ) -> int:
             exit_code = 0
 
             async def start():
                 nonlocal exit_code
 
                 successful = 0
                 async with _start(
-                    image_names=image_names,
+                    connectables=connectables,
                     make_validator=make_validator,
                     reporter=reporter,
                     read_timeout_sec=read_timeout_sec,
                 ) as implementations:
                     for each in implementations:  # FIXME: respect --quiet
                         try:
-                            implementation = await each
+                            connectable_implementation = await each
                         except (NoSuchImplementation, StartupFailed) as error:
-                            exit_code |= _EX_CONFIG
+                            exit_code |= EX.CONFIG
                             STDERR.print(error)
                             continue
 
                         successful += 1
-                        yield implementation
+                        yield connectable_implementation
 
                     if not successful and default_implementations:
                         # TODO: show a diagnostic that collects crash causes
-                        exit_code |= _EX_CONFIG
+                        exit_code |= EX.CONFIG
                         return
 
+            # FIXME: Convert this to an instance presumably, but for now we
+            #        just want this data available in the functions,
+            #        and introducing another type is annoying when most of the
+            #        complexity has to do with _run / _start still existing --
+            #        we need to finish removing them.
+            start.connectables = [each.to_terse() for each in connectables]  # type: ignore[reportFunctionMemberAccess]
+
             fn_exit_code = await fn(start=start, **kw)
             return exit_code | (fn_exit_code or 0)
 
         @subcommand
         @click.option(
             "--implementation",
             "-i",
-            "image_names",
-            type=_Image(),
+            "connectables",
+            type=_connectables.ClickParam(),
             default=lambda: (
                 default_implementations
                 if sys.stdin.isatty()
                 else [line.strip() for line in sys.stdin]
             ),
             multiple=True,
             metavar="IMPLEMENTATION",
             help="A container image which implements the bowtie IO protocol.",
         )
         @TIMEOUT
         @wraps(fn)
-        def cmd(image_names: Iterable[str], **kwargs: Any) -> int:
-            return asyncio.run(run(image_names=image_names, **kwargs))
+        def cmd(
+            connectables: Iterable[_connectables.Connectable],
+            **kwargs: Any,
+        ) -> int:
+            return asyncio.run(run(connectables=connectables, **kwargs))
 
         return cmd
 
     return wrapper
 
 
 @subcommand
@@ -344,15 +355,15 @@
             causes=[f"{outdir} is an existing directory."],
             hint_stmt=(
                 "If you intended to replace its contents with new badges, "
                 "delete the directory first."
             ),
         )
         STDERR.print(error)
-        return _EX_CONFIG
+        return EX.CONFIG
 
     supported_versions: dict[Path, Iterable[Dialect]] = {}
 
     for name, dialect in Dialect.by_short_name().items():
         try:
             file = site.joinpath(f"{name}.json").open()
         except FileNotFoundError:
@@ -363,15 +374,15 @@
                 error = DiagnosticError(
                     code="empty-report",
                     message="A Bowtie report is empty.",
                     causes=[f"The {name} report contains no results."],
                     hint_stmt="Check that site generation has not failed.",
                 )
                 STDERR.print(error)
-                return _EX_DATAERR
+                return EX.DATAERR
 
             badge_name = f"{dialect.short_name}.json"
 
             for each, badge in report.compliance_badges():
                 dir = outdir / f"{each.language}-{each.name}"
 
                 compliance = dir / "compliance"
@@ -394,15 +405,15 @@
                         ],
                         hint_stmt=(
                             "Check that the implementation produces "
                             "consistent output and that a run has not failed."
                         ),
                     )
                     STDERR.print(error)
-                    return _EX_CONFIG
+                    return EX.CONFIG
 
     for dir, dialects in supported_versions.items():
         badge = _report.supported_version_badge(dialects=dialects)
         dir.joinpath("supported_versions.json").write_text(json.dumps(badge))
 
 
 _F = Literal["json", "pretty", "markdown"]
@@ -478,44 +489,44 @@
             hint_stmt=(
                 "If you are piping data into bowtie summary, "
                 "check to ensure that what you've run has succeeded, "
                 "otherwise it may be emitting no report data."
             ),
         )
         STDERR.print(error)
-        return _EX_NOINPUT
+        return EX.NOINPUT
     except json.JSONDecodeError as err:
         error = DiagnosticError(
             code="report-not-json",
             message="The Bowtie report looks corrupt.",
             causes=[f"{input.name} is not valid JSON.", str(err)],
             hint_stmt=(
                 "If you are piping data, the command producing the report "
                 "has likely failed and the real error is above this one. "
                 "Otherwise, ensure you are passing in a report generated by "
                 "Bowtie."
             ),
         )
         STDERR.print(error)
-        return _EX_DATAERR
+        return EX.DATAERR
     except _report.MissingFooter:
         error = DiagnosticError(
             code="truncated-report",
             message="The Bowtie report looks corrupt.",
             causes=[
                 f"{input.name} is missing its footer, which usually means "
                 "it has been somehow truncated.",
             ],
             hint_stmt=(
                 "Try running the command you used to produce the report, "
                 "without piping it. If it crashes, file a bug report!"
             ),
         )
         STDERR.print(error)
-        return _EX_DATAERR
+        return EX.DATAERR
 
     if show == "failures":
         results = report.worst_to_best()
         to_table = _failure_table
         to_markdown_table = _failure_table_in_markdown
 
         def to_serializable(  # type: ignore[reportRedeclaration]
@@ -755,44 +766,14 @@
     return validate
 
 
 def do_not_validate(*ignored: SchemaResource) -> Callable[..., None]:
     return lambda *args, **kwargs: None
 
 
-class _Image(click.ParamType):
-    """
-    Select a supported Bowtie implementation.
-    """
-
-    name = "implementation"
-
-    def convert(
-        self,
-        value: str,
-        param: click.Parameter | None,
-        ctx: click.Context | None,
-    ) -> str:
-        if "/" in value:  # a fully qualified image name
-            return value
-        return f"{IMAGE_REPOSITORY}/{value}"
-
-    def shell_complete(
-        self,
-        ctx: click.Context,
-        param: click.Parameter,
-        incomplete: str,
-    ) -> list[CompletionItem]:
-        return [
-            CompletionItem(name)
-            for name in Implementation.known()
-            if name.startswith(incomplete.lower())
-        ]
-
-
 class _Dialect(click.ParamType):
     """
     Select a JSON Schema dialect.
     """
 
     name = "dialect"
 
@@ -901,16 +882,16 @@
 def _do_nothing(*args: Any, **kwargs: Any) -> CaseTransform:
     return lambda cases: cases
 
 
 IMPLEMENTATION = click.option(
     "--implementation",
     "-i",
-    "image_names",
-    type=_Image(),
+    "connectables",
+    type=_connectables.ClickParam(),
     required=True,
     multiple=True,
     metavar="IMPLEMENTATION",
     help="A container image which implements the bowtie IO protocol.",
 )
 DIALECT = click.option(
     "--dialect",
@@ -1116,15 +1097,15 @@
     description: str,
     **kwargs: Any,
 ):
     """
     Validate instances under a schema across any supported implementation.
     """
     if not instances:
-        return _EX_NOINPUT
+        return EX.NOINPUT
 
     tests = [Example(description="", instance=each) for each in instances]
     if expect is not None:
         tests = [test.expect(expect) for test in tests]
     case = TestCase(description=description, schema=schema, tests=tests)
     return asyncio.run(_run(fail_fast=False, **kwargs, cases=[case]))
 
@@ -1170,32 +1151,35 @@
     multiple=True,
     metavar="LANGUAGE",
     help="Only include implementations in the given programming language",
 )
 @click.pass_context
 async def filter_implementations(
     ctx: click.Context,
-    start: Callable[[], AsyncIterator[Implementation]],
+    start: Callable[
+        [],
+        AsyncIterator[tuple[ImplementationId, Implementation]],
+    ],
     dialects: Sequence[Dialect],
     languages: Set[str],
 ):
     """
     Output implementations which match the given criteria.
 
     Useful for piping or otherwise using the resulting output for further
     Bowtie commands.
     """
     if not dialects and languages == KNOWN_LANGUAGES:
-        for implementation in ctx.params.get("image_names", ()):
-            click.echo(implementation.removeprefix(f"{IMAGE_REPOSITORY}/"))
+        for name in start.connectables:  # type: ignore[reportFunctionMemberAccess]
+            click.echo(name)
         return
 
-    async for each in start():
+    async for name, each in start():
         if each.supports(*dialects) and each.info.language in languages:
-            click.echo(each.name.removeprefix(f"{IMAGE_REPOSITORY}/"))
+            click.echo(name)
 
 
 @implementation_subcommand(default_implementations=frozenset())  # type: ignore[reportArgumentType]
 @click.option(
     "--dialect",
     "-d",
     "dialects",
@@ -1220,15 +1204,18 @@
     default=None,
     help=(
         "If provided, show only dialects which do (or do not) "
         "support boolean schemas. Otherwise show either kind."
     ),
 )
 async def filter_dialects(
-    start: Callable[[], AsyncIterator[Implementation]],
+    start: Callable[
+        [],
+        AsyncIterator[tuple[ImplementationId, Implementation]],
+    ],
     dialects: Iterable[Dialect],
     latest: bool,
     booleans: bool | None,
 ):
     """
     Output dialect URIs matching a given criteria.
 
@@ -1237,39 +1224,42 @@
     """
     matching = {
         dialect
         for dialect in dialects
         if booleans is None or dialect.has_boolean_schemas == booleans
     }
 
-    async for implementation in start():
+    async for _, implementation in start():
         matching &= implementation.info.dialects
 
     if not matching:
         click.echo("No dialects match.", file=sys.stderr)
-        return _EX_DATAERR
+        return EX.DATAERR
 
     for dialect in sorted(matching, reverse=True):
         click.echo(dialect.uri)
         if latest:
             break
 
 
 @implementation_subcommand()  # type: ignore[reportArgumentType]
 @format_option
 async def info(
-    start: Callable[[], AsyncIterator[Implementation]],
+    start: Callable[
+        [],
+        AsyncIterator[tuple[ImplementationId, Implementation]],
+    ],
     format: _F,
 ):
     """
     Show information about a supported implementation.
     """
     serializable: dict[ImplementationId, dict[str, Any]] = {}
 
-    async for each in start():
+    async for _, each in start():
         metadata = [(k, v) for k, v in each.info.serializable().items() if v]
         metadata.sort(
             key=lambda kv: (
                 kv[0] != "name",
                 kv[0] != "language",
                 kv[0] != "version",
                 kv[0] == "links",
@@ -1313,32 +1303,35 @@
     # makes this work without doing it manually with callback.
     callback=lambda _, __, v: click.echo if not v else lambda *_, **__: None,  # type: ignore[reportUnknownLambdaType]
     is_flag=True,
     help="Don't print any output, just exit with nonzero status on failure.",
 )
 @format_option
 async def smoke(
-    start: Callable[[], AsyncIterator[Implementation]],
+    start: Callable[
+        [],
+        AsyncIterator[tuple[ImplementationId, Implementation]],
+    ],
     format: _F,
     echo: Callable[..., None],
 ) -> int:
     """
     Smoke test implementations for basic correctness against Bowtie's protocol.
     """
     exit_code = 0
 
-    async for implementation in start():
+    async for _, implementation in start():
         echo(f"Testing {implementation.name!r}...\n", file=sys.stderr)
         serializable: list[dict[str, Any]] = []
         implementation_exit_code = 0
 
         async for _, results in implementation.smoke():
             async for case, result in results:
                 if result.unsuccessful():
-                    implementation_exit_code |= _EX_DATAERR
+                    implementation_exit_code |= EX.DATAERR
 
                 match format:
                     case "json":
                         serializable.append(
                             dict(
                                 case=case.without_expected_results(),
                                 result=asdict(result.result),
@@ -1418,57 +1411,57 @@
     _cases, dialect, metadata = input
     cases = filter(_cases)
     task = _run(**kwargs, dialect=dialect, cases=cases, run_metadata=metadata)
     return asyncio.run(task)
 
 
 async def _run(
-    image_names: Iterable[str],
+    connectables: Iterable[_connectables.Connectable],
     cases: Iterable[TestCase],
     dialect: Dialect,
     fail_fast: bool,
     maybe_set_schema: Callable[[Dialect], CaseTransform],
     max_fail: int | None = None,
     max_error: int | None = None,
     run_metadata: dict[str, Any] = {},
     reporter: _report.Reporter = _report.Reporter(),
     **kwargs: Any,
 ) -> int:
     exit_code = 0
     acknowledged: list[ImplementationInfo] = []
     runners: list[DialectRunner] = []
     async with _start(
-        image_names=image_names,
+        connectables=connectables,
         reporter=reporter,
         **kwargs,
     ) as starting:
         for each in starting:
             try:
-                implementation = await each
+                _, implementation = await each
             except (NoSuchImplementation, StartupFailed) as error:
-                exit_code |= _EX_CONFIG
+                exit_code |= EX.CONFIG
                 STDERR.print(error)
                 continue
 
             try:
                 runner = await implementation.start_speaking(dialect)
             except DialectError as error:
-                exit_code |= _EX_CONFIG
+                exit_code |= EX.CONFIG
                 STDERR.print(error)
             except UnsupportedDialect as error:
                 STDERR.print(error)
             else:
                 acknowledged.append(implementation.info)
                 runners.append(runner)
 
         if not runners:
             STDERR.print(
                 "[bold red]No implementations started successfully![/]",
             )
-            return exit_code | _EX_CONFIG
+            return exit_code | EX.CONFIG
 
         reporter.ready(
             _report.RunMetadata(
                 implementations=acknowledged,
                 dialect=dialect,
                 metadata=run_metadata,
             ),
@@ -1498,56 +1491,40 @@
                 STDERR.print(
                     "[bold yellow]Stopping -- the maximum number of "
                     "unsuccessful tests was reached![/]",
                 )
                 break
         reporter.finished(did_fail_fast=should_stop)
         if count == 0:
-            exit_code = _EX_NOINPUT
+            exit_code = EX.NOINPUT
             STDERR.print("[bold red]No test cases ran.[/]")
         elif count > 1:  # XXX: Ugh, this should be removed when Reporter dies
             STDERR.print(f"Ran [green]{count}[/] test cases.")
     return exit_code
 
 
 @asynccontextmanager
 async def _start(
-    image_names: Iterable[str],
-    make_validator: MakeValidator,
+    connectables: Iterable[_connectables.Connectable],
     read_timeout_sec: float,
     **kwargs: Any,
 ):
-    @asynccontextmanager
-    async def _client(
-        docker: Docker,
-        image_name: str,
-    ) -> AsyncIterator[Implementation]:
-        async with (
-            _containers.Connection.open(
-                docker=docker,
-                image_name=image_name,
-                read_timeout_sec=read_timeout_sec,
-            ) as connection,
-            Implementation.start(
-                id=image_name,
-                connection=connection,
-                make_validator=make_validator,
-                **kwargs,
-            ) as implementation,
-        ):
-            yield implementation
+    async def _connected(
+        connectable: _connectables.Connectable,
+        **kwargs: Any,
+    ):
+        implementation = await stack.enter_async_context(
+            connectable.connect(**kwargs),
+        )
+        return connectable.to_terse(), implementation
 
     async with AsyncExitStack() as stack:
-        docker = await stack.enter_async_context(Docker())
-
-        implementations = [
-            stack.enter_async_context(_client(docker=docker, image_name=name))
-            for name in image_names
-        ]
-        yield asyncio.as_completed(implementations)
+        yield asyncio.as_completed(
+            [_connected(each, **kwargs) for each in connectables],
+        )
 
 
 def _stderr_processor(file: TextIO) -> structlog.typing.Processor:
     def stderr_processor(
         logger: structlog.typing.BindableLogger,
         method_name: str,
         event_dict: structlog.typing.EventDict,
```

### Comparing `bowtie_json_schema-2024.5.4/bowtie/_commands.py` & `bowtie_json_schema-2024.5.5/bowtie/_commands.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/bowtie/_containers.py` & `bowtie_json_schema-2024.5.5/bowtie/_containers.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,36 +9,41 @@
 
 from collections import deque
 from contextlib import asynccontextmanager, suppress
 from typing import TYPE_CHECKING
 import asyncio
 import json
 
+from aiodocker import Docker
 from attrs import field, frozen, mutable
 import aiodocker.exceptions
 
 from bowtie._core import (
     GotStderr,
     InvalidResponse,
     NoSuchImplementation,
     Restarted,
     StartupFailed,
 )
 
 if TYPE_CHECKING:
     from collections.abc import AsyncIterator, Awaitable
+    from contextlib import AbstractAsyncContextManager
     from typing import Any, Self
 
     import aiodocker.containers
     import aiodocker.docker
     import aiodocker.stream  # noqa: TCH004 ??? no it's not?
 
     from bowtie._commands import Message
 
 
+IMAGE_REPOSITORY = "ghcr.io/bowtie-json-schema"
+
+
 @frozen
 class _ClosedStream(Exception):
     """
     The stream is closed, and we tried to send something on it.
 
     This exception should never bubble out of this module, it should be handled
     by the connection.
@@ -151,40 +156,44 @@
     _stream: Stream = field(default=None, repr=False, alias="stream")
 
     # Maybe second versions of these will be useful also at the Implementation
     # level again, to control for non-protocol-related flakiness or slowness
     _restarts: int = field(default=10, repr=False, alias="restarts")
     _read_timeout_sec: float | None = field(
         default=2.0,
-        converter=lambda value: value or None,  # type: ignore[reportUnknownArgumentType]
+        converter=lambda value: value or None,  # type: ignore[reportUnknownLambdaType]
         repr=False,
     )
 
     #: A per-request number of retries, before giving up
     _retry: int = field(default=3, repr=False)
 
     @classmethod
     @asynccontextmanager
     async def open(
         cls,
         image_name: str,
         **kwargs: Any,
     ) -> AsyncIterator[Self]:
-        self = cls(image=image_name, **kwargs)
+        async with Docker() as docker:
+            self = cls(docker=docker, image=image_name, **kwargs)
 
-        try:
-            await self._start_container_maybe_pull()
-        except GotStderr as error:
-            err = StartupFailed(name=image_name, stderr=error.stderr.decode())
-            raise err from None
-        except _ClosedStream:
-            raise StartupFailed(name=image_name) from None
+            try:
+                await self._start_container_maybe_pull()
+            except GotStderr as error:
+                err = StartupFailed(
+                    name=image_name,
+                    stderr=error.stderr.decode(),
+                )
+                raise err from None
+            except _ClosedStream:
+                raise StartupFailed(name=image_name) from None
 
-        yield self
-        await self._stream.ensure_deleted()
+            yield self
+            await self._stream.ensure_deleted()
 
     async def _start_container_maybe_pull(self):
         # You would think we would use aiodocker's container.start() function
         # which essentially does the below. You would think wrong.
         # That function will pull the *entire* image repository if it ends up
         # pulling our harness image -- so here we reimplement it, but only
         # pull :latest when the image is missing.
@@ -276,7 +285,23 @@
             except json.JSONDecodeError as err:
                 raise InvalidResponse(contents=response) from err
 
     async def poison(self, message: dict[str, Any]) -> None:
         request = f"{json.dumps(message)}\n"
         with suppress(_ClosedStream):
             await self._stream.send(request)
+
+
+@frozen
+class ConnectableImage:
+
+    _id: str = field(
+        converter=lambda value: (  # type: ignore[reportUnknownLambdaType]
+            value if "/" in value else f"{IMAGE_REPOSITORY}/{value}"
+        ),
+        alias="id",
+    )
+
+    connector = "image"
+
+    def connect(self) -> AbstractAsyncContextManager[Connection]:
+        return Connection.open(image_name=self._id)
```

### Comparing `bowtie_json_schema-2024.5.4/bowtie/_core.py` & `bowtie_json_schema-2024.5.5/bowtie/_core.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/bowtie/_registry.py` & `bowtie_json_schema-2024.5.5/bowtie/_registry.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,63 +13,80 @@
 if TYPE_CHECKING:
     from referencing.jsonschema import Schema, SchemaRegistry, SchemaResource
 
 
 ErrorsFor = Callable[[Any], Iterable[Exception]]
 
 
+class UnexpectedlyValid(Exception):
+    """
+    An instance which was expected to be invalid just isn't.
+    """
+
+
 @frozen
 class Validator:
     """
     A compiled schema, ready to validate instances.
     """
 
     errors_for: ErrorsFor
+    _raises: tuple[type[Exception], ...] = field(alias="raises")
     _registry: ValidatorRegistry = field(alias="registry")
 
     def __rmatmul__(
         self,
         resources: SchemaResource | Iterable[SchemaResource],
     ) -> Validator:
         return evolve(self, registry=resources @ self._registry)
 
     def validate(self, instance: Any):
         exception = next(iter(self.errors_for(instance)), None)
         if exception is not None:
             raise exception
 
+    def invalidate(self, instance: Any):
+        exception = next(iter(self.errors_for(instance)), None)
+        if not isinstance(exception, self._raises):
+            raise UnexpectedlyValid(instance)
+
 
 @frozen
 class ValidatorRegistry:
 
     _compile: Callable[[Schema, SchemaRegistry], ErrorsFor] = field(
         alias="compile",
     )
+    _raises: tuple[type[Exception], ...] = field(
+        default=(Exception,),
+        alias="raises",
+    )
     _registry: SchemaRegistry = field(default=EMPTY_REGISTRY, alias="registry")
 
     def __rmatmul__(
         self,
         resources: SchemaResource | Iterable[SchemaResource],
     ) -> ValidatorRegistry:
         return evolve(self, registry=resources @ self._registry)
 
     @classmethod
     def jsonschema(cls, **kwargs: Any) -> ValidatorRegistry:
         """
         A registry which uses the `jsonschema` module to do validation.
         """
+        from jsonschema.exceptions import ValidationError
         from jsonschema.validators import (
             validator_for,  # type: ignore[reportUnknownVariableType]
         )
 
         def compile(schema: Schema, registry: SchemaRegistry) -> ErrorsFor:
             _Validator = validator_for(schema)  # type: ignore[reportUnknownVariableType]
             return _Validator(schema, registry=registry).iter_errors  # type: ignore[reportUnknownVariableType]
 
-        return cls(compile=compile, **kwargs)
+        return cls(compile=compile, raises=(ValidationError,), **kwargs)
 
     def schema(self, uri: str) -> Schema:
         """
         Return the schema identified by the given URI.
         """
         return self._registry.contents(uri)
 
@@ -80,8 +97,12 @@
         return self.for_schema(self.schema(uri))
 
     def for_schema(self, schema: Schema) -> Validator:
         """
         Return a `Validator` using the given schema.
         """
         errors_for: ErrorsFor = self._compile(schema, self._registry)
-        return Validator(errors_for=errors_for, registry=self)
+        return Validator(
+            errors_for=errors_for,
+            raises=self._raises,
+            registry=self,
+        )
```

### Comparing `bowtie_json_schema-2024.5.4/bowtie/_report.py` & `bowtie_json_schema-2024.5.5/bowtie/_report.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/bowtie/_suite.py` & `bowtie_json_schema-2024.5.5/bowtie/_suite.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/bowtie/exceptions.py` & `bowtie_json_schema-2024.5.5/bowtie/exceptions.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/bowtie/hypothesis.py` & `bowtie_json_schema-2024.5.5/bowtie/hypothesis.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/bowtie/schemas/report.json` & `bowtie_json_schema-2024.5.5/bowtie/schemas/report.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/bowtie/schemas/cli/info.json` & `bowtie_json_schema-2024.5.5/bowtie/schemas/cli/info.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/bowtie/schemas/cli/summary.json` & `bowtie_json_schema-2024.5.5/bowtie/schemas/cli/summary.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/bowtie/schemas/io/v1.json` & `bowtie_json_schema-2024.5.5/bowtie/schemas/io/v1.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/bowtie/schemas/io/commands/dialect.json` & `bowtie_json_schema-2024.5.5/bowtie/schemas/io/commands/dialect.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/bowtie/schemas/io/commands/run.json` & `bowtie_json_schema-2024.5.5/bowtie/schemas/io/commands/run.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/bowtie/schemas/io/commands/start.json` & `bowtie_json_schema-2024.5.5/bowtie/schemas/io/commands/start.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/bowtie/schemas/models/dialect.json` & `bowtie_json_schema-2024.5.5/bowtie/schemas/models/dialect.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/bowtie/schemas/models/group.json` & `bowtie_json_schema-2024.5.5/bowtie/schemas/models/group.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/bowtie/schemas/models/implementation.json` & `bowtie_json_schema-2024.5.5/bowtie/schemas/models/implementation.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/bowtie/schemas/models/test.json` & `bowtie_json_schema-2024.5.5/bowtie/schemas/models/test.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/data/dialects.json` & `bowtie_json_schema-2024.5.5/data/dialects.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/docs/Makefile` & `bowtie_json_schema-2024.5.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/docs/cli.rst` & `bowtie_json_schema-2024.5.5/docs/cli.rst`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     In general, these same subcommands allow repeating this argument multiple times to run across multiple implementations.
     In many or even most cases, you may be interested in running against *all* implementations Bowtie supports.
     For somewhat boring reasons (partially having to do with the GitHub API) this "run against all implementations" functionality is slightly nontrivial to implement in a seamless way, though doing so is nevertheless tracked in :issue:`this issue <24>`.
 
     In the interim, it's often convenient to use a local checkout of Bowtie in order to list this information.
 
     Specifically, all supported implementations live in the ``implementations/`` directory, and therefore you can construct a string of ``-i`` arguments using a small bit of shell vomit.
-    If you have cloned Bowtie to :file:`/path/to/bowtie` you should be able to use ``$(ls /path/to/bowtie/implementations/ | sed 's/^| /-i /')`` in any command to expand out to all implementations.
+    If you have cloned Bowtie to :file:`/path/to/bowtie` you should be able to use ``$(bowtie filter-implementations | sed 's/^/-i /')`` in any command to expand out to all implementations.
     See `below <cli:running the official suite across all implementations>` for a full example.
 
 Examples
 --------
 
 Validating a Specific Instance Against One or More Implementations
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
@@ -70,25 +70,25 @@
 Running the Official Suite Across All Implementations
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 The following will run all Draft 7 tests from the `official test suite`_ (which it will automatically retrieve) across all implementations supporting Draft 7, showing a summary of any test failures.
 
 .. code:: sh
 
-    $ bowtie suite $(ls /path/to/bowtie/implementations/ | sed 's/^| /-i /') https://github.com/json-schema-org/JSON-Schema-Test-Suite/tree/main/tests/draft7 | bowtie summary --show failures
+    $ bowtie suite $(bowtie filter-implementations | sed 's/^/-i /') https://github.com/json-schema-org/JSON-Schema-Test-Suite/tree/main/tests/draft7 | bowtie summary --show failures
 
 
 Running Test Suite Tests From Local Checkouts
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Providing a local path to the test suite can be used as well, which is useful if you have local changes:
 
 .. code:: sh
 
-    $ bowtie suite $(ls /path/to/bowtie/implementations/ | sed 's/^| /-i /') ~/path/to/json-schema-org/suite/tests/draft2020-12/ | bowtie summary --show failures
+    $ bowtie suite $(bowtie filter-implementations | sed 's/^/-i /') ~/path/to/json-schema-org/suite/tests/draft2020-12/ | bowtie summary --show failures
 
 
 Checking An Implementation Functions On Basic Input
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 If you wish to verify that a particular implementation works on your machine (e.g. if you suspect a problem with the container image, or otherwise aren't seeing results), you can run `bowtie smoke <cli:smoke>`.
 E.g., to verify the Golang ``jsonschema`` implementation is functioning, you can run:
```

### Comparing `bowtie_json_schema-2024.5.4/docs/conf.py` & `bowtie_json_schema-2024.5.5/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,14 +127,15 @@
 intersphinx_mapping = {
     "click": ("https://click.palletsprojects.com", None),
     "nox": ("https://nox.thea.codes/en/stable/", None),
     "pip": ("https://pip.pypa.io/en/stable/", None),
     "podman": ("https://docs.podman.io/en/latest", None),
     "python": ("https://docs.python.org/", None),
     "sphinx": ("https://www.sphinx-doc.org", None),
+    "twisted": ("https://docs.twistedmatrix.com/en/stable", None),
 }
 
 # -- extlinks --
 
 extlinks = {
     "gh": (str(REPO) + "/%s", None),
     "github": (str(GITHUB) + "/%s", None),
```

### Comparing `bowtie_json_schema-2024.5.4/docs/contributing.rst` & `bowtie_json_schema-2024.5.5/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/docs/github-actions.rst` & `bowtie_json_schema-2024.5.5/docs/github-actions.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/docs/implementers.rst` & `bowtie_json_schema-2024.5.5/docs/implementers.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/docs/index.rst` & `bowtie_json_schema-2024.5.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/docs/motd.txt` & `bowtie_json_schema-2024.5.5/docs/motd.txt`

 * *Files 5% similar despite different names*

```diff
@@ -37,10 +37,10 @@
 
     Given some collection of implementations to check - here perhaps two Javascript implementations - it takes a single schema and one or more instances to check against it.
 
   $ bowtie suite -i lua-jsonschema https://github.com/json-schema-org/JSON-Schema-Test-Suite/blob/main/tests/draft7/type.json | bowtie summary --show failures
 
     Run a specific file from the draft 7 official test suite against a single implementation.
 
-  $ bowtie suite $(ls /path/to/bowtie/implementations/ | sed 's/^| /-i /') https://github.com/json-schema-org/JSON-Schema-Test-Suite/tree/main/tests/draft7 | bowtie summary --show failures
+  $ bowtie suite $(bowtie filter-implementations | sed 's/^/-i /') https://github.com/json-schema-org/JSON-Schema-Test-Suite/tree/main/tests/draft7 | bowtie summary --show failures
 
     Run the entire draft 2020-12 test suite against all implementations which support it.
```

### Comparing `bowtie_json_schema-2024.5.4/docs/requirements.txt` & `bowtie_json_schema-2024.5.5/docs/requirements.txt`

 * *Files 1% similar despite different names*

```diff
@@ -10,30 +10,30 @@
     # via sphinx
 attrs==23.2.0
     # via
     #   aiohttp
     #   bowtie-json-schema
     #   jsonschema
     #   referencing
-babel==2.14.0
+babel==2.15.0
     # via sphinx
 beautifulsoup4==4.12.3
     # via furo
 bowtie-json-schema @ file:.#egg=bowtie-json-schema
 certifi==2024.2.2
     # via requests
 cffi==1.16.0
     # via cryptography
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via
     #   rich-click
     #   sphinx-click
-cryptography==42.0.5
+cryptography==42.0.7
     # via pyjwt
 diagnostic==2.1.0
     # via bowtie-json-schema
 docutils==0.21.2
     # via
     #   diagnostic
     #   sphinx
@@ -41,24 +41,24 @@
     #   sphinx-prompt
     #   sphinx-substitution-extensions
     #   sphinx-tabs
 frozenlist==1.4.1
     # via
     #   aiohttp
     #   aiosignal
-furo==2024.4.27
+furo==2024.5.6
 github3-py==4.0.1
     # via bowtie-json-schema
 idna==3.7
     # via
     #   requests
     #   yarl
 imagesize==1.4.1
     # via sphinx
-jinja2==3.1.3
+jinja2==3.1.4
     # via sphinx
 jsonschema==4.22.0
     # via bowtie-json-schema
 jsonschema-lexer==0.2.1
     # via bowtie-json-schema
 jsonschema-specifications==2023.12.1
     # via jsonschema
@@ -78,29 +78,29 @@
     #   yarl
 packaging==24.0
     # via sphinx
 pycparser==2.22
     # via cffi
 pyenchant==3.2.2
     # via sphinxcontrib-spelling
-pygments==2.17.2
+pygments==2.18.0
     # via
     #   furo
     #   jsonschema-lexer
     #   pygments-github-lexers
     #   rich
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
 pygments-github-lexers==0.0.5
 pyjwt==2.8.0
     # via github3-py
 python-dateutil==2.9.0.post0
     # via github3-py
-referencing==0.35.0
+referencing==0.35.1
     # via
     #   bowtie-json-schema
     #   jsonschema
     #   jsonschema-specifications
     #   referencing-loaders
 referencing-loaders==2024.5.2
     # via bowtie-json-schema
@@ -111,15 +111,15 @@
 rich==13.7.1
     # via
     #   bowtie-json-schema
     #   diagnostic
     #   rich-click
 rich-click==1.8.0
     # via bowtie-json-schema
-rpds-py==0.18.0
+rpds-py==0.18.1
     # via
     #   bowtie-json-schema
     #   jsonschema
     #   referencing
 six==1.16.0
     # via python-dateutil
 snowballstemmer==2.2.0
```

### Comparing `bowtie_json_schema-2024.5.4/docs/_static/bowtie_diagram_dark.svg` & `bowtie_json_schema-2024.5.5/docs/_static/bowtie_diagram_dark.svg`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/docs/_static/bowtie_diagram_light.svg` & `bowtie_json_schema-2024.5.5/docs/_static/bowtie_diagram_light.svg`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/docs/_static/logo.svg` & `bowtie_json_schema-2024.5.5/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/frontend/package.json` & `bowtie_json_schema-2024.5.5/frontend/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9473684210526315%*

 * *Differences: {"'devDependencies'": "{'@types/react-syntax-highlighter': '^15.5.13', 'vitest': '^1.6.0'}",*

 * * "'packageManager'": "'pnpm@9.1.0'"}*

```diff
@@ -10,15 +10,15 @@
         "react-syntax-highlighter": "^15.5.0",
         "urijs": "^1.19.11"
     },
     "description": "The UI displays the outcomes generated by Bowtie, which serves as a meta-validator for the JSON Schema specification",
     "devDependencies": {
         "@types/react": "^18.3.1",
         "@types/react-dom": "^18.3.0",
-        "@types/react-syntax-highlighter": "^15.5.11",
+        "@types/react-syntax-highlighter": "^15.5.13",
         "@types/react-test-renderer": "^18.3.0",
         "@types/urijs": "^1.19.25",
         "@typescript-eslint/eslint-plugin": "^7.8.0",
         "@typescript-eslint/parser": "^7.8.0",
         "@vitejs/plugin-react": "^4.2.1",
         "eslint": "8.57.0",
         "eslint-plugin-react": "7.34.1",
@@ -26,15 +26,15 @@
         "jsdom": "^24.0.0",
         "react-test-renderer": "^18.3.1",
         "ts-loader": "^9.5.1",
         "ts-node": "^10.9.2",
         "typescript": "^5.4.5",
         "vite": "^5.2.11",
         "vite-bundle-visualizer": "^1.1.0",
-        "vitest": "^1.5.3"
+        "vitest": "^1.6.0"
     },
     "engines": {
         "node": ">=21.0.0"
     },
     "eslintConfig": {
         "env": {
             "browser": true,
@@ -70,15 +70,15 @@
         "settings": {
             "react": {
                 "version": "18.2"
             }
         }
     },
     "name": "bowtie",
-    "packageManager": "pnpm@9.0.6",
+    "packageManager": "pnpm@9.1.0",
     "scripts": {
         "build": "tsc && vite build",
         "bundle-visualizer": "vite-bundle-visualizer",
         "lint": "eslint src --max-warnings 0",
         "preview": "vite preview",
         "start": "vite --no-clearScreen",
         "test": "vitest run",
```

### Comparing `bowtie_json_schema-2024.5.4/frontend/pnpm-lock.yaml` & `bowtie_json_schema-2024.5.5/frontend/pnpm-lock.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -39,16 +39,16 @@
       '@types/react':
         specifier: ^18.3.1
         version: 18.3.1
       '@types/react-dom':
         specifier: ^18.3.0
         version: 18.3.0
       '@types/react-syntax-highlighter':
-        specifier: ^15.5.11
-        version: 15.5.11
+        specifier: ^15.5.13
+        version: 15.5.13
       '@types/react-test-renderer':
         specifier: ^18.3.0
         version: 18.3.0
       '@types/urijs':
         specifier: ^1.19.25
         version: 1.19.25
       '@typescript-eslint/eslint-plugin':
@@ -87,16 +87,16 @@
       vite:
         specifier: ^5.2.11
         version: 5.2.11(@types/node@20.11.5)(terser@5.27.0)
       vite-bundle-visualizer:
         specifier: ^1.1.0
         version: 1.1.0(rollup@4.17.2)
       vitest:
-        specifier: ^1.5.3
-        version: 1.5.3(@types/node@20.11.5)(jsdom@24.0.0)(terser@5.27.0)
+        specifier: ^1.6.0
+        version: 1.6.0(@types/node@20.11.5)(jsdom@24.0.0)(terser@5.27.0)
 
 packages:
 
   '@ampproject/remapping@2.3.0':
     resolution: {integrity: sha512-30iZtAPgz+LTIYoeivqYo853f02jBYSd5uGnGpkFV0M3xOt9aN73erkgYAmZU43x4VfqcnLxW9Kpg3R5LC4YYw==}
     engines: {node: '>=6.0.0'}
 
@@ -572,16 +572,16 @@
 
   '@types/prop-types@15.7.12':
     resolution: {integrity: sha512-5zvhXYtRNRluoE/jAp4GVsSduVUzNWKkOZrCDBWYtE7biZywwdC2AcEzg+cSMLFRfVgeAFqpfNabiPjxFddV1Q==}
 
   '@types/react-dom@18.3.0':
     resolution: {integrity: sha512-EhwApuTmMBmXuFOikhQLIBUn6uFg81SwLMOAUgodJF14SOBOCMdU04gDoYi0WOJJHD144TL32z4yDqCW3dnkQg==}
 
-  '@types/react-syntax-highlighter@15.5.11':
-    resolution: {integrity: sha512-ZqIJl+Pg8kD+47kxUjvrlElrraSUrYa4h0dauY/U/FTUuprSCqvUj+9PNQNQzVc6AJgIWUUxn87/gqsMHNbRjw==}
+  '@types/react-syntax-highlighter@15.5.13':
+    resolution: {integrity: sha512-uLGJ87j6Sz8UaBAooU0T6lWJ0dBmjZgN1PZTrj05TNql2/XpC6+4HhMT5syIdFUUt+FASfCeLLv4kBygNU+8qA==}
 
   '@types/react-test-renderer@18.3.0':
     resolution: {integrity: sha512-HW4MuEYxfDbOHQsVlY/XtOvNHftCVEPhJF2pQXXwcUiUF+Oyb0usgp48HSgpK5rt8m9KZb22yqOeZm+rrVG8gw==}
 
   '@types/react-transition-group@4.4.10':
     resolution: {integrity: sha512-hT/+s0VQs2ojCX823m60m5f0sL5idt9SO6Tj6Dg+rdphGPIeJbJ6CxvBYkgkGKrYeDjvIpKTR38UzmtHJOGW3Q==}
 
@@ -663,28 +663,28 @@
 
   '@vitejs/plugin-react@4.2.1':
     resolution: {integrity: sha512-oojO9IDc4nCUUi8qIR11KoQm0XFFLIwsRBwHRR4d/88IWghn1y6ckz/bJ8GHDCsYEJee8mDzqtJxh15/cisJNQ==}
     engines: {node: ^14.18.0 || >=16.0.0}
     peerDependencies:
       vite: ^4.2.0 || ^5.0.0
 
-  '@vitest/expect@1.5.3':
-    resolution: {integrity: sha512-y+waPz31pOFr3rD7vWTbwiLe5+MgsMm40jTZbQE8p8/qXyBX3CQsIXRx9XK12IbY7q/t5a5aM/ckt33b4PxK2g==}
+  '@vitest/expect@1.6.0':
+    resolution: {integrity: sha512-ixEvFVQjycy/oNgHjqsL6AZCDduC+tflRluaHIzKIsdbzkLn2U/iBnVeJwB6HsIjQBdfMR8Z0tRxKUsvFJEeWQ==}
 
-  '@vitest/runner@1.5.3':
-    resolution: {integrity: sha512-7PlfuReN8692IKQIdCxwir1AOaP5THfNkp0Uc4BKr2na+9lALNit7ub9l3/R7MP8aV61+mHKRGiqEKRIwu6iiQ==}
+  '@vitest/runner@1.6.0':
+    resolution: {integrity: sha512-P4xgwPjwesuBiHisAVz/LSSZtDjOTPYZVmNAnpHHSR6ONrf8eCJOFRvUwdHn30F5M1fxhqtl7QZQUk2dprIXAg==}
 
-  '@vitest/snapshot@1.5.3':
-    resolution: {integrity: sha512-K3mvIsjyKYBhNIDujMD2gfQEzddLe51nNOAf45yKRt/QFJcUIeTQd2trRvv6M6oCBHNVnZwFWbQ4yj96ibiDsA==}
+  '@vitest/snapshot@1.6.0':
+    resolution: {integrity: sha512-+Hx43f8Chus+DCmygqqfetcAZrDJwvTj0ymqjQq4CvmpKFSTVteEOBzCusu1x2tt4OJcvBflyHUE0DZSLgEMtQ==}
 
-  '@vitest/spy@1.5.3':
-    resolution: {integrity: sha512-Llj7Jgs6lbnL55WoshJUUacdJfjU2honvGcAJBxhra5TPEzTJH8ZuhI3p/JwqqfnTr4PmP7nDmOXP53MS7GJlg==}
+  '@vitest/spy@1.6.0':
+    resolution: {integrity: sha512-leUTap6B/cqi/bQkXUu6bQV5TZPx7pmMBKBQiI0rJA8c3pB56ZsaTbREnF7CJfmvAS4V2cXIBAh/3rVwrrCYgw==}
 
-  '@vitest/utils@1.5.3':
-    resolution: {integrity: sha512-rE9DTN1BRhzkzqNQO+kw8ZgfeEBCLXiHJwetk668shmNBpSagQxneT5eSqEBLP+cqSiAeecvQmbpFfdMyLcIQA==}
+  '@vitest/utils@1.6.0':
+    resolution: {integrity: sha512-21cPiuGMoMZwiOHa2i4LXkMkMkCGzA+MVFV70jRwHo95dL4x/ts5GZhML1QWuy7yfp3WzK3lRvZi3JnXTYqrBw==}
 
   '@webassemblyjs/ast@1.12.1':
     resolution: {integrity: sha512-EKfMUOPRRUTy5UII4qJDGPpqfwjOmZ5jeGFwid9mnoqIFK+e0vqoi1qH56JpmZSzEL53jKnNzScdmftJyG5xWg==}
 
   '@webassemblyjs/floating-point-hex-parser@1.11.6':
     resolution: {integrity: sha512-ejAj9hfRJ2XMsNHk/v6Fu2dGS+i4UaXBXGemOfQ/JfQ6mdQg/WXtwleQRLLS4OvfDhv8rYnVwH27YJLMyYsxhw==}
 
@@ -2270,16 +2270,16 @@
     resolution: {integrity: sha512-wa7YjyUGfNZngI/vtK0UHAN+lgDCxBPCylVXGp0zu59Fz5aiGtNXaq3DhIov063MorB+VfufLh3JlF2KdTK3xg==}
 
   vite-bundle-visualizer@1.1.0:
     resolution: {integrity: sha512-cmi5OuS7Eta5keTJmCTEbBBA7gOsUQ4K44W5dbsP+n/X0GIilIIFbJeXF120MQpTxdiZ/GIx4A9zkPEcKpPAog==}
     engines: {node: ^18.19.0 || >=20.6.0}
     hasBin: true
 
-  vite-node@1.5.3:
-    resolution: {integrity: sha512-axFo00qiCpU/JLd8N1gu9iEYL3xTbMbMrbe5nDp9GL0nb6gurIdZLkkFogZXWnE8Oyy5kfSLwNVIcVsnhE7lgQ==}
+  vite-node@1.6.0:
+    resolution: {integrity: sha512-de6HJgzC+TFzOu0NTC4RAIsyf/DY/ibWDYQUcuEA84EMHhcefTUGkjFHKKEJhQN4A+6I0u++kr3l36ZF2d7XRw==}
     engines: {node: ^18.0.0 || >=20.0.0}
     hasBin: true
 
   vite@5.2.11:
     resolution: {integrity: sha512-HndV31LWW05i1BLPMUCE1B9E9GFbOu1MbenhS58FuK6owSO5qHm7GiCotrNY1YE5rMeQSFBGmT5ZaLEjFizgiQ==}
     engines: {node: ^18.0.0 || >=20.0.0}
     hasBin: true
@@ -2303,23 +2303,23 @@
       stylus:
         optional: true
       sugarss:
         optional: true
       terser:
         optional: true
 
-  vitest@1.5.3:
-    resolution: {integrity: sha512-2oM7nLXylw3mQlW6GXnRriw+7YvZFk/YNV8AxIC3Z3MfFbuziLGWP9GPxxu/7nRlXhqyxBikpamr+lEEj1sUEw==}
+  vitest@1.6.0:
+    resolution: {integrity: sha512-H5r/dN06swuFnzNFhq/dnz37bPXnq8xB2xB5JOVk8K09rUtoeNN+LHWkoQ0A/i3hvbUKKcCei9KpbxqHMLhLLA==}
     engines: {node: ^18.0.0 || >=20.0.0}
     hasBin: true
     peerDependencies:
       '@edge-runtime/vm': '*'
       '@types/node': ^18.0.0 || >=20.0.0
-      '@vitest/browser': 1.5.3
-      '@vitest/ui': 1.5.3
+      '@vitest/browser': 1.6.0
+      '@vitest/ui': 1.6.0
       happy-dom: '*'
       jsdom: '*'
     peerDependenciesMeta:
       '@edge-runtime/vm':
         optional: true
       '@types/node':
         optional: true
@@ -2897,15 +2897,15 @@
 
   '@types/prop-types@15.7.12': {}
 
   '@types/react-dom@18.3.0':
     dependencies:
       '@types/react': 18.3.1
 
-  '@types/react-syntax-highlighter@15.5.11':
+  '@types/react-syntax-highlighter@15.5.13':
     dependencies:
       '@types/react': 18.3.1
 
   '@types/react-test-renderer@18.3.0':
     dependencies:
       '@types/react': 18.3.1
 
@@ -3021,37 +3021,37 @@
       '@babel/plugin-transform-react-jsx-source': 7.24.1(@babel/core@7.24.5)
       '@types/babel__core': 7.20.5
       react-refresh: 0.14.2
       vite: 5.2.11(@types/node@20.11.5)(terser@5.27.0)
     transitivePeerDependencies:
       - supports-color
 
-  '@vitest/expect@1.5.3':
+  '@vitest/expect@1.6.0':
     dependencies:
-      '@vitest/spy': 1.5.3
-      '@vitest/utils': 1.5.3
+      '@vitest/spy': 1.6.0
+      '@vitest/utils': 1.6.0
       chai: 4.4.1
 
-  '@vitest/runner@1.5.3':
+  '@vitest/runner@1.6.0':
     dependencies:
-      '@vitest/utils': 1.5.3
+      '@vitest/utils': 1.6.0
       p-limit: 5.0.0
       pathe: 1.1.2
 
-  '@vitest/snapshot@1.5.3':
+  '@vitest/snapshot@1.6.0':
     dependencies:
       magic-string: 0.30.10
       pathe: 1.1.2
       pretty-format: 29.7.0
 
-  '@vitest/spy@1.5.3':
+  '@vitest/spy@1.6.0':
     dependencies:
       tinyspy: 2.2.1
 
-  '@vitest/utils@1.5.3':
+  '@vitest/utils@1.6.0':
     dependencies:
       diff-sequences: 29.6.3
       estree-walker: 3.0.3
       loupe: 2.3.7
       pretty-format: 29.7.0
 
   '@webassemblyjs/ast@1.12.1':
@@ -4886,15 +4886,15 @@
       import-from-esm: 1.3.4
       rollup-plugin-visualizer: 5.12.0(rollup@4.17.2)
       tmp: 0.2.3
     transitivePeerDependencies:
       - rollup
       - supports-color
 
-  vite-node@1.5.3(@types/node@20.11.5)(terser@5.27.0):
+  vite-node@1.6.0(@types/node@20.11.5)(terser@5.27.0):
     dependencies:
       cac: 6.7.14
       debug: 4.3.4
       pathe: 1.1.2
       picocolors: 1.0.0
       vite: 5.2.11(@types/node@20.11.5)(terser@5.27.0)
     transitivePeerDependencies:
@@ -4913,35 +4913,35 @@
       postcss: 8.4.38
       rollup: 4.17.2
     optionalDependencies:
       '@types/node': 20.11.5
       fsevents: 2.3.3
       terser: 5.27.0
 
-  vitest@1.5.3(@types/node@20.11.5)(jsdom@24.0.0)(terser@5.27.0):
+  vitest@1.6.0(@types/node@20.11.5)(jsdom@24.0.0)(terser@5.27.0):
     dependencies:
-      '@vitest/expect': 1.5.3
-      '@vitest/runner': 1.5.3
-      '@vitest/snapshot': 1.5.3
-      '@vitest/spy': 1.5.3
-      '@vitest/utils': 1.5.3
+      '@vitest/expect': 1.6.0
+      '@vitest/runner': 1.6.0
+      '@vitest/snapshot': 1.6.0
+      '@vitest/spy': 1.6.0
+      '@vitest/utils': 1.6.0
       acorn-walk: 8.3.2
       chai: 4.4.1
       debug: 4.3.4
       execa: 8.0.1
       local-pkg: 0.5.0
       magic-string: 0.30.10
       pathe: 1.1.2
       picocolors: 1.0.0
       std-env: 3.7.0
       strip-literal: 2.1.0
       tinybench: 2.8.0
       tinypool: 0.8.4
       vite: 5.2.11(@types/node@20.11.5)(terser@5.27.0)
-      vite-node: 1.5.3(@types/node@20.11.5)(terser@5.27.0)
+      vite-node: 1.6.0(@types/node@20.11.5)(terser@5.27.0)
       why-is-node-running: 2.2.2
     optionalDependencies:
       '@types/node': 20.11.5
       jsdom: 24.0.0
     transitivePeerDependencies:
       - less
       - lightningcss
```

### Comparing `bowtie_json_schema-2024.5.4/frontend/tsconfig.json` & `bowtie_json_schema-2024.5.5/frontend/tsconfig.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/frontend/public/favicon.svg` & `bowtie_json_schema-2024.5.5/frontend/public/favicon.svg`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/frontend/src/DialectReportView.tsx` & `bowtie_json_schema-2024.5.5/frontend/src/DialectReportView.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/frontend/src/ReportDataHandler.tsx` & `bowtie_json_schema-2024.5.5/frontend/src/ReportDataHandler.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/frontend/src/index.tsx` & `bowtie_json_schema-2024.5.5/frontend/src/index.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/frontend/src/assets/landscape-logo.svg` & `bowtie_json_schema-2024.5.5/frontend/src/assets/landscape-logo.svg`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/frontend/src/components/CopyToClipboard.tsx` & `bowtie_json_schema-2024.5.5/frontend/src/components/CopyToClipboard.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/frontend/src/components/FilterSection.tsx` & `bowtie_json_schema-2024.5.5/frontend/src/components/FilterSection.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/frontend/src/components/NavBar.tsx` & `bowtie_json_schema-2024.5.5/frontend/src/components/NavBar.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/frontend/src/components/OtherImplementations.tsx` & `bowtie_json_schema-2024.5.5/frontend/src/components/OtherImplementations.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/frontend/src/components/BowtieInfo/BowtieInfoSection.tsx` & `bowtie_json_schema-2024.5.5/frontend/src/components/BowtieInfo/BowtieInfoSection.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/frontend/src/components/Cases/CaseItem.tsx` & `bowtie_json_schema-2024.5.5/frontend/src/components/Cases/CaseItem.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/frontend/src/components/Cases/CaseResultSvg.test.tsx` & `bowtie_json_schema-2024.5.5/frontend/src/components/Cases/CaseResultSvg.test.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/frontend/src/components/Cases/CaseResultSvg.tsx` & `bowtie_json_schema-2024.5.5/frontend/src/components/Cases/CaseResultSvg.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/frontend/src/components/Cases/CasesSection.tsx` & `bowtie_json_schema-2024.5.5/frontend/src/components/Cases/CasesSection.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/frontend/src/components/Cases/SchemaDisplay.tsx` & `bowtie_json_schema-2024.5.5/frontend/src/components/Cases/SchemaDisplay.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/frontend/src/components/DragAndDrop/DragAndDrop.tsx` & `bowtie_json_schema-2024.5.5/frontend/src/components/DragAndDrop/DragAndDrop.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/frontend/src/components/ImplementationReportView/DialectCompliance.tsx` & `bowtie_json_schema-2024.5.5/frontend/src/components/ImplementationReportView/DialectCompliance.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/frontend/src/components/ImplementationReportView/EmbedBadges.tsx` & `bowtie_json_schema-2024.5.5/frontend/src/components/ImplementationReportView/EmbedBadges.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/frontend/src/components/ImplementationReportView/ImplementationReportView.tsx` & `bowtie_json_schema-2024.5.5/frontend/src/components/ImplementationReportView/ImplementationReportView.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/frontend/src/components/Modals/DetailsButtonModal.tsx` & `bowtie_json_schema-2024.5.5/frontend/src/components/Modals/DetailsButtonModal.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/frontend/src/components/RunInfo/RunInfoSection.tsx` & `bowtie_json_schema-2024.5.5/frontend/src/components/RunInfo/RunInfoSection.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/frontend/src/components/Summary/ImplementationRow.css` & `bowtie_json_schema-2024.5.5/frontend/src/components/Summary/ImplementationRow.css`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/frontend/src/components/Summary/ImplementationRow.tsx` & `bowtie_json_schema-2024.5.5/frontend/src/components/Summary/ImplementationRow.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/frontend/src/components/Summary/SummarySection.tsx` & `bowtie_json_schema-2024.5.5/frontend/src/components/Summary/SummarySection.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/frontend/src/components/Summary/SummaryTable.tsx` & `bowtie_json_schema-2024.5.5/frontend/src/components/Summary/SummaryTable.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/frontend/src/context/BowtieVersionContext.tsx` & `bowtie_json_schema-2024.5.5/frontend/src/context/BowtieVersionContext.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/frontend/src/context/ThemeContext.tsx` & `bowtie_json_schema-2024.5.5/frontend/src/context/ThemeContext.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/frontend/src/data/Badge.test.ts` & `bowtie_json_schema-2024.5.5/frontend/src/data/Badge.test.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/frontend/src/data/Badge.ts` & `bowtie_json_schema-2024.5.5/frontend/src/data/Badge.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/frontend/src/data/Dialect.ts` & `bowtie_json_schema-2024.5.5/frontend/src/data/Dialect.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/frontend/src/data/Site.test.ts` & `bowtie_json_schema-2024.5.5/frontend/src/data/Site.test.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/frontend/src/data/parseReportData.test.ts` & `bowtie_json_schema-2024.5.5/frontend/src/data/parseReportData.test.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/frontend/src/data/parseReportData.ts` & `bowtie_json_schema-2024.5.5/frontend/src/data/parseReportData.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/implementations/.java-implementations-pmd-ruleset.xml` & `bowtie_json_schema-2024.5.5/implementations/.java-implementations-pmd-ruleset.xml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/implementations/clojure-json-schema/Dockerfile` & `bowtie_json_schema-2024.5.5/implementations/clojure-json-schema/Dockerfile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/implementations/clojure-json-schema/src/bowtie_json_schema/core.clj` & `bowtie_json_schema-2024.5.5/implementations/clojure-json-schema/src/bowtie_json_schema/core.clj`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/implementations/cpp-valijson/bowtie_valijson.cpp` & `bowtie_json_schema-2024.5.5/implementations/cpp-valijson/bowtie_valijson.cpp`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/implementations/dotnet-jsonschema-net/.gitignore` & `bowtie_json_schema-2024.5.5/implementations/dotnet-jsonschema-net/.gitignore`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/implementations/dotnet-jsonschema-net/Program.cs` & `bowtie_json_schema-2024.5.5/implementations/dotnet-jsonschema-net/Program.cs`

 * *Files 1% similar despite different names*

```diff
@@ -151,15 +151,15 @@
             throw new UnknownCommand(cmd);
     }
 }
 
 static string GetLibVersion()
 {
     var attribute = typeof(JsonSchema).Assembly.GetCustomAttribute<AssemblyInformationalVersionAttribute>();
-    return Regex.Match(attribute!.InformationalVersion, @"\d+\.\d+\.\d+").Value;
+    return Regex.Match(attribute!.InformationalVersion, @"\d+(\.\d+)+").Value;
 }
 
 class UnknownCommand : Exception
 {
     public UnknownCommand(string message) { }
 }
```

### Comparing `bowtie_json_schema-2024.5.4/implementations/go-gojsonschema/bowtie_gojsonschema.go` & `bowtie_json_schema-2024.5.5/implementations/go-gojsonschema/bowtie_gojsonschema.go`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/implementations/go-gojsonschema/go.sum` & `bowtie_json_schema-2024.5.5/implementations/go-gojsonschema/go.sum`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/implementations/go-jsonschema/bowtie_jsonschema.go` & `bowtie_json_schema-2024.5.5/implementations/go-jsonschema/bowtie_jsonschema.go`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/implementations/java-json-schema/BowtieJsonSchema.java` & `bowtie_json_schema-2024.5.5/implementations/java-json-schema/BowtieJsonSchema.java`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/implementations/java-json-schema/build.gradle` & `bowtie_json_schema-2024.5.5/implementations/java-json-schema/build.gradle`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         group: 'dev.harrel',
         name: 'json-schema',
         version: '1.6.0'
 ]
 def jsonProvider = [
         group: 'com.fasterxml.jackson.core',
         name: 'jackson-databind',
-        version: '2.17.0'
+        version: '2.17.1'
 ]
 
 dependencies {
     /* Verbose dependency notation for dependabot */
     implementation "$harnessImplementation.group:$harnessImplementation.name:$harnessImplementation.version"
     implementation "$jsonProvider.group:$jsonProvider.name:$jsonProvider.version"
 }
```

### Comparing `bowtie_json_schema-2024.5.4/implementations/java-json-schema-validator/BowtieJsonSchemaValidator.java` & `bowtie_json_schema-2024.5.5/implementations/java-networknt-json-schema-validator/BowtieJsonSchemaValidator.java`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/implementations/java-json-schema-validator/build.gradle` & `bowtie_json_schema-2024.5.5/implementations/java-networknt-json-schema-validator/build.gradle`

 * *Files 9% similar despite different names*

```diff
@@ -30,11 +30,11 @@
     archiveBaseName = 'harness'
     duplicatesStrategy = DuplicatesStrategy.EXCLUDE
     from {
         configurations.runtimeClasspath.collect { it.isDirectory() ? it : zipTree(it) }
     }
     manifest {
         attributes "Main-Class": "BowtieJsonSchemaValidator"
-        attributes "Implementation-Name": harnessImplementation.name
+        attributes "Implementation-Name": "$harnessImplementation.group-$harnessImplementation.name"
         attributes "Implementation-Version": harnessImplementation.version
     }
 }
```

### Comparing `bowtie_json_schema-2024.5.4/implementations/java-jsonschemafriend/BowtieJsonSchemaFriend.java` & `bowtie_json_schema-2024.5.5/implementations/java-jsonschemafriend/BowtieJsonSchemaFriend.java`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/implementations/java-jsonschemafriend/build.gradle` & `bowtie_json_schema-2024.5.5/implementations/java-jsonschemafriend/build.gradle`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         group: 'net.jimblackler.jsonschemafriend',
         name: 'core',
         version: '0.12.4'
 ]
 def jsonProvider = [
         group: 'com.fasterxml.jackson.core',
         name: 'jackson-databind',
-        version: '2.17.0'
+        version: '2.17.1'
 ]
 
 dependencies {
     /* Verbose dependency notation for dependabot */
     implementation "$harnessImplementation.group:$harnessImplementation.name:$harnessImplementation.version"
     implementation "$jsonProvider.group:$jsonProvider.name:$jsonProvider.version"
 }
```

### Comparing `bowtie_json_schema-2024.5.4/implementations/java-openapiprocessor/build.gradle.kts` & `bowtie_json_schema-2024.5.5/implementations/java-openapiprocessor/build.gradle.kts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/implementations/java-openapiprocessor/justfile` & `bowtie_json_schema-2024.5.5/implementations/java-openapiprocessor/justfile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/implementations/java-openapiprocessor/gradle/libs.versions.toml` & `bowtie_json_schema-2024.5.5/implementations/java-openapiprocessor/gradle/libs.versions.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [versions]
 validator = "2024.2"
 
-kotlin = "1.9.23"
+kotlin = "1.9.24"
 build-jdk = "11"
 
 [libraries]
 jsv-bom = { module = "io.openapiprocessor:json-schema-validator-bom", version.ref = "validator" }
 jsv-validator = { module = "io.openapiprocessor:json-schema-validator" }
 io-interfaces = { module = "io.openapiprocessor:io-interfaces" }
 io-jackson = { module = "io.openapiprocessor:io-jackson" }
 
-jackson-bom = "com.fasterxml.jackson:jackson-bom:2.17.0"
+jackson-bom = "com.fasterxml.jackson:jackson-bom:2.17.1"
 jackson-databind = { module = "com.fasterxml.jackson.core:jackson-databind" }
 jackson-kotlin = { module = "com.fasterxml.jackson.module:jackson-module-kotlin" }
 
 logback = "ch.qos.logback:logback-classic:1.5.6"
 
 [plugins]
 kotlin = { id = "org.jetbrains.kotlin.jvm", version.ref = "kotlin" }
```

### Comparing `bowtie_json_schema-2024.5.4/implementations/java-openapiprocessor/src/main/kotlin/Runner.kt` & `bowtie_json_schema-2024.5.5/implementations/java-openapiprocessor/src/main/kotlin/Runner.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/implementations/java-openapiprocessor/src/main/kotlin/Support.kt` & `bowtie_json_schema-2024.5.5/implementations/java-openapiprocessor/src/main/kotlin/Support.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/implementations/java-openapiprocessor/src/main/kotlin/commands/Request.kt` & `bowtie_json_schema-2024.5.5/implementations/java-openapiprocessor/src/main/kotlin/commands/Request.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/implementations/java-openapiprocessor/src/main/kotlin/commands/RunCmd.kt` & `bowtie_json_schema-2024.5.5/implementations/java-openapiprocessor/src/main/kotlin/commands/RunCmd.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/implementations/java-openapiprocessor/src/main/kotlin/commands/StartCmd.kt` & `bowtie_json_schema-2024.5.5/implementations/java-openapiprocessor/src/main/kotlin/commands/StartCmd.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/implementations/js-ajv/bowtie_ajv.js` & `bowtie_json_schema-2024.5.5/implementations/js-ajv/bowtie_ajv.js`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/implementations/js-ajv/package-lock.json` & `bowtie_json_schema-2024.5.5/implementations/js-ajv/package-lock.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/implementations/js-hyperjump/bowtie_hyperjump.js` & `bowtie_json_schema-2024.5.5/implementations/js-hyperjump/bowtie_hyperjump.js`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/implementations/js-json-schema/bowtie_json_schema.js` & `bowtie_json_schema-2024.5.5/implementations/js-json-schema/bowtie_json_schema.js`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/implementations/js-jsonschema/bowtie_jsonschema.js` & `bowtie_json_schema-2024.5.5/implementations/js-jsonschema/bowtie_jsonschema.js`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/implementations/kotlin-kmp-json-schema-validator/build.gradle.kts` & `bowtie_json_schema-2024.5.5/implementations/kotlin-kmp-json-schema-validator/build.gradle.kts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/BowtieSampsonSchemaValidatorLauncher.kt` & `bowtie_json_schema-2024.5.5/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/BowtieSampsonSchemaValidatorLauncher.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Commands.kt` & `bowtie_json_schema-2024.5.5/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Commands.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Responses.kt` & `bowtie_json_schema-2024.5.5/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Responses.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/TestFilters.kt` & `bowtie_json_schema-2024.5.5/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/TestFilters.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/implementations/lua-jsonschema/Dockerfile` & `bowtie_json_schema-2024.5.5/implementations/lua-jsonschema/Dockerfile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/implementations/lua-jsonschema/bowtie_jsonschema.lua` & `bowtie_json_schema-2024.5.5/implementations/lua-jsonschema/bowtie_jsonschema.lua`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/implementations/lua-jsonschema/json.lua` & `bowtie_json_schema-2024.5.5/implementations/lua-jsonschema/json.lua`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/implementations/php-opis-json-schema/bowtieJsonSchema.php` & `bowtie_json_schema-2024.5.5/implementations/php-opis-json-schema/bowtieJsonSchema.php`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/implementations/python-fastjsonschema/bowtie_fastjsonschema.py` & `bowtie_json_schema-2024.5.5/implementations/python-fastjsonschema/bowtie_fastjsonschema.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/implementations/python-jschon/bowtie_jschon.py` & `bowtie_json_schema-2024.5.5/implementations/python-jschon/bowtie_jschon.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/implementations/python-jsonschema/bowtie_jsonschema.py` & `bowtie_json_schema-2024.5.5/implementations/python-jsonschema/bowtie_jsonschema.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/implementations/ruby-json_schemer/bowtie_json_schemer.rb` & `bowtie_json_schema-2024.5.5/implementations/ruby-json_schemer/bowtie_json_schemer.rb`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/implementations/rust-boon/Cargo.lock` & `bowtie_json_schema-2024.5.5/implementations/rust-boon/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -300,17 +300,17 @@
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.116"
+version = "1.0.117"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3e17db7126d17feb94eb3fad46bf1a96b034e8aacbc2e775fe81505f8b0b2813"
+checksum = "455182ea6142b14f93f4bc5320a2b31c1f266b66a4a5c858b013302a5d8cbfc3"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
```

### Comparing `bowtie_json_schema-2024.5.4/implementations/rust-boon/Dockerfile` & `bowtie_json_schema-2024.5.5/implementations/rust-boon/Dockerfile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/implementations/rust-boon/src/main.rs` & `bowtie_json_schema-2024.5.5/implementations/rust-boon/src/main.rs`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/implementations/rust-jsonschema/Cargo.lock` & `bowtie_json_schema-2024.5.5/implementations/rust-jsonschema/Cargo.lock`

 * *Files 6% similar despite different names*

```diff
@@ -38,23 +38,24 @@
 checksum = "b2969dcb958b36655471fc61f7e416fa76033bdd4bfed0678d8fee1e2d07a1f0"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "anstream"
-version = "0.6.4"
+version = "0.6.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2ab91ebe16eb252986481c5b62f6098f3b698a45e34b5b98200cf20dd2484a44"
+checksum = "418c75fa768af9c03be99d17643f93f79bbba589895012a80e3452a19ddda15b"
 dependencies = [
  "anstyle",
  "anstyle-parse",
  "anstyle-query",
  "anstyle-wincon",
  "colorchoice",
+ "is_terminal_polyfill",
  "utf8parse",
 ]
 
 [[package]]
 name = "anstyle"
 version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -113,17 +114,17 @@
  "miniz_oxide",
  "object",
  "rustc-demangle",
 ]
 
 [[package]]
 name = "base64"
-version = "0.21.5"
+version = "0.22.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "35636a1494ede3b646cc98f74f8e62c773a38a659ebc777a2cf26b9b74171df9"
+checksum = "72b3254f16251a8381aa12e40e3c4d2f0199f8c6508fbecb9d91f575e0fbb8c6"
 
 [[package]]
 name = "bit-set"
 version = "0.5.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0700ddab506f33b20a03b13996eccd309a48e5ff77d0d95926aa0210fb4e95f1"
 dependencies = [
@@ -196,106 +197,82 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "clap"
-version = "4.4.7"
+version = "4.5.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ac495e00dcec98c83465d5ad66c5c4fabd652fd6686e7c6269b117e729a6f17b"
+checksum = "90bc066a67923782aa8515dbaea16946c5bcc5addbd668bb80af688e53e548a0"
 dependencies = [
  "clap_builder",
  "clap_derive",
 ]
 
 [[package]]
 name = "clap_builder"
-version = "4.4.7"
+version = "4.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c77ed9a32a62e6ca27175d00d29d05ca32e396ea1eb5fb01d8256b669cec7663"
+checksum = "ae129e2e766ae0ec03484e609954119f123cc1fe650337e155d03b022f24f7b4"
 dependencies = [
  "anstream",
  "anstyle",
  "clap_lex",
  "strsim",
 ]
 
 [[package]]
 name = "clap_derive"
-version = "4.4.7"
+version = "4.5.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cf9804afaaf59a91e75b022a30fb7229a7901f60c755489cc61c9b423b836442"
+checksum = "528131438037fd55894f62d6e9f068b8f45ac57ffa77517819645d10aed04f64"
 dependencies = [
  "heck",
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "clap_lex"
-version = "0.6.0"
+version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "702fc72eb24e5a1e48ce58027a675bc24edd52096d5397d4aea7c6dd9eca0bd1"
+checksum = "98cc8fbded0c607b7ba9dd60cd98df59af97e84d24e49c8557331cfc26d301ce"
 
 [[package]]
 name = "colorchoice"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "acbf1af155f9b9ef647e42cdc158db4b64a1b61f743629225fde6f3e0be2a7c7"
 
 [[package]]
-name = "core-foundation"
-version = "0.9.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "194a7a9e6de53fa55116934067c844d9d749312f75c6f6d0980e8c252f8c2146"
-dependencies = [
- "core-foundation-sys",
- "libc",
-]
-
-[[package]]
-name = "core-foundation-sys"
-version = "0.8.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e496a50fda8aacccc86d7529e2c1e0892dbd0f898a6b5645b5561b89c3210efa"
-
-[[package]]
 name = "deranged"
 version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0f32d04922c60427da6f9fef14d042d9edddef64cb9d4ce0d64d0685fbeb1fd3"
 dependencies = [
  "powerfmt",
 ]
 
 [[package]]
-name = "encoding_rs"
-version = "0.8.33"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7268b386296a025e474d5140678f75d6de9493ae55a5d709eeb9dd08149945e1"
-dependencies = [
- "cfg-if",
-]
-
-[[package]]
 name = "equivalent"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5443807d6dff69373d433ab9ef5378ad8df50ca6298caf15de6e52e24aaf54d5"
 
 [[package]]
 name = "fancy-regex"
-version = "0.11.0"
+version = "0.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b95f7c0680e4142284cf8b22c14a476e87d61b004a3a0861872b32ef7ead40a2"
+checksum = "531e46835a22af56d1e3b66f04844bed63158bc094a628bec1d321d9b4c44bf2"
 dependencies = [
  "bit-set",
- "regex",
+ "regex-automata",
+ "regex-syntax",
 ]
 
 [[package]]
 name = "fnv"
 version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3f9eec918d3f24069decb9af1554cad7c880e2da24a9afd88aca000531ab82c1"
@@ -307,29 +284,30 @@
 checksum = "e13624c2627564efccf4934284bdd98cbaa14e79b0b5a141218e507b3a823456"
 dependencies = [
  "percent-encoding",
 ]
 
 [[package]]
 name = "fraction"
-version = "0.13.1"
+version = "0.15.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3027ae1df8d41b4bed2241c8fdad4acc1e7af60c8e17743534b545e77182d678"
+checksum = "fac69bd85b6b19696fae3aa269c3e03c2d12e19a87f0e67f01bc1518cf0025e0"
 dependencies = [
  "lazy_static",
  "num",
 ]
 
 [[package]]
 name = "futures-channel"
 version = "0.3.29"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ff4dd66668b557604244583e3e1e1eada8c5c2e96a6d0d6653ede395b78bbacb"
 dependencies = [
  "futures-core",
+ "futures-sink",
 ]
 
 [[package]]
 name = "futures-core"
 version = "0.3.29"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "eb1d22c66e66d9d72e1758f0bd7d4fd0bee04cad842ee34587d68c07e45d088c"
@@ -356,14 +334,15 @@
 name = "futures-util"
 version = "0.3.29"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a19526d624e703a3179b3d322efec918b6246ea0fa51d41124525f00f1cc8104"
 dependencies = [
  "futures-core",
  "futures-io",
+ "futures-sink",
  "futures-task",
  "memchr",
  "pin-project-lite",
  "pin-utils",
  "slab",
 ]
 
@@ -383,106 +362,108 @@
 [[package]]
 name = "gimli"
 version = "0.28.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6fb8d784f27acf97159b40fc4db5ecd8aa23b9ad5ef69cdd136d3bc80665f0c0"
 
 [[package]]
-name = "h2"
-version = "0.3.26"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "81fe527a889e1532da5c525686d96d4c2e74cdd345badf8dfef9f6b39dd5f5e8"
-dependencies = [
- "bytes",
- "fnv",
- "futures-core",
- "futures-sink",
- "futures-util",
- "http",
- "indexmap",
- "slab",
- "tokio",
- "tokio-util",
- "tracing",
-]
-
-[[package]]
 name = "hashbrown"
 version = "0.14.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f93e7192158dbcda357bdec5fb5788eebf8bbac027f3f33e719d29135ae84156"
 
 [[package]]
 name = "heck"
-version = "0.4.1"
+version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
+checksum = "2304e00983f87ffb38b55b444b5e3b60a884b5d30c0fca7d82fe33449bbe55ea"
 
 [[package]]
 name = "hermit-abi"
 version = "0.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d77f7ec81a6d05a3abb01ab6eb7590f6083d08449fe5a1c8b1e620283546ccb7"
 
 [[package]]
 name = "http"
-version = "0.2.9"
+version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bd6effc99afb63425aff9b05836f029929e345a6148a14b7ecd5ab67af944482"
+checksum = "21b9ddb458710bc376481b842f5da65cdf31522de232c1ca8146abce2a358258"
 dependencies = [
  "bytes",
  "fnv",
  "itoa",
 ]
 
 [[package]]
 name = "http-body"
-version = "0.4.5"
+version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d5f38f16d184e36f2408a55281cd658ecbd3ca05cce6d6510a176eca393e26d1"
+checksum = "1cac85db508abc24a2e48553ba12a996e87244a0395ce011e62b37158745d643"
 dependencies = [
  "bytes",
  "http",
+]
+
+[[package]]
+name = "http-body-util"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0475f8b2ac86659c21b64320d5d653f9efe42acd2a4e560073ec61a155a34f1d"
+dependencies = [
+ "bytes",
+ "futures-core",
+ "http",
+ "http-body",
  "pin-project-lite",
 ]
 
 [[package]]
 name = "httparse"
 version = "1.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d897f394bad6a705d5f4104762e116a75639e470d80901eed05a860a95cb1904"
 
 [[package]]
-name = "httpdate"
-version = "1.0.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "df3b46402a9d5adb4c86a0cf463f42e19994e3ee891101b1841f30a545cb49a9"
-
-[[package]]
 name = "hyper"
-version = "0.14.27"
+version = "1.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ffb1cfd654a8219eaef89881fdb3bb3b1cdc5fa75ded05d6933b2b382e395468"
+checksum = "fe575dd17d0862a9a33781c8c4696a55c320909004a67a00fb286ba8b1bc496d"
 dependencies = [
  "bytes",
  "futures-channel",
- "futures-core",
  "futures-util",
- "h2",
  "http",
  "http-body",
  "httparse",
- "httpdate",
  "itoa",
  "pin-project-lite",
- "socket2 0.4.10",
+ "smallvec",
  "tokio",
+ "want",
+]
+
+[[package]]
+name = "hyper-util"
+version = "0.1.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ca38ef113da30126bbff9cd1705f9273e15d45498615d138b0c20279ac7a76aa"
+dependencies = [
+ "bytes",
+ "futures-channel",
+ "futures-util",
+ "http",
+ "http-body",
+ "hyper",
+ "pin-project-lite",
+ "socket2",
+ "tokio",
+ "tower",
  "tower-service",
  "tracing",
- "want",
 ]
 
 [[package]]
 name = "idna"
 version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "634d9b1461af396cad843f47fdba5597a4f9e6ddd4bfb6ff5d85028c25cb12f6"
@@ -504,14 +485,20 @@
 [[package]]
 name = "ipnet"
 version = "2.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f518f335dce6725a761382244631d86cf0ccb2863413590b31338feb467f9c3"
 
 [[package]]
+name = "is_terminal_polyfill"
+version = "1.70.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f8478577c03552c21db0e2724ffb8986a5ce7af88107e6be5d2ee6e158c12800"
+
+[[package]]
 name = "iso8601"
 version = "0.6.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "924e5d73ea28f59011fec52a0d12185d496a9b075d360657aed2a5707f701153"
 dependencies = [
  "nom",
 ]
@@ -529,17 +516,17 @@
 checksum = "c5f195fe497f702db0f318b07fdd68edb16955aed830df8363d837542f8f935a"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "jsonschema"
-version = "0.17.1"
+version = "0.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2a071f4f7efc9a9118dfb627a0a94ef247986e1ab8606a4c806ae2b3aa3b6978"
+checksum = "ec0afd06142c9bcb03f4a8787c77897a87b6be9c4918f1946c33caa714c27578"
 dependencies = [
  "ahash",
  "anyhow",
  "base64",
  "bytecount",
  "clap",
  "fancy-regex",
@@ -587,17 +574,17 @@
 name = "log"
 version = "0.4.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b5e6163cb8c49088c2c36f57875e58ccd8c87c7427f7fbd50ea6710b2f3f2e8f"
 
 [[package]]
 name = "memchr"
-version = "2.6.4"
+version = "2.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f665ee40bc4a3c5590afb1e9677db74a508659dfd71e126420da8274909a0167"
+checksum = "6c8640c5d730cb13ebd907d8d04b52f55ac9a2eec55b440c8892f40d56c76c1d"
 
 [[package]]
 name = "mime"
 version = "0.3.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6877bb514081ee2a7ff5ef9de3281f14a4dd4bceac4c09388074a6b5df8a139a"
 
@@ -736,17 +723,17 @@
 checksum = "9cf5f9dd3933bd50a9e1f149ec995f39ae2c496d31fd772c1fd45ebc27e902b0"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.18.0"
+version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
+checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
 
 [[package]]
 name = "os_info"
 version = "3.8.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ae99c7fa6dd38c7cafe1ec085e804f8f555a2f8659b0dbe03f1f9963a9b51092"
 dependencies = [
@@ -781,14 +768,34 @@
 [[package]]
 name = "percent-encoding"
 version = "2.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e3148f5046208a5d56bcfc03053e3ca6334e51da8dfb19b6cdc8b306fae3283e"
 
 [[package]]
+name = "pin-project"
+version = "1.1.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b6bf43b791c5b9e34c3d182969b4abb522f9343702850a2e57f460d00d09b4b3"
+dependencies = [
+ "pin-project-internal",
+]
+
+[[package]]
+name = "pin-project-internal"
+version = "1.1.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2f38a4412a78282e09a2cf38d195ea5420d15ba0602cb375210efbc877243965"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn",
+]
+
+[[package]]
 name = "pin-project-lite"
 version = "0.2.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8afb450f006bf6385ca15ef45d71d2288452bc3683ce2e2cacc0d18e4be60b58"
 
 [[package]]
 name = "pin-utils"
@@ -856,38 +863,39 @@
 name = "regex-syntax"
 version = "0.8.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c08c74e62047bb2de4ff487b251e4a92e24f48745648451635cec7d591162d9f"
 
 [[package]]
 name = "reqwest"
-version = "0.11.22"
+version = "0.12.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "046cd98826c46c2ac8ddecae268eb5c2e58628688a5fc7a2643704a73faba95b"
+checksum = "566cafdd92868e0939d3fb961bd0dc25fcfaaed179291093b3d43e6b3150ea10"
 dependencies = [
  "base64",
  "bytes",
- "encoding_rs",
+ "futures-channel",
  "futures-core",
  "futures-util",
- "h2",
  "http",
  "http-body",
+ "http-body-util",
  "hyper",
+ "hyper-util",
  "ipnet",
  "js-sys",
  "log",
  "mime",
  "once_cell",
  "percent-encoding",
  "pin-project-lite",
  "serde",
  "serde_json",
  "serde_urlencoded",
- "system-configuration",
+ "sync_wrapper",
  "tokio",
  "tower-service",
  "url",
  "wasm-bindgen",
  "wasm-bindgen-futures",
  "web-sys",
  "winreg",
@@ -937,37 +945,37 @@
 checksum = "836fa6a3e1e547f9a2c4040802ec865b5d85f4014efe00555d7090a3dcaa1090"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "serde"
-version = "1.0.200"
+version = "1.0.201"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ddc6f9cc94d67c0e21aaf7eda3a010fd3af78ebf6e096aa6e2e13c79749cce4f"
+checksum = "780f1cebed1629e4753a1a38a3c72d30b97ec044f0aef68cb26650a3c5cf363c"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.200"
+version = "1.0.201"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "856f046b9400cee3c8c94ed572ecdb752444c24528c035cd35882aad6f492bcb"
+checksum = "c5e405930b9796f1c00bee880d03fc7e0bb4b9a11afc776885ffe84320da2865"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.116"
+version = "1.0.117"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3e17db7126d17feb94eb3fad46bf1a96b034e8aacbc2e775fe81505f8b0b2813"
+checksum = "455182ea6142b14f93f4bc5320a2b31c1f266b66a4a5c858b013302a5d8cbfc3"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -998,75 +1006,50 @@
 checksum = "8f92a496fb766b417c996b9c5e57daf2f7ad3b0bebe1ccfca4856390e3d3bb67"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "smallvec"
-version = "1.11.1"
+version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "942b4a808e05215192e39f4ab80813e599068285906cc91aa64f923db842bd5a"
-
-[[package]]
-name = "socket2"
-version = "0.4.10"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9f7916fc008ca5542385b89a3d3ce689953c143e9304a9bf8beec1de48994c0d"
-dependencies = [
- "libc",
- "winapi",
-]
+checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "socket2"
 version = "0.5.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7b5fac59a5cb5dd637972e5fca70daf0523c9067fcdc4842f053dae04a18f8e9"
 dependencies = [
  "libc",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "strsim"
-version = "0.10.0"
+version = "0.11.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "73473c0e59e6d5812c5dfe2a064a6444949f089e20eec9a2e5506596494e4623"
+checksum = "7da8b5736845d9f2fcb837ea5d9e2628564b3b043a70948a3f0b778838c5fb4f"
 
 [[package]]
 name = "syn"
 version = "2.0.46"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "89456b690ff72fddcecf231caedbe615c59480c93358a93dfae7fc29e3ebbf0e"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
-name = "system-configuration"
-version = "0.5.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ba3a3adc5c275d719af8cb4272ea1c4a6d668a777f37e115f6d11ddbc1c8e0e7"
-dependencies = [
- "bitflags",
- "core-foundation",
- "system-configuration-sys",
-]
-
-[[package]]
-name = "system-configuration-sys"
-version = "0.5.0"
+name = "sync_wrapper"
+version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a75fb188eb626b924683e3b95e3a48e63551fcfb51949de2f06a9d91dbee93c9"
-dependencies = [
- "core-foundation-sys",
- "libc",
-]
+checksum = "2047c6ded9c721764247e62cd3b03c09ffc529b2ba5b10ec482ae507a4a70160"
 
 [[package]]
 name = "time"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c4a34ab300f2dee6e562c10a046fc05e358b29f9bf92277f30c3c8d82275f6f5"
 dependencies = [
@@ -1110,38 +1093,23 @@
 [[package]]
 name = "tokio"
 version = "1.33.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4f38200e3ef7995e5ef13baec2f432a6da0aa9ac495b2c0e8f3b7eec2c92d653"
 dependencies = [
  "backtrace",
- "bytes",
  "libc",
  "mio",
  "num_cpus",
  "pin-project-lite",
- "socket2 0.5.5",
+ "socket2",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
-name = "tokio-util"
-version = "0.7.10"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5419f34732d9eb6ee4c3578b7989078579b7f039cbbb9ca2c4da015749371e15"
-dependencies = [
- "bytes",
- "futures-core",
- "futures-sink",
- "pin-project-lite",
- "tokio",
- "tracing",
-]
-
-[[package]]
 name = "toml"
 version = "0.7.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dd79e69d3b627db300ff956027cc6c3798cef26d22526befdfcd12feeb6d2257"
 dependencies = [
  "serde",
  "serde_spanned",
@@ -1168,25 +1136,48 @@
  "serde",
  "serde_spanned",
  "toml_datetime",
  "winnow",
 ]
 
 [[package]]
+name = "tower"
+version = "0.4.13"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b8fa9be0de6cf49e536ce1851f987bd21a43b771b09473c3549a6c853db37c1c"
+dependencies = [
+ "futures-core",
+ "futures-util",
+ "pin-project",
+ "pin-project-lite",
+ "tokio",
+ "tower-layer",
+ "tower-service",
+ "tracing",
+]
+
+[[package]]
+name = "tower-layer"
+version = "0.3.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c20c8dbed6283a09604c3e69b4b7eeb54e298b8a600d4d5ecb5ad39de609f1d0"
+
+[[package]]
 name = "tower-service"
 version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b6bc1c9ce2b5135ac7f93c72918fc37feb872bdc6a5533a8b85eb4b86bfdae52"
 
 [[package]]
 name = "tracing"
 version = "0.1.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c3523ab5a71916ccf420eebdf5521fcef02141234bbc0b8a49f2fdc4544364ef"
 dependencies = [
+ "log",
  "pin-project-lite",
  "tracing-core",
 ]
 
 [[package]]
 name = "tracing-core"
 version = "0.1.32"
@@ -1340,36 +1331,14 @@
 checksum = "9b85cbef8c220a6abc02aefd892dfc0fc23afb1c6a426316ec33253a3877249b"
 dependencies = [
  "js-sys",
  "wasm-bindgen",
 ]
 
 [[package]]
-name = "winapi"
-version = "0.3.9"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5c839a674fcd7a98952e593242ea400abe93992746761e38641405d28b00f419"
-dependencies = [
- "winapi-i686-pc-windows-gnu",
- "winapi-x86_64-pc-windows-gnu",
-]
-
-[[package]]
-name = "winapi-i686-pc-windows-gnu"
-version = "0.4.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ac3b87c63620426dd9b991e5ce0329eff545bccbbb34f3be09ff6fb6ab51b7b6"
-
-[[package]]
-name = "winapi-x86_64-pc-windows-gnu"
-version = "0.4.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
-
-[[package]]
 name = "windows-sys"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
 dependencies = [
  "windows-targets 0.48.5",
 ]
@@ -1504,17 +1473,17 @@
 checksum = "176b6138793677221d420fd2f0aeeced263f197688b36484660da767bca2fa32"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "winreg"
-version = "0.50.0"
+version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "524e57b2c537c0f9b1e69f1965311ec12182b4122e45035b1508cd24d2adadb1"
+checksum = "a277a57398d4bfa075df44f501a17cfdf8542d224f0d36095a2adc7aee4ef0a5"
 dependencies = [
  "cfg-if",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "zerocopy"
```

### Comparing `bowtie_json_schema-2024.5.4/implementations/rust-jsonschema/Dockerfile` & `bowtie_json_schema-2024.5.5/implementations/rust-jsonschema/Dockerfile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/implementations/rust-jsonschema/src/main.rs` & `bowtie_json_schema-2024.5.5/implementations/rust-jsonschema/src/main.rs`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/implementations/scala-mjs-validator/Harness.scala` & `bowtie_json_schema-2024.5.5/implementations/scala-mjs-validator/Harness.scala`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/implementations/scala-mjs-validator/build.sbt` & `bowtie_json_schema-2024.5.5/implementations/scala-mjs-validator/build.sbt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/implementations/scala-rc-circe-json-validator/Harness.scala` & `bowtie_json_schema-2024.5.5/implementations/scala-rc-circe-json-validator/Harness.scala`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/implementations/scala-rc-circe-json-validator/build.sbt` & `bowtie_json_schema-2024.5.5/implementations/scala-rc-circe-json-validator/build.sbt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/implementations/ts-vscode-json-languageservice/bowtie_jsonls.ts` & `bowtie_json_schema-2024.5.5/implementations/ts-vscode-json-languageservice/bowtie_jsonls.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/tests/test_github.py` & `bowtie_json_schema-2024.5.5/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/tests/test_hypothesis.py` & `bowtie_json_schema-2024.5.5/tests/test_hypothesis.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/tests/test_integration.py` & `bowtie_json_schema-2024.5.5/tests/test_integration.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from aiodocker.exceptions import DockerError
 from markdown_it import MarkdownIt
 from markdown_it.tree import SyntaxTreeNode
 import pexpect
 import pytest
 import pytest_asyncio
 
+from bowtie._cli import EX
 from bowtie._commands import ErroredTest, TestResult
 from bowtie._core import (
     Dialect,
     Implementation,
     Test,
     TestCase,
     validator_registry,
@@ -44,15 +45,15 @@
 
 async def command_validator(command):
     stdout, stderr = await bowtie(command, "--schema")
     assert stderr == "", stderr
     return validator_registry().for_schema(_json.loads(stdout))
 
 
-async def bowtie(*argv, stdin: str = "", exit_code=0, json=False):
+async def bowtie(*argv, stdin: str = "", exit_code=EX.OK, json=False):
     """
     Run a Bowtie subprocess asynchronously to completion.
 
     An exit code of `-1` means "any non-zero exit code".
     """
     process = await asyncio.create_subprocess_exec(
         sys.executable,
@@ -474,30 +475,30 @@
     assert results == [
         {tag("envsonschema"): TestResult.VALID},
     ], stderr
 
 
 @pytest.mark.asyncio
 async def test_no_tests_run(envsonschema):
-    async with run("-i", envsonschema, exit_code=os.EX_NOINPUT) as send:
+    async with run("-i", envsonschema, exit_code=EX.NOINPUT) as send:
         results, stderr = await send("")
 
     assert results == []
     assert stderr != ""
 
 
 @pytest.mark.asyncio
 async def test_unknown_dialect(envsonschema):
     dialect = "some://other/URI/"
     async with run(
         "-i",
         envsonschema,
         "--dialect",
         dialect,
-        exit_code=-1,
+        exit_code=2,  # comes from click
     ) as send:
         results, stderr = await send("")
 
     assert results == []
     assert "not a known dialect" in stderr, stderr
 
 
@@ -505,30 +506,30 @@
 async def test_nonurl_dialect(envsonschema):
     dialect = ";;;;;"
     async with run(
         "-i",
         envsonschema,
         "--dialect",
         dialect,
-        exit_code=-1,
+        exit_code=2,  # comes from click
     ) as send:
         results, stderr = await send("")
 
     assert results == []
     assert "not a known dialect" in stderr, stderr
 
 
 @pytest.mark.asyncio
 async def test_unsupported_known_dialect(only_draft3):
     async with run(
         "-i",
         only_draft3,
         "--dialect",
         str(Dialect.by_alias()["draft2020-12"].uri),
-        exit_code=-1,
+        exit_code=EX.CONFIG,
     ) as send:
         results, stderr = await send("")
 
     assert results == []
     assert "does not support" in stderr, stderr
 
 
@@ -558,15 +559,15 @@
 @pytest.mark.asyncio
 async def test_handles_dead_implementations(succeed_immediately, envsonschema):
     async with run(
         "-i",
         succeed_immediately,
         "-i",
         envsonschema,
-        exit_code=-1,
+        exit_code=EX.CONFIG,
     ) as send:
         results, stderr = await send(
             """
             {"description": "1", "schema": {}, "tests": [{"description": "foo", "instance": {}}] }
             {"description": "2", "schema": {}, "tests": [{"description": "bar", "instance": {}}] }
             """,  # noqa: E501
         )
@@ -579,15 +580,15 @@
 
 
 @pytest.mark.asyncio
 async def test_it_exits_when_no_implementations_succeed(succeed_immediately):
     """
     Don't uselessly "run" tests on no implementations.
     """
-    async with run("-i", succeed_immediately, exit_code=-1) as send:
+    async with run("-i", succeed_immediately, exit_code=EX.CONFIG) as send:
         results, stderr = await send(
             """
             {"description": "1", "schema": {}, "tests": [{"description": "foo", "instance": {}}] }
             {"description": "2", "schema": {}, "tests": [{"description": "bar", "instance": {}}] }
             {"description": "3", "schema": {}, "tests": [{"description": "bar", "instance": {}}] }
             """,  # noqa: E501
         )
@@ -602,15 +603,15 @@
     envsonschema,
 ):
     async with run(
         "-i",
         fail_immediately,
         "-i",
         envsonschema,
-        exit_code=-1,
+        exit_code=EX.CONFIG,
     ) as send:
         results, stderr = await send(
             """
             {"description": "1", "schema": {}, "tests": [{"description": "foo", "instance": {}}] }
             {"description": "2", "schema": {}, "tests": [{"description": "bar", "instance": {}}] }
             """,  # noqa: E501
         )
@@ -629,15 +630,15 @@
     envsonschema,
 ):
     async with run(
         "-i",
         fail_on_start,
         "-i",
         envsonschema,
-        exit_code=-1,
+        exit_code=EX.CONFIG,
     ) as send:
         results, stderr = await send(
             """
             {"description": "1", "schema": {}, "tests": [{"description": "foo", "instance": {}}] }
             {"description": "2", "schema": {}, "tests": [{"description": "bar", "instance": {}}] }
             """,  # noqa: E501
         )
@@ -653,15 +654,15 @@
 @pytest.mark.asyncio
 async def test_it_handles_broken_dialect_implementations(fail_on_dialect):
     async with run(
         "-i",
         fail_on_dialect,
         "--dialect",
         "http://json-schema.org/draft-07/schema#",
-        exit_code=-1,
+        exit_code=EX.CONFIG,
     ) as send:
         results, stderr = await send(
             """
             {"description": "1", "schema": {}, "tests": [{"description": "foo", "instance": {}}] }
             """,  # noqa: E501
         )
 
@@ -755,15 +756,15 @@
         {tag("envsonschema"): TestResult.VALID},
         {tag("envsonschema"): TestResult.INVALID},
     ], stderr
 
 
 @pytest.mark.asyncio
 async def test_it_handles_invalid_start_responses(missing_homepage):
-    async with run("-i", missing_homepage, "-V", exit_code=-1) as send:
+    async with run("-i", missing_homepage, "-V", exit_code=EX.CONFIG) as send:
         results, stderr = await send(
             """
             {"description": "1", "schema": {}, "tests": [{"description": "foo", "instance": {}}] }
             """,  # noqa: E501
         )
 
     assert "failed to start" in stderr, stderr
@@ -819,15 +820,15 @@
     An implementation speaking the wrong version of the protocol is skipped.
     """
     async with run(
         "-i",
         wrong_version,
         "--dialect",
         "http://json-schema.org/draft-07/schema#",
-        exit_code=-1,
+        exit_code=1,  # FIXME: We're emitting the traceback
     ) as send:
         results, stderr = await send(
             """
             {"description": "1", "schema": {}, "tests": [{"description": "valid:1", "instance": {}, "valid": true}] }
             """,  # noqa: E501
         )
 
@@ -923,27 +924,27 @@
     stdout, stderr = await bowtie(
         "run",
         "-i",
         envsonschema,
         "--max-fail",
         "2",
         "--fail-fast",
-        exit_code=-1,
+        exit_code=2,  # comes from click
     )
     assert stdout == ""
     assert "don't provide both" in stderr, stderr
 
     stdout, stderr = await bowtie(
         "run",
         "-i",
         envsonschema,
         "--fail-fast",
         "--max-fail",
         "2",
-        exit_code=-1,
+        exit_code=2,  # comes from click
     )
     assert stdout == ""
     assert "don't provide both" in stderr, stderr
 
 
 @pytest.mark.asyncio
 async def test_filter(envsonschema):
@@ -966,15 +967,15 @@
 async def test_smoke_pretty(envsonschema):
     stdout, stderr = await bowtie(
         "smoke",
         "--format",
         "pretty",
         "-i",
         envsonschema,
-        exit_code=-1,  # because indeed envsonschema gets answers wrong.
+        exit_code=EX.DATAERR,  # because indeed envsonschema gets answers wrong
     )
     assert (
         dedent(stdout)
         == dedent(
             """
             · allow-everything: ✗✗✗✗✗✗
             · allow-nothing: ✓✓✓✓✓✓
@@ -987,15 +988,15 @@
 async def test_smoke_markdown(envsonschema):
     stdout, stderr = await bowtie(
         "smoke",
         "--format",
         "markdown",
         "-i",
         envsonschema,
-        exit_code=-1,  # because indeed envsonschema gets answers wrong.
+        exit_code=EX.DATAERR,  # because indeed envsonschema gets answers wrong
     )
     assert (
         dedent(stdout)
         == dedent(
             """
             * allow-everything: ✗✗✗✗✗✗
             * allow-nothing: ✓✓✓✓✓✓
@@ -1008,15 +1009,15 @@
 async def test_smoke_valid_markdown(envsonschema):
     stdout, stderr = await bowtie(
         "smoke",
         "--format",
         "markdown",
         "-i",
         envsonschema,
-        exit_code=-1,  # because indeed envsonschema gets answers wrong.
+        exit_code=EX.DATAERR,  # because indeed envsonschema gets answers wrong
     )
     parsed_markdown = MarkdownIt("gfm-like", {"linkify": False}).parse(stdout)
     tokens = SyntaxTreeNode(parsed_markdown).pretty(indent=2)
     assert (
         tokens
         == """
         <root>
@@ -1039,15 +1040,15 @@
     jsonout, stderr = await bowtie(
         "smoke",
         "--format",
         "json",
         "-i",
         envsonschema,
         json=True,
-        exit_code=-1,  # because indeed envsonschema gets answers wrong.
+        exit_code=EX.DATAERR,  # because indeed envsonschema gets answers wrong
     )
 
     (await command_validator("smoke")).validate(jsonout)
     assert jsonout == [
         {
             "case": {
                 "description": "allow-everything",
@@ -1107,30 +1108,30 @@
 @pytest.mark.asyncio
 async def test_smoke_quiet(envsonschema):
     stdout, stderr = await bowtie(
         "smoke",
         "--quiet",
         "-i",
         envsonschema,
-        exit_code=-1,  # because indeed envsonschema gets answers wrong.
+        exit_code=EX.DATAERR,  # because indeed envsonschema gets answers wrong
     )
     assert stdout == "", stderr
 
 
 @pytest.mark.asyncio
 async def test_smoke_multiple(envsonschema, passes_smoke):
     stdout, stderr = await bowtie(
         "smoke",
         "--format",
         "pretty",
         "-i",
         envsonschema,
         "-i",
         passes_smoke,
-        exit_code=-1,  # because indeed envsonschema gets answers wrong.
+        exit_code=EX.DATAERR,  # because indeed envsonschema gets answers wrong
     )
     assert (
         dedent(stderr)
         == dedent(
             """\
             Testing 'bowtie-integration-tests/passes_smoke'...
 
@@ -1397,15 +1398,15 @@
 
 @pytest.mark.asyncio
 async def test_info_unsuccessful_start(succeed_immediately):
     stdout, stderr = await bowtie(
         "info",
         "-i",
         succeed_immediately,
-        exit_code=-1,
+        exit_code=EX.CONFIG,
     )
 
     assert stdout.strip() in {"", "{}"}  # empty, but ignore if JSON or not
     assert "failed to start" in stderr, stderr
 
 
 @pytest.mark.asyncio
@@ -1564,15 +1565,15 @@
 @pytest.mark.asyncio
 async def test_filter_dialects_no_results(only_draft3):
     stdout, stderr = await bowtie(
         "filter-dialects",
         "-i",
         only_draft3,
         "--boolean-schemas",
-        exit_code=-1,
+        exit_code=EX.DATAERR,
     )
     assert (stdout.strip(), stderr) == ("", "No dialects match.\n")
 
 
 @pytest.mark.asyncio
 async def test_validate(envsonschema, tmp_path):
     tmp_path.joinpath("schema.json").write_text("{}")
@@ -1753,15 +1754,15 @@
     schema = tmp_path / "schema.json"
     schema.write_text("{}")
     stdout, stderr = await bowtie(
         "validate",
         "-i",
         envsonschema,
         schema,
-        exit_code=-1,
+        exit_code=EX.NOINPUT,
     )
     assert stdout == ""
     assert stderr == ""
 
 
 @pytest.mark.asyncio
 @pytest.mark.json
@@ -1952,15 +1953,15 @@
     )
 
     badges = tmp_path / "badges"
     stdout, stderr = await bowtie(
         "badges",
         badges,
         stdin=run_stdout,
-        exit_code=-1,
+        exit_code=2,  # comes from click
     )
     assert stdout == ""
     assert stderr != ""
     assert not badges.is_dir()
 
 
 @pytest.mark.asyncio
@@ -2003,55 +2004,55 @@
 
 @pytest.mark.asyncio
 async def test_no_such_image(tmp_path):
     stdout, stderr = await bowtie(
         "run",
         "-i",
         "no-such-image",
-        exit_code=-1,
+        exit_code=EX.CONFIG,
     )
     assert stdout == ""
     assert (
         "'ghcr.io/bowtie-json-schema/no-such-image' is not a known " in stderr
     ), stderr
 
     stdout, stderr = await bowtie(
         "smoke",
         "-i",
         "no-such-image",
-        exit_code=-1,
+        exit_code=EX.CONFIG,
     )
     assert "/no-such-image' is not a known" in stderr, stderr
 
     foo = tmp_path / "foo.json"
     foo.write_text("{}")
 
     stdout, stderr = await bowtie(
         "validate",
         "-i",
         "no-such-image",
         "-",
         foo,
         stdin="{}",
-        exit_code=-1,
+        exit_code=EX.CONFIG,
     )
     assert stdout == ""
     assert (
         "'ghcr.io/bowtie-json-schema/no-such-image' is not a known " in stderr
     ), stderr
 
 
 @pytest.mark.asyncio
 async def test_suite_not_a_suite_directory(envsonschema, tmp_path):
     _, stderr = await bowtie(
         "suite",
         "-i",
         envsonschema,
         tmp_path,
-        exit_code=-1,
+        exit_code=2,  # comes from click
     )
     assert "does not contain" in stderr, stderr
 
 
 @pytest.mark.asyncio
 async def test_validate_mismatched_dialect(envsonschema, tmp_path):
     tmp_path.joinpath("schema.json").write_text(
```

### Comparing `bowtie_json_schema-2024.5.4/tests/test_report.py` & `bowtie_json_schema-2024.5.5/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/tests/test_schemas.py` & `bowtie_json_schema-2024.5.5/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/tests/fauxmplementations/envsonschema/envsonschema` & `bowtie_json_schema-2024.5.5/tests/fauxmplementations/envsonschema/envsonschema`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/tests/fauxmplementations/lintsonschema/lintsonschema` & `bowtie_json_schema-2024.5.5/tests/fauxmplementations/lintsonschema/lintsonschema`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/tests/fauxmplementations/lintsonschema/schemas/report.json` & `bowtie_json_schema-2024.5.5/tests/fauxmplementations/lintsonschema/schemas/report.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/tests/fauxmplementations/lintsonschema/schemas/cli/info.json` & `bowtie_json_schema-2024.5.5/tests/fauxmplementations/lintsonschema/schemas/cli/info.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/tests/fauxmplementations/lintsonschema/schemas/cli/summary.json` & `bowtie_json_schema-2024.5.5/tests/fauxmplementations/lintsonschema/schemas/cli/summary.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/tests/fauxmplementations/lintsonschema/schemas/io/v1.json` & `bowtie_json_schema-2024.5.5/tests/fauxmplementations/lintsonschema/schemas/io/v1.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/tests/fauxmplementations/lintsonschema/schemas/io/commands/dialect.json` & `bowtie_json_schema-2024.5.5/tests/fauxmplementations/lintsonschema/schemas/io/commands/dialect.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/tests/fauxmplementations/lintsonschema/schemas/io/commands/run.json` & `bowtie_json_schema-2024.5.5/tests/fauxmplementations/lintsonschema/schemas/io/commands/run.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/tests/fauxmplementations/lintsonschema/schemas/io/commands/start.json` & `bowtie_json_schema-2024.5.5/tests/fauxmplementations/lintsonschema/schemas/io/commands/start.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/tests/fauxmplementations/lintsonschema/schemas/models/dialect.json` & `bowtie_json_schema-2024.5.5/tests/fauxmplementations/lintsonschema/schemas/models/dialect.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/tests/fauxmplementations/lintsonschema/schemas/models/group.json` & `bowtie_json_schema-2024.5.5/tests/fauxmplementations/lintsonschema/schemas/models/group.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/tests/fauxmplementations/lintsonschema/schemas/models/implementation.json` & `bowtie_json_schema-2024.5.5/tests/fauxmplementations/lintsonschema/schemas/models/implementation.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/tests/fauxmplementations/lintsonschema/schemas/models/test.json` & `bowtie_json_schema-2024.5.5/tests/fauxmplementations/lintsonschema/schemas/models/test.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/.gitignore` & `bowtie_json_schema-2024.5.5/.gitignore`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/LICENSE` & `bowtie_json_schema-2024.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/README.rst` & `bowtie_json_schema-2024.5.5/README.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/hatch_build.py` & `bowtie_json_schema-2024.5.5/hatch_build.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/pyproject.toml` & `bowtie_json_schema-2024.5.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.4/PKG-INFO` & `bowtie_json_schema-2024.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bowtie-json-schema
-Version: 2024.5.4
+Version: 2024.5.5
 Summary: A meta-validator for the JSON Schema specification.
 Project-URL: Documentation, https://docs.bowtie.report/
 Project-URL: Homepage, https://bowtie.report/
 Project-URL: Issues, https://github.com/bowtie-json-schema/bowtie/issues/
 Project-URL: Funding, https://github.com/sponsors/Julian
 Project-URL: Source, https://github.com/bowtie-json-schema/bowtie
 Author-email: Julian Berman <Julian+bowtie@GrayVines.com>
```

