
# UC Berkeley - Professional Certificate in Machine Learning and Artificial Intelligence

Capstone Project


## 🔗 Links
[![portfolio](https://img.shields.io/badge/my_portfolio-000?style=for-the-badge&logo=ko-fi&logoColor=white)](https://github.com/BrendanThomasByrne/UCBerkeley.git)

## Problem
How does the combination of current water level and rainfall affect the change in water level on the Russian River by my house?  My theory is that as water level rises, each inch of rain raises the water level of the river less due to widening shore lines.  A good model can help me predict floods on my property which are fairly common.

## Results and Important Findings

Correlation between rainfall and water level rising:
Correlations by lag (days):
Lag 0 days: 0.435

Lag 1 days: 0.625

Lag 2 days: 0.618

Lag 3 days: 0.517

Lag 4 days: 0.431

Lag 5 days: 0.374

Lag 6 days: 0.329

Lag 7 days: 0.293

Lag 8 days: 0.268

Lag 9 days: 0.250

This shows that water level height was most impacted by rainfall 1 day earlier.  As expected, earlier rain still affects the water level, but not to the extent that the prior 24 hours does.  This becomes quite apparent with the simple graph of water level and precipitation on the same chart.  From the visual, the human eye can easily see that water levels peak 24 hours after the rain peaks.  While rainfall 10 to 20 days later (notebook has all 20) still has an impact, the river also drains rapidly into the ocean, so rainfall must exceed the drain off for an appreciable gain in height. This helps explain why even with correlated impact 10 days later, the river height peaks in the first 24 hours.

When looking at water level changes in the absence of rain, I produced the following chart:

Statistics by Water Level Range (all values in feet):

            Level_Drop                            WaterLevel

                 count   mean    std   min    max       mean
Level_Range                                                 
4.0-7.5ft          911  0.102  0.292 -4.29   2.56      6.481
7.5-8.2ft          921  0.057  0.228 -2.63   1.57      7.995
8.2-8.3ft          940  0.020  0.156 -1.80   1.86      8.269
8.3-8.5ft          886  0.020  0.121 -0.26   1.65      8.434
8.5-45.2ft         892  1.081  1.739 -5.81  18.72     12.168

As can be seen, the mean drop in water level increases as water level increases.  While the chart shows a slight decrease from 4 to 8.5 feet this makes sense.  If the water level is above the minimum, it means we have had some recent rain.  The residual rain will limit the drainage numbers.  But at larger levels (above 8.5 ft) we see a substantial jump in the drain off.  This confirms the working theory and feels strongly supported.

A simple chart validates the simplest of our theories, that more rain indicates higher water level changes.  (See chart below)

Water Level Change by Precipitation (ft):

                count  mean    std
Rain_Category
No Rain         4550 -0.252  0.893
Light            284 -0.756  1.759
Moderate         424 -0.388  2.437
Heavy            243  0.504  2.651
Very Heavy       410  2.802  4.086

I then attempted to identify the optimum number of prior days' precipitation to use in building a predictive model.  Despite some correlation for the previous days, using more than just the prior day led to worse results. 

I then made one final graph based on a LSTM model. While it does show some of the characteristics that we see in the linear regression models, the variations are very subtle and individual data points look questionable if not outright doubtful. It feels like it sees some of the pattern but doesn't quite make the right decisions and leans too strongly towards a norm. My conclusion is that the time series models were not as accurate as the linear regression models.  

Some final thoughts:
Water level rises quicker at lower water levels given the same amount of rainfall.  We can also relatively accurately estimate what the water level will be 24 hours ahead of existing levels based on the rainfall we get or predict to get.  The models are also very good at predicting water levels if there is no precipitation.  This still involves change as the river runs off into the ocean and levels will drop down to 5 feet with no rain.  It drops faster at higher levels as expected.

The fact that the predicted models seems to confirm the theorized behavior provides confidence in the models.

## Next Steps

I will continue to experiment with additional cross validation models and also explore the use of different hyperparameters and the creation of additional features from existing data.  The actual water levels are clearly not linear in relationship so finding ways to create models that best make use of the limited number of data features will be explored.  My work already includes some experimentation with this in adding the square of the precipitation and even changing scaling to emphasize the polynomial features.  More experimentation is needed here.  Once I have developed models I like I will add additional rain meter data from other nearby locations.
