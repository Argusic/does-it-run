# VoiceFlow

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/infiniV/VoiceFlow, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/voiceflow

## Pinned environment

- Project commit: `f63609a50da3e58a80701b96295d4bf863113f23`
- Test commit: `f63609a50da3e58a80701b96295d4bf863113f23`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 22.5 to 22.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 22 | 22.5 | 5 | 5 | [run](https://argusic.com/run/1187eb48-6414-40b2-bb93-5ee3492c32fd) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `pnpm 12.x requires onlyBuiltDependencies in pnpm-workspace.yaml (esbuild, pnpm)`
- 3 min: `evdev C extension build fails: Python.h not found (libpython3.12-dev headers missing)`
- 2 min: `PortAudio library missing - sounddevice cannot import`
- 5 min: `@tailwindcss/oxide-linux-x64-gnu native binding requires Node >= 20 but system has Node 18`
- 1 min: `pyperclip clipboard fails - xclip not installed`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
