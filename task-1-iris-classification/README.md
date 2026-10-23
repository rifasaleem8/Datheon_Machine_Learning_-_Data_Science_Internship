# Multi-Class Benchmark Classification Pipeline

## Project Overview

This project implements and compares two machine learning classification algorithms, Logistic Regression and Decision Tree, using the Iris dataset.

The objective is to build an end-to-end classification pipeline, explore the dataset, train the models, evaluate their performance using multiple classification metrics, and visualize their decision boundaries.

## Dataset

- **Dataset:** Iris flower dataset
- **Source:** [Seaborn Iris Dataset](https://raw.githubusercontent.com/mwaskom/seaborn-data/master/iris.csv)
- **Target variable:** `species`
- **Features:** `sepal_length`, `sepal_width`, `petal_length`, `petal_width`
- **Classes:** Setosa, Versicolor, Virginica

The dataset contains measurements of iris flowers belonging to three species.

## Technologies Used

- Python
- Pandas
- Matplotlib
- Seaborn
- Scikit-Learn
- Jupyter Notebook

## Project Workflow

1. **Data Loading:** Loaded the Iris dataset using Pandas.
2. **Exploratory Data Analysis:** Inspected dataset dimensions, data types, missing values, duplicate rows, class distributions, and feature relationships.
3. **Data Cleaning:** Removed one duplicate row and verified that no duplicate rows remained.
4. **Feature and Target Separation:** Separated the four numerical features from the target species.
5. **Train-Test Split:** Split the data into 80% training data and 20% testing data using stratified sampling.
6. **Model Development:** Trained Logistic Regression using a Scikit-Learn pipeline with StandardScaler and trained a Decision Tree classifier.
7. **Model Evaluation:** Evaluated both models using accuracy, macro precision, macro recall, macro F1-score, and confusion matrices.
8. **Model Comparison:** Compared the performance metrics and predictions of both classifiers.
9. **Decision Boundary Visualization:** Visualized how Logistic Regression and Decision Tree classify observations using petal length and petal width.

## Machine Learning Models

### 1. Logistic Regression

A classification algorithm used to predict the species of an iris flower. StandardScaler was included in a Scikit-Learn pipeline to standardize the numerical features before classification.

### 2. Decision Tree Classifier

A tree-based classification algorithm that learns decision rules from the training data to classify iris species.

## Model Evaluation Results

Both models were evaluated on the same test set of 30 observations.

| Metric | Logistic Regression | Decision Tree |
|---|---:|---:|
| Accuracy | 0.9333 | 0.9333 |
| Macro Precision | 0.9333 | 0.9333 |
| Macro Recall | 0.9333 | 0.9333 |
| Macro F1-score | 0.9333 | 0.9333 |

Both classifiers achieved **93.33% accuracy**, correctly predicting 28 out of 30 test observations. They also produced the same predictions on this test split.

## Visualizations

The project includes:

- Pairplot to explore relationships between numerical features.
- Boxplots to compare petal length and petal width across species.
- Confusion matrices to examine correct and incorrect classifications.
- Decision boundary plots to visualize the classification regions of both models using two features.

## Key Learnings

- Performing exploratory data analysis before model training.
- Identifying and handling duplicate records.
- Separating features and target variables.
- Using stratified train-test splitting.
- Building a Scikit-Learn pipeline with feature scaling.
- Training and evaluating different classification algorithms.
- Interpreting accuracy, precision, recall, F1-score, and confusion matrices.
- Visualizing decision boundaries and comparing classifier behavior.

## Conclusion

Both Logistic Regression and Decision Tree achieved the same evaluation scores on the selected test set. The results demonstrate how two different classification algorithms can perform similarly on the same dataset.

The decision boundary visualizations illustrate how each model separates the three iris species using petal measurements.

These results are based on one train-test split. Further evaluation using cross-validation and different splits would help assess the consistency of the models' performance.

## How to Run

1. Clone or download this repository.
2. Install the required Python libraries.
3. Open `iris_classification.ipynb` in Jupyter Notebook or JupyterLab.
4. Run the notebook cells in order.

Install the dependencies with:

```bash
pip install pandas matplotlib seaborn scikit-learn jupyter
```

---

**Project Type:** Machine Learning — Multi-Class Classification

**Status:** Completed
