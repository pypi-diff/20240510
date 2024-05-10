# Comparing `tmp/spyglass_neuro-0.5.2.tar.gz` & `tmp/spyglass_neuro-0.5.2a1.tar.gz`

## Comparing `spyglass_neuro-0.5.2.tar` & `spyglass_neuro-0.5.2a1.tar`

### file list

```diff
@@ -1,289 +1,289 @@
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/.gitattributes
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/.markdownlint.yaml
--rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     9432 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/CHANGELOG.md
--rw-r--r--   0        0        0     5933 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/CITATION.cff
--rw-r--r--   0        0        0     5490 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/MANIFEST.in
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/dj_local_conf_example.json
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/environment.yml
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/environment_dlc.yml
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/setup.cfg
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/.github/pull_request_template.md
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/.github/workflows/lint.yml
--rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/.github/workflows/publish-docs.yml
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/.github/workflows/test-conda.yml
--rw-r--r--   0        0        0     2861 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/.github/workflows/test-package-build.yml
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/.vscode/extensions.json
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/.vscode/settings.json
--rwxr-xr-x   0        0        0      336 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/config/add_dj_collaborator.py
--rwxr-xr-x   0        0        0      335 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/config/add_dj_guest.py
--rwxr-xr-x   0        0        0      326 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/config/add_dj_module.py
--rwxr-xr-x   0        0        0      351 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/config/add_dj_user.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/config/datajoint_user_config.yml
--rwxr-xr-x   0        0        0      678 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/config/dj_config.py
--rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/docs/README.md
--rwxr-xr-x   0        0        0     2190 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/docs/build-docs.sh
--rw-r--r--   0        0        0     4349 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/docs/mkdocs.yml
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/docs/overrides/nav.html
--rw-r--r--   0        0        0     9683 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/docs/src/contribute.md
--rw-r--r--   0        0        0     4517 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/docs/src/index.md
--rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/docs/src/installation.md
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/docs/src/api/index.md
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/docs/src/api/make_pages.py
--rw-r--r--   0        0        0   297397 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/docs/src/images/FrankLab.png
--rw-r--r--   0        0        0    75394 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/docs/src/images/Spyglass.png
--rw-r--r--   0        0        0    12413 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/docs/src/images/Spyglass.svg
--rw-r--r--   0        0        0    52116 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/docs/src/images/fig1.png
--rw-r--r--   0        0        0    98482 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/docs/src/images/merge_diagram.png
--rw-r--r--   0        0        0     7495 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/docs/src/misc/database_management.md
--rw-r--r--   0        0        0     5366 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/docs/src/misc/export.md
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/docs/src/misc/figurl_views.md
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/docs/src/misc/index.md
--rw-r--r--   0        0        0     4287 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/docs/src/misc/insert_data.md
--rw-r--r--   0        0        0     3586 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/docs/src/misc/merge_tables.md
--rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/docs/src/misc/mixin.md
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/docs/src/misc/session_groups.md
--rw-r--r--   0        0        0     2840 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/docs/src/stylesheets/extra.css
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/examples/cli_examples/artifactdetectionparameters_default.yaml
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/examples/cli_examples/artifactdetectionparameters_none.yaml
--rwxr-xr-x   0        0        0      305 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/examples/cli_examples/create_session_group.py
--rwxr-xr-x   0        0        0      159 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/examples/cli_examples/create_spike_sorting_recording.sh
--rwxr-xr-x   0        0        0      111 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/examples/cli_examples/create_spike_sorting_recording_view.sh
--rwxr-xr-x   0        0        0      101 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/examples/cli_examples/create_spike_sorting_view.sh
--rwxr-xr-x   0        0        0       73 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/examples/cli_examples/create_spyglass_view.sh
--rwxr-xr-x   0        0        0      270 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/examples/cli_examples/insert_artifact_detection_parameters.sh
--rwxr-xr-x   0        0        0      114 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/examples/cli_examples/insert_lab_member.sh
--rwxr-xr-x   0        0        0      105 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/examples/cli_examples/insert_lab_team.sh
--rwxr-xr-x   0        0        0      137 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/examples/cli_examples/insert_lab_team_member.sh
--rwxr-xr-x   0        0        0      101 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/examples/cli_examples/insert_session.sh
--rwxr-xr-x   0        0        0      653 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/examples/cli_examples/insert_sort_interval.py
--rwxr-xr-x   0        0        0      159 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/examples/cli_examples/insert_spike_sorter_parameters.sh
--rwxr-xr-x   0        0        0      195 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/examples/cli_examples/insert_spike_sorting_preprocessing_parameters.sh
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/examples/cli_examples/labmember.yaml
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/examples/cli_examples/labteammember.yaml
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/examples/cli_examples/parameters.yaml
--rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/examples/cli_examples/readme.md
--rwxr-xr-x   0        0        0      136 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/examples/cli_examples/run_spike_sorting.sh
--rwxr-xr-x   0        0        0      343 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/examples/cli_examples/set_sort_groups_by_shank.py
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/examples/cli_examples/spikesorterparameters_default.yaml
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/examples/cli_examples/spikesortingpreprocessingparameters.yaml
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/examples/cli_examples/team.yaml
--rwxr-xr-x   0        0        0      152 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/examples/cli_examples/update_lab_team_description.py
--rw-r--r--   0        0        0     5353 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/examples/config_yaml/entries.yaml
--rw-r--r--   0        0        0    53048 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/examples/config_yaml/sub-AppleBottom_ses-AppleBottom-DY20-g3_behavior+ecephys_spyglass_config.yaml
--rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/franklab_scripts/alter_tables.py
--rwxr-xr-x   0        0        0      701 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/franklab_scripts/nightly_cleanup.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/franklab_scripts/sort.py
--rw-r--r--   0        0        0    11234 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/00_Setup.ipynb
--rw-r--r--   0        0        0   128150 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/01_Insert_Data.ipynb
--rw-r--r--   0        0        0    47991 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/02_Data_Sync.ipynb
--rw-r--r--   0        0        0  2174485 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/03_Merge_Tables.ipynb
--rw-r--r--   0        0        0    10342 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/04_PopulateConfigFile.ipynb
--rw-r--r--   0        0        0    27301 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/05_Export.ipynb
--rw-r--r--   0        0        0   137862 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/10_Spike_SortingV0.ipynb
--rw-r--r--   0        0        0    99395 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/10_Spike_SortingV1.ipynb
--rw-r--r--   0        0        0   699515 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/20_Position_Trodes.ipynb
--rw-r--r--   0        0        0    84430 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/21_DLC.ipynb
--rw-r--r--   0        0        0    31324 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/22_DLC_Loop.ipynb
--rw-r--r--   0        0        0   877085 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/24_Linearization.ipynb
--rw-r--r--   0        0        0   232187 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/30_LFP.ipynb
--rw-r--r--   0        0        0   520960 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/31_Theta.ipynb
--rw-r--r--   0        0        0   404028 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/32_Ripple_Detection.ipynb
--rw-r--r--   0        0        0    92888 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/40_Extracting_Clusterless_Waveform_Features.ipynb
--rw-r--r--   0        0        0   178894 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/41_Decoding_Clusterless.ipynb
--rw-r--r--   0        0        0    75214 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/42_Decoding_SortedSpikes.ipynb
--rw-r--r--   0        0        0   129019 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/50_MUA_Detection.ipynb
--rw-r--r--   0        0        0     3259 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/README.md
--rw-r--r--   0        0        0     7797 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/py_scripts/00_Setup.py
--rw-r--r--   0        0        0    15501 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/py_scripts/01_Insert_Data.py
--rw-r--r--   0        0        0    11935 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/py_scripts/02_Data_Sync.py
--rw-r--r--   0        0        0     7198 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/py_scripts/03_Merge_Tables.py
--rw-r--r--   0        0        0     7737 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/py_scripts/04_PopulateConfigFile.py
--rw-r--r--   0        0        0     6013 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/py_scripts/05_Export.py
--rw-r--r--   0        0        0    21388 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/py_scripts/10_Spike_SortingV0.py
--rw-r--r--   0        0        0    13684 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/py_scripts/10_Spike_SortingV1.py
--rw-r--r--   0        0        0    12592 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/py_scripts/20_Position_Trodes.py
--rw-r--r--   0        0        0    26539 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/py_scripts/21_DLC.py
--rw-r--r--   0        0        0    19409 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/py_scripts/22_DLC_Loop.py
--rw-r--r--   0        0        0     9427 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/py_scripts/24_Linearization.py
--rw-r--r--   0        0        0     9414 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/py_scripts/30_LFP.py
--rw-r--r--   0        0        0     5426 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/py_scripts/31_Theta.py
--rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/py_scripts/32_Ripple_Detection.py
--rw-r--r--   0        0        0    11057 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/py_scripts/40_Extracting_Clusterless_Waveform_Features.py
--rw-r--r--   0        0        0    18172 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/py_scripts/41_Decoding_Clusterless.py
--rw-r--r--   0        0        0    10272 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/py_scripts/41_Extracting_Clusterless_Waveform_Features.py
--rw-r--r--   0        0        0    17943 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/py_scripts/42_Decoding_Clusterless.py
--rw-r--r--   0        0        0     6003 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/py_scripts/42_Decoding_SortedSpikes.py
--rw-r--r--   0        0        0     5740 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/py_scripts/43_Decoding_SortedSpikes.py
--rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/py_scripts/51_MUA_Detection.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/_version.py
--rw-r--r--   0        0        0    20126 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/settings.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/cli/__init__.py
--rw-r--r--   0        0        0    14650 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/cli/cli.py
--rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/common/__init__.py
--rw-r--r--   0        0        0    22090 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/common/common_behav.py
--rw-r--r--   0        0        0    26420 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/common/common_device.py
--rw-r--r--   0        0        0     4126 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/common/common_dio.py
--rw-r--r--   0        0        0    35128 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/common/common_ephys.py
--rw-r--r--   0        0        0    19143 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/common/common_filter.py
--rw-r--r--   0        0        0    17246 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/common/common_interval.py
--rw-r--r--   0        0        0     8823 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/common/common_lab.py
--rw-r--r--   0        0        0    28397 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/common/common_nwbfile.py
--rw-r--r--   0        0        0    27415 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/common/common_position.py
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/common/common_region.py
--rw-r--r--   0        0        0    11650 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/common/common_ripple.py
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/common/common_sensors.py
--rw-r--r--   0        0        0     9750 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/common/common_session.py
--rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/common/common_subject.py
--rw-r--r--   0        0        0     7854 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/common/common_task.py
--rw-r--r--   0        0        0    13894 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/common/common_usage.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/common/errors.py
--rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/common/populate_all_common.py
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/common/signal_processing.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/common/prepopulate/__init__.py
--rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/common/prepopulate/prepopulate.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/data_import/__init__.py
--rw-r--r--   0        0        0     5478 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/data_import/insert_sessions.py
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/decoding/__init__.py
--rw-r--r--   0        0        0     5833 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/decoding/decoding_merge.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/decoding/v0/__init__.py
--rw-r--r--   0        0        0    26920 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/decoding/v0/clusterless.py
--rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/decoding/v0/core.py
--rw-r--r--   0        0        0     6521 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/decoding/v0/dj_decoder_conversion.py
--rw-r--r--   0        0        0    14064 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/decoding/v0/sorted_spikes.py
--rw-r--r--   0        0        0    20617 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/decoding/v0/visualization.py
--rw-r--r--   0        0        0     2793 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/decoding/v0/visualization_1D_view.py
--rw-r--r--   0        0        0    11050 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/decoding/v0/visualization_2D_view.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/decoding/v1/__init__.py
--rw-r--r--   0        0        0    18008 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/decoding/v1/clusterless.py
--rw-r--r--   0        0        0     3939 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/decoding/v1/core.py
--rw-r--r--   0        0        0     6436 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/decoding/v1/dj_decoder_conversion.py
--rw-r--r--   0        0        0    16300 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/decoding/v1/sorted_spikes.py
--rw-r--r--   0        0        0    12380 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/decoding/v1/waveform_features.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/lfp/__init__.py
--rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/lfp/lfp_electrode.py
--rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/lfp/lfp_imported.py
--rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/lfp/lfp_merge.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/lfp/analysis/__init__.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/lfp/analysis/v1/__init__.py
--rw-r--r--   0        0        0    18049 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/lfp/analysis/v1/lfp_band.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/lfp/v1/__init__.py
--rw-r--r--   0        0        0     7746 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/lfp/v1/lfp.py
--rw-r--r--   0        0        0     8162 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/lfp/v1/lfp_artifact.py
--rw-r--r--   0        0        0     5332 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/lfp/v1/lfp_artifact_MAD_detection.py
--rw-r--r--   0        0        0    10010 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/lfp/v1/lfp_artifact_difference_detection.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/linearization/__init__.py
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/linearization/merge.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/linearization/v0/__init__.py
--rw-r--r--   0        0        0     6369 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/linearization/v0/main.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/linearization/v1/__init__.py
--rw-r--r--   0        0        0     6499 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/linearization/v1/main.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/lock/__init__.py
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/lock/file_lock.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/mua/__init__.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/mua/v1/__init__.py
--rw-r--r--   0        0        0     6690 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/mua/v1/mua.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/position/__init__.py
--rw-r--r--   0        0        0     8485 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/position/position_merge.py
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/position/v1/__init__.py
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/position/v1/dlc_decorators.py
--rw-r--r--   0        0        0     9140 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/position/v1/dlc_reader.py
--rw-r--r--   0        0        0    45570 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/position/v1/dlc_utils.py
--rw-r--r--   0        0        0    28739 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/position/v1/position_dlc_centroid.py
--rw-r--r--   0        0        0     4384 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/position/v1/position_dlc_cohort.py
--rw-r--r--   0        0        0    11752 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/position/v1/position_dlc_model.py
--rw-r--r--   0        0        0     9110 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/position/v1/position_dlc_orient.py
--rw-r--r--   0        0        0    16388 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/position/v1/position_dlc_pose_estimation.py
--rw-r--r--   0        0        0    17289 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/position/v1/position_dlc_position.py
--rw-r--r--   0        0        0    21769 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/position/v1/position_dlc_project.py
--rw-r--r--   0        0        0    15801 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/position/v1/position_dlc_selection.py
--rw-r--r--   0        0        0     9551 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/position/v1/position_dlc_training.py
--rw-r--r--   0        0        0    14802 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/position/v1/position_trodes_position.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/ripple/__init__.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/ripple/v1/__init__.py
--rw-r--r--   0        0        0    17519 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/ripple/v1/ripple.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/sharing/__init__.py
--rw-r--r--   0        0        0     9098 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/sharing/sharing_kachery.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/spikesorting/__init__.py
--rw-r--r--   0        0        0     4902 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/spikesorting/imported.py
--rw-r--r--   0        0        0     8283 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/spikesorting/spikesorting_merge.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/spikesorting/analysis/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/spikesorting/analysis/v1/__init__.py
--rw-r--r--   0        0        0     6743 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/spikesorting/analysis/v1/group.py
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/spikesorting/v0/__init__.py
--rw-r--r--   0        0        0     6980 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/spikesorting/v0/curation_figurl.py
--rw-r--r--   0        0        0     4518 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/spikesorting/v0/merged_sorting_extractor.py
--rw-r--r--   0        0        0     7577 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/spikesorting/v0/sortingview.py
--rw-r--r--   0        0        0     4992 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/spikesorting/v0/sortingview_helper_fn.py
--rw-r--r--   0        0        0    15520 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/spikesorting/v0/spikesorting_artifact.py
--rw-r--r--   0        0        0    41121 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/spikesorting/v0/spikesorting_curation.py
--rw-r--r--   0        0        0    11481 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/spikesorting/v0/spikesorting_populator.py
--rw-r--r--   0        0        0    23579 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/spikesorting/v0/spikesorting_recording.py
--rw-r--r--   0        0        0    10095 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/spikesorting/v0/spikesorting_sorting.py
--rw-r--r--   0        0        0     3436 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/spikesorting/v0/figurl_views/SpikeSortingRecordingView.py
--rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/spikesorting/v0/figurl_views/SpikeSortingView.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/spikesorting/v0/figurl_views/__init__.py
--rw-r--r--   0        0        0    11393 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/spikesorting/v0/figurl_views/prepare_spikesortingview_data.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/spikesorting/v1/__init__.py
--rw-r--r--   0        0        0    14842 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/spikesorting/v1/artifact.py
--rw-r--r--   0        0        0    16347 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/spikesorting/v1/curation.py
--rw-r--r--   0        0        0     9424 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/spikesorting/v1/figurl_curation.py
--rw-r--r--   0        0        0    19431 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/spikesorting/v1/metric_curation.py
--rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/spikesorting/v1/metric_utils.py
--rw-r--r--   0        0        0    33193 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/spikesorting/v1/recording.py
--rw-r--r--   0        0        0    13943 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/spikesorting/v1/sorting.py
--rw-r--r--   0        0        0     3764 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/spikesorting/v1/utils.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/utils/__init__.py
--rwxr-xr-x   0        0        0     7345 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/utils/database_settings.py
--rw-r--r--   0        0        0    13826 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/utils/dj_chains.py
--rw-r--r--   0        0        0    12976 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/utils/dj_graph.py
--rw-r--r--   0        0        0     8713 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/utils/dj_helper_fn.py
--rw-r--r--   0        0        0    30084 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/utils/dj_merge_tables.py
--rw-r--r--   0        0        0    27533 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/utils/dj_mixin.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/utils/logging.py
--rw-r--r--   0        0        0    17753 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/utils/nwb_helper_fn.py
--rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/tests/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/tests/__init__.py
--rw-r--r--   0        0        0    12154 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/tests/conftest.py
--rw-r--r--   0        0        0     6992 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/tests/container.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/tests/common/__init__.py
--rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/tests/common/conftest.py
--rw-r--r--   0        0        0     4116 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/tests/common/test_behav.py
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/tests/common/test_device.py
--rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/tests/common/test_dio.py
--rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/tests/common/test_ephys.py
--rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/tests/common/test_filter.py
--rw-r--r--   0        0        0     7408 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/tests/common/test_insert.py
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/tests/common/test_interval.py
--rw-r--r--   0        0        0     7476 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/tests/common/test_interval_helpers.py
--rw-r--r--   0        0        0     3112 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/tests/common/test_lab.py
--rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/tests/common/test_nwbfile.py
--rw-r--r--   0        0        0     4324 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/tests/common/test_position.py
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/tests/common/test_region.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/tests/common/test_ripple.py
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/tests/common/test_sensors.py
--rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/tests/common/test_session.py
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/tests/data_import/__init__.py
--rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/tests/data_import/test_insert_sessions.py
--rw-r--r--   0        0        0     6994 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/tests/lfp/conftest.py
--rw-r--r--   0        0        0     3654 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/tests/lfp/test_lfp.py
--rw-r--r--   0        0        0     3402 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/tests/linearization/conftest.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/tests/linearization/test_lin.py
--rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/tests/position/test_trodes.py
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/tests/utils/conftest.py
--rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/tests/utils/test_chains.py
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/tests/utils/test_db_settings.py
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/tests/utils/test_dj_helper_fn.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/tests/utils/test_logging.py
--rw-r--r--   0        0        0     2227 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/tests/utils/test_merge.py
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/tests/utils/test_mixin.py
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/tests/utils/test_nwb_helper_fn.py
--rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/LICENSE
--rw-r--r--   0        0        0     5636 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/README.md
--rw-r--r--   0        0        0     4547 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     9448 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/.gitattributes
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/.markdownlint.yaml
+-rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     9733 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/CHANGELOG.md
+-rw-r--r--   0        0        0     5933 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/CITATION.cff
+-rw-r--r--   0        0        0     5490 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/MANIFEST.in
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/dj_local_conf_example.json
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/environment.yml
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/environment_dlc.yml
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/setup.cfg
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/.github/pull_request_template.md
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/.github/workflows/lint.yml
+-rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/.github/workflows/publish-docs.yml
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/.github/workflows/test-conda.yml
+-rw-r--r--   0        0        0     2824 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/.github/workflows/test-package-build.yml
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/.vscode/extensions.json
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/.vscode/settings.json
+-rwxr-xr-x   0        0        0      336 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/config/add_dj_collaborator.py
+-rwxr-xr-x   0        0        0      335 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/config/add_dj_guest.py
+-rwxr-xr-x   0        0        0      326 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/config/add_dj_module.py
+-rwxr-xr-x   0        0        0      351 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/config/add_dj_user.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/config/datajoint_user_config.yml
+-rwxr-xr-x   0        0        0      678 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/config/dj_config.py
+-rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/docs/README.md
+-rwxr-xr-x   0        0        0     2190 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/docs/build-docs.sh
+-rw-r--r--   0        0        0     4349 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/docs/mkdocs.yml
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/docs/overrides/nav.html
+-rw-r--r--   0        0        0     9683 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/docs/src/contribute.md
+-rw-r--r--   0        0        0     4517 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/docs/src/index.md
+-rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/docs/src/installation.md
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/docs/src/api/index.md
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/docs/src/api/make_pages.py
+-rw-r--r--   0        0        0   297397 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/docs/src/images/FrankLab.png
+-rw-r--r--   0        0        0    75394 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/docs/src/images/Spyglass.png
+-rw-r--r--   0        0        0    12413 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/docs/src/images/Spyglass.svg
+-rw-r--r--   0        0        0    52116 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/docs/src/images/fig1.png
+-rw-r--r--   0        0        0    98482 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/docs/src/images/merge_diagram.png
+-rw-r--r--   0        0        0     7495 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/docs/src/misc/database_management.md
+-rw-r--r--   0        0        0     5366 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/docs/src/misc/export.md
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/docs/src/misc/figurl_views.md
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/docs/src/misc/index.md
+-rw-r--r--   0        0        0     4287 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/docs/src/misc/insert_data.md
+-rw-r--r--   0        0        0     3586 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/docs/src/misc/merge_tables.md
+-rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/docs/src/misc/mixin.md
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/docs/src/misc/session_groups.md
+-rw-r--r--   0        0        0     2840 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/docs/src/stylesheets/extra.css
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/examples/cli_examples/artifactdetectionparameters_default.yaml
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/examples/cli_examples/artifactdetectionparameters_none.yaml
+-rwxr-xr-x   0        0        0      305 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/examples/cli_examples/create_session_group.py
+-rwxr-xr-x   0        0        0      159 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/examples/cli_examples/create_spike_sorting_recording.sh
+-rwxr-xr-x   0        0        0      111 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/examples/cli_examples/create_spike_sorting_recording_view.sh
+-rwxr-xr-x   0        0        0      101 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/examples/cli_examples/create_spike_sorting_view.sh
+-rwxr-xr-x   0        0        0       73 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/examples/cli_examples/create_spyglass_view.sh
+-rwxr-xr-x   0        0        0      270 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/examples/cli_examples/insert_artifact_detection_parameters.sh
+-rwxr-xr-x   0        0        0      114 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/examples/cli_examples/insert_lab_member.sh
+-rwxr-xr-x   0        0        0      105 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/examples/cli_examples/insert_lab_team.sh
+-rwxr-xr-x   0        0        0      137 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/examples/cli_examples/insert_lab_team_member.sh
+-rwxr-xr-x   0        0        0      101 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/examples/cli_examples/insert_session.sh
+-rwxr-xr-x   0        0        0      653 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/examples/cli_examples/insert_sort_interval.py
+-rwxr-xr-x   0        0        0      159 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/examples/cli_examples/insert_spike_sorter_parameters.sh
+-rwxr-xr-x   0        0        0      195 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/examples/cli_examples/insert_spike_sorting_preprocessing_parameters.sh
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/examples/cli_examples/labmember.yaml
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/examples/cli_examples/labteammember.yaml
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/examples/cli_examples/parameters.yaml
+-rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/examples/cli_examples/readme.md
+-rwxr-xr-x   0        0        0      136 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/examples/cli_examples/run_spike_sorting.sh
+-rwxr-xr-x   0        0        0      343 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/examples/cli_examples/set_sort_groups_by_shank.py
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/examples/cli_examples/spikesorterparameters_default.yaml
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/examples/cli_examples/spikesortingpreprocessingparameters.yaml
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/examples/cli_examples/team.yaml
+-rwxr-xr-x   0        0        0      152 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/examples/cli_examples/update_lab_team_description.py
+-rw-r--r--   0        0        0     5353 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/examples/config_yaml/entries.yaml
+-rw-r--r--   0        0        0    53048 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/examples/config_yaml/sub-AppleBottom_ses-AppleBottom-DY20-g3_behavior+ecephys_spyglass_config.yaml
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/franklab_scripts/alter_tables.py
+-rwxr-xr-x   0        0        0      701 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/franklab_scripts/nightly_cleanup.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/franklab_scripts/sort.py
+-rw-r--r--   0        0        0    11234 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/notebooks/00_Setup.ipynb
+-rw-r--r--   0        0        0   128150 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/notebooks/01_Insert_Data.ipynb
+-rw-r--r--   0        0        0    47991 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/notebooks/02_Data_Sync.ipynb
+-rw-r--r--   0        0        0  2174485 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/notebooks/03_Merge_Tables.ipynb
+-rw-r--r--   0        0        0    10342 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/notebooks/04_PopulateConfigFile.ipynb
+-rw-r--r--   0        0        0    27301 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/notebooks/05_Export.ipynb
+-rw-r--r--   0        0        0   137862 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/notebooks/10_Spike_SortingV0.ipynb
+-rw-r--r--   0        0        0    99395 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/notebooks/10_Spike_SortingV1.ipynb
+-rw-r--r--   0        0        0   699515 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/notebooks/20_Position_Trodes.ipynb
+-rw-r--r--   0        0        0    84430 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/notebooks/21_DLC.ipynb
+-rw-r--r--   0        0        0    31324 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/notebooks/22_DLC_Loop.ipynb
+-rw-r--r--   0        0        0   877085 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/notebooks/24_Linearization.ipynb
+-rw-r--r--   0        0        0   232187 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/notebooks/30_LFP.ipynb
+-rw-r--r--   0        0        0   520960 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/notebooks/31_Theta.ipynb
+-rw-r--r--   0        0        0   404028 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/notebooks/32_Ripple_Detection.ipynb
+-rw-r--r--   0        0        0    92888 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/notebooks/40_Extracting_Clusterless_Waveform_Features.ipynb
+-rw-r--r--   0        0        0   178894 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/notebooks/41_Decoding_Clusterless.ipynb
+-rw-r--r--   0        0        0    75214 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/notebooks/42_Decoding_SortedSpikes.ipynb
+-rw-r--r--   0        0        0   129019 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/notebooks/50_MUA_Detection.ipynb
+-rw-r--r--   0        0        0     3259 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/notebooks/README.md
+-rw-r--r--   0        0        0     7797 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/notebooks/py_scripts/00_Setup.py
+-rw-r--r--   0        0        0    15501 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/notebooks/py_scripts/01_Insert_Data.py
+-rw-r--r--   0        0        0    11935 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/notebooks/py_scripts/02_Data_Sync.py
+-rw-r--r--   0        0        0     7198 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/notebooks/py_scripts/03_Merge_Tables.py
+-rw-r--r--   0        0        0     7737 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/notebooks/py_scripts/04_PopulateConfigFile.py
+-rw-r--r--   0        0        0     6013 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/notebooks/py_scripts/05_Export.py
+-rw-r--r--   0        0        0    21388 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/notebooks/py_scripts/10_Spike_SortingV0.py
+-rw-r--r--   0        0        0    13684 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/notebooks/py_scripts/10_Spike_SortingV1.py
+-rw-r--r--   0        0        0    12592 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/notebooks/py_scripts/20_Position_Trodes.py
+-rw-r--r--   0        0        0    26539 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/notebooks/py_scripts/21_DLC.py
+-rw-r--r--   0        0        0    19409 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/notebooks/py_scripts/22_DLC_Loop.py
+-rw-r--r--   0        0        0     9427 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/notebooks/py_scripts/24_Linearization.py
+-rw-r--r--   0        0        0     9414 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/notebooks/py_scripts/30_LFP.py
+-rw-r--r--   0        0        0     5426 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/notebooks/py_scripts/31_Theta.py
+-rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/notebooks/py_scripts/32_Ripple_Detection.py
+-rw-r--r--   0        0        0    11057 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/notebooks/py_scripts/40_Extracting_Clusterless_Waveform_Features.py
+-rw-r--r--   0        0        0    18172 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/notebooks/py_scripts/41_Decoding_Clusterless.py
+-rw-r--r--   0        0        0    10272 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/notebooks/py_scripts/41_Extracting_Clusterless_Waveform_Features.py
+-rw-r--r--   0        0        0    17943 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/notebooks/py_scripts/42_Decoding_Clusterless.py
+-rw-r--r--   0        0        0     6003 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/notebooks/py_scripts/42_Decoding_SortedSpikes.py
+-rw-r--r--   0        0        0     5740 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/notebooks/py_scripts/43_Decoding_SortedSpikes.py
+-rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/notebooks/py_scripts/51_MUA_Detection.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/__init__.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/_version.py
+-rw-r--r--   0        0        0    20126 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/settings.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/cli/__init__.py
+-rw-r--r--   0        0        0    14650 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/cli/cli.py
+-rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/common/__init__.py
+-rw-r--r--   0        0        0    22090 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/common/common_behav.py
+-rw-r--r--   0        0        0    26420 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/common/common_device.py
+-rw-r--r--   0        0        0     4126 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/common/common_dio.py
+-rw-r--r--   0        0        0    35128 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/common/common_ephys.py
+-rw-r--r--   0        0        0    19143 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/common/common_filter.py
+-rw-r--r--   0        0        0    17246 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/common/common_interval.py
+-rw-r--r--   0        0        0     8823 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/common/common_lab.py
+-rw-r--r--   0        0        0    28397 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/common/common_nwbfile.py
+-rw-r--r--   0        0        0    27415 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/common/common_position.py
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/common/common_region.py
+-rw-r--r--   0        0        0    11650 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/common/common_ripple.py
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/common/common_sensors.py
+-rw-r--r--   0        0        0     9750 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/common/common_session.py
+-rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/common/common_subject.py
+-rw-r--r--   0        0        0     7854 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/common/common_task.py
+-rw-r--r--   0        0        0    13894 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/common/common_usage.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/common/errors.py
+-rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/common/populate_all_common.py
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/common/signal_processing.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/common/prepopulate/__init__.py
+-rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/common/prepopulate/prepopulate.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/data_import/__init__.py
+-rw-r--r--   0        0        0     5478 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/data_import/insert_sessions.py
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/decoding/__init__.py
+-rw-r--r--   0        0        0     5833 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/decoding/decoding_merge.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/decoding/v0/__init__.py
+-rw-r--r--   0        0        0    26920 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/decoding/v0/clusterless.py
+-rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/decoding/v0/core.py
+-rw-r--r--   0        0        0     6521 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/decoding/v0/dj_decoder_conversion.py
+-rw-r--r--   0        0        0    14064 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/decoding/v0/sorted_spikes.py
+-rw-r--r--   0        0        0    20617 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/decoding/v0/visualization.py
+-rw-r--r--   0        0        0     2793 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/decoding/v0/visualization_1D_view.py
+-rw-r--r--   0        0        0    11050 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/decoding/v0/visualization_2D_view.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/decoding/v1/__init__.py
+-rw-r--r--   0        0        0    18022 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/decoding/v1/clusterless.py
+-rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/decoding/v1/core.py
+-rw-r--r--   0        0        0     6436 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/decoding/v1/dj_decoder_conversion.py
+-rw-r--r--   0        0        0    16300 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/decoding/v1/sorted_spikes.py
+-rw-r--r--   0        0        0    12380 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/decoding/v1/waveform_features.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/lfp/__init__.py
+-rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/lfp/lfp_electrode.py
+-rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/lfp/lfp_imported.py
+-rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/lfp/lfp_merge.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/lfp/analysis/__init__.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/lfp/analysis/v1/__init__.py
+-rw-r--r--   0        0        0    18049 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/lfp/analysis/v1/lfp_band.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/lfp/v1/__init__.py
+-rw-r--r--   0        0        0     7746 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/lfp/v1/lfp.py
+-rw-r--r--   0        0        0     8162 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/lfp/v1/lfp_artifact.py
+-rw-r--r--   0        0        0     5332 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/lfp/v1/lfp_artifact_MAD_detection.py
+-rw-r--r--   0        0        0    10010 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/lfp/v1/lfp_artifact_difference_detection.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/linearization/__init__.py
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/linearization/merge.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/linearization/v0/__init__.py
+-rw-r--r--   0        0        0     6369 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/linearization/v0/main.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/linearization/v1/__init__.py
+-rw-r--r--   0        0        0     6499 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/linearization/v1/main.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/lock/__init__.py
+-rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/lock/file_lock.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/mua/__init__.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/mua/v1/__init__.py
+-rw-r--r--   0        0        0     6690 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/mua/v1/mua.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/position/__init__.py
+-rw-r--r--   0        0        0     8485 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/position/position_merge.py
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/position/v1/__init__.py
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/position/v1/dlc_decorators.py
+-rw-r--r--   0        0        0     9140 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/position/v1/dlc_reader.py
+-rw-r--r--   0        0        0    45570 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/position/v1/dlc_utils.py
+-rw-r--r--   0        0        0    28739 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/position/v1/position_dlc_centroid.py
+-rw-r--r--   0        0        0     4384 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/position/v1/position_dlc_cohort.py
+-rw-r--r--   0        0        0    11752 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/position/v1/position_dlc_model.py
+-rw-r--r--   0        0        0     9110 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/position/v1/position_dlc_orient.py
+-rw-r--r--   0        0        0    16388 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/position/v1/position_dlc_pose_estimation.py
+-rw-r--r--   0        0        0    17289 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/position/v1/position_dlc_position.py
+-rw-r--r--   0        0        0    21769 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/position/v1/position_dlc_project.py
+-rw-r--r--   0        0        0    15801 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/position/v1/position_dlc_selection.py
+-rw-r--r--   0        0        0     9551 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/position/v1/position_dlc_training.py
+-rw-r--r--   0        0        0    14802 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/position/v1/position_trodes_position.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/ripple/__init__.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/ripple/v1/__init__.py
+-rw-r--r--   0        0        0    17519 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/ripple/v1/ripple.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/sharing/__init__.py
+-rw-r--r--   0        0        0     9098 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/sharing/sharing_kachery.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/spikesorting/__init__.py
+-rw-r--r--   0        0        0     4902 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/spikesorting/imported.py
+-rw-r--r--   0        0        0     8283 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/spikesorting/spikesorting_merge.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/spikesorting/analysis/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/spikesorting/analysis/v1/__init__.py
+-rw-r--r--   0        0        0     6757 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/spikesorting/analysis/v1/group.py
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/spikesorting/v0/__init__.py
+-rw-r--r--   0        0        0     6980 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/spikesorting/v0/curation_figurl.py
+-rw-r--r--   0        0        0     4518 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/spikesorting/v0/merged_sorting_extractor.py
+-rw-r--r--   0        0        0     7577 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/spikesorting/v0/sortingview.py
+-rw-r--r--   0        0        0     4992 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/spikesorting/v0/sortingview_helper_fn.py
+-rw-r--r--   0        0        0    15520 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/spikesorting/v0/spikesorting_artifact.py
+-rw-r--r--   0        0        0    41236 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/spikesorting/v0/spikesorting_curation.py
+-rw-r--r--   0        0        0    11481 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/spikesorting/v0/spikesorting_populator.py
+-rw-r--r--   0        0        0    23579 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/spikesorting/v0/spikesorting_recording.py
+-rw-r--r--   0        0        0    10095 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/spikesorting/v0/spikesorting_sorting.py
+-rw-r--r--   0        0        0     3436 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/spikesorting/v0/figurl_views/SpikeSortingRecordingView.py
+-rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/spikesorting/v0/figurl_views/SpikeSortingView.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/spikesorting/v0/figurl_views/__init__.py
+-rw-r--r--   0        0        0    11393 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/spikesorting/v0/figurl_views/prepare_spikesortingview_data.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/spikesorting/v1/__init__.py
+-rw-r--r--   0        0        0    14842 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/spikesorting/v1/artifact.py
+-rw-r--r--   0        0        0    16347 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/spikesorting/v1/curation.py
+-rw-r--r--   0        0        0     9424 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/spikesorting/v1/figurl_curation.py
+-rw-r--r--   0        0        0    19431 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/spikesorting/v1/metric_curation.py
+-rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/spikesorting/v1/metric_utils.py
+-rw-r--r--   0        0        0    33193 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/spikesorting/v1/recording.py
+-rw-r--r--   0        0        0    13943 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/spikesorting/v1/sorting.py
+-rw-r--r--   0        0        0     3764 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/spikesorting/v1/utils.py
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/utils/__init__.py
+-rwxr-xr-x   0        0        0     7345 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/utils/database_settings.py
+-rw-r--r--   0        0        0    13826 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/utils/dj_chains.py
+-rw-r--r--   0        0        0    12976 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/utils/dj_graph.py
+-rw-r--r--   0        0        0     8713 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/utils/dj_helper_fn.py
+-rw-r--r--   0        0        0    30084 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/utils/dj_merge_tables.py
+-rw-r--r--   0        0        0    27951 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/utils/dj_mixin.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/utils/logging.py
+-rw-r--r--   0        0        0    17753 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/src/spyglass/utils/nwb_helper_fn.py
+-rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/tests/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/tests/__init__.py
+-rw-r--r--   0        0        0    12154 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/tests/conftest.py
+-rw-r--r--   0        0        0     6992 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/tests/container.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/tests/common/__init__.py
+-rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/tests/common/conftest.py
+-rw-r--r--   0        0        0     4116 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/tests/common/test_behav.py
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/tests/common/test_device.py
+-rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/tests/common/test_dio.py
+-rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/tests/common/test_ephys.py
+-rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/tests/common/test_filter.py
+-rw-r--r--   0        0        0     7408 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/tests/common/test_insert.py
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/tests/common/test_interval.py
+-rw-r--r--   0        0        0     7476 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/tests/common/test_interval_helpers.py
+-rw-r--r--   0        0        0     3112 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/tests/common/test_lab.py
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/tests/common/test_nwbfile.py
+-rw-r--r--   0        0        0     4324 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/tests/common/test_position.py
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/tests/common/test_region.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/tests/common/test_ripple.py
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/tests/common/test_sensors.py
+-rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/tests/common/test_session.py
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/tests/data_import/__init__.py
+-rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/tests/data_import/test_insert_sessions.py
+-rw-r--r--   0        0        0     6994 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/tests/lfp/conftest.py
+-rw-r--r--   0        0        0     3654 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/tests/lfp/test_lfp.py
+-rw-r--r--   0        0        0     3402 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/tests/linearization/conftest.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/tests/linearization/test_lin.py
+-rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/tests/position/test_trodes.py
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/tests/utils/conftest.py
+-rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/tests/utils/test_chains.py
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/tests/utils/test_db_settings.py
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/tests/utils/test_dj_helper_fn.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/tests/utils/test_logging.py
+-rw-r--r--   0        0        0     2227 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/tests/utils/test_merge.py
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/tests/utils/test_mixin.py
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/tests/utils/test_nwb_helper_fn.py
+-rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/LICENSE
+-rw-r--r--   0        0        0     6368 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/README.md
+-rw-r--r--   0        0        0     4547 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/pyproject.toml
+-rw-r--r--   0        0        0    10182 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2a1/PKG-INFO
```

