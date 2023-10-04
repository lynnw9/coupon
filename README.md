# COUPON DATASET
****Overall Dataset****
This dataset, sourced from the UCI Machine Learning repository, revolves around a survey conducted on Amazon Mechanical Turk, focusing on driving scenarios and coupon acceptance. The scenarios are described based on various parameters such as the destination, the current time, prevailing weather conditions, and the presence of a passenger, among others. Participants were posed with the query of whether they'd accept a coupon under the given circumstances, were they the driver. Positive responses indicating an intention to use the coupon either immediately or later, before its expiration, are designated with the label 'Y = 1'. On the contrary, outright refusals to accept the coupon are marked as 'Y = 0'. The dataset further categorizes the coupons into five distinct types based on the nature of the establishments: inexpensive restaurants (costing under $20), coffee houses, carry out & take away establishments, bars, and pricier restaurants with expenses ranging from $20 to $50.

The analysis indicates that the dataset includes some missing data in columns "Bar", "RestaurantLessThan20", "CarrayAway", "Restaurant 20To50", "Coffeehouse", and "car." In particular, the column  car  is near empty. Thus, data in this column is difficult to use. For the missing data in the  bar  column, I simply fill them with  never . 

The dataset includes 12684 rows of data, among which 7210 chose to accept the coupon. The overall acceptance rate is 57%. The analysis shows the count of drivers who received various types of coupons, and the respective percentages of those who either accepted or declined these offers. 

The analysis shows the temperatures at the time coupons were provided to drivers. A significant majority of the coupons were dispensed when the temperature exceeded 80 degrees. Interestingly, the acceptance rate appears higher at both the warmer temperatures (above 80 degrees) and colder temperatures (below 40 degrees) compared to the moderate range of 40 - 60 degrees.

****Investigation of bar coupons****
2017 drivers received a bar coupon, and 827 of them accepted the coupon, resulting in an overall acceptance rate of 41%. When dissected based on the frequency of bar visits, those visiting up to 3 times a month have an acceptance rate of 37% (500 out of 1,263), while the rate jumps to 76% (153 out of 199) for those visiting more often. In terms of drivers' acceptance rates based on their bar visits, passengers, and occupations, it's 71% (393 out of 551) for drivers visiting bars more than once a month and having adult passengers not engaged in farming, fishing, or forestry, compared to 29% (434 out of 1,466) for other drivers. This 71% acceptance rate remains consistent for drivers visiting bars more than once a month with adult passengers who are not widowed. Younger drivers, specifically those under 30 who visit bars more than once a month, have a higher acceptance rate of 73% (245 out of 335). Lastly, drivers who frequent cheap restaurants over 4 times a month and earn below 50K have a 46% (124 out of 271) acceptance rate.

Based on the data analysis, the following hypotheses can be generated:
1. Frequency of Bar Visits
There seems to be a direct correlation between the frequency of bar visits and acceptance rates. Individuals who visit bars more often are more likely to accept certain offers or participate in certain activities than those who visit less frequently.

2. Occupation's Influence
The occupation of a driver's passengers appears to influence acceptance rates. It's possible that certain occupations, specifically outside of farming, fishing, and forestry, might have lifestyle preferences or habits that align more closely with frequent bar visits and the associated offers.

3. Marital Status and Bar Visits
The marital status, specifically being non-widowed, might play a role in the likelihood of accepting certain offers during frequent bar visits. This could suggest that social settings or the nature of the offers are more appealing to those not experiencing recent bereavement.

4. Age as a Factor
Younger drivers, particularly those under 30, seem to be more inclined to accept offers or partake in activities associated with bar visits than their older counterparts. This could indicate that the offers or activities cater more to the preferences of a younger demographic.

5. Economic Considerations
Drivers with a certain economic profile, specifically those earning below 50K and frequenting cheaper dining options, have distinctive acceptance rates. This might imply that economic constraints or preferences influence the decision-making process of these drivers.

6. General Behavior Pattern
There's a pattern indicating that individuals with more frequent outings, whether to bars or restaurants, might be more socially active or open to certain offers than those with fewer outings.

Additional investigation of bar coupons based on age
Based on the analysis, younger adults, those just over 21, are particularly inclined to accept these coupons.

Additional investigation of bar coupons based on weather
Based on the analysis, drivers tend to accept coupons more frequently on sunny days. 

Additional investigation of bar coupons based on time
Based on the analysis, the acceptance rate increases around 6pm, which is typically dinner time.

Additional investigation of bar coupons based on marital status
Based on analysis, single individuals have a higher likelihood of accepting bar coupons.
