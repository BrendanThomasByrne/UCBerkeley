
# UC Berkeley - Professional Certificate in Machine Learning and Artificial Intelligence

Capstone Project


## 🔗 Links
[![portfolio](https://img.shields.io/badge/my_portfolio-000?style=for-the-badge&logo=ko-fi&logoColor=white)](https://github.com/BrendanThomasByrne/UCBerkeley.git)

## Problem
How does the combination of current water level and rainfall affect the change in water level on the Russian River by my house?  My theory is that as water level rises, each inch of rain raises the water level of the river less due to widening shore lines.  A good model can help me predict floods on my property which are fairly common.

## Results

The resulting predictive graphs confirm my theories.  

Water levels are most impacted by rain 24 hours later.  This is apparent from looking at the data and seeing the max value for water level comes 24 hours after the max precipitation.  The resulting ARMA model was therefore built to evaluate predicted water levels 24 hours later than what is known.
 
Water level rises quicker at lower water levels given the same amount of rainfall.  We can also relatively accurately estimate what the water level will be 24 hours ahead of existing levels based on the rainfall we get or predict to get.  The models are also very good at predicting water levels if there is no precipitation.  This still involves change as the river runs off into the ocean and levels will drop down to 5 feet with no rain.  It drops faster at higher levels as expected.

The fact that the predicted model seems to confirm the theorized behavior provides confidence in the model.

## Important Findings


## Next Steps
