# luvus

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/RizRiyz/luvus, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/luvus

## Pinned environment

- Project commit: `8029d9b5e3ed216fbab55bfc672060471c4c07aa`
- Test commit: `8029d9b5e3ed216fbab55bfc672060471c4c07aa`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 23.9 to 23.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 35 | 23.9 | 3 | 3 | [run](https://argusic.com/run/d82026c2-3856-42b3-8c05-cdd85d60eabd) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `adjacent_mentions_submit_one_command_to_four_shell_panes: PTY panes wrap paste in bracketed-paste markers, so assert_eq!(paste, b"ls") fails`
- 5 min: `omp_extension tests: Node 18 lacks --experimental-strip-types`
- `hook_script_reports_claude_but_never_a_devin_host: flaky in parallel test suite (passes in isolation)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
