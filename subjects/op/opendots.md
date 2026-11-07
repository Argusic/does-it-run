# OpenDots

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/CopilotKit/OpenDots, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/opendots

## Pinned environment

- Project commit: `565bf781d654339ee1ce83b17ee00d76d679608e`
- Test commit: `565bf781d654339ee1ce83b17ee00d76d679608e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 3 to 13.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 1 | 3 | 0 | 0 | [run](https://argusic.com/run/e3ff139b-91ac-4a5b-abb7-755d576ce3e6) |
| 2 | pass | 100 | 2 | 13.9 | 1 | 1 | [run](https://argusic.com/run/86a473ab-c1fd-4529-8932-bf5d8a48a014) |

## What was observed on a clean machine

Attempt 2:

- `Container has Node.js v18.19.1 but the project requires >=24 (engine constraint in package.json).`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
