# DDS‑8555 — Assignment 4: Nonlinear Models (Abalone)

This repository contains a reproducible pipeline for two nonlinear models and Kaggle-ready submissions.

## Structure
```
DDS8555_A4_GitHub/
  data/                      # put Kaggle CSVs here: train.csv, test.csv, sample_submission.csv
  figs/                      # diagnostics and Kaggle results screenshot
  outputs/                   # submission CSVs + CV summary
  src/
  DDS8555_A4_Abalone_Nonlinear.ipynb
  requirements.txt
  README.md
  .gitignore
```
## Quick start
1. `pip install -r requirements.txt`
2. Place the three Kaggle files into `data/`.
3. Run the notebook. It will train **Model 1 (Polynomial+Ridge)** and **Model 2 (Spline+Ridge)**, perform 3-fold OOF evaluation, and save submissions to `outputs/` (negatives clipped to 0).
4. Upload a submission to Kaggle. Screenshot is in `figs/kaggle_results.png`.