# ruby-progressbar

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/jfelchner/ruby-progressbar, licensed MIT, written in Ruby.

Evidence and recordings: https://argusic.com/subject/ruby-progressbar

## Pinned environment

- Project commit: `bafa278bfb14353282c2ae3207060f69615db7ae`
- Test commit: `bafa278bfb14353282c2ae3207060f69615db7ae`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 11.7 to 11.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 18 | 11.7 | 3 | 3 | [run](https://argusic.com/run/259bbe90-676b-42ce-ae51-f34f735eba7f) |

## What was observed on a clean machine

Attempt 1:

- 12 min: `Ruby 3.4.8 not installed in container`
- 3 min: `zlib development headers missing (needed by Ruby's zlib extension)`
- 3 min: `libyaml development headers missing (needed by Ruby's psych extension)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
