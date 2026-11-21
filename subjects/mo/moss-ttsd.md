# MOSS-TTSD

**Verdict: runs.** Argusic Score 70 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/OpenMOSS/MOSS-TTSD, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/moss-ttsd

## Pinned environment

- Project commit: `46973e425da227bfa3b315dcd7a4aba8b6be5574`
- Test commit: `46973e425da227bfa3b315dcd7a4aba8b6be5574`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, no run possible
- Valid runs: 2; wall time 17.4 to 25.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 6 | 25.3 | 2 | 2 | [run](https://argusic.com/run/d03528ea-cef1-4517-8010-0664bac3cb57) |
| 2 | fail | 40 | 27 | 17.4 | 4 | 2 | [run](https://argusic.com/run/adc29431-ca26-42d5-9c84-c59a7b421758) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `pip install blocked by PEP 668 (externally-managed-environment) on Debian-based container`
- 1 min: `processor(text=...) kwarg raised KeyError: conversations`

Attempt 2:

- 5 min: `Model weights too large to download: MOSS-TTSD-v1.0 (~20GB) and MOSS-Audio-Tokenizer (~10GB) require ~30GB, disk had 5GB free at peak, 300MB after cleanup. RAM insufficient (2GB) for even the 5GB codec safetensors mmap.`
- 5 min: `PyPI torch==2.9.1+cu128 not available on CPU index; used torch==2.9.1 (CPU) and torchaudio==2.9.1 (CPU) from pytorch.org/cpu.`
- 10 min: `Disk space exhaustion during pip install (3.6GB pip cache + CUDA nvidia packages filled 7.8GB disk).`
- 2 min: `No GPU available (torch.cuda.is_available()=False), no nvidia-smi.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
