# R-code-Kaggle-data-set
R code for credit data set from Kaggle
**Executive Summary**
Using credit data from a Kaggle data set that was collected by means of social
experiment, we implemented our knowledge of model fitting and selection to determine
a model that accurately tells the story of what credit applicant attributes factor into
determining whether they will have difficulties in payment, which is more commonly
known as default. Upon initial discovery of the data set we determined nine hypotheses
to test, surrounding attributes which may be predictors of loan default and established
our success criteria as a Sensitivity and Specificity of 70 percent.
The foundation of our analysis started with the consolidation of the data, which
included ridding of some of the categorical variables that were less useful in our end
goal and/or complicated the computation of our models. After fitting four binary
dependent models, we used confusion matrices that compared the Sensitivity and
Specificity of the model and the associated ROC to determine which model was the
best fit. Our study found that the four models were very close in measure; Logistic
Regression, Linear Discriminant Analysis, Quadratic Discriminant Analysis, Stochastic
Gradient Boosting; all nearly identical with their Specificity performance as can be seen
in figure 2. The determining factor for our decision on a model was the Sensitivity
performance, which was arguably very low for all models as figure 2 shows. To combat
this issue, model weights were introduced but the final model chosen was still QDA as it
had acceptable performance when predicting when someone would likely default on a
credit loan. What was concluded from our chosen model is that the variables that have
reliable meaning when determining whether someone will have trouble making
payments on a credit loan are; the gender and age of the individual, the cost of the item 
being purchased with the loan, the total amount of the loan, and the total income of the
individual. The older the individual, the more likely they would not default, men tend to
default more than women and the higher the total income the lower the chance of
default. Interestingly what we see with the cost of the item and the total amount of the
loan is that those factors are dependent on the outcomes of the other variables in the
model, as on their own the distribution of defaults is nearly identical. We believe that
with further analysis we would continue see that with something like loan default/loan
repayment issues, the more granular of an analysis on an individual will not necessarily
yield a more accurate prediction of outcome than that of a simple analysis using only a
few variables that could easily be inclusive of the granularity itself.
