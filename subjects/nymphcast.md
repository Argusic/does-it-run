# NymphCast

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/MayaPosch/NymphCast, licensed BSD-3-Clause, written in C.

Evidence and recordings: https://argusic.com/subject/nymphcast

## Pinned environment

- Project commit: `82c14bb8176f881ef81c5c5fbfd1a72001609912`
- Test commit: `82c14bb8176f881ef81c5c5fbfd1a72001609912`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 23.7 to 23.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 50 | 23.7 | 7 | 7 | [run](https://argusic.com/run/297c4f81-efc0-4af4-912f-f0c07857a3d1) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Build dependencies not installed (no root): libsdl2-dev, libpoco-dev, libavcodec-dev, libfreetype-dev, libfreeimage-dev, etc.`
- 3 min: `NymphRPC shared library linking failed initially because Poco .so files lacked .so.80 symlinks`
- 2 min: `libnymphcast shared library linking failed because NymphRPC .a was not compiled with -fPIC`
- 2 min: `Server compilation failed: missing libavfilter/avfilter.h header`
- 3 min: `Server compilation failed: alsoundlib.h not found, GL/gl.h not found`
- 20 min: `Server linking failed: linker tried static .a archives which triggered long chain of transitive dependency errors`
- 5 min: `Server linking still fails: freeimage.a references libimath symbols (imath_half_to_float_table) from OpenEXR libimath-3-1 that cannot be linked without root or deeper dependency resolution`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