### Comparing `spyglass_neuro-0.5.2/.pre-commit-config.yaml` & `spyglass_neuro-0.5.2a1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/CHANGELOG.md` & `spyglass_neuro-0.5.2a1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,20 @@
 # Change Log
 
+## [0.5.3] (Unreleased)
+
+### Release Notes
+
+<!-- Running draft to be removed immediately prior to release. -->
+
+### Infrastructure
+
+- Create class `SpyglassGroupPart` to aid delete propagations #899
+- Fix bug report template #955
+
 ## [0.5.2] (April 22, 2024)
 
 ### Infrastructure
 
 - Refactor `TableChain` to include `_searched` attribute. #867
 - Fix errors in config import #882
 - Save current spyglass version in analysis nwb files to aid diagnosis #897
@@ -223,7 +234,8 @@
 [0.4.0]: https://github.com/LorenFrankLab/spyglass/releases/tag/0.4.0
 [0.4.1]: https://github.com/LorenFrankLab/spyglass/releases/tag/0.4.1
 [0.4.2]: https://github.com/LorenFrankLab/spyglass/releases/tag/0.4.2
 [0.4.3]: https://github.com/LorenFrankLab/spyglass/releases/tag/0.4.3
 [0.5.0]: https://github.com/LorenFrankLab/spyglass/releases/tag/0.5.0
 [0.5.1]: https://github.com/LorenFrankLab/spyglass/releases/tag/0.5.1
 [0.5.2]: https://github.com/LorenFrankLab/spyglass/releases/tag/0.5.2
