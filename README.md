# Gold Recovery Process Optimization

This project focuses on predicting gold recovery efficiency using industrial process data from multiple purification stages. The goal is to build reliable regression models while addressing real-world challenges such as delayed measurements, missing features, data leakage risk, and anomalous values.

## Dataset
The data consists of three datasets:
- Training dataset
- Test dataset (features only, no targets)
- Full source dataset with all available features

Data is time-indexed, and some parameters are unavailable at prediction time due to delayed measurement.

## Key Objectives
- Validate gold recovery calculations and ensure target correctness
- Analyze metal concentration behavior (Au, Ag, Pb) across processing stages
- Identify and remove anomalous or non-physical values
- Prevent data leakage by comparing feature availability between train and test sets
- Train and evaluate regression models using appropriate industrial metrics

## Approach
- Performed exploratory data analysis to understand concentration trends and total substance distributions
- Validated recovery metrics using Mean Absolute Error (MAE)
- Cleaned and preprocessed data to handle missing, delayed, and inconsistent features
- Trained and compared multiple regression models using cross-validation
- Evaluated model performance using a custom sMAPE metric
- Tested the final model on a holdout dataset

## Tools & Technologies
- Python
- pandas, NumPy
- scikit-learn
- Matplotlib, Seaborn

## Results
The final model demonstrates stable predictive performance on unseen data and highlights the importance of rigorous data validation and leakage prevention when working with industrial process datasets.

## Key Takeaways
- Industrial data requires extensive validation before modeling
- Feature availability timing is critical for fair model evaluation
- Proper preprocessing and anomaly handling significantly improve model reliability
