## Package Dependencies: 
- sklearn == 1.1.2
- plotly == 5.10.0
- numpy == 1.22.3
- pandas == 1.4.2

Data Shape: 518 observations
X variables: Location, Time, MRI_Units, CT_Scanners, Hospital_Beds
y output: Hospital Stay

## TLDR: 
- started off by looking at the correlation between variables 
- strong positive correlation between number of CT scanners and MRI units, this makes sense and probably relates to the size of the hospitals
- Japan, Russia and Korea have the longest length of stay

## Model Outputs: 
- trained linear regression and decision tree regressor
- due to the small amount of data collected, the classical linear regression model outperforms the decision tree. 
- R^2 for the evalated linear regression - 0.901 (a good fit)
- mean squared error of 0.651 

## improvements: 
- find more data either by sourcing from api or interpolating
- adding more useful features 
