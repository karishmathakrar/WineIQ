# WineIQ: Predicting Wine Quality Using Machine Learning

This project aims to predict the quality of Portuguese "Vinho Verde" red wines based on their chemical properties using various machine learning techniques.

## Project Overview

- **Objective**: To develop predictive models that classify wine quality as "good" or "not good" based solely on physicochemical properties.
- **Dataset**: Contains 1,599 samples of red wine with 11 features such as acidity, pH, alcohol content, etc.
- **Models Used**:
  - Logistic Regression
  - K-Nearest Neighbors (KNN)
  - Support Vector Classifier (SVC)
  - Stochastic Gradient Descent (SGD)
  - Random Forest
  - Gradient Boosting
- **Feature Engineering**:
  - Introduced interaction terms between highly correlated features.
  - Removed redundant features to reduce multicollinearity.

## Results

- **Best Performing Model**: Random Forest Classifier
- **Accuracy**: 92% (before and after feature engineering)
- **Key Features**:
  - **Before Feature Engineering**:
    - Alcohol
    - Volatile Acidity
    - Sulphates
  - **After Feature Engineering**:
    - Alcohol
    - Volatile Acidity
    - Interaction of Volatile Acidity and Citric Acid

## Repository Contents

- `A5_final.ipynb`: Jupyter Notebook containing the data analysis, model training, and evaluation.
- `winequality-red.csv`: The dataset used for this project.
- `README.md`: Project overview and instructions (this file).
- `.gitignore`: Specifies intentionally untracked files to ignore.

## Getting Started

### Prerequisites

- Python 3.x
- Jupyter Notebook or JupyterLab

### Installation

1. **Clone the repository**:

   ```bash
   git clone https://github.com/karishmathakrar/WineIQ.git
   cd WineIQ

2. Create and activate a virtual environment (optional but recommended):

python -m venv .venv
# On Windows
.venv\Scripts\activate
# On macOS/Linux
source .venv/bin/activate

3. Install required packages:
pip install -r requirements.txt

4. Launch Jupyter Notebook:
jupyter notebook A5_final.ipynb

Usage
Run the cells in A5_final.ipynb sequentially to reproduce the analysis.
Modify parameters or models as desired to experiment with different configurations.
Citation
Please include this citation if you plan to use this dataset:

P. Cortez, A. Cerdeira, F. Almeida, T. Matos, and J. Reis. Modeling wine preferences by data mining from physicochemical properties. In Decision Support Systems, Elsevier, 47(4):547-553, 2009.

Acknowledgments
Dataset Source: UCI Machine Learning Repository and Kaggle
Inspiration: To provide winemakers with a data-driven approach to assess wine quality based on chemical properties.
