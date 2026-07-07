# Optiver Realized Volatility EDA

Exploratory data analysis for the Optiver Realized Volatility Prediction dataset. The notebook loads the competition train/test data, inspects core fields, checks missing values and outliers, and visualizes relationships between `stock_id`, `time_id`, and the target realized volatility.

## Repository Contents

- `optiver_realized_volatility_eda..ipynb` - main Jupyter notebook for the EDA workflow.
- `README.md` - project overview and usage notes.

## Dataset

This project expects the Optiver Realized Volatility Prediction data files, especially:

- `train.csv`
- `test.csv`

The notebook currently reads data from this Google Drive path:

```python
/content/drive/MyDrive/optiver-realized-volatility-prediction/
```

If you run the notebook locally, update the paths in the data-loading cells to match where you saved the dataset.

## Notebook Workflow

The notebook covers:

1. Loading and checking the data
2. Reviewing variable descriptions
3. Univariate analysis for `stock_id`, `time_id`, and `target`
4. Basic grouped analysis by stock and time
5. Outlier detection using the IQR method
6. Missing value checks
7. Correlation heatmap
8. Bar visualization of `stock_id` versus `target`

## Requirements

The notebook uses Python 3 and the following libraries:

```text
numpy
pandas
matplotlib
seaborn
```

If you are running locally, install them with:

```bash
pip install numpy pandas matplotlib seaborn jupyter
```

## How To Run

1. Download the Optiver Realized Volatility Prediction dataset.
2. Place the CSV files in a local folder or in Google Drive.
3. Open the notebook:

   ```bash
   jupyter notebook "optiver_realized_volatility_eda..ipynb"
   ```

4. Update the `pd.read_csv(...)` paths if needed.
5. Run the notebook cells from top to bottom.

## Notes

- The notebook was written for a Google Colab-style environment and includes a Google Drive mount cell.
- The current project is EDA-focused; it does not train a forecasting model yet.
- The dataset files are not included in this repository.
