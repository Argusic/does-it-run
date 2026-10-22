# fastschema

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/fastschema/fastschema, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/fastschema

## Pinned environment

- Project commit: `813349976c7cf4a884a995f6fcad9aace08b1541`
- Test commit: `813349976c7cf4a884a995f6fcad9aace08b1541`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 17.8 to 17.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 25 | 17.8 | 3 | 3 | [run](https://argusic.com/run/f239cafd-f1af-4983-8a08-75ed173f373e) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `MAIL=/var/mail/runner env var (standard system mailbox path) broke JSON-unmarshal in createMailClients, panicking all tests`
- 2 min: `11 integration test packages fail: dial tcp 127.0.0.1:3307: connection refused`
- `TestSendRequest in pkg/auth fails sporadically: example.local DNS returns 'server misbehaving' instead of 'timeout'`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
