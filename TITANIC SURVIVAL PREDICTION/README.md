Titanic Survival Prediction:


This project demonstrates how to predict survival on the Titanic using machine learning, 
specifically with a Random Forest Classifier. The following steps were performed:

Data Loading:

The dataset was loaded into a Pandas DataFrame from a CSV file.

Data Preprocessing:

Missing values in the Age, Embarked, and Fare columns were handled by filling with median and mode values respectively.
Irrelevant columns (PassengerId, Name, Ticket, Cabin) were removed to simplify the dataset.
Categorical variables (Sex, Embarked) were encoded as numerical values.

Data Splitting:

The data was split into features (X) and target variable (Survived), followed by a training-validation split (80-20).

Model Building:

A RandomForestClassifier was used to train the model on the training data.
The model made predictions on the validation set.

Model Evaluation:

The model's performance was evaluated using accuracy and a confusion matrix.
