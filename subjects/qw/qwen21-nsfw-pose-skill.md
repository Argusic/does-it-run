# qwen21-nsfw-pose-skill

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Arekejoker/qwen21-nsfw-pose-skill, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/qwen21-nsfw-pose-skill

## Pinned environment

- Project commit: `5fa2aa12ebbc106fbf32aa3e05c87f613303aa2c`
- Test commit: `5fa2aa12ebbc106fbf32aa3e05c87f613303aa2c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 7.6 to 31.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 7.6 | 0 | 0 | [run](https://argusic.com/run/25318b89-4f64-4ec6-ab62-57ee4f3fd1f0) |
| 2 | pass | 100 | 32 | 31.7 | 1 | 1 | [run](https://argusic.com/run/fd675658-3742-42a5-a07c-b3e7d2c741ff) |

## What was observed on a clean machine

Attempt 2:

- 3 min: `Default NSFW LoRA from Civitai (model 2986844) requires login with HTTP 401`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
