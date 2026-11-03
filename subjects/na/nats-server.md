# nats-server

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/nats-io/nats-server, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/nats-server

## Pinned environment

- Project commit: `eb6f3a8c57867fcfc04e97a1b865a21646c82702`
- Test commit: `eb6f3a8c57867fcfc04e97a1b865a21646c82702`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 14.8 to 76.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.8 | 14.8 | 1 | 1 | [run](https://argusic.com/run/61376d35-0047-4048-a6fe-5611e8f0d22e) |
| 2 | pass | 100 | 76 | 76.3 | 10 | 10 | [run](https://argusic.com/run/2c16638b-237a-42ef-9679-c53d8b0ec16c) |

## What was observed on a clean machine

Attempt 1:

- `Syslog not available in container causes TestSysLogger failure`

Attempt 2:

- 3 min: `go was not installed; go version failed with 'go: not found'`
- 1 min: `/work/toolchains was not writable`
- 2 min: `the shell lacked the time and nc utilities, so initial probes aborted`
- 7 min: `logger tests failed with 'Unix syslog delivery error' because local syslog sockets are absent`
- 18 min: `server/pse TestPSEmulationMem failed RSS comparison at about 3.17 MB versus 4.7-5.4 MB`
- 7 min: `OCSP must-staple tests expected nats.ErrNoServers but received 'dial tcp [::1]: connect: cannot assign requested address'`
- 25 min: `go test ./... exited 1 after the server package hit its 20m timeout; a 45m ./server run reported three JetStream cluster failures and timed out; ServiceLatencySingleServerConnect failed once`
- 1 min: `a final launch initially failed because monitor port 68222 exceeds 65535`
- 1 min: `a parallel launch probe raced the rebuild and reported nats-server-final: not found`
- 1 min: `a temporary end-to-end probe did not compile because nats.Timeout is not a nats.JSOpt`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
