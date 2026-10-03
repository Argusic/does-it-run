# mirrord

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/metalbear-co/mirrord, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/mirrord

## Pinned environment

- Project commit: `6c5955a3cefcf02e565ef72821aeee7eb1857c03`
- Test commit: `6c5955a3cefcf02e565ef72821aeee7eb1857c03`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 3; wall time 30.2 to 42.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 42.1 | 0 | 0 | [run](https://argusic.com/run/14fb4027-c4a4-4199-a463-a33185d4cf62) |
| 1 | timeout | none | n/a | 42 | 0 | 0 | [run](https://argusic.com/run/4f1a05ae-c106-41c3-896a-49700de42deb) |
| 2 | pass | 100 | 25 | 30.2 | 6 | 6 | [run](https://argusic.com/run/a7b4a227-e2cb-422f-80d6-2c134c51aa65) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `Rust toolchain not installed`
- 1 min: `protoc compiler not found (needed by containerd-client build dependency)`
- 5 min: `libclang.so not found (needed by bindgen for frida-gum-sys)`
- 2 min: `bindgen failed: stddef.h not found (clang missing include paths)`
- 1 min: `MIRRORD_LAYER_FILE env var not defined at compile time`
- 3 min: `Out of disk space (40GB overlay, 24GB in target/) during workspace test run`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
