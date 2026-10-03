# oh-story-claudecode

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/zenstory-ai/oh-story-claudecode, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/oh-story-claudecode

## Pinned environment

- Project commit: `4a50d5583590eb7f207037e35136c1168bc02201`
- Test commit: `4a50d5583590eb7f207037e35136c1168bc02201`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 15.9 to 15.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 15.9 | 1 | 1 | [run](https://argusic.com/run/2c65353b-2e34-4bcd-912d-3ebd4380e319) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `test-prose-net-parity.sh failed because the "node absent" test scenario still had node in PATH (/usr/bin), so node was never truly unavailable; only "/usr/bin:/bin" were in PATH`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
