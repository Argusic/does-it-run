# bridgetown

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/bridgetownrb/bridgetown, licensed MIT, written in Ruby.

Evidence and recordings: https://argusic.com/subject/bridgetown

## Pinned environment

- Project commit: `250d6efe2b015af01707afbfcabc4bac270b4b55`
- Test commit: `250d6efe2b015af01707afbfcabc4bac270b4b55`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 16.5 to 16.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 15.05 | 16.5 | 4 | 4 | [run](https://argusic.com/run/f474d86f-1d7a-4e7c-9a28-449bdfadf123) |

## What was observed on a clean machine

Attempt 1:

- `Ruby not found in container (no ruby binary available)`
- `zlib extension missing in ruby build (libz dev headers not installed)`
- `psych extension missing (libyaml not available)`
- `bundle install failed because psych 5.2.6 gem native extension build failed`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
