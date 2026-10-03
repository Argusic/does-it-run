# github-pages-deploy-action

**Verdict: runs with mocks.** Argusic Score 82 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/JamesIves/github-pages-deploy-action, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/github-pages-deploy-action

## Pinned environment

- Project commit: `8fd6702fce085de3b0afba6ffc90602776d25e80`
- Test commit: `8fd6702fce085de3b0afba6ffc90602776d25e80`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 5.2 to 5.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 82 | 3 | 5.2 | 2 | 1 | [run](https://argusic.com/run/d0c43d59-e3b4-416a-8ce6-781bcdc057d0) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Node.js v18.19.1 present but project requires v24.13.0`
- `rsync not found (no root to install package)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
