# sigal

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/saimn/sigal, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/sigal

## Pinned environment

- Project commit: `5dff40d4c1734b215e7c1b8ea442818c416806cc`
- Test commit: `5dff40d4c1734b215e7c1b8ea442818c416806cc`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 9.7 to 9.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 4 | 9.7 | 1 | 1 | [run](https://argusic.com/run/4f516e9a-1e79-4477-925f-303e12d4bca4) |

## What was observed on a clean machine

Attempt 1:

- 20 min: `sigal build crashed with jinja2 UndefinedError 'list object has no element 0' rendering galleria album.html for a media-less album (.venv/lib64) after its only file failed to decode`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
