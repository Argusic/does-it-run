# copperhead

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/copperheadhq/copperhead, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/copperhead

## Pinned environment

- Project commit: `e26be947ed31a35fbbb52623174bb25017d6cd44`
- Test commit: `e26be947ed31a35fbbb52623174bb25017d6cd44`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 31 to 31 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 68 | 31 | 3 | 3 | [run](https://argusic.com/run/de27ee7b-fed0-46e5-a7a8-7e070e61460d) |

## What was observed on a clean machine

Attempt 1:

- `Node.js v18.19.1 installed but project requires ≥20. Install and typecheck/build succeed with engine warnings.`
- `kicad-cli binary not on PATH. Created mock kicad-cli at /home/runner/bin/kicad-cli that handles version, ERC/DRC reporting, netlist export, load probing, and fab export by returning well-formed empty results.`
- `5 test files / 4 tests fail because they require real KiCad stock footprint libraries and real ERC analysis: board-populate (suite crash, 44 skipped), create-layout-draft (suite crash, all skipped), create-footprints (1 test), draft-ir-bom`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
