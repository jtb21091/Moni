# Moni; updated 8-7-2024

Project: to see if any data points are statistically significant in predicting interstitial fluids

Non-invasive blood glucose / interstitial fluids predictor (if any x variables are statistically significant)

Project issues: I don't have any electrical spectroscopy to measure wrist data (I used apple and fitbit watches for heart rate)

## if you want to help; please reach out

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

Model(s) used: multivariate linear regression; Adjusted R-squared: 0.164; 

Equation: =(-6.8537 * A2) + (-1.5829 * B2) + (2.8971 * C2) + (0.0020 * D2) + (0.4606 * E2) + (-10.5783 * F2) + (-0.0803 * G2) + 1117.6774

A2: Acetone ketones ppm
B2: Blood Pressure Top
C2: Blood Pressure Bottom
D2: Pulse
E2: Heart Rate
F2: Temperature
G2: Pulse Oxygen


Variable	Coefficient	Std. Error	t-Statistic	P-value	95% Confidence Interval
const	1117.6774	1407.446	0.794	0.448	[-2066.186, 4301.541]
Acetone ketones ppm	-6.8537	7.705	-0.890	0.397	[-24.284, 10.576]
Blood Pressure Top	-1.5829	1.816	-0.872	0.406	[-5.690, 2.524]
Blood Pressure Bottom	2.8971	3.112	0.931	0.376	[-4.143, 9.937]
Pulse	0.0020	0.834	0.002	0.998	[-1.885, 1.889]
Heart Rate	0.4606	0.715	0.644	0.536	[-1.157, 2.078]
Temperature	-10.5783	12.359	-0.856	0.414	[-38.535, 17.379]
Pulse Oxygen	-0.0803	11.003	-0.007	0.994	[-24.972, 24.811]
