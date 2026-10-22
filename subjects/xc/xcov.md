# xcov

**Verdict: could not verify.** Argusic Score 50 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/fastlane-community/xcov, licensed MIT, written in Ruby.

Evidence and recordings: https://argusic.com/subject/xcov

## Pinned environment

- Project commit: `206120df3aa2d616e83864dd00233564faef3eef`
- Test commit: `206120df3aa2d616e83864dd00233564faef3eef`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 1.2 to 12.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 12 | 12.1 | 4 | 4 | [run](https://argusic.com/run/db3a951f-1729-4a51-a381-ea0ef8b5ff55) |
| 2 | fail | 20 | n/a | 1.2 | 0 | 0 | [run](https://argusic.com/run/84b82268-4fa9-41cc-bc5f-afe7936d83be) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Ruby not installed in the container`
- 1 min: `psych (YAML) gem required libyaml which was missing`
- 1 min: `zlib Ruby extension failed to build (no -dev headers)`
- 2 min: `xcode-select -p backtick crashed at load time when Xcode absent`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
