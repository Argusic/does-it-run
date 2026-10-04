# enqueue-dev

**Verdict: runs with mocks.** Argusic Score 56 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/php-enqueue/enqueue-dev, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/enqueue-dev

## Pinned environment

- Project commit: `1aa76e9086cd2f8619837666fed9acddae1b3c2e`
- Test commit: `1aa76e9086cd2f8619837666fed9acddae1b3c2e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 13 to 17.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 13 | 0 | 0 | [run](https://argusic.com/run/5ca25079-4a43-4835-81c2-65f31264527a) |
| 2 | pass with mocks | 92 | 18 | 17.4 | 4 | 4 | [run](https://argusic.com/run/6ca900e4-3474-468c-8ad2-002ce4866841) |

## What was observed on a clean machine

Attempt 2:

- 5 min: `PHP and Composer not pre-installed; needed to download static PHP 8.2.13 binary and install Composer manually`
- 8 min: `3 RdKafka unit tests failed expecting LogicException but got RuntimeError because librdkafka version check ran before input validation`
- `134 errors and 11 failures from missing backend services (RabbitMQ, MongoDB, MySQL, PostgreSQL, Redis, Beanstalkd, Gearman, Kafka, WAMP, LocalStack, Stomp)`
- `191 skipped tests due to missing native PHP C extensions (ext-amqp, ext-gearman, ext-mongodb, ext-rdkafka)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
