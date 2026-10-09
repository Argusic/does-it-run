# ollama-gui

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/HelgeSverre/ollama-gui, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/ollama-gui

## Pinned environment

- Project commit: `48b35b91ae59a7e04c72a7b718f319c0cec247df`
- Test commit: `48b35b91ae59a7e04c72a7b718f319c0cec247df`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 3.6 to 3.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 3.6 | 2 | 2 | [run](https://argusic.com/run/a8f711b0-d3fc-4422-88a9-7649ae47a5a4) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Bun binary not found and unzip missing for official installer`
- 1 min: `Node.js v18 too old (Vite 8 requires >=20)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
