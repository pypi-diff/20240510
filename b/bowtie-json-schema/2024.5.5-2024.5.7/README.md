# Comparing `tmp/bowtie_json_schema-2024.5.5.tar.gz` & `tmp/bowtie_json_schema-2024.5.7.tar.gz`

## Comparing `bowtie_json_schema-2024.5.5.tar` & `bowtie_json_schema-2024.5.7.tar`

### file list

```diff
@@ -1,261 +1,261 @@
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/.gitpod.Dockerfile
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/.gitpod.yml
--rw-r--r--   0        0        0     3928 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/.prettierrc.json
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/.readthedocs.yaml
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/CONTRIBUTING.rst
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/action.yml
--rw-r--r--   0        0        0    12706 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/noxfile.py
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/requirements.txt
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/test-requirements.in
--rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/test-requirements.txt
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/.devcontainer/devcontainer.json
--rwxr-xr-x   0        0        0     2229 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/.pre-commit-hooks/check-dependabot
--rwxr-xr-x   0        0        0     1267 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/.pre-commit-hooks/check-lintsonschema-schema
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/bowtie/__init__.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/bowtie/__main__.py
--rw-r--r--   0        0        0    48283 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/bowtie/_cli.py
--rw-r--r--   0        0        0    12066 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/bowtie/_commands.py
--rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/bowtie/_connectables.py
--rw-r--r--   0        0        0    11145 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/bowtie/_containers.py
--rw-r--r--   0        0        0    22876 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/bowtie/_core.py
--rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/bowtie/_registry.py
--rw-r--r--   0        0        0    11625 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/bowtie/_report.py
--rw-r--r--   0        0        0     7661 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/bowtie/_suite.py
--rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/bowtie/exceptions.py
--rw-r--r--   0        0        0     9707 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/bowtie/hypothesis.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/bowtie/py.typed
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/bowtie/schemas/connectables.json
--rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/bowtie/schemas/report.json
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/bowtie/schemas/cli/info.json
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/bowtie/schemas/cli/smoke.json
--rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/bowtie/schemas/cli/summary.json
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/bowtie/schemas/io/v1.json
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/bowtie/schemas/io/commands/dialect.json
--rw-r--r--   0        0        0     3796 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/bowtie/schemas/io/commands/run.json
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/bowtie/schemas/io/commands/start.json
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/bowtie/schemas/io/commands/stop.json
--rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/bowtie/schemas/models/dialect.json
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/bowtie/schemas/models/group.json
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/bowtie/schemas/models/implementation-id.json
--rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/bowtie/schemas/models/implementation.json
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/bowtie/schemas/models/registry.json
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/bowtie/schemas/models/test.json
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/data/dialects.json
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/docs/Makefile
--rw-r--r--   0        0        0     8253 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/docs/cli.rst
--rw-r--r--   0        0        0     4100 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/docs/conf.py
--rw-r--r--   0        0        0     8235 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/docs/contributing.rst
--rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/docs/github-actions.rst
--rw-r--r--   0        0        0    36467 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/docs/implementers.rst
--rw-r--r--   0        0        0     3256 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/docs/index.rst
--rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/docs/motd.txt
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/docs/requirements.in
--rw-r--r--   0        0        0     3713 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/docs/requirements.txt
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/docs/spelling-wordlist.txt
--rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/docs/_static/bowtie_diagram_dark.svg
--rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/docs/_static/bowtie_diagram_light.svg
--rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/docs/_static/logo.svg
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/index.html
--rw-r--r--   0        0        0     2541 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/package.json
--rw-r--r--   0        0        0   163423 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/pnpm-lock.yaml
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/tsconfig.json
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/vite.config.ts
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/public/favicon.svg
--rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/DialectReportView.tsx
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/MainContainer.tsx
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/ReportDataHandler.tsx
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/global.css
--rw-r--r--   0        0        0     3366 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/index.tsx
--rw-r--r--   0        0        0     2451 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/assets/landscape-logo.svg
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/components/CopyToClipboard.tsx
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/components/FilterSection.css
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/components/FilterSection.tsx
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/components/LoadingAnimation.tsx
--rw-r--r--   0        0        0     5644 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/components/NavBar.tsx
--rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/components/OtherImplementations.tsx
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/components/BowtieInfo/BowtieInfoSection.tsx
--rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/components/Cases/CaseItem.tsx
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/components/Cases/CaseResultSvg.test.tsx
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/components/Cases/CaseResultSvg.tsx
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/components/Cases/CasesSection.tsx
--rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/components/Cases/SchemaDisplay.tsx
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/components/DragAndDrop/DragAndDrop.css
--rw-r--r--   0        0        0     4907 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/components/DragAndDrop/DragAndDrop.tsx
--rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/components/ImplementationReportView/DialectCompliance.tsx
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/components/ImplementationReportView/EmbedBadges.css
--rw-r--r--   0        0        0     6071 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/components/ImplementationReportView/EmbedBadges.tsx
--rw-r--r--   0        0        0     4815 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/components/ImplementationReportView/ImplementationReportView.tsx
--rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/components/Modals/DetailsButtonModal.tsx
--rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/components/RunInfo/RunInfoSection.tsx
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/components/Summary/ImplementationRow.css
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/components/Summary/ImplementationRow.tsx
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/components/Summary/SummarySection.tsx
--rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/components/Summary/SummaryTable.tsx
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/context/BowtieVersionContext.tsx
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/context/ThemeContext.tsx
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/data/Badge.test.ts
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/data/Badge.ts
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/data/Dialect.test.ts
--rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/data/Dialect.ts
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/data/Site.test.ts
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/data/Site.ts
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/data/mapLanguage.ts
--rw-r--r--   0        0        0     8855 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/data/parseReportData.test.ts
--rw-r--r--   0        0        0     9164 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/data/parseReportData.ts
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/frontend/src/hooks/useSearchParams.ts
--rw-r--r--   0        0        0    21214 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/.java-implementations-pmd-ruleset.xml
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/clojure-json-schema/Dockerfile
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/clojure-json-schema/project.clj
--rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/clojure-json-schema/src/bowtie_json_schema/core.clj
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/cpp-valijson/.dockerignore
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/cpp-valijson/.gitignore
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/cpp-valijson/Dockerfile
--rw-r--r--   0        0        0     5406 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/cpp-valijson/bowtie_valijson.cpp
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/cpp-valijson/compile_flags.txt
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/dotnet-jsonschema-net/.clang-format
--rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/dotnet-jsonschema-net/.gitignore
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/dotnet-jsonschema-net/Dockerfile
--rw-r--r--   0        0        0     7121 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/dotnet-jsonschema-net/Program.cs
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/dotnet-jsonschema-net/bowtie_json_everything.csproj
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/dotnet-jsonschema-net/Properties/launchSettings.json
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/go-gojsonschema/Dockerfile
--rw-r--r--   0        0        0     4681 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/go-gojsonschema/bowtie_gojsonschema.go
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/go-gojsonschema/go.mod
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/go-gojsonschema/go.sum
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/go-jsonschema/Dockerfile
--rw-r--r--   0        0        0     4958 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/go-jsonschema/bowtie_jsonschema.go
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/go-jsonschema/go.mod
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/go-jsonschema/go.sum
--rw-r--r--   0        0        0     8804 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/java-json-schema/BowtieJsonSchema.java
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/java-json-schema/Dockerfile
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/java-json-schema/build.gradle
--rw-r--r--   0        0        0     7843 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/java-json-tools-json-schema-validator/BowtieJsonSchemaValidator.java
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/java-json-tools-json-schema-validator/Dockerfile
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/java-json-tools-json-schema-validator/build.gradle
--rw-r--r--   0        0        0     7844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/java-jsonschemafriend/BowtieJsonSchemaFriend.java
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/java-jsonschemafriend/Dockerfile
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/java-jsonschemafriend/build.gradle
--rw-r--r--   0        0        0     9453 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/java-networknt-json-schema-validator/BowtieJsonSchemaValidator.java
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/java-networknt-json-schema-validator/Dockerfile
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/java-networknt-json-schema-validator/build.gradle
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/java-openapiprocessor/.dockerignore
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/java-openapiprocessor/.editorconfig
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/java-openapiprocessor/Dockerfile
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/java-openapiprocessor/build.gradle.kts
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/java-openapiprocessor/gradle.properties
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/java-openapiprocessor/justfile
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/java-openapiprocessor/settings.gradle.kts
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/java-openapiprocessor/gradle/libs.versions.toml
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/java-openapiprocessor/src/main/kotlin/Main.kt
--rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/java-openapiprocessor/src/main/kotlin/Runner.kt
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/java-openapiprocessor/src/main/kotlin/Support.kt
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/java-openapiprocessor/src/main/kotlin/commands/Configuration.kt
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/java-openapiprocessor/src/main/kotlin/commands/Dialect.kt
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/java-openapiprocessor/src/main/kotlin/commands/Request.kt
--rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/java-openapiprocessor/src/main/kotlin/commands/RunCmd.kt
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/java-openapiprocessor/src/main/kotlin/commands/StartCmd.kt
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/java-openapiprocessor/src/main/kotlin/commands/StopCmd.kt
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/js-ajv/Dockerfile
--rw-r--r--   0        0        0     2990 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/js-ajv/bowtie_ajv.js
--rw-r--r--   0        0        0     4870 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/js-ajv/package-lock.json
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/js-ajv/package.json
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/js-hyperjump/Dockerfile
--rw-r--r--   0        0        0     5711 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/js-hyperjump/bowtie_hyperjump.js
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/js-hyperjump/package.json
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/js-json-schema/Dockerfile
--rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/js-json-schema/bowtie_json_schema.js
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/js-json-schema/package.json
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/js-jsonschema/Dockerfile
--rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/js-jsonschema/bowtie_jsonschema.js
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/js-jsonschema/package.json
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/kotlin-kmp-json-schema-validator/.gitignore
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/kotlin-kmp-json-schema-validator/Dockerfile
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/kotlin-kmp-json-schema-validator/build.gradle.kts
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/kotlin-kmp-json-schema-validator/settings.gradle.kts
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/kotlin-kmp-json-schema-validator/gradle/libs.versions.toml
--rw-r--r--   0        0        0     7879 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/BowtieSampsonSchemaValidatorLauncher.kt
--rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Commands.kt
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Responses.kt
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/TestFilters.kt
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/lua-jsonschema/Dockerfile
--rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/lua-jsonschema/bowtie_jsonschema.lua
--rw-r--r--   0        0        0     9638 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/lua-jsonschema/json.lua
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/lua-jsonschema/stylua.toml
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/php-opis-json-schema/Dockerfile
--rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/php-opis-json-schema/bowtieJsonSchema.php
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/php-opis-json-schema/composer.json
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/python-fastjsonschema/Dockerfile
--rwxr-xr-x   0        0        0     2980 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/python-fastjsonschema/bowtie_fastjsonschema.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/python-jschon/Dockerfile
--rwxr-xr-x   0        0        0     3844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/python-jschon/bowtie_jschon.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/python-jsonschema/Dockerfile
--rwxr-xr-x   0        0        0     3409 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/python-jsonschema/bowtie_jsonschema.py
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/ruby-json_schemer/.rubocop.yml
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/ruby-json_schemer/Dockerfile
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/ruby-json_schemer/Gemfile
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/ruby-json_schemer/Gemfile.lock
--rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/ruby-json_schemer/bowtie_json_schemer.rb
--rw-r--r--   0        0        0    13200 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/rust-boon/Cargo.lock
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/rust-boon/Cargo.toml
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/rust-boon/Dockerfile
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/rust-boon/build.rs
--rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/rust-boon/src/main.rs
--rw-r--r--   0        0        0    38883 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/rust-jsonschema/Cargo.lock
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/rust-jsonschema/Cargo.toml
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/rust-jsonschema/Dockerfile
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/rust-jsonschema/build.rs
--rw-r--r--   0        0        0     5169 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/rust-jsonschema/src/main.rs
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/scala-mjs-validator/Dockerfile
--rw-r--r--   0        0        0     6835 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/scala-mjs-validator/Harness.scala
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/scala-mjs-validator/build.sbt
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/scala-mjs-validator/project/build.properties
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/scala-mjs-validator/project/plugins.sbt
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/scala-rc-circe-json-validator/Dockerfile
--rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/scala-rc-circe-json-validator/Harness.scala
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/scala-rc-circe-json-validator/build.sbt
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/scala-rc-circe-json-validator/project/build.properties
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/scala-rc-circe-json-validator/project/plugins.sbt
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/ts-vscode-json-languageservice/Dockerfile
--rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/ts-vscode-json-languageservice/bowtie_jsonls.ts
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/ts-vscode-json-languageservice/package.json
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/implementations/ts-vscode-json-languageservice/tsconfig.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/tests/__init__.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/tests/conftest.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/tests/test_cli.py
--rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/tests/test_connectables.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/tests/test_dialect.py
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/tests/test_github.py
--rw-r--r--   0        0        0     3914 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/tests/test_hypothesis.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/tests/test_implementation.py
--rw-r--r--   0        0        0    65160 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/tests/test_integration.py
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/tests/test_registry.py
--rw-r--r--   0        0        0    10149 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/tests/test_report.py
--rw-r--r--   0        0        0     4005 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/tests/test_schemas.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/tests/fauxmplementations/envsonschema/Dockerfile
--rwxr-xr-x   0        0        0     6837 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/tests/fauxmplementations/envsonschema/envsonschema
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/tests/fauxmplementations/lintsonschema/Dockerfile
--rwxr-xr-x   0        0        0     3357 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/tests/fauxmplementations/lintsonschema/lintsonschema
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/tests/fauxmplementations/lintsonschema/schemas/.gitattributes
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/tests/fauxmplementations/lintsonschema/schemas/connectables.json
--rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/tests/fauxmplementations/lintsonschema/schemas/report.json
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/tests/fauxmplementations/lintsonschema/schemas/cli/info.json
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/tests/fauxmplementations/lintsonschema/schemas/cli/smoke.json
--rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/tests/fauxmplementations/lintsonschema/schemas/cli/summary.json
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/tests/fauxmplementations/lintsonschema/schemas/io/v1.json
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/tests/fauxmplementations/lintsonschema/schemas/io/commands/dialect.json
--rw-r--r--   0        0        0     3796 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/tests/fauxmplementations/lintsonschema/schemas/io/commands/run.json
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/tests/fauxmplementations/lintsonschema/schemas/io/commands/start.json
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/tests/fauxmplementations/lintsonschema/schemas/io/commands/stop.json
--rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/tests/fauxmplementations/lintsonschema/schemas/models/dialect.json
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/tests/fauxmplementations/lintsonschema/schemas/models/group.json
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/tests/fauxmplementations/lintsonschema/schemas/models/implementation-id.json
--rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/tests/fauxmplementations/lintsonschema/schemas/models/implementation.json
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/tests/fauxmplementations/lintsonschema/schemas/models/registry.json
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/tests/fauxmplementations/lintsonschema/schemas/models/test.json
--rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/.gitignore
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/LICENSE
--rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/README.rst
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/hatch_build.py
--rw-r--r--   0        0        0     5379 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/pyproject.toml
--rw-r--r--   0        0        0     3652 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.5/PKG-INFO
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/.gitpod.Dockerfile
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/.gitpod.yml
+-rw-r--r--   0        0        0     3928 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/.prettierrc.json
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/.readthedocs.yaml
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/CONTRIBUTING.rst
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/action.yml
+-rw-r--r--   0        0        0    12706 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/noxfile.py
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/requirements.txt
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/test-requirements.in
+-rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/test-requirements.txt
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/.devcontainer/devcontainer.json
+-rwxr-xr-x   0        0        0     2229 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/.pre-commit-hooks/check-dependabot
+-rwxr-xr-x   0        0        0     1267 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/.pre-commit-hooks/check-lintsonschema-schema
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/bowtie/__init__.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/bowtie/__main__.py
+-rw-r--r--   0        0        0    48261 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/bowtie/_cli.py
+-rw-r--r--   0        0        0    12066 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/bowtie/_commands.py
+-rw-r--r--   0        0        0     4100 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/bowtie/_connectables.py
+-rw-r--r--   0        0        0    11145 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/bowtie/_containers.py
+-rw-r--r--   0        0        0    22876 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/bowtie/_core.py
+-rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/bowtie/_registry.py
+-rw-r--r--   0        0        0    11625 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/bowtie/_report.py
+-rw-r--r--   0        0        0     7661 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/bowtie/_suite.py
+-rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/bowtie/exceptions.py
+-rw-r--r--   0        0        0     9707 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/bowtie/hypothesis.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/bowtie/py.typed
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/bowtie/schemas/connectables.json
+-rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/bowtie/schemas/report.json
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/bowtie/schemas/cli/info.json
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/bowtie/schemas/cli/smoke.json
+-rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/bowtie/schemas/cli/summary.json
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/bowtie/schemas/io/v1.json
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/bowtie/schemas/io/commands/dialect.json
+-rw-r--r--   0        0        0     3796 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/bowtie/schemas/io/commands/run.json
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/bowtie/schemas/io/commands/start.json
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/bowtie/schemas/io/commands/stop.json
+-rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/bowtie/schemas/models/dialect.json
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/bowtie/schemas/models/group.json
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/bowtie/schemas/models/implementation-id.json
+-rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/bowtie/schemas/models/implementation.json
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/bowtie/schemas/models/registry.json
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/bowtie/schemas/models/test.json
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/data/dialects.json
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/docs/Makefile
+-rw-r--r--   0        0        0     8253 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/docs/cli.rst
+-rw-r--r--   0        0        0     4100 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/docs/conf.py
+-rw-r--r--   0        0        0     8235 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/docs/contributing.rst
+-rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/docs/github-actions.rst
+-rw-r--r--   0        0        0    36467 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/docs/implementers.rst
+-rw-r--r--   0        0        0     3256 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/docs/index.rst
+-rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/docs/motd.txt
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/docs/requirements.in
+-rw-r--r--   0        0        0     3713 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/docs/requirements.txt
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/docs/spelling-wordlist.txt
+-rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/docs/_static/bowtie_diagram_dark.svg
+-rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/docs/_static/bowtie_diagram_light.svg
+-rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/docs/_static/logo.svg
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/frontend/index.html
+-rw-r--r--   0        0        0     2541 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/frontend/package.json
+-rw-r--r--   0        0        0   163423 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/frontend/pnpm-lock.yaml
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/frontend/tsconfig.json
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/frontend/vite.config.ts
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/frontend/public/favicon.svg
+-rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/frontend/src/DialectReportView.tsx
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/frontend/src/MainContainer.tsx
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/frontend/src/ReportDataHandler.tsx
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/frontend/src/global.css
+-rw-r--r--   0        0        0     3366 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/frontend/src/index.tsx
+-rw-r--r--   0        0        0     2451 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/frontend/src/assets/landscape-logo.svg
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/frontend/src/components/CopyToClipboard.tsx
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/frontend/src/components/FilterSection.css
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/frontend/src/components/FilterSection.tsx
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/frontend/src/components/LoadingAnimation.tsx
+-rw-r--r--   0        0        0     5644 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/frontend/src/components/NavBar.tsx
+-rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/frontend/src/components/OtherImplementations.tsx
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/frontend/src/components/BowtieInfo/BowtieInfoSection.tsx
+-rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/frontend/src/components/Cases/CaseItem.tsx
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/frontend/src/components/Cases/CaseResultSvg.test.tsx
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/frontend/src/components/Cases/CaseResultSvg.tsx
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/frontend/src/components/Cases/CasesSection.tsx
+-rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/frontend/src/components/Cases/SchemaDisplay.tsx
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/frontend/src/components/DragAndDrop/DragAndDrop.css
+-rw-r--r--   0        0        0     4907 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/frontend/src/components/DragAndDrop/DragAndDrop.tsx
+-rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/frontend/src/components/ImplementationReportView/DialectCompliance.tsx
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/frontend/src/components/ImplementationReportView/EmbedBadges.css
+-rw-r--r--   0        0        0     6071 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/frontend/src/components/ImplementationReportView/EmbedBadges.tsx
+-rw-r--r--   0        0        0     4815 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/frontend/src/components/ImplementationReportView/ImplementationReportView.tsx
+-rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/frontend/src/components/Modals/DetailsButtonModal.tsx
+-rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/frontend/src/components/RunInfo/RunInfoSection.tsx
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/frontend/src/components/Summary/ImplementationRow.css
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/frontend/src/components/Summary/ImplementationRow.tsx
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/frontend/src/components/Summary/SummarySection.tsx
+-rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/frontend/src/components/Summary/SummaryTable.tsx
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/frontend/src/context/BowtieVersionContext.tsx
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/frontend/src/context/ThemeContext.tsx
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/frontend/src/data/Badge.test.ts
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/frontend/src/data/Badge.ts
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/frontend/src/data/Dialect.test.ts
+-rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/frontend/src/data/Dialect.ts
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/frontend/src/data/Site.test.ts
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/frontend/src/data/Site.ts
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/frontend/src/data/mapLanguage.ts
+-rw-r--r--   0        0        0     8855 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/frontend/src/data/parseReportData.test.ts
+-rw-r--r--   0        0        0     9164 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/frontend/src/data/parseReportData.ts
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/frontend/src/hooks/useSearchParams.ts
+-rw-r--r--   0        0        0    21214 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/.java-implementations-pmd-ruleset.xml
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/clojure-json-schema/Dockerfile
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/clojure-json-schema/project.clj
+-rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/clojure-json-schema/src/bowtie_json_schema/core.clj
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/cpp-valijson/.dockerignore
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/cpp-valijson/.gitignore
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/cpp-valijson/Dockerfile
+-rw-r--r--   0        0        0     5406 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/cpp-valijson/bowtie_valijson.cpp
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/cpp-valijson/compile_flags.txt
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/dotnet-jsonschema-net/.clang-format
+-rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/dotnet-jsonschema-net/.gitignore
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/dotnet-jsonschema-net/Dockerfile
+-rw-r--r--   0        0        0     7121 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/dotnet-jsonschema-net/Program.cs
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/dotnet-jsonschema-net/bowtie_json_everything.csproj
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/dotnet-jsonschema-net/Properties/launchSettings.json
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/go-gojsonschema/Dockerfile
+-rw-r--r--   0        0        0     4681 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/go-gojsonschema/bowtie_gojsonschema.go
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/go-gojsonschema/go.mod
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/go-gojsonschema/go.sum
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/go-jsonschema/Dockerfile
+-rw-r--r--   0        0        0     4958 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/go-jsonschema/bowtie_jsonschema.go
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/go-jsonschema/go.mod
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/go-jsonschema/go.sum
+-rw-r--r--   0        0        0     8804 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/java-json-schema/BowtieJsonSchema.java
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/java-json-schema/Dockerfile
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/java-json-schema/build.gradle
+-rw-r--r--   0        0        0     7843 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/java-json-tools-json-schema-validator/BowtieJsonSchemaValidator.java
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/java-json-tools-json-schema-validator/Dockerfile
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/java-json-tools-json-schema-validator/build.gradle
+-rw-r--r--   0        0        0     7844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/java-jsonschemafriend/BowtieJsonSchemaFriend.java
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/java-jsonschemafriend/Dockerfile
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/java-jsonschemafriend/build.gradle
+-rw-r--r--   0        0        0     9453 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/java-networknt-json-schema-validator/BowtieJsonSchemaValidator.java
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/java-networknt-json-schema-validator/Dockerfile
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/java-networknt-json-schema-validator/build.gradle
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/java-openapiprocessor/.dockerignore
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/java-openapiprocessor/.editorconfig
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/java-openapiprocessor/Dockerfile
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/java-openapiprocessor/build.gradle.kts
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/java-openapiprocessor/gradle.properties
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/java-openapiprocessor/justfile
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/java-openapiprocessor/settings.gradle.kts
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/java-openapiprocessor/gradle/libs.versions.toml
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/java-openapiprocessor/src/main/kotlin/Main.kt
+-rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/java-openapiprocessor/src/main/kotlin/Runner.kt
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/java-openapiprocessor/src/main/kotlin/Support.kt
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/java-openapiprocessor/src/main/kotlin/commands/Configuration.kt
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/java-openapiprocessor/src/main/kotlin/commands/Dialect.kt
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/java-openapiprocessor/src/main/kotlin/commands/Request.kt
+-rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/java-openapiprocessor/src/main/kotlin/commands/RunCmd.kt
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/java-openapiprocessor/src/main/kotlin/commands/StartCmd.kt
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/java-openapiprocessor/src/main/kotlin/commands/StopCmd.kt
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/js-ajv/Dockerfile
+-rw-r--r--   0        0        0     2990 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/js-ajv/bowtie_ajv.js
+-rw-r--r--   0        0        0     4870 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/js-ajv/package-lock.json
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/js-ajv/package.json
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/js-hyperjump/Dockerfile
+-rw-r--r--   0        0        0     5711 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/js-hyperjump/bowtie_hyperjump.js
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/js-hyperjump/package.json
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/js-json-schema/Dockerfile
+-rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/js-json-schema/bowtie_json_schema.js
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/js-json-schema/package.json
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/js-jsonschema/Dockerfile
+-rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/js-jsonschema/bowtie_jsonschema.js
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/js-jsonschema/package.json
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/kotlin-kmp-json-schema-validator/.gitignore
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/kotlin-kmp-json-schema-validator/Dockerfile
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/kotlin-kmp-json-schema-validator/build.gradle.kts
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/kotlin-kmp-json-schema-validator/settings.gradle.kts
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/kotlin-kmp-json-schema-validator/gradle/libs.versions.toml
+-rw-r--r--   0        0        0     7879 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/BowtieSampsonSchemaValidatorLauncher.kt
+-rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Commands.kt
+-rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Responses.kt
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/TestFilters.kt
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/lua-jsonschema/Dockerfile
+-rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/lua-jsonschema/bowtie_jsonschema.lua
+-rw-r--r--   0        0        0     9638 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/lua-jsonschema/json.lua
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/lua-jsonschema/stylua.toml
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/php-opis-json-schema/Dockerfile
+-rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/php-opis-json-schema/bowtieJsonSchema.php
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/php-opis-json-schema/composer.json
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/python-fastjsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     2980 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/python-fastjsonschema/bowtie_fastjsonschema.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/python-jschon/Dockerfile
+-rwxr-xr-x   0        0        0     3844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/python-jschon/bowtie_jschon.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/python-jsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     3409 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/python-jsonschema/bowtie_jsonschema.py
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/ruby-json_schemer/.rubocop.yml
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/ruby-json_schemer/Dockerfile
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/ruby-json_schemer/Gemfile
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/ruby-json_schemer/Gemfile.lock
+-rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/ruby-json_schemer/bowtie_json_schemer.rb
+-rw-r--r--   0        0        0    13200 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/rust-boon/Cargo.lock
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/rust-boon/Cargo.toml
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/rust-boon/Dockerfile
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/rust-boon/build.rs
+-rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/rust-boon/src/main.rs
+-rw-r--r--   0        0        0    39299 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/rust-jsonschema/Cargo.lock
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/rust-jsonschema/Cargo.toml
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/rust-jsonschema/Dockerfile
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/rust-jsonschema/build.rs
+-rw-r--r--   0        0        0     5169 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/rust-jsonschema/src/main.rs
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/scala-mjs-validator/Dockerfile
+-rw-r--r--   0        0        0     6835 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/scala-mjs-validator/Harness.scala
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/scala-mjs-validator/build.sbt
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/scala-mjs-validator/project/build.properties
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/scala-mjs-validator/project/plugins.sbt
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/scala-rc-circe-json-validator/Dockerfile
+-rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/scala-rc-circe-json-validator/Harness.scala
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/scala-rc-circe-json-validator/build.sbt
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/scala-rc-circe-json-validator/project/build.properties
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/scala-rc-circe-json-validator/project/plugins.sbt
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/ts-vscode-json-languageservice/Dockerfile
+-rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/ts-vscode-json-languageservice/bowtie_jsonls.ts
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/ts-vscode-json-languageservice/package.json
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/implementations/ts-vscode-json-languageservice/tsconfig.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/tests/__init__.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/tests/conftest.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/tests/test_cli.py
+-rw-r--r--   0        0        0     2960 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/tests/test_connectables.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/tests/test_dialect.py
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/tests/test_github.py
+-rw-r--r--   0        0        0     3914 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/tests/test_hypothesis.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/tests/test_implementation.py
+-rw-r--r--   0        0        0    65238 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/tests/test_integration.py
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/tests/test_registry.py
+-rw-r--r--   0        0        0    10149 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/tests/test_report.py
+-rw-r--r--   0        0        0     4005 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/tests/test_schemas.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/tests/fauxmplementations/envsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     6837 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/tests/fauxmplementations/envsonschema/envsonschema
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/tests/fauxmplementations/lintsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     3357 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/tests/fauxmplementations/lintsonschema/lintsonschema
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/tests/fauxmplementations/lintsonschema/schemas/.gitattributes
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/tests/fauxmplementations/lintsonschema/schemas/connectables.json
+-rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/tests/fauxmplementations/lintsonschema/schemas/report.json
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/tests/fauxmplementations/lintsonschema/schemas/cli/info.json
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/tests/fauxmplementations/lintsonschema/schemas/cli/smoke.json
+-rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/tests/fauxmplementations/lintsonschema/schemas/cli/summary.json
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/tests/fauxmplementations/lintsonschema/schemas/io/v1.json
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/tests/fauxmplementations/lintsonschema/schemas/io/commands/dialect.json
+-rw-r--r--   0        0        0     3796 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/tests/fauxmplementations/lintsonschema/schemas/io/commands/run.json
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/tests/fauxmplementations/lintsonschema/schemas/io/commands/start.json
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/tests/fauxmplementations/lintsonschema/schemas/io/commands/stop.json
+-rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/tests/fauxmplementations/lintsonschema/schemas/models/dialect.json
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/tests/fauxmplementations/lintsonschema/schemas/models/group.json
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/tests/fauxmplementations/lintsonschema/schemas/models/implementation-id.json
+-rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/tests/fauxmplementations/lintsonschema/schemas/models/implementation.json
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/tests/fauxmplementations/lintsonschema/schemas/models/registry.json
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/tests/fauxmplementations/lintsonschema/schemas/models/test.json
+-rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/.gitignore
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/LICENSE
+-rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/README.rst
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/hatch_build.py
+-rw-r--r--   0        0        0     5379 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/pyproject.toml
+-rw-r--r--   0        0        0     3652 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.7/PKG-INFO
```

