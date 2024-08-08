# Moni; updated 8-7-2024

Project: to see if any data points are statistically significant in predicting interstitial fluids

Non-invasive blood glucose / interstitial fluids predictor (if any x variables are statistically significant)

Project issues: I don't have any electrical spectroscopy to measure wrist data (I used apple and fitbit watches for heart rate)

## if you want to help; please reach out; I am looking for other variables/devices to test on ~ electrical signals on wrist would be ideal

Products used:

[Link](https://www.amazon.com/gp/product/B0D456ZHQQ/ref=ppx_yo_dt_b_asin_title_o00_s00?ie=UTF8&psc=1)

![image](https://github.com/user-attachments/assets/5b2bc504-a235-41d4-b86b-ae5c81cbd7ae)

[Link](https://www.amazon.com/gp/product/B0B2ZM4PXG/ref=ppx_yo_dt_b_asin_title_o01_s00?ie=UTF8&psc=1)

![image](https://github.com/user-attachments/assets/52784e48-2504-41cf-a380-8b54ce9d8c75)

[Link](https://www.amazon.com/gp/product/B0CXSNG2W4/ref=ppx_yo_dt_b_asin_title_o01_s00?ie=UTF8&psc=1)

![image](https://github.com/user-attachments/assets/043a4b75-9fd7-4b8c-97f6-05b401cfae87)

[Link](https://www.amazon.com/gp/product/B07PQ8WTC4/ref=ppx_yo_dt_b_asin_title_o01_s00?ie=UTF8&psc=1)

![image](https://github.com/user-attachments/assets/17a3e31b-6e5c-4d44-86c4-bacc0c26a3c0)

Measure these with interstitial fluids of Medtronic 780G pump > document data in spreadsheet > run predictive analysis equations

Model(s) used: multivariate linear regression, ridge regression, polynomial regression, lasso regression, elastic net regression; Adjusted R-squared:; 

No variables show statistical significance as of today; p value < .05

Since no variables show significance, I use the average of all the models used to predict blood glucose/interstitial fluids.

Equation: = 1267.57 - 10.57 * A2 - 1.2 * B2 + 1.62 * C2 + 0.15 * D2 + 0.24 * E2 - 6.33 * F2 - 5.24 * G2

= -5554.84 - 0.018 * A2 + 0.001 * B2 - 0.019 * C2 + 0.023 * D2 + 0.005 * E2 - 0.005 * F2 + 0.004 * G2 - 2.207 * (A2^2) + 1.421 * (A2 * B2) + 2.339 * (A2 * C2) - 0.248 * (A2 * D2) + 2.392 * (A2 * E2) - 2.291 * (A2 * F2) - 3.174 * (A2 * G2) - 0.821 * (B2^2) + 1.861 * (B2 * C2) - 0.725 * (B2 * D2) + 0.089 * (B2 * E2) + 0.491 * (B2 * F2) + 0.678 * (B2 * G2) - 1.101 * (C2^2) + 0.488 * (C2 * D2) - 0.638 * (C2 * E2) - 0.072 * (C2 * F2) - 0.535 * (C2 * G2) + 0.269 * (D2^2) - 0.009 * (D2 * E2) + 0.449 * (D2 * F2) - 0.374 * (D2 * G2) + 0.224 * (E2^2) + 2.705 * (E2 * F2) - 2.83 * (E2 * G2) - 1.416 * (F2^2) - 0.044 * (F2 * G2) + 1.68 * (G2^2)

= -5854.11
+ 0.065 * A2
- 0.051 * B2
- 0.062 * C2
+ 0.023 * D2
- 0.006 * E2
+ 0.003 * F2
+ 0.014 * G2
- 2.263 * (A2^2)
+ 1.18 * (A2 * B2)
+ 2.649 * (A2 * C2)
- 0.207 * (A2 * D2)
+ 2.631 * (A2 * E2)
- 2.429 * (A2 * F2)
- 3.242 * (A2 * G2)
- 0.835 * (B2^2)
+ 1.885 * (B2 * C2)
- 0.752 * (B2 * D2)
+ 0.06 * (B2 * E2)
+ 0.831 * (B2 * F2)
+ 0.413 * (B2 * G2)
- 1.133 * (C2^2)
+ 0.486 * (C2 * D2)
- 0.564 * (C2 * E2)
- 0.246 * (C2 * F2)
- 0.418 * (C2 * G2)
+ 0.288 * (D2^2)
- 0.008 * (D2 * E2)
+ 0.704 * (D2 * F2)
- 0.631 * (D2 * G2)
+ 0.234 * (E2^2)
+ 2.344 * (E2 * F2)
- 2.516 * (E2 * G2)
- 1.032 * (F2^2)
- 0.971 * (F2 * G2)
+ 2.256 * (G2^2)

= 339.52 + 64.935 * A2 - 2.635 * B2 - 9.645 * C2 + 8.444 * D2 + 6.872 * E2 + 0 * F2 - 0 * G2 - 4.46 * (A2^2) - 0.148 * (A2 * B2) + 4.609 * (A2 * C2) - 0.978 * (A2 * D2) + 1.65 * (A2 * E2) - 1.74 * (A2 * F2) - 2.801 * (A2 * G2) - 0.038 * (B2^2) + 0.182 * (B2 * C2) - 0.328 * (B2 * D2) - 0.002 * (B2 * E2) + 0.182 * (B2 * F2) + 0.098 * (B2 * G2) + 0.221 * (C2^2) + 0.036 * (C2 * D2) - 0.057 * (C2 * E2) - 0.442 * (C2 * F2) - 0.157 * (C2 * G2) + 0.102 * (D2^2) - 0.158 * (D2 * E2) + 0.438 * (D2 * F2) - 0.141 * (D2 * G2) + 0.097 * (E2^2) + 0.043 * (E2 * F2) - 0.165 * (E2 * G2) + 0.561 * (F2^2) - 1.332 * (F2 * G2) + 0.779 * (G2^2)

= 56.98
+ 0.811 * A2
- 1.779 * B2
- 2.451 * C2
+ 2.687 * D2
+ 3.386 * E2
+ 0 * F2
- 0 * G2
- 3.497 * (A2^2)
- 0.061 * (A2 * B2)
+ 4.897 * (A2 * C2)
- 0.739 * (A2 * D2)
+ 1.431 * (A2 * E2)
- 1.358 * (A2 * F2)
- 2.935 * (A2 * G2)
- 0.035 * (B2^2)
+ 0.188 * (B2 * C2)
- 0.352 * (B2 * D2)
+ 0.02 * (B2 * E2)
+ 0.143 * (B2 * F2)
+ 0.116 * (B2 * G2)
+ 0.196 * (C2^2)
+ 0.04 * (C2 * D2)
- 0.039 * (C2 * E2)
- 0.488 * (C2 * F2)
- 0.18 * (C2 * G2)
+ 0.104 * (D2^2)
- 0.111 * (D2 * E2)
+ 0.489 * (D2 * F2)
- 0.159 * (D2 * G2)
+ 0.081 * (E2^2)
+ 0.034 * (E2 * F2)
- 0.168 * (E2 * G2)
+ 0.565 * (F2^2)
- 1.266 * (F2 * G2)
+ 0.782 * (G2^2)

avg these equations and predict blood glucose/interstitial fluids levels

A2: Acetone ketones ppm
B2: Blood Pressure Top
C2: Blood Pressure Bottom
D2: Pulse
E2: Heart Rate
F2: Temperature
G2: Pulse Oxygen

P values:

Acetone ketones ppm: 

Blood Pressure Top:

Blood Pressure Bottom: 

Pulse:

Heart Rate:

Temperature: 

Pulse Oxygen: 

![image](https://github.com/user-attachments/assets/1b0afaed-8d2d-4193-b653-3bdea7df973d)

## Surprisingly, acetone ketones ppm have an inverse relationship with interstitial fluids; albeit a small sample size
