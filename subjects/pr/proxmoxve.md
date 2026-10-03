# ProxmoxVE

**Verdict: could not verify.** Argusic Score 65 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/community-scripts/ProxmoxVE, licensed MIT, written in Shell.

Evidence and recordings: https://argusic.com/subject/proxmoxve

## Pinned environment

- Project commit: `ac446889250b658f0dbe0a8a713962c69ec6d68a`
- Test commit: `ac446889250b658f0dbe0a8a713962c69ec6d68a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 10.4 to 17.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 50 | 18 | 17.5 | 1 | 1 | [run](https://argusic.com/run/30d1a8a3-af07-4c6d-9d13-85cb4219334e) |
| 2 | fail | 80 | 10 | 10.4 | 0 | 0 | [run](https://argusic.com/run/c225befd-e9fe-4f28-a6a7-0e1947357511) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `8 VM scripts (archlinux-vm, mikrotik-routeros, nextcloud-vm, openwrt-vm, opnsense-vm, owncloud-vm, pimox-haos-vm, umbrel-os-vm) had UTF-8 BOM bytes (EF BB BF) before the shebang line, causing bash -n to reject them as invalid`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
