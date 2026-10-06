# evlog

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/evloghq/evlog, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/evlog

## Pinned environment

- Project commit: `cced5e896135d04bf4d8fa19dd17625211814c7d`
- Test commit: `cced5e896135d04bf4d8fa19dd17625211814c7d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 9.9 to 9.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2.5 | 9.9 | 3 | 3 | [run](https://argusic.com/run/229d2563-6b64-498a-bb6c-d8ac9025030d) |

## What was observed on a clean machine

Attempt 1:

- 1.5 min: `Node v18.19.1 too old for pnpm 11.26.0 (needs >=22.13)`
- 2.5 min: `structuredClone used by cloneForRedaction destroys DOMException objects (prototype properties lost)`
- 1 min: `corepack threw 'Cannot find matching keyid' due to missing signing key`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
