# arscontexta

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/agenticnotetaking/arscontexta, licensed MIT, written in Shell.

Evidence and recordings: https://argusic.com/subject/arscontexta

## Pinned environment

- Project commit: `2acfd5cc4473c4d06c46be63df748e77e00e2746`
- Test commit: `2acfd5cc4473c4d06c46be63df748e77e00e2746`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 15.1 to 15.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.5 | 15.1 | 1 | 1 | [run](https://argusic.com/run/38aee39c-5ff6-4ef6-8146-43f8746b6c5a) |

## What was observed on a clean machine

Attempt 1:

- 0.2 min: `SESS_COUNT assignment in hooks/scripts/session-orient.sh line 119 produced double output when grep returned exit code 1, causing 'integer expression expected' error`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
