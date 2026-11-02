# ai-website-cloner-template

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/JCodesMore/ai-website-cloner-template, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/ai-website-cloner-template

## Pinned environment

- Project commit: `92872bc40ced2c5edb4d5dc9fd3970d40c77f4ca`
- Test commit: `92872bc40ced2c5edb4d5dc9fd3970d40c77f4ca`
- Worker image digests: `sha256:33ceb71981b602c1a7443a53469e4dba065f7503eab3078a2d7a57a2ab987517`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 3.5 to 6.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.2 | 6.4 | 0 | 0 | [run](https://argusic.com/run/01a4ae13-cc7a-4bb4-b65b-e0f3e1762281) |
| 2 | pass | 100 | 2 | 3.5 | 1 | 1 | [run](https://argusic.com/run/d82a9c84-216b-4f6a-8786-f076cf40db10) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `Node.js v18.19.1 installed but project requires >=24`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
