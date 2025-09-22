# Wildcard Topic Innovation Summit 2025

Welcome to the workspace for **Innovation Summit Team 20**. This repository powers our public-facing website and serves as the central hub for sharing code, notes, and deliverables created during the 2025 Innovation Summit wildcard sprint. Everything inside the `docs/` folder is published automatically to GitHub Pages, while analysis code, notebooks, and reusable tools live in `code/`.

- **Live site:** https://cu-esiil.github.io/wildcard-topic-innovation-summit-2025__20/
- **Repository:** https://github.com/CU-ESIIL/wildcard-topic-innovation-summit-2025__20
- **Persistent storage:** `i:/iplant/home/shared/esiil/Innovation_summit/Group_20/`

If you are joining the team mid-sprint, skim the sections below to understand how we organize content and how to make your first contribution.

---

## 1) Repository layout

Think of this space as a shared online project room:

- **`docs/`** – Source files for the MkDocs website (home page, data notes, updates, etc.). Editing these files updates the public site after each commit to `main`.
- **`code/`** – Scripts, notebooks, and utilities. Add clear headers explaining what each file does and list any dependencies.
- **`documentation/`** – Extended internal notes. Summarize key takeaways on the public site so visitors always see the latest story.
- **`containers/` & `workflows/`** – Starter configurations for reproducible runs. Update these as you formalize analysis pipelines.

---

## 2) Updating the website

All public content is stored in Markdown files under `docs/`. You can edit directly in the browser or locally.

### Quick edits in GitHub
1. Open the file you want to change (for example, `docs/index.md`).
2. Click the pencil icon (✏️) to edit.
3. Make your update and scroll to **Commit changes**.
4. Write a short message such as `update day-1 questions` and click **Commit changes**.

> Within 1–2 minutes the site at https://cu-esiil.github.io/wildcard-topic-innovation-summit-2025__20/ will rebuild with your edits.

### Editing locally
```bash
# Clone the repository
git clone https://github.com/CU-ESIIL/wildcard-topic-innovation-summit-2025__20.git
cd wildcard-topic-innovation-summit-2025__20

# Create a branch if you want to test changes before merging
# (Optional) python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt

# Serve the docs locally
mkdocs serve
```
Visit `http://127.0.0.1:8000` to preview the site before pushing changes.

---

## 3) Sharing code and data

- Keep runnable scripts and notebooks in `code/`. When you add a new workflow, document how to run it inside the file and on `docs/code.md`.
- Use lightweight sample data in the repo; store large datasets in our CyVerse community folder (`Group_20`) and link to them from `docs/data.md`.
- Save polished figures or GIFs to `docs/assets/` so they can be embedded on the site.

---

## 4) Common first tasks

1. **Customize the homepage (`docs/index.md`)** with our Day 1 questions, Day 2 methods, and Day 3 findings.
2. **Add yourself to `docs/team.md`** with your role, contact info, and GitHub handle.
3. **Document your first code artifact** on `docs/code.md` and link to the script or notebook in `code/`.
4. **Log daily progress** on `docs/updates.md` so we remember decisions and open questions.

> Need a refresher? The [Instructions](docs/instructions.md) page links to day-by-day prompts and storage how-tos.

---

## 5) Learn more

- [GitHub Pages documentation](https://docs.github.com/en/pages)
- [MkDocs user guide](https://www.mkdocs.org/user-guide/)
- [CyVerse Data Store & GoCommands](https://learning.cyverse.org/ds/gocommands/)

---

## 6) Contact

For questions about the repository or website, reach out in Slack (`#innovation-summit-team-20`) or email the comms lead listed on the [team page](docs/team.md).
