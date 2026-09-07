# Lantz Breeding — Data Repo

Markdown record of truth for the **Lantz** cross, ingested live from the
shared #breeding Discord channel by `monitor_breeding_notes.py`.

- `project.md` — cross-level project record
- `plants/<ID>.md` — one file per plant (`Ltz01`, `Ltz02`, ...)

This repo is cloned and served by **breeding-data-api**
(`registry.json` → `github_repo: joeydouglas/lantz-breeding`), which the
shared `breeding-frontend` renders. `.github/workflows/trigger-do-deploy.yml`
bumps the DigitalOcean app's CACHEBUST on every push so the API re-clones.

Plant ID convention parsed from Discord text: `\bLtz[\s-]?(\d{1,2})\b`.

## Legacy static dashboard

The old generated HTML dashboard (`index.html`, `style.css`, `plants/*.html`
from `generate_dashboard.py`) moved to
**https://github.com/joeydouglas/lantz-dashboard-legacy** (NICK-701) so the
data repo holds data only.

## Data provenance note

Seed data for `Ltz01` was extracted from the Google Doc "Lantz" (1 plant, 3
observation paragraphs). The doc's reference to a "Thanos" group has been
confirmed by Joey (2026-08-25) to be a transcription artifact for "phenos"
(phenotypes) — i.e. "the tallest of all the phenos".
