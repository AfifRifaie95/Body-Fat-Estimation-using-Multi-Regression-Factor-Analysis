# Body Fat Estimation using Multi-Linear Regression & Factor Analysis in SPSS  

![ezgif-6-a6c584d0d8](https://github.com/AfifRifaie95/SPSS-Multivariate-Methods-for-Data-Analysis/assets/159521904/cfe221ec-39ca-42ea-bf7d-8eace4887cbe)

# Multi Linear Regression Analysis
### Project Overview
The purpose of this research is to apply multi regression analysis with a stepwise method to analyze body fat as a dependent variable and related independent variable such as Density, Age, Weight, Height, Neck, Chest, Abdomen, Hip, Thigh, Knee, Ankle, Biceps, Forearm, and Wrist with the main goal of developing a predictive model for body fat association and estimation.

### Table of Contents
- [Multi Linear Regression Analysis](#Multi-Linear-Regression-Analysis)
- [Factor Analysis](#Factor-Analysis)

### Research Objectives
#### Objective 1
To develop a Multiple Linear Regression model using stepwise regression to predict body fat percentage based on a set of metric independent variables.

- Hypothesis 1.1: There is a significant relationship between the independent variables (Density, Age, Weight, Height, Neck, Chest, Abdomen, Hip, Thigh, Knee, Ankle, Biceps, Forearm, and Wrist) and body fat percentage.
- Hypothesis 1.2: The MLR model, including the selected independent variables, will significantly predict body fat percentage.
- Hypothesis 1.3: The stepwise regression method will result in a model that includes the most significant predictor variables for body fat percentage.

#### Objective 2
To assess the significance of individual predictor variables in the model and to identify which variables have the strongest impact on body fat.

- Hypothesis 2.1: Each independent variable significantly contributes to the prediction of body fat percentage.
- Hypothesis 2.2: Some variables will have a stronger impact on body fat percentage than others.
- Hypothesis 2.3: The exclusion of specific variables (e.g., Abdomen, Weight) will significantly improve the predictive accuracy of the model.

### Data Source
The dataset is obained from Kaggle [Available Here](https://www.kaggle.com/datasets/fedesoriano/body-fat-prediction-dataset)

### Software
- IBM SPSS Statistic [Available Here](https://www.ibm.com/products/spss-statistics/gradpack?adoper=227628_2&adobe_mc_sdid=SDID%3D6565759415F6A855-6F3279978D463447%7CMCORGID%3DD10F27705ED7F5130A495C99%40AdobeOrg%7CTS%3D1714019772&adobe_mc_ref=https%3A%2F%2Fwww.google.com%2F)

### Analysis Results and Interpretations
#### Assumption 1 – Linearity of the variables

The first assumption is to use the scatter plot to examine the correlation between the independent and dependent variables. Based on the Scatter Plot 1, there is no linear relationship between body fat and age or height. The density indicates a negative association, but the other predictors show a positive association.


<img width="309" alt="Screenshot 2024-03-21 115321" src="https://github.com/AfifRifaie95/SPSS-Multivariate-Methods-for-Data-Analysis/assets/159521904/13477397-097e-44c2-86cd-86edc67b1485">



The Pearson Correlation Table can also be used to check the linearity. Table 1 below demonstrates that the predictors have a positive linear relationship. However, there is a negative linear relationship between body fat to density and height. Furthermore, Heigh with a significance value of 0.078 greater than p-value 0.05 showed that Heigh is not statistically significant.



<img width="176" alt="Table 1 snipped of correlation table" src="https://github.com/AfifRifaie95/Multi-Regression-Analysis-for-Body-Fat-Percentage/assets/159521904/f831ef91-cb37-41c9-b5e9-5aa049566bdf">


#### Assumption 2 – Constant Variance of Error Term

The second assumption is that the Constant Variance of Error Term, also known as homoscedasticity, is checked. This assumption implies that the variance of the errors, or the spread of the residuals, should be roughly constant for all predictor variable values. According to the scatter plot 2, the points do not fall inside the plus minus 3 range. As a result, it shows that there is a heteroscedasticity problem. We will then examine each predictor to see which independent variables contribute to the outcome. According to scatter plot 4, the error term has attained constant variance after removing the density variable. The points are now normally distributed and range between plus and minus 3. As a result, homoscedasticity is met.


<img width="332" alt="Scatter Plot 2 Constant Variance of Error Term" src="https://github.com/AfifRifaie95/Multi-Regression-Analysis-for-Body-Fat-Percentage/assets/159521904/5a9da722-f9f5-42ba-8f3e-816fafd9e8ea">


<img width="324" alt="Scatter Plot 3 Constant Variance of Error Term of Density Variable" src="https://github.com/AfifRifaie95/Multi-Regression-Analysis-for-Body-Fat-Percentage/assets/159521904/33bdb358-91c3-4d5d-8380-7c9d5a76b312">


<img width="338" alt="Scatter Plot 4 Contant variance of Error Term after removal of Density Variable" src="https://github.com/AfifRifaie95/Multi-Regression-Analysis-for-Body-Fat-Percentage/assets/159521904/0bbe03e4-68fc-43a6-8c90-da3ba7c44d90">


### Assumption 3 – Independence of error term

The third assumption is the independence of errors term. This assumption states that the error term for one observation is not correlated with the error term of any other observation. One common method to check for independence of errors is the Durbin-Watson test. Based on table 2, the Durbin-Watson value is 1.789 close to 2, which indicates that there is no significant autocorrelation. Hence, the error terms are independent of one another.


<img width="370" alt="Table 2 Model Summary Table" src="https://github.com/AfifRifaie95/Multi-Regression-Analysis-for-Body-Fat-Percentage/assets/159521904/199dd408-b79b-4f27-ac9d-c330ff323a3d">


### Assumption 4 – Normality of error term

The fourth assumption is the normality of error terms. This assumption states that the errors (residuals) of the model are normally distributed. P-P plot and Normality test can be used to check for the normality of error term. The points drawn in P-P plot 1 fall along a straight diagonal line, indicating that residuals are regularly distributed. We utilize the Kolmogorov-Smirnov test for the Test of Normality because the sample size is more than 50. The significance value is 0.2, which is more than the P value of 0.05, hence fail to reject the null hypothesis and it indicates that the error terms are normally distributed.


<img width="279" alt="P-P plot 1  Normality of Error Term" src="https://github.com/AfifRifaie95/Multi-Regression-Analysis-for-Body-Fat-Percentage/assets/159521904/2fbf30a8-2ce7-4e13-8622-11e5ed923bb8">


<img width="307" alt="Table 3 Test of Normality" src="https://github.com/AfifRifaie95/Multi-Regression-Analysis-for-Body-Fat-Percentage/assets/159521904/c034f1f0-a26f-49b7-8bf1-0760fb94b6d5">


We can assume that the assumptions are met based on the Linearity, Constance Variance of Error Term, Independence of Error Term, and Normality of Error Term. Hence, we move on to the next step, analysis.


### Analysis Results and Interpretations 2

Based on the Model Summary Table, we may look at the R, R Square (R2), and R Square (R2) Change.


<img width="548" alt="image" src="https://github.com/AfifRifaie95/SPSS-Multivariate-Methods-for-Data-Analysis/assets/159521904/c3835b1e-6ae1-4ddf-a428-7a29c1c266e6">

R is the correlation coefficient, which measures the strength and direction of the linear relationship between the dependent variable and the independent variables. The final model shows 0.857 which close to 1, the predictors and Body Fat are positively associated.


R Square (R²) or known as coefficient of determination, which measures the proportion of the variance in the dependent variable that can be explained by the independent variables. In the final model, it shows that 73.5% of the variation of Body fat, is explained by abdomen, weight, wrist and forearm.


R Square Change (R²) is how much additional variance in the dependent variable is explained by adding a new set of independent variables to the model. In the final model, R square change increased from 0.660 to 0.735. The sig F change is 0.010 lower than P value 0.05, thus it is a significant change.


<img width="200" alt="Table 5 Correlation Table" src="https://github.com/AfifRifaie95/Multi-Regression-Analysis-for-Body-Fat-Percentage/assets/159521904/9ebe094c-7d97-46af-b828-05dce1adb1ff">


According to the Table 5, the significance values are 0.000, which is less than p-value 0.05, indicating that there is a statistically significant correlation between the dependent and independent variables.


<img width="348" alt="Table 6 Correlation Table" src="https://github.com/AfifRifaie95/Multi-Regression-Analysis-for-Body-Fat-Percentage/assets/159521904/cafaab1b-7ff4-4ee7-8d8d-a2984bcaf412">


The significance value of the final model in the ANOVA table is <0.001, which is less than p-value 0.05. It implies that at least one of the independent variables explains Body Fat well.


<img width="782" alt="Table 7 Coefficient Table" src="https://github.com/AfifRifaie95/Multi-Regression-Analysis-for-Body-Fat-Percentage/assets/159521904/d0cb69b0-8ec6-43c2-a4b1-a0b0e8ef1829">


Unstandardized B is a measure that is used to describe the change in the dependent variable for a one-unit change in an independent variable while holding all other variables constant. According to the model, increasing the abdomen by one unit increases body fat by 0.996. A one-unit increase in weight results in a 0.136-unit decrease in body fat. A one-unit increase in wrist reduces body fat by 1.506. Body fat increases by 0.473 units for every unit increase in forearm.


The 95% Confidence Interval for B coefficient indicates the range of values within which the true coefficient is most likely to reside with 95% confidence. Based on the table 7, we can conclude that; as 95% confidence interval does not include value 0, Hence, it can be concluded that abdomen, weight, wrist and forearm are significant independent variables.


The Variance Inflation Factor (VIF) analysis measures the degree of multicollinearity among independent variables. Based on the table 7, Multicollinearity does not appear to be a major issue for any of the four variables in the model. Specifically, the VIF for abdomen is 4.8, indicating a moderate level of multicollinearity, while the VIF for weight is slightly higher at 7.0, suggesting some potential multicollinearity. However, both are below the threshold of 10. The VIF values for wrist and forearm are even lower, at 2.2 and 1.7 respectively, indicating that multicollinearity is not a concern for these variables.


The Tolerance value is the degree of variance in an independence variable that cannot be explained by the other independent variables. Multicollinearity does not appear to be a significant concern for any of the four variables in the model based on the tolerance values, as all values abdomen 0.206, weight 0.142, wrist 0.440, forearm 0.558 are above the 0.1 threshold, indicating that the proportion of variance not explained by other variables is satisfactory.


We can conclude that the regression model is appropriate and significant based on these findings. The model explains a considerable percentage of the variance in Body Fat, and the predictors are significant but not significantly linked with one another.

### Conclusion and Recommendation

The goal of this study was to use a Multiple Linear Regression model with a stepwise method to measure body fat percentage and its associated independent variables. The goal of the study was to create a prediction model for body fat association and quantification based on a set of metric independent variables: density, age, weight, height, neck, chest, abdomen, hip, thigh, knee, ankle, biceps, forearm, and wrist.


The regression model was found to be significant, with a R Square value of 73.5%, implying that the four relevant predictors: abdomen, weight, wrist, and forearm, explain approximately 73.5% of the variation in body fat. The positive correlation coefficient (R) of 0.857 indicates a strong positive association between the predictor variables and body fat. The ANOVA test further confirmed the significance of the model.


### Objective 1
The Multiple Linear Regression model was successfully developed using stepwise regression to predict body fat percentage with selected variables (Abdomen, Weight, Wrist, Forearm).


- Hypothesis 1.1: Supported, as significant relationships were found between body fat percentage and the independent variables in the model.
- Hypothesis 1.2: Supported, as the model significantly predicts body fat percentage with a significant F value and R² value of 73.5%.
- Hypothesis 1.3: Supported, as stepwise regression resulted in a model that includes significant predictor variables for body fat percentage.


### Objective 2
The significance and impact of individual predictor variables in the model were assessed.


- Hypothesis 2.1: Partially supported, as not all original independent variables were included in the final model, indicating that not all significantly contribute to the prediction of body fat percentage.
- Hypothesis 2.2: Supported, as standardized coefficients (Beta) indicate varying strengths of impact on body fat percentage.
- Hypothesis 2.3: Supported, as the exclusion of specific variables like Abdomen and Weight significantly improved the predictive accuracy of the model.


### Finding

The findings of this study have important implications for understanding and managing obesity. The prediction model can help healthcare practitioners and individuals make educated decisions about obesity prevention and treatment.


### Limitation


Secondary data were used in the study, which means they may not be 100% accurate and the model suggests that the predictor variables and the dependent variable are linked in a straight line, but this might not always be the case.


# Factor Analysis

### Project Overview

The goal of factor analysis is to perform data summarization and data reduction. Data summarization is the process of reducing the amount of data in a dataset so that it is easier to understand. This is done in factor analysis by finding the underlying latent factors that show how the measured variables are related to each other.

### SPSS Output for factor analysis on metric independent variables 


<img width="782" alt="Table 2 Correlation Matrix" src="https://github.com/AfifRifaie95/Multi-Regression-Analysis-for-Body-Fat-Percentage/assets/159521904/49fa82ef-e280-4906-9cd3-1b53e87ef355">



<img width="592" alt="Table 3 KMO and Bartlett’s Test" src="https://github.com/AfifRifaie95/Multi-Regression-Analysis-for-Body-Fat-Percentage/assets/159521904/7d9e065e-cdb1-4564-ae9f-0cfd4bed5e51">



<img width="188" alt="Table 4 Communalities Table" src="https://github.com/AfifRifaie95/Multi-Regression-Analysis-for-Body-Fat-Percentage/assets/159521904/4a7c751b-7db2-4c7d-8d11-16f3838a5ba0">



<img width="711" alt="Table 5 Total Variance Explained Table" src="https://github.com/AfifRifaie95/Multi-Regression-Analysis-for-Body-Fat-Percentage/assets/159521904/f54848ad-af9b-4e9f-affc-17371ca9b99d">



<img width="517" alt="Scree Plot 1" src="https://github.com/AfifRifaie95/Multi-Regression-Analysis-for-Body-Fat-Percentage/assets/159521904/bf6c7af0-24d4-4c06-9dd8-7eb40bde4f8b">



<img width="248" alt="Table 6 Component Matrix Table" src="https://github.com/AfifRifaie95/Multi-Regression-Analysis-for-Body-Fat-Percentage/assets/159521904/0e52aa6b-d351-4e41-95e0-cbdaec5aac38">



<img width="290" alt="Table 7 Rotated Component Matrix Table" src="https://github.com/AfifRifaie95/Multi-Regression-Analysis-for-Body-Fat-Percentage/assets/159521904/c12b3bbd-99c7-4cc2-a67e-f0017d3c3fc1">


<img width="341" alt="Table 8 Component Transformation Matrix Table" src="https://github.com/AfifRifaie95/Multi-Regression-Analysis-for-Body-Fat-Percentage/assets/159521904/6769564a-1bdb-4994-bb3c-ee657f3bb8c1">



### By using relevant SPSS outputs, group metric independent variables into factors.


To retain the number of factors, the eigenvalue must be higher than 1. As per Table 5 below, the total value that is higher than 1 is component 1, component 2, and component 3. Hence, 3 factor is retained.


In addition to that, number of factors to retain can be look at percentage of variance. Factor 1 explains 59.5% of the variation in the 15 items. Factor 2 explains 12.7 % of the variation in the 15 items. Factor 3 explains 7.2 % of the variation in the 15 items.


<img width="707" alt="image" src="https://github.com/AfifRifaie95/Multi-Regression-Analysis-for-Body-Fat-Percentage/assets/159521904/325343f8-2c8a-4e08-9aa2-5963d83d04bb">


The Scree Test Criterion, scree plot 1 shows a scree line starts to flattening after third factor, it suggests that the first three factors explain a significant amount of variance in the items, and the remaining factors explain only a small additional amount of variance. Therefore, we would retain the first three factors.


<img width="517" alt="Scree Plot 1" src="https://github.com/AfifRifaie95/Multi-Regression-Analysis-for-Body-Fat-Percentage/assets/159521904/0f7c9ac1-2300-46d2-b800-e8bf1f2f0115">


To know which variables has been assigned to which factor can be looked at the component Matrix. The values in the Component Matrix table can range from -1 to 1, where -1 indicates a perfect negative correlation, 1 indicates a perfect positive correlation, and 0 indicates no correlation. The variable that has higher value will be retained in that particular factor.


<img width="248" alt="Table 6 Component Matrix Table" src="https://github.com/AfifRifaie95/Multi-Regression-Analysis-for-Body-Fat-Percentage/assets/159521904/6ccdbff8-315a-44b7-a1ee-f9436b648cfb">


### Interpret the meaning of communality


Communality represents the proportion of a variable's total variance that is accounted for by the common factors and the communality values range from 0 to 1.


Based Table 4 Communalities Table, all items indicate a communality value close to 1. Which indicates that most of the variance in the item is well-represented by the factors.


<img width="188" alt="Table 4 Communalities Table" src="https://github.com/AfifRifaie95/Multi-Regression-Analysis-for-Body-Fat-Percentage/assets/159521904/e038d590-0732-412b-bdfc-4fcad8cdae16">


### Interpret the meaning of eigenvalue 


Eigenvalue is a measure of the variance in the item that is accounted for by a factor. It represents the total variance explained by the factor. Eigenvalues are used to determine the number of factors to retain and factors with eigenvalues greater than 1 are to be retained.


Based on the table 5 below, the total Eigen value that is higher than 1 is component 1, component 2, and component 3. Hence, 3 factor is retained.


<img width="711" alt="Table 5 Total Variance Explained Table" src="https://github.com/AfifRifaie95/Multi-Regression-Analysis-for-Body-Fat-Percentage/assets/159521904/f72e634c-dfbd-4482-8fbd-c8778021ffcd">


### Explain briefly how the factorability of the dataset can be improved prior to the task of factor analysis.


Factorability can be improved by checking the Multicollinearity. High multicollinearity among variables can improve factorability and it can be checked by examining the correlation matrix. Pairs of variables with correlations above 0.3 indicate potential shared variance that can be captured by factors.


<img width="782" alt="Table 2 Correlation Matrix" src="https://github.com/AfifRifaie95/Multi-Regression-Analysis-for-Body-Fat-Percentage/assets/159521904/22ab8f54-0512-4674-9546-826b0ba5c995">


In addition to that, we can use Kaiser-Meyer-Olkin (KMO) Measure. The KMO measure is a statistic that indicates the proportion of variance among variables that might be common variance. A KMO value close to 1 indicates that factor analysis is likely to be useful, while a value below 0.5 indicates the opposite. Table 3 below shows the KMO of 0.906 which closer to 1.


<img width="592" alt="Table 3 KMO and Bartlett’s Test" src="https://github.com/AfifRifaie95/Multi-Regression-Analysis-for-Body-Fat-Percentage/assets/159521904/74f496aa-4b57-4acf-acbd-4f581c1e9fce">


### Explain what is meant by factor cross-loading.


Cross-loading refers to the situation where a variable has significant loadings on two or more factors. This means that the variable is associated with more than one underlying factor. In the output table 7 below. Chest, Hip and thigh show cross-loading when the variable has significant loadings in factor 1 and factor 2.


<img width="290" alt="Table 7 Rotated Component Matrix Table" src="https://github.com/AfifRifaie95/Multi-Regression-Analysis-for-Body-Fat-Percentage/assets/159521904/12c36188-1b1b-4b88-bc9f-c92176f50c2e">


### Suggestions on how the problem of cross-loading can be reduced.


The problem of cross-loading can be reduced by increase the sample size. Cross-loadings happens due to sample size issues. Increasing the sample size can provide more stable and reliable estimates of factor loadings.


Other suggestions are to implement rotation method such as Orthogonal or Oblique rotation. Rotation can make it easier to interpret and understand the factors. This rotation method is to see the clearer factor structure with fewer cross-loadings. If the cross loading still happening, it is best to drop the variable and re-run the analysis.



### References
- Ai, T. Y., Yee, T. S., Tieng, S. T. S., & Jie, Y. X. (2021). FACTORS THAT CAUSE THE PROBLEM OF OBESITY AMONG ADULTS IN TAMAN SENTOSA, KLANG. Malaysian Journal of Business and Economics (MJBE), 8(1), Article 1. https://doi.org/10.51200/mjbe.vi.3320
- Akindele, M. O., Phillips, J. S., & Igumbor, E. U. (2016). The Relationship Between Body Fat Percentage and Body Mass Index in Overweight and Obese Individuals in an Urban African Setting. Journal of Public Health in Africa, 7(1), 515. https://doi.org/10.4081/jphia.2016.515
- Frankenfield, D. C., Rowe, W. A., Cooney, R. N., Smith, J. S., & Becker, D. (2001). Limits of body mass index to detect obesity and predict body composition. Nutrition, 17(1), 26–30. https://doi.org/10.1016/S0899-9007(00)00471-8
- Pawan Kumar Jha1, Subhasis Mukherjee2, Purab Kalyan Modak3, Sharada Mayee Swain4. (2022). Establishing and testing a multiple regression equation to predict body fat from height, weight, waist circumference, and hip circumference. National Journal of Physiology, Pharmacy and Pharmacology, 12(05), 698.
- Tiwari, A., & Balasundaram, P. (2023). Public Health Considerations Regarding Obesity. In StatPearls. StatPearls Publishing. http://www.ncbi.nlm.nih.gov/books/NBK572122/

