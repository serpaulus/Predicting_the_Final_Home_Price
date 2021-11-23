
![Cover](https://user-images.githubusercontent.com/85421407/142972893-15a9e96c-7e7c-46eb-bff5-8f324ee45638.png)

## Overview

Data analytics is an integral part of almost every industry today. These days It is hard to think of an industry in which Data Analytics does not play a major role.  The housing market, one the bedrocks of the economy, is not an exception. From analyzing national or regional market trends to being able to evaluate the home value before it enters the market; data analytics helps provide key insights that drive some of the most important market decisions and strategies. Real Estate, while being a very good investment, can also be very unpredictable.

As a team, we decided to study and analyze Housing Prices for Ames, Iowa as we all find it intriguing, considering how volatile and unpredictable the real estate market is, due to the impact of the pandemic. 

The goal of our project is to predict the Sale Price of the homes based on the features of each home. In this analysis, we hope to determine if there is any correlation between the home features and the final Sale Price.

Questions:

What is the predicted Sale Price for each home?

Are there any correlation between the Sale Price and the features?

What feature(s) has the most significant effect on the predicted final Sale Price?

What feature(s) has the least significant effect on the predicted final Sale Price?

What could we have done differently, to get better results?

What do we recommend for future analysis?

[Project Presentation Slides](https://docs.google.com/presentation/d/1CP-Y-DHtzvPq8qeBXkekO-sVphJCxbwzYxdpZ75kIPY/edit#slide=id.p1)

## Data Exploration

The dataset used for this project is the Ames, Iowa housing dataset found on Kaggle. The dataset is divided into two: training and test datasets. The training dataset has 1461 rows and 81 columns while the test dataset has 1459 rows and 80 columns. Initially, we selected 20 columns from the 81 features but the more we explored and cleaned the data, we dropped more features as they appear to have little impact on the Sale Price. 

Test data set

Train data set

The main library used to import and clean the datasets was Python Pandas. Once completed, we exported the 20 cleaned dataset into the SQL database. We created features and an overall quality table, which we exported to SQL and merged to form a features/Quality table. The more we explored, the more we updated our dataset and dropped columns, which we will discuss in further detail.

## Machine Learning

When selecting home features for this analysis, we asked ourselves, what features do home buyers look for in their dream home? What features do we look for when buying a home and having our home appraised? What features do we believe will have the most correlation to the Sale Price? The answers to these questions were instrumental in the features we decided to explore. We selected House Style, No_of Bedrooms, Garage_Type, Total_Sqft, Lot Location, Year Built, Year Remodeled, 1st and 2nd Exterior, Masonry Veneer Type, Neighborhood, Overall Quality, Overall Condition, Sale Condition, and Sale price. 

The house dataset has several categorical values that need to be converted to numerical values to accurately analyze the data without errors. Using Label Encoder, we transformed the categorical values in the Dataframe to integers.

StandardScaler was used to scale the data and Seaborn was used to create a heatmap and check the correlation between the features and the Sale Price

![feature_corr_matrix](https://user-images.githubusercontent.com/85421407/142972745-45b22e35-672b-48a2-8ea8-5363f85b1238.png)

Based on the Heatmap, we can conclude that there is a correlation between the House Style and Sale Price. However, not all the figures are clear in the Heatmap. For better visualization, we created a correlation Scatter plot. Based on the results of the Scatter Plot, we can conclude that Total Square footage, Number of Baths and Overall Quality features also have strong correlation to the Sale Price, with Overall Quality having the strongest correlation.

![scatterplot_matrix](https://user-images.githubusercontent.com/85421407/142975667-e94d2f65-dcd0-4278-8a1c-feaae83d1ed6.png)

## Database

We created an [AWS DB instance](https://user-images.githubusercontent.com/85421407/142973441-79e27fed-3e89-4d6e-a320-d15a67af2310.GIF) called “housing-prices” and [using pandas and SQLAlchemy], we connected AWS with SQL to store the working data for this analysis. Once connected, we imported and exported from the database throughout the project. Multiple tables were created during the duration of this project but for the final segment, we merged our updated clean_train table, which was renamed “df” with the price_compare table to properly display the features with the Actual and Predicted Sale Price.



## Results and Dashboad


## Conclusion






## Overview

It is hard to think of any industry in which Data Analytics does not play a major role.  The housing market is not the exception. From analyzing national or regional market trends to be able to assess the value of home before it enters the market data analytics helps provide key insights that drive some of the most important market decisions and strategies. This team project aims to apply machine learning methodologies to analyze various common features to predict the final selling price.     

[Project Dashboard](https://public.tableau.com/views/PredicttheFinalHomePrice/Dashboard?:language=en-US&publish=yes&:display_count=n&:origin=viz_share_link)

## Methodology

### Data Source

Project data was obtained from a active Kaggle challenge to predict the final price of homes in the city of Ames, Iowa, and consists of:

   - [Test data set](https://github.com/serpaulus/Final_Project/blob/main/Data_Sets/test.csv)

   - [Train data set](https://github.com/serpaulus/Final_Project/blob/main/Data_Sets/train.csv)

Description

   - [Qualitative summary](https://github.com/serpaulus/Final_Project/blob/main/Data_Sets/kaggle_data_description.txt)

   - [Test metadata summary](https://github.com/serpaulus/Final_Project/blob/main/Data_Sets/tst_desc.csv)

   - [Train metadata summary](https://github.com/serpaulus/Final_Project/blob/main/Data_Sets/train_desc.csv)
   
      


   

 
 ### Proposed questions to answer 
    
   1)	What is the predicted final price of each home on the test sample?

   2)	What can the prediction results be compared against?

   3)	What is the level of accuracy?

   4)	What factors affect the model accuracy?

   5)	What Home features affect the home prices the most in the prediction model?


  ### Communication protocols
  
 The team will communicate via mainly via Slack and Zoom when required. 

 As much as possible branch merges will be coordinated with team members

 Updates via Slack and request collaboration in a timely manner to minimise delays 

 Leads will be the primary developers in their deliverables, and will submit their deliverable branch; howerver, all team members will try to 
 assist whenever it requested
        
    
 ### GitHub Deliverables 
     
 [X] Main Branch includes a README.md

 [X] At least one branch for each team member

 [X] Each team member has at least four commits from the duration of the first segment


 ### Machine Learning Model Deliverables
 

Team members present a provisional machine learning model that stands in for the final machine learning model and accomplishes the following:
 
[x] Takes in data in from the provisional database
![a](https://github.com/serpaulus/Final_Project/blob/main/Resources/ML_deliv1.PNG)
  
 
### Database Deliverables


Team members present a provisional database that stands in for the final database and accomplishes the following: 
 
[x] Sample data that mimics the expected final database structure or schema
![s](https://github.com/serpaulus/Final_Project/blob/main/Resources/tables_in_pgsql.PNG)

[x] Draft machine learning module is connected to the provisional database
![a](https://github.com/serpaulus/Final_Project/blob/main/Resources/ML_deliv2a.PNG) 
![b](https://github.com/serpaulus/Final_Project/blob/main/Resources/train_lrm_results_in_db.PNG)     

### Technologies

Jupyter Notebook

Python

PostgreSQL




    
    
 



    
    

  
    
    

    
    

    

