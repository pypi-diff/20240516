# Comparing `tmp/relationalai-0.2.8.tar.gz` & `tmp/relationalai-0.2.9.tar.gz`

## Comparing `relationalai-0.2.8.tar` & `relationalai-0.2.9.tar`

### file list

```diff
@@ -1,552 +1,573 @@
--rw-r--r--   0        0        0     6206 2020-02-02 00:00:00.000000 relationalai-0.2.8/README.md
--rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 relationalai-0.2.8/.github/actions/benchmarks/action.yml
--rw-r--r--   0        0        0     5131 2020-02-02 00:00:00.000000 relationalai-0.2.8/.github/actions/end-to-end/action.yml
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 relationalai-0.2.8/.github/workflows/benchmarks.yml
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 relationalai-0.2.8/.github/workflows/end-to-end.yml
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 relationalai-0.2.8/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 relationalai-0.2.8/.github/workflows/ruff.yml
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/README.md
--rw-r--r--   0        0        0    17779 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/getting_started.md
--rw-r--r--   0        0        0     9875 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/_old/OLD_pyrel_quickstart.md
--rw-r--r--   0        0        0     3956 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/_old/metamodel.md
--rw-r--r--   0        0        0     5935 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/_old/python_dsl.md
--rw-r--r--   0        0        0     9371 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/_old/quickstart.md
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/README.md
--rw-r--r--   0        0        0    13377 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/cli/README.md
--rw-r--r--   0        0        0     7095 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/configuration/README.md
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Expression.md
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Property.md
--rw-r--r--   0        0        0    10044 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/README.md
--rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Context/README.md
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Context/enter__.md
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Context/exit__.md
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Context/iter__.md
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Context/model.md
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Context/results.md
--rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/ContextSelect/README.md
--rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/ContextSelect/add.md
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/ContextSelect/call__.md
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/ContextSelect/getattribute__.md
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Instance/README.md
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Instance/persist.md
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Instance/set.md
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Instance/unpersist.md
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/InstanceProperty/README.md
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/InstanceProperty/or_.md
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Model/README.md
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Model/Type.md
--rw-r--r--   0        0        0     3427 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Model/found.md
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Model/name.md
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Model/not_found.md
--rw-r--r--   0        0        0     5008 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Model/ordered_choice.md
--rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Model/query.md
--rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Model/read.md
--rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Model/rule.md
--rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Model/scope.md
--rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Model/union.md
--rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Producer/README.md
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Producer/add__.md
--rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Producer/enter__.md
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Producer/eq__.md
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Producer/exit__.md
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Producer/floordiv__.md
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Producer/ge__.md
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Producer/getattribute__.md
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Producer/gt__.md
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Producer/le__.md
--rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Producer/lt__.md
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Producer/mul__.md
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Producer/ne__.md
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Producer/pow__.md
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Producer/radd__.md
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Producer/rfloordiv__.md
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Producer/rmul__.md
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Producer/rpow__.md
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Producer/rsub__.md
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Producer/rtruediv__.md
--rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Producer/sub__.md
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Producer/truediv__.md
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Type/README.md
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Type/add.md
--rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Type/call__.md
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Type/extend.md
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Type/model.md
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Type/name.md
--rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/Type/or__.md
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/clients/README.md
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/clients/snowflake/PrimaryKey.md
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/clients/snowflake/README.md
--rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/clients/snowflake/Snowflake.md
--rw-r--r--   0        0        0     2588 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/clients/snowflake/SnowflakeTable/README.md
--rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/clients/snowflake/SnowflakeTable/describe.md
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/clients/snowflake/SnowflakeTable/fqname.md
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/clients/snowflake/SnowflakeTable/namespace.md
--rw-r--r--   0        0        0     6011 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/README.md
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/Vars.md
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/alias.md
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/aggregates/README.md
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/aggregates/avg.md
--rw-r--r--   0        0        0     2994 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/aggregates/count.md
--rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/aggregates/max.md
--rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/aggregates/min.md
--rw-r--r--   0        0        0     3303 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/aggregates/rank_asc.md
--rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/aggregates/rank_desc.md
--rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/aggregates/sum.md
--rw-r--r--   0        0        0     3812 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/README.md
--rw-r--r--   0        0        0     3503 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/README.md
--rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/adamic_adar.md
--rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/average_clustering_coefficient.md
--rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/avg_degree.md
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/avg_indegree.md
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/avg_outdegree.md
--rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/betweeness_centrality.md
--rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/common_neighbor.md
--rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/cosine_similarity.md
--rw-r--r--   0        0        0     2349 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/degree.md
--rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/degree_centrality.md
--rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/diameter_range.md
--rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/distance.md
--rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/eigenvector_centrality.md
--rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/indegree.md
--rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/infomap.md
--rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/is_connected.md
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/is_reachable.md
--rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/is_triangle.md
--rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/jaccard_similarity.md
--rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/label_propagation.md
--rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/local_lustering_coefficient.md
--rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/louvain.md
--rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/max_degree.md
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/max_indegree.md
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/max_outdegree.md
--rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/min_degree.md
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/min_indegree.md
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/min_outdegree.md
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/num_edges.md
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/num_nodes.md
--rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/num_triangles.md
--rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/outdegree.md
--rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/pagerank.md
--rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/preferential_attachment.md
--rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/reachable_from.md
--rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/triangles.md
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/weakly_connected_component.md
--rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/weighted_cosine_similarity.md
--rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/weighted_degree_centrality.md
--rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/weighted_distance.md
--rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/weighted_jaccard_similarity.md
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Edge/README.md
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Edge/add.md
--rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Edge/call__.md
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Edge/extend.md
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/EdgeInstance/README.md
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/EdgeInstance/from_.md
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/EdgeInstance/set.md
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/EdgeInstance/to.md
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Graph/Edge.md
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Graph/Node.md
--rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Graph/README.md
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Graph/compute.md
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Graph/fetch.md
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Graph/id.md
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Graph/model.md
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Graph/undirected.md
--rw-r--r--   0        0        0     4167 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Graph/visualize.md
--rw-r--r--   0        0        0    20679 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Graph/img/graph-viz-with-labels-and-colors.png
--rw-r--r--   0        0        0    15558 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Graph/img/graph-viz.png
--rw-r--r--   0        0        0    14921 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/graphs/Graph/img/simple-social-network.png
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/math/README.md
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/math/abs.md
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/math/acos.md
--rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/math/asin.md
--rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/math/atan.md
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/math/cbrt.md
--rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/math/ceil.md
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/math/cos.md
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/math/degrees.md
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/math/floor.md
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/math/isclose.md
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/math/log.md
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/math/radians.md
--rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/math/sign.md
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/math/sin.md
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/math/sqrt.md
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/math/tan.md
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/math/trunc_divide.md
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/strings/README.md
--rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/strings/concat.md
--rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/strings/contains.md
--rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/strings/ends_with.md
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/strings/join.md
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/strings/length.md
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/strings/like.md
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/strings/lowercase.md
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/strings/regex_compile.md
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/strings/regex_match.md
--rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/strings/replace.md
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/strings/split.md
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/strings/split_part.md
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/python/std/strings/uppercase.md
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/api_reference/sql/README.md
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/faq/README.md
--rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/faq/engines.md
--rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/README.md
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/cdc.py
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/custom_snowflake_connection.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/emit_playground.py
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/found.py
--rw-r--r--   0        0        0     6699 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/fraud.ipynb
--rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/fraud.py
--rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/graph_algos.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/load_raw.py
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/nested.py
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/or_types.py
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/remote_load_csv.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/requirements.txt
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/simple.py
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/simple_recursion.py
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/simple_streamlit.py
--rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/solver.py
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/weighted_graph_algos.py
--rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/articles_graph/README.md
--rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/articles_graph/articles_graph.py
--rw-r--r--   0        0        0     5257 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/articles_graph/articles_graph_with_nlp.py
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/articles_graph/pyproject.toml
--rw-r--r--   0        0        0     3399 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/articles_graph/utils.py
--rw-r--r--   0        0        0  1274296 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/articles_graph/daily_articles/04_04_2024.json
--rw-r--r--   0        0        0     4740 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/data/people.csv
--rw-r--r--   0        0        0    10518 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/data/transactions.csv
--rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/ev_penetration/ev_penetration.py
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/ev_penetration/ev_penetration_csv.py
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/ev_penetration/state_stats.csv
--rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/imdb/README.md
--rw-r--r--   0        0        0   787694 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/imdb/imdb.csv
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/imdb/imdb.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/rel/bar.rel
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/rel/foo.rel
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/rel/solver.rel
--rw-r--r--   0        0        0     6174 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/social-money-network/SF_pagerank.ipynb
--rw-r--r--   0        0        0  2419367 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/social-money-network/Simulation-and-SF-Upload.ipynb
--rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 relationalai-0.2.8/examples/social-money-network/snowflake_pagerank.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/.gitignore
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/README.md
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/index.html
--rw-r--r--   0        0        0   463836 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/package-lock.json
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/package.json
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/tsconfig.json
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/vite.config.ts
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/.storybook/main.ts
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/.storybook/preview-body.html
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/.storybook/preview-head.html
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/.storybook/preview.ts
--rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/App.styl
--rw-r--r--   0        0        0     6535 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/App.tsx
--rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/Selection.tsx
--rw-r--r--   0        0        0    11656 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/debugger_client.ts
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/index.css
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/index.tsx
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/logo.svg
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/util.styl
--rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/util.ts
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/ws.ts
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/assets/favicon.png
--rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/EventList.styl
--rw-r--r--   0        0        0     7185 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/EventList.tsx
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/EventViewer.styl
--rw-r--r--   0        0        0     5165 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/EventViewer.tsx
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/FileDropZone.styl
--rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/FileDropZone.tsx
--rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/Sidebar.styl
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/Sidebar.tsx
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/Schematic/NodeIcon.stories.tsx
--rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/Schematic/ScopeProvider.tsx
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/Schematic/index.stories.tsx
--rw-r--r--   0        0        0     4742 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/Schematic/index.styl
--rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/Schematic/index.tsx
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/Schematic/nodes/CallNode.tsx
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/Schematic/nodes/ComputeNode.tsx
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/Schematic/nodes/EffectNode.tsx
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/Schematic/nodes/FilterNode.tsx
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/Schematic/nodes/GetNode.tsx
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/Schematic/nodes/QuantifyNode.tsx
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/Schematic/nodes/ReturnNode.tsx
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/Schematic/nodes/SequenceNode.tsx
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/Schematic/nodes/UnionNode.tsx
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/Schematic/nodes/UnknownNode.tsx
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/Schematic/nodes/base.styl
--rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/Schematic/nodes/base.tsx
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/Schematic/nodes/index.tsx
--rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/ui/Accordion.stories.tsx
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/ui/Accordion.styl
--rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/ui/Accordion.tsx
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/ui/Breadcrumbs.stories.tsx
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/ui/Breadcrumbs.styl
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/ui/Breadcrumbs.tsx
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/ui/Button.styl
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/ui/Button.tsx
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/ui/Code.styl
--rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/ui/Code.tsx
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/ui/Collapsible.stories.tsx
--rw-r--r--   0        0        0     4220 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/ui/Collapsible.styl
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/ui/Collapsible.tsx
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/ui/Field.stories.tsx
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/ui/Field.styl
--rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/ui/Field.tsx
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/ui/Icon.styl
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/ui/Icon.tsx
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/ui/Modal.stories.tsx
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/ui/Modal.styl
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/ui/Modal.tsx
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/ui/Tooltip.stories.tsx
--rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/ui/Tooltip.styl
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/components/ui/Tooltip.tsx
--rw-r--r--   0        0        0     4529 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/fixtures/branch-improved.json
--rw-r--r--   0        0        0     5229 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/fixtures/branch.json
--rw-r--r--   0        0        0    67308 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/fixtures/fraud.json
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/fixtures/index.ts
--rw-r--r--   0        0        0     9536 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/fixtures/not_found.json
--rw-r--r--   0        0        0     6685 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/fixtures/simple.json
--rw-r--r--   0        0        0     6271 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/fixtures/union.json
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/types/json.d.ts
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/types/jsx.d.ts
--rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/types/mech.d.ts
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 relationalai-0.2.8/frontend/debugger/src/utils/fileUtils.ts
--rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/gentest/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/gentest/__init__.py
--rw-r--r--   0        0        0    12329 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/gentest/emit.py
--rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/gentest/exec.py
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/gentest/fixtures.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/gentest/patch.py
--rw-r--r--   0        0        0     7629 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/gentest/util.py
--rwxr-xr-x   0        0        0     3521 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/gentest/cli/__main__.py
--rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/gentest/cli/collect_failures.py
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/gentest/cli/collect_tests.py
--rw-r--r--   0        0        0     5707 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/gentest/cli/repro.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/gentest/cli/run_tests.py
--rw-r--r--   0        0        0    15710 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/gentest/cli/watch.py
--rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/gentest/gen/action.py
--rw-r--r--   0        0        0     5461 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/gentest/gen/context.py
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/gentest/gen/document.py
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/gentest/gen/error.py
--rw-r--r--   0        0        0     6095 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/gentest/gen/group_limited.py
--rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/gentest/gen/ir.py
--rw-r--r--   0        0        0    17029 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/gentest/gen/scope.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/gentest/gen/staged.py
--rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/gentest/gen/task.py
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/gentest/gen/test.py
--rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/gentest/harness/database.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/gentest/harness/vendor_types.py
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/gentest/validate/diff.py
--rw-r--r--   0        0        0     5588 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/gentest/validate/errors.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/gentest/validate/mapping.py
--rw-r--r--   0        0        0     5426 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/gentest/validate/roundtrip.py
--rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/__init__.py
--rw-r--r--   0        0        0     6310 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/compiler.py
--rw-r--r--   0        0        0    11725 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/debugging.py
--rw-r--r--   0        0        0    46572 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/dsl.py
--rw-r--r--   0        0        0    15741 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/errors.py
--rw-r--r--   0        0        0    26752 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/metagen.py
--rw-r--r--   0        0        0    27989 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/metamodel.py
--rw-r--r--   0        0        0    19780 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/rel.py
--rw-r--r--   0        0        0    20453 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/rel2.py
--rw-r--r--   0        0        0    13371 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/rel_emitter.py
--rw-r--r--   0        0        0     3549 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/rel_utils.py
--rw-r--r--   0        0        0     8570 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/analysis/mechanistic.py
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/analysis/whynot.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/clients/__init__.py
--rw-r--r--   0        0        0    14725 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/clients/azure.py
--rw-r--r--   0        0        0    11981 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/clients/client.py
--rw-r--r--   0        0        0    17625 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/clients/config.py
--rw-r--r--   0        0        0    39864 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/clients/snowflake.py
--rw-r--r--   0        0        0     5526 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/clients/test.py
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/clients/types.py
--rw-r--r--   0        0        0     7529 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/loaders/csv.py
--rw-r--r--   0        0        0     7140 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/loaders/loader.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/loaders/types.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/std/__init__.py
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/std/aggregates.py
--rw-r--r--   0        0        0    21043 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/std/graphs.py
--rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/std/math.py
--rw-r--r--   0        0        0     2785 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/std/strings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/tools/__init__.py
--rw-r--r--   0        0        0    59285 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/tools/cli.py
--rw-r--r--   0        0        0    12721 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/tools/cli_controls.py
--rw-r--r--   0        0        0     6886 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/tools/debugger.py
--rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/tools/debugger_client.py
--rw-r--r--   0        0        0     5341 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/tools/debugger_server.py
--rw-r--r--   0        0        0     9121 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/tools/dev.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/tools/notes
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/util/constants.py
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/util/format.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/util/keys.py
--rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/util/snowflake_logger.py
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 relationalai-0.2.8/src/relationalai/util/tracing_logger.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/__init__.py
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/conftest.py
--rw-r--r--   0        0        0     5346 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/util.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/benchmarks/conftest.py
--rw-r--r--   0        0        0     4603 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/benchmarks/test_tastybytes.py
--rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/README.md
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/conftest.py
--rw-r--r--   0        0        0     8024 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/test_graph_visualize.py
--rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/test_snapshots.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/after_errors/query0.txt
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/after_errors/query1.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/agg_ordering/query0.txt
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/bool/query0.txt
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/bool/query1.txt
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/bottom/query0.txt
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/first/query0.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__basics/query0.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__basics/query1.txt
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query0.txt
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query1.txt
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query2.txt
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query3.txt
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query4.txt
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__clustering/query0.txt
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__clustering/query1.txt
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query0.txt
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query1.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query2.txt
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query3.txt
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query4.txt
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__connectivity/query0.txt
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__connectivity/query1.txt
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__connectivity/query2.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query0.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query1.txt
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query10.txt
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query11.txt
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query2.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query3.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query4.txt
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query5.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query6.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query7.txt
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query8.txt
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query9.txt
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__distance/query0.txt
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__distance/query1.txt
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__distance/query2.txt
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__link_prediction/query0.txt
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__link_prediction/query1.txt
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__link_prediction/query2.txt
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__mixed_value_types/query0.txt
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__similarity/query0.txt
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__similarity/query1.txt
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__similarity/query2.txt
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__similarity/query3.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__triangles/query0.txt
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__triangles/query1.txt
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__triangles/query2.txt
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__triangles/query3.txt
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__triangles/query4.txt
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query0.txt
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query1.txt
--rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query2.txt
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query3.txt
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query4.txt
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/not_found/query0.txt
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/not_found/query1.txt
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/numeric_outputs/query0.txt
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/numeric_outputs/query1.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query0.txt
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query1.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query2.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query3.txt
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/smoke/query0.txt
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/smoke/query1.txt
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query0.txt
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query1.txt
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query10.txt
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query11.txt
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query12.txt
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query13.txt
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query14.txt
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query15.txt
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query16.txt
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query17.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query2.txt
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query3.txt
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query4.txt
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query5.txt
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query6.txt
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query7.txt
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query8.txt
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query9.txt
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query0.txt
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query1.txt
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query10.txt
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query2.txt
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query3.txt
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query4.txt
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query5.txt
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query6.txt
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query7.txt
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query8.txt
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query9.txt
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/top/query0.txt
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/union/query0.txt
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query0.txt
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query1.txt
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query2.txt
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query3.txt
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query4.txt
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query5.txt
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/test_cases/after_errors.py
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/test_cases/agg_ordering.py
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/test_cases/bool.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/test_cases/bottom.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/test_cases/export.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/test_cases/first.py
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/test_cases/multi_valued.py
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/test_cases/not_found.py
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/test_cases/numeric_outputs.py
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/test_cases/out_of_context.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/test_cases/persist.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/test_cases/smoke.py
--rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/test_cases/std_math.py
--rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/test_cases/strings.py
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/test_cases/top.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/test_cases/union.py
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/test_cases/weighted_graphs.py
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/test_cases/graphs/basics.py
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/test_cases/graphs/centrality.py
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/test_cases/graphs/clustering.py
--rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/test_cases/graphs/community.py
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/test_cases/graphs/connectivity.py
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/test_cases/graphs/degree.py
--rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/test_cases/graphs/distance.py
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/test_cases/graphs/link_prediction.py
--rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/test_cases/graphs/mixed_value_types.py
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/test_cases/graphs/similarity.py
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/end2end/test_cases/graphs/triangles.py
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/execution/test_core.py
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/execution/test_examples.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/execution/basic/smoketest.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/execution/snapshots/test_core/test_basic/smoketest/query0.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/execution/snapshots/test_examples/test_example/emit_playground/query0.txt
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/execution/snapshots/test_examples/test_example/found/query0.txt
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/execution/snapshots/test_examples/test_example/graph/query0.txt
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/execution/snapshots/test_examples/test_example/graph/query1.txt
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/execution/snapshots/test_examples/test_example/load_raw/query0.txt
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/execution/snapshots/test_examples/test_example/or_types/query0.txt
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/execution/snapshots/test_examples/test_example/simple/query0.txt
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/execution/snapshots/test_examples/test_example/simple_recursion/query0.txt
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/execution/snapshots/test_examples/test_example/simple_streamlit/query0.txt
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/execution/snapshots/test_examples/test_example/test/query0.txt
--rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/init-cli/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/init-cli/__init__.py
--rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/init-cli/azure_basic.py
--rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/init-cli/common.py
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/roundtrip/test_document.py
--rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/roundtrip/test_task.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/unit/test_config_store.py
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/unit/test_configs/config_with_new_profile.toml
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/unit/test_configs/printed_config.txt
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 relationalai-0.2.8/tests/unit/test_configs/raiconfig_example.toml
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 relationalai-0.2.8/.gitignore
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 relationalai-0.2.8/pyproject.toml
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 relationalai-0.2.8/docs/pypi/README.md
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 relationalai-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     6206 2020-02-02 00:00:00.000000 relationalai-0.2.9/README.md
+-rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 relationalai-0.2.9/.github/actions/benchmarks/action.yml
+-rw-r--r--   0        0        0     5131 2020-02-02 00:00:00.000000 relationalai-0.2.9/.github/actions/end-to-end/action.yml
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 relationalai-0.2.9/.github/workflows/benchmarks.yml
+-rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 relationalai-0.2.9/.github/workflows/end-to-end.yml
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 relationalai-0.2.9/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 relationalai-0.2.9/.github/workflows/ruff.yml
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/README.md
+-rw-r--r--   0        0        0    17779 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/getting_started.md
+-rw-r--r--   0        0        0     9875 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/_old/OLD_pyrel_quickstart.md
+-rw-r--r--   0        0        0     3956 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/_old/metamodel.md
+-rw-r--r--   0        0        0     5935 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/_old/python_dsl.md
+-rw-r--r--   0        0        0     9371 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/_old/quickstart.md
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/README.md
+-rw-r--r--   0        0        0     3468 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/cli/README.md
+-rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/cli/config_check.md
+-rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/cli/config_explain.md
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/cli/debugger.md
+-rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/cli/engines_create.md
+-rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/cli/engines_delete.md
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/cli/engines_get.md
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/cli/engines_list.md
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/cli/exports_delete.md
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/cli/exports_list.md
+-rw-r--r--   0        0        0     3602 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/cli/imports_delete.md
+-rw-r--r--   0        0        0     3256 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/cli/imports_list.md
+-rw-r--r--   0        0        0     6175 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/cli/imports_snapshot.md
+-rw-r--r--   0        0        0     6136 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/cli/imports_stream.md
+-rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/cli/init.md
+-rw-r--r--   0        0        0     2631 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/cli/profile_switch.md
+-rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/cli/transactions_cancel.md
+-rw-r--r--   0        0        0     3001 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/cli/transactions_get.md
+-rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/cli/transactions_list.md
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/cli/version.md
+-rw-r--r--   0        0        0     7095 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/configuration/README.md
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Expression.md
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Property.md
+-rw-r--r--   0        0        0    10044 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/README.md
+-rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Context/README.md
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Context/enter__.md
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Context/exit__.md
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Context/iter__.md
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Context/model.md
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Context/results.md
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/ContextSelect/README.md
+-rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/ContextSelect/add.md
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/ContextSelect/call__.md
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/ContextSelect/getattribute__.md
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Instance/README.md
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Instance/persist.md
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Instance/set.md
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Instance/unpersist.md
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/InstanceProperty/README.md
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/InstanceProperty/or_.md
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Model/README.md
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Model/Type.md
+-rw-r--r--   0        0        0     3427 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Model/found.md
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Model/name.md
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Model/not_found.md
+-rw-r--r--   0        0        0     5008 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Model/ordered_choice.md
+-rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Model/query.md
+-rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Model/read.md
+-rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Model/rule.md
+-rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Model/scope.md
+-rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Model/union.md
+-rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Producer/README.md
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Producer/add__.md
+-rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Producer/enter__.md
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Producer/eq__.md
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Producer/exit__.md
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Producer/floordiv__.md
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Producer/ge__.md
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Producer/getattribute__.md
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Producer/gt__.md
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Producer/le__.md
+-rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Producer/lt__.md
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Producer/mul__.md
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Producer/ne__.md
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Producer/pow__.md
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Producer/radd__.md
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Producer/rfloordiv__.md
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Producer/rmul__.md
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Producer/rpow__.md
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Producer/rsub__.md
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Producer/rtruediv__.md
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Producer/sub__.md
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Producer/truediv__.md
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Type/README.md
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Type/add.md
+-rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Type/call__.md
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Type/extend.md
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Type/model.md
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Type/name.md
+-rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/Type/or__.md
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/clients/README.md
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/clients/snowflake/PrimaryKey.md
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/clients/snowflake/README.md
+-rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/clients/snowflake/Snowflake.md
+-rw-r--r--   0        0        0     2588 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/clients/snowflake/SnowflakeTable/README.md
+-rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/clients/snowflake/SnowflakeTable/describe.md
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/clients/snowflake/SnowflakeTable/fqname.md
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/clients/snowflake/SnowflakeTable/namespace.md
+-rw-r--r--   0        0        0     6011 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/README.md
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/Vars.md
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/alias.md
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/aggregates/README.md
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/aggregates/avg.md
+-rw-r--r--   0        0        0     2994 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/aggregates/count.md
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/aggregates/max.md
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/aggregates/min.md
+-rw-r--r--   0        0        0     3303 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/aggregates/rank_asc.md
+-rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/aggregates/rank_desc.md
+-rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/aggregates/sum.md
+-rw-r--r--   0        0        0     3812 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/README.md
+-rw-r--r--   0        0        0     3503 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/README.md
+-rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/adamic_adar.md
+-rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/average_clustering_coefficient.md
+-rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/avg_degree.md
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/avg_indegree.md
+-rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/avg_outdegree.md
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/betweeness_centrality.md
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/common_neighbor.md
+-rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/cosine_similarity.md
+-rw-r--r--   0        0        0     2349 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/degree.md
+-rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/degree_centrality.md
+-rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/diameter_range.md
+-rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/distance.md
+-rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/eigenvector_centrality.md
+-rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/indegree.md
+-rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/infomap.md
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/is_connected.md
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/is_reachable.md
+-rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/is_triangle.md
+-rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/jaccard_similarity.md
+-rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/label_propagation.md
+-rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/local_lustering_coefficient.md
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/louvain.md
+-rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/max_degree.md
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/max_indegree.md
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/max_outdegree.md
+-rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/min_degree.md
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/min_indegree.md
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/min_outdegree.md
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/num_edges.md
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/num_nodes.md
+-rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/num_triangles.md
+-rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/outdegree.md
+-rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/pagerank.md
+-rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/preferential_attachment.md
+-rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/reachable_from.md
+-rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/triangles.md
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/weakly_connected_component.md
+-rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/weighted_cosine_similarity.md
+-rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/weighted_degree_centrality.md
+-rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/weighted_distance.md
+-rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/weighted_jaccard_similarity.md
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Edge/README.md
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Edge/add.md
+-rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Edge/call__.md
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Edge/extend.md
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/EdgeInstance/README.md
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/EdgeInstance/from_.md
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/EdgeInstance/set.md
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/EdgeInstance/to.md
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Graph/Edge.md
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Graph/Node.md
+-rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Graph/README.md
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Graph/compute.md
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Graph/fetch.md
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Graph/id.md
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Graph/model.md
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Graph/undirected.md
+-rw-r--r--   0        0        0     4167 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Graph/visualize.md
+-rw-r--r--   0        0        0    20679 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Graph/img/graph-viz-with-labels-and-colors.png
+-rw-r--r--   0        0        0    15558 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Graph/img/graph-viz.png
+-rw-r--r--   0        0        0    14921 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/graphs/Graph/img/simple-social-network.png
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/math/README.md
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/math/abs.md
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/math/acos.md
+-rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/math/asin.md
+-rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/math/atan.md
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/math/cbrt.md
+-rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/math/ceil.md
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/math/cos.md
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/math/degrees.md
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/math/floor.md
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/math/isclose.md
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/math/log.md
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/math/radians.md
+-rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/math/sign.md
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/math/sin.md
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/math/sqrt.md
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/math/tan.md
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/math/trunc_divide.md
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/strings/README.md
+-rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/strings/concat.md
+-rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/strings/contains.md
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/strings/ends_with.md
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/strings/join.md
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/strings/length.md
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/strings/like.md
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/strings/lowercase.md
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/strings/regex_compile.md
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/strings/regex_match.md
+-rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/strings/replace.md
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/strings/split.md
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/strings/split_part.md
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/python/std/strings/uppercase.md
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/api_reference/sql/README.md
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/faq/README.md
+-rw-r--r--   0        0        0     3175 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/faq/engines.md
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/README.md
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/cdc.py
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/custom_snowflake_connection.py
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/emit_playground.py
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/found.py
+-rw-r--r--   0        0        0     6699 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/fraud.ipynb
+-rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/fraud.py
+-rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/graph_algos.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/load_raw.py
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/nested.py
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/or_types.py
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/remote_load_csv.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/requirements.txt
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/simple.py
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/simple_recursion.py
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/simple_streamlit.py
+-rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/solver.py
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/weighted_graph_algos.py
+-rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/articles_graph/README.md
+-rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/articles_graph/articles_graph.py
+-rw-r--r--   0        0        0     5257 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/articles_graph/articles_graph_with_nlp.py
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/articles_graph/pyproject.toml
+-rw-r--r--   0        0        0     3399 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/articles_graph/utils.py
+-rw-r--r--   0        0        0  1274296 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/articles_graph/daily_articles/04_04_2024.json
+-rw-r--r--   0        0        0     4740 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/data/people.csv
+-rw-r--r--   0        0        0    10518 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/data/transactions.csv
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/ev_penetration/ev_penetration.py
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/ev_penetration/ev_penetration_csv.py
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/ev_penetration/state_stats.csv
+-rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/imdb/README.md
+-rw-r--r--   0        0        0   787694 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/imdb/imdb.csv
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/imdb/imdb.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/rel/bar.rel
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/rel/foo.rel
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/rel/solver.rel
+-rw-r--r--   0        0        0     6174 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/social-money-network/SF_pagerank.ipynb
+-rw-r--r--   0        0        0  2419367 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/social-money-network/Simulation-and-SF-Upload.ipynb
+-rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 relationalai-0.2.9/examples/social-money-network/snowflake_pagerank.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/.gitignore
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/README.md
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/index.html
+-rw-r--r--   0        0        0   463836 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/package-lock.json
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/package.json
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/tsconfig.json
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/vite.config.ts
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/.storybook/main.ts
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/.storybook/preview-body.html
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/.storybook/preview-head.html
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/.storybook/preview.ts
+-rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/App.styl
+-rw-r--r--   0        0        0     6535 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/App.tsx
+-rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/Selection.tsx
+-rw-r--r--   0        0        0    11770 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/debugger_client.ts
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/index.css
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/index.tsx
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/logo.svg
+-rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/util.styl
+-rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/util.ts
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/ws.ts
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/assets/favicon.png
+-rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/EventList.styl
+-rw-r--r--   0        0        0     7185 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/EventList.tsx
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/EventViewer.styl
+-rw-r--r--   0        0        0     5165 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/EventViewer.tsx
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/FileDropZone.styl
+-rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/FileDropZone.tsx
+-rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/Sidebar.styl
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/Sidebar.tsx
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/Schematic/NodeIcon.stories.tsx
+-rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/Schematic/ScopeProvider.tsx
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/Schematic/index.stories.tsx
+-rw-r--r--   0        0        0     4742 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/Schematic/index.styl
+-rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/Schematic/index.tsx
+-rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/Schematic/nodes/CallNode.tsx
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/Schematic/nodes/ComputeNode.tsx
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/Schematic/nodes/EffectNode.tsx
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/Schematic/nodes/FilterNode.tsx
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/Schematic/nodes/GetNode.tsx
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/Schematic/nodes/QuantifyNode.tsx
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/Schematic/nodes/ReturnNode.tsx
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/Schematic/nodes/SequenceNode.tsx
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/Schematic/nodes/UnionNode.tsx
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/Schematic/nodes/UnknownNode.tsx
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/Schematic/nodes/base.styl
+-rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/Schematic/nodes/base.tsx
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/Schematic/nodes/index.tsx
+-rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/ui/Accordion.stories.tsx
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/ui/Accordion.styl
+-rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/ui/Accordion.tsx
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/ui/Breadcrumbs.stories.tsx
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/ui/Breadcrumbs.styl
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/ui/Breadcrumbs.tsx
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/ui/Button.styl
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/ui/Button.tsx
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/ui/Code.styl
+-rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/ui/Code.tsx
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/ui/Collapsible.stories.tsx
+-rw-r--r--   0        0        0     4220 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/ui/Collapsible.styl
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/ui/Collapsible.tsx
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/ui/Field.stories.tsx
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/ui/Field.styl
+-rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/ui/Field.tsx
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/ui/Icon.styl
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/ui/Icon.tsx
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/ui/Modal.stories.tsx
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/ui/Modal.styl
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/ui/Modal.tsx
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/ui/Tooltip.stories.tsx
+-rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/ui/Tooltip.styl
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/components/ui/Tooltip.tsx
+-rw-r--r--   0        0        0     4529 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/fixtures/branch-improved.json
+-rw-r--r--   0        0        0     5229 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/fixtures/branch.json
+-rw-r--r--   0        0        0    67308 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/fixtures/fraud.json
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/fixtures/index.ts
+-rw-r--r--   0        0        0     9536 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/fixtures/not_found.json
+-rw-r--r--   0        0        0     6685 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/fixtures/simple.json
+-rw-r--r--   0        0        0     6271 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/fixtures/union.json
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/types/json.d.ts
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/types/jsx.d.ts
+-rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/types/mech.d.ts
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 relationalai-0.2.9/frontend/debugger/src/utils/fileUtils.ts
+-rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/gentest/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/gentest/__init__.py
+-rw-r--r--   0        0        0    12329 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/gentest/emit.py
+-rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/gentest/exec.py
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/gentest/fixtures.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/gentest/patch.py
+-rw-r--r--   0        0        0     7629 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/gentest/util.py
+-rwxr-xr-x   0        0        0     3521 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/gentest/cli/__main__.py
+-rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/gentest/cli/collect_failures.py
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/gentest/cli/collect_tests.py
+-rw-r--r--   0        0        0     5707 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/gentest/cli/repro.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/gentest/cli/run_tests.py
+-rw-r--r--   0        0        0    15710 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/gentest/cli/watch.py
+-rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/gentest/gen/action.py
+-rw-r--r--   0        0        0     5461 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/gentest/gen/context.py
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/gentest/gen/document.py
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/gentest/gen/error.py
+-rw-r--r--   0        0        0     6095 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/gentest/gen/group_limited.py
+-rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/gentest/gen/ir.py
+-rw-r--r--   0        0        0    17029 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/gentest/gen/scope.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/gentest/gen/staged.py
+-rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/gentest/gen/task.py
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/gentest/gen/test.py
+-rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/gentest/harness/database.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/gentest/harness/vendor_types.py
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/gentest/validate/diff.py
+-rw-r--r--   0        0        0     5588 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/gentest/validate/errors.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/gentest/validate/mapping.py
+-rw-r--r--   0        0        0     5426 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/gentest/validate/roundtrip.py
+-rw-r--r--   0        0        0     2677 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/__init__.py
+-rw-r--r--   0        0        0     6310 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/compiler.py
+-rw-r--r--   0        0        0    12665 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/debugging.py
+-rw-r--r--   0        0        0    46572 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/dsl.py
+-rw-r--r--   0        0        0    15741 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/errors.py
+-rw-r--r--   0        0        0    26752 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/metagen.py
+-rw-r--r--   0        0        0    27989 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/metamodel.py
+-rw-r--r--   0        0        0    19780 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/rel.py
+-rw-r--r--   0        0        0    20453 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/rel2.py
+-rw-r--r--   0        0        0    13371 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/rel_emitter.py
+-rw-r--r--   0        0        0     3549 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/rel_utils.py
+-rw-r--r--   0        0        0     8570 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/analysis/mechanistic.py
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/analysis/whynot.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/clients/__init__.py
+-rw-r--r--   0        0        0    14725 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/clients/azure.py
+-rw-r--r--   0        0        0    11981 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/clients/client.py
+-rw-r--r--   0        0        0    17625 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/clients/config.py
+-rw-r--r--   0        0        0    39864 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/clients/snowflake.py
+-rw-r--r--   0        0        0     5526 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/clients/test.py
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/clients/types.py
+-rw-r--r--   0        0        0     7529 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/loaders/csv.py
+-rw-r--r--   0        0        0     7140 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/loaders/loader.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/loaders/types.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/std/__init__.py
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/std/aggregates.py
+-rw-r--r--   0        0        0    24099 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/std/graphs.py
+-rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/std/math.py
+-rw-r--r--   0        0        0     2785 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/std/strings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/tools/__init__.py
+-rw-r--r--   0        0        0    59285 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/tools/cli.py
+-rw-r--r--   0        0        0    12721 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/tools/cli_controls.py
+-rw-r--r--   0        0        0     6886 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/tools/debugger.py
+-rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/tools/debugger_client.py
+-rw-r--r--   0        0        0     5341 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/tools/debugger_server.py
+-rw-r--r--   0        0        0     9121 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/tools/dev.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/tools/notes
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/util/constants.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/util/format.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/util/keys.py
+-rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/util/snowflake_logger.py
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 relationalai-0.2.9/src/relationalai/util/tracing_logger.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/__init__.py
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/conftest.py
+-rw-r--r--   0        0        0     5346 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/util.py
+-rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/benchmarks/conftest.py
+-rw-r--r--   0        0        0     2584 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/benchmarks/test_heap_snapshots.py
+-rw-r--r--   0        0        0     4125 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/benchmarks/test_tastybytes.py
+-rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/README.md
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/conftest.py
+-rw-r--r--   0        0        0     8133 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/test_graph_visualize.py
+-rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/test_snapshots.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/after_errors/query0.txt
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/after_errors/query1.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/agg_ordering/query0.txt
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/bool/query0.txt
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/bool/query1.txt
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/bottom/query0.txt
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/first/query0.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__basics/query0.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__basics/query1.txt
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query0.txt
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query1.txt
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query2.txt
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query3.txt
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query4.txt
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__clustering/query0.txt
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__clustering/query1.txt
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query0.txt
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query1.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query2.txt
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query3.txt
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query4.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query5.txt
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__connectivity/query0.txt
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__connectivity/query1.txt
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__connectivity/query2.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query0.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query1.txt
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query10.txt
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query11.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query2.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query3.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query4.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query5.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query6.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query7.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query8.txt
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query9.txt
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__distance/query0.txt
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__distance/query1.txt
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__distance/query2.txt
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__link_prediction/query0.txt
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__link_prediction/query1.txt
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__link_prediction/query2.txt
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__mixed_value_types/query0.txt
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__similarity/query0.txt
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__similarity/query1.txt
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__similarity/query2.txt
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__similarity/query3.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__triangles/query0.txt
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__triangles/query1.txt
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__triangles/query2.txt
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__triangles/query3.txt
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__triangles/query4.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query0.txt
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query1.txt
+-rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query2.txt
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query3.txt
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query4.txt
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/not_found/query0.txt
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/not_found/query1.txt
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/numeric_outputs/query0.txt
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/numeric_outputs/query1.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query0.txt
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query1.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query2.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query3.txt
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/smoke/query0.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/smoke/query1.txt
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query0.txt
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query1.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query10.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query11.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query12.txt
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query13.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query14.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query15.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query16.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query17.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query2.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query3.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query4.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query5.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query6.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query7.txt
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query8.txt
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/std_math/query9.txt
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query0.txt
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query1.txt
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query10.txt
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query2.txt
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query3.txt
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query4.txt
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query5.txt
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query6.txt
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query7.txt
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query8.txt
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query9.txt
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/top/query0.txt
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/union/query0.txt
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query0.txt
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query1.txt
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query2.txt
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query3.txt
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query4.txt
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query5.txt
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/test_cases/after_errors.py
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/test_cases/agg_ordering.py
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/test_cases/bool.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/test_cases/bottom.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/test_cases/export.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/test_cases/first.py
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/test_cases/multi_valued.py
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/test_cases/not_found.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/test_cases/numeric_outputs.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/test_cases/out_of_context.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/test_cases/persist.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/test_cases/smoke.py
+-rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/test_cases/std_math.py
+-rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/test_cases/strings.py
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/test_cases/top.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/test_cases/union.py
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/test_cases/weighted_graphs.py
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/test_cases/graphs/basics.py
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/test_cases/graphs/centrality.py
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/test_cases/graphs/clustering.py
+-rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/test_cases/graphs/community.py
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/test_cases/graphs/connectivity.py
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/test_cases/graphs/degree.py
+-rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/test_cases/graphs/distance.py
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/test_cases/graphs/link_prediction.py
+-rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/test_cases/graphs/mixed_value_types.py
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/test_cases/graphs/similarity.py
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/end2end/test_cases/graphs/triangles.py
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/execution/test_core.py
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/execution/test_examples.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/execution/basic/smoketest.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/execution/snapshots/test_core/test_basic/smoketest/query0.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/execution/snapshots/test_examples/test_example/emit_playground/query0.txt
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/execution/snapshots/test_examples/test_example/found/query0.txt
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/execution/snapshots/test_examples/test_example/graph/query0.txt
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/execution/snapshots/test_examples/test_example/graph/query1.txt
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/execution/snapshots/test_examples/test_example/load_raw/query0.txt
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/execution/snapshots/test_examples/test_example/or_types/query0.txt
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/execution/snapshots/test_examples/test_example/simple/query0.txt
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/execution/snapshots/test_examples/test_example/simple_recursion/query0.txt
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/execution/snapshots/test_examples/test_example/simple_streamlit/query0.txt
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/execution/snapshots/test_examples/test_example/test/query0.txt
+-rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/init-cli/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/init-cli/__init__.py
+-rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/init-cli/azure_basic.py
+-rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/init-cli/common.py
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/roundtrip/test_document.py
+-rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/roundtrip/test_task.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/unit/test_config_store.py
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/unit/test_configs/config_with_new_profile.toml
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/unit/test_configs/printed_config.txt
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 relationalai-0.2.9/tests/unit/test_configs/raiconfig_example.toml
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 relationalai-0.2.9/.gitignore
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 relationalai-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 relationalai-0.2.9/docs/pypi/README.md
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 relationalai-0.2.9/PKG-INFO
```

