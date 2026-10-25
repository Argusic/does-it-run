# clayoven

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/artagnon/clayoven, licensed MIT, written in Ruby.

Evidence and recordings: https://argusic.com/subject/clayoven

## Pinned environment

- Project commit: `ed6477fe6b02f1b71232786aed8ff3ed7b23700f`
- Test commit: `ed6477fe6b02f1b71232786aed8ff3ed7b23700f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 10.3 to 10.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 10.3 | 5 | 5 | [run](https://argusic.com/run/342ae586-755d-43bc-b9aa-cd7be719250b) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `Ruby 3.3.5 not pre-installed in container`
- 2 min: `zlib headers missing, Ruby built without zlib support`
- 1 min: `libyaml headers missing, psych extension not built`
- 1 min: `yarn not found, production tests failed`
- `Production tests use external artagnon.com repo which requires Node.js >=20 (container has 18.19.1)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
