# http-kit

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/http-kit/http-kit, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/http-kit

## Pinned environment

- Project commit: `7f8c70159ca1e239957d74baac8731582e269c77`
- Test commit: `7f8c70159ca1e239957d74baac8731582e269c77`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 23.9 to 23.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 28 | 23.9 | 5 | 5 | [run](https://argusic.com/run/d442d32d-2781-4bde-90f9-da2201c3e8d9) |

## What was observed on a clean machine

Attempt 1:

- 6 min: `No Java JDK or JRE installed in container`
- 8 min: `Java cacerts symlink pointed to missing /etc/ssl/certs/java/cacerts; Java.security file symlinks pointed to missing /etc/java-17-openjdk/`
- 2 min: `Leiningen not installed`
- 10 min: `project.clj plugins (lein-pprint, lein-ancient, lein-codox) and nrepl profile plugins (cider-nrepl, enrich-classpath) could not be resolved from any Maven repository`
- 2 min: `IPv6 test fails (test-ipv6): protocol family unavailable in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
