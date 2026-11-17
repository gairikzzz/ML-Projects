# Cognitare – Round 2 Submission

This folder contains the materials for the Cognitare Round 2 submission, including the notebooks, model workflow, input and test data, and saved model artefact.

## Modelling note: feature availability and leakage risk

The original model used `AVG_DOWNHOLE_TEMPERATURE`. In the prediction dataset, this feature was zero for every record, raising a concern about whether the feature would be available in a real prediction setting and whether it could introduce data leakage.

As a check, a second model was built using `AVG_DP_TUBING` in place of `AVG_DOWNHOLE_TEMPERATURE`. The two sets of predictions were reported as close, with an accuracy of **88%**. The original submission selected the first model because it had the higher reported accuracy.

This is the rationale recorded in the original submission; the notebooks and data files contain the underlying work and should be consulted when assessing the modelling decision.

## Files

- `COGNITARE_GAIRIKCHAKRABORTY_SUBMISSIONS.ipynb` — notebook submission
- `COGNITARE_GAIRIKCHAKRABORTY_SUBMISSION - Jupyter Notebook.pdf` — exported submission
- `ML model workflow.jpeg` — model workflow visual
- `input_data_quiz.xlsx`, `test_data_quiz.xlsx`, `Test_data_quiz_results.xlsx` — supporting data files
- `Volve Oilfield.jpg` — supporting image
- `model.pkl` — saved model artefact
