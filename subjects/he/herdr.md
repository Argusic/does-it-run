# herdr

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/herdrdev/herdr, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/herdr

## Pinned environment

- Project commit: `2290257acb2085ce6842ba5c7e3ca50c3ba64f02`
- Test commit: `2290257acb2085ce6842ba5c7e3ca50c3ba64f02`
- Worker image digests: `sha256:33ceb71981b602c1a7443a53469e4dba065f7503eab3078a2d7a57a2ab987517`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 15.3 to 18.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 13 | 17.3 | 3 | 3 | [run](https://argusic.com/run/146318be-8d64-498d-b8fd-2ab642848499) |
| 2 | pass | 100 | 5 | 15.3 | 1 | 1 | [run](https://argusic.com/run/eff57474-5e35-45c6-8d10-38cfc95a2f3f) |
| 3 | pass | 100 | 6 | 18.7 | 0 | 0 | [run](https://argusic.com/run/20df757a-5718-4d32-a8da-6b0bc5d1e08e) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `zig not found for vendored libghostty-vt build`
- 2 min: `fragile workspace ID length test assert len() <= 3 fails after many test runs`
- 2 min: `two tests fail in parallel due to port binding conflict`

Attempt 2:

- 2 min: `workspace::tests::generated_workspace_ids_are_short_base32_handles asserted 'first.len() <= 3' but the 'w' prefix makes valid 3-char base32 handles 4 chars total (e.g. 'w18E')`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
