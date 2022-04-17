# Drop Out Rates in New York State
By: Samira Chatrathi

## Overview
The education system is one of the most life changing organizations within the American government. Due to education’s ability to encourage growth and pave the way for future careers, Americans must trust the systems set in place. In recent years, however, High School dropout rates have increased due to a wide range of different risk factors. In this project, I classify dropout rates into risk-levels as a means of predicting which subgroups are at different tiers of risk level. Educators can use this modeling process as a means of helping students within different risk categories hone their skills and obtain the maximum benefit from their public education systems. 


## Business Understanding

The New York State Education Department deems their mission as a government organization to supervise all public schools in New York, working to build the opportunity for all students within NY State regardless of their background. While this mission is lofty and seemingly holistic, bureaucratic factors tend to work against the schools themselves, focusing on superintendent promotion rather than the long term achievement of all students. In a study conducted by the NY Times, more than 120,000 students have left New York City public schools over the past five years. With the varying levels of COVID-19 surges across the state of NY state, educators and legislators need to focus on how they can improve communities with high dropout rates as well as understand what keeps a student engaged within a high school program and what doesn’t. I have tailored this project towards a member of the New York State Board of Education looking to understand which demographic factors are associated with higher high school dropout rates and which demographic factors are associated with lower dropout rates. Due to the sensitivity of these demographic factors this modeling process is for inferential purposes. The assumption that correlation is not equivalent to causation should be held throughout this modeling process and understanding. 


## Data Understanding

The data set I chose to analyze was from the New York State Education Department’s report card dataset. I chose to stack the report cards within the years of 2012-2016. I began by combining the demographic and associated percentage dropout reports for each year and then stacked the years on top of each other to act as an accumulation of multiple years.  One of the important things I considered when choosing this time frame for my dataset was that school report cards carry heavy weight on how schools will function after the pandemic subsides. Board members can use this past information based on fully opened schools to understand how they can implement new strategies once schools fully re-open. In terms of my exploratory data analysis, I wanted to categorize the dropout rates into three categories. Dropout rates as well as other demographic factors were given in percentages, so it standardized the values for my dataset on all fronts (values took between 0-100%). After all data cleaning (dropping null-values,etc.) and feature engineering was conducted, the final dataset contained 66,198 school entries, over the span of 4 years. Based on initial EDA, I found that the average dropout rate for my dataset was 6%. I binned my target variable based on the risk level associated with the percentage dropout rate. Within the dataset, the target variable was split into 3 classes of “Low-Risk”, “Mid-Risk”, and “High-Risk”. 53% of the entries were categorized as Low-Risk, 31% of the entries were categorized as Mid-Risk, and 16% of the entries were categorized High-Risk, where the percentage of dropout rate was higher than the 75th percentile of dropout rates within the dataset. One limitation to consider from our dataset is how holistic the demographic information is. While students do fall into a wide range of demographic levels, there are always minority groups that are not accounted for.

## Methods
I implemented a Decision Tree Model as well as a KNN Model.Our classification metric is precision. It is important to consider the meaning of precision in this case and why it would be the most productive for this project. Precision encompasses the false positive rate, potentially marking a school high-risk when they are not. This would be a more important factor for two reasons. First, if we marked a school as high-risk for dropout when it isn't it would be better than leaving schools that are high risk un evaluated. Second, our ability to go and see which schools are low-risk will allow us to see which aspects of the school are productive and are leading to these lower levels of drop out rates. The highest level of precision for the KNN model after hypertuning was 73%. Based of off the decision tree results, the top 4 features (all within the class low-risk) are the percentage of Multiracial Students, the percentage of Limited English Proficient Students, the percentage of American Indian or Alaskan Native Students, and the percentage of Students Eligible for Free Lunch.

## Key Takeaways

Based on the modeling process which can be found in the main notebook, I have gathered some actionable insights that can be beneficial to implement. First, the board of education should monitor schools classed as low-risk and understand more about how they are supporting students among different demographics while investing in grand scale implementation. Second, the board of education should continue to hone language diversity within the curriculum as well as providing students with muti-lingual backgrounds with subject resources in languages they can understand difficult concepts in. Finally, the board of education should monitor high risk schools and send in department chairs to assess with faculty and staff as to how to better support students while rebuilding foundational tools for all students. 

## Conclusion
Conclusion:
This modeling project is just the beginning to the long and iterative process of helping the education system. As we work as a community to support students from all backgrounds, we should also consider the importance of mental health when adjusting from a covid-learning environment. I am excited to incorporate mental health data to continue to provide a more nuanced understanding of dropout rates in the near future. 
