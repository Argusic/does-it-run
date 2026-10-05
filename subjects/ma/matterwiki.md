# Matterwiki

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Matterwiki/Matterwiki, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/matterwiki

## Pinned environment

- Project commit: `92ca38c897196ce64c27eec7d798346dc798a4d5`
- Test commit: `92ca38c897196ce64c27eec7d798346dc798a4d5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 31.6 to 31.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 35 | 31.6 | 3 | 3 | [run](https://argusic.com/run/ed512706-8101-4bc6-96ad-e30dec70944a) |

## What was observed on a clean machine

Attempt 1:

- 20 min: `sqlite3@3.1.4 native module fails to compile on Node 18 (V8 API incompatibility and missing python symlink)`
- 10 min: `knex@0.11.10 missing lib/ directory with dialect and driver code after npm install`
- 5 min: `Node 18 crashes on unhandled promise rejections from bookshelf/knex promise chains without .catch() handlers`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
