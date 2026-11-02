# agentic-awesome-skills

**Verdict: runs.** Argusic Score 95.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/sickn33/agentic-awesome-skills, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/agentic-awesome-skills

## Pinned environment

- Project commit: `2ed16bc0af734a66758117c5cf602a899bc312f9`
- Test commit: `2ed16bc0af734a66758117c5cf602a899bc312f9`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 7.6 to 21.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 7.6 | 2 | 2 | [run](https://argusic.com/run/0e383e89-d02b-4ab1-aed5-9a10ac63b1a0) |
| 2 | pass | 91.43 | 19 | 21.4 | 7 | 4 | [run](https://argusic.com/run/753dd3c6-a52c-48da-99c7-f5e77d18ec2d) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `git_pushing_helper.test.js: git init --ref-format=reftable failed (Git 2.43.0, needs ≥2.45)`
- 1 min: `test_audit_consistency.py: ModuleNotFoundError for yaml`

Attempt 2:

- 4 min: `npm ci warned EBADENGINE: project requires Node >=22 (and app requires ^22.22.2), container has Node v18.19.1`
- 2 min: `npm run validate failed with ModuleNotFoundError: No module named 'yaml'; no Python requirements are installed by npm ci`
- 1 min: `npm run app:test crashed: rolldown imports node:util styleText, unavailable on Node 18`
- 6 min: `npm test fails at tools/scripts/tests/git_pushing_helper.test.js: git init --ref-format=reftable exits 129 (Git 2.43 lacks reftable support, needs 2.45+)`
- 2 min: `aas mcp configure exits 5 with opaque AAS_CLI_PATH_NOT_FOUND and no detail about the missing path`
- 1 min: `aas.js --version exits 2 with AAS_CLI_OPTION_VALUE_REQUIRED invalid-input error`
- 1 min: `Backgrounded vite preview died when its parent shell exited, giving curl status 000`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
