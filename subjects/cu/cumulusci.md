# CumulusCI

**Verdict: runs.** Argusic Score 97.1 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/SFDO-Tooling/CumulusCI, licensed BSD-3-Clause, written in Python.

Evidence and recordings: https://argusic.com/subject/cumulusci

## Pinned environment

- Project commit: `38a6b1b5ff082faaf8d10573e414480557b33909`
- Test commit: `38a6b1b5ff082faaf8d10573e414480557b33909`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 38 to 38 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 97.14 | 0.8 | 38 | 7 | 6 | [run](https://argusic.com/run/618b2102-3117-430b-996e-4916dff12732) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `LibraryDocBuilder/ResourceDocBuilder missing doc_format arg (Robot Framework 7.x breaking change)`
- 1 min: `test_service_connect__attr_with_default_value: Click 8.x prompt defaults wrapped in [(PRESET)] not [PRESET]`
- 3 min: `Salesforce PATCH tests fail with ChunkedEncodingError (urllib3 2.x rejects body on 204)`
- 5 min: `MockHttpResponse sub-mock creation fails with unexpected kwarg 'parent' (Python 3.12 unittest.mock)`
- 8 min: `vcrpy 8.x passes bytes_iterator/list-of-bytes for request bodies, _cleanup/simplify_body expects bytes`
- 4 min: `Back-compat test subprocess fails due to ImportPathMismatchError with installed cumulusci package`
- 10 min: `VCR cassettes for upsert tests incompatible with vcrpy 8.x (CannotOverwriteExistingCassetteException)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
