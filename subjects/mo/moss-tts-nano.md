# MOSS-TTS-Nano

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/OpenMOSS/MOSS-TTS-Nano, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/moss-tts-nano

## Pinned environment

- Project commit: `8b7bcc9341b3b4ef3a3a58ba1338a7d85ff133eb`
- Test commit: `8b7bcc9341b3b4ef3a3a58ba1338a7d85ff133eb`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 15.8 to 33.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 15.8 | 0 | 0 | [run](https://argusic.com/run/abe639dc-a9a3-4270-a053-54610793642c) |
| 2 | pass | 100 | 8 | 33.5 | 3 | 3 | [run](https://argusic.com/run/a4eff959-5c92-4a3a-aaeb-407e2e15cfbf) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `System python3 externally managed; pip install -e failed directly`
- 0.5 min: `WeTextProcessing top_level.txt lists itn/tn modules not WeTextProcessing package name`
- 0.5 min: `Web server index page crashes with AttributeError when warmup_manager=None`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
