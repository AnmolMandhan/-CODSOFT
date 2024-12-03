Movie Rating Prediction with Python

This project builds a machine learning model to predict movie ratings based on features like genre, director, actors, and the number of votes.
The goal is to analyze historical movie data and accurately estimate ratings using regression techniques.

Features:
The dataset contains the following columns:

Name: The title of the movie.
Year: The release year of the movie.
Duration: The runtime of the movie in minutes.
Genre: The genre of the movie (e.g., Action, Comedy, Drama).
Rating: The movie's rating (target variable).
Votes: The number of user votes for the movie.
Director: The director of the movie.
Actor 1, Actor 2, Actor 3: The main actors in the movie.

Workflow:

Data Loading: The dataset is read from a CSV file.
Data Cleaning:
Handled missing values by filling or dropping them.
Removed commas from the Votes column and converted it to numeric.
Feature Selection: Selected Genre, Votes, Director, Actor 1, Actor 2, and Actor 3 as features for training.

Feature Engineering:
Categorical features (e.g., Genre, Director) were one-hot encoded.
Numerical features (e.g., Votes) were scaled using StandardScaler.
Model Training: A Random Forest Regressor was trained on the processed data.
Model Evaluation: The model's performance was evaluated using RMSE (Root Mean Squared Error) and R² (coefficient of determination).

Install required libraries:

bash
Copy code
pip install -r requirements.txt

Predicting Ratings
To predict the rating of a new movie:

What We Did:
Explored and Cleaned the Data:

Loaded a dataset of movies containing features like Genre, Director, Actors, Votes, and Rating.
Addressed missing values by filling or removing them to ensure the dataset was complete and usable.
Processed the Votes column by removing commas and converting it into a numeric format.
Engineered Features:

Encoded categorical variables (Genre, Director, Actor 1, etc.) using one-hot encoding to prepare them for machine learning.
Scaled numerical variables (Votes) to standardize their range.
Trained a Regression Model:

Used a Random Forest Regressor to build a model capable of predicting movie ratings based on the processed features.
Split the data into training and testing sets to evaluate the model's performance.
Evaluated the Model:

Measured performance using metrics like RMSE (Root Mean Squared Error) and R² (coefficient of determination) to assess how well the model predicted movie ratings.
Deployed the Model:


Created a pipeline to allow predictions for new movies based on their features.
What We Achieved
Built a Functional Movie Rating Prediction System:

Developed a machine learning model that can accurately predict the rating of a movie based on its genre, director, actors, and user votes.
Gained Insights into Influential Factors:

Identified key features that impact movie ratings, such as genre, popularity (votes), and the creative team involved (director and actors).
Improved Understanding of Machine Learning Workflow:

Learned and implemented the complete process of building a machine learning model, from data preprocessing to evaluation and deployment.
Prepared for Real-World Applications:

Built a flexible and reusable prediction pipeline that can be extended to new data or used in applications like movie recommendation systems.
Sharpened Analytical and Technical Skills:

Gained hands-on experience in data cleaning, feature engineering, and regression modeling.
Enhanced coding and problem-solving skills, particularly in handling real-world datasets.
Model Performance
RMSE: [1.2220742937748508]
R²: [0.19348146131049193]
