# omnara

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/omnara-ai/omnara, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/omnara

## Pinned environment

- Project commit: `7435b5995514d137189652fd47e82fcfeb33500e`
- Test commit: `7435b5995514d137189652fd47e82fcfeb33500e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 43.4 to 56.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 55 | 56.9 | 0 | 0 | [run](https://argusic.com/run/6947485e-358c-4ac5-8559-5e9cabed2d7a) |
| 2 | pass | 100 | 35 | 43.4 | 1 | 1 | [run](https://argusic.com/run/c1d979ea-5460-4166-bc46-42e1b151cd98) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `go test ./internal/emailaddr/ failed: TestNormalize/capital_sharp_s_maps_per_UTS_46 expected user@strasse.de but got user@xn--strae-oqa.de`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
