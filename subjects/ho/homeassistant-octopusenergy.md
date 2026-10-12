# HomeAssistant-OctopusEnergy

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/BottlecapDave/HomeAssistant-OctopusEnergy, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/homeassistant-octopusenergy

## Pinned environment

- Project commit: `e52c185003a4b599274b8efdad2183ebd298217c`
- Test commit: `e52c185003a4b599274b8efdad2183ebd298217c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 13.7 to 13.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 13.7 | 6 | 6 | [run](https://argusic.com/run/0a26e9d7-4559-45e2-bbc5-1cf1036da1d3) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `homeassistant==2025.11.0 requires Python 3.13 but container has Python 3.12`
- 2 min: `from homeassistant.helpers.helper_integration import async_remove_helper_config_entry_from_source_device - module not found in HA 2025.1.4`
- 3 min: `StatisticMeanType and unit_class/mean_type fields not present in StatisticMetaData TypedDict in HA 2025.1.4`
- 2 min: `async_entity_id_to_device not found in homeassistant.helpers.device (renamed to async_entity_id_to_device_id)`
- `Integration tests require real Octopus Energy API credentials (API_KEY, ACCOUNT_ID, etc.)`
- `Local integration tests require HOME_PRO_API_KEY and HOME_PRO_BASE_URL env vars`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
