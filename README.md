# Titanic Survival Prediction

## Project Overview
This project aims to predict whether a passenger survived the Titanic disaster using machine learning classification techniques. The dataset contains various features such as age, gender, ticket class, fare, and others, and the task is to build a classification model to predict the survival of passengers.

## Dataset
The Titanic dataset contains the following features:
- `PassengerId`: Unique identifier for each passenger
- `Pclass`: Ticket class (1 = First Class, 2 = Second Class, 3 = Third Class)
- `Sex`: Gender of the passenger (male/female)
- `Age`: Age of the passenger (in years)
- `SibSp`: Number of siblings or spouses aboard the Titanic
- `Parch`: Number of parents or children aboard the Titanic
- `Fare`: Fare paid for the ticket
- `Embarked`: Port of embarkation (C = Cherbourg, Q = Queenstown, S = Southampton)
- `Survived`: Whether the passenger survived (1 = Survived, 0 = Did not survive)

## Steps Taken
### 1. Data Preprocessing:
- **Missing Values Handling**: 
  - `Age` and `Fare` were imputed using KNN imputation.
  - `Embarked` missing values were filled with the most frequent value.
- **Feature Engineering**: 
  - Categorical features such as `Sex` were mapped to 0 and 1.
  - One-hot encoding was applied to the `Embarked` feature.
- **Feature Scaling**: 
  - Numerical features `Age` and `Fare` were scaled using `StandardScaler`.

### 2. Model Building:
- **Model Selection**: 
  - A **Random Forest Classifier** was chosen for model training.
- **Data Splitting**: 
  - The dataset was split into training and testing sets (80% training, 20% testing).
  
### 3. Model Evaluation:
- **Metrics Used**:
  - Accuracy, Precision, Recall, F1-Score, and ROC-AUC were used to evaluate the model's performance.
- **Confusion Matrix**:
  - A confusion matrix was plotted to visualize the model's prediction performance.

## Model Performance
- **Accuracy**: [Insert your accuracy score here]
- **Precision, Recall, F1-Score**: [Insert classification report here]
- **ROC AUC**: [Insert AUC score here]

## Instructions to Run
1. Clone this repository:
   ```bash
   git clone https://github.com/bhavyasri117/Titanic-Survival-Prediction.git
