# ZeroSight360 V2 Topic-Native Image Set

This directory contains the redesigned 30-image LinkedIn set derived from `posts/posts_30day.json`.

## What changed

The old repository uses a repeated dark navy/teal/coral stat-card system. V2 assigns a visual language to each subject:

- Forensic evidence for IAM, code, cloud exposure, and dependency incidents
- Threat bulletins for exploit windows, breach data, and response clocks
- Data-lab layouts for benchmarks and comparative statistics
- Split-screen arguments for myths, opinions, and then-versus-now posts
- Control-room diagrams for SDLC, AI pipelines, maturity, and defense layers
- Field notes for personal stories and assessment lessons
- Forecast briefs for the 2027 predictions post

## Files

- `v2_day01_*.png` through `v2_day30_*.png`: 30 square PNGs, 1080x1080
- Matching `.html` files: editable Chromium-rendered sources
- `PLAN.md`: topic-to-visual mapping and publishing safety gates
- `generate_v2.py`: deterministic source generator
- `manifest.json`: image/topic/template manifest
- `../posts/posts_30day_v2.json`: copy of the 30 post records pointing at V2 assets

## Activation

The existing GitHub Actions workflow is intentionally unchanged. Review the images and verify statistics/attributions first. To activate this set, change the workflow or the production post metadata to use `posts/posts_30day_v2.json` and the `v2/` image paths in a separate reviewed change.