### Comparing `relationalai-0.2.8/README.md` & `relationalai-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/.github/actions/benchmarks/action.yml` & `relationalai-0.2.9/.github/actions/benchmarks/action.yml`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/.github/actions/end-to-end/action.yml` & `relationalai-0.2.9/.github/actions/end-to-end/action.yml`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/.github/workflows/benchmarks.yml` & `relationalai-0.2.9/.github/workflows/benchmarks.yml`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/.github/workflows/end-to-end.yml` & `relationalai-0.2.9/.github/workflows/end-to-end.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,57 +1,59 @@
 name: Run End To End Tests
 
 on:
   push:
-    branches: [main]
+    branches: [ main ]
   pull_request:
-    branches: [main]
+    branches: [ main ]
 
 concurrency:
   group:
     ${{ github.workflow }}-${{ (github.ref_name == 'main' || github.event_name == 'workflow_dispatch')
     && github.run_id
     || github.ref }}
-  cancel-in-progress: true 
+  cancel-in-progress: true
 
 jobs:
   test:
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
         include:
           - python-version: '3.12'
             cloud-provider: 'snowflake'
           - python-version: '3.10'
             cloud-provider: 'azure'
     steps:
 
-    - uses: actions/checkout@v4
-      name: Checkout repository
-
-    - uses: ./.github/actions/end-to-end
-      with:
-        python_version: ${{ matrix.python-version }}
-        rai_cloud_provider: ${{ matrix.cloud-provider }}
-        rai_client_id: ${{ secrets.RAI_CLIENT_ID }}
-        rai_client_secret: ${{ secrets.RAI_CLIENT_SECRET }}
-        sf_account: ndsoebe-rai_integration_aws_uswest_1_consumer
-        sf_warehouse: int_env_wh
-        sf_rai_app_name: rai_int_app
-        sf_compute_pool: int_env_benchmark_compute_xs
-        sf_username: team-prod-experience@relational.ai
-        sf_password: ${{ secrets.SF_TEST_ACCOUNT_PASSWORD }}
-        datadog_api_key: ${{ secrets.DD_API_KEY }}
-        sf_reporting_password: ${{ secrets.SF_REPORTING_PASSWORD }}
-    
-    - name: Upload Coverage Artifact
-      uses: actions/upload-artifact@v2
-      with:
-        name: coverage-artifact-${{ matrix.python-version }}
-        path: coverage/lcov.info
-
-    - name: Upload Coverage Report
-      uses: actions/upload-artifact@v2
-      with:
-        name: coverage-report-${{ matrix.python-version }}
-        path: coverage/html-report
+      - uses: actions/checkout@v4
+        name: Checkout repository
+        with:
+          ref: ${{ github.event_name == 'pull_request' && github.event.pull_request.head.sha || github.sha }}
+
+      - uses: ./.github/actions/end-to-end
+        with:
+          python_version: ${{ matrix.python-version }}
+          rai_cloud_provider: ${{ matrix.cloud-provider }}
+          rai_client_id: ${{ secrets.RAI_CLIENT_ID }}
+          rai_client_secret: ${{ secrets.RAI_CLIENT_SECRET }}
+          sf_account: ndsoebe-rai_integration_aws_uswest_1_consumer
+          sf_warehouse: int_env_wh
+          sf_rai_app_name: rai_int_app
+          sf_compute_pool: int_env_benchmark_compute_xs
+          sf_username: team-prod-experience@relational.ai
+          sf_password: ${{ secrets.SF_TEST_ACCOUNT_PASSWORD }}
+          datadog_api_key: ${{ secrets.DD_API_KEY }}
+          sf_reporting_password: ${{ secrets.SF_REPORTING_PASSWORD }}
+
+      - name: Upload Coverage Artifact
+        uses: actions/upload-artifact@v2
+        with:
+          name: coverage-artifact-${{ matrix.python-version }}
+          path: coverage/lcov.info
+
+      - name: Upload Coverage Report
+        uses: actions/upload-artifact@v2
+        with:
+          name: coverage-report-${{ matrix.python-version }}
+          path: coverage/html-report
```

### Comparing `relationalai-0.2.8/.github/workflows/publish-to-pypi.yml` & `relationalai-0.2.9/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/.github/workflows/ruff.yml` & `relationalai-0.2.9/.github/workflows/ruff.yml`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 name: Python Ruff Lint
 
 on:
   pull_request:
-    branches: [main]
+    branches: [ main ]
 
 concurrency:
   group:
     ${{ github.workflow }}-${{ (github.ref_name == 'main' || github.event_name == 'workflow_dispatch')
     && github.run_id
     || github.ref }}
-  cancel-in-progress: true 
+  cancel-in-progress: true
 
 jobs:
   lint-and-format:
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
+        with:
+          ref: ${{ github.event_name == 'pull_request' && github.event.pull_request.head.sha || github.sha }}
 
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
           python-version: '3.11'
 
       - name: Create and activate virtual environment
@@ -27,8 +29,8 @@
           python -m venv .venv
       - name: Install dependencies
         run: |
           .venv/bin/python -m pip install --upgrade pip
           .venv/bin/pip install ruff
       - name: Run Ruff Check
         run: .venv/bin/ruff check
-        id: ruff_check
+        id: ruff_check
```

