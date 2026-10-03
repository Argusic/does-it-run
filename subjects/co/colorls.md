# colorls

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/athityakumar/colorls, licensed MIT, written in Ruby.

Evidence and recordings: https://argusic.com/subject/colorls

## Pinned environment

- Project commit: `ec2fbcd36f6b7fa56c72b13e52c235eba277bad0`
- Test commit: `ec2fbcd36f6b7fa56c72b13e52c235eba277bad0`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 18.7 to 18.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 18 | 18.7 | 4 | 4 | [run](https://argusic.com/run/b80e7c63-8837-4f1b-8b2a-b252377a2c61) |

## What was observed on a clean machine

Attempt 1:

- 6 min: `Ruby not installed in environment`
- 2 min: `zlib Ruby extension failed to build (missing headers)`
- 3 min: `psych (YAML) Ruby extension failed to build (missing libyaml)`
- 2 min: `Bundler dependency resolution failed on version constraints`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
