# JMComic-Crawler-Python

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/hect0x7/JMComic-Crawler-Python, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/jmcomic-crawler-python

## Pinned environment

- Project commit: `2838d116de31d6253f4a05d19a5f82fec5f9c83f`
- Test commit: `2838d116de31d6253f4a05d19a5f82fec5f9c83f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 9.6 to 9.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 9.6 | 3 | 3 | [run](https://argusic.com/run/87b6b167-5ad1-424f-8e72-8cdf697db21f) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Missing option_test.yml (no option_test.yml in assets/option/, only option_test_api.yml and option_test_html.yml existed)`
- `test_sync_progress_is_rendered_before_download_finishes: assertIn('本子-JM123456', '') , rendered output empty at time of assertion, a timing race in rich console rendering`
- `test_plugin_uses_real_scheduler_without_stdout_or_image_io: assertIn('album.before', rendered) , 'album.before' not found in rendered rich output (only image.after/photo.after/album.after present), a rendering-order timing issue`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
