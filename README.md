# WARN Notice Analysis
----------------------------------------------------------------
Background
----------------------------------------------------------------
Mass layoffs are a frequent occurrence across various fields and industries. The California Worker Adjustment and Retraining Notification (WARN) Act serves as a crucial safeguard for employees, their families, and communities by necessitating that employers furnish a 60-day notice to affected employees prior to a plant closure or mass layoff. This advance notice period provides workers and their families with the opportunity to navigate through the transition and adjust to the possibility of job loss. Moreover, it affords them the time to seek alternative employment options and, if necessary, acquire additional skills or undergo retraining to enhance their competitiveness in the job market.

Conditions to file:
- Mass layoff: Under California law, a mass layoff is defined as the elimination of 50 or more jobs during any 30-day period because of the lack of funds or because positions have been eliminated.

- Relocation: This refers to a scenario where a company is moving all or most of its commercial and industrial operations to a new location that is at least 100 miles away.

- Termination: A termination or plant closure means that the company has ceased all or most of its industrial and/or commercial operations.

----------------------------------------------------------------
Presentation
----------------------------------------------------------------
TBD

----------------------------------------------------------------
Graphs & Plots
----------------------------------------------------------------
![Distribution_Employees_County_California_Plotly](https://github.com/lleiva25/WARN-Notice-Analysis/assets/140974405/a88de6a0-88a8-402a-b9cf-514d498ab4a6)

![County_Layoff_Status_BarH_Matplotlib](https://github.com/lleiva25/WARN-Notice-Analysis/assets/140974405/b8ed0b51-160c-447f-ace4-dfe0f3240ad8)

![Top10_County_Plotly](https://github.com/lleiva25/WARN-Notice-Analysis/assets/140974405/0908205c-8cdc-48f2-b9fd-6545745a3a5d)

----------------------------------------------------------------
Analysis Walkthrough
----------------------------------------------------------------
1. Columns of original dataframe were renamed for simplicity
         - County/Parish : County
         - Notice\nDate : Notice Date
         - Processed\nDate : Processed Date
         - Effective \nDate : Effective Date
         - Layoff/\nClosure : Layoff Status
         - No. Of\nEmployees : No. of Employees
2. List all the companies names and replace the multiple company variations with the correct spelling. Convert dictionary to dataframe.
3. Combine the correct spelling dataframe with the original WARN dataframe.
4. Find the counties with the highest and lowest number of layoffs.
5. Group by 'County' to find the following:
         - Average Time from WARN Notice to Completion
         - Total No. Employees laid off
         - Number/Percentage of Layoff Status
6. Group by 'Company' to find the following:
         - Average Time from WARN Notice to completion
         - The company with the most lay offs
         - Number/Percentage of layoff status
7. Plot the findings with Matplotlib, Seaborn & Plotly.
----------------------------------------------------------------
Action Items
----------------------------------------------------------------
- Find a method to merge the columns and match the correct spelling for all company. Currently 408 company names haven't found their match.
- Create Dashboard for presenting data
----------------------------------------------------------------
