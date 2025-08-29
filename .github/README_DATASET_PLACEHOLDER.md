<!-- DATASET_USER_README_PLACEHOLDER: Replace all bracketed placeholders then delete this comment block. -->

# Exploring Dataset [DATASET_NAME]

[SHORT_DATASET_DESCRIPTION]

## Available Notebooks
| Notebook | Purpose | Key Libraries |
| -------- | ------- | ------------- |
| [NOTEBOOK_1_NAME].ipynb | [NOTEBOOK_1_PURPOSE] | [PRIMARY_LIBS] |
| (Add more rows) |  |  |

## Quick Start
1. Open a notebook.
2. Run the first (dependency install) cell.
3. Access data via the DATA_DIR environment variable (preferred) or /data.

## Accessing the Data
DATA_DIR points to the mounted read‑only dataset. Example (Python):
```python
import os, pathlib
data_dir = pathlib.Path(os.environ["DATA_DIR"])
print('DATA_DIR:', data_dir)
print('Top-level files:', [p.name for p in data_dir.iterdir()][:10])
```

## Notebook Summaries
- [NOTEBOOK_1_NAME].ipynb: [NOTEBOOK_1_PURPOSE]
- (Add entries)

## Environment & Dependencies
See requirements.txt (Python) or notebook install cells for R / Julia.  
Write outputs to your home directory (~/) or /tmp (dataset directory is read‑only).

## Support / Contact
Questions: [CONTACT_EMAIL_OR_LINK]

## General Help
See [this documentation](https://dev.msdlive.org/dataset-notebooks) 

## License / Terms
[LICENSE_OR_TERMS]
