# credit-risk-analysis
Credit risk modeling is the process of quantifying the likelihood that a borrower will default on a loan and estimating the financial losses that may result. Financial institutions use credit risk models to assess and manage exposure, improve lending decisions, and comply with regulatory requirements.
This project aims to predict the probability of loan default and estimate the expected credit loss of borrowers using a Random Forest Classifier. The dataset contains borrower information such as income, FICO score, employment history, outstanding debt, credit lines, and loan amount.

To improve predictive performance, several features were engineered, including debt-to-income ratio, loan per credit line, income per credit line, job stability indicator, and good credit indicator based on FICO scores. The data was then divided into training and testing sets using an 80:20 split while preserving the class distribution through stratified sampling.

A Random Forest model was trained to estimate the Probability of Default (PD) for each borrower. Using the predicted PD, the Expected Loss (EL) for every loan was calculated with the industry-standard formula:

Expected Loss = Probability of Default (PD) × Loss Given Default (LGD) × Exposure at Default (EAD)

where LGD was assumed to be 90% (10% recovery rate), and EAD was represented by the outstanding loan amount.

The model's performance was evaluated using Mean Absolute Error (MAE), and portfolio-level risk metrics such as average expected loss, total expected loss, maximum expected loss, and minimum expected loss were computed. Additionally, graphical visualizations, including histograms, scatter plots, and bar charts, were created using Matplotlib to analyze the distribution of expected losses and identify high-risk loans.

This project demonstrates the practical application of machine learning in credit risk assessment, enabling financial institutions to make data-driven lending decisions and improve portfolio risk management.

The following is the code file with both Logistic regression and Random Forest methods to find more efficient method.But both give same answers
[task - 3 credit expected loss.ipynb](https://github.com/user-attachments/files/29658956/task.-.3.credit.expected.loss.ipynb)

The file for the Raw data as folow-
[Task 3 and 4_Loan_Data (1).csv](https://github.com/user-attachments/files/29658984/Task.3.and.4_Loan_Data.1.csv)



following is the Outcome of Logistic regression
<img width="772" height="248" alt="image" src="https://github.com/user-attachments/assets/00878bbf-1f06-461c-a151-f55bd65387ab" />



following is the Outcome of Random Forest



<img width="644" height="221" alt="image" src="https://github.com/user-attachments/assets/29971578-98d5-41cf-860c-a17326155823" />