+[0.5.3]: https://github.com/LorenFrankLab/spyglass/releases/tag/0.5.3
```

### Comparing `spyglass_neuro-0.5.2/CITATION.cff` & `spyglass_neuro-0.5.2a1/CITATION.cff`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/CODE_OF_CONDUCT.md` & `spyglass_neuro-0.5.2a1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/dj_local_conf_example.json` & `spyglass_neuro-0.5.2a1/dj_local_conf_example.json`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/environment.yml` & `spyglass_neuro-0.5.2a1/environment.yml`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/environment_dlc.yml` & `spyglass_neuro-0.5.2a1/environment_dlc.yml`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/.github/pull_request_template.md` & `spyglass_neuro-0.5.2a1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/.github/ISSUE_TEMPLATE/bug_report.md` & `spyglass_neuro-0.5.2a1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 Steps to reproduce the behavior:
 
 1. This error is on file '....' at file path '....'
 2. Click on '....'
 3. Scroll down to '....'
 4. See error
 
-</details><summary>Error Stack</summary>
+<details><summary>Error Stack</summary>
 
 ```python
 # Paste the error stack trace here
 ```
 
 </details>
```

### Comparing `spyglass_neuro-0.5.2/.github/ISSUE_TEMPLATE/feature_request.md` & `spyglass_neuro-0.5.2a1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/.github/workflows/publish-docs.yml` & `spyglass_neuro-0.5.2a1/.github/workflows/publish-docs.yml`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/.github/workflows/test-conda.yml` & `spyglass_neuro-0.5.2a1/.github/workflows/test-conda.yml`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/.github/workflows/test-package-build.yml` & `spyglass_neuro-0.5.2a1/.github/workflows/test-package-build.yml`

 * *Files 5% similar despite different names*

```diff
@@ -86,15 +86,15 @@
     runs-on: ubuntu-latest
     needs: [test-package]
     environment:
       name: pypi
       url: https://pypi.org/p/spyglass-neuro
     permissions:
       id-token: write  # IMPORTANT: this permission is mandatory for trusted publishing
