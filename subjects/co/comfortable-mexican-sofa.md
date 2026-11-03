# comfortable-mexican-sofa

**Verdict: runs.** Argusic Score 75 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/comfy/comfortable-mexican-sofa, licensed MIT, written in Ruby.

Evidence and recordings: https://argusic.com/subject/comfortable-mexican-sofa

## Pinned environment

- Project commit: `8f7e425a06aca9cfa8e21de6b7a10669c8495fc3`
- Test commit: `8f7e425a06aca9cfa8e21de6b7a10669c8495fc3`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 31.1 to 52.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 50 | 30.7 | 31.1 | 6 | 6 | [run](https://argusic.com/run/eac72289-0873-48c7-b717-c4b284c8d9d2) |
| 2 | pass | 100 | 52 | 52.5 | 13 | 13 | [run](https://argusic.com/run/e2b52f39-c89b-488e-a389-8b5683776263) |

## What was observed on a clean machine

Attempt 1:

- 20 min: `No Ruby interpreter available in container`
- 2 min: `Bundle install failed on listen gem requiring Ruby < 3.0`
- 3 min: `Bundle install failed on psych (YAML C extension) not compiled`
- 2 min: `Bundle install failed on sqlite3 gem requiring libsqlite3 headers`
- 2 min: `Mocha 1.3.0 references MiniTest constant renamed to Minitest in Ruby 3.2`
- `Rails 5.2 middleware API incompatible with Ruby 3.2 argument passing`

Attempt 2:

- 30 min: `Ruby not installed in container; compiled from source`
- 1 min: `Gem source URLs used http:// instead of https://`
- 1 min: `listen gem version constraint incompatible with Ruby 3.2`
- 1 min: `sqlite3 1.4.4 incompatible with Rails 8`
- 2 min: `mocha 1.3.0 incompatible with Minitest 6`
- 1 min: `Rails 5.2 config default incompatible with Rails 8`
- 2 min: `ActiveStorage missing service_name column in fixture and migration`
- 1 min: `ActiveStorage missing variant_records table`
- 3 min: `fixture_file_upload paths used 'files/' prefix incorrectly`
- 1 min: `Psych YAML deserialization error on revisions data`
- 1 min: `rails-controller-testing integration method signature mismatch with Rails 8`
- 1 min: `Capybara 2.17 incompatible with Rails 8`
- 10 min: `12 errors and 41 failures remain in test suite`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
