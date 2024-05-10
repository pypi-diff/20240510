# Comparing `tmp/pref_voting-1.3.1.tar.gz` & `tmp/pref_voting-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pref_voting-1.3.1.tar", max compression
+gzip compressed data, was "pref_voting-1.3.2.tar", max compression
```

## Comparing `pref_voting-1.3.1.tar` & `pref_voting-1.3.2.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0     1085 2024-03-19 19:26:58.359673 pref_voting-1.3.1/LICENSE
--rw-r--r--   0        0        0     1770 2024-04-24 21:45:43.110237 pref_voting-1.3.1/README.md
--rw-r--r--   0        0        0       22 2024-05-05 19:29:36.349843 pref_voting-1.3.1/pref_voting/__init__.py
--rw-r--r--   0        0        0    18867 2023-11-14 11:21:19.592605 pref_voting-1.3.1/pref_voting/analysis.py
--rw-r--r--   0        0        0     1270 2023-11-14 11:21:20.178458 pref_voting-1.3.1/pref_voting/axiom.py
--rw-r--r--   0        0        0      360 2023-05-10 11:16:28.091090 pref_voting-1.3.1/pref_voting/axiom_helpers.py
--rw-r--r--   0        0        0       91 2023-05-25 14:07:56.083200 pref_voting-1.3.1/pref_voting/axioms.py
--rw-r--r--   0        0        0    36988 2024-05-05 11:00:01.290334 pref_voting-1.3.1/pref_voting/c1_methods.py
--rw-r--r--   0        0        0    17962 2024-05-05 11:00:01.291557 pref_voting-1.3.1/pref_voting/combined_methods.py
--rw-r--r--   0        0        0    12837 2024-05-03 10:23:29.480445 pref_voting-1.3.1/pref_voting/dominance_axioms.py
--rw-r--r--   0        0        0    24283 2024-04-24 20:51:32.848337 pref_voting-1.3.1/pref_voting/generate_profiles.py
--rw-r--r--   0        0        0     7648 2023-09-26 23:38:41.018490 pref_voting-1.3.1/pref_voting/generate_spatial_profiles.py
--rw-r--r--   0        0        0     6181 2023-11-14 11:21:22.463664 pref_voting-1.3.1/pref_voting/generate_utility_profiles.py
--rw-r--r--   0        0        0    12781 2024-01-20 19:48:28.167312 pref_voting-1.3.1/pref_voting/generate_weighted_majority_graphs.py
--rw-r--r--   0        0        0     8796 2024-03-02 21:50:31.229821 pref_voting-1.3.1/pref_voting/grade_methods.py
--rw-r--r--   0        0        0    15536 2024-02-19 21:31:17.860108 pref_voting-1.3.1/pref_voting/grade_profiles.py
--rw-r--r--   0        0        0     8058 2024-05-05 11:00:01.292540 pref_voting-1.3.1/pref_voting/helper.py
--rw-r--r--   0        0        0    12710 2023-10-25 22:23:58.100791 pref_voting-1.3.1/pref_voting/invariance_axioms.py
--rw-r--r--   0        0        0        0 2024-03-17 12:02:53.705325 pref_voting-1.3.1/pref_voting/io/__init__.py
--rw-r--r--   0        0        0    17327 2024-04-15 10:20:24.422714 pref_voting-1.3.1/pref_voting/io/readers.py
--rw-r--r--   0        0        0     9283 2024-04-15 10:10:45.393951 pref_voting-1.3.1/pref_voting/io/writers.py
--rw-r--r--   0        0        0    99732 2024-05-05 11:00:01.292969 pref_voting-1.3.1/pref_voting/iterative_methods.py
--rw-r--r--   0        0        0    20246 2022-07-12 12:12:35.000000 pref_voting-1.3.1/pref_voting/maj_graph_ex1.png
--rw-r--r--   0        0        0    22586 2024-04-15 17:48:22.507316 pref_voting-1.3.1/pref_voting/mappings.py
--rw-r--r--   0        0        0    77572 2024-05-05 19:27:20.666310 pref_voting-1.3.1/pref_voting/margin_based_methods.py
--rw-r--r--   0        0        0    70814 2024-04-27 22:10:28.624211 pref_voting-1.3.1/pref_voting/margin_based_methods_old.py
--rw-r--r--   0        0        0    39807 2024-04-15 09:43:01.243011 pref_voting-1.3.1/pref_voting/monotonicity_axioms.py
--rw-r--r--   0        0        0    30314 2024-05-05 11:00:01.294267 pref_voting-1.3.1/pref_voting/other_methods.py
--rw-r--r--   0        0        0     2994 2024-04-15 22:33:37.313589 pref_voting-1.3.1/pref_voting/prob_voting_method.py
--rw-r--r--   0        0        0     4338 2024-04-15 22:36:04.584538 pref_voting-1.3.1/pref_voting/probabilistic_methods.py
--rw-r--r--   0        0        0    30126 2024-03-21 11:19:48.716586 pref_voting-1.3.1/pref_voting/profiles.py
--rw-r--r--   0        0        0    31608 2024-03-19 11:44:23.373414 pref_voting-1.3.1/pref_voting/profiles_with_ties.py
--rw-r--r--   0        0        0    13859 2024-03-03 16:50:37.545900 pref_voting-1.3.1/pref_voting/rankings.py
--rw-r--r--   0        0        0    23114 2024-05-05 11:00:01.294774 pref_voting-1.3.1/pref_voting/scoring_methods.py
--rw-r--r--   0        0        0     1891 2024-04-15 22:36:47.601045 pref_voting-1.3.1/pref_voting/social_welfare_function.py
--rw-r--r--   0        0        0      362 2024-02-16 02:11:21.780066 pref_voting-1.3.1/pref_voting/social_welfare_functions.py
--rw-r--r--   0        0        0     7395 2024-03-19 17:48:42.747157 pref_voting-1.3.1/pref_voting/spatial_profiles.py
--rw-r--r--   0        0        0    15790 2024-04-30 00:43:41.503635 pref_voting-1.3.1/pref_voting/strategic_axioms.py
--rw-r--r--   0        0        0     7881 2024-05-01 10:27:56.905820 pref_voting-1.3.1/pref_voting/swf_axioms.py
--rw-r--r--   0        0        0        0 2023-12-03 11:15:38.617857 pref_voting-1.3.1/pref_voting/tests/__init__.py
--rw-r--r--   0        0        0      745 2024-04-28 20:04:29.865701 pref_voting-1.3.1/pref_voting/tests/conftest.py
--rw-r--r--   0        0        0     5690 2024-04-28 20:01:53.768645 pref_voting-1.3.1/pref_voting/tests/test_c1_methods.py
--rw-r--r--   0        0        0     3092 2024-04-28 20:01:53.768816 pref_voting-1.3.1/pref_voting/tests/test_combined_methods.py
--rw-r--r--   0        0        0    12962 2024-04-24 20:08:43.229903 pref_voting-1.3.1/pref_voting/tests/test_generate_profiles.py
--rw-r--r--   0        0        0     2504 2024-03-19 18:59:44.204010 pref_voting-1.3.1/pref_voting/tests/test_generate_spatial_profile.py
--rw-r--r--   0        0        0    15002 2024-04-15 10:21:41.931501 pref_voting-1.3.1/pref_voting/tests/test_io.py
--rw-r--r--   0        0        0    11606 2024-04-28 20:41:27.682198 pref_voting-1.3.1/pref_voting/tests/test_iterative_methods.py
--rw-r--r--   0        0        0    11912 2024-03-16 21:03:40.865827 pref_voting-1.3.1/pref_voting/tests/test_majority_graph.py
--rw-r--r--   0        0        0     6284 2024-04-15 17:49:58.759298 pref_voting-1.3.1/pref_voting/tests/test_mapping.py
--rw-r--r--   0        0        0    10335 2024-04-28 12:01:51.077156 pref_voting-1.3.1/pref_voting/tests/test_margin_based_methods.py
--rw-r--r--   0        0        0     7778 2024-04-08 19:41:37.247861 pref_voting-1.3.1/pref_voting/tests/test_margin_graph.py
--rw-r--r--   0        0        0     3722 2024-03-17 11:44:20.741638 pref_voting-1.3.1/pref_voting/tests/test_other_methods.py
--rw-r--r--   0        0        0     1815 2024-04-15 22:34:08.166452 pref_voting-1.3.1/pref_voting/tests/test_prob_voting_method.py
--rw-r--r--   0        0        0    11558 2024-03-19 11:40:09.393149 pref_voting-1.3.1/pref_voting/tests/test_profile.py
--rw-r--r--   0        0        0    20184 2024-04-08 19:41:37.248346 pref_voting-1.3.1/pref_voting/tests/test_profile_with_ties.py
--rw-r--r--   0        0        0     8964 2024-03-17 10:17:34.347218 pref_voting-1.3.1/pref_voting/tests/test_ranking.py
--rw-r--r--   0        0        0     6234 2024-04-28 20:40:55.278187 pref_voting-1.3.1/pref_voting/tests/test_scoring_rules.py
--rw-r--r--   0        0        0     1531 2024-04-15 14:32:09.859043 pref_voting-1.3.1/pref_voting/tests/test_social_welfare_functions.py
--rw-r--r--   0        0        0     5459 2024-04-08 19:41:37.248846 pref_voting-1.3.1/pref_voting/tests/test_spatial_profile.py
--rw-r--r--   0        0        0     2429 2024-04-08 19:41:37.249181 pref_voting-1.3.1/pref_voting/tests/test_support_graph.py
--rw-r--r--   0        0        0     3808 2024-04-15 19:15:01.227825 pref_voting-1.3.1/pref_voting/tests/test_utility_function.py
--rw-r--r--   0        0        0     1943 2024-03-19 18:31:19.950002 pref_voting-1.3.1/pref_voting/tests/test_utility_functions.py
--rw-r--r--   0        0        0     1585 2024-04-08 19:41:37.249465 pref_voting-1.3.1/pref_voting/tests/test_voting_method.py
--rw-r--r--   0        0        0     3963 2024-04-08 22:35:46.799439 pref_voting-1.3.1/pref_voting/utility_functions.py
--rw-r--r--   0        0        0     7245 2024-02-16 01:32:30.000312 pref_voting-1.3.1/pref_voting/utility_methods.py
--rw-r--r--   0        0        0    12673 2024-02-19 23:28:54.492364 pref_voting-1.3.1/pref_voting/utility_profiles.py
--rw-r--r--   0        0        0    18724 2023-12-05 16:58:20.198435 pref_voting-1.3.1/pref_voting/variable_candidate_axioms.py
--rw-r--r--   0        0        0    91144 2024-05-03 10:23:29.483544 pref_voting-1.3.1/pref_voting/variable_voter_axioms.py
--rw-r--r--   0        0        0     7213 2024-05-05 19:29:16.212390 pref_voting-1.3.1/pref_voting/voting_method.py
--rw-r--r--   0        0        0     1341 2024-04-30 00:59:45.610622 pref_voting-1.3.1/pref_voting/voting_method_properties.py
--rw-r--r--   0        0        0      254 2024-05-04 20:05:10.058403 pref_voting-1.3.1/pref_voting/voting_methods.py
--rw-r--r--   0        0        0     4679 2024-05-04 21:29:02.086406 pref_voting-1.3.1/pref_voting/voting_methods_registry.py
--rw-r--r--   0        0        0    57320 2024-04-08 19:41:37.250216 pref_voting-1.3.1/pref_voting/weighted_majority_graphs.py
--rw-r--r--   0        0        0      760 2024-05-05 19:29:36.348083 pref_voting-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     2855 1970-01-01 00:00:00.000000 pref_voting-1.3.1/setup.py
--rw-r--r--   0        0        0     2996 1970-01-01 00:00:00.000000 pref_voting-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1085 2024-03-19 19:26:58.359673 pref_voting-1.3.2/LICENSE
+-rw-r--r--   0        0        0     1770 2024-04-24 21:45:43.110237 pref_voting-1.3.2/README.md
+-rw-r--r--   0        0        0       22 2024-05-10 21:47:10.807987 pref_voting-1.3.2/pref_voting/__init__.py
+-rw-r--r--   0        0        0    18867 2023-11-14 11:21:19.592605 pref_voting-1.3.2/pref_voting/analysis.py
+-rw-r--r--   0        0        0     1270 2023-11-14 11:21:20.178458 pref_voting-1.3.2/pref_voting/axiom.py
+-rw-r--r--   0        0        0      360 2023-05-10 11:16:28.091090 pref_voting-1.3.2/pref_voting/axiom_helpers.py
+-rw-r--r--   0        0        0       91 2023-05-25 14:07:56.083200 pref_voting-1.3.2/pref_voting/axioms.py
+-rw-r--r--   0        0        0    36988 2024-05-05 11:00:01.290334 pref_voting-1.3.2/pref_voting/c1_methods.py
+-rw-r--r--   0        0        0    17962 2024-05-05 11:00:01.291557 pref_voting-1.3.2/pref_voting/combined_methods.py
+-rw-r--r--   0        0        0    12837 2024-05-03 10:23:29.480445 pref_voting-1.3.2/pref_voting/dominance_axioms.py
+-rw-r--r--   0        0        0    24283 2024-04-24 20:51:32.848337 pref_voting-1.3.2/pref_voting/generate_profiles.py
+-rw-r--r--   0        0        0     7648 2023-09-26 23:38:41.018490 pref_voting-1.3.2/pref_voting/generate_spatial_profiles.py
+-rw-r--r--   0        0        0     6181 2023-11-14 11:21:22.463664 pref_voting-1.3.2/pref_voting/generate_utility_profiles.py
+-rw-r--r--   0        0        0    12781 2024-01-20 19:48:28.167312 pref_voting-1.3.2/pref_voting/generate_weighted_majority_graphs.py
+-rw-r--r--   0        0        0     8796 2024-03-02 21:50:31.229821 pref_voting-1.3.2/pref_voting/grade_methods.py
+-rw-r--r--   0        0        0    15536 2024-02-19 21:31:17.860108 pref_voting-1.3.2/pref_voting/grade_profiles.py
+-rw-r--r--   0        0        0     8058 2024-05-05 11:00:01.292540 pref_voting-1.3.2/pref_voting/helper.py
+-rw-r--r--   0        0        0    12710 2023-10-25 22:23:58.100791 pref_voting-1.3.2/pref_voting/invariance_axioms.py
+-rw-r--r--   0        0        0        0 2024-03-17 12:02:53.705325 pref_voting-1.3.2/pref_voting/io/__init__.py
+-rw-r--r--   0        0        0    17327 2024-04-15 10:20:24.422714 pref_voting-1.3.2/pref_voting/io/readers.py
+-rw-r--r--   0        0        0     9283 2024-04-15 10:10:45.393951 pref_voting-1.3.2/pref_voting/io/writers.py
+-rw-r--r--   0        0        0    99843 2024-05-06 20:13:55.325756 pref_voting-1.3.2/pref_voting/iterative_methods.py
+-rw-r--r--   0        0        0    20246 2022-07-12 12:12:35.000000 pref_voting-1.3.2/pref_voting/maj_graph_ex1.png
+-rw-r--r--   0        0        0    22586 2024-04-15 17:48:22.507316 pref_voting-1.3.2/pref_voting/mappings.py
+-rw-r--r--   0        0        0    79313 2024-05-10 21:46:49.192278 pref_voting-1.3.2/pref_voting/margin_based_methods.py
+-rw-r--r--   0        0        0    70814 2024-04-27 22:10:28.624211 pref_voting-1.3.2/pref_voting/margin_based_methods_old.py
+-rw-r--r--   0        0        0    39807 2024-04-15 09:43:01.243011 pref_voting-1.3.2/pref_voting/monotonicity_axioms.py
+-rw-r--r--   0        0        0    30314 2024-05-05 11:00:01.294267 pref_voting-1.3.2/pref_voting/other_methods.py
+-rw-r--r--   0        0        0     2994 2024-04-15 22:33:37.313589 pref_voting-1.3.2/pref_voting/prob_voting_method.py
+-rw-r--r--   0        0        0     4338 2024-04-15 22:36:04.584538 pref_voting-1.3.2/pref_voting/probabilistic_methods.py
+-rw-r--r--   0        0        0    30126 2024-05-06 22:04:52.586763 pref_voting-1.3.2/pref_voting/profiles.py
+-rw-r--r--   0        0        0    31608 2024-03-19 11:44:23.373414 pref_voting-1.3.2/pref_voting/profiles_with_ties.py
+-rw-r--r--   0        0        0    13859 2024-03-03 16:50:37.545900 pref_voting-1.3.2/pref_voting/rankings.py
+-rw-r--r--   0        0        0    23114 2024-05-05 11:00:01.294774 pref_voting-1.3.2/pref_voting/scoring_methods.py
+-rw-r--r--   0        0        0     1891 2024-04-15 22:36:47.601045 pref_voting-1.3.2/pref_voting/social_welfare_function.py
+-rw-r--r--   0        0        0      362 2024-02-16 02:11:21.780066 pref_voting-1.3.2/pref_voting/social_welfare_functions.py
+-rw-r--r--   0        0        0     7395 2024-03-19 17:48:42.747157 pref_voting-1.3.2/pref_voting/spatial_profiles.py
+-rw-r--r--   0        0        0    15790 2024-04-30 00:43:41.503635 pref_voting-1.3.2/pref_voting/strategic_axioms.py
+-rw-r--r--   0        0        0     7881 2024-05-01 10:27:56.905820 pref_voting-1.3.2/pref_voting/swf_axioms.py
+-rw-r--r--   0        0        0        0 2023-12-03 11:15:38.617857 pref_voting-1.3.2/pref_voting/tests/__init__.py
+-rw-r--r--   0        0        0      745 2024-04-28 20:04:29.865701 pref_voting-1.3.2/pref_voting/tests/conftest.py
+-rw-r--r--   0        0        0     5690 2024-04-28 20:01:53.768645 pref_voting-1.3.2/pref_voting/tests/test_c1_methods.py
+-rw-r--r--   0        0        0     3092 2024-04-28 20:01:53.768816 pref_voting-1.3.2/pref_voting/tests/test_combined_methods.py
+-rw-r--r--   0        0        0    12962 2024-04-24 20:08:43.229903 pref_voting-1.3.2/pref_voting/tests/test_generate_profiles.py
+-rw-r--r--   0        0        0     2504 2024-03-19 18:59:44.204010 pref_voting-1.3.2/pref_voting/tests/test_generate_spatial_profile.py
+-rw-r--r--   0        0        0    15002 2024-04-15 10:21:41.931501 pref_voting-1.3.2/pref_voting/tests/test_io.py
+-rw-r--r--   0        0        0    11606 2024-04-28 20:41:27.682198 pref_voting-1.3.2/pref_voting/tests/test_iterative_methods.py
+-rw-r--r--   0        0        0    11912 2024-03-16 21:03:40.865827 pref_voting-1.3.2/pref_voting/tests/test_majority_graph.py
+-rw-r--r--   0        0        0     6284 2024-04-15 17:49:58.759298 pref_voting-1.3.2/pref_voting/tests/test_mapping.py
+-rw-r--r--   0        0        0    10335 2024-04-28 12:01:51.077156 pref_voting-1.3.2/pref_voting/tests/test_margin_based_methods.py
+-rw-r--r--   0        0        0     7778 2024-04-08 19:41:37.247861 pref_voting-1.3.2/pref_voting/tests/test_margin_graph.py
+-rw-r--r--   0        0        0     3722 2024-03-17 11:44:20.741638 pref_voting-1.3.2/pref_voting/tests/test_other_methods.py
+-rw-r--r--   0        0        0     1815 2024-04-15 22:34:08.166452 pref_voting-1.3.2/pref_voting/tests/test_prob_voting_method.py
+-rw-r--r--   0        0        0    11558 2024-03-19 11:40:09.393149 pref_voting-1.3.2/pref_voting/tests/test_profile.py
+-rw-r--r--   0        0        0    20184 2024-04-08 19:41:37.248346 pref_voting-1.3.2/pref_voting/tests/test_profile_with_ties.py
+-rw-r--r--   0        0        0     8964 2024-03-17 10:17:34.347218 pref_voting-1.3.2/pref_voting/tests/test_ranking.py
+-rw-r--r--   0        0        0     6234 2024-04-28 20:40:55.278187 pref_voting-1.3.2/pref_voting/tests/test_scoring_rules.py
+-rw-r--r--   0        0        0     1531 2024-04-15 14:32:09.859043 pref_voting-1.3.2/pref_voting/tests/test_social_welfare_functions.py
+-rw-r--r--   0        0        0     5459 2024-04-08 19:41:37.248846 pref_voting-1.3.2/pref_voting/tests/test_spatial_profile.py
+-rw-r--r--   0        0        0     2429 2024-04-08 19:41:37.249181 pref_voting-1.3.2/pref_voting/tests/test_support_graph.py
+-rw-r--r--   0        0        0     3808 2024-04-15 19:15:01.227825 pref_voting-1.3.2/pref_voting/tests/test_utility_function.py
+-rw-r--r--   0        0        0     1943 2024-03-19 18:31:19.950002 pref_voting-1.3.2/pref_voting/tests/test_utility_functions.py
+-rw-r--r--   0        0        0     1585 2024-04-08 19:41:37.249465 pref_voting-1.3.2/pref_voting/tests/test_voting_method.py
+-rw-r--r--   0        0        0     3963 2024-04-08 22:35:46.799439 pref_voting-1.3.2/pref_voting/utility_functions.py
+-rw-r--r--   0        0        0     7245 2024-02-16 01:32:30.000312 pref_voting-1.3.2/pref_voting/utility_methods.py
+-rw-r--r--   0        0        0    12673 2024-02-19 23:28:54.492364 pref_voting-1.3.2/pref_voting/utility_profiles.py
+-rw-r--r--   0        0        0    18724 2023-12-05 16:58:20.198435 pref_voting-1.3.2/pref_voting/variable_candidate_axioms.py
+-rw-r--r--   0        0        0    91144 2024-05-03 10:23:29.483544 pref_voting-1.3.2/pref_voting/variable_voter_axioms.py
+-rw-r--r--   0        0        0     7222 2024-05-09 10:50:06.223765 pref_voting-1.3.2/pref_voting/voting_method.py
+-rw-r--r--   0        0        0     1341 2024-04-30 00:59:45.610622 pref_voting-1.3.2/pref_voting/voting_method_properties.py
+-rw-r--r--   0        0        0      254 2024-05-04 20:05:10.058403 pref_voting-1.3.2/pref_voting/voting_methods.py
+-rw-r--r--   0        0        0     4679 2024-05-04 21:29:02.086406 pref_voting-1.3.2/pref_voting/voting_methods_registry.py
+-rw-r--r--   0        0        0    57320 2024-04-08 19:41:37.250216 pref_voting-1.3.2/pref_voting/weighted_majority_graphs.py
+-rw-r--r--   0        0        0      760 2024-05-10 21:47:10.806547 pref_voting-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0     2855 1970-01-01 00:00:00.000000 pref_voting-1.3.2/setup.py
+-rw-r--r--   0        0        0     2996 1970-01-01 00:00:00.000000 pref_voting-1.3.2/PKG-INFO
```

### Comparing `pref_voting-1.3.1/LICENSE` & `pref_voting-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.1/README.md` & `pref_voting-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.1/pref_voting/analysis.py` & `pref_voting-1.3.2/pref_voting/analysis.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.1/pref_voting/axiom.py` & `pref_voting-1.3.2/pref_voting/axiom.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.1/pref_voting/c1_methods.py` & `pref_voting-1.3.2/pref_voting/c1_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.1/pref_voting/combined_methods.py` & `pref_voting-1.3.2/pref_voting/combined_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.1/pref_voting/dominance_axioms.py` & `pref_voting-1.3.2/pref_voting/dominance_axioms.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.1/pref_voting/generate_profiles.py` & `pref_voting-1.3.2/pref_voting/generate_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.1/pref_voting/generate_spatial_profiles.py` & `pref_voting-1.3.2/pref_voting/generate_spatial_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.1/pref_voting/generate_utility_profiles.py` & `pref_voting-1.3.2/pref_voting/generate_utility_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.1/pref_voting/generate_weighted_majority_graphs.py` & `pref_voting-1.3.2/pref_voting/generate_weighted_majority_graphs.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.1/pref_voting/grade_methods.py` & `pref_voting-1.3.2/pref_voting/grade_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.1/pref_voting/grade_profiles.py` & `pref_voting-1.3.2/pref_voting/grade_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.1/pref_voting/helper.py` & `pref_voting-1.3.2/pref_voting/helper.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.1/pref_voting/invariance_axioms.py` & `pref_voting-1.3.2/pref_voting/invariance_axioms.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.1/pref_voting/io/readers.py` & `pref_voting-1.3.2/pref_voting/io/readers.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.1/pref_voting/io/writers.py` & `pref_voting-1.3.2/pref_voting/io/writers.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.1/pref_voting/iterative_methods.py` & `pref_voting-1.3.2/pref_voting/iterative_methods.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,18 +122,21 @@
     
     else:
         raise ValueError("Algorithm must be either 'basic' or 'recursive'.")
 
 # Create some aliases for instant runoff
 instant_runoff.set_name("Hare")
 hare = copy.deepcopy(instant_runoff)
+hare.skip_registration = True
 instant_runoff.set_name("Ranked Choice")
 ranked_choice = copy.deepcopy(instant_runoff)
+ranked_choice.skip_registration = True
 instant_runoff.set_name("Alternative Vote")
 alternative_vote = copy.deepcopy(instant_runoff)
+alternative_vote.skip_registration = True
 
 # reset the name Instant Runoff
 instant_runoff.set_name("Instant Runoff")
 
 @swf(name = "Instant Runoff Ranking")
 def instant_runoff_ranking(profile, curr_cands = None):
     """Returns the reverse of the elimination order in the instant runoff voting process.
```

### Comparing `pref_voting-1.3.1/pref_voting/maj_graph_ex1.png` & `pref_voting-1.3.2/pref_voting/maj_graph_ex1.png`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.1/pref_voting/mappings.py` & `pref_voting-1.3.2/pref_voting/mappings.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.1/pref_voting/margin_based_methods.py` & `pref_voting-1.3.2/pref_voting/margin_based_methods.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,4812 +38,4921 @@
 00000250: 696e 0a69 6d70 6f72 7420 6e65 7477 6f72  in.import networ
 00000260: 6b78 2061 7320 6e78 0a66 726f 6d20 7072  kx as nx.from pr
 00000270: 6566 5f76 6f74 696e 672e 766f 7469 6e67  ef_voting.voting
 00000280: 5f6d 6574 686f 645f 7072 6f70 6572 7469  _method_properti
 00000290: 6573 2069 6d70 6f72 7420 566f 7469 6e67  es import Voting
 000002a0: 4d65 7468 6f64 5072 6f70 6572 7469 6573  MethodProperties
 000002b0: 2c20 456c 6563 7469 6f6e 5479 7065 730a  , ElectionTypes.
-000002c0: 0a6d 696e 696d 6178 5f70 726f 7065 7274  .minimax_propert
-000002d0: 6965 7320 3d20 566f 7469 6e67 4d65 7468  ies = VotingMeth
-000002e0: 6f64 5072 6f70 6572 7469 6573 280a 2020  odProperties(.  
-000002f0: 2020 636f 6e64 6f72 6365 745f 7769 6e6e    condorcet_winn
-00000300: 6572 3d54 7275 652c 200a 2020 2020 636f  er=True, .    co
-00000310: 6e64 6f72 6365 745f 6c6f 7365 723d 4661  ndorcet_loser=Fa
-00000320: 6c73 652c 0a20 2020 2070 6172 6574 6f5f  lse,.    pareto_
-00000330: 646f 6d69 6e61 6e63 653d 5472 7565 2c0a  dominance=True,.
-00000340: 2020 2020 706f 7369 7469 7665 5f69 6e76      positive_inv
-00000350: 6f6c 7665 6d65 6e74 3d54 7275 652c 200a  olvement=True, .
-00000360: 2020 2020 290a 4076 6d28 6e61 6d65 203d      ).@vm(name =
-00000370: 2022 4d69 6e69 6d61 7822 2c0a 2020 2020   "Minimax",.    
-00000380: 7072 6f70 6572 7469 6573 3d6d 696e 696d  properties=minim
-00000390: 6178 5f70 726f 7065 7274 6965 732c 0a20  ax_properties,. 
-000003a0: 2020 2069 6e70 7574 5f74 7970 6573 3d5b     input_types=[
-000003b0: 456c 6563 7469 6f6e 5479 7065 732e 5052  ElectionTypes.PR
-000003c0: 4f46 494c 452c 2045 6c65 6374 696f 6e54  OFILE, ElectionT
-000003d0: 7970 6573 2e50 524f 4649 4c45 5f57 4954  ypes.PROFILE_WIT
-000003e0: 485f 5449 4553 2c20 456c 6563 7469 6f6e  H_TIES, Election
-000003f0: 5479 7065 732e 4d41 5247 494e 5f47 5241  Types.MARGIN_GRA
-00000400: 5048 5d0a 2020 2020 290a 6465 6620 6d69  PH].    ).def mi
-00000410: 6e69 6d61 7828 6564 6174 612c 2063 7572  nimax(edata, cur
-00000420: 725f 6361 6e64 7320 3d20 4e6f 6e65 2c20  r_cands = None, 
-00000430: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
-00000440: 6e20 3d20 4e6f 6e65 293a 2020 200a 2020  n = None):   .  
-00000450: 2020 2222 220a 2020 2020 5468 6520 4d69    """.    The Mi
-00000460: 6e69 6d61 7820 7769 6e6e 6572 7320 6172  nimax winners ar
-00000470: 6520 7468 6520 6361 6e64 6964 6174 6573  e the candidates
-00000480: 2077 6974 6820 7468 6520 736d 616c 6c65   with the smalle
-00000490: 7374 206d 6178 696d 756d 2070 6169 7277  st maximum pairw
-000004a0: 6973 6520 6c6f 7373 2e20 2054 6861 7420  ise loss.  That 
-000004b0: 6973 2c20 666f 7220 6561 6368 2063 616e  is, for each can
-000004c0: 6469 6461 7465 203a 6d61 7468 3a60 6160  didate :math:`a`
-000004d0: 2c20 6669 6e64 2074 6865 2062 6967 6765  , find the bigge
-000004e0: 7374 206d 6172 6769 6e20 6f66 2061 2063  st margin of a c
-000004f0: 616e 6469 6461 7465 203a 6d61 7468 3a60  andidate :math:`
-00000500: 6260 206f 7665 7220 3a6d 6174 683a 6061  b` over :math:`a
-00000510: 602c 2074 6865 6e20 656c 6563 7420 7468  `, then elect th
-00000520: 6520 6361 6e64 6964 6174 6528 7329 2077  e candidate(s) w
-00000530: 6974 6820 7468 6520 736d 616c 6c65 7374  ith the smallest
-00000540: 2073 7563 6820 6c6f 7373 2e20 416c 736f   such loss. Also
-00000550: 206b 6e6f 776e 2061 7320 7468 6520 5369   known as the Si
-00000560: 6d70 736f 6e2d 4b72 616d 6572 2052 756c  mpson-Kramer Rul
-00000570: 652e 0a20 2020 200a 2020 2020 4172 6773  e..    .    Args
-00000580: 3a0a 2020 2020 2020 2020 6564 6174 6120  :.        edata 
-00000590: 2850 726f 6669 6c65 2c20 5072 6f66 696c  (Profile, Profil
-000005a0: 6557 6974 6854 6965 732c 204d 6172 6769  eWithTies, Margi
-000005b0: 6e47 7261 7068 293a 2041 6e79 2065 6c65  nGraph): Any ele
-000005c0: 6374 696f 6e20 6461 7461 2074 6861 7420  ction data that 
-000005d0: 6861 7320 6120 606d 6172 6769 6e60 206d  has a `margin` m
-000005e0: 6574 686f 642e 200a 2020 2020 2020 2020  ethod. .        
-000005f0: 6375 7272 5f63 616e 6473 2028 4c69 7374  curr_cands (List
-00000600: 5b69 6e74 5d2c 206f 7074 696f 6e61 6c29  [int], optional)
-00000610: 3a20 4966 2073 6574 2c20 7468 656e 2066  : If set, then f
-00000620: 696e 6420 7468 6520 7769 6e6e 6572 7320  ind the winners 
-00000630: 666f 7220 7468 6520 7072 6f66 696c 6520  for the profile 
-00000640: 7265 7374 7269 6374 6564 2074 6f20 7468  restricted to th
-00000650: 6520 6361 6e64 6964 6174 6573 2069 6e20  e candidates in 
-00000660: 6060 6375 7272 5f63 616e 6473 6060 0a0a  ``curr_cands``..
-00000670: 2020 2020 5265 7475 726e 733a 200a 2020      Returns: .  
-00000680: 2020 2020 2020 4120 736f 7274 6564 206c        A sorted l
-00000690: 6973 7420 6f66 2063 616e 6469 6461 7465  ist of candidate
-000006a0: 730a 0a20 2020 202e 2e20 7365 6561 6c73  s..    .. seeals
-000006b0: 6f3a 3a0a 0a20 2020 2020 2020 203a 6d65  o::..        :me
-000006c0: 7468 3a60 7072 6566 5f76 6f74 696e 672e  th:`pref_voting.
-000006d0: 6d61 7267 696e 5f62 6173 6564 5f6d 6574  margin_based_met
-000006e0: 686f 6473 2e6d 696e 696d 6178 5f73 636f  hods.minimax_sco
-000006f0: 7265 7360 0a0a 2020 2020 3a45 7861 6d70  res`..    :Examp
-00000700: 6c65 3a20 0a0a 2020 2020 2e2e 2070 6c6f  le: ..    .. plo
-00000710: 743a 3a20 206d 6172 6769 6e5f 6772 6170  t::  margin_grap
-00000720: 6873 5f65 7861 6d70 6c65 732f 6d67 5f65  hs_examples/mg_e
-00000730: 785f 6d69 6e69 6d61 782e 7079 0a20 2020  x_minimax.py.   
-00000740: 2020 2020 203a 636f 6e74 6578 743a 2072       :context: r
-00000750: 6573 6574 2020 0a20 2020 2020 2020 203a  eset  .        :
-00000760: 696e 636c 7564 652d 736f 7572 6365 3a20  include-source: 
-00000770: 5472 7565 0a0a 0a20 2020 202e 2e20 636f  True...    .. co
-00000780: 6465 2d62 6c6f 636b 3a3a 200a 0a20 2020  de-block:: ..   
-00000790: 2020 2020 2066 726f 6d20 7072 6566 5f76       from pref_v
-000007a0: 6f74 696e 672e 6d61 7267 696e 5f62 6173  oting.margin_bas
-000007b0: 6564 5f6d 6574 686f 6473 2069 6d70 6f72  ed_methods impor
-000007c0: 7420 6d69 6e69 6d61 780a 0a20 2020 2020  t minimax..     
-000007d0: 2020 206d 696e 696d 6178 2e64 6973 706c     minimax.displ
-000007e0: 6179 2870 726f 6629 0a0a 0a20 2020 202e  ay(prof)...    .
-000007f0: 2e20 6578 6563 5f63 6f64 653a 3a20 0a20  . exec_code:: . 
-00000800: 2020 2020 2020 203a 6869 6465 5f63 6f64         :hide_cod
-00000810: 653a 0a0a 2020 2020 2020 2020 6672 6f6d  e:..        from
-00000820: 2070 7265 665f 766f 7469 6e67 2e70 726f   pref_voting.pro
-00000830: 6669 6c65 7320 696d 706f 7274 2050 726f  files import Pro
-00000840: 6669 6c65 0a20 2020 2020 2020 2066 726f  file.        fro
-00000850: 6d20 7072 6566 5f76 6f74 696e 672e 6d61  m pref_voting.ma
-00000860: 7267 696e 5f62 6173 6564 5f6d 6574 686f  rgin_based_metho
-00000870: 6473 2069 6d70 6f72 7420 6d69 6e69 6d61  ds import minima
-00000880: 780a 2020 2020 2020 2020 0a20 2020 2020  x.        .     
-00000890: 2020 2070 726f 6620 3d20 5072 6f66 696c     prof = Profil
-000008a0: 6528 5b5b 332c 2030 2c20 312c 2032 5d2c  e([[3, 0, 1, 2],
-000008b0: 205b 312c 2033 2c20 322c 2030 5d2c 205b   [1, 3, 2, 0], [
-000008c0: 312c 2033 2c20 302c 2032 5d2c 205b 312c  1, 3, 0, 2], [1,
-000008d0: 2032 2c20 302c 2033 5d2c 205b 332c 2032   2, 0, 3], [3, 2
-000008e0: 2c20 302c 2031 5d2c 205b 302c 2032 2c20  , 0, 1], [0, 2, 
-000008f0: 312c 2033 5d5d 2c20 5b31 2c20 312c 2031  1, 3]], [1, 1, 1
-00000900: 2c20 312c 2032 2c20 315d 290a 0a20 2020  , 1, 2, 1])..   
-00000910: 2020 2020 206d 696e 696d 6178 2e64 6973       minimax.dis
-00000920: 706c 6179 2870 726f 6629 0a0a 2020 2020  play(prof)..    
-00000930: 2222 220a 0a20 2020 2063 616e 6469 6461  """..    candida
-00000940: 7465 7320 3d20 6564 6174 612e 6361 6e64  tes = edata.cand
-00000950: 6964 6174 6573 2069 6620 6375 7272 5f63  idates if curr_c
-00000960: 616e 6473 2069 7320 4e6f 6e65 2065 6c73  ands is None els
-00000970: 6520 6375 7272 5f63 616e 6473 2020 2020  e curr_cands    
-00000980: 0a20 2020 2073 7472 656e 6774 685f 6675  .    strength_fu
-00000990: 6e63 7469 6f6e 203d 2065 6461 7461 2e6d  nction = edata.m
-000009a0: 6172 6769 6e20 6966 2073 7472 656e 6774  argin if strengt
-000009b0: 685f 6675 6e63 7469 6f6e 2069 7320 4e6f  h_function is No
-000009c0: 6e65 2065 6c73 6520 7374 7265 6e67 7468  ne else strength
-000009d0: 5f66 756e 6374 696f 6e0a 0a20 2020 2073  _function..    s
-000009e0: 636f 7265 7320 3d20 7b63 3a20 6d61 7828  cores = {c: max(
-000009f0: 5b73 7472 656e 6774 685f 6675 6e63 7469  [strength_functi
-00000a00: 6f6e 285f 632c 2063 2920 666f 7220 5f63  on(_c, c) for _c
-00000a10: 2069 6e20 6564 6174 612e 646f 6d69 6e61   in edata.domina
-00000a20: 746f 7273 2863 2920 6966 205f 6320 696e  tors(c) if _c in
-00000a30: 2063 616e 6469 6461 7465 735d 2920 6966   candidates]) if
-00000a40: 2061 6e79 285b 5f63 2069 6e20 6564 6174   any([_c in edat
-00000a50: 612e 646f 6d69 6e61 746f 7273 2863 2920  a.dominators(c) 
-00000a60: 666f 7220 5f63 2069 6e20 6361 6e64 6964  for _c in candid
-00000a70: 6174 6573 5d29 2065 6c73 6520 3020 0a20  ates]) else 0 . 
-00000a80: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-00000a90: 2063 2069 6e20 6361 6e64 6964 6174 6573   c in candidates
-00000aa0: 7d0a 2020 2020 6d69 6e5f 7363 6f72 6520  }.    min_score 
-00000ab0: 3d20 6d69 6e28 7363 6f72 6573 2e76 616c  = min(scores.val
-00000ac0: 7565 7328 2929 0a20 2020 2072 6574 7572  ues()).    retur
-00000ad0: 6e20 736f 7274 6564 285b 6320 666f 7220  n sorted([c for 
-00000ae0: 6320 696e 2063 616e 6469 6461 7465 7320  c in candidates 
-00000af0: 6966 2073 636f 7265 735b 635d 203d 3d20  if scores[c] == 
-00000b00: 6d69 6e5f 7363 6f72 655d 290a 0a0a 6465  min_score])...de
-00000b10: 6620 6d69 6e69 6d61 785f 7363 6f72 6573  f minimax_scores
-00000b20: 2865 6461 7461 2c20 6375 7272 5f63 616e  (edata, curr_can
-00000b30: 6473 203d 204e 6f6e 652c 2073 636f 7265  ds = None, score
-00000b40: 5f6d 6574 686f 643d 226d 6172 6769 6e73  _method="margins
-00000b50: 2229 3a0a 2020 2020 2222 2252 6574 7572  "):.    """Retur
-00000b60: 6e20 7468 6520 6d69 6e69 6d61 7820 7363  n the minimax sc
-00000b70: 6f72 6573 2066 6f72 2065 6163 6820 6361  ores for each ca
-00000b80: 6e64 6964 6174 652c 2077 6865 7265 2074  ndidate, where t
-00000b90: 6865 206d 696e 696d 6178 2073 636f 7265  he minimax score
-00000ba0: 2066 6f72 203a 6d61 7468 3a60 6360 2069   for :math:`c` i
-00000bb0: 7320 2d31 202a 2074 6865 206d 6178 696d  s -1 * the maxim
-00000bc0: 756d 2070 6169 7277 6973 6520 6d61 6a6f  um pairwise majo
-00000bd0: 7269 7479 206c 6f73 732e 200a 0a20 2020  rity loss. ..   
-00000be0: 2041 7267 733a 0a20 2020 2020 2020 2065   Args:.        e
-00000bf0: 6461 7461 2028 5072 6f66 696c 652c 2050  data (Profile, P
-00000c00: 726f 6669 6c65 5769 7468 5469 6573 2c20  rofileWithTies, 
-00000c10: 4d61 7267 696e 4772 6170 6829 3a20 416e  MarginGraph): An
-00000c20: 7920 656c 6563 7469 6f6e 2064 6174 6120  y election data 
-00000c30: 7468 6174 2068 6173 2061 2060 6d61 7267  that has a `marg
-00000c40: 696e 6020 6d65 7468 6f64 2e20 0a20 2020  in` method. .   
-00000c50: 2020 2020 2063 7572 725f 6361 6e64 7320       curr_cands 
-00000c60: 284c 6973 745b 696e 745d 2c20 6f70 7469  (List[int], opti
-00000c70: 6f6e 616c 293a 2049 6620 7365 742c 2074  onal): If set, t
-00000c80: 6865 6e20 6669 6e64 2074 6865 2077 696e  hen find the win
-00000c90: 6e65 7273 2066 6f72 2074 6865 2070 726f  ners for the pro
-00000ca0: 6669 6c65 2072 6573 7472 6963 7465 6420  file restricted 
-00000cb0: 746f 2074 6865 2063 616e 6469 6461 7465  to the candidate
-00000cc0: 7320 696e 2060 6063 7572 725f 6361 6e64  s in ``curr_cand
-00000cd0: 7360 600a 2020 2020 2020 2020 7363 6f72  s``.        scor
-00000ce0: 655f 6d65 7468 6f64 2028 7374 722c 206f  e_method (str, o
-00000cf0: 7074 696f 6e61 6c29 3a20 4f70 7469 6f6e  ptional): Option
-00000d00: 7320 696e 636c 7564 6520 226d 6172 6769  s include "margi
-00000d10: 6e73 2220 2874 6865 2064 6566 6175 6c74  ns" (the default
-00000d20: 292c 2022 7769 6e6e 696e 6722 2061 7373  ), "winning" ass
-00000d30: 6967 6e73 2074 6f20 6561 6368 2063 616e  igns to each can
-00000d40: 6469 6461 7465 203a 6d61 7468 3a60 6360  didate :math:`c`
-00000d50: 2074 6865 206d 6178 696d 756d 2073 7570   the maximum sup
-00000d60: 706f 7274 206f 6620 6120 6361 6e64 6964  port of a candid
-00000d70: 6174 6520 6d61 6a6f 7269 7479 2070 7265  ate majority pre
-00000d80: 6665 7272 6564 2074 6f20 3a6d 6174 683a  ferred to :math:
-00000d90: 6063 602c 2020 616e 6420 2270 6169 7277  `c`,  and "pairw
-00000da0: 6973 655f 6f70 706f 7369 7469 6f6e 2220  ise_opposition" 
-00000db0: 6173 7369 676e 7320 746f 2065 6163 6820  assigns to each 
-00000dc0: 6361 6e64 6964 6174 6520 3a6d 6174 683a  candidate :math:
-00000dd0: 6063 6020 7468 6520 6d61 7869 6d75 6d20  `c` the maximum 
-00000de0: 7375 7070 6f72 7420 6f66 2061 6e79 2063  support of any c
-00000df0: 616e 6469 6461 7465 206f 7665 7220 3a6d  andidate over :m
-00000e00: 6174 683a 6063 602e 2020 2054 6865 7365  ath:`c`.   These
-00000e10: 2073 636f 7265 7320 6f6e 6c79 206c 6561   scores only lea
-00000e20: 6420 746f 2064 6966 6665 7265 6e74 2072  d to different r
-00000e30: 6573 756c 7473 206f 6e20 6e6f 6e2d 6c69  esults on non-li
-00000e40: 6e65 6172 2070 726f 6669 6c65 732e 200a  near profiles. .
-00000e50: 0a20 2020 2052 6574 7572 6e73 3a20 0a20  .    Returns: . 
-00000e60: 2020 2020 2020 2041 2064 6963 7469 6f6e         A diction
-00000e70: 6172 7920 6173 736f 6369 6174 696e 6720  ary associating 
-00000e80: 6561 6368 2063 616e 6469 6461 7465 2077  each candidate w
-00000e90: 6974 6820 6974 7320 6d69 6e69 6d61 7820  ith its minimax 
-00000ea0: 7363 6f72 652e 0a0a 2020 2020 2e2e 2073  score...    .. s
-00000eb0: 6565 616c 736f 3a3a 0a0a 2020 2020 2020  eealso::..      
-00000ec0: 2020 3a6d 6574 683a 6070 7265 665f 766f    :meth:`pref_vo
-00000ed0: 7469 6e67 2e6d 6172 6769 6e5f 6261 7365  ting.margin_base
-00000ee0: 645f 6d65 7468 6f64 732e 6d69 6e69 6d61  d_methods.minima
-00000ef0: 7860 0a0a 2020 2020 3a45 7861 6d70 6c65  x`..    :Example
-00000f00: 3a20 0a0a 2020 2020 2e2e 2070 6c6f 743a  : ..    .. plot:
-00000f10: 3a20 206d 6172 6769 6e5f 6772 6170 6873  :  margin_graphs
-00000f20: 5f65 7861 6d70 6c65 732f 6d67 5f65 785f  _examples/mg_ex_
-00000f30: 6d69 6e69 6d61 782e 7079 0a20 2020 2020  minimax.py.     
-00000f40: 2020 203a 636f 6e74 6578 743a 2072 6573     :context: res
-00000f50: 6574 2020 0a20 2020 2020 2020 203a 696e  et  .        :in
-00000f60: 636c 7564 652d 736f 7572 6365 3a20 5472  clude-source: Tr
-00000f70: 7565 0a0a 0a20 2020 202e 2e20 636f 6465  ue...    .. code
-00000f80: 2d62 6c6f 636b 3a3a 200a 0a20 2020 2020  -block:: ..     
-00000f90: 2020 2066 726f 6d20 7072 6566 5f76 6f74     from pref_vot
-00000fa0: 696e 672e 6d61 7267 696e 5f62 6173 6564  ing.margin_based
-00000fb0: 5f6d 6574 686f 6473 2069 6d70 6f72 7420  _methods import 
-00000fc0: 6d69 6e69 6d61 785f 7363 6f72 6573 2c20  minimax_scores, 
-00000fd0: 6d69 6e69 6d61 780a 0a20 2020 2020 2020  minimax..       
-00000fe0: 206d 696e 696d 6178 2e64 6973 706c 6179   minimax.display
-00000ff0: 2870 726f 6629 0a20 2020 2020 2020 2070  (prof).        p
-00001000: 7269 6e74 286d 696e 696d 6178 5f73 636f  rint(minimax_sco
-00001010: 7265 7328 7072 6f66 2929 0a0a 0a20 2020  res(prof))...   
-00001020: 202e 2e20 6578 6563 5f63 6f64 653a 3a20   .. exec_code:: 
-00001030: 0a20 2020 2020 2020 203a 6869 6465 5f63  .        :hide_c
-00001040: 6f64 653a 0a0a 2020 2020 2020 2020 6672  ode:..        fr
-00001050: 6f6d 2070 7265 665f 766f 7469 6e67 2e70  om pref_voting.p
-00001060: 726f 6669 6c65 7320 696d 706f 7274 2050  rofiles import P
-00001070: 726f 6669 6c65 0a20 2020 2020 2020 2066  rofile.        f
-00001080: 726f 6d20 7072 6566 5f76 6f74 696e 672e  rom pref_voting.
-00001090: 6d61 7267 696e 5f62 6173 6564 5f6d 6574  margin_based_met
-000010a0: 686f 6473 2069 6d70 6f72 7420 6d69 6e69  hods import mini
-000010b0: 6d61 782c 206d 696e 696d 6178 5f73 636f  max, minimax_sco
-000010c0: 7265 730a 2020 2020 2020 2020 0a20 2020  res.        .   
-000010d0: 2020 2020 2070 726f 6620 3d20 5072 6f66       prof = Prof
-000010e0: 696c 6528 5b5b 332c 2030 2c20 312c 2032  ile([[3, 0, 1, 2
-000010f0: 5d2c 205b 312c 2033 2c20 322c 2030 5d2c  ], [1, 3, 2, 0],
-00001100: 205b 312c 2033 2c20 302c 2032 5d2c 205b   [1, 3, 0, 2], [
-00001110: 312c 2032 2c20 302c 2033 5d2c 205b 332c  1, 2, 0, 3], [3,
-00001120: 2032 2c20 302c 2031 5d2c 205b 302c 2032   2, 0, 1], [0, 2
-00001130: 2c20 312c 2033 5d5d 2c20 5b31 2c20 312c  , 1, 3]], [1, 1,
-00001140: 2031 2c20 312c 2032 2c20 315d 290a 0a20   1, 1, 2, 1]).. 
-00001150: 2020 2020 2020 206d 696e 696d 6178 2e64         minimax.d
-00001160: 6973 706c 6179 2870 726f 6629 0a20 2020  isplay(prof).   
-00001170: 2020 2020 2070 7269 6e74 286d 696e 696d       print(minim
-00001180: 6178 5f73 636f 7265 7328 7072 6f66 2929  ax_scores(prof))
-00001190: 0a0a 2020 2020 2222 220a 2020 2020 0a20  ..    """.    . 
-000011a0: 2020 2063 616e 6469 6461 7465 7320 3d20     candidates = 
-000011b0: 6564 6174 612e 6361 6e64 6964 6174 6573  edata.candidates
-000011c0: 2069 6620 6375 7272 5f63 616e 6473 2069   if curr_cands i
-000011d0: 7320 4e6f 6e65 2065 6c73 6520 6375 7272  s None else curr
-000011e0: 5f63 616e 6473 0a0a 2020 2020 6966 206c  _cands..    if l
-000011f0: 656e 2863 616e 6469 6461 7465 7329 203d  en(candidates) =
-00001200: 3d20 313a 0a20 2020 2020 2020 2072 6574  = 1:.        ret
-00001210: 7572 6e20 7b63 3a20 3020 666f 7220 6320  urn {c: 0 for c 
-00001220: 696e 2063 616e 6469 6461 7465 737d 0a20  in candidates}. 
-00001230: 2020 200a 2020 2020 2320 7468 6572 6520     .    # there 
-00001240: 6172 6520 6469 6666 6572 656e 7420 7363  are different sc
-00001250: 6f72 696e 6720 6675 6e63 7469 6f6e 7320  oring functions 
-00001260: 7468 6174 2063 616e 2062 6520 7573 6564  that can be used
-00001270: 2074 6f20 6d65 6173 7572 6520 7468 6520   to measure the 
-00001280: 776f 7273 6520 6c6f 7373 2066 6f72 2065  worse loss for e
-00001290: 6163 6820 0a20 2020 2023 2063 616e 6469  ach .    # candi
-000012a0: 6461 7465 2e20 5468 6573 6520 616c 6c20  date. These all 
-000012b0: 7072 6f64 7563 6520 7468 6520 7361 6d65  produce the same
-000012c0: 2073 6574 206f 6620 7769 6e6e 6572 7320   set of winners 
-000012d0: 7768 656e 2076 6f74 6572 7320 7375 626d  when voters subm
-000012e0: 6974 206c 696e 6561 7220 6f72 6465 7273  it linear orders
-000012f0: 2e20 0a20 2020 2073 636f 7265 5f66 756e  . .    score_fun
-00001300: 6374 696f 6e73 203d 207b 0a20 2020 2020  ctions = {.     
-00001310: 2020 2022 7769 6e6e 696e 6722 3a20 6c61     "winning": la
-00001320: 6d62 6461 2063 732c 2063 3a20 6d61 7828  mbda cs, c: max(
-00001330: 5b65 6461 7461 2e73 7570 706f 7274 285f  [edata.support(_
-00001340: 632c 6329 2066 6f72 205f 6320 696e 2063  c,c) for _c in c
-00001350: 735d 2920 6966 206c 656e 2863 7329 203e  s]) if len(cs) >
-00001360: 2030 2065 6c73 6520 302c 0a20 2020 2020   0 else 0,.     
-00001370: 2020 2022 6d61 7267 696e 7322 3a20 6c61     "margins": la
-00001380: 6d62 6461 2063 732c 2063 3a20 6d61 7828  mbda cs, c: max(
-00001390: 5b65 6461 7461 2e6d 6172 6769 6e28 5f63  [edata.margin(_c
-000013a0: 2c63 2920 666f 7220 5f63 2069 6e20 6373  ,c) for _c in cs
-000013b0: 5d29 2069 6620 6c65 6e28 6373 2920 3e20  ]) if len(cs) > 
-000013c0: 3020 656c 7365 2030 2c0a 2020 2020 2020  0 else 0,.      
-000013d0: 2020 2270 6169 7277 6973 655f 6f70 706f    "pairwise_oppo
-000013e0: 7369 7469 6f6e 223a 206c 616d 6264 6120  sition": lambda 
-000013f0: 6373 2c20 633a 206d 6178 285b 6564 6174  cs, c: max([edat
-00001400: 612e 7375 7070 6f72 7428 5f63 2c63 2920  a.support(_c,c) 
-00001410: 666f 7220 5f63 2069 6e20 6373 5d29 0a20  for _c in cs]). 
-00001420: 2020 207d 200a 2020 2020 0a20 2020 2063     } .    .    c
-00001430: 616e 6473 203d 207b 0a20 2020 2020 2020  ands = {.       
-00001440: 2022 7769 6e6e 696e 6722 3a20 6c61 6d62   "winning": lamb
-00001450: 6461 2063 3a20 6564 6174 612e 646f 6d69  da c: edata.domi
-00001460: 6e61 746f 7273 2863 2c20 6375 7272 5f63  nators(c, curr_c
-00001470: 616e 6473 203d 2063 7572 725f 6361 6e64  ands = curr_cand
-00001480: 7329 2c0a 2020 2020 2020 2020 226d 6172  s),.        "mar
-00001490: 6769 6e73 223a 206c 616d 6264 6120 633a  gins": lambda c:
-000014a0: 2065 6461 7461 2e64 6f6d 696e 6174 6f72   edata.dominator
-000014b0: 7328 632c 2063 7572 725f 6361 6e64 7320  s(c, curr_cands 
-000014c0: 3d20 6375 7272 5f63 616e 6473 292c 0a20  = curr_cands),. 
-000014d0: 2020 2020 2020 2022 7061 6972 7769 7365         "pairwise
-000014e0: 5f6f 7070 6f73 6974 696f 6e22 3a20 6c61  _opposition": la
-000014f0: 6d62 6461 2063 3a20 5b5f 6320 666f 7220  mbda c: [_c for 
-00001500: 5f63 2069 6e20 6361 6e64 6964 6174 6573  _c in candidates
-00001510: 2069 6620 5f63 2021 3d20 635d 0a20 2020   if _c != c].   
-00001520: 207d 200a 0a20 2020 2072 6574 7572 6e20   } ..    return 
-00001530: 7b63 3a20 2d31 202a 2073 636f 7265 5f66  {c: -1 * score_f
-00001540: 756e 6374 696f 6e73 5b73 636f 7265 5f6d  unctions[score_m
-00001550: 6574 686f 645d 2863 616e 6473 5b73 636f  ethod](cands[sco
-00001560: 7265 5f6d 6574 686f 645d 2863 292c 2063  re_method](c), c
-00001570: 2920 666f 7220 6320 696e 2063 616e 6469  ) for c in candi
-00001580: 6461 7465 737d 0a0a 0a64 6566 206d 6178  dates}...def max
-00001590: 696d 616c 5f65 6c65 6d65 6e74 7328 6729  imal_elements(g)
-000015a0: 3a20 0a20 2020 2022 2222 7265 7475 726e  : .    """return
-000015b0: 2074 6865 206e 6f64 6573 2069 6e20 6720   the nodes in g 
-000015c0: 7769 7468 206e 6f20 696e 636f 6d69 6e67  with no incoming
-000015d0: 2061 7272 6f77 732e 2222 220a 2020 2020   arrows.""".    
-000015e0: 7265 7475 726e 205b 6e20 666f 7220 6e20  return [n for n 
-000015f0: 696e 2067 2e6e 6f64 6573 2069 6620 672e  in g.nodes if g.
-00001600: 696e 5f64 6567 7265 6528 6e29 203d 3d20  in_degree(n) == 
-00001610: 305d 0a0a 0a64 6566 205f 6265 6174 5f70  0]...def _beat_p
-00001620: 6174 685f 6261 7369 6328 6564 6174 612c  ath_basic(edata,
-00001630: 200a 2020 2020 2020 2020 2020 2020 2020   .              
-00001640: 2020 2020 2020 2063 7572 725f 6361 6e64         curr_cand
-00001650: 7320 3d20 4e6f 6e65 2c20 0a20 2020 2020  s = None, .     
-00001660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001670: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
-00001680: 6e20 3d20 4e6f 6e65 293a 200a 2020 2020  n = None): .    
-00001690: 2222 2241 6e20 696d 706c 656d 656e 7461  """An implementa
-000016a0: 7469 6f6e 206f 6620 7468 6520 4265 6174  tion of the Beat
-000016b0: 2050 6174 6820 6d65 7468 6f64 2074 6861   Path method tha
-000016c0: 7420 7573 6573 2061 2062 6173 6963 2061  t uses a basic a
-000016d0: 6c67 6f72 6974 686d 2e20 2054 6869 7320  lgorithm.  This 
-000016e0: 6973 206e 6f74 2065 6666 6963 6965 6e74  is not efficient
-000016f0: 2066 6f72 206c 6172 6765 2067 7261 7068   for large graph
-00001700: 732e 0a20 2020 200a 2020 2020 4172 6773  s..    .    Args
-00001710: 3a0a 2020 2020 2020 2020 6564 6174 6120  :.        edata 
-00001720: 2850 726f 6669 6c65 2c20 5072 6f66 696c  (Profile, Profil
-00001730: 6557 6974 6854 6965 732c 204d 6172 6769  eWithTies, Margi
-00001740: 6e47 7261 7068 293a 2041 6e79 2065 6c65  nGraph): Any ele
-00001750: 6374 696f 6e20 6461 7461 2074 6861 7420  ction data that 
-00001760: 6861 7320 6120 606d 6172 6769 6e60 206d  has a `margin` m
-00001770: 6574 686f 642e 200a 2020 2020 2020 2020  ethod. .        
-00001780: 6375 7272 5f63 616e 6473 2028 4c69 7374  curr_cands (List
-00001790: 5b69 6e74 5d2c 206f 7074 696f 6e61 6c29  [int], optional)
-000017a0: 3a20 4966 2073 6574 2c20 7468 656e 2066  : If set, then f
-000017b0: 696e 6420 7468 6520 7769 6e6e 6572 7320  ind the winners 
-000017c0: 666f 7220 7468 6520 7072 6f66 696c 6520  for the profile 
-000017d0: 7265 7374 7269 6374 6564 2074 6f20 7468  restricted to th
-000017e0: 6520 6361 6e64 6964 6174 6573 2069 6e20  e candidates in 
-000017f0: 6060 6375 7272 5f63 616e 6473 6060 0a20  ``curr_cands``. 
-00001800: 2020 2020 2020 2073 7472 656e 6774 685f         strength_
-00001810: 6675 6e63 7469 6f6e 2028 6675 6e63 7469  function (functi
-00001820: 6f6e 2c20 6f70 7469 6f6e 616c 293a 2054  on, optional): T
-00001830: 6865 2073 7472 656e 6774 6820 6675 6e63  he strength func
-00001840: 7469 6f6e 2074 6f20 6265 2075 7365 6420  tion to be used 
-00001850: 746f 2063 616c 6375 6c61 7465 2074 6865  to calculate the
-00001860: 2073 7472 656e 6774 6820 6f66 2061 2070   strength of a p
-00001870: 6174 682e 2020 2054 6865 2064 6566 6175  ath.   The defau
-00001880: 6c74 2069 7320 7468 6520 6d61 7267 696e  lt is the margin
-00001890: 206d 6574 686f 6420 6f66 2060 6065 6461   method of ``eda
-000018a0: 7461 6060 2e20 2020 5468 6973 206f 6e6c  ta``.   This onl
-000018b0: 7920 6d61 7474 6572 7320 7768 656e 2074  y matters when t
-000018c0: 6865 2062 616c 6c6f 7473 2061 7265 206e  he ballots are n
-000018d0: 6f74 206c 696e 6561 7220 6f72 6465 7273  ot linear orders
-000018e0: 2e20 0a0a 2020 2020 5265 7475 726e 733a  . ..    Returns:
-000018f0: 200a 2020 2020 2020 2020 4120 736f 7274   .        A sort
-00001900: 6564 206c 6973 7420 6f66 2063 616e 6469  ed list of candi
-00001910: 6461 7465 732e 200a 0a20 2020 2022 2222  dates. ..    """
-00001920: 0a20 2020 2063 616e 6469 6461 7465 7320  .    candidates 
-00001930: 3d20 6564 6174 612e 6361 6e64 6964 6174  = edata.candidat
-00001940: 6573 2069 6620 6375 7272 5f63 616e 6473  es if curr_cands
-00001950: 2069 7320 4e6f 6e65 2065 6c73 6520 6375   is None else cu
-00001960: 7272 5f63 616e 6473 2020 2020 0a20 2020  rr_cands    .   
-00001970: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
-00001980: 6f6e 203d 2065 6461 7461 2e6d 6172 6769  on = edata.margi
-00001990: 6e20 6966 2073 7472 656e 6774 685f 6675  n if strength_fu
-000019a0: 6e63 7469 6f6e 2069 7320 4e6f 6e65 2065  nction is None e
-000019b0: 6c73 6520 7374 7265 6e67 7468 5f66 756e  lse strength_fun
-000019c0: 6374 696f 6e0a 2020 2020 0a20 2020 206d  ction.    .    m
-000019d0: 6720 3d20 6765 745f 6d67 2865 6461 7461  g = get_mg(edata
-000019e0: 2c20 6375 7272 5f63 616e 6473 203d 2063  , curr_cands = c
-000019f0: 7572 725f 6361 6e64 7329 0a20 2020 200a  urr_cands).    .
-00001a00: 2020 2020 6265 6174 5f70 6174 6873 5f77      beat_paths_w
-00001a10: 6569 6768 7473 203d 207b 633a 207b 6332  eights = {c: {c2
-00001a20: 3a30 2066 6f72 2063 3220 696e 2063 616e  :0 for c2 in can
-00001a30: 6469 6461 7465 7320 6966 2063 3220 213d  didates if c2 !=
-00001a40: 2063 7d20 666f 7220 6320 696e 2063 616e   c} for c in can
-00001a50: 6469 6461 7465 737d 0a20 2020 2066 6f72  didates}.    for
-00001a60: 2063 2069 6e20 6361 6e64 6964 6174 6573   c in candidates
-00001a70: 3a20 0a20 2020 2020 2020 2066 6f72 206f  : .        for o
-00001a80: 7468 6572 5f63 2069 6e20 6265 6174 5f70  ther_c in beat_p
-00001a90: 6174 6873 5f77 6569 6768 7473 5b63 5d2e  aths_weights[c].
-00001aa0: 6b65 7973 2829 3a0a 2020 2020 2020 2020  keys():.        
-00001ab0: 2020 2020 616c 6c5f 7061 7468 7320 3d20      all_paths = 
-00001ac0: 206c 6973 7428 6e78 2e61 6c6c 5f73 696d   list(nx.all_sim
-00001ad0: 706c 655f 7061 7468 7328 6d67 2c20 632c  ple_paths(mg, c,
-00001ae0: 206f 7468 6572 5f63 2929 0a20 2020 2020   other_c)).     
-00001af0: 2020 2020 2020 2069 6620 6c65 6e28 616c         if len(al
-00001b00: 6c5f 7061 7468 7329 203e 2030 3a0a 2020  l_paths) > 0:.  
-00001b10: 2020 2020 2020 2020 2020 2020 2020 6265                be
-00001b20: 6174 5f70 6174 6873 5f77 6569 6768 7473  at_paths_weights
-00001b30: 5b63 5d5b 6f74 6865 725f 635d 203d 206d  [c][other_c] = m
-00001b40: 6178 285b 6d69 6e28 5b73 7472 656e 6774  ax([min([strengt
-00001b50: 685f 6675 6e63 7469 6f6e 2870 5b69 5d2c  h_function(p[i],
-00001b60: 2070 5b69 2b31 5d29 200a 2020 2020 2020   p[i+1]) .      
-00001b70: 2020 2020 2020 2020 2020 666f 7220 6920            for i 
-00001b80: 696e 2072 616e 6765 2830 2c6c 656e 2870  in range(0,len(p
-00001b90: 292d 3129 5d29 200a 2020 2020 2020 2020  )-1)]) .        
-00001ba0: 2020 2020 2020 2020 666f 7220 7020 696e          for p in
-00001bb0: 2061 6c6c 5f70 6174 6873 5d29 0a20 2020   all_paths]).   
-00001bc0: 200a 2020 2020 7769 6e6e 6572 7320 3d20   .    winners = 
-00001bd0: 6c69 7374 2829 0a20 2020 2066 6f72 2063  list().    for c
-00001be0: 2069 6e20 6361 6e64 6964 6174 6573 3a20   in candidates: 
-00001bf0: 0a20 2020 2020 2020 2069 6620 616c 6c28  .        if all(
-00001c00: 5b62 6561 745f 7061 7468 735f 7765 6967  [beat_paths_weig
-00001c10: 6874 735b 635d 5b63 325d 203e 3d20 6265  hts[c][c2] >= be
-00001c20: 6174 5f70 6174 6873 5f77 6569 6768 7473  at_paths_weights
-00001c30: 5b63 325d 5b63 5d20 666f 7220 6332 2069  [c2][c] for c2 i
-00001c40: 6e20 6361 6e64 6964 6174 6573 2020 6966  n candidates  if
-00001c50: 2063 3220 213d 2063 5d29 3a0a 2020 2020   c2 != c]):.    
-00001c60: 2020 2020 2020 2020 7769 6e6e 6572 732e          winners.
-00001c70: 6170 7065 6e64 2863 290a 2020 2020 7265  append(c).    re
-00001c80: 7475 726e 2073 6f72 7465 6428 6c69 7374  turn sorted(list
-00001c90: 2877 696e 6e65 7273 2929 0a0a 6465 6620  (winners))..def 
-00001ca0: 5f62 6561 745f 7061 7468 5f66 6c6f 7964  _beat_path_floyd
-00001cb0: 5f77 6172 7368 616c 6c28 0a20 2020 2020  _warshall(.     
-00001cc0: 2020 2065 6461 7461 2c20 0a20 2020 2020     edata, .     
-00001cd0: 2020 2063 7572 725f 6361 6e64 7320 3d20     curr_cands = 
-00001ce0: 4e6f 6e65 2c20 0a20 2020 2020 2020 2073  None, .        s
-00001cf0: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
-00001d00: 203d 204e 6f6e 6529 3a20 2020 0a20 2020   = None):   .   
-00001d10: 2022 2222 416e 2069 6d70 6c65 6d65 6e74   """An implement
-00001d20: 6174 696f 6e20 6f66 2042 6561 7420 5061  ation of Beat Pa
-00001d30: 7468 2075 7369 6e67 2061 2076 6172 6961  th using a varia
-00001d40: 7469 6f6e 206f 6620 7468 6520 466c 6f79  tion of the Floy
-00001d50: 642d 5761 7273 6861 6c6c 2041 6c67 6f72  d-Warshall Algor
-00001d60: 6974 686d 0a20 2020 2053 6565 2068 7474  ithm.    See htt
-00001d70: 7073 3a2f 2f65 6e2e 7769 6b69 7065 6469  ps://en.wikipedi
-00001d80: 612e 6f72 672f 7769 6b69 2f53 6368 756c  a.org/wiki/Schul
-00001d90: 7a65 5f6d 6574 686f 6423 496d 706c 656d  ze_method#Implem
-00001da0: 656e 7461 7469 6f6e 290a 200a 2020 2020  entation). .    
-00001db0: 4172 6773 3a0a 2020 2020 2020 2020 6564  Args:.        ed
-00001dc0: 6174 6120 2850 726f 6669 6c65 2c20 5072  ata (Profile, Pr
-00001dd0: 6f66 696c 6557 6974 6854 6965 732c 204d  ofileWithTies, M
-00001de0: 6172 6769 6e47 7261 7068 293a 2041 6e79  arginGraph): Any
-00001df0: 2065 6c65 6374 696f 6e20 6461 7461 2074   election data t
-00001e00: 6861 7420 6861 7320 6120 606d 6172 6769  hat has a `margi
-00001e10: 6e60 206d 6574 686f 642e 200a 2020 2020  n` method. .    
-00001e20: 2020 2020 6375 7272 5f63 616e 6473 2028      curr_cands (
-00001e30: 4c69 7374 5b69 6e74 5d2c 206f 7074 696f  List[int], optio
-00001e40: 6e61 6c29 3a20 4966 2073 6574 2c20 7468  nal): If set, th
-00001e50: 656e 2066 696e 6420 7468 6520 7769 6e6e  en find the winn
-00001e60: 6572 7320 666f 7220 7468 6520 7072 6f66  ers for the prof
-00001e70: 696c 6520 7265 7374 7269 6374 6564 2074  ile restricted t
-00001e80: 6f20 7468 6520 6361 6e64 6964 6174 6573  o the candidates
-00001e90: 2069 6e20 6060 6375 7272 5f63 616e 6473   in ``curr_cands
-00001ea0: 6060 0a20 2020 2020 2020 2073 7472 656e  ``.        stren
-00001eb0: 6774 685f 6675 6e63 7469 6f6e 2028 6675  gth_function (fu
-00001ec0: 6e63 7469 6f6e 2c20 6f70 7469 6f6e 616c  nction, optional
-00001ed0: 293a 2054 6865 2073 7472 656e 6774 6820  ): The strength 
-00001ee0: 6675 6e63 7469 6f6e 2074 6f20 6265 2075  function to be u
-00001ef0: 7365 6420 746f 2063 616c 6375 6c61 7465  sed to calculate
-00001f00: 2074 6865 2073 7472 656e 6774 6820 6f66   the strength of
-00001f10: 2061 2070 6174 682e 2020 2054 6865 2064   a path.   The d
-00001f20: 6566 6175 6c74 2069 7320 7468 6520 6d61  efault is the ma
-00001f30: 7267 696e 206d 6574 686f 6420 6f66 2060  rgin method of `
-00001f40: 6065 6461 7461 6060 2e20 2020 5468 6973  `edata``.   This
-00001f50: 206f 6e6c 7920 6d61 7474 6572 7320 7768   only matters wh
-00001f60: 656e 2074 6865 2062 616c 6c6f 7473 2061  en the ballots a
-00001f70: 7265 206e 6f74 206c 696e 6561 7220 6f72  re not linear or
-00001f80: 6465 7273 2e20 0a0a 2020 2020 5265 7475  ders. ..    Retu
-00001f90: 726e 733a 200a 2020 2020 2020 2020 4120  rns: .        A 
-00001fa0: 736f 7274 6564 206c 6973 7420 6f66 2063  sorted list of c
-00001fb0: 616e 6469 6461 7465 732e 200a 0a20 2020  andidates. ..   
-00001fc0: 2022 2222 0a0a 2020 2020 6361 6e64 6964   """..    candid
-00001fd0: 6174 6573 203d 2065 6461 7461 2e63 616e  ates = edata.can
-00001fe0: 6469 6461 7465 7320 6966 2063 7572 725f  didates if curr_
-00001ff0: 6361 6e64 7320 6973 204e 6f6e 6520 656c  cands is None el
-00002000: 7365 2063 7572 725f 6361 6e64 7320 2020  se curr_cands   
-00002010: 200a 2020 2020 7374 7265 6e67 7468 5f66   .    strength_f
-00002020: 756e 6374 696f 6e20 3d20 6564 6174 612e  unction = edata.
-00002030: 6d61 7267 696e 2069 6620 7374 7265 6e67  margin if streng
-00002040: 7468 5f66 756e 6374 696f 6e20 6973 204e  th_function is N
-00002050: 6f6e 6520 656c 7365 2073 7472 656e 6774  one else strengt
-00002060: 685f 6675 6e63 7469 6f6e 0a20 2020 2020  h_function.     
-00002070: 2020 200a 2020 2020 735f 6d61 7472 6978     .    s_matrix
-00002080: 203d 205b 5b2d 6e70 2e69 6e66 2066 6f72   = [[-np.inf for
-00002090: 205f 2069 6e20 6361 6e64 6964 6174 6573   _ in candidates
-000020a0: 5d20 666f 7220 5f20 696e 2063 616e 6469  ] for _ in candi
-000020b0: 6461 7465 735d 0a20 2020 2066 6f72 2063  dates].    for c
-000020c0: 315f 6964 782c 2063 3120 696e 2065 6e75  1_idx, c1 in enu
-000020d0: 6d65 7261 7465 2863 616e 6469 6461 7465  merate(candidate
-000020e0: 7329 3a0a 2020 2020 2020 2020 666f 7220  s):.        for 
-000020f0: 6332 5f69 6478 2c20 6332 2069 6e20 656e  c2_idx, c2 in en
-00002100: 756d 6572 6174 6528 6361 6e64 6964 6174  umerate(candidat
-00002110: 6573 293a 0a20 2020 2020 2020 2020 2020  es):.           
-00002120: 2069 6620 2865 6461 7461 2e6d 616a 6f72   if (edata.major
-00002130: 6974 795f 7072 6566 6572 7328 6331 2c20  ity_prefers(c1, 
-00002140: 6332 2920 6f72 2063 3120 3d3d 2063 3229  c2) or c1 == c2)
-00002150: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00002160: 2020 735f 6d61 7472 6978 5b63 315f 6964    s_matrix[c1_id
-00002170: 785d 5b63 325f 6964 785d 203d 2073 7472  x][c2_idx] = str
-00002180: 656e 6774 685f 6675 6e63 7469 6f6e 2863  ength_function(c
-00002190: 312c 2063 3229 200a 2020 2020 7374 7265  1, c2) .    stre
-000021a0: 6e67 7468 203d 206c 6973 7428 6d61 7028  ngth = list(map(
-000021b0: 6c61 6d62 6461 2069 203a 206c 6973 7428  lambda i : list(
-000021c0: 6d61 7028 6c61 6d62 6461 206a 203a 206a  map(lambda j : j
-000021d0: 202c 2069 2929 202c 2073 5f6d 6174 7269   , i)) , s_matri
-000021e0: 7829 290a 2020 2020 666f 7220 695f 6964  x)).    for i_id
-000021f0: 782c 2069 2069 6e20 656e 756d 6572 6174  x, i in enumerat
-00002200: 6528 6361 6e64 6964 6174 6573 293a 2020  e(candidates):  
-00002210: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00002220: 666f 7220 6a5f 6964 782c 206a 2069 6e20  for j_idx, j in 
-00002230: 656e 756d 6572 6174 6528 6361 6e64 6964  enumerate(candid
-00002240: 6174 6573 293a 200a 2020 2020 2020 2020  ates): .        
-00002250: 2020 2020 6966 2069 213d 206a 3a0a 2020      if i!= j:.  
-00002260: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-00002270: 7220 6b5f 6964 782c 206b 2069 6e20 656e  r k_idx, k in en
-00002280: 756d 6572 6174 6528 6361 6e64 6964 6174  umerate(candidat
-00002290: 6573 293a 200a 2020 2020 2020 2020 2020  es): .          
-000022a0: 2020 2020 2020 2020 2020 6966 2069 213d            if i!=
-000022b0: 206b 2061 6e64 206a 2021 3d20 6b3a 0a20   k and j != k:. 
-000022c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000022d0: 2020 2020 2020 2073 7472 656e 6774 685b         strength[
-000022e0: 6a5f 6964 785d 5b6b 5f69 6478 5d20 3d20  j_idx][k_idx] = 
-000022f0: 6d61 7828 7374 7265 6e67 7468 5b6a 5f69  max(strength[j_i
-00002300: 6478 5d5b 6b5f 6964 785d 2c20 6d69 6e28  dx][k_idx], min(
-00002310: 7374 7265 6e67 7468 5b6a 5f69 6478 5d5b  strength[j_idx][
-00002320: 695f 6964 785d 2c73 7472 656e 6774 685b  i_idx],strength[
-00002330: 695f 6964 785d 5b6b 5f69 6478 5d29 290a  i_idx][k_idx])).
-00002340: 2020 2020 7769 6e6e 6572 7320 3d20 7b69      winners = {i
-00002350: 3a54 7275 6520 666f 7220 6920 696e 2063  :True for i in c
-00002360: 616e 6469 6461 7465 737d 0a20 2020 2066  andidates}.    f
-00002370: 6f72 2069 5f69 6478 2c20 6920 696e 2065  or i_idx, i in e
-00002380: 6e75 6d65 7261 7465 2863 616e 6469 6461  numerate(candida
-00002390: 7465 7329 3a20 0a20 2020 2020 2020 2066  tes): .        f
-000023a0: 6f72 206a 5f69 6478 2c20 6a20 696e 2065  or j_idx, j in e
-000023b0: 6e75 6d65 7261 7465 2863 616e 6469 6461  numerate(candida
-000023c0: 7465 7329 3a0a 2020 2020 2020 2020 2020  tes):.          
-000023d0: 2020 6966 2069 213d 6a3a 0a20 2020 2020    if i!=j:.     
-000023e0: 2020 2020 2020 2020 2020 2069 6620 7374             if st
-000023f0: 7265 6e67 7468 5b6a 5f69 6478 5d5b 695f  rength[j_idx][i_
-00002400: 6964 785d 203e 2073 7472 656e 6774 685b  idx] > strength[
-00002410: 695f 6964 785d 5b6a 5f69 6478 5d3a 0a20  i_idx][j_idx]:. 
-00002420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002430: 2020 2077 696e 6e65 7273 5b69 5d20 3d20     winners[i] = 
-00002440: 4661 6c73 650a 2020 2020 7265 7475 726e  False.    return
-00002450: 2073 6f72 7465 6428 5b63 2066 6f72 2063   sorted([c for c
-00002460: 2069 6e20 6361 6e64 6964 6174 6573 2069   in candidates i
-00002470: 6620 7769 6e6e 6572 735b 635d 5d29 0a0a  f winners[c]])..
-00002480: 6465 6620 5f73 6368 7761 7274 7a5f 7365  def _schwartz_se
-00002490: 7175 656e 7469 616c 5f64 726f 7070 696e  quential_droppin
-000024a0: 6728 6564 6174 612c 2063 7572 725f 6361  g(edata, curr_ca
-000024b0: 6e64 7320 3d20 4e6f 6e65 2c20 7374 7265  nds = None, stre
-000024c0: 6e67 7468 5f66 756e 6374 696f 6e20 3d20  ngth_function = 
-000024d0: 4e6f 6e65 293a 0a0a 2020 2020 2222 2254  None):..    """T
-000024e0: 6865 2053 6368 7761 7274 7a20 5365 7175  he Schwartz Sequ
-000024f0: 656e 7469 616c 2044 726f 7070 696e 6720  ential Dropping 
-00002500: 616c 676f 7269 7468 6d2e 2053 6565 2068  algorithm. See h
-00002510: 7474 7073 3a2f 2f65 6e2e 7769 6b69 7065  ttps://en.wikipe
-00002520: 6469 612e 6f72 672f 7769 6b69 2f53 6368  dia.org/wiki/Sch
-00002530: 756c 7a65 5f6d 6574 686f 6423 5469 6573  ulze_method#Ties
-00002540: 5f61 6e64 5f61 6c74 6572 6e61 7469 7665  _and_alternative
-00002550: 5f69 6d70 6c65 6d65 6e74 6174 696f 6e73  _implementations
-00002560: 2e0a 2020 2020 0a20 2020 2041 7267 733a  ..    .    Args:
-00002570: 0a20 2020 2020 2020 2065 6461 7461 2028  .        edata (
-00002580: 5072 6f66 696c 652c 2050 726f 6669 6c65  Profile, Profile
-00002590: 5769 7468 5469 6573 2c20 4d61 7267 696e  WithTies, Margin
-000025a0: 4772 6170 6829 3a20 416e 7920 656c 6563  Graph): Any elec
-000025b0: 7469 6f6e 2064 6174 6120 7468 6174 2068  tion data that h
-000025c0: 6173 2061 2060 6d61 7267 696e 6020 6d65  as a `margin` me
-000025d0: 7468 6f64 2e20 0a20 2020 2020 2020 2063  thod. .        c
-000025e0: 7572 725f 6361 6e64 7320 284c 6973 745b  urr_cands (List[
-000025f0: 696e 745d 2c20 6f70 7469 6f6e 616c 293a  int], optional):
-00002600: 2049 6620 7365 742c 2074 6865 6e20 6669   If set, then fi
-00002610: 6e64 2074 6865 2077 696e 6e65 7273 2066  nd the winners f
-00002620: 6f72 2074 6865 2070 726f 6669 6c65 2072  or the profile r
-00002630: 6573 7472 6963 7465 6420 746f 2074 6865  estricted to the
-00002640: 2063 616e 6469 6461 7465 7320 696e 2060   candidates in `
-00002650: 6063 7572 725f 6361 6e64 7360 600a 2020  `curr_cands``.  
-00002660: 2020 2020 2020 7374 7265 6e67 7468 5f66        strength_f
-00002670: 756e 6374 696f 6e20 2866 756e 6374 696f  unction (functio
-00002680: 6e2c 206f 7074 696f 6e61 6c29 3a20 5468  n, optional): Th
-00002690: 6520 7374 7265 6e67 7468 2066 756e 6374  e strength funct
-000026a0: 696f 6e20 746f 2062 6520 7573 6564 2074  ion to be used t
-000026b0: 6f20 6361 6c63 756c 6174 6520 7468 6520  o calculate the 
-000026c0: 7374 7265 6e67 7468 206f 6620 6120 7061  strength of a pa
-000026d0: 7468 2e20 2020 5468 6520 6465 6661 756c  th.   The defaul
-000026e0: 7420 6973 2074 6865 206d 6172 6769 6e20  t is the margin 
-000026f0: 6d65 7468 6f64 206f 6620 6060 6564 6174  method of ``edat
-00002700: 6160 602e 2020 2054 6869 7320 6f6e 6c79  a``.   This only
-00002710: 206d 6174 7465 7273 2077 6865 6e20 7468   matters when th
-00002720: 6520 6261 6c6c 6f74 7320 6172 6520 6e6f  e ballots are no
-00002730: 7420 6c69 6e65 6172 206f 7264 6572 732e  t linear orders.
-00002740: 200a 0a20 2020 2052 6574 7572 6e73 3a20   ..    Returns: 
-00002750: 0a20 2020 2020 2020 2041 2073 6f72 7465  .        A sorte
-00002760: 6420 6c69 7374 206f 6620 6361 6e64 6964  d list of candid
-00002770: 6174 6573 2e20 0a20 2020 2022 2222 0a20  ates. .    """. 
-00002780: 2020 2066 726f 6d20 7072 6566 5f76 6f74     from pref_vot
-00002790: 696e 672e 6331 5f6d 6574 686f 6473 2069  ing.c1_methods i
-000027a0: 6d70 6f72 7420 676f 6368 610a 0a20 2020  mport gocha..   
-000027b0: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
-000027c0: 6f6e 203d 2065 6461 7461 2e6d 6172 6769  on = edata.margi
-000027d0: 6e20 6966 2073 7472 656e 6774 685f 6675  n if strength_fu
-000027e0: 6e63 7469 6f6e 2069 7320 4e6f 6e65 2065  nction is None e
-000027f0: 6c73 6520 7374 7265 6e67 7468 5f66 756e  lse strength_fun
-00002800: 6374 696f 6e0a 0a20 2020 206d 6720 3d20  ction..    mg = 
-00002810: 6564 6174 6120 6966 2069 7369 6e73 7461  edata if isinsta
-00002820: 6e63 6528 6564 6174 612c 204d 6172 6769  nce(edata, Margi
-00002830: 6e47 7261 7068 2920 656c 7365 2065 6461  nGraph) else eda
-00002840: 7461 2e6d 6172 6769 6e5f 6772 6170 6828  ta.margin_graph(
-00002850: 290a 2020 2020 7363 6877 6172 747a 203d  ).    schwartz =
-00002860: 2067 6f63 6861 286d 672c 2063 7572 725f   gocha(mg, curr_
-00002870: 6361 6e64 7320 3d20 6375 7272 5f63 616e  cands = curr_can
-00002880: 6473 290a 0a20 2020 2069 6620 6c65 6e28  ds)..    if len(
-00002890: 7363 6877 6172 747a 2920 3d3d 2031 3a0a  schwartz) == 1:.
-000028a0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-000028b0: 6368 7761 7274 7a0a 2020 2020 0a20 2020  chwartz.    .   
-000028c0: 2070 6f73 5f73 6368 7761 7274 7a5f 7374   pos_schwartz_st
-000028d0: 7265 6e67 7468 7320 3d20 5b73 7472 656e  rengths = [stren
-000028e0: 6774 685f 6675 6e63 7469 6f6e 2863 2c64  gth_function(c,d
-000028f0: 2920 666f 7220 6320 696e 2073 6368 7761  ) for c in schwa
-00002900: 7274 7a20 666f 7220 6420 696e 2073 6368  rtz for d in sch
-00002910: 7761 7274 7a20 6966 2073 7472 656e 6774  wartz if strengt
-00002920: 685f 6675 6e63 7469 6f6e 2863 2c64 2920  h_function(c,d) 
-00002930: 3e20 305d 0a0a 2020 2020 6966 206c 656e  > 0]..    if len
-00002940: 2870 6f73 5f73 6368 7761 7274 7a5f 7374  (pos_schwartz_st
-00002950: 7265 6e67 7468 7329 203d 3d20 303a 0a20  rengths) == 0:. 
-00002960: 2020 2020 2020 2072 6574 7572 6e20 736f         return so
-00002970: 7274 6564 2873 6368 7761 7274 7a29 0a0a  rted(schwartz)..
-00002980: 2020 2020 6d61 785f 7363 6877 6172 747a      max_schwartz
-00002990: 5f73 7472 656e 6774 6820 3d20 6d61 7828  _strength = max(
-000029a0: 706f 735f 7363 6877 6172 747a 5f73 7472  pos_schwartz_str
-000029b0: 656e 6774 6873 290a 2020 2020 6d69 6e5f  engths).    min_
-000029c0: 7363 6877 6172 747a 5f73 7472 656e 6774  schwartz_strengt
-000029d0: 6820 3d20 6d69 6e28 706f 735f 7363 6877  h = min(pos_schw
-000029e0: 6172 747a 5f73 7472 656e 6774 6873 290a  artz_strengths).
-000029f0: 0a20 2020 2069 6620 6d61 785f 7363 6877  .    if max_schw
-00002a00: 6172 747a 5f73 7472 656e 6774 6820 3d3d  artz_strength ==
-00002a10: 206d 696e 5f73 6368 7761 7274 7a5f 7374   min_schwartz_st
-00002a20: 7265 6e67 7468 3a0a 2020 2020 2020 2020  rength:.        
-00002a30: 7265 7475 726e 2073 6f72 7465 6428 7363  return sorted(sc
-00002a40: 6877 6172 747a 290a 2020 2020 0a20 2020  hwartz).    .   
-00002a50: 2065 6c73 653a 0a20 2020 2020 2020 206e   else:.        n
-00002a60: 6577 5f6d 6720 3d20 4d61 7267 696e 4772  ew_mg = MarginGr
-00002a70: 6170 6828 7363 6877 6172 747a 2c5b 2863  aph(schwartz,[(c
-00002a80: 2c64 2c20 7374 7265 6e67 7468 5f66 756e  ,d, strength_fun
-00002a90: 6374 696f 6e28 632c 6429 2920 666f 7220  ction(c,d)) for 
-00002aa0: 6320 696e 2073 6368 7761 7274 7a20 666f  c in schwartz fo
-00002ab0: 7220 6420 696e 2073 6368 7761 7274 7a20  r d in schwartz 
-00002ac0: 6966 2073 7472 656e 6774 685f 6675 6e63  if strength_func
-00002ad0: 7469 6f6e 2863 2c64 2920 3e20 6d69 6e5f  tion(c,d) > min_
-00002ae0: 7363 6877 6172 747a 5f73 7472 656e 6774  schwartz_strengt
-00002af0: 685d 290a 2020 2020 2020 2020 7265 7475  h]).        retu
-00002b00: 726e 205f 7363 6877 6172 747a 5f73 6571  rn _schwartz_seq
-00002b10: 7565 6e74 6961 6c5f 6472 6f70 7069 6e67  uential_dropping
-00002b20: 286e 6577 5f6d 672c 2073 6368 7761 7274  (new_mg, schwart
-00002b30: 7a29 0a0a 6270 5f70 726f 7065 7274 6965  z)..bp_propertie
-00002b40: 7320 3d20 566f 7469 6e67 4d65 7468 6f64  s = VotingMethod
-00002b50: 5072 6f70 6572 7469 6573 280a 2020 2020  Properties(.    
-00002b60: 636f 6e64 6f72 6365 745f 7769 6e6e 6572  condorcet_winner
-00002b70: 3d54 7275 652c 200a 2020 2020 636f 6e64  =True, .    cond
-00002b80: 6f72 6365 745f 6c6f 7365 723d 5472 7565  orcet_loser=True
-00002b90: 2c0a 2020 2020 7061 7265 746f 5f64 6f6d  ,.    pareto_dom
-00002ba0: 696e 616e 6365 3d54 7275 652c 0a20 2020  inance=True,.   
-00002bb0: 2070 6f73 6974 6976 655f 696e 766f 6c76   positive_involv
-00002bc0: 656d 656e 743d 4661 6c73 652c 200a 2020  ement=False, .  
-00002bd0: 2020 290a 0a40 766d 286e 616d 653d 2242    )..@vm(name="B
-00002be0: 6561 7420 5061 7468 222c 0a20 2020 2070  eat Path",.    p
-00002bf0: 726f 7065 7274 6965 733d 6270 5f70 726f  roperties=bp_pro
-00002c00: 7065 7274 6965 732c 0a20 2020 2069 6e70  perties,.    inp
-00002c10: 7574 5f74 7970 6573 3d5b 456c 6563 7469  ut_types=[Electi
-00002c20: 6f6e 5479 7065 732e 5052 4f46 494c 452c  onTypes.PROFILE,
-00002c30: 2045 6c65 6374 696f 6e54 7970 6573 2e50   ElectionTypes.P
-00002c40: 524f 4649 4c45 5f57 4954 485f 5449 4553  ROFILE_WITH_TIES
-00002c50: 2c20 456c 6563 7469 6f6e 5479 7065 732e  , ElectionTypes.
-00002c60: 4d41 5247 494e 5f47 5241 5048 5d29 0a64  MARGIN_GRAPH]).d
-00002c70: 6566 2062 6561 745f 7061 7468 280a 2020  ef beat_path(.  
-00002c80: 2020 6564 6174 612c 200a 2020 2020 6375    edata, .    cu
-00002c90: 7272 5f63 616e 6473 203d 204e 6f6e 652c  rr_cands = None,
-00002ca0: 200a 2020 2020 7374 7265 6e67 7468 5f66   .    strength_f
-00002cb0: 756e 6374 696f 6e20 3d20 4e6f 6e65 2c20  unction = None, 
-00002cc0: 0a20 2020 2061 6c67 6f72 6974 686d 203d  .    algorithm =
-00002cd0: 2027 666c 6f79 645f 7761 7273 6861 6c6c   'floyd_warshall
-00002ce0: 2729 3a20 200a 0a20 2020 2022 2222 466f  '):  ..    """Fo
-00002cf0: 7220 6361 6e64 6964 6174 6573 203a 6d61  r candidates :ma
-00002d00: 7468 3a60 6160 2061 6e64 203a 6d61 7468  th:`a` and :math
-00002d10: 3a60 6260 2c20 6120 2a2a 7061 7468 2a2a  :`b`, a **path**
-00002d20: 2066 726f 6d20 3a6d 6174 683a 6061 6020   from :math:`a` 
-00002d30: 746f 203a 6d61 7468 3a60 6260 2069 7320  to :math:`b` is 
-00002d40: 6120 7365 7175 656e 6365 200a 2020 2020  a sequence .    
-00002d50: 3a6d 6174 683a 6078 5f31 2c20 5c6c 646f  :math:`x_1, \ldo
-00002d60: 7473 2c20 785f 6e60 206f 6620 6469 7374  ts, x_n` of dist
-00002d70: 696e 6374 2063 616e 6469 6461 7465 7320  inct candidates 
-00002d80: 2077 6974 6820 203a 6d61 7468 3a60 785f   with  :math:`x_
-00002d90: 313d 6160 2061 6e64 203a 6d61 7468 3a60  1=a` and :math:`
-00002da0: 785f 6e3d 6260 2073 7563 6820 7468 6174  x_n=b` such that
-00002db0: 200a 2020 2020 666f 7220 3a6d 6174 683a   .    for :math:
-00002dc0: 6031 5c6c 6571 206b 5c6c 6571 206e 2d31  `1\leq k\leq n-1
-00002dd0: 602c 203a 6d61 7468 3a60 785f 6b60 2069  `, :math:`x_k` i
-00002de0: 7320 6d61 6a6f 7269 7479 2070 7265 6665  s majority prefe
-00002df0: 7272 6564 2074 6f20 3a6d 6174 683a 6078  rred to :math:`x
-00002e00: 5f7b 6b2b 317d 602e 2020 5468 6520 2a2a  _{k+1}`.  The **
-00002e10: 7374 7265 6e67 7468 206f 6620 6120 7061  strength of a pa
-00002e20: 7468 2a2a 0a20 2020 2069 7320 7468 6520  th**.    is the 
-00002e30: 6d69 6e69 6d61 6c20 6d61 7267 696e 2061  minimal margin a
-00002e40: 6c6f 6e67 2074 6861 7420 7061 7468 2e20  long that path. 
-00002e50: 2053 6179 2074 6861 7420 3a6d 6174 683a   Say that :math:
-00002e60: 6061 6020 6465 6665 6174 7320 3a6d 6174  `a` defeats :mat
-00002e70: 683a 6062 6020 6163 636f 7264 696e 6720  h:`b` according 
-00002e80: 746f 2042 6561 7420 5061 7468 2069 6620  to Beat Path if 
-00002e90: 7468 6520 7468 6520 7374 7265 6e67 7468  the the strength
-00002ea0: 206f 6620 7468 6520 7374 726f 6e67 6573   of the stronges
-00002eb0: 7420 7061 7468 2066 726f 6d20 3a6d 6174  t path from :mat
-00002ec0: 683a 6061 6020 746f 203a 6d61 7468 3a60  h:`a` to :math:`
-00002ed0: 6260 2069 7320 6772 6561 7465 7220 7468  b` is greater th
-00002ee0: 616e 2074 6865 2073 7472 656e 6774 6820  an the strength 
-00002ef0: 6f66 2074 6865 2073 7472 6f6e 6765 7374  of the strongest
-00002f00: 2070 6174 6820 6672 6f6d 203a 6d61 7468   path from :math
-00002f10: 3a60 6260 2074 6f20 3a6d 6174 683a 6061  :`b` to :math:`a
-00002f20: 602e 2054 6865 6e20 7468 6520 6361 6e64  `. Then the cand
-00002f30: 6964 6174 6573 2074 6861 7420 6172 6520  idates that are 
-00002f40: 756e 6465 6665 6174 6564 2061 6363 6f72  undefeated accor
-00002f50: 6469 6e67 2074 6f20 4265 6174 2050 6174  ding to Beat Pat
-00002f60: 6820 6172 6520 7468 6520 7769 6e6e 6572  h are the winner
-00002f70: 732e 2020 416c 736f 206b 6e6f 776e 2061  s.  Also known a
-00002f80: 7320 7468 6520 5363 6875 6c7a 6520 5275  s the Schulze Ru
-00002f90: 6c65 2e20 0a0a 2020 2020 4172 6773 3a0a  le. ..    Args:.
-00002fa0: 2020 2020 2020 2020 6564 6174 6120 2850          edata (P
-00002fb0: 726f 6669 6c65 2c20 5072 6f66 696c 6557  rofile, ProfileW
-00002fc0: 6974 6854 6965 732c 204d 6172 6769 6e47  ithTies, MarginG
-00002fd0: 7261 7068 293a 2041 6e79 2065 6c65 6374  raph): Any elect
-00002fe0: 696f 6e20 6461 7461 2074 6861 7420 6861  ion data that ha
-00002ff0: 7320 6120 606d 6172 6769 6e60 206d 6574  s a `margin` met
-00003000: 686f 642e 200a 2020 2020 2020 2020 6375  hod. .        cu
-00003010: 7272 5f63 616e 6473 2028 4c69 7374 5b69  rr_cands (List[i
-00003020: 6e74 5d2c 206f 7074 696f 6e61 6c29 3a20  nt], optional): 
-00003030: 4966 2073 6574 2c20 7468 656e 2066 696e  If set, then fin
-00003040: 6420 7468 6520 7769 6e6e 6572 7320 666f  d the winners fo
-00003050: 7220 7468 6520 7072 6f66 696c 6520 7265  r the profile re
-00003060: 7374 7269 6374 6564 2074 6f20 7468 6520  stricted to the 
-00003070: 6361 6e64 6964 6174 6573 2069 6e20 6060  candidates in ``
-00003080: 6375 7272 5f63 616e 6473 6060 0a20 2020  curr_cands``.   
-00003090: 2020 2020 2073 7472 656e 6774 685f 6675       strength_fu
-000030a0: 6e63 7469 6f6e 2028 6675 6e63 7469 6f6e  nction (function
-000030b0: 2c20 6f70 7469 6f6e 616c 293a 2054 6865  , optional): The
-000030c0: 2073 7472 656e 6774 6820 6675 6e63 7469   strength functi
-000030d0: 6f6e 2074 6f20 6265 2075 7365 6420 746f  on to be used to
-000030e0: 2063 616c 6375 6c61 7465 2074 6865 2073   calculate the s
-000030f0: 7472 656e 6774 6820 6f66 2061 2070 6174  trength of a pat
-00003100: 682e 2020 2054 6865 2064 6566 6175 6c74  h.   The default
-00003110: 2069 7320 7468 6520 6d61 7267 696e 206d   is the margin m
-00003120: 6574 686f 6420 6f66 2060 6065 6461 7461  ethod of ``edata
-00003130: 6060 2e20 2020 5468 6973 206f 6e6c 7920  ``.   This only 
-00003140: 6d61 7474 6572 7320 7768 656e 2074 6865  matters when the
-00003150: 2062 616c 6c6f 7473 2061 7265 206e 6f74   ballots are not
-00003160: 206c 696e 6561 7220 6f72 6465 7273 2e20   linear orders. 
-00003170: 0a20 2020 2020 2020 2061 6c67 6f72 6974  .        algorit
-00003180: 686d 2028 7374 7229 3a20 5370 6563 6966  hm (str): Specif
-00003190: 7920 7768 6963 6820 616c 676f 7269 7468  y which algorith
-000031a0: 6d20 746f 2075 7365 2e20 204f 7074 696f  m to use.  Optio
-000031b0: 6e73 2061 7265 2027 666c 6f79 645f 7761  ns are 'floyd_wa
-000031c0: 7273 6861 6c6c 2720 2874 6865 2064 6566  rshall' (the def
-000031d0: 6175 6c74 292c 2027 6261 7369 6327 2c20  ault), 'basic', 
-000031e0: 616e 6420 2773 6368 7761 7274 7a5f 7365  and 'schwartz_se
-000031f0: 7175 656e 7469 616c 5f64 726f 7070 696e  quential_droppin
-00003200: 6727 2e0a 0a20 2020 2052 6574 7572 6e73  g'...    Returns
-00003210: 3a20 0a20 2020 2020 2020 2041 2073 6f72  : .        A sor
-00003220: 7465 6420 6c69 7374 206f 6620 6361 6e64  ted list of cand
-00003230: 6964 6174 6573 2e20 0a0a 2020 2020 2e2e  idates. ..    ..
-00003240: 2073 6565 616c 736f 3a3a 0a0a 2020 2020   seealso::..    
-00003250: 2020 2020 3a6d 6574 683a 6070 7265 665f      :meth:`pref_
-00003260: 766f 7469 6e67 2e6d 6172 6769 6e5f 6261  voting.margin_ba
-00003270: 7365 645f 6d65 7468 6f64 732e 6265 6174  sed_methods.beat
-00003280: 5f70 6174 685f 6465 6665 6174 600a 0a20  _path_defeat`.. 
-00003290: 2020 203a 4578 616d 706c 653a 200a 0a20     :Example: .. 
-000032a0: 2020 202e 2e20 706c 6f74 3a3a 2020 6d61     .. plot::  ma
-000032b0: 7267 696e 5f67 7261 7068 735f 6578 616d  rgin_graphs_exam
-000032c0: 706c 6573 2f6d 675f 6578 5f62 705f 7270  ples/mg_ex_bp_rp
-000032d0: 2e70 790a 2020 2020 2020 2020 3a63 6f6e  .py.        :con
-000032e0: 7465 7874 3a20 7265 7365 7420 200a 2020  text: reset  .  
-000032f0: 2020 2020 2020 3a69 6e63 6c75 6465 2d73        :include-s
-00003300: 6f75 7263 653a 2054 7275 650a 0a0a 2020  ource: True...  
-00003310: 2020 2e2e 2063 6f64 652d 626c 6f63 6b3a    .. code-block:
-00003320: 3a20 0a0a 2020 2020 2020 2020 6672 6f6d  : ..        from
-00003330: 2070 7265 665f 766f 7469 6e67 2e6d 6172   pref_voting.mar
-00003340: 6769 6e5f 6261 7365 645f 6d65 7468 6f64  gin_based_method
-00003350: 7320 696d 706f 7274 2062 6561 745f 7061  s import beat_pa
-00003360: 7468 0a0a 2020 2020 2020 2020 6265 6174  th..        beat
-00003370: 5f70 6174 682e 6469 7370 6c61 7928 6d67  _path.display(mg
-00003380: 290a 0a0a 2020 2020 2e2e 2065 7865 635f  )...    .. exec_
-00003390: 636f 6465 3a3a 200a 2020 2020 2020 2020  code:: .        
-000033a0: 3a68 6964 655f 636f 6465 3a0a 0a20 2020  :hide_code:..   
-000033b0: 2020 2020 2066 726f 6d20 7072 6566 5f76       from pref_v
-000033c0: 6f74 696e 672e 7765 6967 6874 6564 5f6d  oting.weighted_m
-000033d0: 616a 6f72 6974 795f 6772 6170 6873 2069  ajority_graphs i
-000033e0: 6d70 6f72 7420 4d61 7267 696e 4772 6170  mport MarginGrap
-000033f0: 680a 2020 2020 2020 2020 6672 6f6d 2070  h.        from p
-00003400: 7265 665f 766f 7469 6e67 2e6d 6172 6769  ref_voting.margi
-00003410: 6e5f 6261 7365 645f 6d65 7468 6f64 7320  n_based_methods 
-00003420: 696d 706f 7274 2062 6561 745f 7061 7468  import beat_path
-00003430: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00003440: 2020 6d67 203d 204d 6172 6769 6e47 7261    mg = MarginGra
-00003450: 7068 285b 302c 2031 2c20 322c 2033 5d2c  ph([0, 1, 2, 3],
-00003460: 205b 2830 2c20 322c 2033 292c 2028 312c   [(0, 2, 3), (1,
-00003470: 2030 2c20 3529 2c20 2832 2c20 312c 2035   0, 5), (2, 1, 5
-00003480: 292c 2028 322c 2033 2c20 3129 2c20 2833  ), (2, 3, 1), (3
-00003490: 2c20 302c 2033 292c 2028 332c 2031 2c20  , 0, 3), (3, 1, 
-000034a0: 3129 5d29 0a20 2020 2020 2020 200a 2020  1)]).        .  
-000034b0: 2020 2020 2020 6265 6174 5f70 6174 682e        beat_path.
-000034c0: 6469 7370 6c61 7928 6d67 290a 2020 2020  display(mg).    
-000034d0: 2020 2020 6265 6174 5f70 6174 682e 6469      beat_path.di
-000034e0: 7370 6c61 7928 6d67 2c20 616c 676f 7269  splay(mg, algori
-000034f0: 7468 6d3d 2766 6c6f 7964 5f77 6172 7368  thm='floyd_warsh
-00003500: 616c 6c27 2920 0a20 2020 2020 2020 2062  all') .        b
-00003510: 6561 745f 7061 7468 2e64 6973 706c 6179  eat_path.display
-00003520: 286d 672c 2061 6c67 6f72 6974 686d 3d27  (mg, algorithm='
-00003530: 6261 7369 6327 290a 2020 2020 2222 220a  basic').    """.
-00003540: 0a20 2020 2069 6620 616c 676f 7269 7468  .    if algorith
-00003550: 6d20 3d3d 2027 666c 6f79 645f 7761 7273  m == 'floyd_wars
-00003560: 6861 6c6c 273a 0a20 2020 2020 2020 2072  hall':.        r
-00003570: 6574 7572 6e20 5f62 6561 745f 7061 7468  eturn _beat_path
-00003580: 5f66 6c6f 7964 5f77 6172 7368 616c 6c28  _floyd_warshall(
-00003590: 6564 6174 612c 2063 7572 725f 6361 6e64  edata, curr_cand
-000035a0: 7320 3d20 6375 7272 5f63 616e 6473 2c20  s = curr_cands, 
-000035b0: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
-000035c0: 6e20 3d20 7374 7265 6e67 7468 5f66 756e  n = strength_fun
-000035d0: 6374 696f 6e29 0a20 2020 2065 6c69 6620  ction).    elif 
-000035e0: 616c 676f 7269 7468 6d20 3d3d 2027 6261  algorithm == 'ba
-000035f0: 7369 6327 3a0a 2020 2020 2020 2020 7265  sic':.        re
-00003600: 7475 726e 205f 6265 6174 5f70 6174 685f  turn _beat_path_
-00003610: 6261 7369 6328 6564 6174 612c 2063 7572  basic(edata, cur
-00003620: 725f 6361 6e64 7320 3d20 6375 7272 5f63  r_cands = curr_c
-00003630: 616e 6473 2c20 7374 7265 6e67 7468 5f66  ands, strength_f
-00003640: 756e 6374 696f 6e20 3d20 7374 7265 6e67  unction = streng
-00003650: 7468 5f66 756e 6374 696f 6e29 0a20 2020  th_function).   
-00003660: 2065 6c69 6620 616c 676f 7269 7468 6d20   elif algorithm 
-00003670: 3d3d 2027 7363 6877 6172 747a 5f73 6571  == 'schwartz_seq
-00003680: 7565 6e74 6961 6c5f 6472 6f70 7069 6e67  uential_dropping
-00003690: 273a 0a20 2020 2020 2020 2072 6574 7572  ':.        retur
-000036a0: 6e20 5f73 6368 7761 7274 7a5f 7365 7175  n _schwartz_sequ
-000036b0: 656e 7469 616c 5f64 726f 7070 696e 6728  ential_dropping(
-000036c0: 6564 6174 612c 2063 7572 725f 6361 6e64  edata, curr_cand
-000036d0: 7320 3d20 6375 7272 5f63 616e 6473 2c20  s = curr_cands, 
-000036e0: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
-000036f0: 6e20 3d20 7374 7265 6e67 7468 5f66 756e  n = strength_fun
-00003700: 6374 696f 6e29 0a20 2020 2065 6c73 653a  ction).    else:
-00003710: 0a20 2020 2020 2020 2072 6169 7365 2056  .        raise V
-00003720: 616c 7565 4572 726f 7228 2249 6e76 616c  alueError("Inval
-00003730: 6964 2061 6c67 6f72 6974 686d 2073 7065  id algorithm spe
-00003740: 6369 6669 6564 2e22 290a 0a64 6566 2062  cified.")..def b
-00003750: 6561 745f 7061 7468 5f64 6566 6561 7428  eat_path_defeat(
-00003760: 6564 6174 612c 2063 7572 725f 6361 6e64  edata, curr_cand
-00003770: 7320 3d20 4e6f 6e65 2c20 7374 7265 6e67  s = None, streng
-00003780: 7468 5f66 756e 6374 696f 6e20 3d20 4e6f  th_function = No
-00003790: 6e65 293a 2020 200a 2020 2020 2222 2252  ne):   .    """R
-000037a0: 6574 7572 6e73 2074 6865 2064 6566 6561  eturns the defea
-000037b0: 7420 7265 6c61 7469 6f6e 2066 6f72 2042  t relation for B
-000037c0: 6561 7420 5061 7468 2e20 0a20 2020 200a  eat Path. .    .
-000037d0: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-000037e0: 2020 6564 6174 6120 2850 726f 6669 6c65    edata (Profile
-000037f0: 2c20 5072 6f66 696c 6557 6974 6854 6965  , ProfileWithTie
-00003800: 732c 204d 6172 6769 6e47 7261 7068 293a  s, MarginGraph):
-00003810: 2041 6e79 2065 6c65 6374 696f 6e20 6461   Any election da
-00003820: 7461 2074 6861 7420 6861 7320 6120 606d  ta that has a `m
-00003830: 6172 6769 6e60 206d 6574 686f 642e 200a  argin` method. .
-00003840: 2020 2020 2020 2020 6375 7272 5f63 616e          curr_can
-00003850: 6473 2028 4c69 7374 5b69 6e74 5d2c 206f  ds (List[int], o
-00003860: 7074 696f 6e61 6c29 3a20 4966 2073 6574  ptional): If set
-00003870: 2c20 7468 656e 2066 696e 6420 7468 6520  , then find the 
-00003880: 7769 6e6e 6572 7320 666f 7220 7468 6520  winners for the 
-00003890: 7072 6f66 696c 6520 7265 7374 7269 6374  profile restrict
-000038a0: 6564 2074 6f20 7468 6520 6361 6e64 6964  ed to the candid
-000038b0: 6174 6573 2069 6e20 6060 6375 7272 5f63  ates in ``curr_c
-000038c0: 616e 6473 6060 0a20 2020 2020 2020 2073  ands``.        s
-000038d0: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
-000038e0: 2028 6675 6e63 7469 6f6e 2c20 6f70 7469   (function, opti
-000038f0: 6f6e 616c 293a 2054 6865 2073 7472 656e  onal): The stren
-00003900: 6774 6820 6675 6e63 7469 6f6e 2074 6f20  gth function to 
-00003910: 6265 2075 7365 6420 746f 2063 616c 6375  be used to calcu
-00003920: 6c61 7465 2074 6865 2073 7472 656e 6774  late the strengt
-00003930: 6820 6f66 2061 2070 6174 682e 2020 2054  h of a path.   T
-00003940: 6865 2064 6566 6175 6c74 2069 7320 7468  he default is th
-00003950: 6520 6d61 7267 696e 206d 6574 686f 6420  e margin method 
-00003960: 6f66 2060 6065 6461 7461 6060 2e20 2020  of ``edata``.   
-00003970: 5468 6973 206f 6e6c 7920 6d61 7474 6572  This only matter
-00003980: 7320 7768 656e 2074 6865 2062 616c 6c6f  s when the ballo
-00003990: 7473 2061 7265 206e 6f74 206c 696e 6561  ts are not linea
-000039a0: 7220 6f72 6465 7273 2e20 0a0a 2020 2020  r orders. ..    
-000039b0: 5265 7475 726e 733a 200a 2020 2020 2020  Returns: .      
-000039c0: 2020 4120 6e65 7477 6f72 6b78 2044 6947    A networkx DiG
-000039d0: 7261 7068 2072 6570 7265 7365 6e74 696e  raph representin
-000039e0: 6720 7468 6520 4265 6174 2050 6174 6820  g the Beat Path 
-000039f0: 6465 6665 6174 2072 656c 6174 696f 6e2e  defeat relation.
-00003a00: 200a 0a20 2020 202e 2e20 7365 6561 6c73   ..    .. seeals
-00003a10: 6f3a 3a0a 0a20 2020 2020 2020 203a 6d65  o::..        :me
-00003a20: 7468 3a60 7072 6566 5f76 6f74 696e 672e  th:`pref_voting.
-00003a30: 6d61 7267 696e 5f62 6173 6564 5f6d 6574  margin_based_met
-00003a40: 686f 6473 2e62 6561 745f 7061 7468 602c  hods.beat_path`,
-00003a50: 203a 6d65 7468 3a60 7072 6566 5f76 6f74   :meth:`pref_vot
-00003a60: 696e 672e 6d61 7267 696e 5f62 6173 6564  ing.margin_based
-00003a70: 5f6d 6574 686f 6473 2e62 6561 745f 7061  _methods.beat_pa
-00003a80: 7468 5f46 6c6f 7964 5f57 6172 7368 616c  th_Floyd_Warshal
-00003a90: 6c60 0a0a 2020 2020 3a45 7861 6d70 6c65  l`..    :Example
-00003aa0: 3a20 0a0a 2020 2020 2e2e 2070 6c6f 743a  : ..    .. plot:
-00003ab0: 3a20 206d 6172 6769 6e5f 6772 6170 6873  :  margin_graphs
-00003ac0: 5f65 7861 6d70 6c65 732f 6d67 5f65 785f  _examples/mg_ex_
-00003ad0: 6270 5f64 6566 6561 742e 7079 0a20 2020  bp_defeat.py.   
-00003ae0: 2020 2020 203a 636f 6e74 6578 743a 2072       :context: r
-00003af0: 6573 6574 2020 0a20 2020 2020 2020 203a  eset  .        :
-00003b00: 696e 636c 7564 652d 736f 7572 6365 3a20  include-source: 
-00003b10: 5472 7565 0a0a 2020 2020 2222 220a 0a20  True..    """.. 
-00003b20: 2020 2063 616e 6469 6461 7465 7320 3d20     candidates = 
-00003b30: 6564 6174 612e 6361 6e64 6964 6174 6573  edata.candidates
-00003b40: 2069 6620 6375 7272 5f63 616e 6473 2069   if curr_cands i
-00003b50: 7320 4e6f 6e65 2065 6c73 6520 6375 7272  s None else curr
-00003b60: 5f63 616e 6473 2020 2020 0a20 2020 2073  _cands    .    s
-00003b70: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
-00003b80: 203d 2065 6461 7461 2e6d 6172 6769 6e20   = edata.margin 
-00003b90: 6966 2073 7472 656e 6774 685f 6675 6e63  if strength_func
-00003ba0: 7469 6f6e 2069 7320 4e6f 6e65 2065 6c73  tion is None els
-00003bb0: 6520 7374 7265 6e67 7468 5f66 756e 6374  e strength_funct
-00003bc0: 696f 6e0a 2020 2020 2020 2020 0a20 2020  ion.        .   
-00003bd0: 2073 5f6d 6174 7269 7820 3d20 5b5b 2d6e   s_matrix = [[-n
-00003be0: 702e 696e 6620 666f 7220 5f20 696e 2063  p.inf for _ in c
-00003bf0: 616e 6469 6461 7465 735d 2066 6f72 205f  andidates] for _
-00003c00: 2069 6e20 6361 6e64 6964 6174 6573 5d0a   in candidates].
-00003c10: 2020 2020 666f 7220 6331 5f69 6478 2c20      for c1_idx, 
-00003c20: 6331 2069 6e20 656e 756d 6572 6174 6528  c1 in enumerate(
-00003c30: 6361 6e64 6964 6174 6573 293a 0a20 2020  candidates):.   
-00003c40: 2020 2020 2066 6f72 2063 325f 6964 782c       for c2_idx,
-00003c50: 2063 3220 696e 2065 6e75 6d65 7261 7465   c2 in enumerate
-00003c60: 2863 616e 6469 6461 7465 7329 3a0a 2020  (candidates):.  
-00003c70: 2020 2020 2020 2020 2020 6966 2028 6564            if (ed
-00003c80: 6174 612e 6d61 6a6f 7269 7479 5f70 7265  ata.majority_pre
-00003c90: 6665 7273 2863 312c 2063 3229 206f 7220  fers(c1, c2) or 
-00003ca0: 6331 203d 3d20 6332 293a 0a20 2020 2020  c1 == c2):.     
-00003cb0: 2020 2020 2020 2020 2020 2073 5f6d 6174             s_mat
-00003cc0: 7269 785b 6331 5f69 6478 5d5b 6332 5f69  rix[c1_idx][c2_i
-00003cd0: 6478 5d20 3d20 7374 7265 6e67 7468 5f66  dx] = strength_f
-00003ce0: 756e 6374 696f 6e28 6331 2c20 6332 2920  unction(c1, c2) 
-00003cf0: 0a20 2020 2073 7472 656e 6774 6820 3d20  .    strength = 
-00003d00: 6c69 7374 286d 6170 286c 616d 6264 6120  list(map(lambda 
-00003d10: 6920 3a20 6c69 7374 286d 6170 286c 616d  i : list(map(lam
-00003d20: 6264 6120 6a20 3a20 6a20 2c20 6929 2920  bda j : j , i)) 
-00003d30: 2c20 735f 6d61 7472 6978 2929 0a20 2020  , s_matrix)).   
-00003d40: 2066 6f72 2069 5f69 6478 2c20 6920 696e   for i_idx, i in
-00003d50: 2065 6e75 6d65 7261 7465 2863 616e 6469   enumerate(candi
-00003d60: 6461 7465 7329 3a20 2020 2020 2020 2020  dates):         
-00003d70: 0a20 2020 2020 2020 2066 6f72 206a 5f69  .        for j_i
-00003d80: 6478 2c20 6a20 696e 2065 6e75 6d65 7261  dx, j in enumera
-00003d90: 7465 2863 616e 6469 6461 7465 7329 3a20  te(candidates): 
-00003da0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00003db0: 6921 3d20 6a3a 0a20 2020 2020 2020 2020  i!= j:.         
-00003dc0: 2020 2020 2020 2066 6f72 206b 5f69 6478         for k_idx
-00003dd0: 2c20 6b20 696e 2065 6e75 6d65 7261 7465  , k in enumerate
-00003de0: 2863 616e 6469 6461 7465 7329 3a20 0a20  (candidates): . 
-00003df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003e00: 2020 2069 6620 6921 3d20 6b20 616e 6420     if i!= k and 
-00003e10: 6a20 213d 206b 3a0a 2020 2020 2020 2020  j != k:.        
-00003e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003e30: 7374 7265 6e67 7468 5b6a 5f69 6478 5d5b  strength[j_idx][
-00003e40: 6b5f 6964 785d 203d 206d 6178 2873 7472  k_idx] = max(str
-00003e50: 656e 6774 685b 6a5f 6964 785d 5b6b 5f69  ength[j_idx][k_i
-00003e60: 6478 5d2c 206d 696e 2873 7472 656e 6774  dx], min(strengt
-00003e70: 685b 6a5f 6964 785d 5b69 5f69 6478 5d2c  h[j_idx][i_idx],
-00003e80: 7374 7265 6e67 7468 5b69 5f69 6478 5d5b  strength[i_idx][
-00003e90: 6b5f 6964 785d 2929 0a0a 2020 2020 6465  k_idx]))..    de
-00003ea0: 6665 6174 5f67 7261 7068 203d 206e 782e  feat_graph = nx.
-00003eb0: 4469 4772 6170 6828 290a 2020 2020 6465  DiGraph().    de
-00003ec0: 6665 6174 5f67 7261 7068 2e61 6464 5f6e  feat_graph.add_n
-00003ed0: 6f64 6573 5f66 726f 6d28 6361 6e64 6964  odes_from(candid
-00003ee0: 6174 6573 290a 2020 2020 0a20 2020 2066  ates).    .    f
-00003ef0: 6f72 2069 5f69 6478 2c20 6920 696e 2065  or i_idx, i in e
-00003f00: 6e75 6d65 7261 7465 2863 616e 6469 6461  numerate(candida
-00003f10: 7465 7329 3a20 0a20 2020 2020 2020 2066  tes): .        f
-00003f20: 6f72 206a 5f69 6478 2c20 6a20 696e 2065  or j_idx, j in e
-00003f30: 6e75 6d65 7261 7465 2863 616e 6469 6461  numerate(candida
-00003f40: 7465 7329 3a0a 2020 2020 2020 2020 2020  tes):.          
-00003f50: 2020 6966 2069 213d 6a3a 0a20 2020 2020    if i!=j:.     
-00003f60: 2020 2020 2020 2020 2020 2069 6620 7374             if st
-00003f70: 7265 6e67 7468 5b6a 5f69 6478 5d5b 695f  rength[j_idx][i_
-00003f80: 6964 785d 203e 2073 7472 656e 6774 685b  idx] > strength[
-00003f90: 695f 6964 785d 5b6a 5f69 6478 5d3a 0a20  i_idx][j_idx]:. 
-00003fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003fb0: 2020 2064 6566 6561 745f 6772 6170 682e     defeat_graph.
-00003fc0: 6164 645f 7765 6967 6874 6564 5f65 6467  add_weighted_edg
-00003fd0: 6573 5f66 726f 6d28 5b28 6a2c 692c 735f  es_from([(j,i,s_
-00003fe0: 6d61 7472 6978 5b6a 5f69 6478 5d5b 695f  matrix[j_idx][i_
-00003ff0: 6964 785d 295d 290a 0a20 2020 2072 6574  idx])])..    ret
-00004000: 7572 6e20 6465 6665 6174 5f67 7261 7068  urn defeat_graph
-00004010: 0a0a 0a0a 6465 6620 6861 735f 7374 726f  ....def has_stro
-00004020: 6e67 5f70 6174 6828 412c 2073 6f75 7263  ng_path(A, sourc
-00004030: 652c 2074 6172 6765 742c 206b 293a 0a20  e, target, k):. 
-00004040: 2020 2022 2222 4769 7665 6e20 6120 7371     """Given a sq
-00004050: 7561 7265 206d 6174 7269 7820 412c 2072  uare matrix A, r
-00004060: 6574 7572 6e20 5472 7565 2069 6620 7468  eturn True if th
-00004070: 6572 6520 6973 2061 2070 6174 6820 6672  ere is a path fr
-00004080: 6f6d 2073 6f75 7263 6520 746f 2074 6172  om source to tar
-00004090: 6765 7420 696e 2074 6865 2061 7373 6f63  get in the assoc
-000040a0: 6961 7465 6420 6469 7265 6374 6564 2067  iated directed g
-000040b0: 7261 7068 2020 2020 2077 6865 7265 2065  raph     where e
-000040c0: 6163 6820 6564 6765 2068 6173 2061 2077  ach edge has a w
-000040d0: 6569 6768 7420 6772 6561 7465 7220 7468  eight greater th
-000040e0: 616e 206f 7220 6571 7561 6c20 746f 206b  an or equal to k
-000040f0: 2c20 616e 6420 4661 6c73 6520 6f74 6865  , and False othe
-00004100: 7277 6973 652e 2222 220a 2020 2020 0a20  rwise.""".    . 
-00004110: 2020 206e 203d 2041 2e73 6861 7065 5b30     n = A.shape[0
-00004120: 5d20 2320 6173 7375 6d65 2041 2069 7320  ] # assume A is 
-00004130: 6120 7371 7561 7265 206d 6174 7269 780a  a square matrix.
-00004140: 2020 2020 7669 7369 7465 6420 3d20 6e70      visited = np
-00004150: 2e7a 6572 6f73 286e 2c20 6474 7970 653d  .zeros(n, dtype=
-00004160: 626f 6f6c 290a 0a20 2020 2064 6566 2064  bool)..    def d
-00004170: 6673 286e 6f64 6529 3a0a 2020 2020 2020  fs(node):.      
-00004180: 2020 6966 206e 6f64 6520 3d3d 2074 6172    if node == tar
-00004190: 6765 743a 0a20 2020 2020 2020 2020 2020  get:.           
-000041a0: 2072 6574 7572 6e20 5472 7565 0a20 2020   return True.   
-000041b0: 2020 2020 2076 6973 6974 6564 5b6e 6f64       visited[nod
-000041c0: 655d 203d 2054 7275 650a 2020 2020 2020  e] = True.      
-000041d0: 2020 666f 7220 6e65 6967 6862 6f72 2c20    for neighbor, 
-000041e0: 7765 6967 6874 2069 6e20 656e 756d 6572  weight in enumer
-000041f0: 6174 6528 415b 6e6f 6465 2c20 3a5d 293a  ate(A[node, :]):
-00004200: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00004210: 415b 6e6f 6465 5d5b 6e65 6967 6862 6f72  A[node][neighbor
-00004220: 5d20 3e20 415b 6e65 6967 6862 6f72 5d5b  ] > A[neighbor][
-00004230: 6e6f 6465 5d20 616e 6420 7765 6967 6874  node] and weight
-00004240: 203e 3d20 6b20 616e 6420 6e6f 7420 7669   >= k and not vi
-00004250: 7369 7465 645b 6e65 6967 6862 6f72 5d3a  sited[neighbor]:
-00004260: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004270: 2069 6620 6466 7328 6e65 6967 6862 6f72   if dfs(neighbor
-00004280: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00004290: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
-000042a0: 7565 0a20 2020 2020 2020 2072 6574 7572  ue.        retur
-000042b0: 6e20 4661 6c73 650a 0a20 2020 2072 6574  n False..    ret
-000042c0: 7572 6e20 6466 7328 736f 7572 6365 290a  urn dfs(source).
-000042d0: 0a64 6566 205f 7370 6c69 745f 6379 636c  .def _split_cycl
-000042e0: 655f 6261 7369 6328 0a20 2020 2020 2020  e_basic(.       
-000042f0: 2065 6461 7461 2c20 0a20 2020 2020 2020   edata, .       
-00004300: 2063 7572 725f 6361 6e64 7320 3d20 4e6f   curr_cands = No
-00004310: 6e65 2c20 0a20 2020 2020 2020 2073 7472  ne, .        str
-00004320: 656e 6774 685f 6675 6e63 7469 6f6e 203d  ength_function =
-00004330: 204e 6f6e 6529 3a0a 2020 2020 2222 2241   None):.    """A
-00004340: 6e20 696d 706c 656d 656e 7461 7469 6f6e  n implementation
-00004350: 206f 6620 5370 6c69 7420 4379 636c 6520   of Split Cycle 
-00004360: 6261 7365 6420 6f6e 2074 6865 206d 6174  based on the mat
-00004370: 6865 6d61 7469 6361 6c20 6465 6669 6e69  hematical defini
-00004380: 7469 6f6e 2e20 2054 6869 7320 6973 206d  tion.  This is m
-00004390: 6f72 6520 6566 6669 6369 656e 7420 7468  ore efficient th
-000043a0: 616e 2074 6865 2066 6c6f 7964 5f77 6172  an the floyd_war
-000043b0: 7368 616c 6c20 696d 706c 656d 656e 7461  shall implementa
-000043c0: 7469 6f6e 2e20 0a20 2020 2022 2222 0a20  tion. .    """. 
-000043d0: 2020 2073 7472 656e 6774 685f 6d61 7472     strength_matr
-000043e0: 6978 2c20 6361 6e64 5f74 6f5f 6369 6e64  ix, cand_to_cind
-000043f0: 6578 203d 2065 6461 7461 2e73 7472 656e  ex = edata.stren
-00004400: 6774 685f 6d61 7472 6978 2863 7572 725f  gth_matrix(curr_
-00004410: 6361 6e64 7320 3d20 6375 7272 5f63 616e  cands = curr_can
-00004420: 6473 2c20 7374 7265 6e67 7468 5f66 756e  ds, strength_fun
-00004430: 6374 696f 6e3d 7374 7265 6e67 7468 5f66  ction=strength_f
-00004440: 756e 6374 696f 6e29 0a0a 2020 2020 6361  unction)..    ca
-00004450: 6e64 6964 6174 6573 203d 2065 6461 7461  ndidates = edata
-00004460: 2e63 616e 6469 6461 7465 7320 6966 2063  .candidates if c
-00004470: 7572 725f 6361 6e64 7320 6973 204e 6f6e  urr_cands is Non
-00004480: 6520 656c 7365 2063 7572 725f 6361 6e64  e else curr_cand
-00004490: 7320 200a 0a20 2020 2073 7472 656e 6774  s  ..    strengt
-000044a0: 685f 6675 6e63 7469 6f6e 203d 2065 6461  h_function = eda
-000044b0: 7461 2e6d 6172 6769 6e20 6966 2073 7472  ta.margin if str
-000044c0: 656e 6774 685f 6675 6e63 7469 6f6e 2069  ength_function i
-000044d0: 7320 4e6f 6e65 2065 6c73 6520 7374 7265  s None else stre
-000044e0: 6e67 7468 5f66 756e 6374 696f 6e20 0a0a  ngth_function ..
-000044f0: 2020 2020 706f 7465 6e74 6961 6c5f 7769      potential_wi
-00004500: 6e6e 6572 7320 3d20 7365 7428 6361 6e64  nners = set(cand
-00004510: 6964 6174 6573 290a 0a20 2020 2066 6f72  idates)..    for
-00004520: 2061 2069 6e20 6361 6e64 6964 6174 6573   a in candidates
-00004530: 3a0a 2020 2020 2020 2020 666f 7220 6220  :.        for b 
-00004540: 696e 2063 616e 6469 6461 7465 733a 0a20  in candidates:. 
-00004550: 2020 2020 2020 2020 2020 2069 6620 7374             if st
-00004560: 7265 6e67 7468 5f66 756e 6374 696f 6e28  rength_function(
-00004570: 622c 2061 2920 3e20 7374 7265 6e67 7468  b, a) > strength
-00004580: 5f66 756e 6374 696f 6e28 612c 2062 2920  _function(a, b) 
-00004590: 616e 6420 6e6f 7420 6861 735f 7374 726f  and not has_stro
-000045a0: 6e67 5f70 6174 6828 7374 7265 6e67 7468  ng_path(strength
-000045b0: 5f6d 6174 7269 782c 2063 616e 645f 746f  _matrix, cand_to
-000045c0: 5f63 696e 6465 7828 6129 2c20 6361 6e64  _cindex(a), cand
-000045d0: 5f74 6f5f 6369 6e64 6578 2862 292c 2073  _to_cindex(b), s
-000045e0: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
-000045f0: 2862 2c61 2929 3a0a 2020 2020 2020 2020  (b,a)):.        
-00004600: 2020 2020 2020 2020 706f 7465 6e74 6961          potentia
-00004610: 6c5f 7769 6e6e 6572 732e 6469 7363 6172  l_winners.discar
-00004620: 6428 6129 0a20 2020 2020 2020 2020 2020  d(a).           
-00004630: 2020 2020 2062 7265 616b 0a0a 2020 2020       break..    
-00004640: 7265 7475 726e 2073 6f72 7465 6428 706f  return sorted(po
-00004650: 7465 6e74 6961 6c5f 7769 6e6e 6572 7329  tential_winners)
-00004660: 0a0a 6465 6620 5f73 706c 6974 5f63 7963  ..def _split_cyc
-00004670: 6c65 5f66 6c6f 7964 5f77 6172 7368 616c  le_floyd_warshal
-00004680: 6c28 0a20 2020 2020 2020 2065 6461 7461  l(.        edata
-00004690: 2c20 0a20 2020 2020 2020 2063 7572 725f  , .        curr_
-000046a0: 6361 6e64 7320 3d20 4e6f 6e65 2c20 0a20  cands = None, . 
-000046b0: 2020 2020 2020 2073 7472 656e 6774 685f         strength_
-000046c0: 6675 6e63 7469 6f6e 203d 204e 6f6e 6529  function = None)
-000046d0: 3a20 2020 0a20 2020 2022 2222 416e 2069  :   .    """An i
-000046e0: 6d70 6c65 6d65 6e74 6174 696f 6e20 6f66  mplementation of
-000046f0: 2053 706c 6974 2043 7963 6c65 2062 6173   Split Cycle bas
-00004700: 6564 206f 6e20 7468 6520 466c 6f79 642d  ed on the Floyd-
-00004710: 5761 7273 6861 6c6c 2041 6c67 6f72 6974  Warshall Algorit
-00004720: 686d 2e20 0a0a 2020 2020 5365 6520 6874  hm. ..    See ht
-00004730: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00004740: 2f65 7061 6375 6974 2f73 706c 6974 6379  /epacuit/splitcy
-00004750: 636c 6520 616e 6420 7468 6520 7061 7065  cle and the pape
-00004760: 7220 6874 7470 733a 2f2f 6172 7869 762e  r https://arxiv.
-00004770: 6f72 672f 6162 732f 3230 3034 2e30 3233  org/abs/2004.023
-00004780: 3530 2066 6f72 206d 6f72 6520 696e 666f  50 for more info
-00004790: 726d 6174 696f 6e2e 200a 0a20 2020 2022  rmation. ..    "
-000047a0: 2222 0a0a 2020 2020 6361 6e64 6964 6174  ""..    candidat
-000047b0: 6573 203d 2065 6461 7461 2e63 616e 6469  es = edata.candi
-000047c0: 6461 7465 7320 6966 2063 7572 725f 6361  dates if curr_ca
-000047d0: 6e64 7320 6973 204e 6f6e 6520 656c 7365  nds is None else
-000047e0: 2063 7572 725f 6361 6e64 7320 2020 200a   curr_cands    .
-000047f0: 2020 2020 7374 7265 6e67 7468 5f66 756e      strength_fun
-00004800: 6374 696f 6e20 3d20 6564 6174 612e 6d61  ction = edata.ma
-00004810: 7267 696e 2069 6620 7374 7265 6e67 7468  rgin if strength
-00004820: 5f66 756e 6374 696f 6e20 6973 204e 6f6e  _function is Non
-00004830: 6520 656c 7365 2073 7472 656e 6774 685f  e else strength_
-00004840: 6675 6e63 7469 6f6e 200a 200a 2020 2020  function . .    
-00004850: 7765 616b 5f63 6f6e 646f 7263 6574 5f77  weak_condorcet_w
-00004860: 696e 6e65 7273 203d 207b 633a 5472 7565  inners = {c:True
-00004870: 2066 6f72 2063 2069 6e20 6361 6e64 6964   for c in candid
-00004880: 6174 6573 7d0a 2020 2020 735f 6d61 7472  ates}.    s_matr
-00004890: 6978 203d 205b 5b2d 6e70 2e69 6e66 2066  ix = [[-np.inf f
-000048a0: 6f72 205f 2069 6e20 6361 6e64 6964 6174  or _ in candidat
-000048b0: 6573 5d20 666f 7220 5f20 696e 2063 616e  es] for _ in can
-000048c0: 6469 6461 7465 735d 0a20 2020 200a 2020  didates].    .  
-000048d0: 2020 2320 696e 6974 6961 6c69 7a65 2074    # initialize t
-000048e0: 6865 2073 5f6d 6174 7269 780a 2020 2020  he s_matrix.    
-000048f0: 666f 7220 6331 5f69 6478 2c20 6331 2069  for c1_idx, c1 i
-00004900: 6e20 656e 756d 6572 6174 6528 6361 6e64  n enumerate(cand
-00004910: 6964 6174 6573 293a 0a20 2020 2020 2020  idates):.       
-00004920: 2066 6f72 2063 325f 6964 782c 2063 3220   for c2_idx, c2 
-00004930: 696e 2065 6e75 6d65 7261 7465 2863 616e  in enumerate(can
-00004940: 6469 6461 7465 7329 3a0a 2020 2020 2020  didates):.      
-00004950: 2020 2020 2020 6966 2028 6564 6174 612e        if (edata.
-00004960: 6d61 6a6f 7269 7479 5f70 7265 6665 7273  majority_prefers
-00004970: 2863 312c 2063 3229 206f 7220 6331 203d  (c1, c2) or c1 =
-00004980: 3d20 6332 293a 0a20 2020 2020 2020 2020  = c2):.         
-00004990: 2020 2020 2020 2073 5f6d 6174 7269 785b         s_matrix[
-000049a0: 6331 5f69 6478 5d5b 6332 5f69 6478 5d20  c1_idx][c2_idx] 
-000049b0: 3d20 7374 7265 6e67 7468 5f66 756e 6374  = strength_funct
-000049c0: 696f 6e28 6331 2c20 6332 2920 0a20 2020  ion(c1, c2) .   
-000049d0: 2020 2020 2020 2020 2020 2020 2077 6561               wea
-000049e0: 6b5f 636f 6e64 6f72 6365 745f 7769 6e6e  k_condorcet_winn
-000049f0: 6572 735b 6332 5d20 3d20 7765 616b 5f63  ers[c2] = weak_c
-00004a00: 6f6e 646f 7263 6574 5f77 696e 6e65 7273  ondorcet_winners
-00004a10: 5b63 325d 2061 6e64 2028 6331 203d 3d20  [c2] and (c1 == 
-00004a20: 6332 2920 2320 5765 616b 2043 6f6e 646f  c2) # Weak Condo
-00004a30: 7263 6574 2077 696e 6e65 7273 2061 7265  rcet winners are
-00004a40: 2053 706c 6974 2043 7963 6c65 2077 696e   Split Cycle win
-00004a50: 6e65 7273 0a20 2020 200a 2020 2020 7374  ners.    .    st
-00004a60: 7265 6e67 7468 203d 206c 6973 7428 6d61  rength = list(ma
-00004a70: 7028 6c61 6d62 6461 2069 203a 206c 6973  p(lambda i : lis
-00004a80: 7428 6d61 7028 6c61 6d62 6461 206a 203a  t(map(lambda j :
-00004a90: 206a 202c 2069 2929 202c 2073 5f6d 6174   j , i)) , s_mat
-00004aa0: 7269 7829 290a 2020 2020 666f 7220 695f  rix)).    for i_
-00004ab0: 6964 782c 2069 2069 6e20 656e 756d 6572  idx, i in enumer
-00004ac0: 6174 6528 6361 6e64 6964 6174 6573 293a  ate(candidates):
-00004ad0: 200a 2020 2020 2020 2020 666f 7220 6a5f   .        for j_
-00004ae0: 6964 782c 206a 2069 6e20 656e 756d 6572  idx, j in enumer
-00004af0: 6174 6528 6361 6e64 6964 6174 6573 293a  ate(candidates):
-00004b00: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00004b10: 6921 3d20 6a3a 0a20 2020 2020 2020 2020  i!= j:.         
-00004b20: 2020 2020 2020 2069 6620 6e6f 7420 7765         if not we
-00004b30: 616b 5f63 6f6e 646f 7263 6574 5f77 696e  ak_condorcet_win
-00004b40: 6e65 7273 5b6a 5d3a 2023 2077 6561 6b20  ners[j]: # weak 
-00004b50: 436f 6e64 6f72 6365 7420 7769 6e6e 6572  Condorcet winner
-00004b60: 7320 6172 6520 5370 6c69 7420 4379 636c  s are Split Cycl
-00004b70: 6520 7769 6e6e 6572 730a 2020 2020 2020  e winners.      
-00004b80: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-00004b90: 7220 6b5f 6964 782c 206b 2069 6e20 656e  r k_idx, k in en
-00004ba0: 756d 6572 6174 6528 6361 6e64 6964 6174  umerate(candidat
-00004bb0: 6573 293a 200a 2020 2020 2020 2020 2020  es): .          
-00004bc0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00004bd0: 2069 2021 3d20 6b20 616e 6420 6a20 213d   i != k and j !=
-00004be0: 206b 3a0a 2020 2020 2020 2020 2020 2020   k:.            
-00004bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c00: 7374 7265 6e67 7468 5b6a 5f69 6478 5d5b  strength[j_idx][
-00004c10: 6b5f 6964 785d 203d 206d 6178 2873 7472  k_idx] = max(str
-00004c20: 656e 6774 685b 6a5f 6964 785d 5b6b 5f69  ength[j_idx][k_i
-00004c30: 6478 5d2c 206d 696e 2873 7472 656e 6774  dx], min(strengt
-00004c40: 685b 6a5f 6964 785d 5b69 5f69 6478 5d2c  h[j_idx][i_idx],
-00004c50: 7374 7265 6e67 7468 5b69 5f69 6478 5d5b  strength[i_idx][
-00004c60: 6b5f 6964 785d 2929 0a20 2020 2077 696e  k_idx])).    win
-00004c70: 6e65 7273 203d 207b 693a 5472 7565 2066  ners = {i:True f
-00004c80: 6f72 2069 2069 6e20 6361 6e64 6964 6174  or i in candidat
-00004c90: 6573 7d0a 2020 2020 666f 7220 695f 6964  es}.    for i_id
-00004ca0: 782c 2069 2069 6e20 656e 756d 6572 6174  x, i in enumerat
-00004cb0: 6528 6361 6e64 6964 6174 6573 293a 0a20  e(candidates):. 
-00004cc0: 2020 2020 2020 2066 6f72 206a 5f69 6478         for j_idx
-00004cd0: 2c20 6a20 696e 2065 6e75 6d65 7261 7465  , j in enumerate
-00004ce0: 2863 616e 6469 6461 7465 7329 3a0a 2020  (candidates):.  
-00004cf0: 2020 2020 2020 2020 2020 6966 2069 2021            if i !
-00004d00: 3d20 6a3a 0a20 2020 2020 2020 2020 2020  = j:.           
-00004d10: 2020 2020 2069 6620 735f 6d61 7472 6978       if s_matrix
-00004d20: 5b6a 5f69 6478 5d5b 695f 6964 785d 203e  [j_idx][i_idx] >
-00004d30: 2073 7472 656e 6774 685b 695f 6964 785d   strength[i_idx]
-00004d40: 5b6a 5f69 6478 5d3a 2023 2074 6865 206d  [j_idx]: # the m
-00004d50: 6169 6e20 6469 6666 6572 656e 6365 2077  ain difference w
-00004d60: 6974 6820 4265 6174 2050 6174 680a 2020  ith Beat Path.  
-00004d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004d80: 2020 7769 6e6e 6572 735b 695d 203d 2046    winners[i] = F
-00004d90: 616c 7365 0a20 2020 2072 6574 7572 6e20  alse.    return 
-00004da0: 736f 7274 6564 285b 6320 666f 7220 6320  sorted([c for c 
-00004db0: 696e 2063 616e 6469 6461 7465 7320 6966  in candidates if
-00004dc0: 2077 696e 6e65 7273 5b63 5d5d 290a 0a73   winners[c]])..s
-00004dd0: 635f 7072 6f70 6572 7469 6573 203d 2056  c_properties = V
-00004de0: 6f74 696e 674d 6574 686f 6450 726f 7065  otingMethodPrope
-00004df0: 7274 6965 7328 0a20 2020 2063 6f6e 646f  rties(.    condo
-00004e00: 7263 6574 5f77 696e 6e65 723d 5472 7565  rcet_winner=True
-00004e10: 2c20 0a20 2020 2063 6f6e 646f 7263 6574  , .    condorcet
-00004e20: 5f6c 6f73 6572 3d54 7275 652c 0a20 2020  _loser=True,.   
-00004e30: 2070 6172 6574 6f5f 646f 6d69 6e61 6e63   pareto_dominanc
-00004e40: 653d 5472 7565 2c0a 2020 2020 706f 7369  e=True,.    posi
-00004e50: 7469 7665 5f69 6e76 6f6c 7665 6d65 6e74  tive_involvement
-00004e60: 3d54 7275 652c 200a 2020 2020 290a 4076  =True, .    ).@v
-00004e70: 6d28 6e61 6d65 3d22 5370 6c69 7420 4379  m(name="Split Cy
-00004e80: 636c 6522 2c0a 2020 2020 7072 6f70 6572  cle",.    proper
-00004e90: 7469 6573 3d73 635f 7072 6f70 6572 7469  ties=sc_properti
-00004ea0: 6573 2c0a 2020 2020 696e 7075 745f 7479  es,.    input_ty
-00004eb0: 7065 733d 5b45 6c65 6374 696f 6e54 7970  pes=[ElectionTyp
-00004ec0: 6573 2e50 524f 4649 4c45 2c20 456c 6563  es.PROFILE, Elec
-00004ed0: 7469 6f6e 5479 7065 732e 5052 4f46 494c  tionTypes.PROFIL
-00004ee0: 455f 5749 5448 5f54 4945 532c 2045 6c65  E_WITH_TIES, Ele
-00004ef0: 6374 696f 6e54 7970 6573 2e4d 4152 4749  ctionTypes.MARGI
-00004f00: 4e5f 4752 4150 485d 290a 6465 6620 7370  N_GRAPH]).def sp
-00004f10: 6c69 745f 6379 636c 6528 0a20 2020 2065  lit_cycle(.    e
-00004f20: 6461 7461 2c20 0a20 2020 2063 7572 725f  data, .    curr_
-00004f30: 6361 6e64 733d 4e6f 6e65 2c20 0a20 2020  cands=None, .   
-00004f40: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
-00004f50: 6f6e 3d4e 6f6e 652c 0a20 2020 2061 6c67  on=None,.    alg
-00004f60: 6f72 6974 686d 3d27 6261 7369 6327 293a  orithm='basic'):
-00004f70: 0a0a 2020 2020 2222 2241 202a 2a6d 616a  ..    """A **maj
-00004f80: 6f72 6974 7920 6379 636c 652a 2a20 6973  ority cycle** is
-00004f90: 2061 2073 6571 7565 6e63 6520 3a6d 6174   a sequence :mat
-00004fa0: 683a 6078 5f31 2c20 5c6c 646f 7473 202c  h:`x_1, \ldots ,
-00004fb0: 785f 6e60 206f 6620 6469 7374 696e 6374  x_n` of distinct
-00004fc0: 2063 616e 6469 6461 7465 7320 7769 7468   candidates with
-00004fd0: 203a 6d61 7468 3a60 785f 313d 785f 6e60   :math:`x_1=x_n`
-00004fe0: 2073 7563 6820 7468 6174 2066 6f72 203a   such that for :
-00004ff0: 6d61 7468 3a60 3120 5c6c 6571 206b 205c  math:`1 \leq k \
-00005000: 6c65 7120 6e2d 3160 2c20 203a 6d61 7468  leq n-1`,  :math
-00005010: 3a60 785f 6b60 2069 7320 6d61 6a6f 7269  :`x_k` is majori
-00005020: 7479 2070 7265 6665 7272 6564 2074 6f20  ty preferred to 
-00005030: 3a6d 6174 683a 6078 5f7b 6b2b 317d 602e  :math:`x_{k+1}`.
-00005040: 2020 5468 6520 5370 6c69 7420 4379 636c    The Split Cycl
-00005050: 6520 7769 6e6e 6572 7320 6172 6520 6465  e winners are de
-00005060: 7465 726d 696e 6564 2061 7320 666f 6c6c  termined as foll
-00005070: 6f77 733a 2020 0a20 2020 200a 2020 2020  ows:  .    .    
-00005080: 4966 2063 616e 6469 6461 7465 2078 2068  If candidate x h
-00005090: 6173 2061 2070 6f73 6974 6976 6520 6d61  as a positive ma
-000050a0: 7267 696e 206f 7665 7220 7920 616e 6420  rgin over y and 
-000050b0: 2878 2c79 2920 6973 206e 6f74 2074 6865  (x,y) is not the
-000050c0: 2077 6561 6b65 7374 2065 6467 6520 696e   weakest edge in
-000050d0: 2061 2063 7963 6c65 2c20 7468 656e 2078   a cycle, then x
-000050e0: 2064 6566 6561 7473 2079 2e20 4571 7569   defeats y. Equi
-000050f0: 7661 6c65 6e74 6c79 2c20 6966 2078 2068  valently, if x h
-00005100: 6173 2061 2070 6f73 6974 6976 6520 6d61  as a positive ma
-00005110: 7267 696e 206f 7665 7220 7920 616e 6420  rgin over y and 
-00005120: 7468 6572 6520 6973 206e 6f20 7061 7468  there is no path
-00005130: 2066 726f 6d20 7920 6261 636b 2074 6f20   from y back to 
-00005140: 7820 6f66 2073 7472 656e 6774 6820 6174  x of strength at
-00005150: 206c 6561 7374 2074 6865 206d 6172 6769   least the margi
-00005160: 6e20 6f66 2078 206f 7665 7220 792c 2074  n of x over y, t
-00005170: 6865 6e20 7820 6465 6665 6174 7320 792e  hen x defeats y.
-00005180: 200a 2020 2020 0a20 2020 2054 6865 2063   .    .    The c
-00005190: 616e 6469 6461 7465 7320 7468 6174 2061  andidates that a
-000051a0: 7265 2075 6e64 6566 6561 7465 6420 6172  re undefeated ar
-000051b0: 6520 7468 6520 5370 6c69 7420 4379 636c  e the Split Cycl
-000051c0: 6520 7769 6e6e 6572 732e 0a0a 2020 2020  e winners...    
-000051d0: 5365 6520 6874 7470 733a 2f2f 6769 7468  See https://gith
-000051e0: 7562 2e63 6f6d 2f65 7061 6375 6974 2f73  ub.com/epacuit/s
-000051f0: 706c 6974 6379 636c 6520 616e 6420 7468  plitcycle and th
-00005200: 6520 7061 7065 7220 6874 7470 733a 2f2f  e paper https://
-00005210: 6172 7869 762e 6f72 672f 6162 732f 3230  arxiv.org/abs/20
-00005220: 3034 2e30 3233 3530 2066 6f72 206d 6f72  04.02350 for mor
-00005230: 6520 696e 666f 726d 6174 696f 6e2e 200a  e information. .
-00005240: 0a20 2020 2041 7267 733a 0a20 2020 2020  .    Args:.     
-00005250: 2020 2065 6461 7461 2028 5072 6f66 696c     edata (Profil
-00005260: 652c 2050 726f 6669 6c65 5769 7468 5469  e, ProfileWithTi
-00005270: 6573 2c20 4d61 7267 696e 4772 6170 6829  es, MarginGraph)
-00005280: 3a20 416e 7920 656c 6563 7469 6f6e 2064  : Any election d
-00005290: 6174 6120 7468 6174 2068 6173 2061 2060  ata that has a `
-000052a0: 6d61 7267 696e 6020 6d65 7468 6f64 2e20  margin` method. 
-000052b0: 0a20 2020 2020 2020 2063 7572 725f 6361  .        curr_ca
-000052c0: 6e64 7320 284c 6973 745b 696e 745d 2c20  nds (List[int], 
-000052d0: 6f70 7469 6f6e 616c 293a 2049 6620 7365  optional): If se
-000052e0: 742c 2074 6865 6e20 6669 6e64 2074 6865  t, then find the
-000052f0: 2077 696e 6e65 7273 2066 6f72 2074 6865   winners for the
-00005300: 2070 726f 6669 6c65 2072 6573 7472 6963   profile restric
-00005310: 7465 6420 746f 2074 6865 2063 616e 6469  ted to the candi
-00005320: 6461 7465 7320 696e 2060 6063 7572 725f  dates in ``curr_
-00005330: 6361 6e64 7360 600a 2020 2020 2020 2020  cands``.        
-00005340: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
-00005350: 6e20 2866 756e 6374 696f 6e2c 206f 7074  n (function, opt
-00005360: 696f 6e61 6c29 3a20 5468 6520 7374 7265  ional): The stre
-00005370: 6e67 7468 2066 756e 6374 696f 6e20 746f  ngth function to
-00005380: 2062 6520 7573 6564 2074 6f20 6361 6c63   be used to calc
-00005390: 756c 6174 6520 7468 6520 7374 7265 6e67  ulate the streng
-000053a0: 7468 206f 6620 6120 7061 7468 2e20 2020  th of a path.   
-000053b0: 5468 6520 6465 6661 756c 7420 6973 2074  The default is t
-000053c0: 6865 206d 6172 6769 6e20 6d65 7468 6f64  he margin method
-000053d0: 206f 6620 6060 6564 6174 6160 602e 2020   of ``edata``.  
-000053e0: 2054 6869 7320 6f6e 6c79 206d 6174 7465   This only matte
-000053f0: 7273 2077 6865 6e20 7468 6520 6261 6c6c  rs when the ball
-00005400: 6f74 7320 6172 6520 6e6f 7420 6c69 6e65  ots are not line
-00005410: 6172 206f 7264 6572 732e 200a 2020 2020  ar orders. .    
-00005420: 2020 2020 616c 676f 7269 7468 6d20 2873      algorithm (s
-00005430: 7472 293a 2053 7065 6369 6679 2077 6869  tr): Specify whi
-00005440: 6368 2061 6c67 6f72 6974 686d 2074 6f20  ch algorithm to 
-00005450: 7573 652e 2020 4f70 7469 6f6e 7320 6172  use.  Options ar
-00005460: 6520 2762 6173 6963 2720 2874 6865 2064  e 'basic' (the d
-00005470: 6566 6175 6c74 2920 616e 6420 2766 6c6f  efault) and 'flo
-00005480: 7964 5f77 6172 7368 616c 6c27 2e0a 0a20  yd_warshall'... 
-00005490: 2020 2052 6574 7572 6e73 3a20 0a20 2020     Returns: .   
-000054a0: 2020 2020 2041 2073 6f72 7465 6420 6c69       A sorted li
-000054b0: 7374 206f 6620 6361 6e64 6964 6174 6573  st of candidates
-000054c0: 2e20 0a0a 2020 2020 2e2e 2073 6565 616c  . ..    .. seeal
-000054d0: 736f 3a3a 0a0a 2020 2020 2020 2020 3a6d  so::..        :m
-000054e0: 6574 683a 6070 7265 665f 766f 7469 6e67  eth:`pref_voting
-000054f0: 2e6d 6172 6769 6e5f 6261 7365 645f 6d65  .margin_based_me
-00005500: 7468 6f64 732e 7370 6c69 745f 6379 636c  thods.split_cycl
-00005510: 655f 6465 6665 6174 600a 0a20 2020 203a  e_defeat`..    :
-00005520: 4578 616d 706c 653a 200a 0a20 2020 202e  Example: ..    .
-00005530: 2e20 706c 6f74 3a3a 2020 6d61 7267 696e  . plot::  margin
-00005540: 5f67 7261 7068 735f 6578 616d 706c 6573  _graphs_examples
-00005550: 2f6d 675f 6578 5f62 705f 7270 2e70 790a  /mg_ex_bp_rp.py.
-00005560: 2020 2020 2020 2020 3a63 6f6e 7465 7874          :context
-00005570: 3a20 7265 7365 7420 200a 2020 2020 2020  : reset  .      
-00005580: 2020 3a69 6e63 6c75 6465 2d73 6f75 7263    :include-sourc
-00005590: 653a 2054 7275 650a 0a20 2020 202e 2e20  e: True..    .. 
-000055a0: 636f 6465 2d62 6c6f 636b 3a3a 200a 0a20  code-block:: .. 
-000055b0: 2020 2020 2020 2066 726f 6d20 7072 6566         from pref
-000055c0: 5f76 6f74 696e 672e 6d61 7267 696e 5f62  _voting.margin_b
-000055d0: 6173 6564 5f6d 6574 686f 6473 2069 6d70  ased_methods imp
-000055e0: 6f72 7420 7370 6c69 745f 6379 636c 650a  ort split_cycle.
-000055f0: 0a20 2020 2020 2020 2073 706c 6974 5f63  .        split_c
-00005600: 7963 6c65 2e64 6973 706c 6179 286d 6729  ycle.display(mg)
-00005610: 0a0a 0a20 2020 202e 2e20 6578 6563 5f63  ...    .. exec_c
-00005620: 6f64 653a 3a20 0a20 2020 2020 2020 203a  ode:: .        :
-00005630: 6869 6465 5f63 6f64 653a 0a0a 2020 2020  hide_code:..    
-00005640: 2020 2020 6672 6f6d 2070 7265 665f 766f      from pref_vo
-00005650: 7469 6e67 2e77 6569 6768 7465 645f 6d61  ting.weighted_ma
-00005660: 6a6f 7269 7479 5f67 7261 7068 7320 696d  jority_graphs im
-00005670: 706f 7274 204d 6172 6769 6e47 7261 7068  port MarginGraph
-00005680: 0a20 2020 2020 2020 2066 726f 6d20 7072  .        from pr
-00005690: 6566 5f76 6f74 696e 672e 6d61 7267 696e  ef_voting.margin
-000056a0: 5f62 6173 6564 5f6d 6574 686f 6473 2069  _based_methods i
-000056b0: 6d70 6f72 7420 7370 6c69 745f 6379 636c  mport split_cycl
-000056c0: 650a 2020 2020 2020 2020 0a20 2020 2020  e.        .     
-000056d0: 2020 206d 6720 3d20 4d61 7267 696e 4772     mg = MarginGr
-000056e0: 6170 6828 5b30 2c20 312c 2032 2c20 335d  aph([0, 1, 2, 3]
-000056f0: 2c20 5b28 302c 2032 2c20 3329 2c20 2831  , [(0, 2, 3), (1
-00005700: 2c20 302c 2035 292c 2028 322c 2031 2c20  , 0, 5), (2, 1, 
-00005710: 3529 2c20 2832 2c20 332c 2031 292c 2028  5), (2, 3, 1), (
-00005720: 332c 2030 2c20 3329 2c20 2833 2c20 312c  3, 0, 3), (3, 1,
-00005730: 2031 295d 290a 2020 2020 2020 2020 0a20   1)]).        . 
-00005740: 2020 2020 2020 2073 706c 6974 5f63 7963         split_cyc
-00005750: 6c65 2e64 6973 706c 6179 286d 6729 0a20  le.display(mg). 
-00005760: 2020 2020 2020 2073 706c 6974 5f63 7963         split_cyc
-00005770: 6c65 2e64 6973 706c 6179 286d 672c 2061  le.display(mg, a
-00005780: 6c67 6f72 6974 686d 3d27 6261 7369 6327  lgorithm='basic'
-00005790: 290a 2020 2020 2020 2020 7370 6c69 745f  ).        split_
-000057a0: 6379 636c 652e 6469 7370 6c61 7928 6d67  cycle.display(mg
-000057b0: 2c20 616c 676f 7269 7468 6d3d 2766 6c6f  , algorithm='flo
-000057c0: 7964 5f77 6172 7368 616c 6c27 290a 2020  yd_warshall').  
-000057d0: 2020 2222 220a 2020 2020 0a20 2020 2069    """.    .    i
-000057e0: 6620 616c 676f 7269 7468 6d20 3d3d 2027  f algorithm == '
-000057f0: 6261 7369 6327 3a0a 2020 2020 2020 2020  basic':.        
-00005800: 7265 7475 726e 205f 7370 6c69 745f 6379  return _split_cy
-00005810: 636c 655f 6261 7369 6328 6564 6174 612c  cle_basic(edata,
-00005820: 2063 7572 725f 6361 6e64 7320 3d20 6375   curr_cands = cu
-00005830: 7272 5f63 616e 6473 2c20 7374 7265 6e67  rr_cands, streng
-00005840: 7468 5f66 756e 6374 696f 6e20 3d20 7374  th_function = st
-00005850: 7265 6e67 7468 5f66 756e 6374 696f 6e29  rength_function)
-00005860: 0a20 2020 2065 6c69 6620 616c 676f 7269  .    elif algori
-00005870: 7468 6d20 3d3d 2027 666c 6f79 645f 7761  thm == 'floyd_wa
-00005880: 7273 6861 6c6c 273a 0a20 2020 2020 2020  rshall':.       
-00005890: 2072 6574 7572 6e20 5f73 706c 6974 5f63   return _split_c
-000058a0: 7963 6c65 5f66 6c6f 7964 5f77 6172 7368  ycle_floyd_warsh
-000058b0: 616c 6c28 6564 6174 612c 2063 7572 725f  all(edata, curr_
-000058c0: 6361 6e64 7320 3d20 6375 7272 5f63 616e  cands = curr_can
-000058d0: 6473 2c20 7374 7265 6e67 7468 5f66 756e  ds, strength_fun
-000058e0: 6374 696f 6e20 3d20 7374 7265 6e67 7468  ction = strength
-000058f0: 5f66 756e 6374 696f 6e29 0a20 2020 2065  _function).    e
-00005900: 6c73 653a 0a20 2020 2020 2020 2072 6169  lse:.        rai
-00005910: 7365 2056 616c 7565 4572 726f 7228 2249  se ValueError("I
-00005920: 6e76 616c 6964 2061 6c67 6f72 6974 686d  nvalid algorithm
-00005930: 2073 7065 6369 6669 6564 2e22 290a 0a0a   specified.")...
-00005940: 6465 6620 7370 6c69 745f 6379 636c 655f  def split_cycle_
-00005950: 6465 6665 6174 2865 6461 7461 2c20 6375  defeat(edata, cu
-00005960: 7272 5f63 616e 6473 203d 204e 6f6e 652c  rr_cands = None,
-00005970: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
-00005980: 6f6e 203d 204e 6f6e 6529 3a20 2020 0a20  on = None):   . 
-00005990: 2020 2022 2222 0a20 2020 2052 6574 7572     """.    Retur
-000059a0: 6e73 2074 6865 2053 706c 6974 2043 7963  ns the Split Cyc
-000059b0: 6c65 2064 6566 6561 7420 7265 6c61 7469  le defeat relati
-000059c0: 6f6e 2e20 0a0a 2020 2020 5365 6520 6874  on. ..    See ht
-000059d0: 7470 733a 2f2f 6172 7869 762e 6f72 672f  tps://arxiv.org/
-000059e0: 6162 732f 3230 3038 2e30 3834 3531 2066  abs/2008.08451 f
-000059f0: 6f72 2061 6e20 6578 7465 6e64 6564 2064  or an extended d
-00005a00: 6973 6375 7373 696f 6e20 6f66 2074 6869  iscussion of thi
-00005a10: 7320 6e6f 7469 6f6e 206f 6620 6465 6665  s notion of defe
-00005a20: 6174 2069 6e20 616e 2065 6c65 6374 696f  at in an electio
-00005a30: 6e2e 200a 0a20 2020 2041 7267 733a 0a20  n. ..    Args:. 
-00005a40: 2020 2020 2020 2065 6461 7461 2028 5072         edata (Pr
-00005a50: 6f66 696c 652c 2050 726f 6669 6c65 5769  ofile, ProfileWi
-00005a60: 7468 5469 6573 2c20 4d61 7267 696e 4772  thTies, MarginGr
-00005a70: 6170 6829 3a20 416e 7920 656c 6563 7469  aph): Any electi
-00005a80: 6f6e 2064 6174 6120 7468 6174 2068 6173  on data that has
-00005a90: 2061 2060 6d61 7267 696e 6020 6d65 7468   a `margin` meth
-00005aa0: 6f64 2e20 0a20 2020 2020 2020 2063 7572  od. .        cur
-00005ab0: 725f 6361 6e64 7320 284c 6973 745b 696e  r_cands (List[in
-00005ac0: 745d 2c20 6f70 7469 6f6e 616c 293a 2049  t], optional): I
-00005ad0: 6620 7365 742c 2074 6865 6e20 6669 6e64  f set, then find
-00005ae0: 2074 6865 2077 696e 6e65 7273 2066 6f72   the winners for
-00005af0: 2074 6865 2070 726f 6669 6c65 2072 6573   the profile res
-00005b00: 7472 6963 7465 6420 746f 2074 6865 2063  tricted to the c
-00005b10: 616e 6469 6461 7465 7320 696e 2060 6063  andidates in ``c
-00005b20: 7572 725f 6361 6e64 7360 600a 0a20 2020  urr_cands``..   
-00005b30: 2052 6574 7572 6e73 3a20 0a20 2020 2020   Returns: .     
-00005b40: 2020 2041 206e 6574 776f 726b 7820 4469     A networkx Di
-00005b50: 4772 6170 6820 7265 7072 6573 656e 7469  Graph representi
-00005b60: 6e67 2074 6865 2053 706c 6974 2043 7963  ng the Split Cyc
-00005b70: 6c65 2064 6566 6561 7420 7265 6c61 7469  le defeat relati
-00005b80: 6f6e 2e20 0a0a 2020 2020 2e2e 2073 6565  on. ..    .. see
-00005b90: 616c 736f 3a3a 0a0a 2020 2020 2020 2020  also::..        
-00005ba0: 3a6d 6574 683a 6070 7265 665f 766f 7469  :meth:`pref_voti
-00005bb0: 6e67 2e6d 6172 6769 6e5f 6261 7365 645f  ng.margin_based_
-00005bc0: 6d65 7468 6f64 732e 7370 6c69 745f 6379  methods.split_cy
-00005bd0: 636c 6560 2c20 3a6d 6574 683a 6070 7265  cle`, :meth:`pre
-00005be0: 665f 766f 7469 6e67 2e6d 6172 6769 6e5f  f_voting.margin_
-00005bf0: 6261 7365 645f 6d65 7468 6f64 732e 7370  based_methods.sp
-00005c00: 6c69 745f 6379 636c 655f 466c 6f79 645f  lit_cycle_Floyd_
-00005c10: 5761 7273 6861 6c6c 600a 0a20 2020 203a  Warshall`..    :
-00005c20: 4578 616d 706c 653a 200a 0a20 2020 202e  Example: ..    .
-00005c30: 2e20 706c 6f74 3a3a 2020 6d61 7267 696e  . plot::  margin
-00005c40: 5f67 7261 7068 735f 6578 616d 706c 6573  _graphs_examples
-00005c50: 2f6d 675f 6578 5f73 635f 6465 6665 6174  /mg_ex_sc_defeat
-00005c60: 2e70 790a 2020 2020 2020 2020 3a63 6f6e  .py.        :con
-00005c70: 7465 7874 3a20 7265 7365 7420 200a 2020  text: reset  .  
-00005c80: 2020 2020 2020 3a69 6e63 6c75 6465 2d73        :include-s
-00005c90: 6f75 7263 653a 2054 7275 650a 0a20 2020  ource: True..   
-00005ca0: 2022 2222 0a0a 2020 2020 6361 6e64 6964   """..    candid
-00005cb0: 6174 6573 203d 2065 6461 7461 2e63 616e  ates = edata.can
-00005cc0: 6469 6461 7465 7320 6966 2063 7572 725f  didates if curr_
-00005cd0: 6361 6e64 7320 6973 204e 6f6e 6520 656c  cands is None el
-00005ce0: 7365 2063 7572 725f 6361 6e64 7320 2020  se curr_cands   
-00005cf0: 200a 2020 2020 7374 7265 6e67 7468 5f66   .    strength_f
-00005d00: 756e 6374 696f 6e20 3d20 6564 6174 612e  unction = edata.
-00005d10: 6d61 7267 696e 2069 6620 7374 7265 6e67  margin if streng
-00005d20: 7468 5f66 756e 6374 696f 6e20 6973 204e  th_function is N
-00005d30: 6f6e 6520 656c 7365 2073 7472 656e 6774  one else strengt
-00005d40: 685f 6675 6e63 7469 6f6e 200a 200a 2020  h_function . .  
-00005d50: 2020 7765 616b 5f63 6f6e 646f 7263 6574    weak_condorcet
-00005d60: 5f77 696e 6e65 7273 203d 207b 633a 5472  _winners = {c:Tr
-00005d70: 7565 2066 6f72 2063 2069 6e20 6361 6e64  ue for c in cand
-00005d80: 6964 6174 6573 7d0a 2020 2020 735f 6d61  idates}.    s_ma
-00005d90: 7472 6978 203d 205b 5b2d 6e70 2e69 6e66  trix = [[-np.inf
-00005da0: 2066 6f72 205f 2069 6e20 6361 6e64 6964   for _ in candid
-00005db0: 6174 6573 5d20 666f 7220 5f20 696e 2063  ates] for _ in c
-00005dc0: 616e 6469 6461 7465 735d 0a20 2020 200a  andidates].    .
-00005dd0: 2020 2020 2320 696e 6974 6961 6c69 7a65      # initialize
-00005de0: 2074 6865 2073 5f6d 6174 7269 780a 2020   the s_matrix.  
-00005df0: 2020 666f 7220 6331 5f69 6478 2c20 6331    for c1_idx, c1
-00005e00: 2069 6e20 656e 756d 6572 6174 6528 6361   in enumerate(ca
-00005e10: 6e64 6964 6174 6573 293a 0a20 2020 2020  ndidates):.     
-00005e20: 2020 2066 6f72 2063 325f 6964 782c 2063     for c2_idx, c
-00005e30: 3220 696e 2065 6e75 6d65 7261 7465 2863  2 in enumerate(c
-00005e40: 616e 6469 6461 7465 7329 3a0a 2020 2020  andidates):.    
-00005e50: 2020 2020 2020 2020 6966 2028 6564 6174          if (edat
-00005e60: 612e 6d61 6a6f 7269 7479 5f70 7265 6665  a.majority_prefe
-00005e70: 7273 2863 312c 2063 3229 206f 7220 6331  rs(c1, c2) or c1
-00005e80: 203d 3d20 6332 293a 0a20 2020 2020 2020   == c2):.       
-00005e90: 2020 2020 2020 2020 2073 5f6d 6174 7269           s_matri
-00005ea0: 785b 6331 5f69 6478 5d5b 6332 5f69 6478  x[c1_idx][c2_idx
-00005eb0: 5d20 3d20 7374 7265 6e67 7468 5f66 756e  ] = strength_fun
-00005ec0: 6374 696f 6e28 6331 2c20 6332 2920 0a20  ction(c1, c2) . 
-00005ed0: 2020 2020 2020 2020 2020 2020 2020 2077                 w
-00005ee0: 6561 6b5f 636f 6e64 6f72 6365 745f 7769  eak_condorcet_wi
-00005ef0: 6e6e 6572 735b 6332 5d20 3d20 7765 616b  nners[c2] = weak
-00005f00: 5f63 6f6e 646f 7263 6574 5f77 696e 6e65  _condorcet_winne
-00005f10: 7273 5b63 325d 2061 6e64 2028 6331 203d  rs[c2] and (c1 =
-00005f20: 3d20 6332 2920 2320 7765 616b 2043 6f6e  = c2) # weak Con
-00005f30: 646f 7263 6574 2077 696e 6e65 7273 2061  dorcet winners a
-00005f40: 7265 2053 706c 6974 2043 7963 6c65 2077  re Split Cycle w
-00005f50: 696e 6e65 7273 0a20 2020 200a 2020 2020  inners.    .    
-00005f60: 7374 7265 6e67 7468 203d 206c 6973 7428  strength = list(
-00005f70: 6d61 7028 6c61 6d62 6461 2069 203a 206c  map(lambda i : l
-00005f80: 6973 7428 6d61 7028 6c61 6d62 6461 206a  ist(map(lambda j
-00005f90: 203a 206a 202c 2069 2929 202c 2073 5f6d   : j , i)) , s_m
-00005fa0: 6174 7269 7829 290a 2020 2020 666f 7220  atrix)).    for 
-00005fb0: 695f 6964 782c 2069 2069 6e20 656e 756d  i_idx, i in enum
-00005fc0: 6572 6174 6528 6361 6e64 6964 6174 6573  erate(candidates
-00005fd0: 293a 200a 2020 2020 2020 2020 666f 7220  ): .        for 
-00005fe0: 6a5f 6964 782c 206a 2069 6e20 656e 756d  j_idx, j in enum
-00005ff0: 6572 6174 6528 6361 6e64 6964 6174 6573  erate(candidates
-00006000: 293a 0a20 2020 2020 2020 2020 2020 2069  ):.            i
-00006010: 6620 6921 3d20 6a3a 0a20 2020 2020 2020  f i!= j:.       
-00006020: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
-00006030: 7765 616b 5f63 6f6e 646f 7263 6574 5f77  weak_condorcet_w
-00006040: 696e 6e65 7273 5b6a 5d3a 2023 2077 6561  inners[j]: # wea
-00006050: 6b20 436f 6e64 6f72 6365 7420 7769 6e6e  k Condorcet winn
-00006060: 6572 7320 6172 6520 5370 6c69 7420 4379  ers are Split Cy
-00006070: 636c 6520 7769 6e6e 6572 730a 2020 2020  cle winners.    
-00006080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006090: 666f 7220 6b5f 6964 782c 206b 2069 6e20  for k_idx, k in 
-000060a0: 656e 756d 6572 6174 6528 6361 6e64 6964  enumerate(candid
-000060b0: 6174 6573 293a 200a 2020 2020 2020 2020  ates): .        
-000060c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000060d0: 6966 2069 2021 3d20 6b20 616e 6420 6a20  if i != k and j 
-000060e0: 213d 206b 3a0a 2020 2020 2020 2020 2020  != k:.          
-000060f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006100: 2020 7374 7265 6e67 7468 5b6a 5f69 6478    strength[j_idx
-00006110: 5d5b 6b5f 6964 785d 203d 206d 6178 2873  ][k_idx] = max(s
-00006120: 7472 656e 6774 685b 6a5f 6964 785d 5b6b  trength[j_idx][k
-00006130: 5f69 6478 5d2c 206d 696e 2873 7472 656e  _idx], min(stren
-00006140: 6774 685b 6a5f 6964 785d 5b69 5f69 6478  gth[j_idx][i_idx
-00006150: 5d2c 7374 7265 6e67 7468 5b69 5f69 6478  ],strength[i_idx
-00006160: 5d5b 6b5f 6964 785d 2929 0a20 0a20 2020  ][k_idx])). .   
-00006170: 2064 6566 6561 745f 6772 6170 6820 3d20   defeat_graph = 
-00006180: 6e78 2e44 6947 7261 7068 2829 0a20 2020  nx.DiGraph().   
-00006190: 2064 6566 6561 745f 6772 6170 682e 6164   defeat_graph.ad
-000061a0: 645f 6e6f 6465 735f 6672 6f6d 2863 616e  d_nodes_from(can
-000061b0: 6469 6461 7465 7329 0a0a 2020 2020 666f  didates)..    fo
-000061c0: 7220 695f 6964 782c 2069 2069 6e20 656e  r i_idx, i in en
-000061d0: 756d 6572 6174 6528 6361 6e64 6964 6174  umerate(candidat
-000061e0: 6573 293a 0a20 2020 2020 2020 2066 6f72  es):.        for
-000061f0: 206a 5f69 6478 2c20 6a20 696e 2065 6e75   j_idx, j in enu
-00006200: 6d65 7261 7465 2863 616e 6469 6461 7465  merate(candidate
-00006210: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
-00006220: 6966 2069 2021 3d20 6a3a 0a20 2020 2020  if i != j:.     
-00006230: 2020 2020 2020 2020 2020 2069 6620 735f             if s_
-00006240: 6d61 7472 6978 5b6a 5f69 6478 5d5b 695f  matrix[j_idx][i_
-00006250: 6964 785d 203e 2073 7472 656e 6774 685b  idx] > strength[
-00006260: 695f 6964 785d 5b6a 5f69 6478 5d3a 2023  i_idx][j_idx]: #
-00006270: 2074 6865 206d 6169 6e20 6469 6666 6572   the main differ
-00006280: 656e 6365 2077 6974 6820 4265 6174 2050  ence with Beat P
-00006290: 6174 680a 2020 2020 2020 2020 2020 2020  ath.            
-000062a0: 2020 2020 2020 2020 6465 6665 6174 5f67          defeat_g
-000062b0: 7261 7068 2e61 6464 5f77 6569 6768 7465  raph.add_weighte
-000062c0: 645f 6564 6765 735f 6672 6f6d 285b 286a  d_edges_from([(j
-000062d0: 2c69 2c73 5f6d 6174 7269 785b 6a5f 6964  ,i,s_matrix[j_id
-000062e0: 785d 5b69 5f69 6478 5d29 5d29 0a20 2020  x][i_idx])]).   
-000062f0: 2020 2020 2020 2020 2020 2020 200a 2020               .  
-00006300: 2020 7265 7475 726e 2064 6566 6561 745f    return defeat_
-00006310: 6772 6170 680a 0a0a 2320 666c 6174 7465  graph...# flatte
-00006320: 6e20 6120 3264 206c 6973 7420 2d20 7475  n a 2d list - tu
-00006330: 726e 2061 2032 6420 6c69 7374 2069 6e74  rn a 2d list int
-00006340: 6f20 6120 7369 6e67 6c65 206c 6973 7420  o a single list 
-00006350: 6f66 2069 7465 6d73 0a66 6c61 7474 656e  of items.flatten
-00006360: 203d 206c 616d 6264 6120 6c3a 205b 6974   = lambda l: [it
-00006370: 656d 2066 6f72 2073 7562 6c69 7374 2069  em for sublist i
-00006380: 6e20 6c20 666f 7220 6974 656d 2069 6e20  n l for item in 
-00006390: 7375 626c 6973 745d 0a0a 6465 6620 646f  sublist]..def do
-000063a0: 6573 5f63 7265 6174 655f 6379 636c 6528  es_create_cycle(
-000063b0: 672c 2065 6467 6529 3a0a 2020 2020 2727  g, edge):.    ''
-000063c0: 2772 6574 7572 6e20 5472 7565 2069 6620  'return True if 
-000063d0: 6164 6469 6e67 2074 6865 2065 6467 6520  adding the edge 
-000063e0: 746f 2067 2063 7265 6174 6520 6120 6379  to g create a cy
-000063f0: 636c 652e 0a20 2020 2069 7420 6973 2061  cle..    it is a
-00006400: 7373 756d 6564 2074 6861 7420 6564 6765  ssumed that edge
-00006410: 2069 7320 616c 7265 6164 7920 696e 2067   is already in g
-00006420: 2727 270a 2020 2020 736f 7572 6365 203d  '''.    source =
-00006430: 2065 6467 655b 305d 0a20 2020 2074 6172   edge[0].    tar
-00006440: 6765 7420 3d20 6564 6765 5b31 5d0a 2020  get = edge[1].  
-00006450: 2020 666f 7220 6e20 696e 2067 2e70 7265    for n in g.pre
-00006460: 6465 6365 7373 6f72 7328 736f 7572 6365  decessors(source
-00006470: 293a 0a20 2020 2020 2020 2069 6620 6e78  ):.        if nx
-00006480: 2e68 6173 5f70 6174 6828 672c 2074 6172  .has_path(g, tar
-00006490: 6765 742c 206e 293a 200a 2020 2020 2020  get, n): .      
-000064a0: 2020 2020 2020 7265 7475 726e 2054 7275        return Tru
-000064b0: 650a 2020 2020 7265 7475 726e 2046 616c  e.    return Fal
-000064c0: 7365 0a0a 0a0a 6465 6620 706f 7765 7273  se....def powers
-000064d0: 6574 2869 7465 7261 626c 6529 3a0a 2020  et(iterable):.  
-000064e0: 2020 2222 220a 2020 2020 5265 7475 726e    """.    Return
-000064f0: 2074 6865 2070 6f77 6572 7365 7420 6f66   the powerset of
-00006500: 2060 6069 7465 7261 626c 6560 600a 0a20   ``iterable``.. 
-00006510: 2020 2070 6f77 6572 7365 7428 5b31 2c32     powerset([1,2
-00006520: 2c33 5d29 202d 2d3e 2028 2920 2831 2c29  ,3]) --> () (1,)
-00006530: 2028 322c 2920 2833 2c29 2028 312c 3229   (2,) (3,) (1,2)
-00006540: 2028 312c 3329 2028 322c 3329 2028 312c   (1,3) (2,3) (1,
-00006550: 322c 3329 0a20 2020 2022 2222 0a20 2020  2,3).    """.   
-00006560: 2073 203d 206c 6973 7428 6974 6572 6162   s = list(iterab
-00006570: 6c65 290a 2020 2020 7265 7475 726e 2063  le).    return c
-00006580: 6861 696e 2e66 726f 6d5f 6974 6572 6162  hain.from_iterab
-00006590: 6c65 2863 6f6d 6269 6e61 7469 6f6e 7328  le(combinations(
-000065a0: 732c 2072 2920 666f 7220 7220 696e 2072  s, r) for r in r
-000065b0: 616e 6765 286c 656e 2873 292b 3129 290a  ange(len(s)+1)).
-000065c0: 0a0a 6465 6620 6973 5f73 7461 636b 2865  ..def is_stack(e
-000065d0: 6461 7461 2c20 6361 6e64 5f6c 6973 742c  data, cand_list,
-000065e0: 2063 7572 725f 6361 6e64 733d 4e6f 6e65   curr_cands=None
-000065f0: 293a 200a 2020 2020 2222 220a 2020 2020  ): .    """.    
-00006600: 4120 2a2a 7374 6163 6b2a 2a20 6973 2061  A **stack** is a
-00006610: 206c 696e 6561 7220 6f72 6465 7220 3a6d   linear order :m
-00006620: 6174 683a 604c 6020 6f6e 2074 6865 2063  ath:`L` on the c
-00006630: 616e 6469 6461 7465 2073 7563 6820 7468  andidate such th
-00006640: 6174 2066 6f72 2061 6c6c 2063 616e 6469  at for all candi
-00006650: 6461 7465 7320 3a6d 6174 683a 6061 6020  dates :math:`a` 
-00006660: 616e 6420 3a6d 6174 683a 6062 602c 2069  and :math:`b`, i
-00006670: 6620 3a6d 6174 683a 6061 4c62 602c 2074  f :math:`aLb`, t
-00006680: 6865 6e20 7468 6572 6520 6172 6520 6469  hen there are di
-00006690: 7374 696e 6374 2063 616e 6469 6461 7465  stinct candidate
-000066a0: 7320 3a6d 6174 683a 6078 5f31 2c5c 646f  s :math:`x_1,\do
-000066b0: 7473 2c78 5f6e 6020 7769 7468 203a 6d61  ts,x_n` with :ma
-000066c0: 7468 3a60 785f 313d 6160 2061 6e64 203a  th:`x_1=a` and :
-000066d0: 6d61 7468 3a60 785f 6e3d 6260 2073 7563  math:`x_n=b` suc
-000066e0: 6820 7468 6174 203a 6d61 7468 3a60 785f  h that :math:`x_
-000066f0: 6920 4c20 785f 7b69 2b31 7d60 2061 6e64  i L x_{i+1}` and
-00006700: 2066 6f72 2061 6c6c 203a 6d61 7468 3a60   for all :math:`
-00006710: 695c 696e 205c 7b31 2c5c 646f 7473 2c20  i\in \{1,\dots, 
-00006720: 6e2d 315c 7d60 2c20 7468 6520 6d61 7267  n-1\}`, the marg
-00006730: 696e 206f 6620 3a6d 6174 683a 6078 5f31  in of :math:`x_1
-00006740: 6020 6f76 6572 203a 6d61 7468 3a60 785f  ` over :math:`x_
-00006750: 7b69 2b31 7d60 2069 7320 6772 6561 7465  {i+1}` is greate
-00006760: 7220 7468 616e 206f 7220 6571 7561 6c20  r than or equal 
-00006770: 746f 2074 6865 206d 6172 6769 6e20 6f66  to the margin of
-00006780: 203a 6d61 7468 3a60 6260 206f 7665 7220   :math:`b` over 
-00006790: 3a6d 6174 683a 6061 602e 0a0a 2020 2020  :math:`a`...    
-000067a0: 5468 6973 2064 6566 696e 6974 696f 6e20  This definition 
-000067b0: 6973 2064 7565 2074 6f20 5a61 7669 7374  is due to Zavist
-000067c0: 2061 6e64 2054 6964 656d 616e 2031 3938   and Tideman 198
-000067d0: 392c 2061 6e64 2069 7320 7573 6564 2061  9, and is used a
-000067e0: 7320 616e 2061 6c74 6572 6e61 7469 7665  s an alternative
-000067f0: 2063 6861 7261 6374 6572 697a 6174 696f   characterizatio
-00006800: 6e20 6f66 2052 616e 6b65 6420 5061 6972  n of Ranked Pair
-00006810: 733a 203a 6d61 7468 3a60 6160 2069 7320  s: :math:`a` is 
-00006820: 6120 5261 6e6b 6564 2050 6169 7273 2077  a Ranked Pairs w
-00006830: 696e 6e65 7220 6966 2061 6e64 206f 6e6c  inner if and onl
-00006840: 7920 6966 203a 6d61 7468 3a60 6160 2069  y if :math:`a` i
-00006850: 7320 7468 6520 6d61 7869 6d75 6d20 656c  s the maximum el
-00006860: 656d 656e 7420 6f66 2073 6f6d 6520 7374  ement of some st
-00006870: 6163 6b2e 200a 0a20 2020 2041 7267 733a  ack. ..    Args:
-00006880: 0a20 2020 2020 2020 2065 6461 7461 2028  .        edata (
-00006890: 5072 6f66 696c 652c 2050 726f 6669 6c65  Profile, Profile
-000068a0: 5769 7468 5469 6573 2c20 4d61 7267 696e  WithTies, Margin
-000068b0: 4772 6170 6829 3a20 416e 7920 656c 6563  Graph): Any elec
-000068c0: 7469 6f6e 2064 6174 6120 7468 6174 2068  tion data that h
-000068d0: 6173 2061 2060 6d61 7267 696e 6020 6d65  as a `margin` me
-000068e0: 7468 6f64 2e20 0a20 2020 2020 2020 2063  thod. .        c
-000068f0: 616e 645f 6c69 7374 2028 6c69 7374 293a  and_list (list):
-00006900: 2054 6865 206c 6973 7420 6f66 2063 616e   The list of can
-00006910: 6469 6461 7465 7320 7468 6174 206d 6179  didates that may
-00006920: 2062 6520 6120 7374 6163 6b0a 2020 2020   be a stack.    
-00006930: 2020 2020 6375 7272 5f63 616e 6473 2028      curr_cands (
-00006940: 4c69 7374 5b69 6e74 5d2c 206f 7074 696f  List[int], optio
-00006950: 6e61 6c29 3a20 4966 2073 6574 2c20 7468  nal): If set, th
-00006960: 656e 2066 696e 6420 7468 6520 7769 6e6e  en find the winn
-00006970: 6572 7320 666f 7220 7468 6520 7072 6f66  ers for the prof
-00006980: 696c 6520 7265 7374 7269 6374 6564 2074  ile restricted t
-00006990: 6f20 7468 6520 6361 6e64 6964 6174 6573  o the candidates
-000069a0: 2069 6e20 6060 6375 7272 5f63 616e 6473   in ``curr_cands
-000069b0: 6060 0a0a 2020 2020 5265 7475 726e 733a  ``..    Returns:
-000069c0: 200a 2020 2020 2020 2020 5472 7565 2069   .        True i
-000069d0: 6620 6060 6361 6e64 5f6c 6973 7460 6020  f ``cand_list`` 
-000069e0: 6973 2061 2073 7461 636b 2061 6e64 2046  is a stack and F
-000069f0: 616c 7365 206f 7468 6572 7769 7365 0a0a  alse otherwise..
-00006a00: 2020 2020 3a45 7861 6d70 6c65 3a20 0a20      :Example: . 
-00006a10: 2020 200a 2020 2020 2e2e 2070 6c6f 743a     .    .. plot:
-00006a20: 3a20 206d 6172 6769 6e5f 6772 6170 6873  :  margin_graphs
-00006a30: 5f65 7861 6d70 6c65 732f 6d67 5f65 785f  _examples/mg_ex_
-00006a40: 7270 5f73 7461 636b 732e 7079 0a20 2020  rp_stacks.py.   
-00006a50: 2020 2020 203a 636f 6e74 6578 743a 2072       :context: r
-00006a60: 6573 6574 2020 0a20 2020 2020 2020 203a  eset  .        :
-00006a70: 696e 636c 7564 652d 736f 7572 6365 3a20  include-source: 
-00006a80: 5472 7565 0a0a 0a20 2020 202e 2e20 6578  True...    .. ex
-00006a90: 6563 5f63 6f64 653a 3a0a 2020 2020 2020  ec_code::.      
-00006aa0: 2020 0a20 2020 2020 2020 2066 726f 6d20    .        from 
-00006ab0: 7072 6566 5f76 6f74 696e 672e 7765 6967  pref_voting.weig
-00006ac0: 6874 6564 5f6d 616a 6f72 6974 795f 6772  hted_majority_gr
-00006ad0: 6170 6873 2069 6d70 6f72 7420 4d61 7267  aphs import Marg
-00006ae0: 696e 4772 6170 680a 2020 2020 2020 2020  inGraph.        
-00006af0: 6672 6f6d 2070 7265 665f 766f 7469 6e67  from pref_voting
-00006b00: 2e6d 6172 6769 6e5f 6261 7365 645f 6d65  .margin_based_me
-00006b10: 7468 6f64 7320 696d 706f 7274 2069 735f  thods import is_
-00006b20: 7374 6163 6b0a 2020 2020 2020 2020 6672  stack.        fr
-00006b30: 6f6d 2069 7465 7274 6f6f 6c73 2069 6d70  om itertools imp
-00006b40: 6f72 7420 7065 726d 7574 6174 696f 6e73  ort permutations
-00006b50: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00006b60: 2020 6d67 203d 204d 6172 6769 6e47 7261    mg = MarginGra
-00006b70: 7068 285b 302c 2031 2c20 325d 2c20 5b28  ph([0, 1, 2], [(
-00006b80: 302c 2031 2c20 3229 2c20 2831 2c20 322c  0, 1, 2), (1, 2,
-00006b90: 2034 292c 2028 322c 2030 2c20 3229 5d29   4), (2, 0, 2)])
-00006ba0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00006bb0: 2020 666f 7220 636c 6973 7420 696e 2070    for clist in p
-00006bc0: 6572 6d75 7461 7469 6f6e 7328 6d67 2e63  ermutations(mg.c
-00006bd0: 616e 6469 6461 7465 7329 3a20 0a20 2020  andidates): .   
-00006be0: 2020 2020 2020 2020 2070 7269 6e74 2866           print(f
-00006bf0: 227b 636c 6973 747d 207b 2769 7327 2069  "{clist} {'is' i
-00006c00: 6620 6973 5f73 7461 636b 286d 672c 2063  f is_stack(mg, c
-00006c10: 6c69 7374 2920 656c 7365 2027 6973 206e  list) else 'is n
-00006c20: 6f74 277d 2061 2073 7461 636b 2229 0a20  ot'} a stack"). 
-00006c30: 2020 2020 2020 2020 2020 200a 2020 2020             .    
-00006c40: 2222 220a 2020 2020 0a20 2020 2063 616e  """.    .    can
-00006c50: 6469 6461 7465 7320 3d20 6375 7272 5f63  didates = curr_c
-00006c60: 616e 6473 2069 6620 6375 7272 5f63 616e  ands if curr_can
-00006c70: 6473 2069 7320 6e6f 7420 4e6f 6e65 2065  ds is not None e
-00006c80: 6c73 6520 6564 6174 612e 6361 6e64 6964  lse edata.candid
-00006c90: 6174 6573 0a20 2020 2063 616e 645f 7061  ates.    cand_pa
-00006ca0: 6972 7320 3d20 5b28 612c 2062 2920 6966  irs = [(a, b) if
-00006cb0: 2063 616e 645f 6c69 7374 2e69 6e64 6578   cand_list.index
-00006cc0: 2861 2920 3c20 6361 6e64 5f6c 6973 742e  (a) < cand_list.
-00006cd0: 696e 6465 7828 6229 2065 6c73 6520 2862  index(b) else (b
-00006ce0: 2c20 6129 2066 6f72 2061 2c20 6220 696e  , a) for a, b in
-00006cf0: 2063 6f6d 6269 6e61 7469 6f6e 7328 6361   combinations(ca
-00006d00: 6e64 6964 6174 6573 2c20 3229 5d0a 2020  ndidates, 2)].  
-00006d10: 2020 2020 2020 0a20 2020 2066 6f72 2061        .    for a
-00006d20: 2c20 6220 696e 2063 616e 645f 7061 6972  , b in cand_pair
-00006d30: 733a 0a20 2020 2020 2020 206f 7468 6572  s:.        other
-00006d40: 5f63 616e 6473 203d 205b 6320 666f 7220  _cands = [c for 
-00006d50: 6320 696e 2063 616e 6469 6461 7465 7320  c in candidates 
-00006d60: 6966 2063 2021 3d20 6120 616e 6420 6320  if c != a and c 
-00006d70: 213d 2062 5d0a 2020 2020 2020 2020 666f  != b].        fo
-00006d80: 756e 645f 7061 7468 203d 2046 616c 7365  und_path = False
-00006d90: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00006da0: 2020 7375 626c 6973 7420 3d20 6361 6e64    sublist = cand
-00006db0: 5f6c 6973 745b 6361 6e64 5f6c 6973 742e  _list[cand_list.
-00006dc0: 696e 6465 7828 6129 202b 2031 3a63 616e  index(a) + 1:can
-00006dd0: 645f 6c69 7374 2e69 6e64 6578 2862 295d  d_list.index(b)]
-00006de0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00006df0: 2020 666f 7220 696e 6469 6365 7320 696e    for indices in
-00006e00: 2070 6f77 6572 7365 7428 7261 6e67 6528   powerset(range(
-00006e10: 6c65 6e28 7375 626c 6973 7429 2929 3a20  len(sublist))): 
-00006e20: 0a20 2020 2020 2020 2020 2020 200a 2020  .            .  
-00006e30: 2020 2020 2020 2020 2020 7061 7468 203d            path =
-00006e40: 205b 615d 202b 205b 7375 626c 6973 745b   [a] + [sublist[
-00006e50: 695d 2066 6f72 2069 2069 6e20 736f 7274  i] for i in sort
-00006e60: 6564 2869 6e64 6963 6573 295d 202b 205b  ed(indices)] + [
-00006e70: 625d 0a20 2020 2020 2020 2020 2020 206d  b].            m
-00006e80: 6172 6769 6e73 203d 205b 6564 6174 612e  argins = [edata.
-00006e90: 6d61 7267 696e 2878 692c 2070 6174 685b  margin(xi, path[
-00006ea0: 6920 2b20 315d 2920 666f 7220 692c 2078  i + 1]) for i, x
-00006eb0: 6920 696e 2065 6e75 6d65 7261 7465 2870  i in enumerate(p
-00006ec0: 6174 685b 303a 2d31 5d29 5d0a 2020 2020  ath[0:-1])].    
-00006ed0: 2020 2020 2020 2020 6966 2061 6c6c 285b          if all([
-00006ee0: 6361 6e64 5f6c 6973 742e 696e 6465 7828  cand_list.index(
-00006ef0: 7869 2920 3c20 6361 6e64 5f6c 6973 742e  xi) < cand_list.
-00006f00: 696e 6465 7828 7061 7468 5b69 2b31 5d29  index(path[i+1])
-00006f10: 2066 6f72 2069 2c20 7869 2069 6e20 656e   for i, xi in en
-00006f20: 756d 6572 6174 6528 7061 7468 5b30 3a2d  umerate(path[0:-
-00006f30: 315d 295d 2920 616e 6420 616c 6c28 5b6d  1])]) and all([m
-00006f40: 203e 3d20 6564 6174 612e 6d61 7267 696e   >= edata.margin
-00006f50: 2862 2c20 6129 2066 6f72 206d 2069 6e20  (b, a) for m in 
-00006f60: 6d61 7267 696e 735d 293a 200a 2020 2020  margins]): .    
-00006f70: 2020 2020 2020 2020 2020 2020 666f 756e              foun
-00006f80: 645f 7061 7468 203d 2054 7275 650a 2020  d_path = True.  
-00006f90: 2020 2020 2020 2020 2020 2020 2020 6272                br
-00006fa0: 6561 6b0a 2020 2020 2020 2020 6966 206e  eak.        if n
-00006fb0: 6f74 2066 6f75 6e64 5f70 6174 683a 200a  ot found_path: .
-00006fc0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00006fd0: 726e 2046 616c 7365 0a20 2020 2072 6574  rn False.    ret
-00006fe0: 7572 6e20 5472 7565 0a0a 6465 6620 5f72  urn True..def _r
-00006ff0: 616e 6b65 645f 7061 6972 735f 6672 6f6d  anked_pairs_from
-00007000: 5f73 7461 636b 7328 6564 6174 612c 2063  _stacks(edata, c
-00007010: 7572 725f 6361 6e64 7320 3d20 4e6f 6e65  urr_cands = None
-00007020: 293a 200a 2020 2020 2222 2246 696e 6420  ): .    """Find 
-00007030: 7468 6520 5261 6e6b 6564 2050 6169 7273  the Ranked Pairs
-00007040: 2077 696e 6e65 7273 2062 7920 6974 6572   winners by iter
-00007050: 6174 696e 6720 6f76 6572 2061 6c6c 2070  ating over all p
-00007060: 6572 6d75 7461 7469 6f6e 7320 6f66 2063  ermutations of c
-00007070: 616e 6469 6461 7465 7320 2872 6573 7472  andidates (restr
-00007080: 6963 7465 6420 746f 2060 6063 7572 725f  icted to ``curr_
-00007090: 6361 6e64 7360 6020 6966 206e 6f74 204e  cands`` if not N
-000070a0: 6f6e 6529 2c20 616e 6420 6368 6563 6b69  one), and checki
-000070b0: 6e67 2069 6620 7468 6520 6c69 7374 2069  ng if the list i
-000070c0: 7320 6120 7374 6163 6b2e 200a 0a20 2020  s a stack. ..   
-000070d0: 2041 7267 733a 0a20 2020 2020 2020 2065   Args:.        e
-000070e0: 6461 7461 2028 5072 6f66 696c 652c 2050  data (Profile, P
-000070f0: 726f 6669 6c65 5769 7468 5469 6573 2c20  rofileWithTies, 
-00007100: 4d61 7267 696e 4772 6170 6829 3a20 416e  MarginGraph): An
-00007110: 7920 656c 6563 7469 6f6e 2064 6174 6120  y election data 
-00007120: 7468 6174 2068 6173 2061 2060 6d61 7267  that has a `marg
-00007130: 696e 6020 6d65 7468 6f64 2e20 0a20 2020  in` method. .   
-00007140: 2020 2020 2063 7572 725f 6361 6e64 7320       curr_cands 
-00007150: 284c 6973 745b 696e 745d 2c20 6f70 7469  (List[int], opti
-00007160: 6f6e 616c 293a 2049 6620 7365 742c 2074  onal): If set, t
-00007170: 6865 6e20 6669 6e64 2074 6865 2077 696e  hen find the win
-00007180: 6e65 7273 2066 6f72 2074 6865 2070 726f  ners for the pro
-00007190: 6669 6c65 2072 6573 7472 6963 7465 6420  file restricted 
-000071a0: 746f 2074 6865 2063 616e 6469 6461 7465  to the candidate
-000071b0: 7320 696e 2060 6063 7572 725f 6361 6e64  s in ``curr_cand
-000071c0: 7360 600a 0a20 2020 2052 6574 7572 6e73  s``..    Returns
-000071d0: 3a20 0a20 2020 2020 2020 2041 2073 6f72  : .        A sor
-000071e0: 7465 6420 6c69 7374 206f 6620 6361 6e64  ted list of cand
-000071f0: 6964 6174 6573 2e20 0a0a 2020 2020 2e2e  idates. ..    ..
-00007200: 2073 6565 616c 736f 3a3a 0a20 2020 2020   seealso::.     
-00007210: 2020 200a 2020 2020 2020 2020 3a6d 6574     .        :met
-00007220: 683a 6070 7265 665f 766f 7469 6e67 2e6d  h:`pref_voting.m
-00007230: 6172 6769 6e5f 6261 7365 645f 6d65 7468  argin_based_meth
-00007240: 6f64 732e 6973 5f73 7461 636b 600a 0a0a  ods.is_stack`...
-00007250: 2020 2020 2222 2220 2020 200a 0a20 2020      """    ..   
-00007260: 2063 616e 6469 6461 7465 7320 3d20 6375   candidates = cu
-00007270: 7272 5f63 616e 6473 2069 6620 6375 7272  rr_cands if curr
-00007280: 5f63 616e 6473 2069 7320 6e6f 7420 4e6f  _cands is not No
-00007290: 6e65 2065 6c73 6520 6564 6174 612e 6361  ne else edata.ca
-000072a0: 6e64 6964 6174 6573 0a20 2020 2077 696e  ndidates.    win
-000072b0: 6e65 7273 203d 206c 6973 7428 290a 2020  ners = list().  
-000072c0: 2020 666f 7220 636c 6973 7420 696e 2070    for clist in p
-000072d0: 6572 6d75 7461 7469 6f6e 7328 6361 6e64  ermutations(cand
-000072e0: 6964 6174 6573 293a 200a 2020 2020 2020  idates): .      
-000072f0: 2020 6973 7374 6163 6b20 3d20 6973 5f73    isstack = is_s
-00007300: 7461 636b 2865 6461 7461 2c20 636c 6973  tack(edata, clis
-00007310: 742c 2063 7572 725f 6361 6e64 7320 3d20  t, curr_cands = 
-00007320: 6375 7272 5f63 616e 6473 290a 2020 2020  curr_cands).    
-00007330: 2020 2020 6966 2069 7373 7461 636b 3a20      if isstack: 
-00007340: 0a20 2020 2020 2020 2020 2020 2077 696e  .            win
-00007350: 6e65 7273 2e61 7070 656e 6428 636c 6973  ners.append(clis
-00007360: 745b 305d 290a 2020 2020 2020 2020 2020  t[0]).          
-00007370: 2020 0a20 2020 2072 6574 7572 6e20 736f    .    return so
-00007380: 7274 6564 286c 6973 7428 7365 7428 7769  rted(list(set(wi
-00007390: 6e6e 6572 7329 2929 0a0a 6465 6620 5f72  nners)))..def _r
-000073a0: 616e 6b65 645f 7061 6972 735f 6261 7369  anked_pairs_basi
-000073b0: 6328 0a20 2020 2065 6461 7461 2c20 0a20  c(.    edata, . 
-000073c0: 2020 2063 7572 725f 6361 6e64 7320 3d20     curr_cands = 
-000073d0: 4e6f 6e65 2c20 0a20 2020 2073 7472 656e  None, .    stren
-000073e0: 6774 685f 6675 6e63 7469 6f6e 203d 204e  gth_function = N
-000073f0: 6f6e 6529 3a20 2020 0a20 2020 2022 2222  one):   .    """
-00007400: 416e 2069 6d70 6c65 6d65 6e74 6174 696f  An implementatio
-00007410: 6e20 6f66 2052 616e 6b65 6420 5061 6972  n of Ranked Pair
-00007420: 7320 7468 6174 2075 7365 7320 6120 6261  s that uses a ba
-00007430: 7369 6320 616c 676f 7269 7468 6d2e 200a  sic algorithm. .
-00007440: 0a20 2020 2041 7267 733a 0a20 2020 2020  .    Args:.     
-00007450: 2020 2065 6461 7461 2028 5072 6f66 696c     edata (Profil
-00007460: 652c 2050 726f 6669 6c65 5769 7468 5469  e, ProfileWithTi
-00007470: 6573 2c20 4d61 7267 696e 4772 6170 6829  es, MarginGraph)
-00007480: 3a20 416e 7920 656c 6563 7469 6f6e 2064  : Any election d
-00007490: 6174 6120 7468 6174 2068 6173 2061 2060  ata that has a `
-000074a0: 6d61 7267 696e 6020 6d65 7468 6f64 2e20  margin` method. 
-000074b0: 0a20 2020 2020 2020 2063 7572 725f 6361  .        curr_ca
-000074c0: 6e64 7320 284c 6973 745b 696e 745d 2c20  nds (List[int], 
-000074d0: 6f70 7469 6f6e 616c 293a 2049 6620 7365  optional): If se
-000074e0: 742c 2074 6865 6e20 6669 6e64 2074 6865  t, then find the
-000074f0: 2077 696e 6e65 7273 2066 6f72 2074 6865   winners for the
-00007500: 2070 726f 6669 6c65 2072 6573 7472 6963   profile restric
-00007510: 7465 6420 746f 2074 6865 2063 616e 6469  ted to the candi
-00007520: 6461 7465 7320 696e 2060 6063 7572 725f  dates in ``curr_
-00007530: 6361 6e64 7360 600a 0a20 2020 2052 6574  cands``..    Ret
-00007540: 7572 6e73 3a20 0a20 2020 2020 2020 2041  urns: .        A
-00007550: 2073 6f72 7465 6420 6c69 7374 206f 6620   sorted list of 
-00007560: 6361 6e64 6964 6174 6573 2e20 0a0a 2020  candidates. ..  
-00007570: 2020 2222 220a 2020 2020 6361 6e64 6964    """.    candid
-00007580: 6174 6573 203d 2065 6461 7461 2e63 616e  ates = edata.can
-00007590: 6469 6461 7465 7320 6966 2063 7572 725f  didates if curr_
-000075a0: 6361 6e64 7320 6973 204e 6f6e 6520 656c  cands is None el
-000075b0: 7365 2063 7572 725f 6361 6e64 7320 0a20  se curr_cands . 
-000075c0: 2020 2063 6964 785f 746f 5f63 616e 6420     cidx_to_cand 
-000075d0: 3d20 7b63 6964 783a 2063 2066 6f72 2063  = {cidx: c for c
-000075e0: 6964 782c 2063 2069 6e20 656e 756d 6572  idx, c in enumer
-000075f0: 6174 6528 6361 6e64 6964 6174 6573 297d  ate(candidates)}
-00007600: 2020 0a20 2020 2063 616e 645f 746f 5f63    .    cand_to_c
-00007610: 6964 7820 3d20 7b63 3a20 6369 6478 2066  idx = {c: cidx f
-00007620: 6f72 2063 6964 782c 2063 2069 6e20 656e  or cidx, c in en
-00007630: 756d 6572 6174 6528 6361 6e64 6964 6174  umerate(candidat
-00007640: 6573 297d 2020 0a20 2020 2073 7472 656e  es)}  .    stren
-00007650: 6774 685f 6675 6e63 7469 6f6e 203d 2065  gth_function = e
-00007660: 6461 7461 2e6d 6172 6769 6e20 6966 2073  data.margin if s
-00007670: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
-00007680: 2069 7320 4e6f 6e65 2065 6c73 6520 7374   is None else st
-00007690: 7265 6e67 7468 5f66 756e 6374 696f 6e20  rength_function 
-000076a0: 2020 200a 0a20 2020 2063 7720 3d20 6564     ..    cw = ed
-000076b0: 6174 612e 636f 6e64 6f72 6365 745f 7769  ata.condorcet_wi
-000076c0: 6e6e 6572 2863 7572 725f 6361 6e64 733d  nner(curr_cands=
-000076d0: 6375 7272 5f63 616e 6473 290a 2020 2020  curr_cands).    
-000076e0: 2320 5261 6e6b 6564 2050 6169 7273 2069  # Ranked Pairs i
-000076f0: 7320 436f 6e64 6f72 6365 7420 636f 6e73  s Condorcet cons
-00007700: 6973 7465 6e74 2c20 736f 2073 696d 706c  istent, so simpl
-00007710: 7920 7265 7475 726e 2074 6865 2043 6f6e  y return the Con
-00007720: 646f 7263 6574 2077 696e 6e65 7220 6966  dorcet winner if
-00007730: 2065 7869 7374 730a 2020 2020 6966 2063   exists.    if c
-00007740: 7720 6973 206e 6f74 204e 6f6e 653a 200a  w is not None: .
-00007750: 2020 2020 2020 2020 7769 6e6e 6572 7320          winners 
-00007760: 3d20 5b63 775d 0a20 2020 2065 6c73 653a  = [cw].    else:
-00007770: 0a20 2020 2020 2020 2077 5f65 6467 6573  .        w_edges
-00007780: 203d 205b 2863 312c 2063 322c 2073 7472   = [(c1, c2, str
-00007790: 656e 6774 685f 6675 6e63 7469 6f6e 2863  ength_function(c
-000077a0: 312c 2063 3229 2920 666f 7220 6331 2069  1, c2)) for c1 i
-000077b0: 6e20 6361 6e64 6964 6174 6573 2066 6f72  n candidates for
-000077c0: 2063 3220 696e 2063 616e 6469 6461 7465   c2 in candidate
-000077d0: 7320 0a20 2020 2020 2020 2020 2020 2020  s .             
-000077e0: 2020 2020 2020 6966 2063 3120 213d 2063        if c1 != c
-000077f0: 3220 616e 6420 2865 6461 7461 2e6d 616a  2 and (edata.maj
-00007800: 6f72 6974 795f 7072 6566 6572 7328 6331  ority_prefers(c1
-00007810: 2c20 6332 2920 6f72 2065 6461 7461 2e69  , c2) or edata.i
-00007820: 735f 7469 6564 2863 312c 2063 3229 295d  s_tied(c1, c2))]
-00007830: 0a20 2020 2020 2020 2077 696e 6e65 7273  .        winners
-00007840: 203d 206c 6973 7428 2920 2020 0a20 2020   = list()   .   
-00007850: 2020 2020 2069 6620 6c65 6e28 775f 6564       if len(w_ed
-00007860: 6765 7329 203e 2030 3a20 2020 2020 2020  ges) > 0:       
-00007870: 2020 200a 2020 2020 2020 2020 2020 2020     .            
-00007880: 7374 7265 6e67 7468 7320 3d20 736f 7274  strengths = sort
-00007890: 6564 286c 6973 7428 7365 7428 5b65 5b32  ed(list(set([e[2
-000078a0: 5d20 666f 7220 6520 696e 2077 5f65 6467  ] for e in w_edg
-000078b0: 6573 5d29 292c 2072 6576 6572 7365 3d54  es])), reverse=T
-000078c0: 7275 6529 0a20 2020 2020 2020 2020 2020  rue).           
-000078d0: 2073 6f72 7465 645f 6564 6765 7320 3d20   sorted_edges = 
-000078e0: 5b5b 6520 666f 7220 6520 696e 2077 5f65  [[e for e in w_e
-000078f0: 6467 6573 2069 6620 655b 325d 203d 3d20  dges if e[2] == 
-00007900: 735d 2066 6f72 2073 2069 6e20 7374 7265  s] for s in stre
-00007910: 6e67 7468 735d 0a20 2020 2020 2020 2020  ngths].         
-00007920: 2020 2074 6273 203d 2070 726f 6475 6374     tbs = product
-00007930: 282a 5b70 6572 6d75 7461 7469 6f6e 7328  (*[permutations(
-00007940: 6564 6765 7329 2066 6f72 2065 6467 6573  edges) for edges
-00007950: 2069 6e20 736f 7274 6564 5f65 6467 6573   in sorted_edges
-00007960: 5d29 0a20 2020 2020 2020 2020 2020 2066  ]).            f
-00007970: 6f72 2074 6220 696e 2074 6273 3a0a 2020  or tb in tbs:.  
-00007980: 2020 2020 2020 2020 2020 2020 2020 6564                ed
-00007990: 6765 7320 3d20 666c 6174 7465 6e28 7462  ges = flatten(tb
-000079a0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000079b0: 2020 7270 5f64 6566 6561 7420 3d20 5350    rp_defeat = SP
-000079c0: 4f28 6c65 6e28 6361 6e64 6964 6174 6573  O(len(candidates
-000079d0: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
-000079e0: 2020 2066 6f72 2065 302c 6531 2c73 2069     for e0,e1,s i
-000079f0: 6e20 6564 6765 733a 200a 2020 2020 2020  n edges: .      
-00007a00: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00007a10: 206e 6f74 2072 705f 6465 6665 6174 2e50   not rp_defeat.P
-00007a20: 5b63 616e 645f 746f 5f63 6964 785b 6531  [cand_to_cidx[e1
-00007a30: 5d5d 5b63 616e 645f 746f 5f63 6964 785b  ]][cand_to_cidx[
-00007a40: 6530 5d5d 3a0a 2020 2020 2020 2020 2020  e0]]:.          
-00007a50: 2020 2020 2020 2020 2020 2020 2020 7270                rp
-00007a60: 5f64 6566 6561 742e 6164 6428 6361 6e64  _defeat.add(cand
-00007a70: 5f74 6f5f 6369 6478 5b65 305d 2c63 616e  _to_cidx[e0],can
-00007a80: 645f 746f 5f63 6964 785b 6531 5d29 0a20  d_to_cidx[e1]). 
-00007a90: 2020 2020 2020 2020 2020 2020 2020 2077                 w
-00007aa0: 696e 6e65 7273 2e61 7070 656e 6428 6369  inners.append(ci
-00007ab0: 6478 5f74 6f5f 6361 6e64 5b72 705f 6465  dx_to_cand[rp_de
-00007ac0: 6665 6174 2e69 6e69 7469 616c 5f65 6c65  feat.initial_ele
-00007ad0: 6d65 6e74 7328 295b 305d 5d29 0a20 2020  ments()[0]]).   
-00007ae0: 2020 2020 2065 6c73 653a 200a 2020 2020       else: .    
-00007af0: 2020 2020 2020 2020 7769 6e6e 6572 7320          winners 
-00007b00: 3d20 6361 6e64 6964 6174 6573 0a20 2020  = candidates.   
-00007b10: 2072 6574 7572 6e20 736f 7274 6564 286c   return sorted(l
-00007b20: 6973 7428 7365 7428 7769 6e6e 6572 7329  ist(set(winners)
-00007b30: 2929 0a0a 0a72 705f 7072 6f70 6572 7469  ))...rp_properti
-00007b40: 6573 203d 2056 6f74 696e 674d 6574 686f  es = VotingMetho
-00007b50: 6450 726f 7065 7274 6965 7328 0a20 2020  dProperties(.   
-00007b60: 2063 6f6e 646f 7263 6574 5f77 696e 6e65   condorcet_winne
-00007b70: 723d 5472 7565 2c20 0a20 2020 2063 6f6e  r=True, .    con
-00007b80: 646f 7263 6574 5f6c 6f73 6572 3d54 7275  dorcet_loser=Tru
-00007b90: 652c 0a20 2020 2070 6172 6574 6f5f 646f  e,.    pareto_do
-00007ba0: 6d69 6e61 6e63 653d 5472 7565 2c0a 2020  minance=True,.  
-00007bb0: 2020 706f 7369 7469 7665 5f69 6e76 6f6c    positive_invol
-00007bc0: 7665 6d65 6e74 3d46 616c 7365 2c20 0a20  vement=False, . 
-00007bd0: 2020 2029 0a40 766d 286e 616d 653d 2252     ).@vm(name="R
-00007be0: 616e 6b65 6420 5061 6972 7322 2c0a 2020  anked Pairs",.  
-00007bf0: 2020 7072 6f70 6572 7469 6573 3d72 705f    properties=rp_
-00007c00: 7072 6f70 6572 7469 6573 2c0a 2020 2020  properties,.    
-00007c10: 696e 7075 745f 7479 7065 733d 5b45 6c65  input_types=[Ele
-00007c20: 6374 696f 6e54 7970 6573 2e50 524f 4649  ctionTypes.PROFI
-00007c30: 4c45 2c20 456c 6563 7469 6f6e 5479 7065  LE, ElectionType
-00007c40: 732e 5052 4f46 494c 455f 5749 5448 5f54  s.PROFILE_WITH_T
-00007c50: 4945 532c 2045 6c65 6374 696f 6e54 7970  IES, ElectionTyp
-00007c60: 6573 2e4d 4152 4749 4e5f 4752 4150 485d  es.MARGIN_GRAPH]
-00007c70: 290a 6465 6620 7261 6e6b 6564 5f70 6169  ).def ranked_pai
-00007c80: 7273 280a 2020 2020 6564 6174 612c 200a  rs(.    edata, .
-00007c90: 2020 2020 6375 7272 5f63 616e 6473 3d4e      curr_cands=N
-00007ca0: 6f6e 652c 200a 2020 2020 7374 7265 6e67  one, .    streng
-00007cb0: 7468 5f66 756e 6374 696f 6e3d 4e6f 6e65  th_function=None
-00007cc0: 2c20 0a20 2020 2061 6c67 6f72 6974 686d  , .    algorithm
-00007cd0: 3d27 6261 7369 6327 293a 2020 200a 2020  ='basic'):   .  
-00007ce0: 2020 2222 220a 2020 2020 4f72 6465 7220    """.    Order 
-00007cf0: 7468 6520 6564 6765 7320 696e 2074 6865  the edges in the
-00007d00: 206d 6172 6769 6e20 6772 6170 6820 6672   margin graph fr
-00007d10: 6f6d 206c 6172 6765 7374 2074 6f20 736d  om largest to sm
-00007d20: 616c 6c65 7374 2061 6e64 206c 6f63 6b20  allest and lock 
-00007d30: 7468 656d 2069 6e20 696e 2074 6861 7420  them in in that 
-00007d40: 6f72 6465 722c 2073 6b69 7070 696e 6720  order, skipping 
-00007d50: 6564 6765 7320 7468 6174 2063 7265 6174  edges that creat
-00007d60: 6520 6120 6379 636c 652e 2020 4966 2074  e a cycle.  If t
-00007d70: 6865 7265 2061 7265 2074 6965 7320 696e  here are ties in
-00007d80: 2074 6865 206d 6172 6769 6e73 2c20 6272   the margins, br
-00007d90: 6561 6b20 7468 6520 7469 6573 2075 7369  eak the ties usi
-00007da0: 6e67 2061 2074 6965 2d62 7265 616b 696e  ng a tie-breakin
-00007db0: 6720 7275 6c65 3a20 6120 6c69 6e65 6172  g rule: a linear
-00007dc0: 206f 7264 6572 696e 6720 6f76 6572 2074   ordering over t
-00007dd0: 6865 2065 6467 6573 2e20 2020 4120 6361  he edges.   A ca
-00007de0: 6e64 6964 6174 6520 6973 2061 2052 616e  ndidate is a Ran
-00007df0: 6b65 6420 5061 6972 7320 7769 6e6e 6572  ked Pairs winner
-00007e00: 2069 6620 6974 2077 696e 7320 6163 636f   if it wins acco
-00007e10: 7264 696e 6720 746f 2073 6f6d 6520 7469  rding to some ti
-00007e20: 652d 6272 6561 6b69 6e67 2072 756c 652e  e-breaking rule.
-00007e30: 2041 6c73 6f20 6b6e 6f77 6e20 6173 2054   Also known as T
-00007e40: 6964 656d 616e 2773 2052 756c 652e 0a0a  ideman's Rule...
-00007e50: 2020 2020 2e2e 2077 6172 6e69 6e67 3a3a      .. warning::
-00007e60: 200a 2020 2020 2020 2020 5468 6973 206d   .        This m
-00007e70: 6574 686f 6420 6361 6e20 7461 6b65 2061  ethod can take a
-00007e80: 2076 6572 7920 6c6f 6e67 2074 696d 6520   very long time 
-00007e90: 746f 2066 696e 6420 7769 6e6e 6572 732e  to find winners.
-00007ea0: 200a 2020 2020 2020 2020 0a20 2020 2041   .        .    A
-00007eb0: 7267 733a 0a20 2020 2020 2020 2065 6461  rgs:.        eda
-00007ec0: 7461 2028 5072 6f66 696c 652c 2050 726f  ta (Profile, Pro
-00007ed0: 6669 6c65 5769 7468 5469 6573 2c20 4d61  fileWithTies, Ma
-00007ee0: 7267 696e 4772 6170 6829 3a20 416e 7920  rginGraph): Any 
-00007ef0: 656c 6563 7469 6f6e 2064 6174 6120 7468  election data th
-00007f00: 6174 2068 6173 2061 2060 6d61 7267 696e  at has a `margin
-00007f10: 6020 6d65 7468 6f64 2e20 0a20 2020 2020  ` method. .     
-00007f20: 2020 2063 7572 725f 6361 6e64 7320 284c     curr_cands (L
-00007f30: 6973 745b 696e 745d 2c20 6f70 7469 6f6e  ist[int], option
-00007f40: 616c 293a 2049 6620 7365 742c 2074 6865  al): If set, the
-00007f50: 6e20 6669 6e64 2074 6865 2077 696e 6e65  n find the winne
-00007f60: 7273 2066 6f72 2074 6865 2070 726f 6669  rs for the profi
-00007f70: 6c65 2072 6573 7472 6963 7465 6420 746f  le restricted to
-00007f80: 2074 6865 2063 616e 6469 6461 7465 7320   the candidates 
-00007f90: 696e 2060 6063 7572 725f 6361 6e64 7360  in ``curr_cands`
-00007fa0: 600a 2020 2020 2020 2020 7374 7265 6e67  `.        streng
-00007fb0: 7468 5f66 756e 6374 696f 6e20 2866 756e  th_function (fun
-00007fc0: 6374 696f 6e2c 206f 7074 696f 6e61 6c29  ction, optional)
-00007fd0: 3a20 5468 6520 7374 7265 6e67 7468 2066  : The strength f
-00007fe0: 756e 6374 696f 6e20 746f 2062 6520 7573  unction to be us
-00007ff0: 6564 2074 6f20 6361 6c63 756c 6174 6520  ed to calculate 
-00008000: 7468 6520 7374 7265 6e67 7468 206f 6620  the strength of 
-00008010: 6120 7061 7468 2e20 2020 5468 6520 6465  a path.   The de
-00008020: 6661 756c 7420 6973 2074 6865 206d 6172  fault is the mar
-00008030: 6769 6e20 6d65 7468 6f64 206f 6620 6060  gin method of ``
-00008040: 6564 6174 6160 602e 2020 2054 6869 7320  edata``.   This 
-00008050: 6f6e 6c79 206d 6174 7465 7273 2077 6865  only matters whe
-00008060: 6e20 7468 6520 6261 6c6c 6f74 7320 6172  n the ballots ar
-00008070: 6520 6e6f 7420 6c69 6e65 6172 206f 7264  e not linear ord
-00008080: 6572 732e 200a 2020 2020 2020 2020 616c  ers. .        al
-00008090: 676f 7269 7468 6d20 2873 7472 2c20 6f70  gorithm (str, op
-000080a0: 7469 6f6e 616c 293a 2053 7065 6369 6679  tional): Specify
-000080b0: 2077 6869 6368 2061 6c67 6f72 6974 686d   which algorithm
-000080c0: 2074 6f20 7573 652e 2020 4f70 7469 6f6e   to use.  Option
-000080d0: 7320 6172 6520 2762 6173 6963 2720 2874  s are 'basic' (t
-000080e0: 6865 2064 6566 6175 6c74 2920 616e 6420  he default) and 
-000080f0: 2766 726f 6d5f 7374 6163 6b73 272e 0a0a  'from_stacks'...
-00008100: 2020 2020 5265 7475 726e 733a 200a 2020      Returns: .  
-00008110: 2020 2020 2020 4120 736f 7274 6564 206c        A sorted l
-00008120: 6973 7420 6f66 2063 616e 6469 6461 7465  ist of candidate
-00008130: 732e 200a 0a20 2020 202e 2e20 7365 6561  s. ..    .. seea
-00008140: 6c73 6f3a 3a0a 0a20 2020 2020 2020 203a  lso::..        :
-00008150: 6d65 7468 3a60 7072 6566 5f76 6f74 696e  meth:`pref_votin
-00008160: 672e 6d61 7267 696e 5f62 6173 6564 5f6d  g.margin_based_m
-00008170: 6574 686f 6473 2e72 616e 6b65 645f 7061  ethods.ranked_pa
-00008180: 6972 735f 7769 7468 5f74 6573 7460 2c20  irs_with_test`, 
-00008190: 3a6d 6574 683a 6070 7265 665f 766f 7469  :meth:`pref_voti
-000081a0: 6e67 2e6d 6172 6769 6e5f 6261 7365 645f  ng.margin_based_
-000081b0: 6d65 7468 6f64 732e 7261 6e6b 6564 5f70  methods.ranked_p
-000081c0: 6169 7273 5f7a 7460 2c20 3a6d 6574 683a  airs_zt`, :meth:
-000081d0: 6070 7265 665f 766f 7469 6e67 2e6d 6172  `pref_voting.mar
-000081e0: 6769 6e5f 6261 7365 645f 6d65 7468 6f64  gin_based_method
-000081f0: 732e 7261 6e6b 6564 5f70 6169 7273 5f64  s.ranked_pairs_d
-00008200: 6566 6561 7473 600a 0a20 2020 203a 4578  efeats`..    :Ex
-00008210: 616d 706c 653a 200a 0a20 2020 202e 2e20  ample: ..    .. 
-00008220: 706c 6f74 3a3a 2020 6d61 7267 696e 5f67  plot::  margin_g
-00008230: 7261 7068 735f 6578 616d 706c 6573 2f6d  raphs_examples/m
-00008240: 675f 6578 5f62 705f 7270 2e70 790a 2020  g_ex_bp_rp.py.  
-00008250: 2020 2020 2020 3a63 6f6e 7465 7874 3a20        :context: 
-00008260: 7265 7365 7420 200a 2020 2020 2020 2020  reset  .        
-00008270: 3a69 6e63 6c75 6465 2d73 6f75 7263 653a  :include-source:
-00008280: 2054 7275 650a 0a0a 2020 2020 2e2e 2063   True...    .. c
-00008290: 6f64 652d 626c 6f63 6b3a 3a20 0a0a 2020  ode-block:: ..  
-000082a0: 2020 2020 2020 6672 6f6d 2070 7265 665f        from pref_
-000082b0: 766f 7469 6e67 2e6d 6172 6769 6e5f 6261  voting.margin_ba
-000082c0: 7365 645f 6d65 7468 6f64 7320 696d 706f  sed_methods impo
-000082d0: 7274 2072 616e 6b65 645f 7061 6972 730a  rt ranked_pairs.
-000082e0: 0a20 2020 2020 2020 2072 616e 6b65 645f  .        ranked_
-000082f0: 7061 6972 732e 6469 7370 6c61 7928 6d67  pairs.display(mg
-00008300: 290a 2020 2020 2020 2020 7261 6e6b 6564  ).        ranked
-00008310: 5f70 6169 7273 2e64 6973 706c 6179 286d  _pairs.display(m
-00008320: 672c 2061 6c67 6f72 6974 686d 3d27 6261  g, algorithm='ba
-00008330: 7369 6327 2920 0a20 2020 2020 2020 2072  sic') .        r
-00008340: 616e 6b65 645f 7061 6972 732e 6469 7370  anked_pairs.disp
-00008350: 6c61 7928 6d67 2c20 616c 676f 7269 7468  lay(mg, algorith
-00008360: 6d3d 2766 726f 6d5f 7374 6163 6b73 2729  m='from_stacks')
-00008370: 2020 2020 0a0a 0a20 2020 202e 2e20 6578      ...    .. ex
-00008380: 6563 5f63 6f64 653a 3a20 0a20 2020 2020  ec_code:: .     
-00008390: 2020 203a 6869 6465 5f63 6f64 653a 0a0a     :hide_code:..
-000083a0: 2020 2020 2020 2020 6672 6f6d 2070 7265          from pre
-000083b0: 665f 766f 7469 6e67 2e77 6569 6768 7465  f_voting.weighte
-000083c0: 645f 6d61 6a6f 7269 7479 5f67 7261 7068  d_majority_graph
-000083d0: 7320 696d 706f 7274 204d 6172 6769 6e47  s import MarginG
-000083e0: 7261 7068 0a20 2020 2020 2020 2066 726f  raph.        fro
-000083f0: 6d20 7072 6566 5f76 6f74 696e 672e 6d61  m pref_voting.ma
-00008400: 7267 696e 5f62 6173 6564 5f6d 6574 686f  rgin_based_metho
-00008410: 6473 2069 6d70 6f72 7420 7261 6e6b 6564  ds import ranked
-00008420: 5f70 6169 7273 0a20 2020 2020 2020 200a  _pairs.        .
-00008430: 2020 2020 2020 2020 6d67 203d 204d 6172          mg = Mar
-00008440: 6769 6e47 7261 7068 285b 302c 2031 2c20  ginGraph([0, 1, 
-00008450: 322c 2033 5d2c 205b 2830 2c20 322c 2033  2, 3], [(0, 2, 3
-00008460: 292c 2028 312c 2030 2c20 3529 2c20 2832  ), (1, 0, 5), (2
-00008470: 2c20 312c 2035 292c 2028 322c 2033 2c20  , 1, 5), (2, 3, 
-00008480: 3129 2c20 2833 2c20 302c 2033 292c 2028  1), (3, 0, 3), (
-00008490: 332c 2031 2c20 3129 5d29 0a20 2020 2020  3, 1, 1)]).     
-000084a0: 2020 200a 2020 2020 2020 2020 7261 6e6b     .        rank
-000084b0: 6564 5f70 6169 7273 2e64 6973 706c 6179  ed_pairs.display
-000084c0: 286d 6729 0a20 2020 2020 2020 2072 616e  (mg).        ran
-000084d0: 6b65 645f 7061 6972 732e 6469 7370 6c61  ked_pairs.displa
-000084e0: 7928 6d67 2c20 616c 676f 7269 7468 6d3d  y(mg, algorithm=
-000084f0: 2762 6173 6963 2729 0a20 2020 2020 2020  'basic').       
-00008500: 2072 616e 6b65 645f 7061 6972 732e 6469   ranked_pairs.di
-00008510: 7370 6c61 7928 6d67 2c20 616c 676f 7269  splay(mg, algori
-00008520: 7468 6d3d 2766 726f 6d5f 7374 6163 6b73  thm='from_stacks
-00008530: 2729 0a0a 2020 2020 2222 220a 0a20 2020  ')..    """..   
-00008540: 2069 6620 616c 676f 7269 7468 6d20 3d3d   if algorithm ==
-00008550: 2027 6261 7369 6327 3a0a 2020 2020 2020   'basic':.      
-00008560: 2020 7265 7475 726e 205f 7261 6e6b 6564    return _ranked
-00008570: 5f70 6169 7273 5f62 6173 6963 2865 6461  _pairs_basic(eda
-00008580: 7461 2c20 6375 7272 5f63 616e 6473 203d  ta, curr_cands =
-00008590: 2063 7572 725f 6361 6e64 732c 2073 7472   curr_cands, str
-000085a0: 656e 6774 685f 6675 6e63 7469 6f6e 203d  ength_function =
-000085b0: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
-000085c0: 6f6e 290a 2020 2020 656c 6966 2061 6c67  on).    elif alg
-000085d0: 6f72 6974 686d 203d 3d20 2766 726f 6d5f  orithm == 'from_
-000085e0: 7374 6163 6b73 273a 0a20 2020 2020 2020  stacks':.       
-000085f0: 2072 6574 7572 6e20 5f72 616e 6b65 645f   return _ranked_
-00008600: 7061 6972 735f 6672 6f6d 5f73 7461 636b  pairs_from_stack
-00008610: 7328 6564 6174 612c 2063 7572 725f 6361  s(edata, curr_ca
-00008620: 6e64 7320 3d20 6375 7272 5f63 616e 6473  nds = curr_cands
-00008630: 290a 2020 2020 656c 7365 3a0a 2020 2020  ).    else:.    
-00008640: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
-00008650: 7272 6f72 2822 496e 7661 6c69 6420 616c  rror("Invalid al
-00008660: 676f 7269 7468 6d20 7370 6563 6966 6965  gorithm specifie
-00008670: 642e 2229 0a0a 4076 6d28 6e61 6d65 3d22  d.")..@vm(name="
-00008680: 5261 6e6b 6564 2050 6169 7273 222c 0a20  Ranked Pairs",. 
-00008690: 2020 2073 6b69 705f 7265 6769 7374 7261     skip_registra
-000086a0: 7469 6f6e 3d54 7275 6529 0a64 6566 2072  tion=True).def r
-000086b0: 616e 6b65 645f 7061 6972 735f 7769 7468  anked_pairs_with
-000086c0: 5f74 6573 7428 0a20 2020 2065 6461 7461  _test(.    edata
-000086d0: 2c20 0a20 2020 2063 7572 725f 6361 6e64  , .    curr_cand
-000086e0: 733d 4e6f 6e65 2c20 0a20 2020 2073 7472  s=None, .    str
-000086f0: 656e 6774 685f 6675 6e63 7469 6f6e 3d4e  ength_function=N
-00008700: 6f6e 6529 3a20 2020 0a20 2020 2022 2222  one):   .    """
-00008710: 4669 6e64 2074 6865 2052 616e 6b65 6420  Find the Ranked 
-00008720: 5061 6972 7320 7769 6e6e 6572 732c 2062  Pairs winners, b
-00008730: 7574 2069 6e63 6c75 6465 2061 2074 6573  ut include a tes
-00008740: 7420 746f 2064 6574 6572 6d69 6e65 6420  t to determined 
-00008750: 6966 2069 7420 7769 6c6c 2074 616b 6520  if it will take 
-00008760: 746f 6f20 6c6f 6e67 2074 6f20 636f 6d70  too long to comp
-00008770: 7574 6520 7468 6520 5261 6e6b 6564 2050  ute the Ranked P
-00008780: 6169 7273 2077 696e 6e65 7273 2e20 4966  airs winners. If
-00008790: 2074 6865 2063 616c 6375 6c61 7469 6f6e   the calculation
-000087a0: 206f 6620 7468 6520 7769 6e6e 6572 7320   of the winners 
-000087b0: 7769 6c6c 2074 616b 6520 746f 6f20 6c6f  will take too lo
-000087c0: 6e67 2c20 7265 7475 726e 204e 6f6e 652e  ng, return None.
-000087d0: 0a0a 2020 2020 2e2e 2069 6d70 6f72 7461  ..    .. importa
-000087e0: 6e74 3a3a 0a20 2020 2020 2020 2054 6869  nt::.        Thi
-000087f0: 7320 766f 7469 6e67 206d 6574 686f 6420  s voting method 
-00008800: 7468 6174 206d 6967 6874 2072 6574 7572  that might retur
-00008810: 6e20 4e6f 6e65 2072 6174 6865 7220 7468  n None rather th
-00008820: 616e 2061 206c 6973 7420 6f66 2063 616e  an a list of can
-00008830: 6469 6461 7465 732e 2020 0a0a 2020 2020  didates.  ..    
-00008840: 4172 6773 3a0a 2020 2020 2020 2020 6564  Args:.        ed
-00008850: 6174 6120 2850 726f 6669 6c65 2c20 5072  ata (Profile, Pr
-00008860: 6f66 696c 6557 6974 6854 6965 732c 204d  ofileWithTies, M
-00008870: 6172 6769 6e47 7261 7068 293a 2041 6e79  arginGraph): Any
-00008880: 2065 6c65 6374 696f 6e20 6461 7461 2074   election data t
-00008890: 6861 7420 6861 7320 6120 606d 6172 6769  hat has a `margi
-000088a0: 6e60 206d 6574 686f 642e 200a 2020 2020  n` method. .    
-000088b0: 2020 2020 6375 7272 5f63 616e 6473 2028      curr_cands (
-000088c0: 4c69 7374 5b69 6e74 5d2c 206f 7074 696f  List[int], optio
-000088d0: 6e61 6c29 3a20 4966 2073 6574 2c20 7468  nal): If set, th
-000088e0: 656e 2066 696e 6420 7468 6520 7769 6e6e  en find the winn
-000088f0: 6572 7320 666f 7220 7468 6520 7072 6f66  ers for the prof
-00008900: 696c 6520 7265 7374 7269 6374 6564 2074  ile restricted t
-00008910: 6f20 7468 6520 6361 6e64 6964 6174 6573  o the candidates
-00008920: 2069 6e20 6060 6375 7272 5f63 616e 6473   in ``curr_cands
-00008930: 6060 0a20 2020 2020 2020 2073 7472 656e  ``.        stren
-00008940: 6774 685f 6675 6e63 7469 6f6e 2028 6675  gth_function (fu
-00008950: 6e63 7469 6f6e 2c20 6f70 7469 6f6e 616c  nction, optional
-00008960: 293a 2054 6865 2073 7472 656e 6774 6820  ): The strength 
-00008970: 6675 6e63 7469 6f6e 2074 6f20 6265 2075  function to be u
-00008980: 7365 6420 746f 2063 616c 6375 6c61 7465  sed to calculate
-00008990: 2074 6865 2073 7472 656e 6774 6820 6f66   the strength of
-000089a0: 2061 2070 6174 682e 2020 2054 6865 2064   a path.   The d
-000089b0: 6566 6175 6c74 2069 7320 7468 6520 6d61  efault is the ma
-000089c0: 7267 696e 206d 6574 686f 6420 6f66 2060  rgin method of `
-000089d0: 6065 6461 7461 6060 2e20 2020 5468 6973  `edata``.   This
-000089e0: 206f 6e6c 7920 6d61 7474 6572 7320 7768   only matters wh
-000089f0: 656e 2074 6865 2062 616c 6c6f 7473 2061  en the ballots a
-00008a00: 7265 206e 6f74 206c 696e 6561 7220 6f72  re not linear or
-00008a10: 6465 7273 2e20 0a0a 2020 2020 5265 7475  ders. ..    Retu
-00008a20: 726e 733a 200a 2020 2020 2020 2020 4120  rns: .        A 
-00008a30: 736f 7274 6564 206c 6973 7420 6f66 2063  sorted list of c
-00008a40: 616e 6469 6461 7465 732e 200a 0a20 2020  andidates. ..   
-00008a50: 202e 2e20 7365 6561 6c73 6f3a 3a0a 0a20   .. seealso::.. 
-00008a60: 2020 2020 2020 203a 6d65 7468 3a60 7072         :meth:`pr
-00008a70: 6566 5f76 6f74 696e 672e 6d61 7267 696e  ef_voting.margin
-00008a80: 5f62 6173 6564 5f6d 6574 686f 6473 2e72  _based_methods.r
-00008a90: 616e 6b65 645f 7061 6972 735f 7769 7468  anked_pairs_with
-00008aa0: 5f74 6573 7460 2c20 3a6d 6574 683a 6070  _test`, :meth:`p
-00008ab0: 7265 665f 766f 7469 6e67 2e6d 6172 6769  ref_voting.margi
-00008ac0: 6e5f 6261 7365 645f 6d65 7468 6f64 732e  n_based_methods.
-00008ad0: 7261 6e6b 6564 5f70 6169 7273 5f7a 7460  ranked_pairs_zt`
-00008ae0: 2c20 3a6d 6574 683a 6070 7265 665f 766f  , :meth:`pref_vo
-00008af0: 7469 6e67 2e6d 6172 6769 6e5f 6261 7365  ting.margin_base
-00008b00: 645f 6d65 7468 6f64 732e 7261 6e6b 6564  d_methods.ranked
-00008b10: 5f70 6169 7273 5f64 6566 6561 7473 600a  _pairs_defeats`.
-00008b20: 0a20 2020 203a 4578 616d 706c 653a 200a  .    :Example: .
-00008b30: 0a20 2020 202e 2e20 706c 6f74 3a3a 2020  .    .. plot::  
-00008b40: 6d61 7267 696e 5f67 7261 7068 735f 6578  margin_graphs_ex
-00008b50: 616d 706c 6573 2f6d 675f 6578 5f72 705f  amples/mg_ex_rp_
-00008b60: 7769 7468 5f74 6573 742e 7079 0a20 2020  with_test.py.   
-00008b70: 2020 2020 203a 636f 6e74 6578 743a 2072       :context: r
-00008b80: 6573 6574 2020 0a20 2020 2020 2020 203a  eset  .        :
-00008b90: 696e 636c 7564 652d 736f 7572 6365 3a20  include-source: 
-00008ba0: 5472 7565 0a0a 0a20 2020 202e 2e20 636f  True...    .. co
-00008bb0: 6465 2d62 6c6f 636b 3a3a 200a 0a20 2020  de-block:: ..   
-00008bc0: 2020 2020 2066 726f 6d20 7072 6566 5f76       from pref_v
-00008bd0: 6f74 696e 672e 6d61 7267 696e 5f62 6173  oting.margin_bas
-00008be0: 6564 5f6d 6574 686f 6473 2069 6d70 6f72  ed_methods impor
-00008bf0: 7420 7261 6e6b 6564 5f70 6169 7273 5f77  t ranked_pairs_w
-00008c00: 6974 685f 7465 7374 0a0a 2020 2020 2020  ith_test..      
-00008c10: 2020 7261 6e6b 6564 5f70 6169 7273 5f77    ranked_pairs_w
-00008c20: 6974 685f 7465 7374 2e64 6973 706c 6179  ith_test.display
-00008c30: 286d 6729 0a0a 0a20 2020 202e 2e20 6578  (mg)...    .. ex
-00008c40: 6563 5f63 6f64 653a 3a20 0a20 2020 2020  ec_code:: .     
-00008c50: 2020 203a 6869 6465 5f63 6f64 653a 0a0a     :hide_code:..
-00008c60: 2020 2020 2020 2020 6672 6f6d 2070 7265          from pre
-00008c70: 665f 766f 7469 6e67 2e77 6569 6768 7465  f_voting.weighte
-00008c80: 645f 6d61 6a6f 7269 7479 5f67 7261 7068  d_majority_graph
-00008c90: 7320 696d 706f 7274 204d 6172 6769 6e47  s import MarginG
-00008ca0: 7261 7068 0a20 2020 2020 2020 2066 726f  raph.        fro
-00008cb0: 6d20 7072 6566 5f76 6f74 696e 672e 6d61  m pref_voting.ma
-00008cc0: 7267 696e 5f62 6173 6564 5f6d 6574 686f  rgin_based_metho
-00008cd0: 6473 2069 6d70 6f72 7420 7261 6e6b 6564  ds import ranked
-00008ce0: 5f70 6169 7273 5f77 6974 685f 7465 7374  _pairs_with_test
-00008cf0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00008d00: 2020 6d67 203d 204d 6172 6769 6e47 7261    mg = MarginGra
-00008d10: 7068 285b 302c 2031 2c20 322c 2033 5d2c  ph([0, 1, 2, 3],
-00008d20: 205b 2831 2c20 322c 2032 292c 2028 312c   [(1, 2, 2), (1,
-00008d30: 2033 2c20 3229 2c20 2832 2c20 302c 2032   3, 2), (2, 0, 2
-00008d40: 295d 290a 2020 2020 2020 2020 0a20 2020  )]).        .   
-00008d50: 2020 2020 2072 616e 6b65 645f 7061 6972       ranked_pair
-00008d60: 735f 7769 7468 5f74 6573 742e 6469 7370  s_with_test.disp
-00008d70: 6c61 7928 6d67 290a 0a0a 2020 2020 2222  lay(mg)...    ""
-00008d80: 2220 2020 200a 2020 2020 6361 6e64 6964  "    .    candid
-00008d90: 6174 6573 203d 2065 6461 7461 2e63 616e  ates = edata.can
-00008da0: 6469 6461 7465 7320 6966 2063 7572 725f  didates if curr_
-00008db0: 6361 6e64 7320 6973 204e 6f6e 6520 656c  cands is None el
-00008dc0: 7365 2063 7572 725f 6361 6e64 7320 2020  se curr_cands   
-00008dd0: 200a 2020 2020 6369 6478 5f74 6f5f 6361   .    cidx_to_ca
-00008de0: 6e64 203d 207b 6369 6478 3a20 6320 666f  nd = {cidx: c fo
-00008df0: 7220 6369 6478 2c20 6320 696e 2065 6e75  r cidx, c in enu
-00008e00: 6d65 7261 7465 2863 616e 6469 6461 7465  merate(candidate
-00008e10: 7329 7d20 200a 2020 2020 6361 6e64 5f74  s)}  .    cand_t
-00008e20: 6f5f 6369 6478 203d 207b 633a 2063 6964  o_cidx = {c: cid
-00008e30: 7820 666f 7220 6369 6478 2c20 6320 696e  x for cidx, c in
-00008e40: 2065 6e75 6d65 7261 7465 2863 616e 6469   enumerate(candi
-00008e50: 6461 7465 7329 7d20 200a 2020 2020 0a20  dates)}  .    . 
-00008e60: 2020 2073 7472 656e 6774 685f 6675 6e63     strength_func
-00008e70: 7469 6f6e 203d 2065 6461 7461 2e6d 6172  tion = edata.mar
-00008e80: 6769 6e20 6966 2073 7472 656e 6774 685f  gin if strength_
-00008e90: 6675 6e63 7469 6f6e 2069 7320 4e6f 6e65  function is None
-00008ea0: 2065 6c73 6520 7374 7265 6e67 7468 5f66   else strength_f
-00008eb0: 756e 6374 696f 6e20 2020 0a0a 2020 2020  unction   ..    
-00008ec0: 6377 203d 2065 6461 7461 2e63 6f6e 646f  cw = edata.condo
-00008ed0: 7263 6574 5f77 696e 6e65 7228 6375 7272  rcet_winner(curr
-00008ee0: 5f63 616e 6473 203d 2063 7572 725f 6361  _cands = curr_ca
-00008ef0: 6e64 7329 0a20 2020 2023 2052 616e 6b65  nds).    # Ranke
-00008f00: 6420 5061 6972 7320 6973 2043 6f6e 646f  d Pairs is Condo
-00008f10: 7263 6574 2063 6f6e 7369 7374 656e 742c  rcet consistent,
-00008f20: 2073 6f20 7369 6d70 6c79 2072 6574 7572   so simply retur
-00008f30: 6e20 7468 6520 436f 6e64 6f72 6365 7420  n the Condorcet 
-00008f40: 7769 6e6e 6572 2069 6620 6578 6973 7473  winner if exists
-00008f50: 0a20 2020 2069 6620 6377 2069 7320 6e6f  .    if cw is no
-00008f60: 7420 4e6f 6e65 3a20 0a20 2020 2020 2020  t None: .       
-00008f70: 2077 696e 6e65 7273 203d 205b 6377 5d0a   winners = [cw].
-00008f80: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00008f90: 2020 775f 6564 6765 7320 3d20 5b28 6331    w_edges = [(c1
-00008fa0: 2c20 6332 2c20 7374 7265 6e67 7468 5f66  , c2, strength_f
-00008fb0: 756e 6374 696f 6e28 6331 2c20 6332 2929  unction(c1, c2))
-00008fc0: 2066 6f72 2063 3120 696e 2063 616e 6469   for c1 in candi
-00008fd0: 6461 7465 7320 666f 7220 6332 2069 6e20  dates for c2 in 
-00008fe0: 6361 6e64 6964 6174 6573 200a 2020 2020  candidates .    
-00008ff0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00009000: 6620 6331 2021 3d20 6332 2061 6e64 2028  f c1 != c2 and (
-00009010: 6564 6174 612e 6d61 6a6f 7269 7479 5f70  edata.majority_p
-00009020: 7265 6665 7273 2863 312c 2063 3229 206f  refers(c1, c2) o
-00009030: 7220 6564 6174 612e 6973 5f74 6965 6428  r edata.is_tied(
-00009040: 6331 2c20 6332 2929 5d0a 2020 2020 2020  c1, c2))].      
-00009050: 2020 7769 6e6e 6572 7320 3d20 6c69 7374    winners = list
-00009060: 2829 2020 2020 2020 2020 2020 2020 0a20  ()            . 
-00009070: 2020 2020 2020 2073 7472 656e 6774 6873         strengths
-00009080: 203d 2073 6f72 7465 6428 6c69 7374 2873   = sorted(list(s
-00009090: 6574 285b 655b 325d 2066 6f72 2065 2069  et([e[2] for e i
-000090a0: 6e20 775f 6564 6765 735d 2929 2c20 7265  n w_edges])), re
-000090b0: 7665 7273 653d 5472 7565 290a 2020 2020  verse=True).    
-000090c0: 2020 2020 736f 7274 6564 5f65 6467 6573      sorted_edges
-000090d0: 203d 205b 5b65 2066 6f72 2065 2069 6e20   = [[e for e in 
-000090e0: 775f 6564 6765 7320 6966 2065 5b32 5d20  w_edges if e[2] 
-000090f0: 3d3d 2073 5d20 666f 7220 7320 696e 2073  == s] for s in s
-00009100: 7472 656e 6774 6873 5d0a 2020 2020 2020  trengths].      
-00009110: 2020 6966 206e 702e 7072 6f64 285b 6d61    if np.prod([ma
-00009120: 7468 2e66 6163 746f 7269 616c 286c 656e  th.factorial(len
-00009130: 2865 7329 2920 666f 7220 6573 2069 6e20  (es)) for es in 
-00009140: 736f 7274 6564 5f65 6467 6573 5d29 203e  sorted_edges]) >
-00009150: 2033 3030 303a 200a 2020 2020 2020 2020   3000: .        
-00009160: 2020 2020 7265 7475 726e 204e 6f6e 650a      return None.
-00009170: 2020 2020 2020 2020 656c 7365 3a20 0a20          else: . 
-00009180: 2020 2020 2020 2020 2020 2074 6273 203d             tbs =
-00009190: 2070 726f 6475 6374 282a 5b70 6572 6d75   product(*[permu
-000091a0: 7461 7469 6f6e 7328 6564 6765 7329 2066  tations(edges) f
-000091b0: 6f72 2065 6467 6573 2069 6e20 736f 7274  or edges in sort
-000091c0: 6564 5f65 6467 6573 5d29 0a20 2020 2020  ed_edges]).     
-000091d0: 2020 2020 2020 2066 6f72 2074 6220 696e         for tb in
-000091e0: 2074 6273 3a0a 2020 2020 2020 2020 2020   tbs:.          
-000091f0: 2020 2020 2020 6564 6765 7320 3d20 666c        edges = fl
-00009200: 6174 7465 6e28 7462 290a 2020 2020 2020  atten(tb).      
-00009210: 2020 2020 2020 2020 2020 7270 5f64 6566            rp_def
-00009220: 6561 7420 3d20 5350 4f28 6c65 6e28 6361  eat = SPO(len(ca
-00009230: 6e64 6964 6174 6573 2929 0a20 2020 2020  ndidates)).     
-00009240: 2020 2020 2020 2020 2020 2066 6f72 2065             for e
-00009250: 302c 6531 2c73 2069 6e20 6564 6765 733a  0,e1,s in edges:
-00009260: 200a 2020 2020 2020 2020 2020 2020 2020   .              
-00009270: 2020 2020 2020 6966 206e 6f74 2072 705f        if not rp_
-00009280: 6465 6665 6174 2e50 5b63 616e 645f 746f  defeat.P[cand_to
-00009290: 5f63 6964 785b 6531 5d5d 5b63 616e 645f  _cidx[e1]][cand_
-000092a0: 746f 5f63 6964 785b 6530 5d5d 3a0a 2020  to_cidx[e0]]:.  
-000092b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000092c0: 2020 2020 2020 7270 5f64 6566 6561 742e        rp_defeat.
-000092d0: 6164 6428 6361 6e64 5f74 6f5f 6369 6478  add(cand_to_cidx
-000092e0: 5b65 305d 2c63 616e 645f 746f 5f63 6964  [e0],cand_to_cid
-000092f0: 785b 6531 5d29 0a20 2020 2020 2020 2020  x[e1]).         
-00009300: 2020 2020 2020 2077 696e 6e65 7273 2e61         winners.a
-00009310: 7070 656e 6428 6369 6478 5f74 6f5f 6361  ppend(cidx_to_ca
-00009320: 6e64 5b72 705f 6465 6665 6174 2e69 6e69  nd[rp_defeat.ini
-00009330: 7469 616c 5f65 6c65 6d65 6e74 7328 295b  tial_elements()[
-00009340: 305d 5d29 0a20 2020 2072 6574 7572 6e20  0]]).    return 
-00009350: 736f 7274 6564 286c 6973 7428 7365 7428  sorted(list(set(
-00009360: 7769 6e6e 6572 7329 2929 0a0a 6465 6620  winners)))..def 
-00009370: 7261 6e6b 6564 5f70 6169 7273 5f64 6566  ranked_pairs_def
-00009380: 6561 7473 2865 6461 7461 2c20 6375 7272  eats(edata, curr
-00009390: 5f63 616e 6473 203d 204e 6f6e 652c 2073  _cands = None, s
-000093a0: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
-000093b0: 203d 204e 6f6e 6529 3a20 2020 0a20 2020   = None):   .   
-000093c0: 2022 2222 0a20 2020 2052 6574 7572 6e73   """.    Returns
-000093d0: 2074 6865 2052 616e 6b65 6420 5061 6972   the Ranked Pair
-000093e0: 7320 6465 6665 6174 2072 656c 6174 696f  s defeat relatio
-000093f0: 6e73 2070 726f 6475 6365 6420 6279 2074  ns produced by t
-00009400: 6865 2052 616e 6b65 6420 5061 6972 7320  he Ranked Pairs 
-00009410: 616c 676f 7269 7468 6d2e 200a 0a20 2020  algorithm. ..   
-00009420: 202e 2e20 696d 706f 7274 616e 743a 3a0a   .. important::.
-00009430: 2020 2020 2020 2020 556e 6c69 6b65 2074          Unlike t
-00009440: 6865 206f 7468 6572 2066 756e 6374 696f  he other functio
-00009450: 6e73 2074 6861 7420 7265 7475 726e 2061  ns that return a
-00009460: 2073 696e 676c 6520 6465 6665 6174 2072   single defeat r
-00009470: 656c 6174 696f 6e2c 2074 6869 7320 7265  elation, this re
-00009480: 7475 726e 7320 6120 6c69 7374 206f 6620  turns a list of 
-00009490: 6465 6665 6174 2072 656c 6174 696f 6e73  defeat relations
-000094a0: 2e20 0a20 2020 2020 2020 200a 2020 2020  . .        .    
-000094b0: 4172 6773 3a0a 2020 2020 2020 2020 6564  Args:.        ed
-000094c0: 6174 6120 2850 726f 6669 6c65 2c20 5072  ata (Profile, Pr
-000094d0: 6f66 696c 6557 6974 6854 6965 732c 204d  ofileWithTies, M
-000094e0: 6172 6769 6e47 7261 7068 293a 2041 6e79  arginGraph): Any
-000094f0: 2065 6c65 6374 696f 6e20 6461 7461 2074   election data t
-00009500: 6861 7420 6861 7320 6120 606d 6172 6769  hat has a `margi
-00009510: 6e60 206d 6574 686f 642e 200a 2020 2020  n` method. .    
-00009520: 2020 2020 6375 7272 5f63 616e 6473 2028      curr_cands (
-00009530: 4c69 7374 5b69 6e74 5d2c 206f 7074 696f  List[int], optio
-00009540: 6e61 6c29 3a20 4966 2073 6574 2c20 7468  nal): If set, th
-00009550: 656e 2066 696e 6420 7468 6520 7769 6e6e  en find the winn
-00009560: 6572 7320 666f 7220 7468 6520 7072 6f66  ers for the prof
-00009570: 696c 6520 7265 7374 7269 6374 6564 2074  ile restricted t
-00009580: 6f20 7468 6520 6361 6e64 6964 6174 6573  o the candidates
-00009590: 2069 6e20 6060 6375 7272 5f63 616e 6473   in ``curr_cands
-000095a0: 6060 0a20 2020 2020 2020 2073 7472 656e  ``.        stren
-000095b0: 6774 685f 6675 6e63 7469 6f6e 2028 6675  gth_function (fu
-000095c0: 6e63 7469 6f6e 2c20 6f70 7469 6f6e 616c  nction, optional
-000095d0: 293a 2054 6865 2073 7472 656e 6774 6820  ): The strength 
-000095e0: 6675 6e63 7469 6f6e 2074 6f20 6265 2075  function to be u
-000095f0: 7365 6420 746f 2063 616c 6375 6c61 7465  sed to calculate
-00009600: 2074 6865 2073 7472 656e 6774 6820 6f66   the strength of
-00009610: 2061 2070 6174 682e 2020 2054 6865 2064   a path.   The d
-00009620: 6566 6175 6c74 2069 7320 7468 6520 6d61  efault is the ma
-00009630: 7267 696e 206d 6574 686f 6420 6f66 2060  rgin method of `
-00009640: 6065 6461 7461 6060 2e20 2020 5468 6973  `edata``.   This
-00009650: 206f 6e6c 7920 6d61 7474 6572 7320 7768   only matters wh
-00009660: 656e 2074 6865 2062 616c 6c6f 7473 2061  en the ballots a
-00009670: 7265 206e 6f74 206c 696e 6561 7220 6f72  re not linear or
-00009680: 6465 7273 2e20 0a0a 2020 2020 5265 7475  ders. ..    Retu
-00009690: 726e 733a 200a 2020 2020 2020 2020 4120  rns: .        A 
-000096a0: 6e65 7477 6f72 6b78 2044 6947 7261 7068  networkx DiGraph
-000096b0: 2072 6570 7265 7365 6e74 696e 6720 7468   representing th
-000096c0: 6520 5261 6e6b 6564 2050 6169 7273 2064  e Ranked Pairs d
-000096d0: 6566 6561 7420 7265 6c61 7469 6f6e 2e20  efeat relation. 
-000096e0: 0a0a 2020 2020 2e2e 2073 6565 616c 736f  ..    .. seealso
-000096f0: 3a3a 0a0a 2020 2020 2020 2020 3a6d 6574  ::..        :met
-00009700: 683a 6070 7265 665f 766f 7469 6e67 2e6d  h:`pref_voting.m
-00009710: 6172 6769 6e5f 6261 7365 645f 6d65 7468  argin_based_meth
-00009720: 6f64 732e 7261 6e6b 6564 5f70 6169 7273  ods.ranked_pairs
-00009730: 602c 203a 6d65 7468 3a60 7072 6566 5f76  `, :meth:`pref_v
-00009740: 6f74 696e 672e 6d61 7267 696e 5f62 6173  oting.margin_bas
-00009750: 6564 5f6d 6574 686f 6473 2e72 616e 6b65  ed_methods.ranke
-00009760: 645f 7061 6972 735f 7769 7468 5f74 6573  d_pairs_with_tes
-00009770: 7460 0a0a 2020 2020 3a45 7861 6d70 6c65  t`..    :Example
-00009780: 3a20 0a0a 2020 2020 2e2e 2070 6c6f 743a  : ..    .. plot:
-00009790: 3a20 206d 6172 6769 6e5f 6772 6170 6873  :  margin_graphs
-000097a0: 5f65 7861 6d70 6c65 732f 6d67 5f65 785f  _examples/mg_ex_
-000097b0: 7270 5f64 6566 6561 7473 2e70 790a 2020  rp_defeats.py.  
-000097c0: 2020 2020 2020 3a63 6f6e 7465 7874 3a20        :context: 
-000097d0: 7265 7365 7420 200a 2020 2020 2020 2020  reset  .        
-000097e0: 3a69 6e63 6c75 6465 2d73 6f75 7263 653a  :include-source:
-000097f0: 2054 7275 650a 0a20 2020 202e 2e20 6578   True..    .. ex
-00009800: 6563 5f63 6f64 653a 3a0a 0a0a 2020 2020  ec_code::...    
-00009810: 2020 2020 6672 6f6d 2070 7265 665f 766f      from pref_vo
-00009820: 7469 6e67 2e77 6569 6768 7465 645f 6d61  ting.weighted_ma
-00009830: 6a6f 7269 7479 5f67 7261 7068 7320 696d  jority_graphs im
-00009840: 706f 7274 204d 6172 6769 6e47 7261 7068  port MarginGraph
-00009850: 0a20 2020 2020 2020 2066 726f 6d20 7072  .        from pr
-00009860: 6566 5f76 6f74 696e 672e 6d61 7267 696e  ef_voting.margin
-00009870: 5f62 6173 6564 5f6d 6574 686f 6473 2069  _based_methods i
-00009880: 6d70 6f72 7420 7261 6e6b 6564 5f70 6169  mport ranked_pai
-00009890: 7273 5f64 6566 6561 7473 0a0a 2020 2020  rs_defeats..    
-000098a0: 2020 2020 6d67 203d 204d 6172 6769 6e47      mg = MarginG
-000098b0: 7261 7068 285b 302c 2031 2c20 322c 2033  raph([0, 1, 2, 3
-000098c0: 5d2c 205b 2830 2c20 312c 2031 3029 2c20  ], [(0, 1, 10), 
-000098d0: 2830 2c20 322c 2032 292c 2028 312c 2033  (0, 2, 2), (1, 3
-000098e0: 2c20 3429 2c20 2832 2c20 312c 2036 292c  , 4), (2, 1, 6),
-000098f0: 2028 322c 2033 2c20 3829 2c20 2833 2c20   (2, 3, 8), (3, 
-00009900: 302c 2034 295d 290a 2020 2020 2020 2020  0, 4)]).        
-00009910: 7270 5f64 6566 6561 7473 203d 2072 616e  rp_defeats = ran
-00009920: 6b65 645f 7061 6972 735f 6465 6665 6174  ked_pairs_defeat
-00009930: 7328 6d67 290a 0a20 2020 2020 2020 2066  s(mg)..        f
-00009940: 6f72 2072 7064 2069 6e20 7270 5f64 6566  or rpd in rp_def
-00009950: 6561 7473 3a20 0a20 2020 2020 2020 2020  eats: .         
-00009960: 2020 2070 7269 6e74 2872 7064 2e65 6467     print(rpd.edg
-00009970: 6573 290a 0a20 2020 2022 2222 0a20 2020  es)..    """.   
-00009980: 200a 2020 2020 6361 6e64 6964 6174 6573   .    candidates
-00009990: 203d 2065 6461 7461 2e63 616e 6469 6461   = edata.candida
-000099a0: 7465 7320 6966 2063 7572 725f 6361 6e64  tes if curr_cand
-000099b0: 7320 6973 204e 6f6e 6520 656c 7365 2063  s is None else c
-000099c0: 7572 725f 6361 6e64 7320 2020 200a 2020  urr_cands    .  
-000099d0: 2020 7374 7265 6e67 7468 5f66 756e 6374    strength_funct
-000099e0: 696f 6e20 3d20 6564 6174 612e 6d61 7267  ion = edata.marg
-000099f0: 696e 2069 6620 7374 7265 6e67 7468 5f66  in if strength_f
-00009a00: 756e 6374 696f 6e20 6973 204e 6f6e 6520  unction is None 
-00009a10: 656c 7365 2073 7472 656e 6774 685f 6675  else strength_fu
-00009a20: 6e63 7469 6f6e 2020 2020 0a0a 2020 2020  nction    ..    
-00009a30: 775f 6564 6765 7320 3d20 5b28 6331 2c20  w_edges = [(c1, 
-00009a40: 6332 2c20 7374 7265 6e67 7468 5f66 756e  c2, strength_fun
-00009a50: 6374 696f 6e28 6331 2c20 6332 2929 2066  ction(c1, c2)) f
-00009a60: 6f72 2063 3120 696e 2063 616e 6469 6461  or c1 in candida
-00009a70: 7465 7320 666f 7220 6332 2069 6e20 6361  tes for c2 in ca
-00009a80: 6e64 6964 6174 6573 2069 6620 6331 2021  ndidates if c1 !
-00009a90: 3d20 6332 2061 6e64 2028 6564 6174 612e  = c2 and (edata.
-00009aa0: 6d61 6a6f 7269 7479 5f70 7265 6665 7273  majority_prefers
-00009ab0: 2863 312c 2063 3229 206f 7220 6564 6174  (c1, c2) or edat
-00009ac0: 612e 6973 5f74 6965 6428 6331 2c20 6332  a.is_tied(c1, c2
-00009ad0: 2929 5d0a 2020 2020 7769 6e6e 6572 7320  ))].    winners 
-00009ae0: 3d20 6c69 7374 2829 2020 2020 2020 2020  = list()        
-00009af0: 2020 2020 0a20 2020 2073 7472 656e 6774      .    strengt
-00009b00: 6873 203d 2073 6f72 7465 6428 6c69 7374  hs = sorted(list
-00009b10: 2873 6574 285b 655b 325d 2066 6f72 2065  (set([e[2] for e
-00009b20: 2069 6e20 775f 6564 6765 735d 2929 2c20   in w_edges])), 
-00009b30: 7265 7665 7273 653d 5472 7565 290a 2020  reverse=True).  
-00009b40: 2020 736f 7274 6564 5f65 6467 6573 203d    sorted_edges =
-00009b50: 205b 5b65 2066 6f72 2065 2069 6e20 775f   [[e for e in w_
-00009b60: 6564 6765 7320 6966 2065 5b32 5d20 3d3d  edges if e[2] ==
-00009b70: 2073 5d20 666f 7220 7320 696e 2073 7472   s] for s in str
-00009b80: 656e 6774 6873 5d0a 2020 2020 7462 7320  engths].    tbs 
-00009b90: 3d20 7072 6f64 7563 7428 2a5b 7065 726d  = product(*[perm
-00009ba0: 7574 6174 696f 6e73 2865 6467 6573 2920  utations(edges) 
-00009bb0: 666f 7220 6564 6765 7320 696e 2073 6f72  for edges in sor
-00009bc0: 7465 645f 6564 6765 735d 290a 2020 2020  ted_edges]).    
-00009bd0: 7270 5f64 6566 6561 7473 203d 206c 6973  rp_defeats = lis
-00009be0: 7428 290a 2020 2020 666f 7220 7462 2069  t().    for tb i
-00009bf0: 6e20 7462 733a 0a20 2020 2020 2020 2065  n tbs:.        e
-00009c00: 6467 6573 203d 2066 6c61 7474 656e 2874  dges = flatten(t
-00009c10: 6229 0a20 2020 2020 2020 2072 705f 6465  b).        rp_de
-00009c20: 6665 6174 203d 206e 782e 4469 4772 6170  feat = nx.DiGrap
-00009c30: 6828 2920 0a20 2020 2020 2020 2066 6f72  h() .        for
-00009c40: 2065 2069 6e20 6564 6765 733a 200a 2020   e in edges: .  
-00009c50: 2020 2020 2020 2020 2020 7270 5f64 6566            rp_def
-00009c60: 6561 742e 6164 645f 6564 6765 2865 5b30  eat.add_edge(e[0
-00009c70: 5d2c 2065 5b31 5d2c 2077 6569 6768 743d  ], e[1], weight=
-00009c80: 655b 325d 290a 2020 2020 2020 2020 2020  e[2]).          
-00009c90: 2020 6966 2064 6f65 735f 6372 6561 7465    if does_create
-00009ca0: 5f63 7963 6c65 2872 705f 6465 6665 6174  _cycle(rp_defeat
-00009cb0: 2c20 6529 3a0a 2020 2020 2020 2020 2020  , e):.          
-00009cc0: 2020 2020 2020 7270 5f64 6566 6561 742e        rp_defeat.
-00009cd0: 7265 6d6f 7665 5f65 6467 6528 655b 305d  remove_edge(e[0]
-00009ce0: 2c20 655b 315d 290a 2020 2020 2020 2020  , e[1]).        
-00009cf0: 7270 5f64 6566 6561 7473 2e61 7070 656e  rp_defeats.appen
-00009d00: 6428 7270 5f64 6566 6561 7429 0a20 2020  d(rp_defeat).   
-00009d10: 2020 2020 2077 696e 6e65 7273 2e61 7070       winners.app
-00009d20: 656e 6428 6d61 7869 6d61 6c5f 656c 656d  end(maximal_elem
-00009d30: 656e 7473 2872 705f 6465 6665 6174 295b  ents(rp_defeat)[
-00009d40: 305d 290a 2020 2020 7265 7475 726e 2072  0]).    return r
-00009d50: 705f 6465 6665 6174 730a 0a72 705f 7462  p_defeats..rp_tb
-00009d60: 5f70 726f 7065 7274 6965 7320 3d20 566f  _properties = Vo
-00009d70: 7469 6e67 4d65 7468 6f64 5072 6f70 6572  tingMethodProper
-00009d80: 7469 6573 280a 2020 2020 636f 6e64 6f72  ties(.    condor
-00009d90: 6365 745f 7769 6e6e 6572 3d54 7275 652c  cet_winner=True,
-00009da0: 200a 2020 2020 636f 6e64 6f72 6365 745f   .    condorcet_
-00009db0: 6c6f 7365 723d 5472 7565 2c0a 2020 2020  loser=True,.    
-00009dc0: 7061 7265 746f 5f64 6f6d 696e 616e 6365  pareto_dominance
-00009dd0: 3d54 7275 652c 0a20 2020 2070 6f73 6974  =True,.    posit
-00009de0: 6976 655f 696e 766f 6c76 656d 656e 743d  ive_involvement=
-00009df0: 4661 6c73 652c 200a 2020 2020 290a 4076  False, .    ).@v
-00009e00: 6d28 6e61 6d65 3d22 5261 6e6b 6564 2050  m(name="Ranked P
-00009e10: 6169 7273 2054 4222 2c0a 2020 2020 7072  airs TB",.    pr
-00009e20: 6f70 6572 7469 6573 3d72 705f 7462 5f70  operties=rp_tb_p
-00009e30: 726f 7065 7274 6965 732c 0a20 2020 2069  roperties,.    i
-00009e40: 6e70 7574 5f74 7970 6573 3d5b 456c 6563  nput_types=[Elec
-00009e50: 7469 6f6e 5479 7065 732e 5052 4f46 494c  tionTypes.PROFIL
-00009e60: 452c 2045 6c65 6374 696f 6e54 7970 6573  E, ElectionTypes
-00009e70: 2e50 524f 4649 4c45 5f57 4954 485f 5449  .PROFILE_WITH_TI
-00009e80: 4553 2c20 456c 6563 7469 6f6e 5479 7065  ES, ElectionType
-00009e90: 732e 4d41 5247 494e 5f47 5241 5048 5d29  s.MARGIN_GRAPH])
-00009ea0: 0a64 6566 2072 616e 6b65 645f 7061 6972  .def ranked_pair
-00009eb0: 735f 7462 280a 2020 2020 6564 6174 612c  s_tb(.    edata,
-00009ec0: 200a 2020 2020 6375 7272 5f63 616e 6473   .    curr_cands
-00009ed0: 203d 204e 6f6e 652c 200a 2020 2020 7469   = None, .    ti
-00009ee0: 655f 6272 6561 6b65 7220 3d20 4e6f 6e65  e_breaker = None
-00009ef0: 2c20 0a20 2020 2073 7472 656e 6774 685f  , .    strength_
-00009f00: 6675 6e63 7469 6f6e 203d 204e 6f6e 6529  function = None)
-00009f10: 3a20 2020 0a20 2020 2022 2222 0a20 2020  :   .    """.   
-00009f20: 2052 616e 6b65 6420 5061 6972 7320 7769   Ranked Pairs wi
-00009f30: 7468 2061 2066 6978 6564 206c 696e 6561  th a fixed linea
-00009f40: 7220 6f72 6465 7220 6f6e 2074 6865 2063  r order on the c
-00009f50: 616e 6469 6461 7465 7320 746f 2062 7265  andidates to bre
-00009f60: 616b 2061 6e79 2074 6965 7320 696e 2074  ak any ties in t
-00009f70: 6865 206d 6172 6769 6e73 2e20 2020 0a20  he margins.   . 
-00009f80: 2020 2053 696e 6365 2074 6865 2074 6965     Since the tie
-00009f90: 5f62 7265 616b 6572 2069 7320 6120 6c69  _breaker is a li
-00009fa0: 6e65 6172 206f 7264 6572 2c20 7468 6973  near order, this
-00009fb0: 206d 6574 686f 6420 6973 2072 6573 6f6c   method is resol
-00009fc0: 7574 652e 2020 200a 0a20 2020 2041 7267  ute.   ..    Arg
-00009fd0: 733a 0a20 2020 2020 2020 2065 6461 7461  s:.        edata
-00009fe0: 2028 5072 6f66 696c 652c 2050 726f 6669   (Profile, Profi
-00009ff0: 6c65 5769 7468 5469 6573 2c20 4d61 7267  leWithTies, Marg
-0000a000: 696e 4772 6170 6829 3a20 416e 7920 656c  inGraph): Any el
-0000a010: 6563 7469 6f6e 2064 6174 6120 7468 6174  ection data that
-0000a020: 2068 6173 2061 2060 6d61 7267 696e 6020   has a `margin` 
-0000a030: 6d65 7468 6f64 2e20 0a20 2020 2020 2020  method. .       
-0000a040: 2063 7572 725f 6361 6e64 7320 284c 6973   curr_cands (Lis
-0000a050: 745b 696e 745d 2c20 6f70 7469 6f6e 616c  t[int], optional
-0000a060: 293a 2049 6620 7365 742c 2074 6865 6e20  ): If set, then 
-0000a070: 6669 6e64 2074 6865 2077 696e 6e65 7273  find the winners
-0000a080: 2066 6f72 2074 6865 2070 726f 6669 6c65   for the profile
-0000a090: 2072 6573 7472 6963 7465 6420 746f 2074   restricted to t
-0000a0a0: 6865 2063 616e 6469 6461 7465 7320 696e  he candidates in
-0000a0b0: 2060 6063 7572 725f 6361 6e64 7360 600a   ``curr_cands``.
-0000a0c0: 2020 2020 2020 2020 7374 7265 6e67 7468          strength
-0000a0d0: 5f66 756e 6374 696f 6e20 2866 756e 6374  _function (funct
-0000a0e0: 696f 6e2c 206f 7074 696f 6e61 6c29 3a20  ion, optional): 
-0000a0f0: 5468 6520 7374 7265 6e67 7468 2066 756e  The strength fun
-0000a100: 6374 696f 6e20 746f 2062 6520 7573 6564  ction to be used
-0000a110: 2074 6f20 6361 6c63 756c 6174 6520 7468   to calculate th
-0000a120: 6520 7374 7265 6e67 7468 206f 6620 6120  e strength of a 
-0000a130: 7061 7468 2e20 2020 5468 6520 6465 6661  path.   The defa
-0000a140: 756c 7420 6973 2074 6865 206d 6172 6769  ult is the margi
-0000a150: 6e20 6d65 7468 6f64 206f 6620 6060 6564  n method of ``ed
-0000a160: 6174 6160 602e 2020 2054 6869 7320 6f6e  ata``.   This on
-0000a170: 6c79 206d 6174 7465 7273 2077 6865 6e20  ly matters when 
-0000a180: 7468 6520 6261 6c6c 6f74 7320 6172 6520  the ballots are 
-0000a190: 6e6f 7420 6c69 6e65 6172 206f 7264 6572  not linear order
-0000a1a0: 732e 200a 0a20 2020 2052 6574 7572 6e73  s. ..    Returns
-0000a1b0: 3a20 0a20 2020 2020 2020 2041 2073 6f72  : .        A sor
-0000a1c0: 7465 6420 6c69 7374 206f 6620 6361 6e64  ted list of cand
-0000a1d0: 6964 6174 6573 2e20 0a0a 2020 2020 2e2e  idates. ..    ..
-0000a1e0: 2073 6565 616c 736f 3a3a 0a0a 2020 2020   seealso::..    
-0000a1f0: 2020 2020 3a6d 6574 683a 6070 7265 665f      :meth:`pref_
-0000a200: 766f 7469 6e67 2e6d 6172 6769 6e5f 6261  voting.margin_ba
-0000a210: 7365 645f 6d65 7468 6f64 732e 7261 6e6b  sed_methods.rank
-0000a220: 6564 5f70 6169 7273 602c 203a 6d65 7468  ed_pairs`, :meth
-0000a230: 3a60 7072 6566 5f76 6f74 696e 672e 6d61  :`pref_voting.ma
-0000a240: 7267 696e 5f62 6173 6564 5f6d 6574 686f  rgin_based_metho
-0000a250: 6473 2e72 616e 6b65 645f 7061 6972 735f  ds.ranked_pairs_
-0000a260: 7769 7468 5f74 6573 7460 0a0a 2020 2020  with_test`..    
-0000a270: 2e2e 2065 7865 635f 636f 6465 3a3a 0a0a  .. exec_code::..
-0000a280: 2020 2020 2020 2020 6672 6f6d 2070 7265          from pre
-0000a290: 665f 766f 7469 6e67 2e70 726f 6669 6c65  f_voting.profile
-0000a2a0: 7320 696d 706f 7274 2050 726f 6669 6c65  s import Profile
-0000a2b0: 0a20 2020 2020 2020 2066 726f 6d20 7072  .        from pr
-0000a2c0: 6566 5f76 6f74 696e 672e 6d61 7267 696e  ef_voting.margin
-0000a2d0: 5f62 6173 6564 5f6d 6574 686f 6473 2069  _based_methods i
-0000a2e0: 6d70 6f72 7420 7261 6e6b 6564 5f70 6169  mport ranked_pai
-0000a2f0: 7273 5f74 622c 2072 616e 6b65 645f 7061  rs_tb, ranked_pa
-0000a300: 6972 735f 7a74 0a0a 2020 2020 2020 2020  irs_zt..        
-0000a310: 7072 6f66 203d 2050 726f 6669 6c65 285b  prof = Profile([
-0000a320: 5b32 2c20 332c 2031 2c20 305d 2c20 5b30  [2, 3, 1, 0], [0
-0000a330: 2c20 332c 2031 2c20 325d 2c20 5b31 2c20  , 3, 1, 2], [1, 
-0000a340: 332c 2032 2c20 305d 2c20 5b32 2c20 312c  3, 2, 0], [2, 1,
-0000a350: 2033 2c20 305d 5d2c 205b 312c 2031 2c20   3, 0]], [1, 1, 
-0000a360: 312c 2031 5d29 0a0a 2020 2020 2020 2020  1, 1])..        
-0000a370: 7072 6f66 2e64 6973 706c 6179 2829 0a0a  prof.display()..
-0000a380: 2020 2020 2020 2020 7261 6e6b 6564 5f70          ranked_p
-0000a390: 6169 7273 5f74 622e 6469 7370 6c61 7928  airs_tb.display(
-0000a3a0: 7072 6f66 290a 2020 2020 2020 2020 7261  prof).        ra
-0000a3b0: 6e6b 6564 5f70 6169 7273 5f74 622e 6469  nked_pairs_tb.di
-0000a3c0: 7370 6c61 7928 7072 6f66 2c20 7469 655f  splay(prof, tie_
-0000a3d0: 6272 6561 6b65 7220 3d20 5b33 2c20 322c  breaker = [3, 2,
-0000a3e0: 2031 2c20 305d 290a 2020 2020 2020 2020   1, 0]).        
-0000a3f0: 7261 6e6b 6564 5f70 6169 7273 5f7a 742e  ranked_pairs_zt.
-0000a400: 6469 7370 6c61 7928 7072 6f66 290a 0a20  display(prof).. 
-0000a410: 2020 2022 2222 0a0a 2020 2020 6361 6e64     """..    cand
-0000a420: 6964 6174 6573 203d 2065 6461 7461 2e63  idates = edata.c
-0000a430: 616e 6469 6461 7465 7320 6966 2063 7572  andidates if cur
-0000a440: 725f 6361 6e64 7320 6973 204e 6f6e 6520  r_cands is None 
-0000a450: 656c 7365 2063 7572 725f 6361 6e64 7320  else curr_cands 
-0000a460: 2020 200a 2020 2020 6369 6478 5f74 6f5f     .    cidx_to_
-0000a470: 6361 6e64 203d 207b 6369 6478 3a20 6320  cand = {cidx: c 
-0000a480: 666f 7220 6369 6478 2c20 6320 696e 2065  for cidx, c in e
-0000a490: 6e75 6d65 7261 7465 2863 616e 6469 6461  numerate(candida
-0000a4a0: 7465 7329 7d20 200a 2020 2020 6361 6e64  tes)}  .    cand
-0000a4b0: 5f74 6f5f 6369 6478 203d 207b 633a 2063  _to_cidx = {c: c
-0000a4c0: 6964 7820 666f 7220 6369 6478 2c20 6320  idx for cidx, c 
-0000a4d0: 696e 2065 6e75 6d65 7261 7465 2863 616e  in enumerate(can
-0000a4e0: 6469 6461 7465 7329 7d20 200a 0a20 2020  didates)}  ..   
-0000a4f0: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
-0000a500: 6f6e 203d 2065 6461 7461 2e6d 6172 6769  on = edata.margi
-0000a510: 6e20 6966 2073 7472 656e 6774 685f 6675  n if strength_fu
-0000a520: 6e63 7469 6f6e 2069 7320 4e6f 6e65 2065  nction is None e
-0000a530: 6c73 6520 7374 7265 6e67 7468 5f66 756e  lse strength_fun
-0000a540: 6374 696f 6e0a 2020 2020 0a20 2020 2074  ction.    .    t
-0000a550: 625f 7261 6e6b 696e 6720 3d20 7469 655f  b_ranking = tie_
-0000a560: 6272 6561 6b65 7220 6966 2074 6965 5f62  breaker if tie_b
-0000a570: 7265 616b 6572 2069 7320 6e6f 7420 4e6f  reaker is not No
-0000a580: 6e65 2065 6c73 6520 736f 7274 6564 286c  ne else sorted(l
-0000a590: 6973 7428 6361 6e64 6964 6174 6573 2929  ist(candidates))
-0000a5a0: 0a0a 2020 2020 6377 203d 2065 6461 7461  ..    cw = edata
-0000a5b0: 2e63 6f6e 646f 7263 6574 5f77 696e 6e65  .condorcet_winne
-0000a5c0: 7228 6375 7272 5f63 616e 6473 3d63 7572  r(curr_cands=cur
-0000a5d0: 725f 6361 6e64 7329 0a20 2020 2023 2052  r_cands).    # R
-0000a5e0: 616e 6b65 6420 5061 6972 7320 6973 2043  anked Pairs is C
-0000a5f0: 6f6e 646f 7263 6574 2063 6f6e 7369 7374  ondorcet consist
-0000a600: 656e 742c 2073 6f20 7369 6d70 6c79 2072  ent, so simply r
-0000a610: 6574 7572 6e20 7468 6520 436f 6e64 6f72  eturn the Condor
-0000a620: 6365 7420 7769 6e6e 6572 2069 6620 6578  cet winner if ex
-0000a630: 6973 7473 0a20 2020 2069 6620 6377 2069  ists.    if cw i
-0000a640: 7320 6e6f 7420 4e6f 6e65 3a20 0a20 2020  s not None: .   
-0000a650: 2020 2020 2077 696e 6e65 7273 203d 205b       winners = [
-0000a660: 6377 5d0a 2020 2020 656c 7365 3a0a 2020  cw].    else:.  
-0000a670: 2020 2020 2020 775f 6564 6765 7320 3d20        w_edges = 
-0000a680: 5b28 6331 2c20 6332 2c20 7374 7265 6e67  [(c1, c2, streng
-0000a690: 7468 5f66 756e 6374 696f 6e28 6331 2c20  th_function(c1, 
-0000a6a0: 6332 2929 2066 6f72 2063 3120 696e 2063  c2)) for c1 in c
-0000a6b0: 616e 6469 6461 7465 7320 666f 7220 6332  andidates for c2
-0000a6c0: 2069 6e20 6361 6e64 6964 6174 6573 200a   in candidates .
-0000a6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a6e0: 2020 2069 6620 6331 2021 3d20 6332 2061     if c1 != c2 a
-0000a6f0: 6e64 2028 6564 6174 612e 6d61 6a6f 7269  nd (edata.majori
-0000a700: 7479 5f70 7265 6665 7273 2863 312c 2063  ty_prefers(c1, c
-0000a710: 3229 206f 7220 6564 6174 612e 6973 5f74  2) or edata.is_t
-0000a720: 6965 6428 6331 2c20 6332 2929 5d0a 2020  ied(c1, c2))].  
-0000a730: 2020 2020 2020 7769 6e6e 6572 7320 3d20        winners = 
-0000a740: 6c69 7374 2829 2020 2020 2020 2020 2020  list()          
-0000a750: 2020 0a20 2020 2020 2020 2073 7472 656e    .        stren
-0000a760: 6774 6873 203d 2073 6f72 7465 6428 6c69  gths = sorted(li
-0000a770: 7374 2873 6574 285b 655b 325d 2066 6f72  st(set([e[2] for
-0000a780: 2065 2069 6e20 775f 6564 6765 735d 2929   e in w_edges]))
-0000a790: 2c20 7265 7665 7273 653d 5472 7565 290a  , reverse=True).
-0000a7a0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-0000a7b0: 2072 705f 6465 6665 6174 203d 2053 504f   rp_defeat = SPO
-0000a7c0: 286c 656e 2863 616e 6469 6461 7465 7329  (len(candidates)
-0000a7d0: 290a 0a20 2020 2020 2020 2066 6f72 2073  )..        for s
-0000a7e0: 2069 6e20 7374 7265 6e67 7468 733a 200a   in strengths: .
-0000a7f0: 2020 2020 2020 2020 2020 2020 6564 6765              edge
-0000a800: 7320 3d20 5b65 2066 6f72 2065 2069 6e20  s = [e for e in 
-0000a810: 775f 6564 6765 7320 6966 2065 5b32 5d20  w_edges if e[2] 
-0000a820: 3d3d 2073 5d0a 2020 2020 2020 2020 2020  == s].          
-0000a830: 2020 0a20 2020 2020 2020 2020 2020 2023    .            #
-0000a840: 2062 7265 616b 2074 6965 7320 7573 696e   break ties usin
-0000a850: 6720 7468 6520 6c65 7869 636f 6772 6170  g the lexicograp
-0000a860: 6869 6320 6f72 6465 7269 6e67 206f 6e20  hic ordering on 
-0000a870: 7475 706c 6573 2067 6976 656e 2074 625f  tuples given tb_
-0000a880: 7261 6e6b 696e 670a 2020 2020 2020 2020  ranking.        
-0000a890: 2020 2020 736f 7274 6564 5f65 6467 6573      sorted_edges
-0000a8a0: 203d 2073 6f72 7465 6428 6564 6765 732c   = sorted(edges,
-0000a8b0: 206b 6579 203d 206c 616d 6264 6120 653a   key = lambda e:
-0000a8c0: 2028 7462 5f72 616e 6b69 6e67 2e69 6e64   (tb_ranking.ind
-0000a8d0: 6578 2865 5b30 5d29 2c20 7462 5f72 616e  ex(e[0]), tb_ran
-0000a8e0: 6b69 6e67 2e69 6e64 6578 2865 5b31 5d29  king.index(e[1])
-0000a8f0: 292c 2072 6576 6572 7365 3d46 616c 7365  ), reverse=False
-0000a900: 290a 2020 2020 2020 2020 2020 2020 666f  ).            fo
-0000a910: 7220 6530 2c65 312c 7320 696e 2065 6467  r e0,e1,s in edg
-0000a920: 6573 3a20 0a20 2020 2020 2020 2020 2020  es: .           
-0000a930: 2020 2020 2069 6620 6e6f 7420 7270 5f64       if not rp_d
-0000a940: 6566 6561 742e 505b 6361 6e64 5f74 6f5f  efeat.P[cand_to_
-0000a950: 6369 6478 5b65 315d 5d5b 6361 6e64 5f74  cidx[e1]][cand_t
-0000a960: 6f5f 6369 6478 5b65 305d 5d3a 0a20 2020  o_cidx[e0]]:.   
-0000a970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a980: 2072 705f 6465 6665 6174 2e61 6464 2863   rp_defeat.add(c
-0000a990: 616e 645f 746f 5f63 6964 785b 6530 5d2c  and_to_cidx[e0],
-0000a9a0: 6361 6e64 5f74 6f5f 6369 6478 5b65 315d  cand_to_cidx[e1]
-0000a9b0: 290a 2020 2020 2020 2020 2020 2020 7769  ).            wi
-0000a9c0: 6e6e 6572 732e 6170 7065 6e64 2863 6964  nners.append(cid
-0000a9d0: 785f 746f 5f63 616e 645b 7270 5f64 6566  x_to_cand[rp_def
-0000a9e0: 6561 742e 696e 6974 6961 6c5f 656c 656d  eat.initial_elem
-0000a9f0: 656e 7473 2829 5b30 5d5d 290a 0a20 2020  ents()[0]])..   
-0000aa00: 2072 6574 7572 6e20 736f 7274 6564 286c   return sorted(l
-0000aa10: 6973 7428 7365 7428 7769 6e6e 6572 7329  ist(set(winners)
-0000aa20: 2929 0a0a 7270 5f7a 745f 7072 6f70 6572  ))..rp_zt_proper
-0000aa30: 7469 6573 203d 2056 6f74 696e 674d 6574  ties = VotingMet
-0000aa40: 686f 6450 726f 7065 7274 6965 7328 0a20  hodProperties(. 
-0000aa50: 2020 2063 6f6e 646f 7263 6574 5f77 696e     condorcet_win
-0000aa60: 6e65 723d 5472 7565 2c20 0a20 2020 2063  ner=True, .    c
-0000aa70: 6f6e 646f 7263 6574 5f6c 6f73 6572 3d54  ondorcet_loser=T
-0000aa80: 7275 652c 0a20 2020 2070 6172 6574 6f5f  rue,.    pareto_
-0000aa90: 646f 6d69 6e61 6e63 653d 5472 7565 2c20  dominance=True, 
-0000aaa0: 0a20 2020 2070 6f73 6974 6976 655f 696e  .    positive_in
-0000aab0: 766f 6c76 656d 656e 743d 4661 6c73 652c  volvement=False,
-0000aac0: 0a20 2020 2029 0a40 766d 286e 616d 653d  .    ).@vm(name=
-0000aad0: 2252 616e 6b65 6420 5061 6972 7320 5a54  "Ranked Pairs ZT
-0000aae0: 222c 0a20 2020 2070 726f 7065 7274 6965  ",.    propertie
-0000aaf0: 733d 7270 5f7a 745f 7072 6f70 6572 7469  s=rp_zt_properti
-0000ab00: 6573 2c0a 2020 2020 696e 7075 745f 7479  es,.    input_ty
-0000ab10: 7065 733d 5b45 6c65 6374 696f 6e54 7970  pes=[ElectionTyp
-0000ab20: 6573 2e50 524f 4649 4c45 5d29 0a64 6566  es.PROFILE]).def
-0000ab30: 2072 616e 6b65 645f 7061 6972 735f 7a74   ranked_pairs_zt
-0000ab40: 280a 2020 2020 7072 6f66 696c 652c 200a  (.    profile, .
-0000ab50: 2020 2020 6375 7272 5f63 616e 6473 203d      curr_cands =
-0000ab60: 204e 6f6e 652c 200a 2020 2020 7374 7265   None, .    stre
-0000ab70: 6e67 7468 5f66 756e 6374 696f 6e20 3d20  ngth_function = 
-0000ab80: 4e6f 6e65 293a 2020 200a 2020 2020 2222  None):   .    ""
-0000ab90: 2252 616e 6b65 6420 7061 6972 7320 7768  "Ranked pairs wh
-0000aba0: 6572 6520 6120 6669 7865 6420 766f 7465  ere a fixed vote
-0000abb0: 7220 6272 6561 6b73 2061 6e79 2074 6965  r breaks any tie
-0000abc0: 7320 696e 2074 6865 206d 6172 6769 6e73  s in the margins
-0000abd0: 2e20 2049 7420 6973 2061 6c77 6179 7320  .  It is always 
-0000abe0: 7468 6520 766f 7465 7220 696e 2070 6f73  the voter in pos
-0000abf0: 6974 696f 6e20 3020 7468 6174 2062 7265  ition 0 that bre
-0000ac00: 616b 7320 7468 6520 7469 6573 2e20 2053  aks the ties.  S
-0000ac10: 696e 6365 2076 6f74 6572 7320 6861 7665  ince voters have
-0000ac20: 2073 7472 6963 7420 7072 6566 6572 656e   strict preferen
-0000ac30: 6365 732c 2074 6869 7320 6d65 7468 6f64  ces, this method
-0000ac40: 2069 7320 7265 736f 6c75 7465 2e20 2054   is resolute.  T
-0000ac50: 6869 7320 6973 206b 6e6f 776e 2061 7320  his is known as 
-0000ac60: 5261 6e6b 6564 2050 6169 7273 205a 542c  Ranked Pairs ZT,
-0000ac70: 2066 6f72 205a 6176 6973 7420 5469 6465   for Zavist Tide
-0000ac80: 6d61 6e2e 0a0a 2020 2020 4172 6773 3a0a  man...    Args:.
-0000ac90: 2020 2020 2020 2020 6564 6174 6120 2850          edata (P
-0000aca0: 726f 6669 6c65 293a 2041 2070 726f 6669  rofile): A profi
-0000acb0: 6c65 206f 6620 6c69 6e65 6172 206f 7264  le of linear ord
-0000acc0: 6572 730a 2020 2020 2020 2020 6375 7272  ers.        curr
-0000acd0: 5f63 616e 6473 2028 4c69 7374 5b69 6e74  _cands (List[int
-0000ace0: 5d2c 206f 7074 696f 6e61 6c29 3a20 4966  ], optional): If
-0000acf0: 2073 6574 2c20 7468 656e 2066 696e 6420   set, then find 
-0000ad00: 7468 6520 7769 6e6e 6572 7320 666f 7220  the winners for 
-0000ad10: 7468 6520 7072 6f66 696c 6520 7265 7374  the profile rest
-0000ad20: 7269 6374 6564 2074 6f20 7468 6520 6361  ricted to the ca
-0000ad30: 6e64 6964 6174 6573 2069 6e20 6060 6375  ndidates in ``cu
-0000ad40: 7272 5f63 616e 6473 6060 0a0a 2020 2020  rr_cands``..    
-0000ad50: 5265 7475 726e 733a 200a 2020 2020 2020  Returns: .      
-0000ad60: 2020 4120 736f 7274 6564 206c 6973 7420    A sorted list 
-0000ad70: 6f66 2063 616e 6469 6461 7465 732e 200a  of candidates. .
-0000ad80: 0a20 2020 202e 2e20 7365 6561 6c73 6f3a  .    .. seealso:
-0000ad90: 3a0a 0a20 2020 2020 2020 203a 6d65 7468  :..        :meth
-0000ada0: 3a60 7072 6566 5f76 6f74 696e 672e 6d61  :`pref_voting.ma
-0000adb0: 7267 696e 5f62 6173 6564 5f6d 6574 686f  rgin_based_metho
-0000adc0: 6473 2e72 616e 6b65 645f 7061 6972 7360  ds.ranked_pairs`
-0000add0: 2c20 3a6d 6574 683a 6070 7265 665f 766f  , :meth:`pref_vo
-0000ade0: 7469 6e67 2e6d 6172 6769 6e5f 6261 7365  ting.margin_base
-0000adf0: 645f 6d65 7468 6f64 732e 7261 6e6b 6564  d_methods.ranked
-0000ae00: 5f70 6169 7273 5f77 6974 685f 7465 7374  _pairs_with_test
-0000ae10: 600a 0a20 2020 202e 2e20 6578 6563 5f63  `..    .. exec_c
-0000ae20: 6f64 653a 3a0a 0a20 2020 2020 2020 2066  ode::..        f
-0000ae30: 726f 6d20 7072 6566 5f76 6f74 696e 672e  rom pref_voting.
-0000ae40: 7072 6f66 696c 6573 2069 6d70 6f72 7420  profiles import 
-0000ae50: 5072 6f66 696c 650a 2020 2020 2020 2020  Profile.        
-0000ae60: 6672 6f6d 2070 7265 665f 766f 7469 6e67  from pref_voting
-0000ae70: 2e6d 6172 6769 6e5f 6261 7365 645f 6d65  .margin_based_me
-0000ae80: 7468 6f64 7320 696d 706f 7274 2072 616e  thods import ran
-0000ae90: 6b65 645f 7061 6972 735f 7462 2c20 7261  ked_pairs_tb, ra
-0000aea0: 6e6b 6564 5f70 6169 7273 5f7a 740a 0a20  nked_pairs_zt.. 
-0000aeb0: 2020 2020 2020 2070 726f 6620 3d20 5072         prof = Pr
-0000aec0: 6f66 696c 6528 5b5b 322c 2033 2c20 312c  ofile([[2, 3, 1,
-0000aed0: 2030 5d2c 205b 302c 2033 2c20 312c 2032   0], [0, 3, 1, 2
-0000aee0: 5d2c 205b 312c 2033 2c20 322c 2030 5d2c  ], [1, 3, 2, 0],
-0000aef0: 205b 322c 2031 2c20 332c 2030 5d5d 2c20   [2, 1, 3, 0]], 
-0000af00: 5b31 2c20 312c 2031 2c20 315d 290a 0a20  [1, 1, 1, 1]).. 
-0000af10: 2020 2020 2020 2070 726f 662e 6469 7370         prof.disp
-0000af20: 6c61 7928 290a 0a20 2020 2020 2020 2072  lay()..        r
-0000af30: 616e 6b65 645f 7061 6972 735f 7462 2e64  anked_pairs_tb.d
-0000af40: 6973 706c 6179 2870 726f 6629 0a20 2020  isplay(prof).   
-0000af50: 2020 2020 2072 616e 6b65 645f 7061 6972       ranked_pair
-0000af60: 735f 7462 2e64 6973 706c 6179 2870 726f  s_tb.display(pro
-0000af70: 662c 2074 6965 5f62 7265 616b 6572 203d  f, tie_breaker =
-0000af80: 205b 332c 2032 2c20 312c 2030 5d29 0a20   [3, 2, 1, 0]). 
-0000af90: 2020 2020 2020 2072 616e 6b65 645f 7061         ranked_pa
-0000afa0: 6972 735f 7a74 2e64 6973 706c 6179 2870  irs_zt.display(p
-0000afb0: 726f 6629 0a0a 2020 2020 0a20 2020 2022  rof)..    .    "
-0000afc0: 2222 0a20 2020 2063 616e 6469 6461 7465  "".    candidate
-0000afd0: 7320 3d20 7072 6f66 696c 652e 6361 6e64  s = profile.cand
-0000afe0: 6964 6174 6573 2069 6620 6375 7272 5f63  idates if curr_c
-0000aff0: 616e 6473 2069 7320 4e6f 6e65 2065 6c73  ands is None els
-0000b000: 6520 6375 7272 5f63 616e 6473 2020 2020  e curr_cands    
-0000b010: 0a20 2020 200a 2020 2020 2320 7468 6520  .    .    # the 
-0000b020: 7469 652d 6272 6561 6b65 7220 6973 2061  tie-breaker is a
-0000b030: 6c77 6179 7320 7468 6520 6669 7273 7420  lways the first 
-0000b040: 766f 7465 722e 200a 2020 2020 7462 5f72  voter. .    tb_r
-0000b050: 616e 6b69 6e67 203d 2074 7570 6c65 285b  anking = tuple([
-0000b060: 6320 666f 7220 6320 696e 206c 6973 7428  c for c in list(
-0000b070: 7072 6f66 696c 652e 5f72 616e 6b69 6e67  profile._ranking
-0000b080: 735b 305d 2920 6966 2063 2069 6e20 6361  s[0]) if c in ca
-0000b090: 6e64 6964 6174 6573 5d29 0a20 2020 200a  ndidates]).    .
-0000b0a0: 2020 2020 7265 7475 726e 2072 616e 6b65      return ranke
-0000b0b0: 645f 7061 6972 735f 7462 2870 726f 6669  d_pairs_tb(profi
-0000b0c0: 6c65 2c20 6375 7272 5f63 616e 6473 203d  le, curr_cands =
-0000b0d0: 2063 7572 725f 6361 6e64 732c 2074 6965   curr_cands, tie
-0000b0e0: 5f62 7265 616b 6572 203d 2074 625f 7261  _breaker = tb_ra
-0000b0f0: 6e6b 696e 672c 2073 7472 656e 6774 685f  nking, strength_
-0000b100: 6675 6e63 7469 6f6e 203d 2073 7472 656e  function = stren
-0000b110: 6774 685f 6675 6e63 7469 6f6e 290a 0a72  gth_function)..r
-0000b120: 6976 6572 5f70 726f 7065 7274 6965 7320  iver_properties 
-0000b130: 3d20 566f 7469 6e67 4d65 7468 6f64 5072  = VotingMethodPr
-0000b140: 6f70 6572 7469 6573 280a 2020 2020 636f  operties(.    co
-0000b150: 6e64 6f72 6365 745f 7769 6e6e 6572 3d54  ndorcet_winner=T
-0000b160: 7275 652c 200a 2020 2020 636f 6e64 6f72  rue, .    condor
-0000b170: 6365 745f 6c6f 7365 723d 5472 7565 2c0a  cet_loser=True,.
-0000b180: 2020 2020 7061 7265 746f 5f64 6f6d 696e      pareto_domin
-0000b190: 616e 6365 3d54 7275 652c 0a20 2020 2070  ance=True,.    p
-0000b1a0: 6f73 6974 6976 655f 696e 766f 6c76 656d  ositive_involvem
-0000b1b0: 656e 743d 4661 6c73 652c 200a 2020 2020  ent=False, .    
-0000b1c0: 290a 4076 6d28 6e61 6d65 3d22 5269 7665  ).@vm(name="Rive
-0000b1d0: 7222 2c0a 2020 2020 7072 6f70 6572 7469  r",.    properti
-0000b1e0: 6573 3d72 6976 6572 5f70 726f 7065 7274  es=river_propert
-0000b1f0: 6965 732c 0a20 2020 2069 6e70 7574 5f74  ies,.    input_t
-0000b200: 7970 6573 3d5b 456c 6563 7469 6f6e 5479  ypes=[ElectionTy
-0000b210: 7065 732e 5052 4f46 494c 452c 2045 6c65  pes.PROFILE, Ele
-0000b220: 6374 696f 6e54 7970 6573 2e50 524f 4649  ctionTypes.PROFI
-0000b230: 4c45 5f57 4954 485f 5449 4553 2c20 456c  LE_WITH_TIES, El
-0000b240: 6563 7469 6f6e 5479 7065 732e 4d41 5247  ectionTypes.MARG
-0000b250: 494e 5f47 5241 5048 5d29 0a64 6566 2072  IN_GRAPH]).def r
-0000b260: 6976 6572 2865 6461 7461 2c20 6375 7272  iver(edata, curr
-0000b270: 5f63 616e 6473 203d 204e 6f6e 652c 2073  _cands = None, s
-0000b280: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
-0000b290: 203d 204e 6f6e 6529 3a20 2020 0a20 2020   = None):   .   
-0000b2a0: 2022 2222 0a20 2020 204f 7264 6572 2074   """.    Order t
-0000b2b0: 6865 2065 6467 6573 2069 6e20 7468 6520  he edges in the 
-0000b2c0: 7765 616b 206d 6172 6769 6e20 6772 6170  weak margin grap
-0000b2d0: 6820 6672 6f6d 206c 6172 6765 7374 2074  h from largest t
-0000b2e0: 6f20 736d 616c 6c65 7374 2061 6e64 206c  o smallest and l
-0000b2f0: 6f63 6b20 7468 656d 2069 6e20 696e 2074  ock them in in t
-0000b300: 6861 7420 6f72 6465 722c 2073 6b69 7070  hat order, skipp
-0000b310: 696e 6720 6564 6765 7320 7468 6174 2063  ing edges that c
-0000b320: 7265 6174 6520 6120 6379 636c 6520 2a61  reate a cycle *a
-0000b330: 6e64 2065 6467 6573 2069 6e20 7768 6963  nd edges in whic
-0000b340: 6820 7468 6572 6520 6973 2061 6c72 6561  h there is alrea
-0000b350: 6479 2061 6e20 6564 6765 2070 6f69 6e74  dy an edge point
-0000b360: 696e 6720 746f 2074 6865 2074 6172 6765  ing to the targe
-0000b370: 742a 2e20 2042 7265 616b 2074 6965 7320  t*.  Break ties 
-0000b380: 7573 696e 6720 6120 7469 652d 6272 6561  using a tie-brea
-0000b390: 6b69 6e67 2020 6c69 6e65 6172 206f 7264  king  linear ord
-0000b3a0: 6572 696e 6720 6f76 6572 2074 6865 2065  ering over the e
-0000b3b0: 6467 6573 2e20 2041 2063 616e 6469 6461  dges.  A candida
-0000b3c0: 7465 2069 7320 6120 5269 7665 7220 7769  te is a River wi
-0000b3d0: 6e6e 6572 2069 6620 6974 2077 696e 7320  nner if it wins 
-0000b3e0: 6163 636f 7264 696e 6720 746f 2073 6f6d  according to som
-0000b3f0: 6520 7469 652d 6272 6561 6b69 6e67 2072  e tie-breaking r
-0000b400: 756c 652e 2053 6565 2068 7474 7073 3a2f  ule. See https:/
-0000b410: 2f65 6c65 6374 6f77 696b 692e 6f72 672f  /electowiki.org/
-0000b420: 7769 6b69 2f52 6976 6572 2e0a 0a20 2020  wiki/River...   
-0000b430: 2041 7267 733a 0a20 2020 2020 2020 2065   Args:.        e
-0000b440: 6461 7461 2028 5072 6f66 696c 652c 2050  data (Profile, P
-0000b450: 726f 6669 6c65 5769 7468 5469 6573 2c20  rofileWithTies, 
-0000b460: 4d61 7267 696e 4772 6170 6829 3a20 416e  MarginGraph): An
-0000b470: 7920 656c 6563 7469 6f6e 2064 6174 6120  y election data 
-0000b480: 7468 6174 2068 6173 2061 2060 6d61 7267  that has a `marg
-0000b490: 696e 6020 6d65 7468 6f64 2e20 0a20 2020  in` method. .   
-0000b4a0: 2020 2020 2063 7572 725f 6361 6e64 7320       curr_cands 
-0000b4b0: 284c 6973 745b 696e 745d 2c20 6f70 7469  (List[int], opti
-0000b4c0: 6f6e 616c 293a 2049 6620 7365 742c 2074  onal): If set, t
-0000b4d0: 6865 6e20 6669 6e64 2074 6865 2077 696e  hen find the win
-0000b4e0: 6e65 7273 2066 6f72 2074 6865 2070 726f  ners for the pro
-0000b4f0: 6669 6c65 2072 6573 7472 6963 7465 6420  file restricted 
-0000b500: 746f 2074 6865 2063 616e 6469 6461 7465  to the candidate
-0000b510: 7320 696e 2060 6063 7572 725f 6361 6e64  s in ``curr_cand
-0000b520: 7360 600a 2020 2020 2020 2020 7374 7265  s``.        stre
-0000b530: 6e67 7468 5f66 756e 6374 696f 6e20 2866  ngth_function (f
-0000b540: 756e 6374 696f 6e2c 206f 7074 696f 6e61  unction, optiona
-0000b550: 6c29 3a20 5468 6520 7374 7265 6e67 7468  l): The strength
-0000b560: 2066 756e 6374 696f 6e20 746f 2062 6520   function to be 
-0000b570: 7573 6564 2074 6f20 6361 6c63 756c 6174  used to calculat
-0000b580: 6520 7468 6520 7374 7265 6e67 7468 206f  e the strength o
-0000b590: 6620 6120 7061 7468 2e20 2020 5468 6520  f a path.   The 
-0000b5a0: 6465 6661 756c 7420 6973 2074 6865 206d  default is the m
-0000b5b0: 6172 6769 6e20 6d65 7468 6f64 206f 6620  argin method of 
-0000b5c0: 6060 6564 6174 6160 602e 2020 2054 6869  ``edata``.   Thi
-0000b5d0: 7320 6f6e 6c79 206d 6174 7465 7273 2077  s only matters w
-0000b5e0: 6865 6e20 7468 6520 6261 6c6c 6f74 7320  hen the ballots 
-0000b5f0: 6172 6520 6e6f 7420 6c69 6e65 6172 206f  are not linear o
-0000b600: 7264 6572 732e 200a 0a20 2020 2052 6574  rders. ..    Ret
-0000b610: 7572 6e73 3a20 0a20 2020 2020 2020 2041  urns: .        A
-0000b620: 2073 6f72 7465 6420 6c69 7374 206f 6620   sorted list of 
-0000b630: 6361 6e64 6964 6174 6573 2e20 0a0a 2020  candidates. ..  
-0000b640: 2020 3a45 7861 6d70 6c65 3a20 0a0a 2020    :Example: ..  
-0000b650: 2020 2e2e 2065 7865 635f 636f 6465 3a3a    .. exec_code::
-0000b660: 200a 0a20 2020 2020 2020 2066 726f 6d20   ..        from 
-0000b670: 7072 6566 5f76 6f74 696e 672e 7765 6967  pref_voting.weig
-0000b680: 6874 6564 5f6d 616a 6f72 6974 795f 6772  hted_majority_gr
-0000b690: 6170 6873 2069 6d70 6f72 7420 4d61 7267  aphs import Marg
-0000b6a0: 696e 4772 6170 680a 2020 2020 2020 2020  inGraph.        
-0000b6b0: 6672 6f6d 2070 7265 665f 766f 7469 6e67  from pref_voting
-0000b6c0: 2e6d 6172 6769 6e5f 6261 7365 645f 6d65  .margin_based_me
-0000b6d0: 7468 6f64 7320 696d 706f 7274 2072 6976  thods import riv
-0000b6e0: 6572 2c20 7261 6e6b 6564 5f70 6169 7273  er, ranked_pairs
-0000b6f0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-0000b700: 2020 6d67 203d 204d 6172 6769 6e47 7261    mg = MarginGra
-0000b710: 7068 285b 302c 2031 2c20 322c 2033 5d2c  ph([0, 1, 2, 3],
-0000b720: 205b 2830 2c20 322c 2032 292c 2028 302c   [(0, 2, 2), (0,
-0000b730: 2033 2c20 3829 2c20 2831 2c20 302c 2031   3, 8), (1, 0, 1
-0000b740: 3229 2c20 2832 2c20 332c 2031 3229 2c20  2), (2, 3, 12), 
-0000b750: 2833 2c20 312c 2036 295d 290a 0a20 2020  (3, 1, 6)])..   
-0000b760: 2020 2020 2072 616e 6b65 645f 7061 6972       ranked_pair
-0000b770: 732e 6469 7370 6c61 7928 6d67 290a 2020  s.display(mg).  
-0000b780: 2020 2020 2020 7269 7665 722e 6469 7370        river.disp
-0000b790: 6c61 7928 6d67 290a 0a20 2020 2022 2222  lay(mg)..    """
-0000b7a0: 0a20 2020 2063 616e 6469 6461 7465 7320  .    candidates 
-0000b7b0: 3d20 6564 6174 612e 6361 6e64 6964 6174  = edata.candidat
-0000b7c0: 6573 2069 6620 6375 7272 5f63 616e 6473  es if curr_cands
-0000b7d0: 2069 7320 4e6f 6e65 2065 6c73 6520 6375   is None else cu
-0000b7e0: 7272 5f63 616e 6473 2020 2020 0a20 2020  rr_cands    .   
-0000b7f0: 2063 6964 785f 746f 5f63 616e 6420 3d20   cidx_to_cand = 
-0000b800: 7b63 6964 783a 2063 2066 6f72 2063 6964  {cidx: c for cid
-0000b810: 782c 2063 2069 6e20 656e 756d 6572 6174  x, c in enumerat
-0000b820: 6528 6361 6e64 6964 6174 6573 297d 2020  e(candidates)}  
-0000b830: 0a20 2020 2063 616e 645f 746f 5f63 6964  .    cand_to_cid
-0000b840: 7820 3d20 7b63 3a20 6369 6478 2066 6f72  x = {c: cidx for
-0000b850: 2063 6964 782c 2063 2069 6e20 656e 756d   cidx, c in enum
-0000b860: 6572 6174 6528 6361 6e64 6964 6174 6573  erate(candidates
-0000b870: 297d 2020 0a0a 2020 2020 7374 7265 6e67  )}  ..    streng
-0000b880: 7468 5f66 756e 6374 696f 6e20 3d20 6564  th_function = ed
-0000b890: 6174 612e 6d61 7267 696e 2069 6620 7374  ata.margin if st
-0000b8a0: 7265 6e67 7468 5f66 756e 6374 696f 6e20  rength_function 
-0000b8b0: 6973 204e 6f6e 6520 656c 7365 2073 7472  is None else str
-0000b8c0: 656e 6774 685f 6675 6e63 7469 6f6e 2020  ength_function  
-0000b8d0: 2020 0a0a 2020 2020 6377 203d 2065 6461    ..    cw = eda
-0000b8e0: 7461 2e63 6f6e 646f 7263 6574 5f77 696e  ta.condorcet_win
-0000b8f0: 6e65 7228 6375 7272 5f63 616e 6473 3d63  ner(curr_cands=c
-0000b900: 7572 725f 6361 6e64 7329 0a20 2020 2023  urr_cands).    #
-0000b910: 2052 616e 6b65 6420 5061 6972 7320 6973   Ranked Pairs is
-0000b920: 2043 6f6e 646f 7263 6574 2063 6f6e 7369   Condorcet consi
-0000b930: 7374 656e 742c 2073 6f20 7369 6d70 6c79  stent, so simply
-0000b940: 2072 6574 7572 6e20 7468 6520 436f 6e64   return the Cond
-0000b950: 6f72 6365 7420 7769 6e6e 6572 2069 6620  orcet winner if 
-0000b960: 6578 6973 7473 0a20 2020 2069 6620 6377  exists.    if cw
-0000b970: 2069 7320 6e6f 7420 4e6f 6e65 3a20 0a20   is not None: . 
-0000b980: 2020 2020 2020 2077 696e 6e65 7273 203d         winners =
-0000b990: 205b 6377 5d0a 2020 2020 656c 7365 3a0a   [cw].    else:.
-0000b9a0: 2020 2020 2020 2020 775f 6564 6765 7320          w_edges 
-0000b9b0: 3d20 5b28 6331 2c20 6332 2c20 7374 7265  = [(c1, c2, stre
-0000b9c0: 6e67 7468 5f66 756e 6374 696f 6e28 6331  ngth_function(c1
-0000b9d0: 2c20 6332 2929 2066 6f72 2063 3120 696e  , c2)) for c1 in
-0000b9e0: 2063 616e 6469 6461 7465 7320 666f 7220   candidates for 
-0000b9f0: 6332 2069 6e20 6361 6e64 6964 6174 6573  c2 in candidates
-0000ba00: 200a 2020 2020 2020 2020 2020 2020 2020   .              
-0000ba10: 2020 2020 2069 6620 6331 2021 3d20 6332       if c1 != c2
-0000ba20: 2061 6e64 2028 6564 6174 612e 6d61 6a6f   and (edata.majo
-0000ba30: 7269 7479 5f70 7265 6665 7273 2863 312c  rity_prefers(c1,
-0000ba40: 2063 3229 206f 7220 6564 6174 612e 6973   c2) or edata.is
-0000ba50: 5f74 6965 6428 6331 2c20 6332 2929 5d0a  _tied(c1, c2))].
-0000ba60: 2020 2020 2020 2020 7769 6e6e 6572 7320          winners 
-0000ba70: 3d20 6c69 7374 2829 2020 2020 2020 2020  = list()        
-0000ba80: 2020 2020 0a20 2020 2020 2020 2073 7472      .        str
-0000ba90: 656e 6774 6873 203d 2073 6f72 7465 6428  engths = sorted(
-0000baa0: 6c69 7374 2873 6574 285b 655b 325d 2066  list(set([e[2] f
-0000bab0: 6f72 2065 2069 6e20 775f 6564 6765 735d  or e in w_edges]
-0000bac0: 2929 2c20 7265 7665 7273 653d 5472 7565  )), reverse=True
-0000bad0: 290a 2020 2020 2020 2020 736f 7274 6564  ).        sorted
-0000bae0: 5f65 6467 6573 203d 205b 5b65 2066 6f72  _edges = [[e for
-0000baf0: 2065 2069 6e20 775f 6564 6765 7320 6966   e in w_edges if
-0000bb00: 2065 5b32 5d20 3d3d 2073 5d20 666f 7220   e[2] == s] for 
-0000bb10: 7320 696e 2073 7472 656e 6774 6873 5d0a  s in strengths].
-0000bb20: 2020 2020 2020 2020 7462 7320 3d20 7072          tbs = pr
-0000bb30: 6f64 7563 7428 2a5b 7065 726d 7574 6174  oduct(*[permutat
-0000bb40: 696f 6e73 2865 6467 6573 2920 666f 7220  ions(edges) for 
-0000bb50: 6564 6765 7320 696e 2073 6f72 7465 645f  edges in sorted_
-0000bb60: 6564 6765 735d 290a 2020 2020 2020 2020  edges]).        
-0000bb70: 666f 7220 7462 2069 6e20 7462 733a 0a20  for tb in tbs:. 
-0000bb80: 2020 2020 2020 2020 2020 2065 6467 6573             edges
-0000bb90: 203d 2066 6c61 7474 656e 2874 6229 0a20   = flatten(tb). 
-0000bba0: 2020 2020 2020 2020 2020 2072 765f 6465             rv_de
-0000bbb0: 6665 6174 203d 2053 504f 286c 656e 2863  feat = SPO(len(c
-0000bbc0: 616e 6469 6461 7465 7329 290a 2020 2020  andidates)).    
-0000bbd0: 2020 2020 2020 2020 666f 7220 6530 2c65          for e0,e
-0000bbe0: 312c 7320 696e 2065 6467 6573 3a20 0a20  1,s in edges: . 
-0000bbf0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000bc00: 6620 6e6f 7420 7276 5f64 6566 6561 742e  f not rv_defeat.
-0000bc10: 505b 6361 6e64 5f74 6f5f 6369 6478 5b65  P[cand_to_cidx[e
-0000bc20: 315d 5d5b 6361 6e64 5f74 6f5f 6369 6478  1]][cand_to_cidx
-0000bc30: 5b65 305d 5d20 616e 6420 6c65 6e28 7276  [e0]] and len(rv
-0000bc40: 5f64 6566 6561 742e 7072 6564 735b 6361  _defeat.preds[ca
-0000bc50: 6e64 5f74 6f5f 6369 6478 5b65 315d 5d29  nd_to_cidx[e1]])
-0000bc60: 203d 3d20 303a 0a20 2020 2020 2020 2020   == 0:.         
-0000bc70: 2020 2020 2020 2020 2020 2072 765f 6465             rv_de
-0000bc80: 6665 6174 2e61 6464 2863 616e 645f 746f  feat.add(cand_to
-0000bc90: 5f63 6964 785b 6530 5d2c 6361 6e64 5f74  _cidx[e0],cand_t
-0000bca0: 6f5f 6369 6478 5b65 315d 290a 2020 2020  o_cidx[e1]).    
-0000bcb0: 2020 2020 2020 2020 7769 6e6e 6572 732e          winners.
-0000bcc0: 6170 7065 6e64 2863 6964 785f 746f 5f63  append(cidx_to_c
-0000bcd0: 616e 645b 7276 5f64 6566 6561 742e 696e  and[rv_defeat.in
-0000bce0: 6974 6961 6c5f 656c 656d 656e 7473 2829  itial_elements()
-0000bcf0: 5b30 5d5d 290a 0a20 2020 2072 6574 7572  [0]])..    retur
-0000bd00: 6e20 736f 7274 6564 286c 6973 7428 7365  n sorted(list(se
-0000bd10: 7428 7769 6e6e 6572 7329 2929 0a0a 6465  t(winners)))..de
-0000bd20: 6620 7269 7665 725f 6465 6665 6174 7328  f river_defeats(
-0000bd30: 6564 6174 612c 2063 7572 725f 6361 6e64  edata, curr_cand
-0000bd40: 7320 3d20 4e6f 6e65 2c20 7374 7265 6e67  s = None, streng
-0000bd50: 7468 5f66 756e 6374 696f 6e20 3d20 4e6f  th_function = No
-0000bd60: 6e65 293a 0a20 2020 2022 2222 0a20 2020  ne):.    """.   
-0000bd70: 2052 6574 7572 6e73 2074 6865 2052 6976   Returns the Riv
-0000bd80: 6572 2064 6566 6561 7420 7265 6c61 7469  er defeat relati
-0000bd90: 6f6e 7320 7072 6f64 7563 6564 2062 7920  ons produced by 
-0000bda0: 7468 6520 5269 7665 7220 616c 676f 7269  the River algori
-0000bdb0: 7468 6d2e 0a0a 2020 2020 2e2e 2069 6d70  thm...    .. imp
-0000bdc0: 6f72 7461 6e74 3a3a 0a20 2020 2020 2020  ortant::.       
-0000bdd0: 2055 6e6c 696b 6520 7468 6520 6f74 6865   Unlike the othe
-0000bde0: 7220 6675 6e63 7469 6f6e 7320 7468 6174  r functions that
-0000bdf0: 2072 6574 7572 6e20 6120 7369 6e67 6c65   return a single
-0000be00: 2064 6566 6561 7420 7265 6c61 7469 6f6e   defeat relation
-0000be10: 2c20 7468 6973 2072 6574 7572 6e73 2061  , this returns a
-0000be20: 206c 6973 7420 6f66 2064 6566 6561 7420   list of defeat 
-0000be30: 7265 6c61 7469 6f6e 732e 200a 2020 2020  relations. .    
-0000be40: 2020 2020 0a20 2020 2041 7267 733a 0a20      .    Args:. 
-0000be50: 2020 2020 2020 2065 6461 7461 2028 5072         edata (Pr
-0000be60: 6f66 696c 652c 2050 726f 6669 6c65 5769  ofile, ProfileWi
-0000be70: 7468 5469 6573 2c20 4d61 7267 696e 4772  thTies, MarginGr
-0000be80: 6170 6829 3a20 416e 7920 656c 6563 7469  aph): Any electi
-0000be90: 6f6e 2064 6174 6120 7468 6174 2068 6173  on data that has
-0000bea0: 2061 2060 6d61 7267 696e 6020 6d65 7468   a `margin` meth
-0000beb0: 6f64 2e20 0a20 2020 2020 2020 2063 7572  od. .        cur
-0000bec0: 725f 6361 6e64 7320 284c 6973 745b 696e  r_cands (List[in
-0000bed0: 745d 2c20 6f70 7469 6f6e 616c 293a 2049  t], optional): I
-0000bee0: 6620 7365 742c 2074 6865 6e20 6669 6e64  f set, then find
-0000bef0: 2074 6865 2077 696e 6e65 7273 2066 6f72   the winners for
-0000bf00: 2074 6865 2070 726f 6669 6c65 2072 6573   the profile res
-0000bf10: 7472 6963 7465 6420 746f 2074 6865 2063  tricted to the c
-0000bf20: 616e 6469 6461 7465 7320 696e 2060 6063  andidates in ``c
-0000bf30: 7572 725f 6361 6e64 7360 600a 2020 2020  urr_cands``.    
-0000bf40: 2020 2020 7374 7265 6e67 7468 5f66 756e      strength_fun
-0000bf50: 6374 696f 6e20 2866 756e 6374 696f 6e2c  ction (function,
-0000bf60: 206f 7074 696f 6e61 6c29 3a20 5468 6520   optional): The 
-0000bf70: 7374 7265 6e67 7468 2066 756e 6374 696f  strength functio
-0000bf80: 6e20 746f 2062 6520 7573 6564 2074 6f20  n to be used to 
-0000bf90: 6361 6c63 756c 6174 6520 7468 6520 7374  calculate the st
-0000bfa0: 7265 6e67 7468 206f 6620 6120 7061 7468  rength of a path
-0000bfb0: 2e20 2020 5468 6520 6465 6661 756c 7420  .   The default 
-0000bfc0: 6973 2074 6865 206d 6172 6769 6e20 6d65  is the margin me
-0000bfd0: 7468 6f64 206f 6620 6060 6564 6174 6160  thod of ``edata`
-0000bfe0: 602e 2020 2054 6869 7320 6f6e 6c79 206d  `.   This only m
-0000bff0: 6174 7465 7273 2077 6865 6e20 7468 6520  atters when the 
-0000c000: 6261 6c6c 6f74 7320 6172 6520 6e6f 7420  ballots are not 
-0000c010: 6c69 6e65 6172 206f 7264 6572 732e 200a  linear orders. .
-0000c020: 0a20 2020 2052 6574 7572 6e73 3a20 0a20  .    Returns: . 
-0000c030: 2020 2020 2020 2041 206e 6574 776f 726b         A network
-0000c040: 7820 4469 4772 6170 6820 7265 7072 6573  x DiGraph repres
-0000c050: 656e 7469 6e67 2074 6865 2052 6976 6572  enting the River
-0000c060: 2064 6566 6561 7420 7265 6c61 7469 6f6e   defeat relation
-0000c070: 2e20 0a20 2020 2022 2222 0a0a 2020 2020  . .    """..    
-0000c080: 6361 6e64 6964 6174 6573 203d 2065 6461  candidates = eda
-0000c090: 7461 2e63 616e 6469 6461 7465 7320 6966  ta.candidates if
-0000c0a0: 2063 7572 725f 6361 6e64 7320 6973 204e   curr_cands is N
-0000c0b0: 6f6e 6520 656c 7365 2063 7572 725f 6361  one else curr_ca
-0000c0c0: 6e64 7320 2020 200a 2020 2020 7374 7265  nds    .    stre
-0000c0d0: 6e67 7468 5f66 756e 6374 696f 6e20 3d20  ngth_function = 
-0000c0e0: 6564 6174 612e 6d61 7267 696e 2069 6620  edata.margin if 
-0000c0f0: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
-0000c100: 6e20 6973 204e 6f6e 6520 656c 7365 2073  n is None else s
-0000c110: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
-0000c120: 2020 2020 0a0a 2020 2020 775f 6564 6765      ..    w_edge
-0000c130: 7320 3d20 5b28 6331 2c20 6332 2c20 7374  s = [(c1, c2, st
-0000c140: 7265 6e67 7468 5f66 756e 6374 696f 6e28  rength_function(
-0000c150: 6331 2c20 6332 2929 2066 6f72 2063 3120  c1, c2)) for c1 
-0000c160: 696e 2063 616e 6469 6461 7465 7320 666f  in candidates fo
-0000c170: 7220 6332 2069 6e20 6361 6e64 6964 6174  r c2 in candidat
-0000c180: 6573 2069 6620 6331 2021 3d20 6332 2061  es if c1 != c2 a
-0000c190: 6e64 2028 6564 6174 612e 6d61 6a6f 7269  nd (edata.majori
-0000c1a0: 7479 5f70 7265 6665 7273 2863 312c 2063  ty_prefers(c1, c
-0000c1b0: 3229 206f 7220 6564 6174 612e 6973 5f74  2) or edata.is_t
-0000c1c0: 6965 6428 6331 2c20 6332 2929 5d0a 0a20  ied(c1, c2))].. 
-0000c1d0: 2020 2073 7472 656e 6774 6873 203d 2073     strengths = s
-0000c1e0: 6f72 7465 6428 6c69 7374 2873 6574 285b  orted(list(set([
-0000c1f0: 655b 325d 2066 6f72 2065 2069 6e20 775f  e[2] for e in w_
-0000c200: 6564 6765 735d 2929 2c20 7265 7665 7273  edges])), revers
-0000c210: 653d 5472 7565 290a 2020 2020 736f 7274  e=True).    sort
-0000c220: 6564 5f65 6467 6573 203d 205b 5b65 2066  ed_edges = [[e f
-0000c230: 6f72 2065 2069 6e20 775f 6564 6765 7320  or e in w_edges 
-0000c240: 6966 2065 5b32 5d20 3d3d 2073 5d20 666f  if e[2] == s] fo
-0000c250: 7220 7320 696e 2073 7472 656e 6774 6873  r s in strengths
-0000c260: 5d0a 2020 2020 7462 7320 3d20 7072 6f64  ].    tbs = prod
-0000c270: 7563 7428 2a5b 7065 726d 7574 6174 696f  uct(*[permutatio
-0000c280: 6e73 2865 6467 6573 2920 666f 7220 6564  ns(edges) for ed
-0000c290: 6765 7320 696e 2073 6f72 7465 645f 6564  ges in sorted_ed
-0000c2a0: 6765 735d 290a 0a20 2020 2072 6976 6572  ges])..    river
-0000c2b0: 5f64 6566 6561 7473 203d 206c 6973 7428  _defeats = list(
-0000c2c0: 290a 2020 2020 666f 7220 7462 2069 6e20  ).    for tb in 
-0000c2d0: 7462 733a 0a20 2020 2020 2020 2065 6467  tbs:.        edg
-0000c2e0: 6573 203d 2066 6c61 7474 656e 2874 6229  es = flatten(tb)
-0000c2f0: 0a20 2020 2020 2020 2072 6976 6572 5f64  .        river_d
-0000c300: 6566 6561 7420 3d20 6e78 2e44 6947 7261  efeat = nx.DiGra
-0000c310: 7068 2829 200a 2020 2020 2020 2020 666f  ph() .        fo
-0000c320: 7220 6520 696e 2065 6467 6573 3a20 0a20  r e in edges: . 
-0000c330: 2020 2020 2020 2020 2020 2069 6620 655b             if e[
-0000c340: 315d 206e 6f74 2069 6e20 7269 7665 725f  1] not in river_
-0000c350: 6465 6665 6174 2e6e 6f64 6573 206f 7220  defeat.nodes or 
-0000c360: 6c65 6e28 6c69 7374 2872 6976 6572 5f64  len(list(river_d
-0000c370: 6566 6561 742e 696e 5f65 6467 6573 2865  efeat.in_edges(e
-0000c380: 5b31 5d29 2929 203d 3d20 303a 0a20 2020  [1]))) == 0:.   
-0000c390: 2020 2020 2020 2020 2020 2020 2072 6976               riv
-0000c3a0: 6572 5f64 6566 6561 742e 6164 645f 6564  er_defeat.add_ed
-0000c3b0: 6765 2865 5b30 5d2c 2065 5b31 5d2c 2077  ge(e[0], e[1], w
-0000c3c0: 6569 6768 743d 655b 325d 290a 2020 2020  eight=e[2]).    
-0000c3d0: 2020 2020 2020 2020 2020 2020 6966 2064              if d
-0000c3e0: 6f65 735f 6372 6561 7465 5f63 7963 6c65  oes_create_cycle
-0000c3f0: 2872 6976 6572 5f64 6566 6561 742c 2065  (river_defeat, e
-0000c400: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0000c410: 2020 2020 2020 2072 6976 6572 5f64 6566         river_def
-0000c420: 6561 742e 7265 6d6f 7665 5f65 6467 6528  eat.remove_edge(
-0000c430: 655b 305d 2c20 655b 315d 290a 2020 2020  e[0], e[1]).    
-0000c440: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-0000c450: 2072 6976 6572 5f64 6566 6561 7473 2e61   river_defeats.a
-0000c460: 7070 656e 6428 7269 7665 725f 6465 6665  ppend(river_defe
-0000c470: 6174 290a 0a20 2020 2072 6574 7572 6e20  at)..    return 
-0000c480: 7269 7665 725f 6465 6665 6174 730a 0a40  river_defeats..@
-0000c490: 766d 286e 616d 653d 2252 6976 6572 222c  vm(name="River",
-0000c4a0: 0a20 2020 2073 6b69 705f 7265 6769 7374  .    skip_regist
-0000c4b0: 7261 7469 6f6e 3d54 7275 6529 0a64 6566  ration=True).def
-0000c4c0: 2072 6976 6572 5f77 6974 685f 7465 7374   river_with_test
-0000c4d0: 2865 6461 7461 2c20 6375 7272 5f63 616e  (edata, curr_can
-0000c4e0: 6473 203d 204e 6f6e 652c 2073 7472 656e  ds = None, stren
-0000c4f0: 6774 685f 6675 6e63 7469 6f6e 203d 204e  gth_function = N
-0000c500: 6f6e 6529 3a20 2020 0a20 2020 2022 2222  one):   .    """
-0000c510: 4669 6e64 2074 6865 2052 6976 6572 2077  Find the River w
-0000c520: 696e 6e65 7273 2077 6974 6820 6120 7465  inners with a te
-0000c530: 7374 2074 6f20 6465 7465 726d 696e 6564  st to determined
-0000c540: 2069 6620 6974 2077 696c 6c20 7461 6b65   if it will take
-0000c550: 2074 6f6f 206c 6f6e 6720 746f 2063 6f6d   too long to com
-0000c560: 7075 7465 2074 6865 2052 6976 6572 2077  pute the River w
-0000c570: 696e 6e65 7273 2e20 4966 2074 6865 2063  inners. If the c
-0000c580: 616c 6375 6c61 7469 6f6e 206f 6620 7468  alculation of th
-0000c590: 6520 7769 6e6e 6572 7320 7769 6c6c 2074  e winners will t
-0000c5a0: 616b 6520 746f 6f20 6c6f 6e67 2c20 7265  ake too long, re
-0000c5b0: 7475 726e 204e 6f6e 652e 200a 2020 2020  turn None. .    
-0000c5c0: 2020 2020 0a20 2020 202e 2e20 696d 706f      .    .. impo
-0000c5d0: 7274 616e 743a 3a0a 2020 2020 2020 2020  rtant::.        
-0000c5e0: 5468 6973 2076 6f74 696e 6720 6d65 7468  This voting meth
-0000c5f0: 6f64 2074 6861 7420 6d69 6768 7420 7265  od that might re
-0000c600: 7475 726e 204e 6f6e 6520 7261 7468 6572  turn None rather
-0000c610: 2074 6861 6e20 6120 6c69 7374 206f 6620   than a list of 
-0000c620: 6361 6e64 6964 6174 6573 2e20 200a 0a20  candidates.  .. 
-0000c630: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
-0000c640: 2065 6461 7461 2028 5072 6f66 696c 652c   edata (Profile,
-0000c650: 2050 726f 6669 6c65 5769 7468 5469 6573   ProfileWithTies
-0000c660: 2c20 4d61 7267 696e 4772 6170 6829 3a20  , MarginGraph): 
-0000c670: 416e 7920 656c 6563 7469 6f6e 2064 6174  Any election dat
-0000c680: 6120 7468 6174 2068 6173 2061 2060 6d61  a that has a `ma
-0000c690: 7267 696e 6020 6d65 7468 6f64 2e20 0a20  rgin` method. . 
-0000c6a0: 2020 2020 2020 2063 7572 725f 6361 6e64         curr_cand
-0000c6b0: 7320 284c 6973 745b 696e 745d 2c20 6f70  s (List[int], op
-0000c6c0: 7469 6f6e 616c 293a 2049 6620 7365 742c  tional): If set,
-0000c6d0: 2074 6865 6e20 6669 6e64 2074 6865 2077   then find the w
-0000c6e0: 696e 6e65 7273 2066 6f72 2074 6865 2070  inners for the p
-0000c6f0: 726f 6669 6c65 2072 6573 7472 6963 7465  rofile restricte
-0000c700: 6420 746f 2074 6865 2063 616e 6469 6461  d to the candida
-0000c710: 7465 7320 696e 2060 6063 7572 725f 6361  tes in ``curr_ca
-0000c720: 6e64 7360 600a 2020 2020 2020 2020 7374  nds``.        st
-0000c730: 7265 6e67 7468 5f66 756e 6374 696f 6e20  rength_function 
-0000c740: 2866 756e 6374 696f 6e2c 206f 7074 696f  (function, optio
-0000c750: 6e61 6c29 3a20 5468 6520 7374 7265 6e67  nal): The streng
-0000c760: 7468 2066 756e 6374 696f 6e20 746f 2062  th function to b
-0000c770: 6520 7573 6564 2074 6f20 6361 6c63 756c  e used to calcul
-0000c780: 6174 6520 7468 6520 7374 7265 6e67 7468  ate the strength
-0000c790: 206f 6620 6120 7061 7468 2e20 2020 5468   of a path.   Th
-0000c7a0: 6520 6465 6661 756c 7420 6973 2074 6865  e default is the
-0000c7b0: 206d 6172 6769 6e20 6d65 7468 6f64 206f   margin method o
-0000c7c0: 6620 6060 6564 6174 6160 602e 2020 2054  f ``edata``.   T
-0000c7d0: 6869 7320 6f6e 6c79 206d 6174 7465 7273  his only matters
-0000c7e0: 2077 6865 6e20 7468 6520 6261 6c6c 6f74   when the ballot
-0000c7f0: 7320 6172 6520 6e6f 7420 6c69 6e65 6172  s are not linear
-0000c800: 206f 7264 6572 732e 200a 0a20 2020 2052   orders. ..    R
-0000c810: 6574 7572 6e73 3a20 0a20 2020 2020 2020  eturns: .       
-0000c820: 2041 2073 6f72 7465 6420 6c69 7374 206f   A sorted list o
-0000c830: 6620 6361 6e64 6964 6174 6573 2e20 0a0a  f candidates. ..
-0000c840: 2020 2020 2e2e 2073 6565 616c 736f 3a3a      .. seealso::
-0000c850: 0a0a 2020 2020 2020 2020 3a6d 6574 683a  ..        :meth:
-0000c860: 6070 7265 665f 766f 7469 6e67 2e6d 6172  `pref_voting.mar
-0000c870: 6769 6e5f 6261 7365 645f 6d65 7468 6f64  gin_based_method
-0000c880: 732e 7261 6e6b 6564 5f70 6169 7273 5f77  s.ranked_pairs_w
-0000c890: 6974 685f 7465 7374 602c 203a 6d65 7468  ith_test`, :meth
-0000c8a0: 3a60 7072 6566 5f76 6f74 696e 672e 6d61  :`pref_voting.ma
-0000c8b0: 7267 696e 5f62 6173 6564 5f6d 6574 686f  rgin_based_metho
-0000c8c0: 6473 2e72 6976 6572 600a 0a20 2020 2022  ds.river`..    "
-0000c8d0: 2222 0a20 2020 2063 616e 6469 6461 7465  "".    candidate
-0000c8e0: 7320 3d20 6564 6174 612e 6361 6e64 6964  s = edata.candid
-0000c8f0: 6174 6573 2069 6620 6375 7272 5f63 616e  ates if curr_can
-0000c900: 6473 2069 7320 4e6f 6e65 2065 6c73 6520  ds is None else 
-0000c910: 6375 7272 5f63 616e 6473 2020 2020 0a20  curr_cands    . 
-0000c920: 2020 2063 6964 785f 746f 5f63 616e 6420     cidx_to_cand 
-0000c930: 3d20 7b63 6964 783a 2063 2066 6f72 2063  = {cidx: c for c
-0000c940: 6964 782c 2063 2069 6e20 656e 756d 6572  idx, c in enumer
-0000c950: 6174 6528 6361 6e64 6964 6174 6573 297d  ate(candidates)}
-0000c960: 2020 0a20 2020 2063 616e 645f 746f 5f63    .    cand_to_c
-0000c970: 6964 7820 3d20 7b63 3a20 6369 6478 2066  idx = {c: cidx f
-0000c980: 6f72 2063 6964 782c 2063 2069 6e20 656e  or cidx, c in en
-0000c990: 756d 6572 6174 6528 6361 6e64 6964 6174  umerate(candidat
-0000c9a0: 6573 297d 2020 0a0a 2020 2020 7374 7265  es)}  ..    stre
-0000c9b0: 6e67 7468 5f66 756e 6374 696f 6e20 3d20  ngth_function = 
-0000c9c0: 6564 6174 612e 6d61 7267 696e 2069 6620  edata.margin if 
-0000c9d0: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
-0000c9e0: 6e20 6973 204e 6f6e 6520 656c 7365 2073  n is None else s
-0000c9f0: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
-0000ca00: 2020 2020 0a0a 2020 2020 6377 203d 2065      ..    cw = e
-0000ca10: 6461 7461 2e63 6f6e 646f 7263 6574 5f77  data.condorcet_w
-0000ca20: 696e 6e65 7228 6375 7272 5f63 616e 6473  inner(curr_cands
-0000ca30: 3d63 7572 725f 6361 6e64 7329 0a20 2020  =curr_cands).   
-0000ca40: 2023 2052 616e 6b65 6420 5061 6972 7320   # Ranked Pairs 
-0000ca50: 6973 2043 6f6e 646f 7263 6574 2063 6f6e  is Condorcet con
-0000ca60: 7369 7374 656e 742c 2073 6f20 7369 6d70  sistent, so simp
-0000ca70: 6c79 2072 6574 7572 6e20 7468 6520 436f  ly return the Co
-0000ca80: 6e64 6f72 6365 7420 7769 6e6e 6572 2069  ndorcet winner i
-0000ca90: 6620 6578 6973 7473 0a20 2020 2069 6620  f exists.    if 
-0000caa0: 6377 2069 7320 6e6f 7420 4e6f 6e65 3a20  cw is not None: 
-0000cab0: 0a20 2020 2020 2020 2077 696e 6e65 7273  .        winners
-0000cac0: 203d 205b 6377 5d0a 2020 2020 656c 7365   = [cw].    else
-0000cad0: 3a0a 2020 2020 2020 2020 775f 6564 6765  :.        w_edge
-0000cae0: 7320 3d20 5b28 6331 2c20 6332 2c20 7374  s = [(c1, c2, st
-0000caf0: 7265 6e67 7468 5f66 756e 6374 696f 6e28  rength_function(
-0000cb00: 6331 2c20 6332 2929 2066 6f72 2063 3120  c1, c2)) for c1 
-0000cb10: 696e 2063 616e 6469 6461 7465 7320 666f  in candidates fo
-0000cb20: 7220 6332 2069 6e20 6361 6e64 6964 6174  r c2 in candidat
-0000cb30: 6573 200a 2020 2020 2020 2020 2020 2020  es .            
-0000cb40: 2020 2020 2020 2069 6620 6331 2021 3d20         if c1 != 
-0000cb50: 6332 2061 6e64 2028 6564 6174 612e 6d61  c2 and (edata.ma
-0000cb60: 6a6f 7269 7479 5f70 7265 6665 7273 2863  jority_prefers(c
-0000cb70: 312c 2063 3229 206f 7220 6564 6174 612e  1, c2) or edata.
-0000cb80: 6973 5f74 6965 6428 6331 2c20 6332 2929  is_tied(c1, c2))
-0000cb90: 5d0a 2020 2020 2020 2020 7769 6e6e 6572  ].        winner
-0000cba0: 7320 3d20 6c69 7374 2829 2020 2020 2020  s = list()      
-0000cbb0: 2020 2020 2020 0a20 2020 2020 2020 2073        .        s
-0000cbc0: 7472 656e 6774 6873 203d 2073 6f72 7465  trengths = sorte
-0000cbd0: 6428 6c69 7374 2873 6574 285b 655b 325d  d(list(set([e[2]
-0000cbe0: 2066 6f72 2065 2069 6e20 775f 6564 6765   for e in w_edge
-0000cbf0: 735d 2929 2c20 7265 7665 7273 653d 5472  s])), reverse=Tr
-0000cc00: 7565 290a 2020 2020 2020 2020 736f 7274  ue).        sort
-0000cc10: 6564 5f65 6467 6573 203d 205b 5b65 2066  ed_edges = [[e f
-0000cc20: 6f72 2065 2069 6e20 775f 6564 6765 7320  or e in w_edges 
-0000cc30: 6966 2065 5b32 5d20 3d3d 2073 5d20 666f  if e[2] == s] fo
-0000cc40: 7220 7320 696e 2073 7472 656e 6774 6873  r s in strengths
-0000cc50: 5d0a 2020 2020 2020 2020 6966 206e 702e  ].        if np.
-0000cc60: 7072 6f64 285b 6d61 7468 2e66 6163 746f  prod([math.facto
-0000cc70: 7269 616c 286c 656e 2865 7329 2920 666f  rial(len(es)) fo
-0000cc80: 7220 6573 2069 6e20 736f 7274 6564 5f65  r es in sorted_e
-0000cc90: 6467 6573 5d29 203e 2033 3030 303a 200a  dges]) > 3000: .
-0000cca0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000ccb0: 726e 204e 6f6e 650a 2020 2020 2020 2020  rn None.        
-0000ccc0: 656c 7365 3a20 0a20 2020 2020 2020 2020  else: .         
-0000ccd0: 2020 2074 6273 203d 2070 726f 6475 6374     tbs = product
-0000cce0: 282a 5b70 6572 6d75 7461 7469 6f6e 7328  (*[permutations(
-0000ccf0: 6564 6765 7329 2066 6f72 2065 6467 6573  edges) for edges
-0000cd00: 2069 6e20 736f 7274 6564 5f65 6467 6573   in sorted_edges
-0000cd10: 5d29 0a20 2020 2020 2020 2020 2020 2066  ]).            f
-0000cd20: 6f72 2074 6220 696e 2074 6273 3a0a 2020  or tb in tbs:.  
-0000cd30: 2020 2020 2020 2020 2020 2020 2020 6564                ed
-0000cd40: 6765 7320 3d20 666c 6174 7465 6e28 7462  ges = flatten(tb
-0000cd50: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000cd60: 2020 7276 5f64 6566 6561 7420 3d20 5350    rv_defeat = SP
-0000cd70: 4f28 6c65 6e28 6361 6e64 6964 6174 6573  O(len(candidates
-0000cd80: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
-0000cd90: 2020 2066 6f72 2065 302c 6531 2c73 2069     for e0,e1,s i
-0000cda0: 6e20 6564 6765 733a 200a 2020 2020 2020  n edges: .      
-0000cdb0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0000cdc0: 206e 6f74 2072 765f 6465 6665 6174 2e50   not rv_defeat.P
-0000cdd0: 5b63 616e 645f 746f 5f63 6964 785b 6531  [cand_to_cidx[e1
-0000cde0: 5d5d 5b63 616e 645f 746f 5f63 6964 785b  ]][cand_to_cidx[
-0000cdf0: 6530 5d5d 2061 6e64 206c 656e 2872 765f  e0]] and len(rv_
-0000ce00: 6465 6665 6174 2e70 7265 6473 5b63 616e  defeat.preds[can
-0000ce10: 645f 746f 5f63 6964 785b 6531 5d5d 2920  d_to_cidx[e1]]) 
-0000ce20: 3d3d 2030 3a0a 2020 2020 2020 2020 2020  == 0:.          
-0000ce30: 2020 2020 2020 2020 2020 2020 2020 7276                rv
-0000ce40: 5f64 6566 6561 742e 6164 6428 6361 6e64  _defeat.add(cand
-0000ce50: 5f74 6f5f 6369 6478 5b65 305d 2c63 616e  _to_cidx[e0],can
-0000ce60: 645f 746f 5f63 6964 785b 6531 5d29 0a20  d_to_cidx[e1]). 
-0000ce70: 2020 2020 2020 2020 2020 2020 2020 2077                 w
-0000ce80: 696e 6e65 7273 2e61 7070 656e 6428 6369  inners.append(ci
-0000ce90: 6478 5f74 6f5f 6361 6e64 5b72 765f 6465  dx_to_cand[rv_de
-0000cea0: 6665 6174 2e69 6e69 7469 616c 5f65 6c65  feat.initial_ele
-0000ceb0: 6d65 6e74 7328 295b 305d 5d29 0a20 2020  ments()[0]]).   
-0000cec0: 2072 6574 7572 6e20 736f 7274 6564 286c   return sorted(l
-0000ced0: 6973 7428 7365 7428 7769 6e6e 6572 7329  ist(set(winners)
-0000cee0: 2929 0a0a 7270 5f74 625f 7072 6f70 6572  ))..rp_tb_proper
-0000cef0: 7469 6573 203d 2056 6f74 696e 674d 6574  ties = VotingMet
-0000cf00: 686f 6450 726f 7065 7274 6965 7328 0a20  hodProperties(. 
-0000cf10: 2020 2063 6f6e 646f 7263 6574 5f77 696e     condorcet_win
-0000cf20: 6e65 723d 5472 7565 2c20 0a20 2020 2063  ner=True, .    c
-0000cf30: 6f6e 646f 7263 6574 5f6c 6f73 6572 3d54  ondorcet_loser=T
-0000cf40: 7275 652c 0a20 2020 2070 6172 6574 6f5f  rue,.    pareto_
-0000cf50: 646f 6d69 6e61 6e63 653d 5472 7565 2c0a  dominance=True,.
-0000cf60: 2020 2020 706f 7369 7469 7665 5f69 6e76      positive_inv
-0000cf70: 6f6c 7665 6d65 6e74 3d46 616c 7365 2c20  olvement=False, 
-0000cf80: 0a20 2020 2029 0a40 766d 286e 616d 653d  .    ).@vm(name=
-0000cf90: 2252 6976 6572 2054 4222 2c0a 2020 2020  "River TB",.    
-0000cfa0: 7072 6f70 6572 7469 6573 3d72 705f 7462  properties=rp_tb
-0000cfb0: 5f70 726f 7065 7274 6965 732c 0a20 2020  _properties,.   
-0000cfc0: 2069 6e70 7574 5f74 7970 6573 3d5b 456c   input_types=[El
-0000cfd0: 6563 7469 6f6e 5479 7065 732e 5052 4f46  ectionTypes.PROF
-0000cfe0: 494c 452c 2045 6c65 6374 696f 6e54 7970  ILE, ElectionTyp
-0000cff0: 6573 2e50 524f 4649 4c45 5f57 4954 485f  es.PROFILE_WITH_
-0000d000: 5449 4553 2c20 456c 6563 7469 6f6e 5479  TIES, ElectionTy
-0000d010: 7065 732e 4d41 5247 494e 5f47 5241 5048  pes.MARGIN_GRAPH
-0000d020: 5d29 0a64 6566 2072 6976 6572 5f74 6228  ]).def river_tb(
-0000d030: 6564 6174 612c 2063 7572 725f 6361 6e64  edata, curr_cand
-0000d040: 7320 3d20 4e6f 6e65 2c20 7469 655f 6272  s = None, tie_br
-0000d050: 6561 6b65 7220 3d20 4e6f 6e65 2c20 7374  eaker = None, st
-0000d060: 7265 6e67 7468 5f66 756e 6374 696f 6e20  rength_function 
-0000d070: 3d20 4e6f 6e65 293a 2020 200a 2020 2020  = None):   .    
-0000d080: 2222 220a 2020 2020 5269 7665 7220 7769  """.    River wi
-0000d090: 7468 2061 2066 6978 6564 206c 696e 6561  th a fixed linea
-0000d0a0: 7220 6f72 6465 7220 6f6e 2074 6865 2063  r order on the c
-0000d0b0: 616e 6469 6461 7465 7320 746f 2062 7265  andidates to bre
-0000d0c0: 616b 2061 6e79 2074 6965 7320 696e 2074  ak any ties in t
-0000d0d0: 6865 206d 6172 6769 6e73 2e20 2053 696e  he margins.  Sin
-0000d0e0: 6365 2074 6865 2074 6965 5f62 7265 616b  ce the tie_break
-0000d0f0: 6572 2069 7320 6120 6c69 6e65 6172 206f  er is a linear o
-0000d100: 7264 6572 2c20 7468 6973 206d 6574 686f  rder, this metho
-0000d110: 6420 6973 2072 6573 6f6c 7574 652e 2020  d is resolute.  
-0000d120: 200a 0a20 2020 2041 7267 733a 0a20 2020   ..    Args:.   
-0000d130: 2020 2020 2065 6461 7461 2028 5072 6f66       edata (Prof
-0000d140: 696c 652c 2050 726f 6669 6c65 5769 7468  ile, ProfileWith
-0000d150: 5469 6573 2c20 4d61 7267 696e 4772 6170  Ties, MarginGrap
-0000d160: 6829 3a20 416e 7920 656c 6563 7469 6f6e  h): Any election
-0000d170: 2064 6174 6120 7468 6174 2068 6173 2061   data that has a
-0000d180: 2060 6d61 7267 696e 6020 6d65 7468 6f64   `margin` method
-0000d190: 2e20 0a20 2020 2020 2020 2063 7572 725f  . .        curr_
-0000d1a0: 6361 6e64 7320 284c 6973 745b 696e 745d  cands (List[int]
-0000d1b0: 2c20 6f70 7469 6f6e 616c 293a 2049 6620  , optional): If 
-0000d1c0: 7365 742c 2074 6865 6e20 6669 6e64 2074  set, then find t
-0000d1d0: 6865 2077 696e 6e65 7273 2066 6f72 2074  he winners for t
-0000d1e0: 6865 2070 726f 6669 6c65 2072 6573 7472  he profile restr
-0000d1f0: 6963 7465 6420 746f 2074 6865 2063 616e  icted to the can
-0000d200: 6469 6461 7465 7320 696e 2060 6063 7572  didates in ``cur
-0000d210: 725f 6361 6e64 7360 600a 2020 2020 2020  r_cands``.      
-0000d220: 2020 7469 655f 6272 6561 6b65 7220 284c    tie_breaker (L
-0000d230: 6973 745b 696e 745d 2c20 6f70 7469 6f6e  ist[int], option
-0000d240: 616c 293a 2041 206c 696e 6561 7220 6f72  al): A linear or
-0000d250: 6465 7220 6f6e 2074 6865 2063 616e 6469  der on the candi
-0000d260: 6461 7465 732e 2020 4966 206e 6f74 2073  dates.  If not s
-0000d270: 6574 2c20 7468 656e 2074 6865 2063 616e  et, then the can
-0000d280: 6469 6461 7465 7320 6172 6520 736f 7274  didates are sort
-0000d290: 6564 2069 6e20 6173 6365 6e64 696e 6720  ed in ascending 
-0000d2a0: 6f72 6465 722e 0a20 2020 2020 2020 2073  order..        s
-0000d2b0: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
-0000d2c0: 2028 6675 6e63 7469 6f6e 2c20 6f70 7469   (function, opti
-0000d2d0: 6f6e 616c 293a 2054 6865 2073 7472 656e  onal): The stren
-0000d2e0: 6774 6820 6675 6e63 7469 6f6e 2074 6f20  gth function to 
-0000d2f0: 6265 2075 7365 6420 746f 2063 616c 6375  be used to calcu
-0000d300: 6c61 7465 2074 6865 2073 7472 656e 6774  late the strengt
-0000d310: 6820 6f66 2061 2070 6174 682e 2020 2054  h of a path.   T
-0000d320: 6865 2064 6566 6175 6c74 2069 7320 7468  he default is th
-0000d330: 6520 6d61 7267 696e 206d 6574 686f 6420  e margin method 
-0000d340: 6f66 2060 6065 6461 7461 6060 2e20 2020  of ``edata``.   
-0000d350: 5468 6973 206f 6e6c 7920 6d61 7474 6572  This only matter
-0000d360: 7320 7768 656e 2074 6865 2062 616c 6c6f  s when the ballo
-0000d370: 7473 2061 7265 206e 6f74 206c 696e 6561  ts are not linea
-0000d380: 7220 6f72 6465 7273 2e20 0a0a 2020 2020  r orders. ..    
-0000d390: 5265 7475 726e 733a 200a 2020 2020 2020  Returns: .      
-0000d3a0: 2020 4120 736f 7274 6564 206c 6973 7420    A sorted list 
-0000d3b0: 6f66 2063 616e 6469 6461 7465 732e 200a  of candidates. .
-0000d3c0: 0a20 2020 2022 2222 0a20 2020 2063 616e  .    """.    can
-0000d3d0: 6469 6461 7465 7320 3d20 6564 6174 612e  didates = edata.
-0000d3e0: 6361 6e64 6964 6174 6573 2069 6620 6375  candidates if cu
-0000d3f0: 7272 5f63 616e 6473 2069 7320 4e6f 6e65  rr_cands is None
-0000d400: 2065 6c73 6520 6375 7272 5f63 616e 6473   else curr_cands
-0000d410: 2020 2020 0a20 2020 2063 6964 785f 746f      .    cidx_to
-0000d420: 5f63 616e 6420 3d20 7b63 6964 783a 2063  _cand = {cidx: c
-0000d430: 2066 6f72 2063 6964 782c 2063 2069 6e20   for cidx, c in 
-0000d440: 656e 756d 6572 6174 6528 6361 6e64 6964  enumerate(candid
-0000d450: 6174 6573 297d 2020 0a20 2020 2063 616e  ates)}  .    can
-0000d460: 645f 746f 5f63 6964 7820 3d20 7b63 3a20  d_to_cidx = {c: 
-0000d470: 6369 6478 2066 6f72 2063 6964 782c 2063  cidx for cidx, c
-0000d480: 2069 6e20 656e 756d 6572 6174 6528 6361   in enumerate(ca
-0000d490: 6e64 6964 6174 6573 297d 2020 0a20 2020  ndidates)}  .   
-0000d4a0: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
-0000d4b0: 6f6e 203d 2065 6461 7461 2e6d 6172 6769  on = edata.margi
-0000d4c0: 6e20 6966 2073 7472 656e 6774 685f 6675  n if strength_fu
-0000d4d0: 6e63 7469 6f6e 2069 7320 4e6f 6e65 2065  nction is None e
-0000d4e0: 6c73 6520 7374 7265 6e67 7468 5f66 756e  lse strength_fun
-0000d4f0: 6374 696f 6e20 2020 200a 0a20 2020 2074  ction    ..    t
-0000d500: 625f 7261 6e6b 696e 6720 3d20 7469 655f  b_ranking = tie_
-0000d510: 6272 6561 6b65 7220 6966 2074 6965 5f62  breaker if tie_b
-0000d520: 7265 616b 6572 2069 7320 6e6f 7420 4e6f  reaker is not No
-0000d530: 6e65 2065 6c73 6520 736f 7274 6564 286c  ne else sorted(l
-0000d540: 6973 7428 6361 6e64 6964 6174 6573 2929  ist(candidates))
-0000d550: 0a0a 2020 2020 6377 203d 2065 6461 7461  ..    cw = edata
-0000d560: 2e63 6f6e 646f 7263 6574 5f77 696e 6e65  .condorcet_winne
-0000d570: 7228 6375 7272 5f63 616e 6473 3d63 7572  r(curr_cands=cur
-0000d580: 725f 6361 6e64 7329 0a20 2020 2023 2052  r_cands).    # R
-0000d590: 6976 6572 2069 7320 436f 6e64 6f72 6365  iver is Condorce
-0000d5a0: 7420 636f 6e73 6973 7465 6e74 2c20 736f  t consistent, so
-0000d5b0: 2073 696d 706c 7920 7265 7475 726e 2074   simply return t
-0000d5c0: 6865 2043 6f6e 646f 7263 6574 2077 696e  he Condorcet win
-0000d5d0: 6e65 7220 6966 2065 7869 7374 730a 2020  ner if exists.  
-0000d5e0: 2020 6966 2063 7720 6973 206e 6f74 204e    if cw is not N
-0000d5f0: 6f6e 653a 200a 2020 2020 2020 2020 7769  one: .        wi
-0000d600: 6e6e 6572 7320 3d20 5b63 775d 0a20 2020  nners = [cw].   
-0000d610: 2065 6c73 653a 0a20 2020 2020 2020 2077   else:.        w
-0000d620: 5f65 6467 6573 203d 205b 2863 312c 2063  _edges = [(c1, c
-0000d630: 322c 2073 7472 656e 6774 685f 6675 6e63  2, strength_func
-0000d640: 7469 6f6e 2863 312c 2063 3229 2920 666f  tion(c1, c2)) fo
-0000d650: 7220 6331 2069 6e20 6361 6e64 6964 6174  r c1 in candidat
-0000d660: 6573 2066 6f72 2063 3220 696e 2063 616e  es for c2 in can
-0000d670: 6469 6461 7465 7320 6966 2063 3120 213d  didates if c1 !=
-0000d680: 2063 3220 616e 6420 2865 6461 7461 2e6d   c2 and (edata.m
-0000d690: 616a 6f72 6974 795f 7072 6566 6572 7328  ajority_prefers(
-0000d6a0: 6331 2c20 6332 2920 6f72 2065 6461 7461  c1, c2) or edata
-0000d6b0: 2e69 735f 7469 6564 2863 312c 2063 3229  .is_tied(c1, c2)
-0000d6c0: 295d 0a20 2020 2020 2020 2077 696e 6e65  )].        winne
-0000d6d0: 7273 203d 206c 6973 7428 2920 200a 2020  rs = list()  .  
-0000d6e0: 2020 2020 2020 7374 7265 6e67 7468 7320        strengths 
-0000d6f0: 3d20 736f 7274 6564 286c 6973 7428 7365  = sorted(list(se
-0000d700: 7428 5b65 5b32 5d20 666f 7220 6520 696e  t([e[2] for e in
-0000d710: 2077 5f65 6467 6573 5d29 292c 2072 6576   w_edges])), rev
-0000d720: 6572 7365 3d54 7275 6529 0a0a 2020 2020  erse=True)..    
-0000d730: 2020 2020 7276 5f64 6566 6561 7420 3d20      rv_defeat = 
-0000d740: 5350 4f28 6c65 6e28 6361 6e64 6964 6174  SPO(len(candidat
-0000d750: 6573 2929 0a0a 2020 2020 2020 2020 666f  es))..        fo
-0000d760: 7220 7320 696e 2073 7472 656e 6774 6873  r s in strengths
-0000d770: 3a20 0a20 2020 2020 2020 2020 2020 2065  : .            e
-0000d780: 6467 6573 203d 205b 6520 666f 7220 6520  dges = [e for e 
-0000d790: 696e 2077 5f65 6467 6573 2069 6620 655b  in w_edges if e[
-0000d7a0: 325d 203d 3d20 735d 0a20 2020 2020 2020  2] == s].       
-0000d7b0: 2020 2020 200a 2020 2020 2020 2020 2020       .          
-0000d7c0: 2020 2320 6272 6561 6b20 7469 6573 2075    # break ties u
-0000d7d0: 7369 6e67 2074 6865 206c 6578 6963 6f67  sing the lexicog
-0000d7e0: 7261 7068 6963 206f 7264 6572 696e 6720  raphic ordering 
-0000d7f0: 6f6e 2074 7570 6c65 7320 6769 7665 6e20  on tuples given 
-0000d800: 7462 5f72 616e 6b69 6e67 0a20 2020 2020  tb_ranking.     
-0000d810: 2020 2020 2020 2073 6f72 7465 645f 6564         sorted_ed
-0000d820: 6765 7320 3d20 736f 7274 6564 2865 6467  ges = sorted(edg
-0000d830: 6573 2c20 6b65 7920 3d20 6c61 6d62 6461  es, key = lambda
-0000d840: 2065 3a20 2874 625f 7261 6e6b 696e 672e   e: (tb_ranking.
-0000d850: 696e 6465 7828 655b 305d 292c 2074 625f  index(e[0]), tb_
-0000d860: 7261 6e6b 696e 672e 696e 6465 7828 655b  ranking.index(e[
-0000d870: 315d 2929 2c20 7265 7665 7273 653d 4661  1])), reverse=Fa
-0000d880: 6c73 6529 0a20 2020 2020 2020 2020 2020  lse).           
-0000d890: 2066 6f72 2065 302c 6531 2c73 2069 6e20   for e0,e1,s in 
-0000d8a0: 736f 7274 6564 5f65 6467 6573 3a20 0a20  sorted_edges: . 
-0000d8b0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000d8c0: 6620 6e6f 7420 7276 5f64 6566 6561 742e  f not rv_defeat.
-0000d8d0: 505b 6361 6e64 5f74 6f5f 6369 6478 5b65  P[cand_to_cidx[e
-0000d8e0: 315d 5d5b 6361 6e64 5f74 6f5f 6369 6478  1]][cand_to_cidx
-0000d8f0: 5b65 305d 5d20 616e 6420 6c65 6e28 7276  [e0]] and len(rv
-0000d900: 5f64 6566 6561 742e 7072 6564 735b 6361  _defeat.preds[ca
-0000d910: 6e64 5f74 6f5f 6369 6478 5b65 315d 5d29  nd_to_cidx[e1]])
-0000d920: 203d 3d20 303a 0a20 2020 2020 2020 2020   == 0:.         
-0000d930: 2020 2020 2020 2020 2020 2072 765f 6465             rv_de
-0000d940: 6665 6174 2e61 6464 2863 616e 645f 746f  feat.add(cand_to
-0000d950: 5f63 6964 785b 6530 5d2c 6361 6e64 5f74  _cidx[e0],cand_t
-0000d960: 6f5f 6369 6478 5b65 315d 290a 2020 2020  o_cidx[e1]).    
-0000d970: 2020 2020 2020 2020 7769 6e6e 6572 732e          winners.
-0000d980: 6170 7065 6e64 2863 6964 785f 746f 5f63  append(cidx_to_c
-0000d990: 616e 645b 7276 5f64 6566 6561 742e 696e  and[rv_defeat.in
-0000d9a0: 6974 6961 6c5f 656c 656d 656e 7473 2829  itial_elements()
-0000d9b0: 5b30 5d5d 290a 2020 2020 7265 7475 726e  [0]]).    return
-0000d9c0: 2073 6f72 7465 6428 6c69 7374 2873 6574   sorted(list(set
-0000d9d0: 2877 696e 6e65 7273 2929 290a 0a72 6976  (winners)))..riv
-0000d9e0: 6572 5f7a 745f 7072 6f70 6572 7469 6573  er_zt_properties
-0000d9f0: 203d 2056 6f74 696e 674d 6574 686f 6450   = VotingMethodP
-0000da00: 726f 7065 7274 6965 7328 0a20 2020 2063  roperties(.    c
-0000da10: 6f6e 646f 7263 6574 5f77 696e 6e65 723d  ondorcet_winner=
-0000da20: 5472 7565 2c20 0a20 2020 2063 6f6e 646f  True, .    condo
-0000da30: 7263 6574 5f6c 6f73 6572 3d54 7275 652c  rcet_loser=True,
-0000da40: 0a20 2020 2070 6172 6574 6f5f 646f 6d69  .    pareto_domi
-0000da50: 6e61 6e63 653d 5472 7565 2c0a 2020 2020  nance=True,.    
-0000da60: 706f 7369 7469 7665 5f69 6e76 6f6c 7665  positive_involve
-0000da70: 6d65 6e74 3d46 616c 7365 2c20 0a20 2020  ment=False, .   
-0000da80: 2029 0a40 766d 286e 616d 653d 2252 6976   ).@vm(name="Riv
-0000da90: 6572 205a 5422 2c0a 2020 2020 7072 6f70  er ZT",.    prop
-0000daa0: 6572 7469 6573 3d72 6976 6572 5f7a 745f  erties=river_zt_
-0000dab0: 7072 6f70 6572 7469 6573 2c0a 2020 2020  properties,.    
-0000dac0: 696e 7075 745f 7479 7065 733d 5b45 6c65  input_types=[Ele
-0000dad0: 6374 696f 6e54 7970 6573 2e50 524f 4649  ctionTypes.PROFI
-0000dae0: 4c45 5d29 0a64 6566 2072 6976 6572 5f7a  LE]).def river_z
-0000daf0: 7428 7072 6f66 696c 652c 2063 7572 725f  t(profile, curr_
-0000db00: 6361 6e64 7320 3d20 4e6f 6e65 2c20 7374  cands = None, st
-0000db10: 7265 6e67 7468 5f66 756e 6374 696f 6e20  rength_function 
-0000db20: 3d20 4e6f 6e65 293a 2020 200a 2020 2020  = None):   .    
-0000db30: 2222 2252 6976 6572 2077 6865 7265 2061  """River where a
-0000db40: 2066 6978 6564 2076 6f74 6572 2062 7265   fixed voter bre
-0000db50: 616b 7320 616e 7920 7469 6573 2069 6e20  aks any ties in 
-0000db60: 7468 6520 6d61 7267 696e 732e 2020 4974  the margins.  It
-0000db70: 2069 7320 616c 7761 7973 2074 6865 2076   is always the v
-0000db80: 6f74 6572 2069 6e20 706f 7369 7469 6f6e  oter in position
-0000db90: 2030 2074 6861 7420 6272 6561 6b73 2074   0 that breaks t
-0000dba0: 6865 2074 6965 732e 2020 5369 6e63 6520  he ties.  Since 
-0000dbb0: 766f 7465 7273 2068 6176 6520 7374 7269  voters have stri
-0000dbc0: 6374 2070 7265 6665 7265 6e63 6573 2c20  ct preferences, 
-0000dbd0: 7468 6973 206d 6574 686f 6420 6973 2072  this method is r
-0000dbe0: 6573 6f6c 7574 652e 2020 0a0a 2020 2020  esolute.  ..    
-0000dbf0: 4172 6773 3a0a 2020 2020 2020 2020 6564  Args:.        ed
-0000dc00: 6174 6120 2850 726f 6669 6c65 293a 2041  ata (Profile): A
-0000dc10: 2070 726f 6669 6c65 206f 6620 6c69 6e65   profile of line
-0000dc20: 6172 206f 7264 6572 730a 2020 2020 2020  ar orders.      
-0000dc30: 2020 6375 7272 5f63 616e 6473 2028 4c69    curr_cands (Li
-0000dc40: 7374 5b69 6e74 5d2c 206f 7074 696f 6e61  st[int], optiona
-0000dc50: 6c29 3a20 4966 2073 6574 2c20 7468 656e  l): If set, then
-0000dc60: 2066 696e 6420 7468 6520 7769 6e6e 6572   find the winner
-0000dc70: 7320 666f 7220 7468 6520 7072 6f66 696c  s for the profil
-0000dc80: 6520 7265 7374 7269 6374 6564 2074 6f20  e restricted to 
-0000dc90: 7468 6520 6361 6e64 6964 6174 6573 2069  the candidates i
-0000dca0: 6e20 6060 6375 7272 5f63 616e 6473 6060  n ``curr_cands``
-0000dcb0: 0a0a 2020 2020 5265 7475 726e 733a 200a  ..    Returns: .
-0000dcc0: 2020 2020 2020 2020 4120 736f 7274 6564          A sorted
-0000dcd0: 206c 6973 7420 6f66 2063 616e 6469 6461   list of candida
-0000dce0: 7465 732e 200a 0a20 2020 202e 2e20 7365  tes. ..    .. se
-0000dcf0: 6561 6c73 6f3a 3a0a 0a20 2020 2020 2020  ealso::..       
-0000dd00: 203a 6d65 7468 3a60 7072 6566 5f76 6f74   :meth:`pref_vot
-0000dd10: 696e 672e 6d61 7267 696e 5f62 6173 6564  ing.margin_based
-0000dd20: 5f6d 6574 686f 6473 2e72 6976 6572 602c  _methods.river`,
-0000dd30: 203a 6d65 7468 3a60 7072 6566 5f76 6f74   :meth:`pref_vot
-0000dd40: 696e 672e 6d61 7267 696e 5f62 6173 6564  ing.margin_based
-0000dd50: 5f6d 6574 686f 6473 2e72 6976 6572 5f77  _methods.river_w
-0000dd60: 6974 685f 7465 7374 602c 203a 6d65 7468  ith_test`, :meth
-0000dd70: 3a60 7072 6566 5f76 6f74 696e 672e 6d61  :`pref_voting.ma
-0000dd80: 7267 696e 5f62 6173 6564 5f6d 6574 686f  rgin_based_metho
-0000dd90: 6473 2e72 616e 6b65 645f 7061 6972 7360  ds.ranked_pairs`
-0000dda0: 0a0a 2020 2020 0a20 2020 2022 2222 0a20  ..    .    """. 
-0000ddb0: 2020 2063 616e 6469 6461 7465 7320 3d20     candidates = 
-0000ddc0: 7072 6f66 696c 652e 6361 6e64 6964 6174  profile.candidat
-0000ddd0: 6573 2069 6620 6375 7272 5f63 616e 6473  es if curr_cands
-0000dde0: 2069 7320 4e6f 6e65 2065 6c73 6520 6375   is None else cu
-0000ddf0: 7272 5f63 616e 6473 2020 2020 0a20 2020  rr_cands    .   
-0000de00: 200a 2020 2020 2320 7468 6520 7469 652d   .    # the tie-
-0000de10: 6272 6561 6b65 7220 6973 2061 6c77 6179  breaker is alway
-0000de20: 7320 7468 6520 6669 7273 7420 766f 7465  s the first vote
-0000de30: 722e 200a 2020 2020 7462 5f72 616e 6b69  r. .    tb_ranki
-0000de40: 6e67 203d 2074 7570 6c65 285b 6320 666f  ng = tuple([c fo
-0000de50: 7220 6320 696e 206c 6973 7428 7072 6f66  r c in list(prof
-0000de60: 696c 652e 5f72 616e 6b69 6e67 735b 305d  ile._rankings[0]
-0000de70: 2920 6966 2063 2069 6e20 6361 6e64 6964  ) if c in candid
-0000de80: 6174 6573 5d29 0a20 2020 200a 2020 2020  ates]).    .    
-0000de90: 7265 7475 726e 2072 6976 6572 5f74 6228  return river_tb(
-0000dea0: 7072 6f66 696c 652c 2063 7572 725f 6361  profile, curr_ca
-0000deb0: 6e64 7320 3d20 6375 7272 5f63 616e 6473  nds = curr_cands
-0000dec0: 2c20 7469 655f 6272 6561 6b65 7220 3d20  , tie_breaker = 
-0000ded0: 7462 5f72 616e 6b69 6e67 2c20 7374 7265  tb_ranking, stre
-0000dee0: 6e67 7468 5f66 756e 6374 696f 6e20 3d20  ngth_function = 
-0000def0: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
-0000df00: 6e29 0a20 2020 200a 0a23 2053 696d 706c  n).    ..# Simpl
-0000df10: 6520 5374 6162 6c65 2056 6f74 696e 6720  e Stable Voting 
-0000df20: 0a64 6566 205f 7369 6d70 6c65 5f73 7461  .def _simple_sta
-0000df30: 626c 655f 766f 7469 6e67 2863 7572 725f  ble_voting(curr_
-0000df40: 6361 6e64 732c 200a 2020 2020 2020 2020  cands, .        
-0000df50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000df60: 2020 736f 7274 6564 5f6d 6174 6368 6573    sorted_matches
-0000df70: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000df80: 2020 2020 2020 2020 2020 2020 6d65 6d5f              mem_
-0000df90: 7376 5f77 696e 6e65 7273 293a 0a20 2020  sv_winners):.   
-0000dfa0: 2027 2727 0a20 2020 2044 6574 6572 6d69   '''.    Determi
-0000dfb0: 6e65 2074 6865 2053 696d 706c 6520 5374  ne the Simple St
-0000dfc0: 6162 6c65 2056 6f74 696e 6720 7769 6e6e  able Voting winn
-0000dfd0: 6572 7320 7768 696c 6520 6b65 6570 696e  ers while keepin
-0000dfe0: 6720 7472 6163 6b20 0a20 2020 206f 6620  g track .    of 
-0000dff0: 7468 6520 7769 6e6e 6572 7320 696e 2061  the winners in a
-0000e000: 6e79 2073 7562 7072 6f66 696c 6573 2063  ny subprofiles c
-0000e010: 6865 636b 6564 2064 7572 696e 6720 636f  hecked during co
-0000e020: 6d70 7574 6174 696f 6e2e 200a 2020 2020  mputation. .    
-0000e030: 2727 270a 2020 2020 0a20 2020 2073 765f  '''.    .    sv_
-0000e040: 7769 6e6e 6572 7320 3d20 6c69 7374 2829  winners = list()
-0000e050: 0a20 2020 2020 2020 200a 2020 2020 6966  .        .    if
-0000e060: 206c 656e 2863 7572 725f 6361 6e64 7329   len(curr_cands)
-0000e070: 203d 3d20 313a 200a 2020 2020 2020 2020   == 1: .        
-0000e080: 6d65 6d5f 7376 5f77 696e 6e65 7273 5b74  mem_sv_winners[t
-0000e090: 7570 6c65 2863 7572 725f 6361 6e64 7329  uple(curr_cands)
-0000e0a0: 5d20 3d20 6375 7272 5f63 616e 6473 0a20  ] = curr_cands. 
-0000e0b0: 2020 2020 2020 2072 6574 7572 6e20 6375         return cu
-0000e0c0: 7272 5f63 616e 6473 2c20 6d65 6d5f 7376  rr_cands, mem_sv
-0000e0d0: 5f77 696e 6e65 7273 0a20 2020 200a 2020  _winners.    .  
-0000e0e0: 2020 6d61 7267 696e 5f77 6974 6e65 7373    margin_witness
-0000e0f0: 696e 675f 7769 6e20 3d20 2d6d 6174 682e  ing_win = -math.
-0000e100: 696e 660a 0a20 2020 2066 6f72 2061 2c20  inf..    for a, 
-0000e110: 622c 2073 2069 6e20 736f 7274 6564 5f6d  b, s in sorted_m
-0000e120: 6174 6368 6573 3a0a 2020 2020 2020 2020  atches:.        
-0000e130: 6966 2073 203c 206d 6172 6769 6e5f 7769  if s < margin_wi
-0000e140: 746e 6573 7369 6e67 5f77 696e 3a20 0a20  tnessing_win: . 
-0000e150: 2020 2020 2020 2020 2020 2062 7265 616b             break
-0000e160: 0a20 2020 2020 2020 2069 6620 6120 6e6f  .        if a no
-0000e170: 7420 696e 2073 765f 7769 6e6e 6572 733a  t in sv_winners:
-0000e180: 200a 2020 2020 2020 2020 2020 2020 6361   .            ca
-0000e190: 6e64 735f 6d69 6e75 735f 6220 3d20 5b63  nds_minus_b = [c
-0000e1a0: 2066 6f72 2063 2069 6e20 6375 7272 5f63   for c in curr_c
-0000e1b0: 616e 6473 2069 6620 6320 213d 2062 5d0a  ands if c != b].
-0000e1c0: 2020 2020 2020 2020 2020 2020 6361 6e64              cand
-0000e1d0: 735f 6d69 6e75 735f 625f 6b65 7920 3d20  s_minus_b_key = 
-0000e1e0: 7475 706c 6528 736f 7274 6564 2863 616e  tuple(sorted(can
-0000e1f0: 6473 5f6d 696e 7573 5f62 2929 0a20 2020  ds_minus_b)).   
-0000e200: 2020 2020 2020 2020 2069 6620 6361 6e64           if cand
-0000e210: 735f 6d69 6e75 735f 625f 6b65 7920 6e6f  s_minus_b_key no
-0000e220: 7420 696e 206d 656d 5f73 765f 7769 6e6e  t in mem_sv_winn
-0000e230: 6572 732e 6b65 7973 2829 3a20 0a20 2020  ers.keys(): .   
-0000e240: 2020 2020 2020 2020 2020 2020 2077 732c               ws,
-0000e250: 206d 656d 5f73 765f 7769 6e6e 6572 7320   mem_sv_winners 
-0000e260: 3d20 5f73 696d 706c 655f 7374 6162 6c65  = _simple_stable
-0000e270: 5f76 6f74 696e 6728 6375 7272 5f63 616e  _voting(curr_can
-0000e280: 6473 203d 2063 616e 6473 5f6d 696e 7573  ds = cands_minus
-0000e290: 5f62 2c0a 2020 2020 2020 2020 2020 2020  _b,.            
-0000e2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e2c0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000e2d0: 6f72 7465 645f 6d61 7463 6865 7320 3d20  orted_matches = 
-0000e2e0: 5b28 612c 2063 2c20 7329 2066 6f72 2061  [(a, c, s) for a
-0000e2f0: 2c20 632c 2073 2069 6e20 736f 7274 6564  , c, s in sorted
-0000e300: 5f6d 6174 6368 6573 2069 6620 6120 213d  _matches if a !=
-0000e310: 2062 2061 6e64 2063 2021 3d20 625d 2c0a   b and c != b],.
-0000e320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e350: 2020 2020 2020 2020 2020 206d 656d 5f73             mem_s
-0000e360: 765f 7769 6e6e 6572 7320 3d20 6d65 6d5f  v_winners = mem_
-0000e370: 7376 5f77 696e 6e65 7273 290a 2020 2020  sv_winners).    
-0000e380: 2020 2020 2020 2020 2020 2020 6d65 6d5f              mem_
-0000e390: 7376 5f77 696e 6e65 7273 5b63 616e 6473  sv_winners[cands
-0000e3a0: 5f6d 696e 7573 5f62 5f6b 6579 5d20 3d20  _minus_b_key] = 
-0000e3b0: 7773 0a20 2020 2020 2020 2020 2020 2065  ws.            e
-0000e3c0: 6c73 653a 200a 2020 2020 2020 2020 2020  lse: .          
-0000e3d0: 2020 2020 2020 7773 203d 206d 656d 5f73        ws = mem_s
-0000e3e0: 765f 7769 6e6e 6572 735b 6361 6e64 735f  v_winners[cands_
-0000e3f0: 6d69 6e75 735f 625f 6b65 795d 0a20 2020  minus_b_key].   
-0000e400: 2020 2020 2020 2020 2069 6620 6120 696e           if a in
-0000e410: 2077 733a 0a20 2020 2020 2020 2020 2020   ws:.           
-0000e420: 2020 2020 2073 765f 7769 6e6e 6572 732e       sv_winners.
-0000e430: 6170 7065 6e64 2861 290a 2020 2020 2020  append(a).      
-0000e440: 2020 2020 2020 2020 2020 6d61 7267 696e            margin
-0000e450: 5f77 6974 6e65 7373 696e 675f 7769 6e20  _witnessing_win 
-0000e460: 3d20 730a 0a20 2020 2072 6574 7572 6e20  = s..    return 
-0000e470: 7376 5f77 696e 6e65 7273 2c20 6d65 6d5f  sv_winners, mem_
-0000e480: 7376 5f77 696e 6e65 7273 0a20 2020 200a  sv_winners.    .
-0000e490: 0a40 766d 286e 616d 6520 3d20 2253 696d  .@vm(name = "Sim
-0000e4a0: 706c 6520 5374 6162 6c65 2056 6f74 696e  ple Stable Votin
-0000e4b0: 6722 290a 6465 6620 5f73 696d 706c 655f  g").def _simple_
-0000e4c0: 7374 6162 6c65 5f76 6f74 696e 675f 7769  stable_voting_wi
-0000e4d0: 7468 5f63 6f6e 646f 7263 6574 5f63 6865  th_condorcet_che
-0000e4e0: 636b 280a 2020 2020 6564 6174 612c 200a  ck(.    edata, .
-0000e4f0: 2020 2020 6375 7272 5f63 616e 6473 203d      curr_cands =
-0000e500: 204e 6f6e 652c 200a 2020 2020 7374 7265   None, .    stre
-0000e510: 6e67 7468 5f66 756e 6374 696f 6e20 3d20  ngth_function = 
-0000e520: 4e6f 6e65 293a 200a 2020 2020 2222 2253  None): .    """S
-0000e530: 696d 706c 6520 5374 6162 6c65 2056 6f74  imple Stable Vot
-0000e540: 696e 6720 6973 2043 6f6e 646f 7263 6574  ing is Condorcet
-0000e550: 2063 6f6e 7369 7374 656e 742e 2020 2049   consistent.   I
-0000e560: 7420 6973 2066 6173 7465 7220 746f 2073  t is faster to s
-0000e570: 6b69 7020 6578 6563 7574 696e 6720 7468  kip executing th
-0000e580: 6520 7265 6375 7273 6976 6520 616c 676f  e recursive algo
-0000e590: 7269 7468 6d20 7768 656e 2074 6865 7265  rithm when there
-0000e5a0: 2069 7320 6120 436f 6e64 6f72 6365 7420   is a Condorcet 
-0000e5b0: 7769 6e6e 6572 4669 7273 7420 6368 6563  winnerFirst chec
-0000e5c0: 6b20 6966 2074 6865 7265 2069 7320 6120  k if there is a 
-0000e5d0: 436f 6e64 6f72 6365 7420 7769 6e6e 6572  Condorcet winner
-0000e5e0: 2e20 2049 6620 736f 2c20 7265 7475 726e  .  If so, return
-0000e5f0: 2074 6865 2043 6f6e 646f 7263 6574 2077   the Condorcet w
-0000e600: 696e 6e65 722c 206f 7468 6572 7769 7365  inner, otherwise
-0000e610: 2066 696e 6420 7468 6520 5369 6d70 6c65   find the Simple
-0000e620: 2053 7461 626c 6520 566f 7469 6e67 2077   Stable Voting w
-0000e630: 696e 6e65 7220 7573 696e 6720 5f73 696d  inner using _sim
-0000e640: 706c 655f 7374 6162 6c65 5f76 6f74 696e  ple_stable_votin
-0000e650: 670a 0a20 2020 2041 7267 733a 0a20 2020  g..    Args:.   
-0000e660: 2020 2020 2065 6461 7461 2028 5072 6f66       edata (Prof
-0000e670: 696c 652c 2050 726f 6669 6c65 5769 7468  ile, ProfileWith
-0000e680: 5469 6573 2c20 4d61 7267 696e 4772 6170  Ties, MarginGrap
-0000e690: 6829 3a20 416e 7920 656c 6563 7469 6f6e  h): Any election
-0000e6a0: 2064 6174 6120 7468 6174 2068 6173 2061   data that has a
-0000e6b0: 2060 6d61 7267 696e 6020 6d65 7468 6f64   `margin` method
-0000e6c0: 2e20 0a20 2020 2020 2020 2063 7572 725f  . .        curr_
-0000e6d0: 6361 6e64 7320 284c 6973 745b 696e 745d  cands (List[int]
-0000e6e0: 2c20 6f70 7469 6f6e 616c 293a 2049 6620  , optional): If 
-0000e6f0: 7365 742c 2074 6865 6e20 6669 6e64 2074  set, then find t
-0000e700: 6865 2077 696e 6e65 7273 2066 6f72 2074  he winners for t
-0000e710: 6865 2070 726f 6669 6c65 2072 6573 7472  he profile restr
-0000e720: 6963 7465 6420 746f 2074 6865 2063 616e  icted to the can
-0000e730: 6469 6461 7465 7320 696e 2060 6063 7572  didates in ``cur
-0000e740: 725f 6361 6e64 7360 600a 2020 2020 2020  r_cands``.      
-0000e750: 2020 7374 7265 6e67 7468 5f66 756e 6374    strength_funct
-0000e760: 696f 6e20 2866 756e 6374 696f 6e2c 206f  ion (function, o
-0000e770: 7074 696f 6e61 6c29 3a20 5468 6520 7374  ptional): The st
-0000e780: 7265 6e67 7468 2066 756e 6374 696f 6e20  rength function 
-0000e790: 746f 2062 6520 7573 6564 2074 6f20 6361  to be used to ca
-0000e7a0: 6c63 756c 6174 6520 7468 6520 7374 7265  lculate the stre
-0000e7b0: 6e67 7468 206f 6620 6120 7061 7468 2e20  ngth of a path. 
-0000e7c0: 2020 5468 6520 6465 6661 756c 7420 6973    The default is
-0000e7d0: 2074 6865 206d 6172 6769 6e20 6d65 7468   the margin meth
-0000e7e0: 6f64 206f 6620 6060 6564 6174 6160 602e  od of ``edata``.
-0000e7f0: 2020 2054 6869 7320 6f6e 6c79 206d 6174     This only mat
-0000e800: 7465 7273 2077 6865 6e20 7468 6520 6261  ters when the ba
-0000e810: 6c6c 6f74 7320 6172 6520 6e6f 7420 6c69  llots are not li
-0000e820: 6e65 6172 206f 7264 6572 732e 200a 0a20  near orders. .. 
-0000e830: 2020 2052 6574 7572 6e73 3a20 0a20 2020     Returns: .   
-0000e840: 2020 2020 2041 2073 6f72 7465 6420 6c69       A sorted li
-0000e850: 7374 206f 6620 6361 6e64 6964 6174 6573  st of candidates
-0000e860: 2e20 0a0a 2020 2020 2222 220a 2020 2020  . ..    """.    
-0000e870: 0a20 2020 2063 7720 3d20 6564 6174 612e  .    cw = edata.
-0000e880: 636f 6e64 6f72 6365 745f 7769 6e6e 6572  condorcet_winner
-0000e890: 2863 7572 725f 6361 6e64 7320 3d20 6375  (curr_cands = cu
-0000e8a0: 7272 5f63 616e 6473 290a 2020 2020 6966  rr_cands).    if
-0000e8b0: 2063 7720 6973 206e 6f74 204e 6f6e 653a   cw is not None:
-0000e8c0: 200a 2020 2020 2020 2020 7265 7475 726e   .        return
-0000e8d0: 205b 6377 5d0a 2020 2020 656c 7365 3a20   [cw].    else: 
-0000e8e0: 0a20 2020 2020 2020 2063 7572 725f 6361  .        curr_ca
-0000e8f0: 6e64 7320 3d20 6564 6174 612e 6361 6e64  nds = edata.cand
-0000e900: 6964 6174 6573 2069 6620 6375 7272 5f63  idates if curr_c
-0000e910: 616e 6473 2069 7320 4e6f 6e65 2065 6c73  ands is None els
-0000e920: 6520 6375 7272 5f63 616e 6473 0a20 2020  e curr_cands.   
-0000e930: 2020 2020 2073 7472 656e 6774 685f 6675       strength_fu
-0000e940: 6e63 7469 6f6e 203d 2065 6461 7461 2e6d  nction = edata.m
-0000e950: 6172 6769 6e20 6966 2073 7472 656e 6774  argin if strengt
-0000e960: 685f 6675 6e63 7469 6f6e 2069 7320 4e6f  h_function is No
-0000e970: 6e65 2065 6c73 6520 7374 7265 6e67 7468  ne else strength
-0000e980: 5f66 756e 6374 696f 6e20 200a 0a20 2020  _function  ..   
-0000e990: 2020 2020 206d 6174 6368 6573 203d 205b       matches = [
-0000e9a0: 2861 2c20 622c 2073 7472 656e 6774 685f  (a, b, strength_
-0000e9b0: 6675 6e63 7469 6f6e 2861 2c20 6229 2920  function(a, b)) 
-0000e9c0: 666f 7220 6120 696e 2063 7572 725f 6361  for a in curr_ca
-0000e9d0: 6e64 7320 666f 7220 6220 696e 2063 7572  nds for b in cur
-0000e9e0: 725f 6361 6e64 7320 6966 2061 2021 3d20  r_cands if a != 
-0000e9f0: 625d 0a20 2020 2020 2020 2073 6f72 7465  b].        sorte
-0000ea00: 645f 6d61 7463 6865 7320 3d20 736f 7274  d_matches = sort
-0000ea10: 6564 286d 6174 6368 6573 2c20 7265 7665  ed(matches, reve
-0000ea20: 7273 653d 5472 7565 2c20 6b65 793d 6c61  rse=True, key=la
-0000ea30: 6d62 6461 206d 5f77 5f77 6569 6768 743a  mbda m_w_weight:
-0000ea40: 206d 5f77 5f77 6569 6768 745b 325d 290a   m_w_weight[2]).
-0000ea50: 2020 2020 0a20 2020 2020 2020 2072 6574      .        ret
-0000ea60: 7572 6e20 736f 7274 6564 285f 7369 6d70  urn sorted(_simp
-0000ea70: 6c65 5f73 7461 626c 655f 766f 7469 6e67  le_stable_voting
-0000ea80: 2863 7572 725f 6361 6e64 7320 3d20 6375  (curr_cands = cu
-0000ea90: 7272 5f63 616e 6473 2c20 0a20 2020 2020  rr_cands, .     
-0000eaa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eac0: 2020 2020 2020 2073 6f72 7465 645f 6d61         sorted_ma
-0000ead0: 7463 6865 7320 3d20 736f 7274 6564 5f6d  tches = sorted_m
-0000eae0: 6174 6368 6573 2c0a 2020 2020 2020 2020  atches,.        
-0000eaf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eb00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eb10: 2020 2020 6d65 6d5f 7376 5f77 696e 6e65      mem_sv_winne
-0000eb20: 7273 203d 207b 7d29 5b30 5d29 0a0a 0a64  rs = {})[0])...d
-0000eb30: 6566 205f 7369 6d70 6c65 5f73 7461 626c  ef _simple_stabl
-0000eb40: 655f 766f 7469 6e67 5f62 6173 6963 2865  e_voting_basic(e
-0000eb50: 6461 7461 2c20 6375 7272 5f63 616e 6473  data, curr_cands
-0000eb60: 203d 204e 6f6e 652c 2073 7472 656e 6774   = None, strengt
-0000eb70: 685f 6675 6e63 7469 6f6e 203d 204e 6f6e  h_function = Non
-0000eb80: 6529 3a20 0a20 2020 2022 2222 496d 706c  e): .    """Impl
-0000eb90: 656d 656e 7461 7469 6f6e 206f 6620 5369  ementation of Si
-0000eba0: 6d70 6c65 2053 7461 626c 6520 566f 7469  mple Stable Voti
-0000ebb0: 6e67 2066 726f 6d20 6874 7470 733a 2f2f  ng from https://
-0000ebc0: 6172 7869 762e 6f72 672f 6162 732f 3231  arxiv.org/abs/21
-0000ebd0: 3038 2e30 3035 3432 2e20 0a0a 2020 2020  08.00542. ..    
-0000ebe0: 4172 6773 3a0a 2020 2020 2020 2020 6564  Args:.        ed
-0000ebf0: 6174 6120 2850 726f 6669 6c65 2c20 5072  ata (Profile, Pr
-0000ec00: 6f66 696c 6557 6974 6854 6965 732c 204d  ofileWithTies, M
-0000ec10: 6172 6769 6e47 7261 7068 293a 2041 6e79  arginGraph): Any
-0000ec20: 2065 6c65 6374 696f 6e20 6461 7461 2074   election data t
-0000ec30: 6861 7420 6861 7320 6120 606d 6172 6769  hat has a `margi
-0000ec40: 6e60 206d 6574 686f 642e 200a 2020 2020  n` method. .    
-0000ec50: 2020 2020 6375 7272 5f63 616e 6473 2028      curr_cands (
-0000ec60: 4c69 7374 5b69 6e74 5d2c 206f 7074 696f  List[int], optio
-0000ec70: 6e61 6c29 3a20 4966 2073 6574 2c20 7468  nal): If set, th
-0000ec80: 656e 2066 696e 6420 7468 6520 7769 6e6e  en find the winn
-0000ec90: 6572 7320 666f 7220 7468 6520 7072 6f66  ers for the prof
-0000eca0: 696c 6520 7265 7374 7269 6374 6564 2074  ile restricted t
-0000ecb0: 6f20 7468 6520 6361 6e64 6964 6174 6573  o the candidates
-0000ecc0: 2069 6e20 6060 6375 7272 5f63 616e 6473   in ``curr_cands
-0000ecd0: 6060 0a20 2020 2020 2020 2073 7472 656e  ``.        stren
-0000ece0: 6774 685f 6675 6e63 7469 6f6e 2028 6675  gth_function (fu
-0000ecf0: 6e63 7469 6f6e 2c20 6f70 7469 6f6e 616c  nction, optional
-0000ed00: 293a 2054 6865 2073 7472 656e 6774 6820  ): The strength 
-0000ed10: 6675 6e63 7469 6f6e 2074 6f20 6265 2075  function to be u
-0000ed20: 7365 6420 746f 2063 616c 6375 6c61 7465  sed to calculate
-0000ed30: 2074 6865 2073 7472 656e 6774 6820 6f66   the strength of
-0000ed40: 2061 2070 6174 682e 2020 2054 6865 2064   a path.   The d
-0000ed50: 6566 6175 6c74 2069 7320 7468 6520 6d61  efault is the ma
-0000ed60: 7267 696e 206d 6574 686f 6420 6f66 2060  rgin method of `
-0000ed70: 6065 6461 7461 6060 2e20 2020 5468 6973  `edata``.   This
-0000ed80: 206f 6e6c 7920 6d61 7474 6572 7320 7768   only matters wh
-0000ed90: 656e 2074 6865 2062 616c 6c6f 7473 2061  en the ballots a
-0000eda0: 7265 206e 6f74 206c 696e 6561 7220 6f72  re not linear or
-0000edb0: 6465 7273 2e20 0a0a 2020 2020 5265 7475  ders. ..    Retu
-0000edc0: 726e 733a 200a 2020 2020 2020 2020 4120  rns: .        A 
-0000edd0: 736f 7274 6564 206c 6973 7420 6f66 2063  sorted list of c
-0000ede0: 616e 6469 6461 7465 732e 200a 0a20 2020  andidates. ..   
-0000edf0: 2022 2222 0a20 2020 200a 2020 2020 6375   """.    .    cu
-0000ee00: 7272 5f63 616e 6473 203d 2065 6461 7461  rr_cands = edata
-0000ee10: 2e63 616e 6469 6461 7465 7320 6966 2063  .candidates if c
-0000ee20: 7572 725f 6361 6e64 7320 6973 204e 6f6e  urr_cands is Non
-0000ee30: 6520 656c 7365 2063 7572 725f 6361 6e64  e else curr_cand
-0000ee40: 730a 2020 2020 7374 7265 6e67 7468 5f66  s.    strength_f
-0000ee50: 756e 6374 696f 6e20 3d20 6564 6174 612e  unction = edata.
-0000ee60: 6d61 7267 696e 2069 6620 7374 7265 6e67  margin if streng
-0000ee70: 7468 5f66 756e 6374 696f 6e20 6973 204e  th_function is N
-0000ee80: 6f6e 6520 656c 7365 2073 7472 656e 6774  one else strengt
-0000ee90: 685f 6675 6e63 7469 6f6e 2020 0a0a 2020  h_function  ..  
-0000eea0: 2020 6d61 7463 6865 7320 3d20 5b28 612c    matches = [(a,
-0000eeb0: 2062 2c20 7374 7265 6e67 7468 5f66 756e   b, strength_fun
-0000eec0: 6374 696f 6e28 612c 2062 2929 2066 6f72  ction(a, b)) for
-0000eed0: 2061 2069 6e20 6375 7272 5f63 616e 6473   a in curr_cands
-0000eee0: 2066 6f72 2062 2069 6e20 6375 7272 5f63   for b in curr_c
-0000eef0: 616e 6473 2069 6620 6120 213d 2062 5d0a  ands if a != b].
-0000ef00: 2020 2020 736f 7274 6564 5f6d 6174 6368      sorted_match
-0000ef10: 6573 203d 2073 6f72 7465 6428 6d61 7463  es = sorted(matc
-0000ef20: 6865 732c 2072 6576 6572 7365 3d54 7275  hes, reverse=Tru
-0000ef30: 652c 206b 6579 3d6c 616d 6264 6120 6d5f  e, key=lambda m_
-0000ef40: 775f 7765 6967 6874 3a20 6d5f 775f 7765  w_weight: m_w_we
-0000ef50: 6967 6874 5b32 5d29 0a20 2020 200a 2020  ight[2]).    .  
-0000ef60: 2020 7265 7475 726e 2073 6f72 7465 6428    return sorted(
-0000ef70: 5f73 696d 706c 655f 7374 6162 6c65 5f76  _simple_stable_v
-0000ef80: 6f74 696e 6728 6375 7272 5f63 616e 6473  oting(curr_cands
-0000ef90: 203d 2063 7572 725f 6361 6e64 732c 200a   = curr_cands, .
-0000efa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000efb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000efc0: 2020 2020 2020 2020 736f 7274 6564 5f6d          sorted_m
-0000efd0: 6174 6368 6573 203d 2073 6f72 7465 645f  atches = sorted_
-0000efe0: 6d61 7463 6865 732c 0a20 2020 2020 2020  matches,.       
-0000eff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f010: 206d 656d 5f73 765f 7769 6e6e 6572 7320   mem_sv_winners 
-0000f020: 3d20 7b7d 295b 305d 290a 0a73 7376 5f70  = {})[0])..ssv_p
-0000f030: 726f 7065 7274 6965 7320 3d20 566f 7469  roperties = Voti
-0000f040: 6e67 4d65 7468 6f64 5072 6f70 6572 7469  ngMethodProperti
-0000f050: 6573 280a 2020 2020 636f 6e64 6f72 6365  es(.    condorce
-0000f060: 745f 7769 6e6e 6572 3d54 7275 652c 200a  t_winner=True, .
-0000f070: 2020 2020 636f 6e64 6f72 6365 745f 6c6f      condorcet_lo
-0000f080: 7365 723d 5472 7565 2c0a 2020 2020 7061  ser=True,.    pa
-0000f090: 7265 746f 5f64 6f6d 696e 616e 6365 3d54  reto_dominance=T
-0000f0a0: 7275 652c 0a20 2020 2070 6f73 6974 6976  rue,.    positiv
-0000f0b0: 655f 696e 766f 6c76 656d 656e 743d 4661  e_involvement=Fa
-0000f0c0: 6c73 652c 200a 2020 2020 290a 4076 6d28  lse, .    ).@vm(
-0000f0d0: 6e61 6d65 203d 2022 5369 6d70 6c65 2053  name = "Simple S
-0000f0e0: 7461 626c 6520 566f 7469 6e67 222c 0a20  table Voting",. 
-0000f0f0: 2020 2070 726f 7065 7274 6965 7320 3d20     properties = 
-0000f100: 7373 765f 7072 6f70 6572 7469 6573 2c0a  ssv_properties,.
-0000f110: 2020 2020 696e 7075 745f 7479 7065 7320      input_types 
-0000f120: 3d20 5b45 6c65 6374 696f 6e54 7970 6573  = [ElectionTypes
-0000f130: 2e50 524f 4649 4c45 2c20 456c 6563 7469  .PROFILE, Electi
-0000f140: 6f6e 5479 7065 732e 5052 4f46 494c 455f  onTypes.PROFILE_
-0000f150: 5749 5448 5f54 4945 532c 2045 6c65 6374  WITH_TIES, Elect
-0000f160: 696f 6e54 7970 6573 2e4d 4152 4749 4e5f  ionTypes.MARGIN_
-0000f170: 4752 4150 485d 290a 6465 6620 7369 6d70  GRAPH]).def simp
-0000f180: 6c65 5f73 7461 626c 655f 766f 7469 6e67  le_stable_voting
-0000f190: 280a 2020 2020 6564 6174 612c 200a 2020  (.    edata, .  
-0000f1a0: 2020 6375 7272 5f63 616e 6473 3d4e 6f6e    curr_cands=Non
-0000f1b0: 652c 200a 2020 2020 7374 7265 6e67 7468  e, .    strength
-0000f1c0: 5f66 756e 6374 696f 6e3d 4e6f 6e65 2c0a  _function=None,.
-0000f1d0: 2020 2020 616c 676f 7269 7468 6d20 3d20      algorithm = 
-0000f1e0: 2762 6173 6963 2729 3a20 0a0a 2020 2020  'basic'): ..    
-0000f1f0: 2222 2249 6d70 6c65 6d65 6e74 6174 696f  """Implementatio
-0000f200: 6e20 6f66 2053 696d 706c 6520 5374 6162  n of Simple Stab
-0000f210: 6c65 2056 6f74 696e 6720 6672 6f6d 2068  le Voting from h
-0000f220: 7474 7073 3a2f 2f61 7278 6976 2e6f 7267  ttps://arxiv.org
-0000f230: 2f61 6273 2f32 3130 382e 3030 3534 322e  /abs/2108.00542.
-0000f240: 200a 0a20 2020 2053 696d 706c 6520 5374   ..    Simple St
-0000f250: 6162 6c65 2056 6f74 696e 6720 6973 2061  able Voting is a
-0000f260: 2072 6563 7572 7369 7665 2076 6f74 696e   recursive votin
-0000f270: 6720 6d65 7468 6f64 2064 6566 696e 6564  g method defined
-0000f280: 2061 7320 666f 6c6c 6f77 733a 200a 0a20   as follows: .. 
-0000f290: 2020 2031 2e20 4966 2074 6865 7265 2069     1. If there i
-0000f2a0: 7320 6f6e 6c79 206f 6e65 2063 616e 6469  s only one candi
-0000f2b0: 6461 7465 2069 6e20 7468 6520 7072 6f66  date in the prof
-0000f2c0: 696c 652c 2074 6865 6e20 7468 6174 2063  ile, then that c
-0000f2d0: 616e 6469 6461 7465 2069 7320 7468 6520  andidate is the 
-0000f2e0: 7769 6e6e 6572 2e20 0a20 2020 2032 2e20  winner. .    2. 
-0000f2f0: 4f72 6465 7220 7468 6520 7061 6972 7320  Order the pairs 
-0000f300: 3a6d 6174 683a 6028 612c 6229 6020 6f66  :math:`(a,b)` of
-0000f310: 2063 616e 6469 6461 7465 7320 6672 6f6d   candidates from
-0000f320: 206c 6172 6765 7374 2074 6f20 736d 616c   largest to smal
-0000f330: 6c65 7374 2076 616c 7565 206f 6620 7468  lest value of th
-0000f340: 6520 6d61 7267 696e 206f 6620 3a6d 6174  e margin of :mat
-0000f350: 683a 6061 6020 6f76 6572 203a 6d61 7468  h:`a` over :math
-0000f360: 3a60 6260 2c20 616e 6420 6465 636c 6172  :`b`, and declar
-0000f370: 6520 6173 2053 696d 706c 6520 5374 6162  e as Simple Stab
-0000f380: 6c65 2056 6f74 696e 6720 7769 6e6e 6572  le Voting winner
-0000f390: 7320 7468 6520 6361 6e64 6964 6174 6528  s the candidate(
-0000f3a0: 7329 203a 6d61 7468 3a60 6160 2066 726f  s) :math:`a` fro
-0000f3b0: 6d20 7468 6520 6561 726c 6965 7374 2070  m the earliest p
-0000f3c0: 6169 7228 7329 203a 6d61 7468 3a60 2861  air(s) :math:`(a
-0000f3d0: 2c62 2960 2073 7563 6820 7468 6174 203a  ,b)` such that :
-0000f3e0: 6d61 7468 3a60 6160 2069 7320 6120 5369  math:`a` is a Si
-0000f3f0: 6d70 6c65 2053 7461 626c 6520 566f 7469  mple Stable Voti
-0000f400: 6e67 2077 696e 6e65 7220 696e 2074 6865  ng winner in the
-0000f410: 2065 6c65 6374 696f 6e20 7769 7468 6f75   election withou
-0000f420: 7420 3a6d 6174 683a 6062 602e 200a 0a20  t :math:`b`. .. 
-0000f430: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
-0000f440: 2065 6461 7461 2028 5072 6f66 696c 652c   edata (Profile,
-0000f450: 2050 726f 6669 6c65 5769 7468 5469 6573   ProfileWithTies
-0000f460: 2c20 4d61 7267 696e 4772 6170 6829 3a20  , MarginGraph): 
-0000f470: 416e 7920 656c 6563 7469 6f6e 2064 6174  Any election dat
-0000f480: 6120 7468 6174 2068 6173 2061 2060 6d61  a that has a `ma
-0000f490: 7267 696e 6020 6d65 7468 6f64 2e20 0a20  rgin` method. . 
-0000f4a0: 2020 2020 2020 2063 7572 725f 6361 6e64         curr_cand
-0000f4b0: 7320 284c 6973 745b 696e 745d 2c20 6f70  s (List[int], op
-0000f4c0: 7469 6f6e 616c 293a 2049 6620 7365 742c  tional): If set,
-0000f4d0: 2074 6865 6e20 6669 6e64 2074 6865 2077   then find the w
-0000f4e0: 696e 6e65 7273 2066 6f72 2074 6865 2070  inners for the p
-0000f4f0: 726f 6669 6c65 2072 6573 7472 6963 7465  rofile restricte
-0000f500: 6420 746f 2074 6865 2063 616e 6469 6461  d to the candida
-0000f510: 7465 7320 696e 2060 6063 7572 725f 6361  tes in ``curr_ca
-0000f520: 6e64 7360 600a 2020 2020 2020 2020 7374  nds``.        st
-0000f530: 7265 6e67 7468 5f66 756e 6374 696f 6e20  rength_function 
-0000f540: 2866 756e 6374 696f 6e2c 206f 7074 696f  (function, optio
-0000f550: 6e61 6c29 3a20 5468 6520 7374 7265 6e67  nal): The streng
-0000f560: 7468 2066 756e 6374 696f 6e20 746f 2062  th function to b
-0000f570: 6520 7573 6564 2074 6f20 6361 6c63 756c  e used to calcul
-0000f580: 6174 6520 7468 6520 7374 7265 6e67 7468  ate the strength
-0000f590: 206f 6620 6120 7061 7468 2e20 2020 5468   of a path.   Th
-0000f5a0: 6520 6465 6661 756c 7420 6973 2074 6865  e default is the
-0000f5b0: 206d 6172 6769 6e20 6d65 7468 6f64 206f   margin method o
-0000f5c0: 6620 6060 6564 6174 6160 602e 2020 2054  f ``edata``.   T
-0000f5d0: 6869 7320 6f6e 6c79 206d 6174 7465 7273  his only matters
-0000f5e0: 2077 6865 6e20 7468 6520 6261 6c6c 6f74   when the ballot
-0000f5f0: 7320 6172 6520 6e6f 7420 6c69 6e65 6172  s are not linear
-0000f600: 206f 7264 6572 732e 200a 2020 2020 2020   orders. .      
-0000f610: 2020 616c 676f 7269 7468 6d20 2873 7472    algorithm (str
-0000f620: 2c20 6f70 7469 6f6e 616c 293a 2053 7065  , optional): Spe
-0000f630: 6369 6679 2077 6869 6368 2061 6c67 6f72  cify which algor
-0000f640: 6974 686d 2074 6f20 7573 652e 2020 4f70  ithm to use.  Op
-0000f650: 7469 6f6e 7320 6172 6520 2762 6173 6963  tions are 'basic
-0000f660: 2720 2874 6865 2064 6566 6175 6c74 2920  ' (the default) 
-0000f670: 616e 6420 2777 6974 685f 636f 6e64 6f72  and 'with_condor
-0000f680: 6365 745f 6368 6563 6b27 2e0a 0a20 2020  cet_check'...   
-0000f690: 2052 6574 7572 6e73 3a20 0a20 2020 2020   Returns: .     
-0000f6a0: 2020 2041 2073 6f72 7465 6420 6c69 7374     A sorted list
-0000f6b0: 206f 6620 6361 6e64 6964 6174 6573 2e20   of candidates. 
-0000f6c0: 0a0a 2020 2020 2e2e 2073 6565 616c 736f  ..    .. seealso
-0000f6d0: 3a3a 0a0a 2020 2020 2020 2020 3a6d 6574  ::..        :met
-0000f6e0: 683a 6070 7265 665f 766f 7469 6e67 2e6d  h:`pref_voting.m
-0000f6f0: 6172 6769 6e5f 6261 7365 645f 6d65 7468  argin_based_meth
-0000f700: 6f64 732e 7374 6162 6c65 5f76 6f74 696e  ods.stable_votin
-0000f710: 6760 0a0a 2020 2020 3a45 7861 6d70 6c65  g`..    :Example
-0000f720: 3a20 0a0a 2020 2020 2e2e 2065 7865 635f  : ..    .. exec_
-0000f730: 636f 6465 3a3a 0a0a 2020 2020 2020 2020  code::..        
-0000f740: 6672 6f6d 2070 7265 665f 766f 7469 6e67  from pref_voting
-0000f750: 2e77 6569 6768 7465 645f 6d61 6a6f 7269  .weighted_majori
-0000f760: 7479 5f67 7261 7068 7320 696d 706f 7274  ty_graphs import
-0000f770: 204d 6172 6769 6e47 7261 7068 0a20 2020   MarginGraph.   
-0000f780: 2020 2020 2066 726f 6d20 7072 6566 5f76       from pref_v
-0000f790: 6f74 696e 672e 6d61 7267 696e 5f62 6173  oting.margin_bas
-0000f7a0: 6564 5f6d 6574 686f 6473 2069 6d70 6f72  ed_methods impor
-0000f7b0: 7420 7369 6d70 6c65 5f73 7461 626c 655f  t simple_stable_
-0000f7c0: 766f 7469 6e67 0a0a 2020 2020 2020 2020  voting..        
-0000f7d0: 6d67 203d 204d 6172 6769 6e47 7261 7068  mg = MarginGraph
-0000f7e0: 285b 302c 2031 2c20 322c 2033 5d2c 205b  ([0, 1, 2, 3], [
-0000f7f0: 2830 2c20 332c 2038 292c 2028 312c 2030  (0, 3, 8), (1, 0
-0000f800: 2c20 3130 292c 2028 322c 2030 2c20 3429  , 10), (2, 0, 4)
-0000f810: 2c20 2832 2c20 312c 2038 292c 2028 332c  , (2, 1, 8), (3,
-0000f820: 2031 2c20 3829 5d29 0a0a 2020 2020 2020   1, 8)])..      
-0000f830: 2020 7369 6d70 6c65 5f73 7461 626c 655f    simple_stable_
-0000f840: 766f 7469 6e67 2e64 6973 706c 6179 286d  voting.display(m
-0000f850: 6729 0a20 2020 2020 2020 2073 696d 706c  g).        simpl
-0000f860: 655f 7374 6162 6c65 5f76 6f74 696e 672e  e_stable_voting.
-0000f870: 6469 7370 6c61 7928 6d67 2c20 616c 676f  display(mg, algo
-0000f880: 7269 7468 6d3d 2762 6173 6963 2729 0a20  rithm='basic'). 
-0000f890: 2020 2020 2020 2073 696d 706c 655f 7374         simple_st
-0000f8a0: 6162 6c65 5f76 6f74 696e 672e 6469 7370  able_voting.disp
-0000f8b0: 6c61 7928 6d67 2c20 616c 676f 7269 7468  lay(mg, algorith
-0000f8c0: 6d3d 2777 6974 685f 636f 6e64 6f72 6365  m='with_condorce
-0000f8d0: 745f 6368 6563 6b27 290a 0a20 2020 2022  t_check')..    "
-0000f8e0: 2222 0a20 2020 200a 2020 2020 6966 2061  "".    .    if a
-0000f8f0: 6c67 6f72 6974 686d 203d 3d20 2762 6173  lgorithm == 'bas
-0000f900: 6963 273a 200a 2020 2020 2020 2020 7265  ic': .        re
-0000f910: 7475 726e 205f 7369 6d70 6c65 5f73 7461  turn _simple_sta
-0000f920: 626c 655f 766f 7469 6e67 5f62 6173 6963  ble_voting_basic
-0000f930: 2865 6461 7461 2c20 6375 7272 5f63 616e  (edata, curr_can
-0000f940: 6473 203d 2063 7572 725f 6361 6e64 732c  ds = curr_cands,
-0000f950: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
-0000f960: 6f6e 203d 2073 7472 656e 6774 685f 6675  on = strength_fu
-0000f970: 6e63 7469 6f6e 290a 2020 2020 656c 6966  nction).    elif
-0000f980: 2061 6c67 6f72 6974 686d 203d 3d20 2777   algorithm == 'w
-0000f990: 6974 685f 636f 6e64 6f72 6365 745f 6368  ith_condorcet_ch
-0000f9a0: 6563 6b27 3a0a 2020 2020 2020 2020 7265  eck':.        re
-0000f9b0: 7475 726e 205f 7369 6d70 6c65 5f73 7461  turn _simple_sta
-0000f9c0: 626c 655f 766f 7469 6e67 5f77 6974 685f  ble_voting_with_
-0000f9d0: 636f 6e64 6f72 6365 745f 6368 6563 6b28  condorcet_check(
-0000f9e0: 6564 6174 612c 2063 7572 725f 6361 6e64  edata, curr_cand
-0000f9f0: 7320 3d20 6375 7272 5f63 616e 6473 2c20  s = curr_cands, 
-0000fa00: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
-0000fa10: 6e20 3d20 7374 7265 6e67 7468 5f66 756e  n = strength_fun
-0000fa20: 6374 696f 6e29 0a20 2020 2065 6c73 653a  ction).    else:
-0000fa30: 0a20 2020 2020 2020 2072 6169 7365 2056  .        raise V
-0000fa40: 616c 7565 4572 726f 7228 2249 6e76 616c  alueError("Inval
-0000fa50: 6964 2061 6c67 6f72 6974 686d 2073 7065  id algorithm spe
-0000fa60: 6369 6669 6564 2e22 290a 2020 2020 0a0a  cified.").    ..
-0000fa70: 6465 6620 5f73 7461 626c 655f 766f 7469  def _stable_voti
-0000fa80: 6e67 2865 6461 7461 2c20 0a20 2020 2020  ng(edata, .     
-0000fa90: 2020 2020 2020 2020 2020 2020 2020 6375                cu
-0000faa0: 7272 5f63 616e 6473 2c0a 2020 2020 2020  rr_cands,.      
-0000fab0: 2020 2020 2020 2020 2020 2020 2073 7472               str
-0000fac0: 656e 6774 685f 6675 6e63 7469 6f6e 2c0a  ength_function,.
-0000fad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fae0: 2020 2073 6f72 7465 645f 6d61 7463 6865     sorted_matche
-0000faf0: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
-0000fb00: 2020 2020 2020 6d65 6d5f 7376 5f77 696e        mem_sv_win
-0000fb10: 6e65 7273 293a 200a 2020 2020 2727 270a  ners): .    '''.
-0000fb20: 2020 2020 4465 7465 726d 696e 6520 7468      Determine th
-0000fb30: 6520 5374 6162 6c65 2056 6f74 696e 6720  e Stable Voting 
-0000fb40: 7769 6e6e 6572 7320 666f 7220 7468 6520  winners for the 
-0000fb50: 7072 6f66 696c 6520 7768 696c 6520 6b65  profile while ke
-0000fb60: 6570 696e 6720 7472 6163 6b20 6f66 2074  eping track of t
-0000fb70: 6865 2077 696e 6e65 7273 2069 6e20 616e  he winners in an
-0000fb80: 7920 7375 6270 726f 6669 6c65 7320 6368  y subprofiles ch
-0000fb90: 6563 6b65 6420 6475 7269 6e67 2063 6f6d  ecked during com
-0000fba0: 7075 7461 7469 6f6e 2e20 0a20 2020 2027  putation. .    '
-0000fbb0: 2727 0a20 2020 200a 2020 2020 7376 5f77  ''.    .    sv_w
-0000fbc0: 696e 6e65 7273 203d 206c 6973 7428 290a  inners = list().
-0000fbd0: 2020 2020 0a20 2020 2075 6e64 6566 6561      .    undefea
-0000fbe0: 7465 645f 6361 6e64 6964 6174 6573 203d  ted_candidates =
-0000fbf0: 2073 706c 6974 5f63 7963 6c65 2865 6461   split_cycle(eda
-0000fc00: 7461 2c20 6375 7272 5f63 616e 6473 203d  ta, curr_cands =
-0000fc10: 2063 7572 725f 6361 6e64 732c 2073 7472   curr_cands, str
-0000fc20: 656e 6774 685f 6675 6e63 7469 6f6e 203d  ength_function =
-0000fc30: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
-0000fc40: 6f6e 290a 0a20 2020 2069 6620 6c65 6e28  on)..    if len(
-0000fc50: 6375 7272 5f63 616e 6473 2920 3d3d 2031  curr_cands) == 1
-0000fc60: 3a20 0a20 2020 2020 2020 206d 656d 5f73  : .        mem_s
-0000fc70: 765f 7769 6e6e 6572 735b 7475 706c 6528  v_winners[tuple(
-0000fc80: 6375 7272 5f63 616e 6473 295d 203d 2063  curr_cands)] = c
-0000fc90: 7572 725f 6361 6e64 730a 2020 2020 2020  urr_cands.      
-0000fca0: 2020 7265 7475 726e 2063 7572 725f 6361    return curr_ca
-0000fcb0: 6e64 732c 206d 656d 5f73 765f 7769 6e6e  nds, mem_sv_winn
-0000fcc0: 6572 730a 2020 2020 0a20 2020 206d 6172  ers.    .    mar
-0000fcd0: 6769 6e5f 7769 746e 6573 7369 6e67 5f77  gin_witnessing_w
-0000fce0: 696e 203d 202d 6d61 7468 2e69 6e66 0a0a  in = -math.inf..
-0000fcf0: 2020 2020 666f 7220 612c 2062 2c20 7320      for a, b, s 
-0000fd00: 696e 2073 6f72 7465 645f 6d61 7463 6865  in sorted_matche
-0000fd10: 733a 0a20 2020 2020 2020 2069 6620 7320  s:.        if s 
-0000fd20: 3c20 6d61 7267 696e 5f77 6974 6e65 7373  < margin_witness
-0000fd30: 696e 675f 7769 6e3a 200a 2020 2020 2020  ing_win: .      
-0000fd40: 2020 2020 2020 6272 6561 6b0a 2020 2020        break.    
-0000fd50: 2020 2020 6966 2061 2069 6e20 756e 6465      if a in unde
-0000fd60: 6665 6174 6564 5f63 616e 6469 6461 7465  feated_candidate
-0000fd70: 7320 616e 6420 6120 6e6f 7420 696e 2073  s and a not in s
-0000fd80: 765f 7769 6e6e 6572 733a 200a 2020 2020  v_winners: .    
-0000fd90: 2020 2020 2020 2020 6361 6e64 735f 6d69          cands_mi
-0000fda0: 6e75 735f 6220 3d20 5b63 2066 6f72 2063  nus_b = [c for c
-0000fdb0: 2069 6e20 6375 7272 5f63 616e 6473 2069   in curr_cands i
-0000fdc0: 6620 6320 213d 2062 5d0a 2020 2020 2020  f c != b].      
-0000fdd0: 2020 2020 2020 6361 6e64 735f 6d69 6e75        cands_minu
-0000fde0: 735f 625f 6b65 7920 3d20 7475 706c 6528  s_b_key = tuple(
-0000fdf0: 736f 7274 6564 2863 616e 6473 5f6d 696e  sorted(cands_min
-0000fe00: 7573 5f62 2929 0a20 2020 2020 2020 2020  us_b)).         
-0000fe10: 2020 2069 6620 6361 6e64 735f 6d69 6e75     if cands_minu
-0000fe20: 735f 625f 6b65 7920 6e6f 7420 696e 206d  s_b_key not in m
-0000fe30: 656d 5f73 765f 7769 6e6e 6572 732e 6b65  em_sv_winners.ke
-0000fe40: 7973 2829 3a20 0a20 2020 2020 2020 2020  ys(): .         
-0000fe50: 2020 2020 2020 2077 732c 206d 656d 5f73         ws, mem_s
-0000fe60: 765f 7769 6e6e 6572 7320 3d20 5f73 7461  v_winners = _sta
-0000fe70: 626c 655f 766f 7469 6e67 2865 6461 7461  ble_voting(edata
-0000fe80: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000fe90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000feb0: 2020 2020 2020 6375 7272 5f63 616e 6473        curr_cands
-0000fec0: 203d 2063 616e 6473 5f6d 696e 7573 5f62   = cands_minus_b
-0000fed0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000fee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ff00: 2020 2020 2020 7374 7265 6e67 7468 5f66        strength_f
-0000ff10: 756e 6374 696f 6e20 3d20 7374 7265 6e67  unction = streng
-0000ff20: 7468 5f66 756e 6374 696f 6e2c 0a20 2020  th_function,.   
-0000ff30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ff40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ff50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ff60: 2073 6f72 7465 645f 6d61 7463 6865 7320   sorted_matches 
-0000ff70: 3d20 5b28 612c 2063 2c20 7329 2066 6f72  = [(a, c, s) for
-0000ff80: 2061 2c20 632c 2073 2069 6e20 736f 7274   a, c, s in sort
-0000ff90: 6564 5f6d 6174 6368 6573 2069 6620 6120  ed_matches if a 
-0000ffa0: 213d 2062 2061 6e64 2063 2021 3d20 625d  != b and c != b]
-0000ffb0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000ffc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ffd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ffe0: 2020 2020 2020 6d65 6d5f 7376 5f77 696e        mem_sv_win
-0000fff0: 6e65 7273 203d 206d 656d 5f73 765f 7769  ners = mem_sv_wi
-00010000: 6e6e 6572 7329 0a20 2020 2020 2020 2020  nners).         
-00010010: 2020 2020 2020 206d 656d 5f73 765f 7769         mem_sv_wi
-00010020: 6e6e 6572 735b 6361 6e64 735f 6d69 6e75  nners[cands_minu
-00010030: 735f 625f 6b65 795d 203d 2077 730a 2020  s_b_key] = ws.  
-00010040: 2020 2020 2020 2020 2020 656c 7365 3a20            else: 
-00010050: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010060: 2077 7320 3d20 6d65 6d5f 7376 5f77 696e   ws = mem_sv_win
-00010070: 6e65 7273 5b63 616e 6473 5f6d 696e 7573  ners[cands_minus
-00010080: 5f62 5f6b 6579 5d0a 2020 2020 2020 2020  _b_key].        
-00010090: 2020 2020 6966 2061 2069 6e20 7773 3a0a      if a in ws:.
-000100a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000100b0: 7376 5f77 696e 6e65 7273 2e61 7070 656e  sv_winners.appen
-000100c0: 6428 6129 0a20 2020 2020 2020 2020 2020  d(a).           
-000100d0: 2020 2020 206d 6172 6769 6e5f 7769 746e       margin_witn
-000100e0: 6573 7369 6e67 5f77 696e 203d 2073 0a20  essing_win = s. 
-000100f0: 2020 2020 2020 2020 2020 2020 2020 200a                 .
-00010100: 2020 2020 7265 7475 726e 2073 765f 7769      return sv_wi
-00010110: 6e6e 6572 732c 206d 656d 5f73 765f 7769  nners, mem_sv_wi
-00010120: 6e6e 6572 730a 2020 2020 2020 2020 0a64  nners.        .d
-00010130: 6566 205f 7374 6162 6c65 5f76 6f74 696e  ef _stable_votin
-00010140: 675f 7769 7468 5f63 6f6e 646f 7263 6574  g_with_condorcet
-00010150: 5f63 6865 636b 280a 2020 2020 6564 6174  _check(.    edat
-00010160: 612c 200a 2020 2020 6375 7272 5f63 616e  a, .    curr_can
-00010170: 6473 3d4e 6f6e 652c 200a 2020 2020 7374  ds=None, .    st
-00010180: 7265 6e67 7468 5f66 756e 6374 696f 6e3d  rength_function=
-00010190: 4e6f 6e65 293a 200a 2020 2020 2222 220a  None): .    """.
-000101a0: 2020 2020 5374 6162 6c65 2056 6f74 696e      Stable Votin
-000101b0: 6720 6973 2043 6f6e 646f 7263 6574 2063  g is Condorcet c
-000101c0: 6f6e 7369 7374 656e 742e 2020 2049 7420  onsistent.   It 
-000101d0: 6973 2066 6173 7465 7220 746f 2073 6b69  is faster to ski
-000101e0: 7020 6578 6563 7574 696e 6720 7468 6520  p executing the 
-000101f0: 7265 6375 7273 6976 6520 616c 676f 7269  recursive algori
-00010200: 7468 6d20 7768 656e 2074 6865 7265 2069  thm when there i
-00010210: 7320 6120 436f 6e64 6f72 6365 7420 7769  s a Condorcet wi
-00010220: 6e6e 6572 2e20 200a 0a20 2020 2041 7267  nner.  ..    Arg
-00010230: 733a 0a20 2020 2020 2020 2065 6461 7461  s:.        edata
-00010240: 2028 5072 6f66 696c 652c 2050 726f 6669   (Profile, Profi
-00010250: 6c65 5769 7468 5469 6573 2c20 4d61 7267  leWithTies, Marg
-00010260: 696e 4772 6170 6829 3a20 416e 7920 656c  inGraph): Any el
-00010270: 6563 7469 6f6e 2064 6174 6120 7468 6174  ection data that
-00010280: 2068 6173 2061 2060 6d61 7267 696e 6020   has a `margin` 
-00010290: 6d65 7468 6f64 2e20 0a20 2020 2020 2020  method. .       
-000102a0: 2063 7572 725f 6361 6e64 7320 284c 6973   curr_cands (Lis
-000102b0: 745b 696e 745d 2c20 6f70 7469 6f6e 616c  t[int], optional
-000102c0: 293a 2049 6620 7365 742c 2074 6865 6e20  ): If set, then 
-000102d0: 6669 6e64 2074 6865 2077 696e 6e65 7273  find the winners
-000102e0: 2066 6f72 2074 6865 2070 726f 6669 6c65   for the profile
-000102f0: 2072 6573 7472 6963 7465 6420 746f 2074   restricted to t
-00010300: 6865 2063 616e 6469 6461 7465 7320 696e  he candidates in
-00010310: 2060 6063 7572 725f 6361 6e64 7360 600a   ``curr_cands``.
-00010320: 2020 2020 2020 2020 7374 7265 6e67 7468          strength
-00010330: 5f66 756e 6374 696f 6e20 2866 756e 6374  _function (funct
-00010340: 696f 6e2c 206f 7074 696f 6e61 6c29 3a20  ion, optional): 
-00010350: 5468 6520 7374 7265 6e67 7468 2066 756e  The strength fun
-00010360: 6374 696f 6e20 746f 2062 6520 7573 6564  ction to be used
-00010370: 2074 6f20 6361 6c63 756c 6174 6520 7468   to calculate th
-00010380: 6520 7374 7265 6e67 7468 206f 6620 6120  e strength of a 
-00010390: 7061 7468 2e20 2020 5468 6520 6465 6661  path.   The defa
-000103a0: 756c 7420 6973 2074 6865 206d 6172 6769  ult is the margi
-000103b0: 6e20 6d65 7468 6f64 206f 6620 6060 6564  n method of ``ed
-000103c0: 6174 6160 602e 2020 2054 6869 7320 6f6e  ata``.   This on
-000103d0: 6c79 206d 6174 7465 7273 2077 6865 6e20  ly matters when 
-000103e0: 7468 6520 6261 6c6c 6f74 7320 6172 6520  the ballots are 
-000103f0: 6e6f 7420 6c69 6e65 6172 206f 7264 6572  not linear order
-00010400: 732e 200a 0a20 2020 2052 6574 7572 6e73  s. ..    Returns
-00010410: 3a20 0a20 2020 2020 2020 2041 2073 6f72  : .        A sor
-00010420: 7465 6420 6c69 7374 206f 6620 6361 6e64  ted list of cand
-00010430: 6964 6174 6573 2e20 0a0a 2020 2020 2222  idates. ..    ""
-00010440: 220a 2020 2020 6377 203d 2065 6461 7461  ".    cw = edata
-00010450: 2e63 6f6e 646f 7263 6574 5f77 696e 6e65  .condorcet_winne
-00010460: 7228 6375 7272 5f63 616e 6473 203d 2063  r(curr_cands = c
-00010470: 7572 725f 6361 6e64 7329 0a20 2020 2069  urr_cands).    i
-00010480: 6620 6377 2069 7320 6e6f 7420 4e6f 6e65  f cw is not None
-00010490: 3a20 0a20 2020 2020 2020 2072 6574 7572  : .        retur
-000104a0: 6e20 5b63 775d 0a20 2020 2065 6c73 653a  n [cw].    else:
-000104b0: 200a 2020 2020 2020 2020 6375 7272 5f63   .        curr_c
-000104c0: 616e 6473 203d 2065 6461 7461 2e63 616e  ands = edata.can
-000104d0: 6469 6461 7465 7320 6966 2063 7572 725f  didates if curr_
-000104e0: 6361 6e64 7320 6973 204e 6f6e 6520 656c  cands is None el
-000104f0: 7365 2063 7572 725f 6361 6e64 730a 2020  se curr_cands.  
-00010500: 2020 2020 2020 7374 7265 6e67 7468 5f66        strength_f
-00010510: 756e 6374 696f 6e20 3d20 6564 6174 612e  unction = edata.
-00010520: 6d61 7267 696e 2069 6620 7374 7265 6e67  margin if streng
-00010530: 7468 5f66 756e 6374 696f 6e20 6973 204e  th_function is N
-00010540: 6f6e 6520 656c 7365 2073 7472 656e 6774  one else strengt
-00010550: 685f 6675 6e63 7469 6f6e 2020 0a0a 2020  h_function  ..  
-00010560: 2020 2020 2020 6d61 7463 6865 7320 3d20        matches = 
-00010570: 5b28 612c 2062 2c20 7374 7265 6e67 7468  [(a, b, strength
-00010580: 5f66 756e 6374 696f 6e28 612c 2062 2929  _function(a, b))
-00010590: 2066 6f72 2061 2069 6e20 6375 7272 5f63   for a in curr_c
-000105a0: 616e 6473 2066 6f72 2062 2069 6e20 6375  ands for b in cu
-000105b0: 7272 5f63 616e 6473 2069 6620 6120 213d  rr_cands if a !=
-000105c0: 2062 5d0a 2020 2020 2020 2020 736f 7274   b].        sort
-000105d0: 6564 5f6d 6174 6368 6573 203d 2073 6f72  ed_matches = sor
-000105e0: 7465 6428 6d61 7463 6865 732c 2072 6576  ted(matches, rev
-000105f0: 6572 7365 3d54 7275 652c 206b 6579 3d6c  erse=True, key=l
-00010600: 616d 6264 6120 6d5f 775f 7765 6967 6874  ambda m_w_weight
-00010610: 3a20 6d5f 775f 7765 6967 6874 5b32 5d29  : m_w_weight[2])
-00010620: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00010630: 2073 6f72 7465 6428 5f73 7461 626c 655f   sorted(_stable_
-00010640: 766f 7469 6e67 2865 6461 7461 2c20 0a20  voting(edata, . 
-00010650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010670: 2020 2063 7572 725f 6361 6e64 7320 3d20     curr_cands = 
-00010680: 6375 7272 5f63 616e 6473 2c20 0a20 2020  curr_cands, .   
+000002c0: 696d 706f 7274 206d 756c 7469 7072 6f63  import multiproc
+000002d0: 6573 7369 6e67 2061 7320 6d70 0a66 726f  essing as mp.fro
+000002e0: 6d20 6d75 6c74 6970 726f 6365 7373 696e  m multiprocessin
+000002f0: 6720 696d 706f 7274 2050 6f6f 6c0a 6672  g import Pool.fr
+00000300: 6f6d 2066 756e 6374 6f6f 6c73 2069 6d70  om functools imp
+00000310: 6f72 7420 7061 7274 6961 6c0a 0a6d 696e  ort partial..min
+00000320: 696d 6178 5f70 726f 7065 7274 6965 7320  imax_properties 
+00000330: 3d20 566f 7469 6e67 4d65 7468 6f64 5072  = VotingMethodPr
+00000340: 6f70 6572 7469 6573 280a 2020 2020 636f  operties(.    co
+00000350: 6e64 6f72 6365 745f 7769 6e6e 6572 3d54  ndorcet_winner=T
+00000360: 7275 652c 200a 2020 2020 636f 6e64 6f72  rue, .    condor
+00000370: 6365 745f 6c6f 7365 723d 4661 6c73 652c  cet_loser=False,
+00000380: 0a20 2020 2070 6172 6574 6f5f 646f 6d69  .    pareto_domi
+00000390: 6e61 6e63 653d 5472 7565 2c0a 2020 2020  nance=True,.    
+000003a0: 706f 7369 7469 7665 5f69 6e76 6f6c 7665  positive_involve
+000003b0: 6d65 6e74 3d54 7275 652c 200a 2020 2020  ment=True, .    
+000003c0: 290a 4076 6d28 6e61 6d65 203d 2022 4d69  ).@vm(name = "Mi
+000003d0: 6e69 6d61 7822 2c0a 2020 2020 7072 6f70  nimax",.    prop
+000003e0: 6572 7469 6573 3d6d 696e 696d 6178 5f70  erties=minimax_p
+000003f0: 726f 7065 7274 6965 732c 0a20 2020 2069  roperties,.    i
+00000400: 6e70 7574 5f74 7970 6573 3d5b 456c 6563  nput_types=[Elec
+00000410: 7469 6f6e 5479 7065 732e 5052 4f46 494c  tionTypes.PROFIL
+00000420: 452c 2045 6c65 6374 696f 6e54 7970 6573  E, ElectionTypes
+00000430: 2e50 524f 4649 4c45 5f57 4954 485f 5449  .PROFILE_WITH_TI
+00000440: 4553 2c20 456c 6563 7469 6f6e 5479 7065  ES, ElectionType
+00000450: 732e 4d41 5247 494e 5f47 5241 5048 5d0a  s.MARGIN_GRAPH].
+00000460: 2020 2020 290a 6465 6620 6d69 6e69 6d61      ).def minima
+00000470: 7828 6564 6174 612c 2063 7572 725f 6361  x(edata, curr_ca
+00000480: 6e64 7320 3d20 4e6f 6e65 2c20 7374 7265  nds = None, stre
+00000490: 6e67 7468 5f66 756e 6374 696f 6e20 3d20  ngth_function = 
+000004a0: 4e6f 6e65 293a 2020 200a 2020 2020 2222  None):   .    ""
+000004b0: 220a 2020 2020 5468 6520 4d69 6e69 6d61  ".    The Minima
+000004c0: 7820 7769 6e6e 6572 7320 6172 6520 7468  x winners are th
+000004d0: 6520 6361 6e64 6964 6174 6573 2077 6974  e candidates wit
+000004e0: 6820 7468 6520 736d 616c 6c65 7374 206d  h the smallest m
+000004f0: 6178 696d 756d 2070 6169 7277 6973 6520  aximum pairwise 
+00000500: 6c6f 7373 2e20 2054 6861 7420 6973 2c20  loss.  That is, 
+00000510: 666f 7220 6561 6368 2063 616e 6469 6461  for each candida
+00000520: 7465 203a 6d61 7468 3a60 6160 2c20 6669  te :math:`a`, fi
+00000530: 6e64 2074 6865 2062 6967 6765 7374 206d  nd the biggest m
+00000540: 6172 6769 6e20 6f66 2061 2063 616e 6469  argin of a candi
+00000550: 6461 7465 203a 6d61 7468 3a60 6260 206f  date :math:`b` o
+00000560: 7665 7220 3a6d 6174 683a 6061 602c 2074  ver :math:`a`, t
+00000570: 6865 6e20 656c 6563 7420 7468 6520 6361  hen elect the ca
+00000580: 6e64 6964 6174 6528 7329 2077 6974 6820  ndidate(s) with 
+00000590: 7468 6520 736d 616c 6c65 7374 2073 7563  the smallest suc
+000005a0: 6820 6c6f 7373 2e20 416c 736f 206b 6e6f  h loss. Also kno
+000005b0: 776e 2061 7320 7468 6520 5369 6d70 736f  wn as the Simpso
+000005c0: 6e2d 4b72 616d 6572 2052 756c 652e 0a20  n-Kramer Rule.. 
+000005d0: 2020 200a 2020 2020 4172 6773 3a0a 2020     .    Args:.  
+000005e0: 2020 2020 2020 6564 6174 6120 2850 726f        edata (Pro
+000005f0: 6669 6c65 2c20 5072 6f66 696c 6557 6974  file, ProfileWit
+00000600: 6854 6965 732c 204d 6172 6769 6e47 7261  hTies, MarginGra
+00000610: 7068 293a 2041 6e79 2065 6c65 6374 696f  ph): Any electio
+00000620: 6e20 6461 7461 2074 6861 7420 6861 7320  n data that has 
+00000630: 6120 606d 6172 6769 6e60 206d 6574 686f  a `margin` metho
+00000640: 642e 200a 2020 2020 2020 2020 6375 7272  d. .        curr
+00000650: 5f63 616e 6473 2028 4c69 7374 5b69 6e74  _cands (List[int
+00000660: 5d2c 206f 7074 696f 6e61 6c29 3a20 4966  ], optional): If
+00000670: 2073 6574 2c20 7468 656e 2066 696e 6420   set, then find 
+00000680: 7468 6520 7769 6e6e 6572 7320 666f 7220  the winners for 
+00000690: 7468 6520 7072 6f66 696c 6520 7265 7374  the profile rest
+000006a0: 7269 6374 6564 2074 6f20 7468 6520 6361  ricted to the ca
+000006b0: 6e64 6964 6174 6573 2069 6e20 6060 6375  ndidates in ``cu
+000006c0: 7272 5f63 616e 6473 6060 0a0a 2020 2020  rr_cands``..    
+000006d0: 5265 7475 726e 733a 200a 2020 2020 2020  Returns: .      
+000006e0: 2020 4120 736f 7274 6564 206c 6973 7420    A sorted list 
+000006f0: 6f66 2063 616e 6469 6461 7465 730a 0a20  of candidates.. 
+00000700: 2020 202e 2e20 7365 6561 6c73 6f3a 3a0a     .. seealso::.
+00000710: 0a20 2020 2020 2020 203a 6d65 7468 3a60  .        :meth:`
+00000720: 7072 6566 5f76 6f74 696e 672e 6d61 7267  pref_voting.marg
+00000730: 696e 5f62 6173 6564 5f6d 6574 686f 6473  in_based_methods
+00000740: 2e6d 696e 696d 6178 5f73 636f 7265 7360  .minimax_scores`
+00000750: 0a0a 2020 2020 3a45 7861 6d70 6c65 3a20  ..    :Example: 
+00000760: 0a0a 2020 2020 2e2e 2070 6c6f 743a 3a20  ..    .. plot:: 
+00000770: 206d 6172 6769 6e5f 6772 6170 6873 5f65   margin_graphs_e
+00000780: 7861 6d70 6c65 732f 6d67 5f65 785f 6d69  xamples/mg_ex_mi
+00000790: 6e69 6d61 782e 7079 0a20 2020 2020 2020  nimax.py.       
+000007a0: 203a 636f 6e74 6578 743a 2072 6573 6574   :context: reset
+000007b0: 2020 0a20 2020 2020 2020 203a 696e 636c    .        :incl
+000007c0: 7564 652d 736f 7572 6365 3a20 5472 7565  ude-source: True
+000007d0: 0a0a 0a20 2020 202e 2e20 636f 6465 2d62  ...    .. code-b
+000007e0: 6c6f 636b 3a3a 200a 0a20 2020 2020 2020  lock:: ..       
+000007f0: 2066 726f 6d20 7072 6566 5f76 6f74 696e   from pref_votin
+00000800: 672e 6d61 7267 696e 5f62 6173 6564 5f6d  g.margin_based_m
+00000810: 6574 686f 6473 2069 6d70 6f72 7420 6d69  ethods import mi
+00000820: 6e69 6d61 780a 0a20 2020 2020 2020 206d  nimax..        m
+00000830: 696e 696d 6178 2e64 6973 706c 6179 2870  inimax.display(p
+00000840: 726f 6629 0a0a 0a20 2020 202e 2e20 6578  rof)...    .. ex
+00000850: 6563 5f63 6f64 653a 3a20 0a20 2020 2020  ec_code:: .     
+00000860: 2020 203a 6869 6465 5f63 6f64 653a 0a0a     :hide_code:..
+00000870: 2020 2020 2020 2020 6672 6f6d 2070 7265          from pre
+00000880: 665f 766f 7469 6e67 2e70 726f 6669 6c65  f_voting.profile
+00000890: 7320 696d 706f 7274 2050 726f 6669 6c65  s import Profile
+000008a0: 0a20 2020 2020 2020 2066 726f 6d20 7072  .        from pr
+000008b0: 6566 5f76 6f74 696e 672e 6d61 7267 696e  ef_voting.margin
+000008c0: 5f62 6173 6564 5f6d 6574 686f 6473 2069  _based_methods i
+000008d0: 6d70 6f72 7420 6d69 6e69 6d61 780a 2020  mport minimax.  
+000008e0: 2020 2020 2020 0a20 2020 2020 2020 2070        .        p
+000008f0: 726f 6620 3d20 5072 6f66 696c 6528 5b5b  rof = Profile([[
+00000900: 332c 2030 2c20 312c 2032 5d2c 205b 312c  3, 0, 1, 2], [1,
+00000910: 2033 2c20 322c 2030 5d2c 205b 312c 2033   3, 2, 0], [1, 3
+00000920: 2c20 302c 2032 5d2c 205b 312c 2032 2c20  , 0, 2], [1, 2, 
+00000930: 302c 2033 5d2c 205b 332c 2032 2c20 302c  0, 3], [3, 2, 0,
+00000940: 2031 5d2c 205b 302c 2032 2c20 312c 2033   1], [0, 2, 1, 3
+00000950: 5d5d 2c20 5b31 2c20 312c 2031 2c20 312c  ]], [1, 1, 1, 1,
+00000960: 2032 2c20 315d 290a 0a20 2020 2020 2020   2, 1])..       
+00000970: 206d 696e 696d 6178 2e64 6973 706c 6179   minimax.display
+00000980: 2870 726f 6629 0a0a 2020 2020 2222 220a  (prof)..    """.
+00000990: 0a20 2020 2063 616e 6469 6461 7465 7320  .    candidates 
+000009a0: 3d20 6564 6174 612e 6361 6e64 6964 6174  = edata.candidat
+000009b0: 6573 2069 6620 6375 7272 5f63 616e 6473  es if curr_cands
+000009c0: 2069 7320 4e6f 6e65 2065 6c73 6520 6375   is None else cu
+000009d0: 7272 5f63 616e 6473 2020 2020 0a20 2020  rr_cands    .   
+000009e0: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
+000009f0: 6f6e 203d 2065 6461 7461 2e6d 6172 6769  on = edata.margi
+00000a00: 6e20 6966 2073 7472 656e 6774 685f 6675  n if strength_fu
+00000a10: 6e63 7469 6f6e 2069 7320 4e6f 6e65 2065  nction is None e
+00000a20: 6c73 6520 7374 7265 6e67 7468 5f66 756e  lse strength_fun
+00000a30: 6374 696f 6e0a 0a20 2020 2073 636f 7265  ction..    score
+00000a40: 7320 3d20 7b63 3a20 6d61 7828 5b73 7472  s = {c: max([str
+00000a50: 656e 6774 685f 6675 6e63 7469 6f6e 285f  ength_function(_
+00000a60: 632c 2063 2920 666f 7220 5f63 2069 6e20  c, c) for _c in 
+00000a70: 6564 6174 612e 646f 6d69 6e61 746f 7273  edata.dominators
+00000a80: 2863 2920 6966 205f 6320 696e 2063 616e  (c) if _c in can
+00000a90: 6469 6461 7465 735d 2920 6966 2061 6e79  didates]) if any
+00000aa0: 285b 5f63 2069 6e20 6564 6174 612e 646f  ([_c in edata.do
+00000ab0: 6d69 6e61 746f 7273 2863 2920 666f 7220  minators(c) for 
+00000ac0: 5f63 2069 6e20 6361 6e64 6964 6174 6573  _c in candidates
+00000ad0: 5d29 2065 6c73 6520 3020 0a20 2020 2020  ]) else 0 .     
+00000ae0: 2020 2020 2020 2020 2066 6f72 2063 2069           for c i
+00000af0: 6e20 6361 6e64 6964 6174 6573 7d0a 2020  n candidates}.  
+00000b00: 2020 6d69 6e5f 7363 6f72 6520 3d20 6d69    min_score = mi
+00000b10: 6e28 7363 6f72 6573 2e76 616c 7565 7328  n(scores.values(
+00000b20: 2929 0a20 2020 2072 6574 7572 6e20 736f  )).    return so
+00000b30: 7274 6564 285b 6320 666f 7220 6320 696e  rted([c for c in
+00000b40: 2063 616e 6469 6461 7465 7320 6966 2073   candidates if s
+00000b50: 636f 7265 735b 635d 203d 3d20 6d69 6e5f  cores[c] == min_
+00000b60: 7363 6f72 655d 290a 0a0a 6465 6620 6d69  score])...def mi
+00000b70: 6e69 6d61 785f 7363 6f72 6573 2865 6461  nimax_scores(eda
+00000b80: 7461 2c20 6375 7272 5f63 616e 6473 203d  ta, curr_cands =
+00000b90: 204e 6f6e 652c 2073 636f 7265 5f6d 6574   None, score_met
+00000ba0: 686f 643d 226d 6172 6769 6e73 2229 3a0a  hod="margins"):.
+00000bb0: 2020 2020 2222 2252 6574 7572 6e20 7468      """Return th
+00000bc0: 6520 6d69 6e69 6d61 7820 7363 6f72 6573  e minimax scores
+00000bd0: 2066 6f72 2065 6163 6820 6361 6e64 6964   for each candid
+00000be0: 6174 652c 2077 6865 7265 2074 6865 206d  ate, where the m
+00000bf0: 696e 696d 6178 2073 636f 7265 2066 6f72  inimax score for
+00000c00: 203a 6d61 7468 3a60 6360 2069 7320 2d31   :math:`c` is -1
+00000c10: 202a 2074 6865 206d 6178 696d 756d 2070   * the maximum p
+00000c20: 6169 7277 6973 6520 6d61 6a6f 7269 7479  airwise majority
+00000c30: 206c 6f73 732e 200a 0a20 2020 2041 7267   loss. ..    Arg
+00000c40: 733a 0a20 2020 2020 2020 2065 6461 7461  s:.        edata
+00000c50: 2028 5072 6f66 696c 652c 2050 726f 6669   (Profile, Profi
+00000c60: 6c65 5769 7468 5469 6573 2c20 4d61 7267  leWithTies, Marg
+00000c70: 696e 4772 6170 6829 3a20 416e 7920 656c  inGraph): Any el
+00000c80: 6563 7469 6f6e 2064 6174 6120 7468 6174  ection data that
+00000c90: 2068 6173 2061 2060 6d61 7267 696e 6020   has a `margin` 
+00000ca0: 6d65 7468 6f64 2e20 0a20 2020 2020 2020  method. .       
+00000cb0: 2063 7572 725f 6361 6e64 7320 284c 6973   curr_cands (Lis
+00000cc0: 745b 696e 745d 2c20 6f70 7469 6f6e 616c  t[int], optional
+00000cd0: 293a 2049 6620 7365 742c 2074 6865 6e20  ): If set, then 
+00000ce0: 6669 6e64 2074 6865 2077 696e 6e65 7273  find the winners
+00000cf0: 2066 6f72 2074 6865 2070 726f 6669 6c65   for the profile
+00000d00: 2072 6573 7472 6963 7465 6420 746f 2074   restricted to t
+00000d10: 6865 2063 616e 6469 6461 7465 7320 696e  he candidates in
+00000d20: 2060 6063 7572 725f 6361 6e64 7360 600a   ``curr_cands``.
+00000d30: 2020 2020 2020 2020 7363 6f72 655f 6d65          score_me
+00000d40: 7468 6f64 2028 7374 722c 206f 7074 696f  thod (str, optio
+00000d50: 6e61 6c29 3a20 4f70 7469 6f6e 7320 696e  nal): Options in
+00000d60: 636c 7564 6520 226d 6172 6769 6e73 2220  clude "margins" 
+00000d70: 2874 6865 2064 6566 6175 6c74 292c 2022  (the default), "
+00000d80: 7769 6e6e 696e 6722 2061 7373 6967 6e73  winning" assigns
+00000d90: 2074 6f20 6561 6368 2063 616e 6469 6461   to each candida
+00000da0: 7465 203a 6d61 7468 3a60 6360 2074 6865  te :math:`c` the
+00000db0: 206d 6178 696d 756d 2073 7570 706f 7274   maximum support
+00000dc0: 206f 6620 6120 6361 6e64 6964 6174 6520   of a candidate 
+00000dd0: 6d61 6a6f 7269 7479 2070 7265 6665 7272  majority preferr
+00000de0: 6564 2074 6f20 3a6d 6174 683a 6063 602c  ed to :math:`c`,
+00000df0: 2020 616e 6420 2270 6169 7277 6973 655f    and "pairwise_
+00000e00: 6f70 706f 7369 7469 6f6e 2220 6173 7369  opposition" assi
+00000e10: 676e 7320 746f 2065 6163 6820 6361 6e64  gns to each cand
+00000e20: 6964 6174 6520 3a6d 6174 683a 6063 6020  idate :math:`c` 
+00000e30: 7468 6520 6d61 7869 6d75 6d20 7375 7070  the maximum supp
+00000e40: 6f72 7420 6f66 2061 6e79 2063 616e 6469  ort of any candi
+00000e50: 6461 7465 206f 7665 7220 3a6d 6174 683a  date over :math:
+00000e60: 6063 602e 2020 2054 6865 7365 2073 636f  `c`.   These sco
+00000e70: 7265 7320 6f6e 6c79 206c 6561 6420 746f  res only lead to
+00000e80: 2064 6966 6665 7265 6e74 2072 6573 756c   different resul
+00000e90: 7473 206f 6e20 6e6f 6e2d 6c69 6e65 6172  ts on non-linear
+00000ea0: 2070 726f 6669 6c65 732e 200a 0a20 2020   profiles. ..   
+00000eb0: 2052 6574 7572 6e73 3a20 0a20 2020 2020   Returns: .     
+00000ec0: 2020 2041 2064 6963 7469 6f6e 6172 7920     A dictionary 
+00000ed0: 6173 736f 6369 6174 696e 6720 6561 6368  associating each
+00000ee0: 2063 616e 6469 6461 7465 2077 6974 6820   candidate with 
+00000ef0: 6974 7320 6d69 6e69 6d61 7820 7363 6f72  its minimax scor
+00000f00: 652e 0a0a 2020 2020 2e2e 2073 6565 616c  e...    .. seeal
+00000f10: 736f 3a3a 0a0a 2020 2020 2020 2020 3a6d  so::..        :m
+00000f20: 6574 683a 6070 7265 665f 766f 7469 6e67  eth:`pref_voting
+00000f30: 2e6d 6172 6769 6e5f 6261 7365 645f 6d65  .margin_based_me
+00000f40: 7468 6f64 732e 6d69 6e69 6d61 7860 0a0a  thods.minimax`..
+00000f50: 2020 2020 3a45 7861 6d70 6c65 3a20 0a0a      :Example: ..
+00000f60: 2020 2020 2e2e 2070 6c6f 743a 3a20 206d      .. plot::  m
+00000f70: 6172 6769 6e5f 6772 6170 6873 5f65 7861  argin_graphs_exa
+00000f80: 6d70 6c65 732f 6d67 5f65 785f 6d69 6e69  mples/mg_ex_mini
+00000f90: 6d61 782e 7079 0a20 2020 2020 2020 203a  max.py.        :
+00000fa0: 636f 6e74 6578 743a 2072 6573 6574 2020  context: reset  
+00000fb0: 0a20 2020 2020 2020 203a 696e 636c 7564  .        :includ
+00000fc0: 652d 736f 7572 6365 3a20 5472 7565 0a0a  e-source: True..
+00000fd0: 0a20 2020 202e 2e20 636f 6465 2d62 6c6f  .    .. code-blo
+00000fe0: 636b 3a3a 200a 0a20 2020 2020 2020 2066  ck:: ..        f
+00000ff0: 726f 6d20 7072 6566 5f76 6f74 696e 672e  rom pref_voting.
+00001000: 6d61 7267 696e 5f62 6173 6564 5f6d 6574  margin_based_met
+00001010: 686f 6473 2069 6d70 6f72 7420 6d69 6e69  hods import mini
+00001020: 6d61 785f 7363 6f72 6573 2c20 6d69 6e69  max_scores, mini
+00001030: 6d61 780a 0a20 2020 2020 2020 206d 696e  max..        min
+00001040: 696d 6178 2e64 6973 706c 6179 2870 726f  imax.display(pro
+00001050: 6629 0a20 2020 2020 2020 2070 7269 6e74  f).        print
+00001060: 286d 696e 696d 6178 5f73 636f 7265 7328  (minimax_scores(
+00001070: 7072 6f66 2929 0a0a 0a20 2020 202e 2e20  prof))...    .. 
+00001080: 6578 6563 5f63 6f64 653a 3a20 0a20 2020  exec_code:: .   
+00001090: 2020 2020 203a 6869 6465 5f63 6f64 653a       :hide_code:
+000010a0: 0a0a 2020 2020 2020 2020 6672 6f6d 2070  ..        from p
+000010b0: 7265 665f 766f 7469 6e67 2e70 726f 6669  ref_voting.profi
+000010c0: 6c65 7320 696d 706f 7274 2050 726f 6669  les import Profi
+000010d0: 6c65 0a20 2020 2020 2020 2066 726f 6d20  le.        from 
+000010e0: 7072 6566 5f76 6f74 696e 672e 6d61 7267  pref_voting.marg
+000010f0: 696e 5f62 6173 6564 5f6d 6574 686f 6473  in_based_methods
+00001100: 2069 6d70 6f72 7420 6d69 6e69 6d61 782c   import minimax,
+00001110: 206d 696e 696d 6178 5f73 636f 7265 730a   minimax_scores.
+00001120: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00001130: 2070 726f 6620 3d20 5072 6f66 696c 6528   prof = Profile(
+00001140: 5b5b 332c 2030 2c20 312c 2032 5d2c 205b  [[3, 0, 1, 2], [
+00001150: 312c 2033 2c20 322c 2030 5d2c 205b 312c  1, 3, 2, 0], [1,
+00001160: 2033 2c20 302c 2032 5d2c 205b 312c 2032   3, 0, 2], [1, 2
+00001170: 2c20 302c 2033 5d2c 205b 332c 2032 2c20  , 0, 3], [3, 2, 
+00001180: 302c 2031 5d2c 205b 302c 2032 2c20 312c  0, 1], [0, 2, 1,
+00001190: 2033 5d5d 2c20 5b31 2c20 312c 2031 2c20   3]], [1, 1, 1, 
+000011a0: 312c 2032 2c20 315d 290a 0a20 2020 2020  1, 2, 1])..     
+000011b0: 2020 206d 696e 696d 6178 2e64 6973 706c     minimax.displ
+000011c0: 6179 2870 726f 6629 0a20 2020 2020 2020  ay(prof).       
+000011d0: 2070 7269 6e74 286d 696e 696d 6178 5f73   print(minimax_s
+000011e0: 636f 7265 7328 7072 6f66 2929 0a0a 2020  cores(prof))..  
+000011f0: 2020 2222 220a 2020 2020 0a20 2020 2063    """.    .    c
+00001200: 616e 6469 6461 7465 7320 3d20 6564 6174  andidates = edat
+00001210: 612e 6361 6e64 6964 6174 6573 2069 6620  a.candidates if 
+00001220: 6375 7272 5f63 616e 6473 2069 7320 4e6f  curr_cands is No
+00001230: 6e65 2065 6c73 6520 6375 7272 5f63 616e  ne else curr_can
+00001240: 6473 0a0a 2020 2020 6966 206c 656e 2863  ds..    if len(c
+00001250: 616e 6469 6461 7465 7329 203d 3d20 313a  andidates) == 1:
+00001260: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00001270: 7b63 3a20 3020 666f 7220 6320 696e 2063  {c: 0 for c in c
+00001280: 616e 6469 6461 7465 737d 0a20 2020 200a  andidates}.    .
+00001290: 2020 2020 2320 7468 6572 6520 6172 6520      # there are 
+000012a0: 6469 6666 6572 656e 7420 7363 6f72 696e  different scorin
+000012b0: 6720 6675 6e63 7469 6f6e 7320 7468 6174  g functions that
+000012c0: 2063 616e 2062 6520 7573 6564 2074 6f20   can be used to 
+000012d0: 6d65 6173 7572 6520 7468 6520 776f 7273  measure the wors
+000012e0: 6520 6c6f 7373 2066 6f72 2065 6163 6820  e loss for each 
+000012f0: 0a20 2020 2023 2063 616e 6469 6461 7465  .    # candidate
+00001300: 2e20 5468 6573 6520 616c 6c20 7072 6f64  . These all prod
+00001310: 7563 6520 7468 6520 7361 6d65 2073 6574  uce the same set
+00001320: 206f 6620 7769 6e6e 6572 7320 7768 656e   of winners when
+00001330: 2076 6f74 6572 7320 7375 626d 6974 206c   voters submit l
+00001340: 696e 6561 7220 6f72 6465 7273 2e20 0a20  inear orders. . 
+00001350: 2020 2073 636f 7265 5f66 756e 6374 696f     score_functio
+00001360: 6e73 203d 207b 0a20 2020 2020 2020 2022  ns = {.        "
+00001370: 7769 6e6e 696e 6722 3a20 6c61 6d62 6461  winning": lambda
+00001380: 2063 732c 2063 3a20 6d61 7828 5b65 6461   cs, c: max([eda
+00001390: 7461 2e73 7570 706f 7274 285f 632c 6329  ta.support(_c,c)
+000013a0: 2066 6f72 205f 6320 696e 2063 735d 2920   for _c in cs]) 
+000013b0: 6966 206c 656e 2863 7329 203e 2030 2065  if len(cs) > 0 e
+000013c0: 6c73 6520 302c 0a20 2020 2020 2020 2022  lse 0,.        "
+000013d0: 6d61 7267 696e 7322 3a20 6c61 6d62 6461  margins": lambda
+000013e0: 2063 732c 2063 3a20 6d61 7828 5b65 6461   cs, c: max([eda
+000013f0: 7461 2e6d 6172 6769 6e28 5f63 2c63 2920  ta.margin(_c,c) 
+00001400: 666f 7220 5f63 2069 6e20 6373 5d29 2069  for _c in cs]) i
+00001410: 6620 6c65 6e28 6373 2920 3e20 3020 656c  f len(cs) > 0 el
+00001420: 7365 2030 2c0a 2020 2020 2020 2020 2270  se 0,.        "p
+00001430: 6169 7277 6973 655f 6f70 706f 7369 7469  airwise_oppositi
+00001440: 6f6e 223a 206c 616d 6264 6120 6373 2c20  on": lambda cs, 
+00001450: 633a 206d 6178 285b 6564 6174 612e 7375  c: max([edata.su
+00001460: 7070 6f72 7428 5f63 2c63 2920 666f 7220  pport(_c,c) for 
+00001470: 5f63 2069 6e20 6373 5d29 0a20 2020 207d  _c in cs]).    }
+00001480: 200a 2020 2020 0a20 2020 2063 616e 6473   .    .    cands
+00001490: 203d 207b 0a20 2020 2020 2020 2022 7769   = {.        "wi
+000014a0: 6e6e 696e 6722 3a20 6c61 6d62 6461 2063  nning": lambda c
+000014b0: 3a20 6564 6174 612e 646f 6d69 6e61 746f  : edata.dominato
+000014c0: 7273 2863 2c20 6375 7272 5f63 616e 6473  rs(c, curr_cands
+000014d0: 203d 2063 7572 725f 6361 6e64 7329 2c0a   = curr_cands),.
+000014e0: 2020 2020 2020 2020 226d 6172 6769 6e73          "margins
+000014f0: 223a 206c 616d 6264 6120 633a 2065 6461  ": lambda c: eda
+00001500: 7461 2e64 6f6d 696e 6174 6f72 7328 632c  ta.dominators(c,
+00001510: 2063 7572 725f 6361 6e64 7320 3d20 6375   curr_cands = cu
+00001520: 7272 5f63 616e 6473 292c 0a20 2020 2020  rr_cands),.     
+00001530: 2020 2022 7061 6972 7769 7365 5f6f 7070     "pairwise_opp
+00001540: 6f73 6974 696f 6e22 3a20 6c61 6d62 6461  osition": lambda
+00001550: 2063 3a20 5b5f 6320 666f 7220 5f63 2069   c: [_c for _c i
+00001560: 6e20 6361 6e64 6964 6174 6573 2069 6620  n candidates if 
+00001570: 5f63 2021 3d20 635d 0a20 2020 207d 200a  _c != c].    } .
+00001580: 0a20 2020 2072 6574 7572 6e20 7b63 3a20  .    return {c: 
+00001590: 2d31 202a 2073 636f 7265 5f66 756e 6374  -1 * score_funct
+000015a0: 696f 6e73 5b73 636f 7265 5f6d 6574 686f  ions[score_metho
+000015b0: 645d 2863 616e 6473 5b73 636f 7265 5f6d  d](cands[score_m
+000015c0: 6574 686f 645d 2863 292c 2063 2920 666f  ethod](c), c) fo
+000015d0: 7220 6320 696e 2063 616e 6469 6461 7465  r c in candidate
+000015e0: 737d 0a0a 0a64 6566 206d 6178 696d 616c  s}...def maximal
+000015f0: 5f65 6c65 6d65 6e74 7328 6729 3a20 0a20  _elements(g): . 
+00001600: 2020 2022 2222 7265 7475 726e 2074 6865     """return the
+00001610: 206e 6f64 6573 2069 6e20 6720 7769 7468   nodes in g with
+00001620: 206e 6f20 696e 636f 6d69 6e67 2061 7272   no incoming arr
+00001630: 6f77 732e 2222 220a 2020 2020 7265 7475  ows.""".    retu
+00001640: 726e 205b 6e20 666f 7220 6e20 696e 2067  rn [n for n in g
+00001650: 2e6e 6f64 6573 2069 6620 672e 696e 5f64  .nodes if g.in_d
+00001660: 6567 7265 6528 6e29 203d 3d20 305d 0a0a  egree(n) == 0]..
+00001670: 0a64 6566 205f 6265 6174 5f70 6174 685f  .def _beat_path_
+00001680: 6261 7369 6328 6564 6174 612c 200a 2020  basic(edata, .  
+00001690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000016a0: 2020 2063 7572 725f 6361 6e64 7320 3d20     curr_cands = 
+000016b0: 4e6f 6e65 2c20 0a20 2020 2020 2020 2020  None, .         
+000016c0: 2020 2020 2020 2020 2020 2020 7374 7265              stre
+000016d0: 6e67 7468 5f66 756e 6374 696f 6e20 3d20  ngth_function = 
+000016e0: 4e6f 6e65 293a 200a 2020 2020 2222 2241  None): .    """A
+000016f0: 6e20 696d 706c 656d 656e 7461 7469 6f6e  n implementation
+00001700: 206f 6620 7468 6520 4265 6174 2050 6174   of the Beat Pat
+00001710: 6820 6d65 7468 6f64 2074 6861 7420 7573  h method that us
+00001720: 6573 2061 2062 6173 6963 2061 6c67 6f72  es a basic algor
+00001730: 6974 686d 2e20 2054 6869 7320 6973 206e  ithm.  This is n
+00001740: 6f74 2065 6666 6963 6965 6e74 2066 6f72  ot efficient for
+00001750: 206c 6172 6765 2067 7261 7068 732e 0a20   large graphs.. 
+00001760: 2020 200a 2020 2020 4172 6773 3a0a 2020     .    Args:.  
+00001770: 2020 2020 2020 6564 6174 6120 2850 726f        edata (Pro
+00001780: 6669 6c65 2c20 5072 6f66 696c 6557 6974  file, ProfileWit
+00001790: 6854 6965 732c 204d 6172 6769 6e47 7261  hTies, MarginGra
+000017a0: 7068 293a 2041 6e79 2065 6c65 6374 696f  ph): Any electio
+000017b0: 6e20 6461 7461 2074 6861 7420 6861 7320  n data that has 
+000017c0: 6120 606d 6172 6769 6e60 206d 6574 686f  a `margin` metho
+000017d0: 642e 200a 2020 2020 2020 2020 6375 7272  d. .        curr
+000017e0: 5f63 616e 6473 2028 4c69 7374 5b69 6e74  _cands (List[int
+000017f0: 5d2c 206f 7074 696f 6e61 6c29 3a20 4966  ], optional): If
+00001800: 2073 6574 2c20 7468 656e 2066 696e 6420   set, then find 
+00001810: 7468 6520 7769 6e6e 6572 7320 666f 7220  the winners for 
+00001820: 7468 6520 7072 6f66 696c 6520 7265 7374  the profile rest
+00001830: 7269 6374 6564 2074 6f20 7468 6520 6361  ricted to the ca
+00001840: 6e64 6964 6174 6573 2069 6e20 6060 6375  ndidates in ``cu
+00001850: 7272 5f63 616e 6473 6060 0a20 2020 2020  rr_cands``.     
+00001860: 2020 2073 7472 656e 6774 685f 6675 6e63     strength_func
+00001870: 7469 6f6e 2028 6675 6e63 7469 6f6e 2c20  tion (function, 
+00001880: 6f70 7469 6f6e 616c 293a 2054 6865 2073  optional): The s
+00001890: 7472 656e 6774 6820 6675 6e63 7469 6f6e  trength function
+000018a0: 2074 6f20 6265 2075 7365 6420 746f 2063   to be used to c
+000018b0: 616c 6375 6c61 7465 2074 6865 2073 7472  alculate the str
+000018c0: 656e 6774 6820 6f66 2061 2070 6174 682e  ength of a path.
+000018d0: 2020 2054 6865 2064 6566 6175 6c74 2069     The default i
+000018e0: 7320 7468 6520 6d61 7267 696e 206d 6574  s the margin met
+000018f0: 686f 6420 6f66 2060 6065 6461 7461 6060  hod of ``edata``
+00001900: 2e20 2020 5468 6973 206f 6e6c 7920 6d61  .   This only ma
+00001910: 7474 6572 7320 7768 656e 2074 6865 2062  tters when the b
+00001920: 616c 6c6f 7473 2061 7265 206e 6f74 206c  allots are not l
+00001930: 696e 6561 7220 6f72 6465 7273 2e20 0a0a  inear orders. ..
+00001940: 2020 2020 5265 7475 726e 733a 200a 2020      Returns: .  
+00001950: 2020 2020 2020 4120 736f 7274 6564 206c        A sorted l
+00001960: 6973 7420 6f66 2063 616e 6469 6461 7465  ist of candidate
+00001970: 732e 200a 0a20 2020 2022 2222 0a20 2020  s. ..    """.   
+00001980: 2063 616e 6469 6461 7465 7320 3d20 6564   candidates = ed
+00001990: 6174 612e 6361 6e64 6964 6174 6573 2069  ata.candidates i
+000019a0: 6620 6375 7272 5f63 616e 6473 2069 7320  f curr_cands is 
+000019b0: 4e6f 6e65 2065 6c73 6520 6375 7272 5f63  None else curr_c
+000019c0: 616e 6473 2020 2020 0a20 2020 2073 7472  ands    .    str
+000019d0: 656e 6774 685f 6675 6e63 7469 6f6e 203d  ength_function =
+000019e0: 2065 6461 7461 2e6d 6172 6769 6e20 6966   edata.margin if
+000019f0: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
+00001a00: 6f6e 2069 7320 4e6f 6e65 2065 6c73 6520  on is None else 
+00001a10: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
+00001a20: 6e0a 2020 2020 0a20 2020 206d 6720 3d20  n.    .    mg = 
+00001a30: 6765 745f 6d67 2865 6461 7461 2c20 6375  get_mg(edata, cu
+00001a40: 7272 5f63 616e 6473 203d 2063 7572 725f  rr_cands = curr_
+00001a50: 6361 6e64 7329 0a20 2020 200a 2020 2020  cands).    .    
+00001a60: 6265 6174 5f70 6174 6873 5f77 6569 6768  beat_paths_weigh
+00001a70: 7473 203d 207b 633a 207b 6332 3a30 2066  ts = {c: {c2:0 f
+00001a80: 6f72 2063 3220 696e 2063 616e 6469 6461  or c2 in candida
+00001a90: 7465 7320 6966 2063 3220 213d 2063 7d20  tes if c2 != c} 
+00001aa0: 666f 7220 6320 696e 2063 616e 6469 6461  for c in candida
+00001ab0: 7465 737d 0a20 2020 2066 6f72 2063 2069  tes}.    for c i
+00001ac0: 6e20 6361 6e64 6964 6174 6573 3a20 0a20  n candidates: . 
+00001ad0: 2020 2020 2020 2066 6f72 206f 7468 6572         for other
+00001ae0: 5f63 2069 6e20 6265 6174 5f70 6174 6873  _c in beat_paths
+00001af0: 5f77 6569 6768 7473 5b63 5d2e 6b65 7973  _weights[c].keys
+00001b00: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+00001b10: 616c 6c5f 7061 7468 7320 3d20 206c 6973  all_paths =  lis
+00001b20: 7428 6e78 2e61 6c6c 5f73 696d 706c 655f  t(nx.all_simple_
+00001b30: 7061 7468 7328 6d67 2c20 632c 206f 7468  paths(mg, c, oth
+00001b40: 6572 5f63 2929 0a20 2020 2020 2020 2020  er_c)).         
+00001b50: 2020 2069 6620 6c65 6e28 616c 6c5f 7061     if len(all_pa
+00001b60: 7468 7329 203e 2030 3a0a 2020 2020 2020  ths) > 0:.      
+00001b70: 2020 2020 2020 2020 2020 6265 6174 5f70            beat_p
+00001b80: 6174 6873 5f77 6569 6768 7473 5b63 5d5b  aths_weights[c][
+00001b90: 6f74 6865 725f 635d 203d 206d 6178 285b  other_c] = max([
+00001ba0: 6d69 6e28 5b73 7472 656e 6774 685f 6675  min([strength_fu
+00001bb0: 6e63 7469 6f6e 2870 5b69 5d2c 2070 5b69  nction(p[i], p[i
+00001bc0: 2b31 5d29 200a 2020 2020 2020 2020 2020  +1]) .          
+00001bd0: 2020 2020 2020 666f 7220 6920 696e 2072        for i in r
+00001be0: 616e 6765 2830 2c6c 656e 2870 292d 3129  ange(0,len(p)-1)
+00001bf0: 5d29 200a 2020 2020 2020 2020 2020 2020  ]) .            
+00001c00: 2020 2020 666f 7220 7020 696e 2061 6c6c      for p in all
+00001c10: 5f70 6174 6873 5d29 0a20 2020 200a 2020  _paths]).    .  
+00001c20: 2020 7769 6e6e 6572 7320 3d20 6c69 7374    winners = list
+00001c30: 2829 0a20 2020 2066 6f72 2063 2069 6e20  ().    for c in 
+00001c40: 6361 6e64 6964 6174 6573 3a20 0a20 2020  candidates: .   
+00001c50: 2020 2020 2069 6620 616c 6c28 5b62 6561       if all([bea
+00001c60: 745f 7061 7468 735f 7765 6967 6874 735b  t_paths_weights[
+00001c70: 635d 5b63 325d 203e 3d20 6265 6174 5f70  c][c2] >= beat_p
+00001c80: 6174 6873 5f77 6569 6768 7473 5b63 325d  aths_weights[c2]
+00001c90: 5b63 5d20 666f 7220 6332 2069 6e20 6361  [c] for c2 in ca
+00001ca0: 6e64 6964 6174 6573 2020 6966 2063 3220  ndidates  if c2 
+00001cb0: 213d 2063 5d29 3a0a 2020 2020 2020 2020  != c]):.        
+00001cc0: 2020 2020 7769 6e6e 6572 732e 6170 7065      winners.appe
+00001cd0: 6e64 2863 290a 2020 2020 7265 7475 726e  nd(c).    return
+00001ce0: 2073 6f72 7465 6428 6c69 7374 2877 696e   sorted(list(win
+00001cf0: 6e65 7273 2929 0a0a 6465 6620 5f62 6561  ners))..def _bea
+00001d00: 745f 7061 7468 5f66 6c6f 7964 5f77 6172  t_path_floyd_war
+00001d10: 7368 616c 6c28 0a20 2020 2020 2020 2065  shall(.        e
+00001d20: 6461 7461 2c20 0a20 2020 2020 2020 2063  data, .        c
+00001d30: 7572 725f 6361 6e64 7320 3d20 4e6f 6e65  urr_cands = None
+00001d40: 2c20 0a20 2020 2020 2020 2073 7472 656e  , .        stren
+00001d50: 6774 685f 6675 6e63 7469 6f6e 203d 204e  gth_function = N
+00001d60: 6f6e 6529 3a20 2020 0a20 2020 2022 2222  one):   .    """
+00001d70: 416e 2069 6d70 6c65 6d65 6e74 6174 696f  An implementatio
+00001d80: 6e20 6f66 2042 6561 7420 5061 7468 2075  n of Beat Path u
+00001d90: 7369 6e67 2061 2076 6172 6961 7469 6f6e  sing a variation
+00001da0: 206f 6620 7468 6520 466c 6f79 642d 5761   of the Floyd-Wa
+00001db0: 7273 6861 6c6c 2041 6c67 6f72 6974 686d  rshall Algorithm
+00001dc0: 0a20 2020 2053 6565 2068 7474 7073 3a2f  .    See https:/
+00001dd0: 2f65 6e2e 7769 6b69 7065 6469 612e 6f72  /en.wikipedia.or
+00001de0: 672f 7769 6b69 2f53 6368 756c 7a65 5f6d  g/wiki/Schulze_m
+00001df0: 6574 686f 6423 496d 706c 656d 656e 7461  ethod#Implementa
+00001e00: 7469 6f6e 290a 200a 2020 2020 4172 6773  tion). .    Args
+00001e10: 3a0a 2020 2020 2020 2020 6564 6174 6120  :.        edata 
+00001e20: 2850 726f 6669 6c65 2c20 5072 6f66 696c  (Profile, Profil
+00001e30: 6557 6974 6854 6965 732c 204d 6172 6769  eWithTies, Margi
+00001e40: 6e47 7261 7068 293a 2041 6e79 2065 6c65  nGraph): Any ele
+00001e50: 6374 696f 6e20 6461 7461 2074 6861 7420  ction data that 
+00001e60: 6861 7320 6120 606d 6172 6769 6e60 206d  has a `margin` m
+00001e70: 6574 686f 642e 200a 2020 2020 2020 2020  ethod. .        
+00001e80: 6375 7272 5f63 616e 6473 2028 4c69 7374  curr_cands (List
+00001e90: 5b69 6e74 5d2c 206f 7074 696f 6e61 6c29  [int], optional)
+00001ea0: 3a20 4966 2073 6574 2c20 7468 656e 2066  : If set, then f
+00001eb0: 696e 6420 7468 6520 7769 6e6e 6572 7320  ind the winners 
+00001ec0: 666f 7220 7468 6520 7072 6f66 696c 6520  for the profile 
+00001ed0: 7265 7374 7269 6374 6564 2074 6f20 7468  restricted to th
+00001ee0: 6520 6361 6e64 6964 6174 6573 2069 6e20  e candidates in 
+00001ef0: 6060 6375 7272 5f63 616e 6473 6060 0a20  ``curr_cands``. 
+00001f00: 2020 2020 2020 2073 7472 656e 6774 685f         strength_
+00001f10: 6675 6e63 7469 6f6e 2028 6675 6e63 7469  function (functi
+00001f20: 6f6e 2c20 6f70 7469 6f6e 616c 293a 2054  on, optional): T
+00001f30: 6865 2073 7472 656e 6774 6820 6675 6e63  he strength func
+00001f40: 7469 6f6e 2074 6f20 6265 2075 7365 6420  tion to be used 
+00001f50: 746f 2063 616c 6375 6c61 7465 2074 6865  to calculate the
+00001f60: 2073 7472 656e 6774 6820 6f66 2061 2070   strength of a p
+00001f70: 6174 682e 2020 2054 6865 2064 6566 6175  ath.   The defau
+00001f80: 6c74 2069 7320 7468 6520 6d61 7267 696e  lt is the margin
+00001f90: 206d 6574 686f 6420 6f66 2060 6065 6461   method of ``eda
+00001fa0: 7461 6060 2e20 2020 5468 6973 206f 6e6c  ta``.   This onl
+00001fb0: 7920 6d61 7474 6572 7320 7768 656e 2074  y matters when t
+00001fc0: 6865 2062 616c 6c6f 7473 2061 7265 206e  he ballots are n
+00001fd0: 6f74 206c 696e 6561 7220 6f72 6465 7273  ot linear orders
+00001fe0: 2e20 0a0a 2020 2020 5265 7475 726e 733a  . ..    Returns:
+00001ff0: 200a 2020 2020 2020 2020 4120 736f 7274   .        A sort
+00002000: 6564 206c 6973 7420 6f66 2063 616e 6469  ed list of candi
+00002010: 6461 7465 732e 200a 0a20 2020 2022 2222  dates. ..    """
+00002020: 0a0a 2020 2020 6361 6e64 6964 6174 6573  ..    candidates
+00002030: 203d 2065 6461 7461 2e63 616e 6469 6461   = edata.candida
+00002040: 7465 7320 6966 2063 7572 725f 6361 6e64  tes if curr_cand
+00002050: 7320 6973 204e 6f6e 6520 656c 7365 2063  s is None else c
+00002060: 7572 725f 6361 6e64 7320 2020 200a 2020  urr_cands    .  
+00002070: 2020 7374 7265 6e67 7468 5f66 756e 6374    strength_funct
+00002080: 696f 6e20 3d20 6564 6174 612e 6d61 7267  ion = edata.marg
+00002090: 696e 2069 6620 7374 7265 6e67 7468 5f66  in if strength_f
+000020a0: 756e 6374 696f 6e20 6973 204e 6f6e 6520  unction is None 
+000020b0: 656c 7365 2073 7472 656e 6774 685f 6675  else strength_fu
+000020c0: 6e63 7469 6f6e 0a20 2020 2020 2020 200a  nction.        .
+000020d0: 2020 2020 735f 6d61 7472 6978 203d 205b      s_matrix = [
+000020e0: 5b2d 6e70 2e69 6e66 2066 6f72 205f 2069  [-np.inf for _ i
+000020f0: 6e20 6361 6e64 6964 6174 6573 5d20 666f  n candidates] fo
+00002100: 7220 5f20 696e 2063 616e 6469 6461 7465  r _ in candidate
+00002110: 735d 0a20 2020 2066 6f72 2063 315f 6964  s].    for c1_id
+00002120: 782c 2063 3120 696e 2065 6e75 6d65 7261  x, c1 in enumera
+00002130: 7465 2863 616e 6469 6461 7465 7329 3a0a  te(candidates):.
+00002140: 2020 2020 2020 2020 666f 7220 6332 5f69          for c2_i
+00002150: 6478 2c20 6332 2069 6e20 656e 756d 6572  dx, c2 in enumer
+00002160: 6174 6528 6361 6e64 6964 6174 6573 293a  ate(candidates):
+00002170: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00002180: 2865 6461 7461 2e6d 616a 6f72 6974 795f  (edata.majority_
+00002190: 7072 6566 6572 7328 6331 2c20 6332 2920  prefers(c1, c2) 
+000021a0: 6f72 2063 3120 3d3d 2063 3229 3a0a 2020  or c1 == c2):.  
+000021b0: 2020 2020 2020 2020 2020 2020 2020 735f                s_
+000021c0: 6d61 7472 6978 5b63 315f 6964 785d 5b63  matrix[c1_idx][c
+000021d0: 325f 6964 785d 203d 2073 7472 656e 6774  2_idx] = strengt
+000021e0: 685f 6675 6e63 7469 6f6e 2863 312c 2063  h_function(c1, c
+000021f0: 3229 200a 2020 2020 7374 7265 6e67 7468  2) .    strength
+00002200: 203d 206c 6973 7428 6d61 7028 6c61 6d62   = list(map(lamb
+00002210: 6461 2069 203a 206c 6973 7428 6d61 7028  da i : list(map(
+00002220: 6c61 6d62 6461 206a 203a 206a 202c 2069  lambda j : j , i
+00002230: 2929 202c 2073 5f6d 6174 7269 7829 290a  )) , s_matrix)).
+00002240: 2020 2020 666f 7220 695f 6964 782c 2069      for i_idx, i
+00002250: 2069 6e20 656e 756d 6572 6174 6528 6361   in enumerate(ca
+00002260: 6e64 6964 6174 6573 293a 2020 2020 2020  ndidates):      
+00002270: 2020 200a 2020 2020 2020 2020 666f 7220     .        for 
+00002280: 6a5f 6964 782c 206a 2069 6e20 656e 756d  j_idx, j in enum
+00002290: 6572 6174 6528 6361 6e64 6964 6174 6573  erate(candidates
+000022a0: 293a 200a 2020 2020 2020 2020 2020 2020  ): .            
+000022b0: 6966 2069 213d 206a 3a0a 2020 2020 2020  if i!= j:.      
+000022c0: 2020 2020 2020 2020 2020 666f 7220 6b5f            for k_
+000022d0: 6964 782c 206b 2069 6e20 656e 756d 6572  idx, k in enumer
+000022e0: 6174 6528 6361 6e64 6964 6174 6573 293a  ate(candidates):
+000022f0: 200a 2020 2020 2020 2020 2020 2020 2020   .              
+00002300: 2020 2020 2020 6966 2069 213d 206b 2061        if i!= k a
+00002310: 6e64 206a 2021 3d20 6b3a 0a20 2020 2020  nd j != k:.     
+00002320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002330: 2020 2073 7472 656e 6774 685b 6a5f 6964     strength[j_id
+00002340: 785d 5b6b 5f69 6478 5d20 3d20 6d61 7828  x][k_idx] = max(
+00002350: 7374 7265 6e67 7468 5b6a 5f69 6478 5d5b  strength[j_idx][
+00002360: 6b5f 6964 785d 2c20 6d69 6e28 7374 7265  k_idx], min(stre
+00002370: 6e67 7468 5b6a 5f69 6478 5d5b 695f 6964  ngth[j_idx][i_id
+00002380: 785d 2c73 7472 656e 6774 685b 695f 6964  x],strength[i_id
+00002390: 785d 5b6b 5f69 6478 5d29 290a 2020 2020  x][k_idx])).    
+000023a0: 7769 6e6e 6572 7320 3d20 7b69 3a54 7275  winners = {i:Tru
+000023b0: 6520 666f 7220 6920 696e 2063 616e 6469  e for i in candi
+000023c0: 6461 7465 737d 0a20 2020 2066 6f72 2069  dates}.    for i
+000023d0: 5f69 6478 2c20 6920 696e 2065 6e75 6d65  _idx, i in enume
+000023e0: 7261 7465 2863 616e 6469 6461 7465 7329  rate(candidates)
+000023f0: 3a20 0a20 2020 2020 2020 2066 6f72 206a  : .        for j
+00002400: 5f69 6478 2c20 6a20 696e 2065 6e75 6d65  _idx, j in enume
+00002410: 7261 7465 2863 616e 6469 6461 7465 7329  rate(candidates)
+00002420: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+00002430: 2069 213d 6a3a 0a20 2020 2020 2020 2020   i!=j:.         
+00002440: 2020 2020 2020 2069 6620 7374 7265 6e67         if streng
+00002450: 7468 5b6a 5f69 6478 5d5b 695f 6964 785d  th[j_idx][i_idx]
+00002460: 203e 2073 7472 656e 6774 685b 695f 6964   > strength[i_id
+00002470: 785d 5b6a 5f69 6478 5d3a 0a20 2020 2020  x][j_idx]:.     
+00002480: 2020 2020 2020 2020 2020 2020 2020 2077                 w
+00002490: 696e 6e65 7273 5b69 5d20 3d20 4661 6c73  inners[i] = Fals
+000024a0: 650a 2020 2020 7265 7475 726e 2073 6f72  e.    return sor
+000024b0: 7465 6428 5b63 2066 6f72 2063 2069 6e20  ted([c for c in 
+000024c0: 6361 6e64 6964 6174 6573 2069 6620 7769  candidates if wi
+000024d0: 6e6e 6572 735b 635d 5d29 0a0a 6465 6620  nners[c]])..def 
+000024e0: 5f73 6368 7761 7274 7a5f 7365 7175 656e  _schwartz_sequen
+000024f0: 7469 616c 5f64 726f 7070 696e 6728 6564  tial_dropping(ed
+00002500: 6174 612c 2063 7572 725f 6361 6e64 7320  ata, curr_cands 
+00002510: 3d20 4e6f 6e65 2c20 7374 7265 6e67 7468  = None, strength
+00002520: 5f66 756e 6374 696f 6e20 3d20 4e6f 6e65  _function = None
+00002530: 293a 0a0a 2020 2020 2222 2254 6865 2053  ):..    """The S
+00002540: 6368 7761 7274 7a20 5365 7175 656e 7469  chwartz Sequenti
+00002550: 616c 2044 726f 7070 696e 6720 616c 676f  al Dropping algo
+00002560: 7269 7468 6d2e 2053 6565 2068 7474 7073  rithm. See https
+00002570: 3a2f 2f65 6e2e 7769 6b69 7065 6469 612e  ://en.wikipedia.
+00002580: 6f72 672f 7769 6b69 2f53 6368 756c 7a65  org/wiki/Schulze
+00002590: 5f6d 6574 686f 6423 5469 6573 5f61 6e64  _method#Ties_and
+000025a0: 5f61 6c74 6572 6e61 7469 7665 5f69 6d70  _alternative_imp
+000025b0: 6c65 6d65 6e74 6174 696f 6e73 2e0a 2020  lementations..  
+000025c0: 2020 0a20 2020 2041 7267 733a 0a20 2020    .    Args:.   
+000025d0: 2020 2020 2065 6461 7461 2028 5072 6f66       edata (Prof
+000025e0: 696c 652c 2050 726f 6669 6c65 5769 7468  ile, ProfileWith
+000025f0: 5469 6573 2c20 4d61 7267 696e 4772 6170  Ties, MarginGrap
+00002600: 6829 3a20 416e 7920 656c 6563 7469 6f6e  h): Any election
+00002610: 2064 6174 6120 7468 6174 2068 6173 2061   data that has a
+00002620: 2060 6d61 7267 696e 6020 6d65 7468 6f64   `margin` method
+00002630: 2e20 0a20 2020 2020 2020 2063 7572 725f  . .        curr_
+00002640: 6361 6e64 7320 284c 6973 745b 696e 745d  cands (List[int]
+00002650: 2c20 6f70 7469 6f6e 616c 293a 2049 6620  , optional): If 
+00002660: 7365 742c 2074 6865 6e20 6669 6e64 2074  set, then find t
+00002670: 6865 2077 696e 6e65 7273 2066 6f72 2074  he winners for t
+00002680: 6865 2070 726f 6669 6c65 2072 6573 7472  he profile restr
+00002690: 6963 7465 6420 746f 2074 6865 2063 616e  icted to the can
+000026a0: 6469 6461 7465 7320 696e 2060 6063 7572  didates in ``cur
+000026b0: 725f 6361 6e64 7360 600a 2020 2020 2020  r_cands``.      
+000026c0: 2020 7374 7265 6e67 7468 5f66 756e 6374    strength_funct
+000026d0: 696f 6e20 2866 756e 6374 696f 6e2c 206f  ion (function, o
+000026e0: 7074 696f 6e61 6c29 3a20 5468 6520 7374  ptional): The st
+000026f0: 7265 6e67 7468 2066 756e 6374 696f 6e20  rength function 
+00002700: 746f 2062 6520 7573 6564 2074 6f20 6361  to be used to ca
+00002710: 6c63 756c 6174 6520 7468 6520 7374 7265  lculate the stre
+00002720: 6e67 7468 206f 6620 6120 7061 7468 2e20  ngth of a path. 
+00002730: 2020 5468 6520 6465 6661 756c 7420 6973    The default is
+00002740: 2074 6865 206d 6172 6769 6e20 6d65 7468   the margin meth
+00002750: 6f64 206f 6620 6060 6564 6174 6160 602e  od of ``edata``.
+00002760: 2020 2054 6869 7320 6f6e 6c79 206d 6174     This only mat
+00002770: 7465 7273 2077 6865 6e20 7468 6520 6261  ters when the ba
+00002780: 6c6c 6f74 7320 6172 6520 6e6f 7420 6c69  llots are not li
+00002790: 6e65 6172 206f 7264 6572 732e 200a 0a20  near orders. .. 
+000027a0: 2020 2052 6574 7572 6e73 3a20 0a20 2020     Returns: .   
+000027b0: 2020 2020 2041 2073 6f72 7465 6420 6c69       A sorted li
+000027c0: 7374 206f 6620 6361 6e64 6964 6174 6573  st of candidates
+000027d0: 2e20 0a20 2020 2022 2222 0a20 2020 2066  . .    """.    f
+000027e0: 726f 6d20 7072 6566 5f76 6f74 696e 672e  rom pref_voting.
+000027f0: 6331 5f6d 6574 686f 6473 2069 6d70 6f72  c1_methods impor
+00002800: 7420 676f 6368 610a 0a20 2020 2073 7472  t gocha..    str
+00002810: 656e 6774 685f 6675 6e63 7469 6f6e 203d  ength_function =
+00002820: 2065 6461 7461 2e6d 6172 6769 6e20 6966   edata.margin if
+00002830: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
+00002840: 6f6e 2069 7320 4e6f 6e65 2065 6c73 6520  on is None else 
+00002850: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
+00002860: 6e0a 0a20 2020 206d 6720 3d20 6564 6174  n..    mg = edat
+00002870: 6120 6966 2069 7369 6e73 7461 6e63 6528  a if isinstance(
+00002880: 6564 6174 612c 204d 6172 6769 6e47 7261  edata, MarginGra
+00002890: 7068 2920 656c 7365 2065 6461 7461 2e6d  ph) else edata.m
+000028a0: 6172 6769 6e5f 6772 6170 6828 290a 2020  argin_graph().  
+000028b0: 2020 7363 6877 6172 747a 203d 2067 6f63    schwartz = goc
+000028c0: 6861 286d 672c 2063 7572 725f 6361 6e64  ha(mg, curr_cand
+000028d0: 7320 3d20 6375 7272 5f63 616e 6473 290a  s = curr_cands).
+000028e0: 0a20 2020 2069 6620 6c65 6e28 7363 6877  .    if len(schw
+000028f0: 6172 747a 2920 3d3d 2031 3a0a 2020 2020  artz) == 1:.    
+00002900: 2020 2020 7265 7475 726e 2073 6368 7761      return schwa
+00002910: 7274 7a0a 2020 2020 0a20 2020 2070 6f73  rtz.    .    pos
+00002920: 5f73 6368 7761 7274 7a5f 7374 7265 6e67  _schwartz_streng
+00002930: 7468 7320 3d20 5b73 7472 656e 6774 685f  ths = [strength_
+00002940: 6675 6e63 7469 6f6e 2863 2c64 2920 666f  function(c,d) fo
+00002950: 7220 6320 696e 2073 6368 7761 7274 7a20  r c in schwartz 
+00002960: 666f 7220 6420 696e 2073 6368 7761 7274  for d in schwart
+00002970: 7a20 6966 2073 7472 656e 6774 685f 6675  z if strength_fu
+00002980: 6e63 7469 6f6e 2863 2c64 2920 3e20 305d  nction(c,d) > 0]
+00002990: 0a0a 2020 2020 6966 206c 656e 2870 6f73  ..    if len(pos
+000029a0: 5f73 6368 7761 7274 7a5f 7374 7265 6e67  _schwartz_streng
+000029b0: 7468 7329 203d 3d20 303a 0a20 2020 2020  ths) == 0:.     
+000029c0: 2020 2072 6574 7572 6e20 736f 7274 6564     return sorted
+000029d0: 2873 6368 7761 7274 7a29 0a0a 2020 2020  (schwartz)..    
+000029e0: 6d61 785f 7363 6877 6172 747a 5f73 7472  max_schwartz_str
+000029f0: 656e 6774 6820 3d20 6d61 7828 706f 735f  ength = max(pos_
+00002a00: 7363 6877 6172 747a 5f73 7472 656e 6774  schwartz_strengt
+00002a10: 6873 290a 2020 2020 6d69 6e5f 7363 6877  hs).    min_schw
+00002a20: 6172 747a 5f73 7472 656e 6774 6820 3d20  artz_strength = 
+00002a30: 6d69 6e28 706f 735f 7363 6877 6172 747a  min(pos_schwartz
+00002a40: 5f73 7472 656e 6774 6873 290a 0a20 2020  _strengths)..   
+00002a50: 2069 6620 6d61 785f 7363 6877 6172 747a   if max_schwartz
+00002a60: 5f73 7472 656e 6774 6820 3d3d 206d 696e  _strength == min
+00002a70: 5f73 6368 7761 7274 7a5f 7374 7265 6e67  _schwartz_streng
+00002a80: 7468 3a0a 2020 2020 2020 2020 7265 7475  th:.        retu
+00002a90: 726e 2073 6f72 7465 6428 7363 6877 6172  rn sorted(schwar
+00002aa0: 747a 290a 2020 2020 0a20 2020 2065 6c73  tz).    .    els
+00002ab0: 653a 0a20 2020 2020 2020 206e 6577 5f6d  e:.        new_m
+00002ac0: 6720 3d20 4d61 7267 696e 4772 6170 6828  g = MarginGraph(
+00002ad0: 7363 6877 6172 747a 2c5b 2863 2c64 2c20  schwartz,[(c,d, 
+00002ae0: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
+00002af0: 6e28 632c 6429 2920 666f 7220 6320 696e  n(c,d)) for c in
+00002b00: 2073 6368 7761 7274 7a20 666f 7220 6420   schwartz for d 
+00002b10: 696e 2073 6368 7761 7274 7a20 6966 2073  in schwartz if s
+00002b20: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
+00002b30: 2863 2c64 2920 3e20 6d69 6e5f 7363 6877  (c,d) > min_schw
+00002b40: 6172 747a 5f73 7472 656e 6774 685d 290a  artz_strength]).
+00002b50: 2020 2020 2020 2020 7265 7475 726e 205f          return _
+00002b60: 7363 6877 6172 747a 5f73 6571 7565 6e74  schwartz_sequent
+00002b70: 6961 6c5f 6472 6f70 7069 6e67 286e 6577  ial_dropping(new
+00002b80: 5f6d 672c 2073 6368 7761 7274 7a29 0a0a  _mg, schwartz)..
+00002b90: 6270 5f70 726f 7065 7274 6965 7320 3d20  bp_properties = 
+00002ba0: 566f 7469 6e67 4d65 7468 6f64 5072 6f70  VotingMethodProp
+00002bb0: 6572 7469 6573 280a 2020 2020 636f 6e64  erties(.    cond
+00002bc0: 6f72 6365 745f 7769 6e6e 6572 3d54 7275  orcet_winner=Tru
+00002bd0: 652c 200a 2020 2020 636f 6e64 6f72 6365  e, .    condorce
+00002be0: 745f 6c6f 7365 723d 5472 7565 2c0a 2020  t_loser=True,.  
+00002bf0: 2020 7061 7265 746f 5f64 6f6d 696e 616e    pareto_dominan
+00002c00: 6365 3d54 7275 652c 0a20 2020 2070 6f73  ce=True,.    pos
+00002c10: 6974 6976 655f 696e 766f 6c76 656d 656e  itive_involvemen
+00002c20: 743d 4661 6c73 652c 200a 2020 2020 290a  t=False, .    ).
+00002c30: 0a40 766d 286e 616d 653d 2242 6561 7420  .@vm(name="Beat 
+00002c40: 5061 7468 222c 0a20 2020 2070 726f 7065  Path",.    prope
+00002c50: 7274 6965 733d 6270 5f70 726f 7065 7274  rties=bp_propert
+00002c60: 6965 732c 0a20 2020 2069 6e70 7574 5f74  ies,.    input_t
+00002c70: 7970 6573 3d5b 456c 6563 7469 6f6e 5479  ypes=[ElectionTy
+00002c80: 7065 732e 5052 4f46 494c 452c 2045 6c65  pes.PROFILE, Ele
+00002c90: 6374 696f 6e54 7970 6573 2e50 524f 4649  ctionTypes.PROFI
+00002ca0: 4c45 5f57 4954 485f 5449 4553 2c20 456c  LE_WITH_TIES, El
+00002cb0: 6563 7469 6f6e 5479 7065 732e 4d41 5247  ectionTypes.MARG
+00002cc0: 494e 5f47 5241 5048 5d29 0a64 6566 2062  IN_GRAPH]).def b
+00002cd0: 6561 745f 7061 7468 280a 2020 2020 6564  eat_path(.    ed
+00002ce0: 6174 612c 200a 2020 2020 6375 7272 5f63  ata, .    curr_c
+00002cf0: 616e 6473 203d 204e 6f6e 652c 200a 2020  ands = None, .  
+00002d00: 2020 7374 7265 6e67 7468 5f66 756e 6374    strength_funct
+00002d10: 696f 6e20 3d20 4e6f 6e65 2c20 0a20 2020  ion = None, .   
+00002d20: 2061 6c67 6f72 6974 686d 203d 2027 666c   algorithm = 'fl
+00002d30: 6f79 645f 7761 7273 6861 6c6c 2729 3a20  oyd_warshall'): 
+00002d40: 200a 0a20 2020 2022 2222 466f 7220 6361   ..    """For ca
+00002d50: 6e64 6964 6174 6573 203a 6d61 7468 3a60  ndidates :math:`
+00002d60: 6160 2061 6e64 203a 6d61 7468 3a60 6260  a` and :math:`b`
+00002d70: 2c20 6120 2a2a 7061 7468 2a2a 2066 726f  , a **path** fro
+00002d80: 6d20 3a6d 6174 683a 6061 6020 746f 203a  m :math:`a` to :
+00002d90: 6d61 7468 3a60 6260 2069 7320 6120 7365  math:`b` is a se
+00002da0: 7175 656e 6365 200a 2020 2020 3a6d 6174  quence .    :mat
+00002db0: 683a 6078 5f31 2c20 5c6c 646f 7473 2c20  h:`x_1, \ldots, 
+00002dc0: 785f 6e60 206f 6620 6469 7374 696e 6374  x_n` of distinct
+00002dd0: 2063 616e 6469 6461 7465 7320 2077 6974   candidates  wit
+00002de0: 6820 203a 6d61 7468 3a60 785f 313d 6160  h  :math:`x_1=a`
+00002df0: 2061 6e64 203a 6d61 7468 3a60 785f 6e3d   and :math:`x_n=
+00002e00: 6260 2073 7563 6820 7468 6174 200a 2020  b` such that .  
+00002e10: 2020 666f 7220 3a6d 6174 683a 6031 5c6c    for :math:`1\l
+00002e20: 6571 206b 5c6c 6571 206e 2d31 602c 203a  eq k\leq n-1`, :
+00002e30: 6d61 7468 3a60 785f 6b60 2069 7320 6d61  math:`x_k` is ma
+00002e40: 6a6f 7269 7479 2070 7265 6665 7272 6564  jority preferred
+00002e50: 2074 6f20 3a6d 6174 683a 6078 5f7b 6b2b   to :math:`x_{k+
+00002e60: 317d 602e 2020 5468 6520 2a2a 7374 7265  1}`.  The **stre
+00002e70: 6e67 7468 206f 6620 6120 7061 7468 2a2a  ngth of a path**
+00002e80: 0a20 2020 2069 7320 7468 6520 6d69 6e69  .    is the mini
+00002e90: 6d61 6c20 6d61 7267 696e 2061 6c6f 6e67  mal margin along
+00002ea0: 2074 6861 7420 7061 7468 2e20 2053 6179   that path.  Say
+00002eb0: 2074 6861 7420 3a6d 6174 683a 6061 6020   that :math:`a` 
+00002ec0: 6465 6665 6174 7320 3a6d 6174 683a 6062  defeats :math:`b
+00002ed0: 6020 6163 636f 7264 696e 6720 746f 2042  ` according to B
+00002ee0: 6561 7420 5061 7468 2069 6620 7468 6520  eat Path if the 
+00002ef0: 7468 6520 7374 7265 6e67 7468 206f 6620  the strength of 
+00002f00: 7468 6520 7374 726f 6e67 6573 7420 7061  the strongest pa
+00002f10: 7468 2066 726f 6d20 3a6d 6174 683a 6061  th from :math:`a
+00002f20: 6020 746f 203a 6d61 7468 3a60 6260 2069  ` to :math:`b` i
+00002f30: 7320 6772 6561 7465 7220 7468 616e 2074  s greater than t
+00002f40: 6865 2073 7472 656e 6774 6820 6f66 2074  he strength of t
+00002f50: 6865 2073 7472 6f6e 6765 7374 2070 6174  he strongest pat
+00002f60: 6820 6672 6f6d 203a 6d61 7468 3a60 6260  h from :math:`b`
+00002f70: 2074 6f20 3a6d 6174 683a 6061 602e 2054   to :math:`a`. T
+00002f80: 6865 6e20 7468 6520 6361 6e64 6964 6174  hen the candidat
+00002f90: 6573 2074 6861 7420 6172 6520 756e 6465  es that are unde
+00002fa0: 6665 6174 6564 2061 6363 6f72 6469 6e67  feated according
+00002fb0: 2074 6f20 4265 6174 2050 6174 6820 6172   to Beat Path ar
+00002fc0: 6520 7468 6520 7769 6e6e 6572 732e 2020  e the winners.  
+00002fd0: 416c 736f 206b 6e6f 776e 2061 7320 7468  Also known as th
+00002fe0: 6520 5363 6875 6c7a 6520 5275 6c65 2e20  e Schulze Rule. 
+00002ff0: 0a0a 2020 2020 4172 6773 3a0a 2020 2020  ..    Args:.    
+00003000: 2020 2020 6564 6174 6120 2850 726f 6669      edata (Profi
+00003010: 6c65 2c20 5072 6f66 696c 6557 6974 6854  le, ProfileWithT
+00003020: 6965 732c 204d 6172 6769 6e47 7261 7068  ies, MarginGraph
+00003030: 293a 2041 6e79 2065 6c65 6374 696f 6e20  ): Any election 
+00003040: 6461 7461 2074 6861 7420 6861 7320 6120  data that has a 
+00003050: 606d 6172 6769 6e60 206d 6574 686f 642e  `margin` method.
+00003060: 200a 2020 2020 2020 2020 6375 7272 5f63   .        curr_c
+00003070: 616e 6473 2028 4c69 7374 5b69 6e74 5d2c  ands (List[int],
+00003080: 206f 7074 696f 6e61 6c29 3a20 4966 2073   optional): If s
+00003090: 6574 2c20 7468 656e 2066 696e 6420 7468  et, then find th
+000030a0: 6520 7769 6e6e 6572 7320 666f 7220 7468  e winners for th
+000030b0: 6520 7072 6f66 696c 6520 7265 7374 7269  e profile restri
+000030c0: 6374 6564 2074 6f20 7468 6520 6361 6e64  cted to the cand
+000030d0: 6964 6174 6573 2069 6e20 6060 6375 7272  idates in ``curr
+000030e0: 5f63 616e 6473 6060 0a20 2020 2020 2020  _cands``.       
+000030f0: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
+00003100: 6f6e 2028 6675 6e63 7469 6f6e 2c20 6f70  on (function, op
+00003110: 7469 6f6e 616c 293a 2054 6865 2073 7472  tional): The str
+00003120: 656e 6774 6820 6675 6e63 7469 6f6e 2074  ength function t
+00003130: 6f20 6265 2075 7365 6420 746f 2063 616c  o be used to cal
+00003140: 6375 6c61 7465 2074 6865 2073 7472 656e  culate the stren
+00003150: 6774 6820 6f66 2061 2070 6174 682e 2020  gth of a path.  
+00003160: 2054 6865 2064 6566 6175 6c74 2069 7320   The default is 
+00003170: 7468 6520 6d61 7267 696e 206d 6574 686f  the margin metho
+00003180: 6420 6f66 2060 6065 6461 7461 6060 2e20  d of ``edata``. 
+00003190: 2020 5468 6973 206f 6e6c 7920 6d61 7474    This only matt
+000031a0: 6572 7320 7768 656e 2074 6865 2062 616c  ers when the bal
+000031b0: 6c6f 7473 2061 7265 206e 6f74 206c 696e  lots are not lin
+000031c0: 6561 7220 6f72 6465 7273 2e20 0a20 2020  ear orders. .   
+000031d0: 2020 2020 2061 6c67 6f72 6974 686d 2028       algorithm (
+000031e0: 7374 7229 3a20 5370 6563 6966 7920 7768  str): Specify wh
+000031f0: 6963 6820 616c 676f 7269 7468 6d20 746f  ich algorithm to
+00003200: 2075 7365 2e20 204f 7074 696f 6e73 2061   use.  Options a
+00003210: 7265 2027 666c 6f79 645f 7761 7273 6861  re 'floyd_warsha
+00003220: 6c6c 2720 2874 6865 2064 6566 6175 6c74  ll' (the default
+00003230: 292c 2027 6261 7369 6327 2c20 616e 6420  ), 'basic', and 
+00003240: 2773 6368 7761 7274 7a5f 7365 7175 656e  'schwartz_sequen
+00003250: 7469 616c 5f64 726f 7070 696e 6727 2e0a  tial_dropping'..
+00003260: 0a20 2020 2052 6574 7572 6e73 3a20 0a20  .    Returns: . 
+00003270: 2020 2020 2020 2041 2073 6f72 7465 6420         A sorted 
+00003280: 6c69 7374 206f 6620 6361 6e64 6964 6174  list of candidat
+00003290: 6573 2e20 0a0a 2020 2020 2e2e 2073 6565  es. ..    .. see
+000032a0: 616c 736f 3a3a 0a0a 2020 2020 2020 2020  also::..        
+000032b0: 3a6d 6574 683a 6070 7265 665f 766f 7469  :meth:`pref_voti
+000032c0: 6e67 2e6d 6172 6769 6e5f 6261 7365 645f  ng.margin_based_
+000032d0: 6d65 7468 6f64 732e 6265 6174 5f70 6174  methods.beat_pat
+000032e0: 685f 6465 6665 6174 600a 0a20 2020 203a  h_defeat`..    :
+000032f0: 4578 616d 706c 653a 200a 0a20 2020 202e  Example: ..    .
+00003300: 2e20 706c 6f74 3a3a 2020 6d61 7267 696e  . plot::  margin
+00003310: 5f67 7261 7068 735f 6578 616d 706c 6573  _graphs_examples
+00003320: 2f6d 675f 6578 5f62 705f 7270 2e70 790a  /mg_ex_bp_rp.py.
+00003330: 2020 2020 2020 2020 3a63 6f6e 7465 7874          :context
+00003340: 3a20 7265 7365 7420 200a 2020 2020 2020  : reset  .      
+00003350: 2020 3a69 6e63 6c75 6465 2d73 6f75 7263    :include-sourc
+00003360: 653a 2054 7275 650a 0a0a 2020 2020 2e2e  e: True...    ..
+00003370: 2063 6f64 652d 626c 6f63 6b3a 3a20 0a0a   code-block:: ..
+00003380: 2020 2020 2020 2020 6672 6f6d 2070 7265          from pre
+00003390: 665f 766f 7469 6e67 2e6d 6172 6769 6e5f  f_voting.margin_
+000033a0: 6261 7365 645f 6d65 7468 6f64 7320 696d  based_methods im
+000033b0: 706f 7274 2062 6561 745f 7061 7468 0a0a  port beat_path..
+000033c0: 2020 2020 2020 2020 6265 6174 5f70 6174          beat_pat
+000033d0: 682e 6469 7370 6c61 7928 6d67 290a 0a0a  h.display(mg)...
+000033e0: 2020 2020 2e2e 2065 7865 635f 636f 6465      .. exec_code
+000033f0: 3a3a 200a 2020 2020 2020 2020 3a68 6964  :: .        :hid
+00003400: 655f 636f 6465 3a0a 0a20 2020 2020 2020  e_code:..       
+00003410: 2066 726f 6d20 7072 6566 5f76 6f74 696e   from pref_votin
+00003420: 672e 7765 6967 6874 6564 5f6d 616a 6f72  g.weighted_major
+00003430: 6974 795f 6772 6170 6873 2069 6d70 6f72  ity_graphs impor
+00003440: 7420 4d61 7267 696e 4772 6170 680a 2020  t MarginGraph.  
+00003450: 2020 2020 2020 6672 6f6d 2070 7265 665f        from pref_
+00003460: 766f 7469 6e67 2e6d 6172 6769 6e5f 6261  voting.margin_ba
+00003470: 7365 645f 6d65 7468 6f64 7320 696d 706f  sed_methods impo
+00003480: 7274 2062 6561 745f 7061 7468 0a20 2020  rt beat_path.   
+00003490: 2020 2020 200a 2020 2020 2020 2020 6d67       .        mg
+000034a0: 203d 204d 6172 6769 6e47 7261 7068 285b   = MarginGraph([
+000034b0: 302c 2031 2c20 322c 2033 5d2c 205b 2830  0, 1, 2, 3], [(0
+000034c0: 2c20 322c 2033 292c 2028 312c 2030 2c20  , 2, 3), (1, 0, 
+000034d0: 3529 2c20 2832 2c20 312c 2035 292c 2028  5), (2, 1, 5), (
+000034e0: 322c 2033 2c20 3129 2c20 2833 2c20 302c  2, 3, 1), (3, 0,
+000034f0: 2033 292c 2028 332c 2031 2c20 3129 5d29   3), (3, 1, 1)])
+00003500: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00003510: 2020 6265 6174 5f70 6174 682e 6469 7370    beat_path.disp
+00003520: 6c61 7928 6d67 290a 2020 2020 2020 2020  lay(mg).        
+00003530: 6265 6174 5f70 6174 682e 6469 7370 6c61  beat_path.displa
+00003540: 7928 6d67 2c20 616c 676f 7269 7468 6d3d  y(mg, algorithm=
+00003550: 2766 6c6f 7964 5f77 6172 7368 616c 6c27  'floyd_warshall'
+00003560: 2920 0a20 2020 2020 2020 2062 6561 745f  ) .        beat_
+00003570: 7061 7468 2e64 6973 706c 6179 286d 672c  path.display(mg,
+00003580: 2061 6c67 6f72 6974 686d 3d27 6261 7369   algorithm='basi
+00003590: 6327 290a 2020 2020 2222 220a 0a20 2020  c').    """..   
+000035a0: 2069 6620 616c 676f 7269 7468 6d20 3d3d   if algorithm ==
+000035b0: 2027 666c 6f79 645f 7761 7273 6861 6c6c   'floyd_warshall
+000035c0: 273a 0a20 2020 2020 2020 2072 6574 7572  ':.        retur
+000035d0: 6e20 5f62 6561 745f 7061 7468 5f66 6c6f  n _beat_path_flo
+000035e0: 7964 5f77 6172 7368 616c 6c28 6564 6174  yd_warshall(edat
+000035f0: 612c 2063 7572 725f 6361 6e64 7320 3d20  a, curr_cands = 
+00003600: 6375 7272 5f63 616e 6473 2c20 7374 7265  curr_cands, stre
+00003610: 6e67 7468 5f66 756e 6374 696f 6e20 3d20  ngth_function = 
+00003620: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
+00003630: 6e29 0a20 2020 2065 6c69 6620 616c 676f  n).    elif algo
+00003640: 7269 7468 6d20 3d3d 2027 6261 7369 6327  rithm == 'basic'
+00003650: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+00003660: 205f 6265 6174 5f70 6174 685f 6261 7369   _beat_path_basi
+00003670: 6328 6564 6174 612c 2063 7572 725f 6361  c(edata, curr_ca
+00003680: 6e64 7320 3d20 6375 7272 5f63 616e 6473  nds = curr_cands
+00003690: 2c20 7374 7265 6e67 7468 5f66 756e 6374  , strength_funct
+000036a0: 696f 6e20 3d20 7374 7265 6e67 7468 5f66  ion = strength_f
+000036b0: 756e 6374 696f 6e29 0a20 2020 2065 6c69  unction).    eli
+000036c0: 6620 616c 676f 7269 7468 6d20 3d3d 2027  f algorithm == '
+000036d0: 7363 6877 6172 747a 5f73 6571 7565 6e74  schwartz_sequent
+000036e0: 6961 6c5f 6472 6f70 7069 6e67 273a 0a20  ial_dropping':. 
+000036f0: 2020 2020 2020 2072 6574 7572 6e20 5f73         return _s
+00003700: 6368 7761 7274 7a5f 7365 7175 656e 7469  chwartz_sequenti
+00003710: 616c 5f64 726f 7070 696e 6728 6564 6174  al_dropping(edat
+00003720: 612c 2063 7572 725f 6361 6e64 7320 3d20  a, curr_cands = 
+00003730: 6375 7272 5f63 616e 6473 2c20 7374 7265  curr_cands, stre
+00003740: 6e67 7468 5f66 756e 6374 696f 6e20 3d20  ngth_function = 
+00003750: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
+00003760: 6e29 0a20 2020 2065 6c73 653a 0a20 2020  n).    else:.   
+00003770: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
+00003780: 4572 726f 7228 2249 6e76 616c 6964 2061  Error("Invalid a
+00003790: 6c67 6f72 6974 686d 2073 7065 6369 6669  lgorithm specifi
+000037a0: 6564 2e22 290a 0a64 6566 2062 6561 745f  ed.")..def beat_
+000037b0: 7061 7468 5f64 6566 6561 7428 6564 6174  path_defeat(edat
+000037c0: 612c 2063 7572 725f 6361 6e64 7320 3d20  a, curr_cands = 
+000037d0: 4e6f 6e65 2c20 7374 7265 6e67 7468 5f66  None, strength_f
+000037e0: 756e 6374 696f 6e20 3d20 4e6f 6e65 293a  unction = None):
+000037f0: 2020 200a 2020 2020 2222 2252 6574 7572     .    """Retur
+00003800: 6e73 2074 6865 2064 6566 6561 7420 7265  ns the defeat re
+00003810: 6c61 7469 6f6e 2066 6f72 2042 6561 7420  lation for Beat 
+00003820: 5061 7468 2e20 0a20 2020 200a 2020 2020  Path. .    .    
+00003830: 4172 6773 3a0a 2020 2020 2020 2020 6564  Args:.        ed
+00003840: 6174 6120 2850 726f 6669 6c65 2c20 5072  ata (Profile, Pr
+00003850: 6f66 696c 6557 6974 6854 6965 732c 204d  ofileWithTies, M
+00003860: 6172 6769 6e47 7261 7068 293a 2041 6e79  arginGraph): Any
+00003870: 2065 6c65 6374 696f 6e20 6461 7461 2074   election data t
+00003880: 6861 7420 6861 7320 6120 606d 6172 6769  hat has a `margi
+00003890: 6e60 206d 6574 686f 642e 200a 2020 2020  n` method. .    
+000038a0: 2020 2020 6375 7272 5f63 616e 6473 2028      curr_cands (
+000038b0: 4c69 7374 5b69 6e74 5d2c 206f 7074 696f  List[int], optio
+000038c0: 6e61 6c29 3a20 4966 2073 6574 2c20 7468  nal): If set, th
+000038d0: 656e 2066 696e 6420 7468 6520 7769 6e6e  en find the winn
+000038e0: 6572 7320 666f 7220 7468 6520 7072 6f66  ers for the prof
+000038f0: 696c 6520 7265 7374 7269 6374 6564 2074  ile restricted t
+00003900: 6f20 7468 6520 6361 6e64 6964 6174 6573  o the candidates
+00003910: 2069 6e20 6060 6375 7272 5f63 616e 6473   in ``curr_cands
+00003920: 6060 0a20 2020 2020 2020 2073 7472 656e  ``.        stren
+00003930: 6774 685f 6675 6e63 7469 6f6e 2028 6675  gth_function (fu
+00003940: 6e63 7469 6f6e 2c20 6f70 7469 6f6e 616c  nction, optional
+00003950: 293a 2054 6865 2073 7472 656e 6774 6820  ): The strength 
+00003960: 6675 6e63 7469 6f6e 2074 6f20 6265 2075  function to be u
+00003970: 7365 6420 746f 2063 616c 6375 6c61 7465  sed to calculate
+00003980: 2074 6865 2073 7472 656e 6774 6820 6f66   the strength of
+00003990: 2061 2070 6174 682e 2020 2054 6865 2064   a path.   The d
+000039a0: 6566 6175 6c74 2069 7320 7468 6520 6d61  efault is the ma
+000039b0: 7267 696e 206d 6574 686f 6420 6f66 2060  rgin method of `
+000039c0: 6065 6461 7461 6060 2e20 2020 5468 6973  `edata``.   This
+000039d0: 206f 6e6c 7920 6d61 7474 6572 7320 7768   only matters wh
+000039e0: 656e 2074 6865 2062 616c 6c6f 7473 2061  en the ballots a
+000039f0: 7265 206e 6f74 206c 696e 6561 7220 6f72  re not linear or
+00003a00: 6465 7273 2e20 0a0a 2020 2020 5265 7475  ders. ..    Retu
+00003a10: 726e 733a 200a 2020 2020 2020 2020 4120  rns: .        A 
+00003a20: 6e65 7477 6f72 6b78 2044 6947 7261 7068  networkx DiGraph
+00003a30: 2072 6570 7265 7365 6e74 696e 6720 7468   representing th
+00003a40: 6520 4265 6174 2050 6174 6820 6465 6665  e Beat Path defe
+00003a50: 6174 2072 656c 6174 696f 6e2e 200a 0a20  at relation. .. 
+00003a60: 2020 202e 2e20 7365 6561 6c73 6f3a 3a0a     .. seealso::.
+00003a70: 0a20 2020 2020 2020 203a 6d65 7468 3a60  .        :meth:`
+00003a80: 7072 6566 5f76 6f74 696e 672e 6d61 7267  pref_voting.marg
+00003a90: 696e 5f62 6173 6564 5f6d 6574 686f 6473  in_based_methods
+00003aa0: 2e62 6561 745f 7061 7468 602c 203a 6d65  .beat_path`, :me
+00003ab0: 7468 3a60 7072 6566 5f76 6f74 696e 672e  th:`pref_voting.
+00003ac0: 6d61 7267 696e 5f62 6173 6564 5f6d 6574  margin_based_met
+00003ad0: 686f 6473 2e62 6561 745f 7061 7468 5f46  hods.beat_path_F
+00003ae0: 6c6f 7964 5f57 6172 7368 616c 6c60 0a0a  loyd_Warshall`..
+00003af0: 2020 2020 3a45 7861 6d70 6c65 3a20 0a0a      :Example: ..
+00003b00: 2020 2020 2e2e 2070 6c6f 743a 3a20 206d      .. plot::  m
+00003b10: 6172 6769 6e5f 6772 6170 6873 5f65 7861  argin_graphs_exa
+00003b20: 6d70 6c65 732f 6d67 5f65 785f 6270 5f64  mples/mg_ex_bp_d
+00003b30: 6566 6561 742e 7079 0a20 2020 2020 2020  efeat.py.       
+00003b40: 203a 636f 6e74 6578 743a 2072 6573 6574   :context: reset
+00003b50: 2020 0a20 2020 2020 2020 203a 696e 636c    .        :incl
+00003b60: 7564 652d 736f 7572 6365 3a20 5472 7565  ude-source: True
+00003b70: 0a0a 2020 2020 2222 220a 0a20 2020 2063  ..    """..    c
+00003b80: 616e 6469 6461 7465 7320 3d20 6564 6174  andidates = edat
+00003b90: 612e 6361 6e64 6964 6174 6573 2069 6620  a.candidates if 
+00003ba0: 6375 7272 5f63 616e 6473 2069 7320 4e6f  curr_cands is No
+00003bb0: 6e65 2065 6c73 6520 6375 7272 5f63 616e  ne else curr_can
+00003bc0: 6473 2020 2020 0a20 2020 2073 7472 656e  ds    .    stren
+00003bd0: 6774 685f 6675 6e63 7469 6f6e 203d 2065  gth_function = e
+00003be0: 6461 7461 2e6d 6172 6769 6e20 6966 2073  data.margin if s
+00003bf0: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
+00003c00: 2069 7320 4e6f 6e65 2065 6c73 6520 7374   is None else st
+00003c10: 7265 6e67 7468 5f66 756e 6374 696f 6e0a  rength_function.
+00003c20: 2020 2020 2020 2020 0a20 2020 2073 5f6d          .    s_m
+00003c30: 6174 7269 7820 3d20 5b5b 2d6e 702e 696e  atrix = [[-np.in
+00003c40: 6620 666f 7220 5f20 696e 2063 616e 6469  f for _ in candi
+00003c50: 6461 7465 735d 2066 6f72 205f 2069 6e20  dates] for _ in 
+00003c60: 6361 6e64 6964 6174 6573 5d0a 2020 2020  candidates].    
+00003c70: 666f 7220 6331 5f69 6478 2c20 6331 2069  for c1_idx, c1 i
+00003c80: 6e20 656e 756d 6572 6174 6528 6361 6e64  n enumerate(cand
+00003c90: 6964 6174 6573 293a 0a20 2020 2020 2020  idates):.       
+00003ca0: 2066 6f72 2063 325f 6964 782c 2063 3220   for c2_idx, c2 
+00003cb0: 696e 2065 6e75 6d65 7261 7465 2863 616e  in enumerate(can
+00003cc0: 6469 6461 7465 7329 3a0a 2020 2020 2020  didates):.      
+00003cd0: 2020 2020 2020 6966 2028 6564 6174 612e        if (edata.
+00003ce0: 6d61 6a6f 7269 7479 5f70 7265 6665 7273  majority_prefers
+00003cf0: 2863 312c 2063 3229 206f 7220 6331 203d  (c1, c2) or c1 =
+00003d00: 3d20 6332 293a 0a20 2020 2020 2020 2020  = c2):.         
+00003d10: 2020 2020 2020 2073 5f6d 6174 7269 785b         s_matrix[
+00003d20: 6331 5f69 6478 5d5b 6332 5f69 6478 5d20  c1_idx][c2_idx] 
+00003d30: 3d20 7374 7265 6e67 7468 5f66 756e 6374  = strength_funct
+00003d40: 696f 6e28 6331 2c20 6332 2920 0a20 2020  ion(c1, c2) .   
+00003d50: 2073 7472 656e 6774 6820 3d20 6c69 7374   strength = list
+00003d60: 286d 6170 286c 616d 6264 6120 6920 3a20  (map(lambda i : 
+00003d70: 6c69 7374 286d 6170 286c 616d 6264 6120  list(map(lambda 
+00003d80: 6a20 3a20 6a20 2c20 6929 2920 2c20 735f  j : j , i)) , s_
+00003d90: 6d61 7472 6978 2929 0a20 2020 2066 6f72  matrix)).    for
+00003da0: 2069 5f69 6478 2c20 6920 696e 2065 6e75   i_idx, i in enu
+00003db0: 6d65 7261 7465 2863 616e 6469 6461 7465  merate(candidate
+00003dc0: 7329 3a20 2020 2020 2020 2020 0a20 2020  s):         .   
+00003dd0: 2020 2020 2066 6f72 206a 5f69 6478 2c20       for j_idx, 
+00003de0: 6a20 696e 2065 6e75 6d65 7261 7465 2863  j in enumerate(c
+00003df0: 616e 6469 6461 7465 7329 3a20 0a20 2020  andidates): .   
+00003e00: 2020 2020 2020 2020 2069 6620 6921 3d20           if i!= 
+00003e10: 6a3a 0a20 2020 2020 2020 2020 2020 2020  j:.             
+00003e20: 2020 2066 6f72 206b 5f69 6478 2c20 6b20     for k_idx, k 
+00003e30: 696e 2065 6e75 6d65 7261 7465 2863 616e  in enumerate(can
+00003e40: 6469 6461 7465 7329 3a20 0a20 2020 2020  didates): .     
+00003e50: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00003e60: 6620 6921 3d20 6b20 616e 6420 6a20 213d  f i!= k and j !=
+00003e70: 206b 3a0a 2020 2020 2020 2020 2020 2020   k:.            
+00003e80: 2020 2020 2020 2020 2020 2020 7374 7265              stre
+00003e90: 6e67 7468 5b6a 5f69 6478 5d5b 6b5f 6964  ngth[j_idx][k_id
+00003ea0: 785d 203d 206d 6178 2873 7472 656e 6774  x] = max(strengt
+00003eb0: 685b 6a5f 6964 785d 5b6b 5f69 6478 5d2c  h[j_idx][k_idx],
+00003ec0: 206d 696e 2873 7472 656e 6774 685b 6a5f   min(strength[j_
+00003ed0: 6964 785d 5b69 5f69 6478 5d2c 7374 7265  idx][i_idx],stre
+00003ee0: 6e67 7468 5b69 5f69 6478 5d5b 6b5f 6964  ngth[i_idx][k_id
+00003ef0: 785d 2929 0a0a 2020 2020 6465 6665 6174  x]))..    defeat
+00003f00: 5f67 7261 7068 203d 206e 782e 4469 4772  _graph = nx.DiGr
+00003f10: 6170 6828 290a 2020 2020 6465 6665 6174  aph().    defeat
+00003f20: 5f67 7261 7068 2e61 6464 5f6e 6f64 6573  _graph.add_nodes
+00003f30: 5f66 726f 6d28 6361 6e64 6964 6174 6573  _from(candidates
+00003f40: 290a 2020 2020 0a20 2020 2066 6f72 2069  ).    .    for i
+00003f50: 5f69 6478 2c20 6920 696e 2065 6e75 6d65  _idx, i in enume
+00003f60: 7261 7465 2863 616e 6469 6461 7465 7329  rate(candidates)
+00003f70: 3a20 0a20 2020 2020 2020 2066 6f72 206a  : .        for j
+00003f80: 5f69 6478 2c20 6a20 696e 2065 6e75 6d65  _idx, j in enume
+00003f90: 7261 7465 2863 616e 6469 6461 7465 7329  rate(candidates)
+00003fa0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+00003fb0: 2069 213d 6a3a 0a20 2020 2020 2020 2020   i!=j:.         
+00003fc0: 2020 2020 2020 2069 6620 7374 7265 6e67         if streng
+00003fd0: 7468 5b6a 5f69 6478 5d5b 695f 6964 785d  th[j_idx][i_idx]
+00003fe0: 203e 2073 7472 656e 6774 685b 695f 6964   > strength[i_id
+00003ff0: 785d 5b6a 5f69 6478 5d3a 0a20 2020 2020  x][j_idx]:.     
+00004000: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00004010: 6566 6561 745f 6772 6170 682e 6164 645f  efeat_graph.add_
+00004020: 7765 6967 6874 6564 5f65 6467 6573 5f66  weighted_edges_f
+00004030: 726f 6d28 5b28 6a2c 692c 735f 6d61 7472  rom([(j,i,s_matr
+00004040: 6978 5b6a 5f69 6478 5d5b 695f 6964 785d  ix[j_idx][i_idx]
+00004050: 295d 290a 0a20 2020 2072 6574 7572 6e20  )])..    return 
+00004060: 6465 6665 6174 5f67 7261 7068 0a0a 0a0a  defeat_graph....
+00004070: 6465 6620 6861 735f 7374 726f 6e67 5f70  def has_strong_p
+00004080: 6174 6828 412c 2073 6f75 7263 652c 2074  ath(A, source, t
+00004090: 6172 6765 742c 206b 293a 0a20 2020 2022  arget, k):.    "
+000040a0: 2222 4769 7665 6e20 6120 7371 7561 7265  ""Given a square
+000040b0: 206d 6174 7269 7820 412c 2072 6574 7572   matrix A, retur
+000040c0: 6e20 5472 7565 2069 6620 7468 6572 6520  n True if there 
+000040d0: 6973 2061 2070 6174 6820 6672 6f6d 2073  is a path from s
+000040e0: 6f75 7263 6520 746f 2074 6172 6765 7420  ource to target 
+000040f0: 696e 2074 6865 2061 7373 6f63 6961 7465  in the associate
+00004100: 6420 6469 7265 6374 6564 2067 7261 7068  d directed graph
+00004110: 2020 2020 2077 6865 7265 2065 6163 6820       where each 
+00004120: 6564 6765 2068 6173 2061 2077 6569 6768  edge has a weigh
+00004130: 7420 6772 6561 7465 7220 7468 616e 206f  t greater than o
+00004140: 7220 6571 7561 6c20 746f 206b 2c20 616e  r equal to k, an
+00004150: 6420 4661 6c73 6520 6f74 6865 7277 6973  d False otherwis
+00004160: 652e 2222 220a 2020 2020 0a20 2020 206e  e.""".    .    n
+00004170: 203d 2041 2e73 6861 7065 5b30 5d20 2320   = A.shape[0] # 
+00004180: 6173 7375 6d65 2041 2069 7320 6120 7371  assume A is a sq
+00004190: 7561 7265 206d 6174 7269 780a 2020 2020  uare matrix.    
+000041a0: 7669 7369 7465 6420 3d20 6e70 2e7a 6572  visited = np.zer
+000041b0: 6f73 286e 2c20 6474 7970 653d 626f 6f6c  os(n, dtype=bool
+000041c0: 290a 0a20 2020 2064 6566 2064 6673 286e  )..    def dfs(n
+000041d0: 6f64 6529 3a0a 2020 2020 2020 2020 6966  ode):.        if
+000041e0: 206e 6f64 6520 3d3d 2074 6172 6765 743a   node == target:
+000041f0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00004200: 7572 6e20 5472 7565 0a20 2020 2020 2020  urn True.       
+00004210: 2076 6973 6974 6564 5b6e 6f64 655d 203d   visited[node] =
+00004220: 2054 7275 650a 2020 2020 2020 2020 666f   True.        fo
+00004230: 7220 6e65 6967 6862 6f72 2c20 7765 6967  r neighbor, weig
+00004240: 6874 2069 6e20 656e 756d 6572 6174 6528  ht in enumerate(
+00004250: 415b 6e6f 6465 2c20 3a5d 293a 0a20 2020  A[node, :]):.   
+00004260: 2020 2020 2020 2020 2069 6620 415b 6e6f           if A[no
+00004270: 6465 5d5b 6e65 6967 6862 6f72 5d20 3e20  de][neighbor] > 
+00004280: 415b 6e65 6967 6862 6f72 5d5b 6e6f 6465  A[neighbor][node
+00004290: 5d20 616e 6420 7765 6967 6874 203e 3d20  ] and weight >= 
+000042a0: 6b20 616e 6420 6e6f 7420 7669 7369 7465  k and not visite
+000042b0: 645b 6e65 6967 6862 6f72 5d3a 0a20 2020  d[neighbor]:.   
+000042c0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+000042d0: 6466 7328 6e65 6967 6862 6f72 293a 0a20  dfs(neighbor):. 
+000042e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000042f0: 2020 2072 6574 7572 6e20 5472 7565 0a20     return True. 
+00004300: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
+00004310: 6c73 650a 0a20 2020 2072 6574 7572 6e20  lse..    return 
+00004320: 6466 7328 736f 7572 6365 290a 0a64 6566  dfs(source)..def
+00004330: 205f 7370 6c69 745f 6379 636c 655f 6261   _split_cycle_ba
+00004340: 7369 6328 0a20 2020 2020 2020 2065 6461  sic(.        eda
+00004350: 7461 2c20 0a20 2020 2020 2020 2063 7572  ta, .        cur
+00004360: 725f 6361 6e64 7320 3d20 4e6f 6e65 2c20  r_cands = None, 
+00004370: 0a20 2020 2020 2020 2073 7472 656e 6774  .        strengt
+00004380: 685f 6675 6e63 7469 6f6e 203d 204e 6f6e  h_function = Non
+00004390: 6529 3a0a 2020 2020 2222 2241 6e20 696d  e):.    """An im
+000043a0: 706c 656d 656e 7461 7469 6f6e 206f 6620  plementation of 
+000043b0: 5370 6c69 7420 4379 636c 6520 6261 7365  Split Cycle base
+000043c0: 6420 6f6e 2074 6865 206d 6174 6865 6d61  d on the mathema
+000043d0: 7469 6361 6c20 6465 6669 6e69 7469 6f6e  tical definition
+000043e0: 2e20 2020 0a20 2020 2022 2222 0a20 2020  .   .    """.   
+000043f0: 2073 7472 656e 6774 685f 6d61 7472 6978   strength_matrix
+00004400: 2c20 6361 6e64 5f74 6f5f 6369 6e64 6578  , cand_to_cindex
+00004410: 203d 2065 6461 7461 2e73 7472 656e 6774   = edata.strengt
+00004420: 685f 6d61 7472 6978 2863 7572 725f 6361  h_matrix(curr_ca
+00004430: 6e64 7320 3d20 6375 7272 5f63 616e 6473  nds = curr_cands
+00004440: 2c20 7374 7265 6e67 7468 5f66 756e 6374  , strength_funct
+00004450: 696f 6e3d 7374 7265 6e67 7468 5f66 756e  ion=strength_fun
+00004460: 6374 696f 6e29 0a0a 2020 2020 6361 6e64  ction)..    cand
+00004470: 6964 6174 6573 203d 2065 6461 7461 2e63  idates = edata.c
+00004480: 616e 6469 6461 7465 7320 6966 2063 7572  andidates if cur
+00004490: 725f 6361 6e64 7320 6973 204e 6f6e 6520  r_cands is None 
+000044a0: 656c 7365 2063 7572 725f 6361 6e64 7320  else curr_cands 
+000044b0: 200a 0a20 2020 2073 7472 656e 6774 685f   ..    strength_
+000044c0: 6675 6e63 7469 6f6e 203d 2065 6461 7461  function = edata
+000044d0: 2e6d 6172 6769 6e20 6966 2073 7472 656e  .margin if stren
+000044e0: 6774 685f 6675 6e63 7469 6f6e 2069 7320  gth_function is 
+000044f0: 4e6f 6e65 2065 6c73 6520 7374 7265 6e67  None else streng
+00004500: 7468 5f66 756e 6374 696f 6e20 0a0a 2020  th_function ..  
+00004510: 2020 706f 7465 6e74 6961 6c5f 7769 6e6e    potential_winn
+00004520: 6572 7320 3d20 7365 7428 6361 6e64 6964  ers = set(candid
+00004530: 6174 6573 290a 0a20 2020 2066 6f72 2061  ates)..    for a
+00004540: 2069 6e20 6361 6e64 6964 6174 6573 3a0a   in candidates:.
+00004550: 2020 2020 2020 2020 666f 7220 6220 696e          for b in
+00004560: 2063 616e 6469 6461 7465 733a 0a20 2020   candidates:.   
+00004570: 2020 2020 2020 2020 2069 6620 7374 7265           if stre
+00004580: 6e67 7468 5f66 756e 6374 696f 6e28 622c  ngth_function(b,
+00004590: 2061 2920 3e20 7374 7265 6e67 7468 5f66   a) > strength_f
+000045a0: 756e 6374 696f 6e28 612c 2062 2920 616e  unction(a, b) an
+000045b0: 6420 6e6f 7420 6861 735f 7374 726f 6e67  d not has_strong
+000045c0: 5f70 6174 6828 7374 7265 6e67 7468 5f6d  _path(strength_m
+000045d0: 6174 7269 782c 2063 616e 645f 746f 5f63  atrix, cand_to_c
+000045e0: 696e 6465 7828 6129 2c20 6361 6e64 5f74  index(a), cand_t
+000045f0: 6f5f 6369 6e64 6578 2862 292c 2073 7472  o_cindex(b), str
+00004600: 656e 6774 685f 6675 6e63 7469 6f6e 2862  ength_function(b
+00004610: 2c61 2929 3a0a 2020 2020 2020 2020 2020  ,a)):.          
+00004620: 2020 2020 2020 706f 7465 6e74 6961 6c5f        potential_
+00004630: 7769 6e6e 6572 732e 6469 7363 6172 6428  winners.discard(
+00004640: 6129 0a20 2020 2020 2020 2020 2020 2020  a).             
+00004650: 2020 2062 7265 616b 0a0a 2020 2020 7265     break..    re
+00004660: 7475 726e 2073 6f72 7465 6428 706f 7465  turn sorted(pote
+00004670: 6e74 6961 6c5f 7769 6e6e 6572 7329 0a0a  ntial_winners)..
+00004680: 6465 6620 5f69 735f 6361 6e64 5f73 706c  def _is_cand_spl
+00004690: 6974 5f63 7963 6c65 5f64 6566 6561 7465  it_cycle_defeate
+000046a0: 6428 612c 2073 7472 656e 6774 685f 6d61  d(a, strength_ma
+000046b0: 7472 6978 293a 0a0a 2020 2020 666f 7220  trix):..    for 
+000046c0: 6220 696e 2072 616e 6765 2873 7472 656e  b in range(stren
+000046d0: 6774 685f 6d61 7472 6978 2e73 6861 7065  gth_matrix.shape
+000046e0: 5b30 5d29 3a0a 2020 2020 2020 2020 6966  [0]):.        if
+000046f0: 2073 7472 656e 6774 685f 6d61 7472 6978   strength_matrix
+00004700: 5b62 5d5b 615d 203e 2073 7472 656e 6774  [b][a] > strengt
+00004710: 685f 6d61 7472 6978 5b61 5d5b 625d 2061  h_matrix[a][b] a
+00004720: 6e64 206e 6f74 2068 6173 5f73 7472 6f6e  nd not has_stron
+00004730: 675f 7061 7468 2873 7472 656e 6774 685f  g_path(strength_
+00004740: 6d61 7472 6978 2c20 612c 2020 622c 2073  matrix, a,  b, s
+00004750: 7472 656e 6774 685f 6d61 7472 6978 5b62  trength_matrix[b
+00004760: 5d5b 615d 293a 0a20 2020 2020 2020 2020  ][a]):.         
+00004770: 2020 2072 6574 7572 6e20 5472 7565 0a20     return True. 
+00004780: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
+00004790: 0a0a 6465 6620 6261 7463 6828 6974 6572  ..def batch(iter
+000047a0: 6162 6c65 2c20 6e3d 3129 3a0a 2020 2020  able, n=1):.    
+000047b0: 6c20 3d20 6c65 6e28 6974 6572 6162 6c65  l = len(iterable
+000047c0: 290a 2020 2020 666f 7220 6e64 7820 696e  ).    for ndx in
+000047d0: 2072 616e 6765 2830 2c20 6c2c 206e 293a   range(0, l, n):
+000047e0: 0a20 2020 2020 2020 2079 6965 6c64 2069  .        yield i
+000047f0: 7465 7261 626c 655b 6e64 783a 6d69 6e28  terable[ndx:min(
+00004800: 6e64 7820 2b20 6e2c 206c 295d 0a0a 6465  ndx + n, l)]..de
+00004810: 6620 7072 6f63 6573 735f 6261 7463 685f  f process_batch_
+00004820: 6f66 5f63 616e 6469 6461 7465 7328 6261  of_candidates(ba
+00004830: 7463 682c 2073 7472 656e 6774 685f 6d61  tch, strength_ma
+00004840: 7472 6978 293a 0a20 2020 2072 6573 756c  trix):.    resul
+00004850: 7473 203d 205b 5d0a 2020 2020 666f 7220  ts = [].    for 
+00004860: 6361 6e64 6964 6174 6520 696e 2062 6174  candidate in bat
+00004870: 6368 3a0a 2020 2020 2020 2020 7265 7375  ch:.        resu
+00004880: 6c74 203d 205f 6973 5f63 616e 645f 7370  lt = _is_cand_sp
+00004890: 6c69 745f 6379 636c 655f 6465 6665 6174  lit_cycle_defeat
+000048a0: 6564 2863 616e 6469 6461 7465 2c20 7374  ed(candidate, st
+000048b0: 7265 6e67 7468 5f6d 6174 7269 7829 0a20  rength_matrix). 
+000048c0: 2020 2020 2020 2072 6573 756c 7473 2e61         results.a
+000048d0: 7070 656e 6428 7265 7375 6c74 290a 2020  ppend(result).  
+000048e0: 2020 7265 7475 726e 2072 6573 756c 7473    return results
+000048f0: 0a0a 6465 6620 5f73 706c 6974 5f63 7963  ..def _split_cyc
+00004900: 6c65 5f62 6173 6963 5f70 6172 616c 6c65  le_basic_paralle
+00004910: 6c28 7374 7265 6e67 7468 5f6d 6174 7269  l(strength_matri
+00004920: 782c 206e 756d 5f63 7075 733d 3429 3a0a  x, num_cpus=4):.
+00004930: 0a20 2020 206e 756d 5f63 616e 6473 203d  .    num_cands =
+00004940: 2073 7472 656e 6774 685f 6d61 7472 6978   strength_matrix
+00004950: 2e73 6861 7065 5b30 5d0a 2020 2020 6361  .shape[0].    ca
+00004960: 6e64 7320 3d20 6c69 7374 2872 616e 6765  nds = list(range
+00004970: 286e 756d 5f63 616e 6473 2929 0a20 2020  (num_cands)).   
+00004980: 2062 6174 6368 5f73 697a 6520 3d20 6e75   batch_size = nu
+00004990: 6d5f 6361 6e64 7320 2f2f 206e 756d 5f63  m_cands // num_c
+000049a0: 7075 7320 2b20 286e 756d 5f63 616e 6473  pus + (num_cands
+000049b0: 2025 206e 756d 5f63 7075 7320 3e20 3029   % num_cpus > 0)
+000049c0: 0a20 2020 2063 616e 6469 6461 7465 5f62  .    candidate_b
+000049d0: 6174 6368 6573 203d 206c 6973 7428 6261  atches = list(ba
+000049e0: 7463 6828 6361 6e64 732c 2062 6174 6368  tch(cands, batch
+000049f0: 5f73 697a 6529 290a 2020 2020 7769 7468  _size)).    with
+00004a00: 2050 6f6f 6c28 6e75 6d5f 6370 7573 2920   Pool(num_cpus) 
+00004a10: 6173 2070 6f6f 6c3a 0a20 2020 2020 2020  as pool:.       
+00004a20: 2062 6174 6368 5f61 7267 7320 3d20 5b28   batch_args = [(
+00004a30: 6261 7463 682c 2073 7472 656e 6774 685f  batch, strength_
+00004a40: 6d61 7472 6978 2920 0a20 2020 2020 2020  matrix) .       
+00004a50: 2066 6f72 2062 6174 6368 2069 6e20 6361   for batch in ca
+00004a60: 6e64 6964 6174 655f 6261 7463 6865 735d  ndidate_batches]
+00004a70: 0a20 2020 2020 2020 2072 6573 756c 7473  .        results
+00004a80: 203d 2070 6f6f 6c2e 7374 6172 6d61 7028   = pool.starmap(
+00004a90: 7072 6f63 6573 735f 6261 7463 685f 6f66  process_batch_of
+00004aa0: 5f63 616e 6469 6461 7465 732c 2062 6174  _candidates, bat
+00004ab0: 6368 5f61 7267 7329 0a20 2020 2023 2046  ch_args).    # F
+00004ac0: 6c61 7474 656e 2074 6865 206c 6973 7420  latten the list 
+00004ad0: 6f66 2072 6573 756c 7473 0a20 2020 2073  of results.    s
+00004ae0: 635f 6465 6665 6174 5f64 6174 6120 3d20  c_defeat_data = 
+00004af0: 5b69 7465 6d20 666f 7220 7375 626c 6973  [item for sublis
+00004b00: 7420 696e 2072 6573 756c 7473 2066 6f72  t in results for
+00004b10: 2069 7465 6d20 696e 2073 7562 6c69 7374   item in sublist
+00004b20: 5d0a 0a20 2020 2072 6574 7572 6e20 736f  ]..    return so
+00004b30: 7274 6564 285b 6320 666f 7220 6320 696e  rted([c for c in
+00004b40: 2063 616e 6473 2069 6620 6e6f 7420 7363   cands if not sc
+00004b50: 5f64 6566 6561 745f 6461 7461 5b63 5d5d  _defeat_data[c]]
+00004b60: 290a 0a64 6566 205f 7370 6c69 745f 6379  )..def _split_cy
+00004b70: 636c 655f 666c 6f79 645f 7761 7273 6861  cle_floyd_warsha
+00004b80: 6c6c 280a 2020 2020 2020 2020 6564 6174  ll(.        edat
+00004b90: 612c 200a 2020 2020 2020 2020 6375 7272  a, .        curr
+00004ba0: 5f63 616e 6473 203d 204e 6f6e 652c 200a  _cands = None, .
+00004bb0: 2020 2020 2020 2020 7374 7265 6e67 7468          strength
+00004bc0: 5f66 756e 6374 696f 6e20 3d20 4e6f 6e65  _function = None
+00004bd0: 293a 2020 200a 2020 2020 2222 2241 6e20  ):   .    """An 
+00004be0: 696d 706c 656d 656e 7461 7469 6f6e 206f  implementation o
+00004bf0: 6620 5370 6c69 7420 4379 636c 6520 6261  f Split Cycle ba
+00004c00: 7365 6420 6f6e 2074 6865 2046 6c6f 7964  sed on the Floyd
+00004c10: 2d57 6172 7368 616c 6c20 416c 676f 7269  -Warshall Algori
+00004c20: 7468 6d2e 200a 0a20 2020 2053 6565 2068  thm. ..    See h
+00004c30: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00004c40: 6d2f 6570 6163 7569 742f 7370 6c69 7463  m/epacuit/splitc
+00004c50: 7963 6c65 2061 6e64 2074 6865 2070 6170  ycle and the pap
+00004c60: 6572 2068 7474 7073 3a2f 2f61 7278 6976  er https://arxiv
+00004c70: 2e6f 7267 2f61 6273 2f32 3030 342e 3032  .org/abs/2004.02
+00004c80: 3335 3020 666f 7220 6d6f 7265 2069 6e66  350 for more inf
+00004c90: 6f72 6d61 7469 6f6e 2e20 0a0a 2020 2020  ormation. ..    
+00004ca0: 2222 220a 0a20 2020 2063 616e 6469 6461  """..    candida
+00004cb0: 7465 7320 3d20 6564 6174 612e 6361 6e64  tes = edata.cand
+00004cc0: 6964 6174 6573 2069 6620 6375 7272 5f63  idates if curr_c
+00004cd0: 616e 6473 2069 7320 4e6f 6e65 2065 6c73  ands is None els
+00004ce0: 6520 6375 7272 5f63 616e 6473 2020 2020  e curr_cands    
+00004cf0: 0a20 2020 2073 7472 656e 6774 685f 6675  .    strength_fu
+00004d00: 6e63 7469 6f6e 203d 2065 6461 7461 2e6d  nction = edata.m
+00004d10: 6172 6769 6e20 6966 2073 7472 656e 6774  argin if strengt
+00004d20: 685f 6675 6e63 7469 6f6e 2069 7320 4e6f  h_function is No
+00004d30: 6e65 2065 6c73 6520 7374 7265 6e67 7468  ne else strength
+00004d40: 5f66 756e 6374 696f 6e20 0a20 0a20 2020  _function . .   
+00004d50: 2077 6561 6b5f 636f 6e64 6f72 6365 745f   weak_condorcet_
+00004d60: 7769 6e6e 6572 7320 3d20 7b63 3a54 7275  winners = {c:Tru
+00004d70: 6520 666f 7220 6320 696e 2063 616e 6469  e for c in candi
+00004d80: 6461 7465 737d 0a20 2020 2073 5f6d 6174  dates}.    s_mat
+00004d90: 7269 7820 3d20 5b5b 2d6e 702e 696e 6620  rix = [[-np.inf 
+00004da0: 666f 7220 5f20 696e 2063 616e 6469 6461  for _ in candida
+00004db0: 7465 735d 2066 6f72 205f 2069 6e20 6361  tes] for _ in ca
+00004dc0: 6e64 6964 6174 6573 5d0a 2020 2020 0a20  ndidates].    . 
+00004dd0: 2020 2023 2069 6e69 7469 616c 697a 6520     # initialize 
+00004de0: 7468 6520 735f 6d61 7472 6978 0a20 2020  the s_matrix.   
+00004df0: 2066 6f72 2063 315f 6964 782c 2063 3120   for c1_idx, c1 
+00004e00: 696e 2065 6e75 6d65 7261 7465 2863 616e  in enumerate(can
+00004e10: 6469 6461 7465 7329 3a0a 2020 2020 2020  didates):.      
+00004e20: 2020 666f 7220 6332 5f69 6478 2c20 6332    for c2_idx, c2
+00004e30: 2069 6e20 656e 756d 6572 6174 6528 6361   in enumerate(ca
+00004e40: 6e64 6964 6174 6573 293a 0a20 2020 2020  ndidates):.     
+00004e50: 2020 2020 2020 2069 6620 2865 6461 7461         if (edata
+00004e60: 2e6d 616a 6f72 6974 795f 7072 6566 6572  .majority_prefer
+00004e70: 7328 6331 2c20 6332 2920 6f72 2063 3120  s(c1, c2) or c1 
+00004e80: 3d3d 2063 3229 3a0a 2020 2020 2020 2020  == c2):.        
+00004e90: 2020 2020 2020 2020 735f 6d61 7472 6978          s_matrix
+00004ea0: 5b63 315f 6964 785d 5b63 325f 6964 785d  [c1_idx][c2_idx]
+00004eb0: 203d 2073 7472 656e 6774 685f 6675 6e63   = strength_func
+00004ec0: 7469 6f6e 2863 312c 2063 3229 200a 2020  tion(c1, c2) .  
+00004ed0: 2020 2020 2020 2020 2020 2020 2020 7765                we
+00004ee0: 616b 5f63 6f6e 646f 7263 6574 5f77 696e  ak_condorcet_win
+00004ef0: 6e65 7273 5b63 325d 203d 2077 6561 6b5f  ners[c2] = weak_
+00004f00: 636f 6e64 6f72 6365 745f 7769 6e6e 6572  condorcet_winner
+00004f10: 735b 6332 5d20 616e 6420 2863 3120 3d3d  s[c2] and (c1 ==
+00004f20: 2063 3229 2023 2057 6561 6b20 436f 6e64   c2) # Weak Cond
+00004f30: 6f72 6365 7420 7769 6e6e 6572 7320 6172  orcet winners ar
+00004f40: 6520 5370 6c69 7420 4379 636c 6520 7769  e Split Cycle wi
+00004f50: 6e6e 6572 730a 2020 2020 0a20 2020 2073  nners.    .    s
+00004f60: 7472 656e 6774 6820 3d20 6c69 7374 286d  trength = list(m
+00004f70: 6170 286c 616d 6264 6120 6920 3a20 6c69  ap(lambda i : li
+00004f80: 7374 286d 6170 286c 616d 6264 6120 6a20  st(map(lambda j 
+00004f90: 3a20 6a20 2c20 6929 2920 2c20 735f 6d61  : j , i)) , s_ma
+00004fa0: 7472 6978 2929 0a20 2020 2066 6f72 2069  trix)).    for i
+00004fb0: 5f69 6478 2c20 6920 696e 2065 6e75 6d65  _idx, i in enume
+00004fc0: 7261 7465 2863 616e 6469 6461 7465 7329  rate(candidates)
+00004fd0: 3a20 0a20 2020 2020 2020 2066 6f72 206a  : .        for j
+00004fe0: 5f69 6478 2c20 6a20 696e 2065 6e75 6d65  _idx, j in enume
+00004ff0: 7261 7465 2863 616e 6469 6461 7465 7329  rate(candidates)
+00005000: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+00005010: 2069 213d 206a 3a0a 2020 2020 2020 2020   i!= j:.        
+00005020: 2020 2020 2020 2020 6966 206e 6f74 2077          if not w
+00005030: 6561 6b5f 636f 6e64 6f72 6365 745f 7769  eak_condorcet_wi
+00005040: 6e6e 6572 735b 6a5d 3a20 2320 7765 616b  nners[j]: # weak
+00005050: 2043 6f6e 646f 7263 6574 2077 696e 6e65   Condorcet winne
+00005060: 7273 2061 7265 2053 706c 6974 2043 7963  rs are Split Cyc
+00005070: 6c65 2077 696e 6e65 7273 0a20 2020 2020  le winners.     
+00005080: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00005090: 6f72 206b 5f69 6478 2c20 6b20 696e 2065  or k_idx, k in e
+000050a0: 6e75 6d65 7261 7465 2863 616e 6469 6461  numerate(candida
+000050b0: 7465 7329 3a20 0a20 2020 2020 2020 2020  tes): .         
+000050c0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000050d0: 6620 6920 213d 206b 2061 6e64 206a 2021  f i != k and j !
+000050e0: 3d20 6b3a 0a20 2020 2020 2020 2020 2020  = k:.           
+000050f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005100: 2073 7472 656e 6774 685b 6a5f 6964 785d   strength[j_idx]
+00005110: 5b6b 5f69 6478 5d20 3d20 6d61 7828 7374  [k_idx] = max(st
+00005120: 7265 6e67 7468 5b6a 5f69 6478 5d5b 6b5f  rength[j_idx][k_
+00005130: 6964 785d 2c20 6d69 6e28 7374 7265 6e67  idx], min(streng
+00005140: 7468 5b6a 5f69 6478 5d5b 695f 6964 785d  th[j_idx][i_idx]
+00005150: 2c73 7472 656e 6774 685b 695f 6964 785d  ,strength[i_idx]
+00005160: 5b6b 5f69 6478 5d29 290a 2020 2020 7769  [k_idx])).    wi
+00005170: 6e6e 6572 7320 3d20 7b69 3a54 7275 6520  nners = {i:True 
+00005180: 666f 7220 6920 696e 2063 616e 6469 6461  for i in candida
+00005190: 7465 737d 0a20 2020 2066 6f72 2069 5f69  tes}.    for i_i
+000051a0: 6478 2c20 6920 696e 2065 6e75 6d65 7261  dx, i in enumera
+000051b0: 7465 2863 616e 6469 6461 7465 7329 3a0a  te(candidates):.
+000051c0: 2020 2020 2020 2020 666f 7220 6a5f 6964          for j_id
+000051d0: 782c 206a 2069 6e20 656e 756d 6572 6174  x, j in enumerat
+000051e0: 6528 6361 6e64 6964 6174 6573 293a 0a20  e(candidates):. 
+000051f0: 2020 2020 2020 2020 2020 2069 6620 6920             if i 
+00005200: 213d 206a 3a0a 2020 2020 2020 2020 2020  != j:.          
+00005210: 2020 2020 2020 6966 2073 5f6d 6174 7269        if s_matri
+00005220: 785b 6a5f 6964 785d 5b69 5f69 6478 5d20  x[j_idx][i_idx] 
+00005230: 3e20 7374 7265 6e67 7468 5b69 5f69 6478  > strength[i_idx
+00005240: 5d5b 6a5f 6964 785d 3a20 2320 7468 6520  ][j_idx]: # the 
+00005250: 6d61 696e 2064 6966 6665 7265 6e63 6520  main difference 
+00005260: 7769 7468 2042 6561 7420 5061 7468 0a20  with Beat Path. 
+00005270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005280: 2020 2077 696e 6e65 7273 5b69 5d20 3d20     winners[i] = 
+00005290: 4661 6c73 650a 2020 2020 7265 7475 726e  False.    return
+000052a0: 2073 6f72 7465 6428 5b63 2066 6f72 2063   sorted([c for c
+000052b0: 2069 6e20 6361 6e64 6964 6174 6573 2069   in candidates i
+000052c0: 6620 7769 6e6e 6572 735b 635d 5d29 0a0a  f winners[c]])..
+000052d0: 7363 5f70 726f 7065 7274 6965 7320 3d20  sc_properties = 
+000052e0: 566f 7469 6e67 4d65 7468 6f64 5072 6f70  VotingMethodProp
+000052f0: 6572 7469 6573 280a 2020 2020 636f 6e64  erties(.    cond
+00005300: 6f72 6365 745f 7769 6e6e 6572 3d54 7275  orcet_winner=Tru
+00005310: 652c 200a 2020 2020 636f 6e64 6f72 6365  e, .    condorce
+00005320: 745f 6c6f 7365 723d 5472 7565 2c0a 2020  t_loser=True,.  
+00005330: 2020 7061 7265 746f 5f64 6f6d 696e 616e    pareto_dominan
+00005340: 6365 3d54 7275 652c 0a20 2020 2070 6f73  ce=True,.    pos
+00005350: 6974 6976 655f 696e 766f 6c76 656d 656e  itive_involvemen
+00005360: 743d 5472 7565 2c20 0a20 2020 2029 0a40  t=True, .    ).@
+00005370: 766d 286e 616d 653d 2253 706c 6974 2043  vm(name="Split C
+00005380: 7963 6c65 222c 0a20 2020 2070 726f 7065  ycle",.    prope
+00005390: 7274 6965 733d 7363 5f70 726f 7065 7274  rties=sc_propert
+000053a0: 6965 732c 0a20 2020 2069 6e70 7574 5f74  ies,.    input_t
+000053b0: 7970 6573 3d5b 456c 6563 7469 6f6e 5479  ypes=[ElectionTy
+000053c0: 7065 732e 5052 4f46 494c 452c 2045 6c65  pes.PROFILE, Ele
+000053d0: 6374 696f 6e54 7970 6573 2e50 524f 4649  ctionTypes.PROFI
+000053e0: 4c45 5f57 4954 485f 5449 4553 2c20 456c  LE_WITH_TIES, El
+000053f0: 6563 7469 6f6e 5479 7065 732e 4d41 5247  ectionTypes.MARG
+00005400: 494e 5f47 5241 5048 5d29 0a64 6566 2073  IN_GRAPH]).def s
+00005410: 706c 6974 5f63 7963 6c65 280a 2020 2020  plit_cycle(.    
+00005420: 6564 6174 612c 200a 2020 2020 6375 7272  edata, .    curr
+00005430: 5f63 616e 6473 3d4e 6f6e 652c 200a 2020  _cands=None, .  
+00005440: 2020 7374 7265 6e67 7468 5f66 756e 6374    strength_funct
+00005450: 696f 6e3d 4e6f 6e65 2c0a 2020 2020 616c  ion=None,.    al
+00005460: 676f 7269 7468 6d3d 2762 6173 6963 272c  gorithm='basic',
+00005470: 0a20 2020 206e 756d 5f63 7075 733d 3429  .    num_cpus=4)
+00005480: 3a0a 0a20 2020 2022 2222 4120 2a2a 6d61  :..    """A **ma
+00005490: 6a6f 7269 7479 2063 7963 6c65 2a2a 2069  jority cycle** i
+000054a0: 7320 6120 7365 7175 656e 6365 203a 6d61  s a sequence :ma
+000054b0: 7468 3a60 785f 312c 205c 6c64 6f74 7320  th:`x_1, \ldots 
+000054c0: 2c78 5f6e 6020 6f66 2064 6973 7469 6e63  ,x_n` of distinc
+000054d0: 7420 6361 6e64 6964 6174 6573 2077 6974  t candidates wit
+000054e0: 6820 3a6d 6174 683a 6078 5f31 3d78 5f6e  h :math:`x_1=x_n
+000054f0: 6020 7375 6368 2074 6861 7420 666f 7220  ` such that for 
+00005500: 3a6d 6174 683a 6031 205c 6c65 7120 6b20  :math:`1 \leq k 
+00005510: 5c6c 6571 206e 2d31 602c 2020 3a6d 6174  \leq n-1`,  :mat
+00005520: 683a 6078 5f6b 6020 6973 206d 616a 6f72  h:`x_k` is major
+00005530: 6974 7920 7072 6566 6572 7265 6420 746f  ity preferred to
+00005540: 203a 6d61 7468 3a60 785f 7b6b 2b31 7d60   :math:`x_{k+1}`
+00005550: 2e20 2054 6865 2053 706c 6974 2043 7963  .  The Split Cyc
+00005560: 6c65 2077 696e 6e65 7273 2061 7265 2064  le winners are d
+00005570: 6574 6572 6d69 6e65 6420 6173 2066 6f6c  etermined as fol
+00005580: 6c6f 7773 3a20 200a 2020 2020 0a20 2020  lows:  .    .   
+00005590: 2049 6620 6361 6e64 6964 6174 6520 7820   If candidate x 
+000055a0: 6861 7320 6120 706f 7369 7469 7665 206d  has a positive m
+000055b0: 6172 6769 6e20 6f76 6572 2079 2061 6e64  argin over y and
+000055c0: 2028 782c 7929 2069 7320 6e6f 7420 7468   (x,y) is not th
+000055d0: 6520 7765 616b 6573 7420 6564 6765 2069  e weakest edge i
+000055e0: 6e20 6120 6379 636c 652c 2074 6865 6e20  n a cycle, then 
+000055f0: 7820 6465 6665 6174 7320 792e 2045 7175  x defeats y. Equ
+00005600: 6976 616c 656e 746c 792c 2069 6620 7820  ivalently, if x 
+00005610: 6861 7320 6120 706f 7369 7469 7665 206d  has a positive m
+00005620: 6172 6769 6e20 6f76 6572 2079 2061 6e64  argin over y and
+00005630: 2074 6865 7265 2069 7320 6e6f 2070 6174   there is no pat
+00005640: 6820 6672 6f6d 2079 2062 6163 6b20 746f  h from y back to
+00005650: 2078 206f 6620 7374 7265 6e67 7468 2061   x of strength a
+00005660: 7420 6c65 6173 7420 7468 6520 6d61 7267  t least the marg
+00005670: 696e 206f 6620 7820 6f76 6572 2079 2c20  in of x over y, 
+00005680: 7468 656e 2078 2064 6566 6561 7473 2079  then x defeats y
+00005690: 2e20 0a20 2020 200a 2020 2020 5468 6520  . .    .    The 
+000056a0: 6361 6e64 6964 6174 6573 2074 6861 7420  candidates that 
+000056b0: 6172 6520 756e 6465 6665 6174 6564 2061  are undefeated a
+000056c0: 7265 2074 6865 2053 706c 6974 2043 7963  re the Split Cyc
+000056d0: 6c65 2077 696e 6e65 7273 2e0a 0a20 2020  le winners...   
+000056e0: 2053 6565 2068 7474 7073 3a2f 2f67 6974   See https://git
+000056f0: 6875 622e 636f 6d2f 6570 6163 7569 742f  hub.com/epacuit/
+00005700: 7370 6c69 7463 7963 6c65 2061 6e64 2074  splitcycle and t
+00005710: 6865 2070 6170 6572 2068 7474 7073 3a2f  he paper https:/
+00005720: 2f61 7278 6976 2e6f 7267 2f61 6273 2f32  /arxiv.org/abs/2
+00005730: 3030 342e 3032 3335 3020 666f 7220 6d6f  004.02350 for mo
+00005740: 7265 2069 6e66 6f72 6d61 7469 6f6e 2e20  re information. 
+00005750: 0a0a 2020 2020 4172 6773 3a0a 2020 2020  ..    Args:.    
+00005760: 2020 2020 6564 6174 6120 2850 726f 6669      edata (Profi
+00005770: 6c65 2c20 5072 6f66 696c 6557 6974 6854  le, ProfileWithT
+00005780: 6965 732c 204d 6172 6769 6e47 7261 7068  ies, MarginGraph
+00005790: 293a 2041 6e79 2065 6c65 6374 696f 6e20  ): Any election 
+000057a0: 6461 7461 2074 6861 7420 6861 7320 6120  data that has a 
+000057b0: 606d 6172 6769 6e60 206d 6574 686f 642e  `margin` method.
+000057c0: 200a 2020 2020 2020 2020 6375 7272 5f63   .        curr_c
+000057d0: 616e 6473 2028 4c69 7374 5b69 6e74 5d2c  ands (List[int],
+000057e0: 206f 7074 696f 6e61 6c29 3a20 4966 2073   optional): If s
+000057f0: 6574 2c20 7468 656e 2066 696e 6420 7468  et, then find th
+00005800: 6520 7769 6e6e 6572 7320 666f 7220 7468  e winners for th
+00005810: 6520 7072 6f66 696c 6520 7265 7374 7269  e profile restri
+00005820: 6374 6564 2074 6f20 7468 6520 6361 6e64  cted to the cand
+00005830: 6964 6174 6573 2069 6e20 6060 6375 7272  idates in ``curr
+00005840: 5f63 616e 6473 6060 0a20 2020 2020 2020  _cands``.       
+00005850: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
+00005860: 6f6e 2028 6675 6e63 7469 6f6e 2c20 6f70  on (function, op
+00005870: 7469 6f6e 616c 293a 2054 6865 2073 7472  tional): The str
+00005880: 656e 6774 6820 6675 6e63 7469 6f6e 2074  ength function t
+00005890: 6f20 6265 2075 7365 6420 746f 2063 616c  o be used to cal
+000058a0: 6375 6c61 7465 2074 6865 2073 7472 656e  culate the stren
+000058b0: 6774 6820 6f66 2061 2070 6174 682e 2020  gth of a path.  
+000058c0: 2054 6865 2064 6566 6175 6c74 2069 7320   The default is 
+000058d0: 7468 6520 6d61 7267 696e 206d 6574 686f  the margin metho
+000058e0: 6420 6f66 2060 6065 6461 7461 6060 2e20  d of ``edata``. 
+000058f0: 2020 5468 6973 206f 6e6c 7920 6d61 7474    This only matt
+00005900: 6572 7320 7768 656e 2074 6865 2062 616c  ers when the bal
+00005910: 6c6f 7473 2061 7265 206e 6f74 206c 696e  lots are not lin
+00005920: 6561 7220 6f72 6465 7273 2e20 0a20 2020  ear orders. .   
+00005930: 2020 2020 2061 6c67 6f72 6974 686d 2028       algorithm (
+00005940: 7374 7229 3a20 5370 6563 6966 7920 7768  str): Specify wh
+00005950: 6963 6820 616c 676f 7269 7468 6d20 746f  ich algorithm to
+00005960: 2075 7365 2e20 204f 7074 696f 6e73 2061   use.  Options a
+00005970: 7265 2027 6261 7369 6327 2028 7468 6520  re 'basic' (the 
+00005980: 6465 6661 756c 7429 2061 6e64 2027 666c  default) and 'fl
+00005990: 6f79 645f 7761 7273 6861 6c6c 272e 0a0a  oyd_warshall'...
+000059a0: 2020 2020 5265 7475 726e 733a 200a 2020      Returns: .  
+000059b0: 2020 2020 2020 4120 736f 7274 6564 206c        A sorted l
+000059c0: 6973 7420 6f66 2063 616e 6469 6461 7465  ist of candidate
+000059d0: 732e 200a 0a20 2020 202e 2e20 7365 6561  s. ..    .. seea
+000059e0: 6c73 6f3a 3a0a 0a20 2020 2020 2020 203a  lso::..        :
+000059f0: 6d65 7468 3a60 7072 6566 5f76 6f74 696e  meth:`pref_votin
+00005a00: 672e 6d61 7267 696e 5f62 6173 6564 5f6d  g.margin_based_m
+00005a10: 6574 686f 6473 2e73 706c 6974 5f63 7963  ethods.split_cyc
+00005a20: 6c65 5f64 6566 6561 7460 0a0a 2020 2020  le_defeat`..    
+00005a30: 3a45 7861 6d70 6c65 3a20 0a0a 2020 2020  :Example: ..    
+00005a40: 2e2e 2070 6c6f 743a 3a20 206d 6172 6769  .. plot::  margi
+00005a50: 6e5f 6772 6170 6873 5f65 7861 6d70 6c65  n_graphs_example
+00005a60: 732f 6d67 5f65 785f 6270 5f72 702e 7079  s/mg_ex_bp_rp.py
+00005a70: 0a20 2020 2020 2020 203a 636f 6e74 6578  .        :contex
+00005a80: 743a 2072 6573 6574 2020 0a20 2020 2020  t: reset  .     
+00005a90: 2020 203a 696e 636c 7564 652d 736f 7572     :include-sour
+00005aa0: 6365 3a20 5472 7565 0a0a 2020 2020 2e2e  ce: True..    ..
+00005ab0: 2063 6f64 652d 626c 6f63 6b3a 3a20 0a0a   code-block:: ..
+00005ac0: 2020 2020 2020 2020 6672 6f6d 2070 7265          from pre
+00005ad0: 665f 766f 7469 6e67 2e6d 6172 6769 6e5f  f_voting.margin_
+00005ae0: 6261 7365 645f 6d65 7468 6f64 7320 696d  based_methods im
+00005af0: 706f 7274 2073 706c 6974 5f63 7963 6c65  port split_cycle
+00005b00: 0a0a 2020 2020 2020 2020 7370 6c69 745f  ..        split_
+00005b10: 6379 636c 652e 6469 7370 6c61 7928 6d67  cycle.display(mg
+00005b20: 290a 0a0a 2020 2020 2e2e 2065 7865 635f  )...    .. exec_
+00005b30: 636f 6465 3a3a 200a 2020 2020 2020 2020  code:: .        
+00005b40: 3a68 6964 655f 636f 6465 3a0a 0a20 2020  :hide_code:..   
+00005b50: 2020 2020 2066 726f 6d20 7072 6566 5f76       from pref_v
+00005b60: 6f74 696e 672e 7765 6967 6874 6564 5f6d  oting.weighted_m
+00005b70: 616a 6f72 6974 795f 6772 6170 6873 2069  ajority_graphs i
+00005b80: 6d70 6f72 7420 4d61 7267 696e 4772 6170  mport MarginGrap
+00005b90: 680a 2020 2020 2020 2020 6672 6f6d 2070  h.        from p
+00005ba0: 7265 665f 766f 7469 6e67 2e6d 6172 6769  ref_voting.margi
+00005bb0: 6e5f 6261 7365 645f 6d65 7468 6f64 7320  n_based_methods 
+00005bc0: 696d 706f 7274 2073 706c 6974 5f63 7963  import split_cyc
+00005bd0: 6c65 0a20 2020 2020 2020 200a 2020 2020  le.        .    
+00005be0: 2020 2020 6d67 203d 204d 6172 6769 6e47      mg = MarginG
+00005bf0: 7261 7068 285b 302c 2031 2c20 322c 2033  raph([0, 1, 2, 3
+00005c00: 5d2c 205b 2830 2c20 322c 2033 292c 2028  ], [(0, 2, 3), (
+00005c10: 312c 2030 2c20 3529 2c20 2832 2c20 312c  1, 0, 5), (2, 1,
+00005c20: 2035 292c 2028 322c 2033 2c20 3129 2c20   5), (2, 3, 1), 
+00005c30: 2833 2c20 302c 2033 292c 2028 332c 2031  (3, 0, 3), (3, 1
+00005c40: 2c20 3129 5d29 0a20 2020 2020 2020 200a  , 1)]).        .
+00005c50: 2020 2020 2020 2020 7370 6c69 745f 6379          split_cy
+00005c60: 636c 652e 6469 7370 6c61 7928 6d67 290a  cle.display(mg).
+00005c70: 2020 2020 2020 2020 7370 6c69 745f 6379          split_cy
+00005c80: 636c 652e 6469 7370 6c61 7928 6d67 2c20  cle.display(mg, 
+00005c90: 616c 676f 7269 7468 6d3d 2762 6173 6963  algorithm='basic
+00005ca0: 2729 0a20 2020 2020 2020 2073 706c 6974  ').        split
+00005cb0: 5f63 7963 6c65 2e64 6973 706c 6179 286d  _cycle.display(m
+00005cc0: 672c 2061 6c67 6f72 6974 686d 3d27 666c  g, algorithm='fl
+00005cd0: 6f79 645f 7761 7273 6861 6c6c 2729 0a20  oyd_warshall'). 
+00005ce0: 2020 2022 2222 0a20 2020 200a 2020 2020     """.    .    
+00005cf0: 6966 2061 6c67 6f72 6974 686d 203d 3d20  if algorithm == 
+00005d00: 2762 6173 6963 273a 0a20 2020 2020 2020  'basic':.       
+00005d10: 2072 6574 7572 6e20 5f73 706c 6974 5f63   return _split_c
+00005d20: 7963 6c65 5f62 6173 6963 2865 6461 7461  ycle_basic(edata
+00005d30: 2c20 6375 7272 5f63 616e 6473 203d 2063  , curr_cands = c
+00005d40: 7572 725f 6361 6e64 732c 2073 7472 656e  urr_cands, stren
+00005d50: 6774 685f 6675 6e63 7469 6f6e 203d 2073  gth_function = s
+00005d60: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
+00005d70: 290a 2020 2020 656c 6966 2061 6c67 6f72  ).    elif algor
+00005d80: 6974 686d 203d 3d20 2766 6c6f 7964 5f77  ithm == 'floyd_w
+00005d90: 6172 7368 616c 6c27 3a0a 2020 2020 2020  arshall':.      
+00005da0: 2020 7265 7475 726e 205f 7370 6c69 745f    return _split_
+00005db0: 6379 636c 655f 666c 6f79 645f 7761 7273  cycle_floyd_wars
+00005dc0: 6861 6c6c 2865 6461 7461 2c20 6375 7272  hall(edata, curr
+00005dd0: 5f63 616e 6473 203d 2063 7572 725f 6361  _cands = curr_ca
+00005de0: 6e64 732c 2073 7472 656e 6774 685f 6675  nds, strength_fu
+00005df0: 6e63 7469 6f6e 203d 2073 7472 656e 6774  nction = strengt
+00005e00: 685f 6675 6e63 7469 6f6e 290a 2020 2020  h_function).    
+00005e10: 656c 6966 2061 6c67 6f72 6974 686d 203d  elif algorithm =
+00005e20: 3d20 2762 6173 6963 5f70 6172 616c 6c65  = 'basic_paralle
+00005e30: 6c27 3a0a 2020 2020 2020 2020 6375 7272  l':.        curr
+00005e40: 5f63 616e 6473 203d 2065 6461 7461 2e63  _cands = edata.c
+00005e50: 616e 6469 6461 7465 7320 6966 2063 7572  andidates if cur
+00005e60: 725f 6361 6e64 7320 6973 204e 6f6e 6520  r_cands is None 
+00005e70: 656c 7365 2063 7572 725f 6361 6e64 730a  else curr_cands.
+00005e80: 2020 2020 2020 2020 7374 7265 6e67 7468          strength
+00005e90: 5f6d 6174 7269 782c 2063 616e 645f 746f  _matrix, cand_to
+00005ea0: 5f63 696e 6465 7820 3d20 6564 6174 612e  _cindex = edata.
+00005eb0: 7374 7265 6e67 7468 5f6d 6174 7269 7828  strength_matrix(
+00005ec0: 6375 7272 5f63 616e 6473 203d 2063 7572  curr_cands = cur
+00005ed0: 725f 6361 6e64 732c 2073 7472 656e 6774  r_cands, strengt
+00005ee0: 685f 6675 6e63 7469 6f6e 3d73 7472 656e  h_function=stren
+00005ef0: 6774 685f 6675 6e63 7469 6f6e 290a 2020  gth_function).  
+00005f00: 2020 2020 2020 6369 6e64 785f 746f 5f63        cindx_to_c
+00005f10: 616e 6420 3d20 7b63 616e 645f 746f 5f63  and = {cand_to_c
+00005f20: 696e 6465 7828 6329 3a63 2066 6f72 2063  index(c):c for c
+00005f30: 2069 6e20 6375 7272 5f63 616e 6473 7d0a   in curr_cands}.
+00005f40: 2020 2020 2020 2020 7363 5f77 7320 3d20          sc_ws = 
+00005f50: 5f73 706c 6974 5f63 7963 6c65 5f62 6173  _split_cycle_bas
+00005f60: 6963 5f70 6172 616c 6c65 6c28 7374 7265  ic_parallel(stre
+00005f70: 6e67 7468 5f6d 6174 7269 782c 6e75 6d5f  ngth_matrix,num_
+00005f80: 6370 7573 3d6e 756d 5f63 7075 7329 0a20  cpus=num_cpus). 
+00005f90: 2020 2020 2020 2072 6574 7572 6e20 736f         return so
+00005fa0: 7274 6564 285b 6369 6e64 785f 746f 5f63  rted([cindx_to_c
+00005fb0: 616e 645b 635d 2066 6f72 2063 2069 6e20  and[c] for c in 
+00005fc0: 7363 5f77 735d 290a 2020 2020 656c 7365  sc_ws]).    else
+00005fd0: 3a0a 2020 2020 2020 2020 7261 6973 6520  :.        raise 
+00005fe0: 5661 6c75 6545 7272 6f72 2822 496e 7661  ValueError("Inva
+00005ff0: 6c69 6420 616c 676f 7269 7468 6d20 7370  lid algorithm sp
+00006000: 6563 6966 6965 642e 2229 0a0a 0a64 6566  ecified.")...def
+00006010: 2073 706c 6974 5f63 7963 6c65 5f64 6566   split_cycle_def
+00006020: 6561 7428 6564 6174 612c 2063 7572 725f  eat(edata, curr_
+00006030: 6361 6e64 7320 3d20 4e6f 6e65 2c20 7374  cands = None, st
+00006040: 7265 6e67 7468 5f66 756e 6374 696f 6e20  rength_function 
+00006050: 3d20 4e6f 6e65 293a 2020 200a 2020 2020  = None):   .    
+00006060: 2222 220a 2020 2020 5265 7475 726e 7320  """.    Returns 
+00006070: 7468 6520 5370 6c69 7420 4379 636c 6520  the Split Cycle 
+00006080: 6465 6665 6174 2072 656c 6174 696f 6e2e  defeat relation.
+00006090: 200a 0a20 2020 2053 6565 2068 7474 7073   ..    See https
+000060a0: 3a2f 2f61 7278 6976 2e6f 7267 2f61 6273  ://arxiv.org/abs
+000060b0: 2f32 3030 382e 3038 3435 3120 666f 7220  /2008.08451 for 
+000060c0: 616e 2065 7874 656e 6465 6420 6469 7363  an extended disc
+000060d0: 7573 7369 6f6e 206f 6620 7468 6973 206e  ussion of this n
+000060e0: 6f74 696f 6e20 6f66 2064 6566 6561 7420  otion of defeat 
+000060f0: 696e 2061 6e20 656c 6563 7469 6f6e 2e20  in an election. 
+00006100: 0a0a 2020 2020 4172 6773 3a0a 2020 2020  ..    Args:.    
+00006110: 2020 2020 6564 6174 6120 2850 726f 6669      edata (Profi
+00006120: 6c65 2c20 5072 6f66 696c 6557 6974 6854  le, ProfileWithT
+00006130: 6965 732c 204d 6172 6769 6e47 7261 7068  ies, MarginGraph
+00006140: 293a 2041 6e79 2065 6c65 6374 696f 6e20  ): Any election 
+00006150: 6461 7461 2074 6861 7420 6861 7320 6120  data that has a 
+00006160: 606d 6172 6769 6e60 206d 6574 686f 642e  `margin` method.
+00006170: 200a 2020 2020 2020 2020 6375 7272 5f63   .        curr_c
+00006180: 616e 6473 2028 4c69 7374 5b69 6e74 5d2c  ands (List[int],
+00006190: 206f 7074 696f 6e61 6c29 3a20 4966 2073   optional): If s
+000061a0: 6574 2c20 7468 656e 2066 696e 6420 7468  et, then find th
+000061b0: 6520 7769 6e6e 6572 7320 666f 7220 7468  e winners for th
+000061c0: 6520 7072 6f66 696c 6520 7265 7374 7269  e profile restri
+000061d0: 6374 6564 2074 6f20 7468 6520 6361 6e64  cted to the cand
+000061e0: 6964 6174 6573 2069 6e20 6060 6375 7272  idates in ``curr
+000061f0: 5f63 616e 6473 6060 0a0a 2020 2020 5265  _cands``..    Re
+00006200: 7475 726e 733a 200a 2020 2020 2020 2020  turns: .        
+00006210: 4120 6e65 7477 6f72 6b78 2044 6947 7261  A networkx DiGra
+00006220: 7068 2072 6570 7265 7365 6e74 696e 6720  ph representing 
+00006230: 7468 6520 5370 6c69 7420 4379 636c 6520  the Split Cycle 
+00006240: 6465 6665 6174 2072 656c 6174 696f 6e2e  defeat relation.
+00006250: 200a 0a20 2020 202e 2e20 7365 6561 6c73   ..    .. seeals
+00006260: 6f3a 3a0a 0a20 2020 2020 2020 203a 6d65  o::..        :me
+00006270: 7468 3a60 7072 6566 5f76 6f74 696e 672e  th:`pref_voting.
+00006280: 6d61 7267 696e 5f62 6173 6564 5f6d 6574  margin_based_met
+00006290: 686f 6473 2e73 706c 6974 5f63 7963 6c65  hods.split_cycle
+000062a0: 602c 203a 6d65 7468 3a60 7072 6566 5f76  `, :meth:`pref_v
+000062b0: 6f74 696e 672e 6d61 7267 696e 5f62 6173  oting.margin_bas
+000062c0: 6564 5f6d 6574 686f 6473 2e73 706c 6974  ed_methods.split
+000062d0: 5f63 7963 6c65 5f46 6c6f 7964 5f57 6172  _cycle_Floyd_War
+000062e0: 7368 616c 6c60 0a0a 2020 2020 3a45 7861  shall`..    :Exa
+000062f0: 6d70 6c65 3a20 0a0a 2020 2020 2e2e 2070  mple: ..    .. p
+00006300: 6c6f 743a 3a20 206d 6172 6769 6e5f 6772  lot::  margin_gr
+00006310: 6170 6873 5f65 7861 6d70 6c65 732f 6d67  aphs_examples/mg
+00006320: 5f65 785f 7363 5f64 6566 6561 742e 7079  _ex_sc_defeat.py
+00006330: 0a20 2020 2020 2020 203a 636f 6e74 6578  .        :contex
+00006340: 743a 2072 6573 6574 2020 0a20 2020 2020  t: reset  .     
+00006350: 2020 203a 696e 636c 7564 652d 736f 7572     :include-sour
+00006360: 6365 3a20 5472 7565 0a0a 2020 2020 2222  ce: True..    ""
+00006370: 220a 0a20 2020 2063 616e 6469 6461 7465  "..    candidate
+00006380: 7320 3d20 6564 6174 612e 6361 6e64 6964  s = edata.candid
+00006390: 6174 6573 2069 6620 6375 7272 5f63 616e  ates if curr_can
+000063a0: 6473 2069 7320 4e6f 6e65 2065 6c73 6520  ds is None else 
+000063b0: 6375 7272 5f63 616e 6473 2020 2020 0a20  curr_cands    . 
+000063c0: 2020 2073 7472 656e 6774 685f 6675 6e63     strength_func
+000063d0: 7469 6f6e 203d 2065 6461 7461 2e6d 6172  tion = edata.mar
+000063e0: 6769 6e20 6966 2073 7472 656e 6774 685f  gin if strength_
+000063f0: 6675 6e63 7469 6f6e 2069 7320 4e6f 6e65  function is None
+00006400: 2065 6c73 6520 7374 7265 6e67 7468 5f66   else strength_f
+00006410: 756e 6374 696f 6e20 0a20 0a20 2020 2077  unction . .    w
+00006420: 6561 6b5f 636f 6e64 6f72 6365 745f 7769  eak_condorcet_wi
+00006430: 6e6e 6572 7320 3d20 7b63 3a54 7275 6520  nners = {c:True 
+00006440: 666f 7220 6320 696e 2063 616e 6469 6461  for c in candida
+00006450: 7465 737d 0a20 2020 2073 5f6d 6174 7269  tes}.    s_matri
+00006460: 7820 3d20 5b5b 2d6e 702e 696e 6620 666f  x = [[-np.inf fo
+00006470: 7220 5f20 696e 2063 616e 6469 6461 7465  r _ in candidate
+00006480: 735d 2066 6f72 205f 2069 6e20 6361 6e64  s] for _ in cand
+00006490: 6964 6174 6573 5d0a 2020 2020 0a20 2020  idates].    .   
+000064a0: 2023 2069 6e69 7469 616c 697a 6520 7468   # initialize th
+000064b0: 6520 735f 6d61 7472 6978 0a20 2020 2066  e s_matrix.    f
+000064c0: 6f72 2063 315f 6964 782c 2063 3120 696e  or c1_idx, c1 in
+000064d0: 2065 6e75 6d65 7261 7465 2863 616e 6469   enumerate(candi
+000064e0: 6461 7465 7329 3a0a 2020 2020 2020 2020  dates):.        
+000064f0: 666f 7220 6332 5f69 6478 2c20 6332 2069  for c2_idx, c2 i
+00006500: 6e20 656e 756d 6572 6174 6528 6361 6e64  n enumerate(cand
+00006510: 6964 6174 6573 293a 0a20 2020 2020 2020  idates):.       
+00006520: 2020 2020 2069 6620 2865 6461 7461 2e6d       if (edata.m
+00006530: 616a 6f72 6974 795f 7072 6566 6572 7328  ajority_prefers(
+00006540: 6331 2c20 6332 2920 6f72 2063 3120 3d3d  c1, c2) or c1 ==
+00006550: 2063 3229 3a0a 2020 2020 2020 2020 2020   c2):.          
+00006560: 2020 2020 2020 735f 6d61 7472 6978 5b63        s_matrix[c
+00006570: 315f 6964 785d 5b63 325f 6964 785d 203d  1_idx][c2_idx] =
+00006580: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
+00006590: 6f6e 2863 312c 2063 3229 200a 2020 2020  on(c1, c2) .    
+000065a0: 2020 2020 2020 2020 2020 2020 7765 616b              weak
+000065b0: 5f63 6f6e 646f 7263 6574 5f77 696e 6e65  _condorcet_winne
+000065c0: 7273 5b63 325d 203d 2077 6561 6b5f 636f  rs[c2] = weak_co
+000065d0: 6e64 6f72 6365 745f 7769 6e6e 6572 735b  ndorcet_winners[
+000065e0: 6332 5d20 616e 6420 2863 3120 3d3d 2063  c2] and (c1 == c
+000065f0: 3229 2023 2077 6561 6b20 436f 6e64 6f72  2) # weak Condor
+00006600: 6365 7420 7769 6e6e 6572 7320 6172 6520  cet winners are 
+00006610: 5370 6c69 7420 4379 636c 6520 7769 6e6e  Split Cycle winn
+00006620: 6572 730a 2020 2020 0a20 2020 2073 7472  ers.    .    str
+00006630: 656e 6774 6820 3d20 6c69 7374 286d 6170  ength = list(map
+00006640: 286c 616d 6264 6120 6920 3a20 6c69 7374  (lambda i : list
+00006650: 286d 6170 286c 616d 6264 6120 6a20 3a20  (map(lambda j : 
+00006660: 6a20 2c20 6929 2920 2c20 735f 6d61 7472  j , i)) , s_matr
+00006670: 6978 2929 0a20 2020 2066 6f72 2069 5f69  ix)).    for i_i
+00006680: 6478 2c20 6920 696e 2065 6e75 6d65 7261  dx, i in enumera
+00006690: 7465 2863 616e 6469 6461 7465 7329 3a20  te(candidates): 
+000066a0: 0a20 2020 2020 2020 2066 6f72 206a 5f69  .        for j_i
+000066b0: 6478 2c20 6a20 696e 2065 6e75 6d65 7261  dx, j in enumera
+000066c0: 7465 2863 616e 6469 6461 7465 7329 3a0a  te(candidates):.
+000066d0: 2020 2020 2020 2020 2020 2020 6966 2069              if i
+000066e0: 213d 206a 3a0a 2020 2020 2020 2020 2020  != j:.          
+000066f0: 2020 2020 2020 6966 206e 6f74 2077 6561        if not wea
+00006700: 6b5f 636f 6e64 6f72 6365 745f 7769 6e6e  k_condorcet_winn
+00006710: 6572 735b 6a5d 3a20 2320 7765 616b 2043  ers[j]: # weak C
+00006720: 6f6e 646f 7263 6574 2077 696e 6e65 7273  ondorcet winners
+00006730: 2061 7265 2053 706c 6974 2043 7963 6c65   are Split Cycle
+00006740: 2077 696e 6e65 7273 0a20 2020 2020 2020   winners.       
+00006750: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+00006760: 206b 5f69 6478 2c20 6b20 696e 2065 6e75   k_idx, k in enu
+00006770: 6d65 7261 7465 2863 616e 6469 6461 7465  merate(candidate
+00006780: 7329 3a20 0a20 2020 2020 2020 2020 2020  s): .           
+00006790: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+000067a0: 6920 213d 206b 2061 6e64 206a 2021 3d20  i != k and j != 
+000067b0: 6b3a 0a20 2020 2020 2020 2020 2020 2020  k:.             
+000067c0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000067d0: 7472 656e 6774 685b 6a5f 6964 785d 5b6b  trength[j_idx][k
+000067e0: 5f69 6478 5d20 3d20 6d61 7828 7374 7265  _idx] = max(stre
+000067f0: 6e67 7468 5b6a 5f69 6478 5d5b 6b5f 6964  ngth[j_idx][k_id
+00006800: 785d 2c20 6d69 6e28 7374 7265 6e67 7468  x], min(strength
+00006810: 5b6a 5f69 6478 5d5b 695f 6964 785d 2c73  [j_idx][i_idx],s
+00006820: 7472 656e 6774 685b 695f 6964 785d 5b6b  trength[i_idx][k
+00006830: 5f69 6478 5d29 290a 200a 2020 2020 6465  _idx])). .    de
+00006840: 6665 6174 5f67 7261 7068 203d 206e 782e  feat_graph = nx.
+00006850: 4469 4772 6170 6828 290a 2020 2020 6465  DiGraph().    de
+00006860: 6665 6174 5f67 7261 7068 2e61 6464 5f6e  feat_graph.add_n
+00006870: 6f64 6573 5f66 726f 6d28 6361 6e64 6964  odes_from(candid
+00006880: 6174 6573 290a 0a20 2020 2066 6f72 2069  ates)..    for i
+00006890: 5f69 6478 2c20 6920 696e 2065 6e75 6d65  _idx, i in enume
+000068a0: 7261 7465 2863 616e 6469 6461 7465 7329  rate(candidates)
+000068b0: 3a0a 2020 2020 2020 2020 666f 7220 6a5f  :.        for j_
+000068c0: 6964 782c 206a 2069 6e20 656e 756d 6572  idx, j in enumer
+000068d0: 6174 6528 6361 6e64 6964 6174 6573 293a  ate(candidates):
+000068e0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+000068f0: 6920 213d 206a 3a0a 2020 2020 2020 2020  i != j:.        
+00006900: 2020 2020 2020 2020 6966 2073 5f6d 6174          if s_mat
+00006910: 7269 785b 6a5f 6964 785d 5b69 5f69 6478  rix[j_idx][i_idx
+00006920: 5d20 3e20 7374 7265 6e67 7468 5b69 5f69  ] > strength[i_i
+00006930: 6478 5d5b 6a5f 6964 785d 3a20 2320 7468  dx][j_idx]: # th
+00006940: 6520 6d61 696e 2064 6966 6665 7265 6e63  e main differenc
+00006950: 6520 7769 7468 2042 6561 7420 5061 7468  e with Beat Path
+00006960: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006970: 2020 2020 2064 6566 6561 745f 6772 6170       defeat_grap
+00006980: 682e 6164 645f 7765 6967 6874 6564 5f65  h.add_weighted_e
+00006990: 6467 6573 5f66 726f 6d28 5b28 6a2c 692c  dges_from([(j,i,
+000069a0: 735f 6d61 7472 6978 5b6a 5f69 6478 5d5b  s_matrix[j_idx][
+000069b0: 695f 6964 785d 295d 290a 2020 2020 2020  i_idx])]).      
+000069c0: 2020 2020 2020 2020 2020 0a20 2020 2072            .    r
+000069d0: 6574 7572 6e20 6465 6665 6174 5f67 7261  eturn defeat_gra
+000069e0: 7068 0a0a 0a23 2066 6c61 7474 656e 2061  ph...# flatten a
+000069f0: 2032 6420 6c69 7374 202d 2074 7572 6e20   2d list - turn 
+00006a00: 6120 3264 206c 6973 7420 696e 746f 2061  a 2d list into a
+00006a10: 2073 696e 676c 6520 6c69 7374 206f 6620   single list of 
+00006a20: 6974 656d 730a 666c 6174 7465 6e20 3d20  items.flatten = 
+00006a30: 6c61 6d62 6461 206c 3a20 5b69 7465 6d20  lambda l: [item 
+00006a40: 666f 7220 7375 626c 6973 7420 696e 206c  for sublist in l
+00006a50: 2066 6f72 2069 7465 6d20 696e 2073 7562   for item in sub
+00006a60: 6c69 7374 5d0a 0a64 6566 2064 6f65 735f  list]..def does_
+00006a70: 6372 6561 7465 5f63 7963 6c65 2867 2c20  create_cycle(g, 
+00006a80: 6564 6765 293a 0a20 2020 2027 2727 7265  edge):.    '''re
+00006a90: 7475 726e 2054 7275 6520 6966 2061 6464  turn True if add
+00006aa0: 696e 6720 7468 6520 6564 6765 2074 6f20  ing the edge to 
+00006ab0: 6720 6372 6561 7465 2061 2063 7963 6c65  g create a cycle
+00006ac0: 2e0a 2020 2020 6974 2069 7320 6173 7375  ..    it is assu
+00006ad0: 6d65 6420 7468 6174 2065 6467 6520 6973  med that edge is
+00006ae0: 2061 6c72 6561 6479 2069 6e20 6727 2727   already in g'''
+00006af0: 0a20 2020 2073 6f75 7263 6520 3d20 6564  .    source = ed
+00006b00: 6765 5b30 5d0a 2020 2020 7461 7267 6574  ge[0].    target
+00006b10: 203d 2065 6467 655b 315d 0a20 2020 2066   = edge[1].    f
+00006b20: 6f72 206e 2069 6e20 672e 7072 6564 6563  or n in g.predec
+00006b30: 6573 736f 7273 2873 6f75 7263 6529 3a0a  essors(source):.
+00006b40: 2020 2020 2020 2020 6966 206e 782e 6861          if nx.ha
+00006b50: 735f 7061 7468 2867 2c20 7461 7267 6574  s_path(g, target
+00006b60: 2c20 6e29 3a20 0a20 2020 2020 2020 2020  , n): .         
+00006b70: 2020 2072 6574 7572 6e20 5472 7565 0a20     return True. 
+00006b80: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
+00006b90: 0a0a 0a64 6566 2070 6f77 6572 7365 7428  ...def powerset(
+00006ba0: 6974 6572 6162 6c65 293a 0a20 2020 2022  iterable):.    "
+00006bb0: 2222 0a20 2020 2052 6574 7572 6e20 7468  "".    Return th
+00006bc0: 6520 706f 7765 7273 6574 206f 6620 6060  e powerset of ``
+00006bd0: 6974 6572 6162 6c65 6060 0a0a 2020 2020  iterable``..    
+00006be0: 706f 7765 7273 6574 285b 312c 322c 335d  powerset([1,2,3]
+00006bf0: 2920 2d2d 3e20 2829 2028 312c 2920 2832  ) --> () (1,) (2
+00006c00: 2c29 2028 332c 2920 2831 2c32 2920 2831  ,) (3,) (1,2) (1
+00006c10: 2c33 2920 2832 2c33 2920 2831 2c32 2c33  ,3) (2,3) (1,2,3
+00006c20: 290a 2020 2020 2222 220a 2020 2020 7320  ).    """.    s 
+00006c30: 3d20 6c69 7374 2869 7465 7261 626c 6529  = list(iterable)
+00006c40: 0a20 2020 2072 6574 7572 6e20 6368 6169  .    return chai
+00006c50: 6e2e 6672 6f6d 5f69 7465 7261 626c 6528  n.from_iterable(
+00006c60: 636f 6d62 696e 6174 696f 6e73 2873 2c20  combinations(s, 
+00006c70: 7229 2066 6f72 2072 2069 6e20 7261 6e67  r) for r in rang
+00006c80: 6528 6c65 6e28 7329 2b31 2929 0a0a 0a64  e(len(s)+1))...d
+00006c90: 6566 2069 735f 7374 6163 6b28 6564 6174  ef is_stack(edat
+00006ca0: 612c 2063 616e 645f 6c69 7374 2c20 6375  a, cand_list, cu
+00006cb0: 7272 5f63 616e 6473 3d4e 6f6e 6529 3a20  rr_cands=None): 
+00006cc0: 0a20 2020 2022 2222 0a20 2020 2041 202a  .    """.    A *
+00006cd0: 2a73 7461 636b 2a2a 2069 7320 6120 6c69  *stack** is a li
+00006ce0: 6e65 6172 206f 7264 6572 203a 6d61 7468  near order :math
+00006cf0: 3a60 4c60 206f 6e20 7468 6520 6361 6e64  :`L` on the cand
+00006d00: 6964 6174 6520 7375 6368 2074 6861 7420  idate such that 
+00006d10: 666f 7220 616c 6c20 6361 6e64 6964 6174  for all candidat
+00006d20: 6573 203a 6d61 7468 3a60 6160 2061 6e64  es :math:`a` and
+00006d30: 203a 6d61 7468 3a60 6260 2c20 6966 203a   :math:`b`, if :
+00006d40: 6d61 7468 3a60 614c 6260 2c20 7468 656e  math:`aLb`, then
+00006d50: 2074 6865 7265 2061 7265 2064 6973 7469   there are disti
+00006d60: 6e63 7420 6361 6e64 6964 6174 6573 203a  nct candidates :
+00006d70: 6d61 7468 3a60 785f 312c 5c64 6f74 732c  math:`x_1,\dots,
+00006d80: 785f 6e60 2077 6974 6820 3a6d 6174 683a  x_n` with :math:
+00006d90: 6078 5f31 3d61 6020 616e 6420 3a6d 6174  `x_1=a` and :mat
+00006da0: 683a 6078 5f6e 3d62 6020 7375 6368 2074  h:`x_n=b` such t
+00006db0: 6861 7420 3a6d 6174 683a 6078 5f69 204c  hat :math:`x_i L
+00006dc0: 2078 5f7b 692b 317d 6020 616e 6420 666f   x_{i+1}` and fo
+00006dd0: 7220 616c 6c20 3a6d 6174 683a 6069 5c69  r all :math:`i\i
+00006de0: 6e20 5c7b 312c 5c64 6f74 732c 206e 2d31  n \{1,\dots, n-1
+00006df0: 5c7d 602c 2074 6865 206d 6172 6769 6e20  \}`, the margin 
+00006e00: 6f66 203a 6d61 7468 3a60 785f 3160 206f  of :math:`x_1` o
+00006e10: 7665 7220 3a6d 6174 683a 6078 5f7b 692b  ver :math:`x_{i+
+00006e20: 317d 6020 6973 2067 7265 6174 6572 2074  1}` is greater t
+00006e30: 6861 6e20 6f72 2065 7175 616c 2074 6f20  han or equal to 
+00006e40: 7468 6520 6d61 7267 696e 206f 6620 3a6d  the margin of :m
+00006e50: 6174 683a 6062 6020 6f76 6572 203a 6d61  ath:`b` over :ma
+00006e60: 7468 3a60 6160 2e0a 0a20 2020 2054 6869  th:`a`...    Thi
+00006e70: 7320 6465 6669 6e69 7469 6f6e 2069 7320  s definition is 
+00006e80: 6475 6520 746f 205a 6176 6973 7420 616e  due to Zavist an
+00006e90: 6420 5469 6465 6d61 6e20 3139 3839 2c20  d Tideman 1989, 
+00006ea0: 616e 6420 6973 2075 7365 6420 6173 2061  and is used as a
+00006eb0: 6e20 616c 7465 726e 6174 6976 6520 6368  n alternative ch
+00006ec0: 6172 6163 7465 7269 7a61 7469 6f6e 206f  aracterization o
+00006ed0: 6620 5261 6e6b 6564 2050 6169 7273 3a20  f Ranked Pairs: 
+00006ee0: 3a6d 6174 683a 6061 6020 6973 2061 2052  :math:`a` is a R
+00006ef0: 616e 6b65 6420 5061 6972 7320 7769 6e6e  anked Pairs winn
+00006f00: 6572 2069 6620 616e 6420 6f6e 6c79 2069  er if and only i
+00006f10: 6620 3a6d 6174 683a 6061 6020 6973 2074  f :math:`a` is t
+00006f20: 6865 206d 6178 696d 756d 2065 6c65 6d65  he maximum eleme
+00006f30: 6e74 206f 6620 736f 6d65 2073 7461 636b  nt of some stack
+00006f40: 2e20 0a0a 2020 2020 4172 6773 3a0a 2020  . ..    Args:.  
+00006f50: 2020 2020 2020 6564 6174 6120 2850 726f        edata (Pro
+00006f60: 6669 6c65 2c20 5072 6f66 696c 6557 6974  file, ProfileWit
+00006f70: 6854 6965 732c 204d 6172 6769 6e47 7261  hTies, MarginGra
+00006f80: 7068 293a 2041 6e79 2065 6c65 6374 696f  ph): Any electio
+00006f90: 6e20 6461 7461 2074 6861 7420 6861 7320  n data that has 
+00006fa0: 6120 606d 6172 6769 6e60 206d 6574 686f  a `margin` metho
+00006fb0: 642e 200a 2020 2020 2020 2020 6361 6e64  d. .        cand
+00006fc0: 5f6c 6973 7420 286c 6973 7429 3a20 5468  _list (list): Th
+00006fd0: 6520 6c69 7374 206f 6620 6361 6e64 6964  e list of candid
+00006fe0: 6174 6573 2074 6861 7420 6d61 7920 6265  ates that may be
+00006ff0: 2061 2073 7461 636b 0a20 2020 2020 2020   a stack.       
+00007000: 2063 7572 725f 6361 6e64 7320 284c 6973   curr_cands (Lis
+00007010: 745b 696e 745d 2c20 6f70 7469 6f6e 616c  t[int], optional
+00007020: 293a 2049 6620 7365 742c 2074 6865 6e20  ): If set, then 
+00007030: 6669 6e64 2074 6865 2077 696e 6e65 7273  find the winners
+00007040: 2066 6f72 2074 6865 2070 726f 6669 6c65   for the profile
+00007050: 2072 6573 7472 6963 7465 6420 746f 2074   restricted to t
+00007060: 6865 2063 616e 6469 6461 7465 7320 696e  he candidates in
+00007070: 2060 6063 7572 725f 6361 6e64 7360 600a   ``curr_cands``.
+00007080: 0a20 2020 2052 6574 7572 6e73 3a20 0a20  .    Returns: . 
+00007090: 2020 2020 2020 2054 7275 6520 6966 2060         True if `
+000070a0: 6063 616e 645f 6c69 7374 6060 2069 7320  `cand_list`` is 
+000070b0: 6120 7374 6163 6b20 616e 6420 4661 6c73  a stack and Fals
+000070c0: 6520 6f74 6865 7277 6973 650a 0a20 2020  e otherwise..   
+000070d0: 203a 4578 616d 706c 653a 200a 2020 2020   :Example: .    
+000070e0: 0a20 2020 202e 2e20 706c 6f74 3a3a 2020  .    .. plot::  
+000070f0: 6d61 7267 696e 5f67 7261 7068 735f 6578  margin_graphs_ex
+00007100: 616d 706c 6573 2f6d 675f 6578 5f72 705f  amples/mg_ex_rp_
+00007110: 7374 6163 6b73 2e70 790a 2020 2020 2020  stacks.py.      
+00007120: 2020 3a63 6f6e 7465 7874 3a20 7265 7365    :context: rese
+00007130: 7420 200a 2020 2020 2020 2020 3a69 6e63  t  .        :inc
+00007140: 6c75 6465 2d73 6f75 7263 653a 2054 7275  lude-source: Tru
+00007150: 650a 0a0a 2020 2020 2e2e 2065 7865 635f  e...    .. exec_
+00007160: 636f 6465 3a3a 0a20 2020 2020 2020 200a  code::.        .
+00007170: 2020 2020 2020 2020 6672 6f6d 2070 7265          from pre
+00007180: 665f 766f 7469 6e67 2e77 6569 6768 7465  f_voting.weighte
+00007190: 645f 6d61 6a6f 7269 7479 5f67 7261 7068  d_majority_graph
+000071a0: 7320 696d 706f 7274 204d 6172 6769 6e47  s import MarginG
+000071b0: 7261 7068 0a20 2020 2020 2020 2066 726f  raph.        fro
+000071c0: 6d20 7072 6566 5f76 6f74 696e 672e 6d61  m pref_voting.ma
+000071d0: 7267 696e 5f62 6173 6564 5f6d 6574 686f  rgin_based_metho
+000071e0: 6473 2069 6d70 6f72 7420 6973 5f73 7461  ds import is_sta
+000071f0: 636b 0a20 2020 2020 2020 2066 726f 6d20  ck.        from 
+00007200: 6974 6572 746f 6f6c 7320 696d 706f 7274  itertools import
+00007210: 2070 6572 6d75 7461 7469 6f6e 730a 2020   permutations.  
+00007220: 2020 2020 2020 0a20 2020 2020 2020 206d        .        m
+00007230: 6720 3d20 4d61 7267 696e 4772 6170 6828  g = MarginGraph(
+00007240: 5b30 2c20 312c 2032 5d2c 205b 2830 2c20  [0, 1, 2], [(0, 
+00007250: 312c 2032 292c 2028 312c 2032 2c20 3429  1, 2), (1, 2, 4)
+00007260: 2c20 2832 2c20 302c 2032 295d 290a 2020  , (2, 0, 2)]).  
+00007270: 2020 2020 2020 0a20 2020 2020 2020 2066        .        f
+00007280: 6f72 2063 6c69 7374 2069 6e20 7065 726d  or clist in perm
+00007290: 7574 6174 696f 6e73 286d 672e 6361 6e64  utations(mg.cand
+000072a0: 6964 6174 6573 293a 200a 2020 2020 2020  idates): .      
+000072b0: 2020 2020 2020 7072 696e 7428 6622 7b63        print(f"{c
+000072c0: 6c69 7374 7d20 7b27 6973 2720 6966 2069  list} {'is' if i
+000072d0: 735f 7374 6163 6b28 6d67 2c20 636c 6973  s_stack(mg, clis
+000072e0: 7429 2065 6c73 6520 2769 7320 6e6f 7427  t) else 'is not'
+000072f0: 7d20 6120 7374 6163 6b22 290a 2020 2020  } a stack").    
+00007300: 2020 2020 2020 2020 0a20 2020 2022 2222          .    """
+00007310: 0a20 2020 200a 2020 2020 6361 6e64 6964  .    .    candid
+00007320: 6174 6573 203d 2063 7572 725f 6361 6e64  ates = curr_cand
+00007330: 7320 6966 2063 7572 725f 6361 6e64 7320  s if curr_cands 
+00007340: 6973 206e 6f74 204e 6f6e 6520 656c 7365  is not None else
+00007350: 2065 6461 7461 2e63 616e 6469 6461 7465   edata.candidate
+00007360: 730a 2020 2020 6361 6e64 5f70 6169 7273  s.    cand_pairs
+00007370: 203d 205b 2861 2c20 6229 2069 6620 6361   = [(a, b) if ca
+00007380: 6e64 5f6c 6973 742e 696e 6465 7828 6129  nd_list.index(a)
+00007390: 203c 2063 616e 645f 6c69 7374 2e69 6e64   < cand_list.ind
+000073a0: 6578 2862 2920 656c 7365 2028 622c 2061  ex(b) else (b, a
+000073b0: 2920 666f 7220 612c 2062 2069 6e20 636f  ) for a, b in co
+000073c0: 6d62 696e 6174 696f 6e73 2863 616e 6469  mbinations(candi
+000073d0: 6461 7465 732c 2032 295d 0a20 2020 2020  dates, 2)].     
+000073e0: 2020 200a 2020 2020 666f 7220 612c 2062     .    for a, b
+000073f0: 2069 6e20 6361 6e64 5f70 6169 7273 3a0a   in cand_pairs:.
+00007400: 2020 2020 2020 2020 6f74 6865 725f 6361          other_ca
+00007410: 6e64 7320 3d20 5b63 2066 6f72 2063 2069  nds = [c for c i
+00007420: 6e20 6361 6e64 6964 6174 6573 2069 6620  n candidates if 
+00007430: 6320 213d 2061 2061 6e64 2063 2021 3d20  c != a and c != 
+00007440: 625d 0a20 2020 2020 2020 2066 6f75 6e64  b].        found
+00007450: 5f70 6174 6820 3d20 4661 6c73 650a 2020  _path = False.  
+00007460: 2020 2020 2020 0a20 2020 2020 2020 2073        .        s
+00007470: 7562 6c69 7374 203d 2063 616e 645f 6c69  ublist = cand_li
+00007480: 7374 5b63 616e 645f 6c69 7374 2e69 6e64  st[cand_list.ind
+00007490: 6578 2861 2920 2b20 313a 6361 6e64 5f6c  ex(a) + 1:cand_l
+000074a0: 6973 742e 696e 6465 7828 6229 5d0a 2020  ist.index(b)].  
+000074b0: 2020 2020 2020 0a20 2020 2020 2020 2066        .        f
+000074c0: 6f72 2069 6e64 6963 6573 2069 6e20 706f  or indices in po
+000074d0: 7765 7273 6574 2872 616e 6765 286c 656e  werset(range(len
+000074e0: 2873 7562 6c69 7374 2929 293a 200a 2020  (sublist))): .  
+000074f0: 2020 2020 2020 2020 2020 0a20 2020 2020            .     
+00007500: 2020 2020 2020 2070 6174 6820 3d20 5b61         path = [a
+00007510: 5d20 2b20 5b73 7562 6c69 7374 5b69 5d20  ] + [sublist[i] 
+00007520: 666f 7220 6920 696e 2073 6f72 7465 6428  for i in sorted(
+00007530: 696e 6469 6365 7329 5d20 2b20 5b62 5d0a  indices)] + [b].
+00007540: 2020 2020 2020 2020 2020 2020 6d61 7267              marg
+00007550: 696e 7320 3d20 5b65 6461 7461 2e6d 6172  ins = [edata.mar
+00007560: 6769 6e28 7869 2c20 7061 7468 5b69 202b  gin(xi, path[i +
+00007570: 2031 5d29 2066 6f72 2069 2c20 7869 2069   1]) for i, xi i
+00007580: 6e20 656e 756d 6572 6174 6528 7061 7468  n enumerate(path
+00007590: 5b30 3a2d 315d 295d 0a20 2020 2020 2020  [0:-1])].       
+000075a0: 2020 2020 2069 6620 616c 6c28 5b63 616e       if all([can
+000075b0: 645f 6c69 7374 2e69 6e64 6578 2878 6929  d_list.index(xi)
+000075c0: 203c 2063 616e 645f 6c69 7374 2e69 6e64   < cand_list.ind
+000075d0: 6578 2870 6174 685b 692b 315d 2920 666f  ex(path[i+1]) fo
+000075e0: 7220 692c 2078 6920 696e 2065 6e75 6d65  r i, xi in enume
+000075f0: 7261 7465 2870 6174 685b 303a 2d31 5d29  rate(path[0:-1])
+00007600: 5d29 2061 6e64 2061 6c6c 285b 6d20 3e3d  ]) and all([m >=
+00007610: 2065 6461 7461 2e6d 6172 6769 6e28 622c   edata.margin(b,
+00007620: 2061 2920 666f 7220 6d20 696e 206d 6172   a) for m in mar
+00007630: 6769 6e73 5d29 3a20 0a20 2020 2020 2020  gins]): .       
+00007640: 2020 2020 2020 2020 2066 6f75 6e64 5f70           found_p
+00007650: 6174 6820 3d20 5472 7565 0a20 2020 2020  ath = True.     
+00007660: 2020 2020 2020 2020 2020 2062 7265 616b             break
+00007670: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+00007680: 666f 756e 645f 7061 7468 3a20 0a20 2020  found_path: .   
+00007690: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+000076a0: 4661 6c73 650a 2020 2020 7265 7475 726e  False.    return
+000076b0: 2054 7275 650a 0a64 6566 205f 7261 6e6b   True..def _rank
+000076c0: 6564 5f70 6169 7273 5f66 726f 6d5f 7374  ed_pairs_from_st
+000076d0: 6163 6b73 2865 6461 7461 2c20 6375 7272  acks(edata, curr
+000076e0: 5f63 616e 6473 203d 204e 6f6e 6529 3a20  _cands = None): 
+000076f0: 0a20 2020 2022 2222 4669 6e64 2074 6865  .    """Find the
+00007700: 2052 616e 6b65 6420 5061 6972 7320 7769   Ranked Pairs wi
+00007710: 6e6e 6572 7320 6279 2069 7465 7261 7469  nners by iterati
+00007720: 6e67 206f 7665 7220 616c 6c20 7065 726d  ng over all perm
+00007730: 7574 6174 696f 6e73 206f 6620 6361 6e64  utations of cand
+00007740: 6964 6174 6573 2028 7265 7374 7269 6374  idates (restrict
+00007750: 6564 2074 6f20 6060 6375 7272 5f63 616e  ed to ``curr_can
+00007760: 6473 6060 2069 6620 6e6f 7420 4e6f 6e65  ds`` if not None
+00007770: 292c 2061 6e64 2063 6865 636b 696e 6720  ), and checking 
+00007780: 6966 2074 6865 206c 6973 7420 6973 2061  if the list is a
+00007790: 2073 7461 636b 2e20 0a0a 2020 2020 4172   stack. ..    Ar
+000077a0: 6773 3a0a 2020 2020 2020 2020 6564 6174  gs:.        edat
+000077b0: 6120 2850 726f 6669 6c65 2c20 5072 6f66  a (Profile, Prof
+000077c0: 696c 6557 6974 6854 6965 732c 204d 6172  ileWithTies, Mar
+000077d0: 6769 6e47 7261 7068 293a 2041 6e79 2065  ginGraph): Any e
+000077e0: 6c65 6374 696f 6e20 6461 7461 2074 6861  lection data tha
+000077f0: 7420 6861 7320 6120 606d 6172 6769 6e60  t has a `margin`
+00007800: 206d 6574 686f 642e 200a 2020 2020 2020   method. .      
+00007810: 2020 6375 7272 5f63 616e 6473 2028 4c69    curr_cands (Li
+00007820: 7374 5b69 6e74 5d2c 206f 7074 696f 6e61  st[int], optiona
+00007830: 6c29 3a20 4966 2073 6574 2c20 7468 656e  l): If set, then
+00007840: 2066 696e 6420 7468 6520 7769 6e6e 6572   find the winner
+00007850: 7320 666f 7220 7468 6520 7072 6f66 696c  s for the profil
+00007860: 6520 7265 7374 7269 6374 6564 2074 6f20  e restricted to 
+00007870: 7468 6520 6361 6e64 6964 6174 6573 2069  the candidates i
+00007880: 6e20 6060 6375 7272 5f63 616e 6473 6060  n ``curr_cands``
+00007890: 0a0a 2020 2020 5265 7475 726e 733a 200a  ..    Returns: .
+000078a0: 2020 2020 2020 2020 4120 736f 7274 6564          A sorted
+000078b0: 206c 6973 7420 6f66 2063 616e 6469 6461   list of candida
+000078c0: 7465 732e 200a 0a20 2020 202e 2e20 7365  tes. ..    .. se
+000078d0: 6561 6c73 6f3a 3a0a 2020 2020 2020 2020  ealso::.        
+000078e0: 0a20 2020 2020 2020 203a 6d65 7468 3a60  .        :meth:`
+000078f0: 7072 6566 5f76 6f74 696e 672e 6d61 7267  pref_voting.marg
+00007900: 696e 5f62 6173 6564 5f6d 6574 686f 6473  in_based_methods
+00007910: 2e69 735f 7374 6163 6b60 0a0a 0a20 2020  .is_stack`...   
+00007920: 2022 2222 2020 2020 0a0a 2020 2020 6361   """    ..    ca
+00007930: 6e64 6964 6174 6573 203d 2063 7572 725f  ndidates = curr_
+00007940: 6361 6e64 7320 6966 2063 7572 725f 6361  cands if curr_ca
+00007950: 6e64 7320 6973 206e 6f74 204e 6f6e 6520  nds is not None 
+00007960: 656c 7365 2065 6461 7461 2e63 616e 6469  else edata.candi
+00007970: 6461 7465 730a 2020 2020 7769 6e6e 6572  dates.    winner
+00007980: 7320 3d20 6c69 7374 2829 0a20 2020 2066  s = list().    f
+00007990: 6f72 2063 6c69 7374 2069 6e20 7065 726d  or clist in perm
+000079a0: 7574 6174 696f 6e73 2863 616e 6469 6461  utations(candida
+000079b0: 7465 7329 3a20 0a20 2020 2020 2020 2069  tes): .        i
+000079c0: 7373 7461 636b 203d 2069 735f 7374 6163  sstack = is_stac
+000079d0: 6b28 6564 6174 612c 2063 6c69 7374 2c20  k(edata, clist, 
+000079e0: 6375 7272 5f63 616e 6473 203d 2063 7572  curr_cands = cur
+000079f0: 725f 6361 6e64 7329 0a20 2020 2020 2020  r_cands).       
+00007a00: 2069 6620 6973 7374 6163 6b3a 200a 2020   if isstack: .  
+00007a10: 2020 2020 2020 2020 2020 7769 6e6e 6572            winner
+00007a20: 732e 6170 7065 6e64 2863 6c69 7374 5b30  s.append(clist[0
+00007a30: 5d29 0a20 2020 2020 2020 2020 2020 200a  ]).            .
+00007a40: 2020 2020 7265 7475 726e 2073 6f72 7465      return sorte
+00007a50: 6428 6c69 7374 2873 6574 2877 696e 6e65  d(list(set(winne
+00007a60: 7273 2929 290a 0a64 6566 205f 7261 6e6b  rs)))..def _rank
+00007a70: 6564 5f70 6169 7273 5f62 6173 6963 280a  ed_pairs_basic(.
+00007a80: 2020 2020 6564 6174 612c 200a 2020 2020      edata, .    
+00007a90: 6375 7272 5f63 616e 6473 203d 204e 6f6e  curr_cands = Non
+00007aa0: 652c 200a 2020 2020 7374 7265 6e67 7468  e, .    strength
+00007ab0: 5f66 756e 6374 696f 6e20 3d20 4e6f 6e65  _function = None
+00007ac0: 293a 2020 200a 2020 2020 2222 2241 6e20  ):   .    """An 
+00007ad0: 696d 706c 656d 656e 7461 7469 6f6e 206f  implementation o
+00007ae0: 6620 5261 6e6b 6564 2050 6169 7273 2074  f Ranked Pairs t
+00007af0: 6861 7420 7573 6573 2061 2062 6173 6963  hat uses a basic
+00007b00: 2061 6c67 6f72 6974 686d 2e20 0a0a 2020   algorithm. ..  
+00007b10: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
+00007b20: 6564 6174 6120 2850 726f 6669 6c65 2c20  edata (Profile, 
+00007b30: 5072 6f66 696c 6557 6974 6854 6965 732c  ProfileWithTies,
+00007b40: 204d 6172 6769 6e47 7261 7068 293a 2041   MarginGraph): A
+00007b50: 6e79 2065 6c65 6374 696f 6e20 6461 7461  ny election data
+00007b60: 2074 6861 7420 6861 7320 6120 606d 6172   that has a `mar
+00007b70: 6769 6e60 206d 6574 686f 642e 200a 2020  gin` method. .  
+00007b80: 2020 2020 2020 6375 7272 5f63 616e 6473        curr_cands
+00007b90: 2028 4c69 7374 5b69 6e74 5d2c 206f 7074   (List[int], opt
+00007ba0: 696f 6e61 6c29 3a20 4966 2073 6574 2c20  ional): If set, 
+00007bb0: 7468 656e 2066 696e 6420 7468 6520 7769  then find the wi
+00007bc0: 6e6e 6572 7320 666f 7220 7468 6520 7072  nners for the pr
+00007bd0: 6f66 696c 6520 7265 7374 7269 6374 6564  ofile restricted
+00007be0: 2074 6f20 7468 6520 6361 6e64 6964 6174   to the candidat
+00007bf0: 6573 2069 6e20 6060 6375 7272 5f63 616e  es in ``curr_can
+00007c00: 6473 6060 0a0a 2020 2020 5265 7475 726e  ds``..    Return
+00007c10: 733a 200a 2020 2020 2020 2020 4120 736f  s: .        A so
+00007c20: 7274 6564 206c 6973 7420 6f66 2063 616e  rted list of can
+00007c30: 6469 6461 7465 732e 200a 0a20 2020 2022  didates. ..    "
+00007c40: 2222 0a20 2020 2063 616e 6469 6461 7465  "".    candidate
+00007c50: 7320 3d20 6564 6174 612e 6361 6e64 6964  s = edata.candid
+00007c60: 6174 6573 2069 6620 6375 7272 5f63 616e  ates if curr_can
+00007c70: 6473 2069 7320 4e6f 6e65 2065 6c73 6520  ds is None else 
+00007c80: 6375 7272 5f63 616e 6473 200a 2020 2020  curr_cands .    
+00007c90: 6369 6478 5f74 6f5f 6361 6e64 203d 207b  cidx_to_cand = {
+00007ca0: 6369 6478 3a20 6320 666f 7220 6369 6478  cidx: c for cidx
+00007cb0: 2c20 6320 696e 2065 6e75 6d65 7261 7465  , c in enumerate
+00007cc0: 2863 616e 6469 6461 7465 7329 7d20 200a  (candidates)}  .
+00007cd0: 2020 2020 6361 6e64 5f74 6f5f 6369 6478      cand_to_cidx
+00007ce0: 203d 207b 633a 2063 6964 7820 666f 7220   = {c: cidx for 
+00007cf0: 6369 6478 2c20 6320 696e 2065 6e75 6d65  cidx, c in enume
+00007d00: 7261 7465 2863 616e 6469 6461 7465 7329  rate(candidates)
+00007d10: 7d20 200a 2020 2020 7374 7265 6e67 7468  }  .    strength
+00007d20: 5f66 756e 6374 696f 6e20 3d20 6564 6174  _function = edat
+00007d30: 612e 6d61 7267 696e 2069 6620 7374 7265  a.margin if stre
+00007d40: 6e67 7468 5f66 756e 6374 696f 6e20 6973  ngth_function is
+00007d50: 204e 6f6e 6520 656c 7365 2073 7472 656e   None else stren
+00007d60: 6774 685f 6675 6e63 7469 6f6e 2020 2020  gth_function    
+00007d70: 0a0a 2020 2020 6377 203d 2065 6461 7461  ..    cw = edata
+00007d80: 2e63 6f6e 646f 7263 6574 5f77 696e 6e65  .condorcet_winne
+00007d90: 7228 6375 7272 5f63 616e 6473 3d63 7572  r(curr_cands=cur
+00007da0: 725f 6361 6e64 7329 0a20 2020 2023 2052  r_cands).    # R
+00007db0: 616e 6b65 6420 5061 6972 7320 6973 2043  anked Pairs is C
+00007dc0: 6f6e 646f 7263 6574 2063 6f6e 7369 7374  ondorcet consist
+00007dd0: 656e 742c 2073 6f20 7369 6d70 6c79 2072  ent, so simply r
+00007de0: 6574 7572 6e20 7468 6520 436f 6e64 6f72  eturn the Condor
+00007df0: 6365 7420 7769 6e6e 6572 2069 6620 6578  cet winner if ex
+00007e00: 6973 7473 0a20 2020 2069 6620 6377 2069  ists.    if cw i
+00007e10: 7320 6e6f 7420 4e6f 6e65 3a20 0a20 2020  s not None: .   
+00007e20: 2020 2020 2077 696e 6e65 7273 203d 205b       winners = [
+00007e30: 6377 5d0a 2020 2020 656c 7365 3a0a 2020  cw].    else:.  
+00007e40: 2020 2020 2020 775f 6564 6765 7320 3d20        w_edges = 
+00007e50: 5b28 6331 2c20 6332 2c20 7374 7265 6e67  [(c1, c2, streng
+00007e60: 7468 5f66 756e 6374 696f 6e28 6331 2c20  th_function(c1, 
+00007e70: 6332 2929 2066 6f72 2063 3120 696e 2063  c2)) for c1 in c
+00007e80: 616e 6469 6461 7465 7320 666f 7220 6332  andidates for c2
+00007e90: 2069 6e20 6361 6e64 6964 6174 6573 200a   in candidates .
+00007ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007eb0: 2020 2069 6620 6331 2021 3d20 6332 2061     if c1 != c2 a
+00007ec0: 6e64 2028 6564 6174 612e 6d61 6a6f 7269  nd (edata.majori
+00007ed0: 7479 5f70 7265 6665 7273 2863 312c 2063  ty_prefers(c1, c
+00007ee0: 3229 206f 7220 6564 6174 612e 6973 5f74  2) or edata.is_t
+00007ef0: 6965 6428 6331 2c20 6332 2929 5d0a 2020  ied(c1, c2))].  
+00007f00: 2020 2020 2020 7769 6e6e 6572 7320 3d20        winners = 
+00007f10: 6c69 7374 2829 2020 200a 2020 2020 2020  list()   .      
+00007f20: 2020 6966 206c 656e 2877 5f65 6467 6573    if len(w_edges
+00007f30: 2920 3e20 303a 2020 2020 2020 2020 2020  ) > 0:          
+00007f40: 0a20 2020 2020 2020 2020 2020 2073 7472  .            str
+00007f50: 656e 6774 6873 203d 2073 6f72 7465 6428  engths = sorted(
+00007f60: 6c69 7374 2873 6574 285b 655b 325d 2066  list(set([e[2] f
+00007f70: 6f72 2065 2069 6e20 775f 6564 6765 735d  or e in w_edges]
+00007f80: 2929 2c20 7265 7665 7273 653d 5472 7565  )), reverse=True
+00007f90: 290a 2020 2020 2020 2020 2020 2020 736f  ).            so
+00007fa0: 7274 6564 5f65 6467 6573 203d 205b 5b65  rted_edges = [[e
+00007fb0: 2066 6f72 2065 2069 6e20 775f 6564 6765   for e in w_edge
+00007fc0: 7320 6966 2065 5b32 5d20 3d3d 2073 5d20  s if e[2] == s] 
+00007fd0: 666f 7220 7320 696e 2073 7472 656e 6774  for s in strengt
+00007fe0: 6873 5d0a 2020 2020 2020 2020 2020 2020  hs].            
+00007ff0: 7462 7320 3d20 7072 6f64 7563 7428 2a5b  tbs = product(*[
+00008000: 7065 726d 7574 6174 696f 6e73 2865 6467  permutations(edg
+00008010: 6573 2920 666f 7220 6564 6765 7320 696e  es) for edges in
+00008020: 2073 6f72 7465 645f 6564 6765 735d 290a   sorted_edges]).
+00008030: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00008040: 7462 2069 6e20 7462 733a 0a20 2020 2020  tb in tbs:.     
+00008050: 2020 2020 2020 2020 2020 2065 6467 6573             edges
+00008060: 203d 2066 6c61 7474 656e 2874 6229 0a20   = flatten(tb). 
+00008070: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00008080: 705f 6465 6665 6174 203d 2053 504f 286c  p_defeat = SPO(l
+00008090: 656e 2863 616e 6469 6461 7465 7329 290a  en(candidates)).
+000080a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000080b0: 666f 7220 6530 2c65 312c 7320 696e 2065  for e0,e1,s in e
+000080c0: 6467 6573 3a20 0a20 2020 2020 2020 2020  dges: .         
+000080d0: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
+000080e0: 7420 7270 5f64 6566 6561 742e 505b 6361  t rp_defeat.P[ca
+000080f0: 6e64 5f74 6f5f 6369 6478 5b65 315d 5d5b  nd_to_cidx[e1]][
+00008100: 6361 6e64 5f74 6f5f 6369 6478 5b65 305d  cand_to_cidx[e0]
+00008110: 5d3a 0a20 2020 2020 2020 2020 2020 2020  ]:.             
+00008120: 2020 2020 2020 2020 2020 2072 705f 6465             rp_de
+00008130: 6665 6174 2e61 6464 2863 616e 645f 746f  feat.add(cand_to
+00008140: 5f63 6964 785b 6530 5d2c 6361 6e64 5f74  _cidx[e0],cand_t
+00008150: 6f5f 6369 6478 5b65 315d 290a 2020 2020  o_cidx[e1]).    
+00008160: 2020 2020 2020 2020 2020 2020 7769 6e6e              winn
+00008170: 6572 732e 6170 7065 6e64 2863 6964 785f  ers.append(cidx_
+00008180: 746f 5f63 616e 645b 7270 5f64 6566 6561  to_cand[rp_defea
+00008190: 742e 696e 6974 6961 6c5f 656c 656d 656e  t.initial_elemen
+000081a0: 7473 2829 5b30 5d5d 290a 2020 2020 2020  ts()[0]]).      
+000081b0: 2020 656c 7365 3a20 0a20 2020 2020 2020    else: .       
+000081c0: 2020 2020 2077 696e 6e65 7273 203d 2063       winners = c
+000081d0: 616e 6469 6461 7465 730a 2020 2020 7265  andidates.    re
+000081e0: 7475 726e 2073 6f72 7465 6428 6c69 7374  turn sorted(list
+000081f0: 2873 6574 2877 696e 6e65 7273 2929 290a  (set(winners))).
+00008200: 0a0a 7270 5f70 726f 7065 7274 6965 7320  ..rp_properties 
+00008210: 3d20 566f 7469 6e67 4d65 7468 6f64 5072  = VotingMethodPr
+00008220: 6f70 6572 7469 6573 280a 2020 2020 636f  operties(.    co
+00008230: 6e64 6f72 6365 745f 7769 6e6e 6572 3d54  ndorcet_winner=T
+00008240: 7275 652c 200a 2020 2020 636f 6e64 6f72  rue, .    condor
+00008250: 6365 745f 6c6f 7365 723d 5472 7565 2c0a  cet_loser=True,.
+00008260: 2020 2020 7061 7265 746f 5f64 6f6d 696e      pareto_domin
+00008270: 616e 6365 3d54 7275 652c 0a20 2020 2070  ance=True,.    p
+00008280: 6f73 6974 6976 655f 696e 766f 6c76 656d  ositive_involvem
+00008290: 656e 743d 4661 6c73 652c 200a 2020 2020  ent=False, .    
+000082a0: 290a 4076 6d28 6e61 6d65 3d22 5261 6e6b  ).@vm(name="Rank
+000082b0: 6564 2050 6169 7273 222c 0a20 2020 2070  ed Pairs",.    p
+000082c0: 726f 7065 7274 6965 733d 7270 5f70 726f  roperties=rp_pro
+000082d0: 7065 7274 6965 732c 0a20 2020 2069 6e70  perties,.    inp
+000082e0: 7574 5f74 7970 6573 3d5b 456c 6563 7469  ut_types=[Electi
+000082f0: 6f6e 5479 7065 732e 5052 4f46 494c 452c  onTypes.PROFILE,
+00008300: 2045 6c65 6374 696f 6e54 7970 6573 2e50   ElectionTypes.P
+00008310: 524f 4649 4c45 5f57 4954 485f 5449 4553  ROFILE_WITH_TIES
+00008320: 2c20 456c 6563 7469 6f6e 5479 7065 732e  , ElectionTypes.
+00008330: 4d41 5247 494e 5f47 5241 5048 5d29 0a64  MARGIN_GRAPH]).d
+00008340: 6566 2072 616e 6b65 645f 7061 6972 7328  ef ranked_pairs(
+00008350: 0a20 2020 2065 6461 7461 2c20 0a20 2020  .    edata, .   
+00008360: 2063 7572 725f 6361 6e64 733d 4e6f 6e65   curr_cands=None
+00008370: 2c20 0a20 2020 2073 7472 656e 6774 685f  , .    strength_
+00008380: 6675 6e63 7469 6f6e 3d4e 6f6e 652c 200a  function=None, .
+00008390: 2020 2020 616c 676f 7269 7468 6d3d 2762      algorithm='b
+000083a0: 6173 6963 2729 3a20 2020 0a20 2020 2022  asic'):   .    "
+000083b0: 2222 0a20 2020 204f 7264 6572 2074 6865  "".    Order the
+000083c0: 2065 6467 6573 2069 6e20 7468 6520 6d61   edges in the ma
+000083d0: 7267 696e 2067 7261 7068 2066 726f 6d20  rgin graph from 
+000083e0: 6c61 7267 6573 7420 746f 2073 6d61 6c6c  largest to small
+000083f0: 6573 7420 616e 6420 6c6f 636b 2074 6865  est and lock the
+00008400: 6d20 696e 2069 6e20 7468 6174 206f 7264  m in in that ord
+00008410: 6572 2c20 736b 6970 7069 6e67 2065 6467  er, skipping edg
+00008420: 6573 2074 6861 7420 6372 6561 7465 2061  es that create a
+00008430: 2063 7963 6c65 2e20 2049 6620 7468 6572   cycle.  If ther
+00008440: 6520 6172 6520 7469 6573 2069 6e20 7468  e are ties in th
+00008450: 6520 6d61 7267 696e 732c 2062 7265 616b  e margins, break
+00008460: 2074 6865 2074 6965 7320 7573 696e 6720   the ties using 
+00008470: 6120 7469 652d 6272 6561 6b69 6e67 2072  a tie-breaking r
+00008480: 756c 653a 2061 206c 696e 6561 7220 6f72  ule: a linear or
+00008490: 6465 7269 6e67 206f 7665 7220 7468 6520  dering over the 
+000084a0: 6564 6765 732e 2020 2041 2063 616e 6469  edges.   A candi
+000084b0: 6461 7465 2069 7320 6120 5261 6e6b 6564  date is a Ranked
+000084c0: 2050 6169 7273 2077 696e 6e65 7220 6966   Pairs winner if
+000084d0: 2069 7420 7769 6e73 2061 6363 6f72 6469   it wins accordi
+000084e0: 6e67 2074 6f20 736f 6d65 2074 6965 2d62  ng to some tie-b
+000084f0: 7265 616b 696e 6720 7275 6c65 2e20 416c  reaking rule. Al
+00008500: 736f 206b 6e6f 776e 2061 7320 5469 6465  so known as Tide
+00008510: 6d61 6e27 7320 5275 6c65 2e0a 0a20 2020  man's Rule...   
+00008520: 202e 2e20 7761 726e 696e 673a 3a20 0a20   .. warning:: . 
+00008530: 2020 2020 2020 2054 6869 7320 6d65 7468         This meth
+00008540: 6f64 2063 616e 2074 616b 6520 6120 7665  od can take a ve
+00008550: 7279 206c 6f6e 6720 7469 6d65 2074 6f20  ry long time to 
+00008560: 6669 6e64 2077 696e 6e65 7273 2e20 0a20  find winners. . 
+00008570: 2020 2020 2020 200a 2020 2020 4172 6773         .    Args
+00008580: 3a0a 2020 2020 2020 2020 6564 6174 6120  :.        edata 
+00008590: 2850 726f 6669 6c65 2c20 5072 6f66 696c  (Profile, Profil
+000085a0: 6557 6974 6854 6965 732c 204d 6172 6769  eWithTies, Margi
+000085b0: 6e47 7261 7068 293a 2041 6e79 2065 6c65  nGraph): Any ele
+000085c0: 6374 696f 6e20 6461 7461 2074 6861 7420  ction data that 
+000085d0: 6861 7320 6120 606d 6172 6769 6e60 206d  has a `margin` m
+000085e0: 6574 686f 642e 200a 2020 2020 2020 2020  ethod. .        
+000085f0: 6375 7272 5f63 616e 6473 2028 4c69 7374  curr_cands (List
+00008600: 5b69 6e74 5d2c 206f 7074 696f 6e61 6c29  [int], optional)
+00008610: 3a20 4966 2073 6574 2c20 7468 656e 2066  : If set, then f
+00008620: 696e 6420 7468 6520 7769 6e6e 6572 7320  ind the winners 
+00008630: 666f 7220 7468 6520 7072 6f66 696c 6520  for the profile 
+00008640: 7265 7374 7269 6374 6564 2074 6f20 7468  restricted to th
+00008650: 6520 6361 6e64 6964 6174 6573 2069 6e20  e candidates in 
+00008660: 6060 6375 7272 5f63 616e 6473 6060 0a20  ``curr_cands``. 
+00008670: 2020 2020 2020 2073 7472 656e 6774 685f         strength_
+00008680: 6675 6e63 7469 6f6e 2028 6675 6e63 7469  function (functi
+00008690: 6f6e 2c20 6f70 7469 6f6e 616c 293a 2054  on, optional): T
+000086a0: 6865 2073 7472 656e 6774 6820 6675 6e63  he strength func
+000086b0: 7469 6f6e 2074 6f20 6265 2075 7365 6420  tion to be used 
+000086c0: 746f 2063 616c 6375 6c61 7465 2074 6865  to calculate the
+000086d0: 2073 7472 656e 6774 6820 6f66 2061 2070   strength of a p
+000086e0: 6174 682e 2020 2054 6865 2064 6566 6175  ath.   The defau
+000086f0: 6c74 2069 7320 7468 6520 6d61 7267 696e  lt is the margin
+00008700: 206d 6574 686f 6420 6f66 2060 6065 6461   method of ``eda
+00008710: 7461 6060 2e20 2020 5468 6973 206f 6e6c  ta``.   This onl
+00008720: 7920 6d61 7474 6572 7320 7768 656e 2074  y matters when t
+00008730: 6865 2062 616c 6c6f 7473 2061 7265 206e  he ballots are n
+00008740: 6f74 206c 696e 6561 7220 6f72 6465 7273  ot linear orders
+00008750: 2e20 0a20 2020 2020 2020 2061 6c67 6f72  . .        algor
+00008760: 6974 686d 2028 7374 722c 206f 7074 696f  ithm (str, optio
+00008770: 6e61 6c29 3a20 5370 6563 6966 7920 7768  nal): Specify wh
+00008780: 6963 6820 616c 676f 7269 7468 6d20 746f  ich algorithm to
+00008790: 2075 7365 2e20 204f 7074 696f 6e73 2061   use.  Options a
+000087a0: 7265 2027 6261 7369 6327 2028 7468 6520  re 'basic' (the 
+000087b0: 6465 6661 756c 7429 2061 6e64 2027 6672  default) and 'fr
+000087c0: 6f6d 5f73 7461 636b 7327 2e0a 0a20 2020  om_stacks'...   
+000087d0: 2052 6574 7572 6e73 3a20 0a20 2020 2020   Returns: .     
+000087e0: 2020 2041 2073 6f72 7465 6420 6c69 7374     A sorted list
+000087f0: 206f 6620 6361 6e64 6964 6174 6573 2e20   of candidates. 
+00008800: 0a0a 2020 2020 2e2e 2073 6565 616c 736f  ..    .. seealso
+00008810: 3a3a 0a0a 2020 2020 2020 2020 3a6d 6574  ::..        :met
+00008820: 683a 6070 7265 665f 766f 7469 6e67 2e6d  h:`pref_voting.m
+00008830: 6172 6769 6e5f 6261 7365 645f 6d65 7468  argin_based_meth
+00008840: 6f64 732e 7261 6e6b 6564 5f70 6169 7273  ods.ranked_pairs
+00008850: 5f77 6974 685f 7465 7374 602c 203a 6d65  _with_test`, :me
+00008860: 7468 3a60 7072 6566 5f76 6f74 696e 672e  th:`pref_voting.
+00008870: 6d61 7267 696e 5f62 6173 6564 5f6d 6574  margin_based_met
+00008880: 686f 6473 2e72 616e 6b65 645f 7061 6972  hods.ranked_pair
+00008890: 735f 7a74 602c 203a 6d65 7468 3a60 7072  s_zt`, :meth:`pr
+000088a0: 6566 5f76 6f74 696e 672e 6d61 7267 696e  ef_voting.margin
+000088b0: 5f62 6173 6564 5f6d 6574 686f 6473 2e72  _based_methods.r
+000088c0: 616e 6b65 645f 7061 6972 735f 6465 6665  anked_pairs_defe
+000088d0: 6174 7360 0a0a 2020 2020 3a45 7861 6d70  ats`..    :Examp
+000088e0: 6c65 3a20 0a0a 2020 2020 2e2e 2070 6c6f  le: ..    .. plo
+000088f0: 743a 3a20 206d 6172 6769 6e5f 6772 6170  t::  margin_grap
+00008900: 6873 5f65 7861 6d70 6c65 732f 6d67 5f65  hs_examples/mg_e
+00008910: 785f 6270 5f72 702e 7079 0a20 2020 2020  x_bp_rp.py.     
+00008920: 2020 203a 636f 6e74 6578 743a 2072 6573     :context: res
+00008930: 6574 2020 0a20 2020 2020 2020 203a 696e  et  .        :in
+00008940: 636c 7564 652d 736f 7572 6365 3a20 5472  clude-source: Tr
+00008950: 7565 0a0a 0a20 2020 202e 2e20 636f 6465  ue...    .. code
+00008960: 2d62 6c6f 636b 3a3a 200a 0a20 2020 2020  -block:: ..     
+00008970: 2020 2066 726f 6d20 7072 6566 5f76 6f74     from pref_vot
+00008980: 696e 672e 6d61 7267 696e 5f62 6173 6564  ing.margin_based
+00008990: 5f6d 6574 686f 6473 2069 6d70 6f72 7420  _methods import 
+000089a0: 7261 6e6b 6564 5f70 6169 7273 0a0a 2020  ranked_pairs..  
+000089b0: 2020 2020 2020 7261 6e6b 6564 5f70 6169        ranked_pai
+000089c0: 7273 2e64 6973 706c 6179 286d 6729 0a20  rs.display(mg). 
+000089d0: 2020 2020 2020 2072 616e 6b65 645f 7061         ranked_pa
+000089e0: 6972 732e 6469 7370 6c61 7928 6d67 2c20  irs.display(mg, 
+000089f0: 616c 676f 7269 7468 6d3d 2762 6173 6963  algorithm='basic
+00008a00: 2729 200a 2020 2020 2020 2020 7261 6e6b  ') .        rank
+00008a10: 6564 5f70 6169 7273 2e64 6973 706c 6179  ed_pairs.display
+00008a20: 286d 672c 2061 6c67 6f72 6974 686d 3d27  (mg, algorithm='
+00008a30: 6672 6f6d 5f73 7461 636b 7327 2920 2020  from_stacks')   
+00008a40: 200a 0a0a 2020 2020 2e2e 2065 7865 635f   ...    .. exec_
+00008a50: 636f 6465 3a3a 200a 2020 2020 2020 2020  code:: .        
+00008a60: 3a68 6964 655f 636f 6465 3a0a 0a20 2020  :hide_code:..   
+00008a70: 2020 2020 2066 726f 6d20 7072 6566 5f76       from pref_v
+00008a80: 6f74 696e 672e 7765 6967 6874 6564 5f6d  oting.weighted_m
+00008a90: 616a 6f72 6974 795f 6772 6170 6873 2069  ajority_graphs i
+00008aa0: 6d70 6f72 7420 4d61 7267 696e 4772 6170  mport MarginGrap
+00008ab0: 680a 2020 2020 2020 2020 6672 6f6d 2070  h.        from p
+00008ac0: 7265 665f 766f 7469 6e67 2e6d 6172 6769  ref_voting.margi
+00008ad0: 6e5f 6261 7365 645f 6d65 7468 6f64 7320  n_based_methods 
+00008ae0: 696d 706f 7274 2072 616e 6b65 645f 7061  import ranked_pa
+00008af0: 6972 730a 2020 2020 2020 2020 0a20 2020  irs.        .   
+00008b00: 2020 2020 206d 6720 3d20 4d61 7267 696e       mg = Margin
+00008b10: 4772 6170 6828 5b30 2c20 312c 2032 2c20  Graph([0, 1, 2, 
+00008b20: 335d 2c20 5b28 302c 2032 2c20 3329 2c20  3], [(0, 2, 3), 
+00008b30: 2831 2c20 302c 2035 292c 2028 322c 2031  (1, 0, 5), (2, 1
+00008b40: 2c20 3529 2c20 2832 2c20 332c 2031 292c  , 5), (2, 3, 1),
+00008b50: 2028 332c 2030 2c20 3329 2c20 2833 2c20   (3, 0, 3), (3, 
+00008b60: 312c 2031 295d 290a 2020 2020 2020 2020  1, 1)]).        
+00008b70: 0a20 2020 2020 2020 2072 616e 6b65 645f  .        ranked_
+00008b80: 7061 6972 732e 6469 7370 6c61 7928 6d67  pairs.display(mg
+00008b90: 290a 2020 2020 2020 2020 7261 6e6b 6564  ).        ranked
+00008ba0: 5f70 6169 7273 2e64 6973 706c 6179 286d  _pairs.display(m
+00008bb0: 672c 2061 6c67 6f72 6974 686d 3d27 6261  g, algorithm='ba
+00008bc0: 7369 6327 290a 2020 2020 2020 2020 7261  sic').        ra
+00008bd0: 6e6b 6564 5f70 6169 7273 2e64 6973 706c  nked_pairs.displ
+00008be0: 6179 286d 672c 2061 6c67 6f72 6974 686d  ay(mg, algorithm
+00008bf0: 3d27 6672 6f6d 5f73 7461 636b 7327 290a  ='from_stacks').
+00008c00: 0a20 2020 2022 2222 0a0a 2020 2020 6966  .    """..    if
+00008c10: 2061 6c67 6f72 6974 686d 203d 3d20 2762   algorithm == 'b
+00008c20: 6173 6963 273a 0a20 2020 2020 2020 2072  asic':.        r
+00008c30: 6574 7572 6e20 5f72 616e 6b65 645f 7061  eturn _ranked_pa
+00008c40: 6972 735f 6261 7369 6328 6564 6174 612c  irs_basic(edata,
+00008c50: 2063 7572 725f 6361 6e64 7320 3d20 6375   curr_cands = cu
+00008c60: 7272 5f63 616e 6473 2c20 7374 7265 6e67  rr_cands, streng
+00008c70: 7468 5f66 756e 6374 696f 6e20 3d20 7374  th_function = st
+00008c80: 7265 6e67 7468 5f66 756e 6374 696f 6e29  rength_function)
+00008c90: 0a20 2020 2065 6c69 6620 616c 676f 7269  .    elif algori
+00008ca0: 7468 6d20 3d3d 2027 6672 6f6d 5f73 7461  thm == 'from_sta
+00008cb0: 636b 7327 3a0a 2020 2020 2020 2020 7265  cks':.        re
+00008cc0: 7475 726e 205f 7261 6e6b 6564 5f70 6169  turn _ranked_pai
+00008cd0: 7273 5f66 726f 6d5f 7374 6163 6b73 2865  rs_from_stacks(e
+00008ce0: 6461 7461 2c20 6375 7272 5f63 616e 6473  data, curr_cands
+00008cf0: 203d 2063 7572 725f 6361 6e64 7329 0a20   = curr_cands). 
+00008d00: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00008d10: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
+00008d20: 7228 2249 6e76 616c 6964 2061 6c67 6f72  r("Invalid algor
+00008d30: 6974 686d 2073 7065 6369 6669 6564 2e22  ithm specified."
+00008d40: 290a 0a40 766d 286e 616d 653d 2252 616e  )..@vm(name="Ran
+00008d50: 6b65 6420 5061 6972 7322 2c0a 2020 2020  ked Pairs",.    
+00008d60: 736b 6970 5f72 6567 6973 7472 6174 696f  skip_registratio
+00008d70: 6e3d 5472 7565 290a 6465 6620 7261 6e6b  n=True).def rank
+00008d80: 6564 5f70 6169 7273 5f77 6974 685f 7465  ed_pairs_with_te
+00008d90: 7374 280a 2020 2020 6564 6174 612c 200a  st(.    edata, .
+00008da0: 2020 2020 6375 7272 5f63 616e 6473 3d4e      curr_cands=N
+00008db0: 6f6e 652c 200a 2020 2020 7374 7265 6e67  one, .    streng
+00008dc0: 7468 5f66 756e 6374 696f 6e3d 4e6f 6e65  th_function=None
+00008dd0: 293a 2020 200a 2020 2020 2222 2246 696e  ):   .    """Fin
+00008de0: 6420 7468 6520 5261 6e6b 6564 2050 6169  d the Ranked Pai
+00008df0: 7273 2077 696e 6e65 7273 2c20 6275 7420  rs winners, but 
+00008e00: 696e 636c 7564 6520 6120 7465 7374 2074  include a test t
+00008e10: 6f20 6465 7465 726d 696e 6564 2069 6620  o determined if 
+00008e20: 6974 2077 696c 6c20 7461 6b65 2074 6f6f  it will take too
+00008e30: 206c 6f6e 6720 746f 2063 6f6d 7075 7465   long to compute
+00008e40: 2074 6865 2052 616e 6b65 6420 5061 6972   the Ranked Pair
+00008e50: 7320 7769 6e6e 6572 732e 2049 6620 7468  s winners. If th
+00008e60: 6520 6361 6c63 756c 6174 696f 6e20 6f66  e calculation of
+00008e70: 2074 6865 2077 696e 6e65 7273 2077 696c   the winners wil
+00008e80: 6c20 7461 6b65 2074 6f6f 206c 6f6e 672c  l take too long,
+00008e90: 2072 6574 7572 6e20 4e6f 6e65 2e0a 0a20   return None... 
+00008ea0: 2020 202e 2e20 696d 706f 7274 616e 743a     .. important:
+00008eb0: 3a0a 2020 2020 2020 2020 5468 6973 2076  :.        This v
+00008ec0: 6f74 696e 6720 6d65 7468 6f64 2074 6861  oting method tha
+00008ed0: 7420 6d69 6768 7420 7265 7475 726e 204e  t might return N
+00008ee0: 6f6e 6520 7261 7468 6572 2074 6861 6e20  one rather than 
+00008ef0: 6120 6c69 7374 206f 6620 6361 6e64 6964  a list of candid
+00008f00: 6174 6573 2e20 200a 0a20 2020 2041 7267  ates.  ..    Arg
+00008f10: 733a 0a20 2020 2020 2020 2065 6461 7461  s:.        edata
+00008f20: 2028 5072 6f66 696c 652c 2050 726f 6669   (Profile, Profi
+00008f30: 6c65 5769 7468 5469 6573 2c20 4d61 7267  leWithTies, Marg
+00008f40: 696e 4772 6170 6829 3a20 416e 7920 656c  inGraph): Any el
+00008f50: 6563 7469 6f6e 2064 6174 6120 7468 6174  ection data that
+00008f60: 2068 6173 2061 2060 6d61 7267 696e 6020   has a `margin` 
+00008f70: 6d65 7468 6f64 2e20 0a20 2020 2020 2020  method. .       
+00008f80: 2063 7572 725f 6361 6e64 7320 284c 6973   curr_cands (Lis
+00008f90: 745b 696e 745d 2c20 6f70 7469 6f6e 616c  t[int], optional
+00008fa0: 293a 2049 6620 7365 742c 2074 6865 6e20  ): If set, then 
+00008fb0: 6669 6e64 2074 6865 2077 696e 6e65 7273  find the winners
+00008fc0: 2066 6f72 2074 6865 2070 726f 6669 6c65   for the profile
+00008fd0: 2072 6573 7472 6963 7465 6420 746f 2074   restricted to t
+00008fe0: 6865 2063 616e 6469 6461 7465 7320 696e  he candidates in
+00008ff0: 2060 6063 7572 725f 6361 6e64 7360 600a   ``curr_cands``.
+00009000: 2020 2020 2020 2020 7374 7265 6e67 7468          strength
+00009010: 5f66 756e 6374 696f 6e20 2866 756e 6374  _function (funct
+00009020: 696f 6e2c 206f 7074 696f 6e61 6c29 3a20  ion, optional): 
+00009030: 5468 6520 7374 7265 6e67 7468 2066 756e  The strength fun
+00009040: 6374 696f 6e20 746f 2062 6520 7573 6564  ction to be used
+00009050: 2074 6f20 6361 6c63 756c 6174 6520 7468   to calculate th
+00009060: 6520 7374 7265 6e67 7468 206f 6620 6120  e strength of a 
+00009070: 7061 7468 2e20 2020 5468 6520 6465 6661  path.   The defa
+00009080: 756c 7420 6973 2074 6865 206d 6172 6769  ult is the margi
+00009090: 6e20 6d65 7468 6f64 206f 6620 6060 6564  n method of ``ed
+000090a0: 6174 6160 602e 2020 2054 6869 7320 6f6e  ata``.   This on
+000090b0: 6c79 206d 6174 7465 7273 2077 6865 6e20  ly matters when 
+000090c0: 7468 6520 6261 6c6c 6f74 7320 6172 6520  the ballots are 
+000090d0: 6e6f 7420 6c69 6e65 6172 206f 7264 6572  not linear order
+000090e0: 732e 200a 0a20 2020 2052 6574 7572 6e73  s. ..    Returns
+000090f0: 3a20 0a20 2020 2020 2020 2041 2073 6f72  : .        A sor
+00009100: 7465 6420 6c69 7374 206f 6620 6361 6e64  ted list of cand
+00009110: 6964 6174 6573 2e20 0a0a 2020 2020 2e2e  idates. ..    ..
+00009120: 2073 6565 616c 736f 3a3a 0a0a 2020 2020   seealso::..    
+00009130: 2020 2020 3a6d 6574 683a 6070 7265 665f      :meth:`pref_
+00009140: 766f 7469 6e67 2e6d 6172 6769 6e5f 6261  voting.margin_ba
+00009150: 7365 645f 6d65 7468 6f64 732e 7261 6e6b  sed_methods.rank
+00009160: 6564 5f70 6169 7273 5f77 6974 685f 7465  ed_pairs_with_te
+00009170: 7374 602c 203a 6d65 7468 3a60 7072 6566  st`, :meth:`pref
+00009180: 5f76 6f74 696e 672e 6d61 7267 696e 5f62  _voting.margin_b
+00009190: 6173 6564 5f6d 6574 686f 6473 2e72 616e  ased_methods.ran
+000091a0: 6b65 645f 7061 6972 735f 7a74 602c 203a  ked_pairs_zt`, :
+000091b0: 6d65 7468 3a60 7072 6566 5f76 6f74 696e  meth:`pref_votin
+000091c0: 672e 6d61 7267 696e 5f62 6173 6564 5f6d  g.margin_based_m
+000091d0: 6574 686f 6473 2e72 616e 6b65 645f 7061  ethods.ranked_pa
+000091e0: 6972 735f 6465 6665 6174 7360 0a0a 2020  irs_defeats`..  
+000091f0: 2020 3a45 7861 6d70 6c65 3a20 0a0a 2020    :Example: ..  
+00009200: 2020 2e2e 2070 6c6f 743a 3a20 206d 6172    .. plot::  mar
+00009210: 6769 6e5f 6772 6170 6873 5f65 7861 6d70  gin_graphs_examp
+00009220: 6c65 732f 6d67 5f65 785f 7270 5f77 6974  les/mg_ex_rp_wit
+00009230: 685f 7465 7374 2e70 790a 2020 2020 2020  h_test.py.      
+00009240: 2020 3a63 6f6e 7465 7874 3a20 7265 7365    :context: rese
+00009250: 7420 200a 2020 2020 2020 2020 3a69 6e63  t  .        :inc
+00009260: 6c75 6465 2d73 6f75 7263 653a 2054 7275  lude-source: Tru
+00009270: 650a 0a0a 2020 2020 2e2e 2063 6f64 652d  e...    .. code-
+00009280: 626c 6f63 6b3a 3a20 0a0a 2020 2020 2020  block:: ..      
+00009290: 2020 6672 6f6d 2070 7265 665f 766f 7469    from pref_voti
+000092a0: 6e67 2e6d 6172 6769 6e5f 6261 7365 645f  ng.margin_based_
+000092b0: 6d65 7468 6f64 7320 696d 706f 7274 2072  methods import r
+000092c0: 616e 6b65 645f 7061 6972 735f 7769 7468  anked_pairs_with
+000092d0: 5f74 6573 740a 0a20 2020 2020 2020 2072  _test..        r
+000092e0: 616e 6b65 645f 7061 6972 735f 7769 7468  anked_pairs_with
+000092f0: 5f74 6573 742e 6469 7370 6c61 7928 6d67  _test.display(mg
+00009300: 290a 0a0a 2020 2020 2e2e 2065 7865 635f  )...    .. exec_
+00009310: 636f 6465 3a3a 200a 2020 2020 2020 2020  code:: .        
+00009320: 3a68 6964 655f 636f 6465 3a0a 0a20 2020  :hide_code:..   
+00009330: 2020 2020 2066 726f 6d20 7072 6566 5f76       from pref_v
+00009340: 6f74 696e 672e 7765 6967 6874 6564 5f6d  oting.weighted_m
+00009350: 616a 6f72 6974 795f 6772 6170 6873 2069  ajority_graphs i
+00009360: 6d70 6f72 7420 4d61 7267 696e 4772 6170  mport MarginGrap
+00009370: 680a 2020 2020 2020 2020 6672 6f6d 2070  h.        from p
+00009380: 7265 665f 766f 7469 6e67 2e6d 6172 6769  ref_voting.margi
+00009390: 6e5f 6261 7365 645f 6d65 7468 6f64 7320  n_based_methods 
+000093a0: 696d 706f 7274 2072 616e 6b65 645f 7061  import ranked_pa
+000093b0: 6972 735f 7769 7468 5f74 6573 740a 2020  irs_with_test.  
+000093c0: 2020 2020 2020 0a20 2020 2020 2020 206d        .        m
+000093d0: 6720 3d20 4d61 7267 696e 4772 6170 6828  g = MarginGraph(
+000093e0: 5b30 2c20 312c 2032 2c20 335d 2c20 5b28  [0, 1, 2, 3], [(
+000093f0: 312c 2032 2c20 3229 2c20 2831 2c20 332c  1, 2, 2), (1, 3,
+00009400: 2032 292c 2028 322c 2030 2c20 3229 5d29   2), (2, 0, 2)])
+00009410: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00009420: 2020 7261 6e6b 6564 5f70 6169 7273 5f77    ranked_pairs_w
+00009430: 6974 685f 7465 7374 2e64 6973 706c 6179  ith_test.display
+00009440: 286d 6729 0a0a 0a20 2020 2022 2222 2020  (mg)...    """  
+00009450: 2020 0a20 2020 2063 616e 6469 6461 7465    .    candidate
+00009460: 7320 3d20 6564 6174 612e 6361 6e64 6964  s = edata.candid
+00009470: 6174 6573 2069 6620 6375 7272 5f63 616e  ates if curr_can
+00009480: 6473 2069 7320 4e6f 6e65 2065 6c73 6520  ds is None else 
+00009490: 6375 7272 5f63 616e 6473 2020 2020 0a20  curr_cands    . 
+000094a0: 2020 2063 6964 785f 746f 5f63 616e 6420     cidx_to_cand 
+000094b0: 3d20 7b63 6964 783a 2063 2066 6f72 2063  = {cidx: c for c
+000094c0: 6964 782c 2063 2069 6e20 656e 756d 6572  idx, c in enumer
+000094d0: 6174 6528 6361 6e64 6964 6174 6573 297d  ate(candidates)}
+000094e0: 2020 0a20 2020 2063 616e 645f 746f 5f63    .    cand_to_c
+000094f0: 6964 7820 3d20 7b63 3a20 6369 6478 2066  idx = {c: cidx f
+00009500: 6f72 2063 6964 782c 2063 2069 6e20 656e  or cidx, c in en
+00009510: 756d 6572 6174 6528 6361 6e64 6964 6174  umerate(candidat
+00009520: 6573 297d 2020 0a20 2020 200a 2020 2020  es)}  .    .    
+00009530: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
+00009540: 6e20 3d20 6564 6174 612e 6d61 7267 696e  n = edata.margin
+00009550: 2069 6620 7374 7265 6e67 7468 5f66 756e   if strength_fun
+00009560: 6374 696f 6e20 6973 204e 6f6e 6520 656c  ction is None el
+00009570: 7365 2073 7472 656e 6774 685f 6675 6e63  se strength_func
+00009580: 7469 6f6e 2020 200a 0a20 2020 2063 7720  tion   ..    cw 
+00009590: 3d20 6564 6174 612e 636f 6e64 6f72 6365  = edata.condorce
+000095a0: 745f 7769 6e6e 6572 2863 7572 725f 6361  t_winner(curr_ca
+000095b0: 6e64 7320 3d20 6375 7272 5f63 616e 6473  nds = curr_cands
+000095c0: 290a 2020 2020 2320 5261 6e6b 6564 2050  ).    # Ranked P
+000095d0: 6169 7273 2069 7320 436f 6e64 6f72 6365  airs is Condorce
+000095e0: 7420 636f 6e73 6973 7465 6e74 2c20 736f  t consistent, so
+000095f0: 2073 696d 706c 7920 7265 7475 726e 2074   simply return t
+00009600: 6865 2043 6f6e 646f 7263 6574 2077 696e  he Condorcet win
+00009610: 6e65 7220 6966 2065 7869 7374 730a 2020  ner if exists.  
+00009620: 2020 6966 2063 7720 6973 206e 6f74 204e    if cw is not N
+00009630: 6f6e 653a 200a 2020 2020 2020 2020 7769  one: .        wi
+00009640: 6e6e 6572 7320 3d20 5b63 775d 0a20 2020  nners = [cw].   
+00009650: 2065 6c73 653a 0a20 2020 2020 2020 2077   else:.        w
+00009660: 5f65 6467 6573 203d 205b 2863 312c 2063  _edges = [(c1, c
+00009670: 322c 2073 7472 656e 6774 685f 6675 6e63  2, strength_func
+00009680: 7469 6f6e 2863 312c 2063 3229 2920 666f  tion(c1, c2)) fo
+00009690: 7220 6331 2069 6e20 6361 6e64 6964 6174  r c1 in candidat
+000096a0: 6573 2066 6f72 2063 3220 696e 2063 616e  es for c2 in can
+000096b0: 6469 6461 7465 7320 0a20 2020 2020 2020  didates .       
+000096c0: 2020 2020 2020 2020 2020 2020 6966 2063              if c
+000096d0: 3120 213d 2063 3220 616e 6420 2865 6461  1 != c2 and (eda
+000096e0: 7461 2e6d 616a 6f72 6974 795f 7072 6566  ta.majority_pref
+000096f0: 6572 7328 6331 2c20 6332 2920 6f72 2065  ers(c1, c2) or e
+00009700: 6461 7461 2e69 735f 7469 6564 2863 312c  data.is_tied(c1,
+00009710: 2063 3229 295d 0a20 2020 2020 2020 2077   c2))].        w
+00009720: 696e 6e65 7273 203d 206c 6973 7428 2920  inners = list() 
+00009730: 2020 2020 2020 2020 2020 200a 2020 2020             .    
+00009740: 2020 2020 7374 7265 6e67 7468 7320 3d20      strengths = 
+00009750: 736f 7274 6564 286c 6973 7428 7365 7428  sorted(list(set(
+00009760: 5b65 5b32 5d20 666f 7220 6520 696e 2077  [e[2] for e in w
+00009770: 5f65 6467 6573 5d29 292c 2072 6576 6572  _edges])), rever
+00009780: 7365 3d54 7275 6529 0a20 2020 2020 2020  se=True).       
+00009790: 2073 6f72 7465 645f 6564 6765 7320 3d20   sorted_edges = 
+000097a0: 5b5b 6520 666f 7220 6520 696e 2077 5f65  [[e for e in w_e
+000097b0: 6467 6573 2069 6620 655b 325d 203d 3d20  dges if e[2] == 
+000097c0: 735d 2066 6f72 2073 2069 6e20 7374 7265  s] for s in stre
+000097d0: 6e67 7468 735d 0a20 2020 2020 2020 2069  ngths].        i
+000097e0: 6620 6e70 2e70 726f 6428 5b6d 6174 682e  f np.prod([math.
+000097f0: 6661 6374 6f72 6961 6c28 6c65 6e28 6573  factorial(len(es
+00009800: 2929 2066 6f72 2065 7320 696e 2073 6f72  )) for es in sor
+00009810: 7465 645f 6564 6765 735d 2920 3e20 3330  ted_edges]) > 30
+00009820: 3030 3a20 0a20 2020 2020 2020 2020 2020  00: .           
+00009830: 2072 6574 7572 6e20 4e6f 6e65 0a20 2020   return None.   
+00009840: 2020 2020 2065 6c73 653a 200a 2020 2020       else: .    
+00009850: 2020 2020 2020 2020 7462 7320 3d20 7072          tbs = pr
+00009860: 6f64 7563 7428 2a5b 7065 726d 7574 6174  oduct(*[permutat
+00009870: 696f 6e73 2865 6467 6573 2920 666f 7220  ions(edges) for 
+00009880: 6564 6765 7320 696e 2073 6f72 7465 645f  edges in sorted_
+00009890: 6564 6765 735d 290a 2020 2020 2020 2020  edges]).        
+000098a0: 2020 2020 666f 7220 7462 2069 6e20 7462      for tb in tb
+000098b0: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
+000098c0: 2020 2065 6467 6573 203d 2066 6c61 7474     edges = flatt
+000098d0: 656e 2874 6229 0a20 2020 2020 2020 2020  en(tb).         
+000098e0: 2020 2020 2020 2072 705f 6465 6665 6174         rp_defeat
+000098f0: 203d 2053 504f 286c 656e 2863 616e 6469   = SPO(len(candi
+00009900: 6461 7465 7329 290a 2020 2020 2020 2020  dates)).        
+00009910: 2020 2020 2020 2020 666f 7220 6530 2c65          for e0,e
+00009920: 312c 7320 696e 2065 6467 6573 3a20 0a20  1,s in edges: . 
+00009930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009940: 2020 2069 6620 6e6f 7420 7270 5f64 6566     if not rp_def
+00009950: 6561 742e 505b 6361 6e64 5f74 6f5f 6369  eat.P[cand_to_ci
+00009960: 6478 5b65 315d 5d5b 6361 6e64 5f74 6f5f  dx[e1]][cand_to_
+00009970: 6369 6478 5b65 305d 5d3a 0a20 2020 2020  cidx[e0]]:.     
+00009980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009990: 2020 2072 705f 6465 6665 6174 2e61 6464     rp_defeat.add
+000099a0: 2863 616e 645f 746f 5f63 6964 785b 6530  (cand_to_cidx[e0
+000099b0: 5d2c 6361 6e64 5f74 6f5f 6369 6478 5b65  ],cand_to_cidx[e
+000099c0: 315d 290a 2020 2020 2020 2020 2020 2020  1]).            
+000099d0: 2020 2020 7769 6e6e 6572 732e 6170 7065      winners.appe
+000099e0: 6e64 2863 6964 785f 746f 5f63 616e 645b  nd(cidx_to_cand[
+000099f0: 7270 5f64 6566 6561 742e 696e 6974 6961  rp_defeat.initia
+00009a00: 6c5f 656c 656d 656e 7473 2829 5b30 5d5d  l_elements()[0]]
+00009a10: 290a 2020 2020 7265 7475 726e 2073 6f72  ).    return sor
+00009a20: 7465 6428 6c69 7374 2873 6574 2877 696e  ted(list(set(win
+00009a30: 6e65 7273 2929 290a 0a64 6566 2072 616e  ners)))..def ran
+00009a40: 6b65 645f 7061 6972 735f 6465 6665 6174  ked_pairs_defeat
+00009a50: 7328 6564 6174 612c 2063 7572 725f 6361  s(edata, curr_ca
+00009a60: 6e64 7320 3d20 4e6f 6e65 2c20 7374 7265  nds = None, stre
+00009a70: 6e67 7468 5f66 756e 6374 696f 6e20 3d20  ngth_function = 
+00009a80: 4e6f 6e65 293a 2020 200a 2020 2020 2222  None):   .    ""
+00009a90: 220a 2020 2020 5265 7475 726e 7320 7468  ".    Returns th
+00009aa0: 6520 5261 6e6b 6564 2050 6169 7273 2064  e Ranked Pairs d
+00009ab0: 6566 6561 7420 7265 6c61 7469 6f6e 7320  efeat relations 
+00009ac0: 7072 6f64 7563 6564 2062 7920 7468 6520  produced by the 
+00009ad0: 5261 6e6b 6564 2050 6169 7273 2061 6c67  Ranked Pairs alg
+00009ae0: 6f72 6974 686d 2e20 0a0a 2020 2020 2e2e  orithm. ..    ..
+00009af0: 2069 6d70 6f72 7461 6e74 3a3a 0a20 2020   important::.   
+00009b00: 2020 2020 2055 6e6c 696b 6520 7468 6520       Unlike the 
+00009b10: 6f74 6865 7220 6675 6e63 7469 6f6e 7320  other functions 
+00009b20: 7468 6174 2072 6574 7572 6e20 6120 7369  that return a si
+00009b30: 6e67 6c65 2064 6566 6561 7420 7265 6c61  ngle defeat rela
+00009b40: 7469 6f6e 2c20 7468 6973 2072 6574 7572  tion, this retur
+00009b50: 6e73 2061 206c 6973 7420 6f66 2064 6566  ns a list of def
+00009b60: 6561 7420 7265 6c61 7469 6f6e 732e 200a  eat relations. .
+00009b70: 2020 2020 2020 2020 0a20 2020 2041 7267          .    Arg
+00009b80: 733a 0a20 2020 2020 2020 2065 6461 7461  s:.        edata
+00009b90: 2028 5072 6f66 696c 652c 2050 726f 6669   (Profile, Profi
+00009ba0: 6c65 5769 7468 5469 6573 2c20 4d61 7267  leWithTies, Marg
+00009bb0: 696e 4772 6170 6829 3a20 416e 7920 656c  inGraph): Any el
+00009bc0: 6563 7469 6f6e 2064 6174 6120 7468 6174  ection data that
+00009bd0: 2068 6173 2061 2060 6d61 7267 696e 6020   has a `margin` 
+00009be0: 6d65 7468 6f64 2e20 0a20 2020 2020 2020  method. .       
+00009bf0: 2063 7572 725f 6361 6e64 7320 284c 6973   curr_cands (Lis
+00009c00: 745b 696e 745d 2c20 6f70 7469 6f6e 616c  t[int], optional
+00009c10: 293a 2049 6620 7365 742c 2074 6865 6e20  ): If set, then 
+00009c20: 6669 6e64 2074 6865 2077 696e 6e65 7273  find the winners
+00009c30: 2066 6f72 2074 6865 2070 726f 6669 6c65   for the profile
+00009c40: 2072 6573 7472 6963 7465 6420 746f 2074   restricted to t
+00009c50: 6865 2063 616e 6469 6461 7465 7320 696e  he candidates in
+00009c60: 2060 6063 7572 725f 6361 6e64 7360 600a   ``curr_cands``.
+00009c70: 2020 2020 2020 2020 7374 7265 6e67 7468          strength
+00009c80: 5f66 756e 6374 696f 6e20 2866 756e 6374  _function (funct
+00009c90: 696f 6e2c 206f 7074 696f 6e61 6c29 3a20  ion, optional): 
+00009ca0: 5468 6520 7374 7265 6e67 7468 2066 756e  The strength fun
+00009cb0: 6374 696f 6e20 746f 2062 6520 7573 6564  ction to be used
+00009cc0: 2074 6f20 6361 6c63 756c 6174 6520 7468   to calculate th
+00009cd0: 6520 7374 7265 6e67 7468 206f 6620 6120  e strength of a 
+00009ce0: 7061 7468 2e20 2020 5468 6520 6465 6661  path.   The defa
+00009cf0: 756c 7420 6973 2074 6865 206d 6172 6769  ult is the margi
+00009d00: 6e20 6d65 7468 6f64 206f 6620 6060 6564  n method of ``ed
+00009d10: 6174 6160 602e 2020 2054 6869 7320 6f6e  ata``.   This on
+00009d20: 6c79 206d 6174 7465 7273 2077 6865 6e20  ly matters when 
+00009d30: 7468 6520 6261 6c6c 6f74 7320 6172 6520  the ballots are 
+00009d40: 6e6f 7420 6c69 6e65 6172 206f 7264 6572  not linear order
+00009d50: 732e 200a 0a20 2020 2052 6574 7572 6e73  s. ..    Returns
+00009d60: 3a20 0a20 2020 2020 2020 2041 206e 6574  : .        A net
+00009d70: 776f 726b 7820 4469 4772 6170 6820 7265  workx DiGraph re
+00009d80: 7072 6573 656e 7469 6e67 2074 6865 2052  presenting the R
+00009d90: 616e 6b65 6420 5061 6972 7320 6465 6665  anked Pairs defe
+00009da0: 6174 2072 656c 6174 696f 6e2e 200a 0a20  at relation. .. 
+00009db0: 2020 202e 2e20 7365 6561 6c73 6f3a 3a0a     .. seealso::.
+00009dc0: 0a20 2020 2020 2020 203a 6d65 7468 3a60  .        :meth:`
+00009dd0: 7072 6566 5f76 6f74 696e 672e 6d61 7267  pref_voting.marg
+00009de0: 696e 5f62 6173 6564 5f6d 6574 686f 6473  in_based_methods
+00009df0: 2e72 616e 6b65 645f 7061 6972 7360 2c20  .ranked_pairs`, 
+00009e00: 3a6d 6574 683a 6070 7265 665f 766f 7469  :meth:`pref_voti
+00009e10: 6e67 2e6d 6172 6769 6e5f 6261 7365 645f  ng.margin_based_
+00009e20: 6d65 7468 6f64 732e 7261 6e6b 6564 5f70  methods.ranked_p
+00009e30: 6169 7273 5f77 6974 685f 7465 7374 600a  airs_with_test`.
+00009e40: 0a20 2020 203a 4578 616d 706c 653a 200a  .    :Example: .
+00009e50: 0a20 2020 202e 2e20 706c 6f74 3a3a 2020  .    .. plot::  
+00009e60: 6d61 7267 696e 5f67 7261 7068 735f 6578  margin_graphs_ex
+00009e70: 616d 706c 6573 2f6d 675f 6578 5f72 705f  amples/mg_ex_rp_
+00009e80: 6465 6665 6174 732e 7079 0a20 2020 2020  defeats.py.     
+00009e90: 2020 203a 636f 6e74 6578 743a 2072 6573     :context: res
+00009ea0: 6574 2020 0a20 2020 2020 2020 203a 696e  et  .        :in
+00009eb0: 636c 7564 652d 736f 7572 6365 3a20 5472  clude-source: Tr
+00009ec0: 7565 0a0a 2020 2020 2e2e 2065 7865 635f  ue..    .. exec_
+00009ed0: 636f 6465 3a3a 0a0a 0a20 2020 2020 2020  code::...       
+00009ee0: 2066 726f 6d20 7072 6566 5f76 6f74 696e   from pref_votin
+00009ef0: 672e 7765 6967 6874 6564 5f6d 616a 6f72  g.weighted_major
+00009f00: 6974 795f 6772 6170 6873 2069 6d70 6f72  ity_graphs impor
+00009f10: 7420 4d61 7267 696e 4772 6170 680a 2020  t MarginGraph.  
+00009f20: 2020 2020 2020 6672 6f6d 2070 7265 665f        from pref_
+00009f30: 766f 7469 6e67 2e6d 6172 6769 6e5f 6261  voting.margin_ba
+00009f40: 7365 645f 6d65 7468 6f64 7320 696d 706f  sed_methods impo
+00009f50: 7274 2072 616e 6b65 645f 7061 6972 735f  rt ranked_pairs_
+00009f60: 6465 6665 6174 730a 0a20 2020 2020 2020  defeats..       
+00009f70: 206d 6720 3d20 4d61 7267 696e 4772 6170   mg = MarginGrap
+00009f80: 6828 5b30 2c20 312c 2032 2c20 335d 2c20  h([0, 1, 2, 3], 
+00009f90: 5b28 302c 2031 2c20 3130 292c 2028 302c  [(0, 1, 10), (0,
+00009fa0: 2032 2c20 3229 2c20 2831 2c20 332c 2034   2, 2), (1, 3, 4
+00009fb0: 292c 2028 322c 2031 2c20 3629 2c20 2832  ), (2, 1, 6), (2
+00009fc0: 2c20 332c 2038 292c 2028 332c 2030 2c20  , 3, 8), (3, 0, 
+00009fd0: 3429 5d29 0a20 2020 2020 2020 2072 705f  4)]).        rp_
+00009fe0: 6465 6665 6174 7320 3d20 7261 6e6b 6564  defeats = ranked
+00009ff0: 5f70 6169 7273 5f64 6566 6561 7473 286d  _pairs_defeats(m
+0000a000: 6729 0a0a 2020 2020 2020 2020 666f 7220  g)..        for 
+0000a010: 7270 6420 696e 2072 705f 6465 6665 6174  rpd in rp_defeat
+0000a020: 733a 200a 2020 2020 2020 2020 2020 2020  s: .            
+0000a030: 7072 696e 7428 7270 642e 6564 6765 7329  print(rpd.edges)
+0000a040: 0a0a 2020 2020 2222 220a 2020 2020 0a20  ..    """.    . 
+0000a050: 2020 2063 616e 6469 6461 7465 7320 3d20     candidates = 
+0000a060: 6564 6174 612e 6361 6e64 6964 6174 6573  edata.candidates
+0000a070: 2069 6620 6375 7272 5f63 616e 6473 2069   if curr_cands i
+0000a080: 7320 4e6f 6e65 2065 6c73 6520 6375 7272  s None else curr
+0000a090: 5f63 616e 6473 2020 2020 0a20 2020 2073  _cands    .    s
+0000a0a0: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
+0000a0b0: 203d 2065 6461 7461 2e6d 6172 6769 6e20   = edata.margin 
+0000a0c0: 6966 2073 7472 656e 6774 685f 6675 6e63  if strength_func
+0000a0d0: 7469 6f6e 2069 7320 4e6f 6e65 2065 6c73  tion is None els
+0000a0e0: 6520 7374 7265 6e67 7468 5f66 756e 6374  e strength_funct
+0000a0f0: 696f 6e20 2020 200a 0a20 2020 2077 5f65  ion    ..    w_e
+0000a100: 6467 6573 203d 205b 2863 312c 2063 322c  dges = [(c1, c2,
+0000a110: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
+0000a120: 6f6e 2863 312c 2063 3229 2920 666f 7220  on(c1, c2)) for 
+0000a130: 6331 2069 6e20 6361 6e64 6964 6174 6573  c1 in candidates
+0000a140: 2066 6f72 2063 3220 696e 2063 616e 6469   for c2 in candi
+0000a150: 6461 7465 7320 6966 2063 3120 213d 2063  dates if c1 != c
+0000a160: 3220 616e 6420 2865 6461 7461 2e6d 616a  2 and (edata.maj
+0000a170: 6f72 6974 795f 7072 6566 6572 7328 6331  ority_prefers(c1
+0000a180: 2c20 6332 2920 6f72 2065 6461 7461 2e69  , c2) or edata.i
+0000a190: 735f 7469 6564 2863 312c 2063 3229 295d  s_tied(c1, c2))]
+0000a1a0: 0a20 2020 2077 696e 6e65 7273 203d 206c  .    winners = l
+0000a1b0: 6973 7428 2920 2020 2020 2020 2020 2020  ist()           
+0000a1c0: 200a 2020 2020 7374 7265 6e67 7468 7320   .    strengths 
+0000a1d0: 3d20 736f 7274 6564 286c 6973 7428 7365  = sorted(list(se
+0000a1e0: 7428 5b65 5b32 5d20 666f 7220 6520 696e  t([e[2] for e in
+0000a1f0: 2077 5f65 6467 6573 5d29 292c 2072 6576   w_edges])), rev
+0000a200: 6572 7365 3d54 7275 6529 0a20 2020 2073  erse=True).    s
+0000a210: 6f72 7465 645f 6564 6765 7320 3d20 5b5b  orted_edges = [[
+0000a220: 6520 666f 7220 6520 696e 2077 5f65 6467  e for e in w_edg
+0000a230: 6573 2069 6620 655b 325d 203d 3d20 735d  es if e[2] == s]
+0000a240: 2066 6f72 2073 2069 6e20 7374 7265 6e67   for s in streng
+0000a250: 7468 735d 0a20 2020 2074 6273 203d 2070  ths].    tbs = p
+0000a260: 726f 6475 6374 282a 5b70 6572 6d75 7461  roduct(*[permuta
+0000a270: 7469 6f6e 7328 6564 6765 7329 2066 6f72  tions(edges) for
+0000a280: 2065 6467 6573 2069 6e20 736f 7274 6564   edges in sorted
+0000a290: 5f65 6467 6573 5d29 0a20 2020 2072 705f  _edges]).    rp_
+0000a2a0: 6465 6665 6174 7320 3d20 6c69 7374 2829  defeats = list()
+0000a2b0: 0a20 2020 2066 6f72 2074 6220 696e 2074  .    for tb in t
+0000a2c0: 6273 3a0a 2020 2020 2020 2020 6564 6765  bs:.        edge
+0000a2d0: 7320 3d20 666c 6174 7465 6e28 7462 290a  s = flatten(tb).
+0000a2e0: 2020 2020 2020 2020 7270 5f64 6566 6561          rp_defea
+0000a2f0: 7420 3d20 6e78 2e44 6947 7261 7068 2829  t = nx.DiGraph()
+0000a300: 200a 2020 2020 2020 2020 666f 7220 6520   .        for e 
+0000a310: 696e 2065 6467 6573 3a20 0a20 2020 2020  in edges: .     
+0000a320: 2020 2020 2020 2072 705f 6465 6665 6174         rp_defeat
+0000a330: 2e61 6464 5f65 6467 6528 655b 305d 2c20  .add_edge(e[0], 
+0000a340: 655b 315d 2c20 7765 6967 6874 3d65 5b32  e[1], weight=e[2
+0000a350: 5d29 0a20 2020 2020 2020 2020 2020 2069  ]).            i
+0000a360: 6620 646f 6573 5f63 7265 6174 655f 6379  f does_create_cy
+0000a370: 636c 6528 7270 5f64 6566 6561 742c 2065  cle(rp_defeat, e
+0000a380: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0000a390: 2020 2072 705f 6465 6665 6174 2e72 656d     rp_defeat.rem
+0000a3a0: 6f76 655f 6564 6765 2865 5b30 5d2c 2065  ove_edge(e[0], e
+0000a3b0: 5b31 5d29 0a20 2020 2020 2020 2072 705f  [1]).        rp_
+0000a3c0: 6465 6665 6174 732e 6170 7065 6e64 2872  defeats.append(r
+0000a3d0: 705f 6465 6665 6174 290a 2020 2020 2020  p_defeat).      
+0000a3e0: 2020 7769 6e6e 6572 732e 6170 7065 6e64    winners.append
+0000a3f0: 286d 6178 696d 616c 5f65 6c65 6d65 6e74  (maximal_element
+0000a400: 7328 7270 5f64 6566 6561 7429 5b30 5d29  s(rp_defeat)[0])
+0000a410: 0a20 2020 2072 6574 7572 6e20 7270 5f64  .    return rp_d
+0000a420: 6566 6561 7473 0a0a 7270 5f74 625f 7072  efeats..rp_tb_pr
+0000a430: 6f70 6572 7469 6573 203d 2056 6f74 696e  operties = Votin
+0000a440: 674d 6574 686f 6450 726f 7065 7274 6965  gMethodPropertie
+0000a450: 7328 0a20 2020 2063 6f6e 646f 7263 6574  s(.    condorcet
+0000a460: 5f77 696e 6e65 723d 5472 7565 2c20 0a20  _winner=True, . 
+0000a470: 2020 2063 6f6e 646f 7263 6574 5f6c 6f73     condorcet_los
+0000a480: 6572 3d54 7275 652c 0a20 2020 2070 6172  er=True,.    par
+0000a490: 6574 6f5f 646f 6d69 6e61 6e63 653d 5472  eto_dominance=Tr
+0000a4a0: 7565 2c0a 2020 2020 706f 7369 7469 7665  ue,.    positive
+0000a4b0: 5f69 6e76 6f6c 7665 6d65 6e74 3d46 616c  _involvement=Fal
+0000a4c0: 7365 2c20 0a20 2020 2029 0a40 766d 286e  se, .    ).@vm(n
+0000a4d0: 616d 653d 2252 616e 6b65 6420 5061 6972  ame="Ranked Pair
+0000a4e0: 7320 5442 222c 0a20 2020 2070 726f 7065  s TB",.    prope
+0000a4f0: 7274 6965 733d 7270 5f74 625f 7072 6f70  rties=rp_tb_prop
+0000a500: 6572 7469 6573 2c0a 2020 2020 696e 7075  erties,.    inpu
+0000a510: 745f 7479 7065 733d 5b45 6c65 6374 696f  t_types=[Electio
+0000a520: 6e54 7970 6573 2e50 524f 4649 4c45 2c20  nTypes.PROFILE, 
+0000a530: 456c 6563 7469 6f6e 5479 7065 732e 5052  ElectionTypes.PR
+0000a540: 4f46 494c 455f 5749 5448 5f54 4945 532c  OFILE_WITH_TIES,
+0000a550: 2045 6c65 6374 696f 6e54 7970 6573 2e4d   ElectionTypes.M
+0000a560: 4152 4749 4e5f 4752 4150 485d 290a 6465  ARGIN_GRAPH]).de
+0000a570: 6620 7261 6e6b 6564 5f70 6169 7273 5f74  f ranked_pairs_t
+0000a580: 6228 0a20 2020 2065 6461 7461 2c20 0a20  b(.    edata, . 
+0000a590: 2020 2063 7572 725f 6361 6e64 7320 3d20     curr_cands = 
+0000a5a0: 4e6f 6e65 2c20 0a20 2020 2074 6965 5f62  None, .    tie_b
+0000a5b0: 7265 616b 6572 203d 204e 6f6e 652c 200a  reaker = None, .
+0000a5c0: 2020 2020 7374 7265 6e67 7468 5f66 756e      strength_fun
+0000a5d0: 6374 696f 6e20 3d20 4e6f 6e65 293a 2020  ction = None):  
+0000a5e0: 200a 2020 2020 2222 220a 2020 2020 5261   .    """.    Ra
+0000a5f0: 6e6b 6564 2050 6169 7273 2077 6974 6820  nked Pairs with 
+0000a600: 6120 6669 7865 6420 6c69 6e65 6172 206f  a fixed linear o
+0000a610: 7264 6572 206f 6e20 7468 6520 6361 6e64  rder on the cand
+0000a620: 6964 6174 6573 2074 6f20 6272 6561 6b20  idates to break 
+0000a630: 616e 7920 7469 6573 2069 6e20 7468 6520  any ties in the 
+0000a640: 6d61 7267 696e 732e 2020 200a 2020 2020  margins.   .    
+0000a650: 5369 6e63 6520 7468 6520 7469 655f 6272  Since the tie_br
+0000a660: 6561 6b65 7220 6973 2061 206c 696e 6561  eaker is a linea
+0000a670: 7220 6f72 6465 722c 2074 6869 7320 6d65  r order, this me
+0000a680: 7468 6f64 2069 7320 7265 736f 6c75 7465  thod is resolute
+0000a690: 2e20 2020 0a0a 2020 2020 4172 6773 3a0a  .   ..    Args:.
+0000a6a0: 2020 2020 2020 2020 6564 6174 6120 2850          edata (P
+0000a6b0: 726f 6669 6c65 2c20 5072 6f66 696c 6557  rofile, ProfileW
+0000a6c0: 6974 6854 6965 732c 204d 6172 6769 6e47  ithTies, MarginG
+0000a6d0: 7261 7068 293a 2041 6e79 2065 6c65 6374  raph): Any elect
+0000a6e0: 696f 6e20 6461 7461 2074 6861 7420 6861  ion data that ha
+0000a6f0: 7320 6120 606d 6172 6769 6e60 206d 6574  s a `margin` met
+0000a700: 686f 642e 200a 2020 2020 2020 2020 6375  hod. .        cu
+0000a710: 7272 5f63 616e 6473 2028 4c69 7374 5b69  rr_cands (List[i
+0000a720: 6e74 5d2c 206f 7074 696f 6e61 6c29 3a20  nt], optional): 
+0000a730: 4966 2073 6574 2c20 7468 656e 2066 696e  If set, then fin
+0000a740: 6420 7468 6520 7769 6e6e 6572 7320 666f  d the winners fo
+0000a750: 7220 7468 6520 7072 6f66 696c 6520 7265  r the profile re
+0000a760: 7374 7269 6374 6564 2074 6f20 7468 6520  stricted to the 
+0000a770: 6361 6e64 6964 6174 6573 2069 6e20 6060  candidates in ``
+0000a780: 6375 7272 5f63 616e 6473 6060 0a20 2020  curr_cands``.   
+0000a790: 2020 2020 2073 7472 656e 6774 685f 6675       strength_fu
+0000a7a0: 6e63 7469 6f6e 2028 6675 6e63 7469 6f6e  nction (function
+0000a7b0: 2c20 6f70 7469 6f6e 616c 293a 2054 6865  , optional): The
+0000a7c0: 2073 7472 656e 6774 6820 6675 6e63 7469   strength functi
+0000a7d0: 6f6e 2074 6f20 6265 2075 7365 6420 746f  on to be used to
+0000a7e0: 2063 616c 6375 6c61 7465 2074 6865 2073   calculate the s
+0000a7f0: 7472 656e 6774 6820 6f66 2061 2070 6174  trength of a pat
+0000a800: 682e 2020 2054 6865 2064 6566 6175 6c74  h.   The default
+0000a810: 2069 7320 7468 6520 6d61 7267 696e 206d   is the margin m
+0000a820: 6574 686f 6420 6f66 2060 6065 6461 7461  ethod of ``edata
+0000a830: 6060 2e20 2020 5468 6973 206f 6e6c 7920  ``.   This only 
+0000a840: 6d61 7474 6572 7320 7768 656e 2074 6865  matters when the
+0000a850: 2062 616c 6c6f 7473 2061 7265 206e 6f74   ballots are not
+0000a860: 206c 696e 6561 7220 6f72 6465 7273 2e20   linear orders. 
+0000a870: 0a0a 2020 2020 5265 7475 726e 733a 200a  ..    Returns: .
+0000a880: 2020 2020 2020 2020 4120 736f 7274 6564          A sorted
+0000a890: 206c 6973 7420 6f66 2063 616e 6469 6461   list of candida
+0000a8a0: 7465 732e 200a 0a20 2020 202e 2e20 7365  tes. ..    .. se
+0000a8b0: 6561 6c73 6f3a 3a0a 0a20 2020 2020 2020  ealso::..       
+0000a8c0: 203a 6d65 7468 3a60 7072 6566 5f76 6f74   :meth:`pref_vot
+0000a8d0: 696e 672e 6d61 7267 696e 5f62 6173 6564  ing.margin_based
+0000a8e0: 5f6d 6574 686f 6473 2e72 616e 6b65 645f  _methods.ranked_
+0000a8f0: 7061 6972 7360 2c20 3a6d 6574 683a 6070  pairs`, :meth:`p
+0000a900: 7265 665f 766f 7469 6e67 2e6d 6172 6769  ref_voting.margi
+0000a910: 6e5f 6261 7365 645f 6d65 7468 6f64 732e  n_based_methods.
+0000a920: 7261 6e6b 6564 5f70 6169 7273 5f77 6974  ranked_pairs_wit
+0000a930: 685f 7465 7374 600a 0a20 2020 202e 2e20  h_test`..    .. 
+0000a940: 6578 6563 5f63 6f64 653a 3a0a 0a20 2020  exec_code::..   
+0000a950: 2020 2020 2066 726f 6d20 7072 6566 5f76       from pref_v
+0000a960: 6f74 696e 672e 7072 6f66 696c 6573 2069  oting.profiles i
+0000a970: 6d70 6f72 7420 5072 6f66 696c 650a 2020  mport Profile.  
+0000a980: 2020 2020 2020 6672 6f6d 2070 7265 665f        from pref_
+0000a990: 766f 7469 6e67 2e6d 6172 6769 6e5f 6261  voting.margin_ba
+0000a9a0: 7365 645f 6d65 7468 6f64 7320 696d 706f  sed_methods impo
+0000a9b0: 7274 2072 616e 6b65 645f 7061 6972 735f  rt ranked_pairs_
+0000a9c0: 7462 2c20 7261 6e6b 6564 5f70 6169 7273  tb, ranked_pairs
+0000a9d0: 5f7a 740a 0a20 2020 2020 2020 2070 726f  _zt..        pro
+0000a9e0: 6620 3d20 5072 6f66 696c 6528 5b5b 322c  f = Profile([[2,
+0000a9f0: 2033 2c20 312c 2030 5d2c 205b 302c 2033   3, 1, 0], [0, 3
+0000aa00: 2c20 312c 2032 5d2c 205b 312c 2033 2c20  , 1, 2], [1, 3, 
+0000aa10: 322c 2030 5d2c 205b 322c 2031 2c20 332c  2, 0], [2, 1, 3,
+0000aa20: 2030 5d5d 2c20 5b31 2c20 312c 2031 2c20   0]], [1, 1, 1, 
+0000aa30: 315d 290a 0a20 2020 2020 2020 2070 726f  1])..        pro
+0000aa40: 662e 6469 7370 6c61 7928 290a 0a20 2020  f.display()..   
+0000aa50: 2020 2020 2072 616e 6b65 645f 7061 6972       ranked_pair
+0000aa60: 735f 7462 2e64 6973 706c 6179 2870 726f  s_tb.display(pro
+0000aa70: 6629 0a20 2020 2020 2020 2072 616e 6b65  f).        ranke
+0000aa80: 645f 7061 6972 735f 7462 2e64 6973 706c  d_pairs_tb.displ
+0000aa90: 6179 2870 726f 662c 2074 6965 5f62 7265  ay(prof, tie_bre
+0000aaa0: 616b 6572 203d 205b 332c 2032 2c20 312c  aker = [3, 2, 1,
+0000aab0: 2030 5d29 0a20 2020 2020 2020 2072 616e   0]).        ran
+0000aac0: 6b65 645f 7061 6972 735f 7a74 2e64 6973  ked_pairs_zt.dis
+0000aad0: 706c 6179 2870 726f 6629 0a0a 2020 2020  play(prof)..    
+0000aae0: 2222 220a 0a20 2020 2063 616e 6469 6461  """..    candida
+0000aaf0: 7465 7320 3d20 6564 6174 612e 6361 6e64  tes = edata.cand
+0000ab00: 6964 6174 6573 2069 6620 6375 7272 5f63  idates if curr_c
+0000ab10: 616e 6473 2069 7320 4e6f 6e65 2065 6c73  ands is None els
+0000ab20: 6520 6375 7272 5f63 616e 6473 2020 2020  e curr_cands    
+0000ab30: 0a20 2020 2063 6964 785f 746f 5f63 616e  .    cidx_to_can
+0000ab40: 6420 3d20 7b63 6964 783a 2063 2066 6f72  d = {cidx: c for
+0000ab50: 2063 6964 782c 2063 2069 6e20 656e 756d   cidx, c in enum
+0000ab60: 6572 6174 6528 6361 6e64 6964 6174 6573  erate(candidates
+0000ab70: 297d 2020 0a20 2020 2063 616e 645f 746f  )}  .    cand_to
+0000ab80: 5f63 6964 7820 3d20 7b63 3a20 6369 6478  _cidx = {c: cidx
+0000ab90: 2066 6f72 2063 6964 782c 2063 2069 6e20   for cidx, c in 
+0000aba0: 656e 756d 6572 6174 6528 6361 6e64 6964  enumerate(candid
+0000abb0: 6174 6573 297d 2020 0a0a 2020 2020 7374  ates)}  ..    st
+0000abc0: 7265 6e67 7468 5f66 756e 6374 696f 6e20  rength_function 
+0000abd0: 3d20 6564 6174 612e 6d61 7267 696e 2069  = edata.margin i
+0000abe0: 6620 7374 7265 6e67 7468 5f66 756e 6374  f strength_funct
+0000abf0: 696f 6e20 6973 204e 6f6e 6520 656c 7365  ion is None else
+0000ac00: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
+0000ac10: 6f6e 0a20 2020 200a 2020 2020 7462 5f72  on.    .    tb_r
+0000ac20: 616e 6b69 6e67 203d 2074 6965 5f62 7265  anking = tie_bre
+0000ac30: 616b 6572 2069 6620 7469 655f 6272 6561  aker if tie_brea
+0000ac40: 6b65 7220 6973 206e 6f74 204e 6f6e 6520  ker is not None 
+0000ac50: 656c 7365 2073 6f72 7465 6428 6c69 7374  else sorted(list
+0000ac60: 2863 616e 6469 6461 7465 7329 290a 0a20  (candidates)).. 
+0000ac70: 2020 2063 7720 3d20 6564 6174 612e 636f     cw = edata.co
+0000ac80: 6e64 6f72 6365 745f 7769 6e6e 6572 2863  ndorcet_winner(c
+0000ac90: 7572 725f 6361 6e64 733d 6375 7272 5f63  urr_cands=curr_c
+0000aca0: 616e 6473 290a 2020 2020 2320 5261 6e6b  ands).    # Rank
+0000acb0: 6564 2050 6169 7273 2069 7320 436f 6e64  ed Pairs is Cond
+0000acc0: 6f72 6365 7420 636f 6e73 6973 7465 6e74  orcet consistent
+0000acd0: 2c20 736f 2073 696d 706c 7920 7265 7475  , so simply retu
+0000ace0: 726e 2074 6865 2043 6f6e 646f 7263 6574  rn the Condorcet
+0000acf0: 2077 696e 6e65 7220 6966 2065 7869 7374   winner if exist
+0000ad00: 730a 2020 2020 6966 2063 7720 6973 206e  s.    if cw is n
+0000ad10: 6f74 204e 6f6e 653a 200a 2020 2020 2020  ot None: .      
+0000ad20: 2020 7769 6e6e 6572 7320 3d20 5b63 775d    winners = [cw]
+0000ad30: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
+0000ad40: 2020 2077 5f65 6467 6573 203d 205b 2863     w_edges = [(c
+0000ad50: 312c 2063 322c 2073 7472 656e 6774 685f  1, c2, strength_
+0000ad60: 6675 6e63 7469 6f6e 2863 312c 2063 3229  function(c1, c2)
+0000ad70: 2920 666f 7220 6331 2069 6e20 6361 6e64  ) for c1 in cand
+0000ad80: 6964 6174 6573 2066 6f72 2063 3220 696e  idates for c2 in
+0000ad90: 2063 616e 6469 6461 7465 7320 0a20 2020   candidates .   
+0000ada0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000adb0: 6966 2063 3120 213d 2063 3220 616e 6420  if c1 != c2 and 
+0000adc0: 2865 6461 7461 2e6d 616a 6f72 6974 795f  (edata.majority_
+0000add0: 7072 6566 6572 7328 6331 2c20 6332 2920  prefers(c1, c2) 
+0000ade0: 6f72 2065 6461 7461 2e69 735f 7469 6564  or edata.is_tied
+0000adf0: 2863 312c 2063 3229 295d 0a20 2020 2020  (c1, c2))].     
+0000ae00: 2020 2077 696e 6e65 7273 203d 206c 6973     winners = lis
+0000ae10: 7428 2920 2020 2020 2020 2020 2020 200a  t()            .
+0000ae20: 2020 2020 2020 2020 7374 7265 6e67 7468          strength
+0000ae30: 7320 3d20 736f 7274 6564 286c 6973 7428  s = sorted(list(
+0000ae40: 7365 7428 5b65 5b32 5d20 666f 7220 6520  set([e[2] for e 
+0000ae50: 696e 2077 5f65 6467 6573 5d29 292c 2072  in w_edges])), r
+0000ae60: 6576 6572 7365 3d54 7275 6529 0a20 2020  everse=True).   
+0000ae70: 2020 2020 200a 2020 2020 2020 2020 7270       .        rp
+0000ae80: 5f64 6566 6561 7420 3d20 5350 4f28 6c65  _defeat = SPO(le
+0000ae90: 6e28 6361 6e64 6964 6174 6573 2929 0a0a  n(candidates))..
+0000aea0: 2020 2020 2020 2020 666f 7220 7320 696e          for s in
+0000aeb0: 2073 7472 656e 6774 6873 3a20 0a20 2020   strengths: .   
+0000aec0: 2020 2020 2020 2020 2065 6467 6573 203d           edges =
+0000aed0: 205b 6520 666f 7220 6520 696e 2077 5f65   [e for e in w_e
+0000aee0: 6467 6573 2069 6620 655b 325d 203d 3d20  dges if e[2] == 
+0000aef0: 735d 0a20 2020 2020 2020 2020 2020 200a  s].            .
+0000af00: 2020 2020 2020 2020 2020 2020 2320 6272              # br
+0000af10: 6561 6b20 7469 6573 2075 7369 6e67 2074  eak ties using t
+0000af20: 6865 206c 6578 6963 6f67 7261 7068 6963  he lexicographic
+0000af30: 206f 7264 6572 696e 6720 6f6e 2074 7570   ordering on tup
+0000af40: 6c65 7320 6769 7665 6e20 7462 5f72 616e  les given tb_ran
+0000af50: 6b69 6e67 0a20 2020 2020 2020 2020 2020  king.           
+0000af60: 2073 6f72 7465 645f 6564 6765 7320 3d20   sorted_edges = 
+0000af70: 736f 7274 6564 2865 6467 6573 2c20 6b65  sorted(edges, ke
+0000af80: 7920 3d20 6c61 6d62 6461 2065 3a20 2874  y = lambda e: (t
+0000af90: 625f 7261 6e6b 696e 672e 696e 6465 7828  b_ranking.index(
+0000afa0: 655b 305d 292c 2074 625f 7261 6e6b 696e  e[0]), tb_rankin
+0000afb0: 672e 696e 6465 7828 655b 315d 2929 2c20  g.index(e[1])), 
+0000afc0: 7265 7665 7273 653d 4661 6c73 6529 0a20  reverse=False). 
+0000afd0: 2020 2020 2020 2020 2020 2066 6f72 2065             for e
+0000afe0: 302c 6531 2c73 2069 6e20 6564 6765 733a  0,e1,s in edges:
+0000aff0: 200a 2020 2020 2020 2020 2020 2020 2020   .              
+0000b000: 2020 6966 206e 6f74 2072 705f 6465 6665    if not rp_defe
+0000b010: 6174 2e50 5b63 616e 645f 746f 5f63 6964  at.P[cand_to_cid
+0000b020: 785b 6531 5d5d 5b63 616e 645f 746f 5f63  x[e1]][cand_to_c
+0000b030: 6964 785b 6530 5d5d 3a0a 2020 2020 2020  idx[e0]]:.      
+0000b040: 2020 2020 2020 2020 2020 2020 2020 7270                rp
+0000b050: 5f64 6566 6561 742e 6164 6428 6361 6e64  _defeat.add(cand
+0000b060: 5f74 6f5f 6369 6478 5b65 305d 2c63 616e  _to_cidx[e0],can
+0000b070: 645f 746f 5f63 6964 785b 6531 5d29 0a20  d_to_cidx[e1]). 
+0000b080: 2020 2020 2020 2020 2020 2077 696e 6e65             winne
+0000b090: 7273 2e61 7070 656e 6428 6369 6478 5f74  rs.append(cidx_t
+0000b0a0: 6f5f 6361 6e64 5b72 705f 6465 6665 6174  o_cand[rp_defeat
+0000b0b0: 2e69 6e69 7469 616c 5f65 6c65 6d65 6e74  .initial_element
+0000b0c0: 7328 295b 305d 5d29 0a0a 2020 2020 7265  s()[0]])..    re
+0000b0d0: 7475 726e 2073 6f72 7465 6428 6c69 7374  turn sorted(list
+0000b0e0: 2873 6574 2877 696e 6e65 7273 2929 290a  (set(winners))).
+0000b0f0: 0a72 705f 7a74 5f70 726f 7065 7274 6965  .rp_zt_propertie
+0000b100: 7320 3d20 566f 7469 6e67 4d65 7468 6f64  s = VotingMethod
+0000b110: 5072 6f70 6572 7469 6573 280a 2020 2020  Properties(.    
+0000b120: 636f 6e64 6f72 6365 745f 7769 6e6e 6572  condorcet_winner
+0000b130: 3d54 7275 652c 200a 2020 2020 636f 6e64  =True, .    cond
+0000b140: 6f72 6365 745f 6c6f 7365 723d 5472 7565  orcet_loser=True
+0000b150: 2c0a 2020 2020 7061 7265 746f 5f64 6f6d  ,.    pareto_dom
+0000b160: 696e 616e 6365 3d54 7275 652c 200a 2020  inance=True, .  
+0000b170: 2020 706f 7369 7469 7665 5f69 6e76 6f6c    positive_invol
+0000b180: 7665 6d65 6e74 3d46 616c 7365 2c0a 2020  vement=False,.  
+0000b190: 2020 290a 4076 6d28 6e61 6d65 3d22 5261    ).@vm(name="Ra
+0000b1a0: 6e6b 6564 2050 6169 7273 205a 5422 2c0a  nked Pairs ZT",.
+0000b1b0: 2020 2020 7072 6f70 6572 7469 6573 3d72      properties=r
+0000b1c0: 705f 7a74 5f70 726f 7065 7274 6965 732c  p_zt_properties,
+0000b1d0: 0a20 2020 2069 6e70 7574 5f74 7970 6573  .    input_types
+0000b1e0: 3d5b 456c 6563 7469 6f6e 5479 7065 732e  =[ElectionTypes.
+0000b1f0: 5052 4f46 494c 455d 290a 6465 6620 7261  PROFILE]).def ra
+0000b200: 6e6b 6564 5f70 6169 7273 5f7a 7428 0a20  nked_pairs_zt(. 
+0000b210: 2020 2070 726f 6669 6c65 2c20 0a20 2020     profile, .   
+0000b220: 2063 7572 725f 6361 6e64 7320 3d20 4e6f   curr_cands = No
+0000b230: 6e65 2c20 0a20 2020 2073 7472 656e 6774  ne, .    strengt
+0000b240: 685f 6675 6e63 7469 6f6e 203d 204e 6f6e  h_function = Non
+0000b250: 6529 3a20 2020 0a20 2020 2022 2222 5261  e):   .    """Ra
+0000b260: 6e6b 6564 2070 6169 7273 2077 6865 7265  nked pairs where
+0000b270: 2061 2066 6978 6564 2076 6f74 6572 2062   a fixed voter b
+0000b280: 7265 616b 7320 616e 7920 7469 6573 2069  reaks any ties i
+0000b290: 6e20 7468 6520 6d61 7267 696e 732e 2020  n the margins.  
+0000b2a0: 4974 2069 7320 616c 7761 7973 2074 6865  It is always the
+0000b2b0: 2076 6f74 6572 2069 6e20 706f 7369 7469   voter in positi
+0000b2c0: 6f6e 2030 2074 6861 7420 6272 6561 6b73  on 0 that breaks
+0000b2d0: 2074 6865 2074 6965 732e 2020 5369 6e63   the ties.  Sinc
+0000b2e0: 6520 766f 7465 7273 2068 6176 6520 7374  e voters have st
+0000b2f0: 7269 6374 2070 7265 6665 7265 6e63 6573  rict preferences
+0000b300: 2c20 7468 6973 206d 6574 686f 6420 6973  , this method is
+0000b310: 2072 6573 6f6c 7574 652e 2020 5468 6973   resolute.  This
+0000b320: 2069 7320 6b6e 6f77 6e20 6173 2052 616e   is known as Ran
+0000b330: 6b65 6420 5061 6972 7320 5a54 2c20 666f  ked Pairs ZT, fo
+0000b340: 7220 5a61 7669 7374 2054 6964 656d 616e  r Zavist Tideman
+0000b350: 2e0a 0a20 2020 2041 7267 733a 0a20 2020  ...    Args:.   
+0000b360: 2020 2020 2065 6461 7461 2028 5072 6f66       edata (Prof
+0000b370: 696c 6529 3a20 4120 7072 6f66 696c 6520  ile): A profile 
+0000b380: 6f66 206c 696e 6561 7220 6f72 6465 7273  of linear orders
+0000b390: 0a20 2020 2020 2020 2063 7572 725f 6361  .        curr_ca
+0000b3a0: 6e64 7320 284c 6973 745b 696e 745d 2c20  nds (List[int], 
+0000b3b0: 6f70 7469 6f6e 616c 293a 2049 6620 7365  optional): If se
+0000b3c0: 742c 2074 6865 6e20 6669 6e64 2074 6865  t, then find the
+0000b3d0: 2077 696e 6e65 7273 2066 6f72 2074 6865   winners for the
+0000b3e0: 2070 726f 6669 6c65 2072 6573 7472 6963   profile restric
+0000b3f0: 7465 6420 746f 2074 6865 2063 616e 6469  ted to the candi
+0000b400: 6461 7465 7320 696e 2060 6063 7572 725f  dates in ``curr_
+0000b410: 6361 6e64 7360 600a 0a20 2020 2052 6574  cands``..    Ret
+0000b420: 7572 6e73 3a20 0a20 2020 2020 2020 2041  urns: .        A
+0000b430: 2073 6f72 7465 6420 6c69 7374 206f 6620   sorted list of 
+0000b440: 6361 6e64 6964 6174 6573 2e20 0a0a 2020  candidates. ..  
+0000b450: 2020 2e2e 2073 6565 616c 736f 3a3a 0a0a    .. seealso::..
+0000b460: 2020 2020 2020 2020 3a6d 6574 683a 6070          :meth:`p
+0000b470: 7265 665f 766f 7469 6e67 2e6d 6172 6769  ref_voting.margi
+0000b480: 6e5f 6261 7365 645f 6d65 7468 6f64 732e  n_based_methods.
+0000b490: 7261 6e6b 6564 5f70 6169 7273 602c 203a  ranked_pairs`, :
+0000b4a0: 6d65 7468 3a60 7072 6566 5f76 6f74 696e  meth:`pref_votin
+0000b4b0: 672e 6d61 7267 696e 5f62 6173 6564 5f6d  g.margin_based_m
+0000b4c0: 6574 686f 6473 2e72 616e 6b65 645f 7061  ethods.ranked_pa
+0000b4d0: 6972 735f 7769 7468 5f74 6573 7460 0a0a  irs_with_test`..
+0000b4e0: 2020 2020 2e2e 2065 7865 635f 636f 6465      .. exec_code
+0000b4f0: 3a3a 0a0a 2020 2020 2020 2020 6672 6f6d  ::..        from
+0000b500: 2070 7265 665f 766f 7469 6e67 2e70 726f   pref_voting.pro
+0000b510: 6669 6c65 7320 696d 706f 7274 2050 726f  files import Pro
+0000b520: 6669 6c65 0a20 2020 2020 2020 2066 726f  file.        fro
+0000b530: 6d20 7072 6566 5f76 6f74 696e 672e 6d61  m pref_voting.ma
+0000b540: 7267 696e 5f62 6173 6564 5f6d 6574 686f  rgin_based_metho
+0000b550: 6473 2069 6d70 6f72 7420 7261 6e6b 6564  ds import ranked
+0000b560: 5f70 6169 7273 5f74 622c 2072 616e 6b65  _pairs_tb, ranke
+0000b570: 645f 7061 6972 735f 7a74 0a0a 2020 2020  d_pairs_zt..    
+0000b580: 2020 2020 7072 6f66 203d 2050 726f 6669      prof = Profi
+0000b590: 6c65 285b 5b32 2c20 332c 2031 2c20 305d  le([[2, 3, 1, 0]
+0000b5a0: 2c20 5b30 2c20 332c 2031 2c20 325d 2c20  , [0, 3, 1, 2], 
+0000b5b0: 5b31 2c20 332c 2032 2c20 305d 2c20 5b32  [1, 3, 2, 0], [2
+0000b5c0: 2c20 312c 2033 2c20 305d 5d2c 205b 312c  , 1, 3, 0]], [1,
+0000b5d0: 2031 2c20 312c 2031 5d29 0a0a 2020 2020   1, 1, 1])..    
+0000b5e0: 2020 2020 7072 6f66 2e64 6973 706c 6179      prof.display
+0000b5f0: 2829 0a0a 2020 2020 2020 2020 7261 6e6b  ()..        rank
+0000b600: 6564 5f70 6169 7273 5f74 622e 6469 7370  ed_pairs_tb.disp
+0000b610: 6c61 7928 7072 6f66 290a 2020 2020 2020  lay(prof).      
+0000b620: 2020 7261 6e6b 6564 5f70 6169 7273 5f74    ranked_pairs_t
+0000b630: 622e 6469 7370 6c61 7928 7072 6f66 2c20  b.display(prof, 
+0000b640: 7469 655f 6272 6561 6b65 7220 3d20 5b33  tie_breaker = [3
+0000b650: 2c20 322c 2031 2c20 305d 290a 2020 2020  , 2, 1, 0]).    
+0000b660: 2020 2020 7261 6e6b 6564 5f70 6169 7273      ranked_pairs
+0000b670: 5f7a 742e 6469 7370 6c61 7928 7072 6f66  _zt.display(prof
+0000b680: 290a 0a20 2020 200a 2020 2020 2222 220a  )..    .    """.
+0000b690: 2020 2020 6361 6e64 6964 6174 6573 203d      candidates =
+0000b6a0: 2070 726f 6669 6c65 2e63 616e 6469 6461   profile.candida
+0000b6b0: 7465 7320 6966 2063 7572 725f 6361 6e64  tes if curr_cand
+0000b6c0: 7320 6973 204e 6f6e 6520 656c 7365 2063  s is None else c
+0000b6d0: 7572 725f 6361 6e64 7320 2020 200a 2020  urr_cands    .  
+0000b6e0: 2020 0a20 2020 2023 2074 6865 2074 6965    .    # the tie
+0000b6f0: 2d62 7265 616b 6572 2069 7320 616c 7761  -breaker is alwa
+0000b700: 7973 2074 6865 2066 6972 7374 2076 6f74  ys the first vot
+0000b710: 6572 2e20 0a20 2020 2074 625f 7261 6e6b  er. .    tb_rank
+0000b720: 696e 6720 3d20 7475 706c 6528 5b63 2066  ing = tuple([c f
+0000b730: 6f72 2063 2069 6e20 6c69 7374 2870 726f  or c in list(pro
+0000b740: 6669 6c65 2e5f 7261 6e6b 696e 6773 5b30  file._rankings[0
+0000b750: 5d29 2069 6620 6320 696e 2063 616e 6469  ]) if c in candi
+0000b760: 6461 7465 735d 290a 2020 2020 0a20 2020  dates]).    .   
+0000b770: 2072 6574 7572 6e20 7261 6e6b 6564 5f70   return ranked_p
+0000b780: 6169 7273 5f74 6228 7072 6f66 696c 652c  airs_tb(profile,
+0000b790: 2063 7572 725f 6361 6e64 7320 3d20 6375   curr_cands = cu
+0000b7a0: 7272 5f63 616e 6473 2c20 7469 655f 6272  rr_cands, tie_br
+0000b7b0: 6561 6b65 7220 3d20 7462 5f72 616e 6b69  eaker = tb_ranki
+0000b7c0: 6e67 2c20 7374 7265 6e67 7468 5f66 756e  ng, strength_fun
+0000b7d0: 6374 696f 6e20 3d20 7374 7265 6e67 7468  ction = strength
+0000b7e0: 5f66 756e 6374 696f 6e29 0a0a 7269 7665  _function)..rive
+0000b7f0: 725f 7072 6f70 6572 7469 6573 203d 2056  r_properties = V
+0000b800: 6f74 696e 674d 6574 686f 6450 726f 7065  otingMethodPrope
+0000b810: 7274 6965 7328 0a20 2020 2063 6f6e 646f  rties(.    condo
+0000b820: 7263 6574 5f77 696e 6e65 723d 5472 7565  rcet_winner=True
+0000b830: 2c20 0a20 2020 2063 6f6e 646f 7263 6574  , .    condorcet
+0000b840: 5f6c 6f73 6572 3d54 7275 652c 0a20 2020  _loser=True,.   
+0000b850: 2070 6172 6574 6f5f 646f 6d69 6e61 6e63   pareto_dominanc
+0000b860: 653d 5472 7565 2c0a 2020 2020 706f 7369  e=True,.    posi
+0000b870: 7469 7665 5f69 6e76 6f6c 7665 6d65 6e74  tive_involvement
+0000b880: 3d46 616c 7365 2c20 0a20 2020 2029 0a40  =False, .    ).@
+0000b890: 766d 286e 616d 653d 2252 6976 6572 222c  vm(name="River",
+0000b8a0: 0a20 2020 2070 726f 7065 7274 6965 733d  .    properties=
+0000b8b0: 7269 7665 725f 7072 6f70 6572 7469 6573  river_properties
+0000b8c0: 2c0a 2020 2020 696e 7075 745f 7479 7065  ,.    input_type
+0000b8d0: 733d 5b45 6c65 6374 696f 6e54 7970 6573  s=[ElectionTypes
+0000b8e0: 2e50 524f 4649 4c45 2c20 456c 6563 7469  .PROFILE, Electi
+0000b8f0: 6f6e 5479 7065 732e 5052 4f46 494c 455f  onTypes.PROFILE_
+0000b900: 5749 5448 5f54 4945 532c 2045 6c65 6374  WITH_TIES, Elect
+0000b910: 696f 6e54 7970 6573 2e4d 4152 4749 4e5f  ionTypes.MARGIN_
+0000b920: 4752 4150 485d 290a 6465 6620 7269 7665  GRAPH]).def rive
+0000b930: 7228 6564 6174 612c 2063 7572 725f 6361  r(edata, curr_ca
+0000b940: 6e64 7320 3d20 4e6f 6e65 2c20 7374 7265  nds = None, stre
+0000b950: 6e67 7468 5f66 756e 6374 696f 6e20 3d20  ngth_function = 
+0000b960: 4e6f 6e65 293a 2020 200a 2020 2020 2222  None):   .    ""
+0000b970: 220a 2020 2020 4f72 6465 7220 7468 6520  ".    Order the 
+0000b980: 6564 6765 7320 696e 2074 6865 2077 6561  edges in the wea
+0000b990: 6b20 6d61 7267 696e 2067 7261 7068 2066  k margin graph f
+0000b9a0: 726f 6d20 6c61 7267 6573 7420 746f 2073  rom largest to s
+0000b9b0: 6d61 6c6c 6573 7420 616e 6420 6c6f 636b  mallest and lock
+0000b9c0: 2074 6865 6d20 696e 2069 6e20 7468 6174   them in in that
+0000b9d0: 206f 7264 6572 2c20 736b 6970 7069 6e67   order, skipping
+0000b9e0: 2065 6467 6573 2074 6861 7420 6372 6561   edges that crea
+0000b9f0: 7465 2061 2063 7963 6c65 202a 616e 6420  te a cycle *and 
+0000ba00: 6564 6765 7320 696e 2077 6869 6368 2074  edges in which t
+0000ba10: 6865 7265 2069 7320 616c 7265 6164 7920  here is already 
+0000ba20: 616e 2065 6467 6520 706f 696e 7469 6e67  an edge pointing
+0000ba30: 2074 6f20 7468 6520 7461 7267 6574 2a2e   to the target*.
+0000ba40: 2020 4272 6561 6b20 7469 6573 2075 7369    Break ties usi
+0000ba50: 6e67 2061 2074 6965 2d62 7265 616b 696e  ng a tie-breakin
+0000ba60: 6720 206c 696e 6561 7220 6f72 6465 7269  g  linear orderi
+0000ba70: 6e67 206f 7665 7220 7468 6520 6564 6765  ng over the edge
+0000ba80: 732e 2020 4120 6361 6e64 6964 6174 6520  s.  A candidate 
+0000ba90: 6973 2061 2052 6976 6572 2077 696e 6e65  is a River winne
+0000baa0: 7220 6966 2069 7420 7769 6e73 2061 6363  r if it wins acc
+0000bab0: 6f72 6469 6e67 2074 6f20 736f 6d65 2074  ording to some t
+0000bac0: 6965 2d62 7265 616b 696e 6720 7275 6c65  ie-breaking rule
+0000bad0: 2e20 5365 6520 6874 7470 733a 2f2f 656c  . See https://el
+0000bae0: 6563 746f 7769 6b69 2e6f 7267 2f77 696b  ectowiki.org/wik
+0000baf0: 692f 5269 7665 722e 0a0a 2020 2020 4172  i/River...    Ar
+0000bb00: 6773 3a0a 2020 2020 2020 2020 6564 6174  gs:.        edat
+0000bb10: 6120 2850 726f 6669 6c65 2c20 5072 6f66  a (Profile, Prof
+0000bb20: 696c 6557 6974 6854 6965 732c 204d 6172  ileWithTies, Mar
+0000bb30: 6769 6e47 7261 7068 293a 2041 6e79 2065  ginGraph): Any e
+0000bb40: 6c65 6374 696f 6e20 6461 7461 2074 6861  lection data tha
+0000bb50: 7420 6861 7320 6120 606d 6172 6769 6e60  t has a `margin`
+0000bb60: 206d 6574 686f 642e 200a 2020 2020 2020   method. .      
+0000bb70: 2020 6375 7272 5f63 616e 6473 2028 4c69    curr_cands (Li
+0000bb80: 7374 5b69 6e74 5d2c 206f 7074 696f 6e61  st[int], optiona
+0000bb90: 6c29 3a20 4966 2073 6574 2c20 7468 656e  l): If set, then
+0000bba0: 2066 696e 6420 7468 6520 7769 6e6e 6572   find the winner
+0000bbb0: 7320 666f 7220 7468 6520 7072 6f66 696c  s for the profil
+0000bbc0: 6520 7265 7374 7269 6374 6564 2074 6f20  e restricted to 
+0000bbd0: 7468 6520 6361 6e64 6964 6174 6573 2069  the candidates i
+0000bbe0: 6e20 6060 6375 7272 5f63 616e 6473 6060  n ``curr_cands``
+0000bbf0: 0a20 2020 2020 2020 2073 7472 656e 6774  .        strengt
+0000bc00: 685f 6675 6e63 7469 6f6e 2028 6675 6e63  h_function (func
+0000bc10: 7469 6f6e 2c20 6f70 7469 6f6e 616c 293a  tion, optional):
+0000bc20: 2054 6865 2073 7472 656e 6774 6820 6675   The strength fu
+0000bc30: 6e63 7469 6f6e 2074 6f20 6265 2075 7365  nction to be use
+0000bc40: 6420 746f 2063 616c 6375 6c61 7465 2074  d to calculate t
+0000bc50: 6865 2073 7472 656e 6774 6820 6f66 2061  he strength of a
+0000bc60: 2070 6174 682e 2020 2054 6865 2064 6566   path.   The def
+0000bc70: 6175 6c74 2069 7320 7468 6520 6d61 7267  ault is the marg
+0000bc80: 696e 206d 6574 686f 6420 6f66 2060 6065  in method of ``e
+0000bc90: 6461 7461 6060 2e20 2020 5468 6973 206f  data``.   This o
+0000bca0: 6e6c 7920 6d61 7474 6572 7320 7768 656e  nly matters when
+0000bcb0: 2074 6865 2062 616c 6c6f 7473 2061 7265   the ballots are
+0000bcc0: 206e 6f74 206c 696e 6561 7220 6f72 6465   not linear orde
+0000bcd0: 7273 2e20 0a0a 2020 2020 5265 7475 726e  rs. ..    Return
+0000bce0: 733a 200a 2020 2020 2020 2020 4120 736f  s: .        A so
+0000bcf0: 7274 6564 206c 6973 7420 6f66 2063 616e  rted list of can
+0000bd00: 6469 6461 7465 732e 200a 0a20 2020 203a  didates. ..    :
+0000bd10: 4578 616d 706c 653a 200a 0a20 2020 202e  Example: ..    .
+0000bd20: 2e20 6578 6563 5f63 6f64 653a 3a20 0a0a  . exec_code:: ..
+0000bd30: 2020 2020 2020 2020 6672 6f6d 2070 7265          from pre
+0000bd40: 665f 766f 7469 6e67 2e77 6569 6768 7465  f_voting.weighte
+0000bd50: 645f 6d61 6a6f 7269 7479 5f67 7261 7068  d_majority_graph
+0000bd60: 7320 696d 706f 7274 204d 6172 6769 6e47  s import MarginG
+0000bd70: 7261 7068 0a20 2020 2020 2020 2066 726f  raph.        fro
+0000bd80: 6d20 7072 6566 5f76 6f74 696e 672e 6d61  m pref_voting.ma
+0000bd90: 7267 696e 5f62 6173 6564 5f6d 6574 686f  rgin_based_metho
+0000bda0: 6473 2069 6d70 6f72 7420 7269 7665 722c  ds import river,
+0000bdb0: 2072 616e 6b65 645f 7061 6972 730a 2020   ranked_pairs.  
+0000bdc0: 2020 2020 2020 0a20 2020 2020 2020 206d        .        m
+0000bdd0: 6720 3d20 4d61 7267 696e 4772 6170 6828  g = MarginGraph(
+0000bde0: 5b30 2c20 312c 2032 2c20 335d 2c20 5b28  [0, 1, 2, 3], [(
+0000bdf0: 302c 2032 2c20 3229 2c20 2830 2c20 332c  0, 2, 2), (0, 3,
+0000be00: 2038 292c 2028 312c 2030 2c20 3132 292c   8), (1, 0, 12),
+0000be10: 2028 322c 2033 2c20 3132 292c 2028 332c   (2, 3, 12), (3,
+0000be20: 2031 2c20 3629 5d29 0a0a 2020 2020 2020   1, 6)])..      
+0000be30: 2020 7261 6e6b 6564 5f70 6169 7273 2e64    ranked_pairs.d
+0000be40: 6973 706c 6179 286d 6729 0a20 2020 2020  isplay(mg).     
+0000be50: 2020 2072 6976 6572 2e64 6973 706c 6179     river.display
+0000be60: 286d 6729 0a0a 2020 2020 2222 220a 2020  (mg)..    """.  
+0000be70: 2020 6361 6e64 6964 6174 6573 203d 2065    candidates = e
+0000be80: 6461 7461 2e63 616e 6469 6461 7465 7320  data.candidates 
+0000be90: 6966 2063 7572 725f 6361 6e64 7320 6973  if curr_cands is
+0000bea0: 204e 6f6e 6520 656c 7365 2063 7572 725f   None else curr_
+0000beb0: 6361 6e64 7320 2020 200a 2020 2020 6369  cands    .    ci
+0000bec0: 6478 5f74 6f5f 6361 6e64 203d 207b 6369  dx_to_cand = {ci
+0000bed0: 6478 3a20 6320 666f 7220 6369 6478 2c20  dx: c for cidx, 
+0000bee0: 6320 696e 2065 6e75 6d65 7261 7465 2863  c in enumerate(c
+0000bef0: 616e 6469 6461 7465 7329 7d20 200a 2020  andidates)}  .  
+0000bf00: 2020 6361 6e64 5f74 6f5f 6369 6478 203d    cand_to_cidx =
+0000bf10: 207b 633a 2063 6964 7820 666f 7220 6369   {c: cidx for ci
+0000bf20: 6478 2c20 6320 696e 2065 6e75 6d65 7261  dx, c in enumera
+0000bf30: 7465 2863 616e 6469 6461 7465 7329 7d20  te(candidates)} 
+0000bf40: 200a 0a20 2020 2073 7472 656e 6774 685f   ..    strength_
+0000bf50: 6675 6e63 7469 6f6e 203d 2065 6461 7461  function = edata
+0000bf60: 2e6d 6172 6769 6e20 6966 2073 7472 656e  .margin if stren
+0000bf70: 6774 685f 6675 6e63 7469 6f6e 2069 7320  gth_function is 
+0000bf80: 4e6f 6e65 2065 6c73 6520 7374 7265 6e67  None else streng
+0000bf90: 7468 5f66 756e 6374 696f 6e20 2020 200a  th_function    .
+0000bfa0: 0a20 2020 2063 7720 3d20 6564 6174 612e  .    cw = edata.
+0000bfb0: 636f 6e64 6f72 6365 745f 7769 6e6e 6572  condorcet_winner
+0000bfc0: 2863 7572 725f 6361 6e64 733d 6375 7272  (curr_cands=curr
+0000bfd0: 5f63 616e 6473 290a 2020 2020 2320 5261  _cands).    # Ra
+0000bfe0: 6e6b 6564 2050 6169 7273 2069 7320 436f  nked Pairs is Co
+0000bff0: 6e64 6f72 6365 7420 636f 6e73 6973 7465  ndorcet consiste
+0000c000: 6e74 2c20 736f 2073 696d 706c 7920 7265  nt, so simply re
+0000c010: 7475 726e 2074 6865 2043 6f6e 646f 7263  turn the Condorc
+0000c020: 6574 2077 696e 6e65 7220 6966 2065 7869  et winner if exi
+0000c030: 7374 730a 2020 2020 6966 2063 7720 6973  sts.    if cw is
+0000c040: 206e 6f74 204e 6f6e 653a 200a 2020 2020   not None: .    
+0000c050: 2020 2020 7769 6e6e 6572 7320 3d20 5b63      winners = [c
+0000c060: 775d 0a20 2020 2065 6c73 653a 0a20 2020  w].    else:.   
+0000c070: 2020 2020 2077 5f65 6467 6573 203d 205b       w_edges = [
+0000c080: 2863 312c 2063 322c 2073 7472 656e 6774  (c1, c2, strengt
+0000c090: 685f 6675 6e63 7469 6f6e 2863 312c 2063  h_function(c1, c
+0000c0a0: 3229 2920 666f 7220 6331 2069 6e20 6361  2)) for c1 in ca
+0000c0b0: 6e64 6964 6174 6573 2066 6f72 2063 3220  ndidates for c2 
+0000c0c0: 696e 2063 616e 6469 6461 7465 7320 0a20  in candidates . 
+0000c0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c0e0: 2020 6966 2063 3120 213d 2063 3220 616e    if c1 != c2 an
+0000c0f0: 6420 2865 6461 7461 2e6d 616a 6f72 6974  d (edata.majorit
+0000c100: 795f 7072 6566 6572 7328 6331 2c20 6332  y_prefers(c1, c2
+0000c110: 2920 6f72 2065 6461 7461 2e69 735f 7469  ) or edata.is_ti
+0000c120: 6564 2863 312c 2063 3229 295d 0a20 2020  ed(c1, c2))].   
+0000c130: 2020 2020 2077 696e 6e65 7273 203d 206c       winners = l
+0000c140: 6973 7428 2920 2020 2020 2020 2020 2020  ist()           
+0000c150: 200a 2020 2020 2020 2020 7374 7265 6e67   .        streng
+0000c160: 7468 7320 3d20 736f 7274 6564 286c 6973  ths = sorted(lis
+0000c170: 7428 7365 7428 5b65 5b32 5d20 666f 7220  t(set([e[2] for 
+0000c180: 6520 696e 2077 5f65 6467 6573 5d29 292c  e in w_edges])),
+0000c190: 2072 6576 6572 7365 3d54 7275 6529 0a20   reverse=True). 
+0000c1a0: 2020 2020 2020 2073 6f72 7465 645f 6564         sorted_ed
+0000c1b0: 6765 7320 3d20 5b5b 6520 666f 7220 6520  ges = [[e for e 
+0000c1c0: 696e 2077 5f65 6467 6573 2069 6620 655b  in w_edges if e[
+0000c1d0: 325d 203d 3d20 735d 2066 6f72 2073 2069  2] == s] for s i
+0000c1e0: 6e20 7374 7265 6e67 7468 735d 0a20 2020  n strengths].   
+0000c1f0: 2020 2020 2074 6273 203d 2070 726f 6475       tbs = produ
+0000c200: 6374 282a 5b70 6572 6d75 7461 7469 6f6e  ct(*[permutation
+0000c210: 7328 6564 6765 7329 2066 6f72 2065 6467  s(edges) for edg
+0000c220: 6573 2069 6e20 736f 7274 6564 5f65 6467  es in sorted_edg
+0000c230: 6573 5d29 0a20 2020 2020 2020 2066 6f72  es]).        for
+0000c240: 2074 6220 696e 2074 6273 3a0a 2020 2020   tb in tbs:.    
+0000c250: 2020 2020 2020 2020 6564 6765 7320 3d20          edges = 
+0000c260: 666c 6174 7465 6e28 7462 290a 2020 2020  flatten(tb).    
+0000c270: 2020 2020 2020 2020 7276 5f64 6566 6561          rv_defea
+0000c280: 7420 3d20 5350 4f28 6c65 6e28 6361 6e64  t = SPO(len(cand
+0000c290: 6964 6174 6573 2929 0a20 2020 2020 2020  idates)).       
+0000c2a0: 2020 2020 2066 6f72 2065 302c 6531 2c73       for e0,e1,s
+0000c2b0: 2069 6e20 6564 6765 733a 200a 2020 2020   in edges: .    
+0000c2c0: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+0000c2d0: 6f74 2072 765f 6465 6665 6174 2e50 5b63  ot rv_defeat.P[c
+0000c2e0: 616e 645f 746f 5f63 6964 785b 6531 5d5d  and_to_cidx[e1]]
+0000c2f0: 5b63 616e 645f 746f 5f63 6964 785b 6530  [cand_to_cidx[e0
+0000c300: 5d5d 2061 6e64 206c 656e 2872 765f 6465  ]] and len(rv_de
+0000c310: 6665 6174 2e70 7265 6473 5b63 616e 645f  feat.preds[cand_
+0000c320: 746f 5f63 6964 785b 6531 5d5d 2920 3d3d  to_cidx[e1]]) ==
+0000c330: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
+0000c340: 2020 2020 2020 2020 7276 5f64 6566 6561          rv_defea
+0000c350: 742e 6164 6428 6361 6e64 5f74 6f5f 6369  t.add(cand_to_ci
+0000c360: 6478 5b65 305d 2c63 616e 645f 746f 5f63  dx[e0],cand_to_c
+0000c370: 6964 785b 6531 5d29 0a20 2020 2020 2020  idx[e1]).       
+0000c380: 2020 2020 2077 696e 6e65 7273 2e61 7070       winners.app
+0000c390: 656e 6428 6369 6478 5f74 6f5f 6361 6e64  end(cidx_to_cand
+0000c3a0: 5b72 765f 6465 6665 6174 2e69 6e69 7469  [rv_defeat.initi
+0000c3b0: 616c 5f65 6c65 6d65 6e74 7328 295b 305d  al_elements()[0]
+0000c3c0: 5d29 0a0a 2020 2020 7265 7475 726e 2073  ])..    return s
+0000c3d0: 6f72 7465 6428 6c69 7374 2873 6574 2877  orted(list(set(w
+0000c3e0: 696e 6e65 7273 2929 290a 0a64 6566 2072  inners)))..def r
+0000c3f0: 6976 6572 5f64 6566 6561 7473 2865 6461  iver_defeats(eda
+0000c400: 7461 2c20 6375 7272 5f63 616e 6473 203d  ta, curr_cands =
+0000c410: 204e 6f6e 652c 2073 7472 656e 6774 685f   None, strength_
+0000c420: 6675 6e63 7469 6f6e 203d 204e 6f6e 6529  function = None)
+0000c430: 3a0a 2020 2020 2222 220a 2020 2020 5265  :.    """.    Re
+0000c440: 7475 726e 7320 7468 6520 5269 7665 7220  turns the River 
+0000c450: 6465 6665 6174 2072 656c 6174 696f 6e73  defeat relations
+0000c460: 2070 726f 6475 6365 6420 6279 2074 6865   produced by the
+0000c470: 2052 6976 6572 2061 6c67 6f72 6974 686d   River algorithm
+0000c480: 2e0a 0a20 2020 202e 2e20 696d 706f 7274  ...    .. import
+0000c490: 616e 743a 3a0a 2020 2020 2020 2020 556e  ant::.        Un
+0000c4a0: 6c69 6b65 2074 6865 206f 7468 6572 2066  like the other f
+0000c4b0: 756e 6374 696f 6e73 2074 6861 7420 7265  unctions that re
+0000c4c0: 7475 726e 2061 2073 696e 676c 6520 6465  turn a single de
+0000c4d0: 6665 6174 2072 656c 6174 696f 6e2c 2074  feat relation, t
+0000c4e0: 6869 7320 7265 7475 726e 7320 6120 6c69  his returns a li
+0000c4f0: 7374 206f 6620 6465 6665 6174 2072 656c  st of defeat rel
+0000c500: 6174 696f 6e73 2e20 0a20 2020 2020 2020  ations. .       
+0000c510: 200a 2020 2020 4172 6773 3a0a 2020 2020   .    Args:.    
+0000c520: 2020 2020 6564 6174 6120 2850 726f 6669      edata (Profi
+0000c530: 6c65 2c20 5072 6f66 696c 6557 6974 6854  le, ProfileWithT
+0000c540: 6965 732c 204d 6172 6769 6e47 7261 7068  ies, MarginGraph
+0000c550: 293a 2041 6e79 2065 6c65 6374 696f 6e20  ): Any election 
+0000c560: 6461 7461 2074 6861 7420 6861 7320 6120  data that has a 
+0000c570: 606d 6172 6769 6e60 206d 6574 686f 642e  `margin` method.
+0000c580: 200a 2020 2020 2020 2020 6375 7272 5f63   .        curr_c
+0000c590: 616e 6473 2028 4c69 7374 5b69 6e74 5d2c  ands (List[int],
+0000c5a0: 206f 7074 696f 6e61 6c29 3a20 4966 2073   optional): If s
+0000c5b0: 6574 2c20 7468 656e 2066 696e 6420 7468  et, then find th
+0000c5c0: 6520 7769 6e6e 6572 7320 666f 7220 7468  e winners for th
+0000c5d0: 6520 7072 6f66 696c 6520 7265 7374 7269  e profile restri
+0000c5e0: 6374 6564 2074 6f20 7468 6520 6361 6e64  cted to the cand
+0000c5f0: 6964 6174 6573 2069 6e20 6060 6375 7272  idates in ``curr
+0000c600: 5f63 616e 6473 6060 0a20 2020 2020 2020  _cands``.       
+0000c610: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
+0000c620: 6f6e 2028 6675 6e63 7469 6f6e 2c20 6f70  on (function, op
+0000c630: 7469 6f6e 616c 293a 2054 6865 2073 7472  tional): The str
+0000c640: 656e 6774 6820 6675 6e63 7469 6f6e 2074  ength function t
+0000c650: 6f20 6265 2075 7365 6420 746f 2063 616c  o be used to cal
+0000c660: 6375 6c61 7465 2074 6865 2073 7472 656e  culate the stren
+0000c670: 6774 6820 6f66 2061 2070 6174 682e 2020  gth of a path.  
+0000c680: 2054 6865 2064 6566 6175 6c74 2069 7320   The default is 
+0000c690: 7468 6520 6d61 7267 696e 206d 6574 686f  the margin metho
+0000c6a0: 6420 6f66 2060 6065 6461 7461 6060 2e20  d of ``edata``. 
+0000c6b0: 2020 5468 6973 206f 6e6c 7920 6d61 7474    This only matt
+0000c6c0: 6572 7320 7768 656e 2074 6865 2062 616c  ers when the bal
+0000c6d0: 6c6f 7473 2061 7265 206e 6f74 206c 696e  lots are not lin
+0000c6e0: 6561 7220 6f72 6465 7273 2e20 0a0a 2020  ear orders. ..  
+0000c6f0: 2020 5265 7475 726e 733a 200a 2020 2020    Returns: .    
+0000c700: 2020 2020 4120 6e65 7477 6f72 6b78 2044      A networkx D
+0000c710: 6947 7261 7068 2072 6570 7265 7365 6e74  iGraph represent
+0000c720: 696e 6720 7468 6520 5269 7665 7220 6465  ing the River de
+0000c730: 6665 6174 2072 656c 6174 696f 6e2e 200a  feat relation. .
+0000c740: 2020 2020 2222 220a 0a20 2020 2063 616e      """..    can
+0000c750: 6469 6461 7465 7320 3d20 6564 6174 612e  didates = edata.
+0000c760: 6361 6e64 6964 6174 6573 2069 6620 6375  candidates if cu
+0000c770: 7272 5f63 616e 6473 2069 7320 4e6f 6e65  rr_cands is None
+0000c780: 2065 6c73 6520 6375 7272 5f63 616e 6473   else curr_cands
+0000c790: 2020 2020 0a20 2020 2073 7472 656e 6774      .    strengt
+0000c7a0: 685f 6675 6e63 7469 6f6e 203d 2065 6461  h_function = eda
+0000c7b0: 7461 2e6d 6172 6769 6e20 6966 2073 7472  ta.margin if str
+0000c7c0: 656e 6774 685f 6675 6e63 7469 6f6e 2069  ength_function i
+0000c7d0: 7320 4e6f 6e65 2065 6c73 6520 7374 7265  s None else stre
+0000c7e0: 6e67 7468 5f66 756e 6374 696f 6e20 2020  ngth_function   
+0000c7f0: 200a 0a20 2020 2077 5f65 6467 6573 203d   ..    w_edges =
+0000c800: 205b 2863 312c 2063 322c 2073 7472 656e   [(c1, c2, stren
+0000c810: 6774 685f 6675 6e63 7469 6f6e 2863 312c  gth_function(c1,
+0000c820: 2063 3229 2920 666f 7220 6331 2069 6e20   c2)) for c1 in 
+0000c830: 6361 6e64 6964 6174 6573 2066 6f72 2063  candidates for c
+0000c840: 3220 696e 2063 616e 6469 6461 7465 7320  2 in candidates 
+0000c850: 6966 2063 3120 213d 2063 3220 616e 6420  if c1 != c2 and 
+0000c860: 2865 6461 7461 2e6d 616a 6f72 6974 795f  (edata.majority_
+0000c870: 7072 6566 6572 7328 6331 2c20 6332 2920  prefers(c1, c2) 
+0000c880: 6f72 2065 6461 7461 2e69 735f 7469 6564  or edata.is_tied
+0000c890: 2863 312c 2063 3229 295d 0a0a 2020 2020  (c1, c2))]..    
+0000c8a0: 7374 7265 6e67 7468 7320 3d20 736f 7274  strengths = sort
+0000c8b0: 6564 286c 6973 7428 7365 7428 5b65 5b32  ed(list(set([e[2
+0000c8c0: 5d20 666f 7220 6520 696e 2077 5f65 6467  ] for e in w_edg
+0000c8d0: 6573 5d29 292c 2072 6576 6572 7365 3d54  es])), reverse=T
+0000c8e0: 7275 6529 0a20 2020 2073 6f72 7465 645f  rue).    sorted_
+0000c8f0: 6564 6765 7320 3d20 5b5b 6520 666f 7220  edges = [[e for 
+0000c900: 6520 696e 2077 5f65 6467 6573 2069 6620  e in w_edges if 
+0000c910: 655b 325d 203d 3d20 735d 2066 6f72 2073  e[2] == s] for s
+0000c920: 2069 6e20 7374 7265 6e67 7468 735d 0a20   in strengths]. 
+0000c930: 2020 2074 6273 203d 2070 726f 6475 6374     tbs = product
+0000c940: 282a 5b70 6572 6d75 7461 7469 6f6e 7328  (*[permutations(
+0000c950: 6564 6765 7329 2066 6f72 2065 6467 6573  edges) for edges
+0000c960: 2069 6e20 736f 7274 6564 5f65 6467 6573   in sorted_edges
+0000c970: 5d29 0a0a 2020 2020 7269 7665 725f 6465  ])..    river_de
+0000c980: 6665 6174 7320 3d20 6c69 7374 2829 0a20  feats = list(). 
+0000c990: 2020 2066 6f72 2074 6220 696e 2074 6273     for tb in tbs
+0000c9a0: 3a0a 2020 2020 2020 2020 6564 6765 7320  :.        edges 
+0000c9b0: 3d20 666c 6174 7465 6e28 7462 290a 2020  = flatten(tb).  
+0000c9c0: 2020 2020 2020 7269 7665 725f 6465 6665        river_defe
+0000c9d0: 6174 203d 206e 782e 4469 4772 6170 6828  at = nx.DiGraph(
+0000c9e0: 2920 0a20 2020 2020 2020 2066 6f72 2065  ) .        for e
+0000c9f0: 2069 6e20 6564 6765 733a 200a 2020 2020   in edges: .    
+0000ca00: 2020 2020 2020 2020 6966 2065 5b31 5d20          if e[1] 
+0000ca10: 6e6f 7420 696e 2072 6976 6572 5f64 6566  not in river_def
+0000ca20: 6561 742e 6e6f 6465 7320 6f72 206c 656e  eat.nodes or len
+0000ca30: 286c 6973 7428 7269 7665 725f 6465 6665  (list(river_defe
+0000ca40: 6174 2e69 6e5f 6564 6765 7328 655b 315d  at.in_edges(e[1]
+0000ca50: 2929 2920 3d3d 2030 3a0a 2020 2020 2020  ))) == 0:.      
+0000ca60: 2020 2020 2020 2020 2020 7269 7665 725f            river_
+0000ca70: 6465 6665 6174 2e61 6464 5f65 6467 6528  defeat.add_edge(
+0000ca80: 655b 305d 2c20 655b 315d 2c20 7765 6967  e[0], e[1], weig
+0000ca90: 6874 3d65 5b32 5d29 0a20 2020 2020 2020  ht=e[2]).       
+0000caa0: 2020 2020 2020 2020 2069 6620 646f 6573           if does
+0000cab0: 5f63 7265 6174 655f 6379 636c 6528 7269  _create_cycle(ri
+0000cac0: 7665 725f 6465 6665 6174 2c20 6529 3a0a  ver_defeat, e):.
+0000cad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cae0: 2020 2020 7269 7665 725f 6465 6665 6174      river_defeat
+0000caf0: 2e72 656d 6f76 655f 6564 6765 2865 5b30  .remove_edge(e[0
+0000cb00: 5d2c 2065 5b31 5d29 0a20 2020 2020 2020  ], e[1]).       
+0000cb10: 2020 2020 200a 2020 2020 2020 2020 7269       .        ri
+0000cb20: 7665 725f 6465 6665 6174 732e 6170 7065  ver_defeats.appe
+0000cb30: 6e64 2872 6976 6572 5f64 6566 6561 7429  nd(river_defeat)
+0000cb40: 0a0a 2020 2020 7265 7475 726e 2072 6976  ..    return riv
+0000cb50: 6572 5f64 6566 6561 7473 0a0a 4076 6d28  er_defeats..@vm(
+0000cb60: 6e61 6d65 3d22 5269 7665 7222 2c0a 2020  name="River",.  
+0000cb70: 2020 736b 6970 5f72 6567 6973 7472 6174    skip_registrat
+0000cb80: 696f 6e3d 5472 7565 290a 6465 6620 7269  ion=True).def ri
+0000cb90: 7665 725f 7769 7468 5f74 6573 7428 6564  ver_with_test(ed
+0000cba0: 6174 612c 2063 7572 725f 6361 6e64 7320  ata, curr_cands 
+0000cbb0: 3d20 4e6f 6e65 2c20 7374 7265 6e67 7468  = None, strength
+0000cbc0: 5f66 756e 6374 696f 6e20 3d20 4e6f 6e65  _function = None
+0000cbd0: 293a 2020 200a 2020 2020 2222 2246 696e  ):   .    """Fin
+0000cbe0: 6420 7468 6520 5269 7665 7220 7769 6e6e  d the River winn
+0000cbf0: 6572 7320 7769 7468 2061 2074 6573 7420  ers with a test 
+0000cc00: 746f 2064 6574 6572 6d69 6e65 6420 6966  to determined if
+0000cc10: 2069 7420 7769 6c6c 2074 616b 6520 746f   it will take to
+0000cc20: 6f20 6c6f 6e67 2074 6f20 636f 6d70 7574  o long to comput
+0000cc30: 6520 7468 6520 5269 7665 7220 7769 6e6e  e the River winn
+0000cc40: 6572 732e 2049 6620 7468 6520 6361 6c63  ers. If the calc
+0000cc50: 756c 6174 696f 6e20 6f66 2074 6865 2077  ulation of the w
+0000cc60: 696e 6e65 7273 2077 696c 6c20 7461 6b65  inners will take
+0000cc70: 2074 6f6f 206c 6f6e 672c 2072 6574 7572   too long, retur
+0000cc80: 6e20 4e6f 6e65 2e20 0a20 2020 2020 2020  n None. .       
+0000cc90: 200a 2020 2020 2e2e 2069 6d70 6f72 7461   .    .. importa
+0000cca0: 6e74 3a3a 0a20 2020 2020 2020 2054 6869  nt::.        Thi
+0000ccb0: 7320 766f 7469 6e67 206d 6574 686f 6420  s voting method 
+0000ccc0: 7468 6174 206d 6967 6874 2072 6574 7572  that might retur
+0000ccd0: 6e20 4e6f 6e65 2072 6174 6865 7220 7468  n None rather th
+0000cce0: 616e 2061 206c 6973 7420 6f66 2063 616e  an a list of can
+0000ccf0: 6469 6461 7465 732e 2020 0a0a 2020 2020  didates.  ..    
+0000cd00: 4172 6773 3a0a 2020 2020 2020 2020 6564  Args:.        ed
+0000cd10: 6174 6120 2850 726f 6669 6c65 2c20 5072  ata (Profile, Pr
+0000cd20: 6f66 696c 6557 6974 6854 6965 732c 204d  ofileWithTies, M
+0000cd30: 6172 6769 6e47 7261 7068 293a 2041 6e79  arginGraph): Any
+0000cd40: 2065 6c65 6374 696f 6e20 6461 7461 2074   election data t
+0000cd50: 6861 7420 6861 7320 6120 606d 6172 6769  hat has a `margi
+0000cd60: 6e60 206d 6574 686f 642e 200a 2020 2020  n` method. .    
+0000cd70: 2020 2020 6375 7272 5f63 616e 6473 2028      curr_cands (
+0000cd80: 4c69 7374 5b69 6e74 5d2c 206f 7074 696f  List[int], optio
+0000cd90: 6e61 6c29 3a20 4966 2073 6574 2c20 7468  nal): If set, th
+0000cda0: 656e 2066 696e 6420 7468 6520 7769 6e6e  en find the winn
+0000cdb0: 6572 7320 666f 7220 7468 6520 7072 6f66  ers for the prof
+0000cdc0: 696c 6520 7265 7374 7269 6374 6564 2074  ile restricted t
+0000cdd0: 6f20 7468 6520 6361 6e64 6964 6174 6573  o the candidates
+0000cde0: 2069 6e20 6060 6375 7272 5f63 616e 6473   in ``curr_cands
+0000cdf0: 6060 0a20 2020 2020 2020 2073 7472 656e  ``.        stren
+0000ce00: 6774 685f 6675 6e63 7469 6f6e 2028 6675  gth_function (fu
+0000ce10: 6e63 7469 6f6e 2c20 6f70 7469 6f6e 616c  nction, optional
+0000ce20: 293a 2054 6865 2073 7472 656e 6774 6820  ): The strength 
+0000ce30: 6675 6e63 7469 6f6e 2074 6f20 6265 2075  function to be u
+0000ce40: 7365 6420 746f 2063 616c 6375 6c61 7465  sed to calculate
+0000ce50: 2074 6865 2073 7472 656e 6774 6820 6f66   the strength of
+0000ce60: 2061 2070 6174 682e 2020 2054 6865 2064   a path.   The d
+0000ce70: 6566 6175 6c74 2069 7320 7468 6520 6d61  efault is the ma
+0000ce80: 7267 696e 206d 6574 686f 6420 6f66 2060  rgin method of `
+0000ce90: 6065 6461 7461 6060 2e20 2020 5468 6973  `edata``.   This
+0000cea0: 206f 6e6c 7920 6d61 7474 6572 7320 7768   only matters wh
+0000ceb0: 656e 2074 6865 2062 616c 6c6f 7473 2061  en the ballots a
+0000cec0: 7265 206e 6f74 206c 696e 6561 7220 6f72  re not linear or
+0000ced0: 6465 7273 2e20 0a0a 2020 2020 5265 7475  ders. ..    Retu
+0000cee0: 726e 733a 200a 2020 2020 2020 2020 4120  rns: .        A 
+0000cef0: 736f 7274 6564 206c 6973 7420 6f66 2063  sorted list of c
+0000cf00: 616e 6469 6461 7465 732e 200a 0a20 2020  andidates. ..   
+0000cf10: 202e 2e20 7365 6561 6c73 6f3a 3a0a 0a20   .. seealso::.. 
+0000cf20: 2020 2020 2020 203a 6d65 7468 3a60 7072         :meth:`pr
+0000cf30: 6566 5f76 6f74 696e 672e 6d61 7267 696e  ef_voting.margin
+0000cf40: 5f62 6173 6564 5f6d 6574 686f 6473 2e72  _based_methods.r
+0000cf50: 616e 6b65 645f 7061 6972 735f 7769 7468  anked_pairs_with
+0000cf60: 5f74 6573 7460 2c20 3a6d 6574 683a 6070  _test`, :meth:`p
+0000cf70: 7265 665f 766f 7469 6e67 2e6d 6172 6769  ref_voting.margi
+0000cf80: 6e5f 6261 7365 645f 6d65 7468 6f64 732e  n_based_methods.
+0000cf90: 7269 7665 7260 0a0a 2020 2020 2222 220a  river`..    """.
+0000cfa0: 2020 2020 6361 6e64 6964 6174 6573 203d      candidates =
+0000cfb0: 2065 6461 7461 2e63 616e 6469 6461 7465   edata.candidate
+0000cfc0: 7320 6966 2063 7572 725f 6361 6e64 7320  s if curr_cands 
+0000cfd0: 6973 204e 6f6e 6520 656c 7365 2063 7572  is None else cur
+0000cfe0: 725f 6361 6e64 7320 2020 200a 2020 2020  r_cands    .    
+0000cff0: 6369 6478 5f74 6f5f 6361 6e64 203d 207b  cidx_to_cand = {
+0000d000: 6369 6478 3a20 6320 666f 7220 6369 6478  cidx: c for cidx
+0000d010: 2c20 6320 696e 2065 6e75 6d65 7261 7465  , c in enumerate
+0000d020: 2863 616e 6469 6461 7465 7329 7d20 200a  (candidates)}  .
+0000d030: 2020 2020 6361 6e64 5f74 6f5f 6369 6478      cand_to_cidx
+0000d040: 203d 207b 633a 2063 6964 7820 666f 7220   = {c: cidx for 
+0000d050: 6369 6478 2c20 6320 696e 2065 6e75 6d65  cidx, c in enume
+0000d060: 7261 7465 2863 616e 6469 6461 7465 7329  rate(candidates)
+0000d070: 7d20 200a 0a20 2020 2073 7472 656e 6774  }  ..    strengt
+0000d080: 685f 6675 6e63 7469 6f6e 203d 2065 6461  h_function = eda
+0000d090: 7461 2e6d 6172 6769 6e20 6966 2073 7472  ta.margin if str
+0000d0a0: 656e 6774 685f 6675 6e63 7469 6f6e 2069  ength_function i
+0000d0b0: 7320 4e6f 6e65 2065 6c73 6520 7374 7265  s None else stre
+0000d0c0: 6e67 7468 5f66 756e 6374 696f 6e20 2020  ngth_function   
+0000d0d0: 200a 0a20 2020 2063 7720 3d20 6564 6174   ..    cw = edat
+0000d0e0: 612e 636f 6e64 6f72 6365 745f 7769 6e6e  a.condorcet_winn
+0000d0f0: 6572 2863 7572 725f 6361 6e64 733d 6375  er(curr_cands=cu
+0000d100: 7272 5f63 616e 6473 290a 2020 2020 2320  rr_cands).    # 
+0000d110: 5261 6e6b 6564 2050 6169 7273 2069 7320  Ranked Pairs is 
+0000d120: 436f 6e64 6f72 6365 7420 636f 6e73 6973  Condorcet consis
+0000d130: 7465 6e74 2c20 736f 2073 696d 706c 7920  tent, so simply 
+0000d140: 7265 7475 726e 2074 6865 2043 6f6e 646f  return the Condo
+0000d150: 7263 6574 2077 696e 6e65 7220 6966 2065  rcet winner if e
+0000d160: 7869 7374 730a 2020 2020 6966 2063 7720  xists.    if cw 
+0000d170: 6973 206e 6f74 204e 6f6e 653a 200a 2020  is not None: .  
+0000d180: 2020 2020 2020 7769 6e6e 6572 7320 3d20        winners = 
+0000d190: 5b63 775d 0a20 2020 2065 6c73 653a 0a20  [cw].    else:. 
+0000d1a0: 2020 2020 2020 2077 5f65 6467 6573 203d         w_edges =
+0000d1b0: 205b 2863 312c 2063 322c 2073 7472 656e   [(c1, c2, stren
+0000d1c0: 6774 685f 6675 6e63 7469 6f6e 2863 312c  gth_function(c1,
+0000d1d0: 2063 3229 2920 666f 7220 6331 2069 6e20   c2)) for c1 in 
+0000d1e0: 6361 6e64 6964 6174 6573 2066 6f72 2063  candidates for c
+0000d1f0: 3220 696e 2063 616e 6469 6461 7465 7320  2 in candidates 
+0000d200: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d210: 2020 2020 6966 2063 3120 213d 2063 3220      if c1 != c2 
+0000d220: 616e 6420 2865 6461 7461 2e6d 616a 6f72  and (edata.major
+0000d230: 6974 795f 7072 6566 6572 7328 6331 2c20  ity_prefers(c1, 
+0000d240: 6332 2920 6f72 2065 6461 7461 2e69 735f  c2) or edata.is_
+0000d250: 7469 6564 2863 312c 2063 3229 295d 0a20  tied(c1, c2))]. 
+0000d260: 2020 2020 2020 2077 696e 6e65 7273 203d         winners =
+0000d270: 206c 6973 7428 2920 2020 2020 2020 2020   list()         
+0000d280: 2020 200a 2020 2020 2020 2020 7374 7265     .        stre
+0000d290: 6e67 7468 7320 3d20 736f 7274 6564 286c  ngths = sorted(l
+0000d2a0: 6973 7428 7365 7428 5b65 5b32 5d20 666f  ist(set([e[2] fo
+0000d2b0: 7220 6520 696e 2077 5f65 6467 6573 5d29  r e in w_edges])
+0000d2c0: 292c 2072 6576 6572 7365 3d54 7275 6529  ), reverse=True)
+0000d2d0: 0a20 2020 2020 2020 2073 6f72 7465 645f  .        sorted_
+0000d2e0: 6564 6765 7320 3d20 5b5b 6520 666f 7220  edges = [[e for 
+0000d2f0: 6520 696e 2077 5f65 6467 6573 2069 6620  e in w_edges if 
+0000d300: 655b 325d 203d 3d20 735d 2066 6f72 2073  e[2] == s] for s
+0000d310: 2069 6e20 7374 7265 6e67 7468 735d 0a20   in strengths]. 
+0000d320: 2020 2020 2020 2069 6620 6e70 2e70 726f         if np.pro
+0000d330: 6428 5b6d 6174 682e 6661 6374 6f72 6961  d([math.factoria
+0000d340: 6c28 6c65 6e28 6573 2929 2066 6f72 2065  l(len(es)) for e
+0000d350: 7320 696e 2073 6f72 7465 645f 6564 6765  s in sorted_edge
+0000d360: 735d 2920 3e20 3330 3030 3a20 0a20 2020  s]) > 3000: .   
+0000d370: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0000d380: 4e6f 6e65 0a20 2020 2020 2020 2065 6c73  None.        els
+0000d390: 653a 200a 2020 2020 2020 2020 2020 2020  e: .            
+0000d3a0: 7462 7320 3d20 7072 6f64 7563 7428 2a5b  tbs = product(*[
+0000d3b0: 7065 726d 7574 6174 696f 6e73 2865 6467  permutations(edg
+0000d3c0: 6573 2920 666f 7220 6564 6765 7320 696e  es) for edges in
+0000d3d0: 2073 6f72 7465 645f 6564 6765 735d 290a   sorted_edges]).
+0000d3e0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+0000d3f0: 7462 2069 6e20 7462 733a 0a20 2020 2020  tb in tbs:.     
+0000d400: 2020 2020 2020 2020 2020 2065 6467 6573             edges
+0000d410: 203d 2066 6c61 7474 656e 2874 6229 0a20   = flatten(tb). 
+0000d420: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0000d430: 765f 6465 6665 6174 203d 2053 504f 286c  v_defeat = SPO(l
+0000d440: 656e 2863 616e 6469 6461 7465 7329 290a  en(candidates)).
+0000d450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d460: 666f 7220 6530 2c65 312c 7320 696e 2065  for e0,e1,s in e
+0000d470: 6467 6573 3a20 0a20 2020 2020 2020 2020  dges: .         
+0000d480: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
+0000d490: 7420 7276 5f64 6566 6561 742e 505b 6361  t rv_defeat.P[ca
+0000d4a0: 6e64 5f74 6f5f 6369 6478 5b65 315d 5d5b  nd_to_cidx[e1]][
+0000d4b0: 6361 6e64 5f74 6f5f 6369 6478 5b65 305d  cand_to_cidx[e0]
+0000d4c0: 5d20 616e 6420 6c65 6e28 7276 5f64 6566  ] and len(rv_def
+0000d4d0: 6561 742e 7072 6564 735b 6361 6e64 5f74  eat.preds[cand_t
+0000d4e0: 6f5f 6369 6478 5b65 315d 5d29 203d 3d20  o_cidx[e1]]) == 
+0000d4f0: 303a 0a20 2020 2020 2020 2020 2020 2020  0:.             
+0000d500: 2020 2020 2020 2020 2020 2072 765f 6465             rv_de
+0000d510: 6665 6174 2e61 6464 2863 616e 645f 746f  feat.add(cand_to
+0000d520: 5f63 6964 785b 6530 5d2c 6361 6e64 5f74  _cidx[e0],cand_t
+0000d530: 6f5f 6369 6478 5b65 315d 290a 2020 2020  o_cidx[e1]).    
+0000d540: 2020 2020 2020 2020 2020 2020 7769 6e6e              winn
+0000d550: 6572 732e 6170 7065 6e64 2863 6964 785f  ers.append(cidx_
+0000d560: 746f 5f63 616e 645b 7276 5f64 6566 6561  to_cand[rv_defea
+0000d570: 742e 696e 6974 6961 6c5f 656c 656d 656e  t.initial_elemen
+0000d580: 7473 2829 5b30 5d5d 290a 2020 2020 7265  ts()[0]]).    re
+0000d590: 7475 726e 2073 6f72 7465 6428 6c69 7374  turn sorted(list
+0000d5a0: 2873 6574 2877 696e 6e65 7273 2929 290a  (set(winners))).
+0000d5b0: 0a72 705f 7462 5f70 726f 7065 7274 6965  .rp_tb_propertie
+0000d5c0: 7320 3d20 566f 7469 6e67 4d65 7468 6f64  s = VotingMethod
+0000d5d0: 5072 6f70 6572 7469 6573 280a 2020 2020  Properties(.    
+0000d5e0: 636f 6e64 6f72 6365 745f 7769 6e6e 6572  condorcet_winner
+0000d5f0: 3d54 7275 652c 200a 2020 2020 636f 6e64  =True, .    cond
+0000d600: 6f72 6365 745f 6c6f 7365 723d 5472 7565  orcet_loser=True
+0000d610: 2c0a 2020 2020 7061 7265 746f 5f64 6f6d  ,.    pareto_dom
+0000d620: 696e 616e 6365 3d54 7275 652c 0a20 2020  inance=True,.   
+0000d630: 2070 6f73 6974 6976 655f 696e 766f 6c76   positive_involv
+0000d640: 656d 656e 743d 4661 6c73 652c 200a 2020  ement=False, .  
+0000d650: 2020 290a 4076 6d28 6e61 6d65 3d22 5269    ).@vm(name="Ri
+0000d660: 7665 7220 5442 222c 0a20 2020 2070 726f  ver TB",.    pro
+0000d670: 7065 7274 6965 733d 7270 5f74 625f 7072  perties=rp_tb_pr
+0000d680: 6f70 6572 7469 6573 2c0a 2020 2020 696e  operties,.    in
+0000d690: 7075 745f 7479 7065 733d 5b45 6c65 6374  put_types=[Elect
+0000d6a0: 696f 6e54 7970 6573 2e50 524f 4649 4c45  ionTypes.PROFILE
+0000d6b0: 2c20 456c 6563 7469 6f6e 5479 7065 732e  , ElectionTypes.
+0000d6c0: 5052 4f46 494c 455f 5749 5448 5f54 4945  PROFILE_WITH_TIE
+0000d6d0: 532c 2045 6c65 6374 696f 6e54 7970 6573  S, ElectionTypes
+0000d6e0: 2e4d 4152 4749 4e5f 4752 4150 485d 290a  .MARGIN_GRAPH]).
+0000d6f0: 6465 6620 7269 7665 725f 7462 2865 6461  def river_tb(eda
+0000d700: 7461 2c20 6375 7272 5f63 616e 6473 203d  ta, curr_cands =
+0000d710: 204e 6f6e 652c 2074 6965 5f62 7265 616b   None, tie_break
+0000d720: 6572 203d 204e 6f6e 652c 2073 7472 656e  er = None, stren
+0000d730: 6774 685f 6675 6e63 7469 6f6e 203d 204e  gth_function = N
+0000d740: 6f6e 6529 3a20 2020 0a20 2020 2022 2222  one):   .    """
+0000d750: 0a20 2020 2052 6976 6572 2077 6974 6820  .    River with 
+0000d760: 6120 6669 7865 6420 6c69 6e65 6172 206f  a fixed linear o
+0000d770: 7264 6572 206f 6e20 7468 6520 6361 6e64  rder on the cand
+0000d780: 6964 6174 6573 2074 6f20 6272 6561 6b20  idates to break 
+0000d790: 616e 7920 7469 6573 2069 6e20 7468 6520  any ties in the 
+0000d7a0: 6d61 7267 696e 732e 2020 5369 6e63 6520  margins.  Since 
+0000d7b0: 7468 6520 7469 655f 6272 6561 6b65 7220  the tie_breaker 
+0000d7c0: 6973 2061 206c 696e 6561 7220 6f72 6465  is a linear orde
+0000d7d0: 722c 2074 6869 7320 6d65 7468 6f64 2069  r, this method i
+0000d7e0: 7320 7265 736f 6c75 7465 2e20 2020 0a0a  s resolute.   ..
+0000d7f0: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+0000d800: 2020 6564 6174 6120 2850 726f 6669 6c65    edata (Profile
+0000d810: 2c20 5072 6f66 696c 6557 6974 6854 6965  , ProfileWithTie
+0000d820: 732c 204d 6172 6769 6e47 7261 7068 293a  s, MarginGraph):
+0000d830: 2041 6e79 2065 6c65 6374 696f 6e20 6461   Any election da
+0000d840: 7461 2074 6861 7420 6861 7320 6120 606d  ta that has a `m
+0000d850: 6172 6769 6e60 206d 6574 686f 642e 200a  argin` method. .
+0000d860: 2020 2020 2020 2020 6375 7272 5f63 616e          curr_can
+0000d870: 6473 2028 4c69 7374 5b69 6e74 5d2c 206f  ds (List[int], o
+0000d880: 7074 696f 6e61 6c29 3a20 4966 2073 6574  ptional): If set
+0000d890: 2c20 7468 656e 2066 696e 6420 7468 6520  , then find the 
+0000d8a0: 7769 6e6e 6572 7320 666f 7220 7468 6520  winners for the 
+0000d8b0: 7072 6f66 696c 6520 7265 7374 7269 6374  profile restrict
+0000d8c0: 6564 2074 6f20 7468 6520 6361 6e64 6964  ed to the candid
+0000d8d0: 6174 6573 2069 6e20 6060 6375 7272 5f63  ates in ``curr_c
+0000d8e0: 616e 6473 6060 0a20 2020 2020 2020 2074  ands``.        t
+0000d8f0: 6965 5f62 7265 616b 6572 2028 4c69 7374  ie_breaker (List
+0000d900: 5b69 6e74 5d2c 206f 7074 696f 6e61 6c29  [int], optional)
+0000d910: 3a20 4120 6c69 6e65 6172 206f 7264 6572  : A linear order
+0000d920: 206f 6e20 7468 6520 6361 6e64 6964 6174   on the candidat
+0000d930: 6573 2e20 2049 6620 6e6f 7420 7365 742c  es.  If not set,
+0000d940: 2074 6865 6e20 7468 6520 6361 6e64 6964   then the candid
+0000d950: 6174 6573 2061 7265 2073 6f72 7465 6420  ates are sorted 
+0000d960: 696e 2061 7363 656e 6469 6e67 206f 7264  in ascending ord
+0000d970: 6572 2e0a 2020 2020 2020 2020 7374 7265  er..        stre
+0000d980: 6e67 7468 5f66 756e 6374 696f 6e20 2866  ngth_function (f
+0000d990: 756e 6374 696f 6e2c 206f 7074 696f 6e61  unction, optiona
+0000d9a0: 6c29 3a20 5468 6520 7374 7265 6e67 7468  l): The strength
+0000d9b0: 2066 756e 6374 696f 6e20 746f 2062 6520   function to be 
+0000d9c0: 7573 6564 2074 6f20 6361 6c63 756c 6174  used to calculat
+0000d9d0: 6520 7468 6520 7374 7265 6e67 7468 206f  e the strength o
+0000d9e0: 6620 6120 7061 7468 2e20 2020 5468 6520  f a path.   The 
+0000d9f0: 6465 6661 756c 7420 6973 2074 6865 206d  default is the m
+0000da00: 6172 6769 6e20 6d65 7468 6f64 206f 6620  argin method of 
+0000da10: 6060 6564 6174 6160 602e 2020 2054 6869  ``edata``.   Thi
+0000da20: 7320 6f6e 6c79 206d 6174 7465 7273 2077  s only matters w
+0000da30: 6865 6e20 7468 6520 6261 6c6c 6f74 7320  hen the ballots 
+0000da40: 6172 6520 6e6f 7420 6c69 6e65 6172 206f  are not linear o
+0000da50: 7264 6572 732e 200a 0a20 2020 2052 6574  rders. ..    Ret
+0000da60: 7572 6e73 3a20 0a20 2020 2020 2020 2041  urns: .        A
+0000da70: 2073 6f72 7465 6420 6c69 7374 206f 6620   sorted list of 
+0000da80: 6361 6e64 6964 6174 6573 2e20 0a0a 2020  candidates. ..  
+0000da90: 2020 2222 220a 2020 2020 6361 6e64 6964    """.    candid
+0000daa0: 6174 6573 203d 2065 6461 7461 2e63 616e  ates = edata.can
+0000dab0: 6469 6461 7465 7320 6966 2063 7572 725f  didates if curr_
+0000dac0: 6361 6e64 7320 6973 204e 6f6e 6520 656c  cands is None el
+0000dad0: 7365 2063 7572 725f 6361 6e64 7320 2020  se curr_cands   
+0000dae0: 200a 2020 2020 6369 6478 5f74 6f5f 6361   .    cidx_to_ca
+0000daf0: 6e64 203d 207b 6369 6478 3a20 6320 666f  nd = {cidx: c fo
+0000db00: 7220 6369 6478 2c20 6320 696e 2065 6e75  r cidx, c in enu
+0000db10: 6d65 7261 7465 2863 616e 6469 6461 7465  merate(candidate
+0000db20: 7329 7d20 200a 2020 2020 6361 6e64 5f74  s)}  .    cand_t
+0000db30: 6f5f 6369 6478 203d 207b 633a 2063 6964  o_cidx = {c: cid
+0000db40: 7820 666f 7220 6369 6478 2c20 6320 696e  x for cidx, c in
+0000db50: 2065 6e75 6d65 7261 7465 2863 616e 6469   enumerate(candi
+0000db60: 6461 7465 7329 7d20 200a 2020 2020 7374  dates)}  .    st
+0000db70: 7265 6e67 7468 5f66 756e 6374 696f 6e20  rength_function 
+0000db80: 3d20 6564 6174 612e 6d61 7267 696e 2069  = edata.margin i
+0000db90: 6620 7374 7265 6e67 7468 5f66 756e 6374  f strength_funct
+0000dba0: 696f 6e20 6973 204e 6f6e 6520 656c 7365  ion is None else
+0000dbb0: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
+0000dbc0: 6f6e 2020 2020 0a0a 2020 2020 7462 5f72  on    ..    tb_r
+0000dbd0: 616e 6b69 6e67 203d 2074 6965 5f62 7265  anking = tie_bre
+0000dbe0: 616b 6572 2069 6620 7469 655f 6272 6561  aker if tie_brea
+0000dbf0: 6b65 7220 6973 206e 6f74 204e 6f6e 6520  ker is not None 
+0000dc00: 656c 7365 2073 6f72 7465 6428 6c69 7374  else sorted(list
+0000dc10: 2863 616e 6469 6461 7465 7329 290a 0a20  (candidates)).. 
+0000dc20: 2020 2063 7720 3d20 6564 6174 612e 636f     cw = edata.co
+0000dc30: 6e64 6f72 6365 745f 7769 6e6e 6572 2863  ndorcet_winner(c
+0000dc40: 7572 725f 6361 6e64 733d 6375 7272 5f63  urr_cands=curr_c
+0000dc50: 616e 6473 290a 2020 2020 2320 5269 7665  ands).    # Rive
+0000dc60: 7220 6973 2043 6f6e 646f 7263 6574 2063  r is Condorcet c
+0000dc70: 6f6e 7369 7374 656e 742c 2073 6f20 7369  onsistent, so si
+0000dc80: 6d70 6c79 2072 6574 7572 6e20 7468 6520  mply return the 
+0000dc90: 436f 6e64 6f72 6365 7420 7769 6e6e 6572  Condorcet winner
+0000dca0: 2069 6620 6578 6973 7473 0a20 2020 2069   if exists.    i
+0000dcb0: 6620 6377 2069 7320 6e6f 7420 4e6f 6e65  f cw is not None
+0000dcc0: 3a20 0a20 2020 2020 2020 2077 696e 6e65  : .        winne
+0000dcd0: 7273 203d 205b 6377 5d0a 2020 2020 656c  rs = [cw].    el
+0000dce0: 7365 3a0a 2020 2020 2020 2020 775f 6564  se:.        w_ed
+0000dcf0: 6765 7320 3d20 5b28 6331 2c20 6332 2c20  ges = [(c1, c2, 
+0000dd00: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
+0000dd10: 6e28 6331 2c20 6332 2929 2066 6f72 2063  n(c1, c2)) for c
+0000dd20: 3120 696e 2063 616e 6469 6461 7465 7320  1 in candidates 
+0000dd30: 666f 7220 6332 2069 6e20 6361 6e64 6964  for c2 in candid
+0000dd40: 6174 6573 2069 6620 6331 2021 3d20 6332  ates if c1 != c2
+0000dd50: 2061 6e64 2028 6564 6174 612e 6d61 6a6f   and (edata.majo
+0000dd60: 7269 7479 5f70 7265 6665 7273 2863 312c  rity_prefers(c1,
+0000dd70: 2063 3229 206f 7220 6564 6174 612e 6973   c2) or edata.is
+0000dd80: 5f74 6965 6428 6331 2c20 6332 2929 5d0a  _tied(c1, c2))].
+0000dd90: 2020 2020 2020 2020 7769 6e6e 6572 7320          winners 
+0000dda0: 3d20 6c69 7374 2829 2020 0a20 2020 2020  = list()  .     
+0000ddb0: 2020 2073 7472 656e 6774 6873 203d 2073     strengths = s
+0000ddc0: 6f72 7465 6428 6c69 7374 2873 6574 285b  orted(list(set([
+0000ddd0: 655b 325d 2066 6f72 2065 2069 6e20 775f  e[2] for e in w_
+0000dde0: 6564 6765 735d 2929 2c20 7265 7665 7273  edges])), revers
+0000ddf0: 653d 5472 7565 290a 0a20 2020 2020 2020  e=True)..       
+0000de00: 2072 765f 6465 6665 6174 203d 2053 504f   rv_defeat = SPO
+0000de10: 286c 656e 2863 616e 6469 6461 7465 7329  (len(candidates)
+0000de20: 290a 0a20 2020 2020 2020 2066 6f72 2073  )..        for s
+0000de30: 2069 6e20 7374 7265 6e67 7468 733a 200a   in strengths: .
+0000de40: 2020 2020 2020 2020 2020 2020 6564 6765              edge
+0000de50: 7320 3d20 5b65 2066 6f72 2065 2069 6e20  s = [e for e in 
+0000de60: 775f 6564 6765 7320 6966 2065 5b32 5d20  w_edges if e[2] 
+0000de70: 3d3d 2073 5d0a 2020 2020 2020 2020 2020  == s].          
+0000de80: 2020 0a20 2020 2020 2020 2020 2020 2023    .            #
+0000de90: 2062 7265 616b 2074 6965 7320 7573 696e   break ties usin
+0000dea0: 6720 7468 6520 6c65 7869 636f 6772 6170  g the lexicograp
+0000deb0: 6869 6320 6f72 6465 7269 6e67 206f 6e20  hic ordering on 
+0000dec0: 7475 706c 6573 2067 6976 656e 2074 625f  tuples given tb_
+0000ded0: 7261 6e6b 696e 670a 2020 2020 2020 2020  ranking.        
+0000dee0: 2020 2020 736f 7274 6564 5f65 6467 6573      sorted_edges
+0000def0: 203d 2073 6f72 7465 6428 6564 6765 732c   = sorted(edges,
+0000df00: 206b 6579 203d 206c 616d 6264 6120 653a   key = lambda e:
+0000df10: 2028 7462 5f72 616e 6b69 6e67 2e69 6e64   (tb_ranking.ind
+0000df20: 6578 2865 5b30 5d29 2c20 7462 5f72 616e  ex(e[0]), tb_ran
+0000df30: 6b69 6e67 2e69 6e64 6578 2865 5b31 5d29  king.index(e[1])
+0000df40: 292c 2072 6576 6572 7365 3d46 616c 7365  ), reverse=False
+0000df50: 290a 2020 2020 2020 2020 2020 2020 666f  ).            fo
+0000df60: 7220 6530 2c65 312c 7320 696e 2073 6f72  r e0,e1,s in sor
+0000df70: 7465 645f 6564 6765 733a 200a 2020 2020  ted_edges: .    
+0000df80: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+0000df90: 6f74 2072 765f 6465 6665 6174 2e50 5b63  ot rv_defeat.P[c
+0000dfa0: 616e 645f 746f 5f63 6964 785b 6531 5d5d  and_to_cidx[e1]]
+0000dfb0: 5b63 616e 645f 746f 5f63 6964 785b 6530  [cand_to_cidx[e0
+0000dfc0: 5d5d 2061 6e64 206c 656e 2872 765f 6465  ]] and len(rv_de
+0000dfd0: 6665 6174 2e70 7265 6473 5b63 616e 645f  feat.preds[cand_
+0000dfe0: 746f 5f63 6964 785b 6531 5d5d 2920 3d3d  to_cidx[e1]]) ==
+0000dff0: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
+0000e000: 2020 2020 2020 2020 7276 5f64 6566 6561          rv_defea
+0000e010: 742e 6164 6428 6361 6e64 5f74 6f5f 6369  t.add(cand_to_ci
+0000e020: 6478 5b65 305d 2c63 616e 645f 746f 5f63  dx[e0],cand_to_c
+0000e030: 6964 785b 6531 5d29 0a20 2020 2020 2020  idx[e1]).       
+0000e040: 2020 2020 2077 696e 6e65 7273 2e61 7070       winners.app
+0000e050: 656e 6428 6369 6478 5f74 6f5f 6361 6e64  end(cidx_to_cand
+0000e060: 5b72 765f 6465 6665 6174 2e69 6e69 7469  [rv_defeat.initi
+0000e070: 616c 5f65 6c65 6d65 6e74 7328 295b 305d  al_elements()[0]
+0000e080: 5d29 0a20 2020 2072 6574 7572 6e20 736f  ]).    return so
+0000e090: 7274 6564 286c 6973 7428 7365 7428 7769  rted(list(set(wi
+0000e0a0: 6e6e 6572 7329 2929 0a0a 7269 7665 725f  nners)))..river_
+0000e0b0: 7a74 5f70 726f 7065 7274 6965 7320 3d20  zt_properties = 
+0000e0c0: 566f 7469 6e67 4d65 7468 6f64 5072 6f70  VotingMethodProp
+0000e0d0: 6572 7469 6573 280a 2020 2020 636f 6e64  erties(.    cond
+0000e0e0: 6f72 6365 745f 7769 6e6e 6572 3d54 7275  orcet_winner=Tru
+0000e0f0: 652c 200a 2020 2020 636f 6e64 6f72 6365  e, .    condorce
+0000e100: 745f 6c6f 7365 723d 5472 7565 2c0a 2020  t_loser=True,.  
+0000e110: 2020 7061 7265 746f 5f64 6f6d 696e 616e    pareto_dominan
+0000e120: 6365 3d54 7275 652c 0a20 2020 2070 6f73  ce=True,.    pos
+0000e130: 6974 6976 655f 696e 766f 6c76 656d 656e  itive_involvemen
+0000e140: 743d 4661 6c73 652c 200a 2020 2020 290a  t=False, .    ).
+0000e150: 4076 6d28 6e61 6d65 3d22 5269 7665 7220  @vm(name="River 
+0000e160: 5a54 222c 0a20 2020 2070 726f 7065 7274  ZT",.    propert
+0000e170: 6965 733d 7269 7665 725f 7a74 5f70 726f  ies=river_zt_pro
+0000e180: 7065 7274 6965 732c 0a20 2020 2069 6e70  perties,.    inp
+0000e190: 7574 5f74 7970 6573 3d5b 456c 6563 7469  ut_types=[Electi
+0000e1a0: 6f6e 5479 7065 732e 5052 4f46 494c 455d  onTypes.PROFILE]
+0000e1b0: 290a 6465 6620 7269 7665 725f 7a74 2870  ).def river_zt(p
+0000e1c0: 726f 6669 6c65 2c20 6375 7272 5f63 616e  rofile, curr_can
+0000e1d0: 6473 203d 204e 6f6e 652c 2073 7472 656e  ds = None, stren
+0000e1e0: 6774 685f 6675 6e63 7469 6f6e 203d 204e  gth_function = N
+0000e1f0: 6f6e 6529 3a20 2020 0a20 2020 2022 2222  one):   .    """
+0000e200: 5269 7665 7220 7768 6572 6520 6120 6669  River where a fi
+0000e210: 7865 6420 766f 7465 7220 6272 6561 6b73  xed voter breaks
+0000e220: 2061 6e79 2074 6965 7320 696e 2074 6865   any ties in the
+0000e230: 206d 6172 6769 6e73 2e20 2049 7420 6973   margins.  It is
+0000e240: 2061 6c77 6179 7320 7468 6520 766f 7465   always the vote
+0000e250: 7220 696e 2070 6f73 6974 696f 6e20 3020  r in position 0 
+0000e260: 7468 6174 2062 7265 616b 7320 7468 6520  that breaks the 
+0000e270: 7469 6573 2e20 2053 696e 6365 2076 6f74  ties.  Since vot
+0000e280: 6572 7320 6861 7665 2073 7472 6963 7420  ers have strict 
+0000e290: 7072 6566 6572 656e 6365 732c 2074 6869  preferences, thi
+0000e2a0: 7320 6d65 7468 6f64 2069 7320 7265 736f  s method is reso
+0000e2b0: 6c75 7465 2e20 200a 0a20 2020 2041 7267  lute.  ..    Arg
+0000e2c0: 733a 0a20 2020 2020 2020 2065 6461 7461  s:.        edata
+0000e2d0: 2028 5072 6f66 696c 6529 3a20 4120 7072   (Profile): A pr
+0000e2e0: 6f66 696c 6520 6f66 206c 696e 6561 7220  ofile of linear 
+0000e2f0: 6f72 6465 7273 0a20 2020 2020 2020 2063  orders.        c
+0000e300: 7572 725f 6361 6e64 7320 284c 6973 745b  urr_cands (List[
+0000e310: 696e 745d 2c20 6f70 7469 6f6e 616c 293a  int], optional):
+0000e320: 2049 6620 7365 742c 2074 6865 6e20 6669   If set, then fi
+0000e330: 6e64 2074 6865 2077 696e 6e65 7273 2066  nd the winners f
+0000e340: 6f72 2074 6865 2070 726f 6669 6c65 2072  or the profile r
+0000e350: 6573 7472 6963 7465 6420 746f 2074 6865  estricted to the
+0000e360: 2063 616e 6469 6461 7465 7320 696e 2060   candidates in `
+0000e370: 6063 7572 725f 6361 6e64 7360 600a 0a20  `curr_cands``.. 
+0000e380: 2020 2052 6574 7572 6e73 3a20 0a20 2020     Returns: .   
+0000e390: 2020 2020 2041 2073 6f72 7465 6420 6c69       A sorted li
+0000e3a0: 7374 206f 6620 6361 6e64 6964 6174 6573  st of candidates
+0000e3b0: 2e20 0a0a 2020 2020 2e2e 2073 6565 616c  . ..    .. seeal
+0000e3c0: 736f 3a3a 0a0a 2020 2020 2020 2020 3a6d  so::..        :m
+0000e3d0: 6574 683a 6070 7265 665f 766f 7469 6e67  eth:`pref_voting
+0000e3e0: 2e6d 6172 6769 6e5f 6261 7365 645f 6d65  .margin_based_me
+0000e3f0: 7468 6f64 732e 7269 7665 7260 2c20 3a6d  thods.river`, :m
+0000e400: 6574 683a 6070 7265 665f 766f 7469 6e67  eth:`pref_voting
+0000e410: 2e6d 6172 6769 6e5f 6261 7365 645f 6d65  .margin_based_me
+0000e420: 7468 6f64 732e 7269 7665 725f 7769 7468  thods.river_with
+0000e430: 5f74 6573 7460 2c20 3a6d 6574 683a 6070  _test`, :meth:`p
+0000e440: 7265 665f 766f 7469 6e67 2e6d 6172 6769  ref_voting.margi
+0000e450: 6e5f 6261 7365 645f 6d65 7468 6f64 732e  n_based_methods.
+0000e460: 7261 6e6b 6564 5f70 6169 7273 600a 0a20  ranked_pairs`.. 
+0000e470: 2020 200a 2020 2020 2222 220a 2020 2020     .    """.    
+0000e480: 6361 6e64 6964 6174 6573 203d 2070 726f  candidates = pro
+0000e490: 6669 6c65 2e63 616e 6469 6461 7465 7320  file.candidates 
+0000e4a0: 6966 2063 7572 725f 6361 6e64 7320 6973  if curr_cands is
+0000e4b0: 204e 6f6e 6520 656c 7365 2063 7572 725f   None else curr_
+0000e4c0: 6361 6e64 7320 2020 200a 2020 2020 0a20  cands    .    . 
+0000e4d0: 2020 2023 2074 6865 2074 6965 2d62 7265     # the tie-bre
+0000e4e0: 616b 6572 2069 7320 616c 7761 7973 2074  aker is always t
+0000e4f0: 6865 2066 6972 7374 2076 6f74 6572 2e20  he first voter. 
+0000e500: 0a20 2020 2074 625f 7261 6e6b 696e 6720  .    tb_ranking 
+0000e510: 3d20 7475 706c 6528 5b63 2066 6f72 2063  = tuple([c for c
+0000e520: 2069 6e20 6c69 7374 2870 726f 6669 6c65   in list(profile
+0000e530: 2e5f 7261 6e6b 696e 6773 5b30 5d29 2069  ._rankings[0]) i
+0000e540: 6620 6320 696e 2063 616e 6469 6461 7465  f c in candidate
+0000e550: 735d 290a 2020 2020 0a20 2020 2072 6574  s]).    .    ret
+0000e560: 7572 6e20 7269 7665 725f 7462 2870 726f  urn river_tb(pro
+0000e570: 6669 6c65 2c20 6375 7272 5f63 616e 6473  file, curr_cands
+0000e580: 203d 2063 7572 725f 6361 6e64 732c 2074   = curr_cands, t
+0000e590: 6965 5f62 7265 616b 6572 203d 2074 625f  ie_breaker = tb_
+0000e5a0: 7261 6e6b 696e 672c 2073 7472 656e 6774  ranking, strengt
+0000e5b0: 685f 6675 6e63 7469 6f6e 203d 2073 7472  h_function = str
+0000e5c0: 656e 6774 685f 6675 6e63 7469 6f6e 290a  ength_function).
+0000e5d0: 2020 2020 0a0a 2320 5369 6d70 6c65 2053      ..# Simple S
+0000e5e0: 7461 626c 6520 566f 7469 6e67 200a 6465  table Voting .de
+0000e5f0: 6620 5f73 696d 706c 655f 7374 6162 6c65  f _simple_stable
+0000e600: 5f76 6f74 696e 6728 6375 7272 5f63 616e  _voting(curr_can
+0000e610: 6473 2c20 0a20 2020 2020 2020 2020 2020  ds, .           
+0000e620: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000e630: 6f72 7465 645f 6d61 7463 6865 732c 0a20  orted_matches,. 
+0000e640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e650: 2020 2020 2020 2020 206d 656d 5f73 765f           mem_sv_
+0000e660: 7769 6e6e 6572 7329 3a0a 2020 2020 2727  winners):.    ''
+0000e670: 270a 2020 2020 4465 7465 726d 696e 6520  '.    Determine 
+0000e680: 7468 6520 5369 6d70 6c65 2053 7461 626c  the Simple Stabl
+0000e690: 6520 566f 7469 6e67 2077 696e 6e65 7273  e Voting winners
+0000e6a0: 2077 6869 6c65 206b 6565 7069 6e67 2074   while keeping t
+0000e6b0: 7261 636b 200a 2020 2020 6f66 2074 6865  rack .    of the
+0000e6c0: 2077 696e 6e65 7273 2069 6e20 616e 7920   winners in any 
+0000e6d0: 7375 6270 726f 6669 6c65 7320 6368 6563  subprofiles chec
+0000e6e0: 6b65 6420 6475 7269 6e67 2063 6f6d 7075  ked during compu
+0000e6f0: 7461 7469 6f6e 2e20 0a20 2020 2027 2727  tation. .    '''
+0000e700: 0a20 2020 200a 2020 2020 7376 5f77 696e  .    .    sv_win
+0000e710: 6e65 7273 203d 206c 6973 7428 290a 2020  ners = list().  
+0000e720: 2020 2020 2020 0a20 2020 2069 6620 6c65        .    if le
+0000e730: 6e28 6375 7272 5f63 616e 6473 2920 3d3d  n(curr_cands) ==
+0000e740: 2031 3a20 0a20 2020 2020 2020 206d 656d   1: .        mem
+0000e750: 5f73 765f 7769 6e6e 6572 735b 7475 706c  _sv_winners[tupl
+0000e760: 6528 6375 7272 5f63 616e 6473 295d 203d  e(curr_cands)] =
+0000e770: 2063 7572 725f 6361 6e64 730a 2020 2020   curr_cands.    
+0000e780: 2020 2020 7265 7475 726e 2063 7572 725f      return curr_
+0000e790: 6361 6e64 732c 206d 656d 5f73 765f 7769  cands, mem_sv_wi
+0000e7a0: 6e6e 6572 730a 2020 2020 0a20 2020 206d  nners.    .    m
+0000e7b0: 6172 6769 6e5f 7769 746e 6573 7369 6e67  argin_witnessing
+0000e7c0: 5f77 696e 203d 202d 6d61 7468 2e69 6e66  _win = -math.inf
+0000e7d0: 0a0a 2020 2020 666f 7220 612c 2062 2c20  ..    for a, b, 
+0000e7e0: 7320 696e 2073 6f72 7465 645f 6d61 7463  s in sorted_matc
+0000e7f0: 6865 733a 0a20 2020 2020 2020 2069 6620  hes:.        if 
+0000e800: 7320 3c20 6d61 7267 696e 5f77 6974 6e65  s < margin_witne
+0000e810: 7373 696e 675f 7769 6e3a 200a 2020 2020  ssing_win: .    
+0000e820: 2020 2020 2020 2020 6272 6561 6b0a 2020          break.  
+0000e830: 2020 2020 2020 6966 2061 206e 6f74 2069        if a not i
+0000e840: 6e20 7376 5f77 696e 6e65 7273 3a20 0a20  n sv_winners: . 
+0000e850: 2020 2020 2020 2020 2020 2063 616e 6473             cands
+0000e860: 5f6d 696e 7573 5f62 203d 205b 6320 666f  _minus_b = [c fo
+0000e870: 7220 6320 696e 2063 7572 725f 6361 6e64  r c in curr_cand
+0000e880: 7320 6966 2063 2021 3d20 625d 0a20 2020  s if c != b].   
+0000e890: 2020 2020 2020 2020 2063 616e 6473 5f6d           cands_m
+0000e8a0: 696e 7573 5f62 5f6b 6579 203d 2074 7570  inus_b_key = tup
+0000e8b0: 6c65 2873 6f72 7465 6428 6361 6e64 735f  le(sorted(cands_
+0000e8c0: 6d69 6e75 735f 6229 290a 2020 2020 2020  minus_b)).      
+0000e8d0: 2020 2020 2020 6966 2063 616e 6473 5f6d        if cands_m
+0000e8e0: 696e 7573 5f62 5f6b 6579 206e 6f74 2069  inus_b_key not i
+0000e8f0: 6e20 6d65 6d5f 7376 5f77 696e 6e65 7273  n mem_sv_winners
+0000e900: 2e6b 6579 7328 293a 200a 2020 2020 2020  .keys(): .      
+0000e910: 2020 2020 2020 2020 2020 7773 2c20 6d65            ws, me
+0000e920: 6d5f 7376 5f77 696e 6e65 7273 203d 205f  m_sv_winners = _
+0000e930: 7369 6d70 6c65 5f73 7461 626c 655f 766f  simple_stable_vo
+0000e940: 7469 6e67 2863 7572 725f 6361 6e64 7320  ting(curr_cands 
+0000e950: 3d20 6361 6e64 735f 6d69 6e75 735f 622c  = cands_minus_b,
+0000e960: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e990: 2020 2020 2020 2020 2020 2020 736f 7274              sort
+0000e9a0: 6564 5f6d 6174 6368 6573 203d 205b 2861  ed_matches = [(a
+0000e9b0: 2c20 632c 2073 2920 666f 7220 612c 2063  , c, s) for a, c
+0000e9c0: 2c20 7320 696e 2073 6f72 7465 645f 6d61  , s in sorted_ma
+0000e9d0: 7463 6865 7320 6966 2061 2021 3d20 6220  tches if a != b 
+0000e9e0: 616e 6420 6320 213d 2062 5d2c 0a20 2020  and c != b],.   
+0000e9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ea00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ea10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ea20: 2020 2020 2020 2020 6d65 6d5f 7376 5f77          mem_sv_w
+0000ea30: 696e 6e65 7273 203d 206d 656d 5f73 765f  inners = mem_sv_
+0000ea40: 7769 6e6e 6572 7329 0a20 2020 2020 2020  winners).       
+0000ea50: 2020 2020 2020 2020 206d 656d 5f73 765f           mem_sv_
+0000ea60: 7769 6e6e 6572 735b 6361 6e64 735f 6d69  winners[cands_mi
+0000ea70: 6e75 735f 625f 6b65 795d 203d 2077 730a  nus_b_key] = ws.
+0000ea80: 2020 2020 2020 2020 2020 2020 656c 7365              else
+0000ea90: 3a20 0a20 2020 2020 2020 2020 2020 2020  : .             
+0000eaa0: 2020 2077 7320 3d20 6d65 6d5f 7376 5f77     ws = mem_sv_w
+0000eab0: 696e 6e65 7273 5b63 616e 6473 5f6d 696e  inners[cands_min
+0000eac0: 7573 5f62 5f6b 6579 5d0a 2020 2020 2020  us_b_key].      
+0000ead0: 2020 2020 2020 6966 2061 2069 6e20 7773        if a in ws
+0000eae0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000eaf0: 2020 7376 5f77 696e 6e65 7273 2e61 7070    sv_winners.app
+0000eb00: 656e 6428 6129 0a20 2020 2020 2020 2020  end(a).         
+0000eb10: 2020 2020 2020 206d 6172 6769 6e5f 7769         margin_wi
+0000eb20: 746e 6573 7369 6e67 5f77 696e 203d 2073  tnessing_win = s
+0000eb30: 0a0a 2020 2020 7265 7475 726e 2073 765f  ..    return sv_
+0000eb40: 7769 6e6e 6572 732c 206d 656d 5f73 765f  winners, mem_sv_
+0000eb50: 7769 6e6e 6572 730a 2020 2020 0a0a 4076  winners.    ..@v
+0000eb60: 6d28 6e61 6d65 203d 2022 5369 6d70 6c65  m(name = "Simple
+0000eb70: 2053 7461 626c 6520 566f 7469 6e67 2229   Stable Voting")
+0000eb80: 0a64 6566 205f 7369 6d70 6c65 5f73 7461  .def _simple_sta
+0000eb90: 626c 655f 766f 7469 6e67 5f77 6974 685f  ble_voting_with_
+0000eba0: 636f 6e64 6f72 6365 745f 6368 6563 6b28  condorcet_check(
+0000ebb0: 0a20 2020 2065 6461 7461 2c20 0a20 2020  .    edata, .   
+0000ebc0: 2063 7572 725f 6361 6e64 7320 3d20 4e6f   curr_cands = No
+0000ebd0: 6e65 2c20 0a20 2020 2073 7472 656e 6774  ne, .    strengt
+0000ebe0: 685f 6675 6e63 7469 6f6e 203d 204e 6f6e  h_function = Non
+0000ebf0: 6529 3a20 0a20 2020 2022 2222 5369 6d70  e): .    """Simp
+0000ec00: 6c65 2053 7461 626c 6520 566f 7469 6e67  le Stable Voting
+0000ec10: 2069 7320 436f 6e64 6f72 6365 7420 636f   is Condorcet co
+0000ec20: 6e73 6973 7465 6e74 2e20 2020 4974 2069  nsistent.   It i
+0000ec30: 7320 6661 7374 6572 2074 6f20 736b 6970  s faster to skip
+0000ec40: 2065 7865 6375 7469 6e67 2074 6865 2072   executing the r
+0000ec50: 6563 7572 7369 7665 2061 6c67 6f72 6974  ecursive algorit
+0000ec60: 686d 2077 6865 6e20 7468 6572 6520 6973  hm when there is
+0000ec70: 2061 2043 6f6e 646f 7263 6574 2077 696e   a Condorcet win
+0000ec80: 6e65 7246 6972 7374 2063 6865 636b 2069  nerFirst check i
+0000ec90: 6620 7468 6572 6520 6973 2061 2043 6f6e  f there is a Con
+0000eca0: 646f 7263 6574 2077 696e 6e65 722e 2020  dorcet winner.  
+0000ecb0: 4966 2073 6f2c 2072 6574 7572 6e20 7468  If so, return th
+0000ecc0: 6520 436f 6e64 6f72 6365 7420 7769 6e6e  e Condorcet winn
+0000ecd0: 6572 2c20 6f74 6865 7277 6973 6520 6669  er, otherwise fi
+0000ece0: 6e64 2074 6865 2053 696d 706c 6520 5374  nd the Simple St
+0000ecf0: 6162 6c65 2056 6f74 696e 6720 7769 6e6e  able Voting winn
+0000ed00: 6572 2075 7369 6e67 205f 7369 6d70 6c65  er using _simple
+0000ed10: 5f73 7461 626c 655f 766f 7469 6e67 0a0a  _stable_voting..
+0000ed20: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+0000ed30: 2020 6564 6174 6120 2850 726f 6669 6c65    edata (Profile
+0000ed40: 2c20 5072 6f66 696c 6557 6974 6854 6965  , ProfileWithTie
+0000ed50: 732c 204d 6172 6769 6e47 7261 7068 293a  s, MarginGraph):
+0000ed60: 2041 6e79 2065 6c65 6374 696f 6e20 6461   Any election da
+0000ed70: 7461 2074 6861 7420 6861 7320 6120 606d  ta that has a `m
+0000ed80: 6172 6769 6e60 206d 6574 686f 642e 200a  argin` method. .
+0000ed90: 2020 2020 2020 2020 6375 7272 5f63 616e          curr_can
+0000eda0: 6473 2028 4c69 7374 5b69 6e74 5d2c 206f  ds (List[int], o
+0000edb0: 7074 696f 6e61 6c29 3a20 4966 2073 6574  ptional): If set
+0000edc0: 2c20 7468 656e 2066 696e 6420 7468 6520  , then find the 
+0000edd0: 7769 6e6e 6572 7320 666f 7220 7468 6520  winners for the 
+0000ede0: 7072 6f66 696c 6520 7265 7374 7269 6374  profile restrict
+0000edf0: 6564 2074 6f20 7468 6520 6361 6e64 6964  ed to the candid
+0000ee00: 6174 6573 2069 6e20 6060 6375 7272 5f63  ates in ``curr_c
+0000ee10: 616e 6473 6060 0a20 2020 2020 2020 2073  ands``.        s
+0000ee20: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
+0000ee30: 2028 6675 6e63 7469 6f6e 2c20 6f70 7469   (function, opti
+0000ee40: 6f6e 616c 293a 2054 6865 2073 7472 656e  onal): The stren
+0000ee50: 6774 6820 6675 6e63 7469 6f6e 2074 6f20  gth function to 
+0000ee60: 6265 2075 7365 6420 746f 2063 616c 6375  be used to calcu
+0000ee70: 6c61 7465 2074 6865 2073 7472 656e 6774  late the strengt
+0000ee80: 6820 6f66 2061 2070 6174 682e 2020 2054  h of a path.   T
+0000ee90: 6865 2064 6566 6175 6c74 2069 7320 7468  he default is th
+0000eea0: 6520 6d61 7267 696e 206d 6574 686f 6420  e margin method 
+0000eeb0: 6f66 2060 6065 6461 7461 6060 2e20 2020  of ``edata``.   
+0000eec0: 5468 6973 206f 6e6c 7920 6d61 7474 6572  This only matter
+0000eed0: 7320 7768 656e 2074 6865 2062 616c 6c6f  s when the ballo
+0000eee0: 7473 2061 7265 206e 6f74 206c 696e 6561  ts are not linea
+0000eef0: 7220 6f72 6465 7273 2e20 0a0a 2020 2020  r orders. ..    
+0000ef00: 5265 7475 726e 733a 200a 2020 2020 2020  Returns: .      
+0000ef10: 2020 4120 736f 7274 6564 206c 6973 7420    A sorted list 
+0000ef20: 6f66 2063 616e 6469 6461 7465 732e 200a  of candidates. .
+0000ef30: 0a20 2020 2022 2222 0a20 2020 200a 2020  .    """.    .  
+0000ef40: 2020 6377 203d 2065 6461 7461 2e63 6f6e    cw = edata.con
+0000ef50: 646f 7263 6574 5f77 696e 6e65 7228 6375  dorcet_winner(cu
+0000ef60: 7272 5f63 616e 6473 203d 2063 7572 725f  rr_cands = curr_
+0000ef70: 6361 6e64 7329 0a20 2020 2069 6620 6377  cands).    if cw
+0000ef80: 2069 7320 6e6f 7420 4e6f 6e65 3a20 0a20   is not None: . 
+0000ef90: 2020 2020 2020 2072 6574 7572 6e20 5b63         return [c
+0000efa0: 775d 0a20 2020 2065 6c73 653a 200a 2020  w].    else: .  
+0000efb0: 2020 2020 2020 6375 7272 5f63 616e 6473        curr_cands
+0000efc0: 203d 2065 6461 7461 2e63 616e 6469 6461   = edata.candida
+0000efd0: 7465 7320 6966 2063 7572 725f 6361 6e64  tes if curr_cand
+0000efe0: 7320 6973 204e 6f6e 6520 656c 7365 2063  s is None else c
+0000eff0: 7572 725f 6361 6e64 730a 2020 2020 2020  urr_cands.      
+0000f000: 2020 7374 7265 6e67 7468 5f66 756e 6374    strength_funct
+0000f010: 696f 6e20 3d20 6564 6174 612e 6d61 7267  ion = edata.marg
+0000f020: 696e 2069 6620 7374 7265 6e67 7468 5f66  in if strength_f
+0000f030: 756e 6374 696f 6e20 6973 204e 6f6e 6520  unction is None 
+0000f040: 656c 7365 2073 7472 656e 6774 685f 6675  else strength_fu
+0000f050: 6e63 7469 6f6e 2020 0a0a 2020 2020 2020  nction  ..      
+0000f060: 2020 6d61 7463 6865 7320 3d20 5b28 612c    matches = [(a,
+0000f070: 2062 2c20 7374 7265 6e67 7468 5f66 756e   b, strength_fun
+0000f080: 6374 696f 6e28 612c 2062 2929 2066 6f72  ction(a, b)) for
+0000f090: 2061 2069 6e20 6375 7272 5f63 616e 6473   a in curr_cands
+0000f0a0: 2066 6f72 2062 2069 6e20 6375 7272 5f63   for b in curr_c
+0000f0b0: 616e 6473 2069 6620 6120 213d 2062 5d0a  ands if a != b].
+0000f0c0: 2020 2020 2020 2020 736f 7274 6564 5f6d          sorted_m
+0000f0d0: 6174 6368 6573 203d 2073 6f72 7465 6428  atches = sorted(
+0000f0e0: 6d61 7463 6865 732c 2072 6576 6572 7365  matches, reverse
+0000f0f0: 3d54 7275 652c 206b 6579 3d6c 616d 6264  =True, key=lambd
+0000f100: 6120 6d5f 775f 7765 6967 6874 3a20 6d5f  a m_w_weight: m_
+0000f110: 775f 7765 6967 6874 5b32 5d29 0a20 2020  w_weight[2]).   
+0000f120: 200a 2020 2020 2020 2020 7265 7475 726e   .        return
+0000f130: 2073 6f72 7465 6428 5f73 696d 706c 655f   sorted(_simple_
+0000f140: 7374 6162 6c65 5f76 6f74 696e 6728 6375  stable_voting(cu
+0000f150: 7272 5f63 616e 6473 203d 2063 7572 725f  rr_cands = curr_
+0000f160: 6361 6e64 732c 200a 2020 2020 2020 2020  cands, .        
+0000f170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f190: 2020 2020 736f 7274 6564 5f6d 6174 6368      sorted_match
+0000f1a0: 6573 203d 2073 6f72 7465 645f 6d61 7463  es = sorted_matc
+0000f1b0: 6865 732c 0a20 2020 2020 2020 2020 2020  hes,.           
+0000f1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f1e0: 206d 656d 5f73 765f 7769 6e6e 6572 7320   mem_sv_winners 
+0000f1f0: 3d20 7b7d 295b 305d 290a 0a0a 6465 6620  = {})[0])...def 
+0000f200: 5f73 696d 706c 655f 7374 6162 6c65 5f76  _simple_stable_v
+0000f210: 6f74 696e 675f 6261 7369 6328 6564 6174  oting_basic(edat
+0000f220: 612c 2063 7572 725f 6361 6e64 7320 3d20  a, curr_cands = 
+0000f230: 4e6f 6e65 2c20 7374 7265 6e67 7468 5f66  None, strength_f
+0000f240: 756e 6374 696f 6e20 3d20 4e6f 6e65 293a  unction = None):
+0000f250: 200a 2020 2020 2222 2249 6d70 6c65 6d65   .    """Impleme
+0000f260: 6e74 6174 696f 6e20 6f66 2053 696d 706c  ntation of Simpl
+0000f270: 6520 5374 6162 6c65 2056 6f74 696e 6720  e Stable Voting 
+0000f280: 6672 6f6d 2068 7474 7073 3a2f 2f61 7278  from https://arx
+0000f290: 6976 2e6f 7267 2f61 6273 2f32 3130 382e  iv.org/abs/2108.
+0000f2a0: 3030 3534 322e 200a 0a20 2020 2041 7267  00542. ..    Arg
+0000f2b0: 733a 0a20 2020 2020 2020 2065 6461 7461  s:.        edata
+0000f2c0: 2028 5072 6f66 696c 652c 2050 726f 6669   (Profile, Profi
+0000f2d0: 6c65 5769 7468 5469 6573 2c20 4d61 7267  leWithTies, Marg
+0000f2e0: 696e 4772 6170 6829 3a20 416e 7920 656c  inGraph): Any el
+0000f2f0: 6563 7469 6f6e 2064 6174 6120 7468 6174  ection data that
+0000f300: 2068 6173 2061 2060 6d61 7267 696e 6020   has a `margin` 
+0000f310: 6d65 7468 6f64 2e20 0a20 2020 2020 2020  method. .       
+0000f320: 2063 7572 725f 6361 6e64 7320 284c 6973   curr_cands (Lis
+0000f330: 745b 696e 745d 2c20 6f70 7469 6f6e 616c  t[int], optional
+0000f340: 293a 2049 6620 7365 742c 2074 6865 6e20  ): If set, then 
+0000f350: 6669 6e64 2074 6865 2077 696e 6e65 7273  find the winners
+0000f360: 2066 6f72 2074 6865 2070 726f 6669 6c65   for the profile
+0000f370: 2072 6573 7472 6963 7465 6420 746f 2074   restricted to t
+0000f380: 6865 2063 616e 6469 6461 7465 7320 696e  he candidates in
+0000f390: 2060 6063 7572 725f 6361 6e64 7360 600a   ``curr_cands``.
+0000f3a0: 2020 2020 2020 2020 7374 7265 6e67 7468          strength
+0000f3b0: 5f66 756e 6374 696f 6e20 2866 756e 6374  _function (funct
+0000f3c0: 696f 6e2c 206f 7074 696f 6e61 6c29 3a20  ion, optional): 
+0000f3d0: 5468 6520 7374 7265 6e67 7468 2066 756e  The strength fun
+0000f3e0: 6374 696f 6e20 746f 2062 6520 7573 6564  ction to be used
+0000f3f0: 2074 6f20 6361 6c63 756c 6174 6520 7468   to calculate th
+0000f400: 6520 7374 7265 6e67 7468 206f 6620 6120  e strength of a 
+0000f410: 7061 7468 2e20 2020 5468 6520 6465 6661  path.   The defa
+0000f420: 756c 7420 6973 2074 6865 206d 6172 6769  ult is the margi
+0000f430: 6e20 6d65 7468 6f64 206f 6620 6060 6564  n method of ``ed
+0000f440: 6174 6160 602e 2020 2054 6869 7320 6f6e  ata``.   This on
+0000f450: 6c79 206d 6174 7465 7273 2077 6865 6e20  ly matters when 
+0000f460: 7468 6520 6261 6c6c 6f74 7320 6172 6520  the ballots are 
+0000f470: 6e6f 7420 6c69 6e65 6172 206f 7264 6572  not linear order
+0000f480: 732e 200a 0a20 2020 2052 6574 7572 6e73  s. ..    Returns
+0000f490: 3a20 0a20 2020 2020 2020 2041 2073 6f72  : .        A sor
+0000f4a0: 7465 6420 6c69 7374 206f 6620 6361 6e64  ted list of cand
+0000f4b0: 6964 6174 6573 2e20 0a0a 2020 2020 2222  idates. ..    ""
+0000f4c0: 220a 2020 2020 0a20 2020 2063 7572 725f  ".    .    curr_
+0000f4d0: 6361 6e64 7320 3d20 6564 6174 612e 6361  cands = edata.ca
+0000f4e0: 6e64 6964 6174 6573 2069 6620 6375 7272  ndidates if curr
+0000f4f0: 5f63 616e 6473 2069 7320 4e6f 6e65 2065  _cands is None e
+0000f500: 6c73 6520 6375 7272 5f63 616e 6473 0a20  lse curr_cands. 
+0000f510: 2020 2073 7472 656e 6774 685f 6675 6e63     strength_func
+0000f520: 7469 6f6e 203d 2065 6461 7461 2e6d 6172  tion = edata.mar
+0000f530: 6769 6e20 6966 2073 7472 656e 6774 685f  gin if strength_
+0000f540: 6675 6e63 7469 6f6e 2069 7320 4e6f 6e65  function is None
+0000f550: 2065 6c73 6520 7374 7265 6e67 7468 5f66   else strength_f
+0000f560: 756e 6374 696f 6e20 200a 0a20 2020 206d  unction  ..    m
+0000f570: 6174 6368 6573 203d 205b 2861 2c20 622c  atches = [(a, b,
+0000f580: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
+0000f590: 6f6e 2861 2c20 6229 2920 666f 7220 6120  on(a, b)) for a 
+0000f5a0: 696e 2063 7572 725f 6361 6e64 7320 666f  in curr_cands fo
+0000f5b0: 7220 6220 696e 2063 7572 725f 6361 6e64  r b in curr_cand
+0000f5c0: 7320 6966 2061 2021 3d20 625d 0a20 2020  s if a != b].   
+0000f5d0: 2073 6f72 7465 645f 6d61 7463 6865 7320   sorted_matches 
+0000f5e0: 3d20 736f 7274 6564 286d 6174 6368 6573  = sorted(matches
+0000f5f0: 2c20 7265 7665 7273 653d 5472 7565 2c20  , reverse=True, 
+0000f600: 6b65 793d 6c61 6d62 6461 206d 5f77 5f77  key=lambda m_w_w
+0000f610: 6569 6768 743a 206d 5f77 5f77 6569 6768  eight: m_w_weigh
+0000f620: 745b 325d 290a 2020 2020 0a20 2020 2072  t[2]).    .    r
+0000f630: 6574 7572 6e20 736f 7274 6564 285f 7369  eturn sorted(_si
+0000f640: 6d70 6c65 5f73 7461 626c 655f 766f 7469  mple_stable_voti
+0000f650: 6e67 2863 7572 725f 6361 6e64 7320 3d20  ng(curr_cands = 
+0000f660: 6375 7272 5f63 616e 6473 2c20 0a20 2020  curr_cands, .   
+0000f670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f690: 2020 2020 2073 6f72 7465 645f 6d61 7463       sorted_matc
+0000f6a0: 6865 7320 3d20 736f 7274 6564 5f6d 6174  hes = sorted_mat
+0000f6b0: 6368 6573 2c0a 2020 2020 2020 2020 2020  ches,.          
+0000f6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f6d0: 2020 2020 2020 2020 2020 2020 2020 6d65                me
+0000f6e0: 6d5f 7376 5f77 696e 6e65 7273 203d 207b  m_sv_winners = {
+0000f6f0: 7d29 5b30 5d29 0a0a 7373 765f 7072 6f70  })[0])..ssv_prop
+0000f700: 6572 7469 6573 203d 2056 6f74 696e 674d  erties = VotingM
+0000f710: 6574 686f 6450 726f 7065 7274 6965 7328  ethodProperties(
+0000f720: 0a20 2020 2063 6f6e 646f 7263 6574 5f77  .    condorcet_w
+0000f730: 696e 6e65 723d 5472 7565 2c20 0a20 2020  inner=True, .   
+0000f740: 2063 6f6e 646f 7263 6574 5f6c 6f73 6572   condorcet_loser
+0000f750: 3d54 7275 652c 0a20 2020 2070 6172 6574  =True,.    paret
+0000f760: 6f5f 646f 6d69 6e61 6e63 653d 5472 7565  o_dominance=True
+0000f770: 2c0a 2020 2020 706f 7369 7469 7665 5f69  ,.    positive_i
+0000f780: 6e76 6f6c 7665 6d65 6e74 3d46 616c 7365  nvolvement=False
+0000f790: 2c20 0a20 2020 2029 0a40 766d 286e 616d  , .    ).@vm(nam
+0000f7a0: 6520 3d20 2253 696d 706c 6520 5374 6162  e = "Simple Stab
+0000f7b0: 6c65 2056 6f74 696e 6722 2c0a 2020 2020  le Voting",.    
+0000f7c0: 7072 6f70 6572 7469 6573 203d 2073 7376  properties = ssv
+0000f7d0: 5f70 726f 7065 7274 6965 732c 0a20 2020  _properties,.   
+0000f7e0: 2069 6e70 7574 5f74 7970 6573 203d 205b   input_types = [
+0000f7f0: 456c 6563 7469 6f6e 5479 7065 732e 5052  ElectionTypes.PR
+0000f800: 4f46 494c 452c 2045 6c65 6374 696f 6e54  OFILE, ElectionT
+0000f810: 7970 6573 2e50 524f 4649 4c45 5f57 4954  ypes.PROFILE_WIT
+0000f820: 485f 5449 4553 2c20 456c 6563 7469 6f6e  H_TIES, Election
+0000f830: 5479 7065 732e 4d41 5247 494e 5f47 5241  Types.MARGIN_GRA
+0000f840: 5048 5d29 0a64 6566 2073 696d 706c 655f  PH]).def simple_
+0000f850: 7374 6162 6c65 5f76 6f74 696e 6728 0a20  stable_voting(. 
+0000f860: 2020 2065 6461 7461 2c20 0a20 2020 2063     edata, .    c
+0000f870: 7572 725f 6361 6e64 733d 4e6f 6e65 2c20  urr_cands=None, 
+0000f880: 0a20 2020 2073 7472 656e 6774 685f 6675  .    strength_fu
+0000f890: 6e63 7469 6f6e 3d4e 6f6e 652c 0a20 2020  nction=None,.   
+0000f8a0: 2061 6c67 6f72 6974 686d 203d 2027 6261   algorithm = 'ba
+0000f8b0: 7369 6327 293a 200a 0a20 2020 2022 2222  sic'): ..    """
+0000f8c0: 496d 706c 656d 656e 7461 7469 6f6e 206f  Implementation o
+0000f8d0: 6620 5369 6d70 6c65 2053 7461 626c 6520  f Simple Stable 
+0000f8e0: 566f 7469 6e67 2066 726f 6d20 6874 7470  Voting from http
+0000f8f0: 733a 2f2f 6172 7869 762e 6f72 672f 6162  s://arxiv.org/ab
+0000f900: 732f 3231 3038 2e30 3035 3432 2e20 0a0a  s/2108.00542. ..
+0000f910: 2020 2020 5369 6d70 6c65 2053 7461 626c      Simple Stabl
+0000f920: 6520 566f 7469 6e67 2069 7320 6120 7265  e Voting is a re
+0000f930: 6375 7273 6976 6520 766f 7469 6e67 206d  cursive voting m
+0000f940: 6574 686f 6420 6465 6669 6e65 6420 6173  ethod defined as
+0000f950: 2066 6f6c 6c6f 7773 3a20 0a0a 2020 2020   follows: ..    
+0000f960: 312e 2049 6620 7468 6572 6520 6973 206f  1. If there is o
+0000f970: 6e6c 7920 6f6e 6520 6361 6e64 6964 6174  nly one candidat
+0000f980: 6520 696e 2074 6865 2070 726f 6669 6c65  e in the profile
+0000f990: 2c20 7468 656e 2074 6861 7420 6361 6e64  , then that cand
+0000f9a0: 6964 6174 6520 6973 2074 6865 2077 696e  idate is the win
+0000f9b0: 6e65 722e 200a 2020 2020 322e 204f 7264  ner. .    2. Ord
+0000f9c0: 6572 2074 6865 2070 6169 7273 203a 6d61  er the pairs :ma
+0000f9d0: 7468 3a60 2861 2c62 2960 206f 6620 6361  th:`(a,b)` of ca
+0000f9e0: 6e64 6964 6174 6573 2066 726f 6d20 6c61  ndidates from la
+0000f9f0: 7267 6573 7420 746f 2073 6d61 6c6c 6573  rgest to smalles
+0000fa00: 7420 7661 6c75 6520 6f66 2074 6865 206d  t value of the m
+0000fa10: 6172 6769 6e20 6f66 203a 6d61 7468 3a60  argin of :math:`
+0000fa20: 6160 206f 7665 7220 3a6d 6174 683a 6062  a` over :math:`b
+0000fa30: 602c 2061 6e64 2064 6563 6c61 7265 2061  `, and declare a
+0000fa40: 7320 5369 6d70 6c65 2053 7461 626c 6520  s Simple Stable 
+0000fa50: 566f 7469 6e67 2077 696e 6e65 7273 2074  Voting winners t
+0000fa60: 6865 2063 616e 6469 6461 7465 2873 2920  he candidate(s) 
+0000fa70: 3a6d 6174 683a 6061 6020 6672 6f6d 2074  :math:`a` from t
+0000fa80: 6865 2065 6172 6c69 6573 7420 7061 6972  he earliest pair
+0000fa90: 2873 2920 3a6d 6174 683a 6028 612c 6229  (s) :math:`(a,b)
+0000faa0: 6020 7375 6368 2074 6861 7420 3a6d 6174  ` such that :mat
+0000fab0: 683a 6061 6020 6973 2061 2053 696d 706c  h:`a` is a Simpl
+0000fac0: 6520 5374 6162 6c65 2056 6f74 696e 6720  e Stable Voting 
+0000fad0: 7769 6e6e 6572 2069 6e20 7468 6520 656c  winner in the el
+0000fae0: 6563 7469 6f6e 2077 6974 686f 7574 203a  ection without :
+0000faf0: 6d61 7468 3a60 6260 2e20 0a0a 2020 2020  math:`b`. ..    
+0000fb00: 4172 6773 3a0a 2020 2020 2020 2020 6564  Args:.        ed
+0000fb10: 6174 6120 2850 726f 6669 6c65 2c20 5072  ata (Profile, Pr
+0000fb20: 6f66 696c 6557 6974 6854 6965 732c 204d  ofileWithTies, M
+0000fb30: 6172 6769 6e47 7261 7068 293a 2041 6e79  arginGraph): Any
+0000fb40: 2065 6c65 6374 696f 6e20 6461 7461 2074   election data t
+0000fb50: 6861 7420 6861 7320 6120 606d 6172 6769  hat has a `margi
+0000fb60: 6e60 206d 6574 686f 642e 200a 2020 2020  n` method. .    
+0000fb70: 2020 2020 6375 7272 5f63 616e 6473 2028      curr_cands (
+0000fb80: 4c69 7374 5b69 6e74 5d2c 206f 7074 696f  List[int], optio
+0000fb90: 6e61 6c29 3a20 4966 2073 6574 2c20 7468  nal): If set, th
+0000fba0: 656e 2066 696e 6420 7468 6520 7769 6e6e  en find the winn
+0000fbb0: 6572 7320 666f 7220 7468 6520 7072 6f66  ers for the prof
+0000fbc0: 696c 6520 7265 7374 7269 6374 6564 2074  ile restricted t
+0000fbd0: 6f20 7468 6520 6361 6e64 6964 6174 6573  o the candidates
+0000fbe0: 2069 6e20 6060 6375 7272 5f63 616e 6473   in ``curr_cands
+0000fbf0: 6060 0a20 2020 2020 2020 2073 7472 656e  ``.        stren
+0000fc00: 6774 685f 6675 6e63 7469 6f6e 2028 6675  gth_function (fu
+0000fc10: 6e63 7469 6f6e 2c20 6f70 7469 6f6e 616c  nction, optional
+0000fc20: 293a 2054 6865 2073 7472 656e 6774 6820  ): The strength 
+0000fc30: 6675 6e63 7469 6f6e 2074 6f20 6265 2075  function to be u
+0000fc40: 7365 6420 746f 2063 616c 6375 6c61 7465  sed to calculate
+0000fc50: 2074 6865 2073 7472 656e 6774 6820 6f66   the strength of
+0000fc60: 2061 2070 6174 682e 2020 2054 6865 2064   a path.   The d
+0000fc70: 6566 6175 6c74 2069 7320 7468 6520 6d61  efault is the ma
+0000fc80: 7267 696e 206d 6574 686f 6420 6f66 2060  rgin method of `
+0000fc90: 6065 6461 7461 6060 2e20 2020 5468 6973  `edata``.   This
+0000fca0: 206f 6e6c 7920 6d61 7474 6572 7320 7768   only matters wh
+0000fcb0: 656e 2074 6865 2062 616c 6c6f 7473 2061  en the ballots a
+0000fcc0: 7265 206e 6f74 206c 696e 6561 7220 6f72  re not linear or
+0000fcd0: 6465 7273 2e20 0a20 2020 2020 2020 2061  ders. .        a
+0000fce0: 6c67 6f72 6974 686d 2028 7374 722c 206f  lgorithm (str, o
+0000fcf0: 7074 696f 6e61 6c29 3a20 5370 6563 6966  ptional): Specif
+0000fd00: 7920 7768 6963 6820 616c 676f 7269 7468  y which algorith
+0000fd10: 6d20 746f 2075 7365 2e20 204f 7074 696f  m to use.  Optio
+0000fd20: 6e73 2061 7265 2027 6261 7369 6327 2028  ns are 'basic' (
+0000fd30: 7468 6520 6465 6661 756c 7429 2061 6e64  the default) and
+0000fd40: 2027 7769 7468 5f63 6f6e 646f 7263 6574   'with_condorcet
+0000fd50: 5f63 6865 636b 272e 0a0a 2020 2020 5265  _check'...    Re
+0000fd60: 7475 726e 733a 200a 2020 2020 2020 2020  turns: .        
+0000fd70: 4120 736f 7274 6564 206c 6973 7420 6f66  A sorted list of
+0000fd80: 2063 616e 6469 6461 7465 732e 200a 0a20   candidates. .. 
+0000fd90: 2020 202e 2e20 7365 6561 6c73 6f3a 3a0a     .. seealso::.
+0000fda0: 0a20 2020 2020 2020 203a 6d65 7468 3a60  .        :meth:`
+0000fdb0: 7072 6566 5f76 6f74 696e 672e 6d61 7267  pref_voting.marg
+0000fdc0: 696e 5f62 6173 6564 5f6d 6574 686f 6473  in_based_methods
+0000fdd0: 2e73 7461 626c 655f 766f 7469 6e67 600a  .stable_voting`.
+0000fde0: 0a20 2020 203a 4578 616d 706c 653a 200a  .    :Example: .
+0000fdf0: 0a20 2020 202e 2e20 6578 6563 5f63 6f64  .    .. exec_cod
+0000fe00: 653a 3a0a 0a20 2020 2020 2020 2066 726f  e::..        fro
+0000fe10: 6d20 7072 6566 5f76 6f74 696e 672e 7765  m pref_voting.we
+0000fe20: 6967 6874 6564 5f6d 616a 6f72 6974 795f  ighted_majority_
+0000fe30: 6772 6170 6873 2069 6d70 6f72 7420 4d61  graphs import Ma
+0000fe40: 7267 696e 4772 6170 680a 2020 2020 2020  rginGraph.      
+0000fe50: 2020 6672 6f6d 2070 7265 665f 766f 7469    from pref_voti
+0000fe60: 6e67 2e6d 6172 6769 6e5f 6261 7365 645f  ng.margin_based_
+0000fe70: 6d65 7468 6f64 7320 696d 706f 7274 2073  methods import s
+0000fe80: 696d 706c 655f 7374 6162 6c65 5f76 6f74  imple_stable_vot
+0000fe90: 696e 670a 0a20 2020 2020 2020 206d 6720  ing..        mg 
+0000fea0: 3d20 4d61 7267 696e 4772 6170 6828 5b30  = MarginGraph([0
+0000feb0: 2c20 312c 2032 2c20 335d 2c20 5b28 302c  , 1, 2, 3], [(0,
+0000fec0: 2033 2c20 3829 2c20 2831 2c20 302c 2031   3, 8), (1, 0, 1
+0000fed0: 3029 2c20 2832 2c20 302c 2034 292c 2028  0), (2, 0, 4), (
+0000fee0: 322c 2031 2c20 3829 2c20 2833 2c20 312c  2, 1, 8), (3, 1,
+0000fef0: 2038 295d 290a 0a20 2020 2020 2020 2073   8)])..        s
+0000ff00: 696d 706c 655f 7374 6162 6c65 5f76 6f74  imple_stable_vot
+0000ff10: 696e 672e 6469 7370 6c61 7928 6d67 290a  ing.display(mg).
+0000ff20: 2020 2020 2020 2020 7369 6d70 6c65 5f73          simple_s
+0000ff30: 7461 626c 655f 766f 7469 6e67 2e64 6973  table_voting.dis
+0000ff40: 706c 6179 286d 672c 2061 6c67 6f72 6974  play(mg, algorit
+0000ff50: 686d 3d27 6261 7369 6327 290a 2020 2020  hm='basic').    
+0000ff60: 2020 2020 7369 6d70 6c65 5f73 7461 626c      simple_stabl
+0000ff70: 655f 766f 7469 6e67 2e64 6973 706c 6179  e_voting.display
+0000ff80: 286d 672c 2061 6c67 6f72 6974 686d 3d27  (mg, algorithm='
+0000ff90: 7769 7468 5f63 6f6e 646f 7263 6574 5f63  with_condorcet_c
+0000ffa0: 6865 636b 2729 0a0a 2020 2020 2222 220a  heck')..    """.
+0000ffb0: 2020 2020 0a20 2020 2069 6620 616c 676f      .    if algo
+0000ffc0: 7269 7468 6d20 3d3d 2027 6261 7369 6327  rithm == 'basic'
+0000ffd0: 3a20 0a20 2020 2020 2020 2072 6574 7572  : .        retur
+0000ffe0: 6e20 5f73 696d 706c 655f 7374 6162 6c65  n _simple_stable
+0000fff0: 5f76 6f74 696e 675f 6261 7369 6328 6564  _voting_basic(ed
+00010000: 6174 612c 2063 7572 725f 6361 6e64 7320  ata, curr_cands 
+00010010: 3d20 6375 7272 5f63 616e 6473 2c20 7374  = curr_cands, st
+00010020: 7265 6e67 7468 5f66 756e 6374 696f 6e20  rength_function 
+00010030: 3d20 7374 7265 6e67 7468 5f66 756e 6374  = strength_funct
+00010040: 696f 6e29 0a20 2020 2065 6c69 6620 616c  ion).    elif al
+00010050: 676f 7269 7468 6d20 3d3d 2027 7769 7468  gorithm == 'with
+00010060: 5f63 6f6e 646f 7263 6574 5f63 6865 636b  _condorcet_check
+00010070: 273a 0a20 2020 2020 2020 2072 6574 7572  ':.        retur
+00010080: 6e20 5f73 696d 706c 655f 7374 6162 6c65  n _simple_stable
+00010090: 5f76 6f74 696e 675f 7769 7468 5f63 6f6e  _voting_with_con
+000100a0: 646f 7263 6574 5f63 6865 636b 2865 6461  dorcet_check(eda
+000100b0: 7461 2c20 6375 7272 5f63 616e 6473 203d  ta, curr_cands =
+000100c0: 2063 7572 725f 6361 6e64 732c 2073 7472   curr_cands, str
+000100d0: 656e 6774 685f 6675 6e63 7469 6f6e 203d  ength_function =
+000100e0: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
+000100f0: 6f6e 290a 2020 2020 656c 7365 3a0a 2020  on).    else:.  
+00010100: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
+00010110: 6545 7272 6f72 2822 496e 7661 6c69 6420  eError("Invalid 
+00010120: 616c 676f 7269 7468 6d20 7370 6563 6966  algorithm specif
+00010130: 6965 642e 2229 0a20 2020 200a 0a64 6566  ied.").    ..def
+00010140: 205f 7374 6162 6c65 5f76 6f74 696e 6728   _stable_voting(
+00010150: 6564 6174 612c 200a 2020 2020 2020 2020  edata, .        
+00010160: 2020 2020 2020 2020 2020 2063 7572 725f             curr_
+00010170: 6361 6e64 732c 0a20 2020 2020 2020 2020  cands,.         
+00010180: 2020 2020 2020 2020 2020 7374 7265 6e67            streng
+00010190: 7468 5f66 756e 6374 696f 6e2c 0a20 2020  th_function,.   
+000101a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000101b0: 736f 7274 6564 5f6d 6174 6368 6573 2c0a  sorted_matches,.
+000101c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000101d0: 2020 206d 656d 5f73 765f 7769 6e6e 6572     mem_sv_winner
+000101e0: 7329 3a20 0a20 2020 2027 2727 0a20 2020  s): .    '''.   
+000101f0: 2044 6574 6572 6d69 6e65 2074 6865 2053   Determine the S
+00010200: 7461 626c 6520 566f 7469 6e67 2077 696e  table Voting win
+00010210: 6e65 7273 2066 6f72 2074 6865 2070 726f  ners for the pro
+00010220: 6669 6c65 2077 6869 6c65 206b 6565 7069  file while keepi
+00010230: 6e67 2074 7261 636b 206f 6620 7468 6520  ng track of the 
+00010240: 7769 6e6e 6572 7320 696e 2061 6e79 2073  winners in any s
+00010250: 7562 7072 6f66 696c 6573 2063 6865 636b  ubprofiles check
+00010260: 6564 2064 7572 696e 6720 636f 6d70 7574  ed during comput
+00010270: 6174 696f 6e2e 200a 2020 2020 2727 270a  ation. .    '''.
+00010280: 2020 2020 0a20 2020 2073 765f 7769 6e6e      .    sv_winn
+00010290: 6572 7320 3d20 6c69 7374 2829 0a20 2020  ers = list().   
+000102a0: 200a 2020 2020 756e 6465 6665 6174 6564   .    undefeated
+000102b0: 5f63 616e 6469 6461 7465 7320 3d20 7370  _candidates = sp
+000102c0: 6c69 745f 6379 636c 6528 6564 6174 612c  lit_cycle(edata,
+000102d0: 2063 7572 725f 6361 6e64 7320 3d20 6375   curr_cands = cu
+000102e0: 7272 5f63 616e 6473 2c20 7374 7265 6e67  rr_cands, streng
+000102f0: 7468 5f66 756e 6374 696f 6e20 3d20 7374  th_function = st
+00010300: 7265 6e67 7468 5f66 756e 6374 696f 6e29  rength_function)
+00010310: 0a0a 2020 2020 6966 206c 656e 2863 7572  ..    if len(cur
+00010320: 725f 6361 6e64 7329 203d 3d20 313a 200a  r_cands) == 1: .
+00010330: 2020 2020 2020 2020 6d65 6d5f 7376 5f77          mem_sv_w
+00010340: 696e 6e65 7273 5b74 7570 6c65 2863 7572  inners[tuple(cur
+00010350: 725f 6361 6e64 7329 5d20 3d20 6375 7272  r_cands)] = curr
+00010360: 5f63 616e 6473 0a20 2020 2020 2020 2072  _cands.        r
+00010370: 6574 7572 6e20 6375 7272 5f63 616e 6473  eturn curr_cands
+00010380: 2c20 6d65 6d5f 7376 5f77 696e 6e65 7273  , mem_sv_winners
+00010390: 0a20 2020 200a 2020 2020 6d61 7267 696e  .    .    margin
+000103a0: 5f77 6974 6e65 7373 696e 675f 7769 6e20  _witnessing_win 
+000103b0: 3d20 2d6d 6174 682e 696e 660a 0a20 2020  = -math.inf..   
+000103c0: 2066 6f72 2061 2c20 622c 2073 2069 6e20   for a, b, s in 
+000103d0: 736f 7274 6564 5f6d 6174 6368 6573 3a0a  sorted_matches:.
+000103e0: 2020 2020 2020 2020 6966 2073 203c 206d          if s < m
+000103f0: 6172 6769 6e5f 7769 746e 6573 7369 6e67  argin_witnessing
+00010400: 5f77 696e 3a20 0a20 2020 2020 2020 2020  _win: .         
+00010410: 2020 2062 7265 616b 0a20 2020 2020 2020     break.       
+00010420: 2069 6620 6120 696e 2075 6e64 6566 6561   if a in undefea
+00010430: 7465 645f 6361 6e64 6964 6174 6573 2061  ted_candidates a
+00010440: 6e64 2061 206e 6f74 2069 6e20 7376 5f77  nd a not in sv_w
+00010450: 696e 6e65 7273 3a20 0a20 2020 2020 2020  inners: .       
+00010460: 2020 2020 2063 616e 6473 5f6d 696e 7573       cands_minus
+00010470: 5f62 203d 205b 6320 666f 7220 6320 696e  _b = [c for c in
+00010480: 2063 7572 725f 6361 6e64 7320 6966 2063   curr_cands if c
+00010490: 2021 3d20 625d 0a20 2020 2020 2020 2020   != b].         
+000104a0: 2020 2063 616e 6473 5f6d 696e 7573 5f62     cands_minus_b
+000104b0: 5f6b 6579 203d 2074 7570 6c65 2873 6f72  _key = tuple(sor
+000104c0: 7465 6428 6361 6e64 735f 6d69 6e75 735f  ted(cands_minus_
+000104d0: 6229 290a 2020 2020 2020 2020 2020 2020  b)).            
+000104e0: 6966 2063 616e 6473 5f6d 696e 7573 5f62  if cands_minus_b
+000104f0: 5f6b 6579 206e 6f74 2069 6e20 6d65 6d5f  _key not in mem_
+00010500: 7376 5f77 696e 6e65 7273 2e6b 6579 7328  sv_winners.keys(
+00010510: 293a 200a 2020 2020 2020 2020 2020 2020  ): .            
+00010520: 2020 2020 7773 2c20 6d65 6d5f 7376 5f77      ws, mem_sv_w
+00010530: 696e 6e65 7273 203d 205f 7374 6162 6c65  inners = _stable
+00010540: 5f76 6f74 696e 6728 6564 6174 612c 0a20  _voting(edata,. 
+00010550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010580: 2020 2063 7572 725f 6361 6e64 7320 3d20     curr_cands = 
+00010590: 6361 6e64 735f 6d69 6e75 735f 622c 0a20  cands_minus_b,. 
+000105a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000105b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000105c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000105d0: 2020 2073 7472 656e 6774 685f 6675 6e63     strength_func
+000105e0: 7469 6f6e 203d 2073 7472 656e 6774 685f  tion = strength_
+000105f0: 6675 6e63 7469 6f6e 2c0a 2020 2020 2020  function,.      
+00010600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010620: 2020 2020 2020 2020 2020 2020 2020 736f                so
+00010630: 7274 6564 5f6d 6174 6368 6573 203d 205b  rted_matches = [
+00010640: 2861 2c20 632c 2073 2920 666f 7220 612c  (a, c, s) for a,
+00010650: 2063 2c20 7320 696e 2073 6f72 7465 645f   c, s in sorted_
+00010660: 6d61 7463 6865 7320 6966 2061 2021 3d20  matches if a != 
+00010670: 6220 616e 6420 6320 213d 2062 5d2c 0a20  b and c != b],. 
+00010680: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00010690: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000106a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000106b0: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
-000106c0: 6f6e 203d 2073 7472 656e 6774 685f 6675  on = strength_fu
-000106d0: 6e63 7469 6f6e 2c0a 2020 2020 2020 2020  nction,.        
-000106e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000106f0: 2020 2020 2020 2020 2020 2020 736f 7274              sort
-00010700: 6564 5f6d 6174 6368 6573 203d 2073 6f72  ed_matches = sor
-00010710: 7465 645f 6d61 7463 6865 732c 0a20 2020  ted_matches,.   
-00010720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010740: 206d 656d 5f73 765f 7769 6e6e 6572 7320   mem_sv_winners 
-00010750: 3d20 7b7d 295b 305d 290a 0a64 6566 205f  = {})[0])..def _
-00010760: 7374 6162 6c65 5f76 6f74 696e 675f 6261  stable_voting_ba
-00010770: 7369 6328 0a20 2020 2020 2020 2065 6461  sic(.        eda
-00010780: 7461 2c20 0a20 2020 2020 2020 2063 7572  ta, .        cur
-00010790: 725f 6361 6e64 7320 3d20 4e6f 6e65 2c20  r_cands = None, 
-000107a0: 0a20 2020 2020 2020 2073 7472 656e 6774  .        strengt
-000107b0: 685f 6675 6e63 7469 6f6e 203d 204e 6f6e  h_function = Non
-000107c0: 6529 3a20 0a20 2020 2022 2222 496d 706c  e): .    """Impl
-000107d0: 656d 656e 7461 7469 6f6e 206f 6620 2053  ementation of  S
-000107e0: 7461 626c 6520 566f 7469 6e67 2066 726f  table Voting fro
-000107f0: 6d20 6874 7470 733a 2f2f 6172 7869 762e  m https://arxiv.
-00010800: 6f72 672f 6162 732f 3231 3038 2e30 3035  org/abs/2108.005
-00010810: 3432 2e20 0a0a 2020 2020 4172 6773 3a0a  42. ..    Args:.
-00010820: 2020 2020 2020 2020 6564 6174 6120 2850          edata (P
-00010830: 726f 6669 6c65 2c20 5072 6f66 696c 6557  rofile, ProfileW
-00010840: 6974 6854 6965 732c 204d 6172 6769 6e47  ithTies, MarginG
-00010850: 7261 7068 293a 2041 6e79 2065 6c65 6374  raph): Any elect
-00010860: 696f 6e20 6461 7461 2074 6861 7420 6861  ion data that ha
-00010870: 7320 6120 606d 6172 6769 6e60 206d 6574  s a `margin` met
-00010880: 686f 642e 200a 2020 2020 2020 2020 6375  hod. .        cu
-00010890: 7272 5f63 616e 6473 2028 4c69 7374 5b69  rr_cands (List[i
-000108a0: 6e74 5d2c 206f 7074 696f 6e61 6c29 3a20  nt], optional): 
-000108b0: 4966 2073 6574 2c20 7468 656e 2066 696e  If set, then fin
-000108c0: 6420 7468 6520 7769 6e6e 6572 7320 666f  d the winners fo
-000108d0: 7220 7468 6520 7072 6f66 696c 6520 7265  r the profile re
-000108e0: 7374 7269 6374 6564 2074 6f20 7468 6520  stricted to the 
-000108f0: 6361 6e64 6964 6174 6573 2069 6e20 6060  candidates in ``
-00010900: 6375 7272 5f63 616e 6473 6060 0a20 2020  curr_cands``.   
-00010910: 2020 2020 2073 7472 656e 6774 685f 6675       strength_fu
-00010920: 6e63 7469 6f6e 2028 6675 6e63 7469 6f6e  nction (function
-00010930: 2c20 6f70 7469 6f6e 616c 293a 2054 6865  , optional): The
-00010940: 2073 7472 656e 6774 6820 6675 6e63 7469   strength functi
-00010950: 6f6e 2074 6f20 6265 2075 7365 6420 746f  on to be used to
-00010960: 2063 616c 6375 6c61 7465 2074 6865 2073   calculate the s
-00010970: 7472 656e 6774 6820 6f66 2061 2070 6174  trength of a pat
-00010980: 682e 2020 2054 6865 2064 6566 6175 6c74  h.   The default
-00010990: 2069 7320 7468 6520 6d61 7267 696e 206d   is the margin m
-000109a0: 6574 686f 6420 6f66 2060 6065 6461 7461  ethod of ``edata
-000109b0: 6060 2e20 2020 5468 6973 206f 6e6c 7920  ``.   This only 
-000109c0: 6d61 7474 6572 7320 7768 656e 2074 6865  matters when the
-000109d0: 2062 616c 6c6f 7473 2061 7265 206e 6f74   ballots are not
-000109e0: 206c 696e 6561 7220 6f72 6465 7273 2e20   linear orders. 
-000109f0: 0a0a 2020 2020 5265 7475 726e 733a 200a  ..    Returns: .
-00010a00: 2020 2020 2020 2020 4120 736f 7274 6564          A sorted
-00010a10: 206c 6973 7420 6f66 2063 616e 6469 6461   list of candida
-00010a20: 7465 732e 200a 0a20 2020 2022 2222 0a0a  tes. ..    """..
-00010a30: 2020 2020 6375 7272 5f63 616e 6473 203d      curr_cands =
-00010a40: 2065 6461 7461 2e63 616e 6469 6461 7465   edata.candidate
-00010a50: 7320 6966 2063 7572 725f 6361 6e64 7320  s if curr_cands 
-00010a60: 6973 204e 6f6e 6520 656c 7365 2063 7572  is None else cur
-00010a70: 725f 6361 6e64 730a 2020 2020 7374 7265  r_cands.    stre
-00010a80: 6e67 7468 5f66 756e 6374 696f 6e20 3d20  ngth_function = 
-00010a90: 6564 6174 612e 6d61 7267 696e 2069 6620  edata.margin if 
-00010aa0: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
-00010ab0: 6e20 6973 204e 6f6e 6520 656c 7365 2073  n is None else s
-00010ac0: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
-00010ad0: 2020 0a0a 2020 2020 6d61 7463 6865 7320    ..    matches 
-00010ae0: 3d20 5b28 612c 2062 2c20 7374 7265 6e67  = [(a, b, streng
-00010af0: 7468 5f66 756e 6374 696f 6e28 612c 2062  th_function(a, b
-00010b00: 2929 2066 6f72 2061 2069 6e20 6375 7272  )) for a in curr
-00010b10: 5f63 616e 6473 2066 6f72 2062 2069 6e20  _cands for b in 
-00010b20: 6375 7272 5f63 616e 6473 2069 6620 6120  curr_cands if a 
-00010b30: 213d 2062 5d0a 2020 2020 736f 7274 6564  != b].    sorted
-00010b40: 5f6d 6174 6368 6573 203d 2073 6f72 7465  _matches = sorte
-00010b50: 6428 6d61 7463 6865 732c 2072 6576 6572  d(matches, rever
-00010b60: 7365 3d54 7275 652c 206b 6579 3d6c 616d  se=True, key=lam
-00010b70: 6264 6120 6d5f 775f 7765 6967 6874 3a20  bda m_w_weight: 
-00010b80: 6d5f 775f 7765 6967 6874 5b32 5d29 0a0a  m_w_weight[2])..
-00010b90: 2020 2020 7265 7475 726e 2073 6f72 7465      return sorte
-00010ba0: 6428 5f73 7461 626c 655f 766f 7469 6e67  d(_stable_voting
-00010bb0: 2865 6461 7461 2c20 0a20 2020 2020 2020  (edata, .       
-00010bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010bd0: 2020 2020 2020 2020 2020 6375 7272 5f63            curr_c
-00010be0: 616e 6473 203d 2063 7572 725f 6361 6e64  ands = curr_cand
-00010bf0: 732c 200a 2020 2020 2020 2020 2020 2020  s, .            
-00010c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010c10: 2020 2020 2073 7472 656e 6774 685f 6675       strength_fu
-00010c20: 6e63 7469 6f6e 203d 2073 7472 656e 6774  nction = strengt
-00010c30: 685f 6675 6e63 7469 6f6e 2c0a 2020 2020  h_function,.    
-00010c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010c50: 2020 2020 2020 2020 2020 2020 2073 6f72               sor
-00010c60: 7465 645f 6d61 7463 6865 7320 3d20 736f  ted_matches = so
-00010c70: 7274 6564 5f6d 6174 6368 6573 2c0a 2020  rted_matches,.  
-00010c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010c90: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-00010ca0: 656d 5f73 765f 7769 6e6e 6572 7320 3d20  em_sv_winners = 
-00010cb0: 7b7d 295b 305d 290a 0a73 765f 7072 6f70  {})[0])..sv_prop
-00010cc0: 6572 7469 6573 203d 2056 6f74 696e 674d  erties = VotingM
-00010cd0: 6574 686f 6450 726f 7065 7274 6965 7328  ethodProperties(
-00010ce0: 0a20 2020 2063 6f6e 646f 7263 6574 5f77  .    condorcet_w
-00010cf0: 696e 6e65 723d 5472 7565 2c20 0a20 2020  inner=True, .   
-00010d00: 2063 6f6e 646f 7263 6574 5f6c 6f73 6572   condorcet_loser
-00010d10: 3d54 7275 652c 0a20 2020 2070 6172 6574  =True,.    paret
-00010d20: 6f5f 646f 6d69 6e61 6e63 653d 5472 7565  o_dominance=True
-00010d30: 2c0a 2020 2020 706f 7369 7469 7665 5f69  ,.    positive_i
-00010d40: 6e76 6f6c 7665 6d65 6e74 3d46 616c 7365  nvolvement=False
-00010d50: 2c20 200a 2020 2020 290a 4076 6d28 6e61  ,  .    ).@vm(na
-00010d60: 6d65 203d 2022 5374 6162 6c65 2056 6f74  me = "Stable Vot
-00010d70: 696e 6722 2c0a 2020 2020 7072 6f70 6572  ing",.    proper
-00010d80: 7469 6573 203d 2073 765f 7072 6f70 6572  ties = sv_proper
-00010d90: 7469 6573 2c0a 2020 2020 696e 7075 745f  ties,.    input_
-00010da0: 7479 7065 7320 3d20 5b45 6c65 6374 696f  types = [Electio
-00010db0: 6e54 7970 6573 2e50 524f 4649 4c45 2c20  nTypes.PROFILE, 
-00010dc0: 456c 6563 7469 6f6e 5479 7065 732e 5052  ElectionTypes.PR
-00010dd0: 4f46 494c 455f 5749 5448 5f54 4945 532c  OFILE_WITH_TIES,
-00010de0: 2045 6c65 6374 696f 6e54 7970 6573 2e4d   ElectionTypes.M
-00010df0: 4152 4749 4e5f 4752 4150 485d 290a 6465  ARGIN_GRAPH]).de
-00010e00: 6620 7374 6162 6c65 5f76 6f74 696e 6728  f stable_voting(
-00010e10: 0a20 2020 2065 6461 7461 2c20 0a20 2020  .    edata, .   
-00010e20: 2063 7572 725f 6361 6e64 733d 4e6f 6e65   curr_cands=None
-00010e30: 2c20 0a20 2020 2073 7472 656e 6774 685f  , .    strength_
-00010e40: 6675 6e63 7469 6f6e 3d4e 6f6e 652c 200a  function=None, .
-00010e50: 2020 2020 616c 676f 7269 7468 6d3d 2762      algorithm='b
-00010e60: 6173 6963 2729 3a20 0a20 2020 2022 2222  asic'): .    """
-00010e70: 496d 706c 656d 656e 7461 7469 6f6e 206f  Implementation o
-00010e80: 6620 2053 7461 626c 6520 566f 7469 6e67  f  Stable Voting
-00010e90: 2066 726f 6d20 6874 7470 733a 2f2f 6172   from https://ar
-00010ea0: 7869 762e 6f72 672f 6162 732f 3231 3038  xiv.org/abs/2108
-00010eb0: 2e30 3035 3432 2e20 0a0a 2020 2020 5374  .00542. ..    St
-00010ec0: 6162 6c65 2056 6f74 696e 6720 6973 2061  able Voting is a
-00010ed0: 2072 6563 7572 7369 7665 2076 6f74 696e   recursive votin
-00010ee0: 6720 6d65 7468 6f64 2064 6566 696e 6564  g method defined
-00010ef0: 2061 7320 666f 6c6c 6f77 733a 200a 0a20   as follows: .. 
-00010f00: 2020 2031 2e20 2049 6620 7468 6572 6520     1.  If there 
-00010f10: 6973 206f 6e6c 7920 6f6e 6520 6361 6e64  is only one cand
-00010f20: 6964 6174 6520 696e 2074 6865 2070 726f  idate in the pro
-00010f30: 6669 6c65 2c20 7468 656e 2074 6861 7420  file, then that 
-00010f40: 6361 6e64 6964 6174 6520 6973 2074 6865  candidate is the
-00010f50: 2077 696e 6e65 722e 200a 2020 2020 322e   winner. .    2.
-00010f60: 204f 7264 6572 2074 6865 2070 6169 7273   Order the pairs
-00010f70: 203a 6d61 7468 3a60 2861 2c62 2960 206f   :math:`(a,b)` o
-00010f80: 6620 6361 6e64 6964 6174 6573 2066 726f  f candidates fro
-00010f90: 6d20 6c61 7267 6573 7420 746f 2073 6d61  m largest to sma
-00010fa0: 6c6c 6573 7420 7661 6c75 6520 6f66 2074  llest value of t
-00010fb0: 6865 206d 6172 6769 6e20 6f66 203a 6d61  he margin of :ma
-00010fc0: 7468 3a60 6160 206f 7665 7220 3a6d 6174  th:`a` over :mat
-00010fd0: 683a 6062 6020 7375 6368 2074 6861 7420  h:`b` such that 
-00010fe0: 3a6d 6174 683a 6061 6020 6973 2075 6e64  :math:`a` is und
-00010ff0: 6566 6561 7465 6420 6163 636f 7264 696e  efeated accordin
-00011000: 6720 746f 2053 706c 6974 2043 7963 6c65  g to Split Cycle
-00011010: 2c20 616e 6420 6465 636c 6172 6520 6173  , and declare as
-00011020: 2053 7461 626c 6520 566f 7469 6e67 2077   Stable Voting w
-00011030: 696e 6e65 7273 2074 6865 2063 616e 6469  inners the candi
-00011040: 6461 7465 2873 2920 3a6d 6174 683a 6061  date(s) :math:`a
-00011050: 6020 6672 6f6d 2074 6865 2065 6172 6c69  ` from the earli
-00011060: 6573 7420 7061 6972 2873 2920 3a6d 6174  est pair(s) :mat
-00011070: 683a 6028 612c 6229 6020 7375 6368 2074  h:`(a,b)` such t
-00011080: 6861 7420 3a6d 6174 683a 6061 6020 6973  hat :math:`a` is
-00011090: 2061 2053 696d 706c 6520 5374 6162 6c65   a Simple Stable
-000110a0: 2056 6f74 696e 6720 7769 6e6e 6572 2069   Voting winner i
-000110b0: 6e20 7468 6520 656c 6563 7469 6f6e 2077  n the election w
-000110c0: 6974 686f 7574 203a 6d61 7468 3a60 6260  ithout :math:`b`
-000110d0: 2e20 0a0a 2020 2020 4172 6773 3a0a 2020  . ..    Args:.  
-000110e0: 2020 2020 2020 6564 6174 6120 2850 726f        edata (Pro
-000110f0: 6669 6c65 2c20 5072 6f66 696c 6557 6974  file, ProfileWit
-00011100: 6854 6965 732c 204d 6172 6769 6e47 7261  hTies, MarginGra
-00011110: 7068 293a 2041 6e79 2065 6c65 6374 696f  ph): Any electio
-00011120: 6e20 6461 7461 2074 6861 7420 6861 7320  n data that has 
-00011130: 6120 606d 6172 6769 6e60 206d 6574 686f  a `margin` metho
-00011140: 642e 200a 2020 2020 2020 2020 6375 7272  d. .        curr
-00011150: 5f63 616e 6473 2028 4c69 7374 5b69 6e74  _cands (List[int
-00011160: 5d2c 206f 7074 696f 6e61 6c29 3a20 4966  ], optional): If
-00011170: 2073 6574 2c20 7468 656e 2066 696e 6420   set, then find 
-00011180: 7468 6520 7769 6e6e 6572 7320 666f 7220  the winners for 
-00011190: 7468 6520 7072 6f66 696c 6520 7265 7374  the profile rest
-000111a0: 7269 6374 6564 2074 6f20 7468 6520 6361  ricted to the ca
-000111b0: 6e64 6964 6174 6573 2069 6e20 6060 6375  ndidates in ``cu
-000111c0: 7272 5f63 616e 6473 6060 0a20 2020 2020  rr_cands``.     
-000111d0: 2020 2073 7472 656e 6774 685f 6675 6e63     strength_func
-000111e0: 7469 6f6e 2028 6675 6e63 7469 6f6e 2c20  tion (function, 
-000111f0: 6f70 7469 6f6e 616c 293a 2054 6865 2073  optional): The s
-00011200: 7472 656e 6774 6820 6675 6e63 7469 6f6e  trength function
-00011210: 2074 6f20 6265 2075 7365 6420 746f 2063   to be used to c
-00011220: 616c 6375 6c61 7465 2074 6865 2073 7472  alculate the str
-00011230: 656e 6774 6820 6f66 2061 2070 6174 682e  ength of a path.
-00011240: 2020 2054 6865 2064 6566 6175 6c74 2069     The default i
-00011250: 7320 7468 6520 6d61 7267 696e 206d 6574  s the margin met
-00011260: 686f 6420 6f66 2060 6065 6461 7461 6060  hod of ``edata``
-00011270: 2e20 2020 5468 6973 206f 6e6c 7920 6d61  .   This only ma
-00011280: 7474 6572 7320 7768 656e 2074 6865 2062  tters when the b
-00011290: 616c 6c6f 7473 2061 7265 206e 6f74 206c  allots are not l
-000112a0: 696e 6561 7220 6f72 6465 7273 2e20 0a0a  inear orders. ..
-000112b0: 2020 2020 5265 7475 726e 733a 200a 2020      Returns: .  
-000112c0: 2020 2020 2020 4120 736f 7274 6564 206c        A sorted l
-000112d0: 6973 7420 6f66 2063 616e 6469 6461 7465  ist of candidate
-000112e0: 732e 200a 0a20 2020 202e 2e20 7365 6561  s. ..    .. seea
-000112f0: 6c73 6f3a 3a0a 0a20 2020 2020 2020 203a  lso::..        :
-00011300: 6d65 7468 3a60 7072 6566 5f76 6f74 696e  meth:`pref_votin
-00011310: 672e 6d61 7267 696e 5f62 6173 6564 5f6d  g.margin_based_m
-00011320: 6574 686f 6473 2e73 696d 706c 655f 7374  ethods.simple_st
-00011330: 6162 6c65 5f76 6f74 696e 6760 0a0a 0a20  able_voting`... 
-00011340: 2020 203a 4578 616d 706c 653a 200a 0a20     :Example: .. 
-00011350: 2020 202e 2e20 6578 6563 5f63 6f64 653a     .. exec_code:
-00011360: 3a0a 0a20 2020 2020 2020 2066 726f 6d20  :..        from 
-00011370: 7072 6566 5f76 6f74 696e 672e 7765 6967  pref_voting.weig
-00011380: 6874 6564 5f6d 616a 6f72 6974 795f 6772  hted_majority_gr
-00011390: 6170 6873 2069 6d70 6f72 7420 4d61 7267  aphs import Marg
-000113a0: 696e 4772 6170 680a 2020 2020 2020 2020  inGraph.        
-000113b0: 6672 6f6d 2070 7265 665f 766f 7469 6e67  from pref_voting
-000113c0: 2e6d 6172 6769 6e5f 6261 7365 645f 6d65  .margin_based_me
-000113d0: 7468 6f64 7320 696d 706f 7274 2073 7461  thods import sta
-000113e0: 626c 655f 766f 7469 6e67 0a0a 2020 2020  ble_voting..    
-000113f0: 2020 2020 6d67 203d 204d 6172 6769 6e47      mg = MarginG
-00011400: 7261 7068 285b 302c 2031 2c20 322c 2033  raph([0, 1, 2, 3
-00011410: 5d2c 205b 2830 2c20 332c 2038 292c 2028  ], [(0, 3, 8), (
-00011420: 312c 2030 2c20 3130 292c 2028 322c 2030  1, 0, 10), (2, 0
-00011430: 2c20 3429 2c20 2832 2c20 312c 2038 292c  , 4), (2, 1, 8),
-00011440: 2028 332c 2031 2c20 3829 5d29 0a0a 2020   (3, 1, 8)])..  
-00011450: 2020 2020 2020 7374 6162 6c65 5f76 6f74        stable_vot
-00011460: 696e 672e 6469 7370 6c61 7928 6d67 290a  ing.display(mg).
-00011470: 2020 2020 2020 2020 7374 6162 6c65 5f76          stable_v
-00011480: 6f74 696e 672e 6469 7370 6c61 7928 6d67  oting.display(mg
-00011490: 2c20 616c 676f 7269 7468 6d3d 2762 6173  , algorithm='bas
-000114a0: 6963 2729 0a20 2020 2020 2020 2073 7461  ic').        sta
-000114b0: 626c 655f 766f 7469 6e67 2e64 6973 706c  ble_voting.displ
-000114c0: 6179 286d 672c 2061 6c67 6f72 6974 686d  ay(mg, algorithm
-000114d0: 3d27 7769 7468 5f63 6f6e 646f 7263 6574  ='with_condorcet
-000114e0: 5f63 6865 636b 2729 0a0a 2020 2020 2222  _check')..    ""
-000114f0: 220a 0a20 2020 2069 6620 616c 676f 7269  "..    if algori
-00011500: 7468 6d20 3d3d 2027 6261 7369 6327 3a20  thm == 'basic': 
-00011510: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00011520: 5f73 7461 626c 655f 766f 7469 6e67 5f62  _stable_voting_b
-00011530: 6173 6963 2865 6461 7461 2c20 6375 7272  asic(edata, curr
-00011540: 5f63 616e 6473 203d 2063 7572 725f 6361  _cands = curr_ca
-00011550: 6e64 732c 2073 7472 656e 6774 685f 6675  nds, strength_fu
-00011560: 6e63 7469 6f6e 203d 2073 7472 656e 6774  nction = strengt
-00011570: 685f 6675 6e63 7469 6f6e 290a 2020 2020  h_function).    
-00011580: 656c 6966 2061 6c67 6f72 6974 686d 203d  elif algorithm =
-00011590: 3d20 2777 6974 685f 636f 6e64 6f72 6365  = 'with_condorce
-000115a0: 745f 6368 6563 6b27 3a0a 2020 2020 2020  t_check':.      
-000115b0: 2020 7265 7475 726e 205f 7374 6162 6c65    return _stable
-000115c0: 5f76 6f74 696e 675f 7769 7468 5f63 6f6e  _voting_with_con
-000115d0: 646f 7263 6574 5f63 6865 636b 2865 6461  dorcet_check(eda
-000115e0: 7461 2c20 6375 7272 5f63 616e 6473 203d  ta, curr_cands =
-000115f0: 2063 7572 725f 6361 6e64 732c 2073 7472   curr_cands, str
-00011600: 656e 6774 685f 6675 6e63 7469 6f6e 203d  ength_function =
-00011610: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
-00011620: 6f6e 290a 2020 2020 656c 7365 3a0a 2020  on).    else:.  
-00011630: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
-00011640: 6545 7272 6f72 2822 496e 7661 6c69 6420  eError("Invalid 
-00011650: 616c 676f 7269 7468 6d20 7370 6563 6966  algorithm specif
-00011660: 6965 642e 2229 0a20 2020 200a 0a65 7373  ied.").    ..ess
-00011670: 656e 7469 616c 5f73 6574 5f70 726f 7065  ential_set_prope
-00011680: 7274 6965 7320 3d20 566f 7469 6e67 4d65  rties = VotingMe
-00011690: 7468 6f64 5072 6f70 6572 7469 6573 280a  thodProperties(.
-000116a0: 2020 2020 636f 6e64 6f72 6365 745f 7769      condorcet_wi
-000116b0: 6e6e 6572 3d54 7275 652c 200a 2020 2020  nner=True, .    
-000116c0: 636f 6e64 6f72 6365 745f 6c6f 7365 723d  condorcet_loser=
-000116d0: 5472 7565 2c0a 2020 2020 7061 7265 746f  True,.    pareto
-000116e0: 5f64 6f6d 696e 616e 6365 3d54 7275 652c  _dominance=True,
-000116f0: 0a20 2020 2070 6f73 6974 6976 655f 696e  .    positive_in
-00011700: 766f 6c76 656d 656e 743d 4661 6c73 652c  volvement=False,
-00011710: 200a 2020 2020 290a 4076 6d28 6e61 6d65   .    ).@vm(name
-00011720: 3d22 4573 7365 6e74 6961 6c20 5365 7422  ="Essential Set"
-00011730: 2c0a 2020 2020 7072 6f70 6572 7469 6573  ,.    properties
-00011740: 3d65 7373 656e 7469 616c 5f73 6574 5f70  =essential_set_p
-00011750: 726f 7065 7274 6965 732c 0a20 2020 2069  roperties,.    i
-00011760: 6e70 7574 5f74 7970 6573 3d5b 456c 6563  nput_types=[Elec
-00011770: 7469 6f6e 5479 7065 732e 5052 4f46 494c  tionTypes.PROFIL
-00011780: 452c 2045 6c65 6374 696f 6e54 7970 6573  E, ElectionTypes
-00011790: 2e50 524f 4649 4c45 5f57 4954 485f 5449  .PROFILE_WITH_TI
-000117a0: 4553 2c20 456c 6563 7469 6f6e 5479 7065  ES, ElectionType
-000117b0: 732e 4d41 5247 494e 5f47 5241 5048 5d29  s.MARGIN_GRAPH])
-000117c0: 0a64 6566 2065 7373 656e 7469 616c 2865  .def essential(e
-000117d0: 6461 7461 2c20 6375 7272 5f63 616e 6473  data, curr_cands
-000117e0: 203d 204e 6f6e 652c 2074 6872 6573 686f   = None, thresho
-000117f0: 6c64 203d 2030 2e30 3030 3030 3031 293a  ld = 0.0000001):
-00011800: 200a 2020 2020 2222 2254 6865 2045 7373   .    """The Ess
-00011810: 656e 7469 616c 2053 6574 2069 7320 7468  ential Set is th
-00011820: 6520 7375 7070 6f72 7420 6f66 2074 6865  e support of the
-00011830: 2028 6368 6f73 656e 2920 4332 206d 6178   (chosen) C2 max
-00011840: 696d 616c 206c 6f74 7465 7279 2e0a 0a20  imal lottery... 
-00011850: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
-00011860: 2065 6461 7461 2028 5072 6f66 696c 652c   edata (Profile,
-00011870: 2050 726f 6669 6c65 5769 7468 5469 6573   ProfileWithTies
-00011880: 2c20 4d61 7267 696e 4772 6170 6829 3a20  , MarginGraph): 
-00011890: 416e 7920 656c 6563 7469 6f6e 2064 6174  Any election dat
-000118a0: 6120 7468 6174 2068 6173 2061 2060 6d61  a that has a `ma
-000118b0: 7267 696e 5f6d 6174 7269 7860 2061 7474  rgin_matrix` att
-000118c0: 7269 6275 7465 2e0a 2020 2020 2020 2020  ribute..        
-000118d0: 6375 7272 5f63 616e 6473 2028 4c69 7374  curr_cands (List
-000118e0: 5b69 6e74 5d2c 206f 7074 696f 6e61 6c29  [int], optional)
-000118f0: 3a20 4966 2073 6574 2c20 7468 656e 2066  : If set, then f
-00011900: 696e 6420 7468 6520 7769 6e6e 6572 7320  ind the winners 
-00011910: 666f 7220 7468 6520 7072 6f66 696c 6520  for the profile 
-00011920: 7265 7374 7269 6374 6564 2074 6f20 7468  restricted to th
-00011930: 6520 6361 6e64 6964 6174 6573 2069 6e20  e candidates in 
-00011940: 6060 6375 7272 5f63 616e 6473 6060 0a0a  ``curr_cands``..
-00011950: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
-00011960: 2020 2020 2041 2073 6f72 7465 6420 6c69       A sorted li
-00011970: 7374 206f 6620 6361 6e64 6964 6174 6573  st of candidates
-00011980: 2e0a 0a20 2020 2022 2222 0a20 2020 206d  ...    """.    m
-00011990: 6c20 3d20 6d61 7869 6d61 6c5f 6c6f 7474  l = maximal_lott
-000119a0: 6572 7928 6564 6174 612c 2063 7572 725f  ery(edata, curr_
-000119b0: 6361 6e64 733d 6375 7272 5f63 616e 6473  cands=curr_cands
-000119c0: 290a 0a20 2020 2072 6574 7572 6e20 736f  )..    return so
-000119d0: 7274 6564 285b 6320 666f 7220 6320 696e  rted([c for c in
-000119e0: 206d 6c2e 6b65 7973 2829 2069 6620 6d6c   ml.keys() if ml
-000119f0: 5b63 5d20 3e20 7468 7265 7368 6f6c 645d  [c] > threshold]
-00011a00: 290a 0a77 6569 6768 7465 645f 636f 7665  )..weighted_cove
-00011a10: 7269 6e67 5f70 726f 7065 7274 6965 7320  ring_properties 
-00011a20: 3d20 566f 7469 6e67 4d65 7468 6f64 5072  = VotingMethodPr
-00011a30: 6f70 6572 7469 6573 280a 2020 2020 636f  operties(.    co
-00011a40: 6e64 6f72 6365 745f 7769 6e6e 6572 3d54  ndorcet_winner=T
-00011a50: 7275 652c 200a 2020 2020 636f 6e64 6f72  rue, .    condor
-00011a60: 6365 745f 6c6f 7365 723d 5472 7565 2c0a  cet_loser=True,.
-00011a70: 2020 2020 7061 7265 746f 5f64 6f6d 696e      pareto_domin
-00011a80: 616e 6365 3d54 7275 652c 0a20 2020 2070  ance=True,.    p
-00011a90: 6f73 6974 6976 655f 696e 766f 6c76 656d  ositive_involvem
-00011aa0: 656e 743d 5472 7565 2c20 0a20 2020 2029  ent=True, .    )
-00011ab0: 0a40 766d 286e 616d 653d 2257 6569 6768  .@vm(name="Weigh
-00011ac0: 7465 6420 436f 7665 7269 6e67 222c 0a20  ted Covering",. 
-00011ad0: 2020 2070 726f 7065 7274 6965 733d 7765     properties=we
-00011ae0: 6967 6874 6564 5f63 6f76 6572 696e 675f  ighted_covering_
-00011af0: 7072 6f70 6572 7469 6573 2c0a 2020 2020  properties,.    
-00011b00: 696e 7075 745f 7479 7065 733d 5b45 6c65  input_types=[Ele
-00011b10: 6374 696f 6e54 7970 6573 2e50 524f 4649  ctionTypes.PROFI
-00011b20: 4c45 2c20 456c 6563 7469 6f6e 5479 7065  LE, ElectionType
-00011b30: 732e 5052 4f46 494c 455f 5749 5448 5f54  s.PROFILE_WITH_T
-00011b40: 4945 532c 2045 6c65 6374 696f 6e54 7970  IES, ElectionTyp
-00011b50: 6573 2e4d 4152 4749 4e5f 4752 4150 485d  es.MARGIN_GRAPH]
-00011b60: 290a 6465 6620 7765 6967 6874 6564 5f63  ).def weighted_c
-00011b70: 6f76 6572 696e 6728 6564 6174 612c 2063  overing(edata, c
-00011b80: 7572 725f 6361 6e64 733d 4e6f 6e65 293a  urr_cands=None):
-00011b90: 200a 2020 2020 2222 2241 6363 6f72 6469   .    """Accordi
-00011ba0: 6e67 2074 6f20 5765 6967 6874 6564 2043  ng to Weighted C
-00011bb0: 6f76 6572 696e 672c 2078 2064 6566 6561  overing, x defea
-00011bc0: 7473 2079 2069 6620 7468 6520 6d61 7267  ts y if the marg
-00011bd0: 696e 206f 6620 7820 6f76 6572 2079 2069  in of x over y i
-00011be0: 7320 706f 7369 7469 7665 2061 6e64 2066  s positive and f
-00011bf0: 6f72 2065 7665 7279 206f 7468 6572 207a  or every other z
-00011c00: 2c20 7468 6520 6d61 7267 696e 206f 6620  , the margin of 
-00011c10: 7820 6f76 6572 207a 2069 7320 6772 6561  x over z is grea
-00011c20: 7465 7220 7468 616e 206f 7220 6571 7561  ter than or equa
-00011c30: 6c20 746f 2074 6865 206d 6172 6769 6e20  l to the margin 
-00011c40: 6f66 2079 206f 7665 7220 7a2e 200a 0a20  of y over z. .. 
-00011c50: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
-00011c60: 2065 6461 7461 2028 5072 6f66 696c 652c   edata (Profile,
-00011c70: 2050 726f 6669 6c65 5769 7468 5469 6573   ProfileWithTies
-00011c80: 2c20 4d61 7267 696e 4772 6170 6829 3a20  , MarginGraph): 
-00011c90: 416e 7920 656c 6563 7469 6f6e 2064 6174  Any election dat
-00011ca0: 6120 7468 6174 2068 6173 2061 2060 6d61  a that has a `ma
-00011cb0: 7267 696e 6020 6d65 7468 6f64 2e0a 2020  rgin` method..  
-00011cc0: 2020 2020 2020 6375 7272 5f63 616e 6473        curr_cands
-00011cd0: 2028 4c69 7374 5b69 6e74 5d2c 206f 7074   (List[int], opt
-00011ce0: 696f 6e61 6c29 3a20 4966 2073 6574 2c20  ional): If set, 
-00011cf0: 7468 656e 2066 696e 6420 7468 6520 7769  then find the wi
-00011d00: 6e6e 6572 7320 666f 7220 7468 6520 7072  nners for the pr
-00011d10: 6f66 696c 6520 7265 7374 7269 6374 6564  ofile restricted
-00011d20: 2074 6f20 7468 6520 6361 6e64 6964 6174   to the candidat
-00011d30: 6573 2069 6e20 6060 6375 7272 5f63 616e  es in ``curr_can
-00011d40: 6473 6060 0a0a 2020 2020 5265 7475 726e  ds``..    Return
-00011d50: 733a 0a20 2020 2020 2020 2041 2073 6f72  s:.        A sor
-00011d60: 7465 6420 6c69 7374 206f 6620 6361 6e64  ted list of cand
-00011d70: 6964 6174 6573 2e0a 0a20 2020 202e 2e20  idates...    .. 
-00011d80: 6e6f 7465 3a3a 0a20 2020 2020 2020 2053  note::.        S
-00011d90: 6565 2c20 652e 672e 2c20 4268 6173 6b61  ee, e.g., Bhaska
-00011da0: 7220 4475 7474 6120 616e 6420 4a65 616e  r Dutta and Jean
-00011db0: 2d46 7261 6e63 6f69 7320 4c61 736c 6965  -Francois Laslie
-00011dc0: 722c 2022 436f 6d70 6172 6973 6f6e 2066  r, "Comparison f
-00011dd0: 756e 6374 696f 6e73 2061 6e64 2063 686f  unctions and cho
-00011de0: 6963 6520 636f 7272 6573 706f 6e64 656e  ice corresponden
-00011df0: 6365 732c 2220 536f 6369 616c 2043 686f  ces," Social Cho
-00011e00: 6963 6520 616e 6420 5765 6c66 6172 652c  ice and Welfare,
-00011e10: 2031 363a 3531 33e2 8093 3533 322c 2031   16:513...532, 1
-00011e20: 3939 392c 2064 6f69 3a31 302e 3130 3037  999, doi:10.1007
-00011e30: 2f73 3030 3335 3530 3035 3031 3538 2c20  /s003550050158, 
-00011e40: 616e 6420 5261 75cc 816c 2050 65cc 8172  and Rau..l Pe..r
-00011e50: 657a 2d46 6572 6e61 cc81 6e64 657a 2061  ez-Ferna..ndez a
-00011e60: 6e64 2042 6572 6e61 7264 2044 6520 4261  nd Bernard De Ba
-00011e70: 6574 732c 2022 5468 6520 7375 7065 7263  ets, "The superc
-00011e80: 6f76 6572 696e 6720 7265 6c61 7469 6f6e  overing relation
-00011e90: 2c20 7468 6520 7061 6972 7769 7365 2077  , the pairwise w
-00011ea0: 696e 6e65 722c 2061 6e64 206d 6f72 6520  inner, and more 
-00011eb0: 6d69 7373 696e 6720 6c69 6e6b 7320 6265  missing links be
-00011ec0: 7477 6565 6e20 426f 7264 6120 616e 6420  tween Borda and 
-00011ed0: 436f 6e64 6f72 6365 742c 2220 536f 6369  Condorcet," Soci
-00011ee0: 616c 2043 686f 6963 6520 616e 6420 5765  al Choice and We
-00011ef0: 6c66 6172 652c 2035 303a 3332 39e2 8093  lfare, 50:329...
-00011f00: 3335 322c 2032 3031 382c 2064 6f69 3a31  352, 2018, doi:1
-00011f10: 302e 3130 3037 2f73 3030 3335 352d 3031  0.1007/s00355-01
-00011f20: 372d 3130 3836 2d30 2e0a 2020 2020 2222  7-1086-0..    ""
-00011f30: 220a 0a20 2020 2063 616e 6469 6461 7465  "..    candidate
-00011f40: 7320 3d20 6564 6174 612e 6361 6e64 6964  s = edata.candid
-00011f50: 6174 6573 2069 6620 6375 7272 5f63 616e  ates if curr_can
-00011f60: 6473 2069 7320 4e6f 6e65 2065 6c73 6520  ds is None else 
-00011f70: 6375 7272 5f63 616e 6473 0a0a 2020 2020  curr_cands..    
-00011f80: 7563 5f73 6574 203d 206c 6973 7428 290a  uc_set = list().
-00011f90: 0a20 2020 2066 6f72 2079 2069 6e20 6361  .    for y in ca
-00011fa0: 6e64 6964 6174 6573 3a0a 2020 2020 2020  ndidates:.      
-00011fb0: 2020 6973 5f69 6e5f 7563 7320 3d20 5472    is_in_ucs = Tr
-00011fc0: 7565 0a20 2020 2020 2020 2066 6f72 2078  ue.        for x
-00011fd0: 2069 6e20 6564 6174 612e 646f 6d69 6e61   in edata.domina
-00011fe0: 746f 7273 2879 2c20 6375 7272 5f63 616e  tors(y, curr_can
-00011ff0: 6473 203d 2063 7572 725f 6361 6e64 7329  ds = curr_cands)
-00012000: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
-00012010: 6368 6563 6b20 6966 2079 2063 6f76 6572  check if y cover
-00012020: 7320 782c 2069 2e65 2e2c 2066 6f72 2065  s x, i.e., for e
-00012030: 7665 7279 207a 2c20 6d61 7267 696e 2878  very z, margin(x
-00012040: 2c20 7a29 203e 3d20 6d61 7267 696e 2879  , z) >= margin(y
-00012050: 2c20 7a29 0a20 2020 2020 2020 2020 2020  , z).           
-00012060: 2063 6f76 6572 7320 3d20 5472 7565 0a20   covers = True. 
-00012070: 2020 2020 2020 2020 2020 2066 6f72 207a             for z
-00012080: 2069 6e20 6361 6e64 6964 6174 6573 3a0a   in candidates:.
-00012090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000120a0: 6966 2065 6461 7461 2e6d 6172 6769 6e28  if edata.margin(
-000120b0: 782c 207a 2920 3c20 6564 6174 612e 6d61  x, z) < edata.ma
-000120c0: 7267 696e 2879 2c20 7a29 3a0a 2020 2020  rgin(y, z):.    
-000120d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000120e0: 636f 7665 7273 203d 2046 616c 7365 0a20  covers = False. 
-000120f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012100: 2020 2062 7265 616b 0a20 2020 2020 2020     break.       
-00012110: 2020 200a 2020 2020 2020 2020 2020 2020     .            
-00012120: 6966 2063 6f76 6572 733a 0a20 2020 2020  if covers:.     
-00012130: 2020 2020 2020 2020 2020 2069 735f 696e             is_in
-00012140: 5f75 6373 203d 2046 616c 7365 0a20 2020  _ucs = False.   
-00012150: 2020 2020 2020 2020 2020 2020 2062 7265               bre
-00012160: 616b 0a20 2020 2020 2020 2020 2020 2020  ak.             
-00012170: 2020 200a 2020 2020 2020 2020 6966 2069     .        if i
-00012180: 735f 696e 5f75 6373 3a0a 2020 2020 2020  s_in_ucs:.      
-00012190: 2020 2020 2020 7563 5f73 6574 2e61 7070        uc_set.app
-000121a0: 656e 6428 7929 0a0a 2020 2020 7265 7475  end(y)..    retu
-000121b0: 726e 2073 6f72 7465 6428 7563 5f73 6574  rn sorted(uc_set
-000121c0: 290a 0a6c 6f73 735f 7472 696d 6d65 725f  )..loss_trimmer_
-000121d0: 7072 6f70 6572 7469 6573 203d 2056 6f74  properties = Vot
-000121e0: 696e 674d 6574 686f 6450 726f 7065 7274  ingMethodPropert
-000121f0: 6965 7328 0a20 2020 2063 6f6e 646f 7263  ies(.    condorc
-00012200: 6574 5f77 696e 6e65 723d 5472 7565 2c20  et_winner=True, 
-00012210: 0a20 2020 2063 6f6e 646f 7263 6574 5f6c  .    condorcet_l
-00012220: 6f73 6572 3d54 7275 652c 0a20 2020 2070  oser=True,.    p
-00012230: 6172 6574 6f5f 646f 6d69 6e61 6e63 653d  areto_dominance=
-00012240: 5472 7565 2c0a 2020 2020 706f 7369 7469  True,.    positi
-00012250: 7665 5f69 6e76 6f6c 7665 6d65 6e74 3d46  ve_involvement=F
-00012260: 616c 7365 2c20 0a20 2020 2029 0a40 766d  alse, .    ).@vm
-00012270: 286e 616d 6520 3d20 224c 6f73 732d 5472  (name = "Loss-Tr
-00012280: 696d 6d65 7220 566f 7469 6e67 222c 0a20  immer Voting",. 
-00012290: 2020 2070 726f 7065 7274 6965 7320 3d20     properties = 
-000122a0: 6c6f 7373 5f74 7269 6d6d 6572 5f70 726f  loss_trimmer_pro
-000122b0: 7065 7274 6965 732c 0a20 2020 2069 6e70  perties,.    inp
-000122c0: 7574 5f74 7970 6573 203d 205b 456c 6563  ut_types = [Elec
-000122d0: 7469 6f6e 5479 7065 732e 5052 4f46 494c  tionTypes.PROFIL
-000122e0: 452c 2045 6c65 6374 696f 6e54 7970 6573  E, ElectionTypes
-000122f0: 2e50 524f 4649 4c45 5f57 4954 485f 5449  .PROFILE_WITH_TI
-00012300: 4553 2c20 456c 6563 7469 6f6e 5479 7065  ES, ElectionType
-00012310: 732e 4d41 5247 494e 5f47 5241 5048 5d29  s.MARGIN_GRAPH])
-00012320: 0a64 6566 206c 6f73 735f 7472 696d 6d65  .def loss_trimme
-00012330: 7228 6564 6174 612c 2063 7572 725f 6361  r(edata, curr_ca
-00012340: 6e64 7320 3d20 4e6f 6e65 293a 0a20 2020  nds = None):.   
-00012350: 2022 2222 4974 6572 6174 6976 656c 7920   """Iteratively 
-00012360: 656c 696d 696e 6174 6520 7468 6520 6361  eliminate the ca
-00012370: 6e64 6964 6174 6520 7769 7468 2074 6865  ndidate with the
-00012380: 206c 6172 6765 7374 2073 756d 206f 6620   largest sum of 
-00012390: 6d61 7267 696e 7320 6f66 206c 6f73 7320  margins of loss 
-000123a0: 756e 7469 6c20 6120 436f 6e64 6f72 6365  until a Condorce
-000123b0: 7420 7769 6e6e 6572 2069 7320 666f 756e  t winner is foun
-000123c0: 642e 2049 6e20 7468 6973 2076 6572 7369  d. In this versi
-000123d0: 6f6e 206f 6620 7468 6520 6d65 7468 6f64  on of the method
-000123e0: 2c20 7061 7261 6c6c 656c 2d75 6e69 7665  , parallel-unive
-000123f0: 7273 6520 7469 6562 7265 616b 696e 6720  rse tiebreaking 
-00012400: 6973 2075 7365 6420 6966 2074 6865 7265  is used if there
-00012410: 2061 7265 206d 756c 7469 706c 6520 6361   are multiple ca
-00012420: 6e64 6964 6174 6573 2077 6974 6820 7468  ndidates with th
-00012430: 6520 6c61 7267 6573 7420 7375 6d20 6f66  e largest sum of
-00012440: 206d 6172 6769 6e73 206f 6620 6c6f 7373   margins of loss
-00012450: 2e0a 0a20 2020 2041 7267 733a 0a20 2020  ...    Args:.   
-00012460: 2020 2020 2065 6461 7461 2028 5072 6f66       edata (Prof
-00012470: 696c 652c 2050 726f 6669 6c65 5769 7468  ile, ProfileWith
-00012480: 5469 6573 2c20 4d61 7267 696e 4772 6170  Ties, MarginGrap
-00012490: 6829 3a20 416e 7920 656c 6563 7469 6f6e  h): Any election
-000124a0: 2064 6174 6120 7468 6174 2068 6173 2061   data that has a
-000124b0: 206d 6172 6769 6e20 6d65 7468 6f64 2e0a   margin method..
-000124c0: 2020 2020 2020 2020 6375 7272 5f63 616e          curr_can
-000124d0: 6473 2028 4c69 7374 5b69 6e74 5d2c 206f  ds (List[int], o
-000124e0: 7074 696f 6e61 6c29 3a20 4966 2073 6574  ptional): If set
-000124f0: 2c20 7468 656e 2066 696e 6420 7468 6520  , then find the 
-00012500: 7769 6e6e 6572 7320 666f 7220 7468 6520  winners for the 
-00012510: 7072 6f66 696c 6520 7265 7374 7269 6374  profile restrict
-00012520: 6564 2074 6f20 7468 6520 6361 6e64 6964  ed to the candid
-00012530: 6174 6573 2069 6e20 6060 6375 7272 5f63  ates in ``curr_c
-00012540: 616e 6473 6060 0a0a 2020 2020 5265 7475  ands``..    Retu
-00012550: 726e 733a 200a 2020 2020 2020 2020 4120  rns: .        A 
-00012560: 736f 7274 6564 206c 6973 7420 6f66 2063  sorted list of c
-00012570: 616e 6469 6461 7465 730a 0a20 2020 202e  andidates..    .
-00012580: 2e20 6e6f 7465 3a3a 0a20 2020 2020 2020  . note::.       
-00012590: 204d 6574 686f 6420 7072 6f70 6f73 6564   Method proposed
-000125a0: 2062 7920 5269 6368 6172 6420 422e 2044   by Richard B. D
-000125b0: 6172 6c69 6e67 746f 6e20 696e 2022 5468  arlington in "Th
-000125c0: 6520 4361 7365 2066 6f72 2074 6865 204c  e Case for the L
-000125d0: 6f73 732d 5472 696d 6d65 7220 566f 7469  oss-Trimmer Voti
-000125e0: 6e67 2053 7973 7465 6d2e 220a 0a20 2020  ng System."..   
-000125f0: 2022 2222 0a0a 2020 2020 6375 7272 5f63   """..    curr_c
-00012600: 616e 6473 203d 2065 6461 7461 2e63 616e  ands = edata.can
-00012610: 6469 6461 7465 7320 6966 2063 7572 725f  didates if curr_
-00012620: 6361 6e64 7320 6973 204e 6f6e 6520 656c  cands is None el
-00012630: 7365 2063 7572 725f 6361 6e64 730a 0a20  se curr_cands.. 
-00012640: 2020 2077 6561 6b5f 6377 203d 2065 6461     weak_cw = eda
-00012650: 7461 2e77 6561 6b5f 636f 6e64 6f72 6365  ta.weak_condorce
-00012660: 745f 7769 6e6e 6572 2863 7572 725f 6361  t_winner(curr_ca
-00012670: 6e64 7320 3d20 6375 7272 5f63 616e 6473  nds = curr_cands
-00012680: 290a 2020 2020 2320 4966 2074 6865 7265  ).    # If there
-00012690: 2061 7265 2077 6561 6b20 436f 6e64 6f72   are weak Condor
-000126a0: 6365 7420 7769 6e6e 6572 732c 2072 6574  cet winners, ret
-000126b0: 7572 6e20 7468 6f73 6520 6361 6e64 6964  urn those candid
-000126c0: 6174 6573 0a20 2020 2069 6620 6564 6174  ates.    if edat
-000126d0: 612e 7765 616b 5f63 6f6e 646f 7263 6574  a.weak_condorcet
-000126e0: 5f77 696e 6e65 7228 6375 7272 5f63 616e  _winner(curr_can
-000126f0: 6473 203d 2063 7572 725f 6361 6e64 7329  ds = curr_cands)
-00012700: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00012710: 2020 2020 2020 7265 7475 726e 2073 6f72        return sor
-00012720: 7465 6428 7765 616b 5f63 7729 0a20 2020  ted(weak_cw).   
-00012730: 200a 2020 2020 2320 4f74 6865 7277 6973   .    # Otherwis
-00012740: 652c 2063 616c 6375 6c61 7465 2074 6865  e, calculate the
-00012750: 2073 756d 206f 6620 6d61 7267 696e 7320   sum of margins 
-00012760: 6f66 206c 6f73 7320 666f 7220 6561 6368  of loss for each
-00012770: 2063 616e 6469 6461 7465 0a20 2020 2073   candidate.    s
-00012780: 756d 5f6f 665f 6d61 7267 696e 735f 6f66  um_of_margins_of
-00012790: 5f6c 6f73 7320 3d20 7b63 616e 643a 2073  _loss = {cand: s
-000127a0: 756d 285b 6564 6174 612e 6d61 7267 696e  um([edata.margin
-000127b0: 286f 7468 6572 5f63 616e 642c 2063 616e  (other_cand, can
-000127c0: 6429 2066 6f72 206f 7468 6572 5f63 616e  d) for other_can
-000127d0: 6420 696e 2063 7572 725f 6361 6e64 7320  d in curr_cands 
-000127e0: 6966 2065 6461 7461 2e6d 6172 6769 6e28  if edata.margin(
-000127f0: 6f74 6865 725f 6361 6e64 2c20 6361 6e64  other_cand, cand
-00012800: 2920 3e20 305d 2920 666f 7220 6361 6e64  ) > 0]) for cand
-00012810: 2069 6e20 6375 7272 5f63 616e 6473 7d0a   in curr_cands}.
-00012820: 0a20 2020 2023 2046 696e 6420 7468 6520  .    # Find the 
-00012830: 6361 6e64 6964 6174 6573 2077 6974 6820  candidates with 
-00012840: 7468 6520 6c61 7267 6573 7420 7375 6d20  the largest sum 
-00012850: 6f66 206d 6172 6769 6e73 206f 6620 6c6f  of margins of lo
-00012860: 7373 0a20 2020 206d 6178 5f73 756d 5f6f  ss.    max_sum_o
-00012870: 665f 6d61 7267 696e 735f 6f66 5f6c 6f73  f_margins_of_los
-00012880: 7320 3d20 6d61 7828 7375 6d5f 6f66 5f6d  s = max(sum_of_m
-00012890: 6172 6769 6e73 5f6f 665f 6c6f 7373 2e76  argins_of_loss.v
-000128a0: 616c 7565 7328 2929 0a20 2020 2062 6967  alues()).    big
-000128b0: 6765 7374 5f6c 6f73 6572 7320 3d20 5b63  gest_losers = [c
-000128c0: 616e 6420 666f 7220 6361 6e64 2069 6e20  and for cand in 
-000128d0: 6375 7272 5f63 616e 6473 2069 6620 7375  curr_cands if su
-000128e0: 6d5f 6f66 5f6d 6172 6769 6e73 5f6f 665f  m_of_margins_of_
-000128f0: 6c6f 7373 5b63 616e 645d 203d 3d20 6d61  loss[cand] == ma
-00012900: 785f 7375 6d5f 6f66 5f6d 6172 6769 6e73  x_sum_of_margins
-00012910: 5f6f 665f 6c6f 7373 5d0a 0a20 2020 2077  _of_loss]..    w
-00012920: 696e 6e65 7273 203d 205b 5d0a 0a20 2020  inners = []..   
-00012930: 2023 2046 6f72 2065 6163 6820 6269 6767   # For each bigg
-00012940: 6573 7420 6c6f 7365 722c 2063 616c 6375  est loser, calcu
-00012950: 6c61 7465 2074 6865 2077 696e 6e65 7273  late the winners
-00012960: 2061 6674 6572 2072 656d 6f76 696e 6720   after removing 
-00012970: 7468 6174 2063 616e 6469 6461 7465 2e20  that candidate. 
-00012980: 5468 6520 756e 696f 6e20 6f66 2074 6865  The union of the
-00012990: 7365 2073 6574 7320 6973 2074 6865 2073  se sets is the s
-000129a0: 6574 206f 6620 7769 6e6e 6572 732e 0a20  et of winners.. 
-000129b0: 2020 2066 6f72 2062 6c20 696e 2062 6967     for bl in big
-000129c0: 6765 7374 5f6c 6f73 6572 733a 0a20 2020  gest_losers:.   
-000129d0: 2020 2020 2077 696e 6e65 7273 5f77 6974       winners_wit
-000129e0: 686f 7574 5f62 6c20 3d20 6c6f 7373 5f74  hout_bl = loss_t
-000129f0: 7269 6d6d 6572 2865 6461 7461 2c20 6375  rimmer(edata, cu
-00012a00: 7272 5f63 616e 6473 203d 205b 6361 6e64  rr_cands = [cand
-00012a10: 2066 6f72 2063 616e 6420 696e 2063 7572   for cand in cur
-00012a20: 725f 6361 6e64 7320 6966 2063 616e 6420  r_cands if cand 
-00012a30: 213d 2062 6c5d 290a 2020 2020 2020 2020  != bl]).        
-00012a40: 7769 6e6e 6572 7320 2b3d 2077 696e 6e65  winners += winne
-00012a50: 7273 5f77 6974 686f 7574 5f62 6c0a 0a20  rs_without_bl.. 
-00012a60: 2020 2072 6574 7572 6e20 736f 7274 6564     return sorted
-00012a70: 286c 6973 7428 7365 7428 7769 6e6e 6572  (list(set(winner
-00012a80: 7329 2929 0a0a 0a64 6566 2064 6973 7461  s)))...def dista
-00012a90: 6e63 655f 746f 5f6d 6172 6769 6e5f 6772  nce_to_margin_gr
-00012aa0: 6170 6828 6564 6174 612c 2072 656c 2c20  aph(edata, rel, 
-00012ab0: 6578 7020 3d20 312c 2063 7572 725f 6361  exp = 1, curr_ca
-00012ac0: 6e64 7320 3d20 4e6f 6e65 293a 200a 2020  nds = None): .  
-00012ad0: 2020 2222 220a 2020 2020 4361 6c63 756c    """.    Calcul
-00012ae0: 6174 6520 7468 6520 6469 7374 616e 6365  ate the distance
-00012af0: 206f 6620 6060 7265 6c60 6020 2861 2072   of ``rel`` (a r
-00012b00: 656c 6174 696f 6e29 2074 6f20 7468 6520  elation) to the 
-00012b10: 6d61 6a6f 7269 7479 2067 7261 7068 206f  majority graph o
-00012b20: 6620 6060 6564 6174 6160 602e 200a 2020  f ``edata``. .  
-00012b30: 2020 2222 220a 2020 2020 6361 6e64 6964    """.    candid
-00012b40: 6174 6573 203d 2065 6461 7461 2e63 616e  ates = edata.can
-00012b50: 6469 6461 7465 7320 6966 2063 7572 725f  didates if curr_
-00012b60: 6361 6e64 7320 6973 204e 6f6e 6520 656c  cands is None el
-00012b70: 7365 2063 7572 725f 6361 6e64 730a 2020  se curr_cands.  
-00012b80: 2020 0a20 2020 2069 6620 7479 7065 2865    .    if type(e
-00012b90: 6461 7461 2920 3d3d 204d 616a 6f72 6974  data) == Majorit
-00012ba0: 7947 7261 7068 2061 6e64 2065 7870 203d  yGraph and exp =
-00012bb0: 3d20 303a 0a20 2020 2020 2020 2023 2069  = 0:.        # i
-00012bc0: 6620 6564 6174 6120 6973 2061 204d 616a  f edata is a Maj
-00012bd0: 6f72 6974 7947 7261 7068 2c20 7765 206e  orityGraph, we n
-00012be0: 6565 6420 746f 2061 6464 206d 6172 6769  eed to add margi
-00012bf0: 6e73 2066 6f72 2074 6865 2066 6f6c 6c6f  ns for the follo
-00012c00: 7769 6e67 2063 6f64 6520 746f 2077 6f72  wing code to wor
-00012c10: 6b2e 2020 5468 6520 6d61 7267 696e 7320  k.  The margins 
-00012c20: 646f 206e 6f74 206d 6174 7465 7220 7768  do not matter wh
-00012c30: 656e 2065 7870 3d3d 302e 2020 200a 2020  en exp==0.   .  
-00012c40: 2020 2020 2020 6564 6174 6120 3d20 4d61        edata = Ma
-00012c50: 7267 696e 4772 6170 6828 6361 6e64 6964  rginGraph(candid
-00012c60: 6174 6573 2c20 5b28 6331 2c20 6332 2c20  ates, [(c1, c2, 
-00012c70: 3129 2066 6f72 2063 312c 2063 3220 696e  1) for c1, c2 in
-00012c80: 2065 6461 7461 2e65 6467 6573 2069 6620   edata.edges if 
-00012c90: 2863 3120 696e 2063 616e 6469 6461 7465  (c1 in candidate
-00012ca0: 7320 616e 6420 6332 2069 6e20 6361 6e64  s and c2 in cand
-00012cb0: 6964 6174 6573 295d 290a 2020 2020 7065  idates)]).    pe
-00012cc0: 6e61 6c74 7920 3d20 300a 2020 2020 666f  nalty = 0.    fo
-00012cd0: 7220 612c 6220 696e 2063 6f6d 6269 6e61  r a,b in combina
-00012ce0: 7469 6f6e 7328 6361 6e64 6964 6174 6573  tions(candidates
-00012cf0: 2c20 3229 3a20 0a20 2020 2020 2020 2069  , 2): .        i
-00012d00: 6620 6564 6174 612e 6d61 6a6f 7269 7479  f edata.majority
-00012d10: 5f70 7265 6665 7273 2861 2c20 6229 2061  _prefers(a, b) a
-00012d20: 6e64 2028 622c 6129 2069 6e20 7265 6c3a  nd (b,a) in rel:
-00012d30: 200a 2020 2020 2020 2020 2020 2020 7065   .            pe
-00012d40: 6e61 6c74 7920 2b3d 2028 6564 6174 612e  nalty += (edata.
-00012d50: 6d61 7267 696e 2861 2c20 6229 202a 2a20  margin(a, b) ** 
-00012d60: 6578 7029 0a20 2020 2020 2020 2065 6c69  exp).        eli
-00012d70: 6620 6564 6174 612e 6d61 6a6f 7269 7479  f edata.majority
-00012d80: 5f70 7265 6665 7273 2862 2c20 6129 2061  _prefers(b, a) a
-00012d90: 6e64 2028 612c 6229 2069 6e20 7265 6c3a  nd (a,b) in rel:
-00012da0: 200a 2020 2020 2020 2020 2020 2020 7065   .            pe
-00012db0: 6e61 6c74 7920 2b3d 2028 6564 6174 612e  nalty += (edata.
-00012dc0: 6d61 7267 696e 2862 2c20 6129 202a 2a20  margin(b, a) ** 
-00012dd0: 6578 7029 0a20 2020 2020 2020 2065 6c69  exp).        eli
-00012de0: 6620 6564 6174 612e 6d61 6a6f 7269 7479  f edata.majority
-00012df0: 5f70 7265 6665 7273 2861 2c20 6229 2061  _prefers(a, b) a
-00012e00: 6e64 2028 612c 6229 206e 6f74 2069 6e20  nd (a,b) not in 
-00012e10: 7265 6c20 616e 6420 2862 2c61 2920 6e6f  rel and (b,a) no
-00012e20: 7420 696e 2072 656c 3a20 0a20 2020 2020  t in rel: .     
-00012e30: 2020 2020 2020 2070 656e 616c 7479 202b         penalty +
-00012e40: 3d20 2865 6461 7461 2e6d 6172 6769 6e28  = (edata.margin(
-00012e50: 612c 2062 2920 2a2a 2065 7870 2920 2f20  a, b) ** exp) / 
-00012e60: 3220 0a20 2020 2020 2020 2065 6c69 6620  2 .        elif 
-00012e70: 6564 6174 612e 6d61 6a6f 7269 7479 5f70  edata.majority_p
-00012e80: 7265 6665 7273 2862 2c20 6129 2061 6e64  refers(b, a) and
-00012e90: 2028 612c 6229 206e 6f74 2069 6e20 7265   (a,b) not in re
-00012ea0: 6c20 616e 6420 2862 2c61 2920 6e6f 7420  l and (b,a) not 
-00012eb0: 696e 2072 656c 3a20 0a20 2020 2020 2020  in rel: .       
-00012ec0: 2020 2020 2070 656e 616c 7479 202b 3d20       penalty += 
-00012ed0: 2865 6461 7461 2e6d 6172 6769 6e28 622c  (edata.margin(b,
-00012ee0: 2061 2920 2a2a 2065 7870 2920 202f 2032   a) ** exp)  / 2
-00012ef0: 0a20 2020 2072 6574 7572 6e20 7065 6e61  .    return pena
-00012f00: 6c74 790a                                lty.
+000106b0: 2020 206d 656d 5f73 765f 7769 6e6e 6572     mem_sv_winner
+000106c0: 7320 3d20 6d65 6d5f 7376 5f77 696e 6e65  s = mem_sv_winne
+000106d0: 7273 290a 2020 2020 2020 2020 2020 2020  rs).            
+000106e0: 2020 2020 6d65 6d5f 7376 5f77 696e 6e65      mem_sv_winne
+000106f0: 7273 5b63 616e 6473 5f6d 696e 7573 5f62  rs[cands_minus_b
+00010700: 5f6b 6579 5d20 3d20 7773 0a20 2020 2020  _key] = ws.     
+00010710: 2020 2020 2020 2065 6c73 653a 200a 2020         else: .  
+00010720: 2020 2020 2020 2020 2020 2020 2020 7773                ws
+00010730: 203d 206d 656d 5f73 765f 7769 6e6e 6572   = mem_sv_winner
+00010740: 735b 6361 6e64 735f 6d69 6e75 735f 625f  s[cands_minus_b_
+00010750: 6b65 795d 0a20 2020 2020 2020 2020 2020  key].           
+00010760: 2069 6620 6120 696e 2077 733a 0a20 2020   if a in ws:.   
+00010770: 2020 2020 2020 2020 2020 2020 2073 765f               sv_
+00010780: 7769 6e6e 6572 732e 6170 7065 6e64 2861  winners.append(a
+00010790: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000107a0: 2020 6d61 7267 696e 5f77 6974 6e65 7373    margin_witness
+000107b0: 696e 675f 7769 6e20 3d20 730a 2020 2020  ing_win = s.    
+000107c0: 2020 2020 2020 2020 2020 2020 0a20 2020              .   
+000107d0: 2072 6574 7572 6e20 7376 5f77 696e 6e65   return sv_winne
+000107e0: 7273 2c20 6d65 6d5f 7376 5f77 696e 6e65  rs, mem_sv_winne
+000107f0: 7273 0a20 2020 2020 2020 200a 6465 6620  rs.        .def 
+00010800: 5f73 7461 626c 655f 766f 7469 6e67 5f77  _stable_voting_w
+00010810: 6974 685f 636f 6e64 6f72 6365 745f 6368  ith_condorcet_ch
+00010820: 6563 6b28 0a20 2020 2065 6461 7461 2c20  eck(.    edata, 
+00010830: 0a20 2020 2063 7572 725f 6361 6e64 733d  .    curr_cands=
+00010840: 4e6f 6e65 2c20 0a20 2020 2073 7472 656e  None, .    stren
+00010850: 6774 685f 6675 6e63 7469 6f6e 3d4e 6f6e  gth_function=Non
+00010860: 6529 3a20 0a20 2020 2022 2222 0a20 2020  e): .    """.   
+00010870: 2053 7461 626c 6520 566f 7469 6e67 2069   Stable Voting i
+00010880: 7320 436f 6e64 6f72 6365 7420 636f 6e73  s Condorcet cons
+00010890: 6973 7465 6e74 2e20 2020 4974 2069 7320  istent.   It is 
+000108a0: 6661 7374 6572 2074 6f20 736b 6970 2065  faster to skip e
+000108b0: 7865 6375 7469 6e67 2074 6865 2072 6563  xecuting the rec
+000108c0: 7572 7369 7665 2061 6c67 6f72 6974 686d  ursive algorithm
+000108d0: 2077 6865 6e20 7468 6572 6520 6973 2061   when there is a
+000108e0: 2043 6f6e 646f 7263 6574 2077 696e 6e65   Condorcet winne
+000108f0: 722e 2020 0a0a 2020 2020 4172 6773 3a0a  r.  ..    Args:.
+00010900: 2020 2020 2020 2020 6564 6174 6120 2850          edata (P
+00010910: 726f 6669 6c65 2c20 5072 6f66 696c 6557  rofile, ProfileW
+00010920: 6974 6854 6965 732c 204d 6172 6769 6e47  ithTies, MarginG
+00010930: 7261 7068 293a 2041 6e79 2065 6c65 6374  raph): Any elect
+00010940: 696f 6e20 6461 7461 2074 6861 7420 6861  ion data that ha
+00010950: 7320 6120 606d 6172 6769 6e60 206d 6574  s a `margin` met
+00010960: 686f 642e 200a 2020 2020 2020 2020 6375  hod. .        cu
+00010970: 7272 5f63 616e 6473 2028 4c69 7374 5b69  rr_cands (List[i
+00010980: 6e74 5d2c 206f 7074 696f 6e61 6c29 3a20  nt], optional): 
+00010990: 4966 2073 6574 2c20 7468 656e 2066 696e  If set, then fin
+000109a0: 6420 7468 6520 7769 6e6e 6572 7320 666f  d the winners fo
+000109b0: 7220 7468 6520 7072 6f66 696c 6520 7265  r the profile re
+000109c0: 7374 7269 6374 6564 2074 6f20 7468 6520  stricted to the 
+000109d0: 6361 6e64 6964 6174 6573 2069 6e20 6060  candidates in ``
+000109e0: 6375 7272 5f63 616e 6473 6060 0a20 2020  curr_cands``.   
+000109f0: 2020 2020 2073 7472 656e 6774 685f 6675       strength_fu
+00010a00: 6e63 7469 6f6e 2028 6675 6e63 7469 6f6e  nction (function
+00010a10: 2c20 6f70 7469 6f6e 616c 293a 2054 6865  , optional): The
+00010a20: 2073 7472 656e 6774 6820 6675 6e63 7469   strength functi
+00010a30: 6f6e 2074 6f20 6265 2075 7365 6420 746f  on to be used to
+00010a40: 2063 616c 6375 6c61 7465 2074 6865 2073   calculate the s
+00010a50: 7472 656e 6774 6820 6f66 2061 2070 6174  trength of a pat
+00010a60: 682e 2020 2054 6865 2064 6566 6175 6c74  h.   The default
+00010a70: 2069 7320 7468 6520 6d61 7267 696e 206d   is the margin m
+00010a80: 6574 686f 6420 6f66 2060 6065 6461 7461  ethod of ``edata
+00010a90: 6060 2e20 2020 5468 6973 206f 6e6c 7920  ``.   This only 
+00010aa0: 6d61 7474 6572 7320 7768 656e 2074 6865  matters when the
+00010ab0: 2062 616c 6c6f 7473 2061 7265 206e 6f74   ballots are not
+00010ac0: 206c 696e 6561 7220 6f72 6465 7273 2e20   linear orders. 
+00010ad0: 0a0a 2020 2020 5265 7475 726e 733a 200a  ..    Returns: .
+00010ae0: 2020 2020 2020 2020 4120 736f 7274 6564          A sorted
+00010af0: 206c 6973 7420 6f66 2063 616e 6469 6461   list of candida
+00010b00: 7465 732e 200a 0a20 2020 2022 2222 0a20  tes. ..    """. 
+00010b10: 2020 2063 7720 3d20 6564 6174 612e 636f     cw = edata.co
+00010b20: 6e64 6f72 6365 745f 7769 6e6e 6572 2863  ndorcet_winner(c
+00010b30: 7572 725f 6361 6e64 7320 3d20 6375 7272  urr_cands = curr
+00010b40: 5f63 616e 6473 290a 2020 2020 6966 2063  _cands).    if c
+00010b50: 7720 6973 206e 6f74 204e 6f6e 653a 200a  w is not None: .
+00010b60: 2020 2020 2020 2020 7265 7475 726e 205b          return [
+00010b70: 6377 5d0a 2020 2020 656c 7365 3a20 0a20  cw].    else: . 
+00010b80: 2020 2020 2020 2063 7572 725f 6361 6e64         curr_cand
+00010b90: 7320 3d20 6564 6174 612e 6361 6e64 6964  s = edata.candid
+00010ba0: 6174 6573 2069 6620 6375 7272 5f63 616e  ates if curr_can
+00010bb0: 6473 2069 7320 4e6f 6e65 2065 6c73 6520  ds is None else 
+00010bc0: 6375 7272 5f63 616e 6473 0a20 2020 2020  curr_cands.     
+00010bd0: 2020 2073 7472 656e 6774 685f 6675 6e63     strength_func
+00010be0: 7469 6f6e 203d 2065 6461 7461 2e6d 6172  tion = edata.mar
+00010bf0: 6769 6e20 6966 2073 7472 656e 6774 685f  gin if strength_
+00010c00: 6675 6e63 7469 6f6e 2069 7320 4e6f 6e65  function is None
+00010c10: 2065 6c73 6520 7374 7265 6e67 7468 5f66   else strength_f
+00010c20: 756e 6374 696f 6e20 200a 0a20 2020 2020  unction  ..     
+00010c30: 2020 206d 6174 6368 6573 203d 205b 2861     matches = [(a
+00010c40: 2c20 622c 2073 7472 656e 6774 685f 6675  , b, strength_fu
+00010c50: 6e63 7469 6f6e 2861 2c20 6229 2920 666f  nction(a, b)) fo
+00010c60: 7220 6120 696e 2063 7572 725f 6361 6e64  r a in curr_cand
+00010c70: 7320 666f 7220 6220 696e 2063 7572 725f  s for b in curr_
+00010c80: 6361 6e64 7320 6966 2061 2021 3d20 625d  cands if a != b]
+00010c90: 0a20 2020 2020 2020 2073 6f72 7465 645f  .        sorted_
+00010ca0: 6d61 7463 6865 7320 3d20 736f 7274 6564  matches = sorted
+00010cb0: 286d 6174 6368 6573 2c20 7265 7665 7273  (matches, revers
+00010cc0: 653d 5472 7565 2c20 6b65 793d 6c61 6d62  e=True, key=lamb
+00010cd0: 6461 206d 5f77 5f77 6569 6768 743a 206d  da m_w_weight: m
+00010ce0: 5f77 5f77 6569 6768 745b 325d 290a 0a20  _w_weight[2]).. 
+00010cf0: 2020 2020 2020 2072 6574 7572 6e20 736f         return so
+00010d00: 7274 6564 285f 7374 6162 6c65 5f76 6f74  rted(_stable_vot
+00010d10: 696e 6728 6564 6174 612c 200a 2020 2020  ing(edata, .    
+00010d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010d40: 6375 7272 5f63 616e 6473 203d 2063 7572  curr_cands = cur
+00010d50: 725f 6361 6e64 732c 200a 2020 2020 2020  r_cands, .      
+00010d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010d70: 2020 2020 2020 2020 2020 2020 2020 7374                st
+00010d80: 7265 6e67 7468 5f66 756e 6374 696f 6e20  rength_function 
+00010d90: 3d20 7374 7265 6e67 7468 5f66 756e 6374  = strength_funct
+00010da0: 696f 6e2c 0a20 2020 2020 2020 2020 2020  ion,.           
+00010db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010dc0: 2020 2020 2020 2020 2073 6f72 7465 645f           sorted_
+00010dd0: 6d61 7463 6865 7320 3d20 736f 7274 6564  matches = sorted
+00010de0: 5f6d 6174 6368 6573 2c0a 2020 2020 2020  _matches,.      
+00010df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010e00: 2020 2020 2020 2020 2020 2020 2020 6d65                me
+00010e10: 6d5f 7376 5f77 696e 6e65 7273 203d 207b  m_sv_winners = {
+00010e20: 7d29 5b30 5d29 0a0a 6465 6620 5f73 7461  })[0])..def _sta
+00010e30: 626c 655f 766f 7469 6e67 5f62 6173 6963  ble_voting_basic
+00010e40: 280a 2020 2020 2020 2020 6564 6174 612c  (.        edata,
+00010e50: 200a 2020 2020 2020 2020 6375 7272 5f63   .        curr_c
+00010e60: 616e 6473 203d 204e 6f6e 652c 200a 2020  ands = None, .  
+00010e70: 2020 2020 2020 7374 7265 6e67 7468 5f66        strength_f
+00010e80: 756e 6374 696f 6e20 3d20 4e6f 6e65 293a  unction = None):
+00010e90: 200a 2020 2020 2222 2249 6d70 6c65 6d65   .    """Impleme
+00010ea0: 6e74 6174 696f 6e20 6f66 2020 5374 6162  ntation of  Stab
+00010eb0: 6c65 2056 6f74 696e 6720 6672 6f6d 2068  le Voting from h
+00010ec0: 7474 7073 3a2f 2f61 7278 6976 2e6f 7267  ttps://arxiv.org
+00010ed0: 2f61 6273 2f32 3130 382e 3030 3534 322e  /abs/2108.00542.
+00010ee0: 200a 0a20 2020 2041 7267 733a 0a20 2020   ..    Args:.   
+00010ef0: 2020 2020 2065 6461 7461 2028 5072 6f66       edata (Prof
+00010f00: 696c 652c 2050 726f 6669 6c65 5769 7468  ile, ProfileWith
+00010f10: 5469 6573 2c20 4d61 7267 696e 4772 6170  Ties, MarginGrap
+00010f20: 6829 3a20 416e 7920 656c 6563 7469 6f6e  h): Any election
+00010f30: 2064 6174 6120 7468 6174 2068 6173 2061   data that has a
+00010f40: 2060 6d61 7267 696e 6020 6d65 7468 6f64   `margin` method
+00010f50: 2e20 0a20 2020 2020 2020 2063 7572 725f  . .        curr_
+00010f60: 6361 6e64 7320 284c 6973 745b 696e 745d  cands (List[int]
+00010f70: 2c20 6f70 7469 6f6e 616c 293a 2049 6620  , optional): If 
+00010f80: 7365 742c 2074 6865 6e20 6669 6e64 2074  set, then find t
+00010f90: 6865 2077 696e 6e65 7273 2066 6f72 2074  he winners for t
+00010fa0: 6865 2070 726f 6669 6c65 2072 6573 7472  he profile restr
+00010fb0: 6963 7465 6420 746f 2074 6865 2063 616e  icted to the can
+00010fc0: 6469 6461 7465 7320 696e 2060 6063 7572  didates in ``cur
+00010fd0: 725f 6361 6e64 7360 600a 2020 2020 2020  r_cands``.      
+00010fe0: 2020 7374 7265 6e67 7468 5f66 756e 6374    strength_funct
+00010ff0: 696f 6e20 2866 756e 6374 696f 6e2c 206f  ion (function, o
+00011000: 7074 696f 6e61 6c29 3a20 5468 6520 7374  ptional): The st
+00011010: 7265 6e67 7468 2066 756e 6374 696f 6e20  rength function 
+00011020: 746f 2062 6520 7573 6564 2074 6f20 6361  to be used to ca
+00011030: 6c63 756c 6174 6520 7468 6520 7374 7265  lculate the stre
+00011040: 6e67 7468 206f 6620 6120 7061 7468 2e20  ngth of a path. 
+00011050: 2020 5468 6520 6465 6661 756c 7420 6973    The default is
+00011060: 2074 6865 206d 6172 6769 6e20 6d65 7468   the margin meth
+00011070: 6f64 206f 6620 6060 6564 6174 6160 602e  od of ``edata``.
+00011080: 2020 2054 6869 7320 6f6e 6c79 206d 6174     This only mat
+00011090: 7465 7273 2077 6865 6e20 7468 6520 6261  ters when the ba
+000110a0: 6c6c 6f74 7320 6172 6520 6e6f 7420 6c69  llots are not li
+000110b0: 6e65 6172 206f 7264 6572 732e 200a 0a20  near orders. .. 
+000110c0: 2020 2052 6574 7572 6e73 3a20 0a20 2020     Returns: .   
+000110d0: 2020 2020 2041 2073 6f72 7465 6420 6c69       A sorted li
+000110e0: 7374 206f 6620 6361 6e64 6964 6174 6573  st of candidates
+000110f0: 2e20 0a0a 2020 2020 2222 220a 0a20 2020  . ..    """..   
+00011100: 2063 7572 725f 6361 6e64 7320 3d20 6564   curr_cands = ed
+00011110: 6174 612e 6361 6e64 6964 6174 6573 2069  ata.candidates i
+00011120: 6620 6375 7272 5f63 616e 6473 2069 7320  f curr_cands is 
+00011130: 4e6f 6e65 2065 6c73 6520 6375 7272 5f63  None else curr_c
+00011140: 616e 6473 0a20 2020 2073 7472 656e 6774  ands.    strengt
+00011150: 685f 6675 6e63 7469 6f6e 203d 2065 6461  h_function = eda
+00011160: 7461 2e6d 6172 6769 6e20 6966 2073 7472  ta.margin if str
+00011170: 656e 6774 685f 6675 6e63 7469 6f6e 2069  ength_function i
+00011180: 7320 4e6f 6e65 2065 6c73 6520 7374 7265  s None else stre
+00011190: 6e67 7468 5f66 756e 6374 696f 6e20 200a  ngth_function  .
+000111a0: 0a20 2020 206d 6174 6368 6573 203d 205b  .    matches = [
+000111b0: 2861 2c20 622c 2073 7472 656e 6774 685f  (a, b, strength_
+000111c0: 6675 6e63 7469 6f6e 2861 2c20 6229 2920  function(a, b)) 
+000111d0: 666f 7220 6120 696e 2063 7572 725f 6361  for a in curr_ca
+000111e0: 6e64 7320 666f 7220 6220 696e 2063 7572  nds for b in cur
+000111f0: 725f 6361 6e64 7320 6966 2061 2021 3d20  r_cands if a != 
+00011200: 625d 0a20 2020 2073 6f72 7465 645f 6d61  b].    sorted_ma
+00011210: 7463 6865 7320 3d20 736f 7274 6564 286d  tches = sorted(m
+00011220: 6174 6368 6573 2c20 7265 7665 7273 653d  atches, reverse=
+00011230: 5472 7565 2c20 6b65 793d 6c61 6d62 6461  True, key=lambda
+00011240: 206d 5f77 5f77 6569 6768 743a 206d 5f77   m_w_weight: m_w
+00011250: 5f77 6569 6768 745b 325d 290a 0a20 2020  _weight[2])..   
+00011260: 2072 6574 7572 6e20 736f 7274 6564 285f   return sorted(_
+00011270: 7374 6162 6c65 5f76 6f74 696e 6728 6564  stable_voting(ed
+00011280: 6174 612c 200a 2020 2020 2020 2020 2020  ata, .          
+00011290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000112a0: 2020 2020 2020 2063 7572 725f 6361 6e64         curr_cand
+000112b0: 7320 3d20 6375 7272 5f63 616e 6473 2c20  s = curr_cands, 
+000112c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000112d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000112e0: 2020 7374 7265 6e67 7468 5f66 756e 6374    strength_funct
+000112f0: 696f 6e20 3d20 7374 7265 6e67 7468 5f66  ion = strength_f
+00011300: 756e 6374 696f 6e2c 0a20 2020 2020 2020  unction,.       
+00011310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011320: 2020 2020 2020 2020 2020 736f 7274 6564            sorted
+00011330: 5f6d 6174 6368 6573 203d 2073 6f72 7465  _matches = sorte
+00011340: 645f 6d61 7463 6865 732c 0a20 2020 2020  d_matches,.     
+00011350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011360: 2020 2020 2020 2020 2020 2020 6d65 6d5f              mem_
+00011370: 7376 5f77 696e 6e65 7273 203d 207b 7d29  sv_winners = {})
+00011380: 5b30 5d29 0a0a 7376 5f70 726f 7065 7274  [0])..sv_propert
+00011390: 6965 7320 3d20 566f 7469 6e67 4d65 7468  ies = VotingMeth
+000113a0: 6f64 5072 6f70 6572 7469 6573 280a 2020  odProperties(.  
+000113b0: 2020 636f 6e64 6f72 6365 745f 7769 6e6e    condorcet_winn
+000113c0: 6572 3d54 7275 652c 200a 2020 2020 636f  er=True, .    co
+000113d0: 6e64 6f72 6365 745f 6c6f 7365 723d 5472  ndorcet_loser=Tr
+000113e0: 7565 2c0a 2020 2020 7061 7265 746f 5f64  ue,.    pareto_d
+000113f0: 6f6d 696e 616e 6365 3d54 7275 652c 0a20  ominance=True,. 
+00011400: 2020 2070 6f73 6974 6976 655f 696e 766f     positive_invo
+00011410: 6c76 656d 656e 743d 4661 6c73 652c 2020  lvement=False,  
+00011420: 0a20 2020 2029 0a40 766d 286e 616d 6520  .    ).@vm(name 
+00011430: 3d20 2253 7461 626c 6520 566f 7469 6e67  = "Stable Voting
+00011440: 222c 0a20 2020 2070 726f 7065 7274 6965  ",.    propertie
+00011450: 7320 3d20 7376 5f70 726f 7065 7274 6965  s = sv_propertie
+00011460: 732c 0a20 2020 2069 6e70 7574 5f74 7970  s,.    input_typ
+00011470: 6573 203d 205b 456c 6563 7469 6f6e 5479  es = [ElectionTy
+00011480: 7065 732e 5052 4f46 494c 452c 2045 6c65  pes.PROFILE, Ele
+00011490: 6374 696f 6e54 7970 6573 2e50 524f 4649  ctionTypes.PROFI
+000114a0: 4c45 5f57 4954 485f 5449 4553 2c20 456c  LE_WITH_TIES, El
+000114b0: 6563 7469 6f6e 5479 7065 732e 4d41 5247  ectionTypes.MARG
+000114c0: 494e 5f47 5241 5048 5d29 0a64 6566 2073  IN_GRAPH]).def s
+000114d0: 7461 626c 655f 766f 7469 6e67 280a 2020  table_voting(.  
+000114e0: 2020 6564 6174 612c 200a 2020 2020 6375    edata, .    cu
+000114f0: 7272 5f63 616e 6473 3d4e 6f6e 652c 200a  rr_cands=None, .
+00011500: 2020 2020 7374 7265 6e67 7468 5f66 756e      strength_fun
+00011510: 6374 696f 6e3d 4e6f 6e65 2c20 0a20 2020  ction=None, .   
+00011520: 2061 6c67 6f72 6974 686d 3d27 6261 7369   algorithm='basi
+00011530: 6327 293a 200a 2020 2020 2222 2249 6d70  c'): .    """Imp
+00011540: 6c65 6d65 6e74 6174 696f 6e20 6f66 2020  lementation of  
+00011550: 5374 6162 6c65 2056 6f74 696e 6720 6672  Stable Voting fr
+00011560: 6f6d 2068 7474 7073 3a2f 2f61 7278 6976  om https://arxiv
+00011570: 2e6f 7267 2f61 6273 2f32 3130 382e 3030  .org/abs/2108.00
+00011580: 3534 322e 200a 0a20 2020 2053 7461 626c  542. ..    Stabl
+00011590: 6520 566f 7469 6e67 2069 7320 6120 7265  e Voting is a re
+000115a0: 6375 7273 6976 6520 766f 7469 6e67 206d  cursive voting m
+000115b0: 6574 686f 6420 6465 6669 6e65 6420 6173  ethod defined as
+000115c0: 2066 6f6c 6c6f 7773 3a20 0a0a 2020 2020   follows: ..    
+000115d0: 312e 2020 4966 2074 6865 7265 2069 7320  1.  If there is 
+000115e0: 6f6e 6c79 206f 6e65 2063 616e 6469 6461  only one candida
+000115f0: 7465 2069 6e20 7468 6520 7072 6f66 696c  te in the profil
+00011600: 652c 2074 6865 6e20 7468 6174 2063 616e  e, then that can
+00011610: 6469 6461 7465 2069 7320 7468 6520 7769  didate is the wi
+00011620: 6e6e 6572 2e20 0a20 2020 2032 2e20 4f72  nner. .    2. Or
+00011630: 6465 7220 7468 6520 7061 6972 7320 3a6d  der the pairs :m
+00011640: 6174 683a 6028 612c 6229 6020 6f66 2063  ath:`(a,b)` of c
+00011650: 616e 6469 6461 7465 7320 6672 6f6d 206c  andidates from l
+00011660: 6172 6765 7374 2074 6f20 736d 616c 6c65  argest to smalle
+00011670: 7374 2076 616c 7565 206f 6620 7468 6520  st value of the 
+00011680: 6d61 7267 696e 206f 6620 3a6d 6174 683a  margin of :math:
+00011690: 6061 6020 6f76 6572 203a 6d61 7468 3a60  `a` over :math:`
+000116a0: 6260 2073 7563 6820 7468 6174 203a 6d61  b` such that :ma
+000116b0: 7468 3a60 6160 2069 7320 756e 6465 6665  th:`a` is undefe
+000116c0: 6174 6564 2061 6363 6f72 6469 6e67 2074  ated according t
+000116d0: 6f20 5370 6c69 7420 4379 636c 652c 2061  o Split Cycle, a
+000116e0: 6e64 2064 6563 6c61 7265 2061 7320 5374  nd declare as St
+000116f0: 6162 6c65 2056 6f74 696e 6720 7769 6e6e  able Voting winn
+00011700: 6572 7320 7468 6520 6361 6e64 6964 6174  ers the candidat
+00011710: 6528 7329 203a 6d61 7468 3a60 6160 2066  e(s) :math:`a` f
+00011720: 726f 6d20 7468 6520 6561 726c 6965 7374  rom the earliest
+00011730: 2070 6169 7228 7329 203a 6d61 7468 3a60   pair(s) :math:`
+00011740: 2861 2c62 2960 2073 7563 6820 7468 6174  (a,b)` such that
+00011750: 203a 6d61 7468 3a60 6160 2069 7320 6120   :math:`a` is a 
+00011760: 5369 6d70 6c65 2053 7461 626c 6520 566f  Simple Stable Vo
+00011770: 7469 6e67 2077 696e 6e65 7220 696e 2074  ting winner in t
+00011780: 6865 2065 6c65 6374 696f 6e20 7769 7468  he election with
+00011790: 6f75 7420 3a6d 6174 683a 6062 602e 200a  out :math:`b`. .
+000117a0: 0a20 2020 2041 7267 733a 0a20 2020 2020  .    Args:.     
+000117b0: 2020 2065 6461 7461 2028 5072 6f66 696c     edata (Profil
+000117c0: 652c 2050 726f 6669 6c65 5769 7468 5469  e, ProfileWithTi
+000117d0: 6573 2c20 4d61 7267 696e 4772 6170 6829  es, MarginGraph)
+000117e0: 3a20 416e 7920 656c 6563 7469 6f6e 2064  : Any election d
+000117f0: 6174 6120 7468 6174 2068 6173 2061 2060  ata that has a `
+00011800: 6d61 7267 696e 6020 6d65 7468 6f64 2e20  margin` method. 
+00011810: 0a20 2020 2020 2020 2063 7572 725f 6361  .        curr_ca
+00011820: 6e64 7320 284c 6973 745b 696e 745d 2c20  nds (List[int], 
+00011830: 6f70 7469 6f6e 616c 293a 2049 6620 7365  optional): If se
+00011840: 742c 2074 6865 6e20 6669 6e64 2074 6865  t, then find the
+00011850: 2077 696e 6e65 7273 2066 6f72 2074 6865   winners for the
+00011860: 2070 726f 6669 6c65 2072 6573 7472 6963   profile restric
+00011870: 7465 6420 746f 2074 6865 2063 616e 6469  ted to the candi
+00011880: 6461 7465 7320 696e 2060 6063 7572 725f  dates in ``curr_
+00011890: 6361 6e64 7360 600a 2020 2020 2020 2020  cands``.        
+000118a0: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
+000118b0: 6e20 2866 756e 6374 696f 6e2c 206f 7074  n (function, opt
+000118c0: 696f 6e61 6c29 3a20 5468 6520 7374 7265  ional): The stre
+000118d0: 6e67 7468 2066 756e 6374 696f 6e20 746f  ngth function to
+000118e0: 2062 6520 7573 6564 2074 6f20 6361 6c63   be used to calc
+000118f0: 756c 6174 6520 7468 6520 7374 7265 6e67  ulate the streng
+00011900: 7468 206f 6620 6120 7061 7468 2e20 2020  th of a path.   
+00011910: 5468 6520 6465 6661 756c 7420 6973 2074  The default is t
+00011920: 6865 206d 6172 6769 6e20 6d65 7468 6f64  he margin method
+00011930: 206f 6620 6060 6564 6174 6160 602e 2020   of ``edata``.  
+00011940: 2054 6869 7320 6f6e 6c79 206d 6174 7465   This only matte
+00011950: 7273 2077 6865 6e20 7468 6520 6261 6c6c  rs when the ball
+00011960: 6f74 7320 6172 6520 6e6f 7420 6c69 6e65  ots are not line
+00011970: 6172 206f 7264 6572 732e 200a 0a20 2020  ar orders. ..   
+00011980: 2052 6574 7572 6e73 3a20 0a20 2020 2020   Returns: .     
+00011990: 2020 2041 2073 6f72 7465 6420 6c69 7374     A sorted list
+000119a0: 206f 6620 6361 6e64 6964 6174 6573 2e20   of candidates. 
+000119b0: 0a0a 2020 2020 2e2e 2073 6565 616c 736f  ..    .. seealso
+000119c0: 3a3a 0a0a 2020 2020 2020 2020 3a6d 6574  ::..        :met
+000119d0: 683a 6070 7265 665f 766f 7469 6e67 2e6d  h:`pref_voting.m
+000119e0: 6172 6769 6e5f 6261 7365 645f 6d65 7468  argin_based_meth
+000119f0: 6f64 732e 7369 6d70 6c65 5f73 7461 626c  ods.simple_stabl
+00011a00: 655f 766f 7469 6e67 600a 0a0a 2020 2020  e_voting`...    
+00011a10: 3a45 7861 6d70 6c65 3a20 0a0a 2020 2020  :Example: ..    
+00011a20: 2e2e 2065 7865 635f 636f 6465 3a3a 0a0a  .. exec_code::..
+00011a30: 2020 2020 2020 2020 6672 6f6d 2070 7265          from pre
+00011a40: 665f 766f 7469 6e67 2e77 6569 6768 7465  f_voting.weighte
+00011a50: 645f 6d61 6a6f 7269 7479 5f67 7261 7068  d_majority_graph
+00011a60: 7320 696d 706f 7274 204d 6172 6769 6e47  s import MarginG
+00011a70: 7261 7068 0a20 2020 2020 2020 2066 726f  raph.        fro
+00011a80: 6d20 7072 6566 5f76 6f74 696e 672e 6d61  m pref_voting.ma
+00011a90: 7267 696e 5f62 6173 6564 5f6d 6574 686f  rgin_based_metho
+00011aa0: 6473 2069 6d70 6f72 7420 7374 6162 6c65  ds import stable
+00011ab0: 5f76 6f74 696e 670a 0a20 2020 2020 2020  _voting..       
+00011ac0: 206d 6720 3d20 4d61 7267 696e 4772 6170   mg = MarginGrap
+00011ad0: 6828 5b30 2c20 312c 2032 2c20 335d 2c20  h([0, 1, 2, 3], 
+00011ae0: 5b28 302c 2033 2c20 3829 2c20 2831 2c20  [(0, 3, 8), (1, 
+00011af0: 302c 2031 3029 2c20 2832 2c20 302c 2034  0, 10), (2, 0, 4
+00011b00: 292c 2028 322c 2031 2c20 3829 2c20 2833  ), (2, 1, 8), (3
+00011b10: 2c20 312c 2038 295d 290a 0a20 2020 2020  , 1, 8)])..     
+00011b20: 2020 2073 7461 626c 655f 766f 7469 6e67     stable_voting
+00011b30: 2e64 6973 706c 6179 286d 6729 0a20 2020  .display(mg).   
+00011b40: 2020 2020 2073 7461 626c 655f 766f 7469       stable_voti
+00011b50: 6e67 2e64 6973 706c 6179 286d 672c 2061  ng.display(mg, a
+00011b60: 6c67 6f72 6974 686d 3d27 6261 7369 6327  lgorithm='basic'
+00011b70: 290a 2020 2020 2020 2020 7374 6162 6c65  ).        stable
+00011b80: 5f76 6f74 696e 672e 6469 7370 6c61 7928  _voting.display(
+00011b90: 6d67 2c20 616c 676f 7269 7468 6d3d 2777  mg, algorithm='w
+00011ba0: 6974 685f 636f 6e64 6f72 6365 745f 6368  ith_condorcet_ch
+00011bb0: 6563 6b27 290a 0a20 2020 2022 2222 0a0a  eck')..    """..
+00011bc0: 2020 2020 6966 2061 6c67 6f72 6974 686d      if algorithm
+00011bd0: 203d 3d20 2762 6173 6963 273a 200a 2020   == 'basic': .  
+00011be0: 2020 2020 2020 7265 7475 726e 205f 7374        return _st
+00011bf0: 6162 6c65 5f76 6f74 696e 675f 6261 7369  able_voting_basi
+00011c00: 6328 6564 6174 612c 2063 7572 725f 6361  c(edata, curr_ca
+00011c10: 6e64 7320 3d20 6375 7272 5f63 616e 6473  nds = curr_cands
+00011c20: 2c20 7374 7265 6e67 7468 5f66 756e 6374  , strength_funct
+00011c30: 696f 6e20 3d20 7374 7265 6e67 7468 5f66  ion = strength_f
+00011c40: 756e 6374 696f 6e29 0a20 2020 2065 6c69  unction).    eli
+00011c50: 6620 616c 676f 7269 7468 6d20 3d3d 2027  f algorithm == '
+00011c60: 7769 7468 5f63 6f6e 646f 7263 6574 5f63  with_condorcet_c
+00011c70: 6865 636b 273a 0a20 2020 2020 2020 2072  heck':.        r
+00011c80: 6574 7572 6e20 5f73 7461 626c 655f 766f  eturn _stable_vo
+00011c90: 7469 6e67 5f77 6974 685f 636f 6e64 6f72  ting_with_condor
+00011ca0: 6365 745f 6368 6563 6b28 6564 6174 612c  cet_check(edata,
+00011cb0: 2063 7572 725f 6361 6e64 7320 3d20 6375   curr_cands = cu
+00011cc0: 7272 5f63 616e 6473 2c20 7374 7265 6e67  rr_cands, streng
+00011cd0: 7468 5f66 756e 6374 696f 6e20 3d20 7374  th_function = st
+00011ce0: 7265 6e67 7468 5f66 756e 6374 696f 6e29  rength_function)
+00011cf0: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
+00011d00: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
+00011d10: 726f 7228 2249 6e76 616c 6964 2061 6c67  ror("Invalid alg
+00011d20: 6f72 6974 686d 2073 7065 6369 6669 6564  orithm specified
+00011d30: 2e22 290a 2020 2020 0a0a 6573 7365 6e74  .").    ..essent
+00011d40: 6961 6c5f 7365 745f 7072 6f70 6572 7469  ial_set_properti
+00011d50: 6573 203d 2056 6f74 696e 674d 6574 686f  es = VotingMetho
+00011d60: 6450 726f 7065 7274 6965 7328 0a20 2020  dProperties(.   
+00011d70: 2063 6f6e 646f 7263 6574 5f77 696e 6e65   condorcet_winne
+00011d80: 723d 5472 7565 2c20 0a20 2020 2063 6f6e  r=True, .    con
+00011d90: 646f 7263 6574 5f6c 6f73 6572 3d54 7275  dorcet_loser=Tru
+00011da0: 652c 0a20 2020 2070 6172 6574 6f5f 646f  e,.    pareto_do
+00011db0: 6d69 6e61 6e63 653d 5472 7565 2c0a 2020  minance=True,.  
+00011dc0: 2020 706f 7369 7469 7665 5f69 6e76 6f6c    positive_invol
+00011dd0: 7665 6d65 6e74 3d46 616c 7365 2c20 0a20  vement=False, . 
+00011de0: 2020 2029 0a40 766d 286e 616d 653d 2245     ).@vm(name="E
+00011df0: 7373 656e 7469 616c 2053 6574 222c 0a20  ssential Set",. 
+00011e00: 2020 2070 726f 7065 7274 6965 733d 6573     properties=es
+00011e10: 7365 6e74 6961 6c5f 7365 745f 7072 6f70  sential_set_prop
+00011e20: 6572 7469 6573 2c0a 2020 2020 696e 7075  erties,.    inpu
+00011e30: 745f 7479 7065 733d 5b45 6c65 6374 696f  t_types=[Electio
+00011e40: 6e54 7970 6573 2e50 524f 4649 4c45 2c20  nTypes.PROFILE, 
+00011e50: 456c 6563 7469 6f6e 5479 7065 732e 5052  ElectionTypes.PR
+00011e60: 4f46 494c 455f 5749 5448 5f54 4945 532c  OFILE_WITH_TIES,
+00011e70: 2045 6c65 6374 696f 6e54 7970 6573 2e4d   ElectionTypes.M
+00011e80: 4152 4749 4e5f 4752 4150 485d 290a 6465  ARGIN_GRAPH]).de
+00011e90: 6620 6573 7365 6e74 6961 6c28 6564 6174  f essential(edat
+00011ea0: 612c 2063 7572 725f 6361 6e64 7320 3d20  a, curr_cands = 
+00011eb0: 4e6f 6e65 2c20 7468 7265 7368 6f6c 6420  None, threshold 
+00011ec0: 3d20 302e 3030 3030 3030 3129 3a20 0a20  = 0.0000001): . 
+00011ed0: 2020 2022 2222 5468 6520 4573 7365 6e74     """The Essent
+00011ee0: 6961 6c20 5365 7420 6973 2074 6865 2073  ial Set is the s
+00011ef0: 7570 706f 7274 206f 6620 7468 6520 2863  upport of the (c
+00011f00: 686f 7365 6e29 2043 3220 6d61 7869 6d61  hosen) C2 maxima
+00011f10: 6c20 6c6f 7474 6572 792e 0a0a 2020 2020  l lottery...    
+00011f20: 4172 6773 3a0a 2020 2020 2020 2020 6564  Args:.        ed
+00011f30: 6174 6120 2850 726f 6669 6c65 2c20 5072  ata (Profile, Pr
+00011f40: 6f66 696c 6557 6974 6854 6965 732c 204d  ofileWithTies, M
+00011f50: 6172 6769 6e47 7261 7068 293a 2041 6e79  arginGraph): Any
+00011f60: 2065 6c65 6374 696f 6e20 6461 7461 2074   election data t
+00011f70: 6861 7420 6861 7320 6120 606d 6172 6769  hat has a `margi
+00011f80: 6e5f 6d61 7472 6978 6020 6174 7472 6962  n_matrix` attrib
+00011f90: 7574 652e 0a20 2020 2020 2020 2063 7572  ute..        cur
+00011fa0: 725f 6361 6e64 7320 284c 6973 745b 696e  r_cands (List[in
+00011fb0: 745d 2c20 6f70 7469 6f6e 616c 293a 2049  t], optional): I
+00011fc0: 6620 7365 742c 2074 6865 6e20 6669 6e64  f set, then find
+00011fd0: 2074 6865 2077 696e 6e65 7273 2066 6f72   the winners for
+00011fe0: 2074 6865 2070 726f 6669 6c65 2072 6573   the profile res
+00011ff0: 7472 6963 7465 6420 746f 2074 6865 2063  tricted to the c
+00012000: 616e 6469 6461 7465 7320 696e 2060 6063  andidates in ``c
+00012010: 7572 725f 6361 6e64 7360 600a 0a20 2020  urr_cands``..   
+00012020: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
+00012030: 2020 4120 736f 7274 6564 206c 6973 7420    A sorted list 
+00012040: 6f66 2063 616e 6469 6461 7465 732e 0a0a  of candidates...
+00012050: 2020 2020 2222 220a 2020 2020 6d6c 203d      """.    ml =
+00012060: 206d 6178 696d 616c 5f6c 6f74 7465 7279   maximal_lottery
+00012070: 2865 6461 7461 2c20 6375 7272 5f63 616e  (edata, curr_can
+00012080: 6473 3d63 7572 725f 6361 6e64 7329 0a0a  ds=curr_cands)..
+00012090: 2020 2020 7265 7475 726e 2073 6f72 7465      return sorte
+000120a0: 6428 5b63 2066 6f72 2063 2069 6e20 6d6c  d([c for c in ml
+000120b0: 2e6b 6579 7328 2920 6966 206d 6c5b 635d  .keys() if ml[c]
+000120c0: 203e 2074 6872 6573 686f 6c64 5d29 0a0a   > threshold])..
+000120d0: 7765 6967 6874 6564 5f63 6f76 6572 696e  weighted_coverin
+000120e0: 675f 7072 6f70 6572 7469 6573 203d 2056  g_properties = V
+000120f0: 6f74 696e 674d 6574 686f 6450 726f 7065  otingMethodPrope
+00012100: 7274 6965 7328 0a20 2020 2063 6f6e 646f  rties(.    condo
+00012110: 7263 6574 5f77 696e 6e65 723d 5472 7565  rcet_winner=True
+00012120: 2c20 0a20 2020 2063 6f6e 646f 7263 6574  , .    condorcet
+00012130: 5f6c 6f73 6572 3d54 7275 652c 0a20 2020  _loser=True,.   
+00012140: 2070 6172 6574 6f5f 646f 6d69 6e61 6e63   pareto_dominanc
+00012150: 653d 5472 7565 2c0a 2020 2020 706f 7369  e=True,.    posi
+00012160: 7469 7665 5f69 6e76 6f6c 7665 6d65 6e74  tive_involvement
+00012170: 3d54 7275 652c 200a 2020 2020 290a 4076  =True, .    ).@v
+00012180: 6d28 6e61 6d65 3d22 5765 6967 6874 6564  m(name="Weighted
+00012190: 2043 6f76 6572 696e 6722 2c0a 2020 2020   Covering",.    
+000121a0: 7072 6f70 6572 7469 6573 3d77 6569 6768  properties=weigh
+000121b0: 7465 645f 636f 7665 7269 6e67 5f70 726f  ted_covering_pro
+000121c0: 7065 7274 6965 732c 0a20 2020 2069 6e70  perties,.    inp
+000121d0: 7574 5f74 7970 6573 3d5b 456c 6563 7469  ut_types=[Electi
+000121e0: 6f6e 5479 7065 732e 5052 4f46 494c 452c  onTypes.PROFILE,
+000121f0: 2045 6c65 6374 696f 6e54 7970 6573 2e50   ElectionTypes.P
+00012200: 524f 4649 4c45 5f57 4954 485f 5449 4553  ROFILE_WITH_TIES
+00012210: 2c20 456c 6563 7469 6f6e 5479 7065 732e  , ElectionTypes.
+00012220: 4d41 5247 494e 5f47 5241 5048 5d29 0a64  MARGIN_GRAPH]).d
+00012230: 6566 2077 6569 6768 7465 645f 636f 7665  ef weighted_cove
+00012240: 7269 6e67 2865 6461 7461 2c20 6375 7272  ring(edata, curr
+00012250: 5f63 616e 6473 3d4e 6f6e 6529 3a20 0a20  _cands=None): . 
+00012260: 2020 2022 2222 4163 636f 7264 696e 6720     """According 
+00012270: 746f 2057 6569 6768 7465 6420 436f 7665  to Weighted Cove
+00012280: 7269 6e67 2c20 7820 6465 6665 6174 7320  ring, x defeats 
+00012290: 7920 6966 2074 6865 206d 6172 6769 6e20  y if the margin 
+000122a0: 6f66 2078 206f 7665 7220 7920 6973 2070  of x over y is p
+000122b0: 6f73 6974 6976 6520 616e 6420 666f 7220  ositive and for 
+000122c0: 6576 6572 7920 6f74 6865 7220 7a2c 2074  every other z, t
+000122d0: 6865 206d 6172 6769 6e20 6f66 2078 206f  he margin of x o
+000122e0: 7665 7220 7a20 6973 2067 7265 6174 6572  ver z is greater
+000122f0: 2074 6861 6e20 6f72 2065 7175 616c 2074   than or equal t
+00012300: 6f20 7468 6520 6d61 7267 696e 206f 6620  o the margin of 
+00012310: 7920 6f76 6572 207a 2e20 0a0a 2020 2020  y over z. ..    
+00012320: 4172 6773 3a0a 2020 2020 2020 2020 6564  Args:.        ed
+00012330: 6174 6120 2850 726f 6669 6c65 2c20 5072  ata (Profile, Pr
+00012340: 6f66 696c 6557 6974 6854 6965 732c 204d  ofileWithTies, M
+00012350: 6172 6769 6e47 7261 7068 293a 2041 6e79  arginGraph): Any
+00012360: 2065 6c65 6374 696f 6e20 6461 7461 2074   election data t
+00012370: 6861 7420 6861 7320 6120 606d 6172 6769  hat has a `margi
+00012380: 6e60 206d 6574 686f 642e 0a20 2020 2020  n` method..     
+00012390: 2020 2063 7572 725f 6361 6e64 7320 284c     curr_cands (L
+000123a0: 6973 745b 696e 745d 2c20 6f70 7469 6f6e  ist[int], option
+000123b0: 616c 293a 2049 6620 7365 742c 2074 6865  al): If set, the
+000123c0: 6e20 6669 6e64 2074 6865 2077 696e 6e65  n find the winne
+000123d0: 7273 2066 6f72 2074 6865 2070 726f 6669  rs for the profi
+000123e0: 6c65 2072 6573 7472 6963 7465 6420 746f  le restricted to
+000123f0: 2074 6865 2063 616e 6469 6461 7465 7320   the candidates 
+00012400: 696e 2060 6063 7572 725f 6361 6e64 7360  in ``curr_cands`
+00012410: 600a 0a20 2020 2052 6574 7572 6e73 3a0a  `..    Returns:.
+00012420: 2020 2020 2020 2020 4120 736f 7274 6564          A sorted
+00012430: 206c 6973 7420 6f66 2063 616e 6469 6461   list of candida
+00012440: 7465 732e 0a0a 2020 2020 2e2e 206e 6f74  tes...    .. not
+00012450: 653a 3a0a 2020 2020 2020 2020 5365 652c  e::.        See,
+00012460: 2065 2e67 2e2c 2042 6861 736b 6172 2044   e.g., Bhaskar D
+00012470: 7574 7461 2061 6e64 204a 6561 6e2d 4672  utta and Jean-Fr
+00012480: 616e 636f 6973 204c 6173 6c69 6572 2c20  ancois Laslier, 
+00012490: 2243 6f6d 7061 7269 736f 6e20 6675 6e63  "Comparison func
+000124a0: 7469 6f6e 7320 616e 6420 6368 6f69 6365  tions and choice
+000124b0: 2063 6f72 7265 7370 6f6e 6465 6e63 6573   correspondences
+000124c0: 2c22 2053 6f63 6961 6c20 4368 6f69 6365  ," Social Choice
+000124d0: 2061 6e64 2057 656c 6661 7265 2c20 3136   and Welfare, 16
+000124e0: 3a35 3133 e280 9335 3332 2c20 3139 3939  :513...532, 1999
+000124f0: 2c20 646f 693a 3130 2e31 3030 372f 7330  , doi:10.1007/s0
+00012500: 3033 3535 3030 3530 3135 382c 2061 6e64  03550050158, and
+00012510: 2052 6175 cc81 6c20 5065 cc81 7265 7a2d   Rau..l Pe..rez-
+00012520: 4665 726e 61cc 816e 6465 7a20 616e 6420  Ferna..ndez and 
+00012530: 4265 726e 6172 6420 4465 2042 6165 7473  Bernard De Baets
+00012540: 2c20 2254 6865 2073 7570 6572 636f 7665  , "The supercove
+00012550: 7269 6e67 2072 656c 6174 696f 6e2c 2074  ring relation, t
+00012560: 6865 2070 6169 7277 6973 6520 7769 6e6e  he pairwise winn
+00012570: 6572 2c20 616e 6420 6d6f 7265 206d 6973  er, and more mis
+00012580: 7369 6e67 206c 696e 6b73 2062 6574 7765  sing links betwe
+00012590: 656e 2042 6f72 6461 2061 6e64 2043 6f6e  en Borda and Con
+000125a0: 646f 7263 6574 2c22 2053 6f63 6961 6c20  dorcet," Social 
+000125b0: 4368 6f69 6365 2061 6e64 2057 656c 6661  Choice and Welfa
+000125c0: 7265 2c20 3530 3a33 3239 e280 9333 3532  re, 50:329...352
+000125d0: 2c20 3230 3138 2c20 646f 693a 3130 2e31  , 2018, doi:10.1
+000125e0: 3030 372f 7330 3033 3535 2d30 3137 2d31  007/s00355-017-1
+000125f0: 3038 362d 302e 0a20 2020 2022 2222 0a0a  086-0..    """..
+00012600: 2020 2020 6361 6e64 6964 6174 6573 203d      candidates =
+00012610: 2065 6461 7461 2e63 616e 6469 6461 7465   edata.candidate
+00012620: 7320 6966 2063 7572 725f 6361 6e64 7320  s if curr_cands 
+00012630: 6973 204e 6f6e 6520 656c 7365 2063 7572  is None else cur
+00012640: 725f 6361 6e64 730a 0a20 2020 2075 635f  r_cands..    uc_
+00012650: 7365 7420 3d20 6c69 7374 2829 0a0a 2020  set = list()..  
+00012660: 2020 666f 7220 7920 696e 2063 616e 6469    for y in candi
+00012670: 6461 7465 733a 0a20 2020 2020 2020 2069  dates:.        i
+00012680: 735f 696e 5f75 6373 203d 2054 7275 650a  s_in_ucs = True.
+00012690: 2020 2020 2020 2020 666f 7220 7820 696e          for x in
+000126a0: 2065 6461 7461 2e64 6f6d 696e 6174 6f72   edata.dominator
+000126b0: 7328 792c 2063 7572 725f 6361 6e64 7320  s(y, curr_cands 
+000126c0: 3d20 6375 7272 5f63 616e 6473 293a 0a20  = curr_cands):. 
+000126d0: 2020 2020 2020 2020 2020 2023 2063 6865             # che
+000126e0: 636b 2069 6620 7920 636f 7665 7273 2078  ck if y covers x
+000126f0: 2c20 692e 652e 2c20 666f 7220 6576 6572  , i.e., for ever
+00012700: 7920 7a2c 206d 6172 6769 6e28 782c 207a  y z, margin(x, z
+00012710: 2920 3e3d 206d 6172 6769 6e28 792c 207a  ) >= margin(y, z
+00012720: 290a 2020 2020 2020 2020 2020 2020 636f  ).            co
+00012730: 7665 7273 203d 2054 7275 650a 2020 2020  vers = True.    
+00012740: 2020 2020 2020 2020 666f 7220 7a20 696e          for z in
+00012750: 2063 616e 6469 6461 7465 733a 0a20 2020   candidates:.   
+00012760: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00012770: 6564 6174 612e 6d61 7267 696e 2878 2c20  edata.margin(x, 
+00012780: 7a29 203c 2065 6461 7461 2e6d 6172 6769  z) < edata.margi
+00012790: 6e28 792c 207a 293a 0a20 2020 2020 2020  n(y, z):.       
+000127a0: 2020 2020 2020 2020 2020 2020 2063 6f76               cov
+000127b0: 6572 7320 3d20 4661 6c73 650a 2020 2020  ers = False.    
+000127c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000127d0: 6272 6561 6b0a 2020 2020 2020 2020 2020  break.          
+000127e0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+000127f0: 636f 7665 7273 3a0a 2020 2020 2020 2020  covers:.        
+00012800: 2020 2020 2020 2020 6973 5f69 6e5f 7563          is_in_uc
+00012810: 7320 3d20 4661 6c73 650a 2020 2020 2020  s = False.      
+00012820: 2020 2020 2020 2020 2020 6272 6561 6b0a            break.
+00012830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012840: 0a20 2020 2020 2020 2069 6620 6973 5f69  .        if is_i
+00012850: 6e5f 7563 733a 0a20 2020 2020 2020 2020  n_ucs:.         
+00012860: 2020 2075 635f 7365 742e 6170 7065 6e64     uc_set.append
+00012870: 2879 290a 0a20 2020 2072 6574 7572 6e20  (y)..    return 
+00012880: 736f 7274 6564 2875 635f 7365 7429 0a0a  sorted(uc_set)..
+00012890: 6c6f 7373 5f74 7269 6d6d 6572 5f70 726f  loss_trimmer_pro
+000128a0: 7065 7274 6965 7320 3d20 566f 7469 6e67  perties = Voting
+000128b0: 4d65 7468 6f64 5072 6f70 6572 7469 6573  MethodProperties
+000128c0: 280a 2020 2020 636f 6e64 6f72 6365 745f  (.    condorcet_
+000128d0: 7769 6e6e 6572 3d54 7275 652c 200a 2020  winner=True, .  
+000128e0: 2020 636f 6e64 6f72 6365 745f 6c6f 7365    condorcet_lose
+000128f0: 723d 5472 7565 2c0a 2020 2020 7061 7265  r=True,.    pare
+00012900: 746f 5f64 6f6d 696e 616e 6365 3d54 7275  to_dominance=Tru
+00012910: 652c 0a20 2020 2070 6f73 6974 6976 655f  e,.    positive_
+00012920: 696e 766f 6c76 656d 656e 743d 4661 6c73  involvement=Fals
+00012930: 652c 200a 2020 2020 290a 4076 6d28 6e61  e, .    ).@vm(na
+00012940: 6d65 203d 2022 4c6f 7373 2d54 7269 6d6d  me = "Loss-Trimm
+00012950: 6572 2056 6f74 696e 6722 2c0a 2020 2020  er Voting",.    
+00012960: 7072 6f70 6572 7469 6573 203d 206c 6f73  properties = los
+00012970: 735f 7472 696d 6d65 725f 7072 6f70 6572  s_trimmer_proper
+00012980: 7469 6573 2c0a 2020 2020 696e 7075 745f  ties,.    input_
+00012990: 7479 7065 7320 3d20 5b45 6c65 6374 696f  types = [Electio
+000129a0: 6e54 7970 6573 2e50 524f 4649 4c45 2c20  nTypes.PROFILE, 
+000129b0: 456c 6563 7469 6f6e 5479 7065 732e 5052  ElectionTypes.PR
+000129c0: 4f46 494c 455f 5749 5448 5f54 4945 532c  OFILE_WITH_TIES,
+000129d0: 2045 6c65 6374 696f 6e54 7970 6573 2e4d   ElectionTypes.M
+000129e0: 4152 4749 4e5f 4752 4150 485d 290a 6465  ARGIN_GRAPH]).de
+000129f0: 6620 6c6f 7373 5f74 7269 6d6d 6572 2865  f loss_trimmer(e
+00012a00: 6461 7461 2c20 6375 7272 5f63 616e 6473  data, curr_cands
+00012a10: 203d 204e 6f6e 6529 3a0a 2020 2020 2222   = None):.    ""
+00012a20: 2249 7465 7261 7469 7665 6c79 2065 6c69  "Iteratively eli
+00012a30: 6d69 6e61 7465 2074 6865 2063 616e 6469  minate the candi
+00012a40: 6461 7465 2077 6974 6820 7468 6520 6c61  date with the la
+00012a50: 7267 6573 7420 7375 6d20 6f66 206d 6172  rgest sum of mar
+00012a60: 6769 6e73 206f 6620 6c6f 7373 2075 6e74  gins of loss unt
+00012a70: 696c 2061 2043 6f6e 646f 7263 6574 2077  il a Condorcet w
+00012a80: 696e 6e65 7220 6973 2066 6f75 6e64 2e20  inner is found. 
+00012a90: 496e 2074 6869 7320 7665 7273 696f 6e20  In this version 
+00012aa0: 6f66 2074 6865 206d 6574 686f 642c 2070  of the method, p
+00012ab0: 6172 616c 6c65 6c2d 756e 6976 6572 7365  arallel-universe
+00012ac0: 2074 6965 6272 6561 6b69 6e67 2069 7320   tiebreaking is 
+00012ad0: 7573 6564 2069 6620 7468 6572 6520 6172  used if there ar
+00012ae0: 6520 6d75 6c74 6970 6c65 2063 616e 6469  e multiple candi
+00012af0: 6461 7465 7320 7769 7468 2074 6865 206c  dates with the l
+00012b00: 6172 6765 7374 2073 756d 206f 6620 6d61  argest sum of ma
+00012b10: 7267 696e 7320 6f66 206c 6f73 732e 0a0a  rgins of loss...
+00012b20: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+00012b30: 2020 6564 6174 6120 2850 726f 6669 6c65    edata (Profile
+00012b40: 2c20 5072 6f66 696c 6557 6974 6854 6965  , ProfileWithTie
+00012b50: 732c 204d 6172 6769 6e47 7261 7068 293a  s, MarginGraph):
+00012b60: 2041 6e79 2065 6c65 6374 696f 6e20 6461   Any election da
+00012b70: 7461 2074 6861 7420 6861 7320 6120 6d61  ta that has a ma
+00012b80: 7267 696e 206d 6574 686f 642e 0a20 2020  rgin method..   
+00012b90: 2020 2020 2063 7572 725f 6361 6e64 7320       curr_cands 
+00012ba0: 284c 6973 745b 696e 745d 2c20 6f70 7469  (List[int], opti
+00012bb0: 6f6e 616c 293a 2049 6620 7365 742c 2074  onal): If set, t
+00012bc0: 6865 6e20 6669 6e64 2074 6865 2077 696e  hen find the win
+00012bd0: 6e65 7273 2066 6f72 2074 6865 2070 726f  ners for the pro
+00012be0: 6669 6c65 2072 6573 7472 6963 7465 6420  file restricted 
+00012bf0: 746f 2074 6865 2063 616e 6469 6461 7465  to the candidate
+00012c00: 7320 696e 2060 6063 7572 725f 6361 6e64  s in ``curr_cand
+00012c10: 7360 600a 0a20 2020 2052 6574 7572 6e73  s``..    Returns
+00012c20: 3a20 0a20 2020 2020 2020 2041 2073 6f72  : .        A sor
+00012c30: 7465 6420 6c69 7374 206f 6620 6361 6e64  ted list of cand
+00012c40: 6964 6174 6573 0a0a 2020 2020 2e2e 206e  idates..    .. n
+00012c50: 6f74 653a 3a0a 2020 2020 2020 2020 4d65  ote::.        Me
+00012c60: 7468 6f64 2070 726f 706f 7365 6420 6279  thod proposed by
+00012c70: 2052 6963 6861 7264 2042 2e20 4461 726c   Richard B. Darl
+00012c80: 696e 6774 6f6e 2069 6e20 2254 6865 2043  ington in "The C
+00012c90: 6173 6520 666f 7220 7468 6520 4c6f 7373  ase for the Loss
+00012ca0: 2d54 7269 6d6d 6572 2056 6f74 696e 6720  -Trimmer Voting 
+00012cb0: 5379 7374 656d 2e22 0a0a 2020 2020 2222  System."..    ""
+00012cc0: 220a 0a20 2020 2063 7572 725f 6361 6e64  "..    curr_cand
+00012cd0: 7320 3d20 6564 6174 612e 6361 6e64 6964  s = edata.candid
+00012ce0: 6174 6573 2069 6620 6375 7272 5f63 616e  ates if curr_can
+00012cf0: 6473 2069 7320 4e6f 6e65 2065 6c73 6520  ds is None else 
+00012d00: 6375 7272 5f63 616e 6473 0a0a 2020 2020  curr_cands..    
+00012d10: 7765 616b 5f63 7720 3d20 6564 6174 612e  weak_cw = edata.
+00012d20: 7765 616b 5f63 6f6e 646f 7263 6574 5f77  weak_condorcet_w
+00012d30: 696e 6e65 7228 6375 7272 5f63 616e 6473  inner(curr_cands
+00012d40: 203d 2063 7572 725f 6361 6e64 7329 0a20   = curr_cands). 
+00012d50: 2020 2023 2049 6620 7468 6572 6520 6172     # If there ar
+00012d60: 6520 7765 616b 2043 6f6e 646f 7263 6574  e weak Condorcet
+00012d70: 2077 696e 6e65 7273 2c20 7265 7475 726e   winners, return
+00012d80: 2074 686f 7365 2063 616e 6469 6461 7465   those candidate
+00012d90: 730a 2020 2020 6966 2065 6461 7461 2e77  s.    if edata.w
+00012da0: 6561 6b5f 636f 6e64 6f72 6365 745f 7769  eak_condorcet_wi
+00012db0: 6e6e 6572 2863 7572 725f 6361 6e64 7320  nner(curr_cands 
+00012dc0: 3d20 6375 7272 5f63 616e 6473 2920 6973  = curr_cands) is
+00012dd0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00012de0: 2020 2072 6574 7572 6e20 736f 7274 6564     return sorted
+00012df0: 2877 6561 6b5f 6377 290a 2020 2020 0a20  (weak_cw).    . 
+00012e00: 2020 2023 204f 7468 6572 7769 7365 2c20     # Otherwise, 
+00012e10: 6361 6c63 756c 6174 6520 7468 6520 7375  calculate the su
+00012e20: 6d20 6f66 206d 6172 6769 6e73 206f 6620  m of margins of 
+00012e30: 6c6f 7373 2066 6f72 2065 6163 6820 6361  loss for each ca
+00012e40: 6e64 6964 6174 650a 2020 2020 7375 6d5f  ndidate.    sum_
+00012e50: 6f66 5f6d 6172 6769 6e73 5f6f 665f 6c6f  of_margins_of_lo
+00012e60: 7373 203d 207b 6361 6e64 3a20 7375 6d28  ss = {cand: sum(
+00012e70: 5b65 6461 7461 2e6d 6172 6769 6e28 6f74  [edata.margin(ot
+00012e80: 6865 725f 6361 6e64 2c20 6361 6e64 2920  her_cand, cand) 
+00012e90: 666f 7220 6f74 6865 725f 6361 6e64 2069  for other_cand i
+00012ea0: 6e20 6375 7272 5f63 616e 6473 2069 6620  n curr_cands if 
+00012eb0: 6564 6174 612e 6d61 7267 696e 286f 7468  edata.margin(oth
+00012ec0: 6572 5f63 616e 642c 2063 616e 6429 203e  er_cand, cand) >
+00012ed0: 2030 5d29 2066 6f72 2063 616e 6420 696e   0]) for cand in
+00012ee0: 2063 7572 725f 6361 6e64 737d 0a0a 2020   curr_cands}..  
+00012ef0: 2020 2320 4669 6e64 2074 6865 2063 616e    # Find the can
+00012f00: 6469 6461 7465 7320 7769 7468 2074 6865  didates with the
+00012f10: 206c 6172 6765 7374 2073 756d 206f 6620   largest sum of 
+00012f20: 6d61 7267 696e 7320 6f66 206c 6f73 730a  margins of loss.
+00012f30: 2020 2020 6d61 785f 7375 6d5f 6f66 5f6d      max_sum_of_m
+00012f40: 6172 6769 6e73 5f6f 665f 6c6f 7373 203d  argins_of_loss =
+00012f50: 206d 6178 2873 756d 5f6f 665f 6d61 7267   max(sum_of_marg
+00012f60: 696e 735f 6f66 5f6c 6f73 732e 7661 6c75  ins_of_loss.valu
+00012f70: 6573 2829 290a 2020 2020 6269 6767 6573  es()).    bigges
+00012f80: 745f 6c6f 7365 7273 203d 205b 6361 6e64  t_losers = [cand
+00012f90: 2066 6f72 2063 616e 6420 696e 2063 7572   for cand in cur
+00012fa0: 725f 6361 6e64 7320 6966 2073 756d 5f6f  r_cands if sum_o
+00012fb0: 665f 6d61 7267 696e 735f 6f66 5f6c 6f73  f_margins_of_los
+00012fc0: 735b 6361 6e64 5d20 3d3d 206d 6178 5f73  s[cand] == max_s
+00012fd0: 756d 5f6f 665f 6d61 7267 696e 735f 6f66  um_of_margins_of
+00012fe0: 5f6c 6f73 735d 0a0a 2020 2020 7769 6e6e  _loss]..    winn
+00012ff0: 6572 7320 3d20 5b5d 0a0a 2020 2020 2320  ers = []..    # 
+00013000: 466f 7220 6561 6368 2062 6967 6765 7374  For each biggest
+00013010: 206c 6f73 6572 2c20 6361 6c63 756c 6174   loser, calculat
+00013020: 6520 7468 6520 7769 6e6e 6572 7320 6166  e the winners af
+00013030: 7465 7220 7265 6d6f 7669 6e67 2074 6861  ter removing tha
+00013040: 7420 6361 6e64 6964 6174 652e 2054 6865  t candidate. The
+00013050: 2075 6e69 6f6e 206f 6620 7468 6573 6520   union of these 
+00013060: 7365 7473 2069 7320 7468 6520 7365 7420  sets is the set 
+00013070: 6f66 2077 696e 6e65 7273 2e0a 2020 2020  of winners..    
+00013080: 666f 7220 626c 2069 6e20 6269 6767 6573  for bl in bigges
+00013090: 745f 6c6f 7365 7273 3a0a 2020 2020 2020  t_losers:.      
+000130a0: 2020 7769 6e6e 6572 735f 7769 7468 6f75    winners_withou
+000130b0: 745f 626c 203d 206c 6f73 735f 7472 696d  t_bl = loss_trim
+000130c0: 6d65 7228 6564 6174 612c 2063 7572 725f  mer(edata, curr_
+000130d0: 6361 6e64 7320 3d20 5b63 616e 6420 666f  cands = [cand fo
+000130e0: 7220 6361 6e64 2069 6e20 6375 7272 5f63  r cand in curr_c
+000130f0: 616e 6473 2069 6620 6361 6e64 2021 3d20  ands if cand != 
+00013100: 626c 5d29 0a20 2020 2020 2020 2077 696e  bl]).        win
+00013110: 6e65 7273 202b 3d20 7769 6e6e 6572 735f  ners += winners_
+00013120: 7769 7468 6f75 745f 626c 0a0a 2020 2020  without_bl..    
+00013130: 7265 7475 726e 2073 6f72 7465 6428 6c69  return sorted(li
+00013140: 7374 2873 6574 2877 696e 6e65 7273 2929  st(set(winners))
+00013150: 290a 0a0a 6465 6620 6469 7374 616e 6365  )...def distance
+00013160: 5f74 6f5f 6d61 7267 696e 5f67 7261 7068  _to_margin_graph
+00013170: 2865 6461 7461 2c20 7265 6c2c 2065 7870  (edata, rel, exp
+00013180: 203d 2031 2c20 6375 7272 5f63 616e 6473   = 1, curr_cands
+00013190: 203d 204e 6f6e 6529 3a20 0a20 2020 2022   = None): .    "
+000131a0: 2222 0a20 2020 2043 616c 6375 6c61 7465  "".    Calculate
+000131b0: 2074 6865 2064 6973 7461 6e63 6520 6f66   the distance of
+000131c0: 2060 6072 656c 6060 2028 6120 7265 6c61   ``rel`` (a rela
+000131d0: 7469 6f6e 2920 746f 2074 6865 206d 616a  tion) to the maj
+000131e0: 6f72 6974 7920 6772 6170 6820 6f66 2060  ority graph of `
+000131f0: 6065 6461 7461 6060 2e20 0a20 2020 2022  `edata``. .    "
+00013200: 2222 0a20 2020 2063 616e 6469 6461 7465  "".    candidate
+00013210: 7320 3d20 6564 6174 612e 6361 6e64 6964  s = edata.candid
+00013220: 6174 6573 2069 6620 6375 7272 5f63 616e  ates if curr_can
+00013230: 6473 2069 7320 4e6f 6e65 2065 6c73 6520  ds is None else 
+00013240: 6375 7272 5f63 616e 6473 0a20 2020 200a  curr_cands.    .
+00013250: 2020 2020 6966 2074 7970 6528 6564 6174      if type(edat
+00013260: 6129 203d 3d20 4d61 6a6f 7269 7479 4772  a) == MajorityGr
+00013270: 6170 6820 616e 6420 6578 7020 3d3d 2030  aph and exp == 0
+00013280: 3a0a 2020 2020 2020 2020 2320 6966 2065  :.        # if e
+00013290: 6461 7461 2069 7320 6120 4d61 6a6f 7269  data is a Majori
+000132a0: 7479 4772 6170 682c 2077 6520 6e65 6564  tyGraph, we need
+000132b0: 2074 6f20 6164 6420 6d61 7267 696e 7320   to add margins 
+000132c0: 666f 7220 7468 6520 666f 6c6c 6f77 696e  for the followin
+000132d0: 6720 636f 6465 2074 6f20 776f 726b 2e20  g code to work. 
+000132e0: 2054 6865 206d 6172 6769 6e73 2064 6f20   The margins do 
+000132f0: 6e6f 7420 6d61 7474 6572 2077 6865 6e20  not matter when 
+00013300: 6578 703d 3d30 2e20 2020 0a20 2020 2020  exp==0.   .     
+00013310: 2020 2065 6461 7461 203d 204d 6172 6769     edata = Margi
+00013320: 6e47 7261 7068 2863 616e 6469 6461 7465  nGraph(candidate
+00013330: 732c 205b 2863 312c 2063 322c 2031 2920  s, [(c1, c2, 1) 
+00013340: 666f 7220 6331 2c20 6332 2069 6e20 6564  for c1, c2 in ed
+00013350: 6174 612e 6564 6765 7320 6966 2028 6331  ata.edges if (c1
+00013360: 2069 6e20 6361 6e64 6964 6174 6573 2061   in candidates a
+00013370: 6e64 2063 3220 696e 2063 616e 6469 6461  nd c2 in candida
+00013380: 7465 7329 5d29 0a20 2020 2070 656e 616c  tes)]).    penal
+00013390: 7479 203d 2030 0a20 2020 2066 6f72 2061  ty = 0.    for a
+000133a0: 2c62 2069 6e20 636f 6d62 696e 6174 696f  ,b in combinatio
+000133b0: 6e73 2863 616e 6469 6461 7465 732c 2032  ns(candidates, 2
+000133c0: 293a 200a 2020 2020 2020 2020 6966 2065  ): .        if e
+000133d0: 6461 7461 2e6d 616a 6f72 6974 795f 7072  data.majority_pr
+000133e0: 6566 6572 7328 612c 2062 2920 616e 6420  efers(a, b) and 
+000133f0: 2862 2c61 2920 696e 2072 656c 3a20 0a20  (b,a) in rel: . 
+00013400: 2020 2020 2020 2020 2020 2070 656e 616c             penal
+00013410: 7479 202b 3d20 2865 6461 7461 2e6d 6172  ty += (edata.mar
+00013420: 6769 6e28 612c 2062 2920 2a2a 2065 7870  gin(a, b) ** exp
+00013430: 290a 2020 2020 2020 2020 656c 6966 2065  ).        elif e
+00013440: 6461 7461 2e6d 616a 6f72 6974 795f 7072  data.majority_pr
+00013450: 6566 6572 7328 622c 2061 2920 616e 6420  efers(b, a) and 
+00013460: 2861 2c62 2920 696e 2072 656c 3a20 0a20  (a,b) in rel: . 
+00013470: 2020 2020 2020 2020 2020 2070 656e 616c             penal
+00013480: 7479 202b 3d20 2865 6461 7461 2e6d 6172  ty += (edata.mar
+00013490: 6769 6e28 622c 2061 2920 2a2a 2065 7870  gin(b, a) ** exp
+000134a0: 290a 2020 2020 2020 2020 656c 6966 2065  ).        elif e
+000134b0: 6461 7461 2e6d 616a 6f72 6974 795f 7072  data.majority_pr
+000134c0: 6566 6572 7328 612c 2062 2920 616e 6420  efers(a, b) and 
+000134d0: 2861 2c62 2920 6e6f 7420 696e 2072 656c  (a,b) not in rel
+000134e0: 2061 6e64 2028 622c 6129 206e 6f74 2069   and (b,a) not i
+000134f0: 6e20 7265 6c3a 200a 2020 2020 2020 2020  n rel: .        
+00013500: 2020 2020 7065 6e61 6c74 7920 2b3d 2028      penalty += (
+00013510: 6564 6174 612e 6d61 7267 696e 2861 2c20  edata.margin(a, 
+00013520: 6229 202a 2a20 6578 7029 202f 2032 200a  b) ** exp) / 2 .
+00013530: 2020 2020 2020 2020 656c 6966 2065 6461          elif eda
+00013540: 7461 2e6d 616a 6f72 6974 795f 7072 6566  ta.majority_pref
+00013550: 6572 7328 622c 2061 2920 616e 6420 2861  ers(b, a) and (a
+00013560: 2c62 2920 6e6f 7420 696e 2072 656c 2061  ,b) not in rel a
+00013570: 6e64 2028 622c 6129 206e 6f74 2069 6e20  nd (b,a) not in 
+00013580: 7265 6c3a 200a 2020 2020 2020 2020 2020  rel: .          
+00013590: 2020 7065 6e61 6c74 7920 2b3d 2028 6564    penalty += (ed
+000135a0: 6174 612e 6d61 7267 696e 2862 2c20 6129  ata.margin(b, a)
+000135b0: 202a 2a20 6578 7029 2020 2f20 320a 2020   ** exp)  / 2.  
+000135c0: 2020 7265 7475 726e 2070 656e 616c 7479    return penalty
+000135d0: 0a                                       .
```

### Comparing `pref_voting-1.3.1/pref_voting/margin_based_methods_old.py` & `pref_voting-1.3.2/pref_voting/margin_based_methods_old.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.1/pref_voting/monotonicity_axioms.py` & `pref_voting-1.3.2/pref_voting/monotonicity_axioms.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.1/pref_voting/other_methods.py` & `pref_voting-1.3.2/pref_voting/other_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.1/pref_voting/prob_voting_method.py` & `pref_voting-1.3.2/pref_voting/prob_voting_method.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.1/pref_voting/probabilistic_methods.py` & `pref_voting-1.3.2/pref_voting/probabilistic_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.1/pref_voting/profiles.py` & `pref_voting-1.3.2/pref_voting/profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.1/pref_voting/profiles_with_ties.py` & `pref_voting-1.3.2/pref_voting/profiles_with_ties.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.1/pref_voting/rankings.py` & `pref_voting-1.3.2/pref_voting/rankings.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.1/pref_voting/scoring_methods.py` & `pref_voting-1.3.2/pref_voting/scoring_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.1/pref_voting/social_welfare_function.py` & `pref_voting-1.3.2/pref_voting/social_welfare_function.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.1/pref_voting/spatial_profiles.py` & `pref_voting-1.3.2/pref_voting/spatial_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.1/pref_voting/strategic_axioms.py` & `pref_voting-1.3.2/pref_voting/strategic_axioms.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.1/pref_voting/swf_axioms.py` & `pref_voting-1.3.2/pref_voting/swf_axioms.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.1/pref_voting/tests/conftest.py` & `pref_voting-1.3.2/pref_voting/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.1/pref_voting/tests/test_c1_methods.py` & `pref_voting-1.3.2/pref_voting/tests/test_c1_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.1/pref_voting/tests/test_combined_methods.py` & `pref_voting-1.3.2/pref_voting/tests/test_combined_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.1/pref_voting/tests/test_generate_profiles.py` & `pref_voting-1.3.2/pref_voting/tests/test_generate_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.1/pref_voting/tests/test_generate_spatial_profile.py` & `pref_voting-1.3.2/pref_voting/tests/test_generate_spatial_profile.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.1/pref_voting/tests/test_io.py` & `pref_voting-1.3.2/pref_voting/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.1/pref_voting/tests/test_iterative_methods.py` & `pref_voting-1.3.2/pref_voting/tests/test_iterative_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.1/pref_voting/tests/test_majority_graph.py` & `pref_voting-1.3.2/pref_voting/tests/test_majority_graph.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.1/pref_voting/tests/test_mapping.py` & `pref_voting-1.3.2/pref_voting/tests/test_mapping.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.1/pref_voting/tests/test_margin_based_methods.py` & `pref_voting-1.3.2/pref_voting/tests/test_margin_based_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.1/pref_voting/tests/test_margin_graph.py` & `pref_voting-1.3.2/pref_voting/tests/test_margin_graph.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.1/pref_voting/tests/test_other_methods.py` & `pref_voting-1.3.2/pref_voting/tests/test_other_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.1/pref_voting/tests/test_prob_voting_method.py` & `pref_voting-1.3.2/pref_voting/tests/test_prob_voting_method.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.1/pref_voting/tests/test_profile.py` & `pref_voting-1.3.2/pref_voting/tests/test_profile.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.1/pref_voting/tests/test_profile_with_ties.py` & `pref_voting-1.3.2/pref_voting/tests/test_profile_with_ties.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.1/pref_voting/tests/test_ranking.py` & `pref_voting-1.3.2/pref_voting/tests/test_ranking.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.1/pref_voting/tests/test_scoring_rules.py` & `pref_voting-1.3.2/pref_voting/tests/test_scoring_rules.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.1/pref_voting/tests/test_social_welfare_functions.py` & `pref_voting-1.3.2/pref_voting/tests/test_social_welfare_functions.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.1/pref_voting/tests/test_spatial_profile.py` & `pref_voting-1.3.2/pref_voting/tests/test_spatial_profile.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.1/pref_voting/tests/test_support_graph.py` & `pref_voting-1.3.2/pref_voting/tests/test_support_graph.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.1/pref_voting/tests/test_utility_function.py` & `pref_voting-1.3.2/pref_voting/tests/test_utility_function.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.1/pref_voting/tests/test_utility_functions.py` & `pref_voting-1.3.2/pref_voting/tests/test_utility_functions.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.1/pref_voting/tests/test_voting_method.py` & `pref_voting-1.3.2/pref_voting/tests/test_voting_method.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.1/pref_voting/utility_functions.py` & `pref_voting-1.3.2/pref_voting/utility_functions.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.1/pref_voting/utility_methods.py` & `pref_voting-1.3.2/pref_voting/utility_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.1/pref_voting/utility_profiles.py` & `pref_voting-1.3.2/pref_voting/utility_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.1/pref_voting/variable_candidate_axioms.py` & `pref_voting-1.3.2/pref_voting/variable_candidate_axioms.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.1/pref_voting/variable_voter_axioms.py` & `pref_voting-1.3.2/pref_voting/variable_voter_axioms.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.1/pref_voting/voting_method.py` & `pref_voting-1.3.2/pref_voting/voting_method.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
         
         self.vm = vm
         self.name = name
         self.properties = properties
         self.input_types = input_types
         self.skip_registration = skip_registration
         self.algorithm = None
+        
         functools.update_wrapper(self, vm)   
 
     def __call__(self, edata, curr_cands = None, **kwargs):
         
         if (curr_cands is not None and len(curr_cands) == 0) or len(edata.candidates) == 0: 
             return []
```

### Comparing `pref_voting-1.3.1/pref_voting/voting_method_properties.py` & `pref_voting-1.3.2/pref_voting/voting_method_properties.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.1/pref_voting/voting_methods_registry.py` & `pref_voting-1.3.2/pref_voting/voting_methods_registry.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.1/pref_voting/weighted_majority_graphs.py` & `pref_voting-1.3.2/pref_voting/weighted_majority_graphs.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.1/pyproject.toml` & `pref_voting-1.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "pref_voting"
-version = "1.3.1"
+version = "1.3.2"
 description = "pref_voting is a Python package that contains tools to reason about elections and margin graphs, and implementations of voting methods."
 authors = ["Eric Pacuit <epacuit@umd.edu>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/voting-tools/pref_voting"
 repository = "https://github.com/voting-tools/pref_voting"
```

### Comparing `pref_voting-1.3.1/setup.py` & `pref_voting-1.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'prefsampling>=0.1.16,<0.2.0',
  'random2>=1.0.1,<2.0.0',
  'scipy>=1.0.0,<2.0.0',
  'tabulate>=0.9.0,<0.10.0']
 
 setup_kwargs = {
     'name': 'pref-voting',
-    'version': '1.3.1',
+    'version': '1.3.2',
     'description': 'pref_voting is a Python package that contains tools to reason about elections and margin graphs, and implementations of voting methods.',
     'long_description': 'pref_voting\n==========\n\n## Installation\n\nWith pip package manager:\n\n```bash\npip install pref_voting\n```\n\n## Documentation\n\nOnline documentation is available at [https://pref-voting.readthedocs.io](https://pref-voting.readthedocs.io).\n\n## Example Usage\n\nA profile (of linear orders over the candidates) is created by initializing a `Profile` class object.  Simply provide a list of rankings (each ranking is a tuple of numbers) and a list giving the number of voters with each ranking:\n\n```python\nfrom pref_voting.profiles import Profile\n\nrankings = [\n    (0, 1, 2, 3), \n    (2, 3, 1, 0), \n    (3, 1, 2, 0), \n    (1, 2, 0, 3), \n    (1, 3, 2, 0)]\n\nrcounts = [5, 3, 2, 4, 3]\n\nprof = Profile(rankings, rcounts=rcounts)\n```\n\nThe function `generate_profile` is used to generate a profile for a given number of candidates and voters:  \n\n```python\nfrom pref_voting.generate_profiles import generate_profile\n\n# generate a profile using the Impartial Culture probability model\nprof = generate_profile(3, 4) # prof is a Profile object\n\n# generate a profile using the Impartial Anonymous Culture probability model\nprof = generate_profile(3, 4, probmod = "IAC") # prof is a Profile object \n```\n\nTo use one of the many voting methods, import the function from `pref_voting.voting_methods` and apply it to the profile: \n\n```python\nfrom pref_voting.generate_profiles import generate_profile\nfrom pref_voting.voting_methods import *\n\nprof = generate_profile(3, 4)\nsplit_cycle(prof) # returns the sorted list of winning candidates\nsplit_cycle.display(prof) # display the winning candidates\n\n```\n\n## Questions?\n\nFeel free to [send an email](https://pacuit.org/) if you have questions about the project.\n\n## License\n\n[MIT](https://github.com/jontingvold/pyrankvote/blob/master/LICENSE.txt)\n',
     'author': 'Eric Pacuit',
     'author_email': 'epacuit@umd.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/voting-tools/pref_voting',
```

### Comparing `pref_voting-1.3.1/PKG-INFO` & `pref_voting-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pref-voting
-Version: 1.3.1
+Version: 1.3.2
 Summary: pref_voting is a Python package that contains tools to reason about elections and margin graphs, and implementations of voting methods.
 Home-page: https://github.com/voting-tools/pref_voting
 License: MIT
 Author: Eric Pacuit
 Author-email: epacuit@umd.edu
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

