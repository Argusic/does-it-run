# embyToLocalPlayer

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/kjtsune/embyToLocalPlayer, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/embytolocalplayer

## Pinned environment

- Project commit: `b4f9527519774ea6e9d91ebbe04ca892f41cb98b`
- Test commit: `b4f9527519774ea6e9d91ebbe04ca892f41cb98b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 7.2 to 7.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 8 | 7.2 | 3 | 3 | [run](https://argusic.com/run/16ac0d63-668b-4029-8298-ba6210076b15) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Missing 'requests' module (optional sync features)`
- 1 min: `SyntaxWarning: invalid escape sequence '\|' in utils/downloader.py:493`
- 1 min: `SyntaxWarning: invalid escape sequence '\=' in utils/net_tools.py:43`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
