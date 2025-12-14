# AML2025_unified_model_group9
Unified tabular learning model for AML 2025 — Group 9

## Final Model

The final unified LightGBM model and the corresponding Kaggle submission
are located in the `final_model/` directory.

- `AML2025_unified_lightgbm_final_group9.ipynb`: final trained model with preprocessing, weighting, and sanity checks
- `final_submission_unified_tabular_benchmark_group_09.csv`: Kaggle submission file (public score ≈ 0.94)

We explicitly verified the unified label space to ensure correct multiclass training (11 classes total), preventing label collisions or unintended class collapse.

Unique targets: [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
Number of classes: 11


## Baseline Model
The baseline model was imported from dedicated website: https://huggingface.co/alana89/TabSTAR
The final baseline model from Hugging Face and corresponding data are located in the  `baseline_model/` directory. 

- `baseline_model.ipynb`: file with trained baseline model
- `baseline_model.pkl`: baseline model saved as a pickle
- `baseline_test_results_submission.csv`: results a the baseline model submitted to Kaggle (public score = 0.73190)

Unique targets: [0,1,2,3,4,5,6,7,8,9]
Number of classes: 9

The reason for the number of classes between baseline and final model stems from different approaches explored throughout the evaluation of the final model. While for the baseline model, inclusion of only 9 classes (thus merging binary outcomes for higgs + heloc) was most effective, for the final model, use of 11 classes guaranteed the highest prediction.

## Exploratory models
This repository serves a exploratory approach where the datasets were explored and different models compared on performance.
