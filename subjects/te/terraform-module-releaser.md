# terraform-module-releaser

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/techpivot/terraform-module-releaser, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/terraform-module-releaser

## Pinned environment

- Project commit: `5260b01ca93bf6b56a05ea623f99bcd95be8667e`
- Test commit: `5260b01ca93bf6b56a05ea623f99bcd95be8667e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 4.1 to 4.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 3.5 | 4.1 | 3 | 3 | [run](https://argusic.com/run/efd0dc67-7754-49ba-86d2-c97d7abdb524) |

## What was observed on a clean machine

Attempt 1:

- 1.5 min: `Container has Node 18 but project requires Node >=24. Downloaded Node 24 binary and used it via PATH override.`
- 1 min: `installTerraformDocs() hardcodes sudo to install terraform-docs to /usr/local/bin, but sudo is not available in the container.`
- 0.5 min: `terraform-docs binary not pre-installed. Tests that exercise terraform-docs generation fail without it.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
