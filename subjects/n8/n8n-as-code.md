# n8n-as-code

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/EtienneLescot/n8n-as-code, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/n8n-as-code

## Pinned environment

- Project commit: `cc7f42e8781c39feeb458f87338d6c622f05414d`
- Test commit: `cc7f42e8781c39feeb458f87338d6c622f05414d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 18.7 to 18.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 20 | 18.7 | 5 | 5 | [run](https://argusic.com/run/5f353f7f-4221-4c12-83af-e047be8243e7) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `npm install with scripts fails: plugins/openclaw/n8n-as-code/node_modules/openclaw preinstall script rejects Node 18 (requires >=22.22.3)`
- 3 min: `skills package test script path '--workspace=@n8n-as-code/skills' hardcodes ../../node_modules/.bin/jest which doesn't resolve (jest is in packages/skills/node_modules/.bin/jest)`
- 5 min: `skills fixture n8n-docs-complete.json had 0 pages, wrong categories format (array vs object), missing metadata fields, causing 4 docs-provider tests to fail`
- `cli-live integration tests fail: require a live n8n instance (no .env.test with real credentials)`
- `CLI 'convert' command crashes with SyntaxError: node:util does not export styleText (needs Node >= 20.12)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
