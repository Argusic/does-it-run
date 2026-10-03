# Strata

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Niko1221/Strata, licensed MIT, written in C++.

Evidence and recordings: https://argusic.com/subject/strata

## Pinned environment

- Project commit: `1678de333d0e0711bc414ad992b640e1a37dd814`
- Test commit: `1678de333d0e0711bc414ad992b640e1a37dd814`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 27.4 to 27.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0 | 27.4 | 2 | 2 | [run](https://argusic.com/run/9e14c2a0-9bcf-4b05-a162-f24e3a8c2a57) |

## What was observed on a clean machine

Attempt 1:

- `AMD test hardcoded 'strata.exe' which fails on Linux where setup.EXE='strata'`
- `Golden tests failed: normalize() replaced setup.EXE in log paths changing 'strata-iq3_xxs.log' to '<EXE>-iq3_xxs.log', and Enter-only test hit risk warnings for Unsloth UD-Q4_K_XL on low-RAM PCs`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
