# Inspiration
After working with more than 70 toy datasets, this internship provided a platform to get a detailed overview of how industry works. As most of dataset I worked on used 
to be cleaned ones, this internship helped in getting data in it's raw form. Starting from basic collected data to model building and collecting insigths from it was a 
**full fledged** work I was interested in.

# Data Quality Assessment
* As data was in its raw form, it was necessary to clean it and observe any disperancy in it before proceeding to deriving insigts, as insights from a vague value may
in a **misleading conclusions**.
* Dataset was evaluated based on **Data Quality Framework Table** and a draft was generated which was sent to client for double check. Also strategies were given to 
mitigate such disperancy.

## Feature Engineering
* A dataset was downloaded from **Australian Bureau of Statistics** where each pincode was segregated to different states. Most important finding of such feature 
engineered column was segregating **Australian Capital Territory** from 'New South Wales.

# Insights on current customers
* A RFM analysis was carried out on all the customers and following conclusions were derived:
  ** The company was loosing 39 important customers.
 ![image](https://user-images.githubusercontent.com/102746816/161388081-3f3f0d76-9c15-4c24-8811-a6846c47a7a6.png)
 
 ## Data Preparation before modelling
 * Dataset had **no target variable**, so a column was created from RFM analysis using monetary habits, i.e They were divided into two category based on spending.
 * As there were 12.6% missing value in job_industry_category which was found to be an important indicator in predicting importance of customer, instead of dropping 
 the column a target based encoding is done which took care of the missing values in data. i.e. **WOE(Weight of Evidence) Encoding**
 
 # Model Building
 * Best model was found to be a **Stacking Classifier** which had two KNNClassifier as base models and GausianNB as final_estimator.
  ![image](https://user-images.githubusercontent.com/102746816/161388556-7c885e3b-cbaf-4297-a08d-9767da794869.png)
 * A model was created using full datasets as previously train-test split was compromising patterns present in train dataset. 
 # Prediction
 * The new customer dataset was converted to similar structure to that of train dataset and prediction was carried out.
 * Deciding factor job_industry_category was plotted for better understanding of important customers from different job category.
   ![image](https://user-images.githubusercontent.com/102746816/161388710-15465da4-1279-445d-989d-1ceb6b7d0514.png
   
 # Visualisation
 * A dashboard was created to make client understand about what was happening and what is going to happen among their current customers and new customers.


