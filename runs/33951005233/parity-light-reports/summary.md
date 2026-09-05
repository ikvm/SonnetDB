# SonnetDB Parity Summary

| Field | Value |
|---|---|
| Profile | light |
| Status | failing |
| Pass rate | 100% |
| Scenarios | 23 passed / 27 skipped / 0 failed / 50 total |
| Warning-only performance scenarios | 2 |
| Commit | 775b187273a610a47e25cbd584f1eeecc19e2292 |
| GitHub run | 33951005233 |

## Suites

| Suite | Passed | Skipped | Failed | Total |
|---|---:|---:|---:|---:|
| analytics-51178646 | 0 | 5 | 0 | 5 |
| document-329e8646 | 0 | 5 | 0 | 5 |
| fulltext-ffd355ba | 0 | 6 | 0 | 6 |
| kv-1e8c05d4 | 5 | 0 | 0 | 5 |
| mq-7e4a4660 | 5 | 0 | 0 | 5 |
| object-ef76c04c | 5 | 0 | 0 | 5 |
| relational-5b7ed543 | 8 | 1 | 0 | 9 |
| tsdb-f57a2744 | 0 | 7 | 0 | 7 |
| vector-628d1ca4 | 0 | 3 | 0 | 3 |

## Gate Failures

| Gate | Suite | Scenario | Gap reason | Reason |
|---|---|---|---|---|
| capability | dotnet-test | parity | parity_test_failed | dotnet test exited with code 1 |

## Performance Warnings

| Suite | Scenario | Note |
|---|---|---|
| analytics-51178646 | groupby_time_1b_rows_wallclock | performance metrics are warning only |
| analytics-51178646 | columnar_compression_ratio | performance metrics are warning only |
