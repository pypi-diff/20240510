# Comparing `tmp/pyconcept-0.1.3.tar.gz` & `tmp/pyconcept-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyconcept-0.1.3.tar", last modified: Tue May  7 23:18:13 2024, max compression
+gzip compressed data, was "pyconcept-0.1.4.tar", last modified: Thu May  9 23:28:41 2024, max compression
```

## Comparing `pyconcept-0.1.3.tar` & `pyconcept-0.1.4.tar`

### file list

```diff
@@ -1,282 +1,282 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.603200 pyconcept-0.1.3/
--rw-rw-rw-   0        0        0      637 2024-04-18 12:02:25.000000 pyconcept-0.1.3/CHANGELOG.md
--rw-rw-rw-   0        0        0      955 2024-04-19 23:54:16.000000 pyconcept-0.1.3/CMakeLists.txt
--rw-rw-rw-   0        0        0     1101 2024-04-15 19:05:00.000000 pyconcept-0.1.3/LICENSE
--rw-rw-rw-   0        0        0      162 2024-04-18 08:33:28.000000 pyconcept-0.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0      953 2024-05-07 23:18:13.603200 pyconcept-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      115 2024-04-17 11:33:45.000000 pyconcept-0.1.3/README.md
--rw-rw-rw-   0        0        0        5 2024-05-07 23:12:08.000000 pyconcept-0.1.3/VERSION
-drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.288475 pyconcept-0.1.3/ccl/
--rw-rw-rw-   0        0        0     2133 2024-04-17 08:48:56.000000 pyconcept-0.1.3/ccl/CMakeLists.txt
-drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.259911 pyconcept-0.1.3/ccl/cclCommons/
-drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.259911 pyconcept-0.1.3/ccl/cclCommons/include/
-drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.291475 pyconcept-0.1.3/ccl/cclCommons/include/ccl/
--rw-rw-rw-   0        0        0    10473 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/cclCommons/include/ccl/Strings.hpp
--rw-rw-rw-   0        0        0      895 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/cclCommons/include/ccl/Substitutes.hpp
--rw-rw-rw-   0        0        0     1506 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/cclCommons/include/ccl/cclChange.hpp
--rw-rw-rw-   0        0        0    11710 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/cclCommons/include/ccl/cclMeta.hpp
--rw-rw-rw-   0        0        0     6078 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/cclCommons/include/ccl/cclTypes.hpp
-drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.260912 pyconcept-0.1.3/ccl/cclGraph/
-drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.260912 pyconcept-0.1.3/ccl/cclGraph/include/
-drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.292476 pyconcept-0.1.3/ccl/cclGraph/include/ccl/
--rw-rw-rw-   0        0        0     2749 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/cclGraph/include/ccl/Entity.hpp
-drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.293475 pyconcept-0.1.3/ccl/cclGraph/include/ccl/graph/
--rw-rw-rw-   0        0        0     2907 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/cclGraph/include/ccl/graph/CGraph.h
-drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.293475 pyconcept-0.1.3/ccl/cclGraph/src/
--rw-rw-rw-   0        0        0     9187 2024-05-06 12:39:34.000000 pyconcept-0.1.3/ccl/cclGraph/src/CGraph.cpp
-drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.261911 pyconcept-0.1.3/ccl/cclLang/
-drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.261911 pyconcept-0.1.3/ccl/cclLang/include/
-drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.261911 pyconcept-0.1.3/ccl/cclLang/include/ccl/
-drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.302476 pyconcept-0.1.3/ccl/cclLang/include/ccl/lang/
--rw-rw-rw-   0        0        0     1191 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/cclLang/include/ccl/lang/EntityTermContext.hpp
--rw-rw-rw-   0        0        0     1941 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/cclLang/include/ccl/lang/LexicalTerm.h
--rw-rw-rw-   0        0        0      345 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/cclLang/include/ccl/lang/Literals.h
--rw-rw-rw-   0        0        0     1327 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/cclLang/include/ccl/lang/ManagedText.h
--rw-rw-rw-   0        0        0     8108 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/cclLang/include/ccl/lang/Morphology.h
--rw-rw-rw-   0        0        0     2748 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/cclLang/include/ccl/lang/Reference.h
--rw-rw-rw-   0        0        0     2766 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/cclLang/include/ccl/lang/RefsManager.h
--rw-rw-rw-   0        0        0      514 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/cclLang/include/ccl/lang/TextEnvironment.h
--rw-rw-rw-   0        0        0     1278 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/cclLang/include/ccl/lang/TextProcessor.h
-drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.308475 pyconcept-0.1.3/ccl/cclLang/src/
--rw-rw-rw-   0        0        0     2111 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/cclLang/src/LexicalTerm.cpp
--rw-rw-rw-   0        0        0      307 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/cclLang/src/Literals.cpp
--rw-rw-rw-   0        0        0     2016 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/cclLang/src/ManagedText.cpp
--rw-rw-rw-   0        0        0     2239 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/cclLang/src/Morphology.cpp
--rw-rw-rw-   0        0        0     7475 2024-05-06 12:47:43.000000 pyconcept-0.1.3/ccl/cclLang/src/Reference.cpp
--rw-rw-rw-   0        0        0     6529 2024-05-06 12:48:14.000000 pyconcept-0.1.3/ccl/cclLang/src/RefsManager.cpp
--rw-rw-rw-   0        0        0      452 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/cclLang/src/TextEnvironment.cpp
--rw-rw-rw-   0        0        0     1581 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/cclLang/src/TextProcessor.cpp
-drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.309476 pyconcept-0.1.3/ccl/cclLang/unity/
--rw-rw-rw-   0        0        0      309 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/cclLang/unity/cclLang.cpp
-drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.310475 pyconcept-0.1.3/ccl/cmake/
--rw-rw-rw-   0        0        0     1541 2024-04-19 23:11:05.000000 pyconcept-0.1.3/ccl/cmake/CXXTargets.cmake
--rw-rw-rw-   0        0        0       93 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/conanfile.txt
-drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.267910 pyconcept-0.1.3/ccl/core/
-drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.263912 pyconcept-0.1.3/ccl/core/include/
-drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.312474 pyconcept-0.1.3/ccl/core/include/ccl/
--rw-rw-rw-   0        0        0     2124 2024-05-06 15:23:11.000000 pyconcept-0.1.3/ccl/core/include/ccl/Operation.hpp
--rw-rw-rw-   0        0        0     5309 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/include/ccl/Source.hpp
-drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.313477 pyconcept-0.1.3/ccl/core/include/ccl/api/
--rw-rw-rw-   0        0        0      915 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/include/ccl/api/RSFormJA.h
-drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.314475 pyconcept-0.1.3/ccl/core/include/ccl/env/
--rw-rw-rw-   0        0        0     2904 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/include/ccl/env/SourceManager.hpp
--rw-rw-rw-   0        0        0      624 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/include/ccl/env/cclEnvironment.h
-drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.317476 pyconcept-0.1.3/ccl/core/include/ccl/ops/
--rw-rw-rw-   0        0        0     1998 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/include/ccl/ops/EquationOptions.h
--rw-rw-rw-   0        0        0      850 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/include/ccl/ops/RSAggregator.h
--rw-rw-rw-   0        0        0     1187 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/include/ccl/ops/RSEquationProcessor.h
--rw-rw-rw-   0        0        0     3525 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/include/ccl/ops/RSOperations.h
-drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.323475 pyconcept-0.1.3/ccl/core/include/ccl/oss/
--rw-rw-rw-   0        0        0     4161 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/include/ccl/oss/OSSchema.h
--rw-rw-rw-   0        0        0     1658 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/include/ccl/oss/OperationProcessor.hpp
--rw-rw-rw-   0        0        0      903 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/include/ccl/oss/Pict.hpp
--rw-rw-rw-   0        0        0      934 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/include/ccl/oss/RSSynthesProcessor.h
--rw-rw-rw-   0        0        0     1363 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/include/ccl/oss/ossGraphFacet.h
--rw-rw-rw-   0        0        0     2334 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/include/ccl/oss/ossGridFacet.h
--rw-rw-rw-   0        0        0     2979 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/include/ccl/oss/ossOperationsFacet.h
--rw-rw-rw-   0        0        0     2469 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/include/ccl/oss/ossSourceFacet.h
-drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.362672 pyconcept-0.1.3/ccl/core/include/ccl/semantic/
--rw-rw-rw-   0        0        0      622 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/include/ccl/semantic/ConceptRecord.h
--rw-rw-rw-   0        0        0     1473 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/include/ccl/semantic/CstFilters.hpp
--rw-rw-rw-   0        0        0     2367 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/include/ccl/semantic/CstList.h
--rw-rw-rw-   0        0        0     2523 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/include/ccl/semantic/CstType.hpp
--rw-rw-rw-   0        0        0     1231 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/include/ccl/semantic/IdentityManager.h
--rw-rw-rw-   0        0        0      962 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/include/ccl/semantic/InterpretationStorage.h
--rw-rw-rw-   0        0        0     1095 2024-05-06 14:59:52.000000 pyconcept-0.1.3/ccl/core/include/ccl/semantic/RSConcept.h
--rw-rw-rw-   0        0        0     3584 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/include/ccl/semantic/RSCore.h
--rw-rw-rw-   0        0        0     3430 2024-05-06 15:04:15.000000 pyconcept-0.1.3/ccl/core/include/ccl/semantic/RSForm.h
--rw-rw-rw-   0        0        0     3012 2024-05-06 15:04:05.000000 pyconcept-0.1.3/ccl/core/include/ccl/semantic/RSModel.h
--rw-rw-rw-   0        0        0     5074 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/include/ccl/semantic/Schema.h
--rw-rw-rw-   0        0        0     1122 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/include/ccl/semantic/TextConcept.h
--rw-rw-rw-   0        0        0     2603 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/include/ccl/semantic/TextData.hpp
--rw-rw-rw-   0        0        0     3988 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/include/ccl/semantic/Thesaurus.h
--rw-rw-rw-   0        0        0     1577 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/include/ccl/semantic/rsCalculationFacet.h
--rw-rw-rw-   0        0        0     1648 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/include/ccl/semantic/rsModificationFacet.h
--rw-rw-rw-   0        0        0     1099 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/include/ccl/semantic/rsOperationFacet.h
--rw-rw-rw-   0        0        0     1867 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/include/ccl/semantic/rsValuesFacet.h
-drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.392677 pyconcept-0.1.3/ccl/core/include/ccl/tools/
--rw-rw-rw-   0        0        0      894 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/include/ccl/tools/CstNameGenerator.h
--rw-rw-rw-   0        0        0      523 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/include/ccl/tools/EntityGenerator.h
--rw-rw-rw-   0        0        0     2935 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/include/ccl/tools/EnumJSON.hpp
--rw-rw-rw-   0        0        0     3871 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/include/ccl/tools/JSON.h
-drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.393672 pyconcept-0.1.3/ccl/core/include/nlohmann/
--rw-rw-rw-   0        0        0   945021 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/include/nlohmann/json.hpp
-drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.395672 pyconcept-0.1.3/ccl/core/src/
--rw-rw-rw-   0        0        0    18448 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/src/JSON.cpp
-drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.403672 pyconcept-0.1.3/ccl/core/src/api/
--rw-rw-rw-   0        0        0     3026 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/src/api/RSFormJA.cpp
-drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.405674 pyconcept-0.1.3/ccl/core/src/env/
--rw-rw-rw-   0        0        0      636 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/src/env/cclEnvironment.cpp
-drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.416672 pyconcept-0.1.3/ccl/core/src/ops/
--rw-rw-rw-   0        0        0     1772 2024-05-06 14:58:07.000000 pyconcept-0.1.3/ccl/core/src/ops/EquationOptions.cpp
--rw-rw-rw-   0        0        0     4124 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/src/ops/RSAggregator.cpp
--rw-rw-rw-   0        0        0     4290 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/src/ops/RSEquationProcessor.cpp
--rw-rw-rw-   0        0        0    16240 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/src/ops/RSOperations.cpp
-drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.421673 pyconcept-0.1.3/ccl/core/src/oss/
--rw-rw-rw-   0        0        0     7258 2024-05-06 15:10:47.000000 pyconcept-0.1.3/ccl/core/src/oss/OSSchema.cpp
--rw-rw-rw-   0        0        0     2812 2024-05-06 15:23:33.000000 pyconcept-0.1.3/ccl/core/src/oss/RSSynthesProcessor.cpp
--rw-rw-rw-   0        0        0     4305 2024-05-06 15:06:48.000000 pyconcept-0.1.3/ccl/core/src/oss/ossGraphFacet.cpp
--rw-rw-rw-   0        0        0     3023 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/src/oss/ossGridFacet.cpp
--rw-rw-rw-   0        0        0    11652 2024-05-06 15:05:23.000000 pyconcept-0.1.3/ccl/core/src/oss/ossOperationsFacet.cpp
--rw-rw-rw-   0        0        0    10397 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/src/oss/ossSourceFacet.cpp
-drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.267910 pyconcept-0.1.3/ccl/core/src/semantic/
-drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.440267 pyconcept-0.1.3/ccl/core/src/semantic/rscore/
--rw-rw-rw-   0        0        0      588 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/src/semantic/rscore/ConceptRecord.cpp
--rw-rw-rw-   0        0        0     3957 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/src/semantic/rscore/CstList.cpp
--rw-rw-rw-   0        0        0     1950 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/src/semantic/rscore/IdentityManager.cpp
--rw-rw-rw-   0        0        0    10403 2024-05-06 15:01:20.000000 pyconcept-0.1.3/ccl/core/src/semantic/rscore/RSCore.cpp
-drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.442268 pyconcept-0.1.3/ccl/core/src/semantic/rsform/
--rw-rw-rw-   0        0        0     8112 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/src/semantic/rsform/RSForm.cpp
--rw-rw-rw-   0        0        0     1573 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/src/semantic/rsform/rsModificationFacet.cpp
--rw-rw-rw-   0        0        0     2431 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/src/semantic/rsform/rsOperationFacet.cpp
-drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.445266 pyconcept-0.1.3/ccl/core/src/semantic/rsmodel/
--rw-rw-rw-   0        0        0     1591 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/src/semantic/rsmodel/InterpretationStorage.cpp
--rw-rw-rw-   0        0        0     4755 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/src/semantic/rsmodel/RSModel.cpp
--rw-rw-rw-   0        0        0     3954 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/src/semantic/rsmodel/rsCalculationFacet.cpp
--rw-rw-rw-   0        0        0     6866 2024-05-06 13:08:18.000000 pyconcept-0.1.3/ccl/core/src/semantic/rsmodel/rsValuesFacet.cpp
-drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.446267 pyconcept-0.1.3/ccl/core/src/semantic/schema/
--rw-rw-rw-   0        0        0      830 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/src/semantic/schema/RSConcept.cpp
--rw-rw-rw-   0        0        0    13468 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/src/semantic/schema/Schema.cpp
-drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.448269 pyconcept-0.1.3/ccl/core/src/semantic/thesaurus/
--rw-rw-rw-   0        0        0      919 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/src/semantic/thesaurus/TextConcept.cpp
--rw-rw-rw-   0        0        0    10089 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/src/semantic/thesaurus/Thesaurus.cpp
-drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.450267 pyconcept-0.1.3/ccl/core/src/tools/
--rw-rw-rw-   0        0        0     2682 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/src/tools/CstNameGenerator.cpp
--rw-rw-rw-   0        0        0      773 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/src/tools/EntityGenerator.cpp
-drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.450267 pyconcept-0.1.3/ccl/core/unity/
--rw-rw-rw-   0        0        0     1448 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/core/unity/CCL.cpp
-drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.272910 pyconcept-0.1.3/ccl/rslang/
-drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.470832 pyconcept-0.1.3/ccl/rslang/header/
--rw-rw-rw-   0        0        0     1363 2024-05-06 10:35:16.000000 pyconcept-0.1.3/ccl/rslang/header/ASTNormalizer.h
--rw-rw-rw-   0        0        0    34735 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/header/AsciiLexerImpl.hpp
--rw-rw-rw-   0        0        0     2359 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/header/GeneratorImplAST.h
--rw-rw-rw-   0        0        0    35507 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/header/MathLexerImpl.hpp
--rw-rw-rw-   0        0        0      958 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/header/NameCollector.h
--rw-rw-rw-   0        0        0    32035 2024-05-05 13:23:08.000000 pyconcept-0.1.3/ccl/rslang/header/RSParserImpl.h
--rw-rw-rw-   0        0        0     5446 2024-05-05 13:20:57.000000 pyconcept-0.1.3/ccl/rslang/header/SDImplementation.h
-drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.269911 pyconcept-0.1.3/ccl/rslang/import/
-drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.270910 pyconcept-0.1.3/ccl/rslang/import/reflex/
-drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.269911 pyconcept-0.1.3/ccl/rslang/import/reflex/include/
-drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.488827 pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/
--rw-rw-rw-   0        0        0    16072 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/abslexer.h
--rw-rw-rw-   0        0        0    69252 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/absmatcher.h
--rw-rw-rw-   0        0        0    18001 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/bits.h
--rw-rw-rw-   0        0        0    19348 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/boostmatcher.h
--rw-rw-rw-   0        0        0    11147 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/convert.h
--rw-rw-rw-   0        0        0     6862 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/debug.h
--rw-rw-rw-   0        0        0     6978 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/error.h
--rw-rw-rw-   0        0        0    24462 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/flexlexer.h
--rw-rw-rw-   0        0        0    38598 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/input.h
--rw-rw-rw-   0        0        0     6354 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/linematcher.h
--rw-rw-rw-   0        0        0    15401 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/matcher.h
--rw-rw-rw-   0        0        0    45834 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/pattern.h
--rw-rw-rw-   0        0        0    20060 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/pcre2matcher.h
--rw-rw-rw-   0        0        0     2948 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/posix.h
--rw-rw-rw-   0        0        0    37159 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/ranges.h
--rw-rw-rw-   0        0        0    12093 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/setop.h
--rw-rw-rw-   0        0        0     4594 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/simd.h
--rw-rw-rw-   0        0        0    22985 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/stdmatcher.h
--rw-rw-rw-   0        0        0     4244 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/timer.h
--rw-rw-rw-   0        0        0     3159 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/traits.h
--rw-rw-rw-   0        0        0     2997 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/unicode.h
--rw-rw-rw-   0        0        0     9522 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/utf8.h
-drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.515829 pyconcept-0.1.3/ccl/rslang/import/reflex/lib/
--rw-rw-rw-   0        0        0    78708 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/lib/convert.cpp
--rw-rw-rw-   0        0        0     3792 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/lib/debug.cpp
--rw-rw-rw-   0        0        0     5896 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/lib/error.cpp
--rw-rw-rw-   0        0        0    84320 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/lib/input.cpp
--rw-rw-rw-   0        0        0   116725 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/lib/matcher.cpp
--rw-rw-rw-   0        0        0     2693 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/lib/matcher_avx2.cpp
--rw-rw-rw-   0        0        0     2715 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/lib/matcher_avx512bw.cpp
--rw-rw-rw-   0        0        0   155001 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/lib/pattern.cpp
--rw-rw-rw-   0        0        0     4261 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/lib/posix.cpp
--rw-rw-rw-   0        0        0     5046 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/lib/simd_avx2.cpp
--rw-rw-rw-   0        0        0     3478 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/lib/simd_avx512bw.cpp
--rw-rw-rw-   0        0        0     5118 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/lib/unicode.cpp
--rw-rw-rw-   0        0        0     8872 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/lib/utf8.cpp
-drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.519952 pyconcept-0.1.3/ccl/rslang/import/reflex/unicode/
--rw-rw-rw-   0        0        0    38187 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/unicode/block_scripts.cpp
--rw-rw-rw-   0        0        0    30273 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/unicode/composer.cpp
--rw-rw-rw-   0        0        0   223308 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/unicode/language_scripts.cpp
--rw-rw-rw-   0        0        0    23072 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/import/reflex/unicode/letter_scripts.cpp
-drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.271913 pyconcept-0.1.3/ccl/rslang/include/
-drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.271913 pyconcept-0.1.3/ccl/rslang/include/ccl/
-drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.539955 pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/
--rw-rw-rw-   0        0        0     3600 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/ASTInterpreter.h
--rw-rw-rw-   0        0        0     1048 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/AsciiLexer.h
--rw-rw-rw-   0        0        0      963 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/Auditor.h
--rw-rw-rw-   0        0        0      317 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/DataContext.hpp
--rw-rw-rw-   0        0        0     1120 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/Error.hpp
--rw-rw-rw-   0        0        0      555 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/ErrorLogger.h
--rw-rw-rw-   0        0        0      848 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/Interpreter.h
--rw-rw-rw-   0        0        0     2192 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/LexerBase.hpp
--rw-rw-rw-   0        0        0      254 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/Literals.h
--rw-rw-rw-   0        0        0      998 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/MathLexer.h
--rw-rw-rw-   0        0        0      927 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/Parser.h
--rw-rw-rw-   0        0        0     1667 2024-05-05 09:01:01.000000 pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/ParserState.hpp
--rw-rw-rw-   0        0        0     6503 2024-05-07 22:51:03.000000 pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/RSErrorCodes.hpp
--rw-rw-rw-   0        0        0     1102 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/RSExpr.h
--rw-rw-rw-   0        0        0     1651 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/RSGenerator.h
--rw-rw-rw-   0        0        0      869 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/RSParser.h
--rw-rw-rw-   0        0        0     4722 2024-05-06 14:48:08.000000 pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/RSToken.h
--rw-rw-rw-   0        0        0     1117 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/SDataCompact.h
--rw-rw-rw-   0        0        0     1953 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/Structure.hpp
--rw-rw-rw-   0        0        0     4776 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/StructuredData.h
--rw-rw-rw-   0        0        0    12948 2024-05-07 16:08:23.000000 pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/SyntaxTree.h
--rw-rw-rw-   0        0        0     5373 2024-05-07 15:46:38.000000 pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/TypeAuditor.h
--rw-rw-rw-   0        0        0     1520 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/TypeContext.hpp
--rw-rw-rw-   0        0        0     3875 2024-05-07 15:17:48.000000 pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/Typification.h
--rw-rw-rw-   0        0        0     4297 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/ValueAuditor.h
--rw-rw-rw-   0        0        0      314 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/ValueClass.hpp
-drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.557952 pyconcept-0.1.3/ccl/rslang/src/
--rw-rw-rw-   0        0        0    19744 2024-05-06 10:32:45.000000 pyconcept-0.1.3/ccl/rslang/src/ASTInterpreter.cpp
--rw-rw-rw-   0        0        0     5991 2024-05-06 14:51:18.000000 pyconcept-0.1.3/ccl/rslang/src/ASTNormalizer.cpp
--rw-rw-rw-   0        0        0     2219 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/src/AsciiLexer.cpp
--rw-rw-rw-   0        0        0     1222 2024-05-06 14:50:47.000000 pyconcept-0.1.3/ccl/rslang/src/Auditor.cpp
--rw-rw-rw-   0        0        0     1375 2024-05-06 10:40:35.000000 pyconcept-0.1.3/ccl/rslang/src/ErrorLogger.cpp
--rw-rw-rw-   0        0        0     7204 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/src/GeneratorImplAST.cpp
--rw-rw-rw-   0        0        0     1122 2024-05-06 13:10:50.000000 pyconcept-0.1.3/ccl/rslang/src/Interpreter.cpp
--rw-rw-rw-   0        0        0     2067 2024-05-07 15:44:11.000000 pyconcept-0.1.3/ccl/rslang/src/Literals.cpp
--rw-rw-rw-   0        0        0     2316 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/src/MathLexer.cpp
--rw-rw-rw-   0        0        0     3266 2024-05-06 10:24:04.000000 pyconcept-0.1.3/ccl/rslang/src/NameCollector.cpp
--rw-rw-rw-   0        0        0     3907 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/src/Parser.cpp
--rw-rw-rw-   0        0        0     3409 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/src/RSExpr.cpp
--rw-rw-rw-   0        0        0     7626 2024-05-06 14:51:49.000000 pyconcept-0.1.3/ccl/rslang/src/RSGenerator.cpp
--rw-rw-rw-   0        0        0     8365 2024-05-05 12:24:50.000000 pyconcept-0.1.3/ccl/rslang/src/RSParser.cpp
--rw-rw-rw-   0        0        0    64296 2024-05-07 08:26:17.000000 pyconcept-0.1.3/ccl/rslang/src/RSParserImpl.cpp
--rw-rw-rw-   0        0        0    11051 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/src/RSToken.cpp
--rw-rw-rw-   0        0        0     6872 2024-05-05 13:20:57.000000 pyconcept-0.1.3/ccl/rslang/src/SDImplementation.cpp
--rw-rw-rw-   0        0        0     7639 2024-05-06 13:10:17.000000 pyconcept-0.1.3/ccl/rslang/src/SDataCompact.cpp
--rw-rw-rw-   0        0        0    10421 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/src/StructuredData.cpp
--rw-rw-rw-   0        0        0     6348 2024-05-06 14:51:57.000000 pyconcept-0.1.3/ccl/rslang/src/SyntaxTree.cpp
--rw-rw-rw-   0        0        0    31033 2024-05-07 22:48:22.000000 pyconcept-0.1.3/ccl/rslang/src/TypeAuditor.cpp
--rw-rw-rw-   0        0        0     4000 2024-05-07 15:55:27.000000 pyconcept-0.1.3/ccl/rslang/src/Typification.cpp
--rw-rw-rw-   0        0        0     6172 2024-05-06 12:22:18.000000 pyconcept-0.1.3/ccl/rslang/src/ValueAuditor.cpp
-drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.560952 pyconcept-0.1.3/ccl/rslang/unity/
--rw-rw-rw-   0        0        0      399 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/unity/RSlang.cpp
--rw-rw-rw-   0        0        0      458 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/unity/RSlang2.cpp
--rw-rw-rw-   0        0        0     1195 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/unity/reflex_unity1.cpp
--rw-rw-rw-   0        0        0     1776 2024-04-15 19:05:00.000000 pyconcept-0.1.3/ccl/rslang/unity/reflex_unity2.cpp
-drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.573627 pyconcept-0.1.3/cmake/
--rw-rw-rw-   0        0        0     1490 2024-04-19 23:11:03.000000 pyconcept-0.1.3/cmake/CXXTargets.cmake
--rw-rw-rw-   0        0        0       96 2024-04-16 20:20:08.000000 pyconcept-0.1.3/conanfile.txt
-drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.574629 pyconcept-0.1.3/include/
--rw-rw-rw-   0        0        0     1216 2024-04-15 19:05:00.000000 pyconcept-0.1.3/include/pyconcept.h
-drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.602202 pyconcept-0.1.3/pyconcept.egg-info/
--rw-rw-rw-   0        0        0      953 2024-05-07 23:18:13.000000 pyconcept-0.1.3/pyconcept.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     8509 2024-05-07 23:18:13.000000 pyconcept-0.1.3/pyconcept.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 23:18:13.000000 pyconcept-0.1.3/pyconcept.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-07 23:18:13.000000 pyconcept-0.1.3/pyconcept.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      146 2024-04-17 11:29:28.000000 pyconcept-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0      860 2024-05-07 23:18:13.604200 pyconcept-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     3916 2024-04-17 17:59:03.000000 pyconcept-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.577628 pyconcept-0.1.3/src/
--rw-rw-rw-   0        0        0     1231 2024-04-15 19:05:00.000000 pyconcept-0.1.3/src/pyconcept.cpp
-drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.579628 pyconcept-0.1.3/tests/
--rw-rw-rw-   0        0        0        0 2024-04-15 19:05:00.000000 pyconcept-0.1.3/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.597202 pyconcept-0.1.3/tests/__pycache__/
--rw-rw-rw-   0        0        0      148 2024-04-16 20:55:54.000000 pyconcept-0.1.3/tests/__pycache__/__init__.cpython-312.pyc
--rw-rw-rw-   0        0        0     5032 2024-04-17 18:55:51.000000 pyconcept-0.1.3/tests/__pycache__/testBinding.cpython-312.pyc
-drwxrwxrwx   0        0        0        0 2024-05-07 23:18:13.601205 pyconcept-0.1.3/tests/data/
--rw-rw-rw-   0        0        0     2486 2024-04-15 19:05:00.000000 pyconcept-0.1.3/tests/data/Schema1.trs
--rw-rw-rw-   0        0        0     2606 2024-04-17 16:14:46.000000 pyconcept-0.1.3/tests/testBinding.py
+drwxrwxrwx   0        0        0        0 2024-05-09 23:28:41.555448 pyconcept-0.1.4/
+-rw-rw-rw-   0        0        0      944 2024-05-09 22:41:52.000000 pyconcept-0.1.4/CHANGELOG.md
+-rw-rw-rw-   0        0        0      955 2024-04-19 23:54:16.000000 pyconcept-0.1.4/CMakeLists.txt
+-rw-rw-rw-   0        0        0     1101 2024-04-15 19:05:00.000000 pyconcept-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0      162 2024-04-18 08:33:28.000000 pyconcept-0.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      953 2024-05-09 23:28:41.554449 pyconcept-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      115 2024-04-17 11:33:45.000000 pyconcept-0.1.4/README.md
+-rw-rw-rw-   0        0        0        5 2024-05-09 22:40:47.000000 pyconcept-0.1.4/VERSION
+drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.433610 pyconcept-0.1.4/ccl/
+-rw-rw-rw-   0        0        0     2133 2024-04-17 08:48:56.000000 pyconcept-0.1.4/ccl/CMakeLists.txt
+drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.274368 pyconcept-0.1.4/ccl/cclCommons/
+drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.274368 pyconcept-0.1.4/ccl/cclCommons/include/
+drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.460652 pyconcept-0.1.4/ccl/cclCommons/include/ccl/
+-rw-rw-rw-   0        0        0    10473 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/cclCommons/include/ccl/Strings.hpp
+-rw-rw-rw-   0        0        0      895 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/cclCommons/include/ccl/Substitutes.hpp
+-rw-rw-rw-   0        0        0     1506 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/cclCommons/include/ccl/cclChange.hpp
+-rw-rw-rw-   0        0        0    11710 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/cclCommons/include/ccl/cclMeta.hpp
+-rw-rw-rw-   0        0        0     6078 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/cclCommons/include/ccl/cclTypes.hpp
+drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.275366 pyconcept-0.1.4/ccl/cclGraph/
+drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.275366 pyconcept-0.1.4/ccl/cclGraph/include/
+drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.461652 pyconcept-0.1.4/ccl/cclGraph/include/ccl/
+-rw-rw-rw-   0        0        0     2749 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/cclGraph/include/ccl/Entity.hpp
+drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.462654 pyconcept-0.1.4/ccl/cclGraph/include/ccl/graph/
+-rw-rw-rw-   0        0        0     2907 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/cclGraph/include/ccl/graph/CGraph.h
+drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.464653 pyconcept-0.1.4/ccl/cclGraph/src/
+-rw-rw-rw-   0        0        0     9187 2024-05-06 12:39:34.000000 pyconcept-0.1.4/ccl/cclGraph/src/CGraph.cpp
+drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.277368 pyconcept-0.1.4/ccl/cclLang/
+drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.276365 pyconcept-0.1.4/ccl/cclLang/include/
+drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.276365 pyconcept-0.1.4/ccl/cclLang/include/ccl/
+drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.488349 pyconcept-0.1.4/ccl/cclLang/include/ccl/lang/
+-rw-rw-rw-   0        0        0     1191 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/cclLang/include/ccl/lang/EntityTermContext.hpp
+-rw-rw-rw-   0        0        0     1941 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/cclLang/include/ccl/lang/LexicalTerm.h
+-rw-rw-rw-   0        0        0      345 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/cclLang/include/ccl/lang/Literals.h
+-rw-rw-rw-   0        0        0     1327 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/cclLang/include/ccl/lang/ManagedText.h
+-rw-rw-rw-   0        0        0     8108 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/cclLang/include/ccl/lang/Morphology.h
+-rw-rw-rw-   0        0        0     2748 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/cclLang/include/ccl/lang/Reference.h
+-rw-rw-rw-   0        0        0     2766 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/cclLang/include/ccl/lang/RefsManager.h
+-rw-rw-rw-   0        0        0      514 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/cclLang/include/ccl/lang/TextEnvironment.h
+-rw-rw-rw-   0        0        0     1278 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/cclLang/include/ccl/lang/TextProcessor.h
+drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.541760 pyconcept-0.1.4/ccl/cclLang/src/
+-rw-rw-rw-   0        0        0     2111 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/cclLang/src/LexicalTerm.cpp
+-rw-rw-rw-   0        0        0      307 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/cclLang/src/Literals.cpp
+-rw-rw-rw-   0        0        0     2016 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/cclLang/src/ManagedText.cpp
+-rw-rw-rw-   0        0        0     2239 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/cclLang/src/Morphology.cpp
+-rw-rw-rw-   0        0        0     7475 2024-05-06 12:47:43.000000 pyconcept-0.1.4/ccl/cclLang/src/Reference.cpp
+-rw-rw-rw-   0        0        0     6529 2024-05-06 12:48:14.000000 pyconcept-0.1.4/ccl/cclLang/src/RefsManager.cpp
+-rw-rw-rw-   0        0        0      452 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/cclLang/src/TextEnvironment.cpp
+-rw-rw-rw-   0        0        0     1581 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/cclLang/src/TextProcessor.cpp
+drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.542761 pyconcept-0.1.4/ccl/cclLang/unity/
+-rw-rw-rw-   0        0        0      309 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/cclLang/unity/cclLang.cpp
+drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.613047 pyconcept-0.1.4/ccl/cmake/
+-rw-rw-rw-   0        0        0     1541 2024-04-19 23:11:05.000000 pyconcept-0.1.4/ccl/cmake/CXXTargets.cmake
+-rw-rw-rw-   0        0        0       93 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/conanfile.txt
+drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.284581 pyconcept-0.1.4/ccl/core/
+drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.280578 pyconcept-0.1.4/ccl/core/include/
+drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.711263 pyconcept-0.1.4/ccl/core/include/ccl/
+-rw-rw-rw-   0        0        0     2124 2024-05-06 15:23:11.000000 pyconcept-0.1.4/ccl/core/include/ccl/Operation.hpp
+-rw-rw-rw-   0        0        0     5309 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/include/ccl/Source.hpp
+drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.719042 pyconcept-0.1.4/ccl/core/include/ccl/api/
+-rw-rw-rw-   0        0        0      915 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/include/ccl/api/RSFormJA.h
+drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.748907 pyconcept-0.1.4/ccl/core/include/ccl/env/
+-rw-rw-rw-   0        0        0     2904 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/include/ccl/env/SourceManager.hpp
+-rw-rw-rw-   0        0        0      624 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/include/ccl/env/cclEnvironment.h
+drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.807402 pyconcept-0.1.4/ccl/core/include/ccl/ops/
+-rw-rw-rw-   0        0        0     1998 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/include/ccl/ops/EquationOptions.h
+-rw-rw-rw-   0        0        0      850 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/include/ccl/ops/RSAggregator.h
+-rw-rw-rw-   0        0        0     1187 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/include/ccl/ops/RSEquationProcessor.h
+-rw-rw-rw-   0        0        0     3525 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/include/ccl/ops/RSOperations.h
+drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.845495 pyconcept-0.1.4/ccl/core/include/ccl/oss/
+-rw-rw-rw-   0        0        0     4161 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/include/ccl/oss/OSSchema.h
+-rw-rw-rw-   0        0        0     1658 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/include/ccl/oss/OperationProcessor.hpp
+-rw-rw-rw-   0        0        0      903 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/include/ccl/oss/Pict.hpp
+-rw-rw-rw-   0        0        0      934 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/include/ccl/oss/RSSynthesProcessor.h
+-rw-rw-rw-   0        0        0     1363 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/include/ccl/oss/ossGraphFacet.h
+-rw-rw-rw-   0        0        0     2334 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/include/ccl/oss/ossGridFacet.h
+-rw-rw-rw-   0        0        0     2979 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/include/ccl/oss/ossOperationsFacet.h
+-rw-rw-rw-   0        0        0     2469 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/include/ccl/oss/ossSourceFacet.h
+drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.897611 pyconcept-0.1.4/ccl/core/include/ccl/semantic/
+-rw-rw-rw-   0        0        0      622 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/include/ccl/semantic/ConceptRecord.h
+-rw-rw-rw-   0        0        0     1473 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/include/ccl/semantic/CstFilters.hpp
+-rw-rw-rw-   0        0        0     2367 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/include/ccl/semantic/CstList.h
+-rw-rw-rw-   0        0        0     2523 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/include/ccl/semantic/CstType.hpp
+-rw-rw-rw-   0        0        0     1231 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/include/ccl/semantic/IdentityManager.h
+-rw-rw-rw-   0        0        0      962 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/include/ccl/semantic/InterpretationStorage.h
+-rw-rw-rw-   0        0        0     1095 2024-05-06 14:59:52.000000 pyconcept-0.1.4/ccl/core/include/ccl/semantic/RSConcept.h
+-rw-rw-rw-   0        0        0     3584 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/include/ccl/semantic/RSCore.h
+-rw-rw-rw-   0        0        0     3430 2024-05-06 15:04:15.000000 pyconcept-0.1.4/ccl/core/include/ccl/semantic/RSForm.h
+-rw-rw-rw-   0        0        0     3012 2024-05-06 15:04:05.000000 pyconcept-0.1.4/ccl/core/include/ccl/semantic/RSModel.h
+-rw-rw-rw-   0        0        0     5074 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/include/ccl/semantic/Schema.h
+-rw-rw-rw-   0        0        0     1122 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/include/ccl/semantic/TextConcept.h
+-rw-rw-rw-   0        0        0     2603 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/include/ccl/semantic/TextData.hpp
+-rw-rw-rw-   0        0        0     3988 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/include/ccl/semantic/Thesaurus.h
+-rw-rw-rw-   0        0        0     1577 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/include/ccl/semantic/rsCalculationFacet.h
+-rw-rw-rw-   0        0        0     1648 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/include/ccl/semantic/rsModificationFacet.h
+-rw-rw-rw-   0        0        0     1099 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/include/ccl/semantic/rsOperationFacet.h
+-rw-rw-rw-   0        0        0     1867 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/include/ccl/semantic/rsValuesFacet.h
+drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.903148 pyconcept-0.1.4/ccl/core/include/ccl/tools/
+-rw-rw-rw-   0        0        0      894 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/include/ccl/tools/CstNameGenerator.h
+-rw-rw-rw-   0        0        0      523 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/include/ccl/tools/EntityGenerator.h
+-rw-rw-rw-   0        0        0     2935 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/include/ccl/tools/EnumJSON.hpp
+-rw-rw-rw-   0        0        0     3871 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/include/ccl/tools/JSON.h
+drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.904151 pyconcept-0.1.4/ccl/core/include/nlohmann/
+-rw-rw-rw-   0        0        0   945021 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/include/nlohmann/json.hpp
+drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.907148 pyconcept-0.1.4/ccl/core/src/
+-rw-rw-rw-   0        0        0    18448 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/src/JSON.cpp
+drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.909153 pyconcept-0.1.4/ccl/core/src/api/
+-rw-rw-rw-   0        0        0     3026 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/src/api/RSFormJA.cpp
+drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.911152 pyconcept-0.1.4/ccl/core/src/env/
+-rw-rw-rw-   0        0        0      636 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/src/env/cclEnvironment.cpp
+drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.915148 pyconcept-0.1.4/ccl/core/src/ops/
+-rw-rw-rw-   0        0        0     1772 2024-05-06 14:58:07.000000 pyconcept-0.1.4/ccl/core/src/ops/EquationOptions.cpp
+-rw-rw-rw-   0        0        0     4124 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/src/ops/RSAggregator.cpp
+-rw-rw-rw-   0        0        0     4290 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/src/ops/RSEquationProcessor.cpp
+-rw-rw-rw-   0        0        0    16240 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/src/ops/RSOperations.cpp
+drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.978670 pyconcept-0.1.4/ccl/core/src/oss/
+-rw-rw-rw-   0        0        0     7258 2024-05-06 15:10:47.000000 pyconcept-0.1.4/ccl/core/src/oss/OSSchema.cpp
+-rw-rw-rw-   0        0        0     2812 2024-05-06 15:23:33.000000 pyconcept-0.1.4/ccl/core/src/oss/RSSynthesProcessor.cpp
+-rw-rw-rw-   0        0        0     4305 2024-05-06 15:06:48.000000 pyconcept-0.1.4/ccl/core/src/oss/ossGraphFacet.cpp
+-rw-rw-rw-   0        0        0     3023 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/src/oss/ossGridFacet.cpp
+-rw-rw-rw-   0        0        0    11652 2024-05-06 15:05:23.000000 pyconcept-0.1.4/ccl/core/src/oss/ossOperationsFacet.cpp
+-rw-rw-rw-   0        0        0    10397 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/src/oss/ossSourceFacet.cpp
+drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.283578 pyconcept-0.1.4/ccl/core/src/semantic/
+drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.982669 pyconcept-0.1.4/ccl/core/src/semantic/rscore/
+-rw-rw-rw-   0        0        0      588 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/src/semantic/rscore/ConceptRecord.cpp
+-rw-rw-rw-   0        0        0     3957 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/src/semantic/rscore/CstList.cpp
+-rw-rw-rw-   0        0        0     1950 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/src/semantic/rscore/IdentityManager.cpp
+-rw-rw-rw-   0        0        0    10403 2024-05-06 15:01:20.000000 pyconcept-0.1.4/ccl/core/src/semantic/rscore/RSCore.cpp
+drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.985670 pyconcept-0.1.4/ccl/core/src/semantic/rsform/
+-rw-rw-rw-   0        0        0     8112 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/src/semantic/rsform/RSForm.cpp
+-rw-rw-rw-   0        0        0     1573 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/src/semantic/rsform/rsModificationFacet.cpp
+-rw-rw-rw-   0        0        0     2431 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/src/semantic/rsform/rsOperationFacet.cpp
+drwxrwxrwx   0        0        0        0 2024-05-09 23:28:40.016669 pyconcept-0.1.4/ccl/core/src/semantic/rsmodel/
+-rw-rw-rw-   0        0        0     1591 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/src/semantic/rsmodel/InterpretationStorage.cpp
+-rw-rw-rw-   0        0        0     4755 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/src/semantic/rsmodel/RSModel.cpp
+-rw-rw-rw-   0        0        0     3954 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/src/semantic/rsmodel/rsCalculationFacet.cpp
+-rw-rw-rw-   0        0        0     6866 2024-05-06 13:08:18.000000 pyconcept-0.1.4/ccl/core/src/semantic/rsmodel/rsValuesFacet.cpp
+drwxrwxrwx   0        0        0        0 2024-05-09 23:28:40.052732 pyconcept-0.1.4/ccl/core/src/semantic/schema/
+-rw-rw-rw-   0        0        0      830 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/src/semantic/schema/RSConcept.cpp
+-rw-rw-rw-   0        0        0    13468 2024-05-08 08:09:16.000000 pyconcept-0.1.4/ccl/core/src/semantic/schema/Schema.cpp
+drwxrwxrwx   0        0        0        0 2024-05-09 23:28:40.060736 pyconcept-0.1.4/ccl/core/src/semantic/thesaurus/
+-rw-rw-rw-   0        0        0      919 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/src/semantic/thesaurus/TextConcept.cpp
+-rw-rw-rw-   0        0        0    10089 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/src/semantic/thesaurus/Thesaurus.cpp
+drwxrwxrwx   0        0        0        0 2024-05-09 23:28:40.086732 pyconcept-0.1.4/ccl/core/src/tools/
+-rw-rw-rw-   0        0        0     2682 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/src/tools/CstNameGenerator.cpp
+-rw-rw-rw-   0        0        0      773 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/src/tools/EntityGenerator.cpp
+drwxrwxrwx   0        0        0        0 2024-05-09 23:28:40.087734 pyconcept-0.1.4/ccl/core/unity/
+-rw-rw-rw-   0        0        0     1448 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/unity/CCL.cpp
+drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.288579 pyconcept-0.1.4/ccl/rslang/
+drwxrwxrwx   0        0        0        0 2024-05-09 23:28:40.138787 pyconcept-0.1.4/ccl/rslang/header/
+-rw-rw-rw-   0        0        0     1363 2024-05-06 10:35:16.000000 pyconcept-0.1.4/ccl/rslang/header/ASTNormalizer.h
+-rw-rw-rw-   0        0        0    34735 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/header/AsciiLexerImpl.hpp
+-rw-rw-rw-   0        0        0     2424 2024-05-09 23:22:53.000000 pyconcept-0.1.4/ccl/rslang/header/GeneratorImplAST.h
+-rw-rw-rw-   0        0        0    35507 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/header/MathLexerImpl.hpp
+-rw-rw-rw-   0        0        0      994 2024-05-09 22:59:05.000000 pyconcept-0.1.4/ccl/rslang/header/NameCollector.h
+-rw-rw-rw-   0        0        0    31974 2024-05-09 23:07:18.000000 pyconcept-0.1.4/ccl/rslang/header/RSParserImpl.h
+-rw-rw-rw-   0        0        0     5446 2024-05-05 13:20:57.000000 pyconcept-0.1.4/ccl/rslang/header/SDImplementation.h
+drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.285579 pyconcept-0.1.4/ccl/rslang/import/
+drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.286578 pyconcept-0.1.4/ccl/rslang/import/reflex/
+drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.285579 pyconcept-0.1.4/ccl/rslang/import/reflex/include/
+drwxrwxrwx   0        0        0        0 2024-05-09 23:28:40.211667 pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/
+-rw-rw-rw-   0        0        0    16072 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/abslexer.h
+-rw-rw-rw-   0        0        0    69252 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/absmatcher.h
+-rw-rw-rw-   0        0        0    18001 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/bits.h
+-rw-rw-rw-   0        0        0    19348 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/boostmatcher.h
+-rw-rw-rw-   0        0        0    11147 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/convert.h
+-rw-rw-rw-   0        0        0     6862 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/debug.h
+-rw-rw-rw-   0        0        0     6978 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/error.h
+-rw-rw-rw-   0        0        0    24462 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/flexlexer.h
+-rw-rw-rw-   0        0        0    38598 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/input.h
+-rw-rw-rw-   0        0        0     6354 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/linematcher.h
+-rw-rw-rw-   0        0        0    15401 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/matcher.h
+-rw-rw-rw-   0        0        0    45834 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/pattern.h
+-rw-rw-rw-   0        0        0    20060 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/pcre2matcher.h
+-rw-rw-rw-   0        0        0     2948 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/posix.h
+-rw-rw-rw-   0        0        0    37159 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/ranges.h
+-rw-rw-rw-   0        0        0    12093 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/setop.h
+-rw-rw-rw-   0        0        0     4594 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/simd.h
+-rw-rw-rw-   0        0        0    22985 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/stdmatcher.h
+-rw-rw-rw-   0        0        0     4244 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/timer.h
+-rw-rw-rw-   0        0        0     3159 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/traits.h
+-rw-rw-rw-   0        0        0     2997 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/unicode.h
+-rw-rw-rw-   0        0        0     9522 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/utf8.h
+drwxrwxrwx   0        0        0        0 2024-05-09 23:28:40.305788 pyconcept-0.1.4/ccl/rslang/import/reflex/lib/
+-rw-rw-rw-   0        0        0    78708 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/lib/convert.cpp
+-rw-rw-rw-   0        0        0     3792 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/lib/debug.cpp
+-rw-rw-rw-   0        0        0     5896 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/lib/error.cpp
+-rw-rw-rw-   0        0        0    84320 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/lib/input.cpp
+-rw-rw-rw-   0        0        0   116725 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/lib/matcher.cpp
+-rw-rw-rw-   0        0        0     2693 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/lib/matcher_avx2.cpp
+-rw-rw-rw-   0        0        0     2715 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/lib/matcher_avx512bw.cpp
+-rw-rw-rw-   0        0        0   155001 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/lib/pattern.cpp
+-rw-rw-rw-   0        0        0     4261 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/lib/posix.cpp
+-rw-rw-rw-   0        0        0     5046 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/lib/simd_avx2.cpp
+-rw-rw-rw-   0        0        0     3478 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/lib/simd_avx512bw.cpp
+-rw-rw-rw-   0        0        0     5118 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/lib/unicode.cpp
+-rw-rw-rw-   0        0        0     8872 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/lib/utf8.cpp
+drwxrwxrwx   0        0        0        0 2024-05-09 23:28:40.310782 pyconcept-0.1.4/ccl/rslang/import/reflex/unicode/
+-rw-rw-rw-   0        0        0    38187 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/unicode/block_scripts.cpp
+-rw-rw-rw-   0        0        0    30273 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/unicode/composer.cpp
+-rw-rw-rw-   0        0        0   223308 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/unicode/language_scripts.cpp
+-rw-rw-rw-   0        0        0    23072 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/unicode/letter_scripts.cpp
+drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.287578 pyconcept-0.1.4/ccl/rslang/include/
+drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.287578 pyconcept-0.1.4/ccl/rslang/include/ccl/
+drwxrwxrwx   0        0        0        0 2024-05-09 23:28:41.251388 pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/
+-rw-rw-rw-   0        0        0     3659 2024-05-09 23:22:53.000000 pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/ASTInterpreter.h
+-rw-rw-rw-   0        0        0     1048 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/AsciiLexer.h
+-rw-rw-rw-   0        0        0      963 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/Auditor.h
+-rw-rw-rw-   0        0        0      317 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/DataContext.hpp
+-rw-rw-rw-   0        0        0     1120 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/Error.hpp
+-rw-rw-rw-   0        0        0      555 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/ErrorLogger.h
+-rw-rw-rw-   0        0        0      848 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/Interpreter.h
+-rw-rw-rw-   0        0        0     2192 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/LexerBase.hpp
+-rw-rw-rw-   0        0        0      254 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/Literals.h
+-rw-rw-rw-   0        0        0      998 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/MathLexer.h
+-rw-rw-rw-   0        0        0      927 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/Parser.h
+-rw-rw-rw-   0        0        0     1667 2024-05-05 09:01:01.000000 pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/ParserState.hpp
+-rw-rw-rw-   0        0        0     6503 2024-05-07 22:51:03.000000 pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/RSErrorCodes.hpp
+-rw-rw-rw-   0        0        0     1102 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/RSExpr.h
+-rw-rw-rw-   0        0        0     1651 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/RSGenerator.h
+-rw-rw-rw-   0        0        0      869 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/RSParser.h
+-rw-rw-rw-   0        0        0     4722 2024-05-06 14:48:08.000000 pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/RSToken.h
+-rw-rw-rw-   0        0        0     1117 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/SDataCompact.h
+-rw-rw-rw-   0        0        0     1953 2024-05-08 07:33:13.000000 pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/Structure.hpp
+-rw-rw-rw-   0        0        0     4776 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/StructuredData.h
+-rw-rw-rw-   0        0        0    13165 2024-05-09 23:25:09.000000 pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/SyntaxTree.h
+-rw-rw-rw-   0        0        0     5534 2024-05-09 23:22:53.000000 pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/TypeAuditor.h
+-rw-rw-rw-   0        0        0     1520 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/TypeContext.hpp
+-rw-rw-rw-   0        0        0     3927 2024-05-08 07:34:11.000000 pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/Typification.h
+-rw-rw-rw-   0        0        0     4379 2024-05-09 23:22:53.000000 pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/ValueAuditor.h
+-rw-rw-rw-   0        0        0      314 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/ValueClass.hpp
+drwxrwxrwx   0        0        0        0 2024-05-09 23:28:41.452579 pyconcept-0.1.4/ccl/rslang/src/
+-rw-rw-rw-   0        0        0    19591 2024-05-09 23:22:53.000000 pyconcept-0.1.4/ccl/rslang/src/ASTInterpreter.cpp
+-rw-rw-rw-   0        0        0     5991 2024-05-06 14:51:18.000000 pyconcept-0.1.4/ccl/rslang/src/ASTNormalizer.cpp
+-rw-rw-rw-   0        0        0     2219 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/src/AsciiLexer.cpp
+-rw-rw-rw-   0        0        0     1222 2024-05-06 14:50:47.000000 pyconcept-0.1.4/ccl/rslang/src/Auditor.cpp
+-rw-rw-rw-   0        0        0     1375 2024-05-06 10:40:35.000000 pyconcept-0.1.4/ccl/rslang/src/ErrorLogger.cpp
+-rw-rw-rw-   0        0        0     7222 2024-05-09 23:22:30.000000 pyconcept-0.1.4/ccl/rslang/src/GeneratorImplAST.cpp
+-rw-rw-rw-   0        0        0     1122 2024-05-06 13:10:50.000000 pyconcept-0.1.4/ccl/rslang/src/Interpreter.cpp
+-rw-rw-rw-   0        0        0     2067 2024-05-07 15:44:11.000000 pyconcept-0.1.4/ccl/rslang/src/Literals.cpp
+-rw-rw-rw-   0        0        0     2316 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/src/MathLexer.cpp
+-rw-rw-rw-   0        0        0     3267 2024-05-09 22:58:58.000000 pyconcept-0.1.4/ccl/rslang/src/NameCollector.cpp
+-rw-rw-rw-   0        0        0     3891 2024-05-09 23:09:18.000000 pyconcept-0.1.4/ccl/rslang/src/Parser.cpp
+-rw-rw-rw-   0        0        0     3409 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/src/RSExpr.cpp
+-rw-rw-rw-   0        0        0     7626 2024-05-06 14:51:49.000000 pyconcept-0.1.4/ccl/rslang/src/RSGenerator.cpp
+-rw-rw-rw-   0        0        0     8365 2024-05-05 12:24:50.000000 pyconcept-0.1.4/ccl/rslang/src/RSParser.cpp
+-rw-rw-rw-   0        0        0    63677 2024-05-09 23:07:18.000000 pyconcept-0.1.4/ccl/rslang/src/RSParserImpl.cpp
+-rw-rw-rw-   0        0        0    11051 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/src/RSToken.cpp
+-rw-rw-rw-   0        0        0     6872 2024-05-05 13:20:57.000000 pyconcept-0.1.4/ccl/rslang/src/SDImplementation.cpp
+-rw-rw-rw-   0        0        0     7639 2024-05-08 08:09:16.000000 pyconcept-0.1.4/ccl/rslang/src/SDataCompact.cpp
+-rw-rw-rw-   0        0        0    10421 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/src/StructuredData.cpp
+-rw-rw-rw-   0        0        0     6348 2024-05-06 14:51:57.000000 pyconcept-0.1.4/ccl/rslang/src/SyntaxTree.cpp
+-rw-rw-rw-   0        0        0    32177 2024-05-09 23:22:53.000000 pyconcept-0.1.4/ccl/rslang/src/TypeAuditor.cpp
+-rw-rw-rw-   0        0        0     4114 2024-05-08 07:34:32.000000 pyconcept-0.1.4/ccl/rslang/src/Typification.cpp
+-rw-rw-rw-   0        0        0     6081 2024-05-09 23:22:53.000000 pyconcept-0.1.4/ccl/rslang/src/ValueAuditor.cpp
+drwxrwxrwx   0        0        0        0 2024-05-09 23:28:41.458580 pyconcept-0.1.4/ccl/rslang/unity/
+-rw-rw-rw-   0        0        0      399 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/unity/RSlang.cpp
+-rw-rw-rw-   0        0        0      458 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/unity/RSlang2.cpp
+-rw-rw-rw-   0        0        0     1195 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/unity/reflex_unity1.cpp
+-rw-rw-rw-   0        0        0     1776 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/unity/reflex_unity2.cpp
+drwxrwxrwx   0        0        0        0 2024-05-09 23:28:41.460584 pyconcept-0.1.4/cmake/
+-rw-rw-rw-   0        0        0     1490 2024-04-19 23:11:03.000000 pyconcept-0.1.4/cmake/CXXTargets.cmake
+-rw-rw-rw-   0        0        0       96 2024-04-16 20:20:08.000000 pyconcept-0.1.4/conanfile.txt
+drwxrwxrwx   0        0        0        0 2024-05-09 23:28:41.461578 pyconcept-0.1.4/include/
+-rw-rw-rw-   0        0        0     1216 2024-04-15 19:05:00.000000 pyconcept-0.1.4/include/pyconcept.h
+drwxrwxrwx   0        0        0        0 2024-05-09 23:28:41.552449 pyconcept-0.1.4/pyconcept.egg-info/
+-rw-rw-rw-   0        0        0      953 2024-05-09 23:28:39.000000 pyconcept-0.1.4/pyconcept.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     8509 2024-05-09 23:28:39.000000 pyconcept-0.1.4/pyconcept.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 23:28:39.000000 pyconcept-0.1.4/pyconcept.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-09 23:28:39.000000 pyconcept-0.1.4/pyconcept.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      146 2024-04-17 11:29:28.000000 pyconcept-0.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0      860 2024-05-09 23:28:41.556446 pyconcept-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     3916 2024-04-17 17:59:03.000000 pyconcept-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 23:28:41.469994 pyconcept-0.1.4/src/
+-rw-rw-rw-   0        0        0     1231 2024-04-15 19:05:00.000000 pyconcept-0.1.4/src/pyconcept.cpp
+drwxrwxrwx   0        0        0        0 2024-05-09 23:28:41.471997 pyconcept-0.1.4/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-15 19:05:00.000000 pyconcept-0.1.4/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 23:28:41.474998 pyconcept-0.1.4/tests/__pycache__/
+-rw-rw-rw-   0        0        0      148 2024-04-16 20:55:54.000000 pyconcept-0.1.4/tests/__pycache__/__init__.cpython-312.pyc
+-rw-rw-rw-   0        0        0     5032 2024-04-17 18:55:51.000000 pyconcept-0.1.4/tests/__pycache__/testBinding.cpython-312.pyc
+drwxrwxrwx   0        0        0        0 2024-05-09 23:28:41.520703 pyconcept-0.1.4/tests/data/
+-rw-rw-rw-   0        0        0     2486 2024-04-15 19:05:00.000000 pyconcept-0.1.4/tests/data/Schema1.trs
+-rw-rw-rw-   0        0        0     2606 2024-04-17 16:14:46.000000 pyconcept-0.1.4/tests/testBinding.py
```

### Comparing `pyconcept-0.1.3/CHANGELOG.md` & `pyconcept-0.1.4/CHANGELOG.md`

 * *Files 24% similar despite different names*

```diff
@@ -15,10 +15,25 @@
 - [PROJECTNAME-YYYY](http://tickets.projectname.com/browse/PROJECTNAME-YYYY)
   PATCH Ticket title goes here.
 
 ### Changed
 
 ### Fixed
 
+## [0.1.4] - 2024-05-10
+
+### Fixed
+
+- EmptySet is correctly processed as argument for functions and other operations
+
+## [0.1.3] - 2024-05-08
+
+### Changed
+
+- Allow EmptySet to be used as standalone expression. Mostly used in recursion initialization
+- Grammar rules refactoring
+
 ## [0.1.2] - 2024-04-18
 
-Add URLS to package and improve build process
+### Added
+
+- Add URLS to package and improve build process
```

### Comparing `pyconcept-0.1.3/CMakeLists.txt` & `pyconcept-0.1.4/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/LICENSE` & `pyconcept-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/PKG-INFO` & `pyconcept-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyconcept
-Version: 0.1.3
+Version: 0.1.4
 Summary: Concept core Python wrapper
 Author: CIHT CONCEPT, IRBorisov
 Author-email: iborisov@acconcept.ru
 License: MIT
 Project-URL: GitHub, https://github.com/IRBorisov/ConceptCore/tree/main/pyconcept
 Project-URL: Changelog, https://github.com/IRBorisov/ConceptCore/tree/main/pyconcept/CHANGELOG.md
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pyconcept-0.1.3/ccl/CMakeLists.txt` & `pyconcept-0.1.4/ccl/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/cclCommons/include/ccl/Strings.hpp` & `pyconcept-0.1.4/ccl/cclCommons/include/ccl/Strings.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/cclCommons/include/ccl/Substitutes.hpp` & `pyconcept-0.1.4/ccl/cclCommons/include/ccl/Substitutes.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/cclCommons/include/ccl/cclChange.hpp` & `pyconcept-0.1.4/ccl/cclCommons/include/ccl/cclChange.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/cclCommons/include/ccl/cclMeta.hpp` & `pyconcept-0.1.4/ccl/cclCommons/include/ccl/cclMeta.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/cclCommons/include/ccl/cclTypes.hpp` & `pyconcept-0.1.4/ccl/cclCommons/include/ccl/cclTypes.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/cclGraph/include/ccl/Entity.hpp` & `pyconcept-0.1.4/ccl/cclGraph/include/ccl/Entity.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/cclGraph/include/ccl/graph/CGraph.h` & `pyconcept-0.1.4/ccl/cclGraph/include/ccl/graph/CGraph.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/cclGraph/src/CGraph.cpp` & `pyconcept-0.1.4/ccl/cclGraph/src/CGraph.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/cclLang/include/ccl/lang/EntityTermContext.hpp` & `pyconcept-0.1.4/ccl/cclLang/include/ccl/lang/EntityTermContext.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/cclLang/include/ccl/lang/LexicalTerm.h` & `pyconcept-0.1.4/ccl/cclLang/include/ccl/lang/LexicalTerm.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/cclLang/include/ccl/lang/ManagedText.h` & `pyconcept-0.1.4/ccl/cclLang/include/ccl/lang/ManagedText.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/cclLang/include/ccl/lang/Morphology.h` & `pyconcept-0.1.4/ccl/cclLang/include/ccl/lang/Morphology.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/cclLang/include/ccl/lang/Reference.h` & `pyconcept-0.1.4/ccl/cclLang/include/ccl/lang/Reference.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/cclLang/include/ccl/lang/RefsManager.h` & `pyconcept-0.1.4/ccl/cclLang/include/ccl/lang/RefsManager.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/cclLang/include/ccl/lang/TextEnvironment.h` & `pyconcept-0.1.4/ccl/cclLang/include/ccl/lang/TextEnvironment.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/cclLang/include/ccl/lang/TextProcessor.h` & `pyconcept-0.1.4/ccl/cclLang/include/ccl/lang/TextProcessor.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/cclLang/src/LexicalTerm.cpp` & `pyconcept-0.1.4/ccl/cclLang/src/LexicalTerm.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/cclLang/src/ManagedText.cpp` & `pyconcept-0.1.4/ccl/cclLang/src/ManagedText.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/cclLang/src/Morphology.cpp` & `pyconcept-0.1.4/ccl/cclLang/src/Morphology.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/cclLang/src/Reference.cpp` & `pyconcept-0.1.4/ccl/cclLang/src/Reference.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/cclLang/src/RefsManager.cpp` & `pyconcept-0.1.4/ccl/cclLang/src/RefsManager.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/cclLang/src/TextProcessor.cpp` & `pyconcept-0.1.4/ccl/cclLang/src/TextProcessor.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/cmake/CXXTargets.cmake` & `pyconcept-0.1.4/ccl/cmake/CXXTargets.cmake`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/core/include/ccl/Operation.hpp` & `pyconcept-0.1.4/ccl/core/include/ccl/Operation.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/core/include/ccl/Source.hpp` & `pyconcept-0.1.4/ccl/core/include/ccl/Source.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/core/include/ccl/api/RSFormJA.h` & `pyconcept-0.1.4/ccl/core/include/ccl/api/RSFormJA.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/core/include/ccl/env/SourceManager.hpp` & `pyconcept-0.1.4/ccl/core/include/ccl/env/SourceManager.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/core/include/ccl/env/cclEnvironment.h` & `pyconcept-0.1.4/ccl/core/include/ccl/env/cclEnvironment.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/core/include/ccl/ops/EquationOptions.h` & `pyconcept-0.1.4/ccl/core/include/ccl/ops/EquationOptions.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/core/include/ccl/ops/RSAggregator.h` & `pyconcept-0.1.4/ccl/core/include/ccl/ops/RSAggregator.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/core/include/ccl/ops/RSEquationProcessor.h` & `pyconcept-0.1.4/ccl/core/include/ccl/ops/RSEquationProcessor.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/core/include/ccl/ops/RSOperations.h` & `pyconcept-0.1.4/ccl/core/include/ccl/ops/RSOperations.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/core/include/ccl/oss/OSSchema.h` & `pyconcept-0.1.4/ccl/core/include/ccl/oss/OSSchema.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/core/include/ccl/oss/OperationProcessor.hpp` & `pyconcept-0.1.4/ccl/core/include/ccl/oss/OperationProcessor.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/core/include/ccl/oss/Pict.hpp` & `pyconcept-0.1.4/ccl/core/include/ccl/oss/Pict.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/core/include/ccl/oss/RSSynthesProcessor.h` & `pyconcept-0.1.4/ccl/core/include/ccl/oss/RSSynthesProcessor.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/core/include/ccl/oss/ossGraphFacet.h` & `pyconcept-0.1.4/ccl/core/include/ccl/oss/ossGraphFacet.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/core/include/ccl/oss/ossGridFacet.h` & `pyconcept-0.1.4/ccl/core/include/ccl/oss/ossGridFacet.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/core/include/ccl/oss/ossOperationsFacet.h` & `pyconcept-0.1.4/ccl/core/include/ccl/oss/ossOperationsFacet.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/core/include/ccl/oss/ossSourceFacet.h` & `pyconcept-0.1.4/ccl/core/include/ccl/oss/ossSourceFacet.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/core/include/ccl/semantic/ConceptRecord.h` & `pyconcept-0.1.4/ccl/core/include/ccl/semantic/ConceptRecord.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/core/include/ccl/semantic/CstFilters.hpp` & `pyconcept-0.1.4/ccl/core/include/ccl/semantic/CstFilters.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/core/include/ccl/semantic/CstList.h` & `pyconcept-0.1.4/ccl/core/include/ccl/semantic/CstList.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/core/include/ccl/semantic/CstType.hpp` & `pyconcept-0.1.4/ccl/core/include/ccl/semantic/CstType.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/core/include/ccl/semantic/IdentityManager.h` & `pyconcept-0.1.4/ccl/core/include/ccl/semantic/IdentityManager.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/core/include/ccl/semantic/InterpretationStorage.h` & `pyconcept-0.1.4/ccl/core/include/ccl/semantic/InterpretationStorage.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/core/include/ccl/semantic/RSConcept.h` & `pyconcept-0.1.4/ccl/core/include/ccl/semantic/RSConcept.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/core/include/ccl/semantic/RSCore.h` & `pyconcept-0.1.4/ccl/core/include/ccl/semantic/RSCore.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/core/include/ccl/semantic/RSForm.h` & `pyconcept-0.1.4/ccl/core/include/ccl/semantic/RSForm.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/core/include/ccl/semantic/RSModel.h` & `pyconcept-0.1.4/ccl/core/include/ccl/semantic/RSModel.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/core/include/ccl/semantic/Schema.h` & `pyconcept-0.1.4/ccl/core/include/ccl/semantic/Schema.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/core/include/ccl/semantic/TextConcept.h` & `pyconcept-0.1.4/ccl/core/include/ccl/semantic/TextConcept.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/core/include/ccl/semantic/TextData.hpp` & `pyconcept-0.1.4/ccl/core/include/ccl/semantic/TextData.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/core/include/ccl/semantic/Thesaurus.h` & `pyconcept-0.1.4/ccl/core/include/ccl/semantic/Thesaurus.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/core/include/ccl/semantic/rsCalculationFacet.h` & `pyconcept-0.1.4/ccl/core/include/ccl/semantic/rsCalculationFacet.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/core/include/ccl/semantic/rsModificationFacet.h` & `pyconcept-0.1.4/ccl/core/include/ccl/semantic/rsModificationFacet.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/core/include/ccl/semantic/rsOperationFacet.h` & `pyconcept-0.1.4/ccl/core/include/ccl/semantic/rsOperationFacet.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/core/include/ccl/semantic/rsValuesFacet.h` & `pyconcept-0.1.4/ccl/core/include/ccl/semantic/rsValuesFacet.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/core/include/ccl/tools/CstNameGenerator.h` & `pyconcept-0.1.4/ccl/core/include/ccl/tools/CstNameGenerator.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/core/include/ccl/tools/EntityGenerator.h` & `pyconcept-0.1.4/ccl/core/include/ccl/tools/EntityGenerator.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/core/include/ccl/tools/EnumJSON.hpp` & `pyconcept-0.1.4/ccl/core/include/ccl/tools/EnumJSON.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/core/include/ccl/tools/JSON.h` & `pyconcept-0.1.4/ccl/core/include/ccl/tools/JSON.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/core/include/nlohmann/json.hpp` & `pyconcept-0.1.4/ccl/core/include/nlohmann/json.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/core/src/JSON.cpp` & `pyconcept-0.1.4/ccl/core/src/JSON.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/core/src/api/RSFormJA.cpp` & `pyconcept-0.1.4/ccl/core/src/api/RSFormJA.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/core/src/env/cclEnvironment.cpp` & `pyconcept-0.1.4/ccl/core/src/env/cclEnvironment.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/core/src/ops/EquationOptions.cpp` & `pyconcept-0.1.4/ccl/core/src/ops/EquationOptions.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/core/src/ops/RSAggregator.cpp` & `pyconcept-0.1.4/ccl/core/src/ops/RSAggregator.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/core/src/ops/RSEquationProcessor.cpp` & `pyconcept-0.1.4/ccl/core/src/ops/RSEquationProcessor.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/core/src/ops/RSOperations.cpp` & `pyconcept-0.1.4/ccl/core/src/ops/RSOperations.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/core/src/oss/OSSchema.cpp` & `pyconcept-0.1.4/ccl/core/src/oss/OSSchema.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/core/src/oss/RSSynthesProcessor.cpp` & `pyconcept-0.1.4/ccl/core/src/oss/RSSynthesProcessor.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/core/src/oss/ossGraphFacet.cpp` & `pyconcept-0.1.4/ccl/core/src/oss/ossGraphFacet.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/core/src/oss/ossGridFacet.cpp` & `pyconcept-0.1.4/ccl/core/src/oss/ossGridFacet.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/core/src/oss/ossOperationsFacet.cpp` & `pyconcept-0.1.4/ccl/core/src/oss/ossOperationsFacet.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/core/src/oss/ossSourceFacet.cpp` & `pyconcept-0.1.4/ccl/core/src/oss/ossSourceFacet.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/core/src/semantic/rscore/ConceptRecord.cpp` & `pyconcept-0.1.4/ccl/core/src/semantic/rscore/ConceptRecord.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/core/src/semantic/rscore/CstList.cpp` & `pyconcept-0.1.4/ccl/core/src/semantic/rscore/CstList.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/core/src/semantic/rscore/IdentityManager.cpp` & `pyconcept-0.1.4/ccl/core/src/semantic/rscore/IdentityManager.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/core/src/semantic/rscore/RSCore.cpp` & `pyconcept-0.1.4/ccl/core/src/semantic/rscore/RSCore.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/core/src/semantic/rsform/RSForm.cpp` & `pyconcept-0.1.4/ccl/core/src/semantic/rsform/RSForm.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/core/src/semantic/rsform/rsModificationFacet.cpp` & `pyconcept-0.1.4/ccl/core/src/semantic/rsform/rsModificationFacet.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/core/src/semantic/rsform/rsOperationFacet.cpp` & `pyconcept-0.1.4/ccl/core/src/semantic/rsform/rsOperationFacet.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/core/src/semantic/rsmodel/InterpretationStorage.cpp` & `pyconcept-0.1.4/ccl/core/src/semantic/rsmodel/InterpretationStorage.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/core/src/semantic/rsmodel/RSModel.cpp` & `pyconcept-0.1.4/ccl/core/src/semantic/rsmodel/RSModel.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/core/src/semantic/rsmodel/rsCalculationFacet.cpp` & `pyconcept-0.1.4/ccl/core/src/semantic/rsmodel/rsCalculationFacet.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/core/src/semantic/rsmodel/rsValuesFacet.cpp` & `pyconcept-0.1.4/ccl/core/src/semantic/rsmodel/rsValuesFacet.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/core/src/semantic/schema/RSConcept.cpp` & `pyconcept-0.1.4/ccl/core/src/semantic/schema/RSConcept.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/core/src/semantic/schema/Schema.cpp` & `pyconcept-0.1.4/ccl/core/src/semantic/schema/Schema.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/core/src/semantic/thesaurus/TextConcept.cpp` & `pyconcept-0.1.4/ccl/core/src/semantic/thesaurus/TextConcept.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/core/src/semantic/thesaurus/Thesaurus.cpp` & `pyconcept-0.1.4/ccl/core/src/semantic/thesaurus/Thesaurus.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/core/src/tools/CstNameGenerator.cpp` & `pyconcept-0.1.4/ccl/core/src/tools/CstNameGenerator.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/core/src/tools/EntityGenerator.cpp` & `pyconcept-0.1.4/ccl/core/src/tools/EntityGenerator.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/core/unity/CCL.cpp` & `pyconcept-0.1.4/ccl/core/unity/CCL.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/header/ASTNormalizer.h` & `pyconcept-0.1.4/ccl/rslang/header/ASTNormalizer.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/header/AsciiLexerImpl.hpp` & `pyconcept-0.1.4/ccl/rslang/header/AsciiLexerImpl.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/header/GeneratorImplAST.h` & `pyconcept-0.1.4/ccl/rslang/header/GeneratorImplAST.h`

 * *Files 4% similar despite different names*

```diff
@@ -14,56 +14,57 @@
 
 public:
   static std::string FromTree(const SyntaxTree& ast, Syntax syntax);
 
 private:
   bool VisitDefault(Cursor iter);
 
-  bool ViGlobalDefinition(Cursor iter);
+  bool ViGlobalDeclaration(Cursor iter);
 
   bool ViFunctionDefinition(Cursor iter);
   bool ViFunctionCall(Cursor iter);
 
   // bool ViGlobal(Cursor iter);
+  // bool ViRadical(Cursor iter);
   // bool ViLocal(Cursor iter);
   // bool ViInteger(Cursor /*iter*/);
   // bool ViIntegerSet(Cursor iter)
   // bool ViEmptySet(Cursor iter);
 
-  bool ViLocalBind(Cursor iter);
-  bool ViLocalEnum(Cursor iter);
+  bool ViTupleDeclaration(Cursor iter);
+  bool ViEnumDeclaration(Cursor iter);
   bool ViArgumentsEnum(Cursor iter);
   bool ViArgument(Cursor iter);
 
   bool ViArithmetic(Cursor iter);
   bool ViCard(Cursor iter);
 
   bool ViQuantifier(Cursor iter);
   bool ViNegation(Cursor iter);
   bool ViLogicBinary(Cursor iter);
   bool ViEquals(Cursor iter);
-  bool ViOrdering(Cursor iter) { return ViEquals(iter); }
-  bool ViTypedPredicate(Cursor iter) { return ViEquals(iter); }
+  bool ViIntegerPredicate(Cursor iter) { return ViEquals(iter); }
+  bool ViSetexprPredicate(Cursor iter) { return ViEquals(iter); }
 
   bool ViDeclarative(Cursor iter);
   bool ViImperative(Cursor iter);
   bool ViImpDeclare(Cursor iter);
   bool ViImpAssign(Cursor iter);
   bool ViImpCheck(Cursor iter);
   bool ViRecursion(Cursor iter);
 
   bool ViDecart(Cursor iter);
   bool ViBoolean(Cursor iter);
 
   bool ViTuple(Cursor iter);
-  bool ViSetEnum(Cursor iter);
+  bool ViEnumeration(Cursor iter);
   bool ViBool(Cursor iter) { return ViCard(iter); }
   bool ViDebool(Cursor iter) { return ViCard(iter); }
 
-  bool ViTypedBinary(Cursor iter) { return ViArithmetic(iter); }
+  bool ViSetexprBinary(Cursor iter) { return ViArithmetic(iter); }
   bool ViProjectSet(Cursor iter) { return ViCard(iter); }
   bool ViProjectTuple(Cursor iter) { return ViCard(iter); }
   bool ViFilter(Cursor iter);
   bool ViReduce(Cursor iter) { return ViCard(iter); }
 
 private:
   void SetSyntax(const Syntax newSyntax) noexcept { syntax = newSyntax; }
```

### Comparing `pyconcept-0.1.3/ccl/rslang/header/MathLexerImpl.hpp` & `pyconcept-0.1.4/ccl/rslang/header/MathLexerImpl.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/header/NameCollector.h` & `pyconcept-0.1.4/ccl/rslang/header/NameCollector.h`

 * *Files 11% similar despite different names*

```diff
@@ -18,17 +18,18 @@
 
 public:
   bool Visit(Cursor iter);
 
 protected:
   bool VisitDefault(Cursor iter) { return MergeChildren(iter); }
 
-  bool ViGlobalDefinition(Cursor iter);
+  bool ViGlobalDeclaration(Cursor iter);
 
   bool ViGlobal(Cursor iter);
+  // bool ViRadical(Cursor iter);
   bool ViLocal(Cursor iter);
 
   bool ViQuantifier(Cursor iter);
 
   bool ViDeclarative(Cursor iter) { return ViQuantifier(iter); }
   bool ViImperative(Cursor iter);
   bool ViRecursion(Cursor iter) { return ViQuantifier(iter); }
```

### Comparing `pyconcept-0.1.3/ccl/rslang/header/RSParserImpl.h` & `pyconcept-0.1.4/ccl/rslang/header/RSParserImpl.h`

 * *Files 1% similar despite different names*

```diff
@@ -442,52 +442,51 @@
         S_RS = 57,                               // RS
         S_BAR = 58,                              // BAR
         S_COMMA = 59,                            // COMMA
         S_SEMICOLON = 60,                        // SEMICOLON
         S_YYACCEPT = 61,                         // $accept
         S_expression = 62,                       // expression
         S_global_declaration = 63,               // global_declaration
-        S_function_name = 64,                    // function_name
-        S_logic_or_setexpr = 65,                 // logic_or_setexpr
-        S_function_decl = 66,                    // function_decl
-        S_arguments = 67,                        // arguments
-        S_declaration = 68,                      // declaration
-        S_variable = 69,                         // variable
-        S_var_enum = 70,                         // var_enum
-        S_var_all = 71,                          // var_all
-        S_logic = 72,                            // logic
-        S_logic_all = 73,                        // logic_all
-        S_logic_par = 74,                        // logic_par
-        S_logic_predicates = 75,                 // logic_predicates
-        S_binary_predicate = 76,                 // binary_predicate
-        S_logic_unary = 77,                      // logic_unary
-        S_logic_no_binary = 78,                  // logic_no_binary
-        S_quantifier = 79,                       // quantifier
-        S_quant_var = 80,                        // quant_var
-        S_quant_var_enum = 81,                   // quant_var_enum
-        S_logic_binary = 82,                     // logic_binary
-        S_setexpr = 83,                          // setexpr
-        S_operation_name = 84,                   // operation_name
-        S_setexpr_enum = 85,                     // setexpr_enum
-        S_setexpr_enum_min2 = 86,                // setexpr_enum_min2
-        S_literal = 87,                          // literal
-        S_identifier = 88,                       // identifier
-        S_setexpr_binary = 89,                   // setexpr_binary
-        S_setexpr_generators = 90,               // setexpr_generators
-        S_enumeration = 91,                      // enumeration
-        S_tuple = 92,                            // tuple
-        S_boolean = 93,                          // boolean
-        S_filter_expression = 94,                // filter_expression
-        S_declarative = 95,                      // declarative
-        S_recursion = 96,                        // recursion
-        S_imperative = 97,                       // imperative
-        S_imp_blocks = 98,                       // imp_blocks
-        S_imp_block = 99,                        // imp_block
-        S_RPE = 100,                             // RPE
-        S_RCE = 101                              // RCE
+        S_logic_or_setexpr = 64,                 // logic_or_setexpr
+        S_function_definition = 65,              // function_definition
+        S_arguments = 66,                        // arguments
+        S_declaration = 67,                      // declaration
+        S_variable = 68,                         // variable
+        S_var_enum = 69,                         // var_enum
+        S_var_all = 70,                          // var_all
+        S_logic = 71,                            // logic
+        S_logic_all = 72,                        // logic_all
+        S_logic_par = 73,                        // logic_par
+        S_logic_predicates = 74,                 // logic_predicates
+        S_binary_predicate = 75,                 // binary_predicate
+        S_logic_unary = 76,                      // logic_unary
+        S_logic_no_binary = 77,                  // logic_no_binary
+        S_quantifier = 78,                       // quantifier
+        S_quant_var = 79,                        // quant_var
+        S_quant_var_enum = 80,                   // quant_var_enum
+        S_logic_binary = 81,                     // logic_binary
+        S_setexpr = 82,                          // setexpr
+        S_text_function = 83,                    // text_function
+        S_setexpr_enum = 84,                     // setexpr_enum
+        S_setexpr_enum_min2 = 85,                // setexpr_enum_min2
+        S_literal = 86,                          // literal
+        S_identifier = 87,                       // identifier
+        S_setexpr_binary = 88,                   // setexpr_binary
+        S_setexpr_generators = 89,               // setexpr_generators
+        S_enumeration = 90,                      // enumeration
+        S_tuple = 91,                            // tuple
+        S_boolean = 92,                          // boolean
+        S_filter_expression = 93,                // filter_expression
+        S_declarative = 94,                      // declarative
+        S_recursion = 95,                        // recursion
+        S_imperative = 96,                       // imperative
+        S_imp_blocks = 97,                       // imp_blocks
+        S_imp_block = 98,                        // imp_block
+        S_RPE = 99,                              // RPE
+        S_RCE = 100                              // RCE
       };
     };
 
     /// (Internal) symbol kind.
     typedef symbol_kind::symbol_kind_type symbol_kind_type;
 
     /// The number of tokens.
@@ -977,27 +976,27 @@
 
     /// Pop \a n symbols from the stack.
     void yypop_ (int n = 1);
 
     /// Constants.
     enum
     {
-      yylast_ = 589,     ///< Last index in yytable_.
-      yynnts_ = 41,  ///< Number of nonterminal symbols.
-      yyfinal_ = 85 ///< Termination state number.
+      yylast_ = 640,     ///< Last index in yytable_.
+      yynnts_ = 40,  ///< Number of nonterminal symbols.
+      yyfinal_ = 87 ///< Termination state number.
     };
 
 
     // User arguments.
     ParserState* state;
 
   };
 
 
 #line 15 "RSParserImpl.y"
 } } } // ccl::rslang::detail
-#line 999 "../header/RSParserImpl.h"
+#line 998 "../header/RSParserImpl.h"
 
 
 
 
 #endif // !YY_YY_HEADER_RSPARSERIMPL_H_INCLUDED
```

### Comparing `pyconcept-0.1.3/ccl/rslang/header/SDImplementation.h` & `pyconcept-0.1.4/ccl/rslang/header/SDImplementation.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/abslexer.h` & `pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/abslexer.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/absmatcher.h` & `pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/absmatcher.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/bits.h` & `pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/bits.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/boostmatcher.h` & `pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/boostmatcher.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/convert.h` & `pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/convert.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/debug.h` & `pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/debug.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/error.h` & `pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/error.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/flexlexer.h` & `pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/flexlexer.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/input.h` & `pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/input.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/linematcher.h` & `pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/linematcher.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/matcher.h` & `pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/matcher.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/pattern.h` & `pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/pattern.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/pcre2matcher.h` & `pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/pcre2matcher.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/posix.h` & `pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/posix.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/ranges.h` & `pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/ranges.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/setop.h` & `pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/setop.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/simd.h` & `pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/simd.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/stdmatcher.h` & `pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/stdmatcher.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/timer.h` & `pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/timer.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/traits.h` & `pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/traits.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/unicode.h` & `pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/unicode.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/import/reflex/include/reflex/utf8.h` & `pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/utf8.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/import/reflex/lib/convert.cpp` & `pyconcept-0.1.4/ccl/rslang/import/reflex/lib/convert.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/import/reflex/lib/debug.cpp` & `pyconcept-0.1.4/ccl/rslang/import/reflex/lib/debug.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/import/reflex/lib/error.cpp` & `pyconcept-0.1.4/ccl/rslang/import/reflex/lib/error.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/import/reflex/lib/input.cpp` & `pyconcept-0.1.4/ccl/rslang/import/reflex/lib/input.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/import/reflex/lib/matcher.cpp` & `pyconcept-0.1.4/ccl/rslang/import/reflex/lib/matcher.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/import/reflex/lib/matcher_avx2.cpp` & `pyconcept-0.1.4/ccl/rslang/import/reflex/lib/matcher_avx2.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/import/reflex/lib/matcher_avx512bw.cpp` & `pyconcept-0.1.4/ccl/rslang/import/reflex/lib/matcher_avx512bw.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/import/reflex/lib/pattern.cpp` & `pyconcept-0.1.4/ccl/rslang/import/reflex/lib/pattern.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/import/reflex/lib/posix.cpp` & `pyconcept-0.1.4/ccl/rslang/import/reflex/lib/posix.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/import/reflex/lib/simd_avx2.cpp` & `pyconcept-0.1.4/ccl/rslang/import/reflex/lib/simd_avx2.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/import/reflex/lib/simd_avx512bw.cpp` & `pyconcept-0.1.4/ccl/rslang/import/reflex/lib/simd_avx512bw.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/import/reflex/lib/unicode.cpp` & `pyconcept-0.1.4/ccl/rslang/import/reflex/lib/unicode.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/import/reflex/lib/utf8.cpp` & `pyconcept-0.1.4/ccl/rslang/import/reflex/lib/utf8.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/import/reflex/unicode/block_scripts.cpp` & `pyconcept-0.1.4/ccl/rslang/import/reflex/unicode/block_scripts.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/import/reflex/unicode/composer.cpp` & `pyconcept-0.1.4/ccl/rslang/import/reflex/unicode/composer.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/import/reflex/unicode/language_scripts.cpp` & `pyconcept-0.1.4/ccl/rslang/import/reflex/unicode/language_scripts.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/import/reflex/unicode/letter_scripts.cpp` & `pyconcept-0.1.4/ccl/rslang/import/reflex/unicode/letter_scripts.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/ASTInterpreter.h` & `pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/ASTInterpreter.h`

 * *Files 10% similar despite different names*

```diff
@@ -46,72 +46,73 @@
 public:
   [[nodiscard]] std::optional<ExpressionValue> Evaluate(const SyntaxTree& tree);
   [[nodiscard]] int32_t Iterations() const noexcept { return iterationCounter; }
 
 protected:
   bool VisitDefault(Cursor /*iter*/) noexcept { return false; } // NOLINT(readability-convert-member-functions-to-static)
 
-  bool ViGlobalDefinition(Cursor iter);
+  bool ViGlobalDeclaration(Cursor iter);
 
   // bool ViFunctionDefinition(Cursor iter)
   // bool ViFunctionCall(Cursor iter);
 
   bool ViGlobal(Cursor iter) { return ViLocal(iter); }
+  // bool ViRadical(Cursor iter);
   bool ViLocal(Cursor iter);
   bool ViInteger(Cursor /*iter*/);
   bool ViIntegerSet(Cursor /*iter*/);
   bool ViEmptySet(Cursor iter);
 
-  //bool ViLocalBind(Cursor iter);
-  //bool ViLocalEnum(Cursor iter);
+  //bool ViTupleDeclaration(Cursor iter);
+  //bool ViEnumDeclaration(Cursor iter);
   //bool ViArgumentsEnum(Cursor iter);
   //bool ViArgument(Cursor iter);
 
   bool ViArithmetic(Cursor iter);
   bool ViCard(Cursor iter);
 
   bool ViQuantifier(Cursor iter);
   bool ViNegation(Cursor iter);
   bool ViLogicBinary(Cursor iter);
   bool ViEquals(Cursor iter);
-  bool ViOrdering(Cursor iter);
-  bool ViTypedPredicate(Cursor iter) { return ViTypedBinary(iter); }
+  bool ViIntegerPredicate(Cursor iter);
+  bool ViSetexprPredicate(Cursor iter) { return ViSetexprBinary(iter); }
 
   bool ViDecart(Cursor iter);
   bool ViBoolean(Cursor iter);
 
   bool ViDeclarative(Cursor iter);
   bool ViImperative(Cursor iter);
   //bool ViImpDeclare(Cursor iter);
   //bool ViImpAssign(Cursor iter);
   //bool ViImpCheck(Cursor iter);
   bool ViRecursion(Cursor iter);
 
   bool ViTuple(Cursor iter);
-  bool ViSetEnum(Cursor iter);
+  bool ViEnumeration(Cursor iter);
   bool ViBool(Cursor iter);
   bool ViDebool(Cursor iter);
 
-  bool ViTypedBinary(Cursor iter);
+  bool ViSetexprBinary(Cursor iter);
   bool ViProjectSet(Cursor iter);
   bool ViProjectTuple(Cursor iter);
   bool ViFilter(Cursor iter);
   bool ViReduce(Cursor iter);
 
 private:
   class ImpEvaluator;
 
   void Clear() noexcept;
   void AfterVisit(bool result);
 
   void OnError(ValueEID eid, StrPos position);
   void OnError(ValueEID eid, StrPos position, std::string param);
 
-  [[nodiscard]] bool VisitAndReturn(ExpressionValue&& value) noexcept;
-  [[nodiscard]] bool VisitAndReturn(const ExpressionValue& value) noexcept;
+  [[nodiscard]] bool SetCurrent(ExpressionValue&& value) noexcept;
+  [[nodiscard]] bool SetCurrent(const ExpressionValue& value) noexcept;
   [[nodiscard]] std::optional<ExpressionValue> EvaluateChild(Cursor iter, Index index);
 
   [[nodiscard]] std::optional<object::StructuredData> ExtractDomain(Cursor iter);
   [[nodiscard]] bool TryEvaluateFromFirstArg(TokenID operation, bool firstArgValue) noexcept;
 };
 
 } // namespace ccl::rslang
```

### Comparing `pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/AsciiLexer.h` & `pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/AsciiLexer.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/Auditor.h` & `pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/Auditor.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/Error.hpp` & `pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/Error.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/ErrorLogger.h` & `pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/ErrorLogger.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/Interpreter.h` & `pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/Interpreter.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/LexerBase.hpp` & `pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/LexerBase.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/MathLexer.h` & `pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/MathLexer.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/Parser.h` & `pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/Parser.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/ParserState.hpp` & `pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/ParserState.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/RSErrorCodes.hpp` & `pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/RSErrorCodes.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/RSExpr.h` & `pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/RSExpr.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/RSGenerator.h` & `pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/RSGenerator.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/RSParser.h` & `pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/RSParser.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/RSToken.h` & `pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/RSToken.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/SDataCompact.h` & `pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/SDataCompact.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/Structure.hpp` & `pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/Structure.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/StructuredData.h` & `pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/StructuredData.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/SyntaxTree.h` & `pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/SyntaxTree.h`

 * *Files 5% similar despite different names*

```diff
@@ -139,73 +139,59 @@
     template<typename Visitor>
     bool DispatchVisit(Visitor& visitor) {
       switch (node->token.id) {
       default:
       case TokenID::PUNC_DEFINE:
       case TokenID::PUNC_STRUCT:
         assert(ChildrenCount() != 0);
-        return visitor.ViGlobalDefinition(*this);
+        return visitor.ViGlobalDeclaration(*this);
 
       case TokenID::ID_GLOBAL:
       case TokenID::ID_FUNCTION:
       case TokenID::ID_PREDICATE:
-      case TokenID::ID_RADICAL:
         assert(ChildrenCount() == 0);
         return visitor.ViGlobal(*this);
 
+      case TokenID::ID_LOCAL:
+        assert(ChildrenCount() == 0);
+        return visitor.ViLocal(*this);
+
+      case TokenID::ID_RADICAL:
+        assert(ChildrenCount() == 0);
+        return visitor.ViRadical(*this);
+
       case TokenID::NT_FUNC_DEFINITION:
         assert(ChildrenCount() == 2);
         return visitor.ViFunctionDefinition(*this);
       case TokenID::NT_FUNC_CALL:
         assert(ChildrenCount() > 1);
         return visitor.ViFunctionCall(*this);
 
-      case TokenID::ID_LOCAL:
-        assert(ChildrenCount() == 0);
-        return visitor.ViLocal(*this);
-
       case TokenID::LIT_INTSET:
         assert(ChildrenCount() == 0);
         return visitor.ViIntegerSet(*this);
-
       case TokenID::LIT_INTEGER:
         assert(ChildrenCount() == 0);
         return visitor.ViInteger(*this);
       case TokenID::LIT_EMPTYSET:
         assert(ChildrenCount() == 0);
         return visitor.ViEmptySet(*this);
 
       case TokenID::NT_TUPLE_DECL:
         assert(ChildrenCount() > 1);
-        return visitor.ViLocalBind(*this);
+        return visitor.ViTupleDeclaration(*this);
       case TokenID::NT_ENUM_DECL:
-        return visitor.ViLocalEnum(*this);
+        return visitor.ViEnumDeclaration(*this);
       case TokenID::NT_ARGUMENTS:
         assert(ChildrenCount() > 0);
         return visitor.ViArgumentsEnum(*this);
       case TokenID::NT_ARG_DECL:
         assert(ChildrenCount() == 2);
         return visitor.ViArgument(*this);
 
-      case TokenID::NT_DECLARATIVE_EXPR:
-        assert(ChildrenCount() == 3);
-        return visitor.ViDeclarative(*this);
-      case TokenID::NT_IMPERATIVE_EXPR:
-        assert(ChildrenCount() > 1);
-        return visitor.ViImperative(*this);
-      case TokenID::NT_IMP_DECLARE:
-        assert(ChildrenCount() == 2);
-        return visitor.ViImpDeclare(*this);
-      case TokenID::NT_IMP_ASSIGN:
-        assert(ChildrenCount() == 2);
-        return visitor.ViImpAssign(*this);
-      case TokenID::NT_IMP_LOGIC:
-        assert(ChildrenCount() == 1);
-        return visitor.ViImpCheck(*this);
-
       case TokenID::PLUS:
       case TokenID::MINUS:
       case TokenID::MULTIPLY:
         assert(ChildrenCount() == 2);
         return visitor.ViArithmetic(*this);
       case TokenID::CARD:
         assert(ChildrenCount() == 1);
@@ -232,23 +218,39 @@
         return visitor.ViEquals(*this);
 
       case TokenID::GREATER:
       case TokenID::LESSER:
       case TokenID::GREATER_OR_EQ:
       case TokenID::LESSER_OR_EQ:
         assert(ChildrenCount() == 2);
-        return visitor.ViOrdering(*this);
+        return visitor.ViIntegerPredicate(*this);
 
       case TokenID::IN:
       case TokenID::NOTIN:
       case TokenID::SUBSET:
       case TokenID::SUBSET_OR_EQ:
       case TokenID::NOTSUBSET:
         assert(ChildrenCount() == 2);
-        return visitor.ViTypedPredicate(*this);
+        return visitor.ViSetexprPredicate(*this);
+
+      case TokenID::NT_DECLARATIVE_EXPR:
+        assert(ChildrenCount() == 3);
+        return visitor.ViDeclarative(*this);
+      case TokenID::NT_IMPERATIVE_EXPR:
+        assert(ChildrenCount() > 1);
+        return visitor.ViImperative(*this);
+      case TokenID::NT_IMP_DECLARE:
+        assert(ChildrenCount() == 2);
+        return visitor.ViImpDeclare(*this);
+      case TokenID::NT_IMP_ASSIGN:
+        assert(ChildrenCount() == 2);
+        return visitor.ViImpAssign(*this);
+      case TokenID::NT_IMP_LOGIC:
+        assert(ChildrenCount() == 1);
+        return visitor.ViImpCheck(*this);
 
       case TokenID::DECART:
         assert(ChildrenCount() > 1);
         return visitor.ViDecart(*this);
       case TokenID::BOOLEAN:
         assert(ChildrenCount() == 1);
         return visitor.ViBoolean(*this);
@@ -260,28 +262,28 @@
         assert(ChildrenCount() == 3);
         return visitor.ViRecursion(*this);
 
       case TokenID::NT_TUPLE:
         assert(ChildrenCount() > 1);
         return visitor.ViTuple(*this);
       case TokenID::NT_ENUMERATION:
-        return visitor.ViSetEnum(*this);
+        return visitor.ViEnumeration(*this);
       case TokenID::BOOL:
         assert(ChildrenCount() == 1);
         return visitor.ViBool(*this);
       case TokenID::DEBOOL:
         assert(ChildrenCount() == 1);
         return visitor.ViDebool(*this);
 
       case TokenID::UNION:
       case TokenID::INTERSECTION:
       case TokenID::SET_MINUS:
       case TokenID::SYMMINUS:
         assert(ChildrenCount() == 2);
-        return visitor.ViTypedBinary(*this);
+        return visitor.ViSetexprBinary(*this);
 
       case TokenID::BIGPR:
         assert(ChildrenCount() == 1);
         return visitor.ViProjectSet(*this);
       case TokenID::SMALLPR:
         assert(ChildrenCount() == 1);
         return visitor.ViProjectTuple(*this);
@@ -315,56 +317,57 @@
         return false;
       }
     }
     return true;
   }
 
 private:
-  bool ViGlobalDefinition(Cursor iter) { return this->BaseT().VisitDefault(iter); }
+  bool ViGlobalDeclaration(Cursor iter) { return this->BaseT().VisitDefault(iter); }
 
   bool ViFunctionDefinition(Cursor iter) { return this->BaseT().VisitDefault(iter); }
   bool ViFunctionCall(Cursor iter) { return this->BaseT().VisitDefault(iter); }
 
   bool ViGlobal(Cursor iter) { return this->BaseT().VisitDefault(iter); }
+  bool ViRadical(Cursor iter) { return this->BaseT().VisitDefault(iter); }
   bool ViLocal(Cursor iter)  { return this->BaseT().VisitDefault(iter); }
   bool ViInteger(Cursor iter) { return this->BaseT().VisitDefault(iter); }
   bool ViIntegerSet(Cursor iter) { return this->BaseT().VisitDefault(iter); }
   bool ViEmptySet(Cursor iter) { return this->BaseT().VisitDefault(iter); }
 
-  bool ViLocalBind(Cursor iter) { return this->BaseT().VisitDefault(iter); }
-  bool ViLocalEnum(Cursor iter) { return this->BaseT().VisitDefault(iter); }
+  bool ViTupleDeclaration(Cursor iter) { return this->BaseT().VisitDefault(iter); }
+  bool ViEnumDeclaration(Cursor iter) { return this->BaseT().VisitDefault(iter); }
   bool ViArgumentsEnum(Cursor iter) { return this->BaseT().VisitDefault(iter); }
   bool ViArgument(Cursor iter) { return this->BaseT().VisitDefault(iter); }
 
   bool ViArithmetic(Cursor iter) { return this->BaseT().VisitDefault(iter); }
   bool ViCard(Cursor iter) { return this->BaseT().VisitDefault(iter); }
 
   bool ViQuantifier(Cursor iter) { return this->BaseT().VisitDefault(iter); }
   bool ViNegation(Cursor iter) { return this->BaseT().VisitDefault(iter); }
   bool ViLogicBinary(Cursor iter) { return this->BaseT().VisitDefault(iter); }
   bool ViEquals(Cursor iter) { return this->BaseT().VisitDefault(iter); }
-  bool ViOrdering(Cursor iter) { return this->BaseT().VisitDefault(iter); }
-  bool ViTypedPredicate(Cursor iter) { return this->BaseT().VisitDefault(iter); }
+  bool ViIntegerPredicate(Cursor iter) { return this->BaseT().VisitDefault(iter); }
+  bool ViSetexprPredicate(Cursor iter) { return this->BaseT().VisitDefault(iter); }
 
   bool ViDeclarative(Cursor iter) { return this->BaseT().VisitDefault(iter); }
   bool ViImperative(Cursor iter) { return this->BaseT().VisitDefault(iter); }
   bool ViImpDeclare(Cursor iter) { return this->BaseT().VisitDefault(iter); }
   bool ViImpAssign(Cursor iter) { return this->BaseT().VisitDefault(iter); }
   bool ViImpCheck(Cursor iter) { return this->BaseT().VisitDefault(iter); }
   bool ViRecursion(Cursor iter) { return this->BaseT().VisitDefault(iter); }
 
   bool ViDecart(Cursor iter) { return this->BaseT().VisitDefault(iter); }
   bool ViBoolean(Cursor iter) { return this->BaseT().VisitDefault(iter); }
 
   bool ViTuple(Cursor iter) { return this->BaseT().VisitDefault(iter); }
-  bool ViSetEnum(Cursor iter) { return this->BaseT().VisitDefault(iter); }
+  bool ViEnumeration(Cursor iter) { return this->BaseT().VisitDefault(iter); }
   bool ViBool(Cursor iter) { return this->BaseT().VisitDefault(iter); }
   bool ViDebool(Cursor iter) { return this->BaseT().VisitDefault(iter); }
 
-  bool ViTypedBinary(Cursor iter)  { return this->BaseT().VisitDefault(iter); }
+  bool ViSetexprBinary(Cursor iter)  { return this->BaseT().VisitDefault(iter); }
   bool ViProjectSet(Cursor iter) { return this->BaseT().VisitDefault(iter); }
   bool ViProjectTuple(Cursor iter) { return this->BaseT().VisitDefault(iter); }
   bool ViFilter(Cursor iter) { return this->BaseT().VisitDefault(iter); }
   bool ViReduce(Cursor iter) { return this->BaseT().VisitDefault(iter); }
 };
 
 #ifdef _MSC_VER
```

### Comparing `pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/TypeAuditor.h` & `pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/TypeAuditor.h`

 * *Files 7% similar despite different names*

```diff
@@ -54,94 +54,98 @@
   std::vector<size_t> functionArgsID{};
   FunctionArguments functionArgs{};
 
   bool isTypification{ false };
   types::GuardableBool isArgDeclaration{ false };
   types::GuardableBool isLocalDeclaration{ false };
   types::GuardableBool isFuncDeclaration{ false };
+  types::GuardableBool noWarnings{ false };
 
 public:
   explicit TypeAuditor(const TypeContext& context) noexcept
     : env{ context } {}
   explicit TypeAuditor(const TypeContext& context, ErrorReporter reporter) noexcept
     : env{ context }, reporter{ std::move(reporter) } {}
 
 public:
   [[nodiscard]] bool CheckType(const SyntaxTree& tree);
   [[nodiscard]] const FunctionArguments& GetDeclarationArgs() const noexcept { return functionArgs; }
   [[nodiscard]] const ExpressionType& GetType() const noexcept;
   void SetExepectTypification(const bool value = true) noexcept;
 
 protected:
-  bool ViGlobalDefinition(Cursor iter);
+  bool ViGlobalDeclaration(Cursor iter);
 
   bool ViFunctionDefinition(Cursor iter);
   bool ViFunctionCall(Cursor iter);
 
   bool ViGlobal(Cursor iter);
+  bool ViRadical(Cursor iter);
   bool ViLocal(Cursor iter);
-  bool ViInteger(Cursor /*iter*/) { return VisitAndReturn(Typification::Integer()); }
-  bool ViIntegerSet(Cursor /*iter*/) { return VisitAndReturn(Typification::Integer().Bool()); }
+  bool ViInteger(Cursor /*iter*/) { return SetCurrent(Typification::Integer()); }
+  bool ViIntegerSet(Cursor /*iter*/) { return SetCurrent(Typification::Integer().Bool()); }
   bool ViEmptySet(Cursor /*iter*/);
 
-  bool ViLocalBind(Cursor iter);
-  bool ViLocalEnum(Cursor iter) { return VisitAllAndReturn(iter, LogicT{}); }
-  bool ViArgumentsEnum(Cursor iter) { return VisitAllAndReturn(iter, LogicT{}); }
+  bool ViTupleDeclaration(Cursor iter);
+  bool ViEnumDeclaration(Cursor iter) { return VisitAllAndSetCurrent(iter, LogicT{}); }
+  bool ViArgumentsEnum(Cursor iter) { return VisitAllAndSetCurrent(iter, LogicT{}); }
   bool ViArgument(Cursor iter);
 
   bool ViArithmetic(Cursor iter);
   bool ViCard(Cursor iter);
 
   bool ViQuantifier(Cursor iter);
-  bool ViNegation(Cursor iter) { return VisitAllAndReturn(iter, LogicT{}); }
-  bool ViLogicBinary(Cursor iter) { return VisitAllAndReturn(iter, LogicT{}); }
+  bool ViNegation(Cursor iter) { return VisitAllAndSetCurrent(iter, LogicT{}); }
+  bool ViLogicBinary(Cursor iter) { return VisitAllAndSetCurrent(iter, LogicT{}); }
   bool ViEquals(Cursor iter);
-  bool ViOrdering(Cursor iter);
-  bool ViTypedPredicate(Cursor iter);
+  bool ViIntegerPredicate(Cursor iter);
+  bool ViSetexprPredicate(Cursor iter);
 
   bool ViDecart(Cursor iter);
   bool ViBoolean(Cursor iter);
 
   bool ViDeclarative(Cursor iter);
   bool ViImperative(Cursor iter);
   bool ViImpDeclare(Cursor iter);
   bool ViImpAssign(Cursor iter);
-  bool ViImpCheck(Cursor iter) { return VisitAllAndReturn(iter, LogicT{}); }
+  bool ViImpCheck(Cursor iter) { return VisitAllAndSetCurrent(iter, LogicT{}); }
   bool ViRecursion(Cursor iter);
 
   bool ViTuple(Cursor iter);
-  bool ViSetEnum(Cursor iter);
-  bool ViBool(Cursor iter) { return ViSetEnum(iter); }
+  bool ViEnumeration(Cursor iter);
+  bool ViBool(Cursor iter) { return ViEnumeration(iter); }
   bool ViDebool(Cursor iter);
 
-  bool ViTypedBinary(Cursor iter);
+  bool ViSetexprBinary(Cursor iter);
   bool ViProjectSet(Cursor iter);
   bool ViProjectTuple(Cursor iter);
   bool ViFilter(Cursor iter);
   bool ViReduce(Cursor iter);
 
 private:
   void Clear() noexcept;
 
   [[nodiscard]] bool VisitChildDeclaration(const Cursor& iter, Index index, const Typification& domain);
 
-  [[nodiscard]] bool VisitAndReturn(ExpressionType type) noexcept;
-  [[nodiscard]] bool VisitAllAndReturn(Cursor iter, const ExpressionType& type);
+  [[nodiscard]] bool SetCurrent(ExpressionType type) noexcept;
+  [[nodiscard]] bool VisitAllAndSetCurrent(Cursor iter, const ExpressionType& type);
 
   [[nodiscard]] std::optional<ExpressionType> ChildType(Cursor iter, Index index);
   [[nodiscard]] std::optional<Typification> ChildTypeDebool(Cursor iter, Index index,  SemanticEID eid);
 
   void OnError(SemanticEID eid, StrPos position);
   void OnError(SemanticEID eid, StrPos position, std::string param);
   void OnError(SemanticEID eid, StrPos position, std::vector<std::string> params);
   void OnError(SemanticEID eid, StrPos position, const ExpressionType& expected, const ExpressionType& actual);
 
   [[nodiscard]] std::optional<Typification::Substitutes> 
     CheckFuncArguments(Cursor iter, const std::string& funcName);
 
   [[nodiscard]] const Typification* GetLocalTypification(const std::string& name, StrPos pos);
-  [[nodiscard]] bool AddLocalVar(const std::string& name, const Typification& type, StrPos pos);
+  [[nodiscard]] bool AddLocalVariable(const std::string& name, const Typification& type, StrPos pos);
+  void ClearLocalVariables();
+
   void StartScope() noexcept;
   void EndScope(StrPos pos);
 };
 
 } // namespace ccl::rslang
```

### Comparing `pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/TypeContext.hpp` & `pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/TypeContext.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/Typification.h` & `pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/Typification.h`

 * *Files 1% similar despite different names*

```diff
@@ -89,14 +89,16 @@
   [[nodiscard]] static Typification Tuple(std::vector<Typification> factors);
   [[nodiscard]] static const Typification& Integer();
   [[nodiscard]] static const Typification& EmptySet();
 
 public:
   using Substitutes = std::unordered_map<std::string, Typification>;
 
+  [[nodiscard]] bool IsAnyType() const noexcept;
+
   Typification& ApplyBool();
   [[nodiscard]] Typification Bool() const;
 
   [[nodiscard]] bool operator==(const Typification& t2) const noexcept { return state == t2.state; }
   [[nodiscard]] bool operator!=(const Typification& t2) const noexcept { return !(*this == t2); }
 
   [[nodiscard]] std::string ToString() const noexcept(false);
```

### Comparing `pyconcept-0.1.3/ccl/rslang/include/ccl/rslang/ValueAuditor.h` & `pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/ValueAuditor.h`

 * *Files 20% similar despite different names*

```diff
@@ -29,65 +29,66 @@
     : globalClass{ std::move(globalClass) }, globalAST{ std::move(globalAST) }, reporter{ std::move(reporter) } {}
 
 public:
   [[nodiscard]] bool Check(const SyntaxTree& tree);
   [[nodiscard]] ValueClass VType() const noexcept { return current; }
 
 protected:
-  bool ViGlobalDefinition(Cursor iter);
+  bool ViGlobalDeclaration(Cursor iter);
 
   bool ViFunctionDefinition(Cursor iter) { return VisitAllChildren(iter); }
   bool ViFunctionCall(Cursor iter);
 
   bool ViGlobal(Cursor iter);
+  bool ViRadical(Cursor /*iter*/);
   bool ViLocal(Cursor iter);
-  bool ViInteger(Cursor /*iter*/) noexcept { return VisitAndReturn(ValueClass::value); }
-  bool ViIntegerSet(Cursor /*iter*/) noexcept { return VisitAndReturn(ValueClass::props); }
-  bool ViEmptySet(Cursor /*iter*/) noexcept { return VisitAndReturn(ValueClass::value); }
+  bool ViInteger(Cursor /*iter*/) noexcept { return SetCurrent(ValueClass::value); }
+  bool ViIntegerSet(Cursor /*iter*/) noexcept { return SetCurrent(ValueClass::props); }
+  bool ViEmptySet(Cursor /*iter*/) noexcept { return SetCurrent(ValueClass::value); }
 
-  bool ViLocalBind(Cursor iter) { return VisitAllAndReturn(iter, ValueClass::value); }
-  bool ViLocalEnum(Cursor iter) { return VisitAllAndReturn(iter, ValueClass::value); }
+  bool ViTupleDeclaration(Cursor iter) { return VisitAllAndSetCurrent(iter, ValueClass::value); }
+  bool ViEnumDeclaration(Cursor iter) { return VisitAllAndSetCurrent(iter, ValueClass::value); }
   bool ViArgumentsEnum(Cursor iter) { return VisitAllChildren(iter); }
   bool ViArgument(Cursor iter) { return VisitAllChildren(iter); }
 
-  bool ViArithmetic(Cursor iter) { return VisitAllAndReturn(iter, ValueClass::value); }
+  bool ViArithmetic(Cursor iter) { return VisitAllAndSetCurrent(iter, ValueClass::value); }
   bool ViCard(Cursor iter) { return AssertChildIsValue(iter, 0); }
 
   bool ViQuantifier(Cursor iter);
-  bool ViNegation(Cursor iter) { return VisitAllAndReturn(iter, ValueClass::value); }
-  bool ViLogicBinary(Cursor iter) { return VisitAllAndReturn(iter, ValueClass::value); }
+  bool ViNegation(Cursor iter) { return VisitAllAndSetCurrent(iter, ValueClass::value); }
+  bool ViLogicBinary(Cursor iter) { return VisitAllAndSetCurrent(iter, ValueClass::value); }
   bool ViEquals(Cursor iter) { return AssertAllValues(iter); }
-  bool ViOrdering(Cursor iter) { return VisitAllAndReturn(iter, ValueClass::value); }
-  bool ViTypedPredicate(Cursor iter);
+  bool ViIntegerPredicate(Cursor iter) { return VisitAllAndSetCurrent(iter, ValueClass::value); }
+  bool ViSetexprPredicate(Cursor iter);
 
   bool ViDecart(Cursor iter);
   bool ViBoolean(Cursor iter);
 
   bool ViDeclarative(Cursor iter);
   bool ViImperative(Cursor iter);
   bool ViImpDeclare(Cursor iter) { return AssertChildIsValue(iter, 1); }
   bool ViImpAssign(Cursor iter) { return AssertChildIsValue(iter, 1); }
-  bool ViImpCheck(Cursor iter) { return VisitAllAndReturn(iter, ValueClass::value); }
+  bool ViImpCheck(Cursor iter) { return VisitAllAndSetCurrent(iter, ValueClass::value); }
   bool ViRecursion(Cursor iter) { return AssertAllValues(iter); }
 
   bool ViTuple(Cursor iter) { return AssertAllValues(iter); }
-  bool ViSetEnum(Cursor iter) { return AssertAllValues(iter); }
+  bool ViEnumeration(Cursor iter) { return AssertAllValues(iter); }
   bool ViBool(Cursor iter) { return AssertChildIsValue(iter, 0); }
   bool ViDebool(Cursor iter) { return AssertChildIsValue(iter, 0); }
 
-  bool ViTypedBinary(Cursor iter);
+  bool ViSetexprBinary(Cursor iter);
   bool ViProjectSet(Cursor iter) { return AssertChildIsValue(iter, 0); }
   bool ViProjectTuple(Cursor iter) { return AssertChildIsValue(iter, 0); }
   bool ViFilter(Cursor iter) { return VisitAllChildren(iter); }
   bool ViReduce(Cursor iter) { return AssertChildIsValue(iter, 0); }
 
 private:
   void Clear() noexcept;
-  [[nodiscard]] bool VisitAndReturn(ValueClass type) noexcept;
-  [[nodiscard]] bool VisitAllAndReturn(Cursor iter, ValueClass type);
+  [[nodiscard]] bool SetCurrent(ValueClass type) noexcept;
+  [[nodiscard]] bool VisitAllAndSetCurrent(Cursor iter, ValueClass type);
 
   [[nodiscard]] bool AssertAllValues(Cursor iter);
   [[nodiscard]] bool AssertChildIsValue(Cursor iter, Index index);
 
   [[nodiscard]] bool RunCheckOnFunc(Cursor iter, 
                                     const std::string& funcName, 
                                     const std::vector<ValueClass>& argumentVals);
```

### Comparing `pyconcept-0.1.3/ccl/rslang/src/ASTInterpreter.cpp` & `pyconcept-0.1.4/ccl/rslang/src/ASTInterpreter.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -211,43 +211,43 @@
   idsData.clear();
   nodeVars.clear();
   curValue = {};
   iterationCounter = 0;
   countCriticalErrors = 0;
 }
 
-bool ASTInterpreter::VisitAndReturn(ExpressionValue&& value) noexcept {
+bool ASTInterpreter::SetCurrent(ExpressionValue&& value) noexcept {
   curValue = std::move(value);
   return true;
 }
 
-bool ASTInterpreter::VisitAndReturn(const ExpressionValue& value) noexcept {
+bool ASTInterpreter::SetCurrent(const ExpressionValue& value) noexcept {
   curValue = value;
   return true;
 }
 
-bool ASTInterpreter::ViGlobalDefinition(Cursor iter) {
+bool ASTInterpreter::ViGlobalDeclaration(Cursor iter) {
   return VisitChild(iter, 1);
 }
 
 bool ASTInterpreter::ViLocal(Cursor iter) {
-  return VisitAndReturn(idsData[*begin(nodeVars[iter.get()])]);
+  return SetCurrent(idsData[*begin(nodeVars[iter.get()])]);
 }
 
 bool ASTInterpreter::ViInteger(Cursor iter) {
-  return VisitAndReturn(Factory::Val(iter->data.ToInt()));
+  return SetCurrent(Factory::Val(iter->data.ToInt()));
 }
 
 bool ASTInterpreter::ViIntegerSet(Cursor iter) {
   OnError(ValueEID::iterateInfinity, iter->pos.start);
   return false;
 }
 
 bool ASTInterpreter::ViEmptySet(Cursor /*iter*/) {
-  return VisitAndReturn(Factory::EmptySet());
+  return SetCurrent(Factory::EmptySet());
 }
 
 bool ASTInterpreter::ViArithmetic(Cursor iter) {
   const auto val1 = EvaluateChild(iter, 0);
   if (!val1.has_value()) {
     return false;
   }
@@ -256,33 +256,33 @@
     return false;
   }
   const auto op1 = std::get<StructuredData>(val1.value()).E().Value();
   const auto op2 = std::get<StructuredData>(val2.value()).E().Value();
   switch (iter->id) {
   default:
   case TokenID::PLUS:
-    return VisitAndReturn(Factory::Val(op1 + op2));
+    return SetCurrent(Factory::Val(op1 + op2));
   case TokenID::MINUS:
-    return VisitAndReturn(Factory::Val(op1 - op2));
+    return SetCurrent(Factory::Val(op1 - op2));
   case TokenID::MULTIPLY:
-    return VisitAndReturn(Factory::Val(op1 * op2));
+    return SetCurrent(Factory::Val(op1 * op2));
   }
 }
 
 bool ASTInterpreter::ViCard(Cursor iter) {
   const auto base = EvaluateChild(iter, 0);
   if (!base.has_value()) {
     return false;
   }
   const auto size = std::get<StructuredData>(base.value()).B().Cardinality();
   if (size == StructuredData::SET_INFINITY) {
     OnError(ValueEID::typedOverflow, iter->pos.start, std::to_string(StructuredData::SET_INFINITY));
     return false;
   }
-  return VisitAndReturn(Factory::Val(size));
+  return SetCurrent(Factory::Val(size));
 }
 
 bool ASTInterpreter::ViQuantifier(Cursor iter) {
   const auto domain = ExtractDomain(iter);
   if (!domain.has_value()) {
     return false;
   }
@@ -294,33 +294,33 @@
       OnError(ValueEID::iterationsLimit, iter->pos.start, std::to_string(MAX_ITERATIONS));
       return false;
     }
     idsData[varID] = child;
     if (const auto iterationValue = EvaluateChild(iter, 2); !iterationValue.has_value()) {
       return false;
     } else if (std::get<bool>(iterationValue.value()) != isUniversal) {
-      return VisitAndReturn(!isUniversal);
+      return SetCurrent(!isUniversal);
     }
   }
-  return VisitAndReturn(isUniversal);
+  return SetCurrent(isUniversal);
 }
 
 std::optional<StructuredData> ASTInterpreter::ExtractDomain(Cursor iter) {
   if (!VisitChild(iter, 1)) {
     return std::nullopt;
   }
   return std::optional<StructuredData>{std::get<StructuredData>(curValue)};
 }
 
 bool ASTInterpreter::ViNegation(Cursor iter) {
   const auto childValue = EvaluateChild(iter, 0);
   if (!childValue.has_value()) {
     return false;
   }
-  return VisitAndReturn(!std::get<bool>(childValue.value()));
+  return SetCurrent(!std::get<bool>(childValue.value()));
 }
 
 bool ASTInterpreter::ViLogicBinary(Cursor iter) {
   const auto val1 = EvaluateChild(iter, 0);
   if (!val1.has_value()) {
     return false;
   }
@@ -343,51 +343,51 @@
     case TokenID::EQUIVALENT: curValue = op1 == op2; return true;
   }
 }
 
 bool ASTInterpreter::TryEvaluateFromFirstArg(TokenID operation, bool firstArgValue) noexcept {
   if ((operation == TokenID::AND && !firstArgValue) ||
     (operation == TokenID::OR && firstArgValue)) {
-    return VisitAndReturn(firstArgValue);
+    return SetCurrent(firstArgValue);
   } else if (operation == TokenID::IMPLICATION && !firstArgValue) {
-    return VisitAndReturn(!firstArgValue);
+    return SetCurrent(!firstArgValue);
   } else {
     return false;
   }
 }
 
 bool ASTInterpreter::ViEquals(Cursor iter) {
   const auto val1 = EvaluateChild(iter, 0);
   if (!val1.has_value()) {
     return false;
   }
   const auto val2 = EvaluateChild(iter, 1);
   if (!val2.has_value()) {
     return false;
   }
-  return VisitAndReturn((val1 == val2) != (iter->id == TokenID::NOTEQUAL));
+  return SetCurrent((val1 == val2) != (iter->id == TokenID::NOTEQUAL));
 }
 
-bool ASTInterpreter::ViOrdering(Cursor iter) {
+bool ASTInterpreter::ViIntegerPredicate(Cursor iter) {
   const auto val1 = EvaluateChild(iter, 0);
   if (!val1.has_value()) {
     return false;
   }
   const auto val2 = EvaluateChild(iter, 1);
   if (!val2.has_value()) {
     return false;
   }
   const auto op1 = std::get<StructuredData>(val1.value()).E().Value();
   const auto op2 = std::get<StructuredData>(val2.value()).E().Value();
   switch (iter->id) {
     default:
-    case TokenID::GREATER: return VisitAndReturn(op1 > op2);
-    case TokenID::LESSER: return VisitAndReturn(op1 < op2);
-    case TokenID::GREATER_OR_EQ: return VisitAndReturn(op1 >= op2);
-    case TokenID::LESSER_OR_EQ: return VisitAndReturn(op1 <= op2);
+    case TokenID::GREATER: return SetCurrent(op1 > op2);
+    case TokenID::LESSER: return SetCurrent(op1 < op2);
+    case TokenID::GREATER_OR_EQ: return SetCurrent(op1 >= op2);
+    case TokenID::LESSER_OR_EQ: return SetCurrent(op1 <= op2);
   }
 }
 
 bool ASTInterpreter::ViDeclarative(Cursor iter) {
   const auto setDomain = ExtractDomain(iter);
   if (!setDomain.has_value()) {
     return false;
@@ -404,23 +404,23 @@
     if (!predicatValue.has_value()) {
       return false;
     }
     if (std::get<bool>(predicatValue.value())) {
       result.ModifyB().AddElement(child);
     }
   }
-  return VisitAndReturn(std::move(result));
+  return SetCurrent(std::move(result));
 }
 
 bool ASTInterpreter::ViImperative(const Cursor iter) {
   ImpEvaluator eval{ *this, iter };
   if (!eval.Evaluate()) {
     return false;
   }
-  return VisitAndReturn(eval.value);
+  return SetCurrent(eval.value);
 }
 
 bool ASTInterpreter::ViRecursion(Cursor iter) {
   const auto initial = ExtractDomain(iter);
   if (!initial.has_value()) {
     return false;
   }
@@ -444,15 +444,15 @@
     }
 
     if (!VisitChild(iter, iter->id == TokenID::NT_RECURSIVE_FULL ? 3 : 2)) {
       return false;
     }
     current = std::get<StructuredData>(curValue);
   } while (idsData[varID] != current);
-  return VisitAndReturn(std::move(current));
+  return SetCurrent(std::move(current));
 }
 
 bool ASTInterpreter::ViDecart(Cursor iter) {
   std::vector<StructuredData> args{};
   for (Index child = 0; child < iter.ChildrenCount(); ++child) {
     if (const auto childValue = EvaluateChild(iter, child); !childValue.has_value()) {
       return false;
@@ -482,119 +482,119 @@
     OnError(
       ValueEID::booleanLimit,
       iter->pos.start,
       std::to_string(StructuredData::BOOL_INFINITY)
     );
     return false;
   }
-  return VisitAndReturn(Factory::Boolean(value));
+  return SetCurrent(Factory::Boolean(value));
 }
 
 bool ASTInterpreter::ViTuple(Cursor iter) {
   std::vector<StructuredData> args{};
   for (Index child = 0; child < iter.ChildrenCount(); ++child) {
     const auto childValue = EvaluateChild(iter, child);
     if (!childValue.has_value()) {
       return false;
     }
     args.emplace_back(std::get<StructuredData>(childValue.value()));
   }
-  return VisitAndReturn(Factory::Tuple(args));
+  return SetCurrent(Factory::Tuple(args));
 }
 
-bool ASTInterpreter::ViSetEnum(Cursor iter) {
+bool ASTInterpreter::ViEnumeration(Cursor iter) {
   std::vector<StructuredData> args{};
   for (Index child = 0; child < iter.ChildrenCount(); ++child) {
     const auto childValue = EvaluateChild(iter, child);
     if (!childValue.has_value()) {
       return false;
     }
     args.emplace_back(std::get<StructuredData>(childValue.value()));
   }
-  return VisitAndReturn(Factory::Set(args));
+  return SetCurrent(Factory::Set(args));
 }
 
 bool ASTInterpreter::ViBool(Cursor iter) {
   const auto childValue = EvaluateChild(iter, 0);
   if (!childValue.has_value()) {
     return false;
   }
-  return VisitAndReturn(Factory::Singleton(std::get<StructuredData>(childValue.value())));
+  return SetCurrent(Factory::Singleton(std::get<StructuredData>(childValue.value())));
 }
 
-bool ASTInterpreter::ViTypedBinary(Cursor iter) {
+bool ASTInterpreter::ViSetexprBinary(Cursor iter) {
   const auto val1 = EvaluateChild(iter, 0);
   if (!val1.has_value()) {
     return false;
   }
   const auto val2 = EvaluateChild(iter, 1); 
   if (!val2.has_value()) {
     return false;
   }
 
   const auto& op1 = std::get<StructuredData>(val1.value());
   const auto& op2 = std::get<StructuredData>(val2.value());
   switch (iter->id) {
     default:
-    case TokenID::UNION: return VisitAndReturn(op1.B().Union(op2.B()));
-    case TokenID::INTERSECTION: return VisitAndReturn(op1.B().Intersect(op2.B()));
-    case TokenID::SET_MINUS: return VisitAndReturn(op1.B().Diff(op2.B()));
-    case TokenID::SYMMINUS: return VisitAndReturn(op1.B().SymDiff(op2.B()));
-
-    case TokenID::IN: return VisitAndReturn(op2.B().Contains(op1));
-    case TokenID::NOTIN: return VisitAndReturn(!op2.B().Contains(op1));
-    case TokenID::SUBSET: return VisitAndReturn(!(op1 == op2) && op1.B().IsSubsetOrEq(op2.B()));
-    case TokenID::NOTSUBSET: return VisitAndReturn(op1 == op2 || !op1.B().IsSubsetOrEq(op2.B()));
-    case TokenID::SUBSET_OR_EQ: return VisitAndReturn(op1.B().IsSubsetOrEq(op2.B()));
+    case TokenID::UNION: return SetCurrent(op1.B().Union(op2.B()));
+    case TokenID::INTERSECTION: return SetCurrent(op1.B().Intersect(op2.B()));
+    case TokenID::SET_MINUS: return SetCurrent(op1.B().Diff(op2.B()));
+    case TokenID::SYMMINUS: return SetCurrent(op1.B().SymDiff(op2.B()));
+
+    case TokenID::IN: return SetCurrent(op2.B().Contains(op1));
+    case TokenID::NOTIN: return SetCurrent(!op2.B().Contains(op1));
+    case TokenID::SUBSET: return SetCurrent(!(op1 == op2) && op1.B().IsSubsetOrEq(op2.B()));
+    case TokenID::NOTSUBSET: return SetCurrent(op1 == op2 || !op1.B().IsSubsetOrEq(op2.B()));
+    case TokenID::SUBSET_OR_EQ: return SetCurrent(op1.B().IsSubsetOrEq(op2.B()));
   }
 }
 
 bool ASTInterpreter::ViProjectSet(Cursor iter) {
   const auto childValue = EvaluateChild(iter, 0);
   if (!childValue.has_value()) {
     return false;
   }
-  return VisitAndReturn(std::get<StructuredData>(childValue.value()).B().Projection(iter->data.ToTuple()));
+  return SetCurrent(std::get<StructuredData>(childValue.value()).B().Projection(iter->data.ToTuple()));
 }
 
 bool ASTInterpreter::ViProjectTuple(Cursor iter) {
   const auto childValue = EvaluateChild(iter, 0);
   if (!childValue.has_value()) {
     return false;
   }
   
   const auto& indicies = iter->data.ToTuple();
   std::vector<StructuredData> components{};
   components.reserve(size(indicies));
   for (const auto index : indicies) {
     components.emplace_back(std::get<StructuredData>(childValue.value()).T().Component(index));
   }
-  return VisitAndReturn(Factory::Tuple(components));
+  return SetCurrent(Factory::Tuple(components));
 }
 
 bool ASTInterpreter::ViFilter(Cursor iter) {
   const auto argumentValue = EvaluateChild(iter, static_cast<Index>(iter.ChildrenCount() - 1));
   if (!argumentValue.has_value()) {
     return false;
   }
   const auto& argument = std::get<StructuredData>(argumentValue.value());
   if (argument.B().IsEmpty()) {
-    return VisitAndReturn(Factory::EmptySet());
+    return SetCurrent(Factory::EmptySet());
   }
 
   const auto& indicies = iter->data.ToTuple();
   std::vector<StructuredData> params{};
   params.reserve(size(indicies));
   for (Index child = 0; child < iter.ChildrenCount() - 1; ++child) {
     const auto param = EvaluateChild(iter, child);
     if (!param.has_value()) {
       return false;
     } 
     if (const auto val = std::get<StructuredData>(param.value()); val.B().IsEmpty()) {
-      return VisitAndReturn(Factory::EmptySet());
+      return SetCurrent(Factory::EmptySet());
     } else {
       params.emplace_back(val);
     }
   }
 
   auto result = Factory::EmptySet();
   for (const auto& element : argument.B()) {
@@ -605,36 +605,36 @@
         break;
       }
     }
     if (validElement) {
       result.ModifyB().AddElement(element);
     }
   }
-  return VisitAndReturn(std::move(result));
+  return SetCurrent(std::move(result));
 }
 
 bool ASTInterpreter::ViReduce(Cursor iter) {
   const auto childValue = EvaluateChild(iter, 0);
   if (!childValue.has_value()) {
     return false;
   }
-  return VisitAndReturn(std::get<StructuredData>(childValue.value()).B().Reduce());
+  return SetCurrent(std::get<StructuredData>(childValue.value()).B().Reduce());
 }
 
 bool ASTInterpreter::ViDebool(Cursor iter) {
   const auto childValue = EvaluateChild(iter, 0);
   if (!childValue.has_value()) {
     return false;
   }
   const auto value = std::get<StructuredData>(childValue.value());
   if (value.B().Cardinality() != 1) {
     OnError(ValueEID::invalidDebool, iter->pos.start);
     return false;
   }
-  return VisitAndReturn(std::get<StructuredData>(childValue.value()).B().Debool());
+  return SetCurrent(std::get<StructuredData>(childValue.value()).B().Debool());
 }
 
 std::optional<ExpressionValue> ASTInterpreter::EvaluateChild(Cursor iter, const Index index) {
   assert(iter.ChildrenCount() > index);
 
   ExpressionValue result = curValue;
   iter.MoveToChild(index);
```

### Comparing `pyconcept-0.1.3/ccl/rslang/src/ASTNormalizer.cpp` & `pyconcept-0.1.4/ccl/rslang/src/ASTNormalizer.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/src/AsciiLexer.cpp` & `pyconcept-0.1.4/ccl/rslang/src/AsciiLexer.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/src/Auditor.cpp` & `pyconcept-0.1.4/ccl/rslang/src/Auditor.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/src/ErrorLogger.cpp` & `pyconcept-0.1.4/ccl/rslang/src/ErrorLogger.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/src/GeneratorImplAST.cpp` & `pyconcept-0.1.4/ccl/rslang/src/GeneratorImplAST.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 }
 
 bool GeneratorImplAST::VisitDefault(Cursor iter) {
   rsText += iter->ToString(syntax);
   return true;
 }
 
-bool GeneratorImplAST::ViGlobalDefinition(Cursor iter) {
+bool GeneratorImplAST::ViGlobalDeclaration(Cursor iter) {
   OutputChild(iter, 0);
   rsText += iter->ToString(syntax);
   if (iter.ChildrenCount() > 1) {
     OutputChild(iter, 1);
   }
   return true;
 }
@@ -44,20 +44,20 @@
     }
     OutputChild(iter, child);
   }
   rsText += ']';
   return true;
 }
 
-bool GeneratorImplAST::ViLocalBind(Cursor iter) {
+bool GeneratorImplAST::ViTupleDeclaration(Cursor iter) {
   EnumChildren(iter, '(', ')', std::string(R"(, )"));
   return true;
 }
 
-bool GeneratorImplAST::ViLocalEnum(Cursor iter) {
+bool GeneratorImplAST::ViEnumDeclaration(Cursor iter) {
   EnumChildren(iter, R"(, )");
   return true;
 }
 
 bool GeneratorImplAST::ViArgumentsEnum(Cursor iter) {
   EnumChildren(iter, '[', ']', R"(, )");
   return true;
@@ -233,15 +233,15 @@
 }
 
 bool GeneratorImplAST::ViTuple(Cursor iter) {
   EnumChildren(iter, '(', ')', R"(, )");
   return true;
 }
 
-bool GeneratorImplAST::ViSetEnum(Cursor iter) {
+bool GeneratorImplAST::ViEnumeration(Cursor iter) {
   EnumChildren(iter, '{', '}', R"(, )");
   return true;
 }
 
 void GeneratorImplAST::OutputChild(const Cursor& iter, const Index index, const bool addBrackets) {
   if (addBrackets) {
     rsText += '(';
```

### Comparing `pyconcept-0.1.3/ccl/rslang/src/Interpreter.cpp` & `pyconcept-0.1.4/ccl/rslang/src/Interpreter.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/src/Literals.cpp` & `pyconcept-0.1.4/ccl/rslang/src/Literals.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/src/MathLexer.cpp` & `pyconcept-0.1.4/ccl/rslang/src/MathLexer.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/src/NameCollector.cpp` & `pyconcept-0.1.4/ccl/rslang/src/NameCollector.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     const auto* childNode = iter.Child(child).get();
     args.insert(end(args), begin(parent.nodeVars[childNode]), end(parent.nodeVars[childNode]));
   }
   parent.nodeVars[iter.get()] = args;
   return true;
 }
 
-bool ASTInterpreter::NameCollector::ViGlobalDefinition(Cursor iter) {
+bool ASTInterpreter::NameCollector::ViGlobalDeclaration(Cursor iter) {
   if (iter->id == TokenID::PUNC_STRUCT) {
     return false; // TODO: specify error
   }
   switch (iter(0).id) {
   default:
   case TokenID::ID_FUNCTION:
   case TokenID::ID_PREDICATE: {
```

### Comparing `pyconcept-0.1.3/ccl/rslang/src/Parser.cpp` & `pyconcept-0.1.4/ccl/rslang/src/Parser.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-#pragma once
-
 #include "ccl/rslang/Parser.h"
 
 namespace ccl::rslang {
 
 Syntax Parser::EstimateSyntax(std::string_view expression) noexcept {
   using Syntax::UNDEF;
   using Syntax::MATH;
```

### Comparing `pyconcept-0.1.3/ccl/rslang/src/RSExpr.cpp` & `pyconcept-0.1.4/ccl/rslang/src/RSExpr.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/src/RSGenerator.cpp` & `pyconcept-0.1.4/ccl/rslang/src/RSGenerator.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/src/RSParser.cpp` & `pyconcept-0.1.4/ccl/rslang/src/RSParser.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/src/RSParserImpl.cpp` & `pyconcept-0.1.4/ccl/rslang/src/RSParserImpl.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-// A Bison parser, made by GNU Bison 3.7.4.
-
-// Skeleton implementation for Bison LALR(1) parsers in C++
-
-// Copyright (C) 2002-2015, 2018-2020 Free Software Foundation, Inc.
-
-// This program is free software: you can redistribute it and/or modify
-// it under the terms of the GNU General Public License as published by
-// the Free Software Foundation, either version 3 of the License, or
-// (at your option) any later version.
-
-// This program is distributed in the hope that it will be useful,
-// but WITHOUT ANY WARRANTY; without even the implied warranty of
-// MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-// GNU General Public License for more details.
-
-// You should have received a copy of the GNU General Public License
-// along with this program.  If not, see <http://www.gnu.org/licenses/>.
-
-// As a special exception, you may create a larger work that contains
-// part or all of the Bison parser skeleton and distribute that work
-// under terms of your choice, so long as that work isn't itself a
-// parser generator using the skeleton or a modified version thereof
-// as a parser skeleton.  Alternatively, if you modify or redistribute
-// the parser skeleton itself, you may (at your option) remove this
-// special exception, which will cause the skeleton and the resulting
-// Bison output files to be licensed under the GNU General Public
-// License without this special exception.
-
-// This special exception was added by the Free Software Foundation in
-// version 2.2 of Bison.
-
-// DO NOT RELY ON FEATURES THAT ARE NOT DOCUMENTED in the manual,
-// especially those whose name start with YY_ or yy_.  They are
-// private implementation details that can be changed or removed.
-
-// "%code top" blocks.
-#line 24 "RSParserImpl.y"
+// A Bison parser, made by GNU Bison 3.7.4.
+
+// Skeleton implementation for Bison LALR(1) parsers in C++
+
+// Copyright (C) 2002-2015, 2018-2020 Free Software Foundation, Inc.
+
+// This program is free software: you can redistribute it and/or modify
+// it under the terms of the GNU General Public License as published by
+// the Free Software Foundation, either version 3 of the License, or
+// (at your option) any later version.
+
+// This program is distributed in the hope that it will be useful,
+// but WITHOUT ANY WARRANTY; without even the implied warranty of
+// MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+// GNU General Public License for more details.
+
+// You should have received a copy of the GNU General Public License
+// along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
+// As a special exception, you may create a larger work that contains
+// part or all of the Bison parser skeleton and distribute that work
+// under terms of your choice, so long as that work isn't itself a
+// parser generator using the skeleton or a modified version thereof
+// as a parser skeleton.  Alternatively, if you modify or redistribute
+// the parser skeleton itself, you may (at your option) remove this
+// special exception, which will cause the skeleton and the resulting
+// Bison output files to be licensed under the GNU General Public
+// License without this special exception.
+
+// This special exception was added by the Free Software Foundation in
+// version 2.2 of Bison.
+
+// DO NOT RELY ON FEATURES THAT ARE NOT DOCUMENTED in the manual,
+// especially those whose name start with YY_ or yy_.  They are
+// private implementation details that can be changed or removed.
+
+// "%code top" blocks.
+#line 24 "RSParserImpl.y"
 
 #ifdef _MSC_VER
   #pragma warning( push )
   #pragma warning( disable : 4244 26434 26438 26440 26446 26447 26448 26456 )
   #pragma warning( disable : 26460 26477 26481 26482 26493 26494 26495 26496 )
 #endif
 
@@ -50,1656 +50,1672 @@
 #endif
 
 #if defined(__GNUC__) && !defined(__clang__)
   #pragma GCC diagnostic push
   #pragma GCC diagnostic ignored "-Wuseless-cast"
 #endif
 
-
-#line 59 "RSParserImpl.cpp"
-
-
-
-
-#include "RSParserImpl.h"
-
-
-
-
-#ifndef YY_
-# if defined YYENABLE_NLS && YYENABLE_NLS
-#  if ENABLE_NLS
-#   include <libintl.h> // FIXME: INFRINGES ON USER NAME SPACE.
-#   define YY_(msgid) dgettext ("bison-runtime", msgid)
-#  endif
-# endif
-# ifndef YY_
-#  define YY_(msgid) msgid
-# endif
-#endif
-
-
-// Whether we are compiled with exception support.
-#ifndef YY_EXCEPTIONS
-# if defined __GNUC__ && !defined __EXCEPTIONS
-#  define YY_EXCEPTIONS 0
-# else
-#  define YY_EXCEPTIONS 1
-# endif
-#endif
-
-
-
-// Enable debugging if requested.
-#if YYDEBUG
-
-// A pseudo ostream that takes yydebug_ into account.
-# define YYCDEBUG if (yydebug_) (*yycdebug_)
-
-# define YY_SYMBOL_PRINT(Title, Symbol)         \
-  do {                                          \
-    if (yydebug_)                               \
-    {                                           \
-      *yycdebug_ << Title << ' ';               \
-      yy_print_ (*yycdebug_, Symbol);           \
-      *yycdebug_ << '\n';                       \
-    }                                           \
-  } while (false)
-
-# define YY_REDUCE_PRINT(Rule)          \
-  do {                                  \
-    if (yydebug_)                       \
-      yy_reduce_print_ (Rule);          \
-  } while (false)
-
-# define YY_STACK_PRINT()               \
-  do {                                  \
-    if (yydebug_)                       \
-      yy_stack_print_ ();                \
-  } while (false)
-
-#else // !YYDEBUG
-
-# define YYCDEBUG if (false) std::cerr
-# define YY_SYMBOL_PRINT(Title, Symbol)  YYUSE (Symbol)
-# define YY_REDUCE_PRINT(Rule)           static_cast<void> (0)
-# define YY_STACK_PRINT()                static_cast<void> (0)
-
-#endif // !YYDEBUG
-
-#define yyerrok         (yyerrstatus_ = 0)
-#define yyclearin       (yyla.clear ())
-
-#define YYACCEPT        goto yyacceptlab
-#define YYABORT         goto yyabortlab
-#define YYERROR         goto yyerrorlab
-#define YYRECOVERING()  (!!yyerrstatus_)
-
-#line 15 "RSParserImpl.y"
-namespace ccl { namespace rslang { namespace detail {
-#line 140 "RSParserImpl.cpp"
-
-  /// Build a parser object.
-  RSParserImpl::RSParserImpl (ParserState* state_yyarg)
-#if YYDEBUG
-    : yydebug_ (false),
-      yycdebug_ (&std::cerr),
-#else
-    :
-#endif
-      state (state_yyarg)
-  {}
-
-  RSParserImpl::~RSParserImpl ()
-  {}
-
-  RSParserImpl::syntax_error::~syntax_error () YY_NOEXCEPT YY_NOTHROW
-  {}
-
-  /*---------------.
-  | symbol kinds.  |
-  `---------------*/
-
-  // basic_symbol.
-  template <typename Base>
-  RSParserImpl::basic_symbol<Base>::basic_symbol (const basic_symbol& that)
-    : Base (that)
-    , value (that.value)
-  {}
-
-
-  /// Constructor for valueless symbols.
-  template <typename Base>
-  RSParserImpl::basic_symbol<Base>::basic_symbol (typename Base::kind_type t)
-    : Base (t)
-    , value ()
-  {}
-
-  template <typename Base>
-  RSParserImpl::basic_symbol<Base>::basic_symbol (typename Base::kind_type t, YY_RVREF (semantic_type) v)
-    : Base (t)
-    , value (YY_MOVE (v))
-  {}
-
-  template <typename Base>
-  RSParserImpl::symbol_kind_type
-  RSParserImpl::basic_symbol<Base>::type_get () const YY_NOEXCEPT
-  {
-    return this->kind ();
-  }
-
-  template <typename Base>
-  bool
-  RSParserImpl::basic_symbol<Base>::empty () const YY_NOEXCEPT
-  {
-    return this->kind () == symbol_kind::S_YYEMPTY;
-  }
-
-  template <typename Base>
-  void
-  RSParserImpl::basic_symbol<Base>::move (basic_symbol& s)
-  {
-    super_type::move (s);
-    value = YY_MOVE (s.value);
-  }
-
-  // by_kind.
-  RSParserImpl::by_kind::by_kind ()
-    : kind_ (symbol_kind::S_YYEMPTY)
-  {}
-
-#if 201103L <= YY_CPLUSPLUS
-  RSParserImpl::by_kind::by_kind (by_kind&& that)
-    : kind_ (that.kind_)
-  {
-    that.clear ();
-  }
-#endif
-
-  RSParserImpl::by_kind::by_kind (const by_kind& that)
-    : kind_ (that.kind_)
-  {}
-
-  RSParserImpl::by_kind::by_kind (token_kind_type t)
-    : kind_ (yytranslate_ (t))
-  {}
-
-  void
-  RSParserImpl::by_kind::clear ()
-  {
-    kind_ = symbol_kind::S_YYEMPTY;
-  }
-
-  void
-  RSParserImpl::by_kind::move (by_kind& that)
-  {
-    kind_ = that.kind_;
-    that.clear ();
-  }
-
-  RSParserImpl::symbol_kind_type
-  RSParserImpl::by_kind::kind () const YY_NOEXCEPT
-  {
-    return kind_;
-  }
-
-  RSParserImpl::symbol_kind_type
-  RSParserImpl::by_kind::type_get () const YY_NOEXCEPT
-  {
-    return this->kind ();
-  }
-
-
-  // by_state.
-  RSParserImpl::by_state::by_state () YY_NOEXCEPT
-    : state (empty_state)
-  {}
-
-  RSParserImpl::by_state::by_state (const by_state& that) YY_NOEXCEPT
-    : state (that.state)
-  {}
-
-  void
-  RSParserImpl::by_state::clear () YY_NOEXCEPT
-  {
-    state = empty_state;
-  }
-
-  void
-  RSParserImpl::by_state::move (by_state& that)
-  {
-    state = that.state;
-    that.clear ();
-  }
-
-  RSParserImpl::by_state::by_state (state_type s) YY_NOEXCEPT
-    : state (s)
-  {}
-
-  RSParserImpl::symbol_kind_type
-  RSParserImpl::by_state::kind () const YY_NOEXCEPT
-  {
-    if (state == empty_state)
-      return symbol_kind::S_YYEMPTY;
-    else
-      return YY_CAST (symbol_kind_type, yystos_[+state]);
-  }
-
-  RSParserImpl::stack_symbol_type::stack_symbol_type ()
-  {}
-
-  RSParserImpl::stack_symbol_type::stack_symbol_type (YY_RVREF (stack_symbol_type) that)
-    : super_type (YY_MOVE (that.state), YY_MOVE (that.value))
-  {
-#if 201103L <= YY_CPLUSPLUS
-    // that is emptied.
-    that.state = empty_state;
-#endif
-  }
-
-  RSParserImpl::stack_symbol_type::stack_symbol_type (state_type s, YY_MOVE_REF (symbol_type) that)
-    : super_type (s, YY_MOVE (that.value))
-  {
-    // that is emptied.
-    that.kind_ = symbol_kind::S_YYEMPTY;
-  }
-
-#if YY_CPLUSPLUS < 201103L
-  RSParserImpl::stack_symbol_type&
-  RSParserImpl::stack_symbol_type::operator= (const stack_symbol_type& that)
-  {
-    state = that.state;
-    value = that.value;
-    return *this;
-  }
-
-  RSParserImpl::stack_symbol_type&
-  RSParserImpl::stack_symbol_type::operator= (stack_symbol_type& that)
-  {
-    state = that.state;
-    value = that.value;
-    // that is emptied.
-    that.state = empty_state;
-    return *this;
-  }
-#endif
-
-  template <typename Base>
-  void
-  RSParserImpl::yy_destroy_ (const char* yymsg, basic_symbol<Base>& yysym) const
-  {
-    if (yymsg)
-      YY_SYMBOL_PRINT (yymsg, yysym);
-
-    // User destructor.
-    YYUSE (yysym.kind ());
-  }
-
-#if YYDEBUG
-  template <typename Base>
-  void
-  RSParserImpl::yy_print_ (std::ostream& yyo, const basic_symbol<Base>& yysym) const
-  {
-    std::ostream& yyoutput = yyo;
-    YYUSE (yyoutput);
-    if (yysym.empty ())
-      yyo << "empty symbol";
-    else
-      {
-        symbol_kind_type yykind = yysym.kind ();
-        yyo << (yykind < YYNTOKENS ? "token" : "nterm")
-            << ' ' << yysym.name () << " (";
-        YYUSE (yykind);
-        yyo << ')';
-      }
-  }
-#endif
-
-  void
-  RSParserImpl::yypush_ (const char* m, YY_MOVE_REF (stack_symbol_type) sym)
-  {
-    if (m)
-      YY_SYMBOL_PRINT (m, sym);
-    yystack_.push (YY_MOVE (sym));
-  }
-
-  void
-  RSParserImpl::yypush_ (const char* m, state_type s, YY_MOVE_REF (symbol_type) sym)
-  {
-#if 201103L <= YY_CPLUSPLUS
-    yypush_ (m, stack_symbol_type (s, std::move (sym)));
-#else
-    stack_symbol_type ss (s, sym);
-    yypush_ (m, ss);
-#endif
-  }
-
-  void
-  RSParserImpl::yypop_ (int n)
-  {
-    yystack_.pop (n);
-  }
-
-#if YYDEBUG
-  std::ostream&
-  RSParserImpl::debug_stream () const
-  {
-    return *yycdebug_;
-  }
-
-  void
-  RSParserImpl::set_debug_stream (std::ostream& o)
-  {
-    yycdebug_ = &o;
-  }
-
-
-  RSParserImpl::debug_level_type
-  RSParserImpl::debug_level () const
-  {
-    return yydebug_;
-  }
-
-  void
-  RSParserImpl::set_debug_level (debug_level_type l)
-  {
-    yydebug_ = l;
-  }
-#endif // YYDEBUG
-
-  RSParserImpl::state_type
-  RSParserImpl::yy_lr_goto_state_ (state_type yystate, int yysym)
-  {
-    int yyr = yypgoto_[yysym - YYNTOKENS] + yystate;
-    if (0 <= yyr && yyr <= yylast_ && yycheck_[yyr] == yystate)
-      return yytable_[yyr];
-    else
-      return yydefgoto_[yysym - YYNTOKENS];
-  }
-
-  bool
-  RSParserImpl::yy_pact_value_is_default_ (int yyvalue)
-  {
-    return yyvalue == yypact_ninf_;
-  }
-
-  bool
-  RSParserImpl::yy_table_value_is_error_ (int yyvalue)
-  {
-    return yyvalue == yytable_ninf_;
-  }
-
-  int
-  RSParserImpl::operator() ()
-  {
-    return parse ();
-  }
-
-  int
-  RSParserImpl::parse ()
-  {
-    int yyn;
-    /// Length of the RHS of the rule being reduced.
-    int yylen = 0;
-
-    // Error handling.
-    int yynerrs_ = 0;
-    int yyerrstatus_ = 0;
-
-    /// The lookahead symbol.
-    symbol_type yyla;
-
-    /// The return value of parse ().
-    int yyresult;
-
-#if YY_EXCEPTIONS
-    try
-#endif // YY_EXCEPTIONS
-      {
-    YYCDEBUG << "Starting parse\n";
-
-
-    /* Initialize the stack.  The initial state will be set in
-       yynewstate, since the latter expects the semantical and the
-       location values to have been already stored, initialize these
-       stacks with a primary value.  */
-    yystack_.clear ();
-    yypush_ (YY_NULLPTR, 0, YY_MOVE (yyla));
-
-  /*-----------------------------------------------.
-  | yynewstate -- push a new symbol on the stack.  |
-  `-----------------------------------------------*/
-  yynewstate:
-    YYCDEBUG << "Entering state " << int (yystack_[0].state) << '\n';
-    YY_STACK_PRINT ();
-
-    // Accept?
-    if (yystack_[0].state == yyfinal_)
-      YYACCEPT;
-
-    goto yybackup;
-
-
-  /*-----------.
-  | yybackup.  |
-  `-----------*/
-  yybackup:
-    // Try to take a decision without lookahead.
-    yyn = yypact_[+yystack_[0].state];
-    if (yy_pact_value_is_default_ (yyn))
-      goto yydefault;
-
-    // Read a lookahead token.
-    if (yyla.empty ())
-      {
-        YYCDEBUG << "Reading a token\n";
-#if YY_EXCEPTIONS
-        try
-#endif // YY_EXCEPTIONS
-          {
-            yyla.kind_ = yytranslate_ (yylex (&yyla.value, state));
-          }
-#if YY_EXCEPTIONS
-        catch (const syntax_error& yyexc)
-          {
-            YYCDEBUG << "Caught exception: " << yyexc.what() << '\n';
-            error (yyexc);
-            goto yyerrlab1;
-          }
-#endif // YY_EXCEPTIONS
-      }
-    YY_SYMBOL_PRINT ("Next token is", yyla);
-
-    if (yyla.kind () == symbol_kind::S_YYerror)
-    {
-      // The scanner already issued an error message, process directly
-      // to error recovery.  But do not keep the error token as
-      // lookahead, it is too special and may lead us to an endless
-      // loop in error recovery. */
-      yyla.kind_ = symbol_kind::S_YYUNDEF;
-      goto yyerrlab1;
-    }
-
-    /* If the proper action on seeing token YYLA.TYPE is to reduce or
-       to detect an error, take that action.  */
-    yyn += yyla.kind ();
-    if (yyn < 0 || yylast_ < yyn || yycheck_[yyn] != yyla.kind ())
-      {
-        goto yydefault;
-      }
-
-    // Reduce or error.
-    yyn = yytable_[yyn];
-    if (yyn <= 0)
-      {
-        if (yy_table_value_is_error_ (yyn))
-          goto yyerrlab;
-        yyn = -yyn;
-        goto yyreduce;
-      }
-
-    // Count tokens shifted since error; after three, turn off error status.
-    if (yyerrstatus_)
-      --yyerrstatus_;
-
-    // Shift the lookahead token.
-    yypush_ ("Shifting", state_type (yyn), YY_MOVE (yyla));
-    goto yynewstate;
-
-
-  /*-----------------------------------------------------------.
-  | yydefault -- do the default action for the current state.  |
-  `-----------------------------------------------------------*/
-  yydefault:
-    yyn = yydefact_[+yystack_[0].state];
-    if (yyn == 0)
-      goto yyerrlab;
-    goto yyreduce;
-
-
-  /*-----------------------------.
-  | yyreduce -- do a reduction.  |
-  `-----------------------------*/
-  yyreduce:
-    yylen = yyr2_[yyn];
-    {
-      stack_symbol_type yylhs;
-      yylhs.state = yy_lr_goto_state_ (yystack_[yylen].state, yyr1_[yyn]);
-      /* If YYLEN is nonzero, implement the default value of the
-         action: '$$ = $1'.  Otherwise, use the top of the stack.
-
-         Otherwise, the following line sets YYLHS.VALUE to garbage.
-         This behavior is undocumented and Bison users should not rely
-         upon it.  */
-      if (yylen)
-        yylhs.value = yystack_[yylen - 1].value;
-      else
-        yylhs.value = yystack_[0].value;
-
-
-      // Perform the reduction.
-      YY_REDUCE_PRINT (yyn);
-#if YY_EXCEPTIONS
-      try
-#endif // YY_EXCEPTIONS
-        {
-          switch (yyn)
-            {
-  case 3: // expression: logic_or_setexpr
-#line 263 "RSParserImpl.y"
-                                            { state->FinalizeExpression(yystack_[0].value); }
-#line 591 "RSParserImpl.cpp"
-    break;
-
-  case 4: // expression: function_decl
-#line 264 "RSParserImpl.y"
-                                            { state->FinalizeExpression(yystack_[0].value); }
-#line 597 "RSParserImpl.cpp"
-    break;
-
-  case 5: // global_declaration: GLOBAL DEFINE
-#line 268 "RSParserImpl.y"
-                                            { state->FinalizeCstEmpty(yystack_[1].value, yystack_[0].value); }
-#line 603 "RSParserImpl.cpp"
-    break;
-
-  case 6: // global_declaration: GLOBAL STRUCT setexpr
-#line 269 "RSParserImpl.y"
-                                            { state->FinalizeCstExpression(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
-#line 609 "RSParserImpl.cpp"
-    break;
-
-  case 7: // global_declaration: GLOBAL DEFINE logic_or_setexpr
-#line 270 "RSParserImpl.y"
-                                            { state->FinalizeCstExpression(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
-#line 615 "RSParserImpl.cpp"
-    break;
-
-  case 8: // global_declaration: function_name DEFINE function_decl
-#line 271 "RSParserImpl.y"
-                                            { state->FinalizeCstExpression(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
-#line 621 "RSParserImpl.cpp"
-    break;
-
-  case 13: // function_decl: LS arguments RS logic_or_setexpr
-#line 284 "RSParserImpl.y"
-                                            { yylhs.value = FunctionDeclaration(yystack_[3].value, yystack_[2].value, yystack_[0].value); }
-#line 627 "RSParserImpl.cpp"
-    break;
-
-  case 14: // function_decl: LS error
-#line 285 "RSParserImpl.y"
-                                            { state->OnError(ParseEID::expectedDeclaration); YYABORT; }
-#line 633 "RSParserImpl.cpp"
-    break;
-
-  case 15: // arguments: declaration
-#line 290 "RSParserImpl.y"
-                                            { yylhs.value = AddNode(TokenID::NT_ARGUMENTS, yystack_[0].value); }
-#line 639 "RSParserImpl.cpp"
-    break;
-
-  case 16: // arguments: arguments COMMA declaration
-#line 291 "RSParserImpl.y"
-                                            { yylhs.value = Enumeration(TokenID::NT_ARGUMENTS, yystack_[2].value, yystack_[0].value); }
-#line 645 "RSParserImpl.cpp"
-    break;
-
-  case 17: // arguments: arguments COMMA error
-#line 292 "RSParserImpl.y"
-                                            { state->OnError(ParseEID::expectedLocal); YYABORT; }
-#line 651 "RSParserImpl.cpp"
-    break;
-
-  case 18: // declaration: LOCAL IN setexpr
-#line 295 "RSParserImpl.y"
-                                            { yylhs.value = AddNode(TokenID::NT_ARG_DECL, yystack_[2].value, yystack_[0].value); }
-#line 657 "RSParserImpl.cpp"
-    break;
-
-  case 19: // declaration: LOCAL error
-#line 296 "RSParserImpl.y"
-                                            { state->OnError(ParseEID::expectedDeclaration); YYABORT; }
-#line 663 "RSParserImpl.cpp"
-    break;
-
-  case 21: // variable: LP var_enum RPE
-#line 301 "RSParserImpl.y"
-                                            { yylhs.value = ReplaceBrackets(TokenID::NT_TUPLE_DECL, yystack_[2].value, yystack_[1].value, yystack_[0].value); }
-#line 669 "RSParserImpl.cpp"
-    break;
-
-  case 22: // var_enum: var_all COMMA var_all
-#line 304 "RSParserImpl.y"
-                                            { yylhs.value = Enumeration(TokenID::INTERRUPT, yystack_[2].value, yystack_[0].value); }
-#line 675 "RSParserImpl.cpp"
-    break;
-
-  case 23: // var_enum: var_all COMMA error
-#line 305 "RSParserImpl.y"
-                                            { state->OnError(ParseEID::expectedLocal); YYABORT; }
-#line 681 "RSParserImpl.cpp"
-    break;
-
-  case 31: // logic_par: LP logic_binary RPE
-#line 323 "RSParserImpl.y"
-                                            { yylhs.value = RemoveBrackets(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
-#line 687 "RSParserImpl.cpp"
-    break;
-
-  case 32: // logic_par: LP logic_predicates RPE
-#line 324 "RSParserImpl.y"
-                                            { yylhs.value = RemoveBrackets(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
-#line 693 "RSParserImpl.cpp"
-    break;
-
-  case 33: // logic_predicates: setexpr binary_predicate setexpr
-#line 328 "RSParserImpl.y"
-                                            { yylhs.value = BinaryOperation(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
-#line 699 "RSParserImpl.cpp"
-    break;
-
-  case 45: // logic_unary: NOT logic_no_binary
-#line 345 "RSParserImpl.y"
-                                            { yylhs.value = UnaryOperation(yystack_[1].value, yystack_[0].value);}
-#line 705 "RSParserImpl.cpp"
-    break;
-
-  case 46: // logic_unary: quantifier quant_var IN setexpr logic_no_binary
-#line 346 "RSParserImpl.y"
-                                                      { yylhs.value = Quantifier(yystack_[4].value, yystack_[3].value, yystack_[1].value, yystack_[0].value);}
-#line 711 "RSParserImpl.cpp"
-    break;
-
-  case 47: // logic_unary: quantifier error
-#line 347 "RSParserImpl.y"
-                                            { state->OnError(ParseEID::invalidQuantifier); YYABORT; }
-#line 717 "RSParserImpl.cpp"
-    break;
-
-  case 48: // logic_unary: PREDICATE LS setexpr_enum RS
-#line 348 "RSParserImpl.y"
-                                            { yylhs.value = FunctionCall(yystack_[3].value, yystack_[1].value, yystack_[0].value); }
-#line 723 "RSParserImpl.cpp"
-    break;
-
-  case 56: // quant_var: LP error
-#line 362 "RSParserImpl.y"
-                                            { state->OnError(ParseEID::invalidQuantifier); YYABORT; }
-#line 729 "RSParserImpl.cpp"
-    break;
-
-  case 57: // quant_var_enum: quant_var COMMA quant_var
-#line 365 "RSParserImpl.y"
-                                            { yylhs.value = Enumeration(TokenID::NT_ENUM_DECL, yystack_[2].value, yystack_[0].value); }
-#line 735 "RSParserImpl.cpp"
-    break;
-
-  case 58: // quant_var_enum: quant_var COMMA error
-#line 366 "RSParserImpl.y"
-                                            { state->OnError(ParseEID::expectedLocal); YYABORT; }
-#line 741 "RSParserImpl.cpp"
-    break;
-
-  case 59: // logic_binary: logic_all EQUIVALENT logic_all
-#line 370 "RSParserImpl.y"
-                                            { yylhs.value = BinaryOperation(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
-#line 747 "RSParserImpl.cpp"
-    break;
-
-  case 60: // logic_binary: logic_all IMPLICATION logic_all
-#line 371 "RSParserImpl.y"
-                                            { yylhs.value = BinaryOperation(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
-#line 753 "RSParserImpl.cpp"
-    break;
-
-  case 61: // logic_binary: logic_all OR logic_all
-#line 372 "RSParserImpl.y"
-                                            { yylhs.value = BinaryOperation(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
-#line 759 "RSParserImpl.cpp"
-    break;
-
-  case 62: // logic_binary: logic_all AND logic_all
-#line 373 "RSParserImpl.y"
-                                            { yylhs.value = BinaryOperation(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
-#line 765 "RSParserImpl.cpp"
-    break;
-
-  case 67: // setexpr: FUNCTION LS setexpr_enum RS
-#line 383 "RSParserImpl.y"
-                                            { yylhs.value = FunctionCall(yystack_[3].value, yystack_[1].value, yystack_[0].value); }
-#line 771 "RSParserImpl.cpp"
-    break;
-
-  case 68: // setexpr: operation_name LP setexpr RPE
-#line 384 "RSParserImpl.y"
-                                            { yylhs.value = TextOperator(yystack_[3].value, yystack_[1].value, yystack_[0].value); }
-#line 777 "RSParserImpl.cpp"
-    break;
-
-  case 75: // setexpr_enum: setexpr
-#line 395 "RSParserImpl.y"
-                                            { yylhs.value = AddNode(TokenID::INTERRUPT, yystack_[0].value); }
-#line 783 "RSParserImpl.cpp"
-    break;
-
-  case 77: // setexpr_enum_min2: setexpr_enum COMMA setexpr
-#line 399 "RSParserImpl.y"
-                                            { yylhs.value = Enumeration(TokenID::INTERRUPT, yystack_[2].value, yystack_[0].value); }
-#line 789 "RSParserImpl.cpp"
-    break;
-
-  case 85: // setexpr_binary: setexpr PLUS setexpr
-#line 416 "RSParserImpl.y"
-                                            { yylhs.value = BinaryOperation(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
-#line 795 "RSParserImpl.cpp"
-    break;
-
-  case 86: // setexpr_binary: setexpr MINUS setexpr
-#line 417 "RSParserImpl.y"
-                                            { yylhs.value = BinaryOperation(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
-#line 801 "RSParserImpl.cpp"
-    break;
-
-  case 87: // setexpr_binary: setexpr MULTIPLY setexpr
-#line 418 "RSParserImpl.y"
-                                            { yylhs.value = BinaryOperation(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
-#line 807 "RSParserImpl.cpp"
-    break;
-
-  case 88: // setexpr_binary: setexpr UNION setexpr
-#line 419 "RSParserImpl.y"
-                                            { yylhs.value = BinaryOperation(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
-#line 813 "RSParserImpl.cpp"
-    break;
-
-  case 89: // setexpr_binary: setexpr SET_MINUS setexpr
-#line 420 "RSParserImpl.y"
-                                            { yylhs.value = BinaryOperation(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
-#line 819 "RSParserImpl.cpp"
-    break;
-
-  case 90: // setexpr_binary: setexpr SYMMINUS setexpr
-#line 421 "RSParserImpl.y"
-                                            { yylhs.value = BinaryOperation(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
-#line 825 "RSParserImpl.cpp"
-    break;
-
-  case 91: // setexpr_binary: setexpr INTERSECTION setexpr
-#line 422 "RSParserImpl.y"
-                                            { yylhs.value = BinaryOperation(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
-#line 831 "RSParserImpl.cpp"
-    break;
-
-  case 92: // setexpr_binary: setexpr DECART setexpr
-#line 423 "RSParserImpl.y"
-                                            { yylhs.value = Decartian(yystack_[2].value, yystack_[1].value, yystack_[0].value);}
-#line 837 "RSParserImpl.cpp"
-    break;
-
-  case 93: // setexpr_binary: LP setexpr_binary RPE
-#line 424 "RSParserImpl.y"
-                                            { yylhs.value = RemoveBrackets(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
-#line 843 "RSParserImpl.cpp"
-    break;
-
-  case 101: // enumeration: LC setexpr_enum RC
-#line 437 "RSParserImpl.y"
-                                            { yylhs.value = ReplaceBrackets(TokenID::NT_ENUMERATION, yystack_[2].value, yystack_[1].value, yystack_[0].value); }
-#line 849 "RSParserImpl.cpp"
-    break;
-
-  case 102: // tuple: LP setexpr_enum_min2 RPE
-#line 440 "RSParserImpl.y"
-                                            { yylhs.value = ReplaceBrackets(TokenID::NT_TUPLE, yystack_[2].value, yystack_[1].value, yystack_[0].value); }
-#line 855 "RSParserImpl.cpp"
-    break;
-
-  case 103: // boolean: BOOLEAN LP setexpr RPE
-#line 443 "RSParserImpl.y"
-                                            { yylhs.value = TextOperator(yystack_[3].value, yystack_[1].value, yystack_[0].value); }
-#line 861 "RSParserImpl.cpp"
-    break;
-
-  case 104: // boolean: BOOLEAN boolean
-#line 444 "RSParserImpl.y"
-                                            { yylhs.value = UnaryOperation(yystack_[1].value, yystack_[0].value); }
-#line 867 "RSParserImpl.cpp"
-    break;
-
-  case 105: // filter_expression: FILTER LS setexpr_enum RS LP setexpr RPE
-#line 447 "RSParserImpl.y"
-                                               { yylhs.value = FilterCall(yystack_[6].value, yystack_[4].value, yystack_[1].value, yystack_[0].value); }
-#line 873 "RSParserImpl.cpp"
-    break;
-
-  case 106: // declarative: LC LOCAL IN setexpr BAR logic RCE
-#line 451 "RSParserImpl.y"
-                                            { yylhs.value = TermDeclaration(yystack_[6].value, yystack_[5].value, yystack_[3].value, yystack_[1].value, yystack_[0].value); }
-#line 879 "RSParserImpl.cpp"
-    break;
-
-  case 107: // declarative: DECLARATIVE LC variable IN setexpr BAR logic RCE
-#line 452 "RSParserImpl.y"
-                                                       { yylhs.value = TermDeclaration(yystack_[7].value, yystack_[5].value, yystack_[3].value, yystack_[1].value, yystack_[0].value); }
-#line 885 "RSParserImpl.cpp"
-    break;
-
-  case 108: // recursion: RECURSIVE LC variable ASSIGN setexpr BAR logic BAR setexpr RCE
-#line 455 "RSParserImpl.y"
-                                                                     { yylhs.value = FullRecursion(yystack_[9].value, yystack_[7].value, yystack_[5].value, yystack_[3].value, yystack_[1].value, yystack_[0].value); }
-#line 891 "RSParserImpl.cpp"
-    break;
-
-  case 109: // recursion: RECURSIVE LC variable ASSIGN setexpr BAR setexpr RCE
-#line 456 "RSParserImpl.y"
-                                                           { yylhs.value = ShortRecursion(yystack_[7].value, yystack_[5].value, yystack_[3].value, yystack_[1].value, yystack_[0].value); }
-#line 897 "RSParserImpl.cpp"
-    break;
-
-  case 110: // imperative: IMPERATIVE LC setexpr BAR imp_blocks RCE
-#line 459 "RSParserImpl.y"
-                                               { yylhs.value = Imperative(yystack_[5].value, yystack_[3].value, yystack_[1].value, yystack_[0].value); }
-#line 903 "RSParserImpl.cpp"
-    break;
-
-  case 111: // imp_blocks: imp_block
-#line 462 "RSParserImpl.y"
-                                            { yylhs.value = AddNode(TokenID::INTERRUPT, yystack_[0].value); }
-#line 909 "RSParserImpl.cpp"
-    break;
-
-  case 112: // imp_blocks: imp_blocks SEMICOLON imp_blocks
-#line 463 "RSParserImpl.y"
-                                            { yylhs.value = Enumeration(TokenID::INTERRUPT, yystack_[2].value, yystack_[0].value); }
-#line 915 "RSParserImpl.cpp"
-    break;
-
-  case 113: // imp_block: LOCAL ITERATE setexpr
-#line 466 "RSParserImpl.y"
-                                            { yylhs.value = AddNode(TokenID::NT_IMP_DECLARE, yystack_[2].value, yystack_[0].value); }
-#line 921 "RSParserImpl.cpp"
-    break;
-
-  case 114: // imp_block: LOCAL ASSIGN setexpr
-#line 467 "RSParserImpl.y"
-                                            { yylhs.value = AddNode(TokenID::NT_IMP_ASSIGN, yystack_[2].value, yystack_[0].value); }
-#line 927 "RSParserImpl.cpp"
-    break;
-
-  case 115: // imp_block: logic
-#line 468 "RSParserImpl.y"
-                                            { yylhs.value = AddNode(TokenID::NT_IMP_LOGIC, yystack_[0].value); }
-#line 933 "RSParserImpl.cpp"
-    break;
-
-  case 117: // RPE: error
-#line 475 "RSParserImpl.y"
-            { state->OnError(ParseEID::missingParenthesis); YYABORT; }
-#line 939 "RSParserImpl.cpp"
-    break;
-
-  case 119: // RCE: error
-#line 479 "RSParserImpl.y"
-            { state->OnError(ParseEID::missingCurlyBrace); YYABORT; }
-#line 945 "RSParserImpl.cpp"
-    break;
-
-
-#line 949 "RSParserImpl.cpp"
-
-            default:
-              break;
-            }
-        }
-#if YY_EXCEPTIONS
-      catch (const syntax_error& yyexc)
-        {
-          YYCDEBUG << "Caught exception: " << yyexc.what() << '\n';
-          error (yyexc);
-          YYERROR;
-        }
-#endif // YY_EXCEPTIONS
-      YY_SYMBOL_PRINT ("-> $$ =", yylhs);
-      yypop_ (yylen);
-      yylen = 0;
-
-      // Shift the result of the reduction.
-      yypush_ (YY_NULLPTR, YY_MOVE (yylhs));
-    }
-    goto yynewstate;
-
-
-  /*--------------------------------------.
-  | yyerrlab -- here on detecting error.  |
-  `--------------------------------------*/
-  yyerrlab:
-    // If not already recovering from an error, report this error.
-    if (!yyerrstatus_)
-      {
-        ++yynerrs_;
-        context yyctx (*this, yyla);
-        std::string msg = yysyntax_error_ (yyctx);
-        error (YY_MOVE (msg));
-      }
-
-
-    if (yyerrstatus_ == 3)
-      {
-        /* If just tried and failed to reuse lookahead token after an
-           error, discard it.  */
-
-        // Return failure if at end of input.
-        if (yyla.kind () == symbol_kind::S_YYEOF)
-          YYABORT;
-        else if (!yyla.empty ())
-          {
-            yy_destroy_ ("Error: discarding", yyla);
-            yyla.clear ();
-          }
-      }
-
-    // Else will try to reuse lookahead token after shifting the error token.
-    goto yyerrlab1;
-
-
-  /*---------------------------------------------------.
-  | yyerrorlab -- error raised explicitly by YYERROR.  |
-  `---------------------------------------------------*/
-  yyerrorlab:
-    /* Pacify compilers when the user code never invokes YYERROR and
-       the label yyerrorlab therefore never appears in user code.  */
-    if (false)
-      YYERROR;
-
-    /* Do not reclaim the symbols of the rule whose action triggered
-       this YYERROR.  */
-    yypop_ (yylen);
-    yylen = 0;
-    YY_STACK_PRINT ();
-    goto yyerrlab1;
-
-
-  /*-------------------------------------------------------------.
-  | yyerrlab1 -- common code for both syntax error and YYERROR.  |
-  `-------------------------------------------------------------*/
-  yyerrlab1:
-    yyerrstatus_ = 3;   // Each real token shifted decrements this.
-    // Pop stack until we find a state that shifts the error token.
-    for (;;)
-      {
-        yyn = yypact_[+yystack_[0].state];
-        if (!yy_pact_value_is_default_ (yyn))
-          {
-            yyn += symbol_kind::S_YYerror;
-            if (0 <= yyn && yyn <= yylast_
-                && yycheck_[yyn] == symbol_kind::S_YYerror)
-              {
-                yyn = yytable_[yyn];
-                if (0 < yyn)
-                  break;
-              }
-          }
-
-        // Pop the current state because it cannot handle the error token.
-        if (yystack_.size () == 1)
-          YYABORT;
-
-        yy_destroy_ ("Error: popping", yystack_[0]);
-        yypop_ ();
-        YY_STACK_PRINT ();
-      }
-    {
-      stack_symbol_type error_token;
-
-
-      // Shift the error token.
-      error_token.state = state_type (yyn);
-      yypush_ ("Shifting", YY_MOVE (error_token));
-    }
-    goto yynewstate;
-
-
-  /*-------------------------------------.
-  | yyacceptlab -- YYACCEPT comes here.  |
-  `-------------------------------------*/
-  yyacceptlab:
-    yyresult = 0;
-    goto yyreturn;
-
-
-  /*-----------------------------------.
-  | yyabortlab -- YYABORT comes here.  |
-  `-----------------------------------*/
-  yyabortlab:
-    yyresult = 1;
-    goto yyreturn;
-
-
-  /*-----------------------------------------------------.
-  | yyreturn -- parsing is finished, return the result.  |
-  `-----------------------------------------------------*/
-  yyreturn:
-    if (!yyla.empty ())
-      yy_destroy_ ("Cleanup: discarding lookahead", yyla);
-
-    /* Do not reclaim the symbols of the rule whose action triggered
-       this YYABORT or YYACCEPT.  */
-    yypop_ (yylen);
-    YY_STACK_PRINT ();
-    while (1 < yystack_.size ())
-      {
-        yy_destroy_ ("Cleanup: popping", yystack_[0]);
-        yypop_ ();
-      }
-
-    return yyresult;
-  }
-#if YY_EXCEPTIONS
-    catch (...)
-      {
-        YYCDEBUG << "Exception caught: cleaning lookahead and stack\n";
-        // Do not try to display the values of the reclaimed symbols,
-        // as their printers might throw an exception.
-        if (!yyla.empty ())
-          yy_destroy_ (YY_NULLPTR, yyla);
-
-        while (1 < yystack_.size ())
-          {
-            yy_destroy_ (YY_NULLPTR, yystack_[0]);
-            yypop_ ();
-          }
-        throw;
-      }
-#endif // YY_EXCEPTIONS
-  }
-
-  void
-  RSParserImpl::error (const syntax_error& yyexc)
-  {
-    error (yyexc.what ());
-  }
-
-  /* Return YYSTR after stripping away unnecessary quotes and
-     backslashes, so that it's suitable for yyerror.  The heuristic is
-     that double-quoting is unnecessary unless the string contains an
-     apostrophe, a comma, or backslash (other than backslash-backslash).
-     YYSTR is taken from yytname.  */
-  std::string
-  RSParserImpl::yytnamerr_ (const char *yystr)
-  {
-    if (*yystr == '"')
-      {
-        std::string yyr;
-        char const *yyp = yystr;
-
-        for (;;)
-          switch (*++yyp)
-            {
-            case '\'':
-            case ',':
-              goto do_not_strip_quotes;
-
-            case '\\':
-              if (*++yyp != '\\')
-                goto do_not_strip_quotes;
-              else
-                goto append;
-
-            append:
-            default:
-              yyr += *yyp;
-              break;
-
-            case '"':
-              return yyr;
-            }
-      do_not_strip_quotes: ;
-      }
-
-    return yystr;
-  }
-
-  std::string
-  RSParserImpl::symbol_name (symbol_kind_type yysymbol)
-  {
-    return yytnamerr_ (yytname_[yysymbol]);
-  }
-
-
-
-  // RSParserImpl::context.
-  RSParserImpl::context::context (const RSParserImpl& yyparser, const symbol_type& yyla)
-    : yyparser_ (yyparser)
-    , yyla_ (yyla)
-  {}
-
-  int
-  RSParserImpl::context::expected_tokens (symbol_kind_type yyarg[], int yyargn) const
-  {
-    // Actual number of expected tokens
-    int yycount = 0;
-
-    int yyn = yypact_[+yyparser_.yystack_[0].state];
-    if (!yy_pact_value_is_default_ (yyn))
-      {
-        /* Start YYX at -YYN if negative to avoid negative indexes in
-           YYCHECK.  In other words, skip the first -YYN actions for
-           this state because they are default actions.  */
-        int yyxbegin = yyn < 0 ? -yyn : 0;
-        // Stay within bounds of both yycheck and yytname.
-        int yychecklim = yylast_ - yyn + 1;
-        int yyxend = yychecklim < YYNTOKENS ? yychecklim : YYNTOKENS;
-        for (int yyx = yyxbegin; yyx < yyxend; ++yyx)
-          if (yycheck_[yyx + yyn] == yyx && yyx != symbol_kind::S_YYerror
-              && !yy_table_value_is_error_ (yytable_[yyx + yyn]))
-            {
-              if (!yyarg)
-                ++yycount;
-              else if (yycount == yyargn)
-                return 0;
-              else
-                yyarg[yycount++] = YY_CAST (symbol_kind_type, yyx);
-            }
-      }
-
-    if (yyarg && yycount == 0 && 0 < yyargn)
-      yyarg[0] = symbol_kind::S_YYEMPTY;
-    return yycount;
-  }
-
-
-
-  int
-  RSParserImpl::yy_syntax_error_arguments_ (const context& yyctx,
-                                                 symbol_kind_type yyarg[], int yyargn) const
-  {
-    /* There are many possibilities here to consider:
-       - If this state is a consistent state with a default action, then
-         the only way this function was invoked is if the default action
-         is an error action.  In that case, don't check for expected
-         tokens because there are none.
-       - The only way there can be no lookahead present (in yyla) is
-         if this state is a consistent state with a default action.
-         Thus, detecting the absence of a lookahead is sufficient to
-         determine that there is no unexpected or expected token to
-         report.  In that case, just report a simple "syntax error".
-       - Don't assume there isn't a lookahead just because this state is
-         a consistent state with a default action.  There might have
-         been a previous inconsistent state, consistent state with a
-         non-default action, or user semantic action that manipulated
-         yyla.  (However, yyla is currently not documented for users.)
-       - Of course, the expected token list depends on states to have
-         correct lookahead information, and it depends on the parser not
-         to perform extra reductions after fetching a lookahead from the
-         scanner and before detecting a syntax error.  Thus, state merging
-         (from LALR or IELR) and default reductions corrupt the expected
-         token list.  However, the list is correct for canonical LR with
-         one exception: it will still contain any token that will not be
-         accepted due to an error action in a later state.
-    */
-
-    if (!yyctx.lookahead ().empty ())
-      {
-        if (yyarg)
-          yyarg[0] = yyctx.token ();
-        int yyn = yyctx.expected_tokens (yyarg ? yyarg + 1 : yyarg, yyargn - 1);
-        return yyn + 1;
-      }
-    return 0;
-  }
-
-  // Generate an error message.
-  std::string
-  RSParserImpl::yysyntax_error_ (const context& yyctx) const
-  {
-    // Its maximum.
-    enum { YYARGS_MAX = 5 };
-    // Arguments of yyformat.
-    symbol_kind_type yyarg[YYARGS_MAX];
-    int yycount = yy_syntax_error_arguments_ (yyctx, yyarg, YYARGS_MAX);
-
-    char const* yyformat = YY_NULLPTR;
-    switch (yycount)
-      {
-#define YYCASE_(N, S)                         \
-        case N:                               \
-          yyformat = S;                       \
-        break
-      default: // Avoid compiler warnings.
-        YYCASE_ (0, YY_("syntax error"));
-        YYCASE_ (1, YY_("syntax error, unexpected %s"));
-        YYCASE_ (2, YY_("syntax error, unexpected %s, expecting %s"));
-        YYCASE_ (3, YY_("syntax error, unexpected %s, expecting %s or %s"));
-        YYCASE_ (4, YY_("syntax error, unexpected %s, expecting %s or %s or %s"));
-        YYCASE_ (5, YY_("syntax error, unexpected %s, expecting %s or %s or %s or %s"));
-#undef YYCASE_
-      }
-
-    std::string yyres;
-    // Argument number.
-    std::ptrdiff_t yyi = 0;
-    for (char const* yyp = yyformat; *yyp; ++yyp)
-      if (yyp[0] == '%' && yyp[1] == 's' && yyi < yycount)
-        {
-          yyres += symbol_name (yyarg[yyi++]);
-          ++yyp;
-        }
-      else
-        yyres += *yyp;
-    return yyres;
-  }
-
-
-  const signed char RSParserImpl::yypact_ninf_ = -58;
-
-  const signed char RSParserImpl::yytable_ninf_ = -116;
-
-  const short
-  RSParserImpl::yypact_[] =
-  {
-     236,   -58,   111,   -34,   -17,   -58,   -58,   -58,   -58,   -58,
-     -58,   342,    82,   -58,   -58,    25,   -58,   -58,   -58,   -58,
-      46,    56,    75,   342,   414,     9,    60,   -58,    85,   -58,
-     -58,   137,   224,   -58,   -58,   -58,    79,   -58,   553,   118,
-     -58,   -58,   -58,   -58,   -58,   -58,   -58,   -58,   -58,   -58,
-     -58,   342,   466,   466,   466,   -58,   -58,   -58,   -58,   -58,
-     -58,   553,   466,   -58,   466,    35,    35,   466,   -58,    70,
-     101,   553,   121,    17,   202,   157,   -58,   466,   175,    24,
-     -58,   -58,    10,    63,   -58,   -58,    97,   342,   342,   342,
-     342,   -58,   -58,   100,   -58,   -19,   -58,   466,   466,   466,
-     -58,   -58,   -58,   -58,   -58,   -58,   -58,   -58,   -58,   -58,
-     -58,   466,   466,   466,   466,   466,   466,   466,   -58,   175,
-     126,   203,   129,   206,    35,   163,   144,   489,   -58,   -58,
-     -58,   -58,   466,   -58,   -58,   466,   -58,   -58,   466,   342,
-      89,   -58,   120,   241,   176,   -58,   -58,   -58,    19,   146,
-     466,   148,   143,   143,   190,   -58,   -58,   -58,   -58,   -58,
-     175,   129,   -58,   -58,   -58,   207,   466,   466,   394,   175,
-     503,   175,   -58,   -58,   -58,   -58,   154,   290,   -58,   -58,
-     -58,   466,   516,   521,   123,     6,     8,   -58,   342,   -58,
-     -58,   -58,   -58,   129,   342,   342,   466,   466,   -58,   -58,
-     394,   -58,    33,   -58,    33,   169,    14,   175,   175,   -58,
-     -58,   -58,   466,   -58,    73,   -58
-  };
-
-  const signed char
-  RSParserImpl::yydefact_[] =
-  {
-       0,    84,    81,     9,    10,    83,    78,    80,    79,    52,
-      53,     0,     0,    72,    73,     0,    74,    69,    70,    71,
-       0,     0,     0,     0,     0,     0,     0,     2,    82,     3,
-       4,    29,     0,    30,    26,    27,     0,    28,    12,     0,
-      63,    64,    65,    66,    94,    95,    96,    97,    98,   100,
-      99,     5,     0,     0,     0,    81,    82,    51,    49,    50,
-      45,     0,     0,   104,     0,     0,     0,     0,    29,     0,
-       0,    75,     0,     0,     0,    84,    10,     0,    75,     0,
-      76,    14,     0,     0,    15,     1,     0,     0,     0,     0,
-       0,    47,    20,     0,    54,     0,    55,     0,     0,     0,
-      41,    42,    43,    44,    40,    39,    34,    35,    36,    37,
-      38,     0,     0,     0,     0,     0,     0,     0,     7,     6,
-       0,     0,     0,     0,     0,     0,     0,     0,   117,   116,
-      32,    31,     0,   102,    93,     0,   101,    19,     0,     0,
-       0,     8,    59,    60,    61,    62,    56,    24,     0,     0,
-       0,     0,    85,    86,    87,    92,    88,    91,    89,    90,
-      33,     0,    67,    48,   103,     0,     0,     0,     0,    77,
-       0,    18,    13,    17,    16,    21,     0,     0,    58,    57,
-      68,     0,     0,     0,    84,    29,     0,   111,     0,    23,
-      25,    22,    46,     0,     0,     0,     0,     0,   119,   118,
-       0,   110,     0,   105,     0,    29,     0,   114,   113,   112,
-     106,   107,     0,   109,     0,   108
-  };
-
-  const short
-  RSParserImpl::yypgoto_[] =
-  {
-     -58,   -58,   -58,   228,   -50,   178,   -58,   128,   -30,    93,
-      95,     4,   164,    -8,    -9,   -58,    -6,   107,   -58,   119,
-     -58,   249,     0,   -58,    94,    -4,   -58,   -58,    -2,   -58,
-     -58,   -58,   273,   -58,   -58,   -58,   -58,    86,   -58,   -57,
-     -13
-  };
-
-  const short
-  RSParserImpl::yydefgoto_[] =
-  {
-      -1,    26,    27,    56,    29,    30,    83,    84,   147,   148,
-     149,    68,    32,    33,    34,   116,    35,    60,    36,    95,
-      96,    37,    61,    39,    72,    80,    40,    41,    42,    43,
-      44,    45,    46,    47,    48,    49,    50,   186,   187,   130,
-     201
-  };
-
-  const short
-  RSParserImpl::yytable_[] =
-  {
-      38,   118,    58,    57,    31,    59,    94,  -115,   150,   198,
-      81,   137,    82,   131,    69,   198,   133,   134,   128,    73,
-     128,    74,    53,    71,    78,    97,    98,    99,   100,   101,
-     102,   103,   104,   105,   198,   125,   126,   138,    92,    54,
-     151,   106,   107,   108,   109,   110,   111,   112,   113,   114,
-     115,    38,   119,    78,    78,    31,   -29,   -29,   -29,   -29,
-      85,  -115,   122,   199,    78,   164,  -115,   127,   200,   199,
-     129,   128,   129,    73,   198,    74,   -76,    78,   -25,   136,
-      91,    64,    92,   132,    97,    98,    99,   124,   199,   172,
-     173,   175,    82,   -26,   -26,   -26,   -26,   152,   153,   154,
-      65,   146,   128,    92,   180,   111,   112,   113,   114,   115,
-      66,   155,   156,   157,   158,   159,   160,   161,    79,    12,
-     139,    94,   140,   129,   -28,   -28,   -28,   -28,   199,    67,
-     128,    93,   169,    86,    62,   170,   203,   -11,   171,    38,
-      97,    98,    99,    31,    88,    89,    90,   120,   121,   178,
-     177,    92,   124,    25,   129,   189,    99,    92,   123,    51,
-      52,   111,   112,   113,   114,   115,   182,   183,    58,    57,
-     117,    59,   185,   196,   197,   111,   112,   113,   114,   115,
-     132,   193,   129,   162,   135,   132,    97,    98,    99,   210,
-     166,   211,   202,   213,   167,   206,   207,   208,   204,   205,
-      93,   215,    90,   128,   185,   176,   124,   111,   112,   113,
-     114,   115,   214,   -65,   -65,   -65,   -65,   -65,   -65,   -65,
-     -65,   -65,   111,   112,   113,   114,   115,   212,    28,   -65,
-     -65,   -65,   -65,   -65,   -65,   -65,   -65,   -65,   -65,     1,
-       2,     3,     4,     5,     6,     7,     8,    87,    88,    89,
-      90,   142,   143,   144,   145,   129,     9,    10,    11,   181,
-     163,   -65,   132,   165,   141,   132,    89,    90,   174,   190,
-     179,   191,    70,    12,    13,    14,    15,    16,    17,    18,
-      19,    20,    21,    22,   192,    63,   209,     0,    23,     0,
-      24,     0,    25,     1,    55,     3,     4,     5,     6,     7,
-       8,    97,    98,    99,     0,     0,     0,     0,     0,     0,
-       9,    10,    11,     0,     0,     0,     0,     0,     0,     0,
-       0,     0,   111,   112,   113,   114,   115,    12,    13,    14,
-      15,    16,    17,    18,    19,    20,    21,    22,     0,     0,
-       0,     0,    23,     0,    24,     1,    55,     3,     4,     5,
-       6,     7,     8,     0,     0,     0,     0,     0,     0,     0,
-       0,     0,     9,    10,    11,     0,     0,     0,     0,     0,
-       0,     0,     0,     0,     0,     0,     0,     0,     0,    12,
-      13,    14,    15,    16,    17,    18,    19,    20,    21,    22,
-       0,     0,     0,     0,    23,     0,    24,   184,    55,     3,
-       4,     5,     6,     7,     8,     0,     0,     0,     0,     0,
-       0,     0,     0,     0,     9,    10,    11,    75,    55,     3,
-      76,     5,     6,     7,     8,     0,     0,     0,     0,     0,
-       0,    12,    13,    14,    15,    16,    17,    18,    19,    20,
-      21,    22,     0,     0,     0,     0,    23,     0,    24,     0,
-       0,    12,    13,    14,    15,    16,    17,    18,    19,    20,
-      21,    22,     0,     0,     0,     0,    77,     0,    24,     1,
-      55,     3,    76,     5,     6,     7,     8,     0,     0,     0,
-       0,     0,     0,     0,     0,     0,     0,     0,     0,     0,
-       0,     0,     0,     0,     0,     0,     0,     0,     0,     0,
-      97,    98,    99,    12,    13,    14,    15,    16,    17,    18,
-      19,    20,    21,    22,    97,    98,    99,     0,    77,     0,
-      24,   111,   112,   113,   114,   115,     0,    97,    98,    99,
-       0,     0,    97,    98,    99,   111,   112,   113,   114,   115,
-       0,     0,     0,     0,     0,     0,     0,   168,   111,   112,
-     113,   114,   115,   111,   112,   113,   114,   115,     0,     0,
-       0,   188,     0,     0,    97,    98,    99,   100,   101,   102,
-     103,   104,   105,     0,   194,     0,     0,     0,     0,   195,
-     106,   107,   108,   109,   110,   111,   112,   113,   114,   115
-  };
-
-  const short
-  RSParserImpl::yycheck_[] =
-  {
-       0,    51,    11,    11,     0,    11,    36,     1,    27,     1,
-       1,     1,     3,    70,    23,     1,    73,    74,     1,    23,
-       1,    23,    56,    23,    24,    11,    12,    13,    14,    15,
-      16,    17,    18,    19,     1,    65,    66,    27,     3,    56,
-      59,    27,    28,    29,    30,    31,    32,    33,    34,    35,
-      36,    51,    52,    53,    54,    51,    23,    24,    25,    26,
-       0,    55,    62,    55,    64,   122,    60,    67,    60,    55,
-      53,     1,    53,    77,     1,    77,    59,    77,    59,    55,
-       1,    56,     3,    59,    11,    12,    13,    52,    55,   139,
-       1,   148,     3,    23,    24,    25,    26,    97,    98,    99,
-      54,     1,     1,     3,   161,    32,    33,    34,    35,    36,
-      54,   111,   112,   113,   114,   115,   116,   117,    24,    37,
-      57,   151,    59,    53,    23,    24,    25,    26,    55,    54,
-       1,    52,   132,    48,    52,   135,   193,     0,   138,   139,
-      11,    12,    13,   139,    24,    25,    26,    53,    54,     1,
-     150,     3,    52,    56,    53,     1,    13,     3,    64,    48,
-      49,    32,    33,    34,    35,    36,   166,   167,   177,   177,
-      52,   177,   168,    50,    51,    32,    33,    34,    35,    36,
-      59,   181,    53,    57,    27,    59,    11,    12,    13,   202,
-      27,   204,   188,   206,    50,   195,   196,   197,   194,   195,
-      52,   214,    26,     1,   200,    59,    52,    32,    33,    34,
-      35,    36,   212,    11,    12,    13,    14,    15,    16,    17,
-      18,    19,    32,    33,    34,    35,    36,    58,     0,    27,
-      28,    29,    30,    31,    32,    33,    34,    35,    36,     3,
-       4,     5,     6,     7,     8,     9,    10,    23,    24,    25,
-      26,    87,    88,    89,    90,    53,    20,    21,    22,    52,
-      57,    59,    59,    57,    86,    59,    25,    26,   140,   176,
-     151,   176,    23,    37,    38,    39,    40,    41,    42,    43,
-      44,    45,    46,    47,   177,    12,   200,    -1,    52,    -1,
-      54,    -1,    56,     3,     4,     5,     6,     7,     8,     9,
-      10,    11,    12,    13,    -1,    -1,    -1,    -1,    -1,    -1,
-      20,    21,    22,    -1,    -1,    -1,    -1,    -1,    -1,    -1,
-      -1,    -1,    32,    33,    34,    35,    36,    37,    38,    39,
-      40,    41,    42,    43,    44,    45,    46,    47,    -1,    -1,
-      -1,    -1,    52,    -1,    54,     3,     4,     5,     6,     7,
-       8,     9,    10,    -1,    -1,    -1,    -1,    -1,    -1,    -1,
-      -1,    -1,    20,    21,    22,    -1,    -1,    -1,    -1,    -1,
-      -1,    -1,    -1,    -1,    -1,    -1,    -1,    -1,    -1,    37,
-      38,    39,    40,    41,    42,    43,    44,    45,    46,    47,
-      -1,    -1,    -1,    -1,    52,    -1,    54,     3,     4,     5,
-       6,     7,     8,     9,    10,    -1,    -1,    -1,    -1,    -1,
-      -1,    -1,    -1,    -1,    20,    21,    22,     3,     4,     5,
-       6,     7,     8,     9,    10,    -1,    -1,    -1,    -1,    -1,
-      -1,    37,    38,    39,    40,    41,    42,    43,    44,    45,
-      46,    47,    -1,    -1,    -1,    -1,    52,    -1,    54,    -1,
-      -1,    37,    38,    39,    40,    41,    42,    43,    44,    45,
-      46,    47,    -1,    -1,    -1,    -1,    52,    -1,    54,     3,
-       4,     5,     6,     7,     8,     9,    10,    -1,    -1,    -1,
-      -1,    -1,    -1,    -1,    -1,    -1,    -1,    -1,    -1,    -1,
-      -1,    -1,    -1,    -1,    -1,    -1,    -1,    -1,    -1,    -1,
-      11,    12,    13,    37,    38,    39,    40,    41,    42,    43,
-      44,    45,    46,    47,    11,    12,    13,    -1,    52,    -1,
-      54,    32,    33,    34,    35,    36,    -1,    11,    12,    13,
-      -1,    -1,    11,    12,    13,    32,    33,    34,    35,    36,
-      -1,    -1,    -1,    -1,    -1,    -1,    -1,    58,    32,    33,
-      34,    35,    36,    32,    33,    34,    35,    36,    -1,    -1,
-      -1,    58,    -1,    -1,    11,    12,    13,    14,    15,    16,
-      17,    18,    19,    -1,    58,    -1,    -1,    -1,    -1,    58,
-      27,    28,    29,    30,    31,    32,    33,    34,    35,    36
-  };
-
-  const signed char
-  RSParserImpl::yystos_[] =
-  {
-       0,     3,     4,     5,     6,     7,     8,     9,    10,    20,
-      21,    22,    37,    38,    39,    40,    41,    42,    43,    44,
-      45,    46,    47,    52,    54,    56,    62,    63,    64,    65,
-      66,    72,    73,    74,    75,    77,    79,    82,    83,    84,
-      87,    88,    89,    90,    91,    92,    93,    94,    95,    96,
-      97,    48,    49,    56,    56,     4,    64,    74,    75,    77,
-      78,    83,    52,    93,    56,    54,    54,    54,    72,    75,
-      82,    83,    85,    86,    89,     3,     6,    52,    83,    85,
-      86,     1,     3,    67,    68,     0,    48,    23,    24,    25,
-      26,     1,     3,    52,    69,    80,    81,    11,    12,    13,
-      14,    15,    16,    17,    18,    19,    27,    28,    29,    30,
-      31,    32,    33,    34,    35,    36,    76,    52,    65,    83,
-      85,    85,    83,    85,    52,    69,    69,    83,     1,    53,
-     100,   100,    59,   100,   100,    27,    55,     1,    27,    57,
-      59,    66,    73,    73,    73,    73,     1,    69,    70,    71,
-      27,    59,    83,    83,    83,    83,    83,    83,    83,    83,
-      83,    83,    57,    57,   100,    57,    27,    50,    58,    83,
-      83,    83,    65,     1,    68,   100,    59,    83,     1,    80,
-     100,    52,    83,    83,     3,    72,    98,    99,    58,     1,
-      70,    71,    78,    83,    58,    58,    50,    51,     1,    55,
-      60,   101,    72,   100,    72,    72,    83,    83,    83,    98,
-     101,   101,    58,   101,    83,   101
-  };
-
-  const signed char
-  RSParserImpl::yyr1_[] =
-  {
-       0,    61,    62,    62,    62,    63,    63,    63,    63,    64,
-      64,    65,    65,    66,    66,    67,    67,    67,    68,    68,
-      69,    69,    70,    70,    71,    71,    72,    72,    72,    73,
-      73,    74,    74,    75,    76,    76,    76,    76,    76,    76,
-      76,    76,    76,    76,    76,    77,    77,    77,    77,    78,
-      78,    78,    79,    79,    80,    80,    80,    81,    81,    82,
-      82,    82,    82,    83,    83,    83,    83,    83,    83,    84,
-      84,    84,    84,    84,    84,    85,    85,    86,    87,    87,
-      87,    88,    88,    88,    88,    89,    89,    89,    89,    89,
-      89,    89,    89,    89,    90,    90,    90,    90,    90,    90,
-      90,    91,    92,    93,    93,    94,    95,    95,    96,    96,
-      97,    98,    98,    99,    99,    99,   100,   100,   101,   101
-  };
-
-  const signed char
-  RSParserImpl::yyr2_[] =
-  {
-       0,     2,     1,     1,     1,     2,     3,     3,     3,     1,
-       1,     1,     1,     4,     2,     1,     3,     3,     3,     2,
-       1,     3,     3,     3,     1,     1,     1,     1,     1,     1,
-       1,     3,     3,     3,     1,     1,     1,     1,     1,     1,
-       1,     1,     1,     1,     1,     2,     5,     2,     4,     1,
-       1,     1,     1,     1,     1,     1,     2,     3,     3,     3,
-       3,     3,     3,     1,     1,     1,     1,     4,     4,     1,
-       1,     1,     1,     1,     1,     1,     1,     3,     1,     1,
-       1,     1,     1,     1,     1,     3,     3,     3,     3,     3,
-       3,     3,     3,     3,     1,     1,     1,     1,     1,     1,
-       1,     3,     3,     4,     2,     7,     7,     8,    10,     8,
-       6,     1,     3,     3,     3,     1,     1,     1,     1,     1
-  };
-
-
-#if YYDEBUG || 1
-  // YYTNAME[SYMBOL-NUM] -- String name of the symbol SYMBOL-NUM.
-  // First, the terminals, then, starting at \a YYNTOKENS, nonterminals.
-  const char*
-  const RSParserImpl::yytname_[] =
-  {
-  "\"end of file\"", "error", "\"invalid token\"", "LOCAL", "GLOBAL",
-  "FUNCTION", "PREDICATE", "RADICAL", "INTEGER", "INTSET", "EMPTYSET",
-  "PLUS", "MINUS", "MULTIPLY", "GREATER", "LESSER", "GREATER_OR_EQ",
-  "LESSER_OR_EQ", "EQUAL", "NOTEQUAL", "FORALL", "EXISTS", "NOT",
-  "EQUIVALENT", "IMPLICATION", "OR", "AND", "IN", "NOTIN", "SUBSET",
-  "SUBSET_OR_EQ", "NOTSUBSET", "DECART", "UNION", "INTERSECTION",
-  "SET_MINUS", "SYMMINUS", "BOOLEAN", "BIGPR", "SMALLPR", "FILTER", "CARD",
-  "BOOL", "DEBOOL", "RED", "DECLARATIVE", "RECURSIVE", "IMPERATIVE",
-  "DEFINE", "STRUCT", "ASSIGN", "ITERATE", "LP", "RP", "LC", "RC", "LS",
-  "RS", "BAR", "COMMA", "SEMICOLON", "$accept", "expression",
-  "global_declaration", "function_name", "logic_or_setexpr",
-  "function_decl", "arguments", "declaration", "variable", "var_enum",
-  "var_all", "logic", "logic_all", "logic_par", "logic_predicates",
-  "binary_predicate", "logic_unary", "logic_no_binary", "quantifier",
-  "quant_var", "quant_var_enum", "logic_binary", "setexpr",
-  "operation_name", "setexpr_enum", "setexpr_enum_min2", "literal",
-  "identifier", "setexpr_binary", "setexpr_generators", "enumeration",
-  "tuple", "boolean", "filter_expression", "declarative", "recursion",
-  "imperative", "imp_blocks", "imp_block", "RPE", "RCE", YY_NULLPTR
-  };
-#endif
-
-
-#if YYDEBUG
-  const short
-  RSParserImpl::yyrline_[] =
-  {
-       0,   262,   262,   263,   264,   268,   269,   270,   271,   274,
-     275,   279,   280,   284,   285,   290,   291,   292,   295,   296,
-     300,   301,   304,   305,   308,   309,   314,   315,   316,   319,
-     320,   323,   324,   328,   331,   332,   333,   334,   335,   336,
-     337,   338,   339,   340,   341,   345,   346,   347,   348,   351,
-     352,   353,   356,   357,   360,   361,   362,   365,   366,   370,
-     371,   372,   373,   379,   380,   381,   382,   383,   384,   387,
-     388,   389,   390,   391,   392,   395,   396,   399,   403,   404,
-     405,   409,   410,   411,   412,   416,   417,   418,   419,   420,
-     421,   422,   423,   424,   428,   429,   430,   431,   432,   433,
-     434,   437,   440,   443,   444,   447,   451,   452,   455,   456,
-     459,   462,   463,   466,   467,   468,   474,   475,   478,   479
-  };
-
-  void
-  RSParserImpl::yy_stack_print_ () const
-  {
-    *yycdebug_ << "Stack now";
-    for (stack_type::const_iterator
-           i = yystack_.begin (),
-           i_end = yystack_.end ();
-         i != i_end; ++i)
-      *yycdebug_ << ' ' << int (i->state);
-    *yycdebug_ << '\n';
-  }
-
-  void
-  RSParserImpl::yy_reduce_print_ (int yyrule) const
-  {
-    int yylno = yyrline_[yyrule];
-    int yynrhs = yyr2_[yyrule];
-    // Print the symbols being reduced, and their result.
-    *yycdebug_ << "Reducing stack by rule " << yyrule - 1
-               << " (line " << yylno << "):\n";
-    // The symbols being reduced.
-    for (int yyi = 0; yyi < yynrhs; yyi++)
-      YY_SYMBOL_PRINT ("   $" << yyi + 1 << " =",
-                       yystack_[(yynrhs) - (yyi + 1)]);
-  }
-#endif // YYDEBUG
-
-  RSParserImpl::symbol_kind_type
-  RSParserImpl::yytranslate_ (int t)
-  {
-    // YYTRANSLATE[TOKEN-NUM] -- Symbol number corresponding to
-    // TOKEN-NUM as returned by yylex.
-    static
-    const signed char
-    translate_table[] =
-    {
-       0,     2,     2,     2,     2,     2,     2,     2,     2,     2,
-       2,     2,     2,     2,     2,     2,     2,     2,     2,     2,
-       2,     2,     2,     2,     2,     2,     2,     2,     2,     2,
-       2,     2,     2,     2,     2,     2,     2,     2,     2,     2,
-       2,     2,     2,     2,     2,     2,     2,     2,     2,     2,
-       2,     2,     2,     2,     2,     2,     2,     2,     2,     2,
-       2,     2,     2,     2,     2,     2,     2,     2,     2,     2,
-       2,     2,     2,     2,     2,     2,     2,     2,     2,     2,
-       2,     2,     2,     2,     2,     2,     2,     2,     2,     2,
-       2,     2,     2,     2,     2,     2,     2,     2,     2,     2,
-       2,     2,     2,     2,     2,     2,     2,     2,     2,     2,
-       2,     2,     2,     2,     2,     2,     2,     2,     2,     2,
-       2,     2,     2,     2,     2,     2,     2,     2,     2,     2,
-       2,     2,     2,     2,     2,     2,     2,     2,     2,     2,
-       2,     2,     2,     2,     2,     2,     2,     2,     2,     2,
-       2,     2,     2,     2,     2,     2,     2,     2,     2,     2,
-       2,     2,     2,     2,     2,     2,     2,     2,     2,     2,
-       2,     2,     2,     2,     2,     2,     2,     2,     2,     2,
-       2,     2,     2,     2,     2,     2,     2,     2,     2,     2,
-       2,     2,     2,     2,     2,     2,     2,     2,     2,     2,
-       2,     2,     2,     2,     2,     2,     2,     2,     2,     2,
-       2,     2,     2,     2,     2,     2,     2,     2,     2,     2,
-       2,     2,     2,     2,     2,     2,     2,     2,     2,     2,
-       2,     2,     2,     2,     2,     2,     2,     2,     2,     2,
-       2,     2,     2,     2,     2,     2,     2,     2,     2,     2,
-       2,     2,     2,     2,     2,     2,     1,     2,     3,     4,
-       5,     6,     7,     8,     9,    10,    11,    12,    13,    14,
-      15,    16,    17,    18,    19,    20,    21,    22,    23,    24,
-      25,    26,    27,    28,    29,    30,    31,    32,    33,    34,
-      35,    36,    37,    38,    39,    40,    41,    42,    43,    44,
-      45,    46,    47,    48,    49,    50,    51,    52,    53,    54,
-      55,    56,    57,    58,    59,    60
-    };
-    // Last valid token kind.
-    const int code_max = 315;
-
-    if (t <= 0)
-      return symbol_kind::S_YYEOF;
-    else if (t <= code_max)
-      return YY_CAST (symbol_kind_type, translate_table[t]);
-    else
-      return symbol_kind::S_YYUNDEF;
-  }
-
-#line 15 "RSParserImpl.y"
-} } } // ccl::rslang::detail
-#line 1691 "RSParserImpl.cpp"
-
-#line 486 "RSParserImpl.y"
+
+#line 59 "RSParserImpl.cpp"
+
+
+
+
+#include "RSParserImpl.h"
+
+
+
+
+#ifndef YY_
+# if defined YYENABLE_NLS && YYENABLE_NLS
+#  if ENABLE_NLS
+#   include <libintl.h> // FIXME: INFRINGES ON USER NAME SPACE.
+#   define YY_(msgid) dgettext ("bison-runtime", msgid)
+#  endif
+# endif
+# ifndef YY_
+#  define YY_(msgid) msgid
+# endif
+#endif
+
+
+// Whether we are compiled with exception support.
+#ifndef YY_EXCEPTIONS
+# if defined __GNUC__ && !defined __EXCEPTIONS
+#  define YY_EXCEPTIONS 0
+# else
+#  define YY_EXCEPTIONS 1
+# endif
+#endif
+
+
+
+// Enable debugging if requested.
+#if YYDEBUG
+
+// A pseudo ostream that takes yydebug_ into account.
+# define YYCDEBUG if (yydebug_) (*yycdebug_)
+
+# define YY_SYMBOL_PRINT(Title, Symbol)         \
+  do {                                          \
+    if (yydebug_)                               \
+    {                                           \
+      *yycdebug_ << Title << ' ';               \
+      yy_print_ (*yycdebug_, Symbol);           \
+      *yycdebug_ << '\n';                       \
+    }                                           \
+  } while (false)
+
+# define YY_REDUCE_PRINT(Rule)          \
+  do {                                  \
+    if (yydebug_)                       \
+      yy_reduce_print_ (Rule);          \
+  } while (false)
+
+# define YY_STACK_PRINT()               \
+  do {                                  \
+    if (yydebug_)                       \
+      yy_stack_print_ ();                \
+  } while (false)
+
+#else // !YYDEBUG
+
+# define YYCDEBUG if (false) std::cerr
+# define YY_SYMBOL_PRINT(Title, Symbol)  YYUSE (Symbol)
+# define YY_REDUCE_PRINT(Rule)           static_cast<void> (0)
+# define YY_STACK_PRINT()                static_cast<void> (0)
+
+#endif // !YYDEBUG
+
+#define yyerrok         (yyerrstatus_ = 0)
+#define yyclearin       (yyla.clear ())
+
+#define YYACCEPT        goto yyacceptlab
+#define YYABORT         goto yyabortlab
+#define YYERROR         goto yyerrorlab
+#define YYRECOVERING()  (!!yyerrstatus_)
+
+#line 15 "RSParserImpl.y"
+namespace ccl { namespace rslang { namespace detail {
+#line 140 "RSParserImpl.cpp"
+
+  /// Build a parser object.
+  RSParserImpl::RSParserImpl (ParserState* state_yyarg)
+#if YYDEBUG
+    : yydebug_ (false),
+      yycdebug_ (&std::cerr),
+#else
+    :
+#endif
+      state (state_yyarg)
+  {}
+
+  RSParserImpl::~RSParserImpl ()
+  {}
+
+  RSParserImpl::syntax_error::~syntax_error () YY_NOEXCEPT YY_NOTHROW
+  {}
+
+  /*---------------.
+  | symbol kinds.  |
+  `---------------*/
+
+  // basic_symbol.
+  template <typename Base>
+  RSParserImpl::basic_symbol<Base>::basic_symbol (const basic_symbol& that)
+    : Base (that)
+    , value (that.value)
+  {}
+
+
+  /// Constructor for valueless symbols.
+  template <typename Base>
+  RSParserImpl::basic_symbol<Base>::basic_symbol (typename Base::kind_type t)
+    : Base (t)
+    , value ()
+  {}
+
+  template <typename Base>
+  RSParserImpl::basic_symbol<Base>::basic_symbol (typename Base::kind_type t, YY_RVREF (semantic_type) v)
+    : Base (t)
+    , value (YY_MOVE (v))
+  {}
+
+  template <typename Base>
+  RSParserImpl::symbol_kind_type
+  RSParserImpl::basic_symbol<Base>::type_get () const YY_NOEXCEPT
+  {
+    return this->kind ();
+  }
+
+  template <typename Base>
+  bool
+  RSParserImpl::basic_symbol<Base>::empty () const YY_NOEXCEPT
+  {
+    return this->kind () == symbol_kind::S_YYEMPTY;
+  }
+
+  template <typename Base>
+  void
+  RSParserImpl::basic_symbol<Base>::move (basic_symbol& s)
+  {
+    super_type::move (s);
+    value = YY_MOVE (s.value);
+  }
+
+  // by_kind.
+  RSParserImpl::by_kind::by_kind ()
+    : kind_ (symbol_kind::S_YYEMPTY)
+  {}
+
+#if 201103L <= YY_CPLUSPLUS
+  RSParserImpl::by_kind::by_kind (by_kind&& that)
+    : kind_ (that.kind_)
+  {
+    that.clear ();
+  }
+#endif
+
+  RSParserImpl::by_kind::by_kind (const by_kind& that)
+    : kind_ (that.kind_)
+  {}
+
+  RSParserImpl::by_kind::by_kind (token_kind_type t)
+    : kind_ (yytranslate_ (t))
+  {}
+
+  void
+  RSParserImpl::by_kind::clear ()
+  {
+    kind_ = symbol_kind::S_YYEMPTY;
+  }
+
+  void
+  RSParserImpl::by_kind::move (by_kind& that)
+  {
+    kind_ = that.kind_;
+    that.clear ();
+  }
+
+  RSParserImpl::symbol_kind_type
+  RSParserImpl::by_kind::kind () const YY_NOEXCEPT
+  {
+    return kind_;
+  }
+
+  RSParserImpl::symbol_kind_type
+  RSParserImpl::by_kind::type_get () const YY_NOEXCEPT
+  {
+    return this->kind ();
+  }
+
+
+  // by_state.
+  RSParserImpl::by_state::by_state () YY_NOEXCEPT
+    : state (empty_state)
+  {}
+
+  RSParserImpl::by_state::by_state (const by_state& that) YY_NOEXCEPT
+    : state (that.state)
+  {}
+
+  void
+  RSParserImpl::by_state::clear () YY_NOEXCEPT
+  {
+    state = empty_state;
+  }
+
+  void
+  RSParserImpl::by_state::move (by_state& that)
+  {
+    state = that.state;
+    that.clear ();
+  }
+
+  RSParserImpl::by_state::by_state (state_type s) YY_NOEXCEPT
+    : state (s)
+  {}
+
+  RSParserImpl::symbol_kind_type
+  RSParserImpl::by_state::kind () const YY_NOEXCEPT
+  {
+    if (state == empty_state)
+      return symbol_kind::S_YYEMPTY;
+    else
+      return YY_CAST (symbol_kind_type, yystos_[+state]);
+  }
+
+  RSParserImpl::stack_symbol_type::stack_symbol_type ()
+  {}
+
+  RSParserImpl::stack_symbol_type::stack_symbol_type (YY_RVREF (stack_symbol_type) that)
+    : super_type (YY_MOVE (that.state), YY_MOVE (that.value))
+  {
+#if 201103L <= YY_CPLUSPLUS
+    // that is emptied.
+    that.state = empty_state;
+#endif
+  }
+
+  RSParserImpl::stack_symbol_type::stack_symbol_type (state_type s, YY_MOVE_REF (symbol_type) that)
+    : super_type (s, YY_MOVE (that.value))
+  {
+    // that is emptied.
+    that.kind_ = symbol_kind::S_YYEMPTY;
+  }
+
+#if YY_CPLUSPLUS < 201103L
+  RSParserImpl::stack_symbol_type&
+  RSParserImpl::stack_symbol_type::operator= (const stack_symbol_type& that)
+  {
+    state = that.state;
+    value = that.value;
+    return *this;
+  }
+
+  RSParserImpl::stack_symbol_type&
+  RSParserImpl::stack_symbol_type::operator= (stack_symbol_type& that)
+  {
+    state = that.state;
+    value = that.value;
+    // that is emptied.
+    that.state = empty_state;
+    return *this;
+  }
+#endif
+
+  template <typename Base>
+  void
+  RSParserImpl::yy_destroy_ (const char* yymsg, basic_symbol<Base>& yysym) const
+  {
+    if (yymsg)
+      YY_SYMBOL_PRINT (yymsg, yysym);
+
+    // User destructor.
+    YYUSE (yysym.kind ());
+  }
+
+#if YYDEBUG
+  template <typename Base>
+  void
+  RSParserImpl::yy_print_ (std::ostream& yyo, const basic_symbol<Base>& yysym) const
+  {
+    std::ostream& yyoutput = yyo;
+    YYUSE (yyoutput);
+    if (yysym.empty ())
+      yyo << "empty symbol";
+    else
+      {
+        symbol_kind_type yykind = yysym.kind ();
+        yyo << (yykind < YYNTOKENS ? "token" : "nterm")
+            << ' ' << yysym.name () << " (";
+        YYUSE (yykind);
+        yyo << ')';
+      }
+  }
+#endif
+
+  void
+  RSParserImpl::yypush_ (const char* m, YY_MOVE_REF (stack_symbol_type) sym)
+  {
+    if (m)
+      YY_SYMBOL_PRINT (m, sym);
+    yystack_.push (YY_MOVE (sym));
+  }
+
+  void
+  RSParserImpl::yypush_ (const char* m, state_type s, YY_MOVE_REF (symbol_type) sym)
+  {
+#if 201103L <= YY_CPLUSPLUS
+    yypush_ (m, stack_symbol_type (s, std::move (sym)));
+#else
+    stack_symbol_type ss (s, sym);
+    yypush_ (m, ss);
+#endif
+  }
+
+  void
+  RSParserImpl::yypop_ (int n)
+  {
+    yystack_.pop (n);
+  }
+
+#if YYDEBUG
+  std::ostream&
+  RSParserImpl::debug_stream () const
+  {
+    return *yycdebug_;
+  }
+
+  void
+  RSParserImpl::set_debug_stream (std::ostream& o)
+  {
+    yycdebug_ = &o;
+  }
+
+
+  RSParserImpl::debug_level_type
+  RSParserImpl::debug_level () const
+  {
+    return yydebug_;
+  }
+
+  void
+  RSParserImpl::set_debug_level (debug_level_type l)
+  {
+    yydebug_ = l;
+  }
+#endif // YYDEBUG
+
+  RSParserImpl::state_type
+  RSParserImpl::yy_lr_goto_state_ (state_type yystate, int yysym)
+  {
+    int yyr = yypgoto_[yysym - YYNTOKENS] + yystate;
+    if (0 <= yyr && yyr <= yylast_ && yycheck_[yyr] == yystate)
+      return yytable_[yyr];
+    else
+      return yydefgoto_[yysym - YYNTOKENS];
+  }
+
+  bool
+  RSParserImpl::yy_pact_value_is_default_ (int yyvalue)
+  {
+    return yyvalue == yypact_ninf_;
+  }
+
+  bool
+  RSParserImpl::yy_table_value_is_error_ (int yyvalue)
+  {
+    return yyvalue == yytable_ninf_;
+  }
+
+  int
+  RSParserImpl::operator() ()
+  {
+    return parse ();
+  }
+
+  int
+  RSParserImpl::parse ()
+  {
+    int yyn;
+    /// Length of the RHS of the rule being reduced.
+    int yylen = 0;
+
+    // Error handling.
+    int yynerrs_ = 0;
+    int yyerrstatus_ = 0;
+
+    /// The lookahead symbol.
+    symbol_type yyla;
+
+    /// The return value of parse ().
+    int yyresult;
+
+#if YY_EXCEPTIONS
+    try
+#endif // YY_EXCEPTIONS
+      {
+    YYCDEBUG << "Starting parse\n";
+
+
+    /* Initialize the stack.  The initial state will be set in
+       yynewstate, since the latter expects the semantical and the
+       location values to have been already stored, initialize these
+       stacks with a primary value.  */
+    yystack_.clear ();
+    yypush_ (YY_NULLPTR, 0, YY_MOVE (yyla));
+
+  /*-----------------------------------------------.
+  | yynewstate -- push a new symbol on the stack.  |
+  `-----------------------------------------------*/
+  yynewstate:
+    YYCDEBUG << "Entering state " << int (yystack_[0].state) << '\n';
+    YY_STACK_PRINT ();
+
+    // Accept?
+    if (yystack_[0].state == yyfinal_)
+      YYACCEPT;
+
+    goto yybackup;
+
+
+  /*-----------.
+  | yybackup.  |
+  `-----------*/
+  yybackup:
+    // Try to take a decision without lookahead.
+    yyn = yypact_[+yystack_[0].state];
+    if (yy_pact_value_is_default_ (yyn))
+      goto yydefault;
+
+    // Read a lookahead token.
+    if (yyla.empty ())
+      {
+        YYCDEBUG << "Reading a token\n";
+#if YY_EXCEPTIONS
+        try
+#endif // YY_EXCEPTIONS
+          {
+            yyla.kind_ = yytranslate_ (yylex (&yyla.value, state));
+          }
+#if YY_EXCEPTIONS
+        catch (const syntax_error& yyexc)
+          {
+            YYCDEBUG << "Caught exception: " << yyexc.what() << '\n';
+            error (yyexc);
+            goto yyerrlab1;
+          }
+#endif // YY_EXCEPTIONS
+      }
+    YY_SYMBOL_PRINT ("Next token is", yyla);
+
+    if (yyla.kind () == symbol_kind::S_YYerror)
+    {
+      // The scanner already issued an error message, process directly
+      // to error recovery.  But do not keep the error token as
+      // lookahead, it is too special and may lead us to an endless
+      // loop in error recovery. */
+      yyla.kind_ = symbol_kind::S_YYUNDEF;
+      goto yyerrlab1;
+    }
+
+    /* If the proper action on seeing token YYLA.TYPE is to reduce or
+       to detect an error, take that action.  */
+    yyn += yyla.kind ();
+    if (yyn < 0 || yylast_ < yyn || yycheck_[yyn] != yyla.kind ())
+      {
+        goto yydefault;
+      }
+
+    // Reduce or error.
+    yyn = yytable_[yyn];
+    if (yyn <= 0)
+      {
+        if (yy_table_value_is_error_ (yyn))
+          goto yyerrlab;
+        yyn = -yyn;
+        goto yyreduce;
+      }
+
+    // Count tokens shifted since error; after three, turn off error status.
+    if (yyerrstatus_)
+      --yyerrstatus_;
+
+    // Shift the lookahead token.
+    yypush_ ("Shifting", state_type (yyn), YY_MOVE (yyla));
+    goto yynewstate;
+
+
+  /*-----------------------------------------------------------.
+  | yydefault -- do the default action for the current state.  |
+  `-----------------------------------------------------------*/
+  yydefault:
+    yyn = yydefact_[+yystack_[0].state];
+    if (yyn == 0)
+      goto yyerrlab;
+    goto yyreduce;
+
+
+  /*-----------------------------.
+  | yyreduce -- do a reduction.  |
+  `-----------------------------*/
+  yyreduce:
+    yylen = yyr2_[yyn];
+    {
+      stack_symbol_type yylhs;
+      yylhs.state = yy_lr_goto_state_ (yystack_[yylen].state, yyr1_[yyn]);
+      /* If YYLEN is nonzero, implement the default value of the
+         action: '$$ = $1'.  Otherwise, use the top of the stack.
+
+         Otherwise, the following line sets YYLHS.VALUE to garbage.
+         This behavior is undocumented and Bison users should not rely
+         upon it.  */
+      if (yylen)
+        yylhs.value = yystack_[yylen - 1].value;
+      else
+        yylhs.value = yystack_[0].value;
+
+
+      // Perform the reduction.
+      YY_REDUCE_PRINT (yyn);
+#if YY_EXCEPTIONS
+      try
+#endif // YY_EXCEPTIONS
+        {
+          switch (yyn)
+            {
+  case 3: // expression: logic_or_setexpr
+#line 263 "RSParserImpl.y"
+                                            { state->FinalizeExpression(yystack_[0].value); }
+#line 591 "RSParserImpl.cpp"
+    break;
+
+  case 4: // expression: function_definition
+#line 264 "RSParserImpl.y"
+                                            { state->FinalizeExpression(yystack_[0].value); }
+#line 597 "RSParserImpl.cpp"
+    break;
+
+  case 5: // global_declaration: GLOBAL DEFINE
+#line 268 "RSParserImpl.y"
+                                            { state->FinalizeCstEmpty(yystack_[1].value, yystack_[0].value); }
+#line 603 "RSParserImpl.cpp"
+    break;
+
+  case 6: // global_declaration: GLOBAL STRUCT setexpr
+#line 269 "RSParserImpl.y"
+                                            { state->FinalizeCstExpression(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
+#line 609 "RSParserImpl.cpp"
+    break;
+
+  case 7: // global_declaration: GLOBAL DEFINE logic_or_setexpr
+#line 270 "RSParserImpl.y"
+                                            { state->FinalizeCstExpression(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
+#line 615 "RSParserImpl.cpp"
+    break;
+
+  case 8: // global_declaration: FUNCTION DEFINE function_definition
+#line 271 "RSParserImpl.y"
+                                            { state->FinalizeCstExpression(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
+#line 621 "RSParserImpl.cpp"
+    break;
+
+  case 9: // global_declaration: PREDICATE DEFINE function_definition
+#line 272 "RSParserImpl.y"
+                                                { state->FinalizeCstExpression(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
+#line 627 "RSParserImpl.cpp"
+    break;
+
+  case 12: // function_definition: LS arguments RS logic_or_setexpr
+#line 281 "RSParserImpl.y"
+                                            { yylhs.value = FunctionDeclaration(yystack_[3].value, yystack_[2].value, yystack_[0].value); }
+#line 633 "RSParserImpl.cpp"
+    break;
+
+  case 13: // function_definition: LS error
+#line 282 "RSParserImpl.y"
+                                            { state->OnError(ParseEID::expectedDeclaration); YYABORT; }
+#line 639 "RSParserImpl.cpp"
+    break;
+
+  case 14: // arguments: declaration
+#line 287 "RSParserImpl.y"
+                                            { yylhs.value = AddNode(TokenID::NT_ARGUMENTS, yystack_[0].value); }
+#line 645 "RSParserImpl.cpp"
+    break;
+
+  case 15: // arguments: arguments COMMA declaration
+#line 288 "RSParserImpl.y"
+                                            { yylhs.value = Enumeration(TokenID::NT_ARGUMENTS, yystack_[2].value, yystack_[0].value); }
+#line 651 "RSParserImpl.cpp"
+    break;
+
+  case 16: // arguments: arguments COMMA error
+#line 289 "RSParserImpl.y"
+                                            { state->OnError(ParseEID::expectedLocal); YYABORT; }
+#line 657 "RSParserImpl.cpp"
+    break;
+
+  case 17: // declaration: LOCAL IN setexpr
+#line 292 "RSParserImpl.y"
+                                            { yylhs.value = AddNode(TokenID::NT_ARG_DECL, yystack_[2].value, yystack_[0].value); }
+#line 663 "RSParserImpl.cpp"
+    break;
+
+  case 18: // declaration: LOCAL error
+#line 293 "RSParserImpl.y"
+                                            { state->OnError(ParseEID::expectedDeclaration); YYABORT; }
+#line 669 "RSParserImpl.cpp"
+    break;
+
+  case 20: // variable: LP var_enum RPE
+#line 298 "RSParserImpl.y"
+                                            { yylhs.value = ReplaceBrackets(TokenID::NT_TUPLE_DECL, yystack_[2].value, yystack_[1].value, yystack_[0].value); }
+#line 675 "RSParserImpl.cpp"
+    break;
+
+  case 21: // var_enum: var_all COMMA var_all
+#line 301 "RSParserImpl.y"
+                                            { yylhs.value = Enumeration(TokenID::INTERRUPT, yystack_[2].value, yystack_[0].value); }
+#line 681 "RSParserImpl.cpp"
+    break;
+
+  case 22: // var_enum: var_all COMMA error
+#line 302 "RSParserImpl.y"
+                                            { state->OnError(ParseEID::expectedLocal); YYABORT; }
+#line 687 "RSParserImpl.cpp"
+    break;
+
+  case 30: // logic_par: LP logic_binary RPE
+#line 320 "RSParserImpl.y"
+                                            { yylhs.value = RemoveBrackets(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
+#line 693 "RSParserImpl.cpp"
+    break;
+
+  case 31: // logic_par: LP logic_predicates RPE
+#line 321 "RSParserImpl.y"
+                                            { yylhs.value = RemoveBrackets(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
+#line 699 "RSParserImpl.cpp"
+    break;
+
+  case 32: // logic_predicates: setexpr binary_predicate setexpr
+#line 325 "RSParserImpl.y"
+                                            { yylhs.value = BinaryOperation(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
+#line 705 "RSParserImpl.cpp"
+    break;
+
+  case 44: // logic_unary: NOT logic_no_binary
+#line 342 "RSParserImpl.y"
+                                            { yylhs.value = UnaryOperation(yystack_[1].value, yystack_[0].value);}
+#line 711 "RSParserImpl.cpp"
+    break;
+
+  case 45: // logic_unary: quantifier quant_var IN setexpr logic_no_binary
+#line 343 "RSParserImpl.y"
+                                                      { yylhs.value = Quantifier(yystack_[4].value, yystack_[3].value, yystack_[1].value, yystack_[0].value);}
+#line 717 "RSParserImpl.cpp"
+    break;
+
+  case 46: // logic_unary: quantifier error
+#line 344 "RSParserImpl.y"
+                                            { state->OnError(ParseEID::invalidQuantifier); YYABORT; }
+#line 723 "RSParserImpl.cpp"
+    break;
+
+  case 47: // logic_unary: PREDICATE LS setexpr_enum RS
+#line 345 "RSParserImpl.y"
+                                            { yylhs.value = FunctionCall(yystack_[3].value, yystack_[1].value, yystack_[0].value); }
+#line 729 "RSParserImpl.cpp"
+    break;
+
+  case 55: // quant_var: LP error
+#line 359 "RSParserImpl.y"
+                                            { state->OnError(ParseEID::invalidQuantifier); YYABORT; }
+#line 735 "RSParserImpl.cpp"
+    break;
+
+  case 56: // quant_var_enum: quant_var COMMA quant_var
+#line 362 "RSParserImpl.y"
+                                            { yylhs.value = Enumeration(TokenID::NT_ENUM_DECL, yystack_[2].value, yystack_[0].value); }
+#line 741 "RSParserImpl.cpp"
+    break;
+
+  case 57: // quant_var_enum: quant_var COMMA error
+#line 363 "RSParserImpl.y"
+                                            { state->OnError(ParseEID::expectedLocal); YYABORT; }
+#line 747 "RSParserImpl.cpp"
+    break;
+
+  case 58: // logic_binary: logic_all EQUIVALENT logic_all
+#line 367 "RSParserImpl.y"
+                                            { yylhs.value = BinaryOperation(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
+#line 753 "RSParserImpl.cpp"
+    break;
+
+  case 59: // logic_binary: logic_all IMPLICATION logic_all
+#line 368 "RSParserImpl.y"
+                                            { yylhs.value = BinaryOperation(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
+#line 759 "RSParserImpl.cpp"
+    break;
+
+  case 60: // logic_binary: logic_all OR logic_all
+#line 369 "RSParserImpl.y"
+                                            { yylhs.value = BinaryOperation(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
+#line 765 "RSParserImpl.cpp"
+    break;
+
+  case 61: // logic_binary: logic_all AND logic_all
+#line 370 "RSParserImpl.y"
+                                            { yylhs.value = BinaryOperation(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
+#line 771 "RSParserImpl.cpp"
+    break;
+
+  case 66: // setexpr: FUNCTION LS setexpr_enum RS
+#line 380 "RSParserImpl.y"
+                                            { yylhs.value = FunctionCall(yystack_[3].value, yystack_[1].value, yystack_[0].value); }
+#line 777 "RSParserImpl.cpp"
+    break;
+
+  case 67: // setexpr: text_function LP setexpr RPE
+#line 381 "RSParserImpl.y"
+                                            { yylhs.value = TextOperator(yystack_[3].value, yystack_[1].value, yystack_[0].value); }
+#line 783 "RSParserImpl.cpp"
+    break;
+
+  case 74: // setexpr_enum: setexpr
+#line 392 "RSParserImpl.y"
+                                            { yylhs.value = AddNode(TokenID::INTERRUPT, yystack_[0].value); }
+#line 789 "RSParserImpl.cpp"
+    break;
+
+  case 76: // setexpr_enum_min2: setexpr_enum COMMA setexpr
+#line 396 "RSParserImpl.y"
+                                            { yylhs.value = Enumeration(TokenID::INTERRUPT, yystack_[2].value, yystack_[0].value); }
+#line 795 "RSParserImpl.cpp"
+    break;
+
+  case 85: // setexpr_binary: setexpr PLUS setexpr
+#line 414 "RSParserImpl.y"
+                                            { yylhs.value = BinaryOperation(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
+#line 801 "RSParserImpl.cpp"
+    break;
+
+  case 86: // setexpr_binary: setexpr MINUS setexpr
+#line 415 "RSParserImpl.y"
+                                            { yylhs.value = BinaryOperation(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
+#line 807 "RSParserImpl.cpp"
+    break;
+
+  case 87: // setexpr_binary: setexpr MULTIPLY setexpr
+#line 416 "RSParserImpl.y"
+                                            { yylhs.value = BinaryOperation(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
+#line 813 "RSParserImpl.cpp"
+    break;
+
+  case 88: // setexpr_binary: setexpr UNION setexpr
+#line 417 "RSParserImpl.y"
+                                            { yylhs.value = BinaryOperation(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
+#line 819 "RSParserImpl.cpp"
+    break;
+
+  case 89: // setexpr_binary: setexpr SET_MINUS setexpr
+#line 418 "RSParserImpl.y"
+                                            { yylhs.value = BinaryOperation(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
+#line 825 "RSParserImpl.cpp"
+    break;
+
+  case 90: // setexpr_binary: setexpr SYMMINUS setexpr
+#line 419 "RSParserImpl.y"
+                                            { yylhs.value = BinaryOperation(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
+#line 831 "RSParserImpl.cpp"
+    break;
+
+  case 91: // setexpr_binary: setexpr INTERSECTION setexpr
+#line 420 "RSParserImpl.y"
+                                            { yylhs.value = BinaryOperation(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
+#line 837 "RSParserImpl.cpp"
+    break;
+
+  case 92: // setexpr_binary: setexpr DECART setexpr
+#line 421 "RSParserImpl.y"
+                                            { yylhs.value = Decartian(yystack_[2].value, yystack_[1].value, yystack_[0].value);}
+#line 843 "RSParserImpl.cpp"
+    break;
+
+  case 93: // setexpr_binary: LP setexpr_binary RPE
+#line 422 "RSParserImpl.y"
+                                            { yylhs.value = RemoveBrackets(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
+#line 849 "RSParserImpl.cpp"
+    break;
+
+  case 101: // enumeration: LC setexpr_enum RC
+#line 435 "RSParserImpl.y"
+                                            { yylhs.value = ReplaceBrackets(TokenID::NT_ENUMERATION, yystack_[2].value, yystack_[1].value, yystack_[0].value); }
+#line 855 "RSParserImpl.cpp"
+    break;
+
+  case 102: // tuple: LP setexpr_enum_min2 RPE
+#line 438 "RSParserImpl.y"
+                                            { yylhs.value = ReplaceBrackets(TokenID::NT_TUPLE, yystack_[2].value, yystack_[1].value, yystack_[0].value); }
+#line 861 "RSParserImpl.cpp"
+    break;
+
+  case 103: // boolean: BOOLEAN LP setexpr RPE
+#line 441 "RSParserImpl.y"
+                                            { yylhs.value = TextOperator(yystack_[3].value, yystack_[1].value, yystack_[0].value); }
+#line 867 "RSParserImpl.cpp"
+    break;
+
+  case 104: // boolean: BOOLEAN boolean
+#line 442 "RSParserImpl.y"
+                                            { yylhs.value = UnaryOperation(yystack_[1].value, yystack_[0].value); }
+#line 873 "RSParserImpl.cpp"
+    break;
+
+  case 105: // filter_expression: FILTER LS setexpr_enum RS LP setexpr RPE
+#line 445 "RSParserImpl.y"
+                                               { yylhs.value = FilterCall(yystack_[6].value, yystack_[4].value, yystack_[1].value, yystack_[0].value); }
+#line 879 "RSParserImpl.cpp"
+    break;
+
+  case 106: // declarative: LC LOCAL IN setexpr BAR logic RCE
+#line 449 "RSParserImpl.y"
+                                            { yylhs.value = TermDeclaration(yystack_[6].value, yystack_[5].value, yystack_[3].value, yystack_[1].value, yystack_[0].value); }
+#line 885 "RSParserImpl.cpp"
+    break;
+
+  case 107: // declarative: DECLARATIVE LC variable IN setexpr BAR logic RCE
+#line 450 "RSParserImpl.y"
+                                                       { yylhs.value = TermDeclaration(yystack_[7].value, yystack_[5].value, yystack_[3].value, yystack_[1].value, yystack_[0].value); }
+#line 891 "RSParserImpl.cpp"
+    break;
+
+  case 108: // recursion: RECURSIVE LC variable ASSIGN setexpr BAR logic BAR setexpr RCE
+#line 453 "RSParserImpl.y"
+                                                                     { yylhs.value = FullRecursion(yystack_[9].value, yystack_[7].value, yystack_[5].value, yystack_[3].value, yystack_[1].value, yystack_[0].value); }
+#line 897 "RSParserImpl.cpp"
+    break;
+
+  case 109: // recursion: RECURSIVE LC variable ASSIGN setexpr BAR setexpr RCE
+#line 454 "RSParserImpl.y"
+                                                           { yylhs.value = ShortRecursion(yystack_[7].value, yystack_[5].value, yystack_[3].value, yystack_[1].value, yystack_[0].value); }
+#line 903 "RSParserImpl.cpp"
+    break;
+
+  case 110: // imperative: IMPERATIVE LC setexpr BAR imp_blocks RCE
+#line 457 "RSParserImpl.y"
+                                               { yylhs.value = Imperative(yystack_[5].value, yystack_[3].value, yystack_[1].value, yystack_[0].value); }
+#line 909 "RSParserImpl.cpp"
+    break;
+
+  case 111: // imp_blocks: imp_block
+#line 460 "RSParserImpl.y"
+                                            { yylhs.value = AddNode(TokenID::INTERRUPT, yystack_[0].value); }
+#line 915 "RSParserImpl.cpp"
+    break;
+
+  case 112: // imp_blocks: imp_blocks SEMICOLON imp_blocks
+#line 461 "RSParserImpl.y"
+                                            { yylhs.value = Enumeration(TokenID::INTERRUPT, yystack_[2].value, yystack_[0].value); }
+#line 921 "RSParserImpl.cpp"
+    break;
+
+  case 113: // imp_block: LOCAL ITERATE setexpr
+#line 464 "RSParserImpl.y"
+                                            { yylhs.value = AddNode(TokenID::NT_IMP_DECLARE, yystack_[2].value, yystack_[0].value); }
+#line 927 "RSParserImpl.cpp"
+    break;
+
+  case 114: // imp_block: LOCAL ASSIGN setexpr
+#line 465 "RSParserImpl.y"
+                                            { yylhs.value = AddNode(TokenID::NT_IMP_ASSIGN, yystack_[2].value, yystack_[0].value); }
+#line 933 "RSParserImpl.cpp"
+    break;
+
+  case 115: // imp_block: logic
+#line 466 "RSParserImpl.y"
+                                            { yylhs.value = AddNode(TokenID::NT_IMP_LOGIC, yystack_[0].value); }
+#line 939 "RSParserImpl.cpp"
+    break;
+
+  case 117: // RPE: error
+#line 473 "RSParserImpl.y"
+            { state->OnError(ParseEID::missingParenthesis); YYABORT; }
+#line 945 "RSParserImpl.cpp"
+    break;
+
+  case 119: // RCE: error
+#line 477 "RSParserImpl.y"
+            { state->OnError(ParseEID::missingCurlyBrace); YYABORT; }
+#line 951 "RSParserImpl.cpp"
+    break;
+
+
+#line 955 "RSParserImpl.cpp"
+
+            default:
+              break;
+            }
+        }
+#if YY_EXCEPTIONS
+      catch (const syntax_error& yyexc)
+        {
+          YYCDEBUG << "Caught exception: " << yyexc.what() << '\n';
+          error (yyexc);
+          YYERROR;
+        }
+#endif // YY_EXCEPTIONS
+      YY_SYMBOL_PRINT ("-> $$ =", yylhs);
+      yypop_ (yylen);
+      yylen = 0;
+
+      // Shift the result of the reduction.
+      yypush_ (YY_NULLPTR, YY_MOVE (yylhs));
+    }
+    goto yynewstate;
+
+
+  /*--------------------------------------.
+  | yyerrlab -- here on detecting error.  |
+  `--------------------------------------*/
+  yyerrlab:
+    // If not already recovering from an error, report this error.
+    if (!yyerrstatus_)
+      {
+        ++yynerrs_;
+        context yyctx (*this, yyla);
+        std::string msg = yysyntax_error_ (yyctx);
+        error (YY_MOVE (msg));
+      }
+
+
+    if (yyerrstatus_ == 3)
+      {
+        /* If just tried and failed to reuse lookahead token after an
+           error, discard it.  */
+
+        // Return failure if at end of input.
+        if (yyla.kind () == symbol_kind::S_YYEOF)
+          YYABORT;
+        else if (!yyla.empty ())
+          {
+            yy_destroy_ ("Error: discarding", yyla);
+            yyla.clear ();
+          }
+      }
+
+    // Else will try to reuse lookahead token after shifting the error token.
+    goto yyerrlab1;
+
+
+  /*---------------------------------------------------.
+  | yyerrorlab -- error raised explicitly by YYERROR.  |
+  `---------------------------------------------------*/
+  yyerrorlab:
+    /* Pacify compilers when the user code never invokes YYERROR and
+       the label yyerrorlab therefore never appears in user code.  */
+    if (false)
+      YYERROR;
+
+    /* Do not reclaim the symbols of the rule whose action triggered
+       this YYERROR.  */
+    yypop_ (yylen);
+    yylen = 0;
+    YY_STACK_PRINT ();
+    goto yyerrlab1;
+
+
+  /*-------------------------------------------------------------.
+  | yyerrlab1 -- common code for both syntax error and YYERROR.  |
+  `-------------------------------------------------------------*/
+  yyerrlab1:
+    yyerrstatus_ = 3;   // Each real token shifted decrements this.
+    // Pop stack until we find a state that shifts the error token.
+    for (;;)
+      {
+        yyn = yypact_[+yystack_[0].state];
+        if (!yy_pact_value_is_default_ (yyn))
+          {
+            yyn += symbol_kind::S_YYerror;
+            if (0 <= yyn && yyn <= yylast_
+                && yycheck_[yyn] == symbol_kind::S_YYerror)
+              {
+                yyn = yytable_[yyn];
+                if (0 < yyn)
+                  break;
+              }
+          }
+
+        // Pop the current state because it cannot handle the error token.
+        if (yystack_.size () == 1)
+          YYABORT;
+
+        yy_destroy_ ("Error: popping", yystack_[0]);
+        yypop_ ();
+        YY_STACK_PRINT ();
+      }
+    {
+      stack_symbol_type error_token;
+
+
+      // Shift the error token.
+      error_token.state = state_type (yyn);
+      yypush_ ("Shifting", YY_MOVE (error_token));
+    }
+    goto yynewstate;
+
+
+  /*-------------------------------------.
+  | yyacceptlab -- YYACCEPT comes here.  |
+  `-------------------------------------*/
+  yyacceptlab:
+    yyresult = 0;
+    goto yyreturn;
+
+
+  /*-----------------------------------.
+  | yyabortlab -- YYABORT comes here.  |
+  `-----------------------------------*/
+  yyabortlab:
+    yyresult = 1;
+    goto yyreturn;
+
+
+  /*-----------------------------------------------------.
+  | yyreturn -- parsing is finished, return the result.  |
+  `-----------------------------------------------------*/
+  yyreturn:
+    if (!yyla.empty ())
+      yy_destroy_ ("Cleanup: discarding lookahead", yyla);
+
+    /* Do not reclaim the symbols of the rule whose action triggered
+       this YYABORT or YYACCEPT.  */
+    yypop_ (yylen);
+    YY_STACK_PRINT ();
+    while (1 < yystack_.size ())
+      {
+        yy_destroy_ ("Cleanup: popping", yystack_[0]);
+        yypop_ ();
+      }
+
+    return yyresult;
+  }
+#if YY_EXCEPTIONS
+    catch (...)
+      {
+        YYCDEBUG << "Exception caught: cleaning lookahead and stack\n";
+        // Do not try to display the values of the reclaimed symbols,
+        // as their printers might throw an exception.
+        if (!yyla.empty ())
+          yy_destroy_ (YY_NULLPTR, yyla);
+
+        while (1 < yystack_.size ())
+          {
+            yy_destroy_ (YY_NULLPTR, yystack_[0]);
+            yypop_ ();
+          }
+        throw;
+      }
+#endif // YY_EXCEPTIONS
+  }
+
+  void
+  RSParserImpl::error (const syntax_error& yyexc)
+  {
+    error (yyexc.what ());
+  }
+
+  /* Return YYSTR after stripping away unnecessary quotes and
+     backslashes, so that it's suitable for yyerror.  The heuristic is
+     that double-quoting is unnecessary unless the string contains an
+     apostrophe, a comma, or backslash (other than backslash-backslash).
+     YYSTR is taken from yytname.  */
+  std::string
+  RSParserImpl::yytnamerr_ (const char *yystr)
+  {
+    if (*yystr == '"')
+      {
+        std::string yyr;
+        char const *yyp = yystr;
+
+        for (;;)
+          switch (*++yyp)
+            {
+            case '\'':
+            case ',':
+              goto do_not_strip_quotes;
+
+            case '\\':
+              if (*++yyp != '\\')
+                goto do_not_strip_quotes;
+              else
+                goto append;
+
+            append:
+            default:
+              yyr += *yyp;
+              break;
+
+            case '"':
+              return yyr;
+            }
+      do_not_strip_quotes: ;
+      }
+
+    return yystr;
+  }
+
+  std::string
+  RSParserImpl::symbol_name (symbol_kind_type yysymbol)
+  {
+    return yytnamerr_ (yytname_[yysymbol]);
+  }
+
+
+
+  // RSParserImpl::context.
+  RSParserImpl::context::context (const RSParserImpl& yyparser, const symbol_type& yyla)
+    : yyparser_ (yyparser)
+    , yyla_ (yyla)
+  {}
+
+  int
+  RSParserImpl::context::expected_tokens (symbol_kind_type yyarg[], int yyargn) const
+  {
+    // Actual number of expected tokens
+    int yycount = 0;
+
+    int yyn = yypact_[+yyparser_.yystack_[0].state];
+    if (!yy_pact_value_is_default_ (yyn))
+      {
+        /* Start YYX at -YYN if negative to avoid negative indexes in
+           YYCHECK.  In other words, skip the first -YYN actions for
+           this state because they are default actions.  */
+        int yyxbegin = yyn < 0 ? -yyn : 0;
+        // Stay within bounds of both yycheck and yytname.
+        int yychecklim = yylast_ - yyn + 1;
+        int yyxend = yychecklim < YYNTOKENS ? yychecklim : YYNTOKENS;
+        for (int yyx = yyxbegin; yyx < yyxend; ++yyx)
+          if (yycheck_[yyx + yyn] == yyx && yyx != symbol_kind::S_YYerror
+              && !yy_table_value_is_error_ (yytable_[yyx + yyn]))
+            {
+              if (!yyarg)
+                ++yycount;
+              else if (yycount == yyargn)
+                return 0;
+              else
+                yyarg[yycount++] = YY_CAST (symbol_kind_type, yyx);
+            }
+      }
+
+    if (yyarg && yycount == 0 && 0 < yyargn)
+      yyarg[0] = symbol_kind::S_YYEMPTY;
+    return yycount;
+  }
+
+
+
+  int
+  RSParserImpl::yy_syntax_error_arguments_ (const context& yyctx,
+                                                 symbol_kind_type yyarg[], int yyargn) const
+  {
+    /* There are many possibilities here to consider:
+       - If this state is a consistent state with a default action, then
+         the only way this function was invoked is if the default action
+         is an error action.  In that case, don't check for expected
+         tokens because there are none.
+       - The only way there can be no lookahead present (in yyla) is
+         if this state is a consistent state with a default action.
+         Thus, detecting the absence of a lookahead is sufficient to
+         determine that there is no unexpected or expected token to
+         report.  In that case, just report a simple "syntax error".
+       - Don't assume there isn't a lookahead just because this state is
+         a consistent state with a default action.  There might have
+         been a previous inconsistent state, consistent state with a
+         non-default action, or user semantic action that manipulated
+         yyla.  (However, yyla is currently not documented for users.)
+       - Of course, the expected token list depends on states to have
+         correct lookahead information, and it depends on the parser not
+         to perform extra reductions after fetching a lookahead from the
+         scanner and before detecting a syntax error.  Thus, state merging
+         (from LALR or IELR) and default reductions corrupt the expected
+         token list.  However, the list is correct for canonical LR with
+         one exception: it will still contain any token that will not be
+         accepted due to an error action in a later state.
+    */
+
+    if (!yyctx.lookahead ().empty ())
+      {
+        if (yyarg)
+          yyarg[0] = yyctx.token ();
+        int yyn = yyctx.expected_tokens (yyarg ? yyarg + 1 : yyarg, yyargn - 1);
+        return yyn + 1;
+      }
+    return 0;
+  }
+
+  // Generate an error message.
+  std::string
+  RSParserImpl::yysyntax_error_ (const context& yyctx) const
+  {
+    // Its maximum.
+    enum { YYARGS_MAX = 5 };
+    // Arguments of yyformat.
+    symbol_kind_type yyarg[YYARGS_MAX];
+    int yycount = yy_syntax_error_arguments_ (yyctx, yyarg, YYARGS_MAX);
+
+    char const* yyformat = YY_NULLPTR;
+    switch (yycount)
+      {
+#define YYCASE_(N, S)                         \
+        case N:                               \
+          yyformat = S;                       \
+        break
+      default: // Avoid compiler warnings.
+        YYCASE_ (0, YY_("syntax error"));
+        YYCASE_ (1, YY_("syntax error, unexpected %s"));
+        YYCASE_ (2, YY_("syntax error, unexpected %s, expecting %s"));
+        YYCASE_ (3, YY_("syntax error, unexpected %s, expecting %s or %s"));
+        YYCASE_ (4, YY_("syntax error, unexpected %s, expecting %s or %s or %s"));
+        YYCASE_ (5, YY_("syntax error, unexpected %s, expecting %s or %s or %s or %s"));
+#undef YYCASE_
+      }
+
+    std::string yyres;
+    // Argument number.
+    std::ptrdiff_t yyi = 0;
+    for (char const* yyp = yyformat; *yyp; ++yyp)
+      if (yyp[0] == '%' && yyp[1] == 's' && yyi < yycount)
+        {
+          yyres += symbol_name (yyarg[yyi++]);
+          ++yyp;
+        }
+      else
+        yyres += *yyp;
+    return yyres;
+  }
+
+
+  const signed char RSParserImpl::yypact_ninf_ = -115;
+
+  const signed char RSParserImpl::yytable_ninf_ = -116;
+
+  const short
+  RSParserImpl::yypact_[] =
+  {
+     289,  -115,    83,   -21,     1,  -115,  -115,  -115,  -115,  -115,
+    -115,   395,     8,  -115,  -115,   -20,  -115,  -115,  -115,  -115,
+     -36,    -2,    42,   395,   467,    36,    46,  -115,  -115,  -115,
+      61,   161,  -115,  -115,  -115,    25,  -115,   604,    30,  -115,
+    -115,  -115,  -115,  -115,  -115,  -115,  -115,  -115,  -115,  -115,
+     395,   519,    65,   519,    65,   519,  -115,    71,    78,  -115,
+    -115,  -115,  -115,   604,   519,  -115,   519,    22,    22,   519,
+    -115,   100,   135,   604,    81,    12,   204,   140,  -115,   519,
+     326,   -38,  -115,  -115,    21,    -1,  -115,  -115,   395,   395,
+     395,   395,  -115,  -115,    28,  -115,   -12,  -115,   519,   519,
+     519,  -115,  -115,  -115,  -115,  -115,  -115,  -115,  -115,  -115,
+    -115,  -115,   519,   519,   519,   519,   519,   519,   519,  -115,
+     326,  -115,    26,  -115,    86,   143,   123,    22,   145,   107,
+     215,  -115,  -115,  -115,  -115,   519,  -115,  -115,   519,  -115,
+    -115,   519,   395,    92,    80,   177,   155,  -115,  -115,  -115,
+      19,   134,   519,    29,   115,   115,   130,  -115,  -115,  -115,
+    -115,  -115,   326,   143,  -115,  -115,  -115,   152,   519,   519,
+     447,   326,   542,   326,  -115,  -115,  -115,  -115,    37,   343,
+    -115,  -115,  -115,   519,   556,   569,   157,     7,    15,  -115,
+     395,  -115,  -115,  -115,  -115,   143,   395,   395,   519,   519,
+    -115,  -115,   447,  -115,    18,  -115,    18,   137,   253,   326,
+     326,  -115,  -115,  -115,   519,  -115,    75,  -115
+  };
+
+  const signed char
+  RSParserImpl::yydefact_[] =
+  {
+       0,    83,    80,    81,    82,    84,    77,    79,    78,    51,
+      52,     0,     0,    71,    72,     0,    73,    68,    69,    70,
+       0,     0,     0,     0,     0,     0,     0,     2,     3,     4,
+      28,     0,    29,    25,    26,     0,    27,    11,     0,    62,
+      63,    64,    65,    94,    95,    96,    97,    98,   100,    99,
+       5,     0,     0,     0,     0,     0,    80,    81,    82,    50,
+      48,    49,    44,     0,     0,   104,     0,     0,     0,     0,
+      28,     0,     0,    74,     0,     0,     0,    83,    82,     0,
+      74,     0,    75,    13,     0,     0,    14,     1,     0,     0,
+       0,     0,    46,    19,     0,    53,     0,    54,     0,     0,
+       0,    40,    41,    42,    43,    39,    38,    33,    34,    35,
+      36,    37,     0,     0,     0,     0,     0,     0,     0,     7,
+       6,     8,     0,     9,     0,     0,     0,     0,     0,     0,
+       0,   117,   116,    31,    30,     0,   102,    93,     0,   101,
+      18,     0,     0,     0,    58,    59,    60,    61,    55,    23,
+       0,     0,     0,     0,    85,    86,    87,    92,    88,    91,
+      89,    90,    32,     0,    66,    47,   103,     0,     0,     0,
+       0,    76,     0,    17,    12,    16,    15,    20,     0,     0,
+      57,    56,    67,     0,     0,     0,    83,    28,     0,   111,
+       0,    22,    24,    21,    45,     0,     0,     0,     0,     0,
+     119,   118,     0,   110,     0,   105,     0,    28,     0,   114,
+     113,   112,   106,   107,     0,   109,     0,   108
+  };
+
+  const short
+  RSParserImpl::yypgoto_[] =
+  {
+    -115,  -115,  -115,   -39,    85,  -115,    66,   -34,    32,    33,
+       4,   101,    -8,    -9,  -115,    -6,    34,  -115,    59,  -115,
+     201,     0,  -115,    67,   -16,  -115,  -115,   -11,  -115,  -115,
+    -115,   213,  -115,  -115,  -115,  -115,    27,  -115,   -66,  -114
+  };
+
+  const short
+  RSParserImpl::yydefgoto_[] =
+  {
+      -1,    26,    27,    28,    29,    85,    86,   149,   150,   151,
+      70,    31,    32,    33,   117,    34,    62,    35,    96,    97,
+      36,    63,    38,    74,    82,    39,    40,    41,    42,    43,
+      44,    45,    46,    47,    48,    49,   188,   189,   133,   203
+  };
+
+  const short
+  RSParserImpl::yytable_[] =
+  {
+      37,    95,    60,    59,    30,    61,   134,    75,  -115,   136,
+     137,   119,    76,   131,    71,   152,   200,   139,    67,   200,
+     131,   135,   140,    73,    80,    93,    92,    52,    93,   148,
+     180,    93,    93,   128,   129,    53,    66,    83,   191,    84,
+      93,   -28,   -28,   -28,   -28,    12,    87,   153,   141,    54,
+      37,   120,    68,    80,    30,    80,   142,    55,   143,   166,
+      64,   -10,  -115,    75,   125,   132,    80,  -115,    76,   130,
+     201,   -75,   132,   201,   127,   202,   200,    94,   -24,    80,
+     127,    94,   118,   164,   177,   135,    98,    99,   100,   127,
+     212,    81,   213,   175,   215,    84,    69,   182,   154,   155,
+     156,   131,   217,   174,    89,    90,    91,   112,   113,   114,
+     115,   116,   157,   158,   159,   160,   161,   162,   163,    95,
+     122,    25,   124,   -25,   -25,   -25,   -25,    53,   100,   205,
+     201,    50,    51,   126,    55,   171,   131,   121,   172,   123,
+     135,   173,    37,   165,   131,   135,    30,   112,   113,   114,
+     115,   116,   179,   132,    98,    99,   100,   169,   -27,   -27,
+     -27,   -27,   112,   113,   114,   115,   116,   138,   184,   185,
+      60,    59,   168,    61,   187,   112,   113,   114,   115,   116,
+     167,    91,   135,   195,    88,    89,    90,    91,   132,   144,
+     145,   146,   147,   178,   204,   214,   132,   208,   209,   210,
+     206,   207,    90,    91,   183,   131,   187,   198,   199,   176,
+     192,   193,   181,   194,   216,   -64,   -64,   -64,   -64,   -64,
+     -64,   -64,   -64,   -64,    72,    65,    98,    99,   100,   211,
+       0,   -64,   -64,   -64,   -64,   -64,   -64,   -64,   -64,   -64,
+     -64,     0,     0,     0,     0,     0,     0,   112,   113,   114,
+     115,   116,     0,     0,   200,     0,     0,   132,     0,     0,
+       0,     0,     0,   -64,    98,    99,   100,   101,   102,   103,
+     104,   105,   106,   170,     0,     0,     0,     0,     0,     0,
+     107,   108,   109,   110,   111,   112,   113,   114,   115,   116,
+       0,     0,     1,     2,     3,     4,     5,     6,     7,     8,
+       0,     0,     0,     0,     0,     0,     0,     0,   201,     9,
+      10,    11,     0,     0,     0,     0,     0,     0,     0,     0,
+       0,     0,     0,     0,     0,     0,    12,    13,    14,    15,
+      16,    17,    18,    19,    20,    21,    22,    98,    99,   100,
+       0,    23,     0,    24,     0,    25,     1,    56,    57,    58,
+       5,     6,     7,     8,    98,    99,   100,     0,   112,   113,
+     114,   115,   116,     9,    10,    11,     0,     0,     0,     0,
+       0,     0,     0,     0,     0,   112,   113,   114,   115,   116,
+      12,    13,    14,    15,    16,    17,    18,    19,    20,    21,
+      22,     0,     0,     0,     0,    23,     0,    24,     1,    56,
+      57,    58,     5,     6,     7,     8,     0,     0,     0,     0,
+       0,     0,     0,     0,     0,     9,    10,    11,     0,     0,
+       0,     0,     0,     0,     0,     0,     0,     0,     0,     0,
+       0,     0,    12,    13,    14,    15,    16,    17,    18,    19,
+      20,    21,    22,     0,     0,     0,     0,    23,     0,    24,
+     186,    56,    57,    58,     5,     6,     7,     8,     0,     0,
+       0,     0,     0,     0,     0,     0,     0,     9,    10,    11,
+      77,    56,    57,    78,     5,     6,     7,     8,     0,     0,
+       0,     0,     0,     0,    12,    13,    14,    15,    16,    17,
+      18,    19,    20,    21,    22,     0,     0,     0,     0,    23,
+       0,    24,     0,     0,    12,    13,    14,    15,    16,    17,
+      18,    19,    20,    21,    22,     0,     0,     0,     0,    79,
+       0,    24,     1,    56,    57,    78,     5,     6,     7,     8,
+       0,     0,     0,     0,     0,     0,     0,     0,     0,     0,
+       0,     0,     0,     0,     0,     0,     0,     0,     0,     0,
+       0,     0,     0,    98,    99,   100,    12,    13,    14,    15,
+      16,    17,    18,    19,    20,    21,    22,    98,    99,   100,
+       0,    79,     0,    24,   112,   113,   114,   115,   116,     0,
+      98,    99,   100,     0,     0,     0,     0,     0,   112,   113,
+     114,   115,   116,     0,     0,     0,     0,     0,     0,     0,
+     190,   112,   113,   114,   115,   116,     0,     0,     0,     0,
+       0,     0,     0,     0,   196,    98,    99,   100,   101,   102,
+     103,   104,   105,   106,     0,     0,     0,   197,     0,     0,
+       0,   107,   108,   109,   110,   111,   112,   113,   114,   115,
+     116
+  };
+
+  const short
+  RSParserImpl::yycheck_[] =
+  {
+       0,    35,    11,    11,     0,    11,    72,    23,     1,    75,
+      76,    50,    23,     1,    23,    27,     1,    55,    54,     1,
+       1,    59,     1,    23,    24,     3,     1,    48,     3,     1,
+       1,     3,     3,    67,    68,    56,    56,     1,     1,     3,
+       3,    23,    24,    25,    26,    37,     0,    59,    27,    48,
+      50,    51,    54,    53,    50,    55,    57,    56,    59,   125,
+      52,     0,    55,    79,    64,    53,    66,    60,    79,    69,
+      55,    59,    53,    55,    52,    60,     1,    52,    59,    79,
+      52,    52,    52,    57,   150,    59,    11,    12,    13,    52,
+     204,    24,   206,     1,   208,     3,    54,   163,    98,    99,
+     100,     1,   216,   142,    24,    25,    26,    32,    33,    34,
+      35,    36,   112,   113,   114,   115,   116,   117,   118,   153,
+      53,    56,    55,    23,    24,    25,    26,    56,    13,   195,
+      55,    48,    49,    66,    56,   135,     1,    52,   138,    54,
+      59,   141,   142,    57,     1,    59,   142,    32,    33,    34,
+      35,    36,   152,    53,    11,    12,    13,    50,    23,    24,
+      25,    26,    32,    33,    34,    35,    36,    27,   168,   169,
+     179,   179,    27,   179,   170,    32,    33,    34,    35,    36,
+      57,    26,    59,   183,    23,    24,    25,    26,    53,    88,
+      89,    90,    91,    59,   190,    58,    53,   197,   198,   199,
+     196,   197,    25,    26,    52,     1,   202,    50,    51,   143,
+     178,   178,   153,   179,   214,    11,    12,    13,    14,    15,
+      16,    17,    18,    19,    23,    12,    11,    12,    13,   202,
+      -1,    27,    28,    29,    30,    31,    32,    33,    34,    35,
+      36,    -1,    -1,    -1,    -1,    -1,    -1,    32,    33,    34,
+      35,    36,    -1,    -1,     1,    -1,    -1,    53,    -1,    -1,
+      -1,    -1,    -1,    59,    11,    12,    13,    14,    15,    16,
+      17,    18,    19,    58,    -1,    -1,    -1,    -1,    -1,    -1,
+      27,    28,    29,    30,    31,    32,    33,    34,    35,    36,
+      -1,    -1,     3,     4,     5,     6,     7,     8,     9,    10,
+      -1,    -1,    -1,    -1,    -1,    -1,    -1,    -1,    55,    20,
+      21,    22,    -1,    -1,    -1,    -1,    -1,    -1,    -1,    -1,
+      -1,    -1,    -1,    -1,    -1,    -1,    37,    38,    39,    40,
+      41,    42,    43,    44,    45,    46,    47,    11,    12,    13,
+      -1,    52,    -1,    54,    -1,    56,     3,     4,     5,     6,
+       7,     8,     9,    10,    11,    12,    13,    -1,    32,    33,
+      34,    35,    36,    20,    21,    22,    -1,    -1,    -1,    -1,
+      -1,    -1,    -1,    -1,    -1,    32,    33,    34,    35,    36,
+      37,    38,    39,    40,    41,    42,    43,    44,    45,    46,
+      47,    -1,    -1,    -1,    -1,    52,    -1,    54,     3,     4,
+       5,     6,     7,     8,     9,    10,    -1,    -1,    -1,    -1,
+      -1,    -1,    -1,    -1,    -1,    20,    21,    22,    -1,    -1,
+      -1,    -1,    -1,    -1,    -1,    -1,    -1,    -1,    -1,    -1,
+      -1,    -1,    37,    38,    39,    40,    41,    42,    43,    44,
+      45,    46,    47,    -1,    -1,    -1,    -1,    52,    -1,    54,
+       3,     4,     5,     6,     7,     8,     9,    10,    -1,    -1,
+      -1,    -1,    -1,    -1,    -1,    -1,    -1,    20,    21,    22,
+       3,     4,     5,     6,     7,     8,     9,    10,    -1,    -1,
+      -1,    -1,    -1,    -1,    37,    38,    39,    40,    41,    42,
+      43,    44,    45,    46,    47,    -1,    -1,    -1,    -1,    52,
+      -1,    54,    -1,    -1,    37,    38,    39,    40,    41,    42,
+      43,    44,    45,    46,    47,    -1,    -1,    -1,    -1,    52,
+      -1,    54,     3,     4,     5,     6,     7,     8,     9,    10,
+      -1,    -1,    -1,    -1,    -1,    -1,    -1,    -1,    -1,    -1,
+      -1,    -1,    -1,    -1,    -1,    -1,    -1,    -1,    -1,    -1,
+      -1,    -1,    -1,    11,    12,    13,    37,    38,    39,    40,
+      41,    42,    43,    44,    45,    46,    47,    11,    12,    13,
+      -1,    52,    -1,    54,    32,    33,    34,    35,    36,    -1,
+      11,    12,    13,    -1,    -1,    -1,    -1,    -1,    32,    33,
+      34,    35,    36,    -1,    -1,    -1,    -1,    -1,    -1,    -1,
+      58,    32,    33,    34,    35,    36,    -1,    -1,    -1,    -1,
+      -1,    -1,    -1,    -1,    58,    11,    12,    13,    14,    15,
+      16,    17,    18,    19,    -1,    -1,    -1,    58,    -1,    -1,
+      -1,    27,    28,    29,    30,    31,    32,    33,    34,    35,
+      36
+  };
+
+  const signed char
+  RSParserImpl::yystos_[] =
+  {
+       0,     3,     4,     5,     6,     7,     8,     9,    10,    20,
+      21,    22,    37,    38,    39,    40,    41,    42,    43,    44,
+      45,    46,    47,    52,    54,    56,    62,    63,    64,    65,
+      71,    72,    73,    74,    76,    78,    81,    82,    83,    86,
+      87,    88,    89,    90,    91,    92,    93,    94,    95,    96,
+      48,    49,    48,    56,    48,    56,     4,     5,     6,    73,
+      74,    76,    77,    82,    52,    92,    56,    54,    54,    54,
+      71,    74,    81,    82,    84,    85,    88,     3,     6,    52,
+      82,    84,    85,     1,     3,    66,    67,     0,    23,    24,
+      25,    26,     1,     3,    52,    68,    79,    80,    11,    12,
+      13,    14,    15,    16,    17,    18,    19,    27,    28,    29,
+      30,    31,    32,    33,    34,    35,    36,    75,    52,    64,
+      82,    65,    84,    65,    84,    82,    84,    52,    68,    68,
+      82,     1,    53,    99,    99,    59,    99,    99,    27,    55,
+       1,    27,    57,    59,    72,    72,    72,    72,     1,    68,
+      69,    70,    27,    59,    82,    82,    82,    82,    82,    82,
+      82,    82,    82,    82,    57,    57,    99,    57,    27,    50,
+      58,    82,    82,    82,    64,     1,    67,    99,    59,    82,
+       1,    79,    99,    52,    82,    82,     3,    71,    97,    98,
+      58,     1,    69,    70,    77,    82,    58,    58,    50,    51,
+       1,    55,    60,   100,    71,    99,    71,    71,    82,    82,
+      82,    97,   100,   100,    58,   100,    82,   100
+  };
+
+  const signed char
+  RSParserImpl::yyr1_[] =
+  {
+       0,    61,    62,    62,    62,    63,    63,    63,    63,    63,
+      64,    64,    65,    65,    66,    66,    66,    67,    67,    68,
+      68,    69,    69,    70,    70,    71,    71,    71,    72,    72,
+      73,    73,    74,    75,    75,    75,    75,    75,    75,    75,
+      75,    75,    75,    75,    76,    76,    76,    76,    77,    77,
+      77,    78,    78,    79,    79,    79,    80,    80,    81,    81,
+      81,    81,    82,    82,    82,    82,    82,    82,    83,    83,
+      83,    83,    83,    83,    84,    84,    85,    86,    86,    86,
+      87,    87,    87,    87,    87,    88,    88,    88,    88,    88,
+      88,    88,    88,    88,    89,    89,    89,    89,    89,    89,
+      89,    90,    91,    92,    92,    93,    94,    94,    95,    95,
+      96,    97,    97,    98,    98,    98,    99,    99,   100,   100
+  };
+
+  const signed char
+  RSParserImpl::yyr2_[] =
+  {
+       0,     2,     1,     1,     1,     2,     3,     3,     3,     3,
+       1,     1,     4,     2,     1,     3,     3,     3,     2,     1,
+       3,     3,     3,     1,     1,     1,     1,     1,     1,     1,
+       3,     3,     3,     1,     1,     1,     1,     1,     1,     1,
+       1,     1,     1,     1,     2,     5,     2,     4,     1,     1,
+       1,     1,     1,     1,     1,     2,     3,     3,     3,     3,
+       3,     3,     1,     1,     1,     1,     4,     4,     1,     1,
+       1,     1,     1,     1,     1,     1,     3,     1,     1,     1,
+       1,     1,     1,     1,     1,     3,     3,     3,     3,     3,
+       3,     3,     3,     3,     1,     1,     1,     1,     1,     1,
+       1,     3,     3,     4,     2,     7,     7,     8,    10,     8,
+       6,     1,     3,     3,     3,     1,     1,     1,     1,     1
+  };
+
+
+#if YYDEBUG || 1
+  // YYTNAME[SYMBOL-NUM] -- String name of the symbol SYMBOL-NUM.
+  // First, the terminals, then, starting at \a YYNTOKENS, nonterminals.
+  const char*
+  const RSParserImpl::yytname_[] =
+  {
+  "\"end of file\"", "error", "\"invalid token\"", "LOCAL", "GLOBAL",
+  "FUNCTION", "PREDICATE", "RADICAL", "INTEGER", "INTSET", "EMPTYSET",
+  "PLUS", "MINUS", "MULTIPLY", "GREATER", "LESSER", "GREATER_OR_EQ",
+  "LESSER_OR_EQ", "EQUAL", "NOTEQUAL", "FORALL", "EXISTS", "NOT",
+  "EQUIVALENT", "IMPLICATION", "OR", "AND", "IN", "NOTIN", "SUBSET",
+  "SUBSET_OR_EQ", "NOTSUBSET", "DECART", "UNION", "INTERSECTION",
+  "SET_MINUS", "SYMMINUS", "BOOLEAN", "BIGPR", "SMALLPR", "FILTER", "CARD",
+  "BOOL", "DEBOOL", "RED", "DECLARATIVE", "RECURSIVE", "IMPERATIVE",
+  "DEFINE", "STRUCT", "ASSIGN", "ITERATE", "LP", "RP", "LC", "RC", "LS",
+  "RS", "BAR", "COMMA", "SEMICOLON", "$accept", "expression",
+  "global_declaration", "logic_or_setexpr", "function_definition",
+  "arguments", "declaration", "variable", "var_enum", "var_all", "logic",
+  "logic_all", "logic_par", "logic_predicates", "binary_predicate",
+  "logic_unary", "logic_no_binary", "quantifier", "quant_var",
+  "quant_var_enum", "logic_binary", "setexpr", "text_function",
+  "setexpr_enum", "setexpr_enum_min2", "literal", "identifier",
+  "setexpr_binary", "setexpr_generators", "enumeration", "tuple",
+  "boolean", "filter_expression", "declarative", "recursion", "imperative",
+  "imp_blocks", "imp_block", "RPE", "RCE", YY_NULLPTR
+  };
+#endif
+
+
+#if YYDEBUG
+  const short
+  RSParserImpl::yyrline_[] =
+  {
+       0,   262,   262,   263,   264,   268,   269,   270,   271,   272,
+     276,   277,   281,   282,   287,   288,   289,   292,   293,   297,
+     298,   301,   302,   305,   306,   311,   312,   313,   316,   317,
+     320,   321,   325,   328,   329,   330,   331,   332,   333,   334,
+     335,   336,   337,   338,   342,   343,   344,   345,   348,   349,
+     350,   353,   354,   357,   358,   359,   362,   363,   367,   368,
+     369,   370,   376,   377,   378,   379,   380,   381,   384,   385,
+     386,   387,   388,   389,   392,   393,   396,   400,   401,   402,
+     406,   407,   408,   409,   410,   414,   415,   416,   417,   418,
+     419,   420,   421,   422,   426,   427,   428,   429,   430,   431,
+     432,   435,   438,   441,   442,   445,   449,   450,   453,   454,
+     457,   460,   461,   464,   465,   466,   472,   473,   476,   477
+  };
+
+  void
+  RSParserImpl::yy_stack_print_ () const
+  {
+    *yycdebug_ << "Stack now";
+    for (stack_type::const_iterator
+           i = yystack_.begin (),
+           i_end = yystack_.end ();
+         i != i_end; ++i)
+      *yycdebug_ << ' ' << int (i->state);
+    *yycdebug_ << '\n';
+  }
+
+  void
+  RSParserImpl::yy_reduce_print_ (int yyrule) const
+  {
+    int yylno = yyrline_[yyrule];
+    int yynrhs = yyr2_[yyrule];
+    // Print the symbols being reduced, and their result.
+    *yycdebug_ << "Reducing stack by rule " << yyrule - 1
+               << " (line " << yylno << "):\n";
+    // The symbols being reduced.
+    for (int yyi = 0; yyi < yynrhs; yyi++)
+      YY_SYMBOL_PRINT ("   $" << yyi + 1 << " =",
+                       yystack_[(yynrhs) - (yyi + 1)]);
+  }
+#endif // YYDEBUG
+
+  RSParserImpl::symbol_kind_type
+  RSParserImpl::yytranslate_ (int t)
+  {
+    // YYTRANSLATE[TOKEN-NUM] -- Symbol number corresponding to
+    // TOKEN-NUM as returned by yylex.
+    static
+    const signed char
+    translate_table[] =
+    {
+       0,     2,     2,     2,     2,     2,     2,     2,     2,     2,
+       2,     2,     2,     2,     2,     2,     2,     2,     2,     2,
+       2,     2,     2,     2,     2,     2,     2,     2,     2,     2,
+       2,     2,     2,     2,     2,     2,     2,     2,     2,     2,
+       2,     2,     2,     2,     2,     2,     2,     2,     2,     2,
+       2,     2,     2,     2,     2,     2,     2,     2,     2,     2,
+       2,     2,     2,     2,     2,     2,     2,     2,     2,     2,
+       2,     2,     2,     2,     2,     2,     2,     2,     2,     2,
+       2,     2,     2,     2,     2,     2,     2,     2,     2,     2,
+       2,     2,     2,     2,     2,     2,     2,     2,     2,     2,
+       2,     2,     2,     2,     2,     2,     2,     2,     2,     2,
+       2,     2,     2,     2,     2,     2,     2,     2,     2,     2,
+       2,     2,     2,     2,     2,     2,     2,     2,     2,     2,
+       2,     2,     2,     2,     2,     2,     2,     2,     2,     2,
+       2,     2,     2,     2,     2,     2,     2,     2,     2,     2,
+       2,     2,     2,     2,     2,     2,     2,     2,     2,     2,
+       2,     2,     2,     2,     2,     2,     2,     2,     2,     2,
+       2,     2,     2,     2,     2,     2,     2,     2,     2,     2,
+       2,     2,     2,     2,     2,     2,     2,     2,     2,     2,
+       2,     2,     2,     2,     2,     2,     2,     2,     2,     2,
+       2,     2,     2,     2,     2,     2,     2,     2,     2,     2,
+       2,     2,     2,     2,     2,     2,     2,     2,     2,     2,
+       2,     2,     2,     2,     2,     2,     2,     2,     2,     2,
+       2,     2,     2,     2,     2,     2,     2,     2,     2,     2,
+       2,     2,     2,     2,     2,     2,     2,     2,     2,     2,
+       2,     2,     2,     2,     2,     2,     1,     2,     3,     4,
+       5,     6,     7,     8,     9,    10,    11,    12,    13,    14,
+      15,    16,    17,    18,    19,    20,    21,    22,    23,    24,
+      25,    26,    27,    28,    29,    30,    31,    32,    33,    34,
+      35,    36,    37,    38,    39,    40,    41,    42,    43,    44,
+      45,    46,    47,    48,    49,    50,    51,    52,    53,    54,
+      55,    56,    57,    58,    59,    60
+    };
+    // Last valid token kind.
+    const int code_max = 315;
+
+    if (t <= 0)
+      return symbol_kind::S_YYEOF;
+    else if (t <= code_max)
+      return YY_CAST (symbol_kind_type, translate_table[t]);
+    else
+      return symbol_kind::S_YYUNDEF;
+  }
+
+#line 15 "RSParserImpl.y"
+} } } // ccl::rslang::detail
+#line 1707 "RSParserImpl.cpp"
+
+#line 484 "RSParserImpl.y"
 
 
 #ifdef _MSC_VER
   #pragma warning( pop )
 #endif
 
 #ifdef __clang__
   #pragma clang diagnostic pop
 #endif
 
 #if defined(__GNUC__) && !defined(__clang__)
   #pragma GCC diagnostic pop
-#endif
+#endif
```

### Comparing `pyconcept-0.1.3/ccl/rslang/src/RSToken.cpp` & `pyconcept-0.1.4/ccl/rslang/src/RSToken.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/src/SDImplementation.cpp` & `pyconcept-0.1.4/ccl/rslang/src/SDImplementation.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/src/SDataCompact.cpp` & `pyconcept-0.1.4/ccl/rslang/src/SDataCompact.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/src/StructuredData.cpp` & `pyconcept-0.1.4/ccl/rslang/src/StructuredData.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/src/SyntaxTree.cpp` & `pyconcept-0.1.4/ccl/rslang/src/SyntaxTree.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/src/TypeAuditor.cpp` & `pyconcept-0.1.4/ccl/rslang/src/TypeAuditor.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -45,16 +45,16 @@
 }
 
 bool IsEchelon(SyntaxTree::Cursor iter, const Index index) {
   iter.MoveToChild(index);
   return IsEchelon(iter);
 }
 
-bool IsRadical(const std::string& globalName) {
-  return !empty(globalName) && globalName.at(0) == 'R';
+bool IsRadical(const std::string& alias) {
+  return !empty(alias) && alias.at(0) == 'R' && alias.at(1) != '0';
 }
 
 void MangleRadicals(const std::string& funcName, Typification& type) {
   switch (type.Structure()) {
   case StructureType::basic: {
     if (IsRadical(type.E().baseID)) {
       type.E().baseID += funcName;
@@ -118,20 +118,19 @@
 
 bool TypeEnv::AreCompatible(const Typification& type1, const Typification& type2) const {
   if (type1 == type2) {
     return true;
   } 
   
   const auto struct1 = type1.Structure();
-  const auto struct2 = type2.Structure();
-  
-  if (struct1 == rslang::StructureType::basic && type1.E().baseID == Typification::anyTypificationName) {
+  if (struct1 == rslang::StructureType::basic && type1.IsAnyType()) {
     return true;
   }
-  if (struct2 == rslang::StructureType::basic && type2.E().baseID == Typification::anyTypificationName) {
+  const auto struct2 = type2.Structure();
+  if (struct2 == rslang::StructureType::basic && type2.IsAnyType()) {
     return true;
   }
   if (struct1 != struct2) {
     return false;
   }
 
   switch (struct1) {
@@ -153,27 +152,26 @@
   }
 }
 
 std::optional<Typification> TypeEnv::Merge(const Typification& type1, const Typification& type2) const {
   if (type1 == type2) {
     return type1;
   }
-  if (type1.Structure() != type2.Structure()) {
-    return std::nullopt;
-  }
 
   const auto struct1 = type1.Structure();
-  const auto struct2 = type2.Structure();
-
-  if (struct1 == rslang::StructureType::basic && type1.E().baseID == Typification::anyTypificationName) {
+  if (struct1 == rslang::StructureType::basic && type1.IsAnyType()) {
     return type2;
   }
-  if (struct2 == rslang::StructureType::basic && type2.E().baseID == Typification::anyTypificationName) {
+  const auto struct2 = type2.Structure();
+  if (struct2 == rslang::StructureType::basic && type2.IsAnyType()) {
     return type1;
   }
+  if (struct1 != struct2) {
+    return std::nullopt;
+  }
 
   switch (struct1) {
   default:
     case rslang::StructureType::basic: {
       const auto* type = CommonType(type1, type2);
       if (type == nullptr) {
         return std::nullopt;
@@ -214,43 +212,49 @@
     return true;
   }
   if (arg.IsElement() && IsRadical(arg.E().baseID)) {
     const auto& base = arg.E().baseID;
     if (!substitutes.contains(base)) {
       substitutes.insert({ base, value });
       return true;
+    } else {
+      auto mergeType = Merge(substitutes.at(base), value);
+      if (!mergeType.has_value()) {
+        return false;
+      }
+      substitutes.at(base) = std::move(mergeType.value());
+      return true;
     }
+  }
 
-    auto mergeType = Merge(substitutes.at(base), value);
-    if (!mergeType.has_value()) {
-      return false;
-    }
-    substitutes.at(base) = std::move(mergeType.value());
+  const auto valueStructure = value.Structure();
+  if (valueStructure == rslang::StructureType::basic && value.IsAnyType()) {
     return true;
-  } else if (arg.Structure() != value.Structure()) {
+  }
+  const auto argStructure = arg.Structure();
+  if (argStructure != valueStructure) {
     return false;
-  } else {
-    switch (arg.Structure()) {
-      default:
-      case rslang::StructureType::basic:
-        return CommonType(arg, value) != nullptr;
-      case rslang::StructureType::collection:
-        return CompareTemplated(substitutes, arg.B().Base(), value.B().Base());
-      case rslang::StructureType::tuple: {
-        if (arg.T().Arity() != value.T().Arity()) {
+  }
+  switch (argStructure) {
+    default:
+    case rslang::StructureType::basic:
+      return CommonType(arg, value) != nullptr;
+    case rslang::StructureType::collection:
+      return CompareTemplated(substitutes, arg.B().Base(), value.B().Base());
+    case rslang::StructureType::tuple: {
+      if (arg.T().Arity() != value.T().Arity()) {
+        return false;
+      }
+      const auto maxIndex = Typification::PR_START + arg.T().Arity();
+      for (auto index = Typification::PR_START; index < maxIndex; ++index) {
+        if (!CompareTemplated(substitutes, arg.T().Component(index), value.T().Component(index))) {
           return false;
         }
-        const auto maxIndex = Typification::PR_START + arg.T().Arity();
-        for (auto index = Typification::PR_START; index < maxIndex; ++index) {
-          if (!CompareTemplated(substitutes, arg.T().Component(index), value.T().Component(index))) {
-            return false;
-          }
-        }
-        return true;
       }
+      return true;
     }
   }
 }
 
 } // namespace details
 
 bool TypeAuditor::CheckType(const rslang::SyntaxTree& tree) {
@@ -293,15 +297,15 @@
 void TypeAuditor::Clear() noexcept {
   localVars.clear();
   functionArgs.clear();
   functionArgsID.clear();
   currentType = {};
 }
 
-bool TypeAuditor::ViGlobalDefinition(Cursor iter) {
+bool TypeAuditor::ViGlobalDeclaration(Cursor iter) {
   const auto childrenCount = iter.ChildrenCount();
   if (iter->id == TokenID::PUNC_STRUCT) {
     if (childrenCount != 2 || !IsEchelon(iter, 1)) {
       OnError(SemanticEID::globalStructure, iter(0).pos.finish);
       return false;
     }
     const auto maybeType = ChildType(iter, 1);
@@ -309,26 +313,26 @@
       return false;
     } 
     
     const auto& type = std::get<Typification>(maybeType.value());
     if (!type.IsCollection()) {
       return false;
     }
-    return VisitAndReturn(type.B().Base());
+    return SetCurrent(type.B().Base());
   } else {
     assert(iter->id == TokenID::PUNC_DEFINE);
     if (childrenCount == 1) {
-      return VisitAndReturn(Typification{ iter(0).data.ToText() }.ApplyBool());
+      return SetCurrent(Typification{ iter(0).data.ToText() }.ApplyBool());
     } 
     
     const auto type = ChildType(iter, 1);
     if (!type.has_value()) {
         return false;
     }
-    return VisitAndReturn(type.value());
+    return SetCurrent(type.value());
   }
 }
 
 bool TypeAuditor::ViFunctionDefinition(Cursor iter) {
   {
     const auto guard = isFuncDeclaration.CreateGuard();
     if (!VisitChild(iter, 0)) {
@@ -340,15 +344,15 @@
     functionArgs.emplace_back(localVars.at(n).arg);
   }
 
   const auto type = ChildType(iter, 1);
   if (!type.has_value()) {
     return false;
   }
-  return VisitAndReturn(type.value());
+  return SetCurrent(type.value());
 }
 
 bool TypeAuditor::ViFunctionCall(Cursor iter) {
   const auto& funcName = iter(0).data.ToText();
   const auto* funcType = env.context.TypeFor(funcName);
   if (funcType == nullptr) {
     OnError(
@@ -359,22 +363,22 @@
     return false;
   }
   const auto substitutes = CheckFuncArguments(iter, funcName);
   if (!substitutes.has_value()) {
     return false;
   }
   if (!std::holds_alternative<Typification>(*funcType)) {
-    return VisitAndReturn(*funcType);
+    return SetCurrent(*funcType);
   } else {
     Typification fixedType = std::get<Typification>(*funcType);
     MangleRadicals(funcName, fixedType);
     if (!empty(substitutes.value())) {
       fixedType.SubstituteBase(substitutes.value());
     }
-    return VisitAndReturn(fixedType);
+    return SetCurrent(fixedType);
   }
 }
 
 std::optional<Typification::Substitutes> TypeAuditor::CheckFuncArguments(Cursor iter, const std::string& funcName) {
   const auto* args = env.context.FunctionArgsFor(funcName);
   if (args == nullptr) {
     OnError(
@@ -412,93 +416,94 @@
       return std::nullopt;
     }
   }
   return substitutes;
 }
 
 bool TypeAuditor::ViGlobal(Cursor iter) {
-  const auto& globalName = iter->data.ToText();
-  if (iter->id == TokenID::ID_RADICAL) {
-    if (!isFuncDeclaration && !isTypification) {
-      OnError(
-        SemanticEID::radicalUsage,
-        iter->pos.start,
-        globalName
-      );
-      return false;
-    }
-    return VisitAndReturn(Typification(globalName).ApplyBool());
-  } else {
-    if (env.context.FunctionArgsFor(globalName) != nullptr) {
-      OnError(
-        SemanticEID::globalFuncWithoutArgs,
-        iter->pos.start,
-        globalName
-      );
-      return false;
-    }
-    const auto* type = env.context.TypeFor(globalName); 
-    if (type == nullptr) {
-      OnError(
-        SemanticEID::globalNotTyped,
-        iter->pos.start,
-        globalName
-      );
-      return false;
-    }
-    return VisitAndReturn(*type);
+  const auto& alias = iter->data.ToText();
+  if (env.context.FunctionArgsFor(alias) != nullptr) {
+    OnError(
+      SemanticEID::globalFuncWithoutArgs,
+      iter->pos.start,
+      alias
+    );
+    return false;
+  }
+  const auto* type = env.context.TypeFor(alias); 
+  if (type == nullptr) {
+    OnError(
+      SemanticEID::globalNotTyped,
+      iter->pos.start,
+      alias
+    );
+    return false;
   }
+  return SetCurrent(*type);
+}
+
+bool TypeAuditor::ViRadical(Cursor iter) {
+  const auto& alias = iter->data.ToText();
+  if (!isFuncDeclaration && !isTypification) {
+    OnError(
+      SemanticEID::radicalUsage,
+      iter->pos.start,
+      alias
+    );
+    return false;
+  }
+  return SetCurrent(Typification(alias).ApplyBool());
 }
 
 bool TypeAuditor::ViLocal(Cursor iter) {
   const auto& localName = iter->data.ToText();
   if (isLocalDeclaration || isArgDeclaration) {
-    return AddLocalVar(localName, std::get<Typification>(currentType), iter->pos.start);
+    return AddLocalVariable(localName, std::get<Typification>(currentType), iter->pos.start);
   } else {
     const auto* local = GetLocalTypification(localName, iter->pos.start);
     if (local == nullptr) {
       return false;
     }
-    return VisitAndReturn(*local);
+    return SetCurrent(*local);
   }
 }
 
 bool TypeAuditor::ViEmptySet(Cursor /*iter*/) {
-  return VisitAndReturn(Typification::EmptySet());
+  return SetCurrent(Typification::EmptySet());
 }
 
-bool TypeAuditor::ViLocalBind(Cursor iter) {
+bool TypeAuditor::ViTupleDeclaration(Cursor iter) {
   assert(isLocalDeclaration || isFuncDeclaration);
   const Typification type = std::get<Typification>(currentType);
   if (!type.IsTuple() || type.T().Arity() != iter.ChildrenCount()) {
     OnError(SemanticEID::invalidBinding, iter(0).pos.start);
     return false;
   }
   for (Index child = 0; child < iter.ChildrenCount(); ++child) {
     currentType = type.T().Component(static_cast<Index>(child + Typification::PR_START));
     if (!VisitChild(iter, child)) {
       return false;
     }
   }
-  return VisitAndReturn(type);
+  return SetCurrent(type);
 }
 
 bool TypeAuditor::ViArgument(Cursor iter) {
   const auto domain = ChildTypeDebool(iter, 1, SemanticEID::invalidTypeOperation);
   if (!domain.has_value()) {
     return false;
   }
   const auto guard{ isArgDeclaration.CreateGuard() };
   currentType = domain.value();
-  return VisitChild(iter, 0) && VisitAndReturn(LogicT{});
+  return VisitChild(iter, 0) && SetCurrent(LogicT{});
 }
 
 bool TypeAuditor::ViCard(Cursor iter) {
   return ChildTypeDebool(iter, 0, SemanticEID::invalidCard).has_value()
-    && VisitAndReturn(Typification::Integer());
+    && SetCurrent(Typification::Integer());
 }
 
 bool TypeAuditor::ViArithmetic(Cursor iter) {
   const auto test1 = ChildType(iter, 0);
   if (!test1.has_value()) {
     return false;
   } 
@@ -534,18 +539,18 @@
       SemanticEID::typesNotCompatible,
       iter(1).pos.start,
       type1,
       type2
     );
     return false;
   }
-  return VisitAndReturn(result.value());
+  return SetCurrent(result.value());
 }
 
-bool TypeAuditor::ViOrdering(Cursor iter) {
+bool TypeAuditor::ViIntegerPredicate(Cursor iter) {
   const auto test1 = ChildType(iter, 0);
   if(!test1.has_value()) {
     return false;
   } 
   
   const auto& type1 = std::get<Typification>(test1.value());
   if (!env.IsOrdered(type1)) {
@@ -577,15 +582,15 @@
       SemanticEID::typesNotCompatible,
       iter(1).pos.start,
       type1,
       type2
     );
     return false;
   }
-  return VisitAndReturn(LogicT{});
+  return SetCurrent(LogicT{});
 }
 
 bool TypeAuditor::ViQuantifier(Cursor iter) {
   StartScope();
 
   const auto domain = ChildTypeDebool(iter, 1, SemanticEID::invalidTypeOperation);
   if (!domain.has_value()) {
@@ -593,15 +598,15 @@
   } else if (!VisitChildDeclaration(iter, 0, domain.value())) {
     return false;
   } else if (!VisitChild(iter, 2)) {
     return false;
   }
 
   EndScope(iter->pos.start);
-  return VisitAndReturn(LogicT{});
+  return SetCurrent(LogicT{});
 }
 
 bool TypeAuditor::ViEquals(Cursor iter) {
   const auto test1 = ChildType(iter, 0);
   if (!test1.has_value()) {
     return false;
   }
@@ -618,18 +623,18 @@
       SemanticEID::typesNotCompatible,
       iter(1).pos.start,
       type1,
       type2
     );
     return false;
   } 
-  return VisitAndReturn(LogicT{});
+  return SetCurrent(LogicT{});
 }
 
-bool TypeAuditor::ViTypedPredicate(Cursor iter) {
+bool TypeAuditor::ViSetexprPredicate(Cursor iter) {
   auto type2 = ChildTypeDebool(iter, 1, SemanticEID::invalidTypeOperation);
   if (!type2.has_value()) {
     return false;
   }
   const auto isSubset = IsSubset(iter->id);
   if (isSubset) {
     type2.value().ApplyBool();
@@ -652,15 +657,15 @@
         SemanticEID::invalidElementPredicate,
         iter(1).pos.start,
         { ToString(type1.value()), iter->ToString(), type2->Bool().ToString() }
       );
     }
     return false;
   }
-  return VisitAndReturn(LogicT{});
+  return SetCurrent(LogicT{});
 }
 
 bool TypeAuditor::ViDeclarative(Cursor iter) {
   StartScope();
 
   auto domain = ChildTypeDebool(iter, 1, SemanticEID::invalidTypeOperation);
   if (!domain.has_value()) {
@@ -668,15 +673,15 @@
   } else if (!VisitChildDeclaration(iter, 0, domain.value())) {
     return false;
   } else if (!VisitChild(iter, 2)) {
     return false;
   }
   
   EndScope(iter->pos.start);
-  return VisitAndReturn(domain->ApplyBool());
+  return SetCurrent(domain->ApplyBool());
 }
 
 bool TypeAuditor::ViImperative(Cursor iter) {
   StartScope();
 
   for (Index child = 1; child < iter.ChildrenCount(); ++child) {
     if (!VisitChild(iter, child)) {
@@ -686,15 +691,15 @@
 
   auto type = ChildType(iter, 0); 
   if (!type.has_value()) {
     return false;
   }
 
   EndScope(iter->pos.start);
-  return VisitAndReturn(std::get<Typification>(type.value()).Bool());
+  return SetCurrent(std::get<Typification>(type.value()).Bool());
 }
 
 bool TypeAuditor::ViImpDeclare(Cursor iter) {
   const auto domain = ChildTypeDebool(iter, 1, SemanticEID::invalidTypeOperation);
   return domain.has_value() 
     && VisitChildDeclaration(iter, 0, domain.value());
 }
@@ -707,77 +712,91 @@
 
 bool TypeAuditor::ViRecursion(Cursor iter) {
   StartScope();
 
   auto initType = ChildType(iter, 1);
   if (!initType.has_value()) {
     return false;
-  } else if (!VisitChildDeclaration(iter, 0, std::get<Typification>(initType.value()))) {
+  } 
+  if (!VisitChildDeclaration(iter, 0, std::get<Typification>(initType.value()))) {
     return false;
   }
 
-  Index iterationIndex{ 2 };
-  if (iter->id == TokenID::NT_RECURSIVE_FULL) {
-    iterationIndex = 3;
-    if (!VisitChild(iter, 2)) {
-      return false;
-    }
-  }
+  const bool isFull = iter->id == TokenID::NT_RECURSIVE_FULL;
+  const auto iterationIndex = static_cast<Index>(isFull ? 3 : 2);
 
   const auto iterationType = ChildType(iter, iterationIndex);
   if (!iterationType.has_value()) {
     return false;
-  } else if (!env.AreCompatible(iterationType.value(), initType.value())) {
+  } 
+  if (!env.AreCompatible(iterationType.value(), initType.value())) {
     OnError(
       SemanticEID::typesNotEqual,
       iter(iterationIndex).pos.start, 
       iterationType.value(),
       initType.value()
     );
     return false;
   }
 
+  { 
+    const auto guard = noWarnings.CreateGuard();
+    ClearLocalVariables();
+    if (!VisitChildDeclaration(iter, 0, std::get<Typification>(iterationType.value()))) {
+      return false;
+    }
+    if (!VisitChild(iter, iterationIndex)) {
+      return false;
+    }
+  }
+
+  if (isFull) {
+    if (!VisitChild(iter, 2)) {
+      return false;
+    }
+  }
+
   EndScope(iter->pos.start);
-  return VisitAndReturn(iterationType.value());
+  return SetCurrent(iterationType.value());
 }
 
 bool TypeAuditor::ViDecart(Cursor iter) {
   std::vector<Typification> factors{};
   for (Index child = 0; child < iter.ChildrenCount(); ++child) {
     const auto type = ChildTypeDebool(iter, child, SemanticEID::invalidDecart);
     if (!type.has_value()) {
       return false;
     } else {
       factors.emplace_back(type.value());
     }
   }
-  return VisitAndReturn(Typification::Tuple(factors).ApplyBool());
+  return SetCurrent(Typification::Tuple(factors).ApplyBool());
 }
 
 bool TypeAuditor::ViBoolean(Cursor iter) {
   auto type = ChildTypeDebool(iter, 0, SemanticEID::invalidBoolean);
   if (!type.has_value()) {
     return false;
   }
-  return VisitAndReturn(type->ApplyBool().ApplyBool());
+  return SetCurrent(type->ApplyBool().ApplyBool());
 }
 
 bool TypeAuditor::ViTuple(Cursor iter) {
   std::vector<Typification> components{};
   for (Index child = 0; child < iter.ChildrenCount(); ++child) {
     const auto type = ChildType(iter, child);
     if (!type.has_value()) {
       return false;
     }
     components.emplace_back(std::get<Typification>(type.value()));
   }
-  return VisitAndReturn(Typification::Tuple(components));
+  return SetCurrent(Typification::Tuple(components));
 }
 
-bool TypeAuditor::ViSetEnum(Cursor iter) {
+bool TypeAuditor::ViEnumeration(Cursor iter) {
   auto test = ChildType(iter, 0);
   if (!test.has_value()) {
     return false;
   }
   auto& type = std::get<Typification>(test.value());
   for (Index child = 1; child < iter.ChildrenCount(); ++child) {
     auto childType = ChildType(iter, child);
@@ -793,26 +812,26 @@
         type,
         childType.value()
       );
       return false;
     }
     type = std::move(merge.value());
   }
-  return VisitAndReturn(type.Bool());
+  return SetCurrent(type.Bool());
 }
 
 bool TypeAuditor::ViDebool(Cursor iter) {
   auto type = ChildTypeDebool(iter, 0, SemanticEID::invalidDebool); 
   if (!type.has_value()) {
     return false;
   }
-  return VisitAndReturn(type.value());
+  return SetCurrent(type.value());
 }
 
-bool TypeAuditor::ViTypedBinary(Cursor iter) {
+bool TypeAuditor::ViSetexprBinary(Cursor iter) {
   auto type1 = ChildTypeDebool(iter, 0, SemanticEID::invalidTypeOperation);
   if (!type1.has_value()) {
     return false;
   }
 
   auto type2 = ChildTypeDebool(iter, 1, SemanticEID::invalidTypeOperation);
   if (!type2.has_value()) {
@@ -825,152 +844,181 @@
       SemanticEID::typesNotEqual,
       iter(1).pos.start,
       type1->Bool(),
       type2->Bool()
     );
     return false;
   }
-  return VisitAndReturn(result.value().Bool());
+  return SetCurrent(result.value().Bool());
 }
 
 bool TypeAuditor::ViProjectSet(Cursor iter) {
   // T(Pri(a)) = B(Pi(D(T(a))))
-  const auto baseType = ChildTypeDebool(iter, 0, SemanticEID::invalidProjectionSet);
-  if (!baseType.has_value()) {
+  const auto maybeArgument = ChildTypeDebool(iter, 0, SemanticEID::invalidProjectionSet);
+  if (!maybeArgument.has_value()) {
     return false;
   }
-  if (!baseType->IsTuple()) {
+  const auto& argument = maybeArgument.value();
+  if (argument.IsAnyType()) {
+    return SetCurrent(Typification::EmptySet());
+  }
+  if (!argument.IsTuple()) {
     OnError(
       SemanticEID::invalidProjectionSet,
       iter(0).pos.start,
-      { iter->ToString(), baseType->ToString() }
+      { iter->ToString(), argument.ToString() }
     );
     return false;
   }
 
   const auto& indicies = iter->data.ToTuple();
   std::vector<Typification> components{};
   components.reserve(size(indicies));
   for (const auto index : indicies) {
-    if (!baseType->T().TestIndex(index)) {
+    if (!argument.T().TestIndex(index)) {
       OnError(
         SemanticEID::invalidProjectionSet,
         iter(0).pos.start,
-        { iter->ToString(), baseType->ToString() }
+        { iter->ToString(), argument.ToString() }
       );
       return false;
     } else {
-      components.emplace_back(baseType->T().Component(index));
+      components.emplace_back(argument.T().Component(index));
     }
   }
-  currentType = Typification::Tuple(components).ApplyBool();
-  return true;
+  return SetCurrent(Typification::Tuple(components).ApplyBool());
 }
 
 bool TypeAuditor::ViProjectTuple(Cursor iter) {
   // T(pri(a)) = Pi(T(a))
-  const auto baseType = ChildType(iter, 0);
-  if (!baseType.has_value()) {
+  const auto maybeArgument = ChildType(iter, 0);
+  if (!maybeArgument.has_value()) {
     return false;
   }
-  const auto& base = std::get<Typification>(baseType.value());
-  if (!base.IsTuple()) {
-    OnError(SemanticEID::invalidProjectionTuple, iter(0).pos.start, { iter->ToString(), base.ToString() });
+  const auto& argument = std::get<Typification>(maybeArgument.value());
+  if (argument.IsAnyType()) {
+    return SetCurrent(argument);
+  }
+  if (!argument.IsTuple()) {
+    OnError(
+      SemanticEID::invalidProjectionTuple,
+      iter(0).pos.start,
+      { iter->ToString(), argument.ToString() }
+    );
     return false;
   }
   
   const auto& indicies = iter->data.ToTuple();
   std::vector<Typification> components{};
   components.reserve(size(indicies));
   for (const auto index : indicies) {
-    if (!base.T().TestIndex(index)) {
-      OnError(SemanticEID::invalidProjectionTuple, iter(0).pos.start, { iter->ToString(), base.ToString() });
+    if (!argument.T().TestIndex(index)) {
+      OnError(
+        SemanticEID::invalidProjectionTuple,
+        iter(0).pos.start,
+        { iter->ToString(), argument.ToString() }
+      );
       return false;
     } else {
-      components.emplace_back(base.T().Component(index));
+      components.emplace_back(argument.T().Component(index));
     }
   }
-  return VisitAndReturn(Typification::Tuple(components));
+  return SetCurrent(Typification::Tuple(components));
 }
 
 bool TypeAuditor::ViFilter(Cursor iter) {
-  const auto baseType = ChildType(iter, static_cast<Index>(iter.ChildrenCount() - 1));
-  if (!baseType.has_value()) {
-    return false;
-  } 
-  const auto& base = std::get<Typification>(baseType.value());
-  if (!base.IsCollection() || !base.B().Base().IsTuple()) {
-    OnError(SemanticEID::invalidFilterArgumentType,
-            iter(static_cast<Index>(iter.ChildrenCount() - 1)).pos.start,
-            { iter->ToString(), base.ToString() });
-    return false;
-  }
-
   const auto& indicies = iter->data.ToTuple();
   if (ssize(indicies) + 1 != iter.ChildrenCount()) {
     OnError(SemanticEID::invalidFilterArity, iter->pos.start);
     return false;
   }
+
+  const auto maybeArgument = ChildType(iter, static_cast<Index>(iter.ChildrenCount() - 1));
+  if (!maybeArgument.has_value()) {
+    return false;
+  } 
+  const auto& argument = std::get<Typification>(maybeArgument.value());
+  if (argument.IsAnyType() || (argument.IsCollection() && argument.B().Base().IsAnyType())) {
+    return SetCurrent(Typification::EmptySet());
+  }
+  if (!argument.IsCollection() || !argument.B().Base().IsTuple()) {
+    OnError(
+      SemanticEID::invalidFilterArgumentType,
+      iter(static_cast<Index>(iter.ChildrenCount() - 1)).pos.start,
+      { iter->ToString(), argument.ToString() }
+    );
+    return false;
+  }
+
   Index child{ 0 };
   for (const auto index : indicies) {
-    if (!base.B().Base().T().TestIndex(index)) {
-      OnError(SemanticEID::invalidFilterArgumentType, iter(static_cast<Index>(iter.ChildrenCount() - 1)).pos.start, 
-              { iter->ToString(), base.ToString() });
+    if (!argument.B().Base().T().TestIndex(index)) {
+      OnError(
+        SemanticEID::invalidFilterArgumentType,
+        iter(static_cast<Index>(iter.ChildrenCount() - 1)).pos.start,
+        { iter->ToString(), argument.ToString() }
+      );
       return false;
     } 
     const auto param = ChildType(iter, child);
     if(!param.has_value()) {
       return false;
     }
     const auto& paramType = std::get<Typification>(param.value());
     if (!paramType.IsCollection() || 
-        !env.AreCompatible(base.B().Base().T().Component(index), paramType.B().Base())) {
-      OnError(SemanticEID::typesNotEqual, iter(child).pos.start,
-              base.B().Base().T().Component(index).Bool(), paramType);
+        !env.AreCompatible(argument.B().Base().T().Component(index), paramType.B().Base())) {
+      OnError(
+        SemanticEID::typesNotEqual,
+        iter(child).pos.start,
+        argument.B().Base().T().Component(index).Bool(), paramType
+      );
       return false;
     }
     ++child;
   }
-  return VisitAndReturn(baseType.value());
+  return SetCurrent(maybeArgument.value());
 }
 
 bool TypeAuditor::ViReduce(Cursor iter) {
   // T(red(a)) = B(DD(T(a)))
-  const auto baseType = ChildType(iter, 0);
-  if (!baseType.has_value()) {
+  const auto maybeArgument = ChildType(iter, 0);
+  if (!maybeArgument.has_value()) {
     return false;
   }
-  const auto& base = std::get<Typification>(baseType.value());
-  if (!base.IsCollection() || !base.B().Base().IsCollection()) {
+  const auto& argument = std::get<Typification>(maybeArgument.value());
+  if (argument.IsAnyType() || (argument.IsCollection() && argument.B().Base().IsAnyType())) {
+    return SetCurrent(Typification::EmptySet());
+  }
+  if (!argument.IsCollection() || !argument.B().Base().IsCollection()) {
     OnError(
       SemanticEID::invalidReduce,
       iter(0).pos.start + 1,
-      base.ToString()
+      argument.ToString()
     );
     return false;
   }
-  return VisitAndReturn(base.B().Base());
+  return SetCurrent(argument.B().Base());
 }
 
-bool TypeAuditor::VisitAndReturn(ExpressionType type) noexcept {
+bool TypeAuditor::SetCurrent(ExpressionType type) noexcept {
   currentType = std::move(type);
   return true;
 }
 
-bool TypeAuditor::VisitAllAndReturn(Cursor iter, const ExpressionType& type) {
-  return VisitAllChildren(iter) && VisitAndReturn(type);
+bool TypeAuditor::VisitAllAndSetCurrent(Cursor iter, const ExpressionType& type) {
+  return VisitAllChildren(iter) && SetCurrent(type);
 }
 
 bool TypeAuditor::VisitChildDeclaration(const Cursor& iter, const Index index, const Typification& domain) {
   currentType = domain;
-  if (const auto guard = isLocalDeclaration.CreateGuard(); 
-      !VisitChild(iter, index)) {
+  const auto guard = isLocalDeclaration.CreateGuard();
+  if (!VisitChild(iter, index)) {
     return false;
   }
-  return VisitAndReturn(LogicT{});
+  return SetCurrent(LogicT{});
 }
 
 std::optional<ExpressionType> TypeAuditor::ChildType(Cursor iter, const Index index) {
   assert(iter.ChildrenCount() > index);
   
   ExpressionType result = currentType;
   iter.MoveToChild(index);
@@ -980,27 +1028,31 @@
     return std::nullopt;
   } else {
     return result;
   }
 }
 
 std::optional<Typification> TypeAuditor::ChildTypeDebool(Cursor iter, const Index index, const SemanticEID eid) {
-  const auto result = ChildType(iter, index);
-  if (!result.has_value() || !std::holds_alternative<Typification>(result.value())) {
+  const auto maybeResult = ChildType(iter, index);
+  if (!maybeResult.has_value() || !std::holds_alternative<Typification>(maybeResult.value())) {
     return std::nullopt;
   }
-  if (!std::get<Typification>(result.value()).IsCollection()) {
+  const auto& result = std::get<Typification>(maybeResult.value());
+  if (result.IsAnyType()) {
+    return result;
+  }
+  if (!result.IsCollection()) {
     OnError(
       eid,
       iter(index).pos.start,
-      ToString(result.value())
+      ToString(maybeResult.value())
     );
     return std::nullopt;
   }
-  return std::get<Typification>(result.value()).B().Base();
+  return result.B().Base();
 }
 
 const Typification* TypeAuditor::GetLocalTypification(const std::string& name, const StrPos pos) {
   const auto varIter = std::find_if(
     begin(localVars),
     end(localVars),
     [&](const auto& data) noexcept { return data.arg.name == name; }
@@ -1026,51 +1078,60 @@
 }
 
 void TypeAuditor::EndScope(const StrPos pos) {
   for (auto& var : localVars) {
     --var.level;
     if (var.level < 0 && var.enabled) {
       var.enabled = false;
-      if (var.useCount == 0) {
+      if (var.useCount == 0 && !noWarnings) {
         OnError(
           SemanticEID::localNotUsed,
           pos,
           var.arg.name
         );
       }
     }
   }
 }
 
-bool TypeAuditor::AddLocalVar(const std::string& name, const Typification& type, const StrPos pos) {
-  auto varIter = std::find_if(begin(localVars), end(localVars),
-                              [&](const auto& data) noexcept { return data.arg.name == name; });
+bool TypeAuditor::AddLocalVariable(const std::string& name, const Typification& type, const StrPos pos) {
+  auto varIter = std::find_if(
+    begin(localVars),
+    end(localVars),
+    [&](const auto& data) noexcept { return data.arg.name == name; }
+  );
   if (varIter != end(localVars)) {
     if (varIter->enabled) {
       OnError(
         SemanticEID::localShadowing,
         pos,
         name
       );
       return false;
     } else {
-      OnError(
-        SemanticEID::localDoubleDeclare,
-        pos,
-        name
-      );
+      if (!noWarnings) {
+        OnError(
+          SemanticEID::localDoubleDeclare,
+          pos,
+          name
+        );
+      }
       varIter->arg.type = type;
       varIter->enabled = true;
       varIter->level = 0;
-      varIter->useCount = 0;
-      return true;
+       return true;
     }
   } else {
     localVars.emplace_back(LocalData{ TypedID{name, type}, 0, 0, true });
     if (isArgDeclaration) {
       functionArgsID.emplace_back(localVars.size() - 1U);
     }
     return true;
   }
 }
 
+
+void TypeAuditor::ClearLocalVariables() {
+  std::erase_if(localVars, [&](const auto& data) noexcept { return data.level <= 0; });
+}
+
 } // namespace ccl::rslang
```

### Comparing `pyconcept-0.1.3/ccl/rslang/src/Typification.cpp` & `pyconcept-0.1.4/ccl/rslang/src/Typification.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 #include "ccl/cclMeta.hpp"
 #include "ccl/rslang/RSToken.h"
 
 #include <algorithm>
 
 namespace ccl::rslang {
 
+bool Typification::IsAnyType() const noexcept {
+  return IsElement() && E().baseID == anyTypificationName;
+}
+
 Typification& Typification::ApplyBool() {
   state = EchelonBool(*this);
   return *this;
 }
 
 Typification Typification::Bool() const {
   Typification newType{ *this };
```

### Comparing `pyconcept-0.1.3/ccl/rslang/src/ValueAuditor.cpp` & `pyconcept-0.1.4/ccl/rslang/src/ValueAuditor.cpp`

 * *Files 26% similar despite different names*

```diff
@@ -33,21 +33,21 @@
   }
 }
 
 void ValueAuditor::Clear() noexcept {
   current = ValueClass::invalid;
 }
 
-bool ValueAuditor::VisitAndReturn(const ValueClass type) noexcept {
+bool ValueAuditor::SetCurrent(const ValueClass type) noexcept {
   current = type;
   return true;
 }
 
-bool ValueAuditor::VisitAllAndReturn(Cursor iter, const ValueClass type) {
-  return VisitAllChildren(iter) && VisitAndReturn(type);
+bool ValueAuditor::VisitAllAndSetCurrent(Cursor iter, const ValueClass type) {
+  return VisitAllChildren(iter) && SetCurrent(type);
 }
 
 bool ValueAuditor::AssertChildIsValue(Cursor iter, const Index index) {
   if (!VisitChild(iter, index)) {
     return false;
   } else if (current != ValueClass::value) {
     OnError(SemanticEID::invalidPropertyUsage, iter(index).pos.start);
@@ -62,29 +62,29 @@
     if (!AssertChildIsValue(iter, child)) {
       return false;
     }
   }
   return true;
 }
 
-bool ValueAuditor::ViGlobalDefinition(Cursor iter) {
+bool ValueAuditor::ViGlobalDeclaration(Cursor iter) {
   if (iter->id == TokenID::PUNC_STRUCT) {
-    return VisitChild(iter, 1) && VisitAndReturn(ValueClass::value);
+    return VisitChild(iter, 1) && SetCurrent(ValueClass::value);
   } else if (iter.ChildrenCount() == 1) {
-    return VisitAndReturn(ValueClass::value);
+    return SetCurrent(ValueClass::value);
   } else {
     return VisitChild(iter, 1);
   }
 }
 
 bool ValueAuditor::ViFunctionCall(Cursor iter) {
-  const auto& globalName = iter(0).data.ToText();
-  const auto funcType = globalClass(globalName);
+  const auto& alias = iter(0).data.ToText();
+  const auto funcType = globalClass(alias);
   if (funcType == ValueClass::invalid) {
-    OnError(SemanticEID::globalNoValue, iter->pos.start, globalName);
+    OnError(SemanticEID::globalNoValue, iter->pos.start, alias);
     return false;
   }
 
   auto childrenIsValue = true;
   std::vector<ValueClass> args{};
   for (Index child = 1; child < iter.ChildrenCount(); ++child) {
     if (!VisitChild(iter, child)) {
@@ -94,15 +94,15 @@
     childrenIsValue = childrenIsValue && current == ValueClass::value;
   }
 
   if (childrenIsValue) {
     current = funcType;
     return true;
   } else {
-    return RunCheckOnFunc(iter, globalName, args);
+    return RunCheckOnFunc(iter, alias, args);
   }
 }
 
 bool ValueAuditor::RunCheckOnFunc(
   Cursor iter, 
   const std::string& funcName, 
   const std::vector<ValueClass>& argumentVals
@@ -127,42 +127,42 @@
     return false;
   }
   current = funcAuditor.VType();
   return true;
 }
 
 bool ValueAuditor::ViGlobal(Cursor iter) {
-  const auto& globalName = iter->data.ToText();
-  if (iter->id == TokenID::ID_RADICAL) {
-    return VisitAndReturn(ValueClass::value);
-  } else {
-    const auto type = globalClass(globalName);
-    if (type == ValueClass::invalid) {
-      OnError(SemanticEID::globalNoValue, iter->pos.start, globalName);
-      return false;
-    }
-    current = type;
-    return true;
+  const auto& alias = iter->data.ToText();
+  const auto type = globalClass(alias);
+  if (type == ValueClass::invalid) {
+    OnError(SemanticEID::globalNoValue, iter->pos.start, alias);
+    return false;
   }
+  current = type;
+  return true;
+}
+
+bool ValueAuditor::ViRadical(Cursor /*iter*/) {
+  return SetCurrent(ValueClass::value);
 }
 
 bool ValueAuditor::ViLocal(Cursor iter) {
   const auto& localName = iter->data.ToText();
   if (std::find(begin(localProps), end(localProps), localName) == end(localProps)) {
-    return VisitAndReturn(ValueClass::value);
+    return SetCurrent(ValueClass::value);
   } else {
-    return VisitAndReturn(ValueClass::props);
+    return SetCurrent(ValueClass::props);
   }
 }
 
 bool ValueAuditor::ViQuantifier(Cursor iter) {
   return AssertChildIsValue(iter, 1) && VisitChild(iter, 2);
 }
 
-bool ValueAuditor::ViTypedPredicate(Cursor iter) {
+bool ValueAuditor::ViSetexprPredicate(Cursor iter) {
   switch (iter->id) {
   default:
   case TokenID::IN:
   case TokenID::NOTIN:
   case TokenID::SUBSET_OR_EQ:
     return VisitChild(iter, 1) && AssertChildIsValue(iter, 0);
 
@@ -191,33 +191,33 @@
     if (!VisitChild(iter, child)) {
       return false;
     }
     if (current == ValueClass::props) {
       type = current;
     }
   }
-  return VisitAndReturn(type);
+  return SetCurrent(type);
 }
 
 bool ValueAuditor::ViBoolean(Cursor iter) {
-  return VisitChild(iter, 0) && VisitAndReturn(ValueClass::props);
+  return VisitChild(iter, 0) && SetCurrent(ValueClass::props);
 }
 
-bool ValueAuditor::ViTypedBinary(Cursor iter) {
+bool ValueAuditor::ViSetexprBinary(Cursor iter) {
   if (!VisitChild(iter, 0)) {
     return false;
   }
   const auto firstValue = current == ValueClass::value;
 
   if (!VisitChild(iter, 1)) {
     return false;
   }
   const auto secondValue = current == ValueClass::value;
 
   if (CombineOperationValues(iter->id, firstValue, secondValue)) {
-    return VisitAndReturn(ValueClass::value);
+    return SetCurrent(ValueClass::value);
   } else {
-    return VisitAndReturn(ValueClass::props);
+    return SetCurrent(ValueClass::props);
   }
 }
 
 } // namespace ccl::rslang
```

### Comparing `pyconcept-0.1.3/ccl/rslang/unity/reflex_unity1.cpp` & `pyconcept-0.1.4/ccl/rslang/unity/reflex_unity1.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/ccl/rslang/unity/reflex_unity2.cpp` & `pyconcept-0.1.4/ccl/rslang/unity/reflex_unity2.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/cmake/CXXTargets.cmake` & `pyconcept-0.1.4/cmake/CXXTargets.cmake`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/include/pyconcept.h` & `pyconcept-0.1.4/include/pyconcept.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/pyconcept.egg-info/PKG-INFO` & `pyconcept-0.1.4/pyconcept.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyconcept
-Version: 0.1.3
+Version: 0.1.4
 Summary: Concept core Python wrapper
 Author: CIHT CONCEPT, IRBorisov
 Author-email: iborisov@acconcept.ru
 License: MIT
 Project-URL: GitHub, https://github.com/IRBorisov/ConceptCore/tree/main/pyconcept
 Project-URL: Changelog, https://github.com/IRBorisov/ConceptCore/tree/main/pyconcept/CHANGELOG.md
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pyconcept-0.1.3/pyconcept.egg-info/SOURCES.txt` & `pyconcept-0.1.4/pyconcept.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/setup.cfg` & `pyconcept-0.1.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/setup.py` & `pyconcept-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/src/pyconcept.cpp` & `pyconcept-0.1.4/src/pyconcept.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/tests/__pycache__/testBinding.cpython-312.pyc` & `pyconcept-0.1.4/tests/__pycache__/testBinding.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/tests/data/Schema1.trs` & `pyconcept-0.1.4/tests/data/Schema1.trs`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.3/tests/testBinding.py` & `pyconcept-0.1.4/tests/testBinding.py`

 * *Files identical despite different names*

