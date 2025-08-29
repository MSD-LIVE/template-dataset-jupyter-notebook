# Dataset Notebook Template – Dataset Author Guide

Audience: dataset authors / repository maintainers of a dataset notebook repository derived from the template.  
Downstream data users only read the root README.md (after swap).

## Terminology
- Template repository: the original upstream template.
- dataset notebook repository: your new repo created from the template.
- Dataset author / maintainer: you.
- Downstream data users: people launching notebooks.

## Recommended Workflow
1. Create dataset notebook repository from template.
2. First push triggers README swap (if template README unmodified).
3. Edit README.md (copied from placeholder) to replace placeholders.
4. Add / adapt notebooks and dependencies.
5. Test: run first cells in each notebook.
6. Remove remaining placeholders.
7. (Optional) Add CI placeholder check.

## Placeholders to Replace in README.md
[DATASET_NAME]  
[SHORT_DATASET_DESCRIPTION]  
[NOTEBOOK_1_NAME], [NOTEBOOK_1_PURPOSE]  
[PRIMARY_LIBS]  
[CONTACT_EMAIL_OR_LINK]  
[LICENSE_OR_TERMS]  

## DATA_DIR Usage
Data mounts read‑only at $DATA_DIR (also /data). Always reference via DATA_DIR for portability.

## Notebook Patterns
First cell: dependency installation.  
Subsequent cells: imports, data listing, examples.

## Automatic README Swap
- Source placeholder: .github/README_DATASET_PLACEHOLDER.md
- Swap happens only if ALL are true:
  1. Initial commit (commit count == 1)
  2. Root README contains TEMPLATE_ROOT_README marker
  3. Root README matches upstream template README exactly (hash compare)
  4. Workflow has write permission to repo contents (permissions: contents: write)

If write permission is removed, the workflow will log the swap attempt but cannot push.

## Optional CI Placeholder Check
Add a workflow that greps for bracketed placeholders and fails if found.

## Support
Contact the MSD-LIVE team.

