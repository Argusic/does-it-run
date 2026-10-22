# Hydra

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/DragonKingpin/Hydra, licensed MIT, written in Java.

Evidence and recordings: https://argusic.com/subject/hydra

## Pinned environment

- Project commit: `6c537e4c868728085e8f095c05fae5031c172524`
- Test commit: `6c537e4c868728085e8f095c05fae5031c172524`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 8.9 to 8.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 9 | 8.9 | 3 | 3 | [run](https://argusic.com/run/879e2c82-d9ed-4a56-8509-b55fb86791c1) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Maven rejected the build: root pom.xml declared child modules in lowercase (pinecones, hydra, saurons, ...) but the actual directories are capitalized (Pinecones, Hydra, Saurons, ...); same mismatch for Pinecones submodules (pinecone/ulfhed`
- 2 min: `Compilation failed on JDK 17: lombok.javac.apt.LombokProcessor cannot access com.sun.tools.javac.processing because module jdk.compiler does not export it (Lombok 1.18.16 from Spring Boot 2.4.1 is incompatible with JDK 17).`
- 4 min: `Runtime crash launching ShadowBoot: NullPointerException 'this.mSubsystemConfig is null' at CentralMicroSystemCabinet.prepare_segment -> ArchSubsystemDirector.<init>; the code reads System.Subsystem from config.json5 but no Subsystem block`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
