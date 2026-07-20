# FTCI_public

Public front door for documents shared with **FTCI (Federation of Tibetan Cooperatives in India)**
during the new hotels-website project. Served via **GitHub Pages**.

**Live site:** https://tenzintsean.github.io/FTCI_public/

## What goes here

Only client-facing documents that have been **explicitly approved for sharing**. Internal working
docs (plans, architecture, costs, briefs) live in the private project repo and never come here.

## Publishing a document (only after approval)

1. Copy the approved HTML into `documents/`.
2. Add an entry to `manifest.json` (`file`, `title`, `date`, `category`, `description`).
3. Regenerate the table of contents:
   ```bash
   python3 build_index.py
   ```
4. `git add -A && git commit -m "publish: <doc>" && git push` — **pushing is the approval gate.**

`index.html` is generated from `manifest.json` — do not hand-edit it.
