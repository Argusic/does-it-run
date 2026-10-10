# repository-harness

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/hoangnb24/repository-harness, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/repository-harness

## Pinned environment

- Project commit: `e765792b635b4d5e3e5fc0578f82f9ca5dea2681`
- Test commit: `e765792b635b4d5e3e5fc0578f82f9ca5dea2681`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 46 to 46 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 4.5 | 46 | 2 | 2 | [run](https://argusic.com/run/e4d017cd-6d95-4ec3-8a38-9be3bac3b2d4) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `test-install-harness-modes.sh hangs - trap 'rm -rf $temp' EXIT blocked by sandbox`
- 1 min: `test-engineering-wisdom-opt-in.sh hangs - same rm -rf trap issue`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
