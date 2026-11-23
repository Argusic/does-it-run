# halp

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/orhun/halp, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/halp

## Pinned environment

- Project commit: `80797eaa0706f6fdfcf5d2905bba52961ebda738`
- Test commit: `80797eaa0706f6fdfcf5d2905bba52961ebda738`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 10 to 10.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 10 | 2 | 2 | [run](https://argusic.com/run/bec57fc3-bb2e-40b9-a45d-a62e27edd19e) |
| 2 | pass | 100 | 10 | 10.6 | 1 | 1 | [run](https://argusic.com/run/bc2b8897-1ae0-4b8c-bd9b-1fd77c740fa7) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `test_check_help_args expected --help success but -h succeeds first in reversed iteration`
- 1 min: `integration test expected -v/-h behavior but config uses long-form args`

Attempt 2:

- 5 min: `4 test failures: test_check_help_args, test_get_default_help, integration test expected output mismatched due to help arg iteration order change; completions/mangen tests missing OUT_DIR env var`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
