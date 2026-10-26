# ai-prd-workflow

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/nurettincoban/ai-prd-workflow, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/ai-prd-workflow

## Pinned environment

- Project commit: `2bc8b2981b34b94bec4cee860252dc8c78e4ab10`
- Test commit: `2bc8b2981b34b94bec4cee860252dc8c78e4ab10`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 2.2 to 2.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 2.2 | 1 | 1 | [run](https://argusic.com/run/6ea9662a-54be-4c30-bb08-bee784ed61ce) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `First test-install.sh run failed on glob skills/*/SKILL.md (frontmatter not found) , re-run passed all 8 groups; a transient shell-glob after --build`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
