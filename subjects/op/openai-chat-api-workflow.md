# openai-chat-api-workflow

**Verdict: could not verify.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/yohasebe/openai-chat-api-workflow, licensed MIT, written in Ruby.

Evidence and recordings: https://argusic.com/subject/openai-chat-api-workflow

## Pinned environment

- Project commit: `a75e903d086484bc429b92460fa70b82959c2a90`
- Test commit: `a75e903d086484bc429b92460fa70b82959c2a90`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 5.6 to 11.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 10 | 11.4 | 3 | 3 | [run](https://argusic.com/run/6cdef407-d537-4107-a2ca-69753bfeea55) |
| 2 | fail | 80 | 4 | 5.6 | 3 | 3 | [run](https://argusic.com/run/1fe61fe7-03eb-4357-9c04-1d8b3ca468ac) |

## What was observed on a clean machine

Attempt 1:

- 6 min: `Ruby not installed in environment`
- 2 min: `WEBrick gem not bundled with Ruby 3.3+`
- `test_openai_tts.rb: test_afplay_available fails - afplay is a macOS command`

Attempt 2:

- 3 min: `Ruby runtime not available in container - installed via Conda`
- 0.5 min: `WEBrick gem not available`
- `test_openai_tts.rb: test_afplay_available fails on Linux - afplay is macOS-only`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
