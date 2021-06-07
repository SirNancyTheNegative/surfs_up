# Surfs Up! Temperature Analysis
## Overview
The purpose of this analysis is to determine temperature trends in Oahu during the hottest and coldest days of the year in order to determine whether or not having a surf-and-ice-cream shop open year-round is a feasible decision. The reigning logic is, if the weather is noticeably different between June and December, the months containing the summer and winter solstices, respectively, then it might not be worthwhile to keep the surf shop open year-round.

## Results

The statistical data from the June temperatures came back as follows:

![alt text](https://raw.githubusercontent.com/SirNancyTheNegative/surfs_up/main/Images/JuneTemps.png)

While the statistical data from December temperatures looks like this:

![alt text](https://raw.githubusercontent.com/SirNancyTheNegative/surfs_up/main/Images/DecemberTemps.png)

From this we can pull a few important metrics:
* The average temperature in December is about 3.9 degrees colder than the average temperature in December. While this doesn't provide any concrete merit on its own, it's important to notice this in order to get a feel for how this number interacts when taken into account with the next two metrics.
* While the highest temperature recorded in June is only two degrees warmer than the highest temperature recorded in December, the coldest temperature recorded in June is eight degrees warmer than the lowest temperature recorded in December. While this means that December is decidedly usually colder than June, we still don't know if it's *consistently* colder than June. 
* At the 1st quartile, median, and 3rd quartile marks, the temperatures recorded in December are consistently 3-4 degrees colder than the temperatures recorded in June. Here we can safely determine that it's pretty consistently colder in December than it is in June.

## Summary

From the data we gathered, it is safe to assume that, although the temperature in December is consistently colder than the temperature in June, it is only slightly so most of the time. A difference of 3-4 degrees Fahrenheit is not enough to discourage having a surf-and-ice-cream shop that's open year-round. However, it also isn't enough to encourage it, either. There's still the matter of other sources of data that are needed, namely weather patterns with respect to temperature. It, therefore, is worthwhile to query for moments in June and December where temperature is low and precipitation is high. That is to say, we can use the data for December and make a query that look for precipitation levels when the temperature is below the median. Even if it's cold and sunny, some people will still go out of their way to enjoy ice cream and some people will still make an effort to surf, but if there's rain involved as well, neither surfers nor ice cream enthusiasts will find much enjoyment out of that. We could additionally do this for July as to create a comparable series of data for the number of days that end up as such in both.

Another query we could run is to look for the number of days that have high temperatures (say, for example, above the median) and low amounts of precipitation (below the 1st quartile) in July and December, and, with the data sets mentioned above, compare the number of likely peak business days in both July and December to see just how much business could feasibly be gained by staying open year-round.