### Comparing `relationalai-0.2.8/docs/getting_started.md` & `relationalai-0.2.9/docs/getting_started.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/_old/OLD_pyrel_quickstart.md` & `relationalai-0.2.9/docs/_old/OLD_pyrel_quickstart.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/_old/metamodel.md` & `relationalai-0.2.9/docs/_old/metamodel.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/_old/python_dsl.md` & `relationalai-0.2.9/docs/_old/python_dsl.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/_old/quickstart.md` & `relationalai-0.2.9/docs/_old/quickstart.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/configuration/README.md` & `relationalai-0.2.9/docs/api_reference/configuration/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/Expression.md` & `relationalai-0.2.9/docs/api_reference/python/Expression.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/Property.md` & `relationalai-0.2.9/docs/api_reference/python/Property.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/README.md` & `relationalai-0.2.9/docs/api_reference/python/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/Context/README.md` & `relationalai-0.2.9/docs/api_reference/python/Context/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/Context/enter__.md` & `relationalai-0.2.9/docs/api_reference/python/Context/enter__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/Context/exit__.md` & `relationalai-0.2.9/docs/api_reference/python/Context/exit__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/Context/iter__.md` & `relationalai-0.2.9/docs/api_reference/python/Context/iter__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/Context/model.md` & `relationalai-0.2.9/docs/api_reference/python/Context/model.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/Context/results.md` & `relationalai-0.2.9/docs/api_reference/python/Context/results.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/ContextSelect/README.md` & `relationalai-0.2.9/docs/api_reference/python/ContextSelect/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/ContextSelect/add.md` & `relationalai-0.2.9/docs/api_reference/python/ContextSelect/add.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/ContextSelect/call__.md` & `relationalai-0.2.9/docs/api_reference/python/ContextSelect/call__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/ContextSelect/getattribute__.md` & `relationalai-0.2.9/docs/api_reference/python/ContextSelect/getattribute__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/Instance/README.md` & `relationalai-0.2.9/docs/api_reference/python/Instance/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/Instance/persist.md` & `relationalai-0.2.9/docs/api_reference/python/Instance/persist.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/Instance/set.md` & `relationalai-0.2.9/docs/api_reference/python/Instance/set.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/Instance/unpersist.md` & `relationalai-0.2.9/docs/api_reference/python/Instance/unpersist.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/InstanceProperty/README.md` & `relationalai-0.2.9/docs/api_reference/python/InstanceProperty/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/InstanceProperty/or_.md` & `relationalai-0.2.9/docs/api_reference/python/InstanceProperty/or_.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/Model/README.md` & `relationalai-0.2.9/docs/api_reference/python/Model/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/Model/Type.md` & `relationalai-0.2.9/docs/api_reference/python/Model/Type.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/Model/found.md` & `relationalai-0.2.9/docs/api_reference/python/Model/found.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/Model/not_found.md` & `relationalai-0.2.9/docs/api_reference/python/Model/not_found.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/Model/ordered_choice.md` & `relationalai-0.2.9/docs/api_reference/python/Model/ordered_choice.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/Model/query.md` & `relationalai-0.2.9/docs/api_reference/python/Model/query.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/Model/read.md` & `relationalai-0.2.9/docs/api_reference/python/Model/read.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/Model/rule.md` & `relationalai-0.2.9/docs/api_reference/python/Model/rule.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/Model/scope.md` & `relationalai-0.2.9/docs/api_reference/python/Model/scope.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/Model/union.md` & `relationalai-0.2.9/docs/api_reference/python/Model/union.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/Producer/README.md` & `relationalai-0.2.9/docs/api_reference/python/Producer/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/Producer/add__.md` & `relationalai-0.2.9/docs/api_reference/python/Producer/add__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/Producer/enter__.md` & `relationalai-0.2.9/docs/api_reference/python/Producer/enter__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/Producer/eq__.md` & `relationalai-0.2.9/docs/api_reference/python/Producer/eq__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/Producer/exit__.md` & `relationalai-0.2.9/docs/api_reference/python/Producer/exit__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/Producer/floordiv__.md` & `relationalai-0.2.9/docs/api_reference/python/Producer/floordiv__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/Producer/ge__.md` & `relationalai-0.2.9/docs/api_reference/python/Producer/ge__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/Producer/getattribute__.md` & `relationalai-0.2.9/docs/api_reference/python/Producer/getattribute__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/Producer/gt__.md` & `relationalai-0.2.9/docs/api_reference/python/Producer/gt__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/Producer/le__.md` & `relationalai-0.2.9/docs/api_reference/python/Producer/le__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/Producer/lt__.md` & `relationalai-0.2.9/docs/api_reference/python/Producer/lt__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/Producer/mul__.md` & `relationalai-0.2.9/docs/api_reference/python/Producer/mul__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/Producer/ne__.md` & `relationalai-0.2.9/docs/api_reference/python/Producer/ne__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/Producer/pow__.md` & `relationalai-0.2.9/docs/api_reference/python/Producer/pow__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/Producer/sub__.md` & `relationalai-0.2.9/docs/api_reference/python/Producer/sub__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/Producer/truediv__.md` & `relationalai-0.2.9/docs/api_reference/python/Producer/truediv__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/Type/README.md` & `relationalai-0.2.9/docs/api_reference/python/Type/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/Type/add.md` & `relationalai-0.2.9/docs/api_reference/python/Type/add.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/Type/call__.md` & `relationalai-0.2.9/docs/api_reference/python/Type/call__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/Type/extend.md` & `relationalai-0.2.9/docs/api_reference/python/Type/extend.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/Type/or__.md` & `relationalai-0.2.9/docs/api_reference/python/Type/or__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/clients/README.md` & `relationalai-0.2.9/docs/api_reference/python/clients/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/clients/snowflake/PrimaryKey.md` & `relationalai-0.2.9/docs/api_reference/python/clients/snowflake/PrimaryKey.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/clients/snowflake/README.md` & `relationalai-0.2.9/docs/api_reference/python/clients/snowflake/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/clients/snowflake/Snowflake.md` & `relationalai-0.2.9/docs/api_reference/python/clients/snowflake/Snowflake.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/clients/snowflake/SnowflakeTable/README.md` & `relationalai-0.2.9/docs/api_reference/python/clients/snowflake/SnowflakeTable/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/clients/snowflake/SnowflakeTable/describe.md` & `relationalai-0.2.9/docs/api_reference/python/clients/snowflake/SnowflakeTable/describe.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/clients/snowflake/SnowflakeTable/fqname.md` & `relationalai-0.2.9/docs/api_reference/python/clients/snowflake/SnowflakeTable/fqname.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/clients/snowflake/SnowflakeTable/namespace.md` & `relationalai-0.2.9/docs/api_reference/python/clients/snowflake/SnowflakeTable/namespace.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/README.md` & `relationalai-0.2.9/docs/api_reference/python/std/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/Vars.md` & `relationalai-0.2.9/docs/api_reference/python/std/Vars.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/alias.md` & `relationalai-0.2.9/docs/api_reference/python/std/alias.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/aggregates/README.md` & `relationalai-0.2.9/docs/api_reference/python/std/aggregates/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/aggregates/avg.md` & `relationalai-0.2.9/docs/api_reference/python/std/aggregates/avg.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/aggregates/count.md` & `relationalai-0.2.9/docs/api_reference/python/std/aggregates/count.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/aggregates/max.md` & `relationalai-0.2.9/docs/api_reference/python/std/aggregates/max.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/aggregates/min.md` & `relationalai-0.2.9/docs/api_reference/python/std/aggregates/min.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/aggregates/rank_asc.md` & `relationalai-0.2.9/docs/api_reference/python/std/aggregates/rank_asc.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/aggregates/rank_desc.md` & `relationalai-0.2.9/docs/api_reference/python/std/aggregates/rank_desc.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/aggregates/sum.md` & `relationalai-0.2.9/docs/api_reference/python/std/aggregates/sum.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/graphs/README.md` & `relationalai-0.2.9/docs/api_reference/python/std/graphs/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/README.md` & `relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/adamic_adar.md` & `relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/adamic_adar.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/average_clustering_coefficient.md` & `relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/average_clustering_coefficient.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/avg_degree.md` & `relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/avg_degree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/avg_indegree.md` & `relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/avg_indegree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/avg_outdegree.md` & `relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/avg_outdegree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/betweeness_centrality.md` & `relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/betweeness_centrality.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/common_neighbor.md` & `relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/common_neighbor.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/cosine_similarity.md` & `relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/cosine_similarity.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/degree.md` & `relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/degree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/degree_centrality.md` & `relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/degree_centrality.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/diameter_range.md` & `relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/diameter_range.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/distance.md` & `relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/distance.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/eigenvector_centrality.md` & `relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/eigenvector_centrality.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/indegree.md` & `relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/indegree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/infomap.md` & `relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/infomap.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/is_connected.md` & `relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/is_connected.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/is_reachable.md` & `relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/is_reachable.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/is_triangle.md` & `relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/is_triangle.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/jaccard_similarity.md` & `relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/jaccard_similarity.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/label_propagation.md` & `relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/label_propagation.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/local_lustering_coefficient.md` & `relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/local_lustering_coefficient.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/louvain.md` & `relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/louvain.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/max_degree.md` & `relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/max_degree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/max_indegree.md` & `relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/max_indegree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/max_outdegree.md` & `relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/max_outdegree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/min_degree.md` & `relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/min_degree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/min_indegree.md` & `relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/min_indegree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/min_outdegree.md` & `relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/min_outdegree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/num_edges.md` & `relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/num_edges.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/num_nodes.md` & `relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/num_nodes.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/num_triangles.md` & `relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/num_triangles.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/outdegree.md` & `relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/outdegree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/pagerank.md` & `relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/pagerank.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/preferential_attachment.md` & `relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/preferential_attachment.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/reachable_from.md` & `relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/reachable_from.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/triangles.md` & `relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/triangles.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/weakly_connected_component.md` & `relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/weakly_connected_component.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/weighted_cosine_similarity.md` & `relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/weighted_cosine_similarity.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/weighted_degree_centrality.md` & `relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/weighted_degree_centrality.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/weighted_distance.md` & `relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/weighted_distance.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/graphs/Compute/weighted_jaccard_similarity.md` & `relationalai-0.2.9/docs/api_reference/python/std/graphs/Compute/weighted_jaccard_similarity.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/graphs/Edge/README.md` & `relationalai-0.2.9/docs/api_reference/python/std/graphs/Edge/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/graphs/Edge/add.md` & `relationalai-0.2.9/docs/api_reference/python/std/graphs/Edge/add.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/graphs/Edge/call__.md` & `relationalai-0.2.9/docs/api_reference/python/std/graphs/Edge/call__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/graphs/Edge/extend.md` & `relationalai-0.2.9/docs/api_reference/python/std/graphs/Edge/extend.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/graphs/EdgeInstance/README.md` & `relationalai-0.2.9/docs/api_reference/python/std/graphs/EdgeInstance/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/graphs/EdgeInstance/from_.md` & `relationalai-0.2.9/docs/api_reference/python/std/graphs/EdgeInstance/from_.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/graphs/EdgeInstance/set.md` & `relationalai-0.2.9/docs/api_reference/python/std/graphs/EdgeInstance/set.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/graphs/EdgeInstance/to.md` & `relationalai-0.2.9/docs/api_reference/python/std/graphs/EdgeInstance/to.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/graphs/Graph/Edge.md` & `relationalai-0.2.9/docs/api_reference/python/std/graphs/Graph/Edge.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/graphs/Graph/Node.md` & `relationalai-0.2.9/docs/api_reference/python/std/graphs/Graph/Node.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/graphs/Graph/README.md` & `relationalai-0.2.9/docs/api_reference/python/std/graphs/Graph/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/graphs/Graph/compute.md` & `relationalai-0.2.9/docs/api_reference/python/std/graphs/Graph/compute.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/graphs/Graph/fetch.md` & `relationalai-0.2.9/docs/api_reference/python/std/graphs/Graph/fetch.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/graphs/Graph/id.md` & `relationalai-0.2.9/docs/api_reference/python/std/graphs/Graph/id.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/graphs/Graph/model.md` & `relationalai-0.2.9/docs/api_reference/python/std/graphs/Graph/model.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/graphs/Graph/undirected.md` & `relationalai-0.2.9/docs/api_reference/python/std/graphs/Graph/undirected.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/graphs/Graph/visualize.md` & `relationalai-0.2.9/docs/api_reference/python/std/graphs/Graph/visualize.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/graphs/Graph/img/graph-viz-with-labels-and-colors.png` & `relationalai-0.2.9/docs/api_reference/python/std/graphs/Graph/img/graph-viz-with-labels-and-colors.png`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/graphs/Graph/img/graph-viz.png` & `relationalai-0.2.9/docs/api_reference/python/std/graphs/Graph/img/graph-viz.png`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/graphs/Graph/img/simple-social-network.png` & `relationalai-0.2.9/docs/api_reference/python/std/graphs/Graph/img/simple-social-network.png`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/math/README.md` & `relationalai-0.2.9/docs/api_reference/python/std/math/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/math/abs.md` & `relationalai-0.2.9/docs/api_reference/python/std/math/abs.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/math/acos.md` & `relationalai-0.2.9/docs/api_reference/python/std/math/acos.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/math/asin.md` & `relationalai-0.2.9/docs/api_reference/python/std/math/asin.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/math/atan.md` & `relationalai-0.2.9/docs/api_reference/python/std/math/atan.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/math/cbrt.md` & `relationalai-0.2.9/docs/api_reference/python/std/math/cbrt.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/math/ceil.md` & `relationalai-0.2.9/docs/api_reference/python/std/math/ceil.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/math/cos.md` & `relationalai-0.2.9/docs/api_reference/python/std/math/cos.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/math/degrees.md` & `relationalai-0.2.9/docs/api_reference/python/std/math/degrees.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/math/floor.md` & `relationalai-0.2.9/docs/api_reference/python/std/math/floor.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/math/isclose.md` & `relationalai-0.2.9/docs/api_reference/python/std/math/isclose.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/math/log.md` & `relationalai-0.2.9/docs/api_reference/python/std/math/log.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/math/radians.md` & `relationalai-0.2.9/docs/api_reference/python/std/math/radians.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/math/sign.md` & `relationalai-0.2.9/docs/api_reference/python/std/math/sign.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/math/sin.md` & `relationalai-0.2.9/docs/api_reference/python/std/math/sin.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/math/sqrt.md` & `relationalai-0.2.9/docs/api_reference/python/std/math/sqrt.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/math/tan.md` & `relationalai-0.2.9/docs/api_reference/python/std/math/tan.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/math/trunc_divide.md` & `relationalai-0.2.9/docs/api_reference/python/std/math/trunc_divide.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/strings/README.md` & `relationalai-0.2.9/docs/api_reference/python/std/strings/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/strings/concat.md` & `relationalai-0.2.9/docs/api_reference/python/std/strings/concat.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/strings/contains.md` & `relationalai-0.2.9/docs/api_reference/python/std/strings/contains.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/strings/ends_with.md` & `relationalai-0.2.9/docs/api_reference/python/std/strings/ends_with.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/strings/join.md` & `relationalai-0.2.9/docs/api_reference/python/std/strings/join.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/strings/length.md` & `relationalai-0.2.9/docs/api_reference/python/std/strings/length.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/strings/like.md` & `relationalai-0.2.9/docs/api_reference/python/std/strings/like.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/strings/lowercase.md` & `relationalai-0.2.9/docs/api_reference/python/std/strings/lowercase.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/strings/regex_compile.md` & `relationalai-0.2.9/docs/api_reference/python/std/strings/regex_compile.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/strings/regex_match.md` & `relationalai-0.2.9/docs/api_reference/python/std/strings/regex_match.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/strings/replace.md` & `relationalai-0.2.9/docs/api_reference/python/std/strings/replace.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/strings/split.md` & `relationalai-0.2.9/docs/api_reference/python/std/strings/split.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/strings/split_part.md` & `relationalai-0.2.9/docs/api_reference/python/std/strings/split_part.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/api_reference/python/std/strings/uppercase.md` & `relationalai-0.2.9/docs/api_reference/python/std/strings/uppercase.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/docs/faq/engines.md` & `relationalai-0.2.9/docs/faq/engines.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,38 @@
 # RelationalAI Engine FAQ
 
 ## How are concurrent workloads handled by an engine?
 
 Engines are the primary mechanism for performance isolation.
