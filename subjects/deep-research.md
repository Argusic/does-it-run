# deep-research

**Verdict: could not verify.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/u14app/deep-research, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/deep-research

## Pinned environment

- Project commit: `4a211edd9face54d0786ecf73e69ce5257627e20`
- Test commit: `4a211edd9face54d0786ecf73e69ce5257627e20`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 16.8 to 18.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 16 | 18.5 | 3 | 3 | [run](https://argusic.com/run/b76e98d2-2508-4e39-8a7c-074322920055) |
| 2 | fail | 80 | 17 | 16.8 | 1 | 1 | [run](https://argusic.com/run/76f919c7-244a-46e5-a7e8-e02d46a5ed47) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `pnpm not found in PATH`
- 4 min: `ERR_PNPM_IGNORED_BUILDS: sharp and unrs-resolver build scripts blocked`
- 1 min: `Next.js build process killed (OOM/exit 137)`

Attempt 2:

- 2 min: `next build killed by OOM (8GB cgroup limit) during static page generation`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
