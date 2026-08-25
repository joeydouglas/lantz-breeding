# Lantz Breeding Tracker

Automated breeding-population dashboard for the **Lantz** cross, ingesting live observations from the shared #breeding Discord channel and syncing to Google Drive.

- Live dashboard: https://joeydouglas.github.io/lantz-breeding/
- Plant ID convention: `Ltz01`, `Ltz02`, ... (parsed from Discord text via `\bLtz[\s-]?(\d{1,2})\b`)
- Source of truth: `tracker.json` in the companion `~/.hermes/breeding/lantz/` working directory (not this repo -- this repo holds the generated static dashboard only).

## Data provenance note

Seed data for `Ltz01` was extracted from the Google Doc "Lantz" (1 plant, 3 observation paragraphs). The doc's reference to a "Thanos" group has been confirmed by Joey (2026-08-25) to be a transcription artifact for "phenos" (phenotypes) -- i.e. "the tallest of all the phenos". Original doc text is preserved verbatim in `tracker.json`'s `original_notes` field for the historical record; see `corrected_reading` on the plant entry and `notes_meta.resolved_ambiguities` for details.
