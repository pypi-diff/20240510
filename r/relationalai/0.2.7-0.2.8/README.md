# Comparing `tmp/relationalai-0.2.7.tar.gz` & `tmp/relationalai-0.2.8.tar.gz`

## Comparing `relationalai-0.2.7.tar` & `relationalai-0.2.8.tar`

### file list

```diff
@@ -1,515 +1,552 @@
--rw-r--r--   0        0        0     6206 2020-02-02 00:00:00.000000 relationalai-0.2.7/README.md
--rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 relationalai-0.2.7/.github/actions/benchmarks/action.yml
--rw-r--r--   0        0        0     5131 2020-02-02 00:00:00.000000 relationalai-0.2.7/.github/actions/end-to-end/action.yml
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 relationalai-0.2.7/.github/workflows/benchmarks.yml
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 relationalai-0.2.7/.github/workflows/end-to-end.yml
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 relationalai-0.2.7/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 relationalai-0.2.7/.github/workflows/ruff.yml
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/README.md
--rw-r--r--   0        0        0    17779 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/getting_started.md
--rw-r--r--   0        0        0     9875 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/_old/OLD_pyrel_quickstart.md
--rw-r--r--   0        0        0     3956 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/_old/metamodel.md
--rw-r--r--   0        0        0     5935 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/_old/python_dsl.md
--rw-r--r--   0        0        0     9371 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/_old/quickstart.md
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/README.md
--rw-r--r--   0        0        0    13377 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/cli/README.md
--rw-r--r--   0        0        0     7100 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/configuration/README.md
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Expression.md
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Property.md
--rw-r--r--   0        0        0     9593 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/README.md
--rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Context/README.md
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Context/enter__.md
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Context/exit__.md
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Context/iter__.md
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Context/model.md
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Context/results.md
--rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/ContextSelect/README.md
--rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/ContextSelect/add.md
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/ContextSelect/call__.md
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/ContextSelect/getattribute__.md
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Instance/README.md
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Instance/persist.md
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Instance/set.md
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Instance/unpersist.md
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/InstanceProperty/README.md
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/InstanceProperty/or_.md
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Model/README.md
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Model/Type.md
--rw-r--r--   0        0        0     3427 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Model/found.md
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Model/name.md
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Model/not_found.md
--rw-r--r--   0        0        0     5008 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Model/ordered_choice.md
--rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Model/query.md
--rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Model/read.md
--rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Model/rule.md
--rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Model/scope.md
--rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Model/union.md
--rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Producer/README.md
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Producer/add__.md
--rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Producer/enter__.md
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Producer/eq__.md
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Producer/exit__.md
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Producer/floordiv__.md
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Producer/ge__.md
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Producer/getattribute__.md
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Producer/gt__.md
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Producer/le__.md
--rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Producer/lt__.md
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Producer/mul__.md
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Producer/ne__.md
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Producer/pow__.md
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Producer/radd__.md
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Producer/rfloordiv__.md
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Producer/rmul__.md
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Producer/rpow__.md
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Producer/rsub__.md
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Producer/rtruediv__.md
--rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Producer/sub__.md
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Producer/truediv__.md
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Type/README.md
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Type/add.md
--rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Type/call__.md
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Type/extend.md
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Type/model.md
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Type/name.md
--rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/Type/or__.md
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/clients/README.md
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/clients/snowflake/PrimaryKey.md
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/clients/snowflake/README.md
--rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/clients/snowflake/Snowflake.md
--rw-r--r--   0        0        0     2588 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/clients/snowflake/SnowflakeTable/README.md
--rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/clients/snowflake/SnowflakeTable/describe.md
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/clients/snowflake/SnowflakeTable/fqname.md
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/clients/snowflake/SnowflakeTable/namespace.md
--rw-r--r--   0        0        0     5595 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/README.md
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/Vars.md
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/alias.md
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/aggregates/README.md
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/aggregates/avg.md
--rw-r--r--   0        0        0     2994 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/aggregates/count.md
--rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/aggregates/max.md
--rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/aggregates/min.md
--rw-r--r--   0        0        0     3303 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/aggregates/rank_asc.md
--rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/aggregates/rank_desc.md
--rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/aggregates/sum.md
--rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/README.md
--rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/README.md
--rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/adamic_adar.md
--rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/avg_degree.md
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/avg_indegree.md
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/avg_outdegree.md
--rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/betweeness_centrality.md
--rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/common_neighbor.md
--rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/cosine_similarity.md
--rw-r--r--   0        0        0     2349 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/degree.md
--rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/degree_centrality.md
--rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/diameter_range.md
--rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/distance.md
--rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/eigenvector_centrality.md
--rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/indegree.md
--rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/infomap.md
--rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/is_connected.md
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/is_reachable.md
--rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/is_triangle.md
--rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/jaccard_similarity.md
--rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/label_propagation.md
--rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/louvain.md
--rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/max_degree.md
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/max_indegree.md
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/max_outdegree.md
--rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/min_degree.md
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/min_indegree.md
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/min_outdegree.md
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/num_edges.md
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/num_nodes.md
--rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/num_triangles.md
--rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/outdegree.md
--rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/pagerank.md
--rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/preferential_attachment.md
--rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/reachable_from.md
--rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/triangles.md
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/weakly_connected_component.md
--rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/weighted_cosine_similarity.md
--rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/weighted_degree_centrality.md
--rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/weighted_distance.md
--rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/weighted_jaccard_similarity.md
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Edge/README.md
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Edge/add.md
--rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Edge/call__.md
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Edge/extend.md
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/EdgeInstance/README.md
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/EdgeInstance/from_.md
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/EdgeInstance/set.md
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/EdgeInstance/to.md
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Graph/Edge.md
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Graph/Node.md
--rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Graph/README.md
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Graph/compute.md
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Graph/fetch.md
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Graph/id.md
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Graph/model.md
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Graph/undirected.md
--rw-r--r--   0        0        0     4167 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Graph/visualize.md
--rw-r--r--   0        0        0    20679 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Graph/img/graph-viz-with-labels-and-colors.png
--rw-r--r--   0        0        0    15558 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Graph/img/graph-viz.png
--rw-r--r--   0        0        0    14921 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/graphs/Graph/img/simple-social-network.png
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/math/README.md
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/math/abs.md
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/math/cbrt.md
--rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/math/ceil.md
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/math/floor.md
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/math/isclose.md
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/math/log.md
--rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/math/sign.md
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/math/sqrt.md
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/math/trunc_divide.md
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/strings/README.md
--rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/strings/concat.md
--rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/strings/contains.md
--rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/strings/ends_with.md
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/strings/join.md
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/strings/length.md
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/strings/like.md
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/strings/lowercase.md
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/strings/regex_compile.md
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/strings/regex_match.md
--rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/strings/replace.md
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/strings/split.md
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/strings/split_part.md
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/python/std/strings/uppercase.md
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/api_reference/sql/README.md
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/faq/README.md
--rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/faq/engines.md
--rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/README.md
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/cdc.py
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/custom_snowflake_connection.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/emit_playground.py
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/found.py
--rw-r--r--   0        0        0     6699 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/fraud.ipynb
--rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/fraud.py
--rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/graph_algos.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/load_raw.py
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/nested.py
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/or_types.py
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/remote_load_csv.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/requirements.txt
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/simple.py
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/simple_recursion.py
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/simple_streamlit.py
--rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/solver.py
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/weighted_graph_algos.py
--rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/articles_graph/README.md
--rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/articles_graph/articles_graph.py
--rw-r--r--   0        0        0     5257 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/articles_graph/articles_graph_with_nlp.py
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/articles_graph/pyproject.toml
--rw-r--r--   0        0        0     3399 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/articles_graph/utils.py
--rw-r--r--   0        0        0  1274296 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/articles_graph/daily_articles/04_04_2024.json
--rw-r--r--   0        0        0     4740 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/data/people.csv
--rw-r--r--   0        0        0    10518 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/data/transactions.csv
--rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/ev_penetration/ev_penetration.py
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/ev_penetration/ev_penetration_csv.py
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/ev_penetration/state_stats.csv
--rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/imdb/README.md
--rw-r--r--   0        0        0   787694 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/imdb/imdb.csv
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/imdb/imdb.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/rel/bar.rel
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/rel/foo.rel
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/rel/solver.rel
--rw-r--r--   0        0        0     6174 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/social-money-network/SF_pagerank.ipynb
--rw-r--r--   0        0        0  2419367 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/social-money-network/Simulation-and-SF-Upload.ipynb
--rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 relationalai-0.2.7/examples/social-money-network/snowflake_pagerank.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/.gitignore
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/README.md
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/index.html
--rw-r--r--   0        0        0   463836 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/package-lock.json
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/package.json
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/tsconfig.json
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/vite.config.ts
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/.storybook/main.ts
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/.storybook/preview-body.html
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/.storybook/preview-head.html
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/.storybook/preview.ts
--rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/App.styl
--rw-r--r--   0        0        0     5857 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/App.tsx
--rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/Selection.tsx
--rw-r--r--   0        0        0    11330 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/debugger_client.ts
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/index.css
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/index.tsx
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/logo.svg
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/util.styl
--rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/util.ts
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/ws.ts
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/assets/favicon.png
--rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/EventList.styl
--rw-r--r--   0        0        0     7570 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/EventList.tsx
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/EventViewer.styl
--rw-r--r--   0        0        0     5165 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/EventViewer.tsx
--rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/Sidebar.styl
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/Sidebar.tsx
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/Schematic/NodeIcon.stories.tsx
--rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/Schematic/ScopeProvider.tsx
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/Schematic/index.stories.tsx
--rw-r--r--   0        0        0     4742 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/Schematic/index.styl
--rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/Schematic/index.tsx
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/Schematic/nodes/CallNode.tsx
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/Schematic/nodes/ComputeNode.tsx
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/Schematic/nodes/EffectNode.tsx
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/Schematic/nodes/FilterNode.tsx
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/Schematic/nodes/GetNode.tsx
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/Schematic/nodes/QuantifyNode.tsx
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/Schematic/nodes/ReturnNode.tsx
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/Schematic/nodes/SequenceNode.tsx
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/Schematic/nodes/UnionNode.tsx
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/Schematic/nodes/UnknownNode.tsx
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/Schematic/nodes/base.styl
--rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/Schematic/nodes/base.tsx
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/Schematic/nodes/index.tsx
--rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/ui/Accordion.stories.tsx
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/ui/Accordion.styl
--rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/ui/Accordion.tsx
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/ui/Breadcrumbs.stories.tsx
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/ui/Breadcrumbs.styl
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/ui/Breadcrumbs.tsx
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/ui/Button.styl
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/ui/Button.tsx
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/ui/Code.styl
--rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/ui/Code.tsx
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/ui/Collapsible.stories.tsx
--rw-r--r--   0        0        0     4217 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/ui/Collapsible.styl
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/ui/Collapsible.tsx
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/ui/Field.stories.tsx
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/ui/Field.styl
--rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/ui/Field.tsx
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/ui/Icon.styl
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/ui/Icon.tsx
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/ui/Modal.stories.tsx
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/ui/Modal.styl
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/ui/Modal.tsx
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/ui/Tooltip.stories.tsx
--rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/ui/Tooltip.styl
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/components/ui/Tooltip.tsx
--rw-r--r--   0        0        0     4529 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/fixtures/branch-improved.json
--rw-r--r--   0        0        0     5229 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/fixtures/branch.json
--rw-r--r--   0        0        0    67308 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/fixtures/fraud.json
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/fixtures/index.ts
--rw-r--r--   0        0        0     9536 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/fixtures/not_found.json
--rw-r--r--   0        0        0     6685 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/fixtures/simple.json
--rw-r--r--   0        0        0     6271 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/fixtures/union.json
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/types/json.d.ts
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/types/jsx.d.ts
--rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 relationalai-0.2.7/frontend/debugger/src/types/mech.d.ts
--rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/gentest/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/gentest/__init__.py
--rw-r--r--   0        0        0    12329 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/gentest/emit.py
--rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/gentest/exec.py
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/gentest/fixtures.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/gentest/patch.py
--rw-r--r--   0        0        0     7629 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/gentest/util.py
--rwxr-xr-x   0        0        0     3521 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/gentest/cli/__main__.py
--rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/gentest/cli/collect_failures.py
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/gentest/cli/collect_tests.py
--rw-r--r--   0        0        0     5707 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/gentest/cli/repro.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/gentest/cli/run_tests.py
--rw-r--r--   0        0        0    15710 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/gentest/cli/watch.py
--rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/gentest/gen/action.py
--rw-r--r--   0        0        0     5461 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/gentest/gen/context.py
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/gentest/gen/document.py
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/gentest/gen/error.py
--rw-r--r--   0        0        0     6095 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/gentest/gen/group_limited.py
--rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/gentest/gen/ir.py
--rw-r--r--   0        0        0    17029 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/gentest/gen/scope.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/gentest/gen/staged.py
--rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/gentest/gen/task.py
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/gentest/gen/test.py
--rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/gentest/harness/database.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/gentest/harness/vendor_types.py
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/gentest/validate/diff.py
--rw-r--r--   0        0        0     5588 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/gentest/validate/errors.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/gentest/validate/mapping.py
--rw-r--r--   0        0        0     5426 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/gentest/validate/roundtrip.py
--rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/__init__.py
--rw-r--r--   0        0        0     6310 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/compiler.py
--rw-r--r--   0        0        0    11634 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/debugging.py
--rw-r--r--   0        0        0    46572 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/dsl.py
--rw-r--r--   0        0        0    15741 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/errors.py
--rw-r--r--   0        0        0    26752 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/metagen.py
--rw-r--r--   0        0        0    27989 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/metamodel.py
--rw-r--r--   0        0        0    19780 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/rel.py
--rw-r--r--   0        0        0    20453 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/rel2.py
--rw-r--r--   0        0        0    13261 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/rel_emitter.py
--rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/rel_utils.py
--rw-r--r--   0        0        0     8570 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/analysis/mechanistic.py
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/analysis/whynot.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/clients/__init__.py
--rw-r--r--   0        0        0    10830 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/clients/azure.py
--rw-r--r--   0        0        0    11891 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/clients/client.py
--rw-r--r--   0        0        0    18211 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/clients/config.py
--rw-r--r--   0        0        0    37604 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/clients/snowflake.py
--rw-r--r--   0        0        0     5526 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/clients/test.py
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/clients/types.py
--rw-r--r--   0        0        0     7349 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/loaders/csv.py
--rw-r--r--   0        0        0     7140 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/loaders/loader.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/loaders/types.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/std/__init__.py
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/std/aggregates.py
--rw-r--r--   0        0        0    18717 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/std/graphs.py
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/std/math.py
--rw-r--r--   0        0        0     2785 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/std/strings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/tools/__init__.py
--rw-r--r--   0        0        0    54404 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/tools/cli.py
--rw-r--r--   0        0        0    12721 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/tools/cli_controls.py
--rw-r--r--   0        0        0     6858 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/tools/debugger.py
--rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/tools/debugger_server.py
--rw-r--r--   0        0        0     9121 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/tools/dev.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/tools/notes
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/util/keys.py
--rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/util/snowflake_logger.py
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 relationalai-0.2.7/src/relationalai/util/tracing_logger.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/__init__.py
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/conftest.py
--rw-r--r--   0        0        0     5346 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/util.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/benchmarks/conftest.py
--rw-r--r--   0        0        0     4603 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/benchmarks/test_tastybytes.py
--rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/README.md
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/conftest.py
--rw-r--r--   0        0        0     8024 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/test_graph_visualize.py
--rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/test_snapshots.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/after_errors/query0.txt
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/after_errors/query1.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/agg_ordering/query0.txt
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/bool/query0.txt
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/bool/query1.txt
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/bottom/query0.txt
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/first/query0.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__basics/query0.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__basics/query1.txt
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query0.txt
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query1.txt
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query2.txt
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query3.txt
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query4.txt
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query0.txt
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query1.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query2.txt
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query3.txt
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query4.txt
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__connectivity/query0.txt
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__connectivity/query1.txt
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__connectivity/query2.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query0.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query1.txt
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query10.txt
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query11.txt
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query2.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query3.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query4.txt
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query5.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query6.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query7.txt
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query8.txt
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query9.txt
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__distance/query0.txt
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__distance/query1.txt
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__distance/query2.txt
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__link_prediction/query0.txt
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__link_prediction/query1.txt
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__link_prediction/query2.txt
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__similarity/query0.txt
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__similarity/query1.txt
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__similarity/query2.txt
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__similarity/query3.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__triangles/query0.txt
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__triangles/query1.txt
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__triangles/query2.txt
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__triangles/query3.txt
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__triangles/query4.txt
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query0.txt
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query1.txt
--rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query2.txt
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query3.txt
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query4.txt
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/not_found/query0.txt
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/not_found/query1.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query0.txt
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query1.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query2.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query3.txt
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/smoke/query0.txt
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/smoke/query1.txt
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query0.txt
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query1.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query2.txt
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query3.txt
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query4.txt
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query5.txt
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query6.txt
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query7.txt
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query8.txt
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query9.txt
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query0.txt
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query1.txt
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query10.txt
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query2.txt
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query3.txt
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query4.txt
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query5.txt
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query6.txt
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query7.txt
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query8.txt
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query9.txt
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/top/query0.txt
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/union/query0.txt
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query0.txt
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query1.txt
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query2.txt
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query3.txt
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query4.txt
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query5.txt
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/test_cases/after_errors.py
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/test_cases/agg_ordering.py
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/test_cases/bool.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/test_cases/bottom.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/test_cases/export.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/test_cases/first.py
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/test_cases/multi_valued.py
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/test_cases/not_found.py
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/test_cases/out_of_context.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/test_cases/persist.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/test_cases/smoke.py
--rw-r--r--   0        0        0     2554 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/test_cases/std_math.py
--rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/test_cases/strings.py
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/test_cases/top.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/test_cases/union.py
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/test_cases/weighted_graphs.py
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/test_cases/graphs/basics.py
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/test_cases/graphs/centrality.py
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/test_cases/graphs/community.py
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/test_cases/graphs/connectivity.py
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/test_cases/graphs/degree.py
--rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/test_cases/graphs/distance.py
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/test_cases/graphs/link_prediction.py
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/test_cases/graphs/similarity.py
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/end2end/test_cases/graphs/triangles.py
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/execution/test_core.py
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/execution/test_examples.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/execution/basic/smoketest.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/execution/snapshots/test_core/test_basic/smoketest/query0.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/execution/snapshots/test_examples/test_example/emit_playground/query0.txt
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/execution/snapshots/test_examples/test_example/found/query0.txt
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/execution/snapshots/test_examples/test_example/graph/query0.txt
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/execution/snapshots/test_examples/test_example/graph/query1.txt
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/execution/snapshots/test_examples/test_example/load_raw/query0.txt
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/execution/snapshots/test_examples/test_example/or_types/query0.txt
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/execution/snapshots/test_examples/test_example/simple/query0.txt
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/execution/snapshots/test_examples/test_example/simple_recursion/query0.txt
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/execution/snapshots/test_examples/test_example/simple_streamlit/query0.txt
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/execution/snapshots/test_examples/test_example/test/query0.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/init-cli/__init__.py
--rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/init-cli/azure_basic.py
--rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/init-cli/common.py
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/roundtrip/test_document.py
--rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 relationalai-0.2.7/tests/roundtrip/test_task.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 relationalai-0.2.7/.gitignore
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 relationalai-0.2.7/pyproject.toml
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 relationalai-0.2.7/docs/pypi/README.md
--rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 relationalai-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     6206 2020-02-02 00:00:00.000000 relationalai-0.2.8/README.md
+-rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 relationalai-0.2.8/.github/actions/benchmarks/action.yml
+-rw-r--r--   0        0        0     5131 2020-02-02 00:00:00.000000 relationalai-0.2.8/.github/actions/end-to-end/action.yml
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 relationalai-0.2.8/.github/workflows/benchmarks.yml
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 relationalai-0.2.8/.github/workflows/end-to-end.yml
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 relationalai-0.2.8/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 relationalai-0.2.8/.github/workflows/ruff.yml
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/README.md
+-rw-r--r--   0        0        0    17779 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/getting_started.md
+-rw-r--r--   0        0        0     9875 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/_old/OLD_pyrel_quickstart.md
+-rw-r--r--   0        0        0     3956 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/_old/metamodel.md
+-rw-r--r--   0        0        0     5935 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/_old/python_dsl.md
+-rw-r--r--   0        0        0     9371 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/_old/quickstart.md
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/README.md
+-rw-r--r--   0        0        0    13377 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/cli/README.md
+-rw-r--r--   0        0        0     7095 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/configuration/README.md
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Expression.md
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Property.md
+-rw-r--r--   0        0        0    10044 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/README.md
+-rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Context/README.md
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Context/enter__.md
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Context/exit__.md
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Context/iter__.md
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Context/model.md
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Context/results.md
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/ContextSelect/README.md
+-rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/ContextSelect/add.md
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/ContextSelect/call__.md
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/ContextSelect/getattribute__.md
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Instance/README.md
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Instance/persist.md
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Instance/set.md
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Instance/unpersist.md
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/InstanceProperty/README.md
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/InstanceProperty/or_.md
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Model/README.md
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Model/Type.md
+-rw-r--r--   0        0        0     3427 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Model/found.md
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Model/name.md
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Model/not_found.md
+-rw-r--r--   0        0        0     5008 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Model/ordered_choice.md
+-rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Model/query.md
+-rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Model/read.md
+-rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Model/rule.md
+-rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Model/scope.md
+-rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Model/union.md
+-rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Producer/README.md
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Producer/add__.md
+-rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Producer/enter__.md
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Producer/eq__.md
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Producer/exit__.md
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Producer/floordiv__.md
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Producer/ge__.md
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Producer/getattribute__.md
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Producer/gt__.md
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Producer/le__.md
+-rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Producer/lt__.md
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Producer/mul__.md
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Producer/ne__.md
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Producer/pow__.md
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Producer/radd__.md
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Producer/rfloordiv__.md
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Producer/rmul__.md
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Producer/rpow__.md
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Producer/rsub__.md
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Producer/rtruediv__.md
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Producer/sub__.md
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Producer/truediv__.md
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Type/README.md
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Type/add.md
+-rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Type/call__.md
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Type/extend.md
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Type/model.md
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Type/name.md
+-rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Type/or__.md
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/clients/README.md
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/clients/snowflake/PrimaryKey.md
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/clients/snowflake/README.md
+-rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/clients/snowflake/Snowflake.md
+-rw-r--r--   0        0        0     2588 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/clients/snowflake/SnowflakeTable/README.md
+-rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/clients/snowflake/SnowflakeTable/describe.md
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/clients/snowflake/SnowflakeTable/fqname.md
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/clients/snowflake/SnowflakeTable/namespace.md
+-rw-r--r--   0        0        0     6011 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/README.md
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/Vars.md
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/alias.md
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/aggregates/README.md
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/aggregates/avg.md
+-rw-r--r--   0        0        0     2994 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/aggregates/count.md
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/aggregates/max.md
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/aggregates/min.md
+-rw-r--r--   0        0        0     3303 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/aggregates/rank_asc.md
+-rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/aggregates/rank_desc.md
+-rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/aggregates/sum.md
+-rw-r--r--   0        0        0     3812 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/README.md
+-rw-r--r--   0        0        0     3503 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/README.md
+-rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/adamic_adar.md
+-rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/average_clustering_coefficient.md
+-rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/avg_degree.md
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/avg_indegree.md
+-rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/avg_outdegree.md
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/betweeness_centrality.md
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/common_neighbor.md
+-rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/cosine_similarity.md
+-rw-r--r--   0        0        0     2349 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/degree.md
+-rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/degree_centrality.md
+-rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/diameter_range.md
+-rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/distance.md
+-rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/eigenvector_centrality.md
+-rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/indegree.md
+-rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/infomap.md
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/is_connected.md
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/is_reachable.md
+-rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/is_triangle.md
+-rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/jaccard_similarity.md
+-rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/label_propagation.md
+-rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/local_lustering_coefficient.md
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/louvain.md
+-rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/max_degree.md
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/max_indegree.md
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/max_outdegree.md
+-rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/min_degree.md
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/min_indegree.md
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/min_outdegree.md
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/num_edges.md
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/num_nodes.md
+-rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/num_triangles.md
+-rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/outdegree.md
+-rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/pagerank.md
+-rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/preferential_attachment.md
+-rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/reachable_from.md
+-rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/triangles.md
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/weakly_connected_component.md
+-rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/weighted_cosine_similarity.md
+-rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/weighted_degree_centrality.md
+-rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/weighted_distance.md
+-rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/weighted_jaccard_similarity.md
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Edge/README.md
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Edge/add.md
+-rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Edge/call__.md
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Edge/extend.md
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/EdgeInstance/README.md
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/EdgeInstance/from_.md
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/EdgeInstance/set.md
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/EdgeInstance/to.md
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Graph/Edge.md
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Graph/Node.md
+-rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Graph/README.md
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Graph/compute.md
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Graph/fetch.md
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Graph/id.md
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Graph/model.md
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Graph/undirected.md
+-rw-r--r--   0        0        0     4167 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Graph/visualize.md
+-rw-r--r--   0        0        0    20679 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Graph/img/graph-viz-with-labels-and-colors.png
+-rw-r--r--   0        0        0    15558 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Graph/img/graph-viz.png
+-rw-r--r--   0        0        0    14921 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Graph/img/simple-social-network.png
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/math/README.md
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/math/abs.md
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/math/acos.md
+-rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/math/asin.md
+-rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/math/atan.md
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/math/cbrt.md
+-rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/math/ceil.md
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/math/cos.md
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/math/degrees.md
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/math/floor.md
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/math/isclose.md
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/math/log.md
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/math/radians.md
+-rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/math/sign.md
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/math/sin.md
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/math/sqrt.md
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/math/tan.md
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/math/trunc_divide.md
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/strings/README.md
+-rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/strings/concat.md
+-rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/strings/contains.md
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/strings/ends_with.md
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/strings/join.md
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/strings/length.md
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/strings/like.md
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/strings/lowercase.md
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/strings/regex_compile.md
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/strings/regex_match.md
+-rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/strings/replace.md
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/strings/split.md
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/strings/split_part.md
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/strings/uppercase.md
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/sql/README.md
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/faq/README.md
+-rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/faq/engines.md
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/README.md
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/cdc.py
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/custom_snowflake_connection.py
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/emit_playground.py
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/found.py
+-rw-r--r--   0        0        0     6699 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/fraud.ipynb
+-rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/fraud.py
+-rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/graph_algos.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/load_raw.py
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/nested.py
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/or_types.py
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/remote_load_csv.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/requirements.txt
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/simple.py
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/simple_recursion.py
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/simple_streamlit.py
+-rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/solver.py
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/weighted_graph_algos.py
+-rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/articles_graph/README.md
+-rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/articles_graph/articles_graph.py
+-rw-r--r--   0        0        0     5257 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/articles_graph/articles_graph_with_nlp.py
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/articles_graph/pyproject.toml
+-rw-r--r--   0        0        0     3399 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/articles_graph/utils.py
+-rw-r--r--   0        0        0  1274296 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/articles_graph/daily_articles/04_04_2024.json
+-rw-r--r--   0        0        0     4740 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/data/people.csv
+-rw-r--r--   0        0        0    10518 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/data/transactions.csv
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/ev_penetration/ev_penetration.py
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/ev_penetration/ev_penetration_csv.py
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/ev_penetration/state_stats.csv
+-rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/imdb/README.md
+-rw-r--r--   0        0        0   787694 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/imdb/imdb.csv
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/imdb/imdb.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/rel/bar.rel
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/rel/foo.rel
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/rel/solver.rel
+-rw-r--r--   0        0        0     6174 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/social-money-network/SF_pagerank.ipynb
+-rw-r--r--   0        0        0  2419367 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/social-money-network/Simulation-and-SF-Upload.ipynb
+-rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/social-money-network/snowflake_pagerank.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/.gitignore
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/README.md
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/index.html
+-rw-r--r--   0        0        0   463836 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/package-lock.json
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/package.json
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/tsconfig.json
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/vite.config.ts
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/.storybook/main.ts
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/.storybook/preview-body.html
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/.storybook/preview-head.html
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/.storybook/preview.ts
+-rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/App.styl
+-rw-r--r--   0        0        0     6535 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/App.tsx
+-rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/Selection.tsx
+-rw-r--r--   0        0        0    11656 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/debugger_client.ts
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/index.css
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/index.tsx
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/logo.svg
+-rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/util.styl
+-rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/util.ts
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/ws.ts
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/assets/favicon.png
+-rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/EventList.styl
+-rw-r--r--   0        0        0     7185 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/EventList.tsx
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/EventViewer.styl
+-rw-r--r--   0        0        0     5165 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/EventViewer.tsx
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/FileDropZone.styl
+-rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/FileDropZone.tsx
+-rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/Sidebar.styl
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/Sidebar.tsx
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/Schematic/NodeIcon.stories.tsx
+-rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/Schematic/ScopeProvider.tsx
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/Schematic/index.stories.tsx
+-rw-r--r--   0        0        0     4742 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/Schematic/index.styl
+-rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/Schematic/index.tsx
+-rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/Schematic/nodes/CallNode.tsx
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/Schematic/nodes/ComputeNode.tsx
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/Schematic/nodes/EffectNode.tsx
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/Schematic/nodes/FilterNode.tsx
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/Schematic/nodes/GetNode.tsx
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/Schematic/nodes/QuantifyNode.tsx
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/Schematic/nodes/ReturnNode.tsx
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/Schematic/nodes/SequenceNode.tsx
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/Schematic/nodes/UnionNode.tsx
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/Schematic/nodes/UnknownNode.tsx
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/Schematic/nodes/base.styl
+-rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/Schematic/nodes/base.tsx
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/Schematic/nodes/index.tsx
+-rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/ui/Accordion.stories.tsx
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/ui/Accordion.styl
+-rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/ui/Accordion.tsx
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/ui/Breadcrumbs.stories.tsx
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/ui/Breadcrumbs.styl
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/ui/Breadcrumbs.tsx
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/ui/Button.styl
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/ui/Button.tsx
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/ui/Code.styl
+-rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/ui/Code.tsx
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/ui/Collapsible.stories.tsx
+-rw-r--r--   0        0        0     4220 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/ui/Collapsible.styl
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/ui/Collapsible.tsx
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/ui/Field.stories.tsx
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/ui/Field.styl
+-rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/ui/Field.tsx
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/ui/Icon.styl
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/ui/Icon.tsx
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/ui/Modal.stories.tsx
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/ui/Modal.styl
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/ui/Modal.tsx
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/ui/Tooltip.stories.tsx
+-rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/ui/Tooltip.styl
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/ui/Tooltip.tsx
+-rw-r--r--   0        0        0     4529 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/fixtures/branch-improved.json
+-rw-r--r--   0        0        0     5229 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/fixtures/branch.json
+-rw-r--r--   0        0        0    67308 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/fixtures/fraud.json
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/fixtures/index.ts
+-rw-r--r--   0        0        0     9536 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/fixtures/not_found.json
+-rw-r--r--   0        0        0     6685 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/fixtures/simple.json
+-rw-r--r--   0        0        0     6271 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/fixtures/union.json
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/types/json.d.ts
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/types/jsx.d.ts
+-rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/types/mech.d.ts
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/utils/fileUtils.ts
+-rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/gentest/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/gentest/__init__.py
+-rw-r--r--   0        0        0    12329 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/gentest/emit.py
+-rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/gentest/exec.py
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/gentest/fixtures.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/gentest/patch.py
+-rw-r--r--   0        0        0     7629 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/gentest/util.py
+-rwxr-xr-x   0        0        0     3521 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/gentest/cli/__main__.py
+-rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/gentest/cli/collect_failures.py
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/gentest/cli/collect_tests.py
+-rw-r--r--   0        0        0     5707 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/gentest/cli/repro.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/gentest/cli/run_tests.py
+-rw-r--r--   0        0        0    15710 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/gentest/cli/watch.py
+-rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/gentest/gen/action.py
+-rw-r--r--   0        0        0     5461 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/gentest/gen/context.py
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/gentest/gen/document.py
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/gentest/gen/error.py
+-rw-r--r--   0        0        0     6095 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/gentest/gen/group_limited.py
+-rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/gentest/gen/ir.py
+-rw-r--r--   0        0        0    17029 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/gentest/gen/scope.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/gentest/gen/staged.py
+-rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/gentest/gen/task.py
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/gentest/gen/test.py
+-rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/gentest/harness/database.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/gentest/harness/vendor_types.py
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/gentest/validate/diff.py
+-rw-r--r--   0        0        0     5588 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/gentest/validate/errors.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/gentest/validate/mapping.py
+-rw-r--r--   0        0        0     5426 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/gentest/validate/roundtrip.py
+-rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/__init__.py
+-rw-r--r--   0        0        0     6310 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/compiler.py
+-rw-r--r--   0        0        0    11725 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/debugging.py
+-rw-r--r--   0        0        0    46572 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/dsl.py
+-rw-r--r--   0        0        0    15741 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/errors.py
+-rw-r--r--   0        0        0    26752 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/metagen.py
+-rw-r--r--   0        0        0    27989 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/metamodel.py
+-rw-r--r--   0        0        0    19780 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/rel.py
+-rw-r--r--   0        0        0    20453 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/rel2.py
+-rw-r--r--   0        0        0    13371 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/rel_emitter.py
+-rw-r--r--   0        0        0     3549 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/rel_utils.py
+-rw-r--r--   0        0        0     8570 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/analysis/mechanistic.py
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/analysis/whynot.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/clients/__init__.py
+-rw-r--r--   0        0        0    14725 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/clients/azure.py
+-rw-r--r--   0        0        0    11981 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/clients/client.py
+-rw-r--r--   0        0        0    17625 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/clients/config.py
+-rw-r--r--   0        0        0    39864 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/clients/snowflake.py
+-rw-r--r--   0        0        0     5526 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/clients/test.py
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/clients/types.py
+-rw-r--r--   0        0        0     7529 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/loaders/csv.py
+-rw-r--r--   0        0        0     7140 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/loaders/loader.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/loaders/types.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/std/__init__.py
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/std/aggregates.py
+-rw-r--r--   0        0        0    21043 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/std/graphs.py
+-rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/std/math.py
+-rw-r--r--   0        0        0     2785 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/std/strings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/tools/__init__.py
+-rw-r--r--   0        0        0    59285 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/tools/cli.py
+-rw-r--r--   0        0        0    12721 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/tools/cli_controls.py
+-rw-r--r--   0        0        0     6886 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/tools/debugger.py
+-rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/tools/debugger_client.py
+-rw-r--r--   0        0        0     5341 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/tools/debugger_server.py
+-rw-r--r--   0        0        0     9121 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/tools/dev.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/tools/notes
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/util/constants.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/util/format.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/util/keys.py
+-rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/util/snowflake_logger.py
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/util/tracing_logger.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/__init__.py
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/conftest.py
+-rw-r--r--   0        0        0     5346 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/util.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/benchmarks/conftest.py
+-rw-r--r--   0        0        0     4603 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/benchmarks/test_tastybytes.py
+-rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/README.md
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/conftest.py
+-rw-r--r--   0        0        0     8024 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/test_graph_visualize.py
+-rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/test_snapshots.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/after_errors/query0.txt
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/after_errors/query1.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/agg_ordering/query0.txt
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/bool/query0.txt
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/bool/query1.txt
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/bottom/query0.txt
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/first/query0.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__basics/query0.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__basics/query1.txt
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query0.txt
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query1.txt
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query2.txt
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query3.txt
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query4.txt
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__clustering/query0.txt
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__clustering/query1.txt
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query0.txt
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query1.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query2.txt
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query3.txt
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query4.txt
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__connectivity/query0.txt
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__connectivity/query1.txt
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__connectivity/query2.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query0.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query1.txt
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query10.txt
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query11.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query2.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query3.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query4.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query5.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query6.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query7.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query8.txt
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query9.txt
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__distance/query0.txt
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__distance/query1.txt
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__distance/query2.txt
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__link_prediction/query0.txt
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__link_prediction/query1.txt
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__link_prediction/query2.txt
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__mixed_value_types/query0.txt
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__similarity/query0.txt
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__similarity/query1.txt
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__similarity/query2.txt
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__similarity/query3.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__triangles/query0.txt
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__triangles/query1.txt
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__triangles/query2.txt
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__triangles/query3.txt
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__triangles/query4.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query0.txt
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query1.txt
+-rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query2.txt
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query3.txt
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query4.txt
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/not_found/query0.txt
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/not_found/query1.txt
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/numeric_outputs/query0.txt
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/numeric_outputs/query1.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query0.txt
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query1.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query2.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query3.txt
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/smoke/query0.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/smoke/query1.txt
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query0.txt
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query1.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query10.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query11.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query12.txt
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query13.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query14.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query15.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query16.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query17.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query2.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query3.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query4.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query5.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query6.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query7.txt
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query8.txt
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query9.txt
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query0.txt
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query1.txt
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query10.txt
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query2.txt
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query3.txt
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query4.txt
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query5.txt
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query6.txt
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query7.txt
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query8.txt
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query9.txt
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/top/query0.txt
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/union/query0.txt
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query0.txt
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query1.txt
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query2.txt
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query3.txt
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query4.txt
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query5.txt
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/test_cases/after_errors.py
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/test_cases/agg_ordering.py
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/test_cases/bool.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/test_cases/bottom.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/test_cases/export.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/test_cases/first.py
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/test_cases/multi_valued.py
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/test_cases/not_found.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/test_cases/numeric_outputs.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/test_cases/out_of_context.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/test_cases/persist.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/test_cases/smoke.py
+-rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/test_cases/std_math.py
+-rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/test_cases/strings.py
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/test_cases/top.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/test_cases/union.py
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/test_cases/weighted_graphs.py
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/test_cases/graphs/basics.py
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/test_cases/graphs/centrality.py
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/test_cases/graphs/clustering.py
+-rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/test_cases/graphs/community.py
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/test_cases/graphs/connectivity.py
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/test_cases/graphs/degree.py
+-rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/test_cases/graphs/distance.py
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/test_cases/graphs/link_prediction.py
+-rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/test_cases/graphs/mixed_value_types.py
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/test_cases/graphs/similarity.py
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/test_cases/graphs/triangles.py
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/execution/test_core.py
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/execution/test_examples.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/execution/basic/smoketest.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/execution/snapshots/test_core/test_basic/smoketest/query0.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/execution/snapshots/test_examples/test_example/emit_playground/query0.txt
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/execution/snapshots/test_examples/test_example/found/query0.txt
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/execution/snapshots/test_examples/test_example/graph/query0.txt
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/execution/snapshots/test_examples/test_example/graph/query1.txt
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/execution/snapshots/test_examples/test_example/load_raw/query0.txt
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/execution/snapshots/test_examples/test_example/or_types/query0.txt
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/execution/snapshots/test_examples/test_example/simple/query0.txt
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/execution/snapshots/test_examples/test_example/simple_recursion/query0.txt
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/execution/snapshots/test_examples/test_example/simple_streamlit/query0.txt
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/execution/snapshots/test_examples/test_example/test/query0.txt
+-rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/init-cli/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/init-cli/__init__.py
+-rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/init-cli/azure_basic.py
+-rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/init-cli/common.py
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/roundtrip/test_document.py
+-rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/roundtrip/test_task.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/unit/test_config_store.py
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/unit/test_configs/config_with_new_profile.toml
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/unit/test_configs/printed_config.txt
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/unit/test_configs/raiconfig_example.toml
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 relationalai-0.2.8/.gitignore
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 relationalai-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/pypi/README.md
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 relationalai-0.2.8/PKG-INFO
```

