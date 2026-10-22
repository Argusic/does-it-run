# devopness

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/devopness/devopness, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/devopness

## Pinned environment

- Project commit: `aec616919c31f7a78ef08b6829b8ac4ddc0e371b`
- Test commit: `aec616919c31f7a78ef08b6829b8ac4ddc0e371b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4.3 to 4.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 11 | 4.3 | 3 | 3 | [run](https://argusic.com/run/b716b6ce-e7c6-44e7-8213-b40002ee0d42) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Node.js v18.19.1 is too old (SDK requires ^20.19.0 || ^22.13.0 || >=24)`
- 3 min: `Python pip install blocked by PEP 668 OS package protection`
- `Java not found, cannot run openapi-generator-cli for JS SDK build`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
