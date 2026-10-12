# gooey-pi

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/am-will/gooey-pi, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/gooey-pi

## Pinned environment

- Project commit: `459c9965690468c69d7434f82acf4b5eeee8e4bf`
- Test commit: `459c9965690468c69d7434f82acf4b5eeee8e4bf`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 3.3 to 3.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 4 | 3.3 | 1 | 1 | [run](https://argusic.com/run/9b25b138-7c4b-4b68-b5ff-af0a01fbad1b) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Electron SUID sandbox helper not configured correctly (chrome-sandbox not owned by root with mode 4755), causing FATAL abort on launch`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
