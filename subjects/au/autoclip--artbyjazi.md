# autoclip

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/artbyjazi/autoclip, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/run/c5a81a83-22fb-462a-907f-b023f6b5b478

## Pinned environment

- Project commit: `5d0eac36fa615b79dd2104083bf273a96f8d68bb`
- Test commit: `5d0eac36fa615b79dd2104083bf273a96f8d68bb`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4.5 to 4.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 4.5 | 3 | 3 | [run](https://argusic.com/run/c5a81a83-22fb-462a-907f-b023f6b5b478) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `pyproject marked externally managed; system pip refused install`
- 4 min: `System Node 18 made npm install skip @tailwindcss/oxide native binding, so 'npm run build' failed with 'Cannot find native binding'`
- 1 min: `Background autoclip serve via nohup was killed when the shell exited`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
