# Beanbun

**Verdict: runs.** Argusic Score 93.5 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/kiddyuchina/Beanbun, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/beanbun

## Pinned environment

- Project commit: `092063908d5831a6cb660748b1f2f49b62afcdc6`
- Test commit: `092063908d5831a6cb660748b1f2f49b62afcdc6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 15.6 to 16.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 16 | 16.3 | 2 | 2 | [run](https://argusic.com/run/947cc50e-529c-43ab-9932-dc8bf3e33665) |
| 2 | pass with mocks | 87 | 15 | 15.6 | 4 | 3 | [run](https://argusic.com/run/9e8bc012-8b71-4ecf-9caa-0a69f365ba53) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `PHP missing from container`
- 8 min: `Composer not available (PHP built without phar extension, complex dep chain)`

Attempt 2:

- 3 min: `PHP and Composer not installed in container`
- 1 min: `Composer blocked guzzlehttp/guzzle ^6.0 for security advisories`
- 1 min: `Undefined array key 'headers' warning in Beanbun.php:432`
- `Static PHP libcurl blocked by seccomp for local loopback connections`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
