# Stat-437-Project
**Project Paper:** Elevational and temporal patterns of pollination success in distylous and homostylous buckwheats (Fagopyrum) in the Hengduan Mountains by Ling-Yun Wu, Shuang-Quan Huang, Ze-Yu Tong

**DOI:** https://doi.org/10.1016/j.pld.2023.10.001

**Link to New Dataset:** https://archive.ics.uci.edu/dataset/519/heart+failure+clinical+records

# Project Introduction
The paper “Elevational and Temporal Patterns of Pollination Success in Distylous and Homostylous Buckwheats (Fagopyrum) in the Hengduan Mountains” by Ling-Yun Wu, Shuang-Quan Huang, and Ze-Yu Tong investigated the reproductive strategies of wild buckwheat in the Hengduan Mountains in China. The authors compared two reproductive strategies including distylous species, which rely on pollinators to pollinate, and homostylous species, which can self-pollinate. At higher elevations and later flowering season there is often a decrease in pollinator activity due to colder temperatures and scarcity of insects. The authors wanted to know if homostylous species have a more reliable reproductive strategy in the challenging mountainous environments compared to the distylous species that rely on insects. In their study, they looked at 28 populations across nine different Fagopyrum species across an elevation gradient from 1299-3315 meters. They measured flower size and collected stigmas, to evaluate pollination success, over a two month period.

In this project we recreated the general statistical approach of the paper using a clinical dataset containing medical records of 299 heart failure patients, each with 13 clinical features collected during follow-up periods. Instead of comparing pollination success across species and environmental gradients, we applied similar comparative statistical methods to investigate differences in clinical outcomes across patient subgroups. Specifically, we analyzed relationships between continuous clinical variables (age, creatinine phosphokinase, ejection fraction, platelets, serum creatinine, serum sodium, and time) and categorical patient characteristics (death event, anaemia, diabetes, high blood pressure, sex, and smoking).

# Variables in our dataset
**Thirteen (13) clinical features:**

* age: age of the patient (years)
* anaemia: decrease of red blood cells or hemoglobin (boolean)
* creatinine phosphokinase  (CPK): level of the CPK enzyme in the blood (mcg/L)
* diabetes: if the patient has diabetes (boolean)
* ejection fraction: percentage of blood leaving the heart at each contraction  (percentage)
* high blood pressure: if the patient has hypertension (boolean)
* platelets: platelets in the blood (kiloplatelets/mL)
* sex: woman or man (binary)
* serum creatinine: level of serum creatinine in the blood (mg/dL)
* serum sodium: level of serum sodium in the blood (mEq/L)
* smoking: if the patient smokes or not (boolean)
* time: follow-up period (days)
* [target] death event: if the patient died during the follow-up period (boolean)

# Statistical Methods used in the paper
* Generalized Linear Mixed Models (GLMM)
* - GLMM with poisson distribution and log-link function
* - GLMM with normal distribution and linear function
* Independant t-tests
* Coefficient Variation (CV) - calculated by dividing the standard deviation by the mean
* Generalized Linear Models (GLM)
* - GLM with normal distribution and linear function
* - GLM with binomial distribution and logit-link function

# Statistical Methods used in our project
* Generalized Linear Mixed Models (GLMM)
* - GLMM with poisson distribution and log-link function
* - GLMM with normal distribution and linear function
* Shapiro-Wilk test
* Wilcoxon rank-sum test
* Levene's test
* Generalized Linear Models (GLM)
* - GLM with normal distribution and linear function
* - GLM with binomial distribution and logit-link function
* Survival Analysis
* - Kaplan-Meier
* - Cox Proportional Hazard Model
    
# R Packages Used
* dplyr
* car
* lme4
* tidyverse
* AER
* MASS
* ggplot2
* gridExtra
* knitr
