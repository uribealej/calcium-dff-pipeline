# Calcium ΔF/F Analysis Pipeline

This project provides a clean, reproducible pipeline for processing calcium imaging data using nuclear-localized GCaMP6s in zebrafish.

## Features

- Preprocess and filter ROIs based on brightness and baseline stability
- Compute smooth baselines using percentile + smoothing
- Calculate ΔF/F₀ (Delta F over F) signals

## Requirements

- Python 3.8+
- NumPy, SciPy, Matplotlib (optional for plots)

## Usage

```python
# Load your data and run:
F0 = compute_percentile_baseline(...)
deltaF_F = (fluo_clean - F0) / F0
