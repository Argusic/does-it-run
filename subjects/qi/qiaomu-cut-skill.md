# qiaomu-cut-skill

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/joeseesun/qiaomu-cut-skill, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/qiaomu-cut-skill

## Pinned environment

- Project commit: `823feff5c1c15066b6641e3c803351ffd6f26076`
- Test commit: `823feff5c1c15066b6641e3c803351ffd6f26076`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 2.4 to 2.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.1 | 2.4 | 1 | 1 | [run](https://argusic.com/run/9b4fee14-2153-4e98-a25f-f4de213a67d1) |

## What was observed on a clean machine

Attempt 1:

- 15 min: `scripts/render_project.js had "- /filter_complex" typo (leading slash) and passed file path to -filter_complex instead of -filter_complex_script on two lines, causing ffmpeg to reject the argument`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
