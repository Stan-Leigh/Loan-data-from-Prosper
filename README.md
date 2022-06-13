# Loan Data Exploration

## Dataset

This dataset consists of information regarding people that take loans. The dataset contains 113,937 rows of people that took loans for one reason or the other. It also contains variables like `LoanStatus`, `EmploymentStatus`, `OriginalLoanAmount`, and many more, that talk about the loan and the borrower in question. There were 81 variables total and 15 variables were used to do this exploration.
The dataset can be gotten [here](https://www.google.com/url?q=https://www.google.com/url?q%3Dhttps://s3.amazonaws.com/udacity-hosted-downloads/ud651/prosperLoanData.csv%26amp;sa%3DD%26amp;ust%3D1581581520570000&sa=D&source=editors&ust=1655039456192919&usg=AOvVaw1Pp9jCevGEcyuoAjDUN058).
The data dictionary that explains the features can be gotten [here](https://docs.google.com/spreadsheets/d/1gDyi_L4UvIrLTEC6Wri5nbaMmkGmLQBk-Yx3z0XDEtI/edit#gid=0).


## Data Wrangling

A few data wrangling steps was carried out on the dataset to make it better fo visualization. Some of the variables like `Term` were converted to categorical datatypes and a few others like `ProsperScore` was mapped from numbers to their original values using the data dictionary.


## Summary of Findings

* In the exploration, I found that there was a strong relationship between Prosper score and Prosper rating. The average prosper score for each Prosper rating increased as the Prosper raing got better. This made relationships discovered with Prosper rating to indicate that a similar relationship might also be present with Prosper score. 
* Borrowers in this dataset preferred to take long term loans as most of the people took loans for 36 and 60 months whilst a very small amount of people went for the 12 month term.
* About 50% of the dataset were taking loans to pay off other debts. The other half were split between Home improvement, Business, Personal loan, Household Expenses, Taxes and a few others.
* More than half of the borrowers in this dataset were Employed. There were also Full-time, Part-time and Self employed options which also took a significant portion of the dataset.
* Home owners and non home owners had similar median Prosper scores.
* Borrowers felt more comforatble taking higher loan amounts if it meant they could take a longer term (time taken to repay the loan).
* The median Prosper score for borrowers that had a stable source of income (Full-time, Part-time, even Retired, which I suspect is because of pensions given to retired workers) was significantly higher than those whose incomes were not stable or those who were not employed (Self-employed, Not-employed).
* Most of the people in this dataset had their loan status on Current. The next most common were those borrowers that had completely paid off their loans (Loan status of Completed). Defaulters and borrowers that were Charged off were the third and fourth most common.
* I discovered that people with better prosper ratings took higher loan amounts on average and they also earned more income per month when comparing with the median. Doing a deeper dive into this made me uncover that people that took loans for a longer amount of time (Longer terms), took larger amounts, and comparing these two variables with prosper rating, I discovered that the amount taken in loans kept increasing for better prosper ratings.
* Borrowers that owned homes had a higher average monthly income and they also borrowed more on average.
* Borrowers that took loans for 36 months and owned homes had a significantly high percentage of better Prosper ratings in comparison to other loan terms or non homw owners.


## Key Insights for Presentation

For the presentation I tend to focus on variables that influence the Prosper score/rating and the Loan status. I will first introduce these variables on interest then I start introducing some of the variables that will be used later to view relationships with the variables of interest.

Afterwards I start introducing relationships between variables of interest and the other features. I will start from bivariate visualizations depicting relationships between two variables to multivariate visualizations that depict relationships between three or more variables.
Different types of plots are used to convey the necessary information as clearly as possible.

When picking plots from a series of plots that were plot together, I wrote the code again, this time for only the plot of interest. This was so that I would have only one plot per slide instead of two or more plots if I copied the code from exploration.

Following the feedbacks gotten from an outside source, I made sure all the colors in the presentation were uniform. Feedback comments are documented in the notes section of the slide deck (Explanatory analysis.ipynb).
