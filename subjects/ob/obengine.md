# ObEngine

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ObEngine/ObEngine, licensed MIT, written in C++.

Evidence and recordings: https://argusic.com/subject/obengine

## Pinned environment

- Project commit: `932ad92df724caf202c0cf89d1f6dd393c1ff192`
- Test commit: `932ad92df724caf202c0cf89d1f6dd393c1ff192`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 17.9 to 37.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 37 | 37.2 | 4 | 4 | [run](https://argusic.com/run/60ee0c14-419a-4321-a3b0-7ae55454a670) |
| 2 | pass | 100 | 17 | 17.9 | 4 | 4 | [run](https://argusic.com/run/bd31ce50-8774-4409-a129-bcbb2562dd0a) |

## What was observed on a clean machine

Attempt 1:

- 18 min: `SFML and X11/OpenAL/GL dev dependencies absent (no root to apt install)`
- 6 min: `Bundled cppnet packet.hpp uses std::int8_t/etc without <cstdint> (GCC 13) - compile error`
- 10 min: `Deep -fPIC/static .a linking failures inside SFML build due to Ubuntu non-PIC static libs`
- 3 min: `Player named-project mount resolution finds no projects.vili when run per CMake layout`

Attempt 2:

- 2 min: `SFML 2.6 not installed (no root for apt)`
- 1 min: `ALSA not found (so loud backend)`
- 2 min: `cppnet/packet.hpp missing <cstdint> (GCC 13 strictness)`
- 1 min: `SFML graphics links libstb.so.0 at runtime`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
