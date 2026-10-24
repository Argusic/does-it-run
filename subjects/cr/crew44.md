# crew44

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/getcrew44/crew44, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/crew44

## Pinned environment

- Project commit: `cfcf1e74d9a23b91cc68e49690a99c8385a7c89d`
- Test commit: `cfcf1e74d9a23b91cc68e49690a99c8385a7c89d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 7.7 to 7.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 7 | 7.7 | 1 | 1 | [run](https://argusic.com/run/070fc304-8352-49cf-bdee-21d3660f1307) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Node 18.19.1 too old (needs >=20.19.0 for jsdom/html-encoding-sniffer CJS/ESM compat); also Go missing`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
