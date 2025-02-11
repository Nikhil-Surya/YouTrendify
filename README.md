# YouTrendify: YouTube Insights Engine

## 🚀 Project Overview
YouTrendify is a machine learning-based engine designed to analyze YouTube video trends, providing valuable insights into factors that drive subscriber growth, video popularity, and potential revenue generation. By leveraging a rich dataset of YouTube channel statistics, YouTrendify enables content creators, advertisers, and researchers to make data-driven decisions.

## 🎯 Motivation
Understanding the factors influencing YouTube video success is crucial for:

+ Creators to enhance content strategy and estimate revenue.  
+ Businesses to target the right influencers for marketing.  
+ Researchers to analyze trends and content dynamics.  
+ Viewers to explore trending and engaging content.

## 📊 Dataset
The project utilizes the Global YouTube Statistics 2023 dataset from Kaggle, containing 995 rows and 28 features, such as:

Channel Title, Category, Video Views, Rank, Earnings, Country, and Subscribers (Target Feature)  
Subscriber Growth Trends over 30 Days  
Geographical and Content-Based Rankings

### 🛠 Data Preprocessing
To ensure the dataset was clean and reliable, we applied:

+ Handling Missing Values: Replacing numerical values with column means.  
+ Duplicate Removal: Eliminating redundant records.  
+ Feature Encoding: Applying label encoding to categorical columns.  
+ Outlier Removal: Filtering extreme values for better model accuracy.  
+ Feature Scaling: Standardization and normalization techniques.

### 📈 Exploratory Data Analysis (EDA)
Several key insights were derived from EDA:

1. Top 10 YouTube Channels by Subscribers: A bar graph showing major content creators.
   ![image](https://github.com/user-attachments/assets/ab78133d-092d-4252-8dcf-fce471cb9e84)

2. Top 10 Channels by Revenue: Highlighting the financial potential of YouTube.
   ![image](https://github.com/user-attachments/assets/a52a6c57-9962-4b23-89e3-f5c9c8583791)

3. Correlation Analysis: Identifying feature relationships and impact on subscriber count.
   ![image](https://github.com/user-attachments/assets/eee7765f-74a6-4c61-88ae-dc2cf1562838)

### 🔍 Feature Selection
Key features chosen for model training:

+ Video Views 📽 (Higher views correlate with more subscribers)  
+ Rank 📊 (Top-ranked YouTubers attract more subscribers)  
+ Highest Monthly Earnings 💵 (High revenue signals strong subscriber engagement)  
+ Population 🌎 (Demographic factors influencing audience size)  

### 🤖 Machine Learning Models Used  
We experimented with multiple regression models:

+ Linear Regression  
+ Decision Tree Regressor (Best Performing)  
+ K-Nearest Neighbors (KNN) Regressor  
+ Ridge Regression
![image](https://github.com/user-attachments/assets/40931ebe-0c96-496e-a452-37ad123b899c)
Model Performance Comparison (Bar Chart of MAE, MSE, RMSE, R² Scores)

### 🎯 Hyperparameter Tuning
To improve accuracy, GridSearchCV was applied with 5-fold cross-validation to optimize:

+ Decision Tree: max_depth, min_samples_split, min_samples_leaf  
+ KNN: n_neighbors, metric  
+ Ridge Regression: alpha, solver

### 🏆 Best Performing Model: Decision Tree Regressor
Evaluation Metrics:
+ Mean Absolute Error (MAE): 0.0091  
+ Mean Squared Error (MSE): 0.0009  
+ Root Mean Squared Error (RMSE): 0.0300  
+ R² Score: 99.79% (Highly Accurate)  
![image](https://github.com/user-attachments/assets/177ce392-ca02-4755-a53f-e9afa7b68048)  
Actual vs. Predicted Subscribers Scatter Plot

## 🏁 Project Findings & Future Scope
✅ Key Findings:

1. Decision Tree Regressor outperforms other models with high accuracy.  
2. Video views, rank, and revenue are strong indicators of subscriber count.  
3. More data on content type, video length, and user demographics could improve predictions.

## 🚀 Future Enhancements:

+ Real-time YouTube Data Streaming for dynamic insights.  
+ Deployment as a Web Application for user-friendly analysis.  
+ Integration with YouTube API to enhance live tracking.

View the analysis:
Jupyter Notebook: YouTrendify_code.ipynb

### 🤝 Contributors
Parth Keyur Gawande  
Nikhil Satish Suryawanshi  
Raghunandan Ramadass
