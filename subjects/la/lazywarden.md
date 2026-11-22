# lazywarden

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/querylab/lazywarden, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/lazywarden

## Pinned environment

- Project commit: `85afd87a3b26c5ae82067f843bc0cd4dda0a4805`
- Test commit: `85afd87a3b26c5ae82067f843bc0cd4dda0a4805`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 9.1 to 32.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 6 | 32.1 | 5 | 5 | [run](https://argusic.com/run/233f68df-3f54-4e92-88ea-6855d1d4a52d) |
| 2 | pass with mocks | 92 | 10 | 9.1 | 6 | 6 | [run](https://argusic.com/run/8ab6f3d4-7414-4a8b-8585-f6d9ddfcf10a) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `pip install -r requirements.txt failed: pycrypto (a dependency of mega.py 1.0.8) fails to build on Python 3.12 without python3-dev headers (no root to apt install)`
- 1 min: `App hardcoded /usr/local/bin/bw (unwritable without root) for all Bitwarden CLI invocations`
- 1 min: `check_server_configured() hardcoded /root/.config/Bitwarden CLI/data.json, causing PermissionError as non-root before any backup could run`
- 1 min: `app/bitwarden_client.py is_vault_unlocked() referenced an undefined variable bw_bin (NameError) after pinning the bw path`
- 1 min: `Secrets manager raised 'badly formed hexadecimal UUID string' because .env passed direct values (BW_URL etc.) while the code assumed every secret env var is a Bitwarden secret UUID`

Attempt 2:

- 3 min: `pycrypto package fails to build from source (needs python3-dev headers which require root to install)`
- 1 min: `bitwarden_client.py has hardcoded /root/.config/Bitwarden CLI path, fails with PermissionError`
- 1 min: `backup.py and import_to_bitwarden.py use hardcoded /usr/local/bin/bw path`
- 1 min: `.env missing required vars (ACCESS_TOKEN, ORGANIZATION_ID, BACKUP_DIR) and has /root/ paths`
- 3 min: `Bitwarden SDK native module requires real Bitwarden server credentials`
- 1 min: `bw CLI not found (not installed), Bitwarden CLI required for subprocess calls`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
