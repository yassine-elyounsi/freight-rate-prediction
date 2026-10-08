# Freight Rate Prediction

XGBoost model that predicts `posted_rate` for each load.

## Approach
- EDA, cleaning (negative/missing weight, missing market_index), feature engineering
- Three models: last-3-days test, random 80/20 split, final model on all data
- Metrics: MAE, RMSE, MAPE, WAPE, R2
- Results: <your WAPE and MAPE for models A and B>

## Run
1. Put `train_test.csv`, `validation.csv`, `validation_predictions_template.csv` and `december_chart_inputs.csv` in a path folder.
2. Install dependencies: `pip install -r requirements.txt`
3. Open `Freight_Rate_Full_Notebook.ipynb` and run all cells (Colab or Jupyter). Outputs are written to `outputs/`.


## Files
- `validation_predictions.csv`: final predictions (`load_id,predicted_rate`)
- `scorer_results/candidate_december.png`: December chart from `score.py`
