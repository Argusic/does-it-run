# AssetOpsBench

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/IBM/AssetOpsBench, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/assetopsbench

## Pinned environment

- Project commit: `81265cbbd36d7348ec0aeae4b398c86d332f2fc1`
- Test commit: `81265cbbd36d7348ec0aeae4b398c86d332f2fc1`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 23.2 to 24.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 20 | 24.9 | 5 | 5 | [run](https://argusic.com/run/f19258a8-7a7b-45a8-9465-fa3bae9539d1) |
| 2 | pass with mocks | 92 | 12 | 23.2 | 4 | 4 | [run](https://argusic.com/run/caec2604-1579-4f46-aa47-47a6080e5d36) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `evaluate_static_json() got unexpected keyword argument 'evaluation_metadata'`
- 2 min: `Vibration requires_couchdb didn't skip on unreachable CouchDB (empty-string env var)`
- 1 min: `FMSR requires_watsonx didn't skip on empty-string WATSONX_APIKEY`
- 2 min: `IoT test_invalid_site tests not guarded against missing CouchDB`
- 2 min: `Observability file_exporter tests missing google.protobuf and opentelemetry-exporter`

Attempt 2:

- 2 min: `mcp 2.x installed but project uses FastMCP (renamed in v2). Pinned to mcp<2.`
- 4 min: `couchdb3.Database.__bool__() raises httpx.ConnectError instead of returning False when CouchDB unreachable, crashing test_invalid_site tests`
- 1 min: `requires_couchdb marker only checked env var, not connectivity`
- 1 min: `Missing pytest, opentelemetry-sdk, opentelemetry-exporter-otlp-proto-http, protobuf`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
