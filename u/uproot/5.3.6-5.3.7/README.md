# Comparing `tmp/uproot-5.3.6.tar.gz` & `tmp/uproot-5.3.7.tar.gz`

## Comparing `uproot-5.3.6.tar` & `uproot-5.3.7.tar`

### file list

```diff
@@ -1,276 +1,277 @@
--rw-r--r--   0        0        0    15427 2020-02-02 00:00:00.000000 uproot-5.3.6/.all-contributorsrc
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 uproot-5.3.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 uproot-5.3.6/.readthedocs.yml
--rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 uproot-5.3.6/CITATION.cff
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 uproot-5.3.6/.github/dependabot.yml
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 uproot-5.3.6/.github/ISSUE_TEMPLATE/bug-report.md
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 uproot-5.3.6/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 uproot-5.3.6/.github/ISSUE_TEMPLATE/documentation.md
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 uproot-5.3.6/.github/ISSUE_TEMPLATE/feature-request.md
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 uproot-5.3.6/.github/workflows/build-distributions.yml
--rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 uproot-5.3.6/.github/workflows/build-test.yml
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 uproot-5.3.6/.github/workflows/deploy.yml
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 uproot-5.3.6/.github/workflows/semantic-pr-title.yml
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 uproot-5.3.6/.github/workflows/upload-nightly-wheels.yml
--rw-r--r--   0        0        0     4297 2020-02-02 00:00:00.000000 uproot-5.3.6/dev/example-objects.py
--rw-r--r--   0        0        0     4133 2020-02-02 00:00:00.000000 uproot-5.3.6/dev/make-models.py
--rw-r--r--   0        0        0    95009 2020-02-02 00:00:00.000000 uproot-5.3.6/docs-img/diagrams/abstraction-layers.png
--rw-r--r--   0        0        0    39940 2020-02-02 00:00:00.000000 uproot-5.3.6/docs-img/diagrams/abstraction-layers.svg
--rw-r--r--   0        0        0    49015 2020-02-02 00:00:00.000000 uproot-5.3.6/docs-img/diagrams/example-dask-graph.png
--rw-r--r--   0        0        0    70413 2020-02-02 00:00:00.000000 uproot-5.3.6/docs-img/diagrams/uproot-awkward-timeline.png
--rw-r--r--   0        0        0    28715 2020-02-02 00:00:00.000000 uproot-5.3.6/docs-img/diagrams/uproot-awkward-timeline.svg
--rw-r--r--   0        0        0     6794 2020-02-02 00:00:00.000000 uproot-5.3.6/docs-img/logo/logo-300px-white.png
--rw-r--r--   0        0        0     8489 2020-02-02 00:00:00.000000 uproot-5.3.6/docs-img/logo/logo-300px.png
--rw-r--r--   0        0        0    17651 2020-02-02 00:00:00.000000 uproot-5.3.6/docs-img/logo/logo-600px.png
--rw-r--r--   0        0        0     7695 2020-02-02 00:00:00.000000 uproot-5.3.6/docs-img/logo/logo.svg
--rw-r--r--   0        0        0   223219 2020-02-02 00:00:00.000000 uproot-5.3.6/docs-img/photos/switcheroo.jpg
--rw-r--r--   0        0        0    69268 2020-02-02 00:00:00.000000 uproot-5.3.6/docs-sphinx/basic.rst
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 uproot-5.3.6/docs-sphinx/conf.py
--rw-r--r--   0        0        0     5622 2020-02-02 00:00:00.000000 uproot-5.3.6/docs-sphinx/index.rst
--rw-r--r--   0        0        0     7841 2020-02-02 00:00:00.000000 uproot-5.3.6/docs-sphinx/make_changelog.py
--rw-r--r--   0        0        0    10456 2020-02-02 00:00:00.000000 uproot-5.3.6/docs-sphinx/prepare_docstrings.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 uproot-5.3.6/docs-sphinx/requirements.txt
--rw-r--r--   0        0        0    22209 2020-02-02 00:00:00.000000 uproot-5.3.6/docs-sphinx/uproot3-to-4.rst
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 uproot-5.3.6/docs-sphinx/_templates/breadcrumbs.html
--rw-r--r--   0        0        0     6952 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/__init__.py
--rw-r--r--   0        0        0     9180 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/_awkwardforth.py
--rw-r--r--   0        0        0    57024 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/_dask.py
--rw-r--r--   0        0        0    34724 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/_util.py
--rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/behavior.py
--rw-r--r--   0        0        0     7506 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/cache.py
--rw-r--r--   0        0        0    19158 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/compression.py
--rw-r--r--   0        0        0     4215 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/const.py
--rw-r--r--   0        0        0    64522 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/containers.py
--rw-r--r--   0        0        0    20731 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/deserialization.py
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/dynamic.py
--rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/exceptions.py
--rw-r--r--   0        0        0     8297 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/extras.py
--rw-r--r--   0        0        0    66033 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/model.py
--rw-r--r--   0        0        0     9625 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/pyroot.py
--rw-r--r--   0        0        0    98111 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/reading.py
--rw-r--r--   0        0        0     3171 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/serialization.py
--rw-r--r--   0        0        0    64326 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/streamers.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/version.py
--rw-r--r--   0        0        0     5649 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/behaviors/RooCurve.py
--rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/behaviors/RooHist.py
--rw-r--r--   0        0        0    10083 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/behaviors/TAxis.py
--rw-r--r--   0        0        0   129715 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/behaviors/TBranch.py
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/behaviors/TBranchElement.py
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/behaviors/TDatime.py
--rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/behaviors/TGraph.py
--rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/behaviors/TGraphAsymmErrors.py
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/behaviors/TGraphErrors.py
--rw-r--r--   0        0        0    12104 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/behaviors/TH1.py
--rw-r--r--   0        0        0     3511 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/behaviors/TH2.py
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/behaviors/TH2Poly.py
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/behaviors/TH3.py
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/behaviors/TParameter.py
--rw-r--r--   0        0        0    12480 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/behaviors/TProfile.py
--rw-r--r--   0        0        0     3950 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/behaviors/TProfile2D.py
--rw-r--r--   0        0        0     4412 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/behaviors/TProfile3D.py
--rw-r--r--   0        0        0     5361 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/behaviors/TTree.py
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/behaviors/__init__.py
--rw-r--r--   0        0        0     8305 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/interpretation/__init__.py
--rw-r--r--   0        0        0     4461 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/interpretation/grouped.py
--rw-r--r--   0        0        0    41203 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/interpretation/identify.py
--rw-r--r--   0        0        0    14929 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/interpretation/jagged.py
--rw-r--r--   0        0        0    38158 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/interpretation/library.py
--rw-r--r--   0        0        0    22691 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/interpretation/numerical.py
--rw-r--r--   0        0        0    37599 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/interpretation/objects.py
--rw-r--r--   0        0        0    18832 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/interpretation/strings.py
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/language/__init__.py
--rw-r--r--   0        0        0    16942 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/language/python.py
--rw-r--r--   0        0        0    32821 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/models/RNTuple.py
--rw-r--r--   0        0        0     4903 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/models/TArray.py
--rw-r--r--   0        0        0    25962 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/models/TAtt.py
--rw-r--r--   0        0        0    11268 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/models/TBasket.py
--rw-r--r--   0        0        0    37710 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/models/TBranch.py
--rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/models/TClonesArray.py
--rw-r--r--   0        0        0     2974 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/models/TDatime.py
--rw-r--r--   0        0        0    35842 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/models/TGraph.py
--rw-r--r--   0        0        0   215525 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/models/TH.py
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/models/THashList.py
--rw-r--r--   0        0        0    34985 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/models/TLeaf.py
--rw-r--r--   0        0        0     3462 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/models/TList.py
--rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/models/TMatrixT.py
--rw-r--r--   0        0        0     3164 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/models/TNamed.py
--rw-r--r--   0        0        0     5879 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/models/TObjArray.py
--rw-r--r--   0        0        0     3948 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/models/TObjString.py
--rw-r--r--   0        0        0     4278 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/models/TObject.py
--rw-r--r--   0        0        0     8575 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/models/TRef.py
--rw-r--r--   0        0        0     3617 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/models/TString.py
--rw-r--r--   0        0        0     7502 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/models/TTable.py
--rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/models/TTime.py
--rw-r--r--   0        0        0    47535 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/models/TTree.py
--rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/models/__init__.py
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/sink/__init__.py
--rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/sink/file.py
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/source/__init__.py
--rw-r--r--   0        0        0    17529 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/source/chunk.py
--rw-r--r--   0        0        0    24376 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/source/cursor.py
--rw-r--r--   0        0        0     8752 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/source/file.py
--rw-r--r--   0        0        0     8185 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/source/fsspec.py
--rw-r--r--   0        0        0    15114 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/source/futures.py
--rw-r--r--   0        0        0    28139 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/source/http.py
--rw-r--r--   0        0        0     4065 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/source/object.py
--rw-r--r--   0        0        0     2851 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/source/s3.py
--rw-r--r--   0        0        0    17188 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/source/xrootd.py
--rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/writing/__init__.py
--rw-r--r--   0        0        0    81089 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/writing/_cascade.py
--rw-r--r--   0        0        0    31428 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/writing/_cascadentuple.py
--rw-r--r--   0        0        0    62357 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/writing/_cascadetree.py
--rw-r--r--   0        0        0     6360 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/writing/_dask_write.py
--rw-r--r--   0        0        0    82120 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/writing/identify.py
--rw-r--r--   0        0        0    80822 2020-02-02 00:00:00.000000 uproot-5.3.6/src/uproot/writing/writable.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/__init__.py
--rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/conftest.py
--rw-r--r--   0        0        0    17012 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0001_source_class.py
--rw-r--r--   0        0        0     7141 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0006_notify_when_downloaded.py
--rw-r--r--   0        0        0     5467 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0007_single_chunk_interface.py
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0008_start_interpretation.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0009_nested_directories.py
--rw-r--r--   0        0        0    29196 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0010_start_streamers.py
--rw-r--r--   0        0        0     4207 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0011_generate_classes_from_streamers.py
--rw-r--r--   0        0        0     3679 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0013_rntuple_anchor.py
--rw-r--r--   0        0        0     9305 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0014_all_ttree_versions.py
--rw-r--r--   0        0        0     3760 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0016_interpretations.py
--rw-r--r--   0        0        0     9651 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0017_multi_basket_multi_branch_fetch.py
--rw-r--r--   0        0        0    33935 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0018_array_fetching_interface.py
--rw-r--r--   0        0        0     8813 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0022_number_of_branches.py
--rw-r--r--   0        0        0    13960 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0023_more_interpretations_1.py
--rw-r--r--   0        0        0    24165 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0023_ttree_versions.py
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0028_fallback_to_read_streamer.py
--rw-r--r--   0        0        0     7606 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0029_more_string_types.py
--rw-r--r--   0        0        0    23329 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0031_test_stl_containers.py
--rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0033_more_interpretations_2.py
--rw-r--r--   0        0        0    46572 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0034_generic_objects_in_ttrees.py
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0035_datatype_generality.py
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0038_memberwise_serialization.py
--rw-r--r--   0        0        0     8188 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0043_iterate_function.py
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0044_concatenate_function.py
--rw-r--r--   0        0        0    68981 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0046_histograms_bh_hist.py
--rw-r--r--   0        0        0     8605 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0053_parents_should_not_be_bases.py
--rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0058_detach_model_objects_from_files.py
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0066_fix_http_fallback_freeze.py
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0067_common_entry_offsets.py
--rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0081_dont_parse_colons.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0087_memberwise_splitting_not_implemented_messages.py
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0088_read_with_http.py
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0099_read_from_file_object.py
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0112_fix_pandas_with_cut.py
--rw-r--r--   0        0        0     7914 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0118_fix_name_fetch_again.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0123_atlas_issues.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0126_turn_unknown_emptyarrays_into_known_types.py
--rw-r--r--   0        0        0     6118 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0167_use_the_common_histogram_interface.py
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0172_allow_allocators_in_vector_typenames.py
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0173_empty_and_multiprocessing_bugs.py
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0182_complain_about_missing_files.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0194_fix_lost_cuts_in_iterate.py
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0220_contiguous_byte_ranges_in_http.py
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0228_read_TProfiles.py
--rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0240_read_TGraphAsymmErrors.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0278_specializations_for_TParameter.py
--rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0302_pickle.py
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0303_empty_jagged_array.py
--rw-r--r--   0        0        0    14234 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0320_start_working_on_ROOT_writing.py
--rw-r--r--   0        0        0     2919 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0322_writablefile_infrastructure.py
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0329_update_existing_root_files.py
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0335_empty_ttree_division_by_zero.py
--rw-r--r--   0        0        0     7555 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0341_manipulate_streamer_info.py
--rw-r--r--   0        0        0     2821 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0344_writabledirectory_can_read.py
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0345_bulk_copy_method.py
--rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0349_write_TObjString.py
--rw-r--r--   0        0        0     6943 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0350_read_RooCurve_RooHist.py
--rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0351_write_TList.py
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0352_write_THashList.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0384_move_behavior_of_and_fix_383.py
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0398_dimensions_in_leaflist.py
--rw-r--r--   0        0        0    26536 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0405_write_a_histogram.py
--rw-r--r--   0        0        0    11518 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0406_write_a_ttree.py
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0407_read_TDatime.py
--rw-r--r--   0        0        0    17062 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0412_write_multidimensional_numpy_to_ttree.py
--rw-r--r--   0        0        0    15363 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0414_write_jagged_arrays.py
--rw-r--r--   0        0        0    26706 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0416_writing_compressed_data.py
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0418_read_TTable.py
--rw-r--r--   0        0        0     3568 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0420_pyroot_uproot_interoperability.py
--rw-r--r--   0        0        0    17479 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0422_hist_integration.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0430_global_index_for_tuples_of_DataFrames.py
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0438_TClonesArray_is_not_AsGrouped.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0439_check_awkward_before_numpy.py
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0442_regular_TClonesArray.py
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0472_tstreamerinfo_for_ttree.py
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0475_remember_to_update_freesegments.py
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0484_manually_add_model_for_TMatrixTSym_double_.py
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0487_implement_asdtypeinplace.py
--rw-r--r--   0        0        0     4527 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0498_create_leaf_branch_in_extend.py
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0519_remove_memmap_copy.py
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0520_dynamic_classes_cant_be_abc_subclasses.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0569_fBits_is_4_bytes.py
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0576_unicode_in_names.py
--rw-r--r--   0        0        0    25906 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0578_dask_for_numpy.py
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0580_round_trip_for_no_flow_histograms.py
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0589_explicitly_interpret_RVec_type.py
--rw-r--r--   0        0        0     2930 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0603_dask_delayed_open.py
--rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0609_num_enteries_func.py
--rw-r--r--   0        0        0    18214 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0610_awkward_form.py
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0630_rntuple_basics.py
--rw-r--r--   0        0        0   132838 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0637_setup_tests_for_AwkwardForth.py
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0643_reading_vector_pair_TLorentzVector_int.py
--rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0651_implement_transformed_axis.py
--rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0652_dask_for_awkward.py
--rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0662_rntuple_stl_containers.py
--rw-r--r--   0        0        0    16181 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0692_fsspec_reading.py
--rw-r--r--   0        0        0     6369 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0692_fsspec_writing.py
--rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0700_dask_empty_arrays.py
--rw-r--r--   0        0        0     2728 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0705_rntuple_writing_metadata.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0750_avoid_empty_TBasket_issue.py
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0755_dask_awkward_column_projection.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0791_protect_uproot_project_columns_from_dask_node_names.py
--rw-r--r--   0        0        0     4885 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0798_DAOD_PHYSLITE.py
--rw-r--r--   0        0        0     2365 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0808_fix_awkward_form_for_AsStridedObjects.py
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0816_separate_AwkwardForth_machines_by_TBranch.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0832_ak_add_doc_should_also_add_to_typetracer.py
--rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0840_support_tleafG.py
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0841_fix_814.py
--rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0844_fix_delete_hist_from_root.py
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0852_fix_strided_interp_extra_offsets.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0870_writing_arrays_of_type_unknown_fix_822.py
--rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0876_uproot_dask_blind_steps.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0886_fix_awkward_form_breadcrumbs.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0910_fix_906_members_non_numerical_branches.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0911_fix_interp_array_non_numerical_objs_issue_880.py
--rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0912_fix_pandas_and_double_nested_vectors_issue_885.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0916_read_from_s3.py
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0927_dont_assume_uproot_in_global_scope_in_TPython_Eval.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0930_expressions_in_pandas.py
--rw-r--r--   0        0        0     7233 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0940_feat_add_TLeafC_string_support.py
--rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0962_RNTuple_update.py
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0965_inverted_axes_variances_hist_888.py
--rw-r--r--   0        0        0     7389 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_0976_path_object_split.py
--rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_1000-write-TProfiles.py
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_1043_const_std_string.py
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_1058_dask_awkward_report.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_1063_dask_distributed.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_1070_pandas_dataframe_building_performance_fix.py
--rw-r--r--   0        0        0     3527 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_1085_dask_write.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_1102_any_locks_in_models_must_be_transient.py
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_1114_fix_attempt_to_concatenate_numpy_with_awkward.py
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_1120_check_decompression_executor_pass_for_dask.py
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_1127_fix_allow_colon_in_key_names.py
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_1146_split_ranges_for_large_files_over_http.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_1154_classof_using_relative_path.py
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_1160_std_string_in_TDirectory.py
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_1180_read_free_floating_vector_issue_1179.py
--rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_1181_support_for_stl_list.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_1182_add_support_for_bitset.py
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_1183_ttime_custom.py
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_1186_dtype_might_raise_ValueError.py
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_1189_dask_failing_on_duplicate_keys.py
--rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_1191_rntuple_fixes.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/test_1207_fix_title_of_TBranch_with_counter.py
--rw-r--r--   0        0        0   128147 2020-02-02 00:00:00.000000 uproot-5.3.6/tests/samples/h_dynamic.pkl
--rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 uproot-5.3.6/.gitignore
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 uproot-5.3.6/LICENSE
--rw-r--r--   0        0        0    29133 2020-02-02 00:00:00.000000 uproot-5.3.6/README.md
--rw-r--r--   0        0        0     3941 2020-02-02 00:00:00.000000 uproot-5.3.6/pyproject.toml
--rw-r--r--   0        0        0    31907 2020-02-02 00:00:00.000000 uproot-5.3.6/PKG-INFO
+-rw-r--r--   0        0        0    15427 2020-02-02 00:00:00.000000 uproot-5.3.7/.all-contributorsrc
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 uproot-5.3.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 uproot-5.3.7/.readthedocs.yml
+-rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 uproot-5.3.7/CITATION.cff
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 uproot-5.3.7/.github/dependabot.yml
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 uproot-5.3.7/.github/ISSUE_TEMPLATE/bug-report.md
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 uproot-5.3.7/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 uproot-5.3.7/.github/ISSUE_TEMPLATE/documentation.md
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 uproot-5.3.7/.github/ISSUE_TEMPLATE/feature-request.md
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 uproot-5.3.7/.github/workflows/build-distributions.yml
+-rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 uproot-5.3.7/.github/workflows/build-test.yml
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 uproot-5.3.7/.github/workflows/deploy.yml
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 uproot-5.3.7/.github/workflows/semantic-pr-title.yml
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 uproot-5.3.7/.github/workflows/upload-nightly-wheels.yml
+-rw-r--r--   0        0        0     4297 2020-02-02 00:00:00.000000 uproot-5.3.7/dev/example-objects.py
+-rw-r--r--   0        0        0     4133 2020-02-02 00:00:00.000000 uproot-5.3.7/dev/make-models.py
+-rw-r--r--   0        0        0    95009 2020-02-02 00:00:00.000000 uproot-5.3.7/docs-img/diagrams/abstraction-layers.png
+-rw-r--r--   0        0        0    39940 2020-02-02 00:00:00.000000 uproot-5.3.7/docs-img/diagrams/abstraction-layers.svg
+-rw-r--r--   0        0        0    49015 2020-02-02 00:00:00.000000 uproot-5.3.7/docs-img/diagrams/example-dask-graph.png
+-rw-r--r--   0        0        0    70413 2020-02-02 00:00:00.000000 uproot-5.3.7/docs-img/diagrams/uproot-awkward-timeline.png
+-rw-r--r--   0        0        0    28715 2020-02-02 00:00:00.000000 uproot-5.3.7/docs-img/diagrams/uproot-awkward-timeline.svg
+-rw-r--r--   0        0        0     6794 2020-02-02 00:00:00.000000 uproot-5.3.7/docs-img/logo/logo-300px-white.png
+-rw-r--r--   0        0        0     8489 2020-02-02 00:00:00.000000 uproot-5.3.7/docs-img/logo/logo-300px.png
+-rw-r--r--   0        0        0    17651 2020-02-02 00:00:00.000000 uproot-5.3.7/docs-img/logo/logo-600px.png
+-rw-r--r--   0        0        0     7695 2020-02-02 00:00:00.000000 uproot-5.3.7/docs-img/logo/logo.svg
+-rw-r--r--   0        0        0   223219 2020-02-02 00:00:00.000000 uproot-5.3.7/docs-img/photos/switcheroo.jpg
+-rw-r--r--   0        0        0    69268 2020-02-02 00:00:00.000000 uproot-5.3.7/docs-sphinx/basic.rst
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 uproot-5.3.7/docs-sphinx/conf.py
+-rw-r--r--   0        0        0     5622 2020-02-02 00:00:00.000000 uproot-5.3.7/docs-sphinx/index.rst
+-rw-r--r--   0        0        0     7841 2020-02-02 00:00:00.000000 uproot-5.3.7/docs-sphinx/make_changelog.py
+-rw-r--r--   0        0        0    10456 2020-02-02 00:00:00.000000 uproot-5.3.7/docs-sphinx/prepare_docstrings.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 uproot-5.3.7/docs-sphinx/requirements.txt
+-rw-r--r--   0        0        0    22209 2020-02-02 00:00:00.000000 uproot-5.3.7/docs-sphinx/uproot3-to-4.rst
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 uproot-5.3.7/docs-sphinx/_templates/breadcrumbs.html
+-rw-r--r--   0        0        0     6952 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/__init__.py
+-rw-r--r--   0        0        0     9180 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/_awkwardforth.py
+-rw-r--r--   0        0        0    57024 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/_dask.py
+-rw-r--r--   0        0        0    34724 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/_util.py
+-rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/behavior.py
+-rw-r--r--   0        0        0     7506 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/cache.py
+-rw-r--r--   0        0        0    19158 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/compression.py
+-rw-r--r--   0        0        0     4215 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/const.py
+-rw-r--r--   0        0        0    64522 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/containers.py
+-rw-r--r--   0        0        0    20731 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/deserialization.py
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/dynamic.py
+-rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/exceptions.py
+-rw-r--r--   0        0        0     8297 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/extras.py
+-rw-r--r--   0        0        0    66033 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/model.py
+-rw-r--r--   0        0        0     9625 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/pyroot.py
+-rw-r--r--   0        0        0    98111 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/reading.py
+-rw-r--r--   0        0        0     3171 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/serialization.py
+-rw-r--r--   0        0        0    64326 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/streamers.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/version.py
+-rw-r--r--   0        0        0     5649 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/behaviors/RooCurve.py
+-rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/behaviors/RooHist.py
+-rw-r--r--   0        0        0    10083 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/behaviors/TAxis.py
+-rw-r--r--   0        0        0   129715 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/behaviors/TBranch.py
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/behaviors/TBranchElement.py
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/behaviors/TDatime.py
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/behaviors/TGraph.py
+-rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/behaviors/TGraphAsymmErrors.py
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/behaviors/TGraphErrors.py
+-rw-r--r--   0        0        0    12104 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/behaviors/TH1.py
+-rw-r--r--   0        0        0     3511 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/behaviors/TH2.py
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/behaviors/TH2Poly.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/behaviors/TH3.py
+-rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/behaviors/TParameter.py
+-rw-r--r--   0        0        0    12480 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/behaviors/TProfile.py
+-rw-r--r--   0        0        0     3950 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/behaviors/TProfile2D.py
+-rw-r--r--   0        0        0     4412 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/behaviors/TProfile3D.py
+-rw-r--r--   0        0        0     5361 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/behaviors/TTree.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/behaviors/__init__.py
+-rw-r--r--   0        0        0     8305 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/interpretation/__init__.py
+-rw-r--r--   0        0        0     4461 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/interpretation/grouped.py
+-rw-r--r--   0        0        0    41203 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/interpretation/identify.py
+-rw-r--r--   0        0        0    14929 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/interpretation/jagged.py
+-rw-r--r--   0        0        0    38158 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/interpretation/library.py
+-rw-r--r--   0        0        0    22691 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/interpretation/numerical.py
+-rw-r--r--   0        0        0    37599 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/interpretation/objects.py
+-rw-r--r--   0        0        0    18832 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/interpretation/strings.py
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/language/__init__.py
+-rw-r--r--   0        0        0    16942 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/language/python.py
+-rw-r--r--   0        0        0    32821 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/models/RNTuple.py
+-rw-r--r--   0        0        0     4903 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/models/TArray.py
+-rw-r--r--   0        0        0    25962 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/models/TAtt.py
+-rw-r--r--   0        0        0    11268 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/models/TBasket.py
+-rw-r--r--   0        0        0    37710 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/models/TBranch.py
+-rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/models/TClonesArray.py
+-rw-r--r--   0        0        0     2974 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/models/TDatime.py
+-rw-r--r--   0        0        0    35842 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/models/TGraph.py
+-rw-r--r--   0        0        0   215525 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/models/TH.py
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/models/THashList.py
+-rw-r--r--   0        0        0    34985 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/models/TLeaf.py
+-rw-r--r--   0        0        0     3462 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/models/TList.py
+-rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/models/TMatrixT.py
+-rw-r--r--   0        0        0     3164 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/models/TNamed.py
+-rw-r--r--   0        0        0     5879 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/models/TObjArray.py
+-rw-r--r--   0        0        0     3948 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/models/TObjString.py
+-rw-r--r--   0        0        0     4278 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/models/TObject.py
+-rw-r--r--   0        0        0     8575 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/models/TRef.py
+-rw-r--r--   0        0        0     3617 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/models/TString.py
+-rw-r--r--   0        0        0     7502 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/models/TTable.py
+-rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/models/TTime.py
+-rw-r--r--   0        0        0    47535 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/models/TTree.py
+-rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/models/__init__.py
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/sink/__init__.py
+-rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/sink/file.py
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/source/__init__.py
+-rw-r--r--   0        0        0    17529 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/source/chunk.py
+-rw-r--r--   0        0        0    24376 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/source/cursor.py
+-rw-r--r--   0        0        0     8752 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/source/file.py
+-rw-r--r--   0        0        0     8185 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/source/fsspec.py
+-rw-r--r--   0        0        0    15114 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/source/futures.py
+-rw-r--r--   0        0        0    28139 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/source/http.py
+-rw-r--r--   0        0        0     4065 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/source/object.py
+-rw-r--r--   0        0        0     2851 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/source/s3.py
+-rw-r--r--   0        0        0    17188 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/source/xrootd.py
+-rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/writing/__init__.py
+-rw-r--r--   0        0        0    81158 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/writing/_cascade.py
+-rw-r--r--   0        0        0    31428 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/writing/_cascadentuple.py
+-rw-r--r--   0        0        0    62357 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/writing/_cascadetree.py
+-rw-r--r--   0        0        0     6360 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/writing/_dask_write.py
+-rw-r--r--   0        0        0    82120 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/writing/identify.py
+-rw-r--r--   0        0        0    80822 2020-02-02 00:00:00.000000 uproot-5.3.7/src/uproot/writing/writable.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/__init__.py
+-rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/conftest.py
+-rw-r--r--   0        0        0    17012 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0001_source_class.py
+-rw-r--r--   0        0        0     7141 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0006_notify_when_downloaded.py
+-rw-r--r--   0        0        0     5467 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0007_single_chunk_interface.py
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0008_start_interpretation.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0009_nested_directories.py
+-rw-r--r--   0        0        0    29196 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0010_start_streamers.py
+-rw-r--r--   0        0        0     4207 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0011_generate_classes_from_streamers.py
+-rw-r--r--   0        0        0     3679 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0013_rntuple_anchor.py
+-rw-r--r--   0        0        0     9305 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0014_all_ttree_versions.py
+-rw-r--r--   0        0        0     3760 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0016_interpretations.py
+-rw-r--r--   0        0        0     9651 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0017_multi_basket_multi_branch_fetch.py
+-rw-r--r--   0        0        0    33935 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0018_array_fetching_interface.py
+-rw-r--r--   0        0        0     8813 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0022_number_of_branches.py
+-rw-r--r--   0        0        0    13960 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0023_more_interpretations_1.py
+-rw-r--r--   0        0        0    24165 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0023_ttree_versions.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0028_fallback_to_read_streamer.py
+-rw-r--r--   0        0        0     7606 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0029_more_string_types.py
+-rw-r--r--   0        0        0    23329 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0031_test_stl_containers.py
+-rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0033_more_interpretations_2.py
+-rw-r--r--   0        0        0    46572 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0034_generic_objects_in_ttrees.py
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0035_datatype_generality.py
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0038_memberwise_serialization.py
+-rw-r--r--   0        0        0     8188 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0043_iterate_function.py
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0044_concatenate_function.py
+-rw-r--r--   0        0        0    68981 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0046_histograms_bh_hist.py
+-rw-r--r--   0        0        0     8605 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0053_parents_should_not_be_bases.py
+-rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0058_detach_model_objects_from_files.py
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0066_fix_http_fallback_freeze.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0067_common_entry_offsets.py
+-rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0081_dont_parse_colons.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0087_memberwise_splitting_not_implemented_messages.py
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0088_read_with_http.py
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0099_read_from_file_object.py
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0112_fix_pandas_with_cut.py
+-rw-r--r--   0        0        0     7914 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0118_fix_name_fetch_again.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0123_atlas_issues.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0126_turn_unknown_emptyarrays_into_known_types.py
+-rw-r--r--   0        0        0     6118 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0167_use_the_common_histogram_interface.py
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0172_allow_allocators_in_vector_typenames.py
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0173_empty_and_multiprocessing_bugs.py
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0182_complain_about_missing_files.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0194_fix_lost_cuts_in_iterate.py
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0220_contiguous_byte_ranges_in_http.py
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0228_read_TProfiles.py
+-rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0240_read_TGraphAsymmErrors.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0278_specializations_for_TParameter.py
+-rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0302_pickle.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0303_empty_jagged_array.py
+-rw-r--r--   0        0        0    14234 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0320_start_working_on_ROOT_writing.py
+-rw-r--r--   0        0        0     2919 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0322_writablefile_infrastructure.py
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0329_update_existing_root_files.py
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0335_empty_ttree_division_by_zero.py
+-rw-r--r--   0        0        0     7555 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0341_manipulate_streamer_info.py
+-rw-r--r--   0        0        0     2821 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0344_writabledirectory_can_read.py
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0345_bulk_copy_method.py
+-rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0349_write_TObjString.py
+-rw-r--r--   0        0        0     6943 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0350_read_RooCurve_RooHist.py
+-rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0351_write_TList.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0352_write_THashList.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0384_move_behavior_of_and_fix_383.py
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0398_dimensions_in_leaflist.py
+-rw-r--r--   0        0        0    26536 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0405_write_a_histogram.py
+-rw-r--r--   0        0        0    11518 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0406_write_a_ttree.py
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0407_read_TDatime.py
+-rw-r--r--   0        0        0    17062 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0412_write_multidimensional_numpy_to_ttree.py
+-rw-r--r--   0        0        0    15363 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0414_write_jagged_arrays.py
+-rw-r--r--   0        0        0    26706 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0416_writing_compressed_data.py
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0418_read_TTable.py
+-rw-r--r--   0        0        0     3568 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0420_pyroot_uproot_interoperability.py
+-rw-r--r--   0        0        0    17479 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0422_hist_integration.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0430_global_index_for_tuples_of_DataFrames.py
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0438_TClonesArray_is_not_AsGrouped.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0439_check_awkward_before_numpy.py
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0442_regular_TClonesArray.py
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0472_tstreamerinfo_for_ttree.py
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0475_remember_to_update_freesegments.py
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0484_manually_add_model_for_TMatrixTSym_double_.py
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0487_implement_asdtypeinplace.py
+-rw-r--r--   0        0        0     4527 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0498_create_leaf_branch_in_extend.py
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0519_remove_memmap_copy.py
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0520_dynamic_classes_cant_be_abc_subclasses.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0569_fBits_is_4_bytes.py
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0576_unicode_in_names.py
+-rw-r--r--   0        0        0    25906 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0578_dask_for_numpy.py
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0580_round_trip_for_no_flow_histograms.py
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0589_explicitly_interpret_RVec_type.py
+-rw-r--r--   0        0        0     2930 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0603_dask_delayed_open.py
+-rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0609_num_enteries_func.py
+-rw-r--r--   0        0        0    18214 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0610_awkward_form.py
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0630_rntuple_basics.py
+-rw-r--r--   0        0        0   132838 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0637_setup_tests_for_AwkwardForth.py
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0643_reading_vector_pair_TLorentzVector_int.py
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0651_implement_transformed_axis.py
+-rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0652_dask_for_awkward.py
+-rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0662_rntuple_stl_containers.py
+-rw-r--r--   0        0        0    16181 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0692_fsspec_reading.py
+-rw-r--r--   0        0        0     6369 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0692_fsspec_writing.py
+-rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0700_dask_empty_arrays.py
+-rw-r--r--   0        0        0     2728 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0705_rntuple_writing_metadata.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0750_avoid_empty_TBasket_issue.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0755_dask_awkward_column_projection.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0791_protect_uproot_project_columns_from_dask_node_names.py
+-rw-r--r--   0        0        0     4885 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0798_DAOD_PHYSLITE.py
+-rw-r--r--   0        0        0     2365 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0808_fix_awkward_form_for_AsStridedObjects.py
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0816_separate_AwkwardForth_machines_by_TBranch.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0832_ak_add_doc_should_also_add_to_typetracer.py
+-rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0840_support_tleafG.py
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0841_fix_814.py
+-rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0844_fix_delete_hist_from_root.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0852_fix_strided_interp_extra_offsets.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0870_writing_arrays_of_type_unknown_fix_822.py
+-rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0876_uproot_dask_blind_steps.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0886_fix_awkward_form_breadcrumbs.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0910_fix_906_members_non_numerical_branches.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0911_fix_interp_array_non_numerical_objs_issue_880.py
+-rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0912_fix_pandas_and_double_nested_vectors_issue_885.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0916_read_from_s3.py
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0927_dont_assume_uproot_in_global_scope_in_TPython_Eval.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0930_expressions_in_pandas.py
+-rw-r--r--   0        0        0     7233 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0940_feat_add_TLeafC_string_support.py
+-rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0962_RNTuple_update.py
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0965_inverted_axes_variances_hist_888.py
+-rw-r--r--   0        0        0     7389 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_0976_path_object_split.py
+-rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_1000-write-TProfiles.py
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_1043_const_std_string.py
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_1058_dask_awkward_report.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_1063_dask_distributed.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_1070_pandas_dataframe_building_performance_fix.py
+-rw-r--r--   0        0        0     3527 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_1085_dask_write.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_1102_any_locks_in_models_must_be_transient.py
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_1114_fix_attempt_to_concatenate_numpy_with_awkward.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_1120_check_decompression_executor_pass_for_dask.py
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_1127_fix_allow_colon_in_key_names.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_1146_split_ranges_for_large_files_over_http.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_1154_classof_using_relative_path.py
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_1160_std_string_in_TDirectory.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_1180_read_free_floating_vector_issue_1179.py
+-rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_1181_support_for_stl_list.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_1182_add_support_for_bitset.py
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_1183_ttime_custom.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_1186_dtype_might_raise_ValueError.py
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_1189_dask_failing_on_duplicate_keys.py
+-rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_1191_rntuple_fixes.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_1207_fix_title_of_TBranch_with_counter.py
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/test_1212_dont_let_update_mess_up_file_version.py
+-rw-r--r--   0        0        0   128147 2020-02-02 00:00:00.000000 uproot-5.3.7/tests/samples/h_dynamic.pkl
+-rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 uproot-5.3.7/.gitignore
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 uproot-5.3.7/LICENSE
+-rw-r--r--   0        0        0    29133 2020-02-02 00:00:00.000000 uproot-5.3.7/README.md
+-rw-r--r--   0        0        0     3941 2020-02-02 00:00:00.000000 uproot-5.3.7/pyproject.toml
+-rw-r--r--   0        0        0    31907 2020-02-02 00:00:00.000000 uproot-5.3.7/PKG-INFO
```

