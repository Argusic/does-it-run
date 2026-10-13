# agent-skills

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/oxylabs/agent-skills, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/agent-skills

## Pinned environment

- Project commit: `35eb7926ef2fc910916f5608587d08657e56d60a`
- Test commit: `35eb7926ef2fc910916f5608587d08657e56d60a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 7 to 7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 8 | 7 | 3 | 3 | [run](https://argusic.com/run/ae5b1e9c-34b7-4fff-8c50-e757fdddf988) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `npx skills requires Node >=22.20.0 but system had v18.19.1; skills CLI crashed with SyntaxError on node:util and node:zlib imports`
- 1 min: `.env.example used OXY_RESI_USERNAME/OXY_RESI_PASSWORD but all docs reference OXY_RES_USERNAME/OXY_RES_PASSWORD`
- 1 min: `pip3 install playwright blocked by PEP 668 system package protection`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
