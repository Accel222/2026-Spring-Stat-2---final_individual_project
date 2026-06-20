# One-Page Infographic Content

## Title
Screen Time and BMI Percentile

## Research Question
Is there a linear relationship between screen time and BMI percentile among high school students?

## Dataset
YRBS 2007 National High School Survey

## Variables
X: screen_time_hours = TV watching hours + computer use hours  
Y: BMI percentile

## Data Preparation
TelevisionWatching and ComputerUse were recoded from categorical responses into approximate numeric hours.  
Rows with missing screen time or BMI percentile values were removed.

## Method
Simple Linear Regression

Model:
Predicted BMI percentile = 61.6837 + 0.8374 × Screen time hours

## Key Results
Sample size: 12844  
Slope: 0.8374  
95% CI for slope: [0.6466, 1.0282]  
p < 0.001  
R²: 0.0057

## Interpretation
For each additional hour of screen time, the predicted BMI percentile increased by about 0.84 percentile points on average.  
The relationship was statistically significant.  
However, screen time explained only about 0.57% of the variation in BMI percentile.

## Main Takeaway
Higher screen time was associated with slightly higher BMI percentile, but screen time alone explained very little variation in BMI percentile.

## Limitations
Screen time was recoded from categorical responses, so it is approximate.  
BMI percentile may be affected by many other factors not included in this simple model.  
This is observational survey data, so the result should be interpreted as association, not causation.
