# tengine

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/alibaba/tengine, licensed BSD-2-Clause, written in C.

Evidence and recordings: https://argusic.com/subject/tengine

## Pinned environment

- Project commit: `f9c9f759c029dec42ad855141fa7f0c24e9a671e`
- Test commit: `f9c9f759c029dec42ad855141fa7f0c24e9a671e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 8.3 to 12.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3.3 | 12.7 | 4 | 4 | [run](https://argusic.com/run/eddae356-fe39-4387-9fee-683dba515ee8) |
| 2 | pass | 92 | 7 | 8.3 | 5 | 3 | [run](https://argusic.com/run/7a808101-6250-42c1-af2c-96c03785343c) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `PCRE library not found at configure time`
- 0.5 min: `zlib library not found at configure time`
- 0.5 min: `Permission denied installing to /usr/local/tengine (no root)`
- 0.3 min: `Permission denied binding to port 80`

Attempt 2:

- 2 min: `The default ./configure exited 1 because the HTTP rewrite module requires the PCRE library.`
- 1 min: `The README default install prefix /usr/local was not writable by user runner.`
- 1 min: `Optional tengine-tests/consistent_hash.t failed to start because the default build has no consistent_hash directive.`
- 2 min: `Optional dynamic_resolve.t and vnswrr4dynamic_ups.t failed because Net::DNS::Nameserver was absent; vnswrr4dynamic_ups.t also found no vnswrr directive.`
- `The optional file utility was missing, so one archive inspection command exited 127.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
