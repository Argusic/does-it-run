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
- Valid runs: 2; wall time 16.2 to 28.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 15 | 16.2 | 4 | 4 | [run](https://argusic.com/run/100f7ef5-a6fc-4066-a232-c1f376870ad0) |
| 2 | pass | 100 | 27 | 28.4 | 6 | 6 | [run](https://argusic.com/run/0bb4670f-2ceb-492e-ab46-d8ce71e682e8) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Missing protoc (protobuf compiler) for etcd-client build dependency`
- 2 min: `No admin web assets in dist/ caused AdminAsset::get('index.html') to return None, failing test_embedded_static_file`
- 3 min: `Expired test certificate caused test_cert assertion failure (not_after 2026-10-06 < current date 2026-10-08)`
- 1 min: `test_etcd_config_manger requires running etcd at 127.0.0.1:2379, which is not available`

Attempt 2:

- 1 min: `Rust toolchain not installed`
- 1 min: `protoc not found, etcd-client build fails`
- 2 min: `Node 18 too old for Vite 8, web admin build fails`
- 2 min: `test_cert in pingap-certificate uses hardcoded expired certificate`
- 3 min: `etc not running, test_etcd_config_manger fails`
- 2 min: `etc background process dies when shell exits`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
