# (Dataset Exploration Title)
## by (your name here)


## Dataset

> The dataset contains information about the individual trips using Ford GoBike (known as Bay Wheels now), a regional public bike sharing system in the San Francisco Bay Area. All data are from February 2019. The dataset has 183412 observation (trips) and 16 attributes. These variables includes the start and end time of the trip, its duration, the start and end station as well as the characterstics of the users such as gender, age and user type (subscriber or customer). 

The dataset needs cleaning as it has some quality and tidiness issues. The start time of the trip was split into three variables: the day of the month, day of the week and the hour of the day. The age was calculated from the birth year column by substracting it from the year of the trips (2019). The gender, user type, day of the week, and hour of the day was transformed to categorical variables. The duration of the trips was calculated in minutes instead of seconds. After the univariate exploration, unusual points values were spotted in the age and duration variables. Treated as outliers, the very large values of the age (above 75) were removed, while the duration outliers were handled by clipping, where the high values, outside the range of .99 percentile were reduced to the value of the upper edge of this interval.  


## Summary of Findings

The primary focus in this analysis is the duration and time of the trips, the characteristics of the users and their relation. 

The bike sharing system is used more in the weekdays than in the weekends. There is a pattern of usage during the weekday, as the trips peaks at around 8 am and at 5 pm. The age of the users is between 25 and 40. The male users, which they are the majority, are older than the female users, and the subscribers (the majority) are slightly older on average than the customers. The trips last between 5 and 15 minutes on average with some trips took way more time. The most of the subsribers don't use the bike all share service.

The duration of the trips depends on the users characteristics such as the age and user type and on the day of week and hour of the day the trip was taken at.

- The duration of the younger users trips are longer than the duration of the older users trips. Since the female users are younger than the male users, the trips taken by female are longer.

- The duration of the trips taken in the weekend are higher than these taken during the week. This can be justified by that the subscribers tend to bike the most in the morning at 9 am and afternoon at 5 pm of the weekdays, hours of going and returning from work , and this leads to shorter trips than the customers trips who use the system more in the middle in the day and much more during the weekend in opposition to the subscribers for other purpose than work.

## Key Insights for Presentation

> Select one or two main threads from your exploration to polish up for your presentation. Note any changes in design from your exploration step here.

1) Duration of the trips depends on the age of the users.
2) The effects of the pattern of usage the customer and subscribers by day of week and hour of day on the duration of the trips.