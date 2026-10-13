# alchemy_cms

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/AlchemyCMS/alchemy_cms, licensed BSD-3-Clause, written in Ruby.

Evidence and recordings: https://argusic.com/subject/alchemy-cms

## Pinned environment

- Project commit: `a58097e6abacca7e0dab533a269bbccaa7877ae1`
- Test commit: `a58097e6abacca7e0dab533a269bbccaa7877ae1`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 69.4 to 69.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 62 | 69.4 | 5 | 5 | [run](https://argusic.com/run/96228c90-d167-45a5-a312-589690d89a7a) |

## What was observed on a clean machine

Attempt 1:

- 38 min: `No Ruby, Docker, pnpm, and only too-old Node 18 present in container`
- 15 min: `Ruby core extensions (psych/zlib/fiddle) failed to build: missing libyaml/zlib/libffi headers/libs and broken extension hdrdir resolution`
- 8 min: `Local openssl extension failed to recompile (ractor header mismatch) during make install of the first build tree`
- 4 min: `sqlite3/ruby-vips native gems initially had missing shared libraries`
- 2 min: `Development server returned HTTP 500 on first boot because dev DB was empty`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
