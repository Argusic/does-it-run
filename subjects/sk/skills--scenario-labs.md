# skills

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/scenario-labs/skills, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/run/933671e6-5683-4c06-ac01-9e5e47cd5ec0

## Pinned environment

- Project commit: `d87071d22edb5eb5871c9034f89cada518657891`
- Test commit: `d87071d22edb5eb5871c9034f89cada518657891`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 8.7 to 8.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 40 | 8.7 | 5 | 5 | [run](https://argusic.com/run/933671e6-5683-4c06-ac01-9e5e47cd5ec0) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `pnpm 11.21.0 from package.json requires Node >=22.13; container has Node 18.19.1`
- 5 min: `pip install fails: externally managed environment (PEP 668)`
- 1 min: `prettier chokes on .venv shell scripts when they aren't in prettierignore`
- 2 min: `cspell 10.0.1 requires Node >=22.18; validates its own version before checking files`
- 1 min: `spec validation needs uvx which is not installed`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
