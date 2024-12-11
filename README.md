
# UC Berkeley - Professional Certificate in Machine Learning and Artificial Intelligence
Practical Application 17.1  


## 🔗 Links
[![portfolio](https://img.shields.io/badge/my_portfolio-000?style=for-the-badge&logo=ko-fi&logoColor=white)](https://github.com/BrendanThomasByrne/UCBerkeley.git)



## Business Problem
From a business perspective, we are tasked with identifying key drivers for used car prices. In the CRISP-DM overview, we are asked to convert this business framing to a data problem definition. Using a few sentences, reframe the task as a data task with the appropriate technical vocabulary.

Identify the features of used cars that most impact price so that dealers can refine their inventory to maximize profits.

Identify AI models that best predict the price that consumers are willing to pay for a vehicle so that we can identify the characteristics that customers most look for and are willing to pay for.

## Findings:
The decision of what cars to sell needs to be a combination of profit per car and how many can you sell.  Unfortunately, we don't have access to purchase prices for this analysis.  The data is available to analyze both when a dealer can consider the offered purchase price of a car for the lot.

Dealers will be expected to know there local market which will dictate things such as how many trucks versus cars you sell.  This analysis does not consider location or regionality.  it is not considered because we are looking at total impact and regionality is not a factor.  For an individual dealer, location will be of prominent importance and will not be addressed in this analysis.

From a volume perspective gas and automatic transmission are vital.  Though diesel and trucks are desireable, just not at the same rate.  Depends on where you live.  I'm sure that regional influences here are critical but not considered in this analysis.

The issue with looking at many of the data points regarding avergae prices is that they don't help a dealer know what to carry.  Yes, a Porche sells for more than a Ford.  But are you making more profit if you sell a $100,000 car you bought for $90,000 than selling 2 Fords for $35,000 that you bought for $20,000.  So you need to look at number of sales and profit per sale.

Towards this end I looked at the top two (by a wide margin) of features that influence price...year and odometer.  By graphing the expected impact when isolated from other features we can get a sense of what the true value of the car is.  Most other features, such as model, truck or car, provide a base expectation from which to make a decision.  You don't decide to sell a Porche or Ford based on car sell price as mentioned above.

Dealers should look at the base price of a vehicle if it were new and then use the graphs of year and odometer impact on price to see what the car should sell for.  They can then look at their purchase price option and decide whether to carry that car or not based on a calculation of profit per that car type (Model, Maker, Gas, Transmission, etc) and how many they can sell.

## Next Steps and Recommendations:

1) Know your local market.  Volumes will adjust massively based on location.  Additional analysis should be computed to determine turnover rate for various makes and models.   Don't try to sell a Porche in South Dakota and don't try to sell a Jeep in Beverly Hills.  I can generate additional recommendations regionally.  This is analysis for all sales.  Regionality is important but not analyzed here.
2) Once you know what types of vehicles you want to sell, you can look at the factors that influence your profit per sale.  The primary two are year and odometer.  For future analysis we can start to look at features such as cylinders or fuel type for the same model and year to determine price impact.
3) For those features (Year and Odometer are graphed above) calculate the percentage decrease in value and apply to the car you can buy.  This should give you a profit estimate.  Multiply this by your volumes expectation (additional analysis) and you will know your gross profit expectations.

