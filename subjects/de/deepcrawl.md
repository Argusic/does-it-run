# deepcrawl

**Verdict: runs.** Argusic Score 93.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/lumpinif/deepcrawl, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/deepcrawl

## Pinned environment

- Project commit: `964de4b1fac95e28094c5e865047abf1ba00b876`
- Test commit: `964de4b1fac95e28094c5e865047abf1ba00b876`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 33.2 to 33.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 93.33 | 18 | 33.2 | 6 | 4 | [run](https://argusic.com/run/58951d8c-32ee-4104-afc4-6119e0718701) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `tsdown build needs Node>=20 (node:util.styleText), container has Node 18`
- 3 min: `rolldown missing native binding @rolldown/binding-linux-x64-gnu`
- 2 min: `Dashboard build failed: [getBaseURL] URL is not defined`
- 5 min: `Wrangler dev requires CLOUDFLARE_API_TOKEN and reaches remote D1/KV/service bindings by default (wrangler.jsonc marks them remote)`
- 5 min: `Auth package fails to load: better-auth-harmony requires validator/es/lib/isEmail.cjs which doesn't exist in validator 13.15`
- `Root env:generate fails: no tsx dependency`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