-    if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags/') && github.ref == 'refs/heads/master'
+    if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags/')
     steps:
       - uses: actions/download-artifact@v3
         with:
           name: dist
           path: dist/
       - name: Publish package distributions to PyPI
         uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `spyglass_neuro-0.5.2/.vscode/extensions.json` & `spyglass_neuro-0.5.2a1/.vscode/extensions.json`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/.vscode/settings.json` & `spyglass_neuro-0.5.2a1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/config/dj_config.py` & `spyglass_neuro-0.5.2a1/config/dj_config.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/docs/README.md` & `spyglass_neuro-0.5.2a1/docs/README.md`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/docs/build-docs.sh` & `spyglass_neuro-0.5.2a1/docs/build-docs.sh`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/docs/mkdocs.yml` & `spyglass_neuro-0.5.2a1/docs/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/docs/src/contribute.md` & `spyglass_neuro-0.5.2a1/docs/src/contribute.md`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/docs/src/index.md` & `spyglass_neuro-0.5.2a1/docs/src/index.md`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/docs/src/installation.md` & `spyglass_neuro-0.5.2a1/docs/src/installation.md`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/docs/src/api/index.md` & `spyglass_neuro-0.5.2a1/docs/src/api/index.md`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/docs/src/api/make_pages.py` & `spyglass_neuro-0.5.2a1/docs/src/api/make_pages.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/docs/src/images/FrankLab.png` & `spyglass_neuro-0.5.2a1/docs/src/images/FrankLab.png`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/docs/src/images/Spyglass.png` & `spyglass_neuro-0.5.2a1/docs/src/images/Spyglass.png`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/docs/src/images/Spyglass.svg` & `spyglass_neuro-0.5.2a1/docs/src/images/Spyglass.svg`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/docs/src/images/fig1.png` & `spyglass_neuro-0.5.2a1/docs/src/images/fig1.png`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/docs/src/images/merge_diagram.png` & `spyglass_neuro-0.5.2a1/docs/src/images/merge_diagram.png`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/docs/src/misc/database_management.md` & `spyglass_neuro-0.5.2a1/docs/src/misc/database_management.md`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/docs/src/misc/export.md` & `spyglass_neuro-0.5.2a1/docs/src/misc/export.md`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/docs/src/misc/figurl_views.md` & `spyglass_neuro-0.5.2a1/docs/src/misc/figurl_views.md`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/docs/src/misc/insert_data.md` & `spyglass_neuro-0.5.2a1/docs/src/misc/insert_data.md`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/docs/src/misc/merge_tables.md` & `spyglass_neuro-0.5.2a1/docs/src/misc/merge_tables.md`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/docs/src/misc/mixin.md` & `spyglass_neuro-0.5.2a1/docs/src/misc/mixin.md`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/docs/src/misc/session_groups.md` & `spyglass_neuro-0.5.2a1/docs/src/misc/session_groups.md`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/docs/src/stylesheets/extra.css` & `spyglass_neuro-0.5.2a1/docs/src/stylesheets/extra.css`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/examples/cli_examples/insert_sort_interval.py` & `spyglass_neuro-0.5.2a1/examples/cli_examples/insert_sort_interval.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/examples/cli_examples/readme.md` & `spyglass_neuro-0.5.2a1/examples/cli_examples/readme.md`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/examples/config_yaml/entries.yaml` & `spyglass_neuro-0.5.2a1/examples/config_yaml/entries.yaml`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/examples/config_yaml/sub-AppleBottom_ses-AppleBottom-DY20-g3_behavior+ecephys_spyglass_config.yaml` & `spyglass_neuro-0.5.2a1/examples/config_yaml/sub-AppleBottom_ses-AppleBottom-DY20-g3_behavior+ecephys_spyglass_config.yaml`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/franklab_scripts/alter_tables.py` & `spyglass_neuro-0.5.2a1/franklab_scripts/alter_tables.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/franklab_scripts/nightly_cleanup.py` & `spyglass_neuro-0.5.2a1/franklab_scripts/nightly_cleanup.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/franklab_scripts/sort.py` & `spyglass_neuro-0.5.2a1/franklab_scripts/sort.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/notebooks/00_Setup.ipynb` & `spyglass_neuro-0.5.2a1/notebooks/00_Setup.ipynb`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/notebooks/01_Insert_Data.ipynb` & `spyglass_neuro-0.5.2a1/notebooks/01_Insert_Data.ipynb`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/notebooks/02_Data_Sync.ipynb` & `spyglass_neuro-0.5.2a1/notebooks/02_Data_Sync.ipynb`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/notebooks/03_Merge_Tables.ipynb` & `spyglass_neuro-0.5.2a1/notebooks/03_Merge_Tables.ipynb`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/notebooks/04_PopulateConfigFile.ipynb` & `spyglass_neuro-0.5.2a1/notebooks/04_PopulateConfigFile.ipynb`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/notebooks/05_Export.ipynb` & `spyglass_neuro-0.5.2a1/notebooks/05_Export.ipynb`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/notebooks/10_Spike_SortingV0.ipynb` & `spyglass_neuro-0.5.2a1/notebooks/10_Spike_SortingV0.ipynb`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/notebooks/10_Spike_SortingV1.ipynb` & `spyglass_neuro-0.5.2a1/notebooks/10_Spike_SortingV1.ipynb`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/notebooks/20_Position_Trodes.ipynb` & `spyglass_neuro-0.5.2a1/notebooks/20_Position_Trodes.ipynb`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/notebooks/21_DLC.ipynb` & `spyglass_neuro-0.5.2a1/notebooks/21_DLC.ipynb`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/notebooks/22_DLC_Loop.ipynb` & `spyglass_neuro-0.5.2a1/notebooks/22_DLC_Loop.ipynb`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/notebooks/24_Linearization.ipynb` & `spyglass_neuro-0.5.2a1/notebooks/24_Linearization.ipynb`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/notebooks/30_LFP.ipynb` & `spyglass_neuro-0.5.2a1/notebooks/30_LFP.ipynb`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/notebooks/31_Theta.ipynb` & `spyglass_neuro-0.5.2a1/notebooks/31_Theta.ipynb`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/notebooks/32_Ripple_Detection.ipynb` & `spyglass_neuro-0.5.2a1/notebooks/32_Ripple_Detection.ipynb`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/notebooks/40_Extracting_Clusterless_Waveform_Features.ipynb` & `spyglass_neuro-0.5.2a1/notebooks/40_Extracting_Clusterless_Waveform_Features.ipynb`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/notebooks/41_Decoding_Clusterless.ipynb` & `spyglass_neuro-0.5.2a1/notebooks/41_Decoding_Clusterless.ipynb`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/notebooks/42_Decoding_SortedSpikes.ipynb` & `spyglass_neuro-0.5.2a1/notebooks/42_Decoding_SortedSpikes.ipynb`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/notebooks/50_MUA_Detection.ipynb` & `spyglass_neuro-0.5.2a1/notebooks/50_MUA_Detection.ipynb`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/notebooks/README.md` & `spyglass_neuro-0.5.2a1/notebooks/README.md`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/notebooks/py_scripts/00_Setup.py` & `spyglass_neuro-0.5.2a1/notebooks/py_scripts/00_Setup.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/notebooks/py_scripts/01_Insert_Data.py` & `spyglass_neuro-0.5.2a1/notebooks/py_scripts/01_Insert_Data.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/notebooks/py_scripts/02_Data_Sync.py` & `spyglass_neuro-0.5.2a1/notebooks/py_scripts/02_Data_Sync.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/notebooks/py_scripts/03_Merge_Tables.py` & `spyglass_neuro-0.5.2a1/notebooks/py_scripts/03_Merge_Tables.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/notebooks/py_scripts/04_PopulateConfigFile.py` & `spyglass_neuro-0.5.2a1/notebooks/py_scripts/04_PopulateConfigFile.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/notebooks/py_scripts/05_Export.py` & `spyglass_neuro-0.5.2a1/notebooks/py_scripts/05_Export.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/notebooks/py_scripts/10_Spike_SortingV0.py` & `spyglass_neuro-0.5.2a1/notebooks/py_scripts/10_Spike_SortingV0.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/notebooks/py_scripts/10_Spike_SortingV1.py` & `spyglass_neuro-0.5.2a1/notebooks/py_scripts/10_Spike_SortingV1.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/notebooks/py_scripts/20_Position_Trodes.py` & `spyglass_neuro-0.5.2a1/notebooks/py_scripts/20_Position_Trodes.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/notebooks/py_scripts/21_DLC.py` & `spyglass_neuro-0.5.2a1/notebooks/py_scripts/21_DLC.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/notebooks/py_scripts/22_DLC_Loop.py` & `spyglass_neuro-0.5.2a1/notebooks/py_scripts/22_DLC_Loop.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/notebooks/py_scripts/24_Linearization.py` & `spyglass_neuro-0.5.2a1/notebooks/py_scripts/24_Linearization.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/notebooks/py_scripts/30_LFP.py` & `spyglass_neuro-0.5.2a1/notebooks/py_scripts/30_LFP.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/notebooks/py_scripts/31_Theta.py` & `spyglass_neuro-0.5.2a1/notebooks/py_scripts/31_Theta.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/notebooks/py_scripts/32_Ripple_Detection.py` & `spyglass_neuro-0.5.2a1/notebooks/py_scripts/32_Ripple_Detection.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/notebooks/py_scripts/40_Extracting_Clusterless_Waveform_Features.py` & `spyglass_neuro-0.5.2a1/notebooks/py_scripts/40_Extracting_Clusterless_Waveform_Features.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/notebooks/py_scripts/41_Decoding_Clusterless.py` & `spyglass_neuro-0.5.2a1/notebooks/py_scripts/41_Decoding_Clusterless.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/notebooks/py_scripts/41_Extracting_Clusterless_Waveform_Features.py` & `spyglass_neuro-0.5.2a1/notebooks/py_scripts/41_Extracting_Clusterless_Waveform_Features.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/notebooks/py_scripts/42_Decoding_Clusterless.py` & `spyglass_neuro-0.5.2a1/notebooks/py_scripts/42_Decoding_Clusterless.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/notebooks/py_scripts/42_Decoding_SortedSpikes.py` & `spyglass_neuro-0.5.2a1/notebooks/py_scripts/42_Decoding_SortedSpikes.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/notebooks/py_scripts/43_Decoding_SortedSpikes.py` & `spyglass_neuro-0.5.2a1/notebooks/py_scripts/43_Decoding_SortedSpikes.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/notebooks/py_scripts/51_MUA_Detection.py` & `spyglass_neuro-0.5.2a1/notebooks/py_scripts/51_MUA_Detection.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/settings.py` & `spyglass_neuro-0.5.2a1/src/spyglass/settings.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/cli/cli.py` & `spyglass_neuro-0.5.2a1/src/spyglass/cli/cli.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/common/__init__.py` & `spyglass_neuro-0.5.2a1/src/spyglass/common/__init__.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/common/common_behav.py` & `spyglass_neuro-0.5.2a1/src/spyglass/common/common_behav.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/common/common_device.py` & `spyglass_neuro-0.5.2a1/src/spyglass/common/common_device.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/common/common_dio.py` & `spyglass_neuro-0.5.2a1/src/spyglass/common/common_dio.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/common/common_ephys.py` & `spyglass_neuro-0.5.2a1/src/spyglass/common/common_ephys.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/common/common_filter.py` & `spyglass_neuro-0.5.2a1/src/spyglass/common/common_filter.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/common/common_interval.py` & `spyglass_neuro-0.5.2a1/src/spyglass/common/common_interval.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/common/common_lab.py` & `spyglass_neuro-0.5.2a1/src/spyglass/common/common_lab.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/common/common_nwbfile.py` & `spyglass_neuro-0.5.2a1/src/spyglass/common/common_nwbfile.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/common/common_position.py` & `spyglass_neuro-0.5.2a1/src/spyglass/common/common_position.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/common/common_region.py` & `spyglass_neuro-0.5.2a1/src/spyglass/common/common_region.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/common/common_ripple.py` & `spyglass_neuro-0.5.2a1/src/spyglass/common/common_ripple.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/common/common_sensors.py` & `spyglass_neuro-0.5.2a1/src/spyglass/common/common_sensors.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/common/common_session.py` & `spyglass_neuro-0.5.2a1/src/spyglass/common/common_session.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/common/common_subject.py` & `spyglass_neuro-0.5.2a1/src/spyglass/common/common_subject.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/common/common_task.py` & `spyglass_neuro-0.5.2a1/src/spyglass/common/common_task.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/common/common_usage.py` & `spyglass_neuro-0.5.2a1/src/spyglass/common/common_usage.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/common/populate_all_common.py` & `spyglass_neuro-0.5.2a1/src/spyglass/common/populate_all_common.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/common/signal_processing.py` & `spyglass_neuro-0.5.2a1/src/spyglass/common/signal_processing.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/common/prepopulate/prepopulate.py` & `spyglass_neuro-0.5.2a1/src/spyglass/common/prepopulate/prepopulate.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/data_import/insert_sessions.py` & `spyglass_neuro-0.5.2a1/src/spyglass/data_import/insert_sessions.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/decoding/__init__.py` & `spyglass_neuro-0.5.2a1/src/spyglass/decoding/__init__.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/decoding/decoding_merge.py` & `spyglass_neuro-0.5.2a1/src/spyglass/decoding/decoding_merge.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/decoding/v0/clusterless.py` & `spyglass_neuro-0.5.2a1/src/spyglass/decoding/v0/clusterless.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/decoding/v0/core.py` & `spyglass_neuro-0.5.2a1/src/spyglass/decoding/v0/core.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/decoding/v0/dj_decoder_conversion.py` & `spyglass_neuro-0.5.2a1/src/spyglass/decoding/v0/dj_decoder_conversion.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/decoding/v0/sorted_spikes.py` & `spyglass_neuro-0.5.2a1/src/spyglass/decoding/v0/sorted_spikes.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/decoding/v0/visualization.py` & `spyglass_neuro-0.5.2a1/src/spyglass/decoding/v0/visualization.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/decoding/v0/visualization_1D_view.py` & `spyglass_neuro-0.5.2a1/src/spyglass/decoding/v0/visualization_1D_view.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/decoding/v0/visualization_2D_view.py` & `spyglass_neuro-0.5.2a1/src/spyglass/decoding/v0/visualization_2D_view.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/decoding/v1/clusterless.py` & `spyglass_neuro-0.5.2a1/src/spyglass/decoding/v1/clusterless.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,27 +28,27 @@
     PositionGroup,
 )  # noqa: F401
 from spyglass.decoding.v1.waveform_features import (
     UnitWaveformFeatures,
 )  # noqa: F401
 from spyglass.position.position_merge import PositionOutput  # noqa: F401
 from spyglass.settings import config