### Comparing `bowtie_json_schema-2024.5.5/.gitpod.yml` & `bowtie_json_schema-2024.5.7/.gitpod.yml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/.pre-commit-config.yaml` & `bowtie_json_schema-2024.5.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/CONTRIBUTING.rst` & `bowtie_json_schema-2024.5.7/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/action.yml` & `bowtie_json_schema-2024.5.7/action.yml`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 runs:
   using: composite
   steps:
     - uses: actions/setup-python@v5
       id: localpython
       with:
-        python-version: "3.10 - 3.11"
+        python-version: "3.10 - 3.12"
         update-environment: false
 
     - name: "Install latest Bowtie"
       if: inputs.version == ''
       run: pipx install --python "${{ steps.localpython.outputs.python-path }}" bowtie-json-schema
       shell: bash
```

### Comparing `bowtie_json_schema-2024.5.5/noxfile.py` & `bowtie_json_schema-2024.5.7/noxfile.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/requirements.txt` & `bowtie_json_schema-2024.5.7/requirements.txt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/test-requirements.txt` & `bowtie_json_schema-2024.5.7/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/.pre-commit-hooks/check-dependabot` & `bowtie_json_schema-2024.5.7/.pre-commit-hooks/check-dependabot`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/.pre-commit-hooks/check-lintsonschema-schema` & `bowtie_json_schema-2024.5.7/.pre-commit-hooks/check-lintsonschema-schema`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/bowtie/_cli.py` & `bowtie_json_schema-2024.5.7/bowtie/_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -298,15 +298,15 @@
         @click.option(
             "--implementation",
             "-i",
             "connectables",
             type=_connectables.ClickParam(),
             default=lambda: (
                 default_implementations
-                if sys.stdin.isatty()
+                if sys.stdin.isatty() or "CI" in os.environ
                 else [line.strip() for line in sys.stdin]
             ),
             multiple=True,
             metavar="IMPLEMENTATION",
             help="A container image which implements the bowtie IO protocol.",
         )
         @TIMEOUT
