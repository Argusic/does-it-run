# rats-search

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/librats/rats-search, licensed MIT, written in C++.

Evidence and recordings: https://argusic.com/subject/rats-search

## Pinned environment

- Project commit: `29b5c64f8e4e9e17017d6188845c90bac1d4182b`
- Test commit: `29b5c64f8e4e9e17017d6188845c90bac1d4182b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 9.4 to 9.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 9.4 | 1 | 1 | [run](https://argusic.com/run/dab1ad00-2209-4000-b65a-cb6b2bfdf958) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Qt6 development packages (qt6-base-dev, qt6-websockets-dev, qt6-base-dev-tools, qmake6, qt6-l10n-tools, qt6-tools-dev, linguist-qt6, libxkbcommon-dev, libproxy1v5/libproxy-dev, libduktape207, libqt6sql6-mysql, libqt6test6t64) not installed`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
