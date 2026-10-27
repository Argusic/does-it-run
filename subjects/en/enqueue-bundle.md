# enqueue-bundle

**Verdict: runs.** Argusic Score 97.5 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/php-enqueue/enqueue-bundle, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/enqueue-bundle

## Pinned environment

- Project commit: `688851f8049e9b26cbe4c61a5f0e4fe8f36ea888`
- Test commit: `688851f8049e9b26cbe4c61a5f0e4fe8f36ea888`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 35.4 to 35.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 97.5 | 34 | 35.4 | 8 | 7 | [run](https://argusic.com/run/3fb774a3-3dde-4c29-b2b2-cc386d34ac20) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `PHP runtime not installed in container`
- 4 min: `PHP built --disable-phar; composer.phar refused to run`
- 3 min: `composer resolution failed: require-dev needs ext-amqp/ext-mongo/ext-mongodb`
- 6 min: `composer could not download dist zips (no zip extension/unzip/7z)`
- 2 min: `Unit tests errored: DMS\PHPUnitExtensions\ArraySubset\Assert not found`
- 3 min: `Functional tests errored: SimpleXML/PDO/sqlite missing and DOCTRINE_DSN unset`
- 2 min: `2 UseCasesTest data-provider tests hard-require /var/rabbitmq_certificates (monorepo layout; no root)`
- 1 min: `Tests/Functional/App/console.php autoload path was monorepo-relative`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
