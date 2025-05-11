# House Prices Prediction Project

This project aims to predict house sale prices using various features describing residential homes in Ames, Iowa. The workflow includes data exploration, feature engineering, model training, and generating predictions for submission.

## Dataset

The dataset consists of the following files:
- **`train.csv`**: Training data with 1460 rows and 81 columns (features + target `SalePrice`).
- **`test.csv`**: Test data with 1459 rows and 80 columns (features only, no `SalePrice`).
- **`sample_submission.csv`**: Example format for submission (`Id`, `SalePrice`).
- **`data_description.txt`**: Detailed descriptions of each feature in the dataset.

### Key Features
Some important features include:
- **MSSubClass**: Type of dwelling involved in the sale.
- **MSZoning**: General zoning classification.
- **LotArea**: Lot size in square feet.
- **OverallQual**: Overall material and finish quality.
- **YearBuilt**: Original construction date.
- **GrLivArea**: Above ground living area (sq ft).
- **SalePrice**: Target variable (only in `train.csv`).

For a full list of features and their descriptions, see [`data_description.txt`](data_description.txt).

## Project Workflow

1. **Data Exploration**
   - Load and inspect the data.
   - Visualize feature distributions and relationships.
   - Identify and handle missing values and outliers.

2. **Feature Engineering**
   - Transform or create new features to improve model performance.
   - Encode categorical variables as needed.

3. **Modeling**
   - Split the training data for validation.
   - Train regression models (e.g., Linear Regression).
   - Evaluate model performance using metrics like RMSE.

4. **Prediction & Submission**
   - Generate predictions for the test set.
   - Save results in the format required by `sample_submission.csv` (as `result.csv`).

## How to Run

1. Open `main.ipynb` in Jupyter Notebook or VS Code.
2. Run all cells in order:
   - Data loading and preprocessing
   - Model training and evaluation
   - Prediction and result export
3. The output predictions will be saved as `result.csv`.

## Requirements

Install the following Python libraries:
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

You can install them with:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

## Data Reference

For detailed feature explanations, refer to [`data_description.txt`](data_description.txt).

## Notes
- Ensure all data files are in the same directory as the notebook.
- The notebook is designed for educational and demonstration purposes.
