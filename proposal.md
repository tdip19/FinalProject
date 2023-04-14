# Research Proposal: Predicting Employment and Economic Trends: An Analysis of the Relationship between Industry Trends and Recession Data. 

By Tim DiPalo, Tom Griffith, and Christyan Jean-Charles

## Research Question

This section should cover:
1. What do we want to know or what problems are we trying to solve? As in the midterm, you should list (1) the "bigger" question/debate/problem you're interested in, and also (2) the specific research question(s) you'll actually try to answer. 
  - The research question will be smaller in scope than the big picture question. But the answer to your specific research question should _shed light_ on the bigger question (although it likely won't conclusively answer it).
  - The answer to your specific research question should _shed light_ on the bigger question (although it likely won't conclusively answer it).

# Our Research Question: Can we use past data on industry trends / leading indicators to predict future employment and economic trends? 

## Specifically, Do job losses in the construction industry drive recessions?

2. If your project is about relationships, what are the hypotheses you're testing?
- As part of our predictive modeling analysis, we will be examining the relationship between the construction industry and recession data to determine how these two factors may be related. We will use statistical analysis techniques to examine the relationship between the construction industry and recession data. This may involve using correlation analysis to quantify the strength of the relationship between these variables, or regression analysis to identify the factors that drive changes in the construction industry during recession periods.

## Necessary Data

This section should cover:
1. What does the final dataset need to look like (mostly dictated by the question and the availability of data):
   - What is an observation, e.g. a firm, or a firm-year, etc.
       - Our observations will be based on job market data so specifically looking at job losses in the construction industry possibly through firm data 
       - The sample conditions/periods will include specifically data from the construction industry spanning over the past 10 years
       - Variables that will prove to be necessary are job data within the construction industry, market data (such as GDP), and many more economical factors
1. What data do we have and what data do we need?

    - Census Bureau data on recessions, interest rates, etc: We've collected data on various economic indicators, including information on recessions, employment, interest rates, consumer spending, and gross domestic product (GDP). These data sets can provide valuable insights into the health and direction of the US economy, allowing our group to identify trends and patterns over time, and make informed predictions about future economic conditions. For instance, the Census Bureau's data on recessions can help us identify periods of economic contraction and their duration, while data on interest rates can provide insights into the monetary policy decisions made by the Federal Reserve and their impact on the economy. 

    - Need industry specific data: In addition to general economic indicators, it is essential that we gather industry data, specifically on the construction industry, to gain a comprehensive understanding of how different sectors of the economy are performing, and to identify patterns and trends that are unique to each industry. We will use this to map the correlation between the construction industry and recession data.

1. How will we collect more data? 
    - In the event that the census bureau data does not provide us with sufficient data to support our predictive modeling analysis, we will explore other government websites to gather market and firm-level data. We will identify and evaluate alternative data sources based on their relevance, reliability, and timeliness, ensuring that the data we collect is comprehensive and relevant to our research question.
    - These alternative data sources may include government agencies such as the Bureau of Labor Statistics, the Federal Reserve, or the Securities and Exchange Commission, which provide a wealth of data on various economic indicators, financial markets, and firms' performance. We may also consider using private data sources such as industry associations, market research firms, or data providers that offer proprietary datasets on specific industries or markets.
1. What are the raw inputs and how will you store them (the folder structure(s) for each input type)? 
    - Our predictive modeling project will utilize a significant amount of census data, which may be too large to be stored in a single CSV file. As a result, we plan to organize the raw inputs into multiple zip files, each containing a subset of the data. To ensure efficient storage and retrieval of the data, we will store the zip files in distinct folders within our final project repository. This will allow us to effectively manage and access the data during the various stages of the predictive modeling process, from data preprocessing to model training and evaluation. Moreover, this organizational approach will help maintain the integrity of the raw data, ensuring that it is properly managed, versioned, and documented throughout the project lifecycle.
1. Speculate at a high level (not specific code!) about how you'll transform the raw data into the final form.
    1. As part of our predictive modeling project, we will follow a structured data pipeline that involves several key stages. First, we will perform an initial exploratory data analysis to gain an understanding of the data's structure, distributions, and relationships. This step will involve using visualizations and summary statistics to identify potential outliers, missing values, and other data quality issues that may need to be addressed.
    1. Once we have a good understanding of the data, we will proceed with data cleaning, which involves identifying and addressing any errors, inconsistencies, or missing values. This step may involve various data cleaning techniques, such as imputation, deletion, or data transformation, to ensure that the data is consistent and accurate.
    1. After cleaning the data, we will merge and manipulate the data to prepare it for modeling. This may involve combining multiple data sources, transforming variables, and creating new features or variables that are more predictive. This step may also involve selecting the most relevant features for the model, based on their ability to accurately predict the outcome of interest.
    1. Next, we will use regression analysis to model the data and generate predictions. This may involve using various regression techniques, such as linear regression, logistic regression, or time series regression, depending on the nature of the data and the problem we are trying to solve. We will use metrics such as R-squared, mean squared error, or cross-validated accuracy to evaluate the performance of the model.
    1. Finally, we will analyze the results of the model to gain insights into the data and to draw conclusions about the relationships between the variables. This step may involve visualizations, statistical tests, or other techniques to help us interpret the model results and communicate our findings effectively.
