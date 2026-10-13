# anatomy

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/wheresryan22/anatomy, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/anatomy

## Pinned environment

- Project commit: `689dcf966e63d92be10a5d593c6e19e10acd4422`
- Test commit: `689dcf966e63d92be10a5d593c6e19e10acd4422`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 13.6 to 13.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 15 | 13.6 | 4 | 4 | [run](https://argusic.com/run/805a25cd-81e5-4609-ba8f-69e8eba76d65) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `System Node v18.19.1 below required 20.10+ (tests need 22); skills CLI needs >=22.20`
- 3 min: `No Chrome/Chromium installed for the repo's headless render checks`
- 3 min: `Chromium aborted: FATAL: No usable sandbox! (container blocks unprivileged user namespaces; repo spawns Chrome without --no-sandbox)`
- 2 min: `skills CLI crashed on Node 18 with 'node:util does not provide styleText'`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
