# django-dbbackup

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Archmonger/django-dbbackup, licensed BSD-3-Clause, written in Python.

Evidence and recordings: https://argusic.com/subject/django-dbbackup

## Pinned environment

- Project commit: `6714cd0122483cd2ba79722764a51bedad6a9caa`
- Test commit: `6714cd0122483cd2ba79722764a51bedad6a9caa`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 6.7 to 6.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 6.7 | 1 | 1 | [run](https://argusic.com/run/a6931a44-5580-43b4-9ebf-b724dfb14692) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `DbbackupAdminEmailHandler.send_mail calls self.connection() which was removed in Django 6.1 (raises AttributeError)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
