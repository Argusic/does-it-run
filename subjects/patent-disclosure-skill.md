# patent-disclosure-skill

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/handsomestWei/patent-disclosure-skill, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/patent-disclosure-skill

## Pinned environment

- Project commit: `1acef5c8bf950ec181d97ffeb4dba0497f642b18`
- Test commit: `1acef5c8bf950ec181d97ffeb4dba0497f642b18`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 5 to 5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 4 | 5 | 3 | 3 | [run](https://argusic.com/run/5b8bf8f7-1a26-4834-b01b-b7437816b29b) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `externally-managed-environment error on system pip install`
- 2 min: `playwright chromium browser not found on first probe`
- 1 min: `patent-map test failed due to floating-point PCA assertion without numpy; patent-oa tests couldn't collect without numpy`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