### Comparing `uproot-5.3.6/.all-contributorsrc` & `uproot-5.3.7/.all-contributorsrc`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/.pre-commit-config.yaml` & `uproot-5.3.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/CITATION.cff` & `uproot-5.3.7/CITATION.cff`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/.github/ISSUE_TEMPLATE/bug-report.md` & `uproot-5.3.7/.github/ISSUE_TEMPLATE/bug-report.md`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/.github/ISSUE_TEMPLATE/feature-request.md` & `uproot-5.3.7/.github/ISSUE_TEMPLATE/feature-request.md`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/.github/workflows/build-distributions.yml` & `uproot-5.3.7/.github/workflows/build-distributions.yml`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/.github/workflows/build-test.yml` & `uproot-5.3.7/.github/workflows/build-test.yml`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/.github/workflows/deploy.yml` & `uproot-5.3.7/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/.github/workflows/upload-nightly-wheels.yml` & `uproot-5.3.7/.github/workflows/upload-nightly-wheels.yml`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/dev/example-objects.py` & `uproot-5.3.7/dev/example-objects.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/dev/make-models.py` & `uproot-5.3.7/dev/make-models.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/docs-img/diagrams/abstraction-layers.png` & `uproot-5.3.7/docs-img/diagrams/abstraction-layers.png`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/docs-img/diagrams/abstraction-layers.svg` & `uproot-5.3.7/docs-img/diagrams/abstraction-layers.svg`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/docs-img/diagrams/example-dask-graph.png` & `uproot-5.3.7/docs-img/diagrams/example-dask-graph.png`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/docs-img/diagrams/uproot-awkward-timeline.png` & `uproot-5.3.7/docs-img/diagrams/uproot-awkward-timeline.png`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/docs-img/diagrams/uproot-awkward-timeline.svg` & `uproot-5.3.7/docs-img/diagrams/uproot-awkward-timeline.svg`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/docs-img/logo/logo-300px-white.png` & `uproot-5.3.7/docs-img/logo/logo-300px-white.png`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/docs-img/logo/logo-300px.png` & `uproot-5.3.7/docs-img/logo/logo-300px.png`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/docs-img/logo/logo-600px.png` & `uproot-5.3.7/docs-img/logo/logo-600px.png`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/docs-img/logo/logo.svg` & `uproot-5.3.7/docs-img/logo/logo.svg`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/docs-img/photos/switcheroo.jpg` & `uproot-5.3.7/docs-img/photos/switcheroo.jpg`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/docs-sphinx/basic.rst` & `uproot-5.3.7/docs-sphinx/basic.rst`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/docs-sphinx/conf.py` & `uproot-5.3.7/docs-sphinx/conf.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/docs-sphinx/index.rst` & `uproot-5.3.7/docs-sphinx/index.rst`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/docs-sphinx/make_changelog.py` & `uproot-5.3.7/docs-sphinx/make_changelog.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/docs-sphinx/prepare_docstrings.py` & `uproot-5.3.7/docs-sphinx/prepare_docstrings.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/docs-sphinx/uproot3-to-4.rst` & `uproot-5.3.7/docs-sphinx/uproot3-to-4.rst`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/__init__.py` & `uproot-5.3.7/src/uproot/__init__.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/_awkwardforth.py` & `uproot-5.3.7/src/uproot/_awkwardforth.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/_dask.py` & `uproot-5.3.7/src/uproot/_dask.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/_util.py` & `uproot-5.3.7/src/uproot/_util.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/behavior.py` & `uproot-5.3.7/src/uproot/behavior.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/cache.py` & `uproot-5.3.7/src/uproot/cache.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/compression.py` & `uproot-5.3.7/src/uproot/compression.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/const.py` & `uproot-5.3.7/src/uproot/const.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/containers.py` & `uproot-5.3.7/src/uproot/containers.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/deserialization.py` & `uproot-5.3.7/src/uproot/deserialization.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/dynamic.py` & `uproot-5.3.7/src/uproot/dynamic.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/exceptions.py` & `uproot-5.3.7/src/uproot/exceptions.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/extras.py` & `uproot-5.3.7/src/uproot/extras.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/model.py` & `uproot-5.3.7/src/uproot/model.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/pyroot.py` & `uproot-5.3.7/src/uproot/pyroot.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/reading.py` & `uproot-5.3.7/src/uproot/reading.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/serialization.py` & `uproot-5.3.7/src/uproot/serialization.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/streamers.py` & `uproot-5.3.7/src/uproot/streamers.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/behaviors/RooCurve.py` & `uproot-5.3.7/src/uproot/behaviors/RooCurve.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/behaviors/RooHist.py` & `uproot-5.3.7/src/uproot/behaviors/RooHist.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/behaviors/TAxis.py` & `uproot-5.3.7/src/uproot/behaviors/TAxis.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/behaviors/TBranch.py` & `uproot-5.3.7/src/uproot/behaviors/TBranch.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/behaviors/TBranchElement.py` & `uproot-5.3.7/src/uproot/behaviors/TBranchElement.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/behaviors/TGraph.py` & `uproot-5.3.7/src/uproot/behaviors/TGraph.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/behaviors/TGraphAsymmErrors.py` & `uproot-5.3.7/src/uproot/behaviors/TGraphAsymmErrors.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/behaviors/TH1.py` & `uproot-5.3.7/src/uproot/behaviors/TH1.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/behaviors/TH2.py` & `uproot-5.3.7/src/uproot/behaviors/TH2.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/behaviors/TH2Poly.py` & `uproot-5.3.7/src/uproot/behaviors/TH2Poly.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/behaviors/TH3.py` & `uproot-5.3.7/src/uproot/behaviors/TH3.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/behaviors/TParameter.py` & `uproot-5.3.7/src/uproot/behaviors/TParameter.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/behaviors/TProfile.py` & `uproot-5.3.7/src/uproot/behaviors/TProfile.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/behaviors/TProfile2D.py` & `uproot-5.3.7/src/uproot/behaviors/TProfile2D.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/behaviors/TProfile3D.py` & `uproot-5.3.7/src/uproot/behaviors/TProfile3D.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/behaviors/TTree.py` & `uproot-5.3.7/src/uproot/behaviors/TTree.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/behaviors/__init__.py` & `uproot-5.3.7/src/uproot/behaviors/__init__.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/interpretation/__init__.py` & `uproot-5.3.7/src/uproot/interpretation/__init__.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/interpretation/grouped.py` & `uproot-5.3.7/src/uproot/interpretation/grouped.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/interpretation/identify.py` & `uproot-5.3.7/src/uproot/interpretation/identify.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/interpretation/jagged.py` & `uproot-5.3.7/src/uproot/interpretation/jagged.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/interpretation/library.py` & `uproot-5.3.7/src/uproot/interpretation/library.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/interpretation/numerical.py` & `uproot-5.3.7/src/uproot/interpretation/numerical.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/interpretation/objects.py` & `uproot-5.3.7/src/uproot/interpretation/objects.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/interpretation/strings.py` & `uproot-5.3.7/src/uproot/interpretation/strings.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/language/__init__.py` & `uproot-5.3.7/src/uproot/language/__init__.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/language/python.py` & `uproot-5.3.7/src/uproot/language/python.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/models/RNTuple.py` & `uproot-5.3.7/src/uproot/models/RNTuple.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/models/TArray.py` & `uproot-5.3.7/src/uproot/models/TArray.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/models/TAtt.py` & `uproot-5.3.7/src/uproot/models/TAtt.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/models/TBasket.py` & `uproot-5.3.7/src/uproot/models/TBasket.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/models/TBranch.py` & `uproot-5.3.7/src/uproot/models/TBranch.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/models/TClonesArray.py` & `uproot-5.3.7/src/uproot/models/TClonesArray.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/models/TDatime.py` & `uproot-5.3.7/src/uproot/models/TDatime.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/models/TGraph.py` & `uproot-5.3.7/src/uproot/models/TGraph.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/models/TH.py` & `uproot-5.3.7/src/uproot/models/TH.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/models/THashList.py` & `uproot-5.3.7/src/uproot/models/THashList.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/models/TLeaf.py` & `uproot-5.3.7/src/uproot/models/TLeaf.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/models/TList.py` & `uproot-5.3.7/src/uproot/models/TList.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/models/TMatrixT.py` & `uproot-5.3.7/src/uproot/models/TMatrixT.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/models/TNamed.py` & `uproot-5.3.7/src/uproot/models/TNamed.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/models/TObjArray.py` & `uproot-5.3.7/src/uproot/models/TObjArray.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/models/TObjString.py` & `uproot-5.3.7/src/uproot/models/TObjString.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/models/TObject.py` & `uproot-5.3.7/src/uproot/models/TObject.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/models/TRef.py` & `uproot-5.3.7/src/uproot/models/TRef.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/models/TString.py` & `uproot-5.3.7/src/uproot/models/TString.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/models/TTable.py` & `uproot-5.3.7/src/uproot/models/TTable.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/models/TTime.py` & `uproot-5.3.7/src/uproot/models/TTime.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/models/TTree.py` & `uproot-5.3.7/src/uproot/models/TTree.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/models/__init__.py` & `uproot-5.3.7/src/uproot/models/__init__.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/sink/__init__.py` & `uproot-5.3.7/src/uproot/sink/__init__.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/sink/file.py` & `uproot-5.3.7/src/uproot/sink/file.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/source/__init__.py` & `uproot-5.3.7/src/uproot/source/__init__.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/source/chunk.py` & `uproot-5.3.7/src/uproot/source/chunk.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/source/cursor.py` & `uproot-5.3.7/src/uproot/source/cursor.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/source/file.py` & `uproot-5.3.7/src/uproot/source/file.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/source/fsspec.py` & `uproot-5.3.7/src/uproot/source/fsspec.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/source/futures.py` & `uproot-5.3.7/src/uproot/source/futures.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/source/http.py` & `uproot-5.3.7/src/uproot/source/http.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/source/object.py` & `uproot-5.3.7/src/uproot/source/object.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/source/s3.py` & `uproot-5.3.7/src/uproot/source/s3.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/source/xrootd.py` & `uproot-5.3.7/src/uproot/source/xrootd.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/writing/__init__.py` & `uproot-5.3.7/src/uproot/writing/__init__.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/writing/_cascade.py` & `uproot-5.3.7/src/uproot/writing/_cascade.py`

 * *Files 0% similar despite different names*

