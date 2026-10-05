# zeroshot

**Verdict: runs.** Argusic Score 95 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/the-open-engine/zeroshot, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/zeroshot

## Pinned environment

- Project commit: `63d4832da7f2a9ec7d61c3b0cb123b1e88bfb18a`
- Test commit: `63d4832da7f2a9ec7d61c3b0cb123b1e88bfb18a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 25.4 to 25.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 95 | 28 | 25.4 | 4 | 3 | [run](https://argusic.com/run/d9e085fc-ddbc-4d7b-929b-183f5a014237) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `npm global install failed EACCES on /usr/local prefix`
- 5 min: `rustc/cargo missing from container`
- 8 min: `cargo link died with Bus error / No space left on device (36G debug target on 40G root)`
- 10 min: `test fetch_waits_for_automatic_maintenance fails: git 2.43 runs maintenance without --no-detach; repo requires git >= 2.47 and fixture hardcodes /usr/bin/git`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
