# Spire

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/lsk569937453/Spire, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/spire

## Pinned environment

- Project commit: `d2abaccedcd88a42f891cfa698d2847da447781f`
- Test commit: `d2abaccedcd88a42f891cfa698d2847da447781f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 76.7 to 76.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 25 | 76.7 | 7 | 7 | [run](https://argusic.com/run/a55bc6e0-d6a5-4b8b-83b8-41f6556e8284) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `test_cors_middleware: async fn handle_response called without await`
- 1 min: `jsonwebtoken: CryptoProvider not installed`
- 1 min: `forward_ip_examples: kind:single not a valid serde variant`
- 1 min: `static_file.yaml: D:\ doc_root doesn't exist on Linux`
- 1 min: `HTTPS/TLS tests expected 'missing key' but got 'missing domains' error`
- 1 min: `compression test expected Some(Zstd) from Gzip-only default`
- 1 min: `proxy adapter test expected 500 but got 404`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