### Comparing `relationalai-0.2.7/README.md` & `relationalai-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/.github/actions/benchmarks/action.yml` & `relationalai-0.2.8/.github/actions/benchmarks/action.yml`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/.github/actions/end-to-end/action.yml` & `relationalai-0.2.8/.github/actions/end-to-end/action.yml`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/.github/workflows/benchmarks.yml` & `relationalai-0.2.8/.github/workflows/benchmarks.yml`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/.github/workflows/end-to-end.yml` & `relationalai-0.2.8/.github/workflows/end-to-end.yml`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/.github/workflows/publish-to-pypi.yml` & `relationalai-0.2.8/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/.github/workflows/ruff.yml` & `relationalai-0.2.8/.github/workflows/ruff.yml`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/getting_started.md` & `relationalai-0.2.8/docs/getting_started.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/_old/OLD_pyrel_quickstart.md` & `relationalai-0.2.8/docs/_old/OLD_pyrel_quickstart.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/_old/metamodel.md` & `relationalai-0.2.8/docs/_old/metamodel.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/_old/python_dsl.md` & `relationalai-0.2.8/docs/_old/python_dsl.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/_old/quickstart.md` & `relationalai-0.2.8/docs/_old/quickstart.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/cli/README.md` & `relationalai-0.2.8/docs/api_reference/cli/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/configuration/README.md` & `relationalai-0.2.8/docs/api_reference/configuration/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -37,29 +37,29 @@
 region = "us-east"
 scheme = "https"
 client_credentials_url = "https://login.relationalai.com/oauth/token"
 client_id = ""
 client_secret = ""
 ```
 
-You can add tables to this file to create multiple profiles. The names of those tables should be prefixed with `profile`. Here's an example showing a profile called `field-team`:
+When you do `rai init`, it will put sets of configuration values in TOML tables that we call *profiles*. Here's an example showing a profile called `field-team`:
 
 ```toml
 [profile.field-team]
 platform = "azure"
 host = "azure.relationalai.com"
 port = 443
 region = "us-east"
 scheme = "https"
 client_credentials_url = "https://login.relationalai.com/oauth/token"
 client_id = ""
 client_secret = ""
 ```
 
-To use specific profile, you can specify the profile name in `rai.Model()` in your, as in `rai.Model(profile="my-other-profile")`. Alternatively, you can assign the `active_profile` key in the `config` table:
+To use specific profile, you can specify the profile name in `rai.Model()` in your Python code, as in `rai.Model(profile="my-other-profile")`. Alternatively, you can assign the `active_profile` key in the `config` table:
 
 ```toml
 active_profile = "field-team"
 
 [profile.field-team]
 platform = "azure"
 host = "azure.relationalai.com"
```

### Comparing `relationalai-0.2.7/docs/api_reference/python/Expression.md` & `relationalai-0.2.8/docs/api_reference/python/Expression.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/Property.md` & `relationalai-0.2.8/docs/api_reference/python/Property.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/README.md` & `relationalai-0.2.8/docs/api_reference/python/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -84,31 +84,32 @@
 - [`aggregates.rank_desc()`](./std/aggregates/rank_desc.md)
 - [`aggregates.sum()`](./std/aggregates/sum.md)
 
 ### [`relationalai.std.graphs`](./std/graphs/README.md)
 
 - [`graphs.Compute`](./std/graphs/Compute/README.md)
   - [`graphs.Compute.adamic_adar()`](./std/graphs/Compute/adamic_adar.md)
+  - [`graphs.Compute.avg_clustering_coefficient()`](./std/graphs/Compute/avg_clustering_coefficient.md)
   - [`graphs.Compute.avg_degree()`](./std/graphs/Compute/avg_degree.md)
   - [`graphs.Compute.avg_indegree()`](./std/graphs/Compute/avg_indegree.md)
   - [`graphs.Compute.avg_outdegree()`](./std/graphs/Compute/avg_outdegree.md)
   - [`graphs.Compute.betweenness_centrality()`](./std/graphs/Compute/betweeness_centrality.md)
   - [`graphs.Compute.cosine_similarity()`](./std/graphs/Compute/cosine_similarity.md)
   - [`graphs.Compute.common_neighbor()`](./std/graphs/Compute/common_neighbor.md)
   - [`graphs.Compute.degree_centrality()`](./std/graphs/Compute/degree_centrality.md)
   - [`graphs.Compute.degree()`](./std/graphs/Compute/degree.md)
   - [`graphs.Compute.diameter_range()`](./std/graphs/Compute/diameter_range.md)
   - [`graphs.Compute.distance()`](./std/graphs/Compute/distance.md)
   - [`graphs.Compute.eigenvector_centrality()`](./std/graphs/Compute/eigenvector_centrality.md)
