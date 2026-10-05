# neuron-ai

**Verdict: runs.** Argusic Score 58.6 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/neuron-core/neuron-ai, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/neuron-ai

## Pinned environment

- Project commit: `f6d4e4507309dbba6c0ecfdd602ddccebbb0bcee`
- Test commit: `f6d4e4507309dbba6c0ecfdd602ddccebbb0bcee`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 10.7 to 33.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 10.7 | 0 | 0 | [run](https://argusic.com/run/4f5a1942-044b-4b14-b763-a233616ff71c) |
| 2 | pass | 97.14 | 15 | 33.3 | 7 | 6 | [run](https://argusic.com/run/109af3f9-1e41-47e9-82e2-633ac1ae15cd) |

## What was observed on a clean machine

Attempt 2:

- 3 min: `PHP 8.1+ not installed (no root apt permissions)`
- 1 min: `Composer.phar requires phar, mbstring extensions`
- 2 min: `Composer install failed: zip extension missing, no unzip binary`
- 2 min: `Disk full (7.8G partition at 100%) during composer install`
- 2 min: `psr.so extension (from php8.3-common) provides PsrExt\Http\Message\ResponseInterface conflicting with PHP-level PSR-7 interfaces`
- 1 min: `PDO SQLite driver not found for Eloquent tests`
- `78 tests skipped (external services: Neo4j, MySQL, Elasticsearch, ChromaDB, Typesense, Weaviate, Qdrant, MeiliSearch, MariaDB, OpenSearch on ports; pdftotext binary not found)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
