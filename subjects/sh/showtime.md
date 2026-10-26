# showtime

**Verdict: runs.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/FavioVazquez/showtime, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/showtime

## Pinned environment

- Project commit: `95c2394bf3e74dd7a51e44eeaa6b87cce387cb76`
- Test commit: `95c2394bf3e74dd7a51e44eeaa6b87cce387cb76`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 57.8 to 57.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 92 | 3 | 57.8 | 5 | 3 | [run](https://argusic.com/run/85dc2d0d-b146-467e-94b0-0c9512287d00) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Missing uv (Python package manager)`
- 1 min: `Node.js 18 too old (needs 20+)`
- 2 min: `System ffmpeg 6.1.1 caused test_cards.py failure (ffmpeg overlay filter with setpts+trim + between)`
- `test_highlights.py: test asserts os.cpu_count()//4 (192//4=48) but app uses sched_getaffinity (4) -> 1 worker`
- `test_render_speed.py: workers_why includes "; memory limit 7.5 GB of 755.0 GB" on 755 GB RAM machine`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
