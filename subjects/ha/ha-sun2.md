# ha-sun2

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/pnbruckner/ha-sun2, licensed Unlicense, written in Python.

Evidence and recordings: https://argusic.com/subject/ha-sun2

## Pinned environment

- Project commit: `eef7ccf7a7a7cd199e141394c1ea8480a5901f3b`
- Test commit: `eef7ccf7a7a7cd199e141394c1ea8480a5901f3b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 10.7 to 10.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 10.7 | 3 | 3 | [run](https://argusic.com/run/2dc52ac4-f91f-46cb-97c1-27eb134504dd) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `pip install homeassistant blocked by externally-managed-environment`
- 5 min: `pyspeex-noise==1.0.2 C extension build fails (missing Python.h) - unrelated to sun2 component`
- `netifaces==0.11.0 / aiodiscover==2.1.0 build fails (missing Python.h) - unrelated to sun2 component`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
