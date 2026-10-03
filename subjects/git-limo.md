# git.limo

**Verdict: runs.** Argusic Score 97.6 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/redrabbit/git.limo, licensed MIT, written in Elixir.

Evidence and recordings: https://argusic.com/subject/git-limo

## Pinned environment

- Project commit: `dd57207273586ebd5b5088921279b957ec42f995`
- Test commit: `dd57207273586ebd5b5088921279b957ec42f995`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 31.7 to 38.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 98 | 36 | 38.3 | 10 | 9 | [run](https://argusic.com/run/900ed811-2496-46b6-88b4-708dc65fe17c) |
| 2 | pass | 97.14 | 29 | 31.7 | 7 | 6 | [run](https://argusic.com/run/1d07817f-abc5-427b-bee2-9c9a07c90c57) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `Missing Erlang/OTP runtime`
- 2 min: `Missing Elixir runtime`
- 1 min: `ssl_verify_fun 1.1.6 fails to compile on Erlang 26`
- 1 min: `ecto 3.9.1 incompatible with Elixir 1.17 (dynamic type redefine)`
- 5 min: `libgit2 shared library not found`
- 2 min: `gitrekt C NIF missing libgit2 headers/zlib`
- 4 min: `PostgreSQL not available`
- 1 min: `npm install fails on @fortawesome/fontawesome-free Pro`
- 2 min: `ssh-keygen not found for SSH key generation`
- `2 test failures remain (relative time rendering, HTML escaping)`

Attempt 2:

- 2 min: `ssl_verify_fun 1.1.6 failed to compile with Erlang 27 (public_key.hrl not found)`
- 4 min: `ecto 3.9.1 defines dynamic/0 type which is built-in in Elixir 1.17`
- 8 min: `libgit2 not installed on system (no root)`
- 3 min: `gitrekt NIF compilation could not find erl_nif.h and git2.h`
- 2 min: `Ecto 3.13+ no longer accepts bare tuple preload syntax ({:repos, :maintainers})`
- 1 min: `SSH key test fails because ssh-keygen not in PATH`
- `scp test always fails because scp hardcodes /usr/bin/ssh path and no root to create symlink`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
