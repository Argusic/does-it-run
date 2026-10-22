# pyosmium

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/osmcode/pyosmium, licensed BSD-2-Clause, written in Python.

Evidence and recordings: https://argusic.com/subject/pyosmium

## Pinned environment

- Project commit: `c4f1ae41f56978b691e738133ab69fedc4a277d8`
- Test commit: `c4f1ae41f56978b691e738133ab69fedc4a277d8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 20.4 to 20.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 22 | 20.4 | 2 | 2 | [run](https://argusic.com/run/19facaf0-2b68-4b40-9f05-5c964617d427) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `CMake could not find Python Development.Module: /usr/include/python3.12 missing (python3-dev not installed)`
- 3 min: `Linker failed on static libs (libz.a, libbz2.a) not compiled with -fPIC when building shared modules`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
