# Insurance Claim Prediction

Educational machine learning project by Nivedha Sivakumar.

## Changes from the saved notebook
- Updated pandas drop syntax
- Replaced row-order split and unused remainder with a stratified holdout
- Excluded billed charges because availability before a claim is unestablished
- Used training-fitted scaling and one-hot encoding for nominal region, sex, and smoker categories
- Added baseline, per-class metrics, ROC AUC and average precision
- Removed obsolete split descriptions and unverified coefficient conclusions

## Run locally
Use Python 3.12, install `pip install -r requirements.txt`, and place an authorized copy of `insurance2.csv` beside the notebook (or in `data/` as shown). Dataset redistribution rights have not been established, so input data is not included. Run all notebook cells in order.

## Validation
Executed successfully top-to-bottom on the local source data using Python 3.12. Exact tested package versions are recorded in requirements-lock.txt. Saved charts were visually reviewed. Historical output claims have been removed; new conclusions must follow the revised evaluation.

## Limits
This is a learning project, not a deployed decision system. Holdout scores do not establish external validity, fairness, or causal effects. 

## Observed results

The revised held-out ROC AUC is 0.899 and average precision is 0.941, with a majority-class baseline accuracy of 58.5%. The target construction and feature observation timing are not verified. Charges were excluded; this remains a course-data experiment, not an underwriting or claim decision tool.
