# ollama-gui

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/HelgeSverre/ollama-gui, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/ollama-gui

## Pinned environment

- Project commit: `48b35b91ae59a7e04c72a7b718f319c0cec247df`
- Test commit: `48b35b91ae59a7e04c72a7b718f319c0cec247df`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 2.9 to 3.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 3.6 | 2 | 2 | [run](https://argusic.com/run/a8f711b0-d3fc-4422-88a9-7649ae47a5a4) |
| 2 | pass with mocks | 92 | 4 | 2.9 | 2 | 2 | [run](https://argusic.com/run/90042859-da9e-4a48-a06c-708fc684067f) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Bun binary not found and unzip missing for official installer`
- 1 min: `Node.js v18 too old (Vite 8 requires >=20)`

Attempt 2:

- 1 min: `bun not installed`
- 1 min: `Node.js 18 too old for Vite 8 / rolldown (missing styleText in node:util)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
