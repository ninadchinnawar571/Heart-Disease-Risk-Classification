# Heart Disease Risk Classification

## Overview
Heart Disease Risk Classification is a machine learning project that compares Support Vector Machine (SVM) and K-Nearest Neighbors (KNN) algorithms to classify heart disease outcomes using clinical data.

The project focuses on data preprocessing, feature analysis, dimensionality reduction, hyperparameter tuning, and model evaluation.

## Objectives
- Analyze and preprocess the heart disease dataset.
- Explore feature relationships using correlation analysis.
- Standardize features using `StandardScaler`.
- Apply Principal Component Analysis (PCA) for dimensionality reduction.
- Train and compare SVM and KNN classification models.
- Optimize model hyperparameters using `GridSearchCV`.
- Evaluate models using accuracy, recall, precision, F1-score, and confusion matrices.

## Technologies and Libraries
- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

## Project Workflow
1. Import the required Python libraries.
2. Load and inspect the heart disease dataset.
3. Check for missing values, duplicate records, and class distribution.
4. Perform exploratory data analysis and correlation analysis.
5. Split the dataset into training and testing sets.
6. Standardize features and analyze PCA explained variance.
7. Build SVM and KNN pipelines.
8. Tune model parameters using cross-validation and `GridSearchCV`, with recall as the primary optimization metric.
9. Evaluate and compare the models on the test dataset.
10. Visualize model performance and summarize the results.

## Models Used

### Support Vector Machine (SVM)
SVM is a supervised learning algorithm that finds a decision boundary to separate classes. The project evaluates different kernels and hyperparameter combinations.

### K-Nearest Neighbors (KNN)
KNN predicts a class based on the labels of nearby training samples. The project evaluates different neighbor counts, distance weighting methods, and distance metrics.

## Evaluation Metrics
- **Accuracy:** Overall proportion of correct predictions.
- **Recall:** Proportion of actual positive cases correctly identified.
- **Precision:** Proportion of predicted positive cases that are actually positive.
- **F1-score:** Harmonic mean of precision and recall.
- **Confusion Matrix:** Displays correct and incorrect predictions by class.

Recall is used as the primary metric during hyperparameter tuning because missing a positive case can be important in a medical classification task.

## Dataset
The notebook loads a CSV file named `heart.csv` and expects the target column to be named `target`.

Place the dataset in the same directory as the notebook before running it.

Use a dataset that you are permitted to access and redistribute. Do not upload private or identifiable patient information.

## Installation and Setup

### 1. Clone the repository
```bash
git clone https://github.com/YOUR-USERNAME/Heart-Disease-Risk-Classification.git
cd Heart-Disease-Risk-Classification
```

### 2. Create a virtual environment (recommended)
```bash
python -m venv .venv
```

Activate it on Windows:
```bash
.venv\Scripts\activate
```

### 3. Install the dependencies
```bash
pip install numpy pandas matplotlib seaborn scikit-learn jupyter
```

### 4. Launch Jupyter Notebook
```bash
jupyter notebook
```

Open `Heart_Disease_Risk.ipynb` and run the cells in order after placing `heart.csv` in the project directory.

## Repository Structure
```text
Heart-Disease-Risk-Classification/
├── Heart_Disease_Risk.ipynb
├── heart.csv
├── README.md
└── .gitignore
```

## Results
The notebook calculates and compares SVM and KNN performance using cross-validation and test-set evaluation. Refer to the notebook outputs for the actual scores and selected hyperparameters.

## Limitations
- Model predictions depend on the quality and representativeness of the dataset.
- Results on a test dataset do not guarantee performance on real-world patients.
- This project is for educational purposes and is not a medical diagnostic tool.

## Future Improvements
- Test the models on additional datasets.
- Add further validation and error analysis.
- Develop a user interface for demonstrating predictions.
- Document model limitations and evaluation results in greater detail.

## Author
Ninad Chinnawar
## Disclaimer
This project is intended for learning and research purposes only. It must not be used as a substitute for professional medical advice or diagnosis.
