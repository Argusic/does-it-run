# claude-vibe-squad

**Verdict: not yet verified.** Argusic Score 50 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/mtarcure/claude-vibe-squad, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/claude-vibe-squad

## Pinned environment

- Project commit: `5392a48276bb17446f9630bcbea98ad23feea079`
- Test commit: `5392a48276bb17446f9630bcbea98ad23feea079`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 44.7 to 44.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 50 | 1 | 44.7 | 3 | 3 | [run](https://argusic.com/run/9e6bfc76-01f5-494d-8897-158760ebf15c) |

## What was observed on a clean machine

Attempt 1:

- 20 min: `dispatch-toolkit.sh crashes on missing private registry file shared/registries/skill-tool-registry.tsv (not shipped in public repo)`
- 10 min: `orphan_supervisor_leak test fails because SQUAD_BASE_BRANCH not set in test env, supervisor exits 74 instead of expected 75`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
