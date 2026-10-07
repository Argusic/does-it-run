# amical

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/amicalhq/amical, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/amical

## Pinned environment

- Project commit: `19d414a91e0ad3e527b67fcc7fdc2be686ac9951`
- Test commit: `19d414a91e0ad3e527b67fcc7fdc2be686ac9951`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 22.9 to 22.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 24 | 22.9 | 4 | 4 | [run](https://argusic.com/run/87a66680-61cc-4876-bd88-1377568bf771) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `onnxruntime-node postinstall failed trying to download Windows CUDA binaries from NuGet on Linux`
- 5 min: `libgomp.a static linking failed: not compiled with -fPIC, cannot link into shared .node extension`
- 2 min: `System Node.js v18.19.1 too old, project requires >=24`
- 1 min: `pnpm not available on system PATH`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
