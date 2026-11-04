# SnowAir

**Verdict: could not verify.** Argusic Score 6 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/CM-idea/SnowAir, licensed Apache-2.0, written in C++.

Evidence and recordings: https://argusic.com/subject/snowair

## Pinned environment

- Project commit: `4709d49e778341de7380765bace594f0a83fc627`
- Test commit: `4709d49e778341de7380765bace594f0a83fc627`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 8.7 to 26 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 12 | 12 | 8.7 | 5 | 3 | [run](https://argusic.com/run/007cd229-1cfd-474e-aee0-e1baaf570cdc) |
| 2 | fail | 0 | 0 | 26 | 2 | 0 | [run](https://argusic.com/run/9fcc0f18-21dc-41c3-85e6-9a9110597ad8) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `A standard source build is impossible: Native/SnowAir.slnx references Native/deps/Ling, Yoga, libwebp, and zxing-cpp-311, but Native/deps is absent; the READMEs state the required custom Ling implementation is unpublished.`
- 1 min: `Downloading into /work/downloads failed with Permission denied.`
- 2 min: `Portable Wine 11.21 amd64 failed with /lib/ld-linux.so.2: could not open because the container lacks the 32-bit loader.`
- 5 min: `Wine prefix initialization timed out while wineboot/rundll32 remained hung after RpcSs failed to start.`
- 3 min: `The official GUI exits with status 9: RoGetActivationFactory cannot find Windows.System.DispatcherQueue, followed by unhandled exception c0000409.`

Attempt 2:

- `Source requires Visual Studio 2026, the proprietary Ling framework (explicitly not published in the repo), and the Microsoft WinRT runtime; none are available on Linux, so the project cannot be compiled from source.`
- `Under Wine 11.21 all GUI launch modes abort because Wine lacks real implementations of WinRT Windows.System.DispatcherQueue (CLASS_E_CLASSNOTAVAILABLE 0x80040111) and Windows.UI.Composition.Compositor (class not registered), which the Ling-`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
