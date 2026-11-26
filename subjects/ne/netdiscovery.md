# NetDiscovery

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/fengzhizi715/NetDiscovery, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/netdiscovery

## Pinned environment

- Project commit: `2d118210e8ef8d0bc0f6a51aeb04768e65aadb71`
- Test commit: `2d118210e8ef8d0bc0f6a51aeb04768e65aadb71`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 10.5 to 68.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 38 | 68.7 | 4 | 4 | [run](https://argusic.com/run/c9613841-e7a4-4a5c-a279-c22d23d6b15a) |
| 2 | pass | 100 | 10 | 10.5 | 5 | 5 | [run](https://argusic.com/run/6a31e037-e588-468a-9bf0-a3af00785344) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `JDK and Gradle not installed and system packages cannot be installed`
- 18 min: `JCenter/novoda bintray-release plugin and duplicate custom libs (hamal-context, proxypool, tony-common, rxcache, bytekit) unavailable from Central/JCenter/JitPack; build failed on dependency resolution`
- 7 min: `downloader:httpclient compile failed: missing Request/Response/HttpRequestBody symbols and undefined lombok version`
- 5 min: `Example runtime probes were answered, but spider downloads via VertxDownloader hid module activity; no module wiring existed for the downloader picker`

Attempt 2:

- 3 min: `No Java JDK installed in container`
- 3 min: `JCenter/Bintray repository is defunct; bintray-release and shadow buildscript deps unavailable`
- 2 min: `imageprocess module uses @Slf4j without Lombok annotation processor`
- 2 min: `downloader:httpclient missing imports for Request/Response Kotlin classes and uses Kotlin boolean getters (isDebug() -> getDebug())`
- 1 min: `RedirectStrategy.java accesses private log field in parent class`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
