# Dataset setup

The datasets used for the academic project are not committed to this public repository because their source and redistribution licence were not included with the original submission.

To run the workflows, place authorised copies of these files in this directory:

| File | Role | Expected shape in the original project |
| --- | --- | ---: |
| `filialumsatz.csv` | Raw daily sales observations | 336,084 rows × 9 columns |
| `filialen.csv` | Store master data | 406 rows × 10 columns |
| `fialialeclean.csv` | Cleaned modelling table produced by workflow 1 | 119,905 rows × 23 columns |

The original filename `fialialeclean.csv` is preserved for workflow compatibility.

Run `01-data-preparation.knwf` first to recreate the cleaned modelling table from the two raw input files. The forecasting and clustering workflows both use the cleaned file.
