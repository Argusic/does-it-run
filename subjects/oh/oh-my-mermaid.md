# oh-my-mermaid

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/oh-my-mermaid/oh-my-mermaid, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/oh-my-mermaid

## Pinned environment

- Project commit: `38ccdb69298adec949177c92c88d6e3ddfb5bab7`
- Test commit: `38ccdb69298adec949177c92c88d6e3ddfb5bab7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 1.2 to 2.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.5 | 1.2 | 0 | 0 | [run](https://argusic.com/run/2e11f143-dbec-4dca-a777-1d1e49a47469) |
| 2 | pass | 100 | 0.5 | 2.7 | 1 | 1 | [run](https://argusic.com/run/4e1aac2f-91ce-4a5c-bdcf-ed4fc4dd89a4) |

## What was observed on a clean machine

Attempt 2:

- 0.2 min: `fs.watch with recursive:true throws 'feature watch recursively is unavailable on the current platform'`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
