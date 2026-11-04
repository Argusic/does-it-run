# claude-skills

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Jeffallan/claude-skills, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/claude-skills

## Pinned environment

- Project commit: `882ef55e377dbf9a4dbe496bb41ac6ccd0e555cf`
- Test commit: `882ef55e377dbf9a4dbe496bb41ac6ccd0e555cf`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 6.1 to 18.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 7 | 6.1 | 5 | 5 | [run](https://argusic.com/run/71b39742-8965-497e-bccd-f6ca1d1e7aca) |
| 2 | pass with mocks | 92 | 17 | 18.4 | 10 | 10 | [run](https://argusic.com/run/80a940e0-0fbb-4bb1-bf5b-b8cc6abd702a) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `python command not found; Makefile and test script used bare python`
- 1 min: `pyyaml not installed; validate-skills.py fell back to broken simple parser producing 17 false errors`
- 1 min: `pyright and ruff not on PATH`
- 2 min: `site/scripts/sync-content.mjs uses import.meta.dirname (Node 21+) but container has Node 18`
- 1 min: `astro requires Node >=20 but container ships Node 18`

Attempt 2:

- `/usr/bin/time was not installed, so the first timing attempt exited 127 before project code ran.`
- 2 min: `make test exited 2 because the Makefile and test script required a python command that does not exist in this container.`
- 2 min: `pip install --user pyyaml was rejected by the externally managed Python environment (PEP 668).`
- 2 min: `npm run build exited 1 because import.meta.dirname was undefined under Node.js 18.19.1.`
- 2 min: `Astro refused to start because Node.js 18.19.1 is below its minimum supported version of 18.20.8.`
- 3 min: `The documented install fullstack-dev-skills@jeffallan failed because the marketplace is named fullstack-dev-skills, not jeffallan.`
- 2 min: `npm run lint exited 1 after checking 97 generated Markdown files.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
