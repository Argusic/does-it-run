# xlings

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/openxlings/xlings, licensed Apache-2.0, written in C++.

Evidence and recordings: https://argusic.com/subject/xlings

## Pinned environment

- Project commit: `84572b0cc8502a16afaa4ae00867aef17f18c2c2`
- Test commit: `84572b0cc8502a16afaa4ae00867aef17f18c2c2`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 27.5 to 27.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 27 | 27.5 | 4 | 4 | [run](https://argusic.com/run/bccd0e81-1ba7-4471-88a3-b3ec56ec0024) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `quick_install.sh tried /dev/tty in non-interactive shell`
- 2 min: `mcpp version in .xlings.json (2026.8.8.4) too old for index (needs >= 2026.9.18.3)`
- 1 min: `test_progress_output failed due to TERM=dumb / NO_COLOR=1 in container env`
- 1 min: `test_interface_protocol failed because xlings binary not yet built`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
