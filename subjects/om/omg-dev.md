# omg.dev

**Verdict: runs.** Argusic Score 96.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/BennyKok/omg.dev, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/omg-dev

## Pinned environment

- Project commit: `015f45a98970f5709f2f2ab4b3de49237b29fdc9`
- Test commit: `015f45a98970f5709f2f2ab4b3de49237b29fdc9`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 28.8 to 38.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 93.33 | 62 | 38.5 | 3 | 2 | [run](https://argusic.com/run/6cd7c896-e07c-465e-bdd6-1f5ea9e35418) |
| 2 | pass | 100 | 10 | 28.8 | 5 | 5 | [run](https://argusic.com/run/8bf92a38-5969-4197-ac05-859b5b859017) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `bun not found in container, installed via npm --prefix ~/.local`
- 1 min: `thinking level test failed because opencode now has reasoning levels in the local model catalog cache`
- `44 test failures are environment-specific (Chromium/desktop, mobile/native, dbus, AI agent subscriptions, hosted service) , see test_depth note`

Attempt 2:

- `xclip is not installed. 3 clipboard tests fail without it. Needs: sudo apt-get install -y xclip (not available, no root).`
- `Chrome/Chromium not available. Desktop lifecycle, capture, one-surface, and onboarding tests fail (roughly 6-8 failures) because they need a real browser.`
- `mobile workspace 'bun install' fails: @novnc/novnc patch does not apply to the resolved package version. This breaks all mobile native-check test files (roughly 12 failures) and tests that spawn them.`
- `2 session-usage tests time out (5s each) waiting for a dev server PID with AGENT_BROWSER_SESSION to appear on a port.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
