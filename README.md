# 🚢 Titanic: Machine Learning from Disaster

A machine learning project built for Kaggle's Titanic competition to predict passenger survival using demographic and travel-related features.

## Overview

This project explores the complete machine learning workflow, including:

- Data cleaning
- Exploratory Data Analysis (EDA)
- Feature engineering
- Model training and evaluation
- Kaggle submission generation

The objective is to predict whether a passenger survived the Titanic disaster based on available passenger information.

## Dataset

The dataset is provided by Kaggle's Titanic: Machine Learning from Disaster competition and contains features such as:

- Passenger Class (`Pclass`)
- Name
- Sex
- Age
- Fare
- Cabin
- Embarked
- Siblings/Spouses Aboard (`SibSp`)
- Parents/Children Aboard (`Parch`)
- Ticket Information

## Feature Engineering

Several custom features were created to improve model performance:

- Extracted passenger titles from names (`Mr`, `Mrs`, `Miss`, etc.)
- Created a `FamilySize` feature
- Extracted cabin deck information
- Handled missing values in `Age`, `Fare`, and `Embarked`
- Applied one-hot encoding to categorical variables

## Model

The current implementation uses a Random Forest Classifier with:

- `n_estimators = 400`
- `max_depth = 7`
- `random_state = 42`

Model performance was evaluated using 5-fold cross-validation.

## Project Structure

```text
Titanic-Machine-Learning-Disaster/
│
├── Titanic.ipynb
├── submission.csv
├── README.md
└── images/
```

## Getting Started

Clone the repository:

```bash
git clone https://github.com/your-username/titanic-machine-learning-disaster.git
cd titanic-machine-learning-disaster
```

Install dependencies:

```bash
pip install pandas numpy scikit-learn matplotlib seaborn
```

Run the notebook:

```bash
jupyter notebook
```

Open `Titanic.ipynb` and execute all cells.

## Future Improvements

- Implement XGBoost
- Hyperparameter tuning
- Ensemble learning
- Additional feature engineering techniques

## Author

**Shayan**