```diff
@@ -2155,16 +2155,18 @@
                 compression_code,
                 info_location,
                 info_num_bytes,
                 uuid_version,
                 uuid_bytes,
             ) = uproot.reading._file_header_fields_big.unpack(raw_bytes)
             assert units == 8
+            outversion = version - 1000000
         else:
             assert units == 4
+            outversion = version
 
         assert begin >= uproot.reading._file_header_fields_small.size
         assert free_location >= 0
         assert free_num_bytes >= 0
         assert free_num_slices_plus_1 >= 1
         assert begin_num_bytes >= 0
         assert compression_code >= 0
@@ -2179,15 +2181,15 @@
             free_num_slices_plus_1 - 1,
             begin_num_bytes,
             uproot.compression.Compression.from_code(compression_code),
             info_location,
             info_num_bytes,
             uuid.UUID(bytes=uuid_bytes),
         )
-        out._version = version - 1000000
+        out._version = outversion
         out._begin = begin
         return out
 
 
 class CascadingFile:
     """
     An object that represents an entire file, the root of the cascading-node tree.
```

### Comparing `uproot-5.3.6/src/uproot/writing/_cascadentuple.py` & `uproot-5.3.7/src/uproot/writing/_cascadentuple.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/writing/_cascadetree.py` & `uproot-5.3.7/src/uproot/writing/_cascadetree.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/writing/_dask_write.py` & `uproot-5.3.7/src/uproot/writing/_dask_write.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/writing/identify.py` & `uproot-5.3.7/src/uproot/writing/identify.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/src/uproot/writing/writable.py` & `uproot-5.3.7/src/uproot/writing/writable.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/conftest.py` & `uproot-5.3.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0001_source_class.py` & `uproot-5.3.7/tests/test_0001_source_class.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0006_notify_when_downloaded.py` & `uproot-5.3.7/tests/test_0006_notify_when_downloaded.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0007_single_chunk_interface.py` & `uproot-5.3.7/tests/test_0007_single_chunk_interface.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0008_start_interpretation.py` & `uproot-5.3.7/tests/test_0008_start_interpretation.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0009_nested_directories.py` & `uproot-5.3.7/tests/test_0009_nested_directories.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0010_start_streamers.py` & `uproot-5.3.7/tests/test_0010_start_streamers.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0011_generate_classes_from_streamers.py` & `uproot-5.3.7/tests/test_0011_generate_classes_from_streamers.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0013_rntuple_anchor.py` & `uproot-5.3.7/tests/test_0013_rntuple_anchor.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0014_all_ttree_versions.py` & `uproot-5.3.7/tests/test_0014_all_ttree_versions.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0016_interpretations.py` & `uproot-5.3.7/tests/test_0016_interpretations.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0017_multi_basket_multi_branch_fetch.py` & `uproot-5.3.7/tests/test_0017_multi_basket_multi_branch_fetch.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0018_array_fetching_interface.py` & `uproot-5.3.7/tests/test_0018_array_fetching_interface.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0022_number_of_branches.py` & `uproot-5.3.7/tests/test_0022_number_of_branches.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0023_more_interpretations_1.py` & `uproot-5.3.7/tests/test_0023_more_interpretations_1.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0023_ttree_versions.py` & `uproot-5.3.7/tests/test_0023_ttree_versions.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0029_more_string_types.py` & `uproot-5.3.7/tests/test_0029_more_string_types.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0031_test_stl_containers.py` & `uproot-5.3.7/tests/test_0031_test_stl_containers.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0033_more_interpretations_2.py` & `uproot-5.3.7/tests/test_0033_more_interpretations_2.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0034_generic_objects_in_ttrees.py` & `uproot-5.3.7/tests/test_0034_generic_objects_in_ttrees.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0035_datatype_generality.py` & `uproot-5.3.7/tests/test_0035_datatype_generality.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0038_memberwise_serialization.py` & `uproot-5.3.7/tests/test_0038_memberwise_serialization.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0043_iterate_function.py` & `uproot-5.3.7/tests/test_0043_iterate_function.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0044_concatenate_function.py` & `uproot-5.3.7/tests/test_0044_concatenate_function.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0046_histograms_bh_hist.py` & `uproot-5.3.7/tests/test_0046_histograms_bh_hist.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0053_parents_should_not_be_bases.py` & `uproot-5.3.7/tests/test_0053_parents_should_not_be_bases.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0058_detach_model_objects_from_files.py` & `uproot-5.3.7/tests/test_0058_detach_model_objects_from_files.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0067_common_entry_offsets.py` & `uproot-5.3.7/tests/test_0067_common_entry_offsets.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0081_dont_parse_colons.py` & `uproot-5.3.7/tests/test_0081_dont_parse_colons.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0087_memberwise_splitting_not_implemented_messages.py` & `uproot-5.3.7/tests/test_0087_memberwise_splitting_not_implemented_messages.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0088_read_with_http.py` & `uproot-5.3.7/tests/test_0088_read_with_http.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0099_read_from_file_object.py` & `uproot-5.3.7/tests/test_0099_read_from_file_object.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0112_fix_pandas_with_cut.py` & `uproot-5.3.7/tests/test_0112_fix_pandas_with_cut.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0118_fix_name_fetch_again.py` & `uproot-5.3.7/tests/test_0118_fix_name_fetch_again.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0167_use_the_common_histogram_interface.py` & `uproot-5.3.7/tests/test_0167_use_the_common_histogram_interface.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0173_empty_and_multiprocessing_bugs.py` & `uproot-5.3.7/tests/test_0173_empty_and_multiprocessing_bugs.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0182_complain_about_missing_files.py` & `uproot-5.3.7/tests/test_0182_complain_about_missing_files.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0220_contiguous_byte_ranges_in_http.py` & `uproot-5.3.7/tests/test_0220_contiguous_byte_ranges_in_http.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0228_read_TProfiles.py` & `uproot-5.3.7/tests/test_0228_read_TProfiles.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0240_read_TGraphAsymmErrors.py` & `uproot-5.3.7/tests/test_0240_read_TGraphAsymmErrors.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0278_specializations_for_TParameter.py` & `uproot-5.3.7/tests/test_0278_specializations_for_TParameter.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0302_pickle.py` & `uproot-5.3.7/tests/test_0302_pickle.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0303_empty_jagged_array.py` & `uproot-5.3.7/tests/test_0303_empty_jagged_array.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0320_start_working_on_ROOT_writing.py` & `uproot-5.3.7/tests/test_0320_start_working_on_ROOT_writing.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0322_writablefile_infrastructure.py` & `uproot-5.3.7/tests/test_0322_writablefile_infrastructure.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0329_update_existing_root_files.py` & `uproot-5.3.7/tests/test_0329_update_existing_root_files.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0341_manipulate_streamer_info.py` & `uproot-5.3.7/tests/test_0341_manipulate_streamer_info.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0344_writabledirectory_can_read.py` & `uproot-5.3.7/tests/test_0344_writabledirectory_can_read.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0345_bulk_copy_method.py` & `uproot-5.3.7/tests/test_0345_bulk_copy_method.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0349_write_TObjString.py` & `uproot-5.3.7/tests/test_0349_write_TObjString.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0350_read_RooCurve_RooHist.py` & `uproot-5.3.7/tests/test_0350_read_RooCurve_RooHist.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0351_write_TList.py` & `uproot-5.3.7/tests/test_0351_write_TList.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0352_write_THashList.py` & `uproot-5.3.7/tests/test_0352_write_THashList.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0384_move_behavior_of_and_fix_383.py` & `uproot-5.3.7/tests/test_0384_move_behavior_of_and_fix_383.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0398_dimensions_in_leaflist.py` & `uproot-5.3.7/tests/test_0398_dimensions_in_leaflist.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0405_write_a_histogram.py` & `uproot-5.3.7/tests/test_0405_write_a_histogram.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0406_write_a_ttree.py` & `uproot-5.3.7/tests/test_0406_write_a_ttree.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0407_read_TDatime.py` & `uproot-5.3.7/tests/test_0407_read_TDatime.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0412_write_multidimensional_numpy_to_ttree.py` & `uproot-5.3.7/tests/test_0412_write_multidimensional_numpy_to_ttree.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0414_write_jagged_arrays.py` & `uproot-5.3.7/tests/test_0414_write_jagged_arrays.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0416_writing_compressed_data.py` & `uproot-5.3.7/tests/test_0416_writing_compressed_data.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0418_read_TTable.py` & `uproot-5.3.7/tests/test_0418_read_TTable.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0420_pyroot_uproot_interoperability.py` & `uproot-5.3.7/tests/test_0420_pyroot_uproot_interoperability.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0422_hist_integration.py` & `uproot-5.3.7/tests/test_0422_hist_integration.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0438_TClonesArray_is_not_AsGrouped.py` & `uproot-5.3.7/tests/test_0438_TClonesArray_is_not_AsGrouped.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0442_regular_TClonesArray.py` & `uproot-5.3.7/tests/test_0442_regular_TClonesArray.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0472_tstreamerinfo_for_ttree.py` & `uproot-5.3.7/tests/test_0472_tstreamerinfo_for_ttree.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0475_remember_to_update_freesegments.py` & `uproot-5.3.7/tests/test_0475_remember_to_update_freesegments.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0487_implement_asdtypeinplace.py` & `uproot-5.3.7/tests/test_0487_implement_asdtypeinplace.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0498_create_leaf_branch_in_extend.py` & `uproot-5.3.7/tests/test_0498_create_leaf_branch_in_extend.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0576_unicode_in_names.py` & `uproot-5.3.7/tests/test_0576_unicode_in_names.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0578_dask_for_numpy.py` & `uproot-5.3.7/tests/test_0578_dask_for_numpy.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0580_round_trip_for_no_flow_histograms.py` & `uproot-5.3.7/tests/test_0580_round_trip_for_no_flow_histograms.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0589_explicitly_interpret_RVec_type.py` & `uproot-5.3.7/tests/test_0589_explicitly_interpret_RVec_type.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0603_dask_delayed_open.py` & `uproot-5.3.7/tests/test_0603_dask_delayed_open.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0609_num_enteries_func.py` & `uproot-5.3.7/tests/test_0609_num_enteries_func.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0610_awkward_form.py` & `uproot-5.3.7/tests/test_0610_awkward_form.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0630_rntuple_basics.py` & `uproot-5.3.7/tests/test_0630_rntuple_basics.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0637_setup_tests_for_AwkwardForth.py` & `uproot-5.3.7/tests/test_0637_setup_tests_for_AwkwardForth.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0643_reading_vector_pair_TLorentzVector_int.py` & `uproot-5.3.7/tests/test_0643_reading_vector_pair_TLorentzVector_int.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0651_implement_transformed_axis.py` & `uproot-5.3.7/tests/test_0651_implement_transformed_axis.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0652_dask_for_awkward.py` & `uproot-5.3.7/tests/test_0652_dask_for_awkward.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0662_rntuple_stl_containers.py` & `uproot-5.3.7/tests/test_0662_rntuple_stl_containers.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0692_fsspec_reading.py` & `uproot-5.3.7/tests/test_0692_fsspec_reading.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0692_fsspec_writing.py` & `uproot-5.3.7/tests/test_0692_fsspec_writing.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0700_dask_empty_arrays.py` & `uproot-5.3.7/tests/test_0700_dask_empty_arrays.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0705_rntuple_writing_metadata.py` & `uproot-5.3.7/tests/test_0705_rntuple_writing_metadata.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0755_dask_awkward_column_projection.py` & `uproot-5.3.7/tests/test_0755_dask_awkward_column_projection.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0791_protect_uproot_project_columns_from_dask_node_names.py` & `uproot-5.3.7/tests/test_0791_protect_uproot_project_columns_from_dask_node_names.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0798_DAOD_PHYSLITE.py` & `uproot-5.3.7/tests/test_0798_DAOD_PHYSLITE.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0808_fix_awkward_form_for_AsStridedObjects.py` & `uproot-5.3.7/tests/test_0808_fix_awkward_form_for_AsStridedObjects.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0816_separate_AwkwardForth_machines_by_TBranch.py` & `uproot-5.3.7/tests/test_0816_separate_AwkwardForth_machines_by_TBranch.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0832_ak_add_doc_should_also_add_to_typetracer.py` & `uproot-5.3.7/tests/test_0832_ak_add_doc_should_also_add_to_typetracer.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0840_support_tleafG.py` & `uproot-5.3.7/tests/test_0840_support_tleafG.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0841_fix_814.py` & `uproot-5.3.7/tests/test_0841_fix_814.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0844_fix_delete_hist_from_root.py` & `uproot-5.3.7/tests/test_0844_fix_delete_hist_from_root.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0876_uproot_dask_blind_steps.py` & `uproot-5.3.7/tests/test_0876_uproot_dask_blind_steps.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0911_fix_interp_array_non_numerical_objs_issue_880.py` & `uproot-5.3.7/tests/test_0911_fix_interp_array_non_numerical_objs_issue_880.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0912_fix_pandas_and_double_nested_vectors_issue_885.py` & `uproot-5.3.7/tests/test_0912_fix_pandas_and_double_nested_vectors_issue_885.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0916_read_from_s3.py` & `uproot-5.3.7/tests/test_0916_read_from_s3.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0930_expressions_in_pandas.py` & `uproot-5.3.7/tests/test_0930_expressions_in_pandas.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0940_feat_add_TLeafC_string_support.py` & `uproot-5.3.7/tests/test_0940_feat_add_TLeafC_string_support.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0962_RNTuple_update.py` & `uproot-5.3.7/tests/test_0962_RNTuple_update.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0965_inverted_axes_variances_hist_888.py` & `uproot-5.3.7/tests/test_0965_inverted_axes_variances_hist_888.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_0976_path_object_split.py` & `uproot-5.3.7/tests/test_0976_path_object_split.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_1000-write-TProfiles.py` & `uproot-5.3.7/tests/test_1000-write-TProfiles.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_1058_dask_awkward_report.py` & `uproot-5.3.7/tests/test_1058_dask_awkward_report.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_1063_dask_distributed.py` & `uproot-5.3.7/tests/test_1063_dask_distributed.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_1085_dask_write.py` & `uproot-5.3.7/tests/test_1085_dask_write.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_1114_fix_attempt_to_concatenate_numpy_with_awkward.py` & `uproot-5.3.7/tests/test_1114_fix_attempt_to_concatenate_numpy_with_awkward.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_1120_check_decompression_executor_pass_for_dask.py` & `uproot-5.3.7/tests/test_1120_check_decompression_executor_pass_for_dask.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_1127_fix_allow_colon_in_key_names.py` & `uproot-5.3.7/tests/test_1127_fix_allow_colon_in_key_names.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_1146_split_ranges_for_large_files_over_http.py` & `uproot-5.3.7/tests/test_1146_split_ranges_for_large_files_over_http.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_1154_classof_using_relative_path.py` & `uproot-5.3.7/tests/test_1154_classof_using_relative_path.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_1160_std_string_in_TDirectory.py` & `uproot-5.3.7/tests/test_1160_std_string_in_TDirectory.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_1180_read_free_floating_vector_issue_1179.py` & `uproot-5.3.7/tests/test_1180_read_free_floating_vector_issue_1179.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_1181_support_for_stl_list.py` & `uproot-5.3.7/tests/test_1181_support_for_stl_list.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_1182_add_support_for_bitset.py` & `uproot-5.3.7/tests/test_1182_add_support_for_bitset.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_1183_ttime_custom.py` & `uproot-5.3.7/tests/test_1183_ttime_custom.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_1186_dtype_might_raise_ValueError.py` & `uproot-5.3.7/tests/test_1186_dtype_might_raise_ValueError.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_1189_dask_failing_on_duplicate_keys.py` & `uproot-5.3.7/tests/test_1189_dask_failing_on_duplicate_keys.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_1191_rntuple_fixes.py` & `uproot-5.3.7/tests/test_1191_rntuple_fixes.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/test_1207_fix_title_of_TBranch_with_counter.py` & `uproot-5.3.7/tests/test_1207_fix_title_of_TBranch_with_counter.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/tests/samples/h_dynamic.pkl` & `uproot-5.3.7/tests/samples/h_dynamic.pkl`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/.gitignore` & `uproot-5.3.7/.gitignore`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/LICENSE` & `uproot-5.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/README.md` & `uproot-5.3.7/README.md`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/pyproject.toml` & `uproot-5.3.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `uproot-5.3.6/PKG-INFO` & `uproot-5.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: uproot
-Version: 5.3.6
+Version: 5.3.7
 Summary: ROOT I/O in pure Python and NumPy.
 Project-URL: Download, https://github.com/scikit-hep/uproot5/releases
 Project-URL: Homepage, https://github.com/scikit-hep/uproot5
 Author-email: Jim Pivarski <pivarski@princeton.edu>
 License-Expression: BSD-3-Clause
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
```

