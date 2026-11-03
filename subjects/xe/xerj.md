# xerj

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/xerj-org/xerj, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/xerj

## Pinned environment

- Project commit: `fa27e936272c335bd2ee4c596e9be485fc290419`
- Test commit: `fa27e936272c335bd2ee4c596e9be485fc290419`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 2.7 to 36.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 2.7 | 0 | 0 | [run](https://argusic.com/run/4744d71f-8dff-4299-8b95-2b34368017e6) |
| 2 | pass | 100 | 33 | 36.5 | 4 | 4 | [run](https://argusic.com/run/84606c9d-e9f0-4824-bd93-e7733852f1f9) |

## What was observed on a clean machine

Attempt 2:

- 3 min: `No Rust toolchain installed`
- 4 min: `Server died after shell session ended (SIGHUP from pipe)`
- 3 min: `autoindex on full engine folder failed: tcp connect error (os error 99)`
- `2 of 71 xerj-server tests failed: IPv6 loopback bind on ::1 (os error 99)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
