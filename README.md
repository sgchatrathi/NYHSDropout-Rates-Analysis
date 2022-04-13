# Drop Out Rates in New York State
By: Samira Chatrathi





## Business Understanding

The New York State Education Department deems their mission as a government organization to supervise all public schools in New York, working to build the opportunity for all students within NY State regardless of their background. While this mission is lofty and seemingly holistic, bureaucratic factors tend to work against the schools themselves, focusing on superintendent promotion rather than the long term achievement of all students. In a study conducted by the NY Times, more than 120,000 students have left New York City public schools over the past five years. With the varying levels of COVID-19 surges across the state of NY state, educators and legislators need to focus on how they can improve communities with high dropout rates as well as understand what keeps a student engaged within a high school program and what doesn’t. I have tailored this project towards a member of the New York State Board of Education looking to understand which demographic factors are associated with higher high school dropout rates and which demographic factors are associated with lower dropout rates. Due to the sensitivity of these demographic factors this modeling process is for inferential purposes. The assumption that correlation is not equivalent to causation should be held throughout this modeling process and understanding. 


## Data Understanding

The data set I chose to analyze was from the New York State Education Department’s report card dataset. I chose to stack the report cards within the years of 2013-2017. I began by combining the demographic and associated percentage dropout reports for each year and then stacked the years on top of each other to act as an accumulation of multiple years.  One of the important things I considered when choosing this time frame for my dataset was that school report cards carry heavy weight on how schools will function after the pandemic subsides. Board members can use this past information based on fully opened schools to understand how they can implement new strategies once schools fully re-open. In terms of my exploratory data analysis, I wanted to categorize the dropout rates into three categories. Dropout rates as well as other demographic factors were given in percentages, so it standardized the values for my dataset on all fronts (values took between 0-100%). After all data cleaning (dropping null-values,etc.) and feature engineering was conducted, the final dataset contained 66,198 school entries, over the span of 4 years. Based on initial EDA, I found that the average dropout rate for my dataset was 6%. I binned my target variable based on the risk level associated with the percentage dropout rate. Within the dataset, the target variable was split into 3 classes of “Low-Risk”, “Mid-Risk”, and “High-Risk”. 53% of the entries were categorized as Low-Risk, 31% of the entries were categorized as Mid-Risk, and 16% of the entries were categorized High-Risk, where the percentage of dropout rate was higher than the 75th percentile of dropout rates within the dataset. One limitation to consider when understanding 

## Modeling Process

## Final Model 

## Conclusion
