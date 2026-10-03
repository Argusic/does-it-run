# iotdb

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/apache/iotdb, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/iotdb

## Pinned environment

- Project commit: `25ab7941cebe6e14f396b5541cdd9daefae0f151`
- Test commit: `25ab7941cebe6e14f396b5541cdd9daefae0f151`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 41.1 to 76.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 43 | 44.1 | 5 | 5 | [run](https://argusic.com/run/1fd8efb9-1105-4945-99ae-5ac04764d037) |
| 2 | pass | 100 | 75 | 76.6 | 5 | 5 | [run](https://argusic.com/run/2512796c-2b87-4d2c-86a4-1052d06f8c6e) |
| 3 | pass | 100 | 37 | 41.1 | 4 | 4 | [run](https://argusic.com/run/73f3d61b-4d1a-4ffb-ad97-829791896842) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Java 17 not installed in container; mvnw could not run`
- 1 min: `Maven not installed; mvnw requires JAVA_HOME`
- 5 min: `Startup scripts could not find java because JAVA_HOME not in environment`
- 10 min: `EdgeNode crashed on first query attempt (default 224M heap + CrashOnOutOfMemoryError)`
- 1 min: `edge distribution lib did not contain org.apache.iotdb.cli.Cli class`

Attempt 2:

- 5 min: `No Java or Maven installed. Downloaded JDK 17 and Maven 3.9.6 manually.`
- 3 min: `Tsfile SNAPSHOT dependency (2.4.1-260806-SNAPSHOT) not in Maven Central. Added Apache snapshot repository to pom.xml so Maven can resolve it.`
- 8 min: `Gradle Enterprise extensions (in .mvn/) blocked build with connection timeouts to ge.apache.org.`
- 12 min: `ConfigNode JVM dies silently ~30s after startup due to parent shell SIGHUP (exec ... & pattern in start script).`
- 3 min: `DataNode fails with InaccessibleObjectException: JDK 17 module system blocks cglib reflective access.`

Attempt 3:

- 1 min: `No JDK 17 installed in container. Required Java >= 17.`
- `No Maven installed. The mvnw wrapper downloaded Maven 3.9.12 automatically.`
- `mvn test-compile fails on 3 pre-existing errors in test files referencing BuiltinPipePlugin.OPC_UA_SINK symbol in OPC UA pipe tests.`
- 15 min: `IoTDB servers require ~1.7GB heap by default, but container has only 754MB RAM. Servers crashed with OOM.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
