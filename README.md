# Moni; updated 8-26-2024

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

=-1161.0931709756671 + (6.216162514840597 * A2) + (-0.6844709384640743 * B2) + (-0.8752494043432677 * C2) + (0.03745623235827271 * D2) + (0.7220013292763969 * E2) + (1.2956058505741308 * F2) + (12.742887131883645 * G2)

R-squared:                       0.144

Adj. R-squared:                  0.004

A2: Acetone ketones ppm
B2: Blood Pressure Top
C2: Blood Pressure Bottom
D2: Pulse
E2: Heart Rate
F2: Temperature
G2: Pulse Oxygen

![image](https://github.com/user-attachments/assets/06fdfbea-4a15-4891-9af9-4a7c5090f3c9)


Arduino using infrared data to predict interstitial fluids

Products used:

![618AQOe0NKL _AC_SL1100_](https://github.com/user-attachments/assets/2399472b-61ae-41e0-8b87-3d8eca41b736)
[https://www.amazon.com/dp/B0CD719R4M?ref=ppx_yo2ov_dt_b_fed_asin_title
](https://www.amazon.com/dp/B081CSJV2V?ref=ppx_yo2ov_dt_b_fed_asin_title&th=1)

![71+6rfcO+DL _SL1500_](https://github.com/user-attachments/assets/1bdba1cf-9245-485e-a37e-699bee3d91ff)
https://www.amazon.com/dp/B0CD719R4M?ref=ppx_yo2ov_dt_b_fed_asin_title

This method showed strong p value but low r square which shows some promise.

https://github.com/user-attachments/assets/d5aa779c-29b8-4b05-bfbd-93402fec3b7b

Blood glucose=152.93+0.0008×IR data
P-value for the model: 0.00151
Adjusted R-squared (Adj. R²): 0.111


(999.7440627574921,
 0.6610514928733869,
 '5549950781761.6504 + -168180325243.0623*Age + 0.0000*Gender + -0.7622*Acetone_ppm + -0.0468*Blood_Pressure_Top + -0.5050*Blood_Pressure_Bottom + 0.2330*Pulse + -0.1593*Heart_Rate + -0.6113*Temperature + 0.0854*Pulse_Oxygen + 0.0000*Age^2 + 0.0000*Age Gender + -25.1530*Age Acetone_ppm + -1.5437*Age Blood_Pressure_Top + -16.6643*Age Blood_Pressure_Bottom + 7.6885*Age Pulse + -5.2563*Age Heart_Rate + -20.1722*Age Temperature + 2.8191*Age Pulse_Oxygen + -0.0000*Gender^2 + -0.7622*Gender Acetone_ppm ')
