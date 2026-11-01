# DSCI 552 — Homework 5

Interpretable decision trees on the UCI Acute Inflammations data (label-powerset
multiclass encoding, full-tree IF-THEN rule extraction, and cost-complexity
pruning with the one-standard-error rule), and regression of
`ViolentCrimesPerPop` on the UCI Communities and Crime data with ordinary least
squares, ridge, two LASSO variants, principal component regression and XGBoost,
all selected by training-only cross-validation.

## structure

- `notebook/Liau_Olivia_HW5.ipynb` — the full assignment (code + written answers)
- `data/` — the supplied data folder exactly as organized: the raw UCI files
  `diagnosis.data`, `diagnosis.names`, `communities.data`, `communities.names`,
  plus the KDnuggets article referenced by the assignment (kept with the data;
  not read by the notebook)

## environment

- Python 3.14 (developed and executed with 3.14.7); any recent Python 3.11+
  should work.
- macOS needs the OpenMP runtime for XGBoost: `brew install libomp`.

```bash
python3 -m venv .venv
.venv/bin/pip install -r requirements.txt
.venv/bin/jupyter notebook notebook/Liau_Olivia_HW5.ipynb
(Kernel -> Restart Kernel and Run All)
```

