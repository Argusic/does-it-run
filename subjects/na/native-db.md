# native_db

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/vincent-herlemont/native_db, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/native-db

## Pinned environment

- Project commit: `b9554fdabbdd44997aa480c883e067ee3f823046`
- Test commit: `b9554fdabbdd44997aa480c883e067ee3f823046`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 3 to 5.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.15 | 5.2 | 0 | 0 | [run](https://argusic.com/run/1856d76b-3687-414b-8e0c-45308b65cf2e) |
| 2 | pass | 100 | 12 | 3 | 1 | 1 | [run](https://argusic.com/run/30537abb-b591-4082-bcb4-0add7280fd97) |

## What was observed on a clean machine

Attempt 2:

- 3 min: `Rust toolchain (rustc, cargo) not found in PATH`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
