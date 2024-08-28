# Mushroom-Classification
A model that can classify mushrooms as edible ('e') or poisonous ('p') using a set of physical attributes provided in the dataset.

# Mushroom Classification for Prediction Submission and EDA with MCC Coefficient

This repository contains a Kaggle notebook focused on the classification of mushrooms using machine learning. The project involves extensive Exploratory Data Analysis (EDA) and model evaluation, with a specific emphasis on the Matthews Correlation Coefficient (MCC) for assessing model performance. The final goal is to generate accurate predictions for submission to a Kaggle competition.

The Kaggle Notebook Link: https://www.kaggle.com/code/nareshkmr/mushroom-classification-analysis/notebook
## Table of Contents

- [Overview](#overview)
- [Dataset](#dataset)
- [Installation](#installation)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Feature Engineering](#feature-engineering)
- [Modeling](#modeling)
- [Evaluation](#evaluation)
- [Prediction Submission](#prediction-submission)
- [Results](#results)
- [Conclusion](#conclusion)
- [Future Work](#future-work)
- [Contributing](#contributing)
- [License](#license)

## Overview

This project is dedicated to predicting whether a mushroom is edible or poisonous based on various physical features. The analysis leverages the Matthews Correlation Coefficient (MCC) as the primary evaluation metric to ensure balanced model performance across both classes. The notebook also provides detailed EDA, feature engineering, and modeling steps, culminating in a prediction submission for a Kaggle competition.

## Dataset

The dataset used in this project is a modified version of the original UCI Mushroom dataset, and includes features such as:
- **Cap shape**
- **Cap color**
- **Gill size**
- **Stalk shape**
- **Spore print color**
- **Odor**
- And more.

The target variable is binary:
- `e` for edible
- `p` for poisonous

## Installation

To run this notebook, you'll need Python and several packages. You can install the necessary packages using the following command:

```bash
pip install -r requirements.txt
```

The required packages include:
- `pandas`
- `numpy`
- `scikit-learn`
- `matplotlib`
- `seaborn`
- `xgboost`
- `lightgbm`

## Exploratory Data Analysis (EDA)

The EDA section explores the dataset and identifies key patterns that could influence the classification task. It includes:
- **Data Cleaning:** Handling missing values and correcting data inconsistencies.
- **Visualizations:** Using Crosstab, Sunburst, Sankey charts, and other visual tools to understand the relationship between features like cap shape and cap color.
- **Correlation Analysis:** Identifying feature correlations and their impact on the target variable.

## Feature Engineering

This section covers the creation of new features or the transformation of existing ones to enhance model performance. Techniques such as one-hot encoding, label encoding, and interaction terms are explored.

## Modeling

Several machine learning models are implemented and tuned, including:
- **Support Vector Machines (SVM)**
- **Decision Trees**
- **Random Forest**
- **XGBoost**
- **LightGBM**

The models are selected based on their performance in terms of the MCC score, which is particularly effective for evaluating binary classification tasks with imbalanced datasets.

## Evaluation

The models are evaluated using the Matthews Correlation Coefficient (MCC) along with other metrics such as accuracy, precision, recall, and F1-score. The MCC is emphasized as it provides a more reliable measure of model performance in scenarios where class distribution may be imbalanced.

## Prediction Submission

The notebook generates predictions for the test set, which are formatted according to the Kaggle competition requirements. The submission file includes the following:
- **ID:** Unique identifier for each mushroom instance.
- **Prediction:** The predicted class (`e` or `p`).

The submission process is outlined step-by-step, ensuring the final file meets all Kaggle requirements.

## Results

The results section summarizes the performance of the models, with a particular focus on:
- **Confusion Matrix:** Visualizing true positives, true negatives, false positives, and false negatives.
- **Feature Importance:** Ranking features based on their contribution to the model.
- **Model Comparison:** Comparing the MCC and other metrics across different models.

## Conclusion

This project successfully demonstrates the use of machine learning to classify mushrooms as either edible or poisonous. By focusing on the MCC, the analysis ensures a balanced and reliable performance across both classes, making it a robust solution for this classification task.

## Future Work

Possible future directions for the project include:
- **Hyperparameter Tuning:** Further optimizing model parameters for better performance.
- **Ensemble Techniques:** Exploring stacking, blending, or other ensemble methods to improve accuracy.
- **Deep Learning Models:** Experimenting with neural networks to potentially increase model precision.
- **External Datasets:** Incorporating additional data sources to enhance generalizability.

## Contributing

Contributions to this project are welcome. If you have suggestions for improvements or new features, please submit a pull request or open an issue.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

This README template is designed to reflect the specific details and focus areas of your project, such as the use of the MCC for evaluation and the preparation of a prediction submission for Kaggle. Adjust any sections as necessary to align with your work.
