# Using Sensor Measurements to Predict NOx Emissions from a Gas Turbine

## Repo Link
https://github.com/TripO7/CT4101-ML

## Research Question
Using trained models & sensor measurements, how accurately could we predict the hourly NOx emissions from a gas
turbine and how would these models perform on predicting the test set/later unseen years? (Regression)

## Training & Test split
training and test split is: training: 2011-2013 & test: 2014-2015

## Folder structure: 

data/ CSV files and data README

notebooks/ 01_data_audit_and_baseline.ipynb

reports/ Empty for now, not commited

src/ Empty for now, not commited

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
2. Run `jupyter notebook` and open `notebooks/01_data_audit_and_baseline.ipynb`.
3. Choose Kernel -> Restart & Run All.
4. The last cell prints the baseline results table.