# scrape-it

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/IonicaBizau/scrape-it, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/scrape-it

## Pinned environment

- Project commit: `8d441141f237c815178233b8a1279f3dc652038f`
- Test commit: `8d441141f237c815178233b8a1279f3dc652038f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 2.8 to 2.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.5 | 2.8 | 1 | 1 | [run](https://argusic.com/run/517ee84f-2dd8-4d86-8373-d79c81de0061) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `ReferenceError: File is not defined due to undici@7.30.0 requiring Node >=20.18.1 (container has Node 18.19.1)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
