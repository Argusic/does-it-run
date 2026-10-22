# svg-diagram

**Verdict: runs.** Argusic Score 93.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/bybit-exchange/svg-diagram, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/svg-diagram

## Pinned environment

- Project commit: `c30c9e3bc9a70f2b77b60c7ea27157de3a88d81a`
- Test commit: `c30c9e3bc9a70f2b77b60c7ea27157de3a88d81a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 5.5 to 5.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 93.33 | 12 | 5.5 | 3 | 2 | [run](https://argusic.com/run/56f14f28-2a1c-4e2d-a2be-ded89d592cff) |

## What was observed on a clean machine

Attempt 1:

- 7 min: `npm test fails on the container's default Node v18.19.1: glob argument 'tools/svg-lint/test/**/*.test.mjs' is not supported ('Could not find ...*.test.mjs')`
- 4 min: `README install command 'npx skills add bybit-exchange/svg-diagram -g' crashes on Node v18.19.1: node:util has no export named styleText (skills@1.7.2 requires node >=22.20.0)`
- 1 min: `No rsvg-convert delegate, so ImageMagick ('convert') cannot rasterize SVG in this container (environment gap, stated in README)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
