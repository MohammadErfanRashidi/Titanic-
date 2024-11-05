# Titanic Survival Prediction

This project aims to predict the survival of passengers on the Titanic using machine learning. It uses the Titanic dataset, which contains information about passengers such as age, sex, class, and whether they survived.

## Methodology

1. **Data Loading and Preprocessing:**
   - The `train.csv` file is loaded into a Pandas DataFrame.
   - The 'Cabin' column is dropped due to a large number of missing values.
   - Missing values in the 'Age' column are filled with the mean age.
   - Missing values in the 'Embarked' column are filled with the most frequent value (mode).
   - Categorical features like 'Embarked' and 'Sex' are converted to numerical values using mapping.

2. **Exploratory Data Analysis (EDA):**
   - Several visualizations are created using Seaborn and Matplotlib to explore the data and identify potential relationships between features and survival.
   - Count plots, distribution plots, and heatmaps are used for visualization.

3. **Model Training:**
   - A Logistic Regression model is used for prediction.
   - The dataset is split into training features (X_train) and target variable (Y_train).
   - The model is trained using the training data.

4. **Model Evaluation:**
   - The model's accuracy is evaluated using the training data.

5. **Prediction on Test Data:**
   - The `test.csv` file is loaded.
   - Similar preprocessing steps are applied to the test data.
   - The trained model is used to predict survival for the passengers in the test data.

6. **Output:**
   - The predictions are added to a copy of the test data.
   - The results are saved to a CSV file named `result.csv`.

## Files

- `train.csv`: Training dataset
- `test.csv`: Test dataset
- `result.csv`: Output file containing predictions
- `titanic_prediction.ipynb`: Jupyter Notebook containing the code

## Libraries Used

- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn (LogisticRegression, accuracy_score)

## Author

[Your Name]
