
# American Express - Default Prediction Project README

## Introduction
This project focuses on predicting credit card defaults using the American Express dataset. The process involves data preprocessing, feature engineering, model training using LightGBM and XGBoost, and finally, making predictions for submission.

## Prerequisites
- Minimum 64GB RAM recommended
- Python environment
- Familiarity with Python and Jupyter Notebooks

## Key Dependencies
- pandas
- numpy
- lightgbm
- pyarrow
- pickle
- tqdm

Install these Python packages using the following command:
```bash
pip install pandas numpy lightgbm pyarrow pickle tqdm
```

## Dataset Download
Download the processed American Express dataset in Parquet format from [this link](https://www.kaggle.com/datasets/raddar/amex-data-integer-dtypes-parquet-format).

## Steps to Run the Project

### 1. Feature Processing
- **Script**: `code/fe_process.py`
- **Purpose**: Generates Parquet feature files. This step requires significant processing time.

### 2. Model Training with LightGBM
- **Script**: `code/lgb.py`
- **Note**: A pre-trained model file is provided due to the long training time.

### 3. Model Training with XGBoost
- **Script**: `code/xgb.py`

### 4. Inference and Results Merging
- **Notebook**: `code/infer.ipynb`
- Generates the final prediction result by merging models.

### 5. Submission
- Submit the `result/sub/submission.csv` file to Kaggle.

## Additional Notes
- The project requires extensive computational resources. Ensure that your system meets the memory and processing requirements.
- Due to the large size of the dataset and extensive processing, some steps might take a long time to complete.

