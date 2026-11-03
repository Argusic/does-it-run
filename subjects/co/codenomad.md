# CodeNomad

**Verdict: runs.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/NeuralNomadsAI/CodeNomad, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/codenomad

## Pinned environment

- Project commit: `903b286df385f8381f55f302e8aa7eb82a9e6792`
- Test commit: `903b286df385f8381f55f302e8aa7eb82a9e6792`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 19.5 to 19.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 80 | 20 | 19.5 | 1 | 0 | [run](https://argusic.com/run/375780e6-08ab-4075-9230-928d6ab77849) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `zsh not installed , desktop POSIX shell selection test fails in user-shell.test.ts (1 of 326 native tests)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