+Load balancing across engines is not automatic, so you retain control over each engine's workload.
+
 As a general rule, all workloads executing concurrently against the same engine affect each other in some way.
 Use separate engines whenever you want to avoid different users having to coordinate their usage.
 
 To illustrate, let's say two developers A and B are working on separate [models](../api_reference/python/Model/README.md),
 but both are using the same engine.
 Now A loads a large amount of test data.
 While the load is ongoing, B will see their model changes spinning.
 Then say B introduces an error into their model, unintentionally causing a very expensive, unconstrained computation.
 As this happens, A will suddenly experience performance degradation.
 
+An engine can queue up to 128 transactions, and this limit is currently not configurable.
+Queued transactions follow a first-in/first-out priority.
+Engine failure cancels queued transactions by marking their status as `ABORTED` with the reason  `'engine failed'`.
+A full queue rejects new transactions, returning [HTTP error 429](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status/429).
+
+Each engine, regardless of size, can concurrently execute up to 8 transactions.
+Currently, this limit is non-configurable.
+High-resource transactions will be serialized.
+For executing large graph algorithms, we recommend sequential execution or using separate engines.
+
+All writes to a RelationalAI database on the _same engine_ are serialized and concurrent writes are queued.
+For concurrent writes to the same database _across engines_, only one commits, while others must retry.
+Avoid writing to the same database from different engines.
+
 ## How can I tell if I need more engines?
 
 Use the[RelationalAI CLI](../api_reference/cli/README.md) to check the status of your transactions:
 
 ```sh
 rai transactions:list
 ```
