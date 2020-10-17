# Predicting-likelyhood-of-commercial-leads-to-complete-subscription-process
Create model assessing the quality of commercial leads by predicting whether application process will be completed

# Problem Statement

In this project, we will create a model able to qualify commercial leads. A commercial lead will be qualified of "quality" if the prospect completes and submit his request for quotation on-line.

Lending companies work by analyzing the financial history of their loan applicants and choosing whether or not the applicant si too risky to be given a loan. This is done by calculating various risk scores and predicting potential default. We will not focus on this task but another scoring dealing with commercial leads.

Applicants are often prospected through partners like intermediary marketplaces and proper marketing and advertising campaign.
Applicants start their application process (request of a loan for example) on the marketplace platform to prequalify before to be proposed to the loan company which has to accept the lead or not on a real-time basis.

The loan company has to assess whether the lead propose dis of good quality, ie whether the application process will be finalized (lead conversion) or aborted before submission. This allows the company to either only accept most promising leads (and acquire only these), or allows to leverage this information to identify the 'less quality' applicants and experiment different onboadring screens with them in order to improve the conversion rate.

# Business Case

We are not focusing on the credit rating part of the screening process but on the likelyhood of lead conversion to quotation / service request.

We assume that the users going through application screens provides information till the e-signing final step. This information comprises both financial details and personnal details.

The dataset available for the project is made of nearly 18,000 records corresponding to application process which were finailzed or not. This is stipulated by the binary response variable  'e-signed' attached to each record.

In addition to the 'e-sign' label, each record has 20 variables covering personnal details (age, address, home details, seniority at work...), financial details (monthly income, pay schedule, bank account details, loan amount requested...) and multiple risk ratings including external ones coming from the third-party marketplace. 

# Notebook steps
- Dataset Exploration and cleaning
- Feature engineering
- Training and best hyper parameters search
- Evaluation

# Results

using random forest, the predictive model performance remains poor overall with precision of 65% (65% of all predicted e-signature are actually e-signature) and recall of 70% (70% of e-signature are correctly predicted). Consequently, F1 score cumulates at 67% only. While the approach developped in the project remains valid, the available information does not allow to predict with high accuracy.
