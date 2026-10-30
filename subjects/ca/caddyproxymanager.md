# CaddyProxyManager

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Pacerino/CaddyProxyManager, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/caddyproxymanager

## Pinned environment

- Project commit: `52cf246adeece9145512816cfb83ed4a101f00dc`
- Test commit: `52cf246adeece9145512816cfb83ed4a101f00dc`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 6.5 to 6.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 6.5 | 5 | 5 | [run](https://argusic.com/run/05414b07-cac1-4717-a638-70535be860c3) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `no Go toolchain and go.mod requires go 1.25.0`
- 2 min: `npm install skipped @tailwindcss/oxide native binding; vite build failed with 'Cannot find native binding'`
- 1 min: `go build failed: embed pattern all:assets/** matched nothing until frontend was built`
- 2 min: `caddy binary missing so GET /api/caddy/modules returned 500`
- 1 min: `restart attempt failed with bind: address already in use`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
