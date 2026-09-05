# SonnetDB Parity Summary

| Field | Value |
|---|---|
| Profile | full |
| Status | failing |
| Pass rate | 68% |
| Scenarios | 28 passed / 6 skipped / 16 failed / 50 total |
| Warning-only performance scenarios | 2 |
| Commit | 775b187273a610a47e25cbd584f1eeecc19e2292 |
| GitHub run | 33951005233 |

## Suites

| Suite | Passed | Skipped | Failed | Total |
|---|---:|---:|---:|---:|
| analytics-fafafb1b | 0 | 5 | 0 | 5 |
| document-3a452675 | 5 | 0 | 0 | 5 |
| fulltext-974f2dc4 | 0 | 0 | 6 | 6 |
| kv-0d79c64b | 5 | 0 | 0 | 5 |
| mq-87d41668 | 5 | 0 | 0 | 5 |
| object-f5713cab | 5 | 0 | 0 | 5 |
| relational-1b2d48b9 | 8 | 1 | 0 | 9 |
| tsdb-a8f1490e | 0 | 0 | 7 | 7 |
| vector-fa46233b | 0 | 0 | 3 | 3 |

## Gate Failures

| Gate | Suite | Scenario | Gap reason | Reason |
|---|---|---|---|---|
| accuracy | fulltext-974f2dc4 | index_1m_documents | scenario_failed | backend reported fail |
| accuracy | fulltext-974f2dc4 | bm25_ranking_top10_overlap | scenario_failed | backend reported fail |
| accuracy | fulltext-974f2dc4 | cjk_tokenize_correctness | scenario_failed | backend reported fail |
| accuracy | fulltext-974f2dc4 | facet_filter_query | scenario_failed | backend reported fail |
| accuracy | fulltext-974f2dc4 | incremental_update_during_query | scenario_failed | backend reported fail |
| accuracy | fulltext-974f2dc4 | typo_tolerant_query | scenario_failed | backend reported fail |
| capability | tsdb-a8f1490e | ingest_1m_points | scenario_failed | backend reported fail |
| accuracy | tsdb-a8f1490e | groupby_time_window | scenario_failed | victoriametrics: row count mismatch: expected 2, actual 0 |
| accuracy | tsdb-a8f1490e | derivative_accuracy | scenario_failed | influxdb: row count mismatch: expected 30, actual 29; victoriametrics: row count mismatch: expected 30, actual 0 |
| accuracy | tsdb-a8f1490e | rate_irate_consistency | scenario_failed | influxdb: row count mismatch: expected 30, actual 29; victoriametrics: row count mismatch: expected 30, actual 0 |
| accuracy | tsdb-a8f1490e | holt_winters_forecast_recall | scenario_failed | influxdb: row 0 column 0 (time) mismatch: expected '1704067280000', actual '0'; influxdb: row 1 column 0 (time) mismatch: expected '1704067281000', actual '1'; influxdb: row 2 column 0 (time) mismatch: expected '1704067282000', actual '2'; influxdb: row 3 column 0 (time) mismatch: expected '1704067283000', actual '3'; influxdb: row 4 column 0 (time) mismatch: expected '1704067284000', actual '4'; influxdb: row 5 column 0 (time) mismatch: expected '1704067285000', actual '5' |
| accuracy | tsdb-a8f1490e | percentile_p95_tdigest_vs_quantile | scenario_failed | victoriametrics: row 0 column 0 (percentile) mismatch: expected '94.06', actual '0' |
| accuracy | tsdb-a8f1490e | distinct_count_hll_2pct_error | scenario_failed | victoriametrics: row 0 column 0 (distinct_count(value)) mismatch: expected '503', actual '0' |
| capability | vector-fa46233b | ann_recall_at_10 | scenario_failed | backend reported fail |
| accuracy | vector-fa46233b | filtered_search | scenario_failed | backend reported fail |
| capability | vector-fa46233b | upsert_during_query | scenario_failed | backend reported fail |
| capability | dotnet-test | parity | parity_test_failed | dotnet test exited with code 1 |

## Performance Warnings

| Suite | Scenario | Note |
|---|---|---|
| analytics-fafafb1b | groupby_time_1b_rows_wallclock | performance metrics are warning only |
| analytics-fafafb1b | columnar_compression_ratio | performance metrics are warning only |
