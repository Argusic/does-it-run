# 1JPM

**Verdict: runs.** Argusic Score 95 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Osiris-Team/1JPM, licensed MIT, written in Java.

Evidence and recordings: https://argusic.com/subject/1jpm

## Pinned environment

- Project commit: `b828b65790849f7d2c7eca82244b0b9e50e51cab`
- Test commit: `b828b65790849f7d2c7eca82244b0b9e50e51cab`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4.9 to 4.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 95 | 11 | 4.9 | 4 | 3 | [run](https://argusic.com/run/def113cd-8d61-4ecc-aeec-a9e8b915b0fa) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `No JDK or Maven installed in the container (no root to apt-get): 'java'/'javac'/'mvn' not found.`
- 4 min: `As-shipped, the README headline command 'java JPM.java' fails from repo root with 'Could not find or load main class JPM.java' because the 'drag-and-drop' JPM.java file is only shipped under src/main/java/com/mycompany/myproject/ in this te`
- 1 min: `Ran 'git checkout pom.xml' expecting to restore the committed pom and verify the tool's own regeneration; observed it rewrote the whole tree (removed JPM.java, .mvn/, mvnw), so I restored the committed pom and the fixed files.`
- 1 min: `repeated run of 'java JPM.java' from repo root`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
