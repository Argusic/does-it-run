# HermesOffice

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/criptogus/HermesOffice, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/hermesoffice

## Pinned environment

- Project commit: `05c5512e75cf5a2b5ab631a922861fa6458b34f8`
- Test commit: `05c5512e75cf5a2b5ab631a922861fa6458b34f8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 18.1 to 27.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 26 | 27.1 | 3 | 3 | [run](https://argusic.com/run/4525886b-ea6d-4af2-bc77-5fab06229df7) |
| 2 | pass | 100 | 2 | 18.1 | 3 | 3 | [run](https://argusic.com/run/caf84206-2386-423c-b25e-4e952f1a6b1f) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Container had Node 18.19.1 but project requires >=22.12.0`
- 2 min: `cargo (Rust) not found, sheets native:xlsx-engine tests/build failed`
- `Electron SUID sandbox helper not configured correctly without root`

Attempt 2:

- 1 min: `Node v18 installed but project requires >=22.12.0; npm install emitted EBADENGINE warnings`
- 1 min: `Rust/cargo not found , sheets native:test and native:build would fail`
- `Electron chrome-sandbox not SUID (no root access)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
