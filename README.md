# County Rainfall and Planting Advisory

**Name:** Timothy Kerre | **Cohort:** 1milliondevs 2026

## Project Summary

A farmer-support NGO sends SMS planting advice to farmers in five counties (Nairobi, Nakuru, Kisumu, Mombasa and Machakos). This project cleans a hand-typed Machakos rainfall record (two invalid readings are imputed with the average of the valid ones), analyses monthly rainfall for all five counties with NumPy, saves a summary to `rainfall_summary.csv`, and produces a planting advisory with data-quality notes.

## How to Run

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/kerre-star/plp-da-a2-rainfall-advisory/blob/main/rainfall_analysis.ipynb)

1. Open `rainfall_analysis.ipynb` with the badge above and choose **Runtime → Run all**.
2. Or run locally: `pip install -r requirements.txt`, then open the notebook in Jupyter and run all cells.

The notebook writes `rainfall_summary.csv` in the working folder.

## Planting Advisory

- Nairobi, Nakuru, Kisumu and Mombasa should plant in **April-May**, their wettest two-month window (265 to 420 mm combined), while Machakos should plant in **November-December** (278 mm) for the short rains.
- Machakos has **6 dry months** (below 50 mm) against none in Kisumu, so Machakos advice should stress drought-tolerant crops and water conservation.

## Files

- `rainfall_analysis.ipynb`: the full analysis (Tasks 1-7), with outputs saved.
- `rainfall_summary.csv`: five rows, one per county.
- `requirements.txt`: Python libraries used (`numpy`).
