# LiveStream-Agent-Studio

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/HanyuanWang/LiveStream-Agent-Studio, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/livestream-agent-studio

## Pinned environment

- Project commit: `1614dfa166f7eb34f5cd9e7c6231de48c5d423c0`
- Test commit: `1614dfa166f7eb34f5cd9e7c6231de48c5d423c0`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 26.6 to 26.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 27 | 26.6 | 7 | 7 | [run](https://argusic.com/run/df721664-aaf0-484a-8d41-a7fc108c61e9) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `System Node is v18 but project requires Node >=22.13`
- 4 min: `Python agent packages not importable for tests (src layout)`
- 2 min: `process_video_with_status.py hardcoded ALIYUN_OSS_ENDPOINT`
- 3 min: `config.py load_dotenv used setdefault so pre-set env overrode .env`
- 5 min: `Gateway /api/connections/verify ignored DASHSCOPE_BASE_URL and used GET models`
- 2 min: `Gateway configure did not persist DASHSCOPE_BASE_URL`
- 2 min: `Gateway retro submit assumed job_id key`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