```

### Comparing `relationalai-0.2.8/examples/README.md` & `relationalai-0.2.9/examples/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/examples/cdc.py` & `relationalai-0.2.9/examples/cdc.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/examples/custom_snowflake_connection.py` & `relationalai-0.2.9/examples/custom_snowflake_connection.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/examples/emit_playground.py` & `relationalai-0.2.9/examples/emit_playground.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/examples/found.py` & `relationalai-0.2.9/examples/found.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/examples/fraud.ipynb` & `relationalai-0.2.9/examples/fraud.ipynb`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/examples/fraud.py` & `relationalai-0.2.9/examples/fraud.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/examples/graph_algos.py` & `relationalai-0.2.9/examples/graph_algos.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/examples/nested.py` & `relationalai-0.2.9/examples/nested.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/examples/or_types.py` & `relationalai-0.2.9/examples/or_types.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/examples/remote_load_csv.py` & `relationalai-0.2.9/examples/remote_load_csv.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/examples/simple_recursion.py` & `relationalai-0.2.9/examples/simple_recursion.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/examples/simple_streamlit.py` & `relationalai-0.2.9/examples/simple_streamlit.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/examples/solver.py` & `relationalai-0.2.9/examples/solver.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/examples/weighted_graph_algos.py` & `relationalai-0.2.9/examples/weighted_graph_algos.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/examples/articles_graph/README.md` & `relationalai-0.2.9/examples/articles_graph/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/examples/articles_graph/articles_graph.py` & `relationalai-0.2.9/examples/articles_graph/articles_graph.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/examples/articles_graph/articles_graph_with_nlp.py` & `relationalai-0.2.9/examples/articles_graph/articles_graph_with_nlp.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/examples/articles_graph/utils.py` & `relationalai-0.2.9/examples/articles_graph/utils.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/examples/articles_graph/daily_articles/04_04_2024.json` & `relationalai-0.2.9/examples/articles_graph/daily_articles/04_04_2024.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/examples/data/people.csv` & `relationalai-0.2.9/examples/data/people.csv`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/examples/data/transactions.csv` & `relationalai-0.2.9/examples/data/transactions.csv`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/examples/ev_penetration/ev_penetration.py` & `relationalai-0.2.9/examples/ev_penetration/ev_penetration.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/examples/ev_penetration/ev_penetration_csv.py` & `relationalai-0.2.9/examples/ev_penetration/ev_penetration_csv.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/examples/ev_penetration/state_stats.csv` & `relationalai-0.2.9/examples/ev_penetration/state_stats.csv`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/examples/imdb/README.md` & `relationalai-0.2.9/examples/imdb/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/examples/imdb/imdb.csv` & `relationalai-0.2.9/examples/imdb/imdb.csv`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/examples/imdb/imdb.py` & `relationalai-0.2.9/examples/imdb/imdb.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/examples/rel/solver.rel` & `relationalai-0.2.9/examples/rel/solver.rel`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/examples/social-money-network/SF_pagerank.ipynb` & `relationalai-0.2.9/examples/social-money-network/SF_pagerank.ipynb`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/examples/social-money-network/Simulation-and-SF-Upload.ipynb` & `relationalai-0.2.9/examples/social-money-network/Simulation-and-SF-Upload.ipynb`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/examples/social-money-network/snowflake_pagerank.py` & `relationalai-0.2.9/examples/social-money-network/snowflake_pagerank.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/frontend/debugger/package-lock.json` & `relationalai-0.2.9/frontend/debugger/package-lock.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/frontend/debugger/package.json` & `relationalai-0.2.9/frontend/debugger/package.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/frontend/debugger/tsconfig.json` & `relationalai-0.2.9/frontend/debugger/tsconfig.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/frontend/debugger/vite.config.ts` & `relationalai-0.2.9/frontend/debugger/vite.config.ts`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/frontend/debugger/.storybook/main.ts` & `relationalai-0.2.9/frontend/debugger/.storybook/main.ts`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/frontend/debugger/src/App.styl` & `relationalai-0.2.9/frontend/debugger/src/App.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/frontend/debugger/src/App.tsx` & `relationalai-0.2.9/frontend/debugger/src/App.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/frontend/debugger/src/Selection.tsx` & `relationalai-0.2.9/frontend/debugger/src/Selection.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/frontend/debugger/src/debugger_client.ts` & `relationalai-0.2.9/frontend/debugger/src/debugger_client.ts`

 * *Files 2% similar despite different names*

```diff
@@ -257,15 +257,15 @@
     protected _send(msg: any) {
         this.connection.send(JSON.stringify(msg));
     }
 
     protected handle_span_start(msg: Message.SpanStart) {
         this.set_root(produce((root) => {
             let parent = get_in(root, this.path);
-            if(!parent || !Span.is_span(parent)) throw new Error();
+            if(!parent || !Span.is_span(parent)) throw new Error(`Parent not found at path ${this.path}`);
             this.path.push(parent.events.length);
             let span_type = msg.span.type;
             let sub: Span = {
                 ...msg.span.attrs,
                 start_time: new Date(msg.span.start_timestamp),
                 end_time: undefined,
                 span_type,
@@ -278,30 +278,30 @@
             parent.events.push(sub)
         }));
     }
 
     protected handle_span_end(msg: Message.SpanEnd) {
         this.set_root(produce((root) => {
             let start = get_in(root, this.path);
-            if(!start || !Span.is_span(start)) throw new Error();
+            if(!start || !Span.is_span(start)) throw new Error(`Start not found at path ${this.path}`);
             start.end_time = new Date(msg.end_timestamp);
             start.elapsed = (start.end_time.getTime() - start.start_time.getTime()) / 1000;
             
             for (let key in msg.end_attrs) {
                 if (key === "span" || key === "event") continue;
                 start[key] = msg[key];
             }
             this.path.pop();
         }));
     }
 
     protected handle_event(msg: Message.Event) {
         this.set_root(produce((root) => {
             let span = get_in(root, this.path);
-            if(!span || !Span.is_span(span)) throw new Error();
+            if(!span || !Span.is_span(span)) throw new Error(`Span not found at path ${this.path}`);
             msg.selection_path = [...this.path, span.events.length],
             Object.defineProperty(msg, "parent", {value: unwrap(span), enumerable: false, configurable: true, writable: true});
             span.events.push(msg);
         }));
     }
 
     protected handle_message = (msg: Message) => {
```

### Comparing `relationalai-0.2.8/frontend/debugger/src/index.tsx` & `relationalai-0.2.9/frontend/debugger/src/index.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/frontend/debugger/src/logo.svg` & `relationalai-0.2.9/frontend/debugger/src/logo.svg`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/frontend/debugger/src/util.styl` & `relationalai-0.2.9/frontend/debugger/src/util.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/frontend/debugger/src/util.ts` & `relationalai-0.2.9/frontend/debugger/src/util.ts`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/frontend/debugger/src/assets/favicon.png` & `relationalai-0.2.9/frontend/debugger/src/assets/favicon.png`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/frontend/debugger/src/components/EventList.styl` & `relationalai-0.2.9/frontend/debugger/src/components/EventList.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/frontend/debugger/src/components/EventList.tsx` & `relationalai-0.2.9/frontend/debugger/src/components/EventList.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/frontend/debugger/src/components/EventViewer.tsx` & `relationalai-0.2.9/frontend/debugger/src/components/EventViewer.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/frontend/debugger/src/components/FileDropZone.styl` & `relationalai-0.2.9/frontend/debugger/src/components/FileDropZone.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/frontend/debugger/src/components/FileDropZone.tsx` & `relationalai-0.2.9/frontend/debugger/src/components/FileDropZone.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/frontend/debugger/src/components/Sidebar.styl` & `relationalai-0.2.9/frontend/debugger/src/components/Sidebar.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/frontend/debugger/src/components/Sidebar.tsx` & `relationalai-0.2.9/frontend/debugger/src/components/Sidebar.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/frontend/debugger/src/components/Schematic/NodeIcon.stories.tsx` & `relationalai-0.2.9/frontend/debugger/src/components/Schematic/NodeIcon.stories.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/frontend/debugger/src/components/Schematic/ScopeProvider.tsx` & `relationalai-0.2.9/frontend/debugger/src/components/Schematic/ScopeProvider.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/frontend/debugger/src/components/Schematic/index.stories.tsx` & `relationalai-0.2.9/frontend/debugger/src/components/Schematic/index.stories.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/frontend/debugger/src/components/Schematic/index.styl` & `relationalai-0.2.9/frontend/debugger/src/components/Schematic/index.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/frontend/debugger/src/components/Schematic/index.tsx` & `relationalai-0.2.9/frontend/debugger/src/components/Schematic/index.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/frontend/debugger/src/components/Schematic/nodes/CallNode.tsx` & `relationalai-0.2.9/frontend/debugger/src/components/Schematic/nodes/CallNode.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/frontend/debugger/src/components/Schematic/nodes/EffectNode.tsx` & `relationalai-0.2.9/frontend/debugger/src/components/Schematic/nodes/EffectNode.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/frontend/debugger/src/components/Schematic/nodes/GetNode.tsx` & `relationalai-0.2.9/frontend/debugger/src/components/Schematic/nodes/GetNode.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/frontend/debugger/src/components/Schematic/nodes/QuantifyNode.tsx` & `relationalai-0.2.9/frontend/debugger/src/components/Schematic/nodes/QuantifyNode.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/frontend/debugger/src/components/Schematic/nodes/ReturnNode.tsx` & `relationalai-0.2.9/frontend/debugger/src/components/Schematic/nodes/ReturnNode.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/frontend/debugger/src/components/Schematic/nodes/SequenceNode.tsx` & `relationalai-0.2.9/frontend/debugger/src/components/Schematic/nodes/SequenceNode.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/frontend/debugger/src/components/Schematic/nodes/UnionNode.tsx` & `relationalai-0.2.9/frontend/debugger/src/components/Schematic/nodes/UnionNode.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/frontend/debugger/src/components/Schematic/nodes/base.styl` & `relationalai-0.2.9/frontend/debugger/src/components/Schematic/nodes/base.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/frontend/debugger/src/components/Schematic/nodes/base.tsx` & `relationalai-0.2.9/frontend/debugger/src/components/Schematic/nodes/base.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/frontend/debugger/src/components/Schematic/nodes/index.tsx` & `relationalai-0.2.9/frontend/debugger/src/components/Schematic/nodes/index.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/frontend/debugger/src/components/ui/Accordion.stories.tsx` & `relationalai-0.2.9/frontend/debugger/src/components/ui/Accordion.stories.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/frontend/debugger/src/components/ui/Accordion.tsx` & `relationalai-0.2.9/frontend/debugger/src/components/ui/Accordion.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/frontend/debugger/src/components/ui/Breadcrumbs.stories.tsx` & `relationalai-0.2.9/frontend/debugger/src/components/ui/Breadcrumbs.stories.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/frontend/debugger/src/components/ui/Breadcrumbs.tsx` & `relationalai-0.2.9/frontend/debugger/src/components/ui/Breadcrumbs.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/frontend/debugger/src/components/ui/Button.tsx` & `relationalai-0.2.9/frontend/debugger/src/components/ui/Button.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/frontend/debugger/src/components/ui/Code.styl` & `relationalai-0.2.9/frontend/debugger/src/components/ui/Code.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/frontend/debugger/src/components/ui/Code.tsx` & `relationalai-0.2.9/frontend/debugger/src/components/ui/Code.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/frontend/debugger/src/components/ui/Collapsible.stories.tsx` & `relationalai-0.2.9/frontend/debugger/src/components/ui/Collapsible.stories.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/frontend/debugger/src/components/ui/Collapsible.styl` & `relationalai-0.2.9/frontend/debugger/src/components/ui/Collapsible.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/frontend/debugger/src/components/ui/Collapsible.tsx` & `relationalai-0.2.9/frontend/debugger/src/components/ui/Collapsible.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/frontend/debugger/src/components/ui/Field.stories.tsx` & `relationalai-0.2.9/frontend/debugger/src/components/ui/Field.stories.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/frontend/debugger/src/components/ui/Field.styl` & `relationalai-0.2.9/frontend/debugger/src/components/ui/Field.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/frontend/debugger/src/components/ui/Field.tsx` & `relationalai-0.2.9/frontend/debugger/src/components/ui/Field.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/frontend/debugger/src/components/ui/Icon.tsx` & `relationalai-0.2.9/frontend/debugger/src/components/ui/Icon.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/frontend/debugger/src/components/ui/Modal.stories.tsx` & `relationalai-0.2.9/frontend/debugger/src/components/ui/Modal.stories.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/frontend/debugger/src/components/ui/Modal.styl` & `relationalai-0.2.9/frontend/debugger/src/components/ui/Modal.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/frontend/debugger/src/components/ui/Modal.tsx` & `relationalai-0.2.9/frontend/debugger/src/components/ui/Modal.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/frontend/debugger/src/components/ui/Tooltip.stories.tsx` & `relationalai-0.2.9/frontend/debugger/src/components/ui/Tooltip.stories.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/frontend/debugger/src/components/ui/Tooltip.styl` & `relationalai-0.2.9/frontend/debugger/src/components/ui/Tooltip.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/frontend/debugger/src/components/ui/Tooltip.tsx` & `relationalai-0.2.9/frontend/debugger/src/components/ui/Tooltip.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/frontend/debugger/src/fixtures/branch-improved.json` & `relationalai-0.2.9/frontend/debugger/src/fixtures/branch-improved.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/frontend/debugger/src/fixtures/branch.json` & `relationalai-0.2.9/frontend/debugger/src/fixtures/branch.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/frontend/debugger/src/fixtures/fraud.json` & `relationalai-0.2.9/frontend/debugger/src/fixtures/fraud.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/frontend/debugger/src/fixtures/not_found.json` & `relationalai-0.2.9/frontend/debugger/src/fixtures/not_found.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/frontend/debugger/src/fixtures/simple.json` & `relationalai-0.2.9/frontend/debugger/src/fixtures/simple.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/frontend/debugger/src/fixtures/union.json` & `relationalai-0.2.9/frontend/debugger/src/fixtures/union.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/frontend/debugger/src/types/mech.d.ts` & `relationalai-0.2.9/frontend/debugger/src/types/mech.d.ts`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/frontend/debugger/src/utils/fileUtils.ts` & `relationalai-0.2.9/frontend/debugger/src/utils/fileUtils.ts`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/src/gentest/README.md` & `relationalai-0.2.9/src/gentest/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/src/gentest/emit.py` & `relationalai-0.2.9/src/gentest/emit.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/src/gentest/exec.py` & `relationalai-0.2.9/src/gentest/exec.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/src/gentest/fixtures.py` & `relationalai-0.2.9/src/gentest/fixtures.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/src/gentest/patch.py` & `relationalai-0.2.9/src/gentest/patch.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/src/gentest/util.py` & `relationalai-0.2.9/src/gentest/util.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/src/gentest/cli/__main__.py` & `relationalai-0.2.9/src/gentest/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/src/gentest/cli/collect_failures.py` & `relationalai-0.2.9/src/gentest/cli/collect_failures.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/src/gentest/cli/collect_tests.py` & `relationalai-0.2.9/src/gentest/cli/collect_tests.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/src/gentest/cli/repro.py` & `relationalai-0.2.9/src/gentest/cli/repro.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/src/gentest/cli/watch.py` & `relationalai-0.2.9/src/gentest/cli/watch.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/src/gentest/gen/action.py` & `relationalai-0.2.9/src/gentest/gen/action.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/src/gentest/gen/context.py` & `relationalai-0.2.9/src/gentest/gen/context.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/src/gentest/gen/document.py` & `relationalai-0.2.9/src/gentest/gen/document.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/src/gentest/gen/group_limited.py` & `relationalai-0.2.9/src/gentest/gen/group_limited.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/src/gentest/gen/ir.py` & `relationalai-0.2.9/src/gentest/gen/ir.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/src/gentest/gen/scope.py` & `relationalai-0.2.9/src/gentest/gen/scope.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/src/gentest/gen/task.py` & `relationalai-0.2.9/src/gentest/gen/task.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/src/gentest/gen/test.py` & `relationalai-0.2.9/src/gentest/gen/test.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/src/gentest/harness/database.py` & `relationalai-0.2.9/src/gentest/harness/database.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/src/gentest/validate/diff.py` & `relationalai-0.2.9/src/gentest/validate/diff.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/src/gentest/validate/errors.py` & `relationalai-0.2.9/src/gentest/validate/errors.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/src/gentest/validate/mapping.py` & `relationalai-0.2.9/src/gentest/validate/mapping.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/src/gentest/validate/roundtrip.py` & `relationalai-0.2.9/src/gentest/validate/roundtrip.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/src/relationalai/__init__.py` & `relationalai-0.2.9/src/relationalai/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 from . import rel
 from .loaders import csv
 from . import analysis
 from . import tools
 import importlib.metadata
 from snowflake.connector import SnowflakeConnection
 
+# Set up global exception handler for debugging
+debugging.setup_exception_handler()
+
 __version__ = importlib.metadata.version(__package__ or __name__)
 
 def Model(
     name: str,
     *,
     profile: str | None = None,
     config: cfg.Config | None = None,
```

### Comparing `relationalai-0.2.8/src/relationalai/compiler.py` & `relationalai-0.2.9/src/relationalai/compiler.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/src/relationalai/debugging.py` & `relationalai-0.2.9/src/relationalai/debugging.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,48 @@
 import ast
 import contextlib
 from dataclasses import dataclass
 import datetime
 import inspect
 import json
+import sys
 from textwrap import dedent
 import os
 from typing import Dict
 import logging
 import uuid
 
 from pandas import DataFrame
 from .metamodel import Action, Task
 
 DEBUG = True
+handled_error = None
+
+
+#--------------------------------------------------
+# Global Error Handling
+#--------------------------------------------------
+
+def global_exception_handler(exc_type, exc_value, exc_traceback):
+    global handled_error
+    if exc_value is not handled_error:
+        # Ensure exc_value is actually an exception instance
+        if isinstance(exc_value, BaseException):
+            error(exc_value)  # Handle the error if it's new or different
+        handled_error = None
+
+    if original_excepthook is not None:
+        original_excepthook(exc_type, exc_value, exc_traceback)
+
+original_excepthook = None
+
+def setup_exception_handler():
+    global original_excepthook
+    original_excepthook = sys.excepthook
+    sys.excepthook = global_exception_handler 
 
 #--------------------------------------------------
 # Log Formatters
 #--------------------------------------------------
 
 def my_encoder(obj):
     if isinstance(obj, DataFrame):
@@ -170,18 +195,21 @@
 def time(type:str, elapsed:float, results:DataFrame = DataFrame(), **kwargs):
     if DEBUG:
         event("time", type=type, elapsed=elapsed, results={
             "values": results,
             "count": len(results)
         }, **kwargs)
 
-def error(err: Exception, **kwargs):
-    event("error", err=err, **kwargs)
-    for handler in logger.handlers:
-        handler.flush()
+def error(err, **kwargs):
+    global handled_error
+    if err is not handled_error:
+        event("error", err=err, **kwargs)  # Emit the error event only if it's a new or different error
+        for handler in logger.handlers:
+            handler.flush()
+        handled_error = err 
 
 def handle_compilation(compilation):
     if not DEBUG:
         return
 
     (file, line, block) = compilation.get_source()
     source = {"file": file, "line": line, "block": block}
```

### Comparing `relationalai-0.2.8/src/relationalai/dsl.py` & `relationalai-0.2.9/src/relationalai/dsl.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/src/relationalai/errors.py` & `relationalai-0.2.9/src/relationalai/errors.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/src/relationalai/metagen.py` & `relationalai-0.2.9/src/relationalai/metagen.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/src/relationalai/metamodel.py` & `relationalai-0.2.9/src/relationalai/metamodel.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/src/relationalai/rel.py` & `relationalai-0.2.9/src/relationalai/rel.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/src/relationalai/rel2.py` & `relationalai-0.2.9/src/relationalai/rel2.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/src/relationalai/rel_emitter.py` & `relationalai-0.2.9/src/relationalai/rel_emitter.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/src/relationalai/rel_utils.py` & `relationalai-0.2.9/src/relationalai/rel_utils.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/src/relationalai/analysis/mechanistic.py` & `relationalai-0.2.9/src/relationalai/analysis/mechanistic.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/src/relationalai/analysis/whynot.py` & `relationalai-0.2.9/src/relationalai/analysis/whynot.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/src/relationalai/clients/azure.py` & `relationalai-0.2.9/src/relationalai/clients/azure.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/src/relationalai/clients/client.py` & `relationalai-0.2.9/src/relationalai/clients/client.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/src/relationalai/clients/config.py` & `relationalai-0.2.9/src/relationalai/clients/config.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/src/relationalai/clients/snowflake.py` & `relationalai-0.2.9/src/relationalai/clients/snowflake.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/src/relationalai/clients/test.py` & `relationalai-0.2.9/src/relationalai/clients/test.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/src/relationalai/clients/types.py` & `relationalai-0.2.9/src/relationalai/clients/types.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/src/relationalai/loaders/csv.py` & `relationalai-0.2.9/src/relationalai/loaders/csv.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/src/relationalai/loaders/loader.py` & `relationalai-0.2.9/src/relationalai/loaders/loader.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/src/relationalai/loaders/types.py` & `relationalai-0.2.9/src/relationalai/loaders/types.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/src/relationalai/std/aggregates.py` & `relationalai-0.2.9/src/relationalai/std/aggregates.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/src/relationalai/std/graphs.py` & `relationalai-0.2.9/src/relationalai/std/graphs.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from collections import defaultdict
 from copy import deepcopy
+from numbers import Number
 import textwrap
 from typing import Any
 from .. import dsl, errors
 import gravis as gv
 from . import rel, Vars
 
 #--------------------------------------------------
@@ -15,37 +16,42 @@
     marked = errors.mark_source(source, source.line, source.line) if source else ""
     content = f"""
     The [yellow]{param}[/yellow] parameter {message}
 
     {marked}
     """
     errors.print_source_error(source, "Invalid algorithm parameter", content)
-    exit(1)
+    raise ValueError(message)
 
 #--------------------------------------------------
 # Validation
 #--------------------------------------------------
 
-def between(param:str, value, min, max):
-    if value < min or value > max:
-        invalid_param(param, f"must be between {min} and {max}")
-
-def positive(param:str, value):
-    if value <= 0:
-        invalid_param(param, "must be positive")
+def between(param:str,value, min, max,  type_=Number):
+    if (not isinstance(value, type_)) or (value < min or value > max):
+        invalid_param(param, f"must be a {type_.__name__.lower()} between {min} and {max}, got {value!r}")
+
+def positive(param:str, value, type_=Number):
+    if (not isinstance(value, type_)) or (value <= 0):
+        invalid_param(param, f"must be a positive {type_.__name__.lower()}, got {value!r}")
+
+def nonnegative(param:str, value, type_=Number):
+    if (not isinstance(value, type_)) or (value < 0):
+        invalid_param(param, f"must be a non-negative {type_.__name__.lower()}, got {value!r}")
 
 #--------------------------------------------------
 # Helpers
 #--------------------------------------------------
 
 def unwrap(v):
     if v is None:
         return None
     return rel.pyrel_default(rel.pyrel_unwrap, v, v)
 
+
 #--------------------------------------------------
 # Algos
 #--------------------------------------------------
 
 class Compute:
     def __init__(self, graph:'Graph'):
         self._graph = graph
@@ -251,20 +257,20 @@
     # --------------------------------------------------
     # Centrality
     # --------------------------------------------------
 
     def pagerank(self, node, damping_factor=0.85, tolerance=1e-6, max_iter=20):
         between("damping_factor", damping_factor, 0, 1)
         positive("tolerance", tolerance)
-        positive("max_iter", max_iter)
+        positive("max_iter", max_iter, type_=int)
 
         config = self._config(
             graph=self._graph,
-            damping_factor=damping_factor,
-            tolerance=tolerance,
+            damping_factor=float(damping_factor),
+            tolerance=float(tolerance),
             max_iter=max_iter,
         )
         return self._lib.pagerank(config, unwrap(node))
 
     def betweenness_centrality(self, node):
         return self._lib.betweenness_centrality(self._graph, unwrap(node))
 
@@ -286,24 +292,84 @@
     def weakly_connected_component(self, node):
         component = self._lib.weakly_connected_component(self._graph, unwrap(node))
         return self._lookup(component)
 
     def triangle_community(self, node):
         return self._lib.triangle_community(self._graph, unwrap(node))
 
-    def infomap(self, node):
-        config = self._config(graph=self._graph)
+    def infomap(
+            self,
+            node,
+            max_levels: int = 4,
+            max_sweeps: int = 8,
+            level_tolerance: float = 0.01,
+            sweep_tolerance: float = 0.0001,
+            teleportation_rate: float = 0.15,
+            visit_rate_tolerance: float = 1e-15,
+            randomization_seed: int | None = None,
+    ):
+        positive("max_levels", max_levels, type_=int)
+        positive("max_sweeps", max_sweeps, type_=int)
+        nonnegative("level_tolerance", level_tolerance)
+        nonnegative("sweep_tolerance", sweep_tolerance)
+        positive("teleportation_rate", teleportation_rate)
+        between("teleportation_rate", teleportation_rate, 0, 1)
+        positive("visit_rate_tolerance", visit_rate_tolerance)
+        _config_dict = {
+            "graph": self._graph,
+            "max_levels": max_levels,
+            "max_sweeps": max_sweeps,
+            "level_tolerance": float(level_tolerance),
+            "sweep_tolerance": float(sweep_tolerance),
+            "teleportation_rate": float(teleportation_rate),
+            "visit_rate_tolerance": float(visit_rate_tolerance),
+        }
+        if randomization_seed is not None:
+            positive("randomization_seed", randomization_seed, type_=int)
+            _config_dict["randomization_seed"] = randomization_seed
+
+        config = self._config(**_config_dict)
         return self._lib.infomap(config, unwrap(node))
 
-    def louvain(self, node):
-        config = self._config(graph=self._graph)
+    def louvain(
+            self,
+            node,
+            max_levels: int = 4,
+            max_sweeps: int = 8,
+            level_tolerance: float = 0.01,
+            sweep_tolerance: float = 0.0001,
+            randomization_seed: int | None = None,
+    ):
+        positive("max_levels", max_levels, type_=int)
+        positive("max_sweeps", max_sweeps, type_=int)
+        nonnegative("level_tolerance", level_tolerance)
+        nonnegative("sweep_tolerance", sweep_tolerance)
+        _config_dict = {
+            "graph": self._graph,
+            "max_levels": max_levels,
+            "max_sweeps": max_sweeps,
+            "level_tolerance": float(level_tolerance),
+            "sweep_tolerance": float(sweep_tolerance),
+        }
+        if randomization_seed is not None:
+            positive("randomization_seed", randomization_seed, type_=int)
+            _config_dict["randomization_seed"] = randomization_seed
+        config = self._config(**_config_dict)
         return self._lib.louvain(config, unwrap(node))
 
-    def label_propagation(self, node):
-        config = self._config(graph=self._graph)
+    def label_propagation(self, node, max_sweeps: int = 1000, randomization_seed: int | None = None):
+        positive("max_sweeps", max_sweeps, type_=int)
+        _config_dict = {
+            "graph": self._graph,
+            "max_sweeps": max_sweeps,
+        }
+        if randomization_seed is not None:
+            positive("randomization_seed", randomization_seed, type_=int)
+            _config_dict["randomization_seed"] = randomization_seed
+        config = self._config(**_config_dict)
         return self._lib.label_propagation(config, unwrap(node))
 
 #--------------------------------------------------
 # Edge
 #--------------------------------------------------
 
 class EdgeInstance:
```

### Comparing `relationalai-0.2.8/src/relationalai/std/math.py` & `relationalai-0.2.9/src/relationalai/std/math.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/src/relationalai/std/strings.py` & `relationalai-0.2.9/src/relationalai/std/strings.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/src/relationalai/tools/cli.py` & `relationalai-0.2.9/src/relationalai/tools/cli.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/src/relationalai/tools/cli_controls.py` & `relationalai-0.2.9/src/relationalai/tools/cli_controls.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/src/relationalai/tools/debugger.py` & `relationalai-0.2.9/src/relationalai/tools/debugger.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/src/relationalai/tools/debugger_client.py` & `relationalai-0.2.9/src/relationalai/tools/debugger_client.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/src/relationalai/tools/debugger_server.py` & `relationalai-0.2.9/src/relationalai/tools/debugger_server.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/src/relationalai/tools/dev.py` & `relationalai-0.2.9/src/relationalai/tools/dev.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/src/relationalai/util/format.py` & `relationalai-0.2.9/src/relationalai/util/format.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/src/relationalai/util/snowflake_logger.py` & `relationalai-0.2.9/src/relationalai/util/snowflake_logger.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/src/relationalai/util/tracing_logger.py` & `relationalai-0.2.9/src/relationalai/util/tracing_logger.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/tests/conftest.py` & `relationalai-0.2.9/tests/conftest.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 from _pytest._io.wcwidth import wcswidth
 from _pytest.terminal import TerminalReporter
 from gentest.util import condense_traceback
 import pytest
+import pandas as pd
+pd.set_option('display.max_columns', None)
+pd.set_option('display.expand_frame_repr', False)
 
 @pytest.hookimpl(hookwrapper=True)
 def pytest_runtest_makereport(item, call):
     term: TerminalReporter = item.config.pluginmanager.getplugin("terminalreporter")
     write_status(term)
 
     yield
```

### Comparing `relationalai-0.2.8/tests/util.py` & `relationalai-0.2.9/tests/util.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/tests/benchmarks/conftest.py` & `relationalai-0.2.9/tests/end2end/conftest.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import pytest
 
 from relationalai.debugging import logger
 from relationalai.util.tracing_logger import TracingLogger
 from tests.util import engine_config_fixture, root_span_fixture, snowflake_logger_fixture
 
 
-@pytest.fixture(scope="function")
+@pytest.fixture(scope="session")
 def engine_config():
     yield from engine_config_fixture()
 
 # Create a root span that all tests will be a part of
 # add `snowflake_logger` as a parameter, to make sure it is initialized before the root span
 # and finishes afterwards
 @pytest.fixture(scope="session", autouse=True)
```

### Comparing `relationalai-0.2.8/tests/benchmarks/test_tastybytes.py` & `relationalai-0.2.9/tests/benchmarks/test_tastybytes.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,121 +4,119 @@
 from relationalai.clients import config as cfg
 from relationalai.std import aggregates, rel
 from relationalai.std.graphs import Graph
 
 from relationalai import debugging
 
 def test_tastybytes(engine_config: cfg.Config):
-    # TODO: move benchmark span to hook?
-    with debugging.span("benchmark", name="tastybytes"):
-        name = "LOYALTY_ORDERS_REGION_CALIFORNIA"
-        # provider = rai.Resources(config=engine_config)
-        # with debugging.span("clone"):
-        #     name = "LOYALTY_ORDERS_REGION_CALIFORNIA_" + str(random.randint(1000000000, 9999999999))
-        #     provider.clone_graph(name, "LOYALTY_ORDERS_REGION_CALIFORNIA")
-        #     atexit.register(lambda: provider.delete_graph(name))
-        
-        model = rai.Model(name, config=engine_config)
-        model._config.set("compiler.use_multi_valued", True)
-        sf = Snowflake(model)
-        Record = sf.TASTYBYTES.HARMONIZED.LOYALTY_ORDERS_REGION_CALIFORNIA
-
-        Customer = model.Type("Customer")
-        Truck = model.Type("Trucks")
-        Transaction = model.Type("Transaction")
-        RelevantConnection = model.Type("RelevantConnection")
-        
-        with model.query(tag="count_all") as select:
-            record = Record()
-            num_records = aggregates.count(record)
-            select(num_records)
-
-        # Define Customer Type
-        with model.rule(dynamic=True):
-            r = Record()
-            Customer.add(customer_id=r.customer_id)
-
-        # Check total number of customers
-        with model.query(tag="count_customers") as select:
-            record = Customer()
-            num_records = aggregates.count(record)
-            select(num_records)
-
-        # Define Truck Type
-        with model.rule():
-            r = Record()
-            Truck.add(truck_id=r.truck_id)
-
-        # Check total number of trucks
-        with model.query(tag="count_trucks") as select:
-            record = Truck()
-            num_records = aggregates.count(record)
-            select(num_records)
-
-        with model.rule():
-            r = Record()
-            Transaction.add(
-                customer_id=r.customer_id,
-                order_id=r.order_id,
-                truck_id=r.truck_id,
-                order_ts=r.order_ts,
-                order_ts_seconds=r.order_ts_seconds,
-                location_id=r.location_id,
-            )
-
-        with model.rule():
-            t1 = Transaction()
-            t2 = Transaction()
-
-            t1.truck_id == t2.truck_id
-            t1.customer_id != t2.customer_id
-            rel.abs(t1.order_ts_seconds - t2.order_ts_seconds) <= 1200
-
-            t1.connected.add(t2)
-
-        with model.query(tag="count_connected_customers") as select:
-            t = Transaction()
-            num_records = aggregates.count(t.customer_id, t.order_ts, t.connected, t.connected.customer_id)
-            select(num_records)
-
-        with model.rule():
-            t = Transaction()
-            total_connections = aggregates.count(
-                t, per=[t.customer_id, t.connected.customer_id]
-            )
-            total_connections > 4
-            RelevantConnection.add(
-                customer_1=Customer(customer_id=t.customer_id),
-                customer_2=Customer(customer_id=t.connected.customer_id),
-                total_connections=total_connections,
-            )        
-
-        # Get the total occurrences where pairs of customers coexisted together more than once
-        with model.query(tag="count_meaningful_connected_customers") as select:
-            record = RelevantConnection()
-            num_records = aggregates.count(record)
-            select(num_records)
-
-        community_graph = Graph(model, undirected=True)
-
-        # Add edges to the graph between customers / Nodes will be added automatically
-        with model.rule():
-            connection = RelevantConnection()
-            community_graph.Edge.add(
-                connection.customer_1,
-                connection.customer_2,
-                weight=connection.total_connections,
-            )
-
-        with model.rule():
-            customer = Customer()
-            community_id = community_graph.compute.louvain(customer)
-            customer.set(community_id=community_id)
-
-            community_graph.Node.add(
-                customer,
-                community_id=community_id,
-                customer_id=customer.customer_id
-            )
+    name = "LOYALTY_ORDERS_REGION_CALIFORNIA"
+    # provider = rai.Resources(config=engine_config)
+    # with debugging.span("clone"):
+    #     name = "LOYALTY_ORDERS_REGION_CALIFORNIA_" + str(random.randint(1000000000, 9999999999))
+    #     provider.clone_graph(name, "LOYALTY_ORDERS_REGION_CALIFORNIA")
+    #     atexit.register(lambda: provider.delete_graph(name))
+    
+    model = rai.Model(name, config=engine_config)
+    model._config.set("compiler.use_multi_valued", True)
+    sf = Snowflake(model)
+    Record = sf.TASTYBYTES.HARMONIZED.LOYALTY_ORDERS_REGION_CALIFORNIA
+
+    Customer = model.Type("Customer")
+    Truck = model.Type("Trucks")
+    Transaction = model.Type("Transaction")
+    RelevantConnection = model.Type("RelevantConnection")
+    
+    with model.query(tag="count_all") as select:
+        record = Record()
+        num_records = aggregates.count(record)
+        select(num_records)
+
+    # Define Customer Type
+    with model.rule(dynamic=True):
+        r = Record()
+        Customer.add(customer_id=r.customer_id)
+
+    # Check total number of customers
+    with model.query(tag="count_customers") as select:
+        record = Customer()
+        num_records = aggregates.count(record)
+        select(num_records)
+
+    # Define Truck Type
+    with model.rule():
+        r = Record()
+        Truck.add(truck_id=r.truck_id)
+
+    # Check total number of trucks
+    with model.query(tag="count_trucks") as select:
+        record = Truck()
+        num_records = aggregates.count(record)
+        select(num_records)
+
+    with model.rule():
+        r = Record()
+        Transaction.add(
+            customer_id=r.customer_id,
+            order_id=r.order_id,
+            truck_id=r.truck_id,
+            order_ts=r.order_ts,
+            order_ts_seconds=r.order_ts_seconds,
+            location_id=r.location_id,
+        )
+
+    with model.rule():
+        t1 = Transaction()
+        t2 = Transaction()
+
+        t1.truck_id == t2.truck_id
+        t1.customer_id != t2.customer_id
+        rel.abs(t1.order_ts_seconds - t2.order_ts_seconds) <= 1200
+
+        t1.connected.add(t2)
+
+    with model.query(tag="count_connected_customers") as select:
+        t = Transaction()
+        num_records = aggregates.count(t.customer_id, t.order_ts, t.connected, t.connected.customer_id)
+        select(num_records)
+
+    with model.rule():
+        t = Transaction()
+        total_connections = aggregates.count(
+            t, per=[t.customer_id, t.connected.customer_id]
+        )
+        total_connections > 4
+        RelevantConnection.add(
+            customer_1=Customer(customer_id=t.customer_id),
+            customer_2=Customer(customer_id=t.connected.customer_id),
+            total_connections=total_connections,
+        )        
+
+    # Get the total occurrences where pairs of customers coexisted together more than once
+    with model.query(tag="count_meaningful_connected_customers") as select:
+        record = RelevantConnection()
+        num_records = aggregates.count(record)
+        select(num_records)
+
+    community_graph = Graph(model, undirected=True)
+
+    # Add edges to the graph between customers / Nodes will be added automatically
+    with model.rule():
+        connection = RelevantConnection()
+        community_graph.Edge.add(
+            connection.customer_1,
+            connection.customer_2,
+            weight=connection.total_connections,
+        )
+
+    with model.rule():
+        customer = Customer()
+        community_id = community_graph.compute.louvain(customer)
+        customer.set(community_id=community_id)
+
+        community_graph.Node.add(
+            customer,
+            community_id=community_id,
+            customer_id=customer.customer_id
+        )
 
-        with debugging.span("fetch", graph="louvain"):
-            community_graph.fetch()
+    with debugging.span("fetch", graph="louvain"):
+        community_graph.fetch()
```

### Comparing `relationalai-0.2.8/tests/end2end/README.md` & `relationalai-0.2.9/tests/end2end/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/tests/end2end/test_graph_visualize.py` & `relationalai-0.2.9/tests/end2end/test_graph_visualize.py`

 * *Files 2% similar despite different names*

```diff
@@ -208,7 +208,10 @@
         ]
 )
 def test_visualize(engine_config, test_input):
     model_name = unique_model_name("testGraphVisualize")
     model = rai.Model(model_name, config=engine_config)
     graph = make_graph(model, test_input)
     assert graph.visualize(style=test_input["style"], **test_input["kwargs"]) is not None
