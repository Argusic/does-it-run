# grist-static

**Verdict: runs.** Argusic Score 56 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/gristlabs/grist-static, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/grist-static

## Pinned environment

- Project commit: `e4aa8369de0229edba33058c9afe1c56e3a7adca`
- Test commit: `e4aa8369de0229edba33058c9afe1c56e3a7adca`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 13 to 28.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 28.6 | 0 | 0 | [run](https://argusic.com/run/85426cf4-88df-4304-81cc-97eb58090277) |
| 2 | pass | 92 | 9 | 13 | 5 | 3 | [run](https://argusic.com/run/9105a3db-688f-448d-a45a-f4a3c4eb4dd8) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `core submodule used SSH URL, no ssh binary; switched to HTTPS`
- 2 min: `Node 18.19.1 too old for core lockfile (needs >=20.17.0); then also needed >=22`
- 3 min: `yarn not available in PATH; npm global install blocked by permissions`
- `build_dist.sh uses rm -rf (rejected by policy); skipped final packaging step`
- `No Chrome/chromedriver in container; browser tests cannot run`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
