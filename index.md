# **Health Risk and Resilience Profiles: Using Data Science to Promote Healthy Living**
## *Data Incubator Project Proposal*
## *Meghan Colosimo, M.S., Ph.D. Candidate (Clinical Health Psychology)*
### Introduction:
Data on health-related risk and protective factors are vital to the prediction of overall physical/mental health and well-being, as well as the development and prognosis of specific chronic illnesses (e.g., heart disease, stroke, asthma, cancer, diabetes, etc.). The Centers for Disease Control and Prevention (CDC) conducts a telephonic, self-report survey annually in order to gather comprehensive information on the current quality of Americans' health, as well as the extent of their engagement in health promoting/disparaging behaviors (e.g., exercise, diet, use of preventative care, substance use, etc.). This national research project, known as the Behavioral Risk Factor Surveillance System (BRFSS), provides a rich, multivariate dataset spanning over three decades of standardized data collection (1984 - 2016) that is publicly accessible. This project aims to employ the most recently collected BRFSS data (2016; ~ 216 MB) in order to improve public awareness of health risk, resilience, and concrete health behavior modifications. Synthesis of the valuable data housed in the BRFSS database into digestible, directly applicable suggestions for improving health and wellness among the general public has the potential for major, positive economic and social impacts on the healthcare industry.

### Project Aims: 
Application of advanced statistical modeling techniques to the Centers for Disease Control and Prevention 2016 Behavioral Risk Factor Surveillance System (BRFSS) dataset, specifically standard multiple regression and logistic regression, will allow the general public to generate individualized "Health Risk and Resilience Profiles (HRPs)" based on the input of demographic and behaviorally modifiable factors, relative to national averages. Furthermore, in addition to obtaining a data-driven understanding of their predicted health risks, users will be provided with a tailored assessment of healthy living "strengths" as well as "opportunities for improvement." HRP opportunities for improvement will highlight the most salient targets of intervention based on the relative strength of behaviorally modifiable predictors (e.g., diet, exercise, substance use) contributing to a specific, high risk disease outcome. Conversely, health promoting behaviors indicated in HRP strengths will provide positive reinforcement and ongoing motivation for those activities in which an individual is already engaged in order to reduce their risk for chronic disease development.

The proposed project was born out of my background in clinical health psychology and penchant for evidence-based intervention supported by data science. I am dedicated to applied clinical research, which by definition yields deliverables that are directly applicable to patient populations and improving wellness. Thus, this project emphasizes public access to valuable health-related data and empirically identified intervention.

### Data Analytic Plan:
Standard multiple linear regression analyses will be utilized to generate a multivariate statistical model to predict continuous outcomes based on the the combined contributing variances of each continuous/categorical (dummy coded) IV included in the model. Conversely, logistic regression analyses will be employed to predict dichotomous outcomes (e.g., disease group membership), while discriminate function analyses will be recruited when predicting categorical outcomes with more than two groups. Assumptions corresponding to each type of regression analysis (e.g., multicollinearity, outliers, normality, linearity, homoscedasticity) will be assessed prior to model interpretation. Beta values (multiple regression) and odds ratios (logistic regression) will be used to interpret that relative strength/value of predictors.

### Project Deliverables:
At the conclusion of the proposed project, deliverables will include:
1. Development of a web-based, user friendly application where the general public can interface with BRFSS data in a meaningful, applied manner. End-users will have the ability to input various demographic/behavioral factors and select chronic disease outcomes of interest.
2. Generation of Health Risk and Resilience Profiles (HRPs) based on user inputs and underlying multiple regression models. HRPs will include graphics indicating where an individual falls on predicted risk for particular disease outcomes compared to deviation from the national average. 
3. Generation of a targeted Health Assessment, including strengths and opportunities for health improvement, based on relative weight of behaviorally modifiable predictors.

### Exploratory Data Analysis:
A sample logstic regression model was designed to assess the feasability of the proposed project, with the goal of predicting diabetes group membership (DV) based on three blocks of theoretically relevant variables included in the BRFSS (2016) database: demographics, modifiable health-related behaviors/characteristics, and perceived physical/mental health-realted quality of life (QoL). Table 1 provides an outline of the model's structure.

Block | Variables Entering Model
------|--------------------------
Block 1: Demographics | Sex, Marital Status, Employment Status, Race, Age, Education Level, Income
Block 2: Modifiable Health Behaviors | BMI, Tobacco Use, Smokeless Tobacco Use, Alcholic Drinks (per week), Physical Activity, Sleep
Block 3: Health-related QoL| Physical QoL, Mental QoL

#### Preliminary Results:
The full model containing all predictors was statistically significant, χ2 (52, *N* = 340881) = 48482.727, *p* < .001. Estimated *r*2 values indicated that the model explained between 13.3% (Cox and Snell *R*2) and 24.1% (Nagelkerke *R*2) of the variance in the DV, diabetes diagnosis. Individual predictor results are included in the *Variables in the Equation* table below.

##### Full Model
[![Omnibus_and_Model_Summary.png](https://s31.postimg.cc/senmp8nvv/Omnibus_and_Model_Summary.png)](https://postimg.cc/image/vli68v8br/)

##### Individual Predictors

Predictor | Predictor Statistics
----------|----------------------
Sex | *B* = .372, *S.E.* = .012, Wald χ2 = 978.726, *p* < .001, OR = 1.450, 95% C.I. = 1.417 - 1.484
Overall Marital Status | Wald χ2 = 56.464, *p* < .001
Overall Employment Status | Wald χ2 = 1040.203, *p* < .001
Overall Race | Wald χ2 = 1445.271, *p* < .001
Overall Age | Wald χ2 = 6378.782, *p* < .001
Overall Education Level | Wald χ2 = 127.782, *p* < .001
Overall Income | Wald χ2 = 355.081, *p* < .001
Overall BMI | Wald χ2 = 10204.194, *p* < .001
Overall Smoking Status | Wald χ2 = 51.851, *p* < .001
Overall E-Cigarette Status | Wald χ2 = 7.876, *p* = .049
Physical Activity | *B* = -.258, *S.E.* = .012, Wald χ2 = 445.156, *p* < .001, OR = .773, 95% C.I. = .755 - .792
Sleep | *B* = .001, *S.E.* = .003, Wald χ2 = 0.24, *p* = .877, OR = 1.001, 95% C.I. = .994 - 1.007
Overall Physical QoL | Wald χ2 = 1464.197, *p* < .001
Overall Mental QoL | Wald χ2 = 103.618, *p* < .001

### *Thank you in advance for your consideration of my application to The Data Incubator!*
