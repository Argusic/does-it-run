# opengap

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/open-gitagent/opengap, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/opengap

## Pinned environment

- Project commit: `d7a8e2edb54b942d6b4635cdd8b919ebd23e5da5`
- Test commit: `d7a8e2edb54b942d6b4635cdd8b919ebd23e5da5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 5.2 to 5.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.02 | 5.2 | 1 | 1 | [run](https://argusic.com/run/e421e32f-8225-41e9-ba19-e6b3860189f4) |

## What was observed on a clean machine

Attempt 1:

- 0.1 min: `init --dir fails if directory doesn't exist (doesn't auto-create)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
