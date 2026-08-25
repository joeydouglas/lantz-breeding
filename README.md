# Lantz Breeding Tracker

Automated breeding-population dashboard for the **Lantz** cross, ingesting live observations from the shared #breeding Discord channel and syncing to Google Drive.

- Live dashboard: https://joeydouglas.github.io/lantz-breeding/
- Plant ID convention: `Ltz01`, `Ltz02`, ... (parsed from Discord text via `\bLtz[\s-]?(\d{1,2})\b`)
- Source of truth: `tracker.json` in the companion `~/.hermes/breeding/lantz/` working directory (not this repo -- this repo holds the generated static dashboard only).

## Data provenance note

Seed data for `Ltz01` was extracted from the Google Doc "Lantz" (1 plant, 3 observation paragraphs). The doc references a "Thanos" group/parent name whose meaning is unconfirmed -- preserved verbatim rather than guessed at. See `tracker.json`'s `notes_meta.flagged_ambiguities` for details.
