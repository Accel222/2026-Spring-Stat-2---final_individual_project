# Presentation Video Outline

## 0:00-0:30 Introduction
Hello, my name is 周朝賢. My student ID is 112310326.  
My final individual project is about screen time and BMI percentile among high school students.

## 0:30-1:10 Research Question
The research question is: Is there a linear relationship between screen time and BMI percentile among high school students?

## 1:10-1:50 Variables
The predictor variable is screen_time_hours.  
It was created by adding TV watching hours and computer use hours.  
The response variable is BMI percentile.

## 1:50-2:40 Data Cleaning
The original TV watching and computer use variables were categorical.  
I recoded them into approximate numeric hours: 0, 0.5, 1, 2, 3, 4, and 5 hours.  
Then I added them together to create total screen time.  
Rows with missing screen time or BMI percentile were removed.  
The final sample size was 12844 students.

## 2:40-3:30 Method
I used simple linear regression.  
The model was: predicted BMI percentile equals intercept plus slope times screen time hours.  
The null hypothesis was that the slope equals zero.  
The alternative hypothesis was that the slope is not equal to zero.

## 3:30-4:30 Results
The estimated slope was 0.8374.  
This means that for each additional hour of screen time, the predicted BMI percentile increased by about 0.84 percentile points on average.  
The 95% confidence interval was [0.6466, 1.0282], and the p-value was p < 0.001.  
So, the relationship was statistically significant.

## 4:30-5:10 Practical Interpretation
Although the result was statistically significant, the R-squared value was only 0.0057.  
This means screen time explained only about 0.57% of the variation in BMI percentile.  
Therefore, the relationship was statistically significant but practically weak.

## 5:10-5:40 Conclusion and Limitations
The main conclusion is that higher screen time was associated with slightly higher BMI percentile.  
However, screen time alone cannot explain most of the variation in BMI percentile.  
Also, this is observational survey data, so we can only say association, not causation.

## 5:40-End Code Explanation
Show the notebooks:
1. data cleaning notebook
2. main regression notebook
3. outputs and summary notebook

Briefly explain the key code for recoding variables, fitting the regression model, and creating figures.
