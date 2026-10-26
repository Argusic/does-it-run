# midea_auto_cloud

**Verdict: could not verify.** Argusic Score 65 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/sususweet/midea_auto_cloud, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/midea-auto-cloud

## Pinned environment

- Project commit: `8d0f9a53ade490a18144c0b333e1e23c9b4895bb`
- Test commit: `8d0f9a53ade490a18144c0b333e1e23c9b4895bb`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, no run possible
- Valid runs: 2; wall time 10.3 to 25.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 50 | 2.5 | 25.7 | 3 | 3 | [run](https://argusic.com/run/93c578a1-43b0-4a46-b960-c0eb06833901) |
| 2 | fail | 80 | 10 | 10.3 | 4 | 4 | [run](https://argusic.com/run/817573cf-4ef7-4246-b8ac-3cd1dd88d4df) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Home Assistant is not available in the container (pip install homeassistant timed out after 2+ min due to 300+ dependency packages). The component is an HA custom_components integration with no standalone entrypoint.`
- `No test suite exists in the repository (no pytest, unittest, or test_ files found)`
- `third_party_keys: Midea cloud API credentials (account/password) are required for real device control. A mock was not attempted because the protocol requires AES-encrypted cloud API communication with real servers.`

Attempt 2:

- 0.5 min: `Missing aiofiles dependency (used in cloud.py but not in manifest.json)`
- 0.5 min: `Missing pycryptodome (Crypto.Cipher used in security.py but not in manifest.json)`
- 1 min: `SensorDeviceClass.WIND_DIRECTION removed in HA 2025.1, 8 references in T0xFA.py`
- 1 min: `example.py: dict literal used as dict key (unhashable type: 'dict') in 'set' block`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
