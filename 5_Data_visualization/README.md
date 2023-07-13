<h1><center>Analysis and Visualization - Prosper Loan Data</center></h1>
<center>By</center>
<h3><center>Nishanth Iruthayaraj</center></h3>

## Dataset
<br>
<div style="text-align: justify">
    
This data set contains 113,937 loans with 81 variables on each loan, including loan amount, borrower rate (or interest rate), current loan status, borrower income, and many others. Each of this feature can be used for various. ince the dataset contains 81 variable, it will tedious to explore each and every varible in our analysis. So I chose few variables that are mainly related to loan process and also make our invertigation meaning. The choosen variables for the data exploration are 'term', 'loan_status', 'borrower_APR', 'borrower_rate', 'prosper_score', 'listing_category_numeric', 'employmentstatus', 'employment_status_duration', 'is_borrower_homeowner', 'debt_to_income_ratio', 'stated_monthly_income', 'loan_original_amount', 'loan_origination_date', 'monthly_loan_payment'. 
</div>

## Summary of Findings
<br>
<div style="text-align: justify">
    
##### Obervation of Univariate exploration:
- What are the findings of main feature of interest?

    - The distribution of Borrower's Annual Percentage Rate (APR) is a multimodal. In addition, there is an unusual spike in the percentage rate around 0.36.   
- What are the findings of other features supporting the investigation?
    - The most frequent loan term is 36 months. The 60 months loan term stands in the second position. But the loan term for 12 months is very very less. It shows that only very few borrowers take loan for short term. 

    - Many of the loan are in current status. Also there are many loans that has been Completed, Chargedoff and Deafaulted. 
    - Past Due (based on days) and the Cancellation (5 counts) status are very minimum comapred to the other loan status. 

    - The interest rate has the multimodal distribution
    - It looks also similar to the distribution of varibale `borrower_APR`

    - There are huge amount of borrowers has very highest risk score (0).
    - The most of the prosper score of the borrowers lies between the range of 2 and 10.  

    - Debt Consolidation is the most frequent loan category that the borrowers applied for

    - The most the borrowers applied for loan are "Employed"

    - Surprisingly, there are equal amount of borrowers i.e: even if the Borrower has their own home or not, the loan Borrowers are almost equal.

    - The most common range of borrower's income is between the range of 2500 and 500. 
    - The income distribution of the borrowrs are right skewed
    - The approximate maximum income lies around 42000

    - The most common loan amount taken by the borrowers is approximately 4500
    - The distribution of the loan amount is also right skewed with multiple spikes
 
    
##### Obervation of Bivariate exploration:
- How is the main feature of interest related to other variable and how does main feature varies with other features of interest? 

    - The Annual Percentage Rate (APR) of Borrowers is decreasing when the loan original amount increases i.e. the `borrower_APR` is negatively correlated with respect to `loan_original_amount`. Also the length of the `term` increase when there is an increase in the `loan_original_amount`. When the Borrowers has higher monthly income, they are capable of getting the high loan amount and can afford to payback the loan amount on monthly basis. 

    - In addition to the above relationships between the features, we can see that the Homeowner has the higher employment rate while comapring to borrowers who doesn't own home. Also The maximam amount of loan take by Homeowner is around 35000 and the Non-Homeowner has around 25000. This also proves that the borrowers can take more loan amount when they own some properties. 
    
##### Obervation of Multivariate exploration:
- The densed `borrower_APR` percentage for the loan `term` of 36 months lies between the range of between 0.05 and 0.4. Whereas the `borrower_APR` percentage for the loan `term` of 60 months lies between the range of 0.09 and 0.36. Also the `borrower_APR` percentage for the loan `term` of 12 months lies between the range of 0.05 and 0.36. It can conclude that the `term` does not affect the `borrower_APR` percentage rate significantly. 
- The interesting insights from the exploration is that the `monthly_loan_payment` decreases gradually when there is an increase in `loan_original_amount` and `term`.   

</div>

## Key Insights for Presentation
<br>
<div style="text-align: justify">
    
- During this project, the chosen main feature of interest from the given dataset is Borrower's Annual Percentage Rate (APR) i.e. `borrower_APR`. 
- Since the dataset contains 81 variables, I choose 14 significant variables necessary for the loan investigation. 
- At the begining I chose univariate exploration to get an insights from each varibale with corresponding plots. 
- Next, I performed bivariate analysis after finding the correlation (either maximum or minimum) between each variable.
-Finally, I did the multivariate data exploration to find the most common varibles that has an impact on the Borrowers Annual Percantage Rate. 
- At the end of exploration, the variables like `monthly_loan_payment`, `loan_original_amount`, and `stated_monthly_income` has an major effect on Borrowers Annual Percentage Rate when comparing with the loan Term. In the presentation, the readers can also see individual visualization clearly.  
    
</div>
