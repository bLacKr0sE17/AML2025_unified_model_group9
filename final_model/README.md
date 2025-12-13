Final Model — AML 2025 (Group 9)

This folder contains the final unified model used for the AML 2025 benchmarking project.

We implement a single tabular learning pipeline that is applied consistently across all three datasets:

HELOC

CoverType

HIGGS

Model

Preprocessing: Mutual Information + PCA

Base models: Logistic Regression, Random Forest, Gradient Boosting, LightGBM

Ensemble: Stacking classifier (Logistic Regression meta-model)

The final model was selected based on baseline comparisons, stacking performance, and targeted stability checks.
All models are trained from scratch using a shared pipeline.

This folder contains only the final training and submission artifacts.
Exploratory and baseline experiments are documented elsewhere in the repository.