+    # delete the DB
+    provider = rai.Resources(config=engine_config)
+    provider.delete_graph(model_name)
```

### Comparing `relationalai-0.2.8/tests/end2end/test_snapshots.py` & `relationalai-0.2.9/tests/end2end/test_snapshots.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query2.txt` & `relationalai-0.2.9/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query2.txt`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/tests/end2end/test_cases/after_errors.py` & `relationalai-0.2.9/tests/end2end/test_cases/after_errors.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/tests/end2end/test_cases/bool.py` & `relationalai-0.2.9/tests/end2end/test_cases/bool.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/tests/end2end/test_cases/bottom.py` & `relationalai-0.2.9/tests/end2end/test_cases/bottom.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/tests/end2end/test_cases/export.py` & `relationalai-0.2.9/tests/end2end/test_cases/export.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/tests/end2end/test_cases/multi_valued.py` & `relationalai-0.2.9/tests/end2end/test_cases/multi_valued.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/tests/end2end/test_cases/not_found.py` & `relationalai-0.2.9/tests/end2end/test_cases/not_found.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/tests/end2end/test_cases/numeric_outputs.py` & `relationalai-0.2.9/tests/end2end/test_cases/numeric_outputs.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/tests/end2end/test_cases/out_of_context.py` & `relationalai-0.2.9/tests/end2end/test_cases/out_of_context.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/tests/end2end/test_cases/persist.py` & `relationalai-0.2.9/tests/end2end/test_cases/persist.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/tests/end2end/test_cases/smoke.py` & `relationalai-0.2.9/tests/end2end/test_cases/smoke.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/tests/end2end/test_cases/std_math.py` & `relationalai-0.2.9/tests/end2end/test_cases/std_math.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/tests/end2end/test_cases/strings.py` & `relationalai-0.2.9/tests/end2end/test_cases/strings.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/tests/end2end/test_cases/top.py` & `relationalai-0.2.9/tests/end2end/test_cases/top.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/tests/end2end/test_cases/union.py` & `relationalai-0.2.9/tests/end2end/test_cases/union.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/tests/end2end/test_cases/weighted_graphs.py` & `relationalai-0.2.9/tests/end2end/test_cases/weighted_graphs.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/tests/end2end/test_cases/graphs/basics.py` & `relationalai-0.2.9/tests/end2end/test_cases/graphs/basics.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/tests/end2end/test_cases/graphs/centrality.py` & `relationalai-0.2.9/tests/end2end/test_cases/graphs/centrality.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/tests/end2end/test_cases/graphs/clustering.py` & `relationalai-0.2.9/tests/end2end/test_cases/graphs/clustering.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/tests/end2end/test_cases/graphs/connectivity.py` & `relationalai-0.2.9/tests/end2end/test_cases/graphs/connectivity.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/tests/end2end/test_cases/graphs/degree.py` & `relationalai-0.2.9/tests/end2end/test_cases/graphs/degree.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/tests/end2end/test_cases/graphs/distance.py` & `relationalai-0.2.9/tests/end2end/test_cases/graphs/distance.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/tests/end2end/test_cases/graphs/link_prediction.py` & `relationalai-0.2.9/tests/end2end/test_cases/graphs/link_prediction.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/tests/end2end/test_cases/graphs/mixed_value_types.py` & `relationalai-0.2.9/tests/end2end/test_cases/graphs/mixed_value_types.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/tests/end2end/test_cases/graphs/similarity.py` & `relationalai-0.2.9/tests/end2end/test_cases/graphs/similarity.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/tests/end2end/test_cases/graphs/triangles.py` & `relationalai-0.2.9/tests/end2end/test_cases/graphs/triangles.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/tests/init-cli/README.md` & `relationalai-0.2.9/tests/init-cli/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/tests/init-cli/azure_basic.py` & `relationalai-0.2.9/tests/init-cli/azure_basic.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/tests/init-cli/common.py` & `relationalai-0.2.9/tests/init-cli/common.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/tests/roundtrip/test_document.py` & `relationalai-0.2.9/tests/roundtrip/test_document.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/tests/roundtrip/test_task.py` & `relationalai-0.2.9/tests/roundtrip/test_task.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/tests/unit/test_config_store.py` & `relationalai-0.2.9/tests/unit/test_config_store.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/tests/unit/test_configs/config_with_new_profile.toml` & `relationalai-0.2.9/tests/unit/test_configs/config_with_new_profile.toml`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/tests/unit/test_configs/raiconfig_example.toml` & `relationalai-0.2.9/tests/unit/test_configs/raiconfig_example.toml`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.8/pyproject.toml` & `relationalai-0.2.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = 'relationalai'
-version = '0.2.8'
+version = '0.2.9'
 description = 'RelationalAI Library and CLI'
 readme="docs/pypi/README.md"
 authors = [
     { name="RelationalAI", email="support@relational.ai" },
 ]
 requires-python = ">= 3.10"
 dependencies = [
```

### Comparing `relationalai-0.2.8/PKG-INFO` & `relationalai-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: relationalai
-Version: 0.2.8
+Version: 0.2.9
 Summary: RelationalAI Library and CLI
 Author-email: RelationalAI <support@relational.ai>
 Requires-Python: >=3.10
 Requires-Dist: aiohttp
 Requires-Dist: bytecode
 Requires-Dist: click
 Requires-Dist: colorama
```

