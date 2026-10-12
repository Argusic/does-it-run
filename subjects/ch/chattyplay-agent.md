# ChattyPlay-Agent

**Verdict: runs.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/P1kaj1uu/ChattyPlay-Agent, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/chattyplay-agent

## Pinned environment

- Project commit: `1f248cb5ae399b366bd0e9b5f41cbdbbf30a0a2a`
- Test commit: `1f248cb5ae399b366bd0e9b5f41cbdbbf30a0a2a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 6.1 to 10.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 1 | 6.1 | 0 | 0 | [run](https://argusic.com/run/6d0c94b9-e98e-4619-be0f-85aca6698ad7) |
| 2 | pass | 80 | 5 | 10.2 | 3 | 0 | [run](https://argusic.com/run/3d259542-5230-42af-9d37-a4885a3a252d) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `npm run lint fails: 'ESLint couldn't find a configuration file' - the repo ships no .eslintrc* or eslint.config.* file`
- `Node engine (EBADENGINE) warnings: pdfjs-dist@5.6.205 and marked require node>=20 while container has node v18.19.1; install and build still completed`
- `vite preview tried to spawn xdg-open (ENOENT, no browser in container); non-fatal, preview still served HTTP 200`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