@@ -1148,17 +1148,15 @@
             for each in value  # type: ignore[reportUnknownArgumentType]
         )
     ),
     multiple=True,
     metavar="LANGUAGE",
     help="Only include implementations in the given programming language",
 )
-@click.pass_context
 async def filter_implementations(
-    ctx: click.Context,
     start: Callable[
         [],
         AsyncIterator[tuple[ImplementationId, Implementation]],
     ],
     dialects: Sequence[Dialect],
     languages: Set[str],
 ):
```

### Comparing `bowtie_json_schema-2024.5.5/bowtie/_commands.py` & `bowtie_json_schema-2024.5.7/bowtie/_commands.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/bowtie/_connectables.py` & `bowtie_json_schema-2024.5.7/bowtie/_connectables.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,14 +82,16 @@
     @classmethod
     def from_str(cls, fqid: ImplementationId):
         connector, sep, id = fqid.partition(":")
         if not sep:
             connector, id = "image", connector
         Connector = cls._connectors.get(connector)
         if Connector is None:
+            if "/" in connector:
+                return cls(id=fqid, connector=cls._connectors["image"](fqid))
             raise UnknownConnector(connector)
         return cls(id=fqid, connector=Connector(id))
 
     @asynccontextmanager
     async def connect(self, **kwargs: Any) -> AsyncIterator[Implementation]:
         async with (
             self._connector.connect() as connection,
```

### Comparing `bowtie_json_schema-2024.5.5/bowtie/_containers.py` & `bowtie_json_schema-2024.5.7/bowtie/_containers.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/bowtie/_core.py` & `bowtie_json_schema-2024.5.7/bowtie/_core.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/bowtie/_registry.py` & `bowtie_json_schema-2024.5.7/bowtie/_registry.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/bowtie/_report.py` & `bowtie_json_schema-2024.5.7/bowtie/_report.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/bowtie/_suite.py` & `bowtie_json_schema-2024.5.7/bowtie/_suite.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/bowtie/exceptions.py` & `bowtie_json_schema-2024.5.7/bowtie/exceptions.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/bowtie/hypothesis.py` & `bowtie_json_schema-2024.5.7/bowtie/hypothesis.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/bowtie/schemas/connectables.json` & `bowtie_json_schema-2024.5.7/bowtie/schemas/connectables.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761904761904762%*

 * *Differences: {"'oneOf'": "{insert: [(1, OrderedDict([('title', 'Implicit Image With Repository & Tag'), "*

 * *            "('pattern', '^[^:/]+/[^:/]+:[^:/]+$')]))]}"}*

```diff
@@ -12,14 +12,18 @@
     "description": "A mini-language for connecting to supported harnesses.",
     "oneOf": [
         {
             "pattern": "^[^:]+$",
             "title": "Implicit Image"
         },
         {
+            "pattern": "^[^:/]+/[^:/]+:[^:/]+$",
+            "title": "Implicit Image With Repository & Tag"
+        },
+        {
             "description": "A connectable with explicit connector.",
             "oneOf": [
                 {
                     "$ref": "#image"
                 }
             ],
             "pattern": "^[^:]+:[^:]+(:[^:]+)?$",
```

### Comparing `bowtie_json_schema-2024.5.5/bowtie/schemas/report.json` & `bowtie_json_schema-2024.5.7/bowtie/schemas/report.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/bowtie/schemas/cli/info.json` & `bowtie_json_schema-2024.5.7/bowtie/schemas/cli/info.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/bowtie/schemas/cli/smoke.json` & `bowtie_json_schema-2024.5.7/bowtie/schemas/cli/smoke.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/bowtie/schemas/cli/summary.json` & `bowtie_json_schema-2024.5.7/bowtie/schemas/cli/summary.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/bowtie/schemas/io/v1.json` & `bowtie_json_schema-2024.5.7/bowtie/schemas/io/v1.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/bowtie/schemas/io/commands/dialect.json` & `bowtie_json_schema-2024.5.7/bowtie/schemas/io/commands/dialect.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/bowtie/schemas/io/commands/run.json` & `bowtie_json_schema-2024.5.7/bowtie/schemas/io/commands/run.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/bowtie/schemas/io/commands/start.json` & `bowtie_json_schema-2024.5.7/bowtie/schemas/io/commands/start.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/bowtie/schemas/models/dialect.json` & `bowtie_json_schema-2024.5.7/bowtie/schemas/models/dialect.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/bowtie/schemas/models/group.json` & `bowtie_json_schema-2024.5.7/bowtie/schemas/models/group.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/bowtie/schemas/models/implementation.json` & `bowtie_json_schema-2024.5.7/bowtie/schemas/models/implementation.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/bowtie/schemas/models/test.json` & `bowtie_json_schema-2024.5.7/bowtie/schemas/models/test.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/data/dialects.json` & `bowtie_json_schema-2024.5.7/data/dialects.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/docs/Makefile` & `bowtie_json_schema-2024.5.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/docs/cli.rst` & `bowtie_json_schema-2024.5.7/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/docs/conf.py` & `bowtie_json_schema-2024.5.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/docs/contributing.rst` & `bowtie_json_schema-2024.5.7/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/docs/github-actions.rst` & `bowtie_json_schema-2024.5.7/docs/github-actions.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/docs/implementers.rst` & `bowtie_json_schema-2024.5.7/docs/implementers.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/docs/index.rst` & `bowtie_json_schema-2024.5.7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/docs/motd.txt` & `bowtie_json_schema-2024.5.7/docs/motd.txt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/docs/requirements.txt` & `bowtie_json_schema-2024.5.7/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/docs/_static/bowtie_diagram_dark.svg` & `bowtie_json_schema-2024.5.7/docs/_static/bowtie_diagram_dark.svg`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/docs/_static/bowtie_diagram_light.svg` & `bowtie_json_schema-2024.5.7/docs/_static/bowtie_diagram_light.svg`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/docs/_static/logo.svg` & `bowtie_json_schema-2024.5.7/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/frontend/package.json` & `bowtie_json_schema-2024.5.7/frontend/package.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/frontend/pnpm-lock.yaml` & `bowtie_json_schema-2024.5.7/frontend/pnpm-lock.yaml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/frontend/tsconfig.json` & `bowtie_json_schema-2024.5.7/frontend/tsconfig.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/frontend/public/favicon.svg` & `bowtie_json_schema-2024.5.7/frontend/public/favicon.svg`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/frontend/src/DialectReportView.tsx` & `bowtie_json_schema-2024.5.7/frontend/src/DialectReportView.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/frontend/src/ReportDataHandler.tsx` & `bowtie_json_schema-2024.5.7/frontend/src/ReportDataHandler.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/frontend/src/index.tsx` & `bowtie_json_schema-2024.5.7/frontend/src/index.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/frontend/src/assets/landscape-logo.svg` & `bowtie_json_schema-2024.5.7/frontend/src/assets/landscape-logo.svg`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/frontend/src/components/CopyToClipboard.tsx` & `bowtie_json_schema-2024.5.7/frontend/src/components/CopyToClipboard.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/frontend/src/components/FilterSection.tsx` & `bowtie_json_schema-2024.5.7/frontend/src/components/FilterSection.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/frontend/src/components/NavBar.tsx` & `bowtie_json_schema-2024.5.7/frontend/src/components/NavBar.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/frontend/src/components/OtherImplementations.tsx` & `bowtie_json_schema-2024.5.7/frontend/src/components/OtherImplementations.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/frontend/src/components/BowtieInfo/BowtieInfoSection.tsx` & `bowtie_json_schema-2024.5.7/frontend/src/components/BowtieInfo/BowtieInfoSection.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/frontend/src/components/Cases/CaseItem.tsx` & `bowtie_json_schema-2024.5.7/frontend/src/components/Cases/CaseItem.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/frontend/src/components/Cases/CaseResultSvg.test.tsx` & `bowtie_json_schema-2024.5.7/frontend/src/components/Cases/CaseResultSvg.test.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/frontend/src/components/Cases/CaseResultSvg.tsx` & `bowtie_json_schema-2024.5.7/frontend/src/components/Cases/CaseResultSvg.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/frontend/src/components/Cases/CasesSection.tsx` & `bowtie_json_schema-2024.5.7/frontend/src/components/Cases/CasesSection.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/frontend/src/components/Cases/SchemaDisplay.tsx` & `bowtie_json_schema-2024.5.7/frontend/src/components/Cases/SchemaDisplay.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/frontend/src/components/DragAndDrop/DragAndDrop.tsx` & `bowtie_json_schema-2024.5.7/frontend/src/components/DragAndDrop/DragAndDrop.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/frontend/src/components/ImplementationReportView/DialectCompliance.tsx` & `bowtie_json_schema-2024.5.7/frontend/src/components/ImplementationReportView/DialectCompliance.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/frontend/src/components/ImplementationReportView/EmbedBadges.tsx` & `bowtie_json_schema-2024.5.7/frontend/src/components/ImplementationReportView/EmbedBadges.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/frontend/src/components/ImplementationReportView/ImplementationReportView.tsx` & `bowtie_json_schema-2024.5.7/frontend/src/components/ImplementationReportView/ImplementationReportView.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/frontend/src/components/Modals/DetailsButtonModal.tsx` & `bowtie_json_schema-2024.5.7/frontend/src/components/Modals/DetailsButtonModal.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/frontend/src/components/RunInfo/RunInfoSection.tsx` & `bowtie_json_schema-2024.5.7/frontend/src/components/RunInfo/RunInfoSection.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/frontend/src/components/Summary/ImplementationRow.css` & `bowtie_json_schema-2024.5.7/frontend/src/components/Summary/ImplementationRow.css`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/frontend/src/components/Summary/ImplementationRow.tsx` & `bowtie_json_schema-2024.5.7/frontend/src/components/Summary/ImplementationRow.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/frontend/src/components/Summary/SummarySection.tsx` & `bowtie_json_schema-2024.5.7/frontend/src/components/Summary/SummarySection.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/frontend/src/components/Summary/SummaryTable.tsx` & `bowtie_json_schema-2024.5.7/frontend/src/components/Summary/SummaryTable.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/frontend/src/context/BowtieVersionContext.tsx` & `bowtie_json_schema-2024.5.7/frontend/src/context/BowtieVersionContext.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/frontend/src/context/ThemeContext.tsx` & `bowtie_json_schema-2024.5.7/frontend/src/context/ThemeContext.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/frontend/src/data/Badge.test.ts` & `bowtie_json_schema-2024.5.7/frontend/src/data/Badge.test.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/frontend/src/data/Badge.ts` & `bowtie_json_schema-2024.5.7/frontend/src/data/Badge.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/frontend/src/data/Dialect.ts` & `bowtie_json_schema-2024.5.7/frontend/src/data/Dialect.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/frontend/src/data/Site.test.ts` & `bowtie_json_schema-2024.5.7/frontend/src/data/Site.test.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/frontend/src/data/parseReportData.test.ts` & `bowtie_json_schema-2024.5.7/frontend/src/data/parseReportData.test.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/frontend/src/data/parseReportData.ts` & `bowtie_json_schema-2024.5.7/frontend/src/data/parseReportData.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/implementations/.java-implementations-pmd-ruleset.xml` & `bowtie_json_schema-2024.5.7/implementations/.java-implementations-pmd-ruleset.xml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/implementations/clojure-json-schema/Dockerfile` & `bowtie_json_schema-2024.5.7/implementations/clojure-json-schema/Dockerfile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/implementations/clojure-json-schema/src/bowtie_json_schema/core.clj` & `bowtie_json_schema-2024.5.7/implementations/clojure-json-schema/src/bowtie_json_schema/core.clj`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/implementations/cpp-valijson/bowtie_valijson.cpp` & `bowtie_json_schema-2024.5.7/implementations/cpp-valijson/bowtie_valijson.cpp`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/implementations/dotnet-jsonschema-net/.gitignore` & `bowtie_json_schema-2024.5.7/implementations/dotnet-jsonschema-net/.gitignore`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/implementations/dotnet-jsonschema-net/Program.cs` & `bowtie_json_schema-2024.5.7/implementations/dotnet-jsonschema-net/Program.cs`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/implementations/go-gojsonschema/bowtie_gojsonschema.go` & `bowtie_json_schema-2024.5.7/implementations/go-gojsonschema/bowtie_gojsonschema.go`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/implementations/go-gojsonschema/go.sum` & `bowtie_json_schema-2024.5.7/implementations/go-gojsonschema/go.sum`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/implementations/go-jsonschema/bowtie_jsonschema.go` & `bowtie_json_schema-2024.5.7/implementations/go-jsonschema/bowtie_jsonschema.go`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/implementations/java-json-schema/BowtieJsonSchema.java` & `bowtie_json_schema-2024.5.7/implementations/java-json-schema/BowtieJsonSchema.java`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/implementations/java-json-schema/build.gradle` & `bowtie_json_schema-2024.5.7/implementations/java-json-schema/build.gradle`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/implementations/java-json-tools-json-schema-validator/BowtieJsonSchemaValidator.java` & `bowtie_json_schema-2024.5.7/implementations/java-json-tools-json-schema-validator/BowtieJsonSchemaValidator.java`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/implementations/java-json-tools-json-schema-validator/build.gradle` & `bowtie_json_schema-2024.5.7/implementations/java-json-tools-json-schema-validator/build.gradle`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/implementations/java-jsonschemafriend/BowtieJsonSchemaFriend.java` & `bowtie_json_schema-2024.5.7/implementations/java-jsonschemafriend/BowtieJsonSchemaFriend.java`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/implementations/java-jsonschemafriend/build.gradle` & `bowtie_json_schema-2024.5.7/implementations/java-jsonschemafriend/build.gradle`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/implementations/java-networknt-json-schema-validator/BowtieJsonSchemaValidator.java` & `bowtie_json_schema-2024.5.7/implementations/java-networknt-json-schema-validator/BowtieJsonSchemaValidator.java`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/implementations/java-networknt-json-schema-validator/build.gradle` & `bowtie_json_schema-2024.5.7/implementations/java-networknt-json-schema-validator/build.gradle`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/implementations/java-openapiprocessor/build.gradle.kts` & `bowtie_json_schema-2024.5.7/implementations/java-openapiprocessor/build.gradle.kts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/implementations/java-openapiprocessor/justfile` & `bowtie_json_schema-2024.5.7/implementations/java-openapiprocessor/justfile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/implementations/java-openapiprocessor/gradle/libs.versions.toml` & `bowtie_json_schema-2024.5.7/implementations/java-openapiprocessor/gradle/libs.versions.toml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/implementations/java-openapiprocessor/src/main/kotlin/Runner.kt` & `bowtie_json_schema-2024.5.7/implementations/java-openapiprocessor/src/main/kotlin/Runner.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/implementations/java-openapiprocessor/src/main/kotlin/Support.kt` & `bowtie_json_schema-2024.5.7/implementations/java-openapiprocessor/src/main/kotlin/Support.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/implementations/java-openapiprocessor/src/main/kotlin/commands/Request.kt` & `bowtie_json_schema-2024.5.7/implementations/java-openapiprocessor/src/main/kotlin/commands/Request.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/implementations/java-openapiprocessor/src/main/kotlin/commands/RunCmd.kt` & `bowtie_json_schema-2024.5.7/implementations/java-openapiprocessor/src/main/kotlin/commands/RunCmd.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/implementations/java-openapiprocessor/src/main/kotlin/commands/StartCmd.kt` & `bowtie_json_schema-2024.5.7/implementations/java-openapiprocessor/src/main/kotlin/commands/StartCmd.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/implementations/js-ajv/bowtie_ajv.js` & `bowtie_json_schema-2024.5.7/implementations/js-ajv/bowtie_ajv.js`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/implementations/js-ajv/package-lock.json` & `bowtie_json_schema-2024.5.7/implementations/js-ajv/package-lock.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/implementations/js-hyperjump/bowtie_hyperjump.js` & `bowtie_json_schema-2024.5.7/implementations/js-hyperjump/bowtie_hyperjump.js`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/implementations/js-json-schema/bowtie_json_schema.js` & `bowtie_json_schema-2024.5.7/implementations/js-json-schema/bowtie_json_schema.js`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/implementations/js-jsonschema/bowtie_jsonschema.js` & `bowtie_json_schema-2024.5.7/implementations/js-jsonschema/bowtie_jsonschema.js`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/implementations/kotlin-kmp-json-schema-validator/build.gradle.kts` & `bowtie_json_schema-2024.5.7/implementations/kotlin-kmp-json-schema-validator/build.gradle.kts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/BowtieSampsonSchemaValidatorLauncher.kt` & `bowtie_json_schema-2024.5.7/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/BowtieSampsonSchemaValidatorLauncher.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Commands.kt` & `bowtie_json_schema-2024.5.7/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Commands.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Responses.kt` & `bowtie_json_schema-2024.5.7/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Responses.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/TestFilters.kt` & `bowtie_json_schema-2024.5.7/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/TestFilters.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/implementations/lua-jsonschema/Dockerfile` & `bowtie_json_schema-2024.5.7/implementations/lua-jsonschema/Dockerfile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/implementations/lua-jsonschema/bowtie_jsonschema.lua` & `bowtie_json_schema-2024.5.7/implementations/lua-jsonschema/bowtie_jsonschema.lua`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/implementations/lua-jsonschema/json.lua` & `bowtie_json_schema-2024.5.7/implementations/lua-jsonschema/json.lua`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/implementations/php-opis-json-schema/bowtieJsonSchema.php` & `bowtie_json_schema-2024.5.7/implementations/php-opis-json-schema/bowtieJsonSchema.php`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/implementations/python-fastjsonschema/bowtie_fastjsonschema.py` & `bowtie_json_schema-2024.5.7/implementations/python-fastjsonschema/bowtie_fastjsonschema.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/implementations/python-jschon/bowtie_jschon.py` & `bowtie_json_schema-2024.5.7/implementations/python-jschon/bowtie_jschon.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/implementations/python-jsonschema/bowtie_jsonschema.py` & `bowtie_json_schema-2024.5.7/implementations/python-jsonschema/bowtie_jsonschema.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/implementations/ruby-json_schemer/bowtie_json_schemer.rb` & `bowtie_json_schema-2024.5.7/implementations/ruby-json_schemer/bowtie_json_schemer.rb`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/implementations/rust-boon/Cargo.lock` & `bowtie_json_schema-2024.5.7/implementations/rust-boon/Cargo.lock`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/implementations/rust-boon/Dockerfile` & `bowtie_json_schema-2024.5.7/implementations/rust-boon/Dockerfile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/implementations/rust-boon/src/main.rs` & `bowtie_json_schema-2024.5.7/implementations/rust-boon/src/main.rs`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/implementations/rust-jsonschema/Cargo.lock` & `bowtie_json_schema-2024.5.7/implementations/rust-jsonschema/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -15,31 +15,31 @@
 name = "adler"
 version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f26201604c87b1e01bd3d98f8d5d9a8fcbb815e8cedb41ffccbeb4bf593a35fe"
 
 [[package]]
 name = "ahash"
-version = "0.8.6"
+version = "0.8.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "91429305e9f0a25f6205c5b8e0d2db09e0708a7a6df0f42212bb56c32c8ac97a"
+checksum = "e89da841a80418a9b391ebaea17f5c112ffaaa96f621d2c285b5174da76b9011"
 dependencies = [
  "cfg-if",
  "getrandom",
  "once_cell",
  "serde",
  "version_check",
  "zerocopy",
 ]
 
 [[package]]
 name = "aho-corasick"
-version = "1.1.2"
+version = "1.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b2969dcb958b36655471fc61f7e416fa76033bdd4bfed0678d8fee1e2d07a1f0"
+checksum = "8e60d3430d3a69478ad0993f19238d2df97c507009a52b3c10addcd7f6bcb916"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "anstream"
 version = "0.6.14"
@@ -53,57 +53,57 @@
  "colorchoice",
  "is_terminal_polyfill",
  "utf8parse",
 ]
 
 [[package]]
 name = "anstyle"
