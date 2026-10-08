# Portable-Local-Studio

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/techjarves/Portable-Local-Studio, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/portable-local-studio

## Pinned environment

- Project commit: `6c3059443666edba1d5ad7f72ec42afad1ca779e`
- Test commit: `6c3059443666edba1d5ad7f72ec42afad1ca779e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 6.6 to 6.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 13 | 6.6 | 4 | 4 | [run](https://argusic.com/run/4e79f3e1-15d7-4879-aaed-1c3e9ad236fe) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `npm install missing for frontend deps`
- 3 min: `vite 8 requires Node 22.12+, system has Node 18`
- 1 min: `rolldown native binding missing for linux-x64-gnu`
- 1 min: `npm run build resolves to system Node 18 via shebang`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
