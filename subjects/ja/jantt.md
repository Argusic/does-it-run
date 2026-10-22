# Jantt

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/AhmadHassan-BTed/Jantt, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/jantt

## Pinned environment

- Project commit: `2fd3830d89090f1cd95683a18f4d715a1c704f44`
- Test commit: `2fd3830d89090f1cd95683a18f4d715a1c704f44`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 13.6 to 13.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 22 | 13.6 | 3 | 3 | [run](https://argusic.com/run/e6e87853-81fc-4c31-bacf-8819e7d06e4b) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `reconciler test: 'cleanly prunes dangling dependencies when predecessor tasks are deleted' failed , tombstone not found due to automated 30-day purge cutting tombstone with date 2026-09-05 on current date 2026-10-18`
- 1 min: `reconciler test: 'performs autonomous JSON maintenance: prunes expired tombstones, caps bloat, strips empty timestamps' failed , fresh tombstone not retained because date 2026-09-05 was >30 days before current date`
- 1 min: `reconciler test: 'handles tombstone lifecycle: resurrection on post-deletion edit and clean tombstone purging' failed , tombstone with date 2026-10-01 at 12:00 vs edit at 2026-10-01 12:15 both pruned by 30-day cutoff`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
