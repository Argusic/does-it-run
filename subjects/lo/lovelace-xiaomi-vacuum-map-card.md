# lovelace-xiaomi-vacuum-map-card

**Verdict: could not verify.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/PiotrMachowski/lovelace-xiaomi-vacuum-map-card, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/lovelace-xiaomi-vacuum-map-card

## Pinned environment

- Project commit: `045c3ac946d4ef0a01201f306e9949643984a155`
- Test commit: `045c3ac946d4ef0a01201f306e9949643984a155`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 3.6 to 4.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 2 | 3.6 | 1 | 1 | [run](https://argusic.com/run/45d0186c-c236-4e6e-95a7-464e1bce1de2) |
| 2 | fail | 80 | 0.2 | 4.2 | 1 | 1 | [run](https://argusic.com/run/988faee1-df3a-4b47-96ac-9b2f2804f07e) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `tslib v2.1.0 bundled with rollup-plugin-typescript2 has exports field that blocks ./tslib.es6.js and ./package.json on Node 18`

Attempt 2:

- 0.1 min: `tslib v2.1.0 has an 'exports' field in package.json lacking subpath entries (.package.json, .tslib.es6.js), causing Node 18 to reject require() calls`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
