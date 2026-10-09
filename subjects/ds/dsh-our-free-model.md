# dsh-our-free-model

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Ebony-Vinyl/dsh-our-free-model, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/dsh-our-free-model

## Pinned environment

- Project commit: `de28949bf73627aa8f746f3ebf98ac77adecd7a1`
- Test commit: `de28949bf73627aa8f746f3ebf98ac77adecd7a1`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 16.2 to 16.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 16.2 | 2 | 2 | [run](https://argusic.com/run/569d4478-3113-4411-888e-7a8184e921b3) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Node.js v18.19.1 too old (requires ^22.19.0 or >=24.0.0)`
- 2 min: `catalog/dsh-plugin.json and catalog/provenance.json sourceRevision pointed at commit 4d31dc8 which does not exist in the squashed clone`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
