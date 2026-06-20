## Research Question

Is there a linear relationship between screen time and BMI percentile among high school students?

## Variables

- Predictor variable: `screen_time_hours`
- Response variable: `bmi_percentile`

`screen_time_hours` was created by adding recoded TV watching hours and computer use hours. Because the original screen time variables were categorical responses, they were recoded into approximate numeric hours.

## Statistical Method

Simple linear regression was used to examine the relationship between screen time and BMI percentile.

The model was:

```text
Predicted BMI percentile = 61.6837 + 0.8374 × Screen time hours
```

## Key Results

- Sample size: 12844
- Slope: 0.8374
- 95% CI for slope: [0.6466, 1.0282]
- p-value: p < 0.001
- R-squared: 0.0057

## Interpretation

For each additional hour of screen time, the predicted BMI percentile increased by about 0.84 percentile points on average.

The slope was statistically significant, with p < 0.001. This suggests a statistically significant positive linear relationship between screen time and BMI percentile.

However, the R-squared value was only 0.0057. This means screen time explained about 0.57% of the variation in BMI percentile. Therefore, although the relationship was statistically significant, the practical effect was weak.

## Conclusion

Higher screen time was associated with slightly higher BMI percentile among high school students. However, screen time alone explained very little variation in BMI percentile. Since the data are observational, the result should be interpreted as association rather than causation.

## Limitations

- Screen time was recoded from categorical responses, so the value is approximate.
- BMI percentile may be affected by many factors not included in this simple model.
- This is observational survey data, so the analysis cannot prove causation.
