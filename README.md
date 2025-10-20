# Black_Friday_Analysis
Project Overview
This project performs a comprehensive analysis of customer purchase behavior during Black Friday sales events. The analysis explores various demographic factors and their influence on purchasing patterns, providing valuable insights for retail businesses and marketing strategies. Through data-driven exploration, we uncover trends in customer spending across different segments including gender, age groups, occupation, and product categories.
Dataset Information
The dataset used in this project is the Black Friday Sales Dataset, commonly available on Kaggle and other data repositories.
Dataset Characteristics:

Records: ~550,000 purchase transactions
Features: 12 variables including demographic and product information
Key Attributes:

User demographics (Gender, Age, City Category, Stay in Current City)
Product details (Product ID, Product Categories)
Purchase amount
User occupation and marital status



Source: Kaggle - Black Friday Dataset
Objectives
This analysis aims to answer the following key questions:

What demographic factors most significantly influence purchase amounts?
How do spending patterns differ across gender and age groups?
Which product categories generate the highest revenue?
What is the relationship between city category and customer spending?
How does marital status affect purchasing behavior?
Can we predict purchase amounts based on customer attributes?

Data Preprocessing
The following preprocessing steps were performed to ensure data quality:

Missing Value Treatment: Handled missing values in Product_Category_2 and Product_Category_3 columns
Data Type Conversion: Converted categorical variables to appropriate formats
Feature Encoding: Applied label encoding and one-hot encoding for categorical features
Outlier Detection: Identified and analyzed outliers in purchase amounts
Feature Engineering: Created new features from existing variables to enhance analysis
Data Normalization: Scaled numerical features for modeling purposes

Exploratory Data Analysis (EDA)
Key insights discovered through visualization and statistical analysis:
Customer Demographics

Gender Analysis: Male customers constitute the majority of purchases with higher average spending
Age Distribution: The 26-35 age group shows the highest purchase frequency and amount
Marital Status: Single customers tend to make more frequent purchases

Product Insights

Category Performance: Product Category 1, 5, and 8 are the top-selling categories
Price Distribution: Most purchases fall within the $5,000-$15,000 range
Purchase Patterns: Certain product combinations are frequently bought together

Geographic Trends

City Categories: City B shows the highest number of transactions
Stay Duration: Customers staying 1 year in current city exhibit different spending patterns

Modeling
Several machine learning models were implemented to predict purchase amounts:
Models Used

Linear Regression: Baseline model for continuous prediction
Random Forest Regressor: Ensemble method for improved accuracy
XGBoost Regressor: Gradient boosting for optimal performance
Ridge/Lasso Regression: Regularized models to prevent overfitting

Model Evaluation Metrics

Mean Absolute Error (MAE)
Root Mean Squared Error (RMSE)
R² Score
Cross-validation scores

Feature Importance
Analysis revealed that Product Category, Age, and Occupation are among the most influential features in predicting purchase amounts.
Results and Insights
Key Findings

Gender Impact: Male customers spend approximately 1.5x more than female customers on average
Age Factor: The 26-35 demographic represents the sweet spot for high-value purchases
Product Strategy: Focusing on top product categories can maximize revenue
City Dynamics: Urban centers (Category B and C) drive higher transaction volumes
Customer Retention: Length of stay in current city correlates with purchase loyalty

Visualizations

Distribution plots for purchase amounts
Bar charts comparing spending across demographics
Heatmaps showing feature correlations
Box plots identifying spending patterns by category
Time-series analysis of purchase trends

Technologies Used
The project leverages the following Python libraries and tools:

Data Manipulation: pandas, numpy
Visualization: matplotlib, seaborn, plotly
Machine Learning: scikit-learn, xgboost
Statistical Analysis: scipy, statsmodels
Jupyter Environment: jupyter notebook, ipywidgets
Utilities: warnings, os, pickle

How to Run the Notebook
Prerequisites
Ensure you have Python 3.8+ installed on your system.
Step 1: Clone the Repository
bashgit clone <repository-url>
cd black-friday-analysis
Step 2: Create Virtual Environment (Recommended)
bashpython -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
Step 3: Install Dependencies
bashpip install pandas numpy matplotlib seaborn scikit-learn xgboost jupyter
Or use the requirements file:
bashpip install -r requirements.txt
Step 4: Download Dataset

Download the Black Friday dataset from Kaggle
Place the CSV file in the project directory
Update the file path in the notebook if necessary

Step 5: Launch Jupyter Notebook
bashjupyter notebook black_friday_analysis.ipynb
Step 6: Run the Analysis

Open the notebook in your browser
Run all cells sequentially using Shift + Enter
Explore visualizations and results

Future Improvements
This project can be extended in several ways:

Deep Learning: Implement neural networks for more complex pattern recognition
Time Series Analysis: Analyze seasonal trends and forecasting
Customer Segmentation: Apply clustering algorithms (K-Means, DBSCAN) to identify customer segments
Recommendation System: Build a product recommendation engine based on purchase history
A/B Testing: Simulate marketing campaigns and measure effectiveness
Real-time Dashboard: Create an interactive dashboard using Streamlit or Dash
Feature Engineering: Develop more sophisticated derived features
Ensemble Methods: Combine multiple models for better predictions

License
This project is open-source and available under the MIT License.
Author
Haris Ansari

For questions, suggestions, or collaboration opportunities, feel free to reach out!

Acknowledgments
Special thanks to the data science community and Kaggle for providing the dataset that made this analysis possible.