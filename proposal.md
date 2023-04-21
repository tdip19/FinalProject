# Research Proposal: Predicting Employment and Economic Trends: An Analysis of the Relationship between Industry Trends and Recession Data. 

**By Tim DiPalo, Tom Griffith, and Christyan Jean-Charles**

This project explores whether we can use past data on industry trends and leading indicators to predict future employment and economic trends. Specifically, do job losses in the construction industry drive recessions?

As part of our predictive modeling analysis, we will be examining the relationship between the construction industry and recession data to determine how these two factors may be related. We will use statistical analysis techniques to examine the relationship between the construction industry and recession data. This may involve using correlation analysis to quantify the strength of the relationship between these variables, or regression analysis to identify the factors that drive changes in the construction industry during recession periods.

As students about to enter the job field, it is important for us to follow industry trends and economic conditions. Being able to identify leading factors that lead to recession can give us insight into how we can prepare for different economic conditions.

## Necessary Data

1. The final dataset:

   - Our observations will be based on job market data so specifically looking at job losses in the construction industry possibly through firm data 
   - The sample conditions/periods will include specific data from the construction industry spanning over the past 10 years
   - Variables that will prove to be necessary are job data within the construction industry, market data (such as GDP), and many more economical factors
   
Example dataframe:

| Index | Year | Industry | Employment rate | CPI | GDP per capita | SP500 return |
| ------- | ----------- | ----------- | ------- | ------- | -------| ------- |
| 1 | 2015 | Construction | 91% | 3% | 134000 | 2%
| 2 | 2018 | Technology | 88% | 7% | 96000 | 3.5%
| 3 | 2012 | Manufacturing | 95% | 4% | 174000 | 1%
   
1. What data do we have and what data do we need?

    - Census Bureau data on recessions, interest rates, etc: We've collected data on various economic indicators, including information on recessions, employment, interest rates, consumer spending, and gross domestic product (GDP). These data sets can provide valuable insights into the health and direction of the US economy, allowing our group to identify trends and patterns over time, and make informed predictions about future economic conditions. For instance, the Census Bureau's data on recessions can help us identify periods of economic contraction and their duration, while data on interest rates can provide insights into the monetary policy decisions made by the Federal Reserve and their impact on the economy. 
    - Need industry-specific data: In addition to general economic indicators, it is essential that we gather industry data, specifically on the construction industry, to gain a comprehensive understanding of how different sectors of the economy are performing, and to identify patterns and trends that are unique to each industry. We will use this to map the correlation between the construction industry and recession data.

1. How will we collect more data? 

    - In the event that the census bureau data does not provide us with sufficient data to support our predictive modeling analysis, we will explore other government websites to gather market and firm-level data. We will identify and evaluate alternative data sources based on their relevance, reliability, and timeliness, ensuring that the data we collect is comprehensive and relevant to our research question.
    - These alternative data sources may include government agencies such as the Bureau of Labor Statistics, the Federal Reserve, or the Securities and Exchange Commission, which provide a wealth of data on various economic indicators, financial markets, and firms' performance. We may also consider using private data sources such as industry associations, market research firms, or data providers that offer proprietary datasets on specific industries or markets.
    
1. What are the raw inputs and how will you store them (the folder structure(s) for each input type)? 

    - Our raw inputs will be comprised of Census Bureau data and industry-specific data as outlined in the data section above. Our census data will come from https://data.census.gov/, and we will use the same S&P data that we have been using for the assignments.
    
    - We plan to download all of our input files into an inputs folder so it is accessible to everyone using the repo. It is likely that our data will be small enough to store and upload easily. Our predictive modeling project will utilize a significant amount of census data, which may be too large to be stored in a single CSV file. If we find that our data is too large, we plan to store it in zip files within the inputs folder. 
    
1. Speculate at a high level (not specific code!) about how you'll transform the raw data into the final form.

    1. We will use get_and_clean_data.ipynb to create a good understanding of the data, then we will proceed with data cleaning, which involves identifying and addressing any errors, inconsistencies, or missing values. This step may involve various data cleaning techniques, such as imputation, deletion, or data transformation, to ensure that the data is consistent and accurate.
    1. After cleaning the data, we will merge and manipulate the data to prepare it for modeling. This may involve combining multiple data sources, transforming variables, and creating new features or variables that are more predictive. This step may also involve selecting the most relevant features for the model, based on their ability to accurately predict the outcome of interest.
    
1. Follow best practices to build, evaluate, and choose between many prediction models

    1. As part of our predictive modeling project, we will follow a structured data pipeline that involves several key stages. First, we will use get_and_clean_data.ipynb to perform an initial, messy exploratory data analysis to gain an understanding of the data's structure, distributions, and relationships. This step will involve using visualizations and summary statistics to identify potential outliers, missing values, and other data quality issues that may need to be addressed.
    1. After that, we will use analysis.ipynb to perform our analysis on the merged dataset. This includes the machine learning and everything outlined below.
    1. After this, we will use regression_analysis.ipynb to use regression analysis to model the data and generate predictions. This may involve using various regression techniques, such as linear regression, logistic regression, or time series regression, depending on the nature of the data and the problem we are trying to solve. We will use metrics such as R-squared and mean squared error to evaluate the correlation.
    1. We will also then use prediction_modeling.ipynb to perform machine learning techniques on our merged dataset to try to predict the effects of economic uncertainty on certain industries. To evaluate the performance of the model, we will use cross-validation (CV) techniques wherein the training periods will expand from the beginning of the sample, and test the performance for a given CV fold in the period subsequent to the end of the fold's training period.
    1. Finally, we will use results.ipynb to analyze the results of the model to gain insights into the data and to draw conclusions about the relationships between the variables. This step may involve visualizations, statistical tests, or other techniques to help us interpret the model results and communicate our findings effectively.