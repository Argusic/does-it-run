# ai-promo-video-maker

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/liyupi/ai-promo-video-maker, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/ai-promo-video-maker

## Pinned environment

- Project commit: `279ba5178c3c80d472b84ac2efa36c6fca33bba2`
- Test commit: `279ba5178c3c80d472b84ac2efa36c6fca33bba2`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 9.6 to 9.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 9 | 9.6 | 5 | 5 | [run](https://argusic.com/run/a07284a8-c33d-4faf-9b24-3f94457c8e08) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Python deps not installed in system python (externally-managed-environment)`
- 3 min: `No CJK fonts on Linux container`
- 2 min: `@tailwindcss/oxide v4 has no x86_64-glibc binary (only musl), breaks Remotion bundling`
- `Remotion concurrency set to 12 on 4-core container`
- `Missing public/audio/mix.wav blocks render`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
