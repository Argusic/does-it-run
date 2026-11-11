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
- Valid runs: 2; wall time 20.6 to 43.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1 | 20.6 | 4 | 4 | [run](https://argusic.com/run/4f0dc180-56b2-4088-8b27-ad05eb54baeb) |
| 2 | pass | 100 | 0.04 | 43.1 | 11 | 11 | [run](https://argusic.com/run/29095b3d-3f9c-429f-80cf-05c23f3dc891) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `PyYAML dependency not installed for system Python`
- 1 min: `Permission approvals expired (2026-09-30) in security/permission_policy.json`
- 1 min: `Stale review document reports/skill-os-2-review.md referenced old scores/blocks`
- 1 min: `Hardcoded 2026-09-30 expiry dates in test files verify_trust_check.py, verify_review_waivers.py, verify_yao_cli.py`

Attempt 2:

- 1 min: `PyYAML not installed for system python3; validate_skill.py failed with ModuleNotFoundError: No module named 'yaml'`
- 3 min: `yao-cli-check: verify_yao_cli.py asserted local_blueprint_ready is True but committed evidence has review-studio blockers`
- 1 min: `yao-cli-check: verify_yao_cli.py asserted evidence decision 'consistent' but committed evidence shows 'evidence-drift-detected'`
- 1 min: `yao-cli-check: verify_yao_cli.py assert report_result['ok'] failed because render_evidence_consistency.py exits with code 2 (drift detected)`
- 2 min: `trust-check: Permission approvals expired (file_write, network, subprocess all expired 2026-09-30)`
- 5 min: `review-studio-check: Multiple assertion failures: decision, world_class_score, blocker_count, action_count, review_action gate_keys, trust_gate status, permission_gate status, waivers_gate status, world_class action keys, local_blueprint_re`
- 1 min: `skill-os2-audit-check: payload.ok expected True but was False (review-studio missing), missing_count expected 0 but was 1`
- 2 min: `skill-os2-coverage-check: Multiple assertion failures for decision, pass_count, warn_count, local_blueprint_ready, review-studio status, evidence-consistency status, markdown text`
- 1 min: `world-class-evidence-check: payload.ok expected True but was False`
- 1 min: `world-class-runbook-check: release_gate_blocked_count expected 4 but was 5, evidence_consistency_clean passed expected True but was False`
- 4 min: `evidence-consistency-check: Multiple failures: check=True raising CalledProcessError on exit code 2, payload.ok expected True, decision expected 'consistent', fail_count expected 0, action keys mismatch, skill-os-2-review status expected 'p`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
