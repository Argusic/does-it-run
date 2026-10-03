# tuicr

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/agavra/tuicr, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/tuicr

## Pinned environment

- Project commit: `9175dc95b97a0a7dd290d43d38385745a7fb7d40`
- Test commit: `9175dc95b97a0a7dd290d43d38385745a7fb7d40`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4.8 to 4.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 10.2 | 4.8 | 1 | 1 | [run](https://argusic.com/run/69a2a093-8b6b-43ba-96e6-16359a0ff9ff) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `2 of 1832 tests failed (should_discover_worktree_with_relativeworktrees_extension, default_preference_routes_reftable_repo_to_cli) , both require git extensions (reftable, relativeworktrees) added in git 2.48+, but container has git 2.43.0`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
