# MSBA Capstone - MasterControl Case Competition

Repository containing my data analytics project for MasterControl, a software company that provides quality and manufacturing products to life sciences companies. This was run as a case competition and includes the whole process of exploratory data analysis and modeling. 

## Contents
- ## Business Problem and Project Objective
  - MasterControl's Manufacturing Solutions product (Mx) is significantly underperforming its Quality Solutions product (Qx). The company believes it may not be targeting the right companies or the right people within those companies, leading to missed revenue opportunities and wasted marketing expenditures.
    
  - Conversion predictions will be generated using a classification model. The model will use historical sales leads and data collected from MasterControl. Patterns will be analyzed to produce models that identify similarities between higher-converting acccounts. This should allow us to gain insight into the characteristics of industries that are more likely to convert to Mx, as well as overlapping qualities between high-conversion for Mx and Qx products that can lead to cross-selling points.

- ## Solution to the Business Problem
  - Our group's proposed solution is for MasterControl to target small-to-medium sized CMO/CDMO companies in pharma or the medical device industry. The best contacts to reach out to will be VP or head-level contacts. Inbound and SEO are also where the best leads come from. This targeted approach will close the gap between Mx and Qx conversion rates.
 
- ## My Contribution to the Project
  - I conducted exploratory data analysis on 16,060 MasterControl CRM leads, uncovering key conversion rate differences between Mx (13%) and Qx (20%) across account types, site functions, job titles, and campaign channels. I built and validated logistic regression models separately for each product using a stratified 70/30 train-test split, achieving AUC scores of 0.829 for Mx and 0.818 for Qx with consistent results across both validation approaches.

- ## Business Value of the Solution
  - When we specifically focus on targeting CMO and CDMO accounts, Mx conversion rates increase from 13% to 17%. That requires no extra spending and no new hires, just calling the right people. Additionally, emails and events are taking up a lot of the marketing budget but they are some of the worst performing channels for Mx. Moving that money toward inbound and SEO leads would be more beneficial since we'd be replacing low quality leads with high quality ones.
 
- ## Difficulties Encountered Along the Way
  - The biggest challenge stemmed from data limitations rather than the modeling itself. Several variables had incomplete observations, which meant we had to either remove certain features or consolidate categories to avoid losing too many records. This limited how much detail we could preserve in the predictors and may have reduced the models' ability to capture nuanced patterns. We also had to deal with a relatively small dataset (~4,000 Mx observations), so more complex models created instability and convergence issues. That is why our group decided to prioritize logistic regression over other approaches to keep it simple and avoid overfitting.
 
- ## What I Learned in the Project
  - This project highlighted the importance of cleaning the data to build reliable models. Most of our efforts went into handling missing data, removing redudant variables, and properly formatting categorical features. We found that sparse categories led to convergence problems so we had to go back several times to clean/manipulate the data so we could produce stable results. 
