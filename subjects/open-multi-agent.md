# open-multi-agent

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/open-multi-agent/open-multi-agent, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/open-multi-agent

## Pinned environment

- Project commit: `dcffce18c8ada9127c954b81131345d26ad5aea7`
- Test commit: `dcffce18c8ada9127c954b81131345d26ad5aea7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 3; wall time 4.1 to 6.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 3.6 | 6.3 | 0 | 0 | [run](https://argusic.com/run/1f46b5ff-4e09-49c3-85b1-4a7e65c0567b) |
| 2 | pass with mocks | 92 | 1 | 4.7 | 0 | 0 | [run](https://argusic.com/run/a208d491-574a-4d7b-9677-2dcec17da158) |
| 3 | pass with mocks | 92 | 0.5 | 4.1 | 1 | 1 | [run](https://argusic.com/run/40ca108e-4179-419e-906e-63e7ae278fe4) |

## What was observed on a clean machine

Attempt 3:

- 0.2 min: `Node.js v18.19.1 is installed but the project requires >=20`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
