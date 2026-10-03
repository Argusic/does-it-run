# button-card

**Verdict: could not verify.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/custom-cards/button-card, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/button-card

## Pinned environment

- Project commit: `dfa304f93ab73b41011b624960657c568672e9c9`
- Test commit: `dfa304f93ab73b41011b624960657c568672e9c9`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 5.2 to 8.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 0.5 | 8.5 | 1 | 1 | [run](https://argusic.com/run/ca38e48d-ed36-4527-9fdb-cd15a0b5f4eb) |
| 2 | fail | 80 | 1.5 | 5.2 | 0 | 0 | [run](https://argusic.com/run/bc7b80b1-d97e-4e57-8347-6eca37435985) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `npm install ERESOLVE dependency conflict between eslint@9.38.0 and eslint-config-airbnb-base@15.0.0`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
