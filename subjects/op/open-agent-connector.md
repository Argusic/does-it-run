# open-agent-connector

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Anil-matcha/open-agent-connector, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/open-agent-connector

## Pinned environment

- Project commit: `41d306722688bb979bceaa83e27a984c390f2a81`
- Test commit: `41d306722688bb979bceaa83e27a984c390f2a81`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 9.4 to 9.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 12 | 9.4 | 4 | 4 | [run](https://argusic.com/run/65664daf-627a-42e3-b0d4-d20a8f8fac2e) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Python externally-managed environment blocks pip install`
- 2 min: `Node.js 18.19.1 incompatible with Next.js 16 (requires >=20.9.0)`
- 1 min: `Stale node_modules from Node 18 caused zod/vitest type errors in build`
- `Standalone test_security_contracts.py fails on action execution (needs real GitHub credentials)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
