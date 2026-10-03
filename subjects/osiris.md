# osiris

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/simplifaisoul/osiris, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/osiris

## Pinned environment

- Project commit: `954dbc9c39cfb8683e3ad99ee9da3947cb99d724`
- Test commit: `954dbc9c39cfb8683e3ad99ee9da3947cb99d724`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 8.2 to 8.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 8.2 | 2 | 2 | [run](https://argusic.com/run/482f15b8-0b5a-4854-b643-e769db7b8b62) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `PostCSS native binding @tailwindcss/oxide not found , npm failed to install the optional native binary for linux-x64-gnu`
- 5 min: `Build failed because Node.js 18.19.1 is too old for Next.js 16.3.4 (requires >=20.9.0)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
