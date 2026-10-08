# brew

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Homebrew/brew, licensed BSD-2-Clause, written in Ruby.

Evidence and recordings: https://argusic.com/subject/brew

## Pinned environment

- Project commit: `1b0b73c84bf684401e2af7dd1ad420ba147ee0fb`
- Test commit: `1b0b73c84bf684401e2af7dd1ad420ba147ee0fb`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 51 to 51 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.5 | 51 | 3 | 3 | [run](https://argusic.com/run/17fce041-f905-408b-a974-d0c72c3b6f47) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `service_spec.rb: 6 tests fail due to umask 0002 creating group-writable env files`
- 2 min: `trust_spec.rb: 1 test fails due to target dir being group-writable`
- 2 min: `cmd/untrust_spec.rb: 1 test fails due to trust_home dir being group-writable`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
