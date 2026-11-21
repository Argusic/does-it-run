# CORAL

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Human-Agent-Society/CORAL, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/coral

## Pinned environment

- Project commit: `0123dfb939b35228cf2c1fde224cd0561e727408`
- Test commit: `0123dfb939b35228cf2c1fde224cd0561e727408`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 19.8 to 21.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 21.2 | 3 | 3 | [run](https://argusic.com/run/211bc8b3-64c3-409a-9ed0-a78b2457da26) |
| 2 | pass | 100 | 5 | 19.8 | 2 | 2 | [run](https://argusic.com/run/37e240e4-e567-48d9-9430-08ee8d6464ee) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Missing tmux binary , 'has_tmux()' returned True for monkeypatched tests but the two tests calling _start_in_tmux/subprocess.run(['tmux',...]) failed with FileNotFoundError`
- 7 min: `Node.js 18.19.1 too old for Vite 8 / Tailwind 4 native bindings; web build failed (rolldown, @tailwindcss/oxide both missing linux-x64-gnu optional deps)`
- `test_distribution_version_is_based_on_latest_reachable_release_tag , requires a git tag reachable from HEAD; this FETCH_HEAD checkout has none`

Attempt 2:

- 10 min: `tmux binary not available in container , test tried to spawn ['tmux', 'display-message', '-p', '#S'] as a subprocess and got FileNotFoundError`
- 5 min: `test_distribution_version_is_based_on_latest_reachable_release_tag failed , git describe couldn't find any tags reachable from HEAD (shallow clone)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
