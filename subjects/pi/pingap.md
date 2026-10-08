# pingap

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/vicanso/pingap, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/pingap

## Pinned environment

- Project commit: `71c4aa98aadecb36ca2d66bb60f58dd03be6d924`
- Test commit: `71c4aa98aadecb36ca2d66bb60f58dd03be6d924`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 16.2 to 16.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 15 | 16.2 | 4 | 4 | [run](https://argusic.com/run/100f7ef5-a6fc-4066-a232-c1f376870ad0) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Missing protoc (protobuf compiler) for etcd-client build dependency`
- 2 min: `No admin web assets in dist/ caused AdminAsset::get('index.html') to return None, failing test_embedded_static_file`
- 3 min: `Expired test certificate caused test_cert assertion failure (not_after 2026-10-06 < current date 2026-10-08)`
- 1 min: `test_etcd_config_manger requires running etcd at 127.0.0.1:2379, which is not available`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
