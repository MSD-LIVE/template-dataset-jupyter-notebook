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
- Trigger: convert-template-readme workflow if TEMPLATE_ROOT_README marker present.

Disable by removing the marker or the workflow file.

## Optional CI Placeholder Check
Add a workflow that greps for bracketed placeholders and fails if found.

## Support
Contact the MSD-LIVE team.