-from spyglass.utils import SpyglassMixin, logger
+from spyglass.utils import SpyglassMixin, SpyglassMixinPart, logger
 
 schema = dj.schema("decoding_clusterless_v1")
 
 
 @schema
 class UnitWaveformFeaturesGroup(SpyglassMixin, dj.Manual):
     definition = """
     -> Session
     waveform_features_group_name: varchar(80)
     """
 
-    class UnitFeatures(SpyglassMixin, dj.Part):
+    class UnitFeatures(SpyglassMixinPart):
         definition = """
         -> UnitWaveformFeaturesGroup
         -> UnitWaveformFeatures
         """
 
     def create_group(
         self, nwb_file_name: str, group_name: str, keys: list[dict]
```

### Comparing `spyglass_neuro-0.5.2/src/spyglass/decoding/v1/core.py` & `spyglass_neuro-0.5.2a1/src/spyglass/decoding/v1/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from spyglass.common.common_session import Session  # noqa: F401
 from spyglass.decoding.v1.dj_decoder_conversion import (
     convert_classes_to_dict,
     restore_classes,
 )
 from spyglass.position.position_merge import PositionOutput  # noqa: F401
-from spyglass.utils import SpyglassMixin
+from spyglass.utils import SpyglassMixin, SpyglassMixinPart
 
 schema = dj.schema("decoding_core_v1")
 
 
 @schema
 class DecodingParameters(SpyglassMixin, dj.Lookup):
     """Parameters for decoding the animal's mental position and some category of interest"""
@@ -90,15 +90,15 @@
     definition = """
     -> Session
     position_group_name: varchar(80)
     ----
     position_variables = NULL: longblob # list of position variables to decode
     """
 
-    class Position(SpyglassMixin, dj.Part):
+    class Position(SpyglassMixinPart):
         definition = """
         -> PositionGroup
         -> PositionOutput.proj(pos_merge_id='merge_id')
         """
 
     def create_group(
         self,
```

### Comparing `spyglass_neuro-0.5.2/src/spyglass/decoding/v1/dj_decoder_conversion.py` & `spyglass_neuro-0.5.2a1/src/spyglass/decoding/v1/dj_decoder_conversion.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/decoding/v1/sorted_spikes.py` & `spyglass_neuro-0.5.2a1/src/spyglass/decoding/v1/sorted_spikes.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/decoding/v1/waveform_features.py` & `spyglass_neuro-0.5.2a1/src/spyglass/decoding/v1/waveform_features.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/lfp/lfp_electrode.py` & `spyglass_neuro-0.5.2a1/src/spyglass/lfp/lfp_electrode.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/lfp/lfp_imported.py` & `spyglass_neuro-0.5.2a1/src/spyglass/lfp/lfp_imported.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/lfp/lfp_merge.py` & `spyglass_neuro-0.5.2a1/src/spyglass/lfp/lfp_merge.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/lfp/analysis/v1/lfp_band.py` & `spyglass_neuro-0.5.2a1/src/spyglass/lfp/analysis/v1/lfp_band.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/lfp/v1/lfp.py` & `spyglass_neuro-0.5.2a1/src/spyglass/lfp/v1/lfp.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/lfp/v1/lfp_artifact.py` & `spyglass_neuro-0.5.2a1/src/spyglass/lfp/v1/lfp_artifact.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/lfp/v1/lfp_artifact_MAD_detection.py` & `spyglass_neuro-0.5.2a1/src/spyglass/lfp/v1/lfp_artifact_MAD_detection.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/lfp/v1/lfp_artifact_difference_detection.py` & `spyglass_neuro-0.5.2a1/src/spyglass/lfp/v1/lfp_artifact_difference_detection.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/linearization/merge.py` & `spyglass_neuro-0.5.2a1/src/spyglass/linearization/merge.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/linearization/v0/main.py` & `spyglass_neuro-0.5.2a1/src/spyglass/linearization/v0/main.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/linearization/v1/main.py` & `spyglass_neuro-0.5.2a1/src/spyglass/linearization/v1/main.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/lock/file_lock.py` & `spyglass_neuro-0.5.2a1/src/spyglass/lock/file_lock.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/mua/v1/mua.py` & `spyglass_neuro-0.5.2a1/src/spyglass/mua/v1/mua.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/position/position_merge.py` & `spyglass_neuro-0.5.2a1/src/spyglass/position/position_merge.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/position/v1/__init__.py` & `spyglass_neuro-0.5.2a1/src/spyglass/position/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/position/v1/dlc_decorators.py` & `spyglass_neuro-0.5.2a1/src/spyglass/position/v1/dlc_decorators.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/position/v1/dlc_reader.py` & `spyglass_neuro-0.5.2a1/src/spyglass/position/v1/dlc_reader.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/position/v1/dlc_utils.py` & `spyglass_neuro-0.5.2a1/src/spyglass/position/v1/dlc_utils.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/position/v1/position_dlc_centroid.py` & `spyglass_neuro-0.5.2a1/src/spyglass/position/v1/position_dlc_centroid.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/position/v1/position_dlc_cohort.py` & `spyglass_neuro-0.5.2a1/src/spyglass/position/v1/position_dlc_cohort.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/position/v1/position_dlc_model.py` & `spyglass_neuro-0.5.2a1/src/spyglass/position/v1/position_dlc_model.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/position/v1/position_dlc_orient.py` & `spyglass_neuro-0.5.2a1/src/spyglass/position/v1/position_dlc_orient.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/position/v1/position_dlc_pose_estimation.py` & `spyglass_neuro-0.5.2a1/src/spyglass/position/v1/position_dlc_pose_estimation.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/position/v1/position_dlc_position.py` & `spyglass_neuro-0.5.2a1/src/spyglass/position/v1/position_dlc_position.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/position/v1/position_dlc_project.py` & `spyglass_neuro-0.5.2a1/src/spyglass/position/v1/position_dlc_project.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/position/v1/position_dlc_selection.py` & `spyglass_neuro-0.5.2a1/src/spyglass/position/v1/position_dlc_selection.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/position/v1/position_dlc_training.py` & `spyglass_neuro-0.5.2a1/src/spyglass/position/v1/position_dlc_training.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/position/v1/position_trodes_position.py` & `spyglass_neuro-0.5.2a1/src/spyglass/position/v1/position_trodes_position.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/ripple/v1/ripple.py` & `spyglass_neuro-0.5.2a1/src/spyglass/ripple/v1/ripple.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/sharing/sharing_kachery.py` & `spyglass_neuro-0.5.2a1/src/spyglass/sharing/sharing_kachery.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/spikesorting/imported.py` & `spyglass_neuro-0.5.2a1/src/spyglass/spikesorting/imported.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/spikesorting/spikesorting_merge.py` & `spyglass_neuro-0.5.2a1/src/spyglass/spikesorting/spikesorting_merge.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/spikesorting/analysis/v1/group.py` & `spyglass_neuro-0.5.2a1/src/spyglass/spikesorting/analysis/v1/group.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import datajoint as dj
 import numpy as np
 from ripple_detection import get_multiunit_population_firing_rate
 
 from spyglass.common import Session  # noqa: F401
 from spyglass.spikesorting.spikesorting_merge import SpikeSortingOutput
-from spyglass.utils.dj_mixin import SpyglassMixin
+from spyglass.utils.dj_mixin import SpyglassMixin, SpyglassMixinPart
 
 schema = dj.schema("spikesorting_group_v1")
 
 
 @schema
 class UnitSelectionParams(SpyglassMixin, dj.Manual):
     definition = """
@@ -47,15 +47,15 @@
 class SortedSpikesGroup(SpyglassMixin, dj.Manual):
     definition = """
     -> Session
     -> UnitSelectionParams
     sorted_spikes_group_name: varchar(80)
     """
 
-    class Units(SpyglassMixin, dj.Part):
+    class Units(SpyglassMixinPart):
         definition = """
         -> master
         -> SpikeSortingOutput.proj(spikesorting_merge_id='merge_id')
         """
 
     def create_group(
         self,
```

### Comparing `spyglass_neuro-0.5.2/src/spyglass/spikesorting/v0/__init__.py` & `spyglass_neuro-0.5.2a1/src/spyglass/spikesorting/v0/__init__.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/spikesorting/v0/curation_figurl.py` & `spyglass_neuro-0.5.2a1/src/spyglass/spikesorting/v0/curation_figurl.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/spikesorting/v0/merged_sorting_extractor.py` & `spyglass_neuro-0.5.2a1/src/spyglass/spikesorting/v0/merged_sorting_extractor.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/spikesorting/v0/sortingview.py` & `spyglass_neuro-0.5.2a1/src/spyglass/spikesorting/v0/sortingview.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/spikesorting/v0/sortingview_helper_fn.py` & `spyglass_neuro-0.5.2a1/src/spyglass/spikesorting/v0/sortingview_helper_fn.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/spikesorting/v0/spikesorting_artifact.py` & `spyglass_neuro-0.5.2a1/src/spyglass/spikesorting/v0/spikesorting_artifact.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/spikesorting/v0/spikesorting_curation.py` & `spyglass_neuro-0.5.2a1/src/spyglass/spikesorting/v0/spikesorting_curation.py`

 * *Files 1% similar despite different names*

```diff
@@ -509,18 +509,21 @@
     ---
     quality_metrics_path: varchar(500)
     -> AnalysisNwbfile
     object_id: varchar(40) # Object ID for the metrics in NWB file
     """
 
     def make(self, key):
-        key["analysis_file_name"] = AnalysisNwbfile().create(  # logged
+        analysis_file_name = AnalysisNwbfile().create(  # logged
             key["nwb_file_name"]
         )
         waveform_extractor = Waveforms().load_waveforms(key)
+        key["analysis_file_name"] = (
+            analysis_file_name  # add to key here to prevent fetch errors
+        )
         qm = {}
         params = (MetricParameters & key).fetch1("metric_params")
         for metric_name, metric_params in params.items():
             metric = self._compute_metric(
                 waveform_extractor, metric_name, **metric_params
             )
             qm[metric_name] = metric
```

### Comparing `spyglass_neuro-0.5.2/src/spyglass/spikesorting/v0/spikesorting_populator.py` & `spyglass_neuro-0.5.2a1/src/spyglass/spikesorting/v0/spikesorting_populator.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/spikesorting/v0/spikesorting_recording.py` & `spyglass_neuro-0.5.2a1/src/spyglass/spikesorting/v0/spikesorting_recording.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/spikesorting/v0/spikesorting_sorting.py` & `spyglass_neuro-0.5.2a1/src/spyglass/spikesorting/v0/spikesorting_sorting.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/spikesorting/v0/figurl_views/SpikeSortingRecordingView.py` & `spyglass_neuro-0.5.2a1/src/spyglass/spikesorting/v0/figurl_views/SpikeSortingRecordingView.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/spikesorting/v0/figurl_views/SpikeSortingView.py` & `spyglass_neuro-0.5.2a1/src/spyglass/spikesorting/v0/figurl_views/SpikeSortingView.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/spikesorting/v0/figurl_views/prepare_spikesortingview_data.py` & `spyglass_neuro-0.5.2a1/src/spyglass/spikesorting/v0/figurl_views/prepare_spikesortingview_data.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/spikesorting/v1/__init__.py` & `spyglass_neuro-0.5.2a1/src/spyglass/spikesorting/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/spikesorting/v1/artifact.py` & `spyglass_neuro-0.5.2a1/src/spyglass/spikesorting/v1/artifact.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/spikesorting/v1/curation.py` & `spyglass_neuro-0.5.2a1/src/spyglass/spikesorting/v1/curation.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/spikesorting/v1/figurl_curation.py` & `spyglass_neuro-0.5.2a1/src/spyglass/spikesorting/v1/figurl_curation.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/spikesorting/v1/metric_curation.py` & `spyglass_neuro-0.5.2a1/src/spyglass/spikesorting/v1/metric_curation.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/spikesorting/v1/metric_utils.py` & `spyglass_neuro-0.5.2a1/src/spyglass/spikesorting/v1/metric_utils.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/spikesorting/v1/recording.py` & `spyglass_neuro-0.5.2a1/src/spyglass/spikesorting/v1/recording.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/spikesorting/v1/sorting.py` & `spyglass_neuro-0.5.2a1/src/spyglass/spikesorting/v1/sorting.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/spikesorting/v1/utils.py` & `spyglass_neuro-0.5.2a1/src/spyglass/spikesorting/v1/utils.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/utils/database_settings.py` & `spyglass_neuro-0.5.2a1/src/spyglass/utils/database_settings.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/utils/dj_chains.py` & `spyglass_neuro-0.5.2a1/src/spyglass/utils/dj_chains.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/utils/dj_graph.py` & `spyglass_neuro-0.5.2a1/src/spyglass/utils/dj_graph.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/utils/dj_helper_fn.py` & `spyglass_neuro-0.5.2a1/src/spyglass/utils/dj_helper_fn.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/utils/dj_merge_tables.py` & `spyglass_neuro-0.5.2a1/src/spyglass/utils/dj_merge_tables.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/utils/dj_mixin.py` & `spyglass_neuro-0.5.2a1/src/spyglass/utils/dj_mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -733,7 +733,19 @@
             if "file" in field:
                 attr = field
                 break
         if not attr:
             logger.error(f"No file-like field found in {self.full_table_name}")
             return
         return self & f"{attr} LIKE '%{name}%'"
+
+
+class SpyglassMixinPart(SpyglassMixin, dj.Part):
+    """
+    A part table for Spyglass Group tables. Assists in propagating
+    delete calls from upstreeam tables to downstream tables.
+    """
+
+    def delete(self, *args, **kwargs):
+        """Delete master and part entries."""
+        restriction = self.restriction or True  # for (tbl & restr).delete()
+        (self.master & restriction).delete(*args, **kwargs)
```

### Comparing `spyglass_neuro-0.5.2/src/spyglass/utils/logging.py` & `spyglass_neuro-0.5.2a1/src/spyglass/utils/logging.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/src/spyglass/utils/nwb_helper_fn.py` & `spyglass_neuro-0.5.2a1/src/spyglass/utils/nwb_helper_fn.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/tests/README.md` & `spyglass_neuro-0.5.2a1/tests/README.md`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/tests/conftest.py` & `spyglass_neuro-0.5.2a1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/tests/container.py` & `spyglass_neuro-0.5.2a1/tests/container.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/tests/common/conftest.py` & `spyglass_neuro-0.5.2a1/tests/common/conftest.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/tests/common/test_behav.py` & `spyglass_neuro-0.5.2a1/tests/common/test_behav.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/tests/common/test_device.py` & `spyglass_neuro-0.5.2a1/tests/common/test_device.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/tests/common/test_dio.py` & `spyglass_neuro-0.5.2a1/tests/common/test_dio.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/tests/common/test_ephys.py` & `spyglass_neuro-0.5.2a1/tests/common/test_ephys.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/tests/common/test_filter.py` & `spyglass_neuro-0.5.2a1/tests/common/test_filter.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/tests/common/test_insert.py` & `spyglass_neuro-0.5.2a1/tests/common/test_insert.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/tests/common/test_interval.py` & `spyglass_neuro-0.5.2a1/tests/common/test_interval.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/tests/common/test_interval_helpers.py` & `spyglass_neuro-0.5.2a1/tests/common/test_interval_helpers.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/tests/common/test_lab.py` & `spyglass_neuro-0.5.2a1/tests/common/test_lab.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/tests/common/test_nwbfile.py` & `spyglass_neuro-0.5.2a1/tests/common/test_nwbfile.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/tests/common/test_position.py` & `spyglass_neuro-0.5.2a1/tests/common/test_position.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/tests/common/test_region.py` & `spyglass_neuro-0.5.2a1/tests/common/test_region.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/tests/common/test_sensors.py` & `spyglass_neuro-0.5.2a1/tests/common/test_sensors.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/tests/common/test_session.py` & `spyglass_neuro-0.5.2a1/tests/common/test_session.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/tests/data_import/test_insert_sessions.py` & `spyglass_neuro-0.5.2a1/tests/data_import/test_insert_sessions.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/tests/lfp/conftest.py` & `spyglass_neuro-0.5.2a1/tests/lfp/conftest.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/tests/lfp/test_lfp.py` & `spyglass_neuro-0.5.2a1/tests/lfp/test_lfp.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/tests/linearization/conftest.py` & `spyglass_neuro-0.5.2a1/tests/linearization/conftest.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/tests/position/test_trodes.py` & `spyglass_neuro-0.5.2a1/tests/position/test_trodes.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/tests/utils/conftest.py` & `spyglass_neuro-0.5.2a1/tests/utils/conftest.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/tests/utils/test_chains.py` & `spyglass_neuro-0.5.2a1/tests/utils/test_chains.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/tests/utils/test_db_settings.py` & `spyglass_neuro-0.5.2a1/tests/utils/test_db_settings.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/tests/utils/test_merge.py` & `spyglass_neuro-0.5.2a1/tests/utils/test_merge.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/tests/utils/test_mixin.py` & `spyglass_neuro-0.5.2a1/tests/utils/test_mixin.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/tests/utils/test_nwb_helper_fn.py` & `spyglass_neuro-0.5.2a1/tests/utils/test_nwb_helper_fn.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/.gitignore` & `spyglass_neuro-0.5.2a1/.gitignore`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/LICENSE` & `spyglass_neuro-0.5.2a1/LICENSE`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/README.md` & `spyglass_neuro-0.5.2a1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -58,14 +58,16 @@
 [https://lorenfranklab.github.io/spyglass/](https://lorenfranklab.github.io/spyglass/)
 
 ## Installation
 
 For installation instructions see -
 [https://lorenfranklab.github.io/spyglass/latest/installation/](https://lorenfranklab.github.io/spyglass/latest/installation/)
 
+Typical installation time is: 5-10 minutes
+
 ## Tutorials
 
 The tutorials for `spyglass` is currently in the form of Jupyter Notebooks and
 can be found in the
 [notebooks](https://github.com/LorenFrankLab/spyglass/tree/master/notebooks)
 directory. We strongly recommend opening them in the context of `jupyterlab`.
 
@@ -77,14 +79,24 @@
 [https://lorenfranklab.github.io/spyglass/latest/contribute/](https://lorenfranklab.github.io/spyglass/latest/contribute/)
 
 ## License/Copyright
 
 License and Copyright notice can be found at
 [https://lorenfranklab.github.io/spyglass/latest/LICENSE/](https://lorenfranklab.github.io/spyglass/latest/LICENSE/)
 
+## System requirements
+
+Spyglass has been tested on Linux Ubuntu 20.04 and MacOS 10.15. It has not been tested on Windows and likely will not work.
+
+No specific hardware requirements are needed to run spyglass. However, the amount of data that can be stored and analyzed is limited by the available disk space and memory. GPUs are required for some of the analysis tools, such as DeepLabCut.
+
+See [pyproject.toml](pyproject.toml), [environment.yml](environment.yml), or [environment_dlc.yml](environment_dlc.yml) for software dependencies.
+
+See [spec-file.txt](https://github.com/LorenFrankLab/spyglass-demo/blob/main/spec-file/spec-file.txt) for the conda environment used in the demo.
+
 ## Citation
 
 > Lee, K.H.\*, Denovellis, E.L.\*, Ly, R., Magland, J., Soules, J., Comrie, A.E., Gramling, D.P., Guidera, J.A., Nevers, R., Adenekan, P., Brozdowski, C., Bray, S., Monroe, E., Bak, J.H., Coulter, M.E., Sun, X., Broyles, E., Shin, D., Chiang, S., Holobetz, C., Tritt, A., Rübel, O., Nguyen, T., Yatsenko, D., Chu, J., Kemere, C., Garcia, S., Buccino, A., Frank, L.M., 2024. Spyglass: a data analysis framework for reproducible and shareable neuroscience research. bioRxiv. [10.1101/2024.01.25.577295](https://doi.org/10.1101/2024.01.25.577295).
 
 *\* Equal contribution*
 
 See paper related code [here](https://github.com/LorenFrankLab/spyglass-paper).
```

### Comparing `spyglass_neuro-0.5.2/pyproject.toml` & `spyglass_neuro-0.5.2a1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.2/PKG-INFO` & `spyglass_neuro-0.5.2a1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: spyglass-neuro
-Version: 0.5.2
+Version: 0.5.2a1
 Summary: Neuroscience data analysis framework for reproducible research
 Project-URL: Homepage, https://github.com/LorenFrankLab/spyglass
 Project-URL: Bug Tracker, https://github.com/LorenFrankLab/spyglass/issues
 Author-email: Loren Frank <loren.frank@ucsf.edu>, Kyu Hyun Lee <kyuhyun.lee@ucsf.edu>, Eric Denovellis <eric.denovellis@ucsf.edu>, Ryan Ly <rly@lbl.gov>, Daniel Gramling <daniel.gramling@ucsf.edu>, Chris Brozdowski <chris.broz@ucsf.edu>
 License: Copyright (c) 2020-present Loren Frank
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
@@ -138,14 +138,16 @@
 [https://lorenfranklab.github.io/spyglass/](https://lorenfranklab.github.io/spyglass/)
 
 ## Installation
 
 For installation instructions see -
 [https://lorenfranklab.github.io/spyglass/latest/installation/](https://lorenfranklab.github.io/spyglass/latest/installation/)
 
+Typical installation time is: 5-10 minutes
+
 ## Tutorials
 
 The tutorials for `spyglass` is currently in the form of Jupyter Notebooks and
 can be found in the
 [notebooks](https://github.com/LorenFrankLab/spyglass/tree/master/notebooks)
 directory. We strongly recommend opening them in the context of `jupyterlab`.
 
@@ -157,14 +159,24 @@
 [https://lorenfranklab.github.io/spyglass/latest/contribute/](https://lorenfranklab.github.io/spyglass/latest/contribute/)
 
 ## License/Copyright
 
 License and Copyright notice can be found at
 [https://lorenfranklab.github.io/spyglass/latest/LICENSE/](https://lorenfranklab.github.io/spyglass/latest/LICENSE/)
 
+## System requirements
+
+Spyglass has been tested on Linux Ubuntu 20.04 and MacOS 10.15. It has not been tested on Windows and likely will not work.
+
+No specific hardware requirements are needed to run spyglass. However, the amount of data that can be stored and analyzed is limited by the available disk space and memory. GPUs are required for some of the analysis tools, such as DeepLabCut.
+
+See [pyproject.toml](pyproject.toml), [environment.yml](environment.yml), or [environment_dlc.yml](environment_dlc.yml) for software dependencies.
+
+See [spec-file.txt](https://github.com/LorenFrankLab/spyglass-demo/blob/main/spec-file/spec-file.txt) for the conda environment used in the demo.
+
 ## Citation
 
 > Lee, K.H.\*, Denovellis, E.L.\*, Ly, R., Magland, J., Soules, J., Comrie, A.E., Gramling, D.P., Guidera, J.A., Nevers, R., Adenekan, P., Brozdowski, C., Bray, S., Monroe, E., Bak, J.H., Coulter, M.E., Sun, X., Broyles, E., Shin, D., Chiang, S., Holobetz, C., Tritt, A., Rübel, O., Nguyen, T., Yatsenko, D., Chu, J., Kemere, C., Garcia, S., Buccino, A., Frank, L.M., 2024. Spyglass: a data analysis framework for reproducible and shareable neuroscience research. bioRxiv. [10.1101/2024.01.25.577295](https://doi.org/10.1101/2024.01.25.577295).
 
 *\* Equal contribution*
 
 See paper related code [here](https://github.com/LorenFrankLab/spyglass-paper).
```

