# middleman-blog

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/middleman/middleman-blog, licensed MIT, written in Ruby.

Evidence and recordings: https://argusic.com/subject/middleman-blog

## Pinned environment

- Project commit: `ce508ca38985f287b0e5273c56c849a70ce13205`
- Test commit: `ce508ca38985f287b0e5273c56c849a70ce13205`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4.9 to 4.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 4 | 4.9 | 3 | 3 | [run](https://argusic.com/run/90e76a47-bd37-4e6e-a97b-09c161aaaaf3) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Ruby not installed in container`
- 1 min: `libyaml shared library missing for psych.so`
- 1 min: `Cucumber 12 removed --strict flag; Rakefile used it in cucumber_opts`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
