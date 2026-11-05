# flowchart.js

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/adrai/flowchart.js, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/flowchart-js

## Pinned environment

- Project commit: `0186b39a95f180fc735a60803c95eb1fb0d24083`
- Test commit: `0186b39a95f180fc735a60803c95eb1fb0d24083`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 4.4 to 8.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 16 | 8.5 | 0 | 0 | [run](https://argusic.com/run/bb114392-ff24-463e-a266-1cec28764b60) |
| 2 | pass | 100 | 1.5 | 4.4 | 3 | 3 | [run](https://argusic.com/run/15fe0c8e-20f2-44d7-8395-ed9d12aa318e) |

## What was observed on a clean machine

Attempt 2:

- 3 min: `Raphael (raphael.min.js) loads into global scope and minified JS code spews to stdout when loaded in Node.js without a browser DOM`
- 1 min: `jsdom v30+ requires Node >=22; unsupported on Node 18 in container`
- 2 min: `jsdom SVG elements lack createSVGMatrix method; Raphael calls it during rendering`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
