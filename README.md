# PyBer_Analysis
## Overview 
PyBer is a company that created a ride sharing app to connect riders and drivers. The executives at PyBer requested an exploratory analysis of two datasets: city data and ride data. I merged these two datasets using Python scripts in Jupyter notebook with the Pandas libraries. Then I used Matplot lib to visualize the relationship between the type of city, number of riders and drivers, and total fares.  

## Results

The PyBer data categorized cities into three types: Urban, Suburban, Rural. Using the groupby function, I created this dataframe to compare the relationship between the total rides, number of drivers, and fares.

![Pyber_Summary_DF](Analysis/Summary_DF.png)

Comparing the number of total rides by city type: Urban cities took the lead (1,625 total rides), followed by Suburban (625 total rides), and lastly Rural cities (125 total rides). The relationship of total drivers by city type also followed a simlilar relationship with Urban cities leading (2,405 drivers), followed by Suburban (490 drivers), and lastly Rural cities (78 drivers). The sum of fares in each city type followed suit with Urban cities ($39k), then Suburban ($19k), and lastly Rural cities ($4k). Total fares was **directly proportional** to the city size, total rides, and total drivers.

The average fares had in **inverse relationship** with the size of the city. The largest cities had the lowest fares with Urban average fare per ride at $25 per ride, Suburban $31 per ride and Rural $35 per ride. 
The average fare per driver was also negatively correlated to the city type and number of drivers. With less drivers came higher average fares per driver: Urban ($17 / driver), Suburban ($40 / driver), Rural ($55 / driver).

These results made me ask two questions:
- Why do larger cities have more rides, drivers and fares?
- Why do larger cities have lower fares per ride and per driver?

Knowing Urban cities are more densely populated, it makes sense that the total rides, drivers, and fares directly correlates to the size of the city type. The higher demand in larger cities for ride sharing would mean more overall rides needed, there more drivers, and high total fares. With less drivers in rural areas, there could be higher fares.

However, it's worth considering other factors at play. For example, the ride distance was not captured in this analysis, so if fares are calculated based on distance, we could assume the shorter distances in Urban areas played a part in the lower fares. There was also no rider demographic data to see relationships based on city type and average rider age, income, etc.

![PyBer_Fare_Summary](Analysis/PyBer_fare_summary.png)

There are clear weeks where across all city types, the fares tend to be highest. PyBer should be aware of these cycles as they plan their business with facotrs like advertising, promotional discounts, or driver incentives. Seasonality could play a part in the weeks with higher fares. Other external factors like fuel cost could also play into the fare. More data and analysis could confirm this hypothesis. 

## Summary
The Pyber city and ride data analysis showed strong relationships between city type, total rides, drivers, and fares. As a business, PyBer should consider which city types have the most demand, market size, and most profit, so advertising, marketing, and sales efforts can focus on the highest business priorities and drive outcomes. 

One key aspect of ride sharing data is ride distance, which was not captured in this data. Incorporating some distance measures could help inform what length of rides are the sweet spot for business, to focus efforts on these types of ride sharing.

Looking deeper into the driver data could also share some key metrics to see if a large percentage of the rides and fares are managed by a small group of drivers (outliers) or more evenly paced. Pricing competitive fares could encourage more drivers in less populous areas, like rural areas, to have more options and lower the cost for consumers, and hopefully increase demand.

Is ride affordability a goal for PyBer? If so, increasing the number of drivers in rural areas would likely lower the average fare per rides and encourage more total rides.
