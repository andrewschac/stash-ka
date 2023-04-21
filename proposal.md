# Research Proposal: Work from Home's Influence on Employee Opportunities and Performance
### By Jon Trzaska and Andrew Schachter

## Research Question

The inspiration for our final project stems from the wide-ranging work from home (WFH) work done by Nicholas Bloom. We plan to utilize some of the data that he has compiled in his work and apply it to understand how the recent WFH shift has influenced employees' experience in the workplace. Generally, we are asking the following questions:
1. Does WFH contribute to a worse experience for employees in regard to training, development, and integration?
2. What is WFH's effect on employee performance?

We plan to approach these questions by assessing the employees on a macro scale. By this, we mean looking at general trends across time and comparing levels of training/development sentiment and performance to the proportion of WFH employees. Some of the specific questions we are going to answer to assess the impact of WFH on employees include:
1. Is an employee more likely to leave a company if they WFH?
2. Does WFH increase employee productivity?
3. How is WFH correlated with employee promotion opportunities? 

In answering these questions, we mostly intend to assess how the levels of variables like productivity are different in times before and after the WFH boom (COVID-19 era). For other variables, like employee retention or promotion opportunities, we plan to compare the correlation of them to the proportion of WFH over time. Our project is wholly meant to explore the relationship between WFH and different variables that quantify employee opportunity and performance. Both of us having experience as students who were forced to learn from home and having WFH work experience in the past, we generally expect the influence of WFH to have a positive impact in most aspects of an employee's experience. Our general hypotheses and corresponding thoughts are outlined below:
- WFH makes an employee more likely to stay with a company
    - *Working from home adds more flexibility to an individual's schedule and reduces unnecessary aspects associated with working (commutes, less time wasted in meetings, monetary savings in regard to food/commute, etc.).*
- WFH increases employee productivity
    - *Employees are more distracted in the workplace and they avoid the downtime that occurs within an office setting.* 
- WFH hinders employees opportunities for growth
    - *With less in-office, face-to-face interaction with superiors, there are less opportunities for employees to be recognized by those who offer promotions and there is less collaboration with other employees.*
    
## Data

Our project assess employee variables on the industry-level, meaning our dataset will be a **panel dataset**. More specifically, each year will have a list of industries as well as the work from home data for each industry in each year. Our idea is to combine the [Bureau of Labor Statistics' National Compensation Survey Dataset](https://www.bls.gov/ebs/publications/september-2022-landing-page-employee-benefits-in-the-united-states-march-2022.htm)(2010-2022 excel sheet) with other variables that define employee opportunities and performance. The variables we intend to add to this dataset include the following:
- Turnover - % of US employees who left their firm
- Productivity - Total Factor Productivity
- Employee Growth - ? 
- Promotion Opportunities - % of US employees who elevated to a high position

General Dataset Structure:
| year | Industry | WFH_percent 
| --- | --- | --- |
| 2010 | Private sector, Finance and Insurance | 3
| 2011 | Private sector, Finance and Insurance | 3.5
| 2012 | Private sector, Finance and Insurance | 6
| 2010 | State and Local Government, Hospitals | 5.8
| 2011 | State and Local Government, Hospitals | 5.8
| 2012 | State and Local Government, Hospitals | 5.8

Though we have access to the overall percentage of the US working population who is WFH, by industry, annually, we still need to acquire some of the variable data. We intend to measure employee productivity by utilizing Total Factor Productivity, a measure that is tracked by the [Bureau of Labor Statistics](https://www.bls.gov/productivity/data.htm). We are still researching ways to gain access to U.S. turnover and promotion data. In regard to employee growth, we are struggling to find ways to quantify the measures of training, development, and integration. 

Our final dataset will span from years 2010 - 2022. Though the Bloom WFH dataset spans from 1965-now, we think that the data before 2000 is largely irrelevant to our analysis and the dataset we sourced from the BLS National Compensation Survey begins in 2010. Our thought process is that most people before then didn't have the same capability to WFH even if they wanted to due to the financial barriers of having a separate PC at home. We also believe that the post 2010 data is sufficient enough for our analysis because it still compares pre-COVID to COVID and beyond. Other sample conditions that we mentioned include limiting our scope to the U.S. working population. An added bonus we found when importing and quickly querying the dataset was that it also spans civil and state/government industries, not just private sectors. 

Another option we are exploring to add variables to our final dataset is downloading the survey data that Nicholas Bloom and his colleagues have utilized in some of their research. This data explores WFH employees, managers, and their sentiment about WFH in different circumstances. Our general plan for obtaining the data is to download the csv and excel files we found online and manipulate them into dataframes that we can use to test our hypotheses. We are visualizing an inputs folder with subfolders that contain all our raw inputs and data. More specifically, we would download the raw data from the inputs folder then use eda techniques on the data to clean it and check for errors or outliers. Then we will merge the different datasets into one dataframe that we can manipulate and use to create visualizations. 

## Visualizations

We are planning to include a few different visualizations in our final work product that will give more context to our answers to our questions. First, we will use regression to talk about work from home across industries. Some questions these visualizations would answer could include are individuals who work for WFH companies  productive than their office counterparts, or how does work from home vary by industry. Both of these questions could be answered with simple regression models, like the second question, where the industry would be on the x-axis and percentage of work from home employees would be on the y-axis. Other visualizations we are thinking about include a heat map of industry vs. work from home vs. productivity. None of these visualizations are overly complex but they would be informative and provide good additions to our data.
