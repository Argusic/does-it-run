# thumbsup

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/thumbsup/thumbsup, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/thumbsup

## Pinned environment

- Project commit: `6c6cba0dc812640e1dce2f25f4d8f2786a6eee7d`
- Test commit: `6c6cba0dc812640e1dce2f25f4d8f2786a6eee7d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 11.2 to 11.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1 | 11.2 | 2 | 2 | [run](https://argusic.com/run/456113e9-f392-47e0-a1c7-240a0c7d38ca) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `Missing mandatory binary: exiftool - a prior cpan build left the script at /home/runner/perl5/bin/exiftool but it couldn't find its perl libs`
- 2 min: `Missing mandatory binary: gm (GraphicsMagick) - not installed, but ImageMagick's convert is available`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
