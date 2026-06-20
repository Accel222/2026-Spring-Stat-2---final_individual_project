# Screen Time and BMI Percentile

## Student Information

Name: 周朝賢
Student ID: 112310326

## Project Repository

GitHub link will be added here.

## Presentation Video

YouTube link will be added here.

---

## Project Overview

This final individual project examines the relationship between screen time and BMI percentile among high school students using the YRBS 2007 dataset.

The project follows a complete statistical workflow:

```text
research question → data preparation → method → result → interpretation
```

The main statistical method used in this project is **simple linear regression**.

---

## Research Question

Is there a linear relationship between screen time and BMI percentile among high school students?

---

## Dataset

This project uses the **YRBS 2007 National High School Survey** dataset.

The Youth Risk Behavior Survey includes information about high school students' health-related behaviors, including physical activity, screen time, dietary behavior, and body measurements.

---

## Variables

### Predictor Variable

`screen_time_hours`

This variable was created by combining:

- `TelevisionWatching`
- `ComputerUse`

The original variables were categorical responses. They were recoded into approximate numeric hours:

| Original Code | Approximate Hours |
|---:|---:|
| 1 | 0 |
| 2 | 0.5 |
| 3 | 1 |
| 4 | 2 |
| 5 | 3 |
| 6 | 4 |
| 7 | 5 |

Then, the total screen time variable was created as:

```text
screen_time_hours = tv_hours + computer_hours
```

### Response Variable

`bmi_percentile`

This variable represents BMI percentile among students.

---

## Data Preparation

The data cleaning process included the following steps:

1. Selected the variables needed for the analysis:
   - `TelevisionWatching`
   - `ComputerUse`
   - `BMIPCT`

2. Recoded `TelevisionWatching` and `ComputerUse` into approximate numeric hours.

3. Created a new variable:

```text
screen_time_hours = tv_hours + computer_hours
```

4. Renamed `BMIPCT` as `bmi_percentile`.

5. Removed rows with missing values in screen time or BMI percentile.

After cleaning, the final sample size was:

```text
n = 12,844
```

---

## Statistical Method

Simple linear regression was used to examine whether screen time is linearly related to BMI percentile.

The regression model was:

```text
Predicted BMI percentile = 61.6837 + 0.8374 × Screen time hours
```

The hypotheses were:

```text
H0: β1 = 0
H1: β1 ≠ 0
```

Where:

- `β1` is the slope for screen time.
- `H0` means there is no linear relationship between screen time and BMI percentile.
- `H1` means there is a linear relationship between screen time and BMI percentile.

---

## Key Results

| Statistic | Result |
|---|---:|
| Sample size | 12,844 |
| Intercept | 61.6837 |
| Slope | 0.8374 |
| 95% CI for slope | [0.6466, 1.0282] |
| p-value | p < 0.001 |
| R-squared | 0.0057 |
| Adjusted R-squared | 0.0056 |

---

## Interpretation

The slope was **0.8374**. This means that for each additional hour of screen time, the predicted BMI percentile increased by about **0.84 percentile points** on average.

The p-value was less than 0.001, so the null hypothesis was rejected. This suggests that there is statistically significant evidence of a positive linear relationship between screen time and BMI percentile.

However, the R-squared value was only **0.0057**. This means that screen time explained only about **0.57%** of the variation in BMI percentile. Therefore, although the relationship was statistically significant, the practical effect was weak.

---

## Conclusion

Higher screen time was associated with slightly higher BMI percentile among high school students. However, screen time alone explained very little variation in BMI percentile.

The main takeaway is:

```text
Screen time has a statistically significant but practically weak positive association with BMI percentile.
```

Because this study uses observational survey data, the result should be interpreted as **association**, not causation.

---

## Limitations

This project has several limitations:

1. Screen time was recoded from categorical responses into approximate numeric hours, so the measurement is not perfectly precise.

2. BMI percentile may be affected by many other factors not included in this simple regression model, such as diet, physical activity, sleep, genetics, and socioeconomic background.

3. The analysis uses observational survey data, so it cannot prove that screen time causes changes in BMI percentile.

4. The R-squared value was very small, which means screen time alone has limited ability to explain BMI percentile variation.

---

## Project Structure

```text
final-screen-time-bmi/
├── README.md
├── data/
│   ├── raw/
│   │   └── YRBS_2007.csv
│   └── processed/
│       ├── screen_time_bmi_cleaned.csv
│       └── screen_time_bmi_model_output.csv
├── notebooks/
│   ├── 01_data_cleaning_screen_time_bmi.ipynb
│   ├── 02_main_regression_screen_time_bmi.ipynb
│   └── 03_outputs_and_summary_screen_time_bmi.ipynb
├── outputs/
│   ├── figures/
│   ├── tables/
│   └── summary/
├── report/
│   └── one_page_infographic_content.md
└── references/
```

---

## Notebooks

### 1. `01_data_cleaning_screen_time_bmi.ipynb`

This notebook prepares the dataset for analysis. It recodes screen time variables, creates `screen_time_hours`, removes missing values, and saves the cleaned dataset.

### 2. `02_main_regression_screen_time_bmi.ipynb`

This notebook performs the main simple linear regression analysis. It outputs the regression summary, key results, regression figure, and residual plots.

### 3. `03_outputs_and_summary_screen_time_bmi.ipynb`

This notebook organizes the final results for the README, one-page infographic summary, and presentation video.

---

## Figures

The project includes the following figures:

- Distribution of screen time hours
- Distribution of BMI percentile
- Initial scatter plot of screen time and BMI percentile
- Regression line plot
- Residuals vs fitted values plot
- Residual distribution plot
- Q-Q plot of residuals

---

## Final Takeaway

This project found that screen time was positively associated with BMI percentile, but the effect was very small. The regression result was statistically significant because of the large sample size, but screen time explained only a very small portion of BMI percentile variation.

Therefore, screen time may be related to BMI percentile, but it should not be treated as the only or main factor explaining BMI percentile among high school students.
