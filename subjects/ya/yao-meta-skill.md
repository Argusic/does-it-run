# yao-meta-skill

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/yaojingang/yao-meta-skill, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/yao-meta-skill

## Pinned environment

- Project commit: `f5d8f681372edae1915991e2de0c23dc306dd30f`
- Test commit: `f5d8f681372edae1915991e2de0c23dc306dd30f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 20.6 to 20.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1 | 20.6 | 4 | 4 | [run](https://argusic.com/run/4f0dc180-56b2-4088-8b27-ad05eb54baeb) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `PyYAML dependency not installed for system Python`
- 1 min: `Permission approvals expired (2026-09-30) in security/permission_policy.json`
- 1 min: `Stale review document reports/skill-os-2-review.md referenced old scores/blocks`
- 1 min: `Hardcoded 2026-09-30 expiry dates in test files verify_trust_check.py, verify_review_waivers.py, verify_yao_cli.py`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
