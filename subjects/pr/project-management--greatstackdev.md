# project-management

**Verdict: runs.** Argusic Score 95 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/GreatStackDev/project-management, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/run/ead09977-4865-4494-af89-85d20c27d5b8

## Pinned environment

- Project commit: `5949a8193e666155f9b18cc0ce2384f41f022d30`
- Test commit: `5949a8193e666155f9b18cc0ce2384f41f022d30`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 8.3 to 8.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 95 | 50 | 8.3 | 4 | 3 | [run](https://argusic.com/run/ead09977-4865-4494-af89-85d20c27d5b8) |

## What was observed on a clean machine

Attempt 1:

- 25 min: `The repo's package-lock.json omits all platform binary optionalDependencies (@rollup/rollup-linux-x64-gnu, @tailwindcss/oxide-linux-x64-gnu, lightningcss-linux-x64-gnu), so npm install produced a tree missing Rollup, Oxide, and lightningcss`
- 15 min: `Container has Node v18.19.1; Vite 7.1.9 dev server crashed at startup with 'TypeError: crypto.hash is not a function' (Node 20.19+/22.12+ required), and vite build only warned.`
- 5 min: `Bundled precompiled vite-app/playwright verification scripts could not resolve package 'playwright' from /tmp because their ESM module resolution walks up from the script location, not the cwd.`
- 5 min: `'npm run lint' reports 7 pre-existing no-unused-vars errors in src (StatsGrid.jsx, Navbar.jsx, Sidebar.jsx, etc.) and 5 react-hooks warnings; not fixed because they are upstream code defects unrelated to installation.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
