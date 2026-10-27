# Archimate-PlantUML

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/plantuml-stdlib/Archimate-PlantUML, licensed MIT, written in Shell.

Evidence and recordings: https://argusic.com/subject/archimate-plantuml

## Pinned environment

- Project commit: `12f7a140bdd4d9f82ec730b8ac51f2294e45f53e`
- Test commit: `12f7a140bdd4d9f82ec730b8ac51f2294e45f53e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 14.7 to 14.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 18 | 14.7 | 3 | 3 | [run](https://argusic.com/run/ce09d767-f2d5-468f-bc4d-2db8dcda038a) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `No Java runtime found in the container (no JRE/JDK binary on PATH)`
- 1 min: `Bundled npm plantuml@0.0.2 vendor jar (PlantUML 1.2022.7) is too old , the '?=' define operator in Archimate.puml is unsupported, producing error-page SVGs`
- `Graphviz (dot) not installed , PlantUML warns 'Dot executable does not exist'`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
