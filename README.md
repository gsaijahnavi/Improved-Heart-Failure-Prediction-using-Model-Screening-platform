# Improved Heart Failure Prediction using Model Screening platform
## Best poster award at JMP discovery Summit 2023

## Introductiom

Cardiovascular disease is the number one cause of death globally, claiming an estimated 17.9 million lives in 2019, accounting for 32% of all deaths worldwide that year.【1】
Developed a classification model for classifying Heart disease. Leveraged predictions using  Model Screening, Model Comparison, and Dashboard feature in JMP 16. The model output will help in understanding the importance of factors leading to heart disease and the probability of developing heart disease under certain conditions.
## Objective:
To build the best model and also to find factors that are leading to heart failure.

## Methodology

The data set included 918 participants from different countries and 11 factors associated with heart failure, such as age, sex, blood pressure, blood glucose.
Performed pre-processing of data by exploring null values and outliers. Further, performed Exploratory Data Analysis to understand the importance and relationship of each feature in relation to heart failure.

To build the model,  we incorporated the following JMP-16 capabilities in our methodology.
### Model Screening: An efficient platform for simultaneously fitting, comparing, exploring, selecting, and then deploying the best predictive model. 
### Model Comparison: Enables easy to compare and select the best-performing predictive model.
### Dashboards: Efficient way to better represent EDA concisely also it can be run anytime as new data is available. 

![image](https://user-images.githubusercontent.com/82319213/218238621-e6347cd5-5292-4e7b-a193-c78de3d472e9.png)

## Exploring Outliers & Null Values
While exploring the outliers, we identified some patients have higher values on some tests. Since the dataset reflected the actual physical condition of the patient, we decided not to exclude or impute these values.
![image](https://user-images.githubusercontent.com/82319213/218238666-1ba8e741-ff81-4048-816c-93be6d6ac156.png)
![image](https://user-images.githubusercontent.com/82319213/218238680-0823a618-61e5-4b8a-9de0-b4e5bfc1ba97.png)![image](https://user-images.githubusercontent.com/82319213/218238686-4e9bb699-081c-4a91-9397-0216e82c80d1.png)
![image](https://user-images.githubusercontent.com/82319213/218238693-bdc3071c-0bf2-4645-ae2e-74be79c47fed.png)
![image](https://user-images.githubusercontent.com/82319213/218238762-5351bb96-a848-4e5e-a30a-b0a092e87e84.png)
![image](https://user-images.githubusercontent.com/82319213/218238935-13c2e83c-b8f7-4ad9-bf06-17447b5f0d99.png)

## Exploratory Data Analysis
### Influence of Gender
Gender is an important element since men who suffer from heart disease are twice as likely as women.

![image](https://user-images.githubusercontent.com/82319213/218238962-6b6f83f5-8029-4720-9454-75b843dd1425.png)

### Influence of Fasting Blood Sugar
Blood sugar also has a big impact on heart disease because diabetic have a higher risk of heart disease.
![image](https://user-images.githubusercontent.com/82319213/218239068-00d14f71-7f26-43af-95b3-0c2e5d9a3152.png)
###  Influence of ST Slope
The ST slope of the electrocardiogram after exercise is also a relatively clear judgment basis. A flat slope means higher risk.
![image](https://user-images.githubusercontent.com/82319213/218239098-e37f61d6-e32a-41c7-a0a5-42c6fbf84181.png)

### Influence of Chest Pain Type 
ASY is shown to be the most dangerous type of chest pain as it has the highest incident rate of heart disease.
![image](https://user-images.githubusercontent.com/82319213/218239222-d8983ad6-b99d-4c4f-a388-4b8bb4d0afa7.png)

### Influence of Blood sugar
Blood sugar also has a big impact on heart disease because diabetics have a higher risk of heart disease.
![image](https://user-images.githubusercontent.com/82319213/218239397-0108030d-9e20-4ada-b9ee-f16194b11c05.png)

## Results
### Models 
![image](https://user-images.githubusercontent.com/82319213/218239540-3c20cc66-bfd6-4f38-8e91-3eb48d86bdad.png)
#### Confusion matrix
![image](https://user-images.githubusercontent.com/82319213/218239632-f2a7177a-03f6-4fd0-9f69-4d21bba8cc4d.png)
### ROC curve
![image](https://user-images.githubusercontent.com/82319213/218239636-c79344bc-21f2-4ba7-bacd-18a618489dd0.png)

* Chosen model with the least number of False Positives (9) as the cost is high.
* Accuracy achieved is 90.6%, with an AUC of 95.5.

## Column contributions
![image](https://user-images.githubusercontent.com/82319213/218239660-21329851-e264-44db-b716-70bdfb1646ad.png)
* Exercise Angina, Sex, FastingBS, Resting ECG, ST_slope,ChestpainType contribute more than 75% to heart failure.

* Cholesterol, RestingBP, MaxHR, Oldpeak, and Age contribute least to our target.

* These least predictors are shown statistically insignificant in our logistic regression, so they can be omitted to reduce the complexity of the model


## Model comparision
![image](https://user-images.githubusercontent.com/82319213/218239698-e6d82f93-cd02-4fb2-83aa-1850e76f70de.png)

## Profiler
![image](https://user-images.githubusercontent.com/82319213/218239712-4ebaf4d6-d6be-4fe1-bff7-cdda31ac1cac.png)
* Using the profiler feature in JMP-16, we can predict heart risk of a new patient based on inputting his vitals like Age, chest pain, etc.  
* We noticed Male Diabetic with a flat pattern in ECG is shown to be more prone to a heart attack.




## Conclusion
* Using a model screening platform, we explored the best predictive model for heart failure prediction.
* Leveraged the JMP 16 dashboard utility to develop an interactive platform that outputs the probability of heart failure based on input parameters.

![image](https://user-images.githubusercontent.com/82319213/218239688-eba03f97-507b-40da-99b8-e4e3ecfbd621.png)















