# [Project title]

> **How to use this template:** click **Use this template → Create a new repository**, choose the owner **Tum-Soil-Biophysics**, keep it **Private**, and name it `Topic_Method` (e.g. `RWU_NeutronRadiographyD2O_InverseModelling`). Then replace every `[...]` below and delete this note.

[One or two sentences: what this code does and which question it answers.]

**Related article:** [Authors (Year). Title. Journal. DOI] *(add at acceptance)*
**Code DOI (Zenodo):** [DOI] *(created with the first release)*

## Data

Raw and large data are **not** stored in this repository.

| Data | Location |
|---|---|
| Raw data (during the project) | Group drive `\\nas.ads.mwn.de\tus4\b1e\[path]` |
| Published data | [mediaTUM or Zenodo DOI] *(at publication)* |
| Small example data | `data/example/` |

## Structure

```
code/              scripts and functions
notebooks/         Jupyter notebooks (exploration, figures)
data/example/      small example data only (a few MB)
results/figures/   figures produced by the code
requirements.txt   Python packages
CITATION.cff       how to cite this code
```

## Installation

```bash
git clone https://github.com/Tum-Soil-Biophysics/[repository].git
cd [repository]
python -m venv .venv
.venv\Scripts\activate          # Windows  (macOS/Linux: source .venv/bin/activate)
pip install -r requirements.txt
```

## How to run

```bash
python code/[script].py --input data/example
```

[Describe the main steps, inputs and outputs.]

## Authors

[Name], [Name], Mohsen Zarebanadkouki
Professorship for Soil Biophysics and Environmental Systems, Technical University of Munich

## License

MIT, see [LICENSE](LICENSE). If you use this code, please cite the related article and this repository (see [CITATION.cff](CITATION.cff)).
