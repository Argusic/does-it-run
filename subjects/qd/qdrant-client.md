# qdrant-client

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/qdrant/qdrant-client, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/qdrant-client

## Pinned environment

- Project commit: `cf747f4b6fa71ba35dfb467931f3fa65f2cdf263`
- Test commit: `cf747f4b6fa71ba35dfb467931f3fa65f2cdf263`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 5.8 to 32.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.1 | 32.1 | 3 | 3 | [run](https://argusic.com/run/7c4f341a-a1bb-4b38-aec3-b6f897d3c8e3) |
| 2 | pass | 80 | 15 | 5.8 | 1 | 0 | [run](https://argusic.com/run/e305fbf7-28e1-4207-a82a-8a398f8f9742) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `Qdrant server process killed between exec sessions; tests needing server fail with connection refused unless server runs in the same exec command`
- `test_text_match_on_unindexed_field(text_any) congruence test: local Qdrant client and server v1.19.1 differ on text-any matching against unindexed fields`
- `httpx/httpcore receives Errno 99 (Cannot assign requested address) when connecting to localhost due to IPv6 resolution failure in container`

Attempt 2:

- `112 local-mode tests pass; tests requiring a Qdrant server fail with Cannot assign requested address - no Qdrant server or Docker available in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
