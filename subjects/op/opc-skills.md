# opc-skills

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ReScienceLab/opc-skills, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/opc-skills

## Pinned environment

- Project commit: `af31273aa82606e42cf5b265c9033eb15e48b9e7`
- Test commit: `af31273aa82606e42cf5b265c9033eb15e48b9e7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 23.9 to 23.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 90 | 26 | 23.9 | 4 | 2 | [run](https://argusic.com/run/d6defdad-f9cc-4ac6-a80a-92027a25d7f5) |

## What was observed on a clean machine

Attempt 1:

- 18 min: `Reddit www.reddit.com JSON returned HTTP 403 (Blocked) for all reddit skill scripts`
- 8 min: `Installer npx skills add failed with SyntaxError on node:util styleText under system Node 18.19.1`
- 3 min: `website/package.json defines no lint/typecheck/test/build scripts though docs list them`
- 1 min: `scripts/create-blog.py validate reports 4 pre-existing missing 'schema' errors in 2 blog posts`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
