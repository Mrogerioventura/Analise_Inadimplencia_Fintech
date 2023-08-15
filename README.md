# Default Risk Analysis.

Objective: This work aims to increase the number of contracts of a Fintech, with a decrease in the Risk of Default.

## 1. Introduction

It is a data analysis work, using Microsoft Excel as a tool, seeking, through the application of statistical methods, to respond to a need of a Fintech company.

## 2 – Contextualization

A Credit Fintech started its personal loan operation and monitored the payment performance of 1,000 customers after 1 year. Based on this sample, it requested a Data Analysis to verify the risk factors of customers, in order to be able to approve more contracts with the lowest possible default.

## 3 – Metadata:

Default - 1 if the customer defaulted at some point after the loan or 0 otherwise;

Age - Customer age:

Gender - M: Man and M: Woman;

Schooling - High School, Undergraduate and Postgraduate;

Type_Housing - If you live on a favor, pay rent or have your own home;

Balance_Investment - Borrower has an investment account in another bank and what is its balance range;

Balance_Conta_Corrente - If the borrower has a current account at another bank and what is its balance range;

Valor_Loan - personal loan amount requested;

Duracao_Emprestimo - Duration in months of the requested personal loan.


## 4 – Methodology
The adopted methodology consisted of an initial approach based on the frequentist theory, followed by an Information Value (IV) analysis for a deeper bivariate analysis. Below is a description of this methodology:

### 4.1 - Univariate analysis using frequentist theory.
The first step was to conduct a univariate analysis, examining each variable independently. The frequentist theory approach was used to analyze the proportions and frequencies of the categories in each variable. The percentages of occurrence of each category and the proportions of response (delinquency) in relation to each category were calculated. This analysis provided an overview of the individual characteristics of each variable and its relationship with the response variable (delinquency).

### 4.2 - Bivariate analysis using Information Value (IV).
After the univariate analysis, a bivariate analysis was performed using the concept of Information Value (IV).
IV is a statistical measure that evaluates the importance of each independent variable in relation to the response variable (delinquency).
Calculating the IV involves comparing the proportions of response (delinquency) for each category of the independent variable, in relation to the general proportion of response. Based on the IV calculation, it was possible to determine the degree of influence of each independent variable on default, classifying them in terms of their importance for predicting default risk.
This methodology allowed for a systematic approach to data analysis, starting with a univariate analysis to understand the individual characteristics of each variable and then performing a bivariate analysis using IV to identify the variables that most contributed to the prediction of default.
This approach is effective in highlighting the most relevant variables and assisting in making strategic decisions to reduce defaults and increase the number of contracts more accurately.

## 5 - Analysis of the results.

In this section, the main results obtained from the data analysis will be presented.

### 5.1 – Graphs developed during the univariate exploratory analysis.
![image](https://github.com/Mrogerioventura/Analise_Inadimplencia_Fintech/assets/67667695/df772783-e800-4465-b41e-b47409e78e41)
![image](https://github.com/Mrogerioventura/Analise_Inadimplencia_Fintech/assets/67667695/f7341d46-389e-48ef-95f4-a7c3bc290b68)
![image](https://github.com/Mrogerioventura/Analise_Inadimplencia_Fintech/assets/67667695/616b1af2-443b-4ed1-a8ce-f33c8bfd5e83)


The data above can be found on the Univariate tab of the Spreadsheet Base_Delinquency V5.xlsx.

### 5.2 - Table with variables ordered by Information Value (IV), highlighting those with greater predictive power in relation to default.
It is found in the Bivariate tab of the Spreadsheet Base_Delinquency V5.xlsx.

### 5.3 - Deepening the analysis using Feature Engineering.

In the Base file, a column was added combining the values of the features Saldo_Invest + Saldo_CC, making it possible to obtain more details of the influence of these two variables, now together, on the risk that they can generate for the increase in default.

By observing the TABLE shown below in the **Análise_Bi2** tab, of the Base_Delinquency Worksheet V5.xlsx, we can see the different categories of the variable "Baldo_Invest + Saldo_CC" and the corresponding response proportions for each category. In addition, the response percentages (delinquency) for each category are provided, as well as the expected proportions of response for each one.

![image](https://github.com/Mrogerioventura/Analise_Inadimplencia_Fintech/assets/67667695/69277208-f467-487c-a171-9d6800106b5e)

Applying the IV calculation, we obtain a value of 0.8048. This value indicates a significant influence of the variable "Saldo_Invest + Saldo_CC" on customer default.

It is important to note that the IV not only quantifies the importance of the variable, but also indicates the direction of the relationship. In the case under analysis, it is observed that the categories with higher IV values (such as "Pouco-Pouco" and "Pouco-Sem conta") are associated with a higher proportion of defaults, while categories with lower IV values (such as " High-High" and "Moderate-High") are associated with a lower proportion of default.

Based on these results, it is concluded that the variable "Saldo_Invest + Saldo_CC" plays a significant role in predicting customer default. Therefore, when developing strategies to approve more contracts with the lowest possible default, it is important to carefully consider and evaluate this variable, taking into account the characteristics and risks associated with each category.

## 6 - Recommendations and suggested Action Plan.

Based on the results of the analysis, specific recommendations were presented for the company in order to increase the number of contracts without increasing defaults, according to the Action Plan below, also located on the Action Plan tab of the Spreadsheet Base_Delinquency V5.xlsx.
![image](https://github.com/Mrogerioventura/Analise_Inadimplencia_Fintech/assets/67667695/c5031ce9-0edb-4671-9073-0ce397d8d512)

## 7 - Limitations and recommendations for future studies.
We know how important it is to recognize that the job doesn't end with data analysis, and identifying opportunities for future improvement is paramount.

Some points that should be taken into account:

• Sample size: At the moment it was what we had for the development of the work, but a future study can be carried out to verify how much the sample of 1,000 clients is representative enough to extrapolate the results to the entire population.

• Other variables: As well as the sample quantity, additional variables may be identified that may be relevant for a new analysis and that were not included in the data provided. We suggest a meeting with each business team, which together can consider these new variables;

• Continuous improvement: Data analysis is a continuous process in which the results obtained must be monitored and reviewed regularly to ensure the effectiveness of the implemented strategies.

These additional topics will provide a more complete and in-depth context for the report, allowing the company to better understand the data analysis results and make informed decisions to improve its policies and processes related to lending.




