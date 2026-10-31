# Serein

**Verdict: runs.** Argusic Score 97.5 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Yinglianchun/Serein, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/serein

## Pinned environment

- Project commit: `4d40ac8f9abaea5eb5eeeb8e37825a7c0783eb3c`
- Test commit: `4d40ac8f9abaea5eb5eeeb8e37825a7c0783eb3c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 86.6 to 86.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 97.5 | 40 | 86.6 | 8 | 7 | [run](https://argusic.com/run/f98f2054-41bd-4ec8-9417-865338e11448) |

## What was observed on a clean machine

Attempt 1:

- 45 min: `pipeline tests failed: compact agent packets no longer expose messages content/text`
- 10 min: `pipeline tests failed: compact active_tracks omit recent_turns/status`
- 3 min: `gateway contract test failed: SELF_USE_TOOLS has 15 entries not 14`
- 10 min: `legacy migration crashed on save_settings with policies=None`
- 15 min: `promote_event tests failed: promotion now requires mailbox_select first`
- 80 min: `image pipeline retried failed transcription for old settled Event originals in a new scope`
- 50 min: `test_local_runtime port-conflict probe failed with EADDRINUSE after stop`
- 15 min: `intermittent sqlite 'database is locked' in test_narrative_candidates (1-2 tests per full run, passes in isolation)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
