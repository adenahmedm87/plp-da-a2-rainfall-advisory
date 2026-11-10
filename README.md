# County Rainfall and Planting Advisory

**Name:** ADEN AHMED MOHAMED  
**Cohort:** 1M DEVIS

This project cleans the supplied Machakos rainfall readings, combines five counties into a 5 × 12 NumPy array, analyses annual and monthly rainfall, and exports a five-county CSV summary. NumPy performs the numerical calculations; Python’s built-in csv module writes the output.

## How to run

[Open in Colab](https://colab.research.google.com/github/adenahmedm87/plp-da-a2-rainfall-advisory/blob/main/rainfall_analysis.ipynb), then choose **Runtime → Restart session and run all**. For local use, install Python 3 and Jupyter, run `python -m pip install -r requirements.txt`, open `rainfall_analysis.ipynb`, and restart the kernel and run all cells. The notebook writes `rainfall_summary.csv` in the current working directory. Numerical outputs are already saved in the committed notebook.

## Planting advisory

- Plan around April–May for Nairobi, Nakuru, Kisumu and Mombasa, whose two-month rainfall totals are 395, 265, 420 and 390 mm respectively.
- Use November–December as Machakos’s rainfall-based planning window at 278 mm, and prioritise water conservation there because 6 months receive less than 50 mm.
- Treat Machakos results as estimates because April and September were imputed at 68 mm each, and confirm station records, current forecasts, crop needs and soil conditions before sending planting advice.

## Files and dependencies

- `rainfall_analysis.ipynb`: cleaning, NumPy analysis, saved outputs and advisory.
- `rainfall_summary.csv`: header plus exactly five county records.
- `requirements.txt`: NumPy, the only external library imported by the notebook.
- `README.md`: project summary and run instructions.

The csv module is part of Python’s standard library and does not require a pip entry. Planting windows follow the assignment’s highest consecutive two-month rainfall rule, without December–January wrapping; ties choose the earliest window.
