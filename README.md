![cover](https://user-images.githubusercontent.com/85421407/142942183-964584eb-71af-4eff-822c-f5cae98343b9.jpg)

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
   
      

### [Project Presentation Slides](https://docs.google.com/presentation/d/1z0xOtSOFEzmkXZrz9OE3YVoVVCDtRbS0/edit#slide=id.p1)
   

 
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

### Database

We created an AWS DB instance called “housing-prices” and using pandas and SQLAlchemy, we connected AWS with SQL to store the working data for this analysis. Once connected, we imported and exported from the database throughout the project. Multiple tables were created during the duration of this project but for the final segment, we merged our updated clean_train table, which was renamed “df” with the price_compare table to properly display the features with the Actual and Predicted Sale Price.

![a]("https://user-images.githubusercontent.com/85265504/142972335-32539432-4dbe-478f-9c57-ea6e2763ee8f.png")

![Database Connection]("https://user-images.githubusercontent.com/85265504/142972433-689f8e36-adc3-4342-856c-3e79d31a6a9c.png")


### Technologies

Jupyter Notebook

Python

PostgreSQL




    
    
 



    
    

  
    
    

    
    

    

