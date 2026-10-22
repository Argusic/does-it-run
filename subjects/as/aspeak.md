# aspeak

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/kxxt/aspeak, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/aspeak

## Pinned environment

- Project commit: `98cd49d9b44cb3db1616da0b57a833177510bc59`
- Test commit: `98cd49d9b44cb3db1616da0b57a833177510bc59`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 9.5 to 9.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 4.2 | 9.5 | 2 | 2 | [run](https://argusic.com/run/c9d9586c-1563-4dbc-a6e3-d63421975f83) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `alsa-sys build fails: libasound2-dev not installed (no root)`
- 0.2 min: `Linker cannot find libasound.so symlink`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
