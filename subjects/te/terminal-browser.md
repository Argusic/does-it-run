# terminal-browser

**Verdict: runs with mocks.** Argusic Score 56 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/zenbu-labs/terminal-browser, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/terminal-browser

## Pinned environment

- Project commit: `2bdf227cceb645fa49de353c6856092937aa6ac3`
- Test commit: `2bdf227cceb645fa49de353c6856092937aa6ac3`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 3.7 to 9.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | 0 | 3.7 | 0 | 0 | [run](https://argusic.com/run/0cb3edfc-c3ee-4242-981c-f92fb1f73658) |
| 2 | pass with mocks | 92 | 7 | 9.4 | 4 | 4 | [run](https://argusic.com/run/200b4875-6c5f-4421-a79c-4f189fff9a6c) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `import.meta.dirname unsupported on Node 18 in pixel postinstall script`
- 1 min: `unzip binary not available in container`
- 1 min: `node:sqlite missing on Node 18 (system Node)`
- `zsh shell-safety test skipped (zsh not installed in container)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
