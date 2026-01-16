# Data Dictionary — cardio_train.csv

Source: https://www.kaggle.com/datasets/sulianova/cardiovascular-disease-dataset

## Columns
- id: Row identifier
- age: Age in days (converted in notebook to age_years)
- gender: Sex (dataset encoded as 1/2)
- height: cm
- weight: kg
- ap_hi: Systolic blood pressure (mmHg)
- ap_lo: Diastolic blood pressure (mmHg)
- cholesterol: 1 normal, 2 above normal, 3 well above normal
- gluc: 1 normal, 2 above normal, 3 well above normal
- smoke: 0/1
- alco: 0/1
- active: 0/1
- cardio: target label (0 no CVD, 1 CVD)

## Engineered (in notebook)
- age_years: age / 365.25
- bmi: weight / (height_m^2)
