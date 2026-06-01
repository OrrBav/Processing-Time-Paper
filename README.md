# Processing-delay perturbation analysis of colorectal cancer TCR repertoires

Reproducibility repository accompanying the manuscript:

> *CORE clonotypes: a reproducible structural component of the peripheral TCR repertoire revealed through variation in blood processing times*
This repository contains the analysis notebook and code used to reproduce the main and supplementary analyses and figures presented in the manuscript.

## Repository contents

- `notebooks/manuscript_analysis.ipynb` — main analysis notebook
- `requirements.txt` — Python package requirements
- `figures/` — generated manuscript figures
- `data/` — input data directory structure

## Environment

Analyses were performed in Python using the following major packages:

- pandas
- numpy
- matplotlib
- seaborn
- scipy
- scirpy
- anndata
- logomaker
- biopython
- statsmodels
- networkx
- tqdm

Install dependencies with:

```bash
pip install -r requirements.txt
```

## Data

This repository does not include raw sequencing files.

To reproduce the analyses:

1. Download the public sequencing data described in the manuscript.
2. Process TRB repertoires with MiXCR using the parameters described in the Methods.
3. Place per-sample MiXCR clonotype `.tsv` files in:

```text
data/mixcr_trb/
```

4. Place the sample metadata file as:

```text
data/colon_meta_time.csv
```

The analysis notebook reads these files directly.

## Reproducibility

The notebook is organized according to manuscript figures and can be executed sequentially to reproduce the reported analyses and visualizations.
