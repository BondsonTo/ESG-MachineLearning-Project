# ESG Score to Explain Company Financial Performance
This is my Master degree data analysis dissertation project.  Models built with various machine learning alglorithms trying to validate if companies ESG efforts would contribute to financial growth.

## Background

Environmental, Social and Governance (ESG) became increasingly important for businesses and investors due to the growing awareness. Despite of inter-governmental efforts to promote ESG, Investors are also paying more attention to ESG performance as their investment criteria. Some viewed compliance and reporting requirement associated with ESG effort would adversely affect the company financials. This project aimed at investigating if ESG efforts and transformation really paid off at company level.

## Abstract

This project investigates the relationship between **Environmental, Social, and Governance (ESG) scores** and C**orporate Financial Performance (CFP)** using machine learning models. With a dataset of 3,422 companies across 26 countries, the research deploys four machine learning techniques, including **Linear Regression, Random Forest, Support Vector Regression, and Artificial Neural Networks**, to predict Return on **Equity (ROE)** based on ESG scores. The findings indicate a notable correlation between high ESG scores and improved financial performance. ESG score with factor significance to explain company ROE comparable to company net sales. Such correlation is highly industry-specific with complex relationship remain unresolved. The findings support companies putting higher emphasis in ESG efforts and transformation.

![Power BI Dashboard](https://github.com/user-attachments/assets/6ee913f9-926c-4a6a-9911-ef0d9a9ca002)

## Findings
The dissertation employs both parametric (Linear Regression) and non-parametric (Random Forest, Support Vector Regression, Artificial Neural Networks) methods. The models are evaluated based on performance metrics such as adjusted R-squared, mean squared error, and root mean square error. Model findings are summarized below:

### Company ESG performance matters in financial outcomes
(1)	Model Selection and performance metric: The analysis reveals that the Random Forest model outperforms other methods, achieving an adjusted R-square of 0.4950. This represents **the best model explained 49.5% of variability of the ROE** with given ESG score and other input characteristics. Linear regression comes 2nd best with adjusted R-square 0.3227.

(2)	Correlation matrix: **ESG scores changes in the same direction with ROE**, but the relationship is not strong. The **weak positive relationship** was supported with correlation coefficient 0.1075 – 0.2008 between ROE, ESG combined scores and individual pillar scores (Correlation coefficient 0 means no linear relation, where one means perfect strong linear relation)

(3)	Feature significance: The features in the best model were measured with their importance with feature importance score ranged from 0 to 1. Closer to 1 represent the feature has greater influence on the model predictions. Profit margin % is the most important feature with score of 0.2814. While ESG combined score measured at 0.0210 compared to same of company net sales 0.0248. **ESG score has comparable significance with annual net sales in ROE prediction**.

(4)	Feature selection: ANOVA F-statistics is 96.26 suggested the **linear model is statistically significant**. With feature selection on all 39 features, **ESG combined score and individual pillar score remained significant predictors** in the final model within selected 23 features.

### ESG impact varied among industries: 
(1)	Feature selection in regression: The dataset contains companies from 84 industries while 17 industries exhibit linear ESG-CFP relationships, with encoded industry features remained in final regression model. **Some industries came with more sophisticated non-linear ESG-CFP relationships** which remained unresolved.

(2)	Feature coefficient: The standardized coefficient of industry exhibited a wide range from -5.0885 to 1.6952. Biotechnology companies had coefficient -5.0885 and capital market companies had 1.6952. If one biotech and one capital market company with same ESG score, the **ROE is more sensitive to company with industry coefficient with higher magnitude**.





## Limitations and Future Implications
**ESG as higher priority for companies**: ROE exhibited moderated positive correlation with ESG scores across the companies. Higher performance in ESG initiatives is associated with higher financial performances.

**Investor shall put focus on company ESG effort**: Company ESG performance shall not be ignored when making investment decisions. ROE is more sensitive in some industries to ESG performance.

**Demand for more comprehensive ESG data**: Future research should aim to expand the dataset to include Asian and African countries to attain a holistic view in the ESG-CFP relationship. Companies’ dataset in the model training was biased to US and European companies due to availability of data in Refinitiv database, which accounted for 79.7% (2,728 out of 3,422) of total observations.  

**Industry specific factors to reveal complex ESG-CFP relationship**: The dissertation serves as a foundational study for understanding the nuanced dynamics between ESG performance and financial outcomes. ESG-CFP relationship was well quantified in 17 industries with the extent ROE would change in respect of ESG scores. Remaining 57 industries were not able to quantify, which call for further industry specific modelling efforts in future.



> [!NOTE]
> Useful information that users should know, even when skimming content.
