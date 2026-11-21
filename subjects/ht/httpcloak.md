# httpcloak

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/sardanioss/httpcloak, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/httpcloak

## Pinned environment

- Project commit: `30379124605d212efe5240aacd60bd4b9ab7c6cf`
- Test commit: `30379124605d212efe5240aacd60bd4b9ab7c6cf`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 7 to 7.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 8 | 7.9 | 0 | 0 | [run](https://argusic.com/run/4607c01f-34c6-4be2-a6f4-63a095f2708c) |
| 2 | pass | 100 | 1 | 7 | 2 | 2 | [run](https://argusic.com/run/11cafdf1-6374-4088-ae2d-fb83775a55fd) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `Go compiler not found in container`
- 2 min: `go vet failures in 8 example files due to fmt.Println/fmt.Print with % directives in raw string literals`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
