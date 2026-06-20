# Variable Notes

## Dataset

This project uses the YRBS 2007 National High School Survey dataset.

## Research Question

Is there a linear relationship between screen time and BMI percentile among high school students?

## Variables Used

### TelevisionWatching

This variable measures the amount of time students reported watching television on an average school day.

### ComputerUse

This variable measures the amount of time students reported using computers or video games for non-school purposes on an average school day.

### BMIPCT

This variable represents BMI percentile.

## Recoding Method

The original screen time variables were categorical responses. They were recoded into approximate numeric hours as follows:

| Original Code | Approximate Hours |
|---:|---:|
| 1 | 0 |
| 2 | 0.5 |
| 3 | 1 |
| 4 | 2 |
| 5 | 3 |
| 6 | 4 |
| 7 | 5 |

Then, total screen time was created as:

```text
screen_time_hours = tv_hours + computer_hours