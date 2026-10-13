# jenkinsapi

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/pycontribs/jenkinsapi, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/jenkinsapi

## Pinned environment

- Project commit: `dda58f4e4efb143cd0c70f4ad4ee46a41b514337`
- Test commit: `dda58f4e4efb143cd0c70f4ad4ee46a41b514337`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 5.4 to 5.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 5 | 5.4 | 4 | 4 | [run](https://argusic.com/run/3393ba83-5170-4a39-a945-f49d9f8175dc) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `pip install 'jenkinsapi[dev]' left dev extras uninstalled (only runtime deps were installed)`
- 1 min: `requests-kerberos dependency requires system krb5-config (gssapi build fails; no root to install libkrb5-dev)`
- 2 min: `first mock server returned XML at /api/python but the library expects JSON, causing JenkinsAPIException 'Cannot parse' (my mock was not schema-correct)`
- 2 min: `jenkins_invoke CLI run used CrumbRequester by default and hit /job/demo_job/buildWithParameters while my mock only served /build`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
