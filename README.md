# Santander Customer Satisfaction

This project aims to predict customer satisfaction using the **Santander Customer Satisfaction dataset**. The analysis includes feature selection, handling dataset imbalance, and training machine learning models to achieve accurate predictions.

## Dataset

The dataset consists of customer-related attributes:

- `train.csv`: Contains features and a target column indicating customer satisfaction (1: Satisfied, 0: Not Satisfied).
- `test.csv`: Includes features for prediction without the target column.

The dataset is imbalanced, with a higher volume of dissatisfied customers.

## Key Steps

### 1. Exploratory Data Analysis (EDA)
- **Target Variable Distribution**: Analyzed the imbalance in the satisfaction data using histograms.
- Identified features with constant or quasi-constant values.

### 2. Feature Selection
- **Quasi-Constant Features**: Removed features with variance below a threshold (0.01).
  - These features provide minimal information and do not contribute significantly to model performance.

### 3. Handling Dataset Imbalance
- Applied techniques to address imbalance, ensuring models are not biased toward the majority class.

### 4. Model Training
- Built and evaluated machine learning models for prediction.
- Focused on achieving a balance between precision and recall due to the imbalanced dataset.

## Requirements

Install the necessary Python libraries:

```bash
pip install pandas numpy scikit-learn matplotlib
```

## Usage

1. Clone the repository:

   ```bash
   git clone https://github.com/Ashray11/Santander-Customer-Satisfaction.git
   cd Santander-Customer-Satisfaction
   ```

2. Run the Jupyter Notebook to reproduce the analysis:

   ```bash
   jupyter notebook santarder-customer-satisfaction.ipynb
   ```

3. Train and test the models using the provided scripts or customize the notebook for further exploration.

## Results

- Insights into customer satisfaction trends.
- Improved model performance by removing redundant features and addressing imbalance.

## Visualization

Graphs and visualizations (e.g., histograms) are included in the notebook to illustrate key findings and model performance.

## Future Work

- Experiment with advanced algorithms such as Gradient Boosting or Neural Networks.
- Explore alternative techniques for handling imbalanced datasets, such as SMOTE or ADASYN.

## Acknowledgments

This project is inspired by the Kaggle competition "Santander Customer Satisfaction."
