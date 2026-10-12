# NaturalVoiceSAPIAdapter

**Verdict: could not verify.** Argusic Score 9.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/gexgd0419/NaturalVoiceSAPIAdapter, licensed MIT, written in C++.

Evidence and recordings: https://argusic.com/subject/naturalvoicesapiadapter

## Pinned environment

- Project commit: `7194eca5b78d8e477793c159d731d62b6357ffbf`
- Test commit: `7194eca5b78d8e477793c159d731d62b6357ffbf`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 20.3 to 27.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 6.67 | 44 | 27.9 | 3 | 1 | [run](https://argusic.com/run/89b3f057-3760-4f49-bcd5-c0273370bd32) |
| 2 | fail | 12 | 21 | 20.3 | 5 | 3 | [run](https://argusic.com/run/6a3e381d-42db-4b73-92fe-35835dc26de9) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `Cannot build from source: project requires Microsoft Visual Studio (MSBuild), NuGet, and Windows SDK headers , none available on this Linux system`
- `Cannot build submodules (AzureSpeechSDKShim, ttsapplication): same MSBuild/NuGet dependency`
- 34 min: `Release binaries exist and DLL registers under Wine 11.19, but TtsApplication.exe shows error dialog because Wine's built-in sapi.dll has stub implementations of spvoice_GetOutputStream and token_category_GetDefaultTokenId`

Attempt 2:

- 0.5 min: `Submodules not initialized`
- 5 min: `Wine not installed and cannot apt install (no root)`
- 5 min: `zlib1.dll missing , wine's user32.dll requires it at load time`
- `Cannot build from source , VC++ projects require MSBuild and Windows SDK (v143, Win10)`
- `x86 binaries not runnable , wine32 not available, only wine64 was extracted`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
