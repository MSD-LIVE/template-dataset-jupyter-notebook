<!--
MAINTAINER NOTICE:
Replace all bracketed placeholders ([LIKE_THIS]) then delete this comment block.
See Notebook_Developers_README.md for guidance.
-->

<!-- TEMPLATE_ROOT_README: Root README for the TEMPLATE REPOSITORY itself.
     In derived dataset repositories this file will be auto-replaced (if unchanged)
     by the dataset user README placeholder stored at .github/README_DATASET_PLACEHOLDER.md -->

# MSD-LIVE Dataset Notebook Template

This repository is a GitHub Template used to create per-dataset notebook repositories.
After you click “Use this template” the resulting dataset notebook repository will (on first push)
swap this README for an end‑user dataset README (if you have not edited it yet).

## What This Template Provides
- Example notebooks: example_python.ipynb, example_r.ipynb, example_julia.ipynb
- Author guide: in .github/NOTEBOOK_DEVELOPERS_GUIDE.md
- Automated README swap workflow
- Pattern for dependency installation & DATA_DIR usage

## Files That Will Move / Be Swapped
- .github/README_DATASET_PLACEHOLDER.md -> becomes README.md in new repos (if marker intact)
- .github/NOTEBOOK_DEVELOPERS_GUIDE.md stays in .github (not shown on project home page)

## How the Swap Works
1. You generate a new repository from this template.
2. On the first push, if THIS README:
   - Still contains TEMPLATE_ROOT_README marker, AND
   - Matches the upstream template README content exactly, THEN
   the workflow copies .github/README_DATASET_PLACEHOLDER.md to README.md
3. You then customize placeholders in the new README.

If you prefer to keep this template overview visible in the new repo, remove the marker comment.

## Quick Start (For Template Users)
1. Generate new repository from template.
2. Push (or manually copy the placeholder README if you disabled the workflow).
3. Edit README.md placeholders.
4. Customize notebooks & requirements.
5. Commit and ensure no placeholder tokens remain.

## DATA_DIR Convention
Dataset files mount read‑only at $DATA_DIR (also /data symlink). All relative paths in notebooks should use DATA_DIR.

## Support
See internal documentation or contact the MSD-LIVE team.