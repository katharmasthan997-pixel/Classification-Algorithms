Classification Algorithms for Crowdfunding Campaign Success Prediction
📌 Project Overview

This project applies machine learning classification algorithms to predict whether a crowdfunding campaign will be successful. Using campaign-related information, the notebook explores the dataset, performs preprocessing, trains multiple classification models, and compares their performance.

The project focuses on understanding how different classification algorithms perform on a binary classification problem.

🎯 Objectives
Explore and understand the crowdfunding dataset.
Perform data cleaning and preprocessing.
Encode categorical variables into numerical values.
Train and evaluate multiple classification algorithms.
Apply cross-validation and hyperparameter tuning.
Compare model performance and identify areas for improvement.
📂 Dataset Description

The dataset contains 100,000 rows and 15 columns related to crowdfunding campaigns.

Important features include:

Feature	Description
CampaignID	Unique campaign identifier
GoalAmount	Target amount for the campaign
RaisedAmount	Amount raised by the campaign
DurationDays	Campaign duration
NumBackers	Number of campaign supporters
Category	Campaign category
LaunchMonth	Month the campaign was launched
Country	Campaign country
Currency	Campaign currency
OwnerExperience	Experience of the campaign owner
VideoIncluded	Whether a campaign video is included
SocialMediaPresence	Social media presence indicator
NumUpdates	Number of campaign updates
IsSuccessful	Target variable indicating campaign success

The target variable is IsSuccessful, a binary variable representing the campaign's success or failure.

Dataset source: Crowdfunding Dataset on GitHub

🛠️ Technologies Used
Python
Pandas
NumPy
Matplotlib
Seaborn
Scikit-learn
Google Colab / Jupyter Notebook
🔍 Project Workflow
1. Data Exploration
Load the crowdfunding dataset.
Examine its dimensions, column names, and data types.
Inspect sample records and categorical variables.
Understand the target variable and feature distribution.
2. Data Preprocessing
Prepare the dataset for machine learning.
Encode categorical features using LabelEncoder.
Exclude identifier and selected campaign outcome-related features from model training.
Apply StandardScaler where appropriate for scale-sensitive algorithms.
3. Model Training

The notebook explores multiple classification algorithms, including:

Random Forest Classifier
K-Nearest Neighbors (KNN)
Decision Tree Classifier
Gaussian Naive Bayes
Support Vector Machine (SVM), including LinearSVC

Each algorithm provides a different approach to learning patterns from the dataset.

4. Model Evaluation

The models are compared using classification evaluation techniques. Cross-validation with StratifiedKFold is used to assess model performance across multiple folds.

5. Hyperparameter Tuning

The notebook applies:

GridSearchCV
RandomizedSearchCV

These techniques search for suitable hyperparameter configurations to improve model performance.

📊 Key Findings
Multiple classification algorithms are evaluated on the crowdfunding campaign dataset.
Cross-validation and hyperparameter tuning are used to compare model configurations.
The tuned LinearSVC model showed slightly better performance in the notebook's comparison.
The observed accuracy was around 50%, indicating that further feature engineering, preprocessing improvements, and model investigation may be needed.

Note: Exact evaluation metrics should be taken from the final executed notebook results.

🚀 Potential Improvements
Investigate class distribution and possible class imbalance.
Review feature encoding and preprocessing choices.
Evaluate feature importance and remove irrelevant features.
Compare precision, recall, F1-score, and ROC-AUC alongside accuracy.
Test additional models and feature engineering strategies.
Investigate possible data leakage and the suitability of the selected input features.
Improve hyperparameter search and cross-validation strategies.
📁 Project Structure
Classification-Algorithms/
│
├── Classificaton_Algorithms.ipynb
└── README.md
▶️ How to Run
Clone or download this repository.
Open Classificaton_Algorithms.ipynb in Google Colab or Jupyter Notebook.
Install the required libraries if they are not already installed.
Run the notebook cells in order.
Review the evaluation results and model comparisons.
📚 Learning Outcomes

Through this project, I practised:

Exploratory data analysis
Data preprocessing and categorical encoding
Classification model training
Model evaluation and cross-validation
Hyperparameter tuning
Comparing machine learning algorithms
👨‍💻 Conclusion

This project demonstrates a practical machine learning workflow for predicting crowdfunding campaign success using classification algorithms. It provides experience in data preparation, model comparison, cross-validation, and hyperparameter optimization, while highlighting opportunities to improve predictive performance.
