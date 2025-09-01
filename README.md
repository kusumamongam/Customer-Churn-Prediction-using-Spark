# Customer-Churn-Prediction-using-Spark


This project focuses on predicting customer churn in a banking dataset using Apache Spark for distributed data processing and PySpark MLlib for machine learning. The goal is to build models that can identify customers who are likely to leave (churn) based on their demographic and financial details.

#📂 Dataset

The dataset contains customer details such as:

Customer ID, Surname, Age, Gender, Geography

Credit Score, Balance, Tenure, Number of Products

Credit Card Ownership, Active Membership, Estimated Salary

Target Column: Exited (1 = Churn, 0 = Retained)

#⚙️ Tools & Libraries Used

Python (Google Colab environment)

Apache Spark / PySpark

SparkSession for managing Spark jobs

pyspark.sql.functions for transformations

VectorAssembler for feature engineering

LogisticRegression, RandomForestClassifier, DecisionTreeClassifier, GBTClassifier for modeling

MulticlassClassificationEvaluator for evaluation

Google Colab (for execution and dataset handling)

#🔄 Project Workflow

Data Loading & Cleaning

Load dataset into Spark DataFrame

Handle missing values using na.drop()

Feature Engineering

Select key features (Age, Balance, EstimatedSalary)

Assemble features into a single vector using VectorAssembler

Model Training

Train models including Logistic Regression and Random Forest

Use an 80:20 train–test split

Model Evaluation

Evaluate models with F1 Score and Accuracy

Example results:

Logistic Regression → F1 Score: ~0.71, Accuracy: ~77.8%

Random Forest → F1 Score: ~0.78, Accuracy: ~81.0%

Prediction

Generate churn predictions with probability scores

#📖 Future Improvements

Include more features from the dataset for better accuracy

Tune hyperparameters using cross-validation

Implement Gradient Boosted Trees and Ensemble Models

Deploy as a web API for real-time predictions
