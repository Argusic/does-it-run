# firstmate

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/kunchenguid/firstmate, licensed MIT, written in Shell.

Evidence and recordings: https://argusic.com/subject/firstmate

## Pinned environment

- Project commit: `3c2a91d70e07b48c982a8fe3460ba367795bb5d3`
- Test commit: `3c2a91d70e07b48c982a8fe3460ba367795bb5d3`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 44.9 to 44.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.5 | 44.9 | 2 | 2 | [run](https://argusic.com/run/c30f687b-e606-455d-a4b7-e63be8f6f09e) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `fm-pi-branch-extension.test.sh: Node 18 cannot load .ts files as ESM without package.json type:module marker`
- 2 min: `fm-lint.test.sh: ShellCheck and actionlint not on PATH`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
