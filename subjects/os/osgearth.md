# osgearth

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/pelicanmapping/osgearth, licensed MIT, written in C.

Evidence and recordings: https://argusic.com/subject/osgearth

## Pinned environment

- Project commit: `59f16569ec4de5f768ef0a8831480dc96662f5cf`
- Test commit: `59f16569ec4de5f768ef0a8831480dc96662f5cf`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 73 to 73 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 76 | 73 | 7 | 7 | [run](https://argusic.com/run/60593fda-7b3f-4dfa-90d8-c99b1ce04be0) |

## What was observed on a clean machine

Attempt 1:

- 30 min: `CMake could not find OpenGL, X11, and other system -dev packages because libgl-dev and other -dev packages were not installed in the container`
- 10 min: `Broken symlinks in extracted sysroot .deb files blocked linking`
- 5 min: `Static libsqlite3.a from -dev package not compiled with -fPIC, could not link into shared library`
- 15 min: `GDAL system library links to many optional plugin libraries not available in container`
- 5 min: `ExpressionTests.cpp failed to compile: evaluateExpression() function not found at template instantiation point`
- 3 min: `libprotoc.so.32 missing for protoc compiler used by protobuf_generate_cpp()`
- `Some test cases fail due to disabled components (script engine, gltf plugin) and Windows-specific path expectations`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
