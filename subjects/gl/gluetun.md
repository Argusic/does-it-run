# gluetun

**Verdict: runs.** Argusic Score 93.5 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/passteque/gluetun, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/gluetun

## Pinned environment

- Project commit: `1267bae7d4b3043957d931c0c3dc0bbd88737b8e`
- Test commit: `1267bae7d4b3043957d931c0c3dc0bbd88737b8e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 4.1 to 11.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 95 | 9 | 11.3 | 4 | 3 | [run](https://argusic.com/run/2179956a-b25d-4bc9-864b-d8b60efbbfd0) |
| 2 | pass with mocks | 92 | 2 | 4.1 | 1 | 1 | [run](https://argusic.com/run/a6dd7c24-0904-4ff5-a278-7707583b0bc0) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Go not found in PATH`
- 3 min: `DNS leak test failed: json: cannot unmarshal array into Go struct field ipLeakData.ip`
- 2 min: `golangci-lint not found`
- `54 test packages pass, 2 packages fail for missing Linux capabilities (CAP_NET_ADMIN, CAP_NET_RAW) - not fixable without root`

Attempt 2:

- `6 privilege-requiring tests fail without NET_ADMIN/netlink/raw socket capabilities in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
