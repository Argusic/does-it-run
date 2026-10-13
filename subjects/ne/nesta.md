# nesta

**Verdict: runs.** Argusic Score 93.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/gma/nesta, licensed MIT, written in Ruby.

Evidence and recordings: https://argusic.com/subject/nesta

## Pinned environment

- Project commit: `8597b9a3854b651416f6e386739983093011cee9`
- Test commit: `8597b9a3854b651416f6e386739983093011cee9`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 9.7 to 9.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 93.33 | 8 | 9.7 | 3 | 2 | [run](https://argusic.com/run/c8459dd4-b46d-4d2a-8c7e-cae211a57948) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Ruby not installed in container`
- 2 min: `bundle install failed building native extensions (RedCloth, rdiscount) due to missing libruby-3.2.so linker symlink and missing ruby-dev headers`
- 1 min: `nesta build command fails with Tilt::MarukuTemplate NameError in haml-contrib gem`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
