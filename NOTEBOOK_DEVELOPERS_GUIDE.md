# Dataset Notebook Template – Dataset Author Guide

Audience: dataset authors / repository maintainers of a dataset notebook repository.
Downstream data users only read the root README.md (after swap).

## Terminology
- Dataset notebook repository: your new repo created from the template.
- Dataset author / maintainer: you.
- Downstream data users: people launching notebooks.

## Recommended Workflow
1. Create dataset notebook repository from [this](https://github.com/MSD-LIVE/template-dataset-jupyter-notebook) template.
3. Edit README.md to replace placeholders.
4. Add / adapt notebooks and dependencies.
5. Test: Click the 'Explore the data' link or 'Launch Notebook Lab' button from the linked dataset's landing page in MSD-LIVE's [data repository](https://data.msdlive.org/).
6. Remove remaining placeholders.

## Placeholders to Replace in README.md
[DATASET_NAME]  
[SHORT_DATASET_DESCRIPTION]  
[NOTEBOOK_1_NAME], [NOTEBOOK_1_PURPOSE]  
[PRIMARY_LIBS]  
[CONTACT_EMAIL_OR_LINK]  
[LICENSE_OR_TERMS]  

## DATA_DIR Usage
The dataset's data is mounted as read‑only at $DATA_DIR (also /data and ~/data). Always reference via DATA_DIR for portability.

## Notebook Patterns
First cell: dependency installation.  
Subsequent cells: imports, data listing, examples.

## Support
Contact the MSD-LIVE team at info@msdlive.org.

