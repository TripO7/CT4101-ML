# Using Sensor Measurements to Predict NOx Emissions from a Gas Turbine

## Repo Link
https://github.com/TripO7/CT4101-ML

## Research Question
Using trained models & sensor measurements, how accurately could we predict the hourly NOx emissions from a gas
turbine and how would these models perform on predicting the test set/later unseen years? (Regression)

## Training & Test split
Training: 2011-2013 & test: 2014-2015. Models are compared using two forward chaining folds inside the
training years (train 2011, validate 2012; train 2011-2012, validate 2013). The test years have not been used yet.

## Folder structure:

data/ CSV files and data README

notebooks/ 01_data_audit_and_baseline.ipynb, 02_model_comparison.ipynb

outputs/ Results table, residual plot and error table written by notebook 02

reports/ Empty for now, not committed

src/ Empty for now, not committed

## Data
Source, citation, licence and collection details are in `data/README.md`.

## Setup:
Tested with Python Version: 3.14.7

```bash
python -m venv .venv
# Windows:      .venv\Scripts\activate
# macOS/Linux:  source .venv/bin/activate
pip install -r requirements.txt
```

## Run Instructions:
1. Activate the virtual environment (see Setup).
2. Run `jupyter notebook`.
3. Open notebooks/01_data_audit_and_baseline.ipynb and choose Kernel -> Restart & Run All.
   The last cell prints the baseline results table.
4. Open notebooks/02_model_comparison.ipynb and choose Kernel -> Restart & Run All.
   It trains gradient boosting and two neural networks, prints the results table and
   saves results.csv, gb_residuals_2013.png and gb_error_by_nox_range_2013.csv to outputs/.