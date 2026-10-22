# qmarkdowntextedit

**Verdict: could not verify.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/pbek/qmarkdowntextedit, licensed MIT, written in C++.

Evidence and recordings: https://argusic.com/subject/qmarkdowntextedit

## Pinned environment

- Project commit: `fe9e5703b735fad999747ec62468a8429b841957`
- Test commit: `fe9e5703b735fad999747ec62468a8429b841957`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 5.5 to 7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 5 | 5.5 | 3 | 3 | [run](https://argusic.com/run/0837cdb7-bf5d-4446-a795-4d4f0015c906) |
| 2 | fail | 80 | 7.1 | 7 | 3 | 3 | [run](https://argusic.com/run/bb9747f6-8569-488c-b26a-4520764e46f7) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Missing qt6-base-dev package (Qt 6 headers and cmake integration not installed)`
- 1 min: `cmake couldn't find OpenGL libraries because symlinks in prefix pointed to missing .so files`
- 1 min: `cmake couldn't find qmake binary referenced by Qt6CoreTools cmake targets`

Attempt 2:

- 5.2 min: `Missing Qt6 development packages (qt6-base-dev)`
- 0.5 min: `Missing versioned .so symlinks in extracted prefix`
- 1.1 min: `Missing OpenGL/GLX development files`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
