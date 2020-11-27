# expolaration-project
## Dataset
 Ford GoBike is the first bike-sharing system introduced in the US West Coast. 
 Its 540 stations and 7,000 bikes sprawl across five cities in San Francisco Bay Area.
 A docked bike can be checked out at any station and must be returned to a station when the trip is complete.
## Highlights
### The ratio of male to female users is 3:1.
### The median age of users is 35.
### More than 90% of the rides are under 30 minutes.
### The peak hours across all rides in 2018 are 9 AM and 6 PM, which align with normal working hours.
## Data wrangling process:
### fix the data types, i.e. start_time, end_time should be datetime type, user_type and member_gender should be categorical data type, etc
### add new columns for trip duration in minute
### add a new column cfor the riders' age from 'member_birth_year'
### filter out outlier ages from visual examination of the member age distribution
### fill the missing values in the age.
### cast 'member_birth_year' and 'member_age' to integer instead of float type
### cast 'start_dayofweek' to category dtype
### cast 'start_month' to category dtype for easy plotting
### filter out outlier trip records where the duration was very long
