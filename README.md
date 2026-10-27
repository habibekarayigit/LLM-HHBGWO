# LLM-HHBGWO
LLM-driven adaptive operator selection for binary Grey Wolf feature selection

This repository provides the supplementary data and materials for LLM-HHBGWO.

### Datasets

All datasets are public. Raw data are **not** redistributed here; please download them from the original sources.

| Dataset | Type | Source |
|---|---|---|
| Mice Protein Expression | Tabular (1,080 samples, 77 protein features) | [UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/342/mice+protein+expression) (Higuera et al., 2015) |
| Arrhythmia | Tabular (452 samples, 279 features) | [UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/5/arrhythmia) (Güvenir et al., 1997) |
| ATC (Abusive Turkish Comments) | Text (public, anonymized Instagram comments) | Karayiğit et al. (2021); see https://github.com/habibekarayigit/Turkish_Datasets |

### How to obtain the datasets

**Mice Protein Expression and Arrhythmia**
1. Open the UCI link in the table above.
2. Click **Download** (top right of the dataset page) and extract the archive.
3. Place the files under `data/raw/mice_protein/` and `data/raw/arrhythmia/`.

**ATC**
1. Open the ATC link in the table above.
2. Download the dataset files.
3. Place them under `data/raw/atc/`.

The ATC corpus consists of previously published, anonymized comments and is used as published. No new data were collected and no personal data beyond the published corpus were processed.

### Repository contents

```
LLM-HHBGWO/
├── README.md
├── LICENSE
├── supplementary_data/    DataS1-DataS90 (CSV): supplementary tables
```

Each file is named `DataS<k>_Table<id>.csv` (k = 1-90) and corresponds to the supplementary table with the same number (e.g., `DataS1_TableS1.csv` = Table S1).

The following materials will also be added to this repository:
- BGWO-family controller harness and configurations
- Hashed initial populations
- Logged optimizer states and LLM decisions
- Derived TF-IDF matrices and fold indices
- Oracle and placebo scripts

### Data availability

The datasets are public and available from the sources listed above. The materials in this repository will be archived with a DOI upon acceptance.

### License

Code and supplementary tables are released under the MIT License (see `LICENSE`). The original datasets remain subject to the licenses of their respective providers.

---
