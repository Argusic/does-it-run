# PersonalWiki

**Verdict: runs.** Argusic Score 75 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/aleen42/PersonalWiki, licensed MIT, written in C.

Evidence and recordings: https://argusic.com/subject/personalwiki

## Pinned environment

- Project commit: `a04254d51874503cebdfd5200c45e4260bbe1f08`
- Test commit: `a04254d51874503cebdfd5200c45e4260bbe1f08`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 15 to 60.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 50 | 5.2 | 60.3 | 4 | 4 | [run](https://argusic.com/run/f615e7f1-e71c-4b0b-92c1-c01af8830c70) |
| 2 | pass | 100 | 15 | 15 | 2 | 2 | [run](https://argusic.com/run/6992381d-329c-4026-9f7c-0391afe257ec) |

## What was observed on a clean machine

Attempt 1:

- 1.9 min: `HonKit 3.6.22 full build hangs with 677 pages - page generation stalls indefinitely during serial processing`
- 7.3 min: `Node 18 incompatible with honkit@7.0.1 (requires Node >=20) - undici File is not defined`
- 0.5 min: `book.json and package.json missing from repo`
- 0.5 min: `'''def code block in Embedded_System/autogen/autogen.md triggers highlight.js error`

Attempt 2:

- 8 min: `graceful-fs polyfill crashes on Node 18 with cb.apply is not a function`
- 2 min: `honkit (Python and npm) fails with undici File not defined on Node 18`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
