# spree_i18n

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/spree-contrib/spree_i18n, licensed BSD-3-Clause, written in Ruby.

Evidence and recordings: https://argusic.com/subject/spree-i18n

## Pinned environment

- Project commit: `35a2e59c888f50a0a042b32e8e130927eadaf11e`
- Test commit: `35a2e59c888f50a0a042b32e8e130927eadaf11e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 17.1 to 17.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 16 | 17.1 | 3 | 3 | [run](https://argusic.com/run/df405b61-88ef-487b-a110-26ea13573cb2) |

## What was observed on a clean machine

Attempt 1:

- 14 min: `No Ruby runtime found in container`
- 2 min: `MissingTranslationData for activerecord.attributes.spree/address.zipcode in en locale (Spree 6.0 renamed zipcode to postal_code)`
- 0.5 min: `DeprecationException: Spree.t is deprecated and raises errors in test mode`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
