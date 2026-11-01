## Research Question
Using trained models & sensor measurements, how accurately could we predict the hourly NOx emissions from a gas
turbine and how would these models perform on predicting the test set/later unseen years? (Regression)

Source: https://doi.org/10.24432/C5WC95

Citation: Kaya, H., Tüfekci, P., & Uzun, E. (2019). Predicting CO and NOx emissions from gas turbines: novel data and
a benchmark PEMS. Turkish Journal of Electrical Engineering & Computer Sciences, 27(6), 4783-4796.
https://doi.org/10.3906/elk-1807-87

The data was collected from 2011-2015, there are 36733 instances of 11 sensor measures aggregated over one hour (by means of average or sum) from a gas turbine located in Turkey's north western region.

Dataset is in /data & training and test split is: training: 2011-2013 & test:2014-2015

Python Version: 3.14.7

## Folder structure: 

data/ 

notebooks/ 

reports/

src/

## Setup:

python -m venv .venv

Windows:      .venv\Scripts\activate

macOS/Linux:  source .venv/bin/activate
pip install -r requirements.txt

jupyter notebook

## Run Instructions:
