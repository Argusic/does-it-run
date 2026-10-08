# Tracely-ai

**Verdict: runs.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Jwuthri/Tracely-ai, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/tracely-ai

## Pinned environment

- Project commit: `f332bc865d60cd4828dedf857bb58c15f388a045`
- Test commit: `f332bc865d60cd4828dedf857bb58c15f388a045`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 43.1 to 43.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 80 | 5 | 43.1 | 2 | 0 | [run](https://argusic.com/run/94f66228-6fad-41a8-8384-41ee0e109864) |

## What was observed on a clean machine

Attempt 1:

- 15 min: `frontend vitest tests fail on Node 18 - jsdom@30 depends on whatwg-url@17.1.0 (engines: ^22.14.0) and undici@8.10.1 (engines: >=22.19.0), container has Node 18.19.1`
- 5 min: `pnpm build (next build) OOM killed during static page generation after successful compilation`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
