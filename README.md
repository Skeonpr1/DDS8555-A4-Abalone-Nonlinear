# DDS‑8555 — Assignment 4: Nonlinear Models (Abalone)

This repository contains a reproducible pipeline for two nonlinear models and Kaggle-ready submissions.
**Kaggle results (Late Submission)**
- Model 1 (Polynomial+Ridge): Public 0.15632 • Private 0.15556
- Model 2 (Spline+Ridge):    Public 0.15830 • Private 0.15911  
See `figs/kaggle_results.png` for the submission screenshot.

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
