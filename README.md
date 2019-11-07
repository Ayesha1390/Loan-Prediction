# Loan Prediction

Company wants to automate the loan eligibility process (real time) based on customer detail provided while filling online application form. These details are Gender, Marital Status, Education, Number of Dependents, Income, Loan Amount, Credit History and others. 
To automate this process, they have given a problem to identify the customers segments, those are eligible for loan amount so that they can specifically target these customers.

### Exploratory Data Analysis
Target variable has two categories: 
Yes = Loan Approved to the Customer, No = Loan not approved to the customer. 
We can clearly see that our data is highly imbalanced. 
![](https://github.com/Ayesha1390/supreme-memory/blob/master/Images/Loan_Status.png)

Distribution of Numerical Variables:-
These variables are  skewed therefore require transformation. Used Logarithmic transformation technique.

#### Applicant Income
![](https://github.com/Ayesha1390/supreme-memory/blob/master/Images/ApplicantIncome.png)

#### CoApplicant Income
![](https://github.com/Ayesha1390/supreme-memory/blob/master/Images/CoapplicantIncome.png)

#### Loan Amount
![](https://github.com/Ayesha1390/supreme-memory/blob/master/Images/Loan_Amount.png)

#### Loan Amount Term
![](https://github.com/Ayesha1390/supreme-memory/blob/master/Images/Loan_Amount_term.png)

Correlation amongst variables post converting categorical variables in numeric variables.
#### Correlation
![](https://github.com/Ayesha1390/supreme-memory/blob/master/Images/Correlation.png)

#### RandomOverSampler
As the data was imbalanced used RandomOverSampler to balance out the data.
Random oversampling simply replicates randomly the minority class examples.
Original dataset 
Yes: 422, No: 192

After RandomOverSampler
Resampled dataset 
Yes: 422, No: 422

#### Principal Component Analysis
After applying pca to the resampled data to reduce dimensions we found that 11 components explain the variability in the data.

#### Model Evaluation
-Random Forest

-Logistic Regression

-K- Nearest Neighbors

-Naïve Bayes

-SVM


Model Selection
Random forest has the best results for our problem. Random Forest has the best accuracy and lowest false negative rate and also lowest false positive rate.Hence we’ll choose Random Forest.
