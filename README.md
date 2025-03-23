# Titanic Survival Prediction

## Description
This project performs **Titanic survival prediction** using **Logistic Regression**. The dataset used is the Titanic dataset, which contains information about passengers such as age, sex, class, and whether they survived the disaster. The model is trained to predict survival based on these features.

## Features Used
- **Sex**: Male or Female
- **Pclass**: Passenger class (1st, 2nd, or 3rd)
- **Age**: Age of the passenger
- **Survived**: Whether the passenger survived (1) or not (0)

## Dependencies
Ensure you have the following Python libraries installed:
```sh
pip install numpy pandas seaborn matplotlib scikit-learn
```

## Steps Performed in Code

### 1. **Data Loading**
- The dataset is loaded using Pandas from `Titanic_Data.csv`.
- The first few rows of the dataset are displayed to understand the structure.

### 2. **Data Visualization**
- Seaborn and Matplotlib are used to visualize the survival distribution based on:
  - Overall survival count
  - Survival based on gender
  - Survival based on passenger class
  - Age distribution of passengers

### 3. **Data Cleaning & Preprocessing**
- Unnecessary columns (`zero`, `Sex`, `sibsp`, `Parch`, `Embarked`) are removed.
- Categorical features (`Sex` and `Pclass`) are converted into numerical form using `pd.get_dummies()`.

### 4. **Splitting Data for Training & Testing**
- The dataset is divided into input features (X) and output labels (Y).
- It is further split into training and testing sets using `train_test_split()`.

### 5. **Model Training**
- A **Logistic Regression** model is created using `sklearn.linear_model.LogisticRegression()`.
- The model is trained using the training data.

### 6. **Model Testing & Evaluation**
- The trained model is used to make predictions on the test set.
- The accuracy of the model is evaluated using `accuracy_score()`.
- A confusion matrix is generated using `confusion_matrix()` to analyze performance.

## Running the Code
Execute the Python script using:
```sh
python Titanic_Survival_Prediction.py
```

## Expected Output
- Survival prediction visualizations.
- Accuracy of the model.
- Confusion matrix displaying model performance.

## Author
- **Om Deshmukh**
- Date: **22/03/2025**

