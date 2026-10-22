# purrcrypt

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/vxfemboy/purrcrypt, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/purrcrypt

## Pinned environment

- Project commit: `88c7e96eb9e5262952db71aa027ad4393794b2eb`
- Test commit: `88c7e96eb9e5262952db71aa027ad4393794b2eb`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 7.2 to 7.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 7 | 7.2 | 1 | 1 | [run](https://argusic.com/run/77fddc2c-af6e-44d3-ae87-8ad232f0a2b9) |

## What was observed on a clean machine

Attempt 1:

- 25 min: `purr genkey alice wrote a 0-byte public key file (~/.purr/keys/public/alice.pub); subsequent encrypt failed with 'Invalid key format: Failed to parse public key: crypto error'`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
