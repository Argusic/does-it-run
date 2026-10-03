# musicxx

**Verdict: could not verify.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/coolight7/musicxx, licensed MIT, written in C++.

Evidence and recordings: https://argusic.com/subject/musicxx

## Pinned environment

- Project commit: `4b69709d820c4ee2a4868c8878054eb91db3278b`
- Test commit: `4b69709d820c4ee2a4868c8878054eb91db3278b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 11.4 to 24.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 24 | 24.7 | 9 | 9 | [run](https://argusic.com/run/8601dbfd-da27-4d59-a107-b2ff5d00b86c) |
| 2 | fail | 80 | 26 | 11.4 | 3 | 3 | [run](https://argusic.com/run/efeaa96f-3eec-4649-a5a8-fbdf03d8d24a) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `vcpkg bootstrap requires zip/unzip (not installed, no root access)`
- 6 min: `Header dependencies (fmt, spdlog, nlohmann-json, jwt-cpp) not found on system`
- 5 min: `workflow library not present in mylib/`
- 2 min: `CMake could not find fmt, spdlog, nlohmann_json targets`
- 1 min: `nlohmann/json.hpp include not found (header at json.hpp not nlohmann/json.hpp)`
- 1 min: `JWT_CPP_INCLUDE_DIRS undefined`
- 3 min: `myMusic/user/User.h (and lyric/LyricDB.h, song/SongDB.h) missing from checkout`
- 1 min: `MyMServiceWorkBase.h uses MySqlTask_c but does not include MySqlTask.h`
- 1 min: `UserJWT_c stub missing 'aud' member`

Attempt 2:

- 1 min: `Missing find_package(fmt REQUIRED) in src/myServer/CMakeLists.txt caused cmake configure failure`
- 1 min: `Missing source files myMusic/user/User.h and myMusic/lyric/LyricDB.h blocked myMusic target compilation`
- 1 min: `Missing #include 'myServer/MySqlTask.h' in MyMServiceWorkBase.h caused compilation errors (MySqlTask_c not declared)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
