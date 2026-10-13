# SoL-Pi

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/NVlabs/SoL-Pi, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/sol-pi

## Pinned environment

- Project commit: `06b3ee358ddc5cebc5fb21a8e7493fab2db508ce`
- Test commit: `06b3ee358ddc5cebc5fb21a8e7493fab2db508ce`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 3.2 to 3.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 3.2 | 2 | 2 | [run](https://argusic.com/run/c732acf6-d548-4a5f-951d-48142fdc48c2) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Container's system Node is v18.19.1, below the project's required >=22.19.0.`
- 2 min: `npm audit --audit-level=high exits 1 with 6 vulnerabilities (3 moderate, 3 high) in the pinned Pi 0.85.1 dev toolchain (undici, brace-expansion, source-map-js, vitest).`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
