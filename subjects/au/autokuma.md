# AutoKuma

**Verdict: could not verify.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/BigBoot/AutoKuma, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/autokuma

## Pinned environment

- Project commit: `1cba1f0e12ce001b115f93507130059f35a6613e`
- Test commit: `1cba1f0e12ce001b115f93507130059f35a6613e`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 4; wall time 6.7 to 87.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 12 | 23.6 | 1 | 1 | [run](https://argusic.com/run/78b67556-6f1c-43e4-bdf9-11bed130295d) |
| 1 | fail | 80 | 3.5 | 6.7 | 1 | 1 | [run](https://argusic.com/run/8e3901d8-1447-4e5a-9bd3-7549c02bc61d) |
| 2 | timeout | none | 49 | 49.5 | 4 | 4 | [run](https://argusic.com/run/06437a9a-4df3-4552-9681-f061e9c97dd7) |
| 2 | timeout | none | n/a | 87.2 | 0 | 0 | [run](https://argusic.com/run/49d2af0e-7526-400c-ae1b-c4d0924e84cf) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Doctest in kuma-client/src/client.rs failed to compile (missing imports, await outside async fn)`

Attempt 1:

- 2 min: `kuma-client/src/client.rs doctest had async code in a non-async context, referencing types not imported in the doctest scope (Client, Config, Url, TagDefinition, MonitorGroup, Tag, Notification, MonitorHttp)`

Attempt 2:

- 30 min: `No C compiler (cc/gcc) installed in container`
- 5 min: `No pkg-config installed`
- 7 min: `Missing kernel and glibc C/C++ headers`
- 5 min: `lld linker could not find pthread_atfork symbol`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
