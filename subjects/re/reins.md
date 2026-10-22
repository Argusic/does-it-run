# reins

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/pegasi-ai/reins, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/reins

## Pinned environment

- Project commit: `d5bc85ddfc9ad13ec22925c63312f85da94b96a7`
- Test commit: `d5bc85ddfc9ad13ec22925c63312f85da94b96a7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 17.2 to 17.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 15 | 17.2 | 3 | 3 | [run](https://argusic.com/run/8b33ff1f-d38c-4e7e-9983-c68373e36822) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `package.json had dangling 'winston': '^3.11.0' inside the keywords array instead of keywords array item`
- 0.5 min: `inquirer v9 is ESM-only but project compiles to CommonJS (tsc module: commonjs), so require() of inquirer/lib/index.js fails`
- 2 min: `3 scan tests expected exit code 1 but Node 18.19.1 is flagged as vulnerable by isNodeVersionVulnerable (< 22.14.0), producing EXPOSED verdict (exit code 2)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
