
# UC Berkeley - Professional Certificate in Machine Learning and Artificial Intelligence

Practical Application Assignment 5.1  


## 🔗 Links
[![portfolio](https://img.shields.io/badge/my_portfolio-000?style=for-the-badge&logo=ko-fi&logoColor=white)](https://github.com/BrendanThomasByrne/UCBerkeley.git)



## Business Problem
In this third practical application assignment, my goal is to compare the performance of the classifiers (k-nearest neighbors, logistic regression, decision trees, and support vector machines) I encountered in this section of the program. I will use a dataset related to the marketing of bank products over the telephone.

The data is related with direct marketing campaigns of a Portuguese banking institution. The marketing campaigns were based on phone calls. Often, more than one contact to the same client was required, in order to access if the product (bank term deposit) would be ('yes') or not ('no') subscribed.

The classification goal is to predict if the client will subscribe (yes/no) a term deposit (variable y).

Citation for data: https://archive.ics.uci.edu/dataset/222/bank+marketing Moro, S., Rita, P., & Cortez, P. (2014). Bank Marketing [Dataset]. UCI Machine Learning Repository. https://doi.org/10.24432/C5K306.

## Findings:
Previous positive results are the best indicator of potential success

Timing was of obvious importance and best and worst performing time periods should be an important consideration.

Other financial indicators such as an existing home loan, existance of a personal loan, and average balance are good indicators to filter the targets.

Demographics such as age and job can be used to improve targettuing results but are of lesser importance than the other factors.

## Next Steps and Recommendations:

Business Recommendations: Focus on past success and identify the optimal period to wait before contacting to make the offer.

Operational considerations: Schedule campaigns to maximize efficiency by focussing on high probability time periods and avoiding bad months. Campaigns can be scheduled to utilize the most effective times of year and eliminate the bad periods.

The ROC curve can be used to determine how many people to assign to these campaigns and who should be on the call list. AI can clearly identify and rate the candidates with good efficiency. The fact that the ROC curve shows that an 80/20 split on precision can be had shows that even with low acceptance rates, relatively high precision can be acquired with some data targetting. It wiull become a factor of cost benefit analysis to determine how many calls to make and where the break point should be on assigning staff to conduct these campaigns.

