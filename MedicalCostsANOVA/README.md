## Packages Dependencies: 
- pandas == 1.4.2
- numpy == 1.22.3
- seaborn == 0.11.2
- matplotlib == 3.5.2
- sklearn == 1.1.2
- scipy == 1.8.1

## This Folder holds two files an insurance dataset saved as a csv file, and an ipynb containing my analysis. 
Data shape: 1300 samples
X variables: age, sex, bmi, # of children, region
Y output: insurance charge ($)

- the original goal was to conduct one way ANOVA on the independet variables to determine whether or not there was any change between categories. 
- After completing ANOVA I decided to test some models to see if I could estimate the charge price based on the factors

## TLDR (If you don't want to view full analysis):
### Anova: 
- We can reject the null hypothesis, there is a diference in average charges billed for male and female
- We can reject the null hypothesis, the average billing for smoker is greater than the non-smoker
- We can reject the null hypothesis. The average billing is different for samples
- males and smokers are billed higher amounts

### Model Output:
- best model based on chosen metrics - R^2 (about 83%), mean absolute error and root mean squared error was the Random Forest regressor
- On average the root mean squared error for the model was $5800, meaning there is definitely room for improvement. 
- KFold cross validation using 7 splits gave the best error values
- Grid search tuned to find number of samples to be used for Regressor (300 samples)
- Random forest tends to overfit with small sample sizes such as here. Therefore, the model can definitely be improved with more data, adding features, 
feature engineering, further tuning of hyper parameters, another consideration - possibly using an ensemble method or tuning other models. 


