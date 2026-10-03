# skills

**Verdict: runs.** Argusic Score 85 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/browser-act/skills, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/run/65424f1f-7048-4b53-b2ae-77b93f8be507

## Pinned environment

- Project commit: `11c057b03f92101642cadc9f840564574120d184`
- Test commit: `11c057b03f92101642cadc9f840564574120d184`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 5.3 to 7.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 12 | 7.9 | 3 | 3 | [run](https://argusic.com/run/65424f1f-7048-4b53-b2ae-77b93f8be507) |
| 2 | pass | 90 | 6 | 5.3 | 6 | 3 | [run](https://argusic.com/run/0bd740fb-2706-4a9c-970c-daf389a749d2) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `pip3 install blocked by externally-managed-environment (PEP 668)`
- 1 min: `Skill handshake version mismatch blocked browser commands on first run`
- 2 min: `Chrome/Chromium not found for chrome-direct browser sessions`

Attempt 2:

- 0.5 min: `uv tool not found after pip install (PATH issue)`
- 0.5 min: `pip3 install uv blocked by externally-managed-environment`
- 2 min: `Skill version incompatible block: CLI refused all commands`
- 2 min: `auth set rejects API keys with server-side Invalid authorization`
- 2 min: `stealth-extract requires a BrowserAct API key (server-side validated, cannot mock)`
- 1 min: `chrome-direct type requires local Chrome installation (not available in container)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