-version = "1.0.4"
+version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7079075b41f533b8c61d2a4d073c4676e1f8b249ff94a393b0595db304e0dd87"
+checksum = "038dfcf04a5feb68e9c60b21c9625a54c2c0616e79b72b0fd87075a056ae1d1b"
 
 [[package]]
 name = "anstyle-parse"
-version = "0.2.2"
+version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "317b9a89c1868f5ea6ff1d9539a69f45dffc21ce321ac1fd1160dfa48c8e2140"
+checksum = "c03a11a9034d92058ceb6ee011ce58af4a9bf61491aa7e1e59ecd24bd40d22d4"
 dependencies = [
  "utf8parse",
 ]
 
 [[package]]
 name = "anstyle-query"
-version = "1.0.0"
+version = "1.0.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5ca11d4be1bab0c8bc8734a9aa7bf4ee8316d462a08c6ac5052f888fef5b494b"
+checksum = "a64c907d4e79225ac72e2a354c9ce84d50ebb4586dee56c82b3ee73004f537f5"
 dependencies = [
- "windows-sys 0.48.0",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "anstyle-wincon"
-version = "3.0.1"
+version = "3.0.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f0699d10d2f4d628a98ee7b57b289abbc98ff3bad977cb3152709d4bf2330628"
+checksum = "61a38449feb7068f52bb06c12759005cf459ee52bb4adc1d5a7c4322d716fb19"
 dependencies = [
  "anstyle",
- "windows-sys 0.48.0",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "anyhow"
-version = "1.0.75"
+version = "1.0.83"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a4668cab20f66d8d020e1fbc0ebe47217433c1b6c8f2040faf858554e394ace6"
+checksum = "25bdb32cbbdce2b519a9cd7df3a678443100e265d5e25ca763b7572a5104f5f3"
 
 [[package]]
 name = "autocfg"
-version = "1.1.0"
+version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
+checksum = "0c4b4d0bd25bd0b74681c0ad21497610ce1b7c91b1022cd21c80c6fbdd9476b0"
 
 [[package]]
 name = "backtrace"
 version = "0.3.71"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "26b05800d2e817c8b3b4b54abd461726265fa9789ae34330622f2db9ee696f9d"
 dependencies = [
@@ -135,17 +135,17 @@
 name = "bit-vec"
 version = "0.6.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "349f9b6a179ed607305526ca489b34ad0a41aed5f7980fa90eb03160b69598fb"
 
 [[package]]
 name = "bitflags"
-version = "1.3.2"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
+checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
 
 [[package]]
 name = "bowtie-rust-jsonschema"
 version = "0.1.0"
 dependencies = [
  "backtrace",
  "cargo-lock",
@@ -155,29 +155,29 @@
  "serde",
  "serde_json",
  "url",
 ]
 
 [[package]]
 name = "bumpalo"
-version = "3.14.0"
+version = "3.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7f30e7476521f6f8af1a1c4c0b8cc94f0bee37d91763d0ca2665f299b6cd8aec"
+checksum = "79296716171880943b8470b5f8d03aa55eb2e645a4874bdbb28adb49162e012c"
 
 [[package]]
 name = "bytecount"
-version = "0.6.7"
+version = "0.6.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e1e5f035d16fc623ae5f74981db80a439803888314e3a555fd6f04acd51a3205"
+checksum = "5ce89b21cab1437276d2650d57e971f9d548a2d9037cc231abdc0562b97498ce"
 
 [[package]]
 name = "bytes"
-version = "1.5.0"
+version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a2bd12c1caf447e69cd4528f47f94d203fd2582878ecb9e9465484c4148a8223"
+checksum = "514de17de45fdb8dc022b1a7975556c53c86f9f0aa5f534b98977b171857c2c9"
 
 [[package]]
 name = "cargo-lock"
 version = "9.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e11c675378efb449ed3ce8de78d75d0d80542fc98487c26aba28eb3b82feac72"
 dependencies = [
@@ -185,17 +185,17 @@
  "serde",
  "toml",
  "url",
 ]
 
 [[package]]
 name = "cc"
-version = "1.0.90"
+version = "1.0.97"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8cd6604a82acf3039f1144f54b8eb34e91ffba622051189e71b781822d5ee1f5"
+checksum = "099a5357d84c4c61eb35fc8eafa9a79a902c2f76911e5747ced4e032edd8d9b4"
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
@@ -237,23 +237,23 @@
 name = "clap_lex"
 version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "98cc8fbded0c607b7ba9dd60cd98df59af97e84d24e49c8557331cfc26d301ce"
 
 [[package]]
 name = "colorchoice"
-version = "1.0.0"
+version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "acbf1af155f9b9ef647e42cdc158db4b64a1b61f743629225fde6f3e0be2a7c7"
+checksum = "0b6a852b24ab71dffc585bcb46eaf7959d175cb865a7152e35b348d1b2960422"
 
 [[package]]
 name = "deranged"
-version = "0.3.9"
+version = "0.3.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0f32d04922c60427da6f9fef14d042d9edddef64cb9d4ce0d64d0685fbeb1fd3"
+checksum = "b42b6fa04a440b495c8b04d0e71b707c585f83cb9cb28cf8cd0d976c315e31b4"
 dependencies = [
  "powerfmt",
 ]
 
 [[package]]
 name = "equivalent"
 version = "1.0.1"
@@ -294,98 +294,98 @@
 dependencies = [
  "lazy_static",
  "num",
 ]
 
 [[package]]
 name = "futures-channel"
-version = "0.3.29"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ff4dd66668b557604244583e3e1e1eada8c5c2e96a6d0d6653ede395b78bbacb"
+checksum = "eac8f7d7865dcb88bd4373ab671c8cf4508703796caa2b1985a9ca867b3fcb78"
 dependencies = [
  "futures-core",
  "futures-sink",
 ]
 
 [[package]]
 name = "futures-core"
-version = "0.3.29"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "eb1d22c66e66d9d72e1758f0bd7d4fd0bee04cad842ee34587d68c07e45d088c"
+checksum = "dfc6580bb841c5a68e9ef15c77ccc837b40a7504914d52e47b8b0e9bbda25a1d"
 
 [[package]]
 name = "futures-io"
-version = "0.3.29"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8bf34a163b5c4c52d0478a4d757da8fb65cabef42ba90515efee0f6f9fa45aaa"
+checksum = "a44623e20b9681a318efdd71c299b6b222ed6f231972bfe2f224ebad6311f0c1"
 
 [[package]]
 name = "futures-sink"
-version = "0.3.29"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e36d3378ee38c2a36ad710c5d30c2911d752cb941c00c72dbabfb786a7970817"
+checksum = "9fb8e00e87438d937621c1c6269e53f536c14d3fbd6a042bb24879e57d474fb5"
 
 [[package]]
 name = "futures-task"
-version = "0.3.29"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "efd193069b0ddadc69c46389b740bbccdd97203899b48d09c5f7969591d6bae2"
+checksum = "38d84fa142264698cdce1a9f9172cf383a0c82de1bddcf3092901442c4097004"
 
 [[package]]
 name = "futures-util"
-version = "0.3.29"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a19526d624e703a3179b3d322efec918b6246ea0fa51d41124525f00f1cc8104"
+checksum = "3d6401deb83407ab3da39eba7e33987a73c3df0c82b4bb5813ee871c19c41d48"
 dependencies = [
  "futures-core",
  "futures-io",
  "futures-sink",
  "futures-task",
  "memchr",
  "pin-project-lite",
  "pin-utils",
  "slab",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.10"
+version = "0.2.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "be4136b2a15dd319360be1c07d9933517ccf0be8f16bf62a3bee4f0d618df427"
+checksum = "c4567c8db10ae91089c99af84c68c38da3ec2f087c3f82960bcdbf3656b6f4d7"
 dependencies = [
  "cfg-if",
  "js-sys",
  "libc",
  "wasi",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "gimli"
-version = "0.28.0"
+version = "0.28.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6fb8d784f27acf97159b40fc4db5ecd8aa23b9ad5ef69cdd136d3bc80665f0c0"
+checksum = "4271d37baee1b8c7e4b708028c57d816cf9d2434acb33a549475f78c181f6253"
 
 [[package]]
 name = "hashbrown"
-version = "0.14.2"
+version = "0.14.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f93e7192158dbcda357bdec5fb5788eebf8bbac027f3f33e719d29135ae84156"
+checksum = "e5274423e17b7c9fc20b6e7e208532f9b19825d82dfd615708b70edd83df41f1"
 
 [[package]]
 name = "heck"
 version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2304e00983f87ffb38b55b444b5e3b60a884b5d30c0fca7d82fe33449bbe55ea"
 
 [[package]]
 name = "hermit-abi"
-version = "0.3.3"
+version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d77f7ec81a6d05a3abb01ab6eb7590f6083d08449fe5a1c8b1e620283546ccb7"
+checksum = "d231dfb89cfffdbc30e7fc41579ed6066ad03abda9e567ccafae602b97ec5024"
 
 [[package]]
 name = "http"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "21b9ddb458710bc376481b842f5da65cdf31522de232c1ca8146abce2a358258"
 dependencies = [
@@ -470,17 +470,17 @@
 dependencies = [
  "unicode-bidi",
  "unicode-normalization",
 ]
 
 [[package]]
 name = "indexmap"
-version = "2.0.2"
+version = "2.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8adf3ddd720272c6ea8bf59463c04e0f93d0bbf7c5439b691bca2987e0270897"
+checksum = "168fb715dda47215e360912c096649d23d58bf392ac62f73919e831745e40f26"
 dependencies = [
  "equivalent",
  "hashbrown",
 ]
 
 [[package]]
 name = "ipnet"
@@ -501,23 +501,23 @@
 checksum = "924e5d73ea28f59011fec52a0d12185d496a9b075d360657aed2a5707f701153"
 dependencies = [
  "nom",
 ]
 
 [[package]]
 name = "itoa"
-version = "1.0.9"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "af150ab688ff2122fcef229be89cb50dd66af9e01a4ff320cc137eecc9bacc38"
+checksum = "49f1f14873335454500d59611f1cf4a4b0f786f9ac11f4312a78e4cf2566695b"
 
 [[package]]
 name = "js-sys"
-version = "0.3.64"
+version = "0.3.69"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c5f195fe497f702db0f318b07fdd68edb16955aed830df8363d837542f8f935a"
+checksum = "29c15563dc2726973df627357ce0c9ddddbea194836909d655df6a75d2cf296d"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "jsonschema"
 version = "0.18.0"
@@ -552,33 +552,33 @@
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.149"
+version = "0.2.154"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a08173bc88b7955d1b3145aa561539096c421ac8debde8cbc3612ec635fee29b"
+checksum = "ae743338b92ff9146ce83992f766a31066a91a8c84a45e0e9f21e7cf6de6d346"
 
 [[package]]
 name = "lock_api"
-version = "0.4.11"
+version = "0.4.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c168f8615b12bc01f9c17e2eb0cc07dcae1940121185446edc3744920e8ef45"
+checksum = "07af8b9cdd281b7915f413fa73f29ebd5d55d0d3f0155584dade1ff18cea1b17"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
-version = "0.4.20"
+version = "0.4.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b5e6163cb8c49088c2c36f57875e58ccd8c87c7427f7fbd50ea6710b2f3f2e8f"
+checksum = "90ed8c1e510134f979dbc4f070f87d4313098b704861a105fe34231c70a3901c"
 
 [[package]]
 name = "memchr"
 version = "2.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6c8640c5d730cb13ebd907d8d04b52f55ac9a2eec55b440c8892f40d56c76c1d"
 
@@ -592,17 +592,17 @@
 name = "minimal-lexical"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "68354c5c6bd36d73ff3feceb05efa59b6acb7626617f4962be322a825e61f79a"
 
 [[package]]
 name = "miniz_oxide"
-version = "0.7.1"
+version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e7810e0be55b428ada41041c41f32c9f1a42817901b4ccf45fa3d4b6561e74c7"
+checksum = "9d811f3e15f28568be3407c8e7fdb6514c1cda3cb30683f15b6a1a1dc4ea14a7"
 dependencies = [
  "adler",
 ]
 
 [[package]]
 name = "mio"
 version = "0.8.11"
@@ -622,90 +622,93 @@
 dependencies = [
  "memchr",
  "minimal-lexical",
 ]
 
 [[package]]
 name = "num"
-version = "0.4.1"
+version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b05180d69e3da0e530ba2a1dae5110317e49e3b7f3d41be227dc5f92e49ee7af"
+checksum = "35bd024e8b2ff75562e5f34e7f4905839deb4b22955ef5e73d2fea1b9813cb23"
 dependencies = [
  "num-bigint",
  "num-complex",
  "num-integer",
  "num-iter",
  "num-rational",
  "num-traits",
 ]
 
 [[package]]
 name = "num-bigint"
-version = "0.4.4"
+version = "0.4.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "608e7659b5c3d7cba262d894801b9ec9d00de989e8a82bd4bef91d08da45cdc0"
+checksum = "c165a9ab64cf766f73521c0dd2cfdff64f488b8f0b3e621face3462d3db536d7"
 dependencies = [
- "autocfg",
  "num-integer",
  "num-traits",
 ]
 
 [[package]]
 name = "num-cmp"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "63335b2e2c34fae2fb0aa2cecfd9f0832a1e24b3b32ecec612c3426d46dc8aaa"
 
 [[package]]
 name = "num-complex"
-version = "0.4.4"
+version = "0.4.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1ba157ca0885411de85d6ca030ba7e2a83a28636056c7c699b07c8b6f7383214"
+checksum = "73f88a1307638156682bada9d7604135552957b7818057dcef22705b4d509495"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
+name = "num-conv"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "51d515d32fb182ee37cda2ccdcb92950d6a3c2893aa280e540671c2cd0f3b1d9"
+
+[[package]]
 name = "num-integer"
-version = "0.1.45"
+version = "0.1.46"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "225d3389fb3509a24c93f5c29eb6bde2586b98d9f016636dff58d7c6f7569cd9"
+checksum = "7969661fd2958a5cb096e56c8e1ad0444ac2bbcd0061bd28660485a44879858f"
 dependencies = [
- "autocfg",
  "num-traits",
 ]
 
 [[package]]
 name = "num-iter"
-version = "0.1.43"
+version = "0.1.45"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7d03e6c028c5dc5cac6e2dec0efda81fc887605bb3d884578bb6d6bf7514e252"
+checksum = "1429034a0490724d0075ebb2bc9e875d6503c3cf69e235a8941aa757d83ef5bf"
 dependencies = [
  "autocfg",
  "num-integer",
  "num-traits",
 ]
 
 [[package]]
 name = "num-rational"
-version = "0.4.1"
+version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0638a1c9d0a3c0914158145bc76cff373a75a627e6ecbfb71cbe6f453a5a19b0"
+checksum = "f83d14da390562dca69fc84082e73e548e1ad308d24accdedd2720017cb37824"
 dependencies = [
- "autocfg",
  "num-bigint",
  "num-integer",
  "num-traits",
 ]
 
 [[package]]
 name = "num-traits"
-version = "0.2.17"
+version = "0.2.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "39e3200413f237f41ab11ad6d161bc7239c84dcb631773ccd7de3dfe4b5c267c"
+checksum = "071dfc062690e90b734c0b2273ce72ad0ffa95f0c74596bc250dcfd960262841"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "num_cpus"
 version = "1.16.0"
@@ -714,17 +717,17 @@
 dependencies = [
  "hermit-abi",
  "libc",
 ]
 
 [[package]]
 name = "object"
-version = "0.32.1"
+version = "0.32.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9cf5f9dd3933bd50a9e1f149ec995f39ae2c496d31fd772c1fd45ebc27e902b0"
+checksum = "a6a622008b6e321afc04970976f62ee297fdbaa6f95318ca343e3eebb9648441"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "once_cell"
 version = "1.19.0"
@@ -740,33 +743,33 @@
  "log",
  "serde",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "parking_lot"
-version = "0.12.1"
+version = "0.12.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
+checksum = "7e4af0ca4f6caed20e900d564c242b8e5d4903fdacf31d3daf527b66fe6f42fb"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.9"
+version = "0.9.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c42a9226546d68acdd9c0a280d17ce19bfe27a46bf68784e4066115788d008e"
+checksum = "1e401f977ab385c9e4e3ab30627d6f26d00e2c73eef317493c4ec6d468726cf8"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-targets 0.48.5",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "percent-encoding"
 version = "2.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e3148f5046208a5d56bcfc03053e3ca6334e51da8dfb19b6cdc8b306fae3283e"
@@ -789,17 +792,17 @@
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pin-project-lite"
-version = "0.2.13"
+version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8afb450f006bf6385ca15ef45d71d2288452bc3683ce2e2cacc0d18e4be60b58"
+checksum = "bda66fc9667c18cb2758a2ac84d1167245054bcf85d5d1aaa6923f45801bdd02"
 
 [[package]]
 name = "pin-utils"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b870d8c151b6f2fb93e84a13146138f05d02ed11c7e7c54f8826aaaf7c9f184"
 
@@ -807,67 +810,67 @@
 name = "powerfmt"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "439ee305def115ba05938db6eb1644ff94165c5ab5e9420d1c1bcedbba909391"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.74"
+version = "1.0.82"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2de98502f212cfcea8d0bb305bd0f49d7ebdd75b64ba0a68f937d888f4e0d6db"
+checksum = "8ad3d49ab951a01fbaafe34f2ec74122942fe18a3f9814c3268f1bb72042131b"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.35"
+version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "291ec9ab5efd934aaf503a6466c5d5251535d108ee747472c3977cc5acc868ef"
+checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.4.1"
+version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
+checksum = "469052894dcb553421e483e4209ee581a45100d31b4018de03e5a7ad86374a7e"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "regex"
-version = "1.10.2"
+version = "1.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "380b951a9c5e80ddfd6136919eef32310721aa4aacd4889a8d39124b026ab343"
+checksum = "c117dbdfde9c8308975b6a18d71f3f385c89461f7b3fb054288ecf2a2058ba4c"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-automata",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-automata"
-version = "0.4.3"
+version = "0.4.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5f804c7828047e88b2d32e2d7fe5a105da8ee3264f01902f796c8e067dc2483f"
+checksum = "86b83b8b9847f9bf95ef68afb0b8e6cdb80f498442f5179a29fad448fcc1eaea"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.8.2"
+version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c08c74e62047bb2de4ff487b251e4a92e24f48745648451635cec7d591162d9f"
+checksum = "adad44e29e4c806119491a7f06f03de4d1af22c3a680dd47f1e6e179439d1f56"
 
 [[package]]
 name = "reqwest"
 version = "0.12.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "566cafdd92868e0939d3fb961bd0dc25fcfaaed179291093b3d43e6b3150ea10"
 dependencies = [
@@ -899,17 +902,17 @@
  "wasm-bindgen-futures",
  "web-sys",
  "winreg",
 ]
 
 [[package]]
 name = "rustc-demangle"
-version = "0.1.23"
+version = "0.1.24"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d626bb9dae77e28219937af045c257c28bfd3f69333c512553507f5f9798cb76"
+checksum = "719b953e2095829ee67db738b3bfa9fa368c94900df327b3f07fe6e794d2fe1f"
 
 [[package]]
 name = "rustc_version"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
 dependencies = [
@@ -924,29 +927,29 @@
 dependencies = [
  "rustc_version",
  "semver",
 ]
 
 [[package]]
 name = "ryu"
-version = "1.0.15"
+version = "1.0.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1ad4cc8da4ef723ed60bced201181d83791ad433213d8c24efffda1eec85d741"
+checksum = "f3cb5ba0dc43242ce17de99c180e96db90b235b8a9fdc9543c96d2209116bd9f"
 
 [[package]]
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "semver"
-version = "1.0.20"
+version = "1.0.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "836fa6a3e1e547f9a2c4040802ec865b5d85f4014efe00555d7090a3dcaa1090"
+checksum = "61697e0a1c7e512e84a621326239844a24d8207b4669b41bc18b32ea5cbf988b"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "serde"
 version = "1.0.201"
@@ -976,17 +979,17 @@
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
 name = "serde_spanned"
-version = "0.6.4"
+version = "0.6.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "12022b835073e5b11e90a14f86838ceb1c8fb0325b72416845c487ac0fa95e80"
+checksum = "eb3622f419d1296904700073ea6cc23ad690adbd66f13ea683df73298736f0c1"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "serde_urlencoded"
 version = "0.7.1"
@@ -1012,70 +1015,72 @@
 name = "smallvec"
 version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "socket2"
-version = "0.5.5"
+version = "0.5.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b5fac59a5cb5dd637972e5fca70daf0523c9067fcdc4842f053dae04a18f8e9"
+checksum = "ce305eb0b4296696835b71df73eb912e0f1ffd2556a501fcede6e0c50349191c"
 dependencies = [
  "libc",
- "windows-sys 0.48.0",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "strsim"
 version = "0.11.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7da8b5736845d9f2fcb837ea5d9e2628564b3b043a70948a3f0b778838c5fb4f"
 
 [[package]]
 name = "syn"
-version = "2.0.46"
+version = "2.0.61"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "89456b690ff72fddcecf231caedbe615c59480c93358a93dfae7fc29e3ebbf0e"
+checksum = "c993ed8ccba56ae856363b1845da7266a7cb78e1d146c8a32d54b45a8b831fc9"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "sync_wrapper"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2047c6ded9c721764247e62cd3b03c09ffc529b2ba5b10ec482ae507a4a70160"
 
 [[package]]
 name = "time"
-version = "0.3.30"
+version = "0.3.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c4a34ab300f2dee6e562c10a046fc05e358b29f9bf92277f30c3c8d82275f6f5"
+checksum = "5dfd88e563464686c916c7e46e623e520ddc6d79fa6641390f2e3fa86e83e885"
 dependencies = [
  "deranged",
+ "num-conv",
  "powerfmt",
  "serde",
  "time-core",
  "time-macros",
 ]
 
 [[package]]
 name = "time-core"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ef927ca75afb808a4d64dd374f00a2adf8d0fcff8e7b184af886c3c87ec4a3f3"
 
 [[package]]
 name = "time-macros"
-version = "0.2.15"
+version = "0.2.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4ad70d68dba9e1f8aceda7aa6711965dfec1cac869f311a51bd08b3a2ccbce20"
+checksum = "3f252a68540fde3a3877aeea552b832b40ab9a69e318efd078774a01ddee1ccf"
 dependencies = [
+ "num-conv",
  "time-core",
 ]
 
 [[package]]
 name = "tinyvec"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1088,17 +1093,17 @@
 name = "tinyvec_macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
 
 [[package]]
 name = "tokio"
-version = "1.33.0"
+version = "1.37.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4f38200e3ef7995e5ef13baec2f432a6da0aa9ac495b2c0e8f3b7eec2c92d653"
+checksum = "1adbebffeca75fcfd058afa480fb6c0b81e165a0323f9c9d39c9697e37c46787"
 dependencies = [
  "backtrace",
  "libc",
  "mio",
  "num_cpus",
  "pin-project-lite",
  "socket2",
@@ -1185,35 +1190,35 @@
 checksum = "c06d3da6113f116aaee68e4d601191614c9053067f9ab7f6edbcb161237daa54"
 dependencies = [
  "once_cell",
 ]
 
 [[package]]
 name = "try-lock"
-version = "0.2.4"
+version = "0.2.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3528ecfd12c466c6f163363caf2d02a71161dd5e1cc6ae7b34207ea2d42d81ed"
+checksum = "e421abadd41a4225275504ea4d6566923418b7f05506fbc9c0fe86ba7396114b"
 
 [[package]]
 name = "unicode-bidi"
-version = "0.3.13"
+version = "0.3.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "92888ba5573ff080736b3648696b70cafad7d250551175acbaa4e0385b3e1460"
+checksum = "08f95100a766bf4f8f28f90d77e0a5461bbdb219042e7679bebe79004fed8d75"
 
 [[package]]
 name = "unicode-ident"
 version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3354b9ac3fae1ff6755cb6db53683adb661634f67557942dea4facebec0fee4b"
 
 [[package]]
 name = "unicode-normalization"
-version = "0.1.22"
+version = "0.1.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5c5713f0fc4b5db668a2ac63cdb7bb4469d8c9fed047b1d0292cc7b0ce2ba921"
+checksum = "a56d1686db2308d901306f92a263857ef59ea39678a5458e7cb17f01415101f5"
 dependencies = [
  "tinyvec",
 ]
 
 [[package]]
 name = "url"
 version = "2.5.0"
@@ -1229,17 +1234,17 @@
 name = "utf8parse"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "711b9620af191e0cdc7468a8d14e709c3dcdb115b36f838e601583af800a370a"
 
 [[package]]
 name = "uuid"
-version = "1.5.0"
+version = "1.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "88ad59a7560b41a70d191093a945f0b87bc1deeda46fb237479708a1d6b6cdfc"
+checksum = "a183cf7feeba97b4dd1c0d46788634f6221d87fa961b305bed08c851829efcc0"
 
 [[package]]
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
 
@@ -1256,83 +1261,83 @@
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wasm-bindgen"
-version = "0.2.87"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7706a72ab36d8cb1f80ffbf0e071533974a60d0a308d01a5d0375bf60499a342"
+checksum = "4be2531df63900aeb2bca0daaaddec08491ee64ceecbee5076636a3b026795a8"
 dependencies = [
  "cfg-if",
  "wasm-bindgen-macro",
 ]
 
 [[package]]
 name = "wasm-bindgen-backend"
-version = "0.2.87"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5ef2b6d3c510e9625e5fe6f509ab07d66a760f0885d858736483c32ed7809abd"
+checksum = "614d787b966d3989fa7bb98a654e369c762374fd3213d212cfc0251257e747da"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
  "syn",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-futures"
-version = "0.4.37"
+version = "0.4.42"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c02dbc21516f9f1f04f187958890d7e6026df8d16540b7ad9492bc34a67cea03"
+checksum = "76bc14366121efc8dbb487ab05bcc9d346b3b5ec0eaa76e46594cabbe51762c0"
 dependencies = [
  "cfg-if",
  "js-sys",
  "wasm-bindgen",
  "web-sys",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
-version = "0.2.87"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dee495e55982a3bd48105a7b947fd2a9b4a8ae3010041b9e0faab3f9cd028f1d"
+checksum = "a1f8823de937b71b9460c0c34e25f3da88250760bec0ebac694b49997550d726"
 dependencies = [
  "quote",
  "wasm-bindgen-macro-support",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro-support"
-version = "0.2.87"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "54681b18a46765f095758388f2d0cf16eb8d4169b639ab575a8f5693af210c7b"
+checksum = "e94f17b526d0a461a191c78ea52bbce64071ed5c04c9ffe424dcb38f74171bb7"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
-version = "0.2.87"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ca6ad05a4870b2bf5fe995117d3728437bd27d7cd5f06f13c17443ef369775a1"
+checksum = "af190c94f2773fdb3729c55b007a722abb5384da03bc0986df4c289bf5567e96"
 
 [[package]]
 name = "web-sys"
-version = "0.3.64"
+version = "0.3.69"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9b85cbef8c220a6abc02aefd892dfc0fc23afb1c6a426316ec33253a3877249b"
+checksum = "77afa9a11836342370f4817622a2f0f418b134426d91a82dfb48f532d2ec13ef"
 dependencies = [
  "js-sys",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "windows-sys"
@@ -1345,15 +1350,15 @@
 
 [[package]]
 name = "windows-sys"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "282be5f36a8ce781fad8c8ae18fa3f9beff57ec1b52cb3de0789201425d9a33d"
 dependencies = [
- "windows-targets 0.52.4",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
@@ -1365,116 +1370,123 @@
  "windows_x86_64_gnu 0.48.5",
  "windows_x86_64_gnullvm 0.48.5",
  "windows_x86_64_msvc 0.48.5",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7dd37b7e5ab9018759f893a1952c9420d060016fc19a472b4bb20d1bdd694d1b"
+checksum = "6f0713a46559409d202e70e28227288446bf7841d3211583a4b53e3f6d96e7eb"
 dependencies = [
- "windows_aarch64_gnullvm 0.52.4",
- "windows_aarch64_msvc 0.52.4",
- "windows_i686_gnu 0.52.4",
- "windows_i686_msvc 0.52.4",
- "windows_x86_64_gnu 0.52.4",
- "windows_x86_64_gnullvm 0.52.4",
- "windows_x86_64_msvc 0.52.4",
+ "windows_aarch64_gnullvm 0.52.5",
+ "windows_aarch64_msvc 0.52.5",
+ "windows_i686_gnu 0.52.5",
+ "windows_i686_gnullvm",
+ "windows_i686_msvc 0.52.5",
+ "windows_x86_64_gnu 0.52.5",
+ "windows_x86_64_gnullvm 0.52.5",
+ "windows_x86_64_msvc 0.52.5",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bcf46cf4c365c6f2d1cc93ce535f2c8b244591df96ceee75d8e83deb70a9cac9"
+checksum = "7088eed71e8b8dda258ecc8bac5fb1153c5cffaf2578fc8ff5d61e23578d3263"
 
 [[package]]
 name = "windows_aarch64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da9f259dd3bcf6990b55bffd094c4f7235817ba4ceebde8e6d11cd0c5633b675"
+checksum = "9985fd1504e250c615ca5f281c3f7a6da76213ebd5ccc9561496568a2752afb6"
 
 [[package]]
 name = "windows_i686_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.52.4"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "88ba073cf16d5372720ec942a8ccbf61626074c6d4dd2e745299726ce8b89670"
+
+[[package]]
+name = "windows_i686_gnullvm"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b474d8268f99e0995f25b9f095bc7434632601028cf86590aea5c8a5cb7801d3"
+checksum = "87f4261229030a858f36b459e748ae97545d6f1ec60e5e0d6a3d32e0dc232ee9"
 
 [[package]]
 name = "windows_i686_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1515e9a29e5bed743cb4415a9ecf5dfca648ce85ee42e15873c3cd8610ff8e02"
+checksum = "db3c2bf3d13d5b658be73463284eaf12830ac9a26a90c717b7f771dfe97487bf"
 
 [[package]]
 name = "windows_x86_64_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5eee091590e89cc02ad514ffe3ead9eb6b660aedca2183455434b93546371a03"
+checksum = "4e4246f76bdeff09eb48875a0fd3e2af6aada79d409d33011886d3e1581517d9"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "77ca79f2451b49fa9e2af39f0747fe999fcda4f5e241b2898624dca97a1f2177"
+checksum = "852298e482cd67c356ddd9570386e2862b5673c85bd5f88df9ab6802b334c596"
 
 [[package]]
 name = "windows_x86_64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "32b752e52a2da0ddfbdbcc6fceadfeede4c939ed16d13e648833a61dfb611ed8"
+checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
 
 [[package]]
 name = "winnow"
-version = "0.5.18"
+version = "0.5.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "176b6138793677221d420fd2f0aeeced263f197688b36484660da767bca2fa32"
+checksum = "f593a95398737aeed53e489c785df13f3618e41dbcd6718c6addbf1395aa6876"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "winreg"
 version = "0.52.0"
@@ -1483,24 +1495,24 @@
 dependencies = [
  "cfg-if",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "zerocopy"
-version = "0.7.31"
+version = "0.7.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1c4061bedbb353041c12f413700357bec76df2c7e2ca8e4df8bac24c6bf68e3d"
+checksum = "ae87e3fcd617500e5d106f0380cf7b77f3c6092aae37191433159dda23cfb087"
 dependencies = [
  "zerocopy-derive",
 ]
 
 [[package]]
 name = "zerocopy-derive"
-version = "0.7.31"
+version = "0.7.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b3c129550b3e6de3fd0ba67ba5c81818f9805e58b8d7fee80a3a59d2c9fc601a"
+checksum = "15e934569e47891f7d9411f1a451d947a60e000ab3bd24fbb970f000387d1b3b"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
```

### Comparing `bowtie_json_schema-2024.5.5/implementations/rust-jsonschema/Dockerfile` & `bowtie_json_schema-2024.5.7/implementations/rust-jsonschema/Dockerfile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/implementations/rust-jsonschema/src/main.rs` & `bowtie_json_schema-2024.5.7/implementations/rust-jsonschema/src/main.rs`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/implementations/scala-mjs-validator/Harness.scala` & `bowtie_json_schema-2024.5.7/implementations/scala-mjs-validator/Harness.scala`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/implementations/scala-mjs-validator/build.sbt` & `bowtie_json_schema-2024.5.7/implementations/scala-mjs-validator/build.sbt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/implementations/scala-rc-circe-json-validator/Harness.scala` & `bowtie_json_schema-2024.5.7/implementations/scala-rc-circe-json-validator/Harness.scala`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/implementations/scala-rc-circe-json-validator/build.sbt` & `bowtie_json_schema-2024.5.7/implementations/scala-rc-circe-json-validator/build.sbt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/implementations/ts-vscode-json-languageservice/bowtie_jsonls.ts` & `bowtie_json_schema-2024.5.7/implementations/ts-vscode-json-languageservice/bowtie_jsonls.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/tests/test_connectables.py` & `bowtie_json_schema-2024.5.7/tests/test_connectables.py`

 * *Files 12% similar despite different names*

```diff
@@ -45,14 +45,34 @@
     connectable = Connectable.from_str(id)
     assert connectable == Connectable(
         id=id,
         connector=ConnectableImage(id=f"{IMAGE_REPOSITORY}/bar"),
     )
 
 
+def test_explicit_image_with_repository_and_tag():
+    id = "image:foo/bar:latest"
+    validator.validate(id)
+    connectable = Connectable.from_str(id)
+    assert connectable == Connectable(
+        id=id,
+        connector=ConnectableImage(id="foo/bar:latest"),
+    )
+
+
+def test_implicit_image_with_repository_and_tag():
+    id = "foo/bar:latest"
+    validator.validate(id)
+    connectable = Connectable.from_str(id)
+    assert connectable == Connectable(
+        id=id,
+        connector=ConnectableImage(id="foo/bar:latest"),
+    )
+
+
 def test_unknown_connector():
     id = "asdf:foo"
     validator.invalidate(id)
     with pytest.raises(UnknownConnector):
         Connectable.from_str(id)
```

### Comparing `bowtie_json_schema-2024.5.5/tests/test_github.py` & `bowtie_json_schema-2024.5.7/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/tests/test_hypothesis.py` & `bowtie_json_schema-2024.5.7/tests/test_hypothesis.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/tests/test_integration.py` & `bowtie_json_schema-2024.5.7/tests/test_integration.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 
 
 HERE = Path(__file__).parent
 FAUXMPLEMENTATIONS = HERE / "fauxmplementations"
 
 # Make believe we're wide for tests to avoid line breaks in rich-click.
 WIDE_TERMINAL_ENV = dict(os.environ, TERMINAL_WIDTH="512")
+WIDE_TERMINAL_ENV.pop("CI", None)  # Run subprocesses as if they're not in CI
 
 
 def tag(name: str):
     return f"bowtie-integration-tests/{name}"
 
 
 async def command_validator(command):
```

### Comparing `bowtie_json_schema-2024.5.5/tests/test_registry.py` & `bowtie_json_schema-2024.5.7/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/tests/test_report.py` & `bowtie_json_schema-2024.5.7/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/tests/test_schemas.py` & `bowtie_json_schema-2024.5.7/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/tests/fauxmplementations/envsonschema/envsonschema` & `bowtie_json_schema-2024.5.7/tests/fauxmplementations/envsonschema/envsonschema`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/tests/fauxmplementations/lintsonschema/lintsonschema` & `bowtie_json_schema-2024.5.7/tests/fauxmplementations/lintsonschema/lintsonschema`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/tests/fauxmplementations/lintsonschema/schemas/connectables.json` & `bowtie_json_schema-2024.5.7/tests/fauxmplementations/lintsonschema/schemas/connectables.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761904761904762%*

 * *Differences: {"'oneOf'": "{insert: [(1, OrderedDict([('title', 'Implicit Image With Repository & Tag'), "*

 * *            "('pattern', '^[^:/]+/[^:/]+:[^:/]+$')]))]}"}*

```diff
@@ -12,14 +12,18 @@
     "description": "A mini-language for connecting to supported harnesses.",
     "oneOf": [
         {
             "pattern": "^[^:]+$",
             "title": "Implicit Image"
         },
         {
+            "pattern": "^[^:/]+/[^:/]+:[^:/]+$",
+            "title": "Implicit Image With Repository & Tag"
+        },
+        {
             "description": "A connectable with explicit connector.",
             "oneOf": [
                 {
                     "$ref": "#image"
                 }
             ],
             "pattern": "^[^:]+:[^:]+(:[^:]+)?$",
```

### Comparing `bowtie_json_schema-2024.5.5/tests/fauxmplementations/lintsonschema/schemas/report.json` & `bowtie_json_schema-2024.5.7/tests/fauxmplementations/lintsonschema/schemas/report.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/tests/fauxmplementations/lintsonschema/schemas/cli/info.json` & `bowtie_json_schema-2024.5.7/tests/fauxmplementations/lintsonschema/schemas/cli/info.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/tests/fauxmplementations/lintsonschema/schemas/cli/smoke.json` & `bowtie_json_schema-2024.5.7/tests/fauxmplementations/lintsonschema/schemas/cli/smoke.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/tests/fauxmplementations/lintsonschema/schemas/cli/summary.json` & `bowtie_json_schema-2024.5.7/tests/fauxmplementations/lintsonschema/schemas/cli/summary.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/tests/fauxmplementations/lintsonschema/schemas/io/v1.json` & `bowtie_json_schema-2024.5.7/tests/fauxmplementations/lintsonschema/schemas/io/v1.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/tests/fauxmplementations/lintsonschema/schemas/io/commands/dialect.json` & `bowtie_json_schema-2024.5.7/tests/fauxmplementations/lintsonschema/schemas/io/commands/dialect.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/tests/fauxmplementations/lintsonschema/schemas/io/commands/run.json` & `bowtie_json_schema-2024.5.7/tests/fauxmplementations/lintsonschema/schemas/io/commands/run.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/tests/fauxmplementations/lintsonschema/schemas/io/commands/start.json` & `bowtie_json_schema-2024.5.7/tests/fauxmplementations/lintsonschema/schemas/io/commands/start.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/tests/fauxmplementations/lintsonschema/schemas/models/dialect.json` & `bowtie_json_schema-2024.5.7/tests/fauxmplementations/lintsonschema/schemas/models/dialect.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/tests/fauxmplementations/lintsonschema/schemas/models/group.json` & `bowtie_json_schema-2024.5.7/tests/fauxmplementations/lintsonschema/schemas/models/group.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/tests/fauxmplementations/lintsonschema/schemas/models/implementation.json` & `bowtie_json_schema-2024.5.7/tests/fauxmplementations/lintsonschema/schemas/models/implementation.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/tests/fauxmplementations/lintsonschema/schemas/models/test.json` & `bowtie_json_schema-2024.5.7/tests/fauxmplementations/lintsonschema/schemas/models/test.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/.gitignore` & `bowtie_json_schema-2024.5.7/.gitignore`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/LICENSE` & `bowtie_json_schema-2024.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/README.rst` & `bowtie_json_schema-2024.5.7/README.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/hatch_build.py` & `bowtie_json_schema-2024.5.7/hatch_build.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/pyproject.toml` & `bowtie_json_schema-2024.5.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.5/PKG-INFO` & `bowtie_json_schema-2024.5.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bowtie-json-schema
-Version: 2024.5.5
+Version: 2024.5.7
 Summary: A meta-validator for the JSON Schema specification.
 Project-URL: Documentation, https://docs.bowtie.report/
 Project-URL: Homepage, https://bowtie.report/
 Project-URL: Issues, https://github.com/bowtie-json-schema/bowtie/issues/
 Project-URL: Funding, https://github.com/sponsors/Julian
 Project-URL: Source, https://github.com/bowtie-json-schema/bowtie
 Author-email: Julian Berman <Julian+bowtie@GrayVines.com>
```

