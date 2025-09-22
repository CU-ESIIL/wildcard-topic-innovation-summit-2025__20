# Code catalog

A quick index of the scripts and notebooks powering the Wildcard Atlas. Keep this page current so collaborators can reproduce our steps without digging through the repository tree.

## Python & notebook workflows

### `code/prism_quicklook.py`
- **Purpose:** Prototype text-cleaning and clustering pipeline using SentenceTransformers + BERTopic.
- **Inputs:** `data/intake/intake_responses.csv` (export from the CyVerse form), optional facilitator tags in `data/intake/facilitator_notes.csv`.
- **How to run:**
  ```bash
  python code/prism_quicklook.py --responses data/intake/intake_responses.csv --notes data/intake/facilitator_notes.csv --out outputs/bertopic/
  ```
- **Outputs:** `outputs/bertopic/topic_summary.csv` (cluster labels, keywords) and `outputs/bertopic/topic_viz.html` for quick review.

### `code/single_hull_demo.py`
- **Purpose:** Generates the radial scoring visualization used in the atlas cards.
- **Inputs:** `data/scores/wildcard_scores.csv` with columns `idea`, `novelty`, `feasibility`, `impact`.
- **How to run:**
  ```bash
  python code/single_hull_demo.py --scores data/scores/wildcard_scores.csv --out docs/assets/results/
  ```
- **Outputs:** PNG plots saved to `docs/assets/results/` that can be embedded directly on the site.

### `code/fired_time_hull_panel.ipynb`
- **Purpose:** Notebook scaffolding for multi-panel storyboards. We adapt it to arrange atlas cards and timeline callouts.
- **Usage notes:** Open in JupyterLab, update the `DATA_DIR` constant to point at `data/scores/`, and export key figures to `docs/assets/`.

## Documentation helpers

### `code/data_processing.md`
- **Summary:** Markdown log outlining how we clean raw submissions (de-duplication, anonymization) before analysis.

### `code/data_analysis.md`
- **Summary:** High-level overview of clustering experiments, scoring heuristics, and evaluation metrics. Update after each iteration.

### `code/visualizations.md`
- **Summary:** Gallery of visual treatments we’ve tested. Include notes on what resonates with stakeholders and what to avoid.

## Contributing
- Keep scripts lightweight and include docstrings with parameter descriptions.
- Commit generated plots to `docs/assets/results/` when they explain a finding; otherwise store large assets in CyVerse.
- Open an issue if you change expected inputs/outputs so others can update their workflows promptly.
