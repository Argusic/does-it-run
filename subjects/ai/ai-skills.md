# ai-skills

**Verdict: runs with mocks.** Argusic Score 86.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/sanjay3290/ai-skills, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/ai-skills

## Pinned environment

- Project commit: `281d88df199357e3091a3be5c743a0fca9a9ae1b`
- Test commit: `281d88df199357e3091a3be5c743a0fca9a9ae1b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 40.5 to 40.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 86.29 | 5 | 40.5 | 7 | 5 | [run](https://argusic.com/run/74f9b7a2-6a16-4ee0-bc89-cdc7365d0c1b) |

## What was observed on a clean machine

Attempt 1:

- 18 min: `pymssql TDS wire mock: login accepted by FreeTDS but token stream rejected (189-20002 errors), no real SQL Server in container`
- 10 min: `repo test binary uses /usr/bin/python3 without project deps; smoke test crashed importing playwright`
- 25 min: `outline.py crashed on real API payload shape (documents.search/collections.list/list.documents data nesting, auth.info team shape)`
- 6 min: `no DB servers inside container; postgres/mysql/mssql scripts need real servers`
- 3 min: `notebooklm smoke required playwright chromium binary per README`
- `MSSQL/Postgres/MySQL real over-the-wire queries could not be verified; Docker/podman absent and system packages blocked; only mssql mock was attempted and it failed persistently`
- 12 min: `hero network TLS: eleven/google-tts terminals hardcoded real hostnames; verified via env-overridable base URLs + local mocks (audio mp3 decoded clean with ffmpeg)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
