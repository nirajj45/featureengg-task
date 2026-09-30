# Titanic Feature Engineering & Preprocessing Pipeline

This project is for Internship Task 03: Feature Engineering & Preprocessing Pipeline.

## Files

- `feature_engineering_titanic.ipynb` — main deliverable notebook
- `README.md` — setup and submission notes
- `data/` — optional location for a local `titanic.csv`

## Run in VS Code

1. Open this folder in VS Code.
2. Install the Python and Jupyter extensions.
3. Create/activate a Python virtual environment.
4. Install:
   `pip install pandas numpy matplotlib scikit-learn jupyter ipykernel`
5. Open `feature_engineering_titanic.ipynb`.
6. Select the virtual environment as the notebook kernel.
7. Run all cells.

If `data/titanic.csv` is not present, the notebook downloads the Titanic dataset through Scikit-Learn/OpenML when you run the loading cell.

## What the notebook demonstrates

1. Dataset loading and inspection
2. Data-quality checks
3. Leakage-aware feature selection
4. Train/test split before fitting transformations
5. Feature engineering: `family_size` and `is_alone`
6. Numerical imputation + scaling
7. Categorical imputation + one-hot encoding
8. `ColumnTransformer`
9. End-to-end `Pipeline`
10. Random Forest classification
11. Test-set evaluation
12. Tree-based feature importance
13. Optional permutation importance

## Important

Do not include target-derived Titanic columns such as `alive`, `boat`, or `body` as predictors. They can reveal the outcome and cause target leakage.

The notebook is intentionally written as a reusable baseline rather than a Kaggle competition solution.
