# Ford GoBike Trip July 2018 Data Analysis
## by Lauriston Nunes


## Dataset

> This document explores a dataset containing trip duration and additional attributes for approximately 199,222 bike trips for the Ford GoBike bike share system for the month of July 2018. There are 183,694 bike trips in the dataset with 16 features (duration_sec, start_time, end_time, start_station_id, start_station_name, start_station_latitude, start_station_longitude, end_station_id, end_station_name, end_station_latitude, end_station_longitude, bike_id, user_type, member_birth_year, member_gender, and bike_share_for_all_trip). About half of the variables are numeric in nature, however we also have date_time objects (start_time, end_time), categorical objects (user_type, bike_share_for_all_trip, member_gender), and string objects (start_station_name, end_station_name). I removed records with a null start_station_id and records with a null member_birth_year so that I could change the data type and remove the records with missing information that will be needed for analysis.


## Summary of Findings

> Majority of the bike share users are millenial male subscribers. The first thing I looked at were the categorical data types (user_type, bike_share_for_all_trip, member_gender). I found that there were 158,672 subscribers and only 25,022 customers, so we can gather that most users are subscribers. After breaking down the member_gender, we see that there are 133,329 Male bike users 47,272 Female bike users, and 3,093 bike users that identify as Other. After investigating the member_birth_year variable we can see that majority of the user base is people born in the late 70s up to 2000, or Generation Xers and Milennials. Outliers are probably due to people using fake birth days when registering. The bivariate and multivariate exploration give us different views of how these variables are related. The most interesting insight I found was that the distance of the bike trip is inversely related to the duration of bike trip.


## Key Insights for Presentation

> Majority of the bike share users are millenial male subscribers. Another interesting insight is that duration and distance are inversely related. I calculated the distance by using the haversine formula, which determines the great-circle distance between two points on a sphere given their longitudes and latitudes.
