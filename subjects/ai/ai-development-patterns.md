# ai-development-patterns

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/PaulDuvall/ai-development-patterns, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/ai-development-patterns

## Pinned environment

- Project commit: `bf3ccc73be64c4bef6134fab778e13a7d1e0e8b0`
- Test commit: `bf3ccc73be64c4bef6134fab778e13a7d1e0e8b0`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 7.4 to 7.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 7.4 | 5 | 5 | [run](https://argusic.com/run/3e17abe0-ad2a-41b6-9321-e698f409a22a) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `pip install -e . failed: flat-layout package discovery conflict in pyproject.toml`
- `test_evidence_urls_alive failed: 1 URL returns 404 (centralized-rules.yaml -> docs.port.io/guides)`
- `test_complete_evidence_quotes_still_present failed: 4 URLs had content drift (redirects or missing quotes)`
- 1 min: `test_status_view_in_sync failed: verification/STATUS.md was stale`
- `git push failed: no credentials configured for https://github.com`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
