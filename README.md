# Interactive SHAP Explanations for a Diabetes Prediction Model

## Project Overview
This project demonstrates how machine learning predictions can be explained using SHAP (SHapley Additive exPlanations). A Gradient Boosting Regressor is trained on the diabetes dataset, and SHAP visualizations are used to understand how individual features influence model predictions.

## Objectives
- Load and explore the diabetes dataset.
- Train a Gradient Boosting Regression model.
- Evaluate the model using Mean Squared Error (MSE) and R² score.
- Explain model predictions using SHAP.
- Generate summary and individual prediction visualizations.
- Save predictions and visualizations for further analysis.

## Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- SHAP
- Jupyter Notebook

## Dataset
The project uses the diabetes dataset provided by `sklearn.datasets.load_diabetes`. It contains 442 samples and 10 input features.

## Model
A `GradientBoostingRegressor` is trained using an 80/20 train-test split with a fixed random state of 42.

## Explainability
SHAP is used to generate:
- A summary beeswarm plot to examine feature contributions across test samples.
- A waterfall plot to explain the contribution of features to an individual prediction.

## Evaluation Metrics
- Mean Squared Error (MSE)
- R² Score

Actual evaluation values are displayed when the notebook runs.

## Output Files
The notebook saves these files in the `outputs/` directory:
- `predictions.csv`
- `shap_summary.png`
- `individual_explanation.png`

## How to Run

1. Clone or download this repository.
2. Create and activate a Python virtual environment.
3. Install the dependencies:
   `pip install -r requirements.txt`
4. Open `diabetes_shap_explainer.ipynb` in VS Code or Jupyter Notebook.
5. Select the project's Python environment as the notebook kernel.
6. Run the notebook cells in order.

## Disclaimer
This project is for educational and machine learning explainability purposes. It is not a medical diagnostic tool.