-  - [`graphs.Compute.num_edges()`](./std/graphs//Compute/num_edges.md)
   - [`graphs.Compute.indegree()`](./std/graphs/Compute/indegree.md)
   - [`graphs.Compute.is_connected()`](./std/graphs/Compute/is_connected.md)
   - [`graphs.Compute.is_reachable()`](./std/graphs/Compute/is_reachable.md)
   - [`graphs.Compute.is_triangle()`](./std/graphs/Compute/is_triangle.md)
   - [`graphs.Compute.label_propagation()`](./std/graphs/Compute/label_propagation.md)
+  - [`graphs.Compute.local_clustering_coefficient()`](./std/graphs/Compute/local_clustering_coefficient.md)
   - [`graphs.Compute.louvain()`](./std/graphs/Compute/louvain.md)
   - [`graphs.Compute.max_degree()`](./std/graphs/Compute/max_degree.md)
   - [`graphs.Compute.max_indegree()`](./std/graphs/Compute/max_indegree.md)
   - [`graphs.Compute.max_outdegree()`](./std/graphs/Compute/max_outdegree.md)
   - [`graphs.Compute.min_degree()`](./std/graphs/Compute/min_degree.md)
   - [`graphs.Compute.min_indegree()`](./std/graphs/Compute/min_indegree.md)
   - [`graphs.Compute.min_outdegree()`](./std/graphs/Compute/min_outdegree.md)
@@ -141,21 +142,29 @@
   - [`graphs.Graph.Node`](./std/graphs/Graph/Node.md)
   - [`graphs.Graph.undirected`](./std/graphs/Graph/undirected.md)
   - [`graphs.Graph.visualize()`](./std/graphs/Graph/visualize.md)
 
 ### [`relationalai.std.math`](./std/math/README.md)
 
 - [`math.abs()`](./std/math/abs.md)
+- [`math.acos()`](./std/math/acos.md)
+- [`math.asin()`](./std/math/asin.md)
+- [`math.atan()`](./std/math/atan.md)
 - [`math.isclose()`](./std/math/isclose.md)
 - [`math.ceil()`](./std/math/ceil.md)
 - [`math.cbrt()`](./std/math/cbrt.md)
+- [`math.cos()`](./std/math/cos.md)
+- [`math.degrees()`](./std/math/degrees.md)
 - [`math.floor()`](./std/math/floor.md)
 - [`math.log()`](./std/math/log.md)
+- [`math.radians()`](./std/math/radians.md)
 - [`math.sign()`](./std/math/sign.md)
+- [`math.sin()`](./std/math/sin.md)
 - [`math.sqrt()`](./std/math/sqrt.md)
+- [`math.tan()`](./std/math/tan.md)
 - [`math.trunc_divide()`](./std/math/trunc_divide.md)
 
 ### [`relationalai.std.strings`](./std/strings/README.md)
 
 - [`strings.concat()`](./std/strings/concat.md)
 - [`strings.contains()`](./std/strings/contains.md)
 - [`strings.ends_with()`](./std/strings/ends_with.md)
```

### Comparing `relationalai-0.2.7/docs/api_reference/python/Context/README.md` & `relationalai-0.2.8/docs/api_reference/python/Context/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/Context/enter__.md` & `relationalai-0.2.8/docs/api_reference/python/Context/enter__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/Context/exit__.md` & `relationalai-0.2.8/docs/api_reference/python/Context/exit__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/Context/iter__.md` & `relationalai-0.2.8/docs/api_reference/python/Context/iter__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/Context/model.md` & `relationalai-0.2.8/docs/api_reference/python/Context/model.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/Context/results.md` & `relationalai-0.2.8/docs/api_reference/python/Context/results.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/ContextSelect/README.md` & `relationalai-0.2.8/docs/api_reference/python/ContextSelect/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/ContextSelect/add.md` & `relationalai-0.2.8/docs/api_reference/python/ContextSelect/add.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/ContextSelect/call__.md` & `relationalai-0.2.8/docs/api_reference/python/ContextSelect/call__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/ContextSelect/getattribute__.md` & `relationalai-0.2.8/docs/api_reference/python/ContextSelect/getattribute__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/Instance/README.md` & `relationalai-0.2.8/docs/api_reference/python/Instance/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/Instance/persist.md` & `relationalai-0.2.8/docs/api_reference/python/Instance/persist.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/Instance/set.md` & `relationalai-0.2.8/docs/api_reference/python/Instance/set.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/Instance/unpersist.md` & `relationalai-0.2.8/docs/api_reference/python/Instance/unpersist.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/InstanceProperty/README.md` & `relationalai-0.2.8/docs/api_reference/python/InstanceProperty/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/InstanceProperty/or_.md` & `relationalai-0.2.8/docs/api_reference/python/InstanceProperty/or_.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/Model/README.md` & `relationalai-0.2.8/docs/api_reference/python/Model/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/Model/Type.md` & `relationalai-0.2.8/docs/api_reference/python/Model/Type.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/Model/found.md` & `relationalai-0.2.8/docs/api_reference/python/Model/found.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/Model/not_found.md` & `relationalai-0.2.8/docs/api_reference/python/Model/not_found.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/Model/ordered_choice.md` & `relationalai-0.2.8/docs/api_reference/python/Model/ordered_choice.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/Model/query.md` & `relationalai-0.2.8/docs/api_reference/python/Model/query.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/Model/read.md` & `relationalai-0.2.8/docs/api_reference/python/Model/read.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/Model/rule.md` & `relationalai-0.2.8/docs/api_reference/python/Model/rule.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/Model/scope.md` & `relationalai-0.2.8/docs/api_reference/python/Model/scope.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/Model/union.md` & `relationalai-0.2.8/docs/api_reference/python/Model/union.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/Producer/README.md` & `relationalai-0.2.8/docs/api_reference/python/Producer/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/Producer/add__.md` & `relationalai-0.2.8/docs/api_reference/python/Producer/add__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/Producer/enter__.md` & `relationalai-0.2.8/docs/api_reference/python/Producer/enter__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/Producer/eq__.md` & `relationalai-0.2.8/docs/api_reference/python/Producer/eq__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/Producer/exit__.md` & `relationalai-0.2.8/docs/api_reference/python/Producer/exit__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/Producer/floordiv__.md` & `relationalai-0.2.8/docs/api_reference/python/Producer/floordiv__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/Producer/ge__.md` & `relationalai-0.2.8/docs/api_reference/python/Producer/ge__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/Producer/getattribute__.md` & `relationalai-0.2.8/docs/api_reference/python/Producer/getattribute__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/Producer/gt__.md` & `relationalai-0.2.8/docs/api_reference/python/Producer/gt__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/Producer/le__.md` & `relationalai-0.2.8/docs/api_reference/python/Producer/le__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/Producer/lt__.md` & `relationalai-0.2.8/docs/api_reference/python/Producer/lt__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/Producer/mul__.md` & `relationalai-0.2.8/docs/api_reference/python/Producer/mul__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/Producer/ne__.md` & `relationalai-0.2.8/docs/api_reference/python/Producer/ne__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/Producer/pow__.md` & `relationalai-0.2.8/docs/api_reference/python/Producer/pow__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/Producer/sub__.md` & `relationalai-0.2.8/docs/api_reference/python/Producer/sub__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/Producer/truediv__.md` & `relationalai-0.2.8/docs/api_reference/python/Producer/truediv__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/Type/README.md` & `relationalai-0.2.8/docs/api_reference/python/Type/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/Type/add.md` & `relationalai-0.2.8/docs/api_reference/python/Type/add.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/Type/call__.md` & `relationalai-0.2.8/docs/api_reference/python/Type/call__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/Type/extend.md` & `relationalai-0.2.8/docs/api_reference/python/Type/extend.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/Type/or__.md` & `relationalai-0.2.8/docs/api_reference/python/Type/or__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/clients/README.md` & `relationalai-0.2.8/docs/api_reference/python/clients/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/clients/snowflake/PrimaryKey.md` & `relationalai-0.2.8/docs/api_reference/python/clients/snowflake/PrimaryKey.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/clients/snowflake/README.md` & `relationalai-0.2.8/docs/api_reference/python/clients/snowflake/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/clients/snowflake/Snowflake.md` & `relationalai-0.2.8/docs/api_reference/python/clients/snowflake/Snowflake.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/clients/snowflake/SnowflakeTable/README.md` & `relationalai-0.2.8/docs/api_reference/python/clients/snowflake/SnowflakeTable/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/clients/snowflake/SnowflakeTable/describe.md` & `relationalai-0.2.8/docs/api_reference/python/clients/snowflake/SnowflakeTable/describe.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/clients/snowflake/SnowflakeTable/fqname.md` & `relationalai-0.2.8/docs/api_reference/python/clients/snowflake/SnowflakeTable/fqname.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/clients/snowflake/SnowflakeTable/namespace.md` & `relationalai-0.2.8/docs/api_reference/python/clients/snowflake/SnowflakeTable/namespace.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/README.md` & `relationalai-0.2.8/docs/api_reference/python/std/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 - [`aggregates.rank_desc()`](./aggregates/rank_desc.md)
 - [`aggregates.sum()`](./aggregates/sum.md)
 
 ## [`relationalai.std.graphs`](./graphs/README.md)
 
 - [`graphs.Compute`](./graphs/Compute/README.md)
   - [`graphs.Compute.adamic_adar()`](./graphs/Compute/adamic_adar.md)
+  - [`graphs.Compute.avg_clustering_coefficient()`](./graphs/Compute/avg_clustering_coefficient.md)
   - [`graphs.Compute.avg_degree()`](./graphs/Compute/avg_degree.md)
   - [`graphs.Compute.avg_indegree()`](./graphs/Compute/avg_indegree.md)
   - [`graphs.Compute.avg_outdegree()`](./graphs/Compute/avg_outdegree.md)
   - [`graphs.Compute.betweenness_centrality()`](./graphs/Compute/betweeness_centrality.md)
   - [`graphs.Compute.common_neighbor()`](./graphs/Compute/common_neighbor.md)
   - [`graphs.Compute.cosine_similarity()`](./graphs/Compute/cosine_similarity.md)
   - [`graphs.Compute.common_neighbor()`](./graphs/Compute/common_neighbor.md)
@@ -30,17 +31,17 @@
   - [`graphs.Compute.degree()`](./graphs/Compute/degree.md)
   - [`graphs.Compute.diameter_range()`](./graphs/Compute/diameter_range.md)
   - [`graphs.Compute.distance()`](./graphs/Compute/distance.md)
   - [`graphs.Compute.eigenvector_centrality()`](./graphs/Compute/eigenvector_centrality.md)
   - [`graphs.Compute.is_connected()`](./graphs/Compute/is_connected.md)
   - [`graphs.Compute.is_reachable()`](./graphs/Compute/is_reachable.md)
   - [`graphs.Compute.is_triangle()`](./graphs/Compute/is_triangle.md)
-  - [`graphs.Compute.num_edges()`](./graphs/Compute/num_edges.md)
   - [`graphs.Compute.indegree()`](./graphs/Compute/indegree.md)
   - [`graphs.Compute.label_propagation()`](./graphs/Compute/label_propagation.md)
+  - [`graphs.Compute.local_clustering_coefficient()`](./graphs/Compute/local_clustering_coefficient.md)
   - [`graphs.Compute.louvain()`](./graphs/Compute/louvain.md)
   - [`graphs.Compute.max_degree()`](./graphs/Compute/max_degree.md)
   - [`graphs.Compute.max_indegree()`](./graphs/Compute/max_indegree.md)
   - [`graphs.Compute.max_outdegree()`](./graphs/Compute/max_outdegree.md)
   - [`graphs.Compute.min_degree()`](./graphs/Compute/min_degree.md)
   - [`graphs.Compute.min_indegree()`](./graphs/Compute/min_indegree.md)
   - [`graphs.Compute.min_outdegree()`](./graphs/Compute/min_outdegree.md)
@@ -74,21 +75,29 @@
   - [`graphs.Graph.Node`](./graphs/Graph/Node.md)
   - [`graphs.Graph.undirected`](./graphs/Graph/undirected.md)
   - [`graphs.Graph.visualize()`](./graphs/Graph/visualize.md)
   
 ## [`relationalai.std.math`](./math/README.md)
 
 - [`math.abs()`](./math/abs.md)
+- [`math.acos()`](./math/acos.md)
+- [`math.asin()`](./math/asin.md)
+- [`math.atan()`](./math/atan.md)
 - [`math.isclose()`](./math/isclose.md)
 - [`math.ceil()`](./math/ceil.md)
 - [`math.cbrt()`](./math/cbrt.md)
+- [`math.cos()`](./math/cos.md)
+- [`math.degrees()`](./math/degrees.md)
 - [`math.floor()`](./math/floor.md)
 - [`math.log()`](./math/log.md)
+- [`math.radians()`](./math/radians.md)
 - [`math.sign()`](./math/sign.md)
+- [`math.sin()`](./math/sin.md)
 - [`math.sqrt()`](./math/sqrt.md)
+- [`math.tan()`](./math/tan.md)
 - [`math.trunc_divide()`](./math/trunc_divide.md)
 
 ## [`relationalai.std.strings`](./strings/README.md)
 
 - [`strings.concat()`](./strings/concat.md)
 - [`strings.contains()`](./strings/contains.md)
 - [`strings.ends_with()`](./strings/ends_with.md)
```

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/Vars.md` & `relationalai-0.2.8/docs/api_reference/python/std/Vars.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/alias.md` & `relationalai-0.2.8/docs/api_reference/python/std/alias.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/aggregates/README.md` & `relationalai-0.2.8/docs/api_reference/python/std/aggregates/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/aggregates/avg.md` & `relationalai-0.2.8/docs/api_reference/python/std/aggregates/avg.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/aggregates/count.md` & `relationalai-0.2.8/docs/api_reference/python/std/aggregates/count.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/aggregates/max.md` & `relationalai-0.2.8/docs/api_reference/python/std/aggregates/max.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/aggregates/min.md` & `relationalai-0.2.8/docs/api_reference/python/std/aggregates/min.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/aggregates/rank_asc.md` & `relationalai-0.2.8/docs/api_reference/python/std/aggregates/rank_asc.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/aggregates/rank_desc.md` & `relationalai-0.2.8/docs/api_reference/python/std/aggregates/rank_desc.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/aggregates/sum.md` & `relationalai-0.2.8/docs/api_reference/python/std/aggregates/sum.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/graphs/README.md` & `relationalai-0.2.8/docs/api_reference/python/std/graphs/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # `relationalai.std.graphs`
 
 The `relationalai.std.graphs` namespace contains functions and classes for building
 [graphs](./Graph/README.md) from objects in a [model](../../Model/README.md) and doing graph analytics.
 
 - [`graphs.Compute`](./Compute/README.md)
+  - [`graphs.Compute.adamic_adar()`](./Compute/adamic_adar.md)
+  - [`graphs.compute.avg_clustering_coefficient()`](./Compute/avg_clustering_coefficient.md)
   - [`graphs.Compute.avg_degree()`](./Compute/avg_degree.md)
   - [`graphs.Compute.avg_indegree()`](./Compute/avg_indegree.md)
   - [`graphs.Compute.avg_outdegree()`](./Compute/avg_outdegree.md)
   - [`graphs.Compute.betweenness_centrality()`](./Compute/betweeness_centrality.md)
   - [`graphs.Compute.common_neighbor()`](./Compute/common_neighbor.md)
   - [`graphs.Compute.cosine_similarity()`](./Compute/cosine_similarity.md)
   - [`graphs.Compute.degree_centrality()`](./Compute/degree_centrality.md)
@@ -16,14 +18,15 @@
   - [`graphs.Compute.distance()`](./Compute/distance.md)
   - [`graphs.Compute.eigenvector_centrality()`](./Compute/eigenvector_centrality.md)
   - [`graph.Compute.indegree()`](./Compute/indegree.md)
   - [`graphs.Compute.is_connected()`](./Compute/is_connected.md)
   - [`graphs.Compute.is_reachable()`](./Compute/is_reachable.md)
   - [`graphs.Compute.is_triangle()`](./Compute/is_triangle.md)
   - [`graphs.Compute.label_propagation()`](./Compute/label_propagation.md)
+  - [`graphs.Compute.local_clustering_coefficient()`](./Compute/local_clustering_coefficient.md)
   - [`graphs.Compute.louvain()`](./Compute/louvain.md)
   - [`graphs.Compute.max_degree()`](./Compute/max_degree.md)
   - [`graphs.Compute.max_indegree()`](./Compute/max_indegree.md)
   - [`graphs.Compute.max_outdegree()`](./Compute/max_outdegree.md)
   - [`graphs.Compute.min_degree()`](./Compute/min_degree.md)
   - [`graphs.Compute.min_indegree()`](./Compute/min_indegree.md)
   - [`graphs.Compute.min_outdegree()`](./Compute/min_outdegree.md)
```

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/README.md` & `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 - [`Compute.degree_centrality()`](./degree_centrality.md)
 - [`Compute.eigenvector_centrality()`](./eigenvector_centrality.md)
 - [`Compute.indegree()`](./indegree.md)
 - [`Compute.is_connected()`](./is_connected.md)
 - [`Compute.is_reachable()`](./is_reachable.md)
 - [`Compute.is_triangle()`](./is_triangle.md)
 - [`Compute.label_propagation()`](./label_propagation.md)
+- [`Compute.local_clustering_coefficient()`](./local_clustering_coefficient.md)
 - [`Compute.louvain()`](./louvain.md)
 - [`Compute.max_degree()`](./max_degree.md)
 - [`Compute.max_indegree()`](./max_indegree.md)
 - [`Compute.max_outdegree()`](./max_outdegree.md)
 - [`Compute.min_degree()`](./min_degree.md)
 - [`Compute.min_indegree()`](./min_indegree.md)
 - [`Compute.min_outdegree()`](./min_outdegree.md)
```

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/adamic_adar.md` & `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/adamic_adar.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/avg_degree.md` & `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/avg_degree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/avg_indegree.md` & `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/avg_indegree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/avg_outdegree.md` & `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/avg_outdegree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/betweeness_centrality.md` & `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/betweeness_centrality.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/common_neighbor.md` & `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/common_neighbor.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/cosine_similarity.md` & `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/cosine_similarity.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/degree.md` & `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/degree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/degree_centrality.md` & `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/degree_centrality.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/diameter_range.md` & `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/diameter_range.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/distance.md` & `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/distance.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/eigenvector_centrality.md` & `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/eigenvector_centrality.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/indegree.md` & `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/indegree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/infomap.md` & `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/infomap.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/is_connected.md` & `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/is_connected.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/is_reachable.md` & `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/is_reachable.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/is_triangle.md` & `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/is_triangle.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/jaccard_similarity.md` & `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/jaccard_similarity.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/label_propagation.md` & `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/label_propagation.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/louvain.md` & `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/louvain.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/max_degree.md` & `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/max_degree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/max_indegree.md` & `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/max_indegree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/max_outdegree.md` & `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/max_outdegree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/min_degree.md` & `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/min_degree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/min_indegree.md` & `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/min_indegree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/min_outdegree.md` & `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/min_outdegree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/num_edges.md` & `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/num_edges.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/num_nodes.md` & `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/num_nodes.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/num_triangles.md` & `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/num_triangles.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/outdegree.md` & `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/outdegree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/pagerank.md` & `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/pagerank.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/preferential_attachment.md` & `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/preferential_attachment.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/reachable_from.md` & `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/reachable_from.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/triangles.md` & `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/triangles.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/weakly_connected_component.md` & `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/weakly_connected_component.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/weighted_cosine_similarity.md` & `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/weighted_cosine_similarity.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/weighted_degree_centrality.md` & `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/weighted_degree_centrality.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/weighted_distance.md` & `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/weighted_distance.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/graphs/Compute/weighted_jaccard_similarity.md` & `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/weighted_jaccard_similarity.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/graphs/Edge/README.md` & `relationalai-0.2.8/docs/api_reference/python/std/graphs/Edge/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/graphs/Edge/add.md` & `relationalai-0.2.8/docs/api_reference/python/std/graphs/Edge/add.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/graphs/Edge/call__.md` & `relationalai-0.2.8/docs/api_reference/python/std/graphs/Edge/call__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/graphs/Edge/extend.md` & `relationalai-0.2.8/docs/api_reference/python/std/graphs/Edge/extend.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/graphs/EdgeInstance/README.md` & `relationalai-0.2.8/docs/api_reference/python/std/graphs/EdgeInstance/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/graphs/EdgeInstance/from_.md` & `relationalai-0.2.8/docs/api_reference/python/std/graphs/EdgeInstance/from_.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/graphs/EdgeInstance/set.md` & `relationalai-0.2.8/docs/api_reference/python/std/graphs/EdgeInstance/set.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/graphs/EdgeInstance/to.md` & `relationalai-0.2.8/docs/api_reference/python/std/graphs/EdgeInstance/to.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/graphs/Graph/Edge.md` & `relationalai-0.2.8/docs/api_reference/python/std/graphs/Graph/Edge.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/graphs/Graph/Node.md` & `relationalai-0.2.8/docs/api_reference/python/std/graphs/Graph/Node.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/graphs/Graph/README.md` & `relationalai-0.2.8/docs/api_reference/python/std/graphs/Graph/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/graphs/Graph/compute.md` & `relationalai-0.2.8/docs/api_reference/python/std/graphs/Graph/compute.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/graphs/Graph/fetch.md` & `relationalai-0.2.8/docs/api_reference/python/std/graphs/Graph/fetch.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/graphs/Graph/id.md` & `relationalai-0.2.8/docs/api_reference/python/std/graphs/Graph/id.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/graphs/Graph/model.md` & `relationalai-0.2.8/docs/api_reference/python/std/graphs/Graph/model.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/graphs/Graph/undirected.md` & `relationalai-0.2.8/docs/api_reference/python/std/graphs/Graph/undirected.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/graphs/Graph/visualize.md` & `relationalai-0.2.8/docs/api_reference/python/std/graphs/Graph/visualize.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/graphs/Graph/img/graph-viz-with-labels-and-colors.png` & `relationalai-0.2.8/docs/api_reference/python/std/graphs/Graph/img/graph-viz-with-labels-and-colors.png`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/graphs/Graph/img/graph-viz.png` & `relationalai-0.2.8/docs/api_reference/python/std/graphs/Graph/img/graph-viz.png`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/graphs/Graph/img/simple-social-network.png` & `relationalai-0.2.8/docs/api_reference/python/std/graphs/Graph/img/simple-social-network.png`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/math/abs.md` & `relationalai-0.2.8/docs/api_reference/python/std/math/abs.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/math/cbrt.md` & `relationalai-0.2.8/docs/api_reference/python/std/math/cbrt.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/math/ceil.md` & `relationalai-0.2.8/docs/api_reference/python/std/math/ceil.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/math/floor.md` & `relationalai-0.2.8/docs/api_reference/python/std/math/floor.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/math/isclose.md` & `relationalai-0.2.8/docs/api_reference/python/std/math/isclose.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/math/log.md` & `relationalai-0.2.8/docs/api_reference/python/std/math/log.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/math/sign.md` & `relationalai-0.2.8/docs/api_reference/python/std/math/sign.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/math/sqrt.md` & `relationalai-0.2.8/docs/api_reference/python/std/math/sqrt.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/math/trunc_divide.md` & `relationalai-0.2.8/docs/api_reference/python/std/math/trunc_divide.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/strings/README.md` & `relationalai-0.2.8/docs/api_reference/python/std/strings/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/strings/concat.md` & `relationalai-0.2.8/docs/api_reference/python/std/strings/concat.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/strings/contains.md` & `relationalai-0.2.8/docs/api_reference/python/std/strings/contains.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/strings/ends_with.md` & `relationalai-0.2.8/docs/api_reference/python/std/strings/ends_with.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/strings/join.md` & `relationalai-0.2.8/docs/api_reference/python/std/strings/join.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/strings/length.md` & `relationalai-0.2.8/docs/api_reference/python/std/strings/length.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/strings/like.md` & `relationalai-0.2.8/docs/api_reference/python/std/strings/like.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/strings/lowercase.md` & `relationalai-0.2.8/docs/api_reference/python/std/strings/lowercase.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/strings/regex_compile.md` & `relationalai-0.2.8/docs/api_reference/python/std/strings/regex_compile.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/strings/regex_match.md` & `relationalai-0.2.8/docs/api_reference/python/std/strings/regex_match.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/strings/replace.md` & `relationalai-0.2.8/docs/api_reference/python/std/strings/replace.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/strings/split.md` & `relationalai-0.2.8/docs/api_reference/python/std/strings/split.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/strings/split_part.md` & `relationalai-0.2.8/docs/api_reference/python/std/strings/split_part.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/api_reference/python/std/strings/uppercase.md` & `relationalai-0.2.8/docs/api_reference/python/std/strings/uppercase.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/docs/faq/engines.md` & `relationalai-0.2.8/docs/faq/engines.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/examples/README.md` & `relationalai-0.2.8/examples/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/examples/cdc.py` & `relationalai-0.2.8/examples/cdc.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/examples/custom_snowflake_connection.py` & `relationalai-0.2.8/examples/custom_snowflake_connection.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/examples/emit_playground.py` & `relationalai-0.2.8/examples/emit_playground.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/examples/found.py` & `relationalai-0.2.8/examples/found.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/examples/fraud.ipynb` & `relationalai-0.2.8/examples/fraud.ipynb`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/examples/fraud.py` & `relationalai-0.2.8/examples/fraud.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/examples/graph_algos.py` & `relationalai-0.2.8/examples/graph_algos.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 import rich
 
 #--------------------------------------------------
 # Types
 #--------------------------------------------------
 
 model = rai.Model("MyCoolDatabase")
+model._config.set("compiler.use_multi_valued", True)
+
 Person = model.Type("Person")
 Criminal = model.Type("Criminal")
 Transaction = model.Type("Transaction")
 
 #--------------------------------------------------
 # Load data
 #--------------------------------------------------
@@ -20,19 +22,18 @@
 with model.rule():
     joe = Person.add(name="Joe")
     jane = Person.add(name="Jane")
     bob = Person.add(name="Bob")
     dylan = Person.add(Criminal, name="Dylan")
     dave = Person.add(name="Dave")
 
-    joe.set(knows=jane)
-    jane.set(knows=bob)
-    bob.set(knows=joe)
-    bob.set(knows=dylan)
-    dylan.set(knows=joe)
+    joe.knows.add(jane)
+    jane.knows.add(bob)
+    bob.knows.extend([joe, dylan])
+    dylan.knows.add(joe)
 
     Transaction.add(from_=joe, to=jane, amount=100)
     Transaction.add(from_=joe, to=jane, amount=1000)
     Transaction.add(from_=joe, to=jane, amount=10)
     Transaction.add(from_=joe, to=bob, amount=10)
 
 #--------------------------------------------------
@@ -61,13 +62,13 @@
 #--------------------------------------------------
 
 data = graph.fetch()
 rich.print(data)
 graph.visualize(three=True, style={
     "node": {
         "color": lambda x: "red" if x.get("criminal") else "blue",
-        "size": lambda x: (x["rank"] * 2) ** 2
+        "size": lambda x: (x.get("rank", 1) * 2) ** 2
     },
     "edge": {
         "color": "yellow",
     }
 }).display()
```

### Comparing `relationalai-0.2.7/examples/nested.py` & `relationalai-0.2.8/examples/nested.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/examples/or_types.py` & `relationalai-0.2.8/examples/or_types.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/examples/remote_load_csv.py` & `relationalai-0.2.8/examples/remote_load_csv.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/examples/simple_recursion.py` & `relationalai-0.2.8/examples/simple_recursion.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/examples/simple_streamlit.py` & `relationalai-0.2.8/examples/simple_streamlit.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/examples/solver.py` & `relationalai-0.2.8/examples/solver.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/examples/weighted_graph_algos.py` & `relationalai-0.2.8/examples/weighted_graph_algos.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/examples/articles_graph/README.md` & `relationalai-0.2.8/examples/articles_graph/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/examples/articles_graph/articles_graph.py` & `relationalai-0.2.8/examples/articles_graph/articles_graph.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/examples/articles_graph/articles_graph_with_nlp.py` & `relationalai-0.2.8/examples/articles_graph/articles_graph_with_nlp.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/examples/articles_graph/utils.py` & `relationalai-0.2.8/examples/articles_graph/utils.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/examples/articles_graph/daily_articles/04_04_2024.json` & `relationalai-0.2.8/examples/articles_graph/daily_articles/04_04_2024.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/examples/data/people.csv` & `relationalai-0.2.8/examples/data/people.csv`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/examples/data/transactions.csv` & `relationalai-0.2.8/examples/data/transactions.csv`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/examples/ev_penetration/ev_penetration.py` & `relationalai-0.2.8/examples/ev_penetration/ev_penetration.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/examples/ev_penetration/ev_penetration_csv.py` & `relationalai-0.2.8/examples/ev_penetration/ev_penetration_csv.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/examples/ev_penetration/state_stats.csv` & `relationalai-0.2.8/examples/ev_penetration/state_stats.csv`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/examples/imdb/README.md` & `relationalai-0.2.8/examples/imdb/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/examples/imdb/imdb.csv` & `relationalai-0.2.8/examples/imdb/imdb.csv`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/examples/imdb/imdb.py` & `relationalai-0.2.8/examples/imdb/imdb.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/examples/rel/solver.rel` & `relationalai-0.2.8/examples/rel/solver.rel`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/examples/social-money-network/SF_pagerank.ipynb` & `relationalai-0.2.8/examples/social-money-network/SF_pagerank.ipynb`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/examples/social-money-network/Simulation-and-SF-Upload.ipynb` & `relationalai-0.2.8/examples/social-money-network/Simulation-and-SF-Upload.ipynb`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/examples/social-money-network/snowflake_pagerank.py` & `relationalai-0.2.8/examples/social-money-network/snowflake_pagerank.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/frontend/debugger/package-lock.json` & `relationalai-0.2.8/frontend/debugger/package-lock.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/frontend/debugger/package.json` & `relationalai-0.2.8/frontend/debugger/package.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.875%*

 * *Differences: {"'type'": "'module'"}*

```diff
@@ -32,9 +32,10 @@
         "build": "vite build",
         "build-storybook": "storybook build",
         "dev": "vite",
         "serve": "vite preview",
         "start": "vite",
         "storybook": "storybook dev -p 6006"
     },
+    "type": "module",
     "version": "0.0.0"
 }
```

### Comparing `relationalai-0.2.7/frontend/debugger/tsconfig.json` & `relationalai-0.2.8/frontend/debugger/tsconfig.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/frontend/debugger/vite.config.ts` & `relationalai-0.2.8/frontend/debugger/vite.config.ts`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/frontend/debugger/.storybook/main.ts` & `relationalai-0.2.8/frontend/debugger/.storybook/main.ts`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/frontend/debugger/src/App.styl` & `relationalai-0.2.8/frontend/debugger/src/App.styl`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
 app-chrome {
   display: flex;
   flex-direction: row;
   height: 100vh;
   overflow: hidden;
 
-  & > .sidebar.left {
+  .app-sidebar {
     flex: 0 0 auto;
 
     .sidebar-content {
       overflow-y: auto;
       .os-windows & {
         -ms-overflow-style: none;
         scrollbar-width: none;
```

### Comparing `relationalai-0.2.7/frontend/debugger/src/App.tsx` & `relationalai-0.2.8/frontend/debugger/src/App.tsx`

 * *Files 5% similar despite different names*

```diff
@@ -4,28 +4,37 @@
 import { EventViewer } from "./components/EventViewer";
 import { Sidebar } from "./components/Sidebar";
 import { Button } from "./components/ui/Button";
 import { Field, Format } from "./components/ui/Field";
 import { Icon } from "./components/ui/Icon";
 import { Modal } from "./components/ui/Modal";
 import { Tooltip } from "./components/ui/Tooltip";
+import { FileDropZone } from "./components/FileDropZone";
 import { Message, Span, client, get_in, type Subject } from "./debugger_client";
 import "./App.styl";
 import { Breadcrumbs } from "./components/ui/Breadcrumbs";
-import { unwrap } from "solid-js/store";
 
 function App() {
     const event_list_selection = new Selection<Subject>("EventList");
 
     const clear = () => {
         client.connection.disconnect();
         event_list_selection.clear()
         client.clear();
     };
 
+    const exportData = () => {
+        client.exportData();
+	};
+
+    const handleFileDrop = (jsonObjects: any[]) => {
+        clear();
+        client.importData(jsonObjects[0]);
+    }
+
     const [pinned, set_pinned] = createSignal<boolean>(true);
 
     createEffect((prev_len: number|undefined) => {
         const cur_len = client.spans().length;
         const cur = event_list_selection.primary();
         if (pinned() && cur_len !== prev_len && cur) {
             event_list_selection.select({ event: "placeholder", selection_path: [cur_len - 1, ...cur.selection_path.slice(1)] })
@@ -42,31 +51,38 @@
             }
         }
     });
 
     return (
         <EventListSelection.Provider value={event_list_selection}>
             <app-chrome>
-                <Sidebar side="left" defaultOpen>
-                    <header>
-                        <Button class="icon" onclick={clear} tooltip="clear events">
-                            <Icon name="ban" />
-                        </Button>
-                        <Button class="icon" tooltip="Follow last run" onclick={() => set_pinned(v => !v)}>
-                            <Icon name="pin" type={pinned() ? "filled" : "outline"} />
-                        </Button>
-                        <span style="flex: 1" />
-                        <Modal title="Settings" content={<Settings />}>
-                            <Modal.Trigger as={Button} class="icon" tooltip="settings">
-                                <Icon name="settings" />
-                            </Modal.Trigger>
-                        </Modal>
-                    </header>
-                    <EventList events={client.spans()} />
-                </Sidebar>
+                <FileDropZone onFileDrop={handleFileDrop}>
+                    <Sidebar side="left" defaultOpen class="app-sidebar">
+                        <header>
+                            <Button class="icon" onclick={clear} tooltip="clear events">
+                                <Icon name="ban" />
+                            </Button>
+                            <Button class="icon" tooltip="Follow last run" onclick={() => set_pinned(v => !v)}>
+                                <Icon name="pin" type={pinned() ? "filled" : "outline"} />
+                            </Button>
+                            <span style="flex: 1" />
+
+                            <Button class="icon" tooltip="Export events" onclick={exportData}>
+                                <Icon name="download" />
+                            </Button>
+
+                            <Modal title="Settings" content={<Settings />}>
+                                <Modal.Trigger as={Button} class="icon" tooltip="settings">
+                                    <Icon name="settings" />
+                                </Modal.Trigger>
+                            </Modal>
+                        </header>
+                        <EventList events={client.spans()} />
+                    </Sidebar>
+                </FileDropZone >
                 <main>
                     <Show when={event_list_selection.primary()}>
                         <EventBreadcrumbs subject={event_list_selection.primary()!} select={event_list_selection.select} />
                         <scroll-container>
                             <scroll-inner>
                                 <EventViewer subject={event_list_selection.primary()!} />
                             </scroll-inner>
@@ -99,15 +115,18 @@
         <>
             <section>
                 <h3>Connection</h3>
                 <Field.Number label="Polling Interval" formatOptions={Format.seconds} minValue={1}
                     defaultValue={client.connection.reconnectInterval / 1000}
                     onRawValueChange={(v) => client.connection.reconnectInterval = v * 1000} />
                 <Field.Text label={"Debug URL"} placeholder={"ws://localhost:1234"}
-                    defaultValue={client.connection.ws_url} onChange={(v) => client.connection.ws_url = v} />
+                    defaultValue={client.connection.ws_url} onChange={(v) => {
+                        client.connection.ws_url = v
+                        client.connection.disconnect();
+                    }} />
             </section>
 
         </>
     )
 }
 
 interface EventBreadcrumbsProps {
```

### Comparing `relationalai-0.2.7/frontend/debugger/src/Selection.tsx` & `relationalai-0.2.8/frontend/debugger/src/Selection.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/frontend/debugger/src/debugger_client.ts` & `relationalai-0.2.8/frontend/debugger/src/debugger_client.ts`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import { Accessor, Setter, batch, createMemo, createSignal } from "solid-js";
+import { Accessor, Setter, batch, createSignal } from "solid-js";
 import { SetStoreFunction, createStore, produce, unwrap } from "solid-js/store";
 import * as Mech from "./types/mech";
 import { create_ws } from "./ws";
 
 //------------------------------------------------------------------------------
 // Utils
 //------------------------------------------------------------------------------
@@ -199,49 +199,69 @@
 
     connected: Accessor<boolean>;
     protected set_connected: Setter<boolean>;
 
     protected path: number[] = [];
 
     latest: Accessor<Span.Program|undefined>;
-    latest_blocks: Accessor<Span.Block[]|undefined>;
 
     constructor(ws_url: string) {
         this.connection = new Connection(ws_url);
         [this.messages, this.set_messages] = createSignal<Message[]>([], {equals: () => false});
         [this.root, this.set_root] = createStore<Span>({
             event: "span",
             span_type: "root",
             span: [],
             start_time: new Date(0),
             events: [],
             selection_path: []
         });
         [this.connected, this.set_connected] = createSignal<boolean>(false, {equals: () => false});
 
-        this.latest = createMemo(() => {
-            return this.spans().findLast(Span.is_program);
-        }, undefined, { equals: (prev, neue) => false });
-
-        this.latest_blocks = createMemo(() => {
-            return this.latest()?.events.filter(Span.is_block) ?? [];
-        }, [], { equals: () => false });
+        this.latest = () => this.spans().findLast(Span.is_program);
 
         this.connection.onreceive = this.handle_message;
         this.connection.onconnect = this.set_connected;
     }
 
     clear() {
         batch(() => {
             this.path = [];
             this.set_messages([]);
             this.set_root({event: "span", span_type: "root", span: [], start_time: new Date(0), events: []});
         });
     }
 
+    exportData = () => {
+        const data = JSON.stringify(unwrap(this.root));
+        const blob = new Blob([data], {type: "application/json"});
+
+
+        const a = document.createElement("a");
+        const url = URL.createObjectURL(blob);
+        a.href = url;
+        a.download = "debugger_data.json";
+
+        document.body.appendChild(a);
+        a.click();
+        document.body.removeChild(a);
+    }
+
+    importData = (data: Span) => {
+        this.set_root(data);
+    }
+
+    send = {
+        ping: () => this._send({type: "ping"})
+    }
+
+    protected _send(msg: any) {
+        this.connection.send(JSON.stringify(msg));
+    }
+
     protected handle_span_start(msg: Message.SpanStart) {
         this.set_root(produce((root) => {
             let parent = get_in(root, this.path);
             if(!parent || !Span.is_span(parent)) throw new Error();
             this.path.push(parent.events.length);
             let span_type = msg.span.type;
             let sub: Span = {
@@ -373,8 +393,8 @@
 
     public close(): void {
         this.shouldReconnect = false;
         this.disconnect();
     }
 }
 
-export const client = new DebuggerClient(`ws://${location.hostname}:5678`);
+export const client = new DebuggerClient(`ws://${location.host}/ws/client`);
```

### Comparing `relationalai-0.2.7/frontend/debugger/src/index.tsx` & `relationalai-0.2.8/frontend/debugger/src/index.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/frontend/debugger/src/logo.svg` & `relationalai-0.2.8/frontend/debugger/src/logo.svg`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/frontend/debugger/src/util.styl` & `relationalai-0.2.8/frontend/debugger/src/util.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/frontend/debugger/src/util.ts` & `relationalai-0.2.8/frontend/debugger/src/util.ts`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/frontend/debugger/src/assets/favicon.png` & `relationalai-0.2.8/frontend/debugger/src/assets/favicon.png`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/frontend/debugger/src/components/EventList.styl` & `relationalai-0.2.8/frontend/debugger/src/components/EventList.styl`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-@require "../../util.styl";
+@require "../util.styl";
 
 .event-list {
   box-sizing: border-box;
   display: flex;
   flex-direction: column;
+  padding-bottom: 40px;
   gap: 8px;
 
   .event-list-item {
     display: block;
     position: relative;
     box-sizing: border-box;
```

### Comparing `relationalai-0.2.7/frontend/debugger/src/components/EventList.tsx` & `relationalai-0.2.8/frontend/debugger/src/components/EventList.tsx`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import { Message, Span, client, type Subject } from "@src/debugger_client"
-import { Component, For, Show, children, createEffect, createSignal, untrack, useContext, type JSXElement } from "solid-js"
+import { Component, For, Show, createEffect, createSignal, untrack, useContext, type JSXElement } from "solid-js"
 import { Collapsible } from "./ui/Collapsible";
 import { EventListSelection } from "@src/Selection";
 import { Dynamic } from "solid-js/web";
 import { CodeBlock } from "./ui/Code";
 import "./EventList.styl";
 import { fmt, prefix_of } from "@src/util";
 import { Icon } from "./ui/Icon";
@@ -67,19 +67,19 @@
         if(subject_path.length < span_path.length) return false;
         for(let ix = 0; ix < span_path.length; ix += 1) {
             if(subject_path[ix] !== span_path[ix]) return false;
         }
         return true;
     });
 
-    const [open, set_open] = createSignal(contains_selection());
+    const [open, set_open] = createSignal(contains_selection() || props.open);
 
     createEffect(() => {
         let should_be_open = contains_selection();
-        if (untrack(() => open()) !== should_be_open) {
+        if (untrack(() => open()) !== should_be_open && untrack(() => selection.selected().length)) {
             set_open(should_be_open);
         }
     });
 
     return (
         <Collapsible side="top" open={open()} onOpenChange={set_open} class={klass()}>
             <Collapsible.Trigger as="header">
@@ -113,14 +113,15 @@
 // Items
 //------------------------------------------------------------------------------
 
 export function EventItemProgram(props: EventListItemProps<Span.Program>) {
     const selection = useContext(EventListSelection);
     const is_selection_inside = () => !!selection.selected().find(item => prefix_of(item.selection_path, props.event.selection_path));
     const should_open = () => is_selection_inside() || client.latest() === props.event;
+
     return (
         <EventListBranch event={props.event} open={should_open()} class="naked">
             <span class="event-label">Run #{(props.event as Span.Program).run}</span>
 
             <span class="event-detail">
                 {props.event.main}
             </span>
@@ -167,29 +168,20 @@
                 {fmt.time.ms(props.event.elapsed * 1000)}
             </span>
         </EventListLeaf>
     )
 }
 
 export function EventItemUnknownSpan(props: EventListItemProps<Span>) {
-    const selection = useContext(EventListSelection);
-    const is_selected = () => selection.is_selected(props.selects ?? props.event);
-    const klass = () => `event-list-item branch unknown ${is_selected() ? "selected" : ""}`;
-    const content = children(() => (
+    return (
         <For each={props.event.events}>
             {(event) => <EventListItem event={event} selects={props.selects} />}
         </For>
-    ));
-    return (
-        <Show when={content.toArray()?.filter((v) => v).length}>
-            <div class={klass()}>
-                {content()}
-            </div>
-        </Show>
     )
+
 }
 
 export function EventItemUnknown(props: EventListItemProps<Message.Event>) {
     return (
         <EventListLeaf event={props.event} class="unknown" selects={props.selects}>
             <span>
                 {props.event.event}
```

### Comparing `relationalai-0.2.7/frontend/debugger/src/components/EventViewer.tsx` & `relationalai-0.2.8/frontend/debugger/src/components/EventViewer.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/frontend/debugger/src/components/Sidebar.styl` & `relationalai-0.2.8/frontend/debugger/src/components/Sidebar.styl`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     animation-duration: var(--sidebar-anim-duration);
     animation-easing-function: ease-out;
 
     & > .ui-collapsible-inner {
       box-sizing: border-box;
       height: 100%;
       width: 100%;
+      min-width: 280px;
       padding: 0;
       display: flex;
       flex-direction: column;
     }
   }
 
   &.left, &.right {
```

### Comparing `relationalai-0.2.7/frontend/debugger/src/components/Sidebar.tsx` & `relationalai-0.2.8/frontend/debugger/src/components/Sidebar.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/frontend/debugger/src/components/Schematic/NodeIcon.stories.tsx` & `relationalai-0.2.8/frontend/debugger/src/components/Schematic/NodeIcon.stories.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/frontend/debugger/src/components/Schematic/ScopeProvider.tsx` & `relationalai-0.2.8/frontend/debugger/src/components/Schematic/ScopeProvider.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/frontend/debugger/src/components/Schematic/index.stories.tsx` & `relationalai-0.2.8/frontend/debugger/src/components/Schematic/index.stories.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/frontend/debugger/src/components/Schematic/index.styl` & `relationalai-0.2.8/frontend/debugger/src/components/Schematic/index.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/frontend/debugger/src/components/Schematic/index.tsx` & `relationalai-0.2.8/frontend/debugger/src/components/Schematic/index.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/frontend/debugger/src/components/Schematic/nodes/CallNode.tsx` & `relationalai-0.2.8/frontend/debugger/src/components/Schematic/nodes/CallNode.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/frontend/debugger/src/components/Schematic/nodes/EffectNode.tsx` & `relationalai-0.2.8/frontend/debugger/src/components/Schematic/nodes/EffectNode.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/frontend/debugger/src/components/Schematic/nodes/GetNode.tsx` & `relationalai-0.2.8/frontend/debugger/src/components/Schematic/nodes/GetNode.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/frontend/debugger/src/components/Schematic/nodes/QuantifyNode.tsx` & `relationalai-0.2.8/frontend/debugger/src/components/Schematic/nodes/QuantifyNode.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/frontend/debugger/src/components/Schematic/nodes/ReturnNode.tsx` & `relationalai-0.2.8/frontend/debugger/src/components/Schematic/nodes/ReturnNode.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/frontend/debugger/src/components/Schematic/nodes/SequenceNode.tsx` & `relationalai-0.2.8/frontend/debugger/src/components/Schematic/nodes/SequenceNode.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/frontend/debugger/src/components/Schematic/nodes/UnionNode.tsx` & `relationalai-0.2.8/frontend/debugger/src/components/Schematic/nodes/UnionNode.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/frontend/debugger/src/components/Schematic/nodes/base.styl` & `relationalai-0.2.8/frontend/debugger/src/components/Schematic/nodes/base.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/frontend/debugger/src/components/Schematic/nodes/base.tsx` & `relationalai-0.2.8/frontend/debugger/src/components/Schematic/nodes/base.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/frontend/debugger/src/components/Schematic/nodes/index.tsx` & `relationalai-0.2.8/frontend/debugger/src/components/Schematic/nodes/index.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/frontend/debugger/src/components/ui/Accordion.stories.tsx` & `relationalai-0.2.8/frontend/debugger/src/components/ui/Accordion.stories.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/frontend/debugger/src/components/ui/Accordion.tsx` & `relationalai-0.2.8/frontend/debugger/src/components/ui/Accordion.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/frontend/debugger/src/components/ui/Breadcrumbs.stories.tsx` & `relationalai-0.2.8/frontend/debugger/src/components/ui/Breadcrumbs.stories.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/frontend/debugger/src/components/ui/Breadcrumbs.tsx` & `relationalai-0.2.8/frontend/debugger/src/components/ui/Breadcrumbs.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/frontend/debugger/src/components/ui/Button.tsx` & `relationalai-0.2.8/frontend/debugger/src/components/ui/Button.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/frontend/debugger/src/components/ui/Code.styl` & `relationalai-0.2.8/frontend/debugger/src/components/ui/Code.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/frontend/debugger/src/components/ui/Code.tsx` & `relationalai-0.2.8/frontend/debugger/src/components/ui/Code.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/frontend/debugger/src/components/ui/Collapsible.stories.tsx` & `relationalai-0.2.8/frontend/debugger/src/components/ui/Collapsible.stories.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/frontend/debugger/src/components/ui/Collapsible.styl` & `relationalai-0.2.8/frontend/debugger/src/components/ui/Collapsible.styl`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     // grid-template-rows: minmax(auto, 1fr);
     // grid-template-columns: minmax(auto, 1fr);
     // align-items: stretch;
     // justify-items: stretch;
 
     animation-duration: var(--collapsible-anim-duration);
     animation-easing-function: ease-out;
-    animation-fill-mode: forwards;
+    // animation-fill-mode: forwards;
 
     & > .ui-collapsible-inner {
       box-sizing: border-box;
     }
   }
 
   &.left, &.right {
```

### Comparing `relationalai-0.2.7/frontend/debugger/src/components/ui/Collapsible.tsx` & `relationalai-0.2.8/frontend/debugger/src/components/ui/Collapsible.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/frontend/debugger/src/components/ui/Field.stories.tsx` & `relationalai-0.2.8/frontend/debugger/src/components/ui/Field.stories.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/frontend/debugger/src/components/ui/Field.styl` & `relationalai-0.2.8/frontend/debugger/src/components/ui/Field.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/frontend/debugger/src/components/ui/Field.tsx` & `relationalai-0.2.8/frontend/debugger/src/components/ui/Field.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/frontend/debugger/src/components/ui/Icon.tsx` & `relationalai-0.2.8/frontend/debugger/src/components/ui/Icon.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/frontend/debugger/src/components/ui/Modal.stories.tsx` & `relationalai-0.2.8/frontend/debugger/src/components/ui/Modal.stories.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/frontend/debugger/src/components/ui/Modal.styl` & `relationalai-0.2.8/frontend/debugger/src/components/ui/Modal.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/frontend/debugger/src/components/ui/Modal.tsx` & `relationalai-0.2.8/frontend/debugger/src/components/ui/Modal.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/frontend/debugger/src/components/ui/Tooltip.stories.tsx` & `relationalai-0.2.8/frontend/debugger/src/components/ui/Tooltip.stories.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/frontend/debugger/src/components/ui/Tooltip.styl` & `relationalai-0.2.8/frontend/debugger/src/components/ui/Tooltip.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/frontend/debugger/src/components/ui/Tooltip.tsx` & `relationalai-0.2.8/frontend/debugger/src/components/ui/Tooltip.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/frontend/debugger/src/fixtures/branch-improved.json` & `relationalai-0.2.8/frontend/debugger/src/fixtures/branch-improved.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/frontend/debugger/src/fixtures/branch.json` & `relationalai-0.2.8/frontend/debugger/src/fixtures/branch.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/frontend/debugger/src/fixtures/fraud.json` & `relationalai-0.2.8/frontend/debugger/src/fixtures/fraud.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/frontend/debugger/src/fixtures/not_found.json` & `relationalai-0.2.8/frontend/debugger/src/fixtures/not_found.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/frontend/debugger/src/fixtures/simple.json` & `relationalai-0.2.8/frontend/debugger/src/fixtures/simple.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/frontend/debugger/src/fixtures/union.json` & `relationalai-0.2.8/frontend/debugger/src/fixtures/union.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/frontend/debugger/src/types/mech.d.ts` & `relationalai-0.2.8/frontend/debugger/src/types/mech.d.ts`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/src/gentest/README.md` & `relationalai-0.2.8/src/gentest/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/src/gentest/emit.py` & `relationalai-0.2.8/src/gentest/emit.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/src/gentest/exec.py` & `relationalai-0.2.8/src/gentest/exec.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/src/gentest/fixtures.py` & `relationalai-0.2.8/src/gentest/fixtures.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/src/gentest/patch.py` & `relationalai-0.2.8/src/gentest/patch.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/src/gentest/util.py` & `relationalai-0.2.8/src/gentest/util.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/src/gentest/cli/__main__.py` & `relationalai-0.2.8/src/gentest/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/src/gentest/cli/collect_failures.py` & `relationalai-0.2.8/src/gentest/cli/collect_failures.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/src/gentest/cli/collect_tests.py` & `relationalai-0.2.8/src/gentest/cli/collect_tests.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/src/gentest/cli/repro.py` & `relationalai-0.2.8/src/gentest/cli/repro.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/src/gentest/cli/watch.py` & `relationalai-0.2.8/src/gentest/cli/watch.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/src/gentest/gen/action.py` & `relationalai-0.2.8/src/gentest/gen/action.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/src/gentest/gen/context.py` & `relationalai-0.2.8/src/gentest/gen/context.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/src/gentest/gen/document.py` & `relationalai-0.2.8/src/gentest/gen/document.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/src/gentest/gen/group_limited.py` & `relationalai-0.2.8/src/gentest/gen/group_limited.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/src/gentest/gen/ir.py` & `relationalai-0.2.8/src/gentest/gen/ir.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/src/gentest/gen/scope.py` & `relationalai-0.2.8/src/gentest/gen/scope.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/src/gentest/gen/task.py` & `relationalai-0.2.8/src/gentest/gen/task.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/src/gentest/gen/test.py` & `relationalai-0.2.8/src/gentest/gen/test.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/src/gentest/harness/database.py` & `relationalai-0.2.8/src/gentest/harness/database.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/src/gentest/validate/diff.py` & `relationalai-0.2.8/src/gentest/validate/diff.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/src/gentest/validate/errors.py` & `relationalai-0.2.8/src/gentest/validate/errors.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/src/gentest/validate/mapping.py` & `relationalai-0.2.8/src/gentest/validate/mapping.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/src/gentest/validate/roundtrip.py` & `relationalai-0.2.8/src/gentest/validate/roundtrip.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/src/relationalai/__init__.py` & `relationalai-0.2.8/src/relationalai/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,16 +22,16 @@
     debug=None,
     connection: SnowflakeConnection | None = None,
 ):
     config = config or cfg.Config(profile=profile)
     if debug is None:
         debug = config.get("debug", False)
     if debug:
-        from relationalai.tools.debugger_server import start_debugger_session
-        start_debugger_session(True)
+        from relationalai.tools.debugger_client import start_debugger_session
+        start_debugger_session() # @TODO: add config / env vars / kwargs for debug_host and debug_port
     if not config.file_path:
         if cfg.legacy_config_exists():
             message = (
                 "Use `rai init` to migrate your configuration file "
                 "to the new format (raiconfig.toml)"
             )
         else:
```

### Comparing `relationalai-0.2.7/src/relationalai/compiler.py` & `relationalai-0.2.8/src/relationalai/compiler.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/src/relationalai/debugging.py` & `relationalai-0.2.8/src/relationalai/debugging.py`

 * *Files 2% similar despite different names*

```diff
@@ -270,18 +270,21 @@
 
 jupyter = Jupyter()
 
 #--------------------------------------------------
 # Position capture
 #--------------------------------------------------
 
+rai_site_packages = os.path.join("site-packages", "relationalai")
+rai_src = os.path.join("src", "relationalai")
+
 def first_non_relationalai_frame(frame):
     while frame and frame.f_back:
         file = frame.f_code.co_filename
-        if "site-packages/relationalai" not in file and "src/relationalai" not in file:
+        if rai_site_packages not in file and rai_src not in file:
             break
         frame = frame.f_back
     return frame
 
 def capture_code_info(steps=None):
     # Get the current frame and go back to the caller's frame
     caller_frame = inspect.currentframe()
```

### Comparing `relationalai-0.2.7/src/relationalai/dsl.py` & `relationalai-0.2.8/src/relationalai/dsl.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/src/relationalai/errors.py` & `relationalai-0.2.8/src/relationalai/errors.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/src/relationalai/metagen.py` & `relationalai-0.2.8/src/relationalai/metagen.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/src/relationalai/metamodel.py` & `relationalai-0.2.8/src/relationalai/metamodel.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/src/relationalai/rel.py` & `relationalai-0.2.8/src/relationalai/rel.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/src/relationalai/rel2.py` & `relationalai-0.2.8/src/relationalai/rel2.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/src/relationalai/rel_emitter.py` & `relationalai-0.2.8/src/relationalai/rel_emitter.py`

 * *Files 2% similar despite different names*

```diff
@@ -258,14 +258,15 @@
                     head_vars.add(v)
                 elif i.entity.value == Builtins.Install:
                     (item,) = i.bindings.values()
                     supporting_rules.append(f"declare {self.emit_var(item)}")
                     if isinstance(item.value, Type) and item.value.isa(Builtins.ValueType):
                         vtype = self.sanitize(item.value.name).capitalize() + "Type"
                         supporting_rules.append(f"value type {vtype} {{ UInt128 }}")
+                        supporting_rules.append(f"@inline def pyrel_unwrap(y in {vtype}, x): ^{vtype}(x, y)")
                         for op in ["<", ">"]:
                             supporting_rules.append(f"def ::std::common::({op})[x in {vtype}, y in {vtype}]: exists((a, b) | ^{vtype}(a, x) and ^{vtype}(b, y) and a {op} b)")
                         for op in ["minimum", "maximum"]:
                             supporting_rules.append(f"def ::std::common::{op}(x in {vtype}, y in {vtype}, z in {vtype}): exists((a, b) | ^{vtype}(minimum[a, b], z) and ^{vtype}(a, x) and ^{vtype}(b, y))")
                 else:
                     body.append(self.to_relation(i, body_vars, body))
             elif i.action == ActionType.Bind and i.entity.value == Builtins.Return:
```

### Comparing `relationalai-0.2.7/src/relationalai/rel_utils.py` & `relationalai-0.2.8/src/relationalai/rel_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,15 +32,17 @@
 
 def emit_nested_relation(prefix: str, obj: dict|None = None, keys: Iterable[str]|None = None, raw = False) -> str:
     """Emit a set of defs encoding `obj` in GNF on `prefix`."""
     obj = obj or {}
     result = ""
     for k in keys or obj.keys():
         v = obj.get(k, None)
-        if v is not None:
+        if isinstance(v, dict):
+            result += emit_nested_relation(f"{prefix}{safe_symbol(k)}, ", v)
+        elif v is not None:
             result += f"def {prefix}{safe_symbol(k)}]: {emit_literal(v) if not raw else v}\n"
     return result
 
 #-------------------------------------------------------------------------------
 # Result Handling
 #-------------------------------------------------------------------------------
```

### Comparing `relationalai-0.2.7/src/relationalai/analysis/mechanistic.py` & `relationalai-0.2.8/src/relationalai/analysis/mechanistic.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/src/relationalai/analysis/whynot.py` & `relationalai-0.2.8/src/relationalai/analysis/whynot.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/src/relationalai/clients/azure.py` & `relationalai-0.2.8/src/relationalai/clients/azure.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+from datetime import datetime, timedelta
 import json
 import textwrap
 import time
 from typing import Any, Tuple, List
 import base64
 from urllib.error import HTTPError
 
 from pandas import DataFrame
 import pandas as pd
+import re
+import decimal
 
 from relationalai import debugging
 
 from ..errors import Errors, RAIException
 from ..rel_utils import assert_no_problems
 from ..loaders.loader import emit_delete_import, import_file, list_available_resources
 from .config import Config
@@ -21,14 +24,16 @@
 
 #--------------------------------------------------
 # Constants
 #--------------------------------------------------
 
 UNIXEPOCH = 62135683200000
 MILLISECONDS_PER_DAY = 24 * 60 * 60 * 1000
+TXN_FIELDS = ["id", "account_name", "state", "created_on", "finished_at", "duration", "database_name", "read_only", "engine_name", "query", "query_size", "tags", "user_agent", "response_format_version"]
+TXN_REPLACE_MAP = {"database_name": "database", "engine_name": "engine", "account_name": "account", "user_agent": "agent"}
 VALID_ENGINE_STATES = ["REQUESTED", "PROVISIONED", "PROVISIONING"]
 
 #--------------------------------------------------
 # Resources
 #--------------------------------------------------
 
 class Resources(ResourceProvider):
@@ -213,35 +218,101 @@
         if len(results.results):
             for result in results.results:
                 types = [t for t in result["relationId"].split("/") if t != "" and not t.startswith(":")]
                 result_frame:DataFrame = result["table"].to_pandas()
                 for i, col in enumerate(result_frame.columns):
                     if "UInt128" in types[i]:
                         result_frame[col] = result_frame[col].apply(lambda x: base64.b64encode(x.tobytes()).decode()[:-2])
-                    if types[i] == "Dates.DateTime":
+                    elif "FixedDecimal" in types[i]:
+                        decimal_info = re.search(r"FixedDecimal\{Int(\d+), (\d+)\}", types[i])
+                        if decimal_info:
+                            bits = int(decimal_info.group(1))
+                            scale = int(decimal_info.group(2))
+                            if bits == 128:
+                                result_frame[col] = result_frame[col].apply(lambda x: (decimal.Decimal(str((int(x[1]) << 64) + int(x[0]))) if x[1] > 0 else decimal.Decimal(str(x[0]))) / (10 ** scale))
+                            else:
+                                result_frame[col] = result_frame[col].apply(lambda x: decimal.Decimal(str(x)) / (10 ** scale))
+                    elif "Int128" in types[i]:
+                        result_frame[col] = result_frame[col].apply(lambda x: (int(x[1]) << 64) + int(x[0]) if x[1] > 0 else x[0])
+                    elif types[i] == "Dates.DateTime":
                         result_frame[col] = pd.to_datetime(result_frame[col] - UNIXEPOCH, unit="ms")
-                    if types[i] == "Dates.Date":
+                    elif types[i] == "Dates.Date":
                         result_frame[col] = pd.to_datetime(result_frame[col] * MILLISECONDS_PER_DAY - UNIXEPOCH, unit="ms")
                 ret_cols = task.return_cols()
                 if len(ret_cols) and len(result_frame.columns) == len(ret_cols):
                     result_frame.columns = task.return_cols()[0:len(result_frame.columns)]
                 result["table"] = result_frame
                 if ":output" in result["relationId"]:
                     data_frame = pd.concat([data_frame, result_frame], ignore_index=True)
         return (data_frame, results.problems)
 
     #--------------------------------------------------
     # Transactions
     #--------------------------------------------------
 
-    def list_transactions(self, limit:int, only_active=False):
-        raise Exception("Not implemented")
+    def get_transaction(self, transaction_id):
+        txn = api.get_transaction(self._api_ctx(), transaction_id)
+        if not txn:
+            return None
+        created_on = txn.get("created_on")
+        finished_at = txn.get("finished_at")
+        duration = txn.get("duration")
+        if duration:
+            txn["duration"] = timedelta(milliseconds=duration)
+        else:
+            txn["duration"] = datetime.now() - datetime.fromtimestamp(created_on / 1000)
+        if created_on:
+            txn["created_on"] = datetime.fromtimestamp(created_on / 1000)
+        if finished_at:
+            txn["finished_at"] = datetime.fromtimestamp(finished_at / 1000)
+        # Remap based on the fields we care about
+        result = {TXN_REPLACE_MAP.get(k, k): v for k, v in txn.items() if k in TXN_FIELDS}
+        return result
+
+    def remap_fields(self, transactions):
+        if not transactions:
+            return []
+        for transaction in transactions:
+            for key in list(transaction.keys()):
+                if key in TXN_REPLACE_MAP:
+                    transaction[TXN_REPLACE_MAP[key]] = transaction.pop(key)
+        return transactions
+
+    def list_transactions(self, **kwargs):
+        TERMINAL_STATES = ["COMPLETED", "ABORTED"]
+        VALID_KEYS = ["id", "state"]
+
+        state = kwargs.get("state")
+        only_active = kwargs.get("only_active", False)
+        options = {}
+
+        # Azure sdk supports more than just VALID_KEYS as filters but for now we pass through those
+        for k, v in kwargs.items():
+            if k in VALID_KEYS and v is not None:
+                # Only pass state if it is a valid terminal state
+                if k == "state" and v.upper() in TERMINAL_STATES:
+                    options[k] = v.upper()
+                if k != "state":
+                    options[k] = v
+        # In Azure we store transactions in cosmos and consul
+        # Cosmos if the state is terminal (COMPLETED or ABORTED) and Consul if the state is not (e.g. "RUNNING")
+        # So we can not filter on active non terminal states via the options passed
+        transactions = api.list_transactions(self._api_ctx(), **options)
+
+        if not transactions:
+            return []
+        # We filter non terminal transactions here
+        if only_active:
+            transactions = [t for t in transactions if t["state"] in ["CREATED", "RUNNING", "PENDING"]]
+        if (isinstance(state, str) and state.upper() not in TERMINAL_STATES):
+            transactions = [t for t in transactions if t["state"] in [state.upper()]]
+        return self.remap_fields(transactions)
 
     def cancel_transaction(self, transaction_id):
-        raise Exception("Not implemented")
+        return api.cancel_transaction(self._api_ctx(), transaction_id)
 
     def cancel_pending_transactions(self):
         # all transactions are executed synchronously against azure
         pass
 
 #--------------------------------------------------
 # Graph
@@ -255,10 +326,13 @@
             exists((u) | hash128({x...}, x..., u) and
             hash_value_uint128_convert(u, z))
 
         @inline
         def pyrel_default({F}, c, k..., v):
             F(k..., v) or (not F(k..., _) and v = c)
 
+        @inline
+        def pyrel_unwrap(x in UInt128, y): y = x
+
         declare __resource
     """))
     return dsl.Graph(client, name)
```

### Comparing `relationalai-0.2.7/src/relationalai/clients/client.py` & `relationalai-0.2.8/src/relationalai/clients/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,17 +127,20 @@
 
     def get_app_name(self):
         return self.config.get("rai_app_name", "relationalai")
 
     #--------------------------------------------------
     # Transactions
     #--------------------------------------------------
+    @abstractmethod
+    def get_transaction(self, transaction_id):
+        pass
 
     @abstractmethod
-    def list_transactions(self, limit:int, only_active=False) -> List[dict]:
+    def list_transactions(self, limit:int, only_active=False, **kwargs) -> List[dict]:
         pass
 
     @abstractmethod
     def cancel_transaction(self, transaction_id):
         pass
 
     @abstractmethod
```

### Comparing `relationalai-0.2.7/src/relationalai/clients/config.py` & `relationalai-0.2.8/src/relationalai/clients/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from copy import deepcopy
 import os
-from typing import Dict, Any, cast
+from typing import Dict, Any
 from railib import config
 import configparser
 import toml
 import tomlkit
-from tomlkit.items import Table
 
+from relationalai.util.constants import DEFAULT_PROFILE_NAME, TOP_LEVEL_PROFILE_NAME
 
 #--------------------------------------------------
 # config defaults
 #--------------------------------------------------
 
 CONFIG_FILE = "raiconfig.toml"
 FIELD_PLACEHOLDER = ""
@@ -41,15 +41,27 @@
 
 _no_default = object()
 
 #--------------------------------------------------
 # helpers
 #--------------------------------------------------
 
+def map_toml_value(value: Any):
+    if value is True:
+        return "true"
+    if value is False:
+        return "false"
+    return value
+
 class ConfigFile:
+    """
+    Represents of a file that contains some config information, including both raiconfig.toml and rai.config files.
+
+    Used to handle collection and merging of configuration properties from multiple sources.
+    """
     def __init__(
         self,
         path: str | None = None,
         cfg: Dict[str, Any] = {},
         *,
         format = "toml"
     ):
@@ -67,15 +79,15 @@
                 for k, v in cfg.items()
                 if k != "DEFAULT"
             }
             self.config = {}
         else:
             raise ValueError(f"Unsupported format: {format}")
 
-    def apply_keymap(self):
+    def migrate_old_keys(self):
         keymap = {
             "active-profile": "active_profile",
             "snowflake-connection": "snowflake_connection",
             "snowsql_user": "user",
             "snowsql_pwd": "password",
         }
         new_config = {}
@@ -88,27 +100,27 @@
             for key in props.copy():
                 # self.profiles[profile][keymap.get(key, key)] = props[key]
                 new_profiles[profile][keymap.get(key, key)] = props[key]
         self.profiles = new_profiles
 
     def get_combined_profiles(self):
         combined_profiles = {}
-        combined_profiles["__top_level__"] = self.config or {}
+        combined_profiles[TOP_LEVEL_PROFILE_NAME] = self.config or {}
         for profile in self.profiles:
             combined_profiles[profile] = self.profiles[profile].copy()
         return combined_profiles
 
     def map(self, f):
         """
         Apply a function `f` to all props dictionaries in the configuration files, including the top-level dictionary and all profiles.
         """
         combined_profiles = self.get_combined_profiles()
         for profile in combined_profiles:
             combined_profiles[profile] = f(combined_profiles[profile])
-        config = combined_profiles.pop("__top_level__")
+        config = combined_profiles.pop(TOP_LEVEL_PROFILE_NAME)
         return self.__class__(
             self.path, { **config, "profile": combined_profiles }
         )
 
     def filled_from_snowflake_connection(self):
         def fill(props):
             if "snowflake_connection" in props:
@@ -133,15 +145,15 @@
         all_profile_names = set(combined_profiles) | set(other_combined_profiles)
 
         for profile in all_profile_names:
             self_profile = combined_profiles.get(profile, {})
             other_profile = other_combined_profiles.get(profile, {})
             combined_profiles[profile] = {**other_profile, **self_profile}
 
-        config = combined_profiles.pop("__top_level__", None)
+        config = combined_profiles.pop(TOP_LEVEL_PROFILE_NAME, None)
 
         if config is not None:
             self.config = config
         self.profiles = combined_profiles
 
 
 def first(x):
@@ -184,24 +196,24 @@
     Handles both TOML and INI files.
     """
     if not os.path.exists(file):
         return ConfigFile(cfg={})
     if file.endswith(".toml"):
         try:
             cf = ConfigFile(file, toml.load(file))
-            cf.apply_keymap()
+            cf.migrate_old_keys()
             return cf
         except toml.TomlDecodeError as e:
             raise Exception(f"Error parsing {file}: {e}")
     else:
         try:
             config = configparser.ConfigParser()
             config.read(file)
             cf = ConfigFile(file, {k: v for k, v in config.items() if k != "DEFAULT"}, format="ini")
-            cf.apply_keymap()
+            cf.migrate_old_keys()
             return cf
         except Exception:
             # silently ignore parsing errors for INI files because
             # they are inessential to the flow
             return ConfigFile(cfg={})
 
 def _get_full_config(profile:str|None=None) -> tuple[Dict[str,Any], str|None]:
@@ -222,14 +234,16 @@
     for i in range(len(config_files) - 1, 0, -1):
         config_files[i-1].merge(config_files[i])
     if not config_files:
         return {}, file_path
     root_file = config_files[0]
     if profile:
         root_file.config["active_profile"] = profile
+    if not profile and "active_profile" not in root_file.config:
+        root_file.config["active_profile"] = DEFAULT_PROFILE_NAME
     if ("active_profile" in root_file.config and
         root_file.config["active_profile"] in root_file.profiles):
         active_profile = root_file.config["active_profile"]
         config = {
             **root_file.config,
             **root_file.profiles[active_profile],
         }
@@ -284,57 +298,138 @@
     return result
 
 
 #--------------------------------------------------
 # Config
 #--------------------------------------------------
 
+class ConfigStore():
+    """
+    Interface to the project raiconfig.toml file -- used to read and write configuration properties.
+    """
+    def __init__(self, file_path:str = CONFIG_FILE, toml_string:str|None = None):
+        self.load(file_path, toml_string)
+
+    def load(self, file_path:str = CONFIG_FILE, toml_string:str|None = None):
+        if toml_string:
+            self.file_path = "__inline__"
+            self.tomldoc = tomlkit.parse(toml_string)
+        else:
+            self.file_path = file_path
+            self.tomldoc = tomlkit.document()
+            if os.path.exists(file_path):
+                with open(file_path, "r") as f:
+                    try:
+                        content = f.read()
+                        if not content.endswith("\n"):
+                            content += "\n"
+                        self.tomldoc = tomlkit.parse(content)
+                    except toml.TomlDecodeError as e:
+                        raise Exception(f"Error parsing {file_path}: {e}")
+
+    def get(self, key, default=None):
+        return self.tomldoc.get(key, default)
+
+    def items(self):
+        return self.tomldoc.items()
+    
+    def get_profiles(self):
+        return self.get("profile", {})
+
+    def num_profiles(self):
+        return len(self.get_profiles())
+    
+    def switch_active_profile(self, profile:str):
+        self.tomldoc["active_profile"] = profile
+        self.save()
+
+    def with_new_profile(self, config) -> tomlkit.TOMLDocument:
+        document = deepcopy(self.tomldoc)
+        profiles = document.pop("profile", None)
+        if not profiles:
+            profiles = tomlkit.table()
+        table_for_new_profile = tomlkit.table()
+        for key, value in config.items_with_dots():
+            toml_key = tomlkit.key(key.split(".") if "." in key else key)
+            table_for_new_profile.add(toml_key, value)
+        
+        new_profiles_table = tomlkit.table(is_super_table=True)
+        new_profiles_table.add(config.profile, table_for_new_profile)
+        for k, v in profiles.items():
+            if k == config.profile:
+                continue
+            new_profiles_table.add(k, v)
+        document.add("profile", new_profiles_table)
+
+        return document
+
+    def add_profile(self, config):
+        self.tomldoc = self.with_new_profile(config)
+
+    def save(self):
+        with open(self.file_path, "w") as f:
+            f.write(self.tomldoc.as_string())
+
+    def change_active_profile(self, profile:str):
+        document = tomlkit.document()
+        document.add("active_profile", profile) # type: ignore
+        document.add(tomlkit.nl())
+        for key, value in self.tomldoc.items():
+            if key != "active_profile":
+                document.add(key, value) # type: ignore
+        self.tomldoc = document
+        
+    def __str__(self):
+        return self.tomldoc.as_string()
+    
+    def get_config(self):
+        props = {}
+        for key, value in self.items():
+            if key != "profile":
+                props[key] = value
+        profile = None
+        if "active_profile" in props:
+            active_profile = props.pop("active_profile")
+            profiles = self.get("profile", {})
+            if active_profile in profiles:
+                props.update(profiles[active_profile])
+                profile = active_profile
+        config = Config(props, fetch=False)
+        if profile:
+            config.profile = profile
+        return config
+
 class Config():
+    """
+    Represents an active collection of configuration properties.
+    """
     def __init__(self, profile:str|Dict[str,Any]|None=None, fetch=True):
         supplied_props = None
         if isinstance(profile, dict):
             supplied_props = profile
-            profile = "__top_level__"
+            profile = TOP_LEVEL_PROFILE_NAME
         if fetch:
             self.fetch(profile)
         else:
-            self.profile = "__top_level__"
+            self.profile = TOP_LEVEL_PROFILE_NAME
             self.props = {}
-        self.cache_config_file_contents()
+            self.file_path = None
         if supplied_props is not None:
             for k, v in supplied_props.items():
                 self.set(k, v)
             if not self.file_path:
                 self.file_path = "__inline__"
-
-    def get_profiles(self):
-        if not self.original_toml:
-            return {}
-        return self.original_toml.get("profile", {})
-
+    
     def fetch(self, profile:str|None=None):
         profile = profile or os.environ.get("RAI_PROFILE", None)
         cfg, path = _get_full_config(profile)
-        self.profile = profile or cfg.get("active_profile", "__top_level__")
+        self.profile = profile or cfg.get("active_profile", TOP_LEVEL_PROFILE_NAME)
         self.file_path = path
         self.props = cfg
 
-    def cache_config_file_contents(self):
-        self.original_toml = tomlkit.document()
-        if os.path.exists(CONFIG_FILE):
-            with open(CONFIG_FILE, "r") as f:
-                try:
-                    content = f.read()
-                    if not content.endswith("\n"):
-                        content += "\n"
-                    self.original_toml = tomlkit.parse(content)
-                except toml.TomlDecodeError as e:
-                    raise Exception(f"Error parsing {self.file_path}: {e}")
-            return
-
     def clone_profile(self):
         self.props = {k: v for k,v in self.props.items()}
 
     def clone(self):
         return deepcopy(self)
 
     def get(self, name:str, default:Any=_no_default, strict:bool=True):
@@ -365,140 +460,39 @@
 
     def clear_props(self):
         self.props = {}
 
     def unset(self, name:str):
         del self.props[name]
 
-    def update(self, other, save_progress=False):
+    def update(self, other):
         self.props.update(other)
 
     def __contains__(self, key):
         return key in self.props
 
     def items(self):
         return self.props.items()
-
-    def print(self):
-        for k, v in self.items():
-            print(f"{k}: {v}")
+    
+    def items_with_dots(self):
+        return items_with_dots(self.props)
+    
+    def __str__(self):
+        return "\n".join(f"{k}: {map_toml_value(v)}" for k, v in self.items_with_dots())
 
     def to_rai_config(self) -> Dict[str, Any]:
         return to_rai_config(self.props)
 
-    def save(self, update_active_profile=True):
-        new_document = tomlkit.document()
-
-        # handle the active_profile key that appears at the top:
-        if self.profile != "__top_level__":
-            if update_active_profile:
-                active_profile = self.profile
-            else:
-                active_profile = self.original_toml.get("active_profile", None)
-        else:
-            active_profile = self.get("active_profile", None)
-        if active_profile is not None:
-            new_document["active_profile"] = active_profile
-
-        # add key-value pairs at the top level if this is the top-level profile:
-        if self.profile == "__top_level__":
-            for k, v in self.props.items():
-                if k != "active_profile":
-                    new_document[k] = v
-
-        active_profile_table = tomlkit.table()
-        for k, v in self.props.items():
-            active_profile_table[k] = v
-
-        original_top_level_profile = None
-
-        profiles = tomlkit.table(is_super_table=True)
-
-        def adjust_trailing_newlines(item, action):
-            match item.__class__.__name__:
-                case "TOMLDocument":
-                    body = getattr(item, "body", None)
-                    if body is None or len(body) == 0:
-                        return
-                    adjust_trailing_newlines(body[-1], action)
-                case "tuple":
-                    if len(item) < 2:
-                        return
-                    _, value = item
-                    adjust_trailing_newlines(value, action)
-                case "Container":
-                    body = getattr(item, "body", None)
-                    if body is None or len(body) == 0:
-                        return
-                    adjust_trailing_newlines(body[-1], action)
-                case "Table":
-                    value = getattr(item, "value", None)
-                    if value is None:
-                        return
-                    adjust_trailing_newlines(value, action)
-                case "Whitespace":
-                    action(item)
-
-        def ensure_profiles_added():
-            if not new_document.get("profile"):
-                # this hack is necessary because tomlkit sometimes
-                # inserts spurious newlines just before the profile
-                # section
-                # related: https://github.com/sdispater/tomlkit/issues/48
-                def trim_one(item):
-                    if item.value.endswith("\n"):
-                        item._s = item.value[:-1]
-                adjust_trailing_newlines(new_document, trim_one)
-                new_document.add("profile", profiles)
-
-        # fill in from the original TOML file contents:
-        for key, value in self.original_toml.items():
-            # the "active-profile" check is here to make the migration smooth
-            # from when we used "active-profile" instead of "active_profile"
-            if key == "profile":
-                ensure_profiles_added()
-                for profile in value:
-                    if profile == active_profile:
-                        profiles.add(profile, active_profile_table)
-                    else:
-                        profiles.add(profile, value[profile])
-            if key in new_document or key == "active_profile":
-                continue
-            elif key in all_prop_keys:
-                ensure_profiles_added()
-                if not original_top_level_profile:
-                    k = 0
-                    while True:
-                        original = "original" if k == 0 else f"original-{k}"
-                        if self.original_toml.get("profile", {}).get(original) is None:
-                            break
-                        k += 1
-                    original_top_level_profile = original
-                    profiles.add(original_top_level_profile, tomlkit.table())
-                original_profile = cast(Table, profiles.get(original_top_level_profile))
-                original_profile.add(key, value)
-            else:
-                # preserve all keys unrelated to the profiles:
-                new_document[key] = value
-
-        if active_profile is not None:
-            ensure_profiles_added()
-            if profiles.get(active_profile) is None:
-                profiles.add(active_profile, active_profile_table)
-
-        with open(CONFIG_FILE, "w") as f:
-            f.write(new_document.as_string())
-
     def _fill_in_with_defaults(self, defaults: Dict[str, Any], **kwargs):
         props = {k: v for k, v in kwargs.items() if k in defaults}
         self.update({
             **defaults,
             **self.props,
             **props,
-        }, save_progress=True)
+        })
 
     def fill_in_with_azure_defaults(self, **kwargs):
         self._fill_in_with_defaults(azure_default_props, **kwargs)
 
     def fill_in_with_snowflake_defaults(self, **kwargs):
         self._fill_in_with_defaults(snowflake_default_props, **kwargs)
 
@@ -507,7 +501,19 @@
         if platform == "azure":
             self.fill_in_with_azure_defaults()
         elif platform == "snowflake":
             self.fill_in_with_snowflake_defaults()
         else:
             self.set("platform", "snowflake")
             self.fill_in_with_snowflake_defaults()
+
+#--------------------------------------------------
+# helpers
+#--------------------------------------------------
+
+def items_with_dots(d: dict):
+    for k, v in d.items():
+        if isinstance(v, dict):
+            for sub_k, sub_v in items_with_dots(v):
+                yield f"{k}.{sub_k}", sub_v
+        else:
+            yield k, v
```

### Comparing `relationalai-0.2.7/src/relationalai/clients/snowflake.py` & `relationalai-0.2.8/src/relationalai/clients/snowflake.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import textwrap
 from railib.api import TransactionAsyncResponse, poll_with_specified_overhead, _parse_metadata_proto
 import requests
 import snowflake.connector
 import pyarrow as pa
 import pandas as pd
 import time
+import decimal
 from snowflake.connector import SnowflakeConnection
 
 from .. import debugging
 
 from typing import Any, Dict, Iterable, Tuple, List, cast
 import base64
 
@@ -25,21 +26,23 @@
 from ..clients.config import Config
 from ..clients.client import Client, ResourceProvider
 from .. import dsl, rel, metamodel as m
 from ..errors import Errors, RAIException
 from .. import std
 import re
 from concurrent.futures import ThreadPoolExecutor
+from datetime import datetime
 
 #--------------------------------------------------
 # Constants
 #--------------------------------------------------
 
 USE_EXEC_ASYNC = True
 VALID_POOL_STATUS = ["ACTIVE", "IDLE", "SUSPENDED"]
+TXN_SQL_FIELDS = ["id", "database_name", "state", "abort_reason", "read_only", "created_by", "created_on", "finished_at", "duration"]
 VALID_ENGINE_STATES = ["READY", "PENDING"]
 COMPUTE_POOL_MAP = {
     "STANDARD_1": "XS",
     "CPU_X64_XS": "XS",
     "CPU_X64_S": "XS",
     "CPU_X64_M": "S",
     "HIGHMEM_X64_S": "M",
@@ -563,17 +566,28 @@
         if len(results.results):
             for result in results.results:
                 types = [t for t in result["relationId"].split("/") if t != "" and not t.startswith(":")]
                 result_frame:DataFrame = result["table"].to_pandas()
                 for i, col in enumerate(result_frame.columns):
                     if "UInt128" in types[i]:
                         result_frame[col] = result_frame[col].apply(lambda x: base64.b64encode(x.tobytes()).decode()[:-2])
-                    if types[i] == "Dates.DateTime":
+                    elif "FixedDecimal" in types[i]:
+                        decimal_info = re.search(r"FixedDecimal\{Int(\d+), (\d+)\}", types[i])
+                        if decimal_info:
+                            bits = int(decimal_info.group(1))
+                            scale = int(decimal_info.group(2))
+                            if bits == 128:
+                                result_frame[col] = result_frame[col].apply(lambda x: (decimal.Decimal(str((int(x[1]) << 64) + int(x[0]))) if x[1] > 0 else decimal.Decimal(str(x[0]))) / (10 ** scale))
+                            else:
+                                result_frame[col] = result_frame[col].apply(lambda x: decimal.Decimal(str(x)) / (10 ** scale))
+                    elif "Int128" in types[i]:
+                        result_frame[col] = result_frame[col].apply(lambda x: (int(x[1]) << 64) + int(x[0]) if x[1] > 0 else x[0])
+                    elif types[i] == "Dates.DateTime":
                         result_frame[col] = pd.to_datetime(result_frame[col] - UNIXEPOCH, unit="ms")
-                    if types[i] == "Dates.Date":
+                    elif types[i] == "Dates.Date":
                         result_frame[col] = pd.to_datetime(result_frame[col] * MILLISECONDS_PER_DAY - UNIXEPOCH, unit="ms")
                 ret_cols = task.return_cols()
                 if len(ret_cols) and len(result_frame.columns) == len(ret_cols):
                     result_frame.columns = task.return_cols()[0:len(result_frame.columns)]
                 result["table"] = result_frame
                 if ":output" in result["relationId"]:
                     data_frame = pd.concat([data_frame, result_frame], ignore_index=True)
@@ -595,28 +609,61 @@
             return self._format_results_async(results, task)
         else:
             return self._format_results_sync(results, task)
 
     #--------------------------------------------------
     # Transactions
     #--------------------------------------------------
+    def txns_to_dicts(self, transactions):
+        if not transactions:
+            return []
+        map = {"database_name": "database"}
+        mapped = [map.get(f, f) for f in TXN_SQL_FIELDS]
+        return [dict(zip(mapped, row)) for row in transactions]
+
+    def get_transaction(self, transaction_id):
+        results = self._exec(f"CALL {APP_NAME}.api.get_transaction(%s);", [transaction_id])
+        if not results:
+            return None
+        txn = self.txns_to_dicts(results.fetchall())[0]
+        created_on = txn.get("created_on")
+        finished_at = txn.get("finished_at")
+        if created_on:
+            if finished_at:
+                txn['duration'] = finished_at - created_on
+            else:
+                tz_info = created_on.tzinfo
+                txn['duration'] = datetime.now(tz_info) - created_on
+        return txn
+
+    def list_transactions(self, **kwargs):
+        id = kwargs.get("id")
+        only_active = kwargs.get("only_active", False)
+        state = kwargs.get("state", None)
+        where_clause_arr = []
+
+        if id:
+            where_clause_arr.append(f"id = '{id}'")
+        if state:
+            where_clause_arr.append(f"state = '{state.upper()}'")
+        else:
+            if only_active:
+                where_clause_arr.append("state in ('CREATED', 'RUNNING', 'PENDING')")
+
+        if len(where_clause_arr):
+            where_clause = f'WHERE {" AND ".join(where_clause_arr)}'
+        else:
+            where_clause = ""
 
-    def list_transactions(self, limit:int, only_active=False):
-        where = "WHERE state <> 'COMPLETED'" if only_active else ""
-        field_names = [
-            "id", "database_name", "state", "abort_reason", "read_only", "created_by",
-            "duration", "created_on", "finished_at"
-        ]
-        sql_fields = ", ".join([f.upper() for f in field_names])
-        results = self._exec(f"select {sql_fields} from {APP_NAME}.api.transactions {where} LIMIT %s", [limit])
+        limit = kwargs.get("limit", 100)
+        sql_fields = ", ".join([f.upper() for f in TXN_SQL_FIELDS])
+        results = self._exec(f"select {sql_fields} from {APP_NAME}.api.transactions {where_clause} LIMIT %s", [limit])
         if not results:
             return []
-        map = {"database_name": "database"}
-        mapped = [map.get(f, f) for f in field_names]
-        return [dict(zip(mapped, row)) for row in results.fetchall()]
+        return self.txns_to_dicts(results.fetchall())
 
     def cancel_transaction(self, transaction_id):
         self._exec(f"CALL {APP_NAME}.api.CANCEL_TRANSACTION(%s);", [transaction_id])
         if transaction_id in self._pending_transactions:
             self._pending_transactions.remove(transaction_id)
 
     def cancel_pending_transactions(self):
@@ -913,9 +960,12 @@
         def make_identity(x..., z):
             exists((u) | hash128({x...}, x..., u) and
             hash_value_uint128_convert(u, z))
 
         @inline
         def pyrel_default({F}, c, k..., v):
             F(k..., v) or (not F(k..., _) and v = c)
+
+        @inline
+        def pyrel_unwrap(x in UInt128, y): y = x
     """))
     return dsl.Graph(client, name)
```

### Comparing `relationalai-0.2.7/src/relationalai/clients/test.py` & `relationalai-0.2.8/src/relationalai/clients/test.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/src/relationalai/clients/types.py` & `relationalai-0.2.8/src/relationalai/clients/types.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/src/relationalai/loaders/csv.py` & `relationalai-0.2.8/src/relationalai/loaders/csv.py`

 * *Files 5% similar despite different names*

```diff
@@ -86,44 +86,46 @@
 
     return ExternalRow(items, [c for c in df.columns])
 
 class CSVLoader(Loader):
     """Load CSV files and URLs in RAI DB using `load_csv`."""
     type = "csv"
 
-    def load(self, provider: ResourceProvider, model: str, source: ImportSource, *, schema: Schema, syntax: Syntax):
+    def load(self, provider: ResourceProvider, model: str, source: ImportSource, *, schema: Schema|None = None, syntax: Syntax|None = None, integration: dict|None = None):
         assert isinstance(source, ImportSourceFile), "CSV Loader can only load from files and URLs, not {type(source).__name__}"
+        schema = schema or {}
+        syntax = syntax or {}
 
         id = compute_str_hash(source.raw_path)
-        prefix = f"""def config[:path]: "{source.raw_path}" """
+        prefix = f"""def config[:path]: raw"{source.raw_path}" """
         inputs = None
 
         if not source.is_url():
             with open(source.raw_path, "r") as csv_file:
                 data = csv_file.read()
 
             id = compute_file_hash(source.raw_path)
             prefix = "def config[:data]: data"
             inputs = {"data": data}
 
         relation = sanitize(source.name)
-        schema = schema or {}
 
         for key in ["delim", "quotechar", "escapechar"]:
             if syntax.get(key, None) and not isinstance(syntax[key], Char):
                 syntax[key] = Char(syntax[key])
 
         q = f"""
         declare {relation}
         def delete[:{relation}]: {relation}
         def delete[:__resource, k, "{relation}"]: __resource[k, "{relation}"]
 
         {prefix}
         {emit_nested_relation("config[:syntax, ", cast(dict, syntax), api._syntax_options)}
         {emit_nested_relation("config[:schema, ", {col: TYPE_TO_REL_SCHEMA.get(type, "string") for col, type in schema.items()})}
+        {emit_nested_relation("config[:integration, ", integration) if integration else ""}
         {emit_nested_relation("insert[:__resource, ", {
         "id": (relation, id),
         "type": (relation, self.type),
         "name": (relation, source.name)
         })}
         def insert[:__resource, :schema]: ("{relation}", config[:schema])
         def insert[:{relation}]: load_csv[config]
```

### Comparing `relationalai-0.2.7/src/relationalai/loaders/loader.py` & `relationalai-0.2.8/src/relationalai/loaders/loader.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/src/relationalai/loaders/types.py` & `relationalai-0.2.8/src/relationalai/loaders/types.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/src/relationalai/std/aggregates.py` & `relationalai-0.2.8/src/relationalai/std/aggregates.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/src/relationalai/std/graphs.py` & `relationalai-0.2.8/src/relationalai/std/graphs.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from collections import defaultdict
 from copy import deepcopy
+import textwrap
 from typing import Any
 from .. import dsl, errors
 import gravis as gv
 from . import rel, Vars
 
 #--------------------------------------------------
 # Errors
@@ -29,59 +30,74 @@
         invalid_param(param, f"must be between {min} and {max}")
 
 def positive(param:str, value):
     if value <= 0:
         invalid_param(param, "must be positive")
 
 #--------------------------------------------------
+# Helpers
+#--------------------------------------------------
+
+def unwrap(v):
+    if v is None:
+        return None
+    return rel.pyrel_default(rel.pyrel_unwrap, v, v)
+
+#--------------------------------------------------
 # Algos
 #--------------------------------------------------
 
 class Compute:
     def __init__(self, graph:'Graph'):
         self._graph = graph
         self._lib = dsl.global_ns.graphlib
 
     def _config(self, **kwargs):
         return dsl.InlineRelation(self._graph.model, [
             *[(dsl.Symbol(k), v) for k, v in kwargs.items()],
         ])
 
+    def _lookup(self, v):
+        res = Vars(1)
+        lookup_rel = getattr(rel, f"{self._graph._graph_ref()}_lookup")
+        rel.pyrel_default(lookup_rel, v, v, res)
+        return res
+
     # --------------------------------------------------
     # Degree
     # --------------------------------------------------
 
     def degree(self, node, weight=None):
         if not weight:
-            return self._lib.degree(self._graph, node)
-        return self._lib.weighted_degree(self._graph, node)
+            return self._lib.degree(self._graph, unwrap(node))
+        return self._lib.weighted_degree(self._graph, unwrap(node))
 
     def min_degree(self):
         return self._lib.min_degree(self._graph)
 
     def max_degree(self):
         return self._lib.max_degree(self._graph)
 
     def avg_degree(self):
         return self._lib.average_degree(self._graph)
 
     def indegree(self, node):
-        return self._lib.indegree(self._graph, node)
+        return self._lib.indegree(self._graph, unwrap(node))
 
     def min_indegree(self):
         return self._lib.min_indegree(self._graph)
 
     def max_indegree(self):
         return self._lib.max_indegree(self._graph)
 
     def avg_indegree(self):
         return self._lib.average_indegree(self._graph)
 
     def outdegree(self, node):
-        return self._lib.outdegree(self._graph, node)
+        return self._lib.outdegree(self._graph, unwrap(node))
 
     def min_outdegree(self):
         return self._lib.min_outdegree(self._graph)
 
     def max_outdegree(self):
         return self._lib.max_outdegree(self._graph)
 
@@ -93,25 +109,25 @@
     # --------------------------------------------------
 
     def num_nodes(self):
         return self._lib.num_nodes(self._graph)
 
     def num_edges(self):
         return self._lib.num_edges(self._graph)
-    
+
     # --------------------------------------------------
     # Distance
     # --------------------------------------------------
-    
+
     def distance(self, node1, node2):
-        return self._lib.distance(self._graph, node1, node2)
-    
+        return self._lib.distance(self._graph, unwrap(node1), unwrap(node2))
+
     def weighted_distance(self, node1, node2):
-        return self._lib.weighted_distance(self._graph, node1, node2)
-    
+        return self._lib.weighted_distance(self._graph, unwrap(node1), unwrap(node2))
+
     def diameter_range(self):
         min, max = Vars(2)
         self._lib.diameter_range(self._graph, "min", min)
         self._lib.diameter_range(self._graph, "max", max)
         return (min, max)
 
     # --------------------------------------------------
@@ -125,95 +141,116 @@
                 self._lib.is_connected(self._graph)
                 v.add(True)
             with model.scope():
                 v.add(False)
         return v
 
     def reachable_from(self, node: dsl.Producer) -> dsl.Expression:
-        return self._lib.transitive_closure(self._graph, node)
+        return self._lib.transitive_closure(self._graph, unwrap(node))
 
     def is_reachable(self, node1: dsl.Producer, node2: dsl.Producer) -> dsl.Expression:
         model = self._graph.model
         with model.ordered_choice() as v:
             with model.scope():
-                self._lib.transitive_closure(self._graph, node1, node2)
+                self._lib.transitive_closure(self._graph, unwrap(node1), unwrap(node2))
                 v.add(True)
             with model.scope():
                 v.add(False)
         return v
 
     # --------------------------------------------------
     # Triangles
     # --------------------------------------------------
 
     def num_triangles(self, node=None):
         if node is None:
             return self._lib.num_triangles(self._graph)
-        return self._lib.triangle_count(self._graph, node)
+        return self._lib.triangle_count(self._graph, unwrap(node))
 
     def is_triangle(self, node1, node2, node3):
         model = dsl.get_graph()
         with model.ordered_choice() as v:
             with model.scope():
-                self._lib.triangle(self._graph, node1, node2, node3)
+                self._lib.triangle(self._graph, unwrap(node1), unwrap(node2), unwrap(node3))
                 v.add(True)
             with model.scope():
                 v.add(False)
         return v
 
     def triangles(self, node=None):
         # If no node is provided, return all triangles in the graph,
         # unique up to ordering of the nodes.
         if node is None:
             x, y, z = Vars(3)
             self._lib.unique_triangle(self._graph, x, y, z)
-            return (x, y, z)
+            lx = self._lookup(x)
+            ly = self._lookup(y)
+            lz = self._lookup(z)
+            return (lx, ly, lz)
         # If a node is provided, return all triangles that include that node,
         # unique up to order of the nodes.
         x, y = Vars(2)
         model = dsl.get_graph()
+        node = unwrap(node)
         with model.union(dynamic=True) as t:
             for (a, b, c) in ([node, x, y], [x, node, y], [x, y, node]):
                 with model.scope():
                     self._lib.unique_triangle(self._graph, a, b, c)
                     t.add(node, a=a, b=b, c=c)
-        return (t.a, t.b, t.c)
+        la = self._lookup(t.a)
+        lb = self._lookup(t.b)
+        lc = self._lookup(t.c)
+        return (la, lb, lc)
+
+    # --------------------------------------------------
+    # Clustering
+    # --------------------------------------------------
+
+    def local_clustering_coefficient(self, node):
+        if not self._graph.undirected:
+            invalid_param("graph", "must be undirected")
+        return self._lib.local_clustering_coefficient(self._graph, unwrap(node))
+
+    def avg_clustering_coefficient(self):
+        if not self._graph.undirected:
+            invalid_param("graph", "must be undirected")
+        return self._lib.average_clustering_coefficient(self._graph)
 
     # --------------------------------------------------
     # Link Prediction
     # --------------------------------------------------
 
     def adamic_adar(self, node1, node2):
-        return self._lib.adamic_adar(self._graph, node1, node2)
+        return self._lib.adamic_adar(self._graph, unwrap(node1), unwrap(node2))
 
     def preferential_attachment(self, node1, node2):
-        return self._lib.preferential_attachment(self._graph, node1, node2)
+        return self._lib.preferential_attachment(self._graph, unwrap(node1), unwrap(node2))
 
     def common_neighbor(self, node1, node2):
-        return self._lib.common_neighbor(self._graph, node1, node2)
+        return self._lib.common_neighbor(self._graph, unwrap(node1), unwrap(node2))
 
     # --------------------------------------------------
     # Similarity
     # --------------------------------------------------
 
     def cosine_similarity(self, node1, node2):
         if not self._graph.undirected:
             invalid_param("graph", "must be undirected")
-        return self._lib.cosine_similarity(self._graph, node1, node2)
+        return self._lib.cosine_similarity(self._graph, unwrap(node1), unwrap(node2))
 
     def weighted_cosine_similarity(self, node1, node2):
         if not self._graph.undirected:
             invalid_param("graph", "must be undirected")
-        return self._lib.weighted_cosine_similarity(self._graph, node1, node2)
+        return self._lib.weighted_cosine_similarity(self._graph, unwrap(node1), unwrap(node2))
 
     def jaccard_similarity(self, node1, node2):
-        return self._lib.jaccard_similarity(self._graph, node1, node2)
+        return self._lib.jaccard_similarity(self._graph, unwrap(node1), unwrap(node2))
 
     def weighted_jaccard_similarity(self, node1, node2):
-        return self._lib.weighted_jaccard_similarity(self._graph, node1, node2)
+        return self._lib.weighted_jaccard_similarity(self._graph, unwrap(node1), unwrap(node2))
 
     # --------------------------------------------------
     # Centrality
     # --------------------------------------------------
 
     def pagerank(self, node, damping_factor=0.85, tolerance=1e-6, max_iter=20):
         between("damping_factor", damping_factor, 0, 1)
@@ -222,51 +259,52 @@
 
         config = self._config(
             graph=self._graph,
             damping_factor=damping_factor,
             tolerance=tolerance,
             max_iter=max_iter,
         )
-        return self._lib.pagerank(config, node)
+        return self._lib.pagerank(config, unwrap(node))
 
     def betweenness_centrality(self, node):
-        return self._lib.betweenness_centrality(self._graph, node)
+        return self._lib.betweenness_centrality(self._graph, unwrap(node))
 
     def degree_centrality(self, node):
-        return self._lib.degree_centrality(self._graph, node)
+        return self._lib.degree_centrality(self._graph, unwrap(node))
 
     def eigenvector_centrality(self, node):
         if not self._graph.undirected:
             invalid_param("graph", "must be undirected")
-        return self._lib.eigenvector_centrality(self._graph, node)
+        return self._lib.eigenvector_centrality(self._graph, unwrap(node))
 
     def weighted_degree_centrality(self, node):
-        return self._lib.weighted_degree_centrality(self._graph, node)
+        return self._lib.weighted_degree_centrality(self._graph, unwrap(node))
 
     # --------------------------------------------------
     # Community Detection
     # --------------------------------------------------
 
     def weakly_connected_component(self, node):
-        return self._lib.weakly_connected_component(self._graph, node)
+        component = self._lib.weakly_connected_component(self._graph, unwrap(node))
+        return self._lookup(component)
 
     def triangle_community(self, node):
-        return self._lib.triangle_community(self._graph, node)
+        return self._lib.triangle_community(self._graph, unwrap(node))
 
     def infomap(self, node):
         config = self._config(graph=self._graph)
-        return self._lib.infomap(config, node)
+        return self._lib.infomap(config, unwrap(node))
 
     def louvain(self, node):
         config = self._config(graph=self._graph)
-        return self._lib.louvain(config, node)
+        return self._lib.louvain(config, unwrap(node))
 
     def label_propagation(self, node):
         config = self._config(graph=self._graph)
-        return self._lib.label_propagation(config, node)
+        return self._lib.label_propagation(config, unwrap(node))
 
 #--------------------------------------------------
 # Edge
 #--------------------------------------------------
 
 class EdgeInstance:
     def __init__(self, edge:'Edge', from_:Any, to:Any, kwargs:dict={}):
@@ -343,46 +381,63 @@
         self.undirected = undirected
         self.weighted = weighted
         self.default_weight=default_weight
         self._last_fetch = None
 
         graph_type = "::graphlib::undirected_graph" if undirected else "::graphlib::directed_graph"
         if weighted:
-            create_graph = f"""{graph_type}[{self.Edge._prop("weight")._name}]"""
+            unwrapped = f"""
+            def {self.Edge._prop("weight")._name}_unwrapped(au, bu, w): {{
+                exists((a, b) |
+                    {self.Edge._prop("weight")._name}(a, b, w) and
+                    pyrel_default(pyrel_unwrap, a, a, au) and
+                    pyrel_default(pyrel_unwrap, b, b, bu)
+                )
+            }}
+            """
+            create_graph = f"""{graph_type}[{self.Edge._prop("weight")._name}_unwrapped]"""
         else:
-            create_graph = f"{graph_type}[{self.Edge._type._name}]"
+            unwrapped = f"""
+            def {self.Edge._type._name}_unwrapped(au, bu): {{
+                exists((a, b) |
+                    {self.Edge._type._name}(a, b) and
+                    pyrel_default(pyrel_unwrap, a, a, au) and
+                    pyrel_default(pyrel_unwrap, b, b, bu)
+                )
+            }}
+            """
+            create_graph = f"{graph_type}[{self.Edge._type._name}_unwrapped]"
 
         node_def = ""
         if with_isolated_nodes:
-            node_def = f"def {self._graph_ref()}[:node]: {{{self.Node._type.name}}}"
+            node_def = f"def {self._graph_ref()}[:node]: {{pyrel_unwrap[{self.Node._type.name}]}}"
 
-        self.model.install_raw(f"""
+        self.model.install_raw(textwrap.dedent(f"""
         declare {self.Node._type.name}
         declare {self.Edge._type._name}
+        {unwrapped}
+        @inline
+        def {self._graph_ref()}_lookup(uw, orig): {{ {self.Node._type.name}(orig) and pyrel_unwrap(orig, uw) }}
+
         {f"declare {self.Edge._prop('weight')._name}" if weighted else ""}
         def {self._graph_ref()} {{{create_graph}}}
         {node_def}
-        @inline
-        def {self._lib_ref()} {{rel[:graphlib, {self._graph_ref()}]}}
-        """)
+        """))
 
         # Add a rule that makes all nodes used in edges are also added to
         # the nodes relation
         with model.rule():
             a, b = dsl.Vars(2)
             self.Edge._type(a, b)
             self.Node.add(a)
             self.Node.add(b)
 
     def _graph_ref(self):
         return f"graph{self.id}"
 
-    def _lib_ref(self):
-        return f"graphlib{self.id}"
-
     def _to_var(self):
         return getattr(rel, self._graph_ref())._to_var()
 
     def _is_weighted(self):
         return self.weighted
         # return self.edges._is_weighted()
```

### Comparing `relationalai-0.2.7/src/relationalai/std/math.py` & `relationalai-0.2.8/src/relationalai/std/math.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,70 +1,107 @@
 import numbers
 
 from .. import dsl
 
 # Custom number type
-Number = numbers.Number | dsl.Producer
+_Number = numbers.Number | dsl.Producer
 
 # NOTE: Right now, common contains all Rel stdlib relations.
 # If the stdlib is split into multiple namespaces, this will have to be updated.
 _math_ns = dsl.global_ns.std.common
 
 
 # ------------------------------
 # Basics
 # ------------------------------
 
-def abs(value: Number) -> dsl.Expression:
+def abs(value: _Number) -> dsl.Expression:
     return _math_ns.abs(value)
 
-def isclose(x: Number, y: Number, tolerance: Number = 1e-9) -> dsl.Expression:
+def isclose(x: _Number, y: _Number, tolerance: _Number = 1e-9) -> dsl.Expression:
     return _math_ns.approx_eq(tolerance, x, y)
 
-def cbrt(value: Number) -> dsl.Expression:
+def cbrt(value: _Number) -> dsl.Expression:
     return _math_ns.cbrt(value)
 
-def log(x: Number, base: Number | None = None) -> dsl.Expression:
+def log(x: _Number, base: _Number | None = None) -> dsl.Expression:
     if isinstance(x, numbers.Number) and x <= 0:
         raise ValueError("Cannot take the logarithm of a negative number")
     if base is None:
         return _math_ns.natural_log(x)
     return _math_ns.log(base, x)
 
-def sign(x: Number) -> dsl.Expression:
+def sign(x: _Number) -> dsl.Expression:
     return _math_ns.sign(x)
 
-def sqrt(value: Number) -> dsl.Expression:
+def sqrt(value: _Number) -> dsl.Expression:
     if isinstance(value, numbers.Number) and value < 0:
         raise ValueError("Cannot take the square root of a negative number")
     return _math_ns.sqrt(value)
 
-def trunc_divide(numerator: Number, denominator: Number) -> dsl.Expression:
+def trunc_divide(numerator: _Number, denominator: _Number) -> dsl.Expression:
     return _math_ns.trunc_divide(numerator, denominator)
 
 
 # ------------------------------
+# Trigonometry
+# ------------------------------
+
+def acos(value: _Number) -> dsl.Expression:
+    return _math_ns.acos(value)
+
+def asin(value: _Number) -> dsl.Expression:
+    return _math_ns.asin(value)
+
+def atan(value: _Number) -> dsl.Expression:
+    return _math_ns.atan(value)
+
+def cos(value: _Number) -> dsl.Expression:
+    return _math_ns.cos(value)
+
+def degrees(radians: _Number) -> dsl.Expression:
+    return _math_ns.rad2deg(radians)
+
+def radians(degrees: _Number) -> dsl.Expression:
+    return _math_ns.deg2rad(degrees)
+
+def sin(value: _Number) -> dsl.Expression:
+    return _math_ns.sin(value)
+
+def tan(value: _Number) -> dsl.Expression:
+    return _math_ns.tan(value)
+
+
+# ------------------------------
 # Rounding
 # ------------------------------
 
-def ceil(value: Number) -> dsl.Expression:
+def ceil(value: _Number) -> dsl.Expression:
     return _math_ns.ceil(value)
 
-def floor(value: Number) -> dsl.Expression:
+def floor(value: _Number) -> dsl.Expression:
     return _math_ns.floor(value)
 
 
 # ------------------------------
 # Exports
 # ------------------------------
 
 __all__ = [
     "abs",
+    "acos",
+    "asin",
+    "atan",
     "isclose",
     "cbrt",
+    "cos",
+    "degrees",
     "log",
+    "radians",
     "sign",
+    "sin",
     "sqrt",
+    "tan",
     "trunc_divide",
     "ceil",
     "floor",
 ]
```

### Comparing `relationalai-0.2.7/src/relationalai/std/strings.py` & `relationalai-0.2.8/src/relationalai/std/strings.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/src/relationalai/tools/cli.py` & `relationalai-0.2.8/src/relationalai/tools/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,48 +4,56 @@
 import io
 import re
 import shlex
 from typing import Sequence, cast, Any, List
 from click.core import Context
 from click.formatting import HelpFormatter
 import requests
-import datetime
 
 from relationalai.clients import azure
 from relationalai.errors import RelQueryError
 from relationalai.loaders.types import LoadType, UnsupportedTypeError
 from relationalai.loaders.csv import CSVLoader
 from relationalai.loaders.loader import Loader, rel_schema_to_type
+from relationalai.util.constants import (
+    DEFAULT_PROFILE_NAME,
+    PARTIAL_PROFILE_NAME,
+    TOP_LEVEL_PROFILE_NAME,
+)
+from relationalai.util.format import humanized_bytes, humanized_duration
 from ..clients.types import ImportSource, ImportSourceFile, ImportSourceTable
 from ..clients.client import ResourceProvider
 from .. import Resources
 import rich
 from rich.console import Console
 from rich import box as rich_box
 from rich.table import Table
 from ..tools import debugger as deb
 from ..clients import config, snowflake
 from ..clients.config import (
     FIELD_PLACEHOLDER,
     CONFIG_FILE,
     ConfigFile,
+    ConfigStore,
     all_configs_including_legacy,
     get_from_snowflake_connections_toml,
     azure_default_props,
+    map_toml_value,
     snowflake_default_props,
 )
 from InquirerPy.base.control import Choice
 from InquirerPy.validator import ValidationError
 
 import os
 import sys
 import click
 from pathlib import Path
 from .cli_controls import divider, Spinner
 from . import cli_controls as controls
+from datetime import datetime, timedelta
 
 #--------------------------------------------------
 # Constants
 #--------------------------------------------------
 
 CONTEXT_SETTINGS = dict(help_option_names=['-h', '--help'])
 ENGINE_SIZES = ["XS", "S", "M", "L", "XL"]
@@ -115,14 +123,23 @@
         sys.exit(1)
 
 def coming_soon():
     rich.print("[yellow]This isn't quite ready yet, but it's coming soon!")
     divider()
     sys.exit(1)
 
+def issue_top_level_profile_warning():
+    rich.print("[yellow]Warning: Using a top-level profile is not recommended")
+    rich.print("[yellow]Consider naming the profile by adding \\[profile.<name>] to your raiconfig.toml file\n")
+    rich.print("[yellow]Example:")
+    rich.print("[yellow]\\[profile.default]")
+    rich.print("[yellow]platform = \"snowflake\"")
+    rich.print("[yellow]account = ...")
+    divider()
+
 def ensure_config(profile:str|None=None) -> config.Config:
     cfg = get_config(profile)
     if not cfg.file_path:
         rich.print("[yellow bold]No configuration file found.")
         rich.print("To create one, run: [green bold]rai init[/green bold]")
         divider()
         sys.exit(1)
@@ -165,15 +182,15 @@
         # @NOTE: I couldn't find a sane way to access the --profile option from here, so insane it is.
         if "--profile" in sys.argv:
             ix = sys.argv.index("--profile") + 1
             if ix < len(sys.argv):
                 PROFILE = sys.argv[ix]
 
         profile = get_config().profile
-        if profile == "__top_level__":
+        if profile == TOP_LEVEL_PROFILE_NAME:
             profile = "[yellow bold]None[/yellow bold]" if not get_config().get("platform", "") else "[ROOT]"
 
         sio = io.StringIO()
         console = Console(file=sio, force_terminal=True)
         divider(console)
         console.print("[bold]Welcome to [green]RelationalAI![/bold]")
         console.print()
@@ -333,19 +350,18 @@
         "SnowSQL password:",
         default=cfg.get("password", ""),
         validator=EMPTY_STRING_REGEX.match,
         invalid_message="Password is required"
     )
     cfg.set("password", password)
 
-    rich.print("\n[dim]  Note: Account ID should look like: myorg-account123")
-    rich.print("[dim]  Details: https://docs.snowflake.com/en/user-guide/admin-account-identifier\n")
-    rich.print("[dim]  Alternatively, you can log in to Snowsight, copy the URL, and paste it here.")
-    rich.print("[dim]  Example: https://app.snowflake.com/myorg/account123/worksheets\n")
-
+    rich.print("\n  Note: Account ID should look like: myorg-account123")
+    rich.print("  Details: https://docs.snowflake.com/en/user-guide/admin-account-identifier\n")
+    rich.print("  Alternatively, you can log in to Snowsight, copy the URL, and paste it here.")
+    rich.print("  Example: https://app.snowflake.com/myorg/account123/worksheets\n")
     account_or_url = controls.text(
         "Snowflake account:",
         default=cfg.get("account", ""),
         validator=EMPTY_STRING_REGEX.match,
         invalid_message="Account is required"
     )
     account = account_from_url(account_or_url)
@@ -364,15 +380,15 @@
         password=password,
         account=account,
     )
 
 def filter_profiles_by_platform(config:ConfigFile, platform:str):
     filtered_config = {}
     for profile, props in config.get_combined_profiles().items():
-        if profile == "__top_level__":
+        if profile == TOP_LEVEL_PROFILE_NAME:
             continue
         if props.get("platform") == platform or (
             props.get("platform") is None
             and platform == "azure"
         ):
             filtered_config[profile] = props
     return filtered_config
@@ -417,18 +433,19 @@
     if not profile:
         return
     cfg.profile = profile
     cfg.update(sf_config[profile])
     return True
 
 def role_flow(provider:ResourceProvider, cfg:config.Config):
+    roles = cast(snowflake.Resources, provider).list_roles()
     result = controls.fuzzy_with_refetch(
             "Select a role:",
             "roles",
-            lambda: [r["name"] for r in cast(snowflake.Resources, provider).list_roles()],
+            lambda: [r["name"] for r in roles],
             default=cfg.get("role", None),
         )
     if isinstance(result, Exception):
         return
     else:
         role = result
     cfg.set("role", role or FIELD_PLACEHOLDER)
@@ -463,33 +480,34 @@
 
 def spcs_flow(provider: ResourceProvider, cfg: config.Config):
     role_flow(provider, cfg)
     warehouse_flow(provider, cfg)
     rai_app_flow(provider, cfg)
 
 def engine_flow(provider:ResourceProvider, cfg:config.Config):
-    app_name = cfg.get("rai_app_name", None)
-    if not app_name:
-        rich.print("[yellow]App name is required for engine selection. Skipping step.\n")
-        return
-    warehouse = cfg.get("warehouse", None)
-    if not warehouse:
-        rich.print("[yellow]Warehouse is required for engine selection. Skipping step.\n")
-        return
+    if provider.config.get("platform") == "snowflake":
+        app_name = cfg.get("rai_app_name", None)
+        if not app_name:
+            rich.print("[yellow]App name is required for engine selection. Skipping step.\n")
+            raise Exception("App name is required for engine selection")
+        warehouse = cfg.get("warehouse", None)
+        if not warehouse:
+            rich.print("[yellow]Warehouse is required for engine selection. Skipping step.\n")
+            raise Exception("Warehouse is required for engine selection")
     result = controls.fuzzy_with_refetch(
         "Select an engine:",
         "engines",
-        lambda: ["Create a new engine"] + [engine.get("name") for engine in provider.list_engines()],
+        lambda: ["[CREATE A NEW ENGINE]"] + [engine.get("name") for engine in provider.list_engines()],
         default=cfg.get("engine", None),
     )
     if not result or isinstance(result, Exception):
-        return
+        raise Exception("Error fetching engines")
     else:
         engine = result
-    if result == "Create a new engine":
+    if result == "[CREATE A NEW ENGINE]":
         engine = create_engine_flow(cfg)
         rich.print("")
     cfg.set("engine", engine or FIELD_PLACEHOLDER)
 
 def gitignore_flow():
     current_dir = Path.cwd()
     prev_dir = None
@@ -506,33 +524,63 @@
                     if add_to_gitignore:
                         with open(gitignore_path, 'a') as gitignore_file:
                             gitignore_file.write(f"\n{CONFIG_FILE}")
                     return
         prev_dir = current_dir
         current_dir = current_dir.parent
 
-def save_flow(cfg:config.Config, check_for_profile_overwrite:bool=True, update_active_profile:bool=True):
-    if cfg.profile in cfg.get_profiles() and check_for_profile_overwrite:
+def is_valid_bare_toml_key(key):
+    pattern = re.compile(r'^[A-Za-z_][A-Za-z0-9_-]*$')
+    return bool(pattern.match(key))
+
+def name_profile_flow(cfg: config.Config):
+    if cfg.profile != TOP_LEVEL_PROFILE_NAME:
+        return
+    profile = controls.text("New name for this profile:", default=DEFAULT_PROFILE_NAME)
+    if not is_valid_bare_toml_key(profile):
+        rich.print(
+            "[yellow]Invalid profile name: should contain only alphanumeric characters, dashes, and hyphens"
+        )
+        return name_profile_flow(cfg)
+    config_store = ConfigStore()
+    if profile in config_store.get_profiles():
+        overwrite = controls.confirm(f"[yellow]Overwrite existing {profile} profile?")
+        if overwrite:
+            return profile
+        else:
+            return name_profile_flow(cfg)
+    return profile
+
+def save_flow(cfg:config.Config):
+    config_store = ConfigStore()
+    if cfg.profile != PARTIAL_PROFILE_NAME and cfg.profile in config_store.get_profiles():
         if not controls.confirm(f"Overwrite existing {cfg.profile} profile"):
             profile_name = controls.text("Profile name:")
             if profile_name:
                 cfg.profile = profile_name
             else:
-                save_flow(cfg, update_active_profile=update_active_profile)
+                save_flow(cfg)
                 return
-    cfg.save(update_active_profile=update_active_profile)
+    config_store.add_profile(cfg)
+    if cfg.profile != PARTIAL_PROFILE_NAME:
+        if config_store.num_profiles() == 1 or controls.confirm("Activate this profile?"):
+            config_store.change_active_profile(cfg.profile)
+    config_store.save()
 
 def init_flow():
     cfg = config.Config(fetch=False)
     try:
         cfg.clone_profile()
         rich.print("\n[dim]---------------------------------------------------\n")
         rich.print("[bold]Welcome to [green]RelationalAI!\n")
         rich.print("Press Control-S to skip a prompt\n")
 
+        if ConfigStore().get("platform"):
+            issue_top_level_profile_warning()
+
         platform = controls.fuzzy("Host platform:", choices=[SNOWFLAKE, AZURE])
         cfg.set("platform", {
             SNOWFLAKE: "snowflake",
             AZURE: "azure"
         }[platform])
 
         if platform == SNOWFLAKE:
@@ -546,34 +594,35 @@
 
         provider = get_resource_provider(None, cfg)
 
         rich.print()
         if platform == SNOWFLAKE:
             spcs_flow(provider, cfg)
         engine_flow(provider, cfg)
+        profile = name_profile_flow(cfg)
+        if profile:
+            cfg.profile = profile
         save_flow(cfg)
 
         gitignore_flow()
         rich.print("")
         rich.print(f"[green]✓ {CONFIG_FILE} saved!")
         rich.print("\n[dim]---------------------------------------------------\n")
     except Exception as e:
         rich.print("")
-        rich.print("[yellow bold]Initialization aborted!")
-        rich.print(f"[yellow]{e}")
+        rich.print("[yellow bold]Initialization aborted!\n")
         print(e.with_traceback(None))
         rich.print("")
 
         save = controls.confirm("Save partial config?")
         if save:
-            if cfg.profile == "__top_level__":
-                cfg.profile = "partial"
+            cfg.profile = PARTIAL_PROFILE_NAME
             rich.print("")
             cfg.fill_in_with_defaults()
-            save_flow(cfg, check_for_profile_overwrite=False, update_active_profile=False)
+            save_flow(cfg)
             gitignore_flow()
             rich.print(f"[yellow bold]✓ Saved partial {CONFIG_FILE} ({os.path.abspath(CONFIG_FILE)})")
 
         divider()
 
 #--------------------------------------------------
 # Profile switcher
@@ -581,32 +630,31 @@
 
 @cli.command(
     name="profile:switch",
     help="Switch to a different profile",
 )
 @click.option("--profile", help="Profile to switch to")
 def profile_switch(profile:str|None=None):
-    cfg = ensure_config()
-    profiles = list(cfg.get_profiles().keys())
+    config_store = ConfigStore()
+    profiles = list(config_store.get_profiles().keys())
     divider()
     if not profile:
         if len(profiles) == 0:
             rich.print("[yellow]No profiles found")
             divider()
             sys.exit(1)
         profile = controls.fuzzy("Select a profile:", profiles)
         divider()
     else:
         if profile not in profiles:
             rich.print(f"[yellow]Profile '{profile}' not found")
             divider()
             sys.exit(1)
-    cfg.original_toml["active_profile"] = profile
-    with open(CONFIG_FILE, "w") as f:
-        f.write(cfg.original_toml.as_string())
+    config_store.change_active_profile(profile)
+    config_store.save()
     rich.print(f"[green]✓ Switched to profile '{profile}'")
     divider()
 
 #--------------------------------------------------
 # Explain config
 #--------------------------------------------------
 
@@ -622,45 +670,49 @@
     "--all-profiles",
     help="Whether to show all profiles in config file",
     is_flag=True,
 )
 def config_explain(profile:str|None=None, all_profiles:bool=False):
     divider()
     cfg = ensure_config(profile)
+    config_store = ConfigStore()
+
+    if config_store.get("platform"):
+        issue_top_level_profile_warning()
 
     rich.print(f"[bold green]{cfg.file_path}")
     if os.getenv("RAI_PROFILE"):
         rich.print(f"[yellow]Environment variable [bold]RAI_PROFILE = {os.getenv('RAI_PROFILE')}[/bold]")
     rich.print("")
-    if cfg.profile != "__top_level__":
+    if cfg.profile != TOP_LEVEL_PROFILE_NAME:
         rich.print(f"[bold]\\[{cfg.profile}]")
 
-    for key, value in cfg.items():
-        if key == "active_profile" and cfg.profile != "__top_level__":
+    for key, value in cfg.items_with_dots():
+        if key == "active_profile" and cfg.profile != TOP_LEVEL_PROFILE_NAME:
             continue
-        rich.print(f"{key} = [cyan bold]{mask(key, value)}")
+        rich.print(f"{key} = [cyan bold]{map_toml_value(mask(key, value))}")
 
     platform = cfg.get("platform", "snowflake")
     defaults = snowflake_default_props if platform == "snowflake" else azure_default_props
 
     for key, value in defaults.items():
         if key not in cfg:
             rich.print(f"[yellow bold]{key}[/yellow bold] = ?" + (
                 f" (default: {value})" if value and value != FIELD_PLACEHOLDER else ""
             ))
 
     if all_profiles:
-        for profile, props in cfg.get_profiles().items():
+        for profile, props in config_store.get_profiles().items():
             if profile == cfg.profile:
                 continue
             if len(props):
                 rich.print()
                 rich.print(f"[bold]\\[{profile}][/bold]")
                 for key, value in props.items():
-                    rich.print(f"{key} = [cyan bold]{mask(key, value)}")
+                    rich.print(f"{key} = [cyan bold]{map_toml_value(mask(key, value))}")
 
     divider()
 
 def mask(key: str, value: Any):
     if key in ["client_secret", "password"]:
         return "*" * len(str(value))
     return value
@@ -671,23 +723,20 @@
 
 @cli.command(
     name="config:check",
     help="Check whether config is valid",
 )
 def config_check(all_profiles:bool=False):
     divider()
+    if ConfigStore().get("platform"):
+        issue_top_level_profile_warning()
     ensure_config()
-    with Spinner("Connecting to platform..."):
-        try:
-            get_resource_provider().list_engines()
-        except Exception as e:
-            rich.print(f"[yellow]Error: {e}")
-            divider()
-            sys.exit(1)
-    rich.print("[green]✓ Connection successful!")
+    with Spinner("Connecting to platform...", "Connection successful!", "Error:"):
+        get_resource_provider().list_engines()
+    divider()
 
 #--------------------------------------------------
 # Version
 #--------------------------------------------------
 
 def latest_version(package_name):
     """Get the current version of a package on PyPI."""
@@ -742,17 +791,23 @@
     divider()
 
 #--------------------------------------------------
 # Debugger
 #--------------------------------------------------
 
 @cli.command(help="Open the RAI debugger")
+@click.option("--host", help="Host to use", default="0.0.0.0")
 @click.option("--port", help="Port to use", default=8080)
-def debugger(port):
-    deb.main(port)
+@click.option("--new", help="Use the new debugger", is_flag=True, default=False)
+def debugger(host, port, new):
+    if new:
+        from relationalai.tools import debugger_server
+        debugger_server.start_server(host, port)
+    else:
+        deb.main(host, port)
 
 #--------------------------------------------------
 # Engine list
 #--------------------------------------------------
 
 @cli.command(name="engines:list", help="List all engines")
 @click.option("--state", help="Filter by engine state")
@@ -818,23 +873,34 @@
     is_snowflake = provider.config.get("platform") == "snowflake"
     is_interactive = name is None or size is None or (is_snowflake and pool is None)
 
     if not name:
         name = controls.prompt(
             "Engine name:",
             name,
-            validator=lambda e: engine_name_validator(cfg, e),
+            validator=ENGINE_NAME_REGEX.match,
+            invalid_message=ENGINE_NAME_ERROR,
             newline=True
         )
+
+    if is_interactive:
+        with Spinner(f"Validating engine '{name}' name", "Engine name validated", "Error:"):
+            is_name_valid = validate_engine_name(cfg, name)
+        if isinstance(is_name_valid, str):
+            rich.print("")
+            rich.print(f"[yellow]{is_name_valid}")
+            rich.print("")
+            return create_engine_flow(cfg)
     else:
         is_name_valid = validate_engine_name(cfg, name)
         if isinstance(is_name_valid, str):
             rich.print(f"[yellow]{is_name_valid}")
             return None
 
+    rich.print()
     if not size:
         size = controls.fuzzy("Engine size:", choices=ENGINE_SIZES)
         rich.print("")
 
     if is_snowflake:
         provider = cast(snowflake.Resources, provider)
         if not pool:
@@ -845,14 +911,15 @@
                 size,
             )
             if isinstance(result, Exception):
                 return None
             else:
                 pool = result
         if is_interactive and not pool:
+            rich.print("[yellow]No compute pool selected\n")
             redo = controls.confirm("Would you like to choose a different engine size?", default=True)
             rich.print("")
             if redo:
                 return create_engine_flow(cfg, name)
             else:
                 return None
     else:
@@ -896,25 +963,38 @@
 #--------------------------------------------------
 
 @cli.command(name="engines:delete", help="Delete an engine")
 @click.option("--name", help="Name of the engine")
 def engines_delete(name):
     divider(flush=True)
     ensure_config()
+    provider = get_resource_provider()
     if not name:
         name = controls.fuzzy_with_refetch(
             "Select an engine:",
             "engines",
-            lambda: [engine["name"] for engine in get_resource_provider().list_engines()],
+            lambda: [engine["name"] for engine in provider.list_engines()],
         )
         if not name or isinstance(name, Exception):
             return
+    else:
+        try:
+            engine = provider.get_engine(name)
+            if not engine:
+                rich.print(f"[yellow]Engine '{name}' not found")
+                divider()
+                return
+        except Exception as e:
+            rich.print(f"[yellow]Error fetching engine: {e}")
+            divider()
+            return
+
     with Spinner(f"Deleting '{name}' engine", f"Engine '{name}' deleted!"):
         try:
-            get_resource_provider().delete_engine(name)
+            provider.delete_engine(name)
         except Exception as e:
             rich.print(f"\n\n[yellow]Error deleting engine: {e}")
     divider()
 
 #--------------------------------------------------
 # Import Source flows
 #--------------------------------------------------
@@ -1361,139 +1441,191 @@
                 provider.delete_export(model, "", source_name)
             except Exception as e:
                 rich.print(f"\n\n[yellow]Error deleting export: {e}")
 
     divider()
 
 #--------------------------------------------------
-# Transactions list
+# Transactions get
 #--------------------------------------------------
 
-def nice_duration(millis):
-    seconds = millis / 1000
-    minutes = seconds / 60
-    hours = minutes / 60
-    days = hours / 24
-
-    display_days = int(days)
-    display_hours = int(hours % 24)
-    display_minutes = int(minutes % 60)
-    display_seconds = seconds % 60
-
-    parts = []
-    if display_days > 0:
-        parts.append(f"{display_days}d")
-    if display_hours > 0:
-        parts.append(f"{display_hours}h")
-    if display_minutes > 0:
-        parts.append(f"{display_minutes}m")
-    if display_seconds > 0:
-        parts.append(f"{display_seconds:,.1f}s")
-    return " ".join(parts[:3])
+def get_color_by_transaction_state(state:str) -> str:
+    match state.lower():
+        case "aborted":
+            return "red"
+        case "completed":
+            return "white"
+        case "created" | "running" | "cancelling":
+            return "bold yellow"
+        case _:
+            return ""
+
+def show_transaction_table(dict):
+    table = Table(show_header=True, border_style="dim", header_style="bold", box=rich_box.SIMPLE_HEAD)
+    table.add_column("Field")
+    table.add_column("Value")
+    for key, value in dict.items():
+        style = get_color_by_transaction_state(value) if key == "state" else ""
+
+        if key == "query_size" and isinstance(value, int):
+            value = humanized_bytes(value)
+
+        match value:
+            case None:
+                val = "N/A"
+            case int():
+                val = f"{value}"
+            case float():
+                val = f"{value}"
+            case list():
+                val = ", ".join(value)
+            case bool():
+                val = f"{value}"
+            case datetime():
+                val = value.strftime("%Y-%m-%d %H:%M:%S")
+            case timedelta():
+                val = humanized_duration(value.total_seconds() * 1000)
+            case _:
+                val = value
+        table.add_row(key, val, style=style)
+    rich.print(table)
+
+@cli.command(name="transactions:get", help="Get transaction details")
+@click.option("--id", help="Transaction id")
+def transactions_get(id):
+    divider()
+    ensure_config()
+    provider = get_resource_provider()
+    transaction = None
+
+    if not id:
+        id = controls.text("Transaction id:")
+        rich.print("")
+
+    with Spinner("Fetching transaction", "Transaction fetched"):
+        try:
+            transaction = provider.get_transaction(id)
+        except Exception as e:
+            rich.print(f"\n\n[yellow]Error fetching transaction: {e}")
+            divider()
+            exit(1)
+
+    rich.print()
+
+    if transaction:
+        show_transaction_table(transaction)
+
+    divider()
+
+#--------------------------------------------------
+# Transactions list
+#--------------------------------------------------
 
 def show_transactions(transactions, limit, all_users):
     config = ensure_config()
+    provider = get_resource_provider()
+    platform = provider.config.get("platform", "snowflake")
     if len(transactions):
         table = Table(show_header=True, border_style="dim", header_style="bold", box=rich_box.SIMPLE_HEAD)
         table.add_column("ID")
         table.add_column("Schema")
         table.add_column("State")
         table.add_column("Created")
         table.add_column("Duration", justify="right")
 
         added = 0
         for txn in transactions:
-            if not all_users and txn.get("created_by", "").lower() != config.get("user", "").lower():
-                continue
+            if platform == "snowflake":
+                if (
+                    not all_users
+                    and txn.get("created_by", "").lower()
+                    != cast(str, config.get("user", "")).lower()
+                ):
+                    continue
             if added >= limit:
                 break
 
-            match txn.get("state", "").lower():
-                case "aborted":
-                    style = "red"
-                case "completed":
-                    style = "white"
-                case "created":
-                    style = "bold yellow"
-                case _:
-                    style = ""
-
+            state = txn.get("state", "")
             duration = txn.get("duration")
+            created_on = txn.get("created_on")
+
+            if isinstance(created_on, int):
+                created_on = datetime.fromtimestamp(created_on / 1000)
             if duration is None:
-                created_on = txn["created_on"]
-                duration = (datetime.datetime.now(created_on.tzinfo) - created_on).total_seconds() * 1000
+                duration = (datetime.now(created_on.tzinfo) - created_on).total_seconds() * 1000
 
             table.add_row(
                 txn.get("id"),
                 txn.get("database"),
-                txn.get("state"),
-                txn.get("created_on").strftime("%Y-%m-%d %H:%M:%S"),
-                nice_duration(duration),
-                style=style
+                state,
+                created_on.strftime("%Y-%m-%d %H:%M:%S"),
+                humanized_duration(duration),
+                style=get_color_by_transaction_state(state)
             )
             added += 1
         rich.print(table)
     else:
         rich.print("[yellow]No transactions found")
 
-
-@supports_platform("snowflake")
 @cli.command(name="transactions:list", help="List transactions")
+@click.option("--id", help="Filter by transaction id", type=str)
+@click.option("--state", help="Filter by transaction state", type=str)
 @click.option("--limit", default=20, help="Limit")
-@click.option("--all-users", is_flag=True, help="Show transactions from all users")
-def transactions_list(limit, all_users):
+@click.option("--all-users", is_flag=True, default=False, help="Show transactions from all users")
+def transactions_list(id, state, limit, all_users):
     divider()
     ensure_config()
     provider = get_resource_provider()
     with Spinner("Fetching transactions", "Transactions fetched"):
         try:
-            transactions = provider.list_transactions(max(limit, 100))
+            transactions = provider.list_transactions(
+                id=id,
+                state=state,
+                limit=max(limit, 100)
+            )
         except Exception as e:
-            rich.print(f"\n\n[yellow]Error fetching transactions: {e}")
+            rich.print(f"\n\n[yellow]Error fetching transactions: {e}\n")
             exit(1)
 
     rich.print()
     show_transactions(transactions, limit, all_users)
 
     divider()
 
 #--------------------------------------------------
 # Transaction cancel
 #--------------------------------------------------
 
-@supports_platform("snowflake")
 @cli.command(name="transactions:cancel", help="Cancel a transaction")
 @click.option("--id", help="Transaction ID")
 @click.option("--all-users", is_flag=True, help="Show transactions from all users")
 def transactions_cancel(id, all_users):
     divider()
     ensure_config()
     provider = get_resource_provider()
     if id is None:
         with Spinner("Fetching transactions", "Transactions fetched"):
             try:
-                transactions = provider.list_transactions(20, only_active=True)
+                transactions = provider.list_transactions(limit=20, only_active=True)
             except Exception as e:
                 rich.print(f"\n\n[yellow]Error fetching transactions: {e}")
                 exit(0)
 
         if not transactions:
-            rich.print("[yellow]No transactions running")
+            rich.print("\n[yellow]No active transactions found")
+            rich.print("")
             exit(1)
 
         show_transactions(transactions, 20, all_users)
 
         id = controls.fuzzy("Select a transaction to cancel:", [t["id"] for t in transactions])
         print()
 
-    with Spinner("Cancelling transaction", "Transaction cancelled"):
-        try:
-            provider.cancel_transaction(id)
-        except Exception as e:
-            rich.print(f"\n\n[yellow]Error cancelling transaction: {e}")
+    with Spinner("Cancelling transaction", "Transaction cancelled", "Error:"):
+        provider.cancel_transaction(id)
 
     divider()
 
 #--------------------------------------------------
 # Main
 #--------------------------------------------------
```

### Comparing `relationalai-0.2.7/src/relationalai/tools/cli_controls.py` & `relationalai-0.2.8/src/relationalai/tools/cli_controls.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/src/relationalai/tools/debugger.py` & `relationalai-0.2.8/src/relationalai/tools/debugger.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,22 +160,22 @@
                 active_item = current_json_objects[active_ix]
             # Refresh the UI with the new objects
             my_stuff.refresh()
             details.refresh()
     except FileNotFoundError:
         pass
 
-def main(port=8080):
+def main(host="0.0.0.0", port=8080):
     ui.dark_mode().enable()
     with ui.row():
         with ui.column() as c:
             c.style("cursor: pointer;")
             my_stuff()
         with ui.column() as c:
             c.style("padding-left: 2em;")
             details()
 
     ui.timer(1, poll)
-    ui.run(reload=False, port=port)
+    ui.run(reload=False, host=host, port=port)
 
 if __name__ == "__main__":
-    main()
+    main()
```

### Comparing `relationalai-0.2.7/src/relationalai/tools/debugger_server.py` & `relationalai-0.2.8/src/relationalai/tools/debugger_client.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,90 +1,81 @@
 import asyncio
 import logging
 import os
 import threading
 import websockets
-
+import queue
 from relationalai import debugging
 import __main__ # to get the users root file path
 
-connected_clients = set()
-has_connected_client = threading.Event()
-buffered_broadcasts = []
-
-async def broadcast(message):
-    buffered_broadcasts.append(message)
-    if connected_clients:
-        tasks = [asyncio.create_task(client.send(message)) for client in connected_clients]
-        await asyncio.wait(tasks)
-
-async def handle_connection(websocket, path):
-    connected_clients.add(websocket)
-    if not has_connected_client.is_set():
-        has_connected_client.set()
-
-    try:
-        for message in buffered_broadcasts:
-            await websocket.send(message)
-        async for message in websocket:
-            print("GOT", message)
-    except websockets.exceptions.ConnectionClosed as e:
-        print(f"Client disconnected with reason: {e}")
-    finally:
-        connected_clients.remove(websocket)
-
-def _start_server(host: str, port: int, program_span: dict):
-    loop = asyncio.new_event_loop()
-    asyncio.set_event_loop(loop)
-
-    start_server_coro = websockets.serve(handle_connection, host, port)
-    server = loop.run_until_complete(start_server_coro)
-
-    try:
-        while True:
-            if not threading.main_thread().is_alive():
-                break
-            loop.run_until_complete(asyncio.sleep(1))
-    finally:
-        debugging.span_end(program_span)
-        server.close()
-        loop.run_until_complete(server.wait_closed())
-        loop.close()
-
+#------------------------------------------------------------------------------
+# Logging Handler
+#------------------------------------------------------------------------------
 
 class WebSocketLoggingHandler(logging.Handler):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         from relationalai.analysis.mechanistic import Mechanism
         self.Mechanism = Mechanism
+        self.queue: queue.Queue[str] = queue.Queue()
+
+    def start(self, url: str):
+        main_path = getattr(__main__, "__file__", None)
+        program_span = debugging.span_start("program",  main=os.path.relpath(main_path) if main_path else "notebook")
+        self.thread = threading.Thread(target=self.connect, args=(url, program_span))
+        self.thread.start()
 
     def emit(self, record):
         d = record.msg
         if (isinstance(d, dict) and
             d["event"] == "span_start" and
             "task" in d["span"].attrs and
             "mech" not in d["span"].attrs):
             d["span"].attrs["mech"] = self.Mechanism(d["span"].attrs["task"])
         log_entry = self.format(record)
-        asyncio.run(broadcast(log_entry))
+        self.queue.put_nowait(log_entry)
+
+    def connect(self, url: str, span: debugging.Span):
+        print(f"Connecting to {url}...")
+        try:
+            try:
+                loop = asyncio.get_running_loop()
+                loop.run_until_complete(self.connect_async(url, span))
+            except RuntimeError:
+                asyncio.run(self.connect_async(url, span))
+        except (ConnectionRefusedError, websockets.WebSocketException, OSError, asyncio.TimeoutError):
+            print(f"Failed to connect to {url}. Running with debug sink disabled.")
+
+    async def connect_async(self, url: str, span: debugging.Span):
+        async with websockets.connect(url) as ws:
+            print("Connected.")
+            while True:
+                if not threading.main_thread().is_alive():
+                    debugging.span_end(span)
+                    log_entry = self.queue.get(timeout=1)
+                    await ws.send(log_entry)
+                    break
+
+                try:
+                    log_entry = self.queue.get(timeout=1)
+                    await ws.send(log_entry)
+                except queue.Empty:
+                    pass
+                except websockets.ConnectionClosedError:
+                    break
+
+#------------------------------------------------------------------------------
+# Enable debugging
+#------------------------------------------------------------------------------
 
 already_debugging = False
-def start_debugger_session(wait_for_connection = False, host = "0.0.0.0", port = 5678):
+def start_debugger_session(host = "0.0.0.0", port = 8080):
     global already_debugging
     if already_debugging:
         return
 
-    already_debugging = True
     ws_handler = WebSocketLoggingHandler()
     ws_handler.setFormatter(debugging.JsonFormatter())
     debugging.logger.addHandler(ws_handler)
+    ws_handler.start(f"ws://{host}:{port}/ws/program")
 
-    program_span = debugging.span_start("program",  main=os.path.relpath(__main__.__file__))
-
-    # daemon so the make program exiting will kill the thread
-    server_thread = threading.Thread(target=_start_server, args=(host, port, program_span)) # , daemon=True
-    server_thread.start()
-
-    if wait_for_connection:
-        print(f"Waiting for debugger client to connect at ws://{host}:{port} ...")
-        has_connected_client.wait()
-        print("Connected.")
+    already_debugging = True
```

### Comparing `relationalai-0.2.7/src/relationalai/tools/dev.py` & `relationalai-0.2.8/src/relationalai/tools/dev.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/src/relationalai/util/snowflake_logger.py` & `relationalai-0.2.8/src/relationalai/util/snowflake_logger.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/src/relationalai/util/tracing_logger.py` & `relationalai-0.2.8/src/relationalai/util/tracing_logger.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/tests/conftest.py` & `relationalai-0.2.8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/tests/util.py` & `relationalai-0.2.8/tests/util.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/tests/benchmarks/conftest.py` & `relationalai-0.2.8/tests/benchmarks/conftest.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/tests/benchmarks/test_tastybytes.py` & `relationalai-0.2.8/tests/benchmarks/test_tastybytes.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/tests/end2end/README.md` & `relationalai-0.2.8/tests/end2end/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/tests/end2end/conftest.py` & `relationalai-0.2.8/tests/end2end/conftest.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/tests/end2end/test_graph_visualize.py` & `relationalai-0.2.8/tests/end2end/test_graph_visualize.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/tests/end2end/test_snapshots.py` & `relationalai-0.2.8/tests/end2end/test_snapshots.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query2.txt` & `relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query2.txt`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/tests/end2end/test_cases/after_errors.py` & `relationalai-0.2.8/tests/end2end/test_cases/after_errors.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/tests/end2end/test_cases/bool.py` & `relationalai-0.2.8/tests/end2end/test_cases/bool.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/tests/end2end/test_cases/bottom.py` & `relationalai-0.2.8/tests/end2end/test_cases/bottom.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/tests/end2end/test_cases/export.py` & `relationalai-0.2.8/tests/end2end/test_cases/export.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/tests/end2end/test_cases/multi_valued.py` & `relationalai-0.2.8/tests/end2end/test_cases/multi_valued.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/tests/end2end/test_cases/not_found.py` & `relationalai-0.2.8/tests/end2end/test_cases/not_found.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/tests/end2end/test_cases/out_of_context.py` & `relationalai-0.2.8/tests/end2end/test_cases/out_of_context.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/tests/end2end/test_cases/persist.py` & `relationalai-0.2.8/tests/end2end/test_cases/persist.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/tests/end2end/test_cases/smoke.py` & `relationalai-0.2.8/tests/end2end/test_cases/smoke.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/tests/end2end/test_cases/std_math.py` & `relationalai-0.2.8/tests/end2end/test_cases/std_math.py`

 * *Files 5% similar despite different names*

```diff
@@ -83,7 +83,22 @@
 
 # Check that the trunc_divide function works
 with model.query(tag="trunc_divide") as select:
     p = Point(x=1.1)
     trunc_divide1 = std.math.trunc_divide(p.x, 2)
     trunc_divide2 = std.math.trunc_divide(-5, 2)
     select(p, trunc_divide1, trunc_divide2)
+
+# Check that the sin, cos functions works
+for func in [
+    std.math.sin,
+    std.math.cos,
+    std.math.tan,
+    std.math.acos,
+    std.math.asin,
+    std.math.atan,
+    std.math.radians,
+    std.math.degrees,
+]:
+    with model.query(tag=func.__name__) as select:
+        p = Point()
+        select(p, func(p.z), func(0))
```

### Comparing `relationalai-0.2.7/tests/end2end/test_cases/strings.py` & `relationalai-0.2.8/tests/end2end/test_cases/strings.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/tests/end2end/test_cases/top.py` & `relationalai-0.2.8/tests/end2end/test_cases/top.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/tests/end2end/test_cases/union.py` & `relationalai-0.2.8/tests/end2end/test_cases/union.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/tests/end2end/test_cases/weighted_graphs.py` & `relationalai-0.2.8/tests/end2end/test_cases/weighted_graphs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import relationalai as rai
 from relationalai.std.graphs import Graph
 
-model = rai.Model(name=globals().get("name", ""), config=globals().get("config"))
+model = rai.Model(name=globals().get("name", "test_weighted"), config=globals().get("config"))
 
 
 def run_test(algo, ix: int, raw_edges):
     Node = model.Type(f"Node{ix}")
     graph = Graph(model, weighted=ix > 0)
 
     # Install graph data
```

### Comparing `relationalai-0.2.7/tests/end2end/test_cases/graphs/basics.py` & `relationalai-0.2.8/tests/end2end/test_cases/graphs/basics.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/tests/end2end/test_cases/graphs/centrality.py` & `relationalai-0.2.8/tests/end2end/test_cases/graphs/centrality.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/tests/end2end/test_cases/graphs/community.py` & `relationalai-0.2.8/tests/end2end/test_cases/graphs/clustering.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,43 @@
 import relationalai as rai
 from relationalai import std
 
-# Query snapshots are output in same order as this list.
-ALGOS = [
-    "louvain",
-    "weakly_connected_component",
-    "triangle_community",  # Expects empty dataframe b/c graph has no triangles.
-    "infomap",
-    "label_propagation",
+# Query snapshots are output in same order as these lists.
+NO_ARGS = [
+    "avg_clustering_coefficient",
+]
+
+ONE_ARG = [
+    "local_clustering_coefficient",
 ]
 
 model = rai.Model(name=globals().get("name", ""), config=globals().get("config"))
 Object = model.Type("Object")
 Relationship = model.Type("Relationship")
 
 with model.rule():
     obj1 = Object.add(id=1)
     obj2 = Object.add(id=2)
     obj3 = Object.add(id=3)
+    obj4 = Object.add(id=4)
     Relationship.add(from_=obj1, to=obj2)
+    Relationship.add(from_=obj1, to=obj3)
+    Relationship.add(from_=obj1, to=obj4)
+    Relationship.add(from_=obj2, to=obj3)
 
-graph = std.graphs.Graph(model, undirected=True, with_isolated_nodes=True)
+graph = std.graphs.Graph(model, undirected=True)
 graph.Node.extend(Object)
 
 with model.rule():
     r = Relationship()
     graph.Edge.add(r.from_, r.to)
 
-for algo_name in ALGOS:
+for algo_name in NO_ARGS:
+    with model.query(tag=algo_name) as select:
+        algo = getattr(graph.compute, algo_name)()
+        select(algo)
+
+for algo_name in ONE_ARG:
     with model.query(tag=algo_name) as select:
         o = Object()
         algo = getattr(graph.compute, algo_name)(o)
-        select(o, algo)
+        select(o, algo)
```

### Comparing `relationalai-0.2.7/tests/end2end/test_cases/graphs/connectivity.py` & `relationalai-0.2.8/tests/end2end/test_cases/graphs/connectivity.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/tests/end2end/test_cases/graphs/degree.py` & `relationalai-0.2.8/tests/end2end/test_cases/graphs/degree.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 BINARY_ALGOS = [
     "degree",
     "indegree",
     "outdegree",
 ]
 
-model = rai.Model(name=globals().get("name", ""), config=globals().get("config"))
+model = rai.Model(name=globals().get("name", "test_degree"), config=globals().get("config"))
 Object = model.Type("Object")
 Relationship = model.Type("Relationship")
 
 with model.rule():
     obj1 = Object.add(id=1)
     obj2 = Object.add(id=2)
     Relationship.add(from_=obj1, to=obj2)
```

### Comparing `relationalai-0.2.7/tests/end2end/test_cases/graphs/distance.py` & `relationalai-0.2.8/tests/end2end/test_cases/graphs/distance.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/tests/end2end/test_cases/graphs/link_prediction.py` & `relationalai-0.2.8/tests/end2end/test_cases/graphs/link_prediction.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/tests/end2end/test_cases/graphs/similarity.py` & `relationalai-0.2.8/tests/end2end/test_cases/graphs/similarity.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/tests/end2end/test_cases/graphs/triangles.py` & `relationalai-0.2.8/tests/end2end/test_cases/graphs/triangles.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/tests/init-cli/azure_basic.py` & `relationalai-0.2.8/tests/init-cli/azure_basic.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/tests/init-cli/common.py` & `relationalai-0.2.8/tests/init-cli/common.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/tests/roundtrip/test_document.py` & `relationalai-0.2.8/tests/roundtrip/test_document.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/tests/roundtrip/test_task.py` & `relationalai-0.2.8/tests/roundtrip/test_task.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.7/pyproject.toml` & `relationalai-0.2.8/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = 'relationalai'
-version = '0.2.7'
+version = '0.2.8'
 description = 'RelationalAI Library and CLI'
 readme="docs/pypi/README.md"
 authors = [
     { name="RelationalAI", email="support@relational.ai" },
 ]
 requires-python = ">= 3.10"
 dependencies = [
@@ -19,15 +19,16 @@
     "click",
     "gravis",
     "bytecode",
     "toml",
     "tomlkit",
     "requests",
     "pyarrow",
-    "websockets"
+    "websockets",
+    "aiohttp",
 ]
 [project.optional-dependencies]
 dev = [
     "pytest",
     "hypothesis",
     "faker",
     "argcomplete",
```

### Comparing `relationalai-0.2.7/PKG-INFO` & `relationalai-0.2.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.3
 Name: relationalai
-Version: 0.2.7
+Version: 0.2.8
 Summary: RelationalAI Library and CLI
 Author-email: RelationalAI <support@relational.ai>
 Requires-Python: >=3.10
+Requires-Dist: aiohttp
 Requires-Dist: bytecode
 Requires-Dist: click
 Requires-Dist: colorama
 Requires-Dist: gravis
 Requires-Dist: inquirerpy
 Requires-Dist: nicegui
 Requires-Dist: numpy
```

