# ORU water and sewer usage analysis

An exploratory Python notebook investigating seasonal water and sewer usage at ORU. The analysis compares off-season months (November through April) with the rest of the year, examines individual meters, and experiments with linear regression.

## Explore the analysis

Open [python_data_analysis.ipynb](python_data_analysis.ipynb) to view the notebook and its saved outputs. Historical outputs describe the original run; they are not a fresh validation of the model.

## Run locally

Use Python 3.10 or newer from the repository root:

```bash
git clone https://github.com/derrickbaruga7/Python-Data-Analysis.git
cd Python-Data-Analysis
python3 -m venv .venv
source .venv/bin/activate
python -m pip install -r requirements.txt
jupyter lab python_data_analysis.ipynb
```

On Windows, activate with `.venv\Scripts\activate` instead.

The source workbook is **not included**. Place an authorized copy at `data/Water_Usage_ORU-2023.xlsx`, or set `ORU_WATER_DATA` to its path before launching Jupyter. The notebook loads all workbook sheets and expects the layout used in the original analysis. Review the transformation cells when using a different workbook. Local data is ignored by Git.

## Methods and limits

- Histograms and time-series plots explore usage patterns and seasonality.
- Meter-level comparisons identify candidates for further investigation.
- Pearson correlations and linear regression explore associations; they do not establish causes or prove that an intervention reduces usage.
- The analysis needs the original workbook and a fresh execution before any reported model performance can be independently reproduced.

Licensed under the [MIT License](LICENSE).
