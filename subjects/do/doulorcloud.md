# DoulorCloud

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Doulor/DoulorCloud, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/doulorcloud

## Pinned environment

- Project commit: `48c114a5e31b7fb978d680d028f45fe54a26fe41`
- Test commit: `48c114a5e31b7fb978d680d028f45fe54a26fe41`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 18.1 to 18.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.09 | 18.1 | 9 | 9 | [run](https://argusic.com/run/ef4c9d49-d12d-4a93-be82-c77ca13130e8) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js v18 too old; required >=20/22 for Vite 8/wrangler 4/vitest 4`
- 1 min: `src/i18n/en.ts missing 2 keys (mod.wl.groupTitleCustom, mod.wl.metric.customTitle)`
- 1 min: `test/dns-audit.test.ts used zoneSuffix (string) but interface expects zoneSuffixes (string[])`
- 1 min: `test/space.test.ts title thresholds didn't match TITLES in achievements.ts`
- 1 min: `src/handlers/points.ts updateShopProduct allowed editing user products; test expected 400 NOT_OFFICIAL_PRODUCT`
- 1 min: `test/donation-proxy.test.ts didn't clean proxy_node_fingerprints, causing false dedup`
- 1 min: `Donation revoke test used same VALID_SUB for both URLs causing fingerprint dedup`
- 1 min: `test/email-gate.test.ts timeout in full suite run`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
