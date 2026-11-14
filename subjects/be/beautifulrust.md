# BeautifulRust

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/morganlinton/BeautifulRust, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/beautifulrust

## Pinned environment

- Project commit: `a2b22682fa69b5e2d41a5d041663df7d51aac521`
- Test commit: `a2b22682fa69b5e2d41a5d041663df7d51aac521`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 2.1 to 6.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 6.9 | 1 | 1 | [run](https://argusic.com/run/0a12e338-3c3f-4811-be8c-573441be37b6) |
| 2 | pass | 100 | 0.4 | 2.1 | 1 | 1 | [run](https://argusic.com/run/c6bb7641-9183-45af-b227-2b8dfb81c957) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `npx skills failed to start: import { styleText } from "node:util" , SyntaxError under the container's Node 18.19 (package requires Node 22.20+)`

Attempt 2:

- 0.2 min: `Rust toolchain not installed in container (no cargo/rustc on PATH)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
