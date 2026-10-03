# gitui

**Verdict: runs.** Argusic Score 97.8 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/gitui-org/gitui, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/gitui

## Pinned environment

- Project commit: `2fa693cb6ed431b21ebc300dd02e83c2476699ce`
- Test commit: `2fa693cb6ed431b21ebc300dd02e83c2476699ce`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 7.8 to 32.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 31 | 32.8 | 3 | 3 | [run](https://argusic.com/run/134a99b9-1959-4d2b-a5de-0d5601e7c47a) |
| 2 | pass | 93.33 | 10 | 10.8 | 3 | 2 | [run](https://argusic.com/run/8da94a59-004e-4d40-9afd-d25cba4dda22) |
| 3 | pass | 100 | 2.5 | 7.8 | 3 | 3 | [run](https://argusic.com/run/5e240865-6b3a-4b5b-8c84-4be6421d31b2) |

## What was observed on a clean machine

Attempt 1:

- 15 min: `No C compiler (gcc) or build tools in container`
- 10 min: `Vendored openssl build failed (missing system headers, make)`
- `3 tests fail due to missing ssh-keygen and gpgsm tools for signing tests`

Attempt 2:

- 2 min: `Rust toolchain not installed`
- 1 min: `python not found (python3 only) - git2-hooks test_pre_commit_py failed`
- `3 e2e signing tests fail: need gpg, ssh-keygen, gpgsm (no root)`

Attempt 3:

- 0.5 min: `Rust toolchain not installed`
- 0.1 min: `python not found in PATH (hooks test pre_commit_py fails)`
- `gpg, ssh-keygen, gpgsm not available (3 signing e2e tests skippable, not core)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
