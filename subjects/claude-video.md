# claude-video

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/bradautomates/claude-video, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/claude-video

## Pinned environment

- Project commit: `03ceb42f7fa2c4439aca01752118044baabffb8f`
- Test commit: `03ceb42f7fa2c4439aca01752118044baabffb8f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4.1 to 4.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1.2 | 4.1 | 1 | 1 | [run](https://argusic.com/run/140191d7-31d5-4b45-b75f-c3fadf98ea6a) |

## What was observed on a clean machine

Attempt 1:

- `unzip not in container; build-skill.sh fails at line 23 but dist/watch.skill is created correctly by git archive`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
