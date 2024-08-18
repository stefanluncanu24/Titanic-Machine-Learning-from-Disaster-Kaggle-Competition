# Titanic---Machine-Learning-from-Disaster-Competition
The "Titanic - Machine Learning from Disaster" on Kaggle is a competition where participants use machine learning to predict passenger survival. I'm excited to be in the top 9% of participants!

# Overview of the Project

## File Explanations
- model.ipynb - code used for the project
- submission.csv - file used for the final submission
- test.csv - unlabeled data used for the final submission
- train.csv - labeled data used for training

### Loading Libraries
- Essential libraries such as NumPy, Pandas, Matplotlib, Seaborn, and scikit-learn are loaded for data manipulation, visualization, and machine learning.

### Loading the Data
- The Titanic dataset is loaded from CSV files into Pandas dataframes. Both training and test datasets are concatenated for complete analysis and preprocessing.

### Data Analysis and Preprocessing
- Initial data exploration including statistics and distribution analysis.
- Handling of missing values in 'Age', 'Fare', and 'Embarked' columns.
- Removal of unnecessary features like 'Cabin', 'Ticket', 'PassengerId', and 'Name'.
- Feature engineering includes logging fare to normalize distribution and creating a 'FamilySize' feature.
- Encoding categorical variables such as 'Sex'.

### Model Building
- Splitting the dataset into training and testing sets.
- Several models are trained and evaluated:
  - **Logistic Regression**
  - **XGBoost** with hyperparameter tuning using GridSearchCV.
  - **Random Forest**
  - **Voting Classifier** which includes hard voting of the above models.

### Results and Evaluation
- Performance of models is assessed using accuracy as the metric.
- The final predictions are made using the best-performing model on the unseen test dataset (in this case i chose XGBoost because it gave me the highest score in the competition)

### Submission
- Preparation of submission file for the Kaggle competition.

## Contributions
- Contributions are welcome! Feel free to fork the project, make improvements, and submit a pull request.

