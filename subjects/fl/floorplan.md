# floorplan

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/haydenschmitty/floorplan, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/floorplan

## Pinned environment

- Project commit: `1ab7e19c8772800b6fbc9453b92d93efb52ddb37`
- Test commit: `1ab7e19c8772800b6fbc9453b92d93efb52ddb37`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 11.5 to 14.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.1 | 11.5 | 0 | 0 | [run](https://argusic.com/run/d44ab9fe-9ef3-4324-8c83-a7207f5d521c) |
| 2 | pass | 100 | 0 | 14.4 | 1 | 1 | [run](https://argusic.com/run/21efd350-6a6a-4094-a104-d3a8df628d00) |

## What was observed on a clean machine

Attempt 2:

- 5 min: `test failure: 'files of unclosed lists and brackets are still read quickly' asserted <2000ms but 'route objects nested deep (1.0 MB)' took 2213ms under full suite load`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
