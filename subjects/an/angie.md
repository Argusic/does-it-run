# angie

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/webserver-llc/angie, licensed BSD-2-Clause, written in C.

Evidence and recordings: https://argusic.com/subject/angie

## Pinned environment

- Project commit: `b401553c1750df3e74379784c6500a19d7c99da4`
- Test commit: `b401553c1750df3e74379784c6500a19d7c99da4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 16.3 to 16.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 16.3 | 5 | 5 | [run](https://argusic.com/run/a70f2b7e-2d5a-4f14-b60c-ad026c3f0cac) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `Missing PCRE2 development headers (libpcre2-dev)`
- 0.5 min: `Missing zlib development headers (zlib1g-dev)`
- 2 min: `Missing Perl modules Test::Deep and JSON`
- `IPv6 loopback (::1) disabled in container; 36 tests skipped`
- `server_cert_type_var.t: 7 of 15 tests fail with undef from $ssl_server_cert_type on OpenSSL 3.0`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
