# Data & Access

All large files live in our CyVerse community folder so we keep the GitHub repository light. Use the links and notes below to find the most recent sources.

## Community storage
- **CyVerse shared path:** `i:/iplant/home/shared/esiil/Innovation_summit/Group_20/`
- **Browse in a web browser:** [CyVerse Data Store viewer](https://de.cyverse.org/data/ds/iplant/home/shared/esiil/Innovation_summit/Group_20?type=folder&resourceId=0ec57af4-95a3-11f0-b0fb-90e2ba675364)
- **Recommended subfolders:**
  - `intake/` – raw CSV exports from the idea intake form
  - `notes/` – facilitator Markdown notes and transcripts
  - `scores/` – cleaned scoring tables used to drive visuals
  - `deliverables/` – slide decks, briefs, and atlas exports

## Key datasets
| Dataset | Location | Description | Notes |
|---------|----------|-------------|-------|
| Intake responses (CSV) | `intake/intake_responses_2025-01-14.csv` | Structured form submissions with contact info, novelty ratings, and tags. | Replace the filename with the latest export when uploading.
| Facilitator notes (Markdown) | `notes/session-notes/` | Summaries from breakout discussions captured by facilitators. | Normalize headings before running text analytics.
| Lightning talk slides (PDF) | `deliverables/lightning-talks/` | Slide decks shared by teams presenting wildcard ideas. | Convert key slides to PNG for embedding on the site.
| Wildcard scoring table (CSV) | `scores/wildcard_scores_day-3.csv` | Aggregated novelty × feasibility × impact scores. | Used by `code/single_hull_demo.py` to render radar plots.

## Tips
- Keep filenames timestamped (`YYYY-MM-DD`) so we can trace which version fed into each figure.
- Store sensitive information (emails, phone numbers) in the CyVerse folder only. Anonymize before publishing to GitHub.
- Document any manual cleaning steps in `code/data_processing.md` so others can reproduce the workflow.
