# VideoCoF

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/knightyxp/VideoCoF, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/videocof

## Pinned environment

- Project commit: `153e6bb31c59a15f8cd667fe0579d3567be8225b`
- Test commit: `153e6bb31c59a15f8cd667fe0579d3567be8225b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 12.6 to 12.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 5 | 12.6 | 6 | 6 | [run](https://argusic.com/run/35ba4984-cb0b-4c04-ab15-4aa6df752757) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `diffusers 0.42.1 requires torch.accelerator (PyTorch >=2.6) but torch 2.5.1 installed`
- 1 min: `scipy 1.18.1 requires numpy >=2.0 but numpy 1.26.4 was installed; numpy.long attribute missing`
- 1 min: `transformers 5.x removed FLAX_WEIGHTS_NAME import used by diffusers 0.31`
- 0.5 min: `Missing asset/1.png gallery placeholder images referenced in videox_fun/ui/ui.py line 260-267`
- 2 min: `Gradio 3.48 unable to launch with share=False due to container localhost unavailability; starlette/jinja2 version conflict caused TemplateResponse TypeError`
- 1 min: `Gradio 4.x incompatible with app (gradio_client error, argparser mismatch); needed gradio 3.x`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
