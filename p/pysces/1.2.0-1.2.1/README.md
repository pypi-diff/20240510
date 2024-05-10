# Comparing `tmp/pysces-1.2.0.tar.gz` & `tmp/pysces-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysces-1.2.0.tar", last modified: Thu Feb 15 09:39:46 2024, max compression
+gzip compressed data, was "pysces-1.2.1.tar", last modified: Fri May 10 08:55:05 2024, max compression
```

## Comparing `pysces-1.2.0.tar` & `pysces-1.2.1.tar`

### file list

```diff
@@ -1,177 +1,177 @@
--rw-r--r--   0        0        0     1953 2024-02-15 09:39:14.000000 pysces-1.2.0/.github/workflows/build-conda.yml
--rw-r--r--   0        0        0     1765 2024-02-15 09:39:14.000000 pysces-1.2.0/.github/workflows/cibuildwheel.yml
--rw-r--r--   0        0        0     1516 2024-02-15 09:39:14.000000 pysces-1.2.0/.github/workflows/release-biosimulators.yml
--rw-r--r--   0        0        0     1371 2024-02-15 09:39:14.000000 pysces-1.2.0/.gitignore
--rw-r--r--   0        0        0       86 2024-02-15 09:39:14.000000 pysces-1.2.0/.gitmodules
--rw-r--r--   0        0        0      608 2024-02-15 09:39:14.000000 pysces-1.2.0/.readthedocs.yaml
--rw-r--r--   0        0        0     2996 2024-02-15 09:39:14.000000 pysces-1.2.0/.zenodo.json
--rw-r--r--   0        0        0     1186 2024-02-15 09:39:14.000000 pysces-1.2.0/ADDITIONAL_LICENCES.md
--rw-r--r--   0        0        0    11573 2024-02-15 09:39:14.000000 pysces-1.2.0/CHANGES.md
--rw-r--r--   0        0        0     1018 2024-02-15 09:39:14.000000 pysces-1.2.0/CITATION.cff
--rw-r--r--   0        0        0      775 2024-02-15 09:39:14.000000 pysces-1.2.0/CONTRIBUTORS.md
--rw-r--r--   0        0        0      953 2024-02-15 09:39:14.000000 pysces-1.2.0/DESCRIPTION.md
--rw-r--r--   0        0        0     4050 2024-02-15 09:39:14.000000 pysces-1.2.0/INSTALL.md
--rw-r--r--   0        0        0      530 2024-02-15 09:39:14.000000 pysces-1.2.0/LATEST.md
--rw-r--r--   0        0        0     1668 2024-02-15 09:39:14.000000 pysces-1.2.0/LICENSE.txt
--rw-r--r--   0        0        0     5396 2024-02-15 09:39:14.000000 pysces-1.2.0/README.md
--rw-r--r--   0        0        0     2016 2024-02-15 09:39:14.000000 pysces-1.2.0/config.py
--rw-r--r--   0        0        0    46274 2024-02-15 09:39:14.000000 pysces-1.2.0/devtest/models/BIOMD0000000012_url.xml
--rw-r--r--   0        0        0    41455 2024-02-15 09:39:14.000000 pysces-1.2.0/devtest/models/BIOMD0000000126.xml
--rw-r--r--   0        0        0    26887 2024-02-15 09:39:14.000000 pysces-1.2.0/devtest/models/BIOMD0000000860.xml
--rw-r--r--   0        0        0     6804 2024-02-15 09:39:14.000000 pysces-1.2.0/devtest/models/rohwer_sucrose2.psc
--rw-r--r--   0        0        0    88346 2024-02-15 09:39:14.000000 pysces-1.2.0/devtest/out/BIOMD0000000012_url.xml/BIOMD0000000012_url.xml-ref.png
--rw-r--r--   0        0        0    53487 2024-02-15 09:39:14.000000 pysces-1.2.0/devtest/out/BIOMD0000000126.xml/BIOMD0000000126.xml-ref.png
--rw-r--r--   0        0        0    39063 2024-02-15 09:39:14.000000 pysces-1.2.0/devtest/out/BIOMD0000000860.xml/BIOMD0000000860.xml-ref.png
--rw-r--r--   0        0        0    31594 2024-02-15 09:39:14.000000 pysces-1.2.0/devtest/out/rohwer_sucrose2/rohwer_sucrose2_fluxes-ref.png
--rw-r--r--   0        0        0    35554 2024-02-15 09:39:14.000000 pysces-1.2.0/devtest/out/rohwer_sucrose2/rohwer_sucrose2_mca-ref.png
--rw-r--r--   0        0        0    34594 2024-02-15 09:39:14.000000 pysces-1.2.0/devtest/out/rohwer_sucrose2/rohwer_sucrose2_species-ref.png
--rw-r--r--   0        0        0   152162 2024-02-15 09:39:14.000000 pysces-1.2.0/devtest/ref_data/BIOMD0000000012_url.xml/simdata.pkl
--rw-r--r--   0        0        0    50721 2024-02-15 09:39:14.000000 pysces-1.2.0/devtest/ref_data/BIOMD0000000126.xml/simdata.pkl
--rw-r--r--   0        0        0   921890 2024-02-15 09:39:14.000000 pysces-1.2.0/devtest/ref_data/BIOMD0000000860.xml/simdata.pkl
--rw-r--r--   0        0        0     2037 2024-02-15 09:39:14.000000 pysces-1.2.0/devtest/ref_data/rohwer_sucrose2/mcadata.pkl
--rw-r--r--   0        0        0     6704 2024-02-15 09:39:14.000000 pysces-1.2.0/devtest/ref_data/rohwer_sucrose2/scandata.pkl
--rw-r--r--   0        0        0      275 2024-02-15 09:39:14.000000 pysces-1.2.0/devtest/ref_data/rohwer_sucrose2/ssdata.pkl
--rw-r--r--   0        0        0      236 2024-02-15 09:39:14.000000 pysces-1.2.0/devtest/run_tests.py
--rw-r--r--   0        0        0     1440 2024-02-15 09:39:14.000000 pysces-1.2.0/devtest/test_sbml_log_ln.py
--rw-r--r--   0        0        0     1032 2024-02-15 09:39:14.000000 pysces-1.2.0/devtest/test_sbml_rules_functions.py
--rw-r--r--   0        0        0     1067 2024-02-15 09:39:14.000000 pysces-1.2.0/devtest/test_sbml_time_events.py
--rw-r--r--   0        0        0     1962 2024-02-15 09:39:14.000000 pysces-1.2.0/devtest/test_state_mca_scans.py
--rw-r--r--   0        0        0      721 2024-02-15 09:39:14.000000 pysces-1.2.0/meson.build
--rw-r--r--   0        0        0      212 2024-02-15 09:39:14.000000 pysces-1.2.0/packaging/cibuildwheel/macos_arm64.toml
--rwxr-xr-x   0        0        0     5648 2024-02-15 09:39:14.000000 pysces-1.2.0/packaging/conda-scripts/README.md
--rw-r--r--   0        0        0     2173 2024-02-15 09:39:14.000000 pysces-1.2.0/packaging/conda-scripts/VS2019_gfortran8_build.md
--rwxr-xr-x   0        0        0      272 2024-02-15 09:39:14.000000 pysces-1.2.0/packaging/conda-scripts/build_conda_linux.sh
--rwxr-xr-x   0        0        0     1322 2024-02-15 09:39:14.000000 pysces-1.2.0/packaging/conda-scripts/build_conda_macos.sh
--rw-r--r--   0        0        0     1264 2024-02-15 09:39:14.000000 pysces-1.2.0/packaging/conda-scripts/build_conda_windows.bat
--rw-r--r--   0        0        0      584 2024-02-15 09:39:14.000000 pysces-1.2.0/packaging/conda-scripts/conda_build.txt
--rw-r--r--   0        0        0      119 2024-02-15 09:39:14.000000 pysces-1.2.0/packaging/conda-unix/conda_build_config.yaml
--rw-r--r--   0        0        0      979 2024-02-15 09:39:14.000000 pysces-1.2.0/packaging/conda-unix/meta.yaml
--rw-r--r--   0        0        0       44 2024-02-15 09:39:14.000000 pysces-1.2.0/packaging/conda-win/conda_build_config.yaml
--rw-r--r--   0        0        0      877 2024-02-15 09:39:14.000000 pysces-1.2.0/packaging/conda-win/meta.yaml
--rwxr-xr-x   0        0        0     1345 2024-02-15 09:39:14.000000 pysces-1.2.0/packaging/many_linux/README.md
--rwxr-xr-x   0        0        0       82 2024-02-15 09:39:14.000000 pysces-1.2.0/packaging/many_linux/build_pysces.sh
--rwxr-xr-x   0        0        0      770 2024-02-15 09:39:14.000000 pysces-1.2.0/packaging/many_linux/build_script.sh
--rwxr-xr-x   0        0        0      221 2024-02-15 09:39:14.000000 pysces-1.2.0/packaging/many_linux/run_pysces.sh
--rw-r--r--   0        0        0      780 2024-02-15 09:39:14.000000 pysces-1.2.0/packaging/wheels_win/Instructions.txt
--rw-r--r--   0        0        0      230 2024-02-15 09:39:14.000000 pysces-1.2.0/packaging/wheels_win/README.md
--rw-r--r--   0        0        0     1612 2024-02-15 09:39:14.000000 pysces-1.2.0/packaging/wheels_win/VS2017_gfortran8_build.md
--rw-r--r--   0        0        0      359 2024-02-15 09:39:14.000000 pysces-1.2.0/packaging/wheels_win/create_environment.bat
--rw-r--r--   0        0        0      309 2024-02-15 09:39:14.000000 pysces-1.2.0/packaging/wheels_win/fix_environment.bat
--rw-r--r--   0        0        0      318 2024-02-15 09:39:14.000000 pysces-1.2.0/packaging/windows_libs/build_export_lib.md
--rw-r--r--   0        0        0  1118720 2024-02-15 09:39:14.000000 pysces-1.2.0/packaging/windows_libs/dlltool.exe
--rw-r--r--   0        0        0    55808 2024-02-15 09:39:14.000000 pysces-1.2.0/packaging/windows_libs/gendef.exe
--rw-r--r--   0        0        0     2566 2024-02-15 09:39:14.000000 pysces-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     2855 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/PyscesConfig.py
--rw-r--r--   0        0        0     6369 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/PyscesContrib.py
--rw-r--r--   0        0        0     1096 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/PyscesContribUser.py
--rw-r--r--   0        0        0     9394 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/PyscesInterfaces.py
--rw-r--r--   0        0        0    32019 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/PyscesJWSParse.py
--rw-r--r--   0        0        0    53184 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/PyscesLink.py
--rw-r--r--   0        0        0    19980 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/PyscesMiniModel.py
--rw-r--r--   0        0        0   352476 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/PyscesModel.py
--rw-r--r--   0        0        0    12084 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/PyscesModelMap.py
--rw-r--r--   0        0        0    13017 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/PyscesParScan.py
--rw-r--r--   0        0        0    57040 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/PyscesParse.py
--rw-r--r--   0        0        0    31197 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/PyscesPlot.py
--rw-r--r--   0        0        0    53209 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/PyscesPlot2.py
--rw-r--r--   0        0        0    32648 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/PyscesRandom.py
--rw-r--r--   0        0        0    30871 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/PyscesSBML.py
--rw-r--r--   0        0        0    18256 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/PyscesSED.py
--rw-r--r--   0        0        0    20424 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/PyscesScan.py
--rw-r--r--   0        0        0    56337 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/PyscesStoich.py
--rw-r--r--   0        0        0    34243 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/PyscesTest.py
--rw-r--r--   0        0        0    12593 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/PyscesUtils.py
--rw-r--r--   0        0        0    14492 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/PyscesWeb.py
--rw-r--r--   0        0        0    57146 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/RateChar.py
--rw-r--r--   0        0        0    17793 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/__init__.py
--rw-r--r--   0        0        0     2250 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/_multicorescan.py
--rw-r--r--   0        0        0     2593 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/contrib/__init__.py
--rw-r--r--   0        0        0      449 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/contrib/demo/__init__.py
--rw-r--r--   0        0        0      691 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/contrib/demo/demotest.py
--rw-r--r--   0        0        0      480 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/contrib/sbw/__init__.py
--rw-r--r--   0        0        0     8929 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/contrib/sbw/sbw_func.py
--rw-r--r--   0        0        0     9674 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/contrib/visualise/VisualiseClasses.py
--rw-r--r--   0        0        0     4668 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/contrib/visualise/VisualiseNodeClasses.py
--rw-r--r--   0        0        0     3293 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/contrib/visualise/VisualiseSBML.py
--rw-r--r--   0        0        0      429 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/contrib/visualise/__init__.py
--rw-r--r--   0        0        0    18615 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/core2/InfixParser.py
--rw-r--r--   0        0        0    55235 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/core2/PyscesCore2.py
--rw-r--r--   0        0        0    82275 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/core2/PyscesCore2Interfaces.py
--rw-r--r--   0        0        0    24562 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/core2/PyscesCore2Modules.py
--rw-r--r--   0        0        0      624 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/core2/__init__.py
--rw-r--r--   0        0        0    42905 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/core2/lex.py
--rw-r--r--   0        0        0       38 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/core2/version.py
--rw-r--r--   0        0        0   137736 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/core2/yacc.py
--rw-r--r--   0        0        0      205 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/docs/DOCS.txt
--rw-r--r--   0        0        0    26145 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/docs/HISTORY.txt
--rw-r--r--   0        0        0   490298 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/docs/userguide.pdf
--rw-r--r--   0        0        0     4105 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/examples/benchmark.ipy
--rw-r--r--   0        0        0     1362 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/examples/parallelscan.ipy
--rw-r--r--   0        0        0     4553 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/examples/pysces_stochpy.py
--rw-r--r--   0        0        0      799 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/examples/testRunScatter.py
--rw-r--r--   0        0        0     2949 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/examples/testinvalidstate.py
--rw-r--r--   0        0        0     2944 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/examples/testparscanner.py
--rw-r--r--   0        0        0     3277 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/examples/testratechar.py
--rw-r--r--   0        0        0    15437 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/kraken/Kraken.py
--rw-r--r--   0        0        0     6758 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/kraken/KrakenDataTools.py
--rw-r--r--   0        0        0    14998 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/kraken/KrakenNET.py
--rw-r--r--   0        0        0    11022 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/kraken/KrakenServer.py
--rw-r--r--   0        0        0      622 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/kraken/__init__.py
--rw-r--r--   0        0        0      304 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/kraken/controllers/kill_tentacles.py
--rw-r--r--   0        0        0     5975 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/kraken/controllers/kraken_continuation.py
--rw-r--r--   0        0        0    11564 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/kraken/controllers/kraken_continuation_eigen.py
--rw-r--r--   0        0        0     5040 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/kraken/controllers/kraken_continuation_eigen2.py
--rw-r--r--   0        0        0     3304 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/kraken/controllers/kraken_intersect.py
--rw-r--r--   0        0        0    13710 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/kraken/controllers/kraken_scanner2.py
--rw-r--r--   0        0        0      138 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/kraken/server_list
--rw-r--r--   0        0        0     3491 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/kraken/startup.py
--rw-r--r--   0        0        0     9861 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/lib/FirstDerivatives.py
--rw-r--r--   0        0        0      622 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/lib/__init__.py
--rw-r--r--   0        0        0    42905 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/lib/lex.py
--rw-r--r--   0        0        0   124351 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/lib/miriamids.py
--rw-r--r--   0        0        0   151642 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/lib/pyparsing.py
--rw-r--r--   0        0        0   137736 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/lib/yacc.py
--rw-r--r--   0        0        0     1333 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/meson.build
--rw-r--r--   0        0        0      882 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/metatool/__init__.py
--rw-r--r--   0        0        0      423 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/nleq2/4.2/__init__.py
--rw-r--r--   0        0        0   171464 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/nleq2/4.2/nleq2.f
--rw-r--r--   0        0        0     2375 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/nleq2/4.2/nleq2.pyf
--rw-r--r--   0        0        0    57391 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/nleq2/4.2/nleq2.tar.gz
--rw-r--r--   0        0        0   171463 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/nleq2/4.2/nleq2_big.f
--rw-r--r--   0        0        0   171464 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/nleq2/4.2/nleq2_gfortran.f
--rw-r--r--   0        0        0   171464 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/nleq2/4.2/nleq2_little.f
--rw-r--r--   0        0        0   171464 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/nleq2/4.2/nleq2_little_pre-gcc41.f
--rw-r--r--   0        0        0      622 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/nleq2/__init__.py
--rw-r--r--   0        0        0    18561 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/nleq2/linalg_nleq2.f
--rw-r--r--   0        0        0      687 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/nleq2/meson.build
--rw-r--r--   0        0        0    55672 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/nleq2/nleq2-4.3.tar.gz
--rw-r--r--   0        0        0   127885 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/nleq2/nleq2.f
--rw-r--r--   0        0        0     2565 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/nleq2/nleq2.pyf
--rw-r--r--   0        0        0     5594 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/nleq2/nleq2_readme.txt
--rw-r--r--   0        0        0      855 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/nleq2/readme.txt
--rw-r--r--   0        0        0     1041 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/nleq2/wnorm.f
--rw-r--r--   0        0        0      681 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/nleq2/zibconst.f
--rw-r--r--   0        0        0    10975 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/nleq2/zibmon.f
--rw-r--r--   0        0        0     1001 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/nleq2/zibsec.f
--rw-r--r--   0        0        0      436 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/pitcon/__init__.py
--rw-r--r--   0        0        0   132416 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/pitcon/dpcon61.f
--rw-r--r--   0        0        0     1917 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/pitcon/dpcon61w.f
--rw-r--r--   0        0        0      558 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/pitcon/meson.build
--rw-r--r--   0        0        0    30665 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/pitcon/pcon61subd.f
--rw-r--r--   0        0        0     2898 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/pitcon/pitcon.pyf
--rw-r--r--   0        0        0     1239 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/pitcon/readme.txt
--rw-r--r--   0        0        0      907 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/pscmodels/Burstmodel.psc
--rw-r--r--   0        0        0      577 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/pscmodels/isola2a.psc
--rw-r--r--   0        0        0     1001 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/pscmodels/lin5_hill.psc
--rw-r--r--   0        0        0      509 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/pscmodels/noisy_lin4.psc
--rw-r--r--   0        0        0      880 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/pscmodels/pysces_test_branch1.psc
--rw-r--r--   0        0        0      399 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/pscmodels/pysces_test_linear1.psc
--rw-r--r--   0        0        0      759 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/pscmodels/pysces_test_moiety1.psc
--rw-r--r--   0        0        0      656 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/pscmodels/pysces_test_pitcon.psc
--rw-r--r--   0        0        0    12091 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/sandbox/Intersect.py
--rw-r--r--   0        0        0      432 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/sandbox/__init__.py
--rw-r--r--   0        0        0      622 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/tests/__init__.py
--rw-r--r--   0        0        0      511 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/version.py
--rw-r--r--   0        0        0        6 2024-02-15 09:39:14.000000 pysces-1.2.0/pysces/version.txt
--rw-r--r--   0        0        0       31 2024-02-15 09:39:14.000000 pysces-1.2.0/requirements.txt
--rw-r--r--   0        0        0     2813 2024-02-15 09:39:47.609358 pysces-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1953 2024-05-10 08:43:00.000000 pysces-1.2.1/.github/workflows/build-conda.yml
+-rw-r--r--   0        0        0     1764 2024-05-10 08:43:00.000000 pysces-1.2.1/.github/workflows/cibuildwheel.yml
+-rw-r--r--   0        0        0     1516 2024-05-10 08:43:00.000000 pysces-1.2.1/.github/workflows/release-biosimulators.yml
+-rw-r--r--   0        0        0     1371 2024-05-10 08:43:00.000000 pysces-1.2.1/.gitignore
+-rw-r--r--   0        0        0       86 2024-05-10 08:43:00.000000 pysces-1.2.1/.gitmodules
+-rw-r--r--   0        0        0      608 2024-05-10 08:43:00.000000 pysces-1.2.1/.readthedocs.yaml
+-rw-r--r--   0        0        0     2996 2024-05-10 08:43:00.000000 pysces-1.2.1/.zenodo.json
+-rw-r--r--   0        0        0     1186 2024-05-10 08:43:00.000000 pysces-1.2.1/ADDITIONAL_LICENCES.md
+-rw-r--r--   0        0        0    14126 2024-05-10 08:43:00.000000 pysces-1.2.1/CHANGES.md
+-rw-r--r--   0        0        0     1018 2024-05-10 08:43:00.000000 pysces-1.2.1/CITATION.cff
+-rw-r--r--   0        0        0      775 2024-05-10 08:43:00.000000 pysces-1.2.1/CONTRIBUTORS.md
+-rw-r--r--   0        0        0      953 2024-05-10 08:43:00.000000 pysces-1.2.1/DESCRIPTION.md
+-rw-r--r--   0        0        0     4303 2024-05-10 08:43:00.000000 pysces-1.2.1/INSTALL.md
+-rw-r--r--   0        0        0      530 2024-05-10 08:43:00.000000 pysces-1.2.1/LATEST.md
+-rw-r--r--   0        0        0     1668 2024-05-10 08:43:00.000000 pysces-1.2.1/LICENSE.txt
+-rw-r--r--   0        0        0     5396 2024-05-10 08:43:00.000000 pysces-1.2.1/README.md
+-rw-r--r--   0        0        0     2016 2024-05-10 08:43:00.000000 pysces-1.2.1/config.py
+-rw-r--r--   0        0        0    46274 2024-05-10 08:43:00.000000 pysces-1.2.1/devtest/models/BIOMD0000000012_url.xml
+-rw-r--r--   0        0        0    41455 2024-05-10 08:43:00.000000 pysces-1.2.1/devtest/models/BIOMD0000000126.xml
+-rw-r--r--   0        0        0    26887 2024-05-10 08:43:00.000000 pysces-1.2.1/devtest/models/BIOMD0000000860.xml
+-rw-r--r--   0        0        0     6804 2024-05-10 08:43:00.000000 pysces-1.2.1/devtest/models/rohwer_sucrose2.psc
+-rw-r--r--   0        0        0    88346 2024-05-10 08:43:00.000000 pysces-1.2.1/devtest/out/BIOMD0000000012_url.xml/BIOMD0000000012_url.xml-ref.png
+-rw-r--r--   0        0        0    53487 2024-05-10 08:43:00.000000 pysces-1.2.1/devtest/out/BIOMD0000000126.xml/BIOMD0000000126.xml-ref.png
+-rw-r--r--   0        0        0    39063 2024-05-10 08:43:00.000000 pysces-1.2.1/devtest/out/BIOMD0000000860.xml/BIOMD0000000860.xml-ref.png
+-rw-r--r--   0        0        0    31594 2024-05-10 08:43:00.000000 pysces-1.2.1/devtest/out/rohwer_sucrose2/rohwer_sucrose2_fluxes-ref.png
+-rw-r--r--   0        0        0    35554 2024-05-10 08:43:00.000000 pysces-1.2.1/devtest/out/rohwer_sucrose2/rohwer_sucrose2_mca-ref.png
+-rw-r--r--   0        0        0    34594 2024-05-10 08:43:00.000000 pysces-1.2.1/devtest/out/rohwer_sucrose2/rohwer_sucrose2_species-ref.png
+-rw-r--r--   0        0        0   152162 2024-05-10 08:43:00.000000 pysces-1.2.1/devtest/ref_data/BIOMD0000000012_url.xml/simdata.pkl
+-rw-r--r--   0        0        0    50721 2024-05-10 08:43:00.000000 pysces-1.2.1/devtest/ref_data/BIOMD0000000126.xml/simdata.pkl
+-rw-r--r--   0        0        0   921890 2024-05-10 08:43:00.000000 pysces-1.2.1/devtest/ref_data/BIOMD0000000860.xml/simdata.pkl
+-rw-r--r--   0        0        0     2037 2024-05-10 08:43:00.000000 pysces-1.2.1/devtest/ref_data/rohwer_sucrose2/mcadata.pkl
+-rw-r--r--   0        0        0     6704 2024-05-10 08:43:00.000000 pysces-1.2.1/devtest/ref_data/rohwer_sucrose2/scandata.pkl
+-rw-r--r--   0        0        0      275 2024-05-10 08:43:00.000000 pysces-1.2.1/devtest/ref_data/rohwer_sucrose2/ssdata.pkl
+-rw-r--r--   0        0        0      236 2024-05-10 08:43:00.000000 pysces-1.2.1/devtest/run_tests.py
+-rw-r--r--   0        0        0     1440 2024-05-10 08:43:00.000000 pysces-1.2.1/devtest/test_sbml_log_ln.py
+-rw-r--r--   0        0        0     1032 2024-05-10 08:43:00.000000 pysces-1.2.1/devtest/test_sbml_rules_functions.py
+-rw-r--r--   0        0        0     1067 2024-05-10 08:43:00.000000 pysces-1.2.1/devtest/test_sbml_time_events.py
+-rw-r--r--   0        0        0     1962 2024-05-10 08:43:00.000000 pysces-1.2.1/devtest/test_state_mca_scans.py
+-rw-r--r--   0        0        0      721 2024-05-10 08:43:00.000000 pysces-1.2.1/meson.build
+-rw-r--r--   0        0        0      212 2024-05-10 08:43:00.000000 pysces-1.2.1/packaging/cibuildwheel/macos_arm64.toml
+-rwxr-xr-x   0        0        0     5648 2024-05-10 08:43:00.000000 pysces-1.2.1/packaging/conda-scripts/README.md
+-rw-r--r--   0        0        0     2173 2024-05-10 08:43:00.000000 pysces-1.2.1/packaging/conda-scripts/VS2019_gfortran8_build.md
+-rwxr-xr-x   0        0        0      272 2024-05-10 08:43:00.000000 pysces-1.2.1/packaging/conda-scripts/build_conda_linux.sh
+-rwxr-xr-x   0        0        0     1322 2024-05-10 08:43:00.000000 pysces-1.2.1/packaging/conda-scripts/build_conda_macos.sh
+-rw-r--r--   0        0        0     1264 2024-05-10 08:43:00.000000 pysces-1.2.1/packaging/conda-scripts/build_conda_windows.bat
+-rw-r--r--   0        0        0      584 2024-05-10 08:43:00.000000 pysces-1.2.1/packaging/conda-scripts/conda_build.txt
+-rw-r--r--   0        0        0      119 2024-05-10 08:43:00.000000 pysces-1.2.1/packaging/conda-unix/conda_build_config.yaml
+-rw-r--r--   0        0        0      979 2024-05-10 08:43:00.000000 pysces-1.2.1/packaging/conda-unix/meta.yaml
+-rw-r--r--   0        0        0       44 2024-05-10 08:43:00.000000 pysces-1.2.1/packaging/conda-win/conda_build_config.yaml
+-rw-r--r--   0        0        0      877 2024-05-10 08:43:00.000000 pysces-1.2.1/packaging/conda-win/meta.yaml
+-rwxr-xr-x   0        0        0     1345 2024-05-10 08:43:00.000000 pysces-1.2.1/packaging/many_linux/README.md
+-rwxr-xr-x   0        0        0       82 2024-05-10 08:43:00.000000 pysces-1.2.1/packaging/many_linux/build_pysces.sh
+-rwxr-xr-x   0        0        0      770 2024-05-10 08:43:00.000000 pysces-1.2.1/packaging/many_linux/build_script.sh
+-rwxr-xr-x   0        0        0      221 2024-05-10 08:43:00.000000 pysces-1.2.1/packaging/many_linux/run_pysces.sh
+-rw-r--r--   0        0        0      780 2024-05-10 08:43:00.000000 pysces-1.2.1/packaging/wheels_win/Instructions.txt
+-rw-r--r--   0        0        0      230 2024-05-10 08:43:00.000000 pysces-1.2.1/packaging/wheels_win/README.md
+-rw-r--r--   0        0        0     1612 2024-05-10 08:43:00.000000 pysces-1.2.1/packaging/wheels_win/VS2017_gfortran8_build.md
+-rw-r--r--   0        0        0      359 2024-05-10 08:43:00.000000 pysces-1.2.1/packaging/wheels_win/create_environment.bat
+-rw-r--r--   0        0        0      309 2024-05-10 08:43:00.000000 pysces-1.2.1/packaging/wheels_win/fix_environment.bat
+-rw-r--r--   0        0        0      318 2024-05-10 08:43:00.000000 pysces-1.2.1/packaging/windows_libs/build_export_lib.md
+-rw-r--r--   0        0        0  1118720 2024-05-10 08:43:00.000000 pysces-1.2.1/packaging/windows_libs/dlltool.exe
+-rw-r--r--   0        0        0    55808 2024-05-10 08:43:00.000000 pysces-1.2.1/packaging/windows_libs/gendef.exe
+-rw-r--r--   0        0        0     2566 2024-05-10 08:43:00.000000 pysces-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2855 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/PyscesConfig.py
+-rw-r--r--   0        0        0     6369 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/PyscesContrib.py
+-rw-r--r--   0        0        0     1096 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/PyscesContribUser.py
+-rw-r--r--   0        0        0     9394 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/PyscesInterfaces.py
+-rw-r--r--   0        0        0    32019 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/PyscesJWSParse.py
+-rw-r--r--   0        0        0    53184 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/PyscesLink.py
+-rw-r--r--   0        0        0    19980 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/PyscesMiniModel.py
+-rw-r--r--   0        0        0   352874 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/PyscesModel.py
+-rw-r--r--   0        0        0    12084 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/PyscesModelMap.py
+-rw-r--r--   0        0        0    13017 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/PyscesParScan.py
+-rw-r--r--   0        0        0    57040 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/PyscesParse.py
+-rw-r--r--   0        0        0    31197 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/PyscesPlot.py
+-rw-r--r--   0        0        0    53209 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/PyscesPlot2.py
+-rw-r--r--   0        0        0    32648 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/PyscesRandom.py
+-rw-r--r--   0        0        0    30871 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/PyscesSBML.py
+-rw-r--r--   0        0        0    18256 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/PyscesSED.py
+-rw-r--r--   0        0        0    20424 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/PyscesScan.py
+-rw-r--r--   0        0        0    55929 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/PyscesStoich.py
+-rw-r--r--   0        0        0    34243 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/PyscesTest.py
+-rw-r--r--   0        0        0    12593 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/PyscesUtils.py
+-rw-r--r--   0        0        0    14492 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/PyscesWeb.py
+-rw-r--r--   0        0        0    57146 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/RateChar.py
+-rw-r--r--   0        0        0    17793 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/__init__.py
+-rw-r--r--   0        0        0     2250 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/_multicorescan.py
+-rw-r--r--   0        0        0     2593 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/contrib/__init__.py
+-rw-r--r--   0        0        0      449 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/contrib/demo/__init__.py
+-rw-r--r--   0        0        0      691 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/contrib/demo/demotest.py
+-rw-r--r--   0        0        0      480 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/contrib/sbw/__init__.py
+-rw-r--r--   0        0        0     8929 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/contrib/sbw/sbw_func.py
+-rw-r--r--   0        0        0     9674 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/contrib/visualise/VisualiseClasses.py
+-rw-r--r--   0        0        0     4668 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/contrib/visualise/VisualiseNodeClasses.py
+-rw-r--r--   0        0        0     3293 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/contrib/visualise/VisualiseSBML.py
+-rw-r--r--   0        0        0      429 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/contrib/visualise/__init__.py
+-rw-r--r--   0        0        0    18615 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/core2/InfixParser.py
+-rw-r--r--   0        0        0    55235 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/core2/PyscesCore2.py
+-rw-r--r--   0        0        0    82275 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/core2/PyscesCore2Interfaces.py
+-rw-r--r--   0        0        0    24562 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/core2/PyscesCore2Modules.py
+-rw-r--r--   0        0        0      624 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/core2/__init__.py
+-rw-r--r--   0        0        0    42905 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/core2/lex.py
+-rw-r--r--   0        0        0       38 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/core2/version.py
+-rw-r--r--   0        0        0   137736 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/core2/yacc.py
+-rw-r--r--   0        0        0      205 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/docs/DOCS.txt
+-rw-r--r--   0        0        0    26145 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/docs/HISTORY.txt
+-rw-r--r--   0        0        0   490298 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/docs/userguide.pdf
+-rw-r--r--   0        0        0     4105 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/examples/benchmark.ipy
+-rw-r--r--   0        0        0     1362 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/examples/parallelscan.ipy
+-rw-r--r--   0        0        0     4553 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/examples/pysces_stochpy.py
+-rw-r--r--   0        0        0      799 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/examples/testRunScatter.py
+-rw-r--r--   0        0        0     2949 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/examples/testinvalidstate.py
+-rw-r--r--   0        0        0     2944 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/examples/testparscanner.py
+-rw-r--r--   0        0        0     3277 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/examples/testratechar.py
+-rw-r--r--   0        0        0    15437 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/kraken/Kraken.py
+-rw-r--r--   0        0        0     6758 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/kraken/KrakenDataTools.py
+-rw-r--r--   0        0        0    14998 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/kraken/KrakenNET.py
+-rw-r--r--   0        0        0    11022 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/kraken/KrakenServer.py
+-rw-r--r--   0        0        0      622 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/kraken/__init__.py
+-rw-r--r--   0        0        0      304 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/kraken/controllers/kill_tentacles.py
+-rw-r--r--   0        0        0     5975 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/kraken/controllers/kraken_continuation.py
+-rw-r--r--   0        0        0    11564 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/kraken/controllers/kraken_continuation_eigen.py
+-rw-r--r--   0        0        0     5040 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/kraken/controllers/kraken_continuation_eigen2.py
+-rw-r--r--   0        0        0     3304 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/kraken/controllers/kraken_intersect.py
+-rw-r--r--   0        0        0    13710 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/kraken/controllers/kraken_scanner2.py
+-rw-r--r--   0        0        0      138 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/kraken/server_list
+-rw-r--r--   0        0        0     3491 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/kraken/startup.py
+-rw-r--r--   0        0        0     9861 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/lib/FirstDerivatives.py
+-rw-r--r--   0        0        0      622 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/lib/__init__.py
+-rw-r--r--   0        0        0    42905 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/lib/lex.py
+-rw-r--r--   0        0        0   124351 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/lib/miriamids.py
+-rw-r--r--   0        0        0   151642 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/lib/pyparsing.py
+-rw-r--r--   0        0        0   137736 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/lib/yacc.py
+-rw-r--r--   0        0        0     1333 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/meson.build
+-rw-r--r--   0        0        0      882 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/metatool/__init__.py
+-rw-r--r--   0        0        0      423 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/nleq2/4.2/__init__.py
+-rw-r--r--   0        0        0   171464 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/nleq2/4.2/nleq2.f
+-rw-r--r--   0        0        0     2375 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/nleq2/4.2/nleq2.pyf
+-rw-r--r--   0        0        0    57391 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/nleq2/4.2/nleq2.tar.gz
+-rw-r--r--   0        0        0   171463 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/nleq2/4.2/nleq2_big.f
+-rw-r--r--   0        0        0   171464 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/nleq2/4.2/nleq2_gfortran.f
+-rw-r--r--   0        0        0   171464 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/nleq2/4.2/nleq2_little.f
+-rw-r--r--   0        0        0   171464 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/nleq2/4.2/nleq2_little_pre-gcc41.f
+-rw-r--r--   0        0        0      622 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/nleq2/__init__.py
+-rw-r--r--   0        0        0    18561 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/nleq2/linalg_nleq2.f
+-rw-r--r--   0        0        0      687 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/nleq2/meson.build
+-rw-r--r--   0        0        0    55672 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/nleq2/nleq2-4.3.tar.gz
+-rw-r--r--   0        0        0   127885 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/nleq2/nleq2.f
+-rw-r--r--   0        0        0     2565 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/nleq2/nleq2.pyf
+-rw-r--r--   0        0        0     5594 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/nleq2/nleq2_readme.txt
+-rw-r--r--   0        0        0      855 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/nleq2/readme.txt
+-rw-r--r--   0        0        0     1041 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/nleq2/wnorm.f
+-rw-r--r--   0        0        0      681 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/nleq2/zibconst.f
+-rw-r--r--   0        0        0    10975 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/nleq2/zibmon.f
+-rw-r--r--   0        0        0     1001 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/nleq2/zibsec.f
+-rw-r--r--   0        0        0      436 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/pitcon/__init__.py
+-rw-r--r--   0        0        0   132416 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/pitcon/dpcon61.f
+-rw-r--r--   0        0        0     1917 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/pitcon/dpcon61w.f
+-rw-r--r--   0        0        0      558 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/pitcon/meson.build
+-rw-r--r--   0        0        0    30665 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/pitcon/pcon61subd.f
+-rw-r--r--   0        0        0     2898 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/pitcon/pitcon.pyf
+-rw-r--r--   0        0        0     1239 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/pitcon/readme.txt
+-rw-r--r--   0        0        0      907 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/pscmodels/Burstmodel.psc
+-rw-r--r--   0        0        0      577 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/pscmodels/isola2a.psc
+-rw-r--r--   0        0        0     1001 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/pscmodels/lin5_hill.psc
+-rw-r--r--   0        0        0      509 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/pscmodels/noisy_lin4.psc
+-rw-r--r--   0        0        0      880 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/pscmodels/pysces_test_branch1.psc
+-rw-r--r--   0        0        0      399 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/pscmodels/pysces_test_linear1.psc
+-rw-r--r--   0        0        0      759 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/pscmodels/pysces_test_moiety1.psc
+-rw-r--r--   0        0        0      656 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/pscmodels/pysces_test_pitcon.psc
+-rw-r--r--   0        0        0    12091 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/sandbox/Intersect.py
+-rw-r--r--   0        0        0      432 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/sandbox/__init__.py
+-rw-r--r--   0        0        0      622 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/tests/__init__.py
+-rw-r--r--   0        0        0      511 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/version.py
+-rw-r--r--   0        0        0        6 2024-05-10 08:43:00.000000 pysces-1.2.1/pysces/version.txt
+-rw-r--r--   0        0        0       31 2024-05-10 08:43:00.000000 pysces-1.2.1/requirements.txt
+-rw-r--r--   0        0        0     2813 2024-05-10 08:55:06.099242 pysces-1.2.1/PKG-INFO
```

### Comparing `pysces-1.2.0/.github/workflows/build-conda.yml` & `pysces-1.2.1/.github/workflows/build-conda.yml`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/.github/workflows/cibuildwheel.yml` & `pysces-1.2.1/.github/workflows/cibuildwheel.yml`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
           name: sdist
           path: ./dist/*.tar.gz
 
   upload_pypi:
     needs: [build_wheels, build_sdist]
     runs-on: ubuntu-latest
     # to publish when a GitHub Release is created:
-#    if: github.event_name == 'release' && github.event.action == 'released'
+    if: github.event_name == 'release' && github.event.action == 'released'
     steps:
       - uses: actions/download-artifact@v4
         with:
           path: dist
           merge-multiple: true
 
       - name: Display structure of downloaded files
```

### Comparing `pysces-1.2.0/.github/workflows/release-biosimulators.yml` & `pysces-1.2.1/.github/workflows/release-biosimulators.yml`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/.gitignore` & `pysces-1.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/.readthedocs.yaml` & `pysces-1.2.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/.zenodo.json` & `pysces-1.2.1/.zenodo.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8888888888888888%*

 * *Differences: {"'publication_date'": "'2024-05-10'", "'version'": "'1.2.1'"}*

```diff
@@ -11,12 +11,12 @@
             "name": "Rohwer, Johann",
             "orcid": "0000-0001-6288-8904"
         }
     ],
     "description": "<p>Computer modelling has become an integral tool in the analysis and understanding of the reaction networks that underlie cellular processes. PySCeS, first released in 2003, is extremely flexible, user-extensible, open source, software actively used and developed by a community of researchers and developers.</p>\n\n<p><strong>Features</strong></p>\n\n<ul>\n\t<li>Simulate&nbsp;your time courses with solvers like LSODA and CVODE.</li>\n\t<li>Efficiently determine&nbsp;steady states&nbsp;using a selection of non-linear, root-finding algorithms (e.g. HYBRD, NLEQ2).</li>\n\t<li>Use&nbsp;Metabolic Control Analysis&nbsp;(MCA) to investigate control and regulation of cellular systems (elasticities, flux- and concentration-control and response coefficients).</li>\n\t<li>Auto-generate the stoichiometric matrix and perform&nbsp;structural analysis, determine nullspaces and reduced stoichiometric and MCA matrices.</li>\n\t<li>Investigate systems which exhibit multiple (stable and unstable) steady-state solutions using a PITCON-based bifurcation analysis module.</li>\n\t<li>Define models with a human-readable&nbsp;Model Description Language.</li>\n\t<li>Use the full power of Python available to test, build and share your modelling experiments.</li>\n\t<li>User-friendly methods for generating and 1-, 2- and n-dimensional&nbsp;parameter scans.</li>\n\t<li>Distributed parameter scanning with the&nbsp;ParScanner&nbsp;module within the&nbsp;<em>ipyparallel</em>&nbsp;framework.</li>\n\t<li>Visualise&nbsp;results of simulations with flexible Matplotlib and Gnuplot interfaces.</li>\n\t<li>PySCeS supports open community standards for&nbsp;model exchange&nbsp;(<a href=\"http://sbml.org/\">SBML</a>) and archiving (SEDML, OMEX).</li>\n</ul>\n\n<p><strong>Installation</strong></p>\n\n<p>PyPI</p>\n\n<pre>pip install pysces</pre>\n\n<p>Anaconda.org</p>\n\n<pre>conda install -c conda-forge -c pysces pysces</pre>\n\n<p><strong>Getting help</strong></p>\n\n<p>We currently encourage users to ask questions and request support using a GitHub&nbsp;<a href=\"https://github.com/PySCeS/pysces/issues\">issue</a>.</p>\n\n<p>General information on PySCeS can be found on the&nbsp;<a href=\"https://pysces.github.io/\">website</a>&nbsp;and extensive documentation on installing, configuring and using PySCeS is available on&nbsp;<a href=\"https://pyscesdocs.readthedocs.io/en/latest/\">pyscesdocs.readthedocs.io</a>.</p>",
     "license": "BSD-3-Clause",
     "notes": "If you use this software, please cite it using the information provided in this metadata.",
-    "publication_date": "2024-02-14",
+    "publication_date": "2024-05-10",
     "title": "The Python Simulator for Cellular Systems: PySCeS",
     "upload_type": "software",
-    "version": "1.2.0"
+    "version": "1.2.1"
 }
```

### Comparing `pysces-1.2.0/ADDITIONAL_LICENCES.md` & `pysces-1.2.1/ADDITIONAL_LICENCES.md`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/CHANGES.md` & `pysces-1.2.1/CHANGES.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,201 +1,257 @@
 # PySCeS changes (per GitHub release)
 
+## PySCeS release 1.2.1 (May 2024)
+
+We are pleased to announce the release of the Python Simulator for Cellular Systems:
+PySCeS (https://pysces.github.io/) version 1.2.1. This is a bugfix release.
+
+### Fixes
+
+- Fixed a bug in model evaluation where a model has events and assignment rules, and the
+  assignment rule contains a variable name and a parameter with the variable a
+  substring match of the parameter (e.g. `E1` and `E1tot`). Previously, this led to
+  garbage code during string replacements.
+- Cleaned up various error messages.
+
+## PySCeS release 1.2.0 (Feb 2024)
+
+We are pleased to announce the release of the Python Simulator for Cellular Systems:
+PySCeS (https://pysces.github.io/) version 1.2.0. This is the first release in the 1.2
+series and contains some new features and various bug fixes.
+
+### New features
+
+There have been major changes in the build system for PySCeS. This release
+implements [meson-python](https://meson-python.readthedocs.io/),
+a [PEP 517](https://peps.python.org/pep-0517/) compliant Python build backend that
+is suitable for building C and Fortran extension modules by implementing
+the [meson build system](https://mesonbuild.com/). There is no more `setup.py` and
+project build options and metadata are now in `pyproject.toml`.
+
+The main **motivation** for this has been support for Python 3.12, which deprecated
+the use of `distutils`, and consequently `numpy` dropped `numpy.distutils`. The
+previous build system had relied on `numpy.distutils` for building Fortran extension
+modules, which would no longer work on Python 3.12. In the mean time, `scipy`, `numpy`,
+as well as a number of other packages in the scientific Python ecosystem have moved
+their build systems to `meson-python`. This version thus brings PySCeS in line with
+the other packages.
+
+In addition, **binary wheels for macOS on Apple silicon** (*arm64*) are provided
+for the first time (Python 3.11 and 3.12).
+
+### What has changed?
+
+- From a regular user perspective, not much. Installation is still via `pip` or `conda`.
+
+- From a developer perspective: there is no longer a `setup.py`. Metadata has been
+  migrated to `pyproject.toml`. Build settings are spread between `pyproject.toml` and
+  various `meson.build` files. The build is straightforward using one of:
+  ```bash
+  $ pip wheel -w dist .
+  $ python -m build .
+  ```
+  as long as the relevant compiler toolchain is installed (gcc and gfortran on Linux and
+  macOS, RTools on Windows). Installation can be done with
+  ```bash
+  $ pip install .
+           or
+  $ pip install --no-build-isolation -e .          (for an editable install)
+  ```
+  Refer to [INSTALL.md](https://github.com/PySCeS/pysces/blob/main/INSTALL.md).
+
+- `Numpy` version >=1.26 is required for the build, as older versions of `f2py` (which
+  is distributed with `numpy`) are not compatible. At runtime, any `numpy` version >
+  =1.23 is supported, older versions don't work due to ABI incompatibility.
+- Binaries (wheels) are distributed for Python versions 3.9-3.12. Python 3.8 support is
+  dropped as the latest `numpy` and `scipy` versions also no longer support it.
+- Documentation has been updated to reflect these changes.
+
+### Bug fixes
+
+- Fixed a bug with assignment rule evaluation when one species was an exact substring of
+  another species.
+- Use vectorised functions `numpy.log`, `numpy.log10`, `numpy.exp` instead of
+  their `math.*` counterparts to support their application to arrays in e.g. assignment
+  rules.
+- Removed a bunch of deprecated `scipy.*` functions that have moved to the `numpy.*`
+  namespace.
+- Cleaned up unused imports.
+
 ## PySCeS release 1.1.1 (Jul 2023)
 
-We are pleased to announce the release of the Python Simulator for Cellular Systems: 
-PySCeS (https://pysces.github.io/) version 1.1.1. This is the first release in the 1.1 
+We are pleased to announce the release of the Python Simulator for Cellular Systems:
+PySCeS (https://pysces.github.io/) version 1.1.1. This is the first release in the 1.1
 series and contains some new features and various bug fixes.
 
 ### New features
 
-- When used in a notebook environment, the `ipympl` backend for matplotlib is now enabled if installed. This allows use in JupyterLab (as opposed to classic notebook). If `ipympl` is not installed, fallback is to the standard `nbAgg`, which is part of matplotlib.
-- Simulation results (`mod.sim` object) can now be returned as a pandas DataFrame if pandas is installed, otherwise a numpy recarray is returned as before. This option is configurable with `custom_datatype = pandas` in the user and system configuration files (see https://pyscesdocs.readthedocs.io/en/latest/userguide_doc.html#configuration), and can be enabled or disabled per session or per model:
+- When used in a notebook environment, the `ipympl` backend for matplotlib is now
+  enabled if installed. This allows use in JupyterLab (as opposed to classic notebook).
+  If `ipympl` is not installed, fallback is to the standard `nbAgg`, which is part of
+  matplotlib.
+- Simulation results (`mod.sim` object) can now be returned as a pandas DataFrame if
+  pandas is installed, otherwise a numpy recarray is returned as before. This option is
+  configurable with `custom_datatype = pandas` in the user and system configuration
+  files (
+  see https://pyscesdocs.readthedocs.io/en/latest/userguide_doc.html#configuration), and
+  can be enabled or disabled per session or per model:
   ```python
   pysces.enablePandas()
   pysces.enablePandas(False)
   mod.enableDataPandas()
   mod.enableDataPandas(False)
   ```
 
 ### Bug fixes
 
-- Fixed a bug in simulations with `RateRules` using Assimulo, where a wrong solver variable was being assigned internally.
+- Fixed a bug in simulations with `RateRules` using Assimulo, where a wrong solver
+  variable was being assigned internally.
 - Fixed SBML export when assignment rules were evaluating reaction rates.
-- Enabled assignment rules (forcing functions) to track parameter changes when using CVODE. This is needed in case events change parameters during the course of the simulation.
-
-README: https://github.com/PySCeS/pysces/blob/master/README.md
-
-DOCUMENTATION: https://pyscesdocs.readthedocs.io/en/latest/
+- Enabled assignment rules (forcing functions) to track parameter changes when using
+  CVODE. This is needed in case events change parameters during the course of the
+  simulation.
 
 ## PySCeS release 1.1.0 (Apr 2023)
 
-We are pleased to announce a new minor release (version 1.1.0) of the Python 
-Simulator for Cellular Systems: PySCeS (https://pysces.github.io/). This is the 
+We are pleased to announce a new minor release (version 1.1.0) of the Python
+Simulator for Cellular Systems: PySCeS (https://pysces.github.io/). This is the
 first release in the 1.1 series.
 
 ### What's new?
 
-The most significant new feature in Version 1.1 is a major upgrade in the way 
-**PySCeS handles events in simulations**. The definition of events follows the 
-framework described in the SBML Level 3 Version 2 specification, thus making the 
-event handling SBML-compliant. Specifically, event **persistence** (for events with 
-a delay) is now handled correctly, and simultaneous events can be executed 
+The most significant new feature in Version 1.1 is a major upgrade in the way
+**PySCeS handles events in simulations**. The definition of events follows the
+framework described in the SBML Level 3 Version 2 specification, thus making the
+event handling SBML-compliant. Specifically, event **persistence** (for events with
+a delay) is now handled correctly, and simultaneous events can be executed
 according to their assigned **priorities**.
 
 The new **event specification** in the PySCeS input file reads:
+
 ```
 Event: <name>, <trigger>, <optional_kwargs> { <assignments> }
 ```
 
-To achieve this, three new optional keyword arguments have been added as a 
-comma-separated list to the event specification. The general syntax for these 
+To achieve this, three new optional keyword arguments have been added as a
+comma-separated list to the event specification. The general syntax for these
 arguments is `<attribute>=<value>`. The keywords are:
 
-- *delay* (float): specifies a delay between when the trigger is fired (and the 
-  assignments are evaluated) and the eventual assignment to the model. If this 
+- *delay* (float): specifies a delay between when the trigger is fired (and the
+  assignments are evaluated) and the eventual assignment to the model. If this
   keyword is not specified, a value of `0.0` is assumed.
-- *priority* (integer or None): specifies a priority for events that trigger at the 
-  same simulation time. Events with a higher priority are executed before those 
-  with a lower priority, while events without a priority (`None`) are executed in 
-  random positions in the sequence. If this keyword is not specified, a value of 
+- *priority* (integer or None): specifies a priority for events that trigger at the
+  same simulation time. Events with a higher priority are executed before those
+  with a lower priority, while events without a priority (`None`) are executed in
+  random positions in the sequence. If this keyword is not specified, a value of
   `None` is assumed.
-- *persistent* (boolean): is only relevant to events with a delay, where the 
-  situation may occur that the trigger condition no longer holds by the time the 
-  delay in the simulation has passed. The persistent attribute specifies how to 
-  deal with this situation: if `True`, the event executes nevertheless; if `False`, 
-  the event does not execute if the trigger condition is no longer valid. If the 
+- *persistent* (boolean): is only relevant to events with a delay, where the
+  situation may occur that the trigger condition no longer holds by the time the
+  delay in the simulation has passed. The persistent attribute specifies how to
+  deal with this situation: if `True`, the event executes nevertheless; if `False`,
+  the event does not execute if the trigger condition is no longer valid. If the
   keyword is not specified, a default of `True` is assumed.
 
-The following event illustrates the use of a delay of ten time units with a 
+The following event illustrates the use of a delay of ten time units with a
 non-persistent trigger and a priority of 3:
+
 ```
 Event: event2, geq(_TIME_, 15.0), delay=10.0, persistent=False, priority=3 {
 V3 = V3*vfact2
 }
 ```
+
 The legacy event syntax is still supported.
 
 ### Other changes
 
-- A new setting has been added to the settings dictionary of the `PysMod` class 
+- A new setting has been added to the settings dictionary of the `PysMod` class
   with the following default:    
   `mod.__settings__["cvode_access_solver"] = True`    
-  This specifies if the Assimulo solver object is available from within the 
-  `PysMod` instance to make low-level changes to the integration algorithm. The 
-  current default emulates previous behaviour, but the setting can be changed to 
-  `False`, which facilitates serialization of the `PysMod` class in e.g. parallel 
-  computations. Previously, the attached Assimulo solver object would prevent 
+  This specifies if the Assimulo solver object is available from within the
+  `PysMod` instance to make low-level changes to the integration algorithm. The
+  current default emulates previous behaviour, but the setting can be changed to
+  `False`, which facilitates serialization of the `PysMod` class in e.g. parallel
+  computations. Previously, the attached Assimulo solver object would prevent
   serialization. Thanks @c-barry
 - Documentation has been updated to reflect the changes to the event syntax.
-- Various bug fixes, including dealing with deprecations for Numpy 1.24.x 
+- Various bug fixes, including dealing with deprecations for Numpy 1.24.x
   compatibility.
 
-README: https://github.com/PySCeS/pysces/blob/master/README.md
-
-DOCUMENTATION: https://pyscesdocs.readthedocs.io/en/latest/
-
-© Brett Olivier and Johann Rohwer, April 2023.
-
-
 ## PySCeS release 1.0.3 (Sep 2022)
 
-We are pleased to announce the release of the Python Simulator for Cellular 
-Systems: PySCeS (https://pysces.github.io/) version 1.0.3. This is the third 
+We are pleased to announce the release of the Python Simulator for Cellular
+Systems: PySCeS (https://pysces.github.io/) version 1.0.3. This is the third
 release in the 1.0 series.
 
 ### What's new?
-- The build-system has been adapted to make use of `scikit-build`. This gets rid of 
-the `distutils` and `numpy.distutils` dependencies, which are deprecated and will 
-be removed with the release of Python 3.12.
+
+- The build-system has been adapted to make use of `scikit-build`. This gets rid of
+  the `distutils` and `numpy.distutils` dependencies, which are deprecated and will
+  be removed with the release of Python 3.12.
 
 ### Bug Fixes:
+
 - Fixed CVODE defaults and set default tolerances to more sane levels
 - Fixed string replacement in parsing and construction of `PieceWise` functions
 
-README: https://github.com/PySCeS/pysces/blob/master/README.md
-
-DOCUMENTATION: https://pyscesdocs.readthedocs.io/en/latest/
-
-&copy; Brett Olivier and Johann Rohwer, September 2022.
-
-
 ## PySCeS release 1.0.2 (May 2022)
 
-We are pleased to announce the release of the Python Simulator for Cellular Systems: 
-PySCeS (https://pysces.github.io/) version 1.0.2. 
+We are pleased to announce the release of the Python Simulator for Cellular Systems:
+PySCeS (https://pysces.github.io/) version 1.0.2.
 This is the second bug-fix release in the 1.0 series.
 
 ### Fixes:
 
 - Fixed a number of bugs with `RateRule` execution with CVODE
-- Reintroduced the functionality to track additional items such as Assignment Rules 
+- Reintroduced the functionality to track additional items such as Assignment Rules
   during a simulation with CVODE
-- The Assimulo `CVODE` implementation has been updated, and legacy PySUNDIALS CVODE 
+- The Assimulo `CVODE` implementation has been updated, and legacy PySUNDIALS CVODE
   code removed
-- The `RateRule` and `AssignmentRule` implementations have been checked against the 
+- The `RateRule` and `AssignmentRule` implementations have been checked against the
   SBML Test Suite
 
-README: https://github.com/PySCeS/pysces/blob/master/README.md
-
-DOCUMENTATION: https://pyscesdocs.readthedocs.io/en/latest/
-
-&copy; Brett Olivier and Johann Rohwer, May 2022.
-
 ## PySCeS release 1.0.1 (Feb 2022)
 
-We are pleased to announce the release of the Python Simulator for Cellular Systems: 
-PySCeS (https://pysces.github.io/) version 1.0.1. This is the first bug-fix release 
+We are pleased to announce the release of the Python Simulator for Cellular Systems:
+PySCeS (https://pysces.github.io/) version 1.0.1. This is the first bug-fix release
 in the 1.0 series.
 
 ### Fixes:
 
 - Fixed references to numpy/scipy
 - Fixed a bug in `mod.Simulate(userinit=1)` with CVODE
-- Fixed bug where the maximal number of steps in LSODA would not be honoured from the 
+- Fixed bug where the maximal number of steps in LSODA would not be honoured from the
   `mod.__settings__["lsoda_mxstep"]` dictionary entry
 - General cleanup of license files, version files, and the way requirements are handled
 
-README: https://github.com/PySCeS/pysces/blob/master/README.md
-
-DOCUMENTATION: https://pyscesdocs.readthedocs.io/en/latest/
-
-&copy; Brett Olivier and Johann Rohwer, February 2022.
-
 ## PySCeS release 1.0.0 (Sep 2021)
 
-We are pleased to announce the release of the Python Simulator for Cellular 
+We are pleased to announce the release of the Python Simulator for Cellular
 Systems: PySCeS (https://pysces.github.io/) version 1.0.0.
 
 **What's new in this release:**
 
-- Re-introduced support for CVODE as integrator under Python 3 (via Assimulo), 
+- Re-introduced support for CVODE as integrator under Python 3 (via Assimulo),
   which brings back support of events in models
 - Improved import and export of SBML
 - Automatic installation of optional dependencies with `pip install "pysces
   [optional_dep]"`
 - Extensive update of documentation
 - Numerous bug fixes
 
-**README:** https://github.com/PySCeS/pysces/blob/master/README.md
-
-**DOCUMENTATION:** https://pyscesdocs.readthedocs.io/en/latest/
-
-&copy; Brett Olivier and Johann Rohwer, September 2021.
-
-
 ## PySCeS release 0.9.8 (May 2020)
 
 We are pleased to announce the release of the Python Simulator for Cellular Systems:
 PySCeS (http://pysces.sourceforge.net) version 0.9.8
 
 **What's new in this release:**
 
 * The main change from a user perspective is that the default model directory and output
-  directory on Windows have moved to `%USERPROFILE%\Pysces` and subfolders 
+  directory on Windows have moved to `%USERPROFILE%\Pysces` and subfolders
   (e.g. `C:\Users\<username>\Pysces`). These folders are created by default on a fresh
   install. The previous default location was `C:\Pysces`. This change brings the Windows
   version in line with the Linux and macOS versions, and moreover allows multiple users
   to maintain their individual PySCeS configurations and model files on the same Windows
   machine.
 
 * If you are **upgrading** from a previous version: For backward compatibility, the
@@ -269,11 +325,11 @@
 
 This release contains new functionality (response coefficients of moiety conserved
 cycles), bugfixes (assignment rules) and updates (SED-ML and COMBINE archive export).
 
 ## PySCeS releases 2004 - 2016
 
 These releases are available for download
-from [SourceForge] (https://sourceforge.net/projects/pysces/files/pysces)
+from [SourceForge](https://sourceforge.net/projects/pysces/files/pysces)
 
-© Brett G. Olivier & Johann M. Rohwer, August 2021
+© Brett G. Olivier & Johann M. Rohwer, 2004-2024
```

### Comparing `pysces-1.2.0/CITATION.cff` & `pysces-1.2.1/CITATION.cff`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # YAML 1.2
 ---
-cff-version: "1.2.0"
+cff-version: "1.2.1"
 message: "If you use this software, please cite it using the information provided in this metadata."
 authors:
   -
     given-names: Brett
     family-names: Olivier
     affiliation: "Vrije Universiteit Amsterdam"
     orcid: "https://orcid.org/0000-0002-5293-5321"
   -
     given-names: Johann
     family-names: Rohwer
     affiliation: "Stellenbosch University"
     orcid: "https://orcid.org/0000-0001-6288-8904"
 title: "The Python Simulator for Cellular Systems: PySCeS"
-version: "1.2.0"
-repository-code: "https://github.com/PySCeS/pysces/tree/1.2.0"
-date-released: 2024-02-14
+version: "1.2.1"
+repository-code: "https://github.com/PySCeS/pysces/tree/1.2.1"
+date-released: 2024-05-10
 doi: "10.5281/zenodo.2600905"
 license: "BSD-3-Clause"
 url: https://pysces.github.io
 abstract: "Computer modelling has become an integral tool in the analysis and understanding
 of the reaction networks that underlie cellular processes. PySCeS, first released in 2003,
 is extremely flexible, user-extendable, open source, software actively used and developed
 by a community of researchers and developers."
```

### Comparing `pysces-1.2.0/CONTRIBUTORS.md` & `pysces-1.2.1/CONTRIBUTORS.md`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/DESCRIPTION.md` & `pysces-1.2.1/DESCRIPTION.md`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/INSTALL.md` & `pysces-1.2.1/INSTALL.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 # Installing PySCeS
 
 Binary install packages for all three OSs and recent Python versions are 
 provided. Anaconda packages are available for 64-bit Windows and Linux, as well as 
-macOS *x86_64* architecture. Apple Silicon (*arm64*) macOS users should install with 
-`pip` (see below). Anaconda users can conveniently install PySCeS with:
+macOS *x86_64* and Apple Silicon (*arm64*) architectures. Anaconda users can 
+conveniently install PySCeS with:
 
 ```bash
 $ conda install -c conda-forge -c pysces pysces
 ```  
 
 Any dependencies will be installed automatically, including the optional dependencies 
-*Assimulo*, *ipyparallel* and *libSBML*. 
+*Assimulo*, *ipyparallel* and *libSBML*.
+> **NOTE:** Anaconda packages are only provided for Python versions 3.9-3.11. The 
+> reason is that Assimulo has not been ported to Python 3.12 and still depends on 
+> `numpy.distutils`. As soon as this has happened, PySCeS Anaconda packages for 3.12 
+> will be built.
 
 Alternatively, you can use *pip* to
-install PySCeS from PyPI. Core dependencies will be installed automatically. Wheels 
-are available for 64-bit Windows and Linux, as well as macOS architectures *x86_64* and 
-*arm64* (starting from PySCeS version 1.2.0).
+install PySCeS from PyPI. Core dependencies will be installed automatically. Wheels
+are available for 64-bit Windows and Linux, as well as macOS architectures *x86_64* and
+*arm64* (starting from PySCeS version 1.2.0, supporting Python 3.11 and 3.12).
 
 ```bash
 $ pip install pysces
 ```
 
 To install the optional dependences:
```

### Comparing `pysces-1.2.0/LATEST.md` & `pysces-1.2.1/LATEST.md`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/LICENSE.txt` & `pysces-1.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/README.md` & `pysces-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/config.py` & `pysces-1.2.1/config.py`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/devtest/models/BIOMD0000000012_url.xml` & `pysces-1.2.1/devtest/models/BIOMD0000000012_url.xml`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/devtest/models/BIOMD0000000126.xml` & `pysces-1.2.1/devtest/models/BIOMD0000000126.xml`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/devtest/models/BIOMD0000000860.xml` & `pysces-1.2.1/devtest/models/BIOMD0000000860.xml`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/devtest/models/rohwer_sucrose2.psc` & `pysces-1.2.1/devtest/models/rohwer_sucrose2.psc`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/devtest/out/BIOMD0000000012_url.xml/BIOMD0000000012_url.xml-ref.png` & `pysces-1.2.1/devtest/out/BIOMD0000000012_url.xml/BIOMD0000000012_url.xml-ref.png`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/devtest/out/BIOMD0000000126.xml/BIOMD0000000126.xml-ref.png` & `pysces-1.2.1/devtest/out/BIOMD0000000126.xml/BIOMD0000000126.xml-ref.png`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/devtest/out/BIOMD0000000860.xml/BIOMD0000000860.xml-ref.png` & `pysces-1.2.1/devtest/out/BIOMD0000000860.xml/BIOMD0000000860.xml-ref.png`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/devtest/out/rohwer_sucrose2/rohwer_sucrose2_fluxes-ref.png` & `pysces-1.2.1/devtest/out/rohwer_sucrose2/rohwer_sucrose2_fluxes-ref.png`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/devtest/out/rohwer_sucrose2/rohwer_sucrose2_mca-ref.png` & `pysces-1.2.1/devtest/out/rohwer_sucrose2/rohwer_sucrose2_mca-ref.png`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/devtest/out/rohwer_sucrose2/rohwer_sucrose2_species-ref.png` & `pysces-1.2.1/devtest/out/rohwer_sucrose2/rohwer_sucrose2_species-ref.png`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/devtest/ref_data/BIOMD0000000012_url.xml/simdata.pkl` & `pysces-1.2.1/devtest/ref_data/BIOMD0000000012_url.xml/simdata.pkl`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/devtest/ref_data/BIOMD0000000126.xml/simdata.pkl` & `pysces-1.2.1/devtest/ref_data/BIOMD0000000126.xml/simdata.pkl`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/devtest/ref_data/BIOMD0000000860.xml/simdata.pkl` & `pysces-1.2.1/devtest/ref_data/BIOMD0000000860.xml/simdata.pkl`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/devtest/ref_data/rohwer_sucrose2/mcadata.pkl` & `pysces-1.2.1/devtest/ref_data/rohwer_sucrose2/mcadata.pkl`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/devtest/ref_data/rohwer_sucrose2/scandata.pkl` & `pysces-1.2.1/devtest/ref_data/rohwer_sucrose2/scandata.pkl`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/devtest/test_sbml_log_ln.py` & `pysces-1.2.1/devtest/test_sbml_log_ln.py`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/devtest/test_sbml_rules_functions.py` & `pysces-1.2.1/devtest/test_sbml_rules_functions.py`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/devtest/test_sbml_time_events.py` & `pysces-1.2.1/devtest/test_sbml_time_events.py`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/devtest/test_state_mca_scans.py` & `pysces-1.2.1/devtest/test_state_mca_scans.py`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/meson.build` & `pysces-1.2.1/meson.build`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/packaging/conda-scripts/README.md` & `pysces-1.2.1/packaging/conda-scripts/README.md`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/packaging/conda-scripts/VS2019_gfortran8_build.md` & `pysces-1.2.1/packaging/conda-scripts/VS2019_gfortran8_build.md`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/packaging/conda-scripts/build_conda_macos.sh` & `pysces-1.2.1/packaging/conda-scripts/build_conda_macos.sh`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/packaging/conda-scripts/build_conda_windows.bat` & `pysces-1.2.1/packaging/conda-scripts/build_conda_windows.bat`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/packaging/conda-scripts/conda_build.txt` & `pysces-1.2.1/packaging/conda-scripts/conda_build.txt`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/packaging/conda-unix/meta.yaml` & `pysces-1.2.1/packaging/conda-unix/meta.yaml`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/packaging/conda-win/meta.yaml` & `pysces-1.2.1/packaging/conda-win/meta.yaml`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/packaging/many_linux/README.md` & `pysces-1.2.1/packaging/many_linux/README.md`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/packaging/many_linux/build_script.sh` & `pysces-1.2.1/packaging/many_linux/build_script.sh`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/packaging/wheels_win/Instructions.txt` & `pysces-1.2.1/packaging/wheels_win/Instructions.txt`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/packaging/wheels_win/VS2017_gfortran8_build.md` & `pysces-1.2.1/packaging/wheels_win/VS2017_gfortran8_build.md`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/packaging/windows_libs/dlltool.exe` & `pysces-1.2.1/packaging/windows_libs/dlltool.exe`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/packaging/windows_libs/gendef.exe` & `pysces-1.2.1/packaging/windows_libs/gendef.exe`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pyproject.toml` & `pysces-1.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/PyscesConfig.py` & `pysces-1.2.1/pysces/PyscesConfig.py`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/PyscesContrib.py` & `pysces-1.2.1/pysces/PyscesContrib.py`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/PyscesContribUser.py` & `pysces-1.2.1/pysces/PyscesContribUser.py`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/PyscesInterfaces.py` & `pysces-1.2.1/pysces/PyscesInterfaces.py`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/PyscesJWSParse.py` & `pysces-1.2.1/pysces/PyscesJWSParse.py`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/PyscesLink.py` & `pysces-1.2.1/pysces/PyscesLink.py`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/PyscesMiniModel.py` & `pysces-1.2.1/pysces/PyscesMiniModel.py`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/PyscesModel.py` & `pysces-1.2.1/pysces/PyscesModel.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
             -----------
 
             This module contains the core PySCeS classes which
             create the model and associated data objects
 
             '''
 import os, copy, time
+import re
 import pickle
 import warnings
 try:
     input = raw_input  # Py2 compatibility
 except NameError:
     pass
 import numpy
@@ -4810,22 +4811,29 @@
         rule['data_sim_string'] = rule['code_string']
         for s in sorted(rule['symbols'], key=len, reverse=True):
             if (
                 s in self.__reactions__
                 or s in self.__rules__
                 or s in self.__species__
             ):
-                # catch any _init so it doesn't get replaced
-                replacements.append((s + '_init', '_zzzz_'))
+                # deal with substrings in symbols
+                partialmatches = []
+                for sym in rule['symbols']:
+                    if not re.fullmatch(s, sym) and re.search(s, sym):
+                        partialmatches.append(sym)
+                # catch any partial matches so they don't get replaced
+                for e in enumerate(partialmatches):
+                    replacements.append((e[1], f'_zzzz_{e[0]}_z'))
                 # replace symbol to get sim data
                 replacements.append(
-                    ('self.' + s, 'self.data_sim.getSimData("' + s + '")[p:q,1]')
+                    (f'self.{s}', f'self.data_sim.getSimData("{s}")[p:q,1]')
                 )
-                # revert the _init
-                replacements.append(('_zzzz_', s + '_init'))
+                # revert the partial match symbol
+                for e in enumerate(partialmatches):
+                    replacements.append((f'_zzzz_{e[0]}_z', e[1]))
 
         for old, new in replacements:
             rule['data_sim_string'] = rule['data_sim_string'].replace(old, new)
 
     @property
     def sim(self):
         if self._sim is None and self.data_sim is not None:
```

### Comparing `pysces-1.2.0/pysces/PyscesModelMap.py` & `pysces-1.2.1/pysces/PyscesModelMap.py`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/PyscesParScan.py` & `pysces-1.2.1/pysces/PyscesParScan.py`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/PyscesParse.py` & `pysces-1.2.1/pysces/PyscesParse.py`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/PyscesPlot.py` & `pysces-1.2.1/pysces/PyscesPlot.py`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/PyscesPlot2.py` & `pysces-1.2.1/pysces/PyscesPlot2.py`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/PyscesRandom.py` & `pysces-1.2.1/pysces/PyscesRandom.py`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/PyscesSBML.py` & `pysces-1.2.1/pysces/PyscesSBML.py`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/PyscesSED.py` & `pysces-1.2.1/pysces/PyscesSED.py`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/PyscesScan.py` & `pysces-1.2.1/pysces/PyscesScan.py`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/PyscesStoich.py` & `pysces-1.2.1/pysces/PyscesStoich.py`

 * *Files 1% similar despite different names*

```diff
@@ -749,27 +749,20 @@
         ##  if self.array_kind[t] == 1:
         ##  getrf = scipy.linalg.clapack.zgetrf #scipy clapack (ATLAS) 20030605
         ##  else:
         ##  getrf = scipy.linalg.clapack.dgetrf #scipy clapack (ATLAS) 20030605
         ##  except Exception, e:
         ##  print "CLAPACK error", e
 
-        if a.shape[0] >= 500 or a.shape[1] >= 500:
-            print('\nMatrix {} using SciPy version: {} on {}'.format(a.shape, scipy.__version__, os.sys.platform))
-            print('Error 766 error detector: only report this if your Python crashes now ...')
-
         if Using_FLAPACK == 1:
             ##  results = getrf(numpy.transpose(a)) # brett 20041226
             results = getrf(a)  # brett 201106
 
         results = list(results)
 
-        if a.shape[0] >= 500 or a.shape[1] >= 500:
-            print('766 error did not occur please continue as normal {} ...'.format(a.shape))
-
         if results[2] < 0:
             print('Argument ', results['info'], ' had an illegal value')
             raise LinAlgError
         elif results[2] > 0:
             pass
 
         if Using_FLAPACK == 1:
```

### Comparing `pysces-1.2.0/pysces/PyscesTest.py` & `pysces-1.2.1/pysces/PyscesTest.py`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/PyscesUtils.py` & `pysces-1.2.1/pysces/PyscesUtils.py`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/PyscesWeb.py` & `pysces-1.2.1/pysces/PyscesWeb.py`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/RateChar.py` & `pysces-1.2.1/pysces/RateChar.py`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/__init__.py` & `pysces-1.2.1/pysces/__init__.py`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/_multicorescan.py` & `pysces-1.2.1/pysces/_multicorescan.py`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/contrib/__init__.py` & `pysces-1.2.1/pysces/contrib/__init__.py`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/contrib/demo/demotest.py` & `pysces-1.2.1/pysces/contrib/demo/demotest.py`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/contrib/sbw/sbw_func.py` & `pysces-1.2.1/pysces/contrib/sbw/sbw_func.py`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/contrib/visualise/VisualiseClasses.py` & `pysces-1.2.1/pysces/contrib/visualise/VisualiseClasses.py`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/contrib/visualise/VisualiseNodeClasses.py` & `pysces-1.2.1/pysces/contrib/visualise/VisualiseNodeClasses.py`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/contrib/visualise/VisualiseSBML.py` & `pysces-1.2.1/pysces/contrib/visualise/VisualiseSBML.py`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/core2/InfixParser.py` & `pysces-1.2.1/pysces/core2/InfixParser.py`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/core2/PyscesCore2.py` & `pysces-1.2.1/pysces/core2/PyscesCore2.py`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/core2/PyscesCore2Interfaces.py` & `pysces-1.2.1/pysces/core2/PyscesCore2Interfaces.py`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/core2/PyscesCore2Modules.py` & `pysces-1.2.1/pysces/core2/PyscesCore2Modules.py`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/core2/__init__.py` & `pysces-1.2.1/pysces/core2/__init__.py`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/core2/lex.py` & `pysces-1.2.1/pysces/core2/lex.py`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/core2/yacc.py` & `pysces-1.2.1/pysces/core2/yacc.py`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/docs/HISTORY.txt` & `pysces-1.2.1/pysces/docs/HISTORY.txt`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/docs/userguide.pdf` & `pysces-1.2.1/pysces/docs/userguide.pdf`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/examples/benchmark.ipy` & `pysces-1.2.1/pysces/examples/benchmark.ipy`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/examples/parallelscan.ipy` & `pysces-1.2.1/pysces/examples/parallelscan.ipy`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/examples/pysces_stochpy.py` & `pysces-1.2.1/pysces/examples/pysces_stochpy.py`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/examples/testRunScatter.py` & `pysces-1.2.1/pysces/examples/testRunScatter.py`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/examples/testinvalidstate.py` & `pysces-1.2.1/pysces/examples/testinvalidstate.py`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/examples/testparscanner.py` & `pysces-1.2.1/pysces/examples/testparscanner.py`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/examples/testratechar.py` & `pysces-1.2.1/pysces/examples/testratechar.py`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/kraken/Kraken.py` & `pysces-1.2.1/pysces/kraken/Kraken.py`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/kraken/KrakenDataTools.py` & `pysces-1.2.1/pysces/kraken/KrakenDataTools.py`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/kraken/KrakenNET.py` & `pysces-1.2.1/pysces/kraken/KrakenNET.py`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/kraken/KrakenServer.py` & `pysces-1.2.1/pysces/kraken/KrakenServer.py`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/kraken/__init__.py` & `pysces-1.2.1/pysces/kraken/__init__.py`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/kraken/controllers/kraken_continuation.py` & `pysces-1.2.1/pysces/kraken/controllers/kraken_continuation.py`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/kraken/controllers/kraken_continuation_eigen.py` & `pysces-1.2.1/pysces/kraken/controllers/kraken_continuation_eigen.py`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/kraken/controllers/kraken_continuation_eigen2.py` & `pysces-1.2.1/pysces/kraken/controllers/kraken_continuation_eigen2.py`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/kraken/controllers/kraken_intersect.py` & `pysces-1.2.1/pysces/kraken/controllers/kraken_intersect.py`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/kraken/controllers/kraken_scanner2.py` & `pysces-1.2.1/pysces/kraken/controllers/kraken_scanner2.py`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/kraken/startup.py` & `pysces-1.2.1/pysces/kraken/startup.py`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/lib/FirstDerivatives.py` & `pysces-1.2.1/pysces/lib/FirstDerivatives.py`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/lib/__init__.py` & `pysces-1.2.1/pysces/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/lib/lex.py` & `pysces-1.2.1/pysces/lib/lex.py`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/lib/miriamids.py` & `pysces-1.2.1/pysces/lib/miriamids.py`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/lib/pyparsing.py` & `pysces-1.2.1/pysces/lib/pyparsing.py`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/lib/yacc.py` & `pysces-1.2.1/pysces/lib/yacc.py`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/meson.build` & `pysces-1.2.1/pysces/meson.build`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/metatool/__init__.py` & `pysces-1.2.1/pysces/metatool/__init__.py`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/nleq2/4.2/nleq2.f` & `pysces-1.2.1/pysces/nleq2/4.2/nleq2.f`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/nleq2/4.2/nleq2.pyf` & `pysces-1.2.1/pysces/nleq2/4.2/nleq2.pyf`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/nleq2/4.2/nleq2.tar.gz` & `pysces-1.2.1/pysces/nleq2/4.2/nleq2.tar.gz`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/nleq2/4.2/nleq2_big.f` & `pysces-1.2.1/pysces/nleq2/4.2/nleq2_big.f`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/nleq2/4.2/nleq2_gfortran.f` & `pysces-1.2.1/pysces/nleq2/4.2/nleq2_gfortran.f`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/nleq2/4.2/nleq2_little.f` & `pysces-1.2.1/pysces/nleq2/4.2/nleq2_little.f`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/nleq2/4.2/nleq2_little_pre-gcc41.f` & `pysces-1.2.1/pysces/nleq2/4.2/nleq2_little_pre-gcc41.f`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/nleq2/__init__.py` & `pysces-1.2.1/pysces/nleq2/__init__.py`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/nleq2/linalg_nleq2.f` & `pysces-1.2.1/pysces/nleq2/linalg_nleq2.f`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/nleq2/meson.build` & `pysces-1.2.1/pysces/nleq2/meson.build`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/nleq2/nleq2-4.3.tar.gz` & `pysces-1.2.1/pysces/nleq2/nleq2-4.3.tar.gz`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/nleq2/nleq2.f` & `pysces-1.2.1/pysces/nleq2/nleq2.f`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/nleq2/nleq2.pyf` & `pysces-1.2.1/pysces/nleq2/nleq2.pyf`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/nleq2/nleq2_readme.txt` & `pysces-1.2.1/pysces/nleq2/nleq2_readme.txt`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/nleq2/readme.txt` & `pysces-1.2.1/pysces/nleq2/readme.txt`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/nleq2/wnorm.f` & `pysces-1.2.1/pysces/nleq2/wnorm.f`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/nleq2/zibconst.f` & `pysces-1.2.1/pysces/nleq2/zibconst.f`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/nleq2/zibmon.f` & `pysces-1.2.1/pysces/nleq2/zibmon.f`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/nleq2/zibsec.f` & `pysces-1.2.1/pysces/nleq2/zibsec.f`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/pitcon/dpcon61.f` & `pysces-1.2.1/pysces/pitcon/dpcon61.f`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/pitcon/dpcon61w.f` & `pysces-1.2.1/pysces/pitcon/dpcon61w.f`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/pitcon/meson.build` & `pysces-1.2.1/pysces/pitcon/meson.build`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/pitcon/pcon61subd.f` & `pysces-1.2.1/pysces/pitcon/pcon61subd.f`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/pitcon/pitcon.pyf` & `pysces-1.2.1/pysces/pitcon/pitcon.pyf`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/pitcon/readme.txt` & `pysces-1.2.1/pysces/pitcon/readme.txt`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/pscmodels/Burstmodel.psc` & `pysces-1.2.1/pysces/pscmodels/Burstmodel.psc`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/pscmodels/isola2a.psc` & `pysces-1.2.1/pysces/pscmodels/isola2a.psc`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/pscmodels/lin5_hill.psc` & `pysces-1.2.1/pysces/pscmodels/lin5_hill.psc`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/pscmodels/pysces_test_branch1.psc` & `pysces-1.2.1/pysces/pscmodels/pysces_test_branch1.psc`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/pscmodels/pysces_test_moiety1.psc` & `pysces-1.2.1/pysces/pscmodels/pysces_test_moiety1.psc`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/pscmodels/pysces_test_pitcon.psc` & `pysces-1.2.1/pysces/pscmodels/pysces_test_pitcon.psc`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/sandbox/Intersect.py` & `pysces-1.2.1/pysces/sandbox/Intersect.py`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/pysces/tests/__init__.py` & `pysces-1.2.1/pysces/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pysces-1.2.0/PKG-INFO` & `pysces-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pysces
-Version: 1.2.0
+Version: 1.2.1
 Summary: The Python Simulator for Cellular Systems - simulation and analysis tools for modelling biological systems
-Keywords: computational systems biology modelling simulation systems biology
+Keywords: computational systems biology,modelling,simulation,systems biology
 Home-page: https://pysces.github.io
 Author-Email: Brett Olivier <pysces@googlegroups.com>, Johann Rohwer <pysces@googlegroups.com>
 Maintainer-Email: Brett Olivier <pysces@googlegroups.com>, Johann Rohwer <pysces@googlegroups.com>
 License: BSD 3-Clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Development Status :: 6 - Mature
 Classifier: Environment :: Console
```

