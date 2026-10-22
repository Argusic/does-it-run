# Ominis-OSINT

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/AnonCatalyst/Ominis-OSINT, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/ominis-osint

## Pinned environment

- Project commit: `35f24e581dca55f26f956112b9ecaf512109750c`
- Test commit: `35f24e581dca55f26f956112b9ecaf512109750c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 10.3 to 10.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 10.3 | 1 | 1 | [run](https://argusic.com/run/28b59c26-34b6-4985-9e1c-dc65dbd40ec2) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `ominis.py line 124 hardcoded absolute Python path /home/ant/.local/share/pipx/venvs/ominis-osint/bin/python which does not exist in container environment`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
