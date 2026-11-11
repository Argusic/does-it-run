# erda

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/erda-project/erda, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/erda

## Pinned environment

- Project commit: `7195c3a774d577783ab834c60cb0a6480ba0300d`
- Test commit: `7195c3a774d577783ab834c60cb0a6480ba0300d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 23.1 to 38.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 39 | 38.9 | 3 | 3 | [run](https://argusic.com/run/126e2741-6509-4991-ac88-78a1fbea086f) |
| 2 | pass | 100 | 23 | 23.1 | 7 | 7 | [run](https://argusic.com/run/1071d099-c084-4916-b40c-efa2f36af397) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `Go not installed in the container (go: not found)`
- 12 min: `erda-proto-go v1.4.0 local replace directory api/proto-go had 0 generated .go files, causing 'no required module provides package' on all erda-proto-go imports`
- 5 min: `erda-proto-go's dependency chain includes 'github.com/coreos/bbolt@v0.0.0-00010101000000-000000000000: invalid version: unknown revision 000000000000' from an old erda-infra, preventing resolution of nearly all packages`

Attempt 2:

- 4 min: `Go not installed in container`
- 7 min: `api/proto-go module empty - no generated Go code from protos`
- 2 min: `golang/protobuf v1.5.2 incompatible with google.golang.org/protobuf v1.34.2 (Default_FileOptions_PhpGenericServices undefined)`
- 1 min: `api/proto-go generated client files reference wrong import paths (hub_info, templates)`
- 4 min: `Go 1.24 vet rejects non-constant format string in fmt.Printf/logrus.Errorf/errors.Errorf (5 source files)`
- 1 min: `oap/collector/receiver/opentelemetry proto missing external dependency (opentelemetry/proto/metrics)`
- 1 min: `Build requires generated CLI command package (tools/cli/generated_cmd)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
