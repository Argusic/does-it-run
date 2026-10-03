# flink-learning

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/zhisheng17/flink-learning, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/flink-learning

## Pinned environment

- Project commit: `d731cee7618021be56d132cc925102ffff8d75e6`
- Test commit: `d731cee7618021be56d132cc925102ffff8d75e6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 53.4 to 53.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 53 | 53.4 | 8 | 8 | [run](https://argusic.com/run/fa450a31-d261-4ff9-ab84-2c9c95a9bb4e) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Java 17+ and Maven 3.9+ not pre-installed in container`
- 1 min: `flink-learning-paimon missing Flink table API dependencies (pom.xml had no <dependencies>)`
- 2 min: `flink-learning-extends Log4jKafkaAppender and Log4j2KafkaAppender: slf4j-api missing (only slf4j-log4j12/log4j-slf4j-impl in provided scope)`
- 1 min: `Log4j2KafkaAppender ExceptionUtilTest imported com.zhisheng.log.util.ExceptionUtil (wrong package - correct is com.zhisheng.flink.util.ExceptionUtil in KafkaAppenderCommon)`
- 1 min: `flink-learning-sql-blink test: TableConfig.getDefault() return type changed in Flink 1.20 (no longer compatible with StreamTableEnvironment.create)`
- 2 min: `Alibaba Cloud Maven mirror (aliyun) returned 502 for some artifacts`
- `DateUtilTests has 3 pre-existing timezone-dependent failures (tests assume JVM default is UTC+8/Asia/Shanghai but container runs UTC)`
- `SqlSubmitTest.testMain fails because it requires a live Kafka cluster`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
