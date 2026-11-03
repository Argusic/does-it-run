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
- Valid runs: 2; wall time 4.1 to 4.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1.2 | 4.1 | 1 | 1 | [run](https://argusic.com/run/140191d7-31d5-4b45-b75f-c3fadf98ea6a) |
| 2 | pass | 100 | 5 | 4.3 | 2 | 2 | [run](https://argusic.com/run/21fa7963-54c8-467f-8ff2-030e3f187382) |

## What was observed on a clean machine

Attempt 1:

- `unzip not in container; build-skill.sh fails at line 23 but dist/watch.skill is created correctly by git archive`

Attempt 2:

- 2 min: `System Node v18.19.1 could not load skills@1.7.5, which requires Node >=22.20.0 (SyntaxError: node:util lacks styleText).`
- 8 min: `build-skill.sh exited 127 because unzip was absent, despite having written a valid bundle.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
