# Light-A-Video

**Verdict: could not verify.** Argusic Score 35 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/bcmi/Light-A-Video, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/light-a-video

## Pinned environment

- Project commit: `1b444823a725f0d5d8dc8185a4d8e1c23aea316c`
- Test commit: `1b444823a725f0d5d8dc8185a4d8e1c23aea316c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, no run possible
- Valid runs: 2; wall time 8.3 to 18.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 50 | 38 | 8.3 | 3 | 3 | [run](https://argusic.com/run/15d31870-5480-4966-a8bc-db52650eb32a) |
| 2 | fail | 20 | n/a | 18.5 | 0 | 0 | [run](https://argusic.com/run/109e04ca-32b7-4be5-82ce-41ed1d4f9c65) |

## What was observed on a clean machine

Attempt 1:

- 12 min: `README install (pip install -r requirements.txt) failed: diffusers==0.32.1 lacks AutoencoderKLWan/WanTransformer3DModel, breaking lav_wan_relight.py and src/wan_pipe.py; sd_origin keys also mismatched IC-Light's 8-channel conv_in (excluded`
- 26 min: `Runtime requires CUDA: lav_relight.py hardcodes torch.device('cuda'); container has a CPU-only torch and no NVIDIA GPU`
- `First CLI launch was OOM-killed (exit 137): control-group memory.max is 8 GiB while loading the full fp32 Undefined pipeline needs >3.2 GiB just for the UNet (vae 319 MB, text 469 MB, peak exceeds cgroup)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
