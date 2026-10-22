# property_web_builder

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/etewiah/property_web_builder, licensed MIT, written in Ruby.

Evidence and recordings: https://argusic.com/subject/property-web-builder

## Pinned environment

- Project commit: `34ed1756762bf3d4ba55b4eabda93e798e9ca6aa`
- Test commit: `34ed1756762bf3d4ba55b4eabda93e798e9ca6aa`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 1.7 to 53.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 1.7 | 0 | 0 | [run](https://argusic.com/run/2e332e2e-bc9a-47bd-b617-702e41adb42f) |
| 2 | pass | 100 | 34 | 53.5 | 7 | 7 | [run](https://argusic.com/run/e2859991-1c4f-4d8f-aad6-2bba162a7918) |

## What was observed on a clean machine

Attempt 2:

- 22 min: `No Ruby/Postgres/Redis in container; system packages unavailable (no root)`
- 9 min: `pgcrypto.so failed: undefined symbol EVP_cast5_cbc (system OpenSSL 3.0 has no CAST5 without legacy provider)`
- 2 min: `Failing spec: seed_runner updated_at nanosecond vs Postgres microsecond precision`
- 6 min: `Localhost root redirected to /setup in loop after seeding because find_by_host could not resolve the default website`
- 5 min: `pwb:db:seed_tenant[default] crashed with 'Please provide valid page_part_key'`
- 3 min: `Tailwind build failed: Cannot find native binding @tailwindcss/oxide-linux-x64-gnu (npm skipped optional dep, Node 18 below engine requirement)`
- `Flaky spec: site_admin users_controller non-existent user returned 200 instead of 404 in full-suite order`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
