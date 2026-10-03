# vscode-restclient

**Verdict: could not verify.** Argusic Score 65 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Huachao/vscode-restclient, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/vscode-restclient

## Pinned environment

- Project commit: `0773d56b65d9e7033259519e99eef8f752f6ba6e`
- Test commit: `0773d56b65d9e7033259519e99eef8f752f6ba6e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 7.4 to 12.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 50 | 4.5 | 7.4 | 1 | 1 | [run](https://argusic.com/run/6a683ab8-cf01-4ef0-80eb-147798f7a373) |
| 2 | fail | 80 | 10 | 12.3 | 1 | 1 | [run](https://argusic.com/run/508e88ed-7687-45d5-a8fc-63e99a22ca2f) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `VS Code extension cannot be launched without the VS Code extension host runtime (vscode module not found outside of VS Code)`

Attempt 2:

- 5 min: `npx webpack --mode production (vscode:prepublish) repeatedly timed out after 30s due to TerserPlugin minification on large bundle`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
