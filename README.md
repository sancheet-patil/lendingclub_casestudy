# Lending Club Case Study
> Lending Club is the largest online loan marketplace, facilitating personal loans, business loans and financing of medical procedures.Borrowers can easily access lower       interest rate loans through a fast online interface.
> Lending Club wants to understand the driving factors behind loan default, i.e. the driver variables which are strong indicators of default. The company can utilise this  knowledge for its portfolio and risk assessment.
> As a data scientist working  for Lending Club analyze the  dataset containing  information about past loan applicants using EDA to understand how consumer attributes and loan attributes influence the tendency of default.




## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
> Lending Club wants to understand the driving factors behind loan default, i.e. the driver variables which are strong indicators of default. The company can utilise this  knowledge for its portfolio and risk assessment.
> As a data scientist working  for Lending Club analyze the  dataset containing  information about past loan applicants using EDA to understand how consumer attributes and loan attributes influence the tendency of default.
> Dataset used is the excel sheet consists of different parameters that are responsible for an individual to be as a defaulter.

## Conclusions
- Removal of columns without much variance and need of the core fintech knowledge are ignored throughout categories and numeric.
- Few other factors which were not a major driving factor for the default/charged off status, yet were observed:
          Home Ownership: Those who have mortgage are less default, who's home_ownership is on rent or other are likely to default.
          States: NV state defaults the most (less population), FL with standard population defaults next, most loans go to CA, Texas & NY has the least default and PA is the                   best performing with a small population.
          Loan amount:Through this we can conclude that the loan amount increment is exactly boosting the number of defaults, Also there is not an entire inverse happening at                       the paid off, it is increasing till the third bracket. Once the loan amount goes passed 75% of the spread,the amount of paid off is declining and                             default is increasing.
          Funded amount : Loan amount and funded amount are entirely the same, again a correlation that can happen between funded_amount and loan_amount
          Installment: The population is comparable and the increment in installment can be a driving factor to the default status. Although till the 50% of the spread of the                        installment, the rate of default doesn't make too much difference. After 50% of the spread which is somewhere around 250 is incrementing the default                          rate. 
          Annual income: Higher the income lower the default rate over proportional distribution, the income is a driving factor univariately.
          Debt to Income: The bigger the debt over the income, the more the debt over income increases,it will result in default.
- Columns like issue date, title and zip code had too many discrete information and cannot be binned.

- As per us the major driving factors towards default/charged off :  Grades, Verification, Purpose, Term, Total payment, Interest rate through the univariate analysis.
- We went through heatmap analysis and scatter plot to figure out correlations. But they do work on numeric to numeric type correlation.
- We tried pivottable to get more clarity on categorical vs numeric type.
- We derived two derived metrics:
- Type driven metric: Approved date was extracted from the description and from there we can derive day, month and year.
- Business driven metric: We derived “Credit score” which is equivalent to “FICO score” and “Cibil score” which can be used by the LC to provide safer loans.

- We used mosaic plot mostly as it gives us both info about the population and categorical comparison, we also tried smthn like multivariate analysis, quite useful

## Technologies Used
- Seaborn library
- Numpy library
- Datetime library
- Pandas library
- pyMosaic

## References:
- https://www.jmp.com/en_us/statistics-knowledge-portal/exploratory-data-analysis/mosaic-plot.html
- https://www.kaggle.com/ekami66/detailed-exploratory-data-analysis-with-python
- https://www.pluralsight.com/guides/cleaning-up-data-from-outliers
- https://pandas.pydata.org/pandas-docs/stable/user_guide/indexing.html#returning-a-view-versus-a-copy



## Contact
Created by [@sancheet-patil] - feel free to contact me!
