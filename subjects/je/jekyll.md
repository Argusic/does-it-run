# jekyll

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/jekyll/jekyll, licensed MIT, written in Ruby.

Evidence and recordings: https://argusic.com/subject/jekyll

## Pinned environment

- Project commit: `541d8b2ee75c8907de4744d4b87a7a6f1f997cae`
- Test commit: `541d8b2ee75c8907de4744d4b87a7a6f1f997cae`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 25.2 to 25.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 25 | 25.2 | 2 | 2 | [run](https://argusic.com/run/3dd7a8ef-53d2-4642-abd2-6fc8c44c426d) |

## What was observed on a clean machine

Attempt 1:

- 12 min: `Ruby not installed in container (no root). Built Ruby 3.3.5 from source via ruby-build.`
- 8 min: `First ruby-build attempt failed due to missing libffi, zlib, and psych/yaml dependencies.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
