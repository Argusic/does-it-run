# Tangent

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/suchnsuch/Tangent, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/tangent

## Pinned environment

- Project commit: `a3173b0d18fd3e7efe6649e04d302546660e8e17`
- Test commit: `a3173b0d18fd3e7efe6649e04d302546660e8e17`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 7.5 to 7.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 23 | 7.5 | 3 | 3 | [run](https://argusic.com/run/80c40ff2-12ce-41b9-ada2-b0cfdb3381a4) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `Node.js 18 too old , 'node:util' lacks 'styleText', Vite 7+ requires >=20`
- 2 min: `e2e Playwright test fixture overrode env without DISPLAY, Electron couldn't find X server`
- `tangent-test-workspace-generator expects jest, not in dependencies`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